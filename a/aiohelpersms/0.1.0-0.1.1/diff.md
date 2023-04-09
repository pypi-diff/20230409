# Comparing `tmp/aiohelpersms-0.1.0.tar.gz` & `tmp/aiohelpersms-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohelpersms-0.1.0.tar", last modified: Sun Apr  9 11:09:50 2023, max compression
+gzip compressed data, was "aiohelpersms-0.1.1.tar", last modified: Sun Apr  9 15:42:29 2023, max compression
```

## Comparing `aiohelpersms-0.1.0.tar` & `aiohelpersms-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 11:09:50.023664 aiohelpersms-0.1.0/
--rw-rw-rw-   0        0        0      232 2023-04-09 11:09:50.024651 aiohelpersms-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-09 11:09:49.902399 aiohelpersms-0.1.0/aiohelpersms/
--rw-rw-rw-   0        0        0       51 2023-04-09 08:20:39.000000 aiohelpersms-0.1.0/aiohelpersms/__init__.py
--rw-rw-rw-   0        0        0     7516 2023-04-09 10:36:18.000000 aiohelpersms-0.1.0/aiohelpersms/aiohelpersms.py
-drwxrwxrwx   0        0        0        0 2023-04-09 11:09:50.019641 aiohelpersms-0.1.0/aiohelpersms.egg-info/
--rw-rw-rw-   0        0        0      232 2023-04-09 11:09:45.000000 aiohelpersms-0.1.0/aiohelpersms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-04-09 11:09:48.000000 aiohelpersms-0.1.0/aiohelpersms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 11:09:46.000000 aiohelpersms-0.1.0/aiohelpersms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-09 11:09:47.000000 aiohelpersms-0.1.0/aiohelpersms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 11:09:50.027665 aiohelpersms-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      302 2023-04-09 11:07:44.000000 aiohelpersms-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 15:42:29.714079 aiohelpersms-0.1.1/
+-rw-rw-rw-   0        0        0      232 2023-04-09 15:42:29.714079 aiohelpersms-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-09 15:42:29.667199 aiohelpersms-0.1.1/aiohelpersms/
+-rw-rw-rw-   0        0        0       51 2023-04-09 15:02:14.000000 aiohelpersms-0.1.1/aiohelpersms/__init__.py
+-rw-rw-rw-   0        0        0     9296 2023-04-09 15:33:18.000000 aiohelpersms-0.1.1/aiohelpersms/aiohelpersms.py
+drwxrwxrwx   0        0        0        0 2023-04-09 15:42:29.698552 aiohelpersms-0.1.1/aiohelpersms.egg-info/
+-rw-rw-rw-   0        0        0      232 2023-04-09 15:42:26.000000 aiohelpersms-0.1.1/aiohelpersms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-04-09 15:42:28.000000 aiohelpersms-0.1.1/aiohelpersms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 15:42:26.000000 aiohelpersms-0.1.1/aiohelpersms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-09 15:42:27.000000 aiohelpersms-0.1.1/aiohelpersms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 15:42:29.714079 aiohelpersms-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      302 2023-04-09 15:36:28.000000 aiohelpersms-0.1.1/setup.py
```

### Comparing `aiohelpersms-0.1.0/aiohelpersms/aiohelpersms.py` & `aiohelpersms-0.1.1/aiohelpersms/aiohelpersms.py`

 * *Files 27% similar despite different names*

```diff
@@ -72,14 +72,17 @@
 					{
 						"id": 6104,
 						"name": "Вконтакте"
 					}
 				]
 			}
 		"""
+		if not isinstance(country_id, int):
+			raise HelperSMSError("Argument country_id must be an integer")
+
 		method = "GET"
 		path = f"/api/services/{country_id}"
 		return await self._request(method, path)
 
 
 	async def get_operators(self, country_id: int):
 		"""Получить список операторов определённой страны
@@ -92,78 +95,94 @@
 				[
 					"mtt",
 					"megafon",
 					"beeline"
 				]
 			}
 		"""
+		if not isinstance(country_id, int):
+			raise HelperSMSError("Argument country_id must be an integer")
+
 		method = "GET"
 		path = f"/api/operators/{country_id}"
 		return await self._request(method, path)
 
 	
-	@validate_arguments
 	async def get_price(
 		self,
 		service_id: int,
 		reorder_ability: Optional[bool] = False,
 	) -> Dict:
 		"""Получить цену СМС для сервиса
 		Args:
 			service_id (int): Айди сервиса
-			reorder_ability (Optional[bool], optional): Возможность переупорядочивания. Default value: false
+			reorder_ability (Optional[bool], optional): Возможность повторной покупки номера после конца аренды. Default value: false
 		Returns:
 			Dict: {
 				"status": true,
 				"data":
 				{
 					"price": 20.04,
 					"service": "vk"
 				}
 			}
 		"""
+		if not isinstance(service_id, int):
+			raise HelperSMSError("Argument service_id must be an integer")
+		if not isinstance(reorder_ability, bool):
+			raise HelperSMSError("Argument reorder_ability must be an boolean")
+
 		method = "GET"
 		path = f"/api/price/{service_id}"
 		data = {
 			'reorder_ability': reorder_ability
 		}
 
 		for key, value in data.copy().items():
 			if value is None:
 				del data[key]
 		
 		return await self._request(method, path, data)
 
 
-	@validate_arguments
+
 	async def get_number(
 		self,
 		service_id: int,
 		operator_code: Optional[str] = 'any',
 		reorder_ability: Optional[bool] = False,
 		max_price: Optional[int] = 0,
 	) -> Dict:
 		"""Купить номер для получения СМС
 		Args:
 			service_id (int): Айди сервиса
 			operator_code: (Optional[str], optional): Код оператора. Default value: any
-			reorder_ability (Optional[bool], optional): Возможность переупорядочивания. Default value: false
+			reorder_ability (Optional[bool], optional): Возможность повторной покупки номера после конца аренды. Default value: false
 			max_price (Optional[int], optional): Максимальная цена. Default value: 0
 		Returns:
 			Dict: {
 				"status": true,
 				"data":
 				{
 					"order_id": 1,
 					"number": "79851478547",
 					"service": "vk",
 					"price": 20.22
 				}
 			}
 		"""
+		if not isinstance(service_id, int):
+			raise HelperSMSError("Argument service_id must be an integer")
+		if not isinstance(operator_code, str):
+			raise HelperSMSError("Argument operator_code must be an string")
+		if not isinstance(reorder_ability, bool):
+			raise HelperSMSError("Argument reorder_ability must be an boolean")
+		if not isinstance(max_price, int):
+			raise HelperSMSError("Argument max_price must be an integer")
+
 		method = "POST"
 		path = f"/api/number"
 		data = {
 			'service_id': service_id,
 			'operator_code': operator_code,
 			'reorder_ability': reorder_ability,
 			'max_price': max_price
@@ -171,43 +190,48 @@
 		for key, value in data.copy().items():
 			if value is None:
 				del data[key]
 		
 		return await self._request(method, path, data)
 
 
-	@validate_arguments
+	
 	async def set_order_status(
 		self,
 		order_id: int,
 		status: str
 	) -> Dict:
 		"""Изменить статус для заказа
 		Args:
 			order_id (int): Номер заказа
 			status: (str): Статус заказа. Допустимые значения: CANCEL, FINISH
 		Returns:
 			Dict: {
 				"status": true
 			}
 		"""
+		if not isinstance(order_id, int):
+			raise HelperSMSError("Argument order_id must be an integer")
+		if not isinstance(status, str):
+			raise HelperSMSError("Argument status must be an string")
+
 		method = "POST"
 		path = "/api/order_status"
 		data = {
 			'order_id': order_id,
 			'status': status,
 		}
 		for key, value in data.copy().items():
 			if value is None:
 				del data[key]
 
 		return await self._request(method, path, data)
 
 
-	@validate_arguments
+
 	async def get_codes(
 		self,
 		order_id: int,
 	) -> Dict:
 		"""Получить список полученных кодов для номера
 		Args:
 			order_id (int): Номер заказа
@@ -221,21 +245,24 @@
 						"5423",
 						"125423",
 						"4158"
 					]
 				}
 			}
 		"""
+		if not isinstance(order_id, int):
+			raise HelperSMSError("Argument order_id must be an integer")
+
 		method = "GET"
 		path = f"/api/codes/{order_id}"
 
 		return await self._request(method, path)
 	
 
-	@validate_arguments
+
 	async def get_rent_services(
 		self,
 		country_id: int,
 	) -> Dict:
 		"""Получить список сервисов для аренды определённой страны
 		Args:
 			country_id (int): Айди страны
@@ -247,21 +274,24 @@
 					{
 						"id": 1,
 						"name": "Alibaba"
 					}
 				]
 			}
 		"""
+		if not isinstance(country_id, int):
+			raise HelperSMSError("Argument country_id must be an integer")
+
 		method = "GET"
 		path = f"/api/rent_services/{country_id}"
 
 		return await self._request(method, path)
 
 
-	@validate_arguments
+
 	async def get_rent_price(
 		self,
 		service_id : int,
 		rent_time: int,
 	) -> Dict:
 		"""Получить цену аренды для сервиса
 		Args:
@@ -273,21 +303,26 @@
 				"data":
 				{
 					"price": 20.04,
 					"service": "vk"
 				}
 			}
 		"""
+		if not isinstance(service_id, int):
+			raise HelperSMSError("Argument service_id must be an integer")
+		if not isinstance(rent_time, int):
+			raise HelperSMSError("Argument rent_time must be an integer")
+
 		method = "GET"
 		path = f"/api/rent_price/{service_id}/{rent_time}"
 
 		return await self._request(method, path)
 
 
-	@validate_arguments
+
 	async def get_rent_number(
 		self,
 		service_id : int,
 		rent_time: int,
 		operator_code: Optional[str] = 'any',
 	) -> Dict:
 		"""Купить номер для аренды
@@ -303,14 +338,21 @@
 					"order_id": 1,
 					"number": "79851478547",
 					"service": "vk",
 					"price": 20.22
 				}
 			}
 		"""
+		if not isinstance(service_id, int):
+			raise HelperSMSError("Argument service_id must be an integer")
+		if not isinstance(rent_time, int):
+			raise HelperSMSError("Argument rent_time must be an integer")
+		if not isinstance(operator_code, str):
+			raise HelperSMSError("Argument operator_code must be an string")
+
 		method = "POST"
 		path = "/api/rent_number"
 		data = {
 			'service_id': service_id,
 			'rent_time': rent_time,
 			'operator_code': operator_code,
 		}
@@ -330,8 +372,8 @@
 			async with session.request(
 				method, url, headers=headers, json=data
 			) as responce:
 				result = await responce.json()
 				if isinstance(result, dict) and 'detail' in result:
 					raise HelperSMSError(result)
 				else:
-					return result
+					return result
```

