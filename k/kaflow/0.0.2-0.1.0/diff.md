# Comparing `tmp/kaflow-0.0.2.tar.gz` & `tmp/kaflow-0.1.0.tar.gz`

## Comparing `kaflow-0.0.2.tar` & `kaflow-0.1.0.tar`

### file list

```diff
@@ -1,31 +1,36 @@
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 kaflow-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 kaflow-0.0.2/Makefile
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 kaflow-0.0.2/.github/workflows/release.yaml
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 kaflow-0.0.2/.github/workflows/test.yaml
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 kaflow-0.0.2/kaflow/__init__.py
--rw-r--r--   0        0        0    17651 2020-02-02 00:00:00.000000 kaflow-0.0.2/kaflow/applications.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 kaflow-0.0.2/kaflow/dependencies.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 kaflow-0.0.2/kaflow/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.0.2/kaflow/py.typed
--rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 kaflow-0.0.2/kaflow/serializers.py
--rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 kaflow-0.0.2/kaflow/topic.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 kaflow-0.0.2/kaflow/typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.0.2/kaflow/worker.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.0.2/kaflow/_utils/__init__.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 kaflow-0.0.2/kaflow/_utils/asyncio.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 kaflow-0.0.2/kaflow/_utils/inspect.py
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 kaflow-0.0.2/kaflow/_utils/typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 kaflow-0.0.2/tests/key_value.proto
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 kaflow-0.0.2/tests/key_value_pb2.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 kaflow-0.0.2/tests/key_value_pb2.pyi
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 kaflow-0.0.2/tests/test_application.py
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 kaflow-0.0.2/tests/test_serializers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.0.2/tests/_utils/__init__.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 kaflow-0.0.2/tests/_utils/test_asyncio.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 kaflow-0.0.2/tests/_utils/test_inspect.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 kaflow-0.0.2/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 kaflow-0.0.2/LICENSE
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 kaflow-0.0.2/README.md
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 kaflow-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 kaflow-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 kaflow-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 kaflow-0.1.0/Makefile
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 kaflow-0.1.0/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 kaflow-0.1.0/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/__init__.py
+-rw-r--r--   0        0        0     8100 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/_consumer.py
+-rw-r--r--   0        0        0    21977 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/applications.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/dependencies.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/exceptions.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/logger.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/message.py
+-rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/parameters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/py.typed
+-rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/serializers.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/_utils/__init__.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/_utils/asyncio.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/_utils/inspect.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/asyncapi/__init__.py
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/asyncapi/_builder.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/asyncapi/docs.py
+-rw-r--r--   0        0        0     9688 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/asyncapi/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 kaflow-0.1.0/tests/key_value.proto
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 kaflow-0.1.0/tests/key_value_pb2.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 kaflow-0.1.0/tests/key_value_pb2.pyi
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 kaflow-0.1.0/tests/test_application.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 kaflow-0.1.0/tests/test_serializers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.0/tests/_utils/__init__.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 kaflow-0.1.0/tests/_utils/test_asyncio.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 kaflow-0.1.0/tests/_utils/test_inspect.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 kaflow-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 kaflow-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 kaflow-0.1.0/README.md
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 kaflow-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 kaflow-0.1.0/PKG-INFO
```

### Comparing `kaflow-0.0.2/.github/workflows/release.yaml` & `kaflow-0.1.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `kaflow-0.0.2/.github/workflows/test.yaml` & `kaflow-0.1.0/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `kaflow-0.0.2/kaflow/applications.py` & `kaflow-0.1.0/kaflow/applications.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,165 +8,205 @@
 from typing import (
     TYPE_CHECKING,
     Any,
     AsyncContextManager,
     AsyncIterator,
     Awaitable,
     Callable,
+    Coroutine,
     Literal,
     Sequence,
+    Union,
 )
+from uuid import uuid4
 
 from aiokafka import AIOKafkaConsumer, AIOKafkaProducer
 from aiokafka.helpers import create_ssl_context
 from di import Container, ScopeState
 from di.dependent import Dependent
 from di.executors import AsyncExecutor
-from pydantic import BaseModel
+from kafka.coordinator.assignors.roundrobin import RoundRobinPartitionAssignor
+from kafka.partitioner.default import DefaultPartitioner
 
+from kaflow import parameters
+from kaflow._consumer import TopicConsumerFunc
 from kaflow._utils.asyncio import asyncify
-from kaflow._utils.inspect import (
-    annotated_param_with,
-    has_return_annotation,
-    is_not_coroutine_function,
-)
+from kaflow._utils.inspect import is_not_coroutine_function
 from kaflow.dependencies import Scopes
-from kaflow.serializers import MESSAGE_SERIALIZER_FLAG, _serialize
-from kaflow.topic import TopicProcessingFunc
-from kaflow.typing import TopicMessage
+from kaflow.exceptions import KaflowDeserializationException
+from kaflow.message import Message
 
 if TYPE_CHECKING:
+    from aiokafka.abc import AbstractTokenProvider
+    from kafka.coordinator.assignors.abstract import AbstractPartitionAssignor
+
+    from kaflow.asyncapi.models import AsyncAPI
     from kaflow.serializers import Serializer
-    from kaflow.typing import (
-        ConsumerFunc,
-        DeserializationErrorHandlerFunc,
-        ExceptionHandlerFunc,
-        ProducerFunc,
-    )
-
-
-def annotated_serializer_info(
-    param: Any,
-) -> tuple[type[BaseModel], type[Serializer], dict[str, Any]]:
-    """Get the type and serializer of a parameter annotated (`Annotated[...]`) with
-    a Kaflow serializer. This function expect the parameter to be `Annotated` with a
-    Kaflow serializer, the `kaflow.serializers.MESSAGE_SERIALIZER_FLAG`, and optionally
-    with a `dict` containing extra information that could be used by the serializer.
-
-    Args:
-        param: the annotated parameter to get the type and serializer from.
-
-    Returns:
-        A tuple with the type and serializer of the annotated parameter, and a `dict`
-        containing extra information that could be used by the serializer.
-    """
-    param_type = param.__args__[0]
-    serializer = param.__metadata__[0]
-    if len(param.__metadata__) == 3:
-        extra_metadata = param.__metadata__[2]
-        extra_annotations_keys = serializer.extra_annotations_keys()
-        missing_keys = extra_annotations_keys - extra_metadata.keys()
-        if missing_keys:
-            raise ValueError(
-                f"Missing keys in extra metadata for {serializer.__name__}: "
-                f"{missing_keys}"
-            )
-        extra_dict = {k: extra_metadata[k] for k in extra_annotations_keys}
-        return param_type, serializer, extra_dict
-    return param_type, serializer, {}
-
-
-def get_message_param_info(
-    param: Any,
-) -> tuple[type[TopicMessage], type[Serializer] | None, dict[str, Any]]:
-    if param is bytes:
-        return bytes, None, {}
-
-    return annotated_serializer_info(param)
-
-
-def bytes_or_serializer_param(signature: inspect.Signature) -> inspect.Parameter | None:
-    """Get the parameter annotated with `kaflow.serializers.MESSAGE_SERIALIZER_FLAG`
-    or of type `bytes` from a function signature.
-
-    Args:
-        signature: The function signature to get the parameter from.
-
-    Returns:
-        The parameter annotated with `kaflow.serializers.MESSAGE_SERIALIZER_FLAG` or of
-        type `bytes` from the function signature, or `None` if no such parameter is
-        found.
-    """
-    for param in signature.parameters.values():
-        if param.annotation is bytes:
-            return param
-        if annotated_param_with(MESSAGE_SERIALIZER_FLAG, param.annotation):
-            return param
-    return None
-
-
-SecurityProtocol = Literal["PLAINTEXT", "SSL", "SASL_PLAINTEXT", "SASL_SSL"]
-SaslMechanism = Literal[
-    "PLAIN", "GSSAPI", "OAUTHBEARER", "SCRAM-SHA-256", "SCRAM-SHA-512"
-]
-AutoOffsetReset = Literal["earliest", "latest", "none"]
+    from kaflow.typing import TopicValueKeyHeader
+
+ConsumerFunc = Callable[..., Union[Message, Awaitable[Union[Message, None]], None]]
+ProducerFunc = Callable[..., Union[Message, Awaitable[Message]]]
+ExceptionHandlerFunc = Callable[[Exception], Awaitable]
+DeserializationErrorHandlerFunc = Callable[[KaflowDeserializationException], Awaitable]
 
 
 class Kaflow:
     def __init__(
         self,
-        name: str,
         brokers: str | list[str],
+        client_id: str | None = None,
         group_id: str | None = None,
-        security_protocol: SecurityProtocol = "PLAINTEXT",
+        acks: Literal[0, 1, "all"] = 1,
+        compression_type: Literal["gzip", "snappy", "lz4", "zstd", None] = None,
+        max_batch_size: int = 16384,
+        partitioner: Callable[
+            [bytes, list[int], list[int]], int
+        ] = DefaultPartitioner(),
+        max_request_size: int = 1048576,
+        linger_ms: int = 0,
+        send_backoff_ms: int = 100,
+        connections_max_idle_ms: int = 540000,
+        enable_idempotence: bool = False,
+        transactional_id: str | None = None,
+        transaction_timeout_ms: int = 60000,
+        fetch_max_wait_ms: int = 500,
+        fetch_max_bytes: int = 52428800,
+        fetch_min_bytes: int = 1,
+        max_partition_fetch_bytes: int = 1 * 1024 * 1024,
+        request_timeout_ms: int = 40 * 1000,
+        retry_backoff_ms: int = 100,
+        auto_offset_reset: Literal["earliest", "latest", "none"] = "latest",
+        enable_auto_commit: bool = True,
+        auto_commit_interval_ms: int = 5000,
+        check_crcs: bool = True,
+        metadata_max_age_ms: int = 5 * 60 * 1000,
+        partition_assignment_strategy: list[AbstractPartitionAssignor] | None = None,
+        max_poll_interval_ms: int = 300000,
+        rebalance_timeout_ms: int | None = None,
+        session_timeout_ms: int = 10000,
+        heartbeat_interval_ms: int = 3000,
+        consumer_timeout_ms: int = 200,
+        max_poll_records: int | None = None,
+        kafka_api_version: str = "auto",
+        security_protocol: Literal[
+            "PLAINTEXT", "SSL", "SASL_PLAINTEXT", "SASL_SSL"
+        ] = "PLAINTEXT",
+        exclude_internal_topics: bool = True,
+        connection_max_idle_ms: int = 540000,
+        isolation_level: Literal[
+            "read_committed", "read_uncommitted"
+        ] = "read_committed",
         cafile: str | None = None,
         capath: str | None = None,
         cadata: bytes | None = None,
         certfile: str | None = None,
         keyfile: str | None = None,
         cert_password: str | None = None,
-        sasl_mechanism: SaslMechanism | None = None,
+        sasl_mechanism: Literal[
+            "PLAIN", "GSSAPI", "OAUTHBEARER", "SCRAM-SHA-256", "SCRAM-SHA-512"
+        ]
+        | None = None,
         sasl_plain_username: str | None = None,
         sasl_plain_password: str | None = None,
-        auto_offset_reset: AutoOffsetReset = "latest",
-        auto_commit: bool = True,
-        auto_commit_interval_ms: int = 5000,
+        sasl_kerberos_service_name: str = "kafka",
+        sasl_kerberos_domain_name: str | None = None,
+        sasl_oauth_token_provider: AbstractTokenProvider | None = None,
         lifespan: Callable[..., AsyncContextManager[None]] | None = None,
+        asyncapi_version: str = "2.6.0",
+        title: str = "Kaflow",
+        version: str = "0.0.1",
+        description: str | None = None,
+        terms_of_service: str | None = None,
+        contact: dict[str, str | Any] | None = None,
+        license_info: dict[str, str | Any] | None = None,
     ) -> None:
-        self.name = name
+        # AIOKafka
         self.brokers = brokers
+        self.client_id = client_id or f"kaflow-{uuid4()}"
         self.group_id = group_id
+        self.acks = acks
+        self.compression_type = compression_type
+        self.max_batch_size = max_batch_size
+        self.partitioner = partitioner
+        self.max_request_size = max_request_size
+        self.linger_ms = linger_ms
+        self.send_backoff_ms = send_backoff_ms
+        self.connections_max_idle_ms = connections_max_idle_ms
+        self.enable_idempotence = enable_idempotence
+        self.transactional_id = transactional_id
+        self.transaction_timeout_ms = transaction_timeout_ms
+        self.fetch_max_wait_ms = fetch_max_wait_ms
+        self.fetch_max_bytes = fetch_max_bytes
+        self.fetch_min_bytes = fetch_min_bytes
+        self.max_partition_fetch_bytes = max_partition_fetch_bytes
+        self.request_timeout_ms = request_timeout_ms
+        self.retry_backoff_ms = retry_backoff_ms
+        self.auto_offset_reset = auto_offset_reset
+        self.enable_auto_commit = enable_auto_commit
+        self.auto_commit_interval_ms = auto_commit_interval_ms
+        self.check_crcs = check_crcs
+        self.metadata_max_age_ms = metadata_max_age_ms
+        self.partition_assignment_strategy = partition_assignment_strategy or (
+            RoundRobinPartitionAssignor,
+        )
+        self.max_poll_interval_ms = max_poll_interval_ms
+        self.rebalance_timeout_ms = rebalance_timeout_ms
+        self.session_timeout_ms = session_timeout_ms
+        self.heartbeat_interval_ms = heartbeat_interval_ms
+        self.consumer_timeout_ms = consumer_timeout_ms
+        self.max_poll_records = max_poll_records
+        self.kafka_api_version = kafka_api_version
         self.security_protocol = security_protocol
+        self.exclude_internal_topics = exclude_internal_topics
+        self.connection_max_idle_ms = connection_max_idle_ms
+        self.isolation_level = isolation_level
+        self.cafile = cafile
+        self.capath = capath
+        self.cadata = cadata
+        self.certfile = certfile
+        self.keyfile = keyfile
+        self.cert_password = cert_password
         self.sasl_mechanism = sasl_mechanism
         self.sasl_plain_username = sasl_plain_username
         self.sasl_plain_password = sasl_plain_password
-        self.auto_offset_reset = auto_offset_reset
-        self.auto_commit = auto_commit
-        self.auto_commit_interval_ms = auto_commit_interval_ms
+        self.sasl_kerberos_service_name = sasl_kerberos_service_name
+        self.sasl_kerberos_domain_name = sasl_kerberos_domain_name
+        self.sasl_oauth_token_provider = sasl_oauth_token_provider
 
         if security_protocol == "SSL" or security_protocol == "SASL_SSL":
             self.ssl_context = create_ssl_context(
                 cafile=cafile,
                 capath=capath,
                 cadata=cadata,
                 certfile=certfile,
                 keyfile=keyfile,
                 password=cert_password,
             )
         else:
             self.ssl_context = None
 
+        # AsyncAPI
+        self.asyncapi_version = asyncapi_version
+        self.title = title
+        self.version = version
+        self.description = description
+        self.terms_of_service = terms_of_service
+        self.contact = contact
+        self.license_info = license_info
+        self.asyncapi_schema: AsyncAPI | None = None
+
+        # di
         self._container = Container()
         self._container_state = ScopeState()
 
         self._loop = asyncio.get_event_loop()
         self._consumer: AIOKafkaConsumer | None = None
         self._producer: AIOKafkaProducer | None = None
 
-        self._consumers: dict[str, TopicProcessingFunc] = {}
+        self._consumers: dict[str, TopicConsumerFunc] = {}
         self._producers: dict[str, list[ProducerFunc]] = defaultdict(list)
         self._sink_topics: set[str] = set()
 
         self._exception_handlers: dict[
             type[Exception], Callable[..., Awaitable[None]]
         ] = {}
         self._deserialization_error_handler: DeserializationErrorHandlerFunc | None = (
@@ -199,173 +239,183 @@
 
         self.lifespan = lifespan_ctx
 
     def _prepare(self) -> None:
         for topic_processor in self._consumers.values():
             topic_processor.prepare(self._container_state)
 
-    def _add_topic_processor(
+    def _add_topic_consumer_func(
         self,
         topic: str,
         func: ConsumerFunc,
-        param_type: type[TopicMessage],
-        deserializer: Serializer | None = None,
-        return_type: type[TopicMessage] | None = None,
-        serializer: Serializer | None = None,
+        value_param_type: type[TopicValueKeyHeader],
+        value_deserializer: Serializer | None = None,
+        key_param_type: type[TopicValueKeyHeader] | None = None,
+        key_deserializer: Serializer | None = None,
+        headers_type_deserializers: dict[
+            str, tuple[type[TopicValueKeyHeader], Serializer | None]
+        ]
+        | None = None,
         sink_topics: Sequence[str] | None = None,
     ) -> None:
-        topic_processor = TopicProcessingFunc(
+        topic_processor = TopicConsumerFunc(
             name=topic,
             container=self._container,
             publish_fn=self._publish,
             exception_handlers=self._exception_handlers,
             deserialization_error_handler=self._deserialization_error_handler,
             func=func,
-            param_type=param_type,
-            deserializer=deserializer,
-            return_type=return_type,
-            serializer=serializer,
+            value_param_type=value_param_type,
+            value_deserializer=value_deserializer,
+            key_param_type=key_param_type,
+            key_deserializer=key_deserializer,
+            headers_type_deserializers=headers_type_deserializers,
             sink_topics=sink_topics,
         )
         self._consumers[topic] = topic_processor
 
     def _create_consumer(self) -> AIOKafkaConsumer:
         return AIOKafkaConsumer(
             *self._consumers.keys(),
             loop=self._loop,
             bootstrap_servers=self.brokers,
-            client_id=self.name,
+            client_id=self.client_id,
             group_id=self.group_id,
-            ssl_context=self.ssl_context,
+            fetch_min_bytes=self.fetch_min_bytes,
+            fetch_max_bytes=self.fetch_max_bytes,
+            fetch_max_wait_ms=self.fetch_max_wait_ms,
+            max_partition_fetch_bytes=self.max_partition_fetch_bytes,
+            max_poll_records=self.max_poll_records,
+            request_timeout_ms=self.request_timeout_ms,
+            retry_backoff_ms=self.retry_backoff_ms,
+            auto_offset_reset=self.auto_offset_reset,
+            enable_auto_commit=self.enable_auto_commit,
+            auto_commit_interval_ms=self.auto_commit_interval_ms,
+            check_crcs=self.check_crcs,
+            metadata_max_age_ms=self.metadata_max_age_ms,
+            partition_assignment_strategy=self.partition_assignment_strategy,
+            max_poll_interval_ms=self.max_poll_interval_ms,
+            rebalance_timeout_ms=self.rebalance_timeout_ms,
+            session_timeout_ms=self.session_timeout_ms,
+            heartbeat_interval_ms=self.heartbeat_interval_ms,
+            consumer_timeout_ms=self.consumer_timeout_ms,
+            api_version=self.kafka_api_version,
             security_protocol=self.security_protocol,
+            ssl_context=self.ssl_context,
+            exclude_internal_topics=self.exclude_internal_topics,
+            connections_max_idle_ms=self.connections_max_idle_ms,
+            isolation_level=self.isolation_level,
             sasl_mechanism=self.sasl_mechanism,
             sasl_plain_username=self.sasl_plain_username,
             sasl_plain_password=self.sasl_plain_password,
-            enable_auto_commit=self.auto_commit,
-            auto_offset_reset=self.auto_offset_reset,
-            auto_commit_interval_ms=self.auto_commit_interval_ms,
+            sasl_kerberos_domain_name=self.sasl_kerberos_domain_name,
+            sasl_kerberos_service_name=self.sasl_kerberos_service_name,
+            sasl_oauth_token_provider=self.sasl_oauth_token_provider,
         )
 
     def _create_producer(self) -> AIOKafkaProducer:
         return AIOKafkaProducer(
             loop=self._loop,
             bootstrap_servers=self.brokers,
-            client_id=self.name,
-            ssl_context=self.ssl_context,
+            client_id=self.client_id,
+            metadata_max_age_ms=self.metadata_max_age_ms,
+            request_timeout_ms=self.request_timeout_ms,
+            api_version=self.kafka_api_version,
+            acks=self.acks,
+            compression_type=self.compression_type,
+            max_batch_size=self.max_batch_size,
+            partitioner=self.partitioner,
+            max_request_size=self.max_request_size,
+            linger_ms=self.linger_ms,
+            send_backoff_ms=self.send_backoff_ms,
+            retry_backoff_ms=self.retry_backoff_ms,
             security_protocol=self.security_protocol,
+            ssl_context=self.ssl_context,
+            connections_max_idle_ms=self.connections_max_idle_ms,
+            enable_idempotence=self.enable_idempotence,
+            transactional_id=self.transactional_id,
+            transaction_timeout_ms=self.transaction_timeout_ms,
             sasl_mechanism=self.sasl_mechanism,
             sasl_plain_username=self.sasl_plain_username,
             sasl_plain_password=self.sasl_plain_password,
+            sasl_kerberos_service_name=self.sasl_kerberos_service_name,
+            sasl_kerberos_domain_name=self.sasl_kerberos_domain_name,
+            sasl_oauth_token_provider=self.sasl_oauth_token_provider,
         )
 
     def consume(
         self,
         topic: str,
         sink_topics: Sequence[str] | None = None,
     ) -> Callable[[ConsumerFunc], ConsumerFunc]:
         def register_consumer(func: ConsumerFunc) -> ConsumerFunc:
-            signature = inspect.signature(func)
-            message_param = bytes_or_serializer_param(signature)
-            if not message_param:
-                raise ValueError(
-                    f"'{func.__name__}' function does not have a parameter with a type"
-                    " like `bytes` or a `pydantic.BaseModel` annotated with a"
-                    " deserializer like `kaflow.serializers.Json` to receive the"
-                    f" message from the topic: `async def  {func.__name__}(message:"
-                    " Json[BaseModel]): ...`."
-                )
-            return_type: Any | None = None
-            serializer_type: type[Serializer] | None = None
-            serializer_extra: dict[str, Any] = {}
-            if has_return_annotation(signature):
-                if (
-                    not annotated_param_with(
-                        MESSAGE_SERIALIZER_FLAG, signature.return_annotation
-                    )
-                    and signature.return_annotation is not bytes
-                ):
-                    raise ValueError(
-                        f"`{signature.return_annotation.__name__}` cannot be used as a"
-                        f" return type for '{func.__name__}' consumer function."
-                        " Consumer functions must return bytes or a"
-                        " `pydantic.BaseModel` annotated with a serializer like"
-                        " `kaflow.serializers.Json` so it can be published to the"
-                        f" `sink_topics`: `async def {func.__name__}(message:"
-                        " Json[BaseModel]) -> Json[BaseModel]: ...`."
-                    )
-                else:
-                    (
-                        return_type,
-                        serializer_type,
-                        serializer_extra,
-                    ) = get_message_param_info(signature.return_annotation)
-            param_type, deserializer_type, deserializer_extra = get_message_param_info(
-                message_param.annotation
-            )
-            deserializer = None
-            if deserializer_type:
-                deserializer = deserializer_type(**deserializer_extra)
-            serializer = None
-            if serializer_type:
-                serializer = serializer_type(**serializer_extra)
-            self._add_topic_processor(
+            (
+                value_param_type,
+                value_deserializer,
+                key_param_type,
+                key_deserializer,
+                headers_type_deserializers,
+            ) = parameters.get_function_parameters_info(func)
+            self._add_topic_consumer_func(
                 topic=topic,
                 func=func,
-                param_type=param_type,
-                deserializer=deserializer,
-                return_type=return_type,
-                serializer=serializer,
+                value_param_type=value_param_type,
+                value_deserializer=value_deserializer,
+                key_param_type=key_param_type,
+                key_deserializer=key_deserializer,
+                headers_type_deserializers=headers_type_deserializers,
                 sink_topics=sink_topics,
             )
-            self._sink_topics.update(sink_topics or [])
+            if sink_topics:
+                self._sink_topics.update(sink_topics)
             if is_not_coroutine_function(func):
                 func = asyncify(func)
             return func
 
         return register_consumer
 
     def produce(self, sink_topic: str) -> Callable[[ProducerFunc], ProducerFunc]:
         def register_producer(func: ProducerFunc) -> Callable[..., Any]:
-            signature = inspect.signature(func)
-            if not has_return_annotation(signature) or not annotated_param_with(
-                MESSAGE_SERIALIZER_FLAG, signature.return_annotation
-            ):
-                raise ValueError(
-                    f"`{signature.return_annotation}` cannot be used as a return type"
-                    f" for '{func.__name__}' consumer function. Producer functions must"
-                    " return a message annotated with a serializer like"
-                    f" `kaflow.serializers.Json`: `async def {func.__name__}() ->"
-                    " Json[BaseModel]: ...`"
-                )
-            (_, serializer_type, serializer_extra) = annotated_serializer_info(
-                signature.return_annotation
-            )
-            serializer = serializer_type(**serializer_extra)
             self._sink_topics.update([sink_topic])
 
+            def _create_coro(topic: str, message: Any) -> Coroutine[Any, Any, None]:
+                if not isinstance(message, Message):
+                    raise ValueError(
+                        "Kaflow producer function has to return an instance of"
+                        " `Message` containing the information of the message to be"
+                        f" send. Update `{func.__name__}` to return a `Message`"
+                        " instance."
+                    )
+                return self._publish(
+                    topic=topic,
+                    value=message.value,
+                    key=message.key,
+                    headers=message.headers,
+                    partition=message.partition,
+                    timestamp=message.timestamp,
+                )
+
             if is_not_coroutine_function(func):
 
                 @wraps(func)
                 def sync_wrapper(*args: Any, **kwargs: Any) -> Any:
-                    r = func(*args, **kwargs)
-                    message = _serialize(r, serializer)
+                    message = func(*args, **kwargs)
                     asyncio.run_coroutine_threadsafe(
-                        coro=self._publish(topic=sink_topic, value=message),
+                        coro=_create_coro(sink_topic, message),
                         loop=self._loop,
                     )
-                    return r
+                    return message
 
                 return sync_wrapper
 
             @wraps(func)
             async def async_wrapper(*args: Any, **kwargs: Any) -> Any:
-                r = await func(*args, **kwargs)  # type: ignore
-                message = _serialize(r, serializer)
-                await self._publish(topic=sink_topic, value=message)
-                return r
+                message = await func(*args, **kwargs)  # type: ignore
+                await _create_coro(sink_topic, message)
+                return message
 
             return async_wrapper
 
         return register_producer
 
     def exception_handler(
         self, exception: type[Exception]
@@ -383,26 +433,65 @@
     def deserialization_error_handler(
         self,
     ) -> Callable[[DeserializationErrorHandlerFunc], DeserializationErrorHandlerFunc]:
         def register_deserialization_error_handler(
             func: DeserializationErrorHandlerFunc,
         ) -> DeserializationErrorHandlerFunc:
             self._deserialization_error_handler = func
+            if is_not_coroutine_function(func):
+                self._deserialization_error_handler = asyncify(func)
             return func
 
         return register_deserialization_error_handler
 
-    async def _publish(self, topic: str, value: bytes) -> None:
+    def asyncapi(self) -> AsyncAPI:
+        # if not self.asyncapi_schema:
+        #     self.asyncapi_schema = build_asyncapi(
+        #         asyncapi_version=self.asyncapi_version,
+        #         title=self.title,
+        #         version=self.version,
+        #         description=self.description,
+        #         terms_of_service=self.terms_of_service,
+        #         contact=self.contact,
+        #         license_info=self.license_info,
+        #         consumers=self._consumers,
+        #         producers=self._producers,
+        #     )
+        # return self.asyncapi_schema
+        raise NotImplementedError("AsyncAPI is not implemented yet.")
+
+    async def _publish(
+        self,
+        topic: str,
+        value: bytes | None = None,
+        key: bytes | None = None,
+        headers: dict[str, bytes] | None = None,
+        partition: int | None = None,
+        timestamp: int | None = None,
+    ) -> None:
         if not self._producer:
             raise RuntimeError(
                 "The producer has not been started yet. You're probably seeing this"
                 f" error because `{self.__class__.__name__}.start` method has not been"
                 " called yet."
             )
-        await self._producer.send_and_wait(topic=topic, value=value)
+
+        if isinstance(headers, dict):
+            headers_ = [(k, v) for k, v in headers.items()]
+        else:
+            headers_ = None
+
+        await self._producer.send_and_wait(
+            topic=topic,
+            value=value,
+            key=key,
+            partition=partition,
+            timestamp_ms=timestamp,
+            headers=headers_,
+        )
 
     async def _consuming_loop(self) -> None:
         if not self._consumer:
             raise RuntimeError(
                 "The consumer has not been started yet. You're probably seeing this"
                 f" error because `{self.__class__.__name__}.start` method has not been"
                 " called yet."
```

### Comparing `kaflow-0.0.2/kaflow/serializers.py` & `kaflow-0.1.0/kaflow/serializers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from __future__ import annotations
 
 import io
 import json
-from typing import TYPE_CHECKING, Any, Protocol, TypeVar, cast
+from abc import ABC, abstractmethod
+from typing import TYPE_CHECKING, Any, TypeVar, cast
 
-from pydantic import BaseModel
-
-from kaflow._utils.typing import Annotated
+from typing_extensions import Annotated
 
 if TYPE_CHECKING:
-    from kaflow.typing import TopicMessage
+    pass
 
 try:
     import fastavro
 
     has_fastavro = True
 except ImportError:
     has_fastavro = False
@@ -26,32 +25,42 @@
     has_protobuf = False
 
 MESSAGE_SERIALIZER_FLAG = "MessageSerializer"
 
 T = TypeVar("T")
 
 
-def _serialize(message: TopicMessage, serializer: Serializer) -> bytes:
-    if isinstance(message, BaseModel):
-        message = message.dict()
-    return serializer.serialize(message)
-
-
-class Serializer(Protocol):
+class Serializer(ABC):
+    @abstractmethod
     def serialize(self, data: Any) -> bytes:
         ...
 
+    @abstractmethod
     def deserialize(self, data: bytes) -> Any:
         ...
 
     @staticmethod
     def extra_annotations_keys() -> list[str]:
         return []
 
 
+class StringSerializer(Serializer):
+    def __init__(self, **kwargs: Any) -> None:
+        pass
+
+    def serialize(self, data: Any) -> bytes:
+        return str(data).encode()
+
+    def deserialize(self, data: bytes) -> Any:
+        return data.decode()
+
+
+String = Annotated[T, StringSerializer, MESSAGE_SERIALIZER_FLAG]
+
+
 class JsonSerializer(Serializer):
     def __init__(self, **kwargs: Any) -> None:
         pass
 
     def serialize(self, data: Any) -> bytes:
         return json.dumps(data).encode()
```

### Comparing `kaflow-0.0.2/kaflow/_utils/asyncio.py` & `kaflow-0.1.0/kaflow/_utils/asyncio.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import asyncio
 import contextvars
 import functools
 from typing import Awaitable, Callable, TypeVar
 
-from kaflow._utils.typing import ParamSpec
+from typing_extensions import ParamSpec
 
 P = ParamSpec("P")
 R = TypeVar("R")
 
 
 # Inspired by https://github.com/tiangolo/asyncer
 def asyncify(func: Callable[P, R]) -> Callable[P, Awaitable[R]]:
```

### Comparing `kaflow-0.0.2/kaflow/_utils/inspect.py` & `kaflow-0.1.0/kaflow/_utils/inspect.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from __future__ import annotations
 
 import inspect
 from typing import TYPE_CHECKING, Any, Awaitable, Callable, TypeVar
 
-from kaflow._utils.typing import Annotated, ParamSpec, TypeGuard, get_args, get_origin
+from typing_extensions import Annotated, ParamSpec, TypeGuard, get_args, get_origin
 
 if TYPE_CHECKING:
     from inspect import Signature
 
 
 def is_annotated_param(param: Any) -> bool:
     return get_origin(param) is Annotated
 
 
 def annotated_param_with(item: Any, param: Any) -> bool:
-    return is_annotated_param(param) and item in get_args(param)
+    if is_annotated_param(param):
+        for arg in get_args(param):
+            if arg == item or (type(item) == type and isinstance(arg, item)):
+                return True
+    return False
 
 
 def has_return_annotation(signature: Signature) -> bool:
     return (
         signature.return_annotation is not None
         and signature.return_annotation != inspect.Signature.empty
     )
```

### Comparing `kaflow-0.0.2/tests/key_value_pb2.py` & `kaflow-0.1.0/tests/key_value_pb2.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.0.2/tests/test_serializers.py` & `kaflow-0.1.0/tests/test_serializers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 from __future__ import annotations
 
-from typing import Any
-
-import pytest
 from pydantic import BaseModel
 
 from kaflow.serializers import (
     AvroSerializer,
     JsonSerializer,
     ProtobufSerializer,
     Serializer,
-    _serialize,
 )
 from tests.key_value_pb2 import KeyValue
 
 
 class KeyValueModel(BaseModel):
     key: str
     value: str
@@ -86,22 +82,7 @@
         "key": "unit_test_key",
         "value": "unit_test_value",
     }
 
 
 def test_protobuf_extra_annotation_keys() -> None:
     assert ProtobufSerializer.extra_annotations_keys() == ["protobuf_schema"]
-
-
-@pytest.mark.parametrize(
-    "message",
-    [
-        {"key": "unit_test_key", "value": "unit_test_value"},
-        KeyValueModel(key="unit_test_key", value="unit_test_value"),
-    ],
-)
-def test__serialize(message: dict[str, Any] | BaseModel) -> None:
-    serializer = JsonSerializer()
-    assert (
-        _serialize(serializer=serializer, message=message)
-        == b'{"key": "unit_test_key", "value": "unit_test_value"}'
-    )
```

### Comparing `kaflow-0.0.2/tests/_utils/test_inspect.py` & `kaflow-0.1.0/tests/_utils/test_inspect.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import inspect
 from typing import Any, Callable
 
 import pytest
+from typing_extensions import Annotated
 
 from kaflow._utils.inspect import (
     annotated_param_with,
     has_return_annotation,
     is_annotated_param,
     is_not_coroutine_function,
 )
-from kaflow._utils.typing import Annotated
 
 
 def func_with_none_return_annotation() -> None:
     pass
 
 
 def func_with_no_return_annotation():
@@ -31,23 +31,28 @@
 @pytest.mark.parametrize(
     "param, expected", [(Annotated[int, "extra", "metadata"], True), (int, False)]
 )
 def test_is_annotated_param_true(param: Any, expected: bool) -> None:
     assert is_annotated_param(param) == expected
 
 
+class DummyUnitTest:
+    pass
+
+
 @pytest.mark.parametrize(
-    "param, expected",
+    "param, annotated_with, expected",
     [
-        (Annotated[int, "magic_unit_test_flag"], True),
-        (Annotated[int, "extra", "metadata"], False),
+        (Annotated[int, "magic_unit_test_flag"], "magic_unit_test_flag", True),
+        (Annotated[int, "extra", "metadata"], "magic_unit_test_flag", False),
+        (Annotated[int, DummyUnitTest()], DummyUnitTest, True),
     ],
 )
-def test_annotated_param_with(param: Any, expected: bool) -> None:
-    assert annotated_param_with("magic_unit_test_flag", param) == expected
+def test_annotated_param_with(param: Any, annotated_with: Any, expected: bool) -> None:
+    assert annotated_param_with(annotated_with, param) == expected
 
 
 @pytest.mark.parametrize(
     "func, expected",
     [
         (func_with_none_return_annotation, False),
         (func_with_no_return_annotation, False),
```

### Comparing `kaflow-0.0.2/.gitignore` & `kaflow-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `kaflow-0.0.2/LICENSE` & `kaflow-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kaflow-0.0.2/README.md` & `kaflow-0.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,20 @@
   <p>
     <em>Kafka streams topic processing in Python.</em>
   </p>
   <p>
     <a href="https://github.com/gabrielmbmb/kaflow/actions?query=workflow%3ATest+event%3Apush+branch%3Amain" target="_blank">
       <img src="https://github.com/gabrielmbmb/kaflow/workflows/Test/badge.svg?event=push&branch=main" alt="Test">
     </a>
+    <a href="https://pypi.org/project/kaflow">
+      <img src="https://img.shields.io/pypi/v/kaflow?color=#2cbe4e">
+    </a>
+    <a href="https://pypi.org/project/kaflow">
+      <img src="https://img.shields.io/pypi/pyversions/kaflow?color=#2cbe4e">
+    </a>
   </p>
 </div>
 
 ---
 
 `kaflow` is a simple framework that allows you to build Kafka streams processing aplications in Python with ease.
```

### Comparing `kaflow-0.0.2/pyproject.toml` & `kaflow-0.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "kaflow"
 description = "Python Stream processing backed by Apache Kafka."
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = "MIT"
 keywords = ["kafka", "stream", "processing", "data", "pipeline", "flow"]
 authors = [
   { name = "Gabriel Martin Blazquez", email = "gmartinbdev@gmail.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
@@ -23,14 +23,15 @@
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "pydantic >=1.10.0,<2.0.0",
   "aiokafka >=0.8.0",
   "di[anyio] ==0.75.2",
+  "typing-extensions >=4.5.0"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
   "black >=23.1.0",
   "ruff ==0.0.257",
@@ -59,15 +60,15 @@
 ignore = ["E501", "B905", "B008"]
 
 [tool.mypy]
 strict = true
 plugins = ["pydantic.mypy"]
 
 [[tool.mypy.overrides]]
-module = ["aiokafka.*"]
+module = ["aiokafka.*", "kafka.*"]
 ignore_missing_imports = true
 
 [tool.coverage.run]
 source = ["kaflow"]
 # parallel = true
 branch = true
 context = '${CONTEXT}'
```

### Comparing `kaflow-0.0.2/PKG-INFO` & `kaflow-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaflow
-Version: 0.0.2
+Version: 0.1.0
 Summary: Python Stream processing backed by Apache Kafka.
 Project-URL: Documentation, https://github.com/gabrielmbmb/kaflow#readme
 Project-URL: Issues, https://github.com/gabrielmbmb/kaflow/issues
 Project-URL: Source, https://github.com/gabrielmbmb/kaflow
 Author-email: Gabriel Martin Blazquez <gmartinbdev@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -14,18 +14,19 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: aiokafka>=0.8.0
 Requires-Dist: di[anyio]==0.75.2
 Requires-Dist: pydantic<2.0.0,>=1.10.0
+Requires-Dist: typing-extensions>=4.5.0
 Provides-Extra: dev
 Requires-Dist: black>=23.1.0; extra == 'dev'
 Requires-Dist: coverage[toml]>=7.0.0; extra == 'dev'
 Requires-Dist: mypy==0.991; extra == 'dev'
 Requires-Dist: pre-commit>=3.0.0; extra == 'dev'
 Requires-Dist: pytest>=7.2.0; extra == 'dev'
 Requires-Dist: ruff==0.0.257; extra == 'dev'
@@ -40,14 +41,20 @@
   <p>
     <em>Kafka streams topic processing in Python.</em>
   </p>
   <p>
     <a href="https://github.com/gabrielmbmb/kaflow/actions?query=workflow%3ATest+event%3Apush+branch%3Amain" target="_blank">
       <img src="https://github.com/gabrielmbmb/kaflow/workflows/Test/badge.svg?event=push&branch=main" alt="Test">
     </a>
+    <a href="https://pypi.org/project/kaflow">
+      <img src="https://img.shields.io/pypi/v/kaflow?color=#2cbe4e">
+    </a>
+    <a href="https://pypi.org/project/kaflow">
+      <img src="https://img.shields.io/pypi/pyversions/kaflow?color=#2cbe4e">
+    </a>
   </p>
 </div>
 
 ---
 
 `kaflow` is a simple framework that allows you to build Kafka streams processing aplications in Python with ease.
```

