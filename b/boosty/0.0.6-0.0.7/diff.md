# Comparing `tmp/boosty-0.0.6.tar.gz` & `tmp/boosty-0.0.7.tar.gz`

## Comparing `boosty-0.0.6.tar` & `boosty-0.0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    24409 2020-02-02 00:00:00.000000 boosty-0.0.6/logo.png
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 boosty-0.0.6/boosty/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 boosty-0.0.6/boosty/api/__init__.py
--rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 boosty-0.0.6/boosty/api/api.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 boosty-0.0.6/boosty/api/auth.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 boosty-0.0.6/boosty/types/__init__.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 boosty-0.0.6/boosty/types/base.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 boosty-0.0.6/boosty/types/comment.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 boosty-0.0.6/boosty/types/content.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 boosty-0.0.6/boosty/types/donator.py
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 boosty-0.0.6/boosty/types/media_types.py
--rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 boosty-0.0.6/boosty/types/post.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 boosty-0.0.6/boosty/types/reactions.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 boosty-0.0.6/boosty/types/reply.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 boosty-0.0.6/boosty/types/teaser.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 boosty-0.0.6/boosty/types/users.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 boosty-0.0.6/boosty/utils/__init__.py
--rw-r--r--   0        0        0     4987 2020-02-02 00:00:00.000000 boosty-0.0.6/boosty/utils/client.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 boosty-0.0.6/boosty/utils/json.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 boosty-0.0.6/boosty/utils/logging.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 boosty-0.0.6/boosty/utils/post.py
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 boosty-0.0.6/boosty/utils/video.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 boosty-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 boosty-0.0.6/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 boosty-0.0.6/LICENSE
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 boosty-0.0.6/README.md
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 boosty-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 boosty-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    24409 2020-02-02 00:00:00.000000 boosty-0.0.7/logo.png
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/api/__init__.py
+-rw-r--r--   0        0        0     3659 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/api/api.py
+-rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/api/auth.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/types/__init__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/types/base.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/types/comment.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/types/content.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/types/donator.py
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/types/media_types.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/types/post.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/types/reactions.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/types/reply.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/types/teaser.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/types/users.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/utils/__init__.py
+-rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/utils/client.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/utils/json.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/utils/logging.py
+-rw-r--r--   0        0        0     5089 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/utils/post.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/utils/video.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 boosty-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 boosty-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 boosty-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 boosty-0.0.7/README.md
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 boosty-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 boosty-0.0.7/PKG-INFO
```

### Comparing `boosty-0.0.6/logo.png` & `boosty-0.0.7/logo.png`

 * *Files identical despite different names*

### Comparing `boosty-0.0.6/boosty/api/api.py` & `boosty-0.0.7/boosty/api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 
 
 class API:
     API_URL = "https://api.boosty.to"
 
     def __init__(
             self,
-            http_client: ABCHTTPClient = None,
-            auth: Auth = None,
+            http_client: ABCHTTPClient = AiohttpClient(),
+            auth: Auth = Auth(),
     ):
-        self.http_client = http_client or AiohttpClient()
-        self.auth = auth or Auth()
+        self.http_client = http_client
+        self.auth = auth
 
     async def request(self, method: str, params: dict, data: dict = None) -> dict:
         if not params:
             params = {}
         if not data:
             data = {}
         params = {key: value for key, value in params.items() if value is not None}
```

### Comparing `boosty-0.0.6/boosty/api/auth.py` & `boosty-0.0.7/boosty/api/auth.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 from time import time
 
 from boosty.utils.client import ABCHTTPClient, AiohttpClient
 from boosty.utils.json import dict_to_file, file_to_dict
 from boosty.utils.logging import logger
 
 
-class Auth:
+class Auth:  # TODO vk auth
     access_token, refresh_token, expires_at, device_id, headers = None, None, None, None, None
-    DEFAULT_USER_AGENT = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/110.0.0.0 Safari/537.36"
+    DEFAULT_USER_AGENT = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/110.0.0.0 Safari/537.36"  # noqa
     """https://techblog.willshouse.com/2012/01/03/most-common-user-agents/"""
 
     def __init__(
             self,
             auth_file: str = "auth.json",
-            user_agent: str = None,
+            user_agent: str = DEFAULT_USER_AGENT,
     ):
         self.auth_file = auth_file
-        self.user_agent = user_agent or self.DEFAULT_USER_AGENT
+        self.user_agent = user_agent
+
         self.load_auth_data()
 
     def load_auth_data(self):
         try:
             auth_dict = file_to_dict(self.auth_file)
         except FileNotFoundError:
             logger.info(f"No auth file ({self.auth_file}) was found, using blank values (anonymous access mode)")
@@ -40,29 +41,31 @@
             "refresh_token": self.refresh_token,
             "expires_at": self.expires_at,
             "device_id": self.device_id,
         }
         dict_to_file(auth_data, self.auth_file)
 
     def save_auth_data_dotenv(self, dotenv_file=None):
-        import dotenv
+        import dotenv  # noqa
 
         if not dotenv_file:
             dotenv_file = dotenv.find_dotenv()
 
         print(f".env file found: {dotenv_file}")
         dotenv.load_dotenv(dotenv_file)
         dotenv.set_key(dotenv_file, "ACCESS_TOKEN", self.access_token, "auto")
         dotenv.set_key(dotenv_file, "REFRESH_TOKEN", self.refresh_token, "auto")
+        dotenv.set_key(dotenv_file, "EXPIRES_AT", self.expires_at, "auto")
+        dotenv.set_key(dotenv_file, "DEVICE_ID", self.device_id, "auto")
 
-    def get_auth_data(self):
-        return self.access_token, self.refresh_token, self.expires_at
-
-    async def refresh_auth_data(self, session: ABCHTTPClient, api_url: str = None):
+    async def refresh_auth_data(self, session: ABCHTTPClient, api_url: str = ""):
         self.load_auth_data()
+        if not self.refresh_token:
+            logger.error("No refresh token was found to refresh auth data")
+            raise ValueError("No refresh token was found to refresh auth data")
 
         response_data = await session.request_json(
             f"{api_url}/oauth/token/",
             method="POST",
             data={
                 "device_id": self.device_id,
                 "device_os": "web",
@@ -82,13 +85,12 @@
         self.save_auth_data()
         self.load_auth_data()
 
 
 async def main():
     auth = Auth()
     await auth.refresh_auth_data(AiohttpClient())
-    access_token, refresh_token, expires = auth.get_auth_data()
-    print(f"{access_token , refresh_token , expires = }")
+    logger.info(f"{auth.access_token, auth.refresh_token, auth.expires_at = }")
 
 
 if __name__ == "__main__":
     asyncio.run(main())
```

### Comparing `boosty-0.0.6/boosty/types/comment.py` & `boosty-0.0.7/boosty/types/reply.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,38 @@
-from typing import Literal, Annotated
 from datetime import datetime
+from typing import Literal
 
-from pydantic import UUID4, Field
+from pydantic import UUID4
 
 from .base import BaseObject
-from .reply import RepliesResponse
 from .users import Commentator
 from .reactions import Reactions, Reacted
-from .media_types import Text, Smile, Link, Image
 
-CommentData = Annotated[
-    Text | Smile | Image | Link,
-    Field(discriminator="type")]
 
-
-class Smile(BaseObject):
-    type: Literal["smile"]
-
-
-class Comment(BaseObject):
+class Reply(BaseObject):
     id: UUID4
     intId: int
     createdAt: datetime
     updatedAt: datetime | None
     isBlocked: bool
     isUpdated: bool
     isDeleted: bool
     author: Commentator
     reactions: Reactions
     reacted: Reacted | None
     replyCount: int
-    replies: RepliesResponse
     post: dict[Literal["id"], UUID4]
-    data: list[CommentData]
+    data: list[dict]
+
+    replyToUser: Commentator
+    replyId: str
+    parentId: str
 
 
-class CommentsResponseExtra(BaseObject):
+class ReplyResponseExtra(BaseObject):
     isLast: bool
-    isFirst: bool | None
+    isFirst: bool
 
 
-class CommentsResponse(BaseObject):
-    data: list[Comment]
-    extra: CommentsResponseExtra
+class RepliesResponse(BaseObject):
+    data: list[Reply]
+    extra: ReplyResponseExtra
```

### Comparing `boosty-0.0.6/boosty/types/media_types.py` & `boosty-0.0.7/boosty/types/media_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     defaultPreview: HttpUrl
     """random frame from video as thumbnail"""
     preview: HttpUrl
     """author thumbnail or defaultPreview"""
     previewId: UUID4 | None
     """author thumbnail image id or None"""
     vid: int
-    """ok.ru video id"""
+    """Unknown, probably ok.ru video id"""
     failoverHost: str
     """Unknown, probably interchangeable host for playerUrls"""
 
 
 class Image(FileBase):
     type: Literal["image"]
     rendition: Literal["", "teaser_auto_background"]
```

### Comparing `boosty-0.0.6/boosty/types/post.py` & `boosty-0.0.7/boosty/types/post.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,49 +53,56 @@
     id: UUID4
     createdAt: datetime
     """Creation timestamp"""
     updatedAt: datetime
     """Last update timestamp"""
     publishTime: datetime
     """Publication timestamp"""
+    isPublished: bool
+    """Is post published to users"""
+    user: BlogUser
+    """Blogger user object"""
+
+    title: str
+    """Post title"""
     data: list[Content]
     """List of contents, attached to post (text included)"""
+    tags: list[Tag]
+
+    hasAccess: bool
+    """Is post available for you"""
+    teaser: list[Teaser]
+    """Post teaser for users which haven't access to post"""
+
     count: Count
     """Count of likes, comments, reactions"""
     comments: CommentsResponse
-    hasAccess: bool
-    """Is post is available for users"""
     isCommentsDenied: bool
     isLiked: bool
-    isPublished: bool
     price: int
     """Price to open post"""
     signedQuery: str
     """Query for media fetching"""
     subscriptionLevel: SubscriptionLevel | None
     """Subscription level for non-free posts"""
-    tags: list[Tag]
-    teaser: list[Teaser]
-    title: str
-    user: BlogUser
 
     reacted: React | None
     """Unknown"""
     isWaitingVideo: bool
     """Unknown, probably an indicator, which shows if video is incomplete"""
     currencyPrices: Currency
     """Unknown"""
     isRecord: bool
     """Is post a stream record"""
     donators: DonatorsResponse
-    """List of donators of post"""
+    """List of sponsors of the post"""
     donations: int
     """Amount of donations"""
     int_id: int
-    """Unknown, probably post uuid to int"""
+    """Unknown, probably post.id to int"""
 
 
 class PostsResponseExtra(BaseObject):
     isLast: bool
     """Is last page"""
     offset: str
     """Value for pagination. Example: :code:`1654884900:923396`"""
```

### Comparing `boosty-0.0.6/boosty/types/reply.py` & `boosty-0.0.7/boosty/types/comment.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,41 @@
+from typing import Literal, Annotated
 from datetime import datetime
-from typing import Literal
 
-from pydantic import UUID4
+from pydantic import UUID4, Field
 
 from .base import BaseObject
+from .reply import RepliesResponse
 from .users import Commentator
 from .reactions import Reactions, Reacted
+from .media_types import Text, Smile, Link, Image
 
+CommentData = Annotated[
+    Text | Smile | Image | Link,
+    Field(discriminator="type")]
 
-class Reply(BaseObject):
+
+class Comment(BaseObject):
     id: UUID4
     intId: int
     createdAt: datetime
     updatedAt: datetime | None
     isBlocked: bool
     isUpdated: bool
     isDeleted: bool
     author: Commentator
     reactions: Reactions
     reacted: Reacted | None
     replyCount: int
+    replies: RepliesResponse
     post: dict[Literal["id"], UUID4]
-    data: list[dict]
-
-    replyToUser: Commentator
-    replyId: str
-    parentId: str
+    data: list[CommentData]
 
 
-class ReplyResponseExtra(BaseObject):
+class CommentsResponseExtra(BaseObject):
     isLast: bool
-    isFirst: bool
+    isFirst: bool | None
 
 
-class RepliesResponse(BaseObject):
-    data: list[Reply]
-    extra: ReplyResponseExtra
+class CommentsResponse(BaseObject):
+    data: list[Comment]
+    extra: CommentsResponseExtra
```

### Comparing `boosty-0.0.6/boosty/types/users.py` & `boosty-0.0.7/boosty/types/users.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 class DonatorUser(BaseUser):
     nickColor: conint(ge=0, le=15)
     """color id from 0 to 15"""
     displayName: str
     vkplayProfileLink: HttpUrl | None
     email: EmailStr
+    isVerifiedStreamer: bool
 
 
 class Commentator(BaseUser):
     nickColor: conint(ge=0, le=15)
     """color id from 0 to 15"""
     displayName: str
     vkplayProfileLink: HttpUrl | Literal[""]
```

### Comparing `boosty-0.0.6/boosty/utils/client.py` & `boosty-0.0.7/boosty/utils/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # stolen from vkbottle with love <3
 
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Any, Optional, Type, TypeVar
+from typing import TYPE_CHECKING, Any, Optional, Type, TypeVar, Mapping
 
 from aiohttp import ClientSession
 from multidict import CIMultiDictProxy
 
 from boosty.utils.json import json
 
 if TYPE_CHECKING:
@@ -45,14 +45,20 @@
     @abstractmethod
     async def request_content(
         self, url: str, method: str = "GET", data: Optional[dict] = None, **kwargs
     ) -> bytes:
         pass
 
     @abstractmethod
+    async def request_headers(
+        self, url: str, data: Optional[dict] = None, **kwargs
+    ) -> Mapping[str, str]:
+        pass
+
+    @abstractmethod
     async def close(self) -> None:
         pass
 
     async def __aenter__(self) -> "ABCHTTPClient":
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb) -> None:
@@ -158,9 +164,9 @@
     def __new__(
         cls: Type[TSingleAiohttpClient], *args: Any, **kwargs: Any
     ) -> TSingleAiohttpClient:
         if cls.__instance__ is None:
             cls.__instance__ = super().__new__(cls, *args, **kwargs)
         return cls.__instance__
 
-    def __aexit__(self, exc_type, exc_val, exc_tb):
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
         pass  # no need to close session in this case
```

### Comparing `boosty-0.0.6/boosty/utils/video.py` & `boosty-0.0.7/boosty/utils/video.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     "full_hd": 5,
     "high": 3,
     "medium": 2,
     "low": 1,
     "lowest": 0,
     "tiny": -1,  # 4
 }
-player_size_by_number: dict[int, player_urls_size_names] = {v: k for k, v in player_size_dict.items()}
+player_size_by_number: dict[int, player_urls_size_names] = {v: k for k, v in player_size_dict.items()}  # type: ignore
 
 
 class VideoSize(BaseObject):
     name: size_names
     url: HttpUrl
     seekSchema: Literal[3]
     disallowed: Literal[False]
```

### Comparing `boosty-0.0.6/.gitignore` & `boosty-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `boosty-0.0.6/LICENSE` & `boosty-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `boosty-0.0.6/README.md` & `boosty-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `boosty-0.0.6/pyproject.toml` & `boosty-0.0.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -28,17 +28,18 @@
 
 [project.urls]
 Documentation = "https://github.com/barsikus007/boosty#readme"
 Issues = "https://github.com/barsikus007/boosty/issues"
 Source = "https://github.com/barsikus007/boosty"
 
 [project.optional-dependencies]
+logging = ["loguru~=0.6.0"]
 dotenv = ["python-dotenv~=1.0.0"]
 fast = ["orjson~=3.8.8", "aiohttp[speedups]~=3.8.4"]
-all = ["boosty[dotenv,fast]"]
+all = ["boosty[logging,dotenv,fast]"]
 
 
 [tool.hatch.version]
 path = "boosty/__init__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
```

### Comparing `boosty-0.0.6/PKG-INFO` & `boosty-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boosty
-Version: 0.0.6
+Version: 0.0.7
 Summary: Asynchronous boosty wrapper with some utils
 Project-URL: Documentation, https://github.com/barsikus007/boosty#readme
 Project-URL: Issues, https://github.com/barsikus007/boosty/issues
 Project-URL: Source, https://github.com/barsikus007/boosty
 Author: barsikus007
 License-Expression: MIT
 License-File: LICENSE
@@ -15,20 +15,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: aiohttp~=3.8.4
 Requires-Dist: pydantic[email]~=1.10.6
 Provides-Extra: all
-Requires-Dist: boosty[dotenv,fast]; extra == 'all'
+Requires-Dist: boosty[dotenv,fast,logging]; extra == 'all'
 Provides-Extra: dotenv
 Requires-Dist: python-dotenv~=1.0.0; extra == 'dotenv'
 Provides-Extra: fast
 Requires-Dist: aiohttp[speedups]~=3.8.4; extra == 'fast'
 Requires-Dist: orjson~=3.8.8; extra == 'fast'
+Provides-Extra: logging
+Requires-Dist: loguru~=0.6.0; extra == 'logging'
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://github.com/barsikus007/boosty">
     <img src="https://raw.githubusercontent.com/barsikus007/boosty/master/logo.png" alt="BoostyPy">
   </a>
 </p>
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 2.1 Name: boosty Version: 0.0.6 Summary: Asynchronous boosty
+Metadata-Version: 2.1 Name: boosty Version: 0.0.7 Summary: Asynchronous boosty
 wrapper with some utils Project-URL: Documentation, https://github.com/
 barsikus007/boosty#readme Project-URL: Issues, https://github.com/barsikus007/
 boosty/issues Project-URL: Source, https://github.com/barsikus007/boosty
 Author: barsikus007 License-Expression: MIT License-File: LICENSE Keywords:
 asyncio,boosty,wrapper Classifier: Development Status :: 4 - Beta Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python ::
 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: Programming
 Language :: Python :: Implementation :: PyPy Requires-Python: >=3.10 Requires-
 Dist: aiohttp~=3.8.4 Requires-Dist: pydantic[email]~=1.10.6 Provides-Extra: all
-Requires-Dist: boosty[dotenv,fast]; extra == 'all' Provides-Extra: dotenv
-Requires-Dist: python-dotenv~=1.0.0; extra == 'dotenv' Provides-Extra: fast
-Requires-Dist: aiohttp[speedups]~=3.8.4; extra == 'fast' Requires-Dist:
-orjson~=3.8.8; extra == 'fast' Description-Content-Type: text/markdown
+Requires-Dist: boosty[dotenv,fast,logging]; extra == 'all' Provides-Extra:
+dotenv Requires-Dist: python-dotenv~=1.0.0; extra == 'dotenv' Provides-Extra:
+fast Requires-Dist: aiohttp[speedups]~=3.8.4; extra == 'fast' Requires-Dist:
+orjson~=3.8.8; extra == 'fast' Provides-Extra: logging Requires-Dist:
+loguru~=0.6.0; extra == 'logging' Description-Content-Type: text/markdown
                                   [BoostyPy]
 # Boosty Wrapper [![PyPI - Version](https://img.shields.io/pypi/v/boosty.svg)]
 (https://pypi.org/project/boosty) [![PyPI - Python Version](https://
 img.shields.io/pypi/pyversions/boosty.svg)](https://pypi.org/project/boosty) [!
 [Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)]
 (https://github.com/pypa/hatch) ----- **Table of Contents** - [Installation]
 (#installation) - [License](#license) - [Usage](#usage) ## Installation
```

