# Comparing `tmp/bus-station-5.1.0.tar.gz` & `tmp/bus_station-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bus-station-5.1.0.tar", max compression
+gzip compressed data, was "bus_station-6.0.0.tar", max compression
```

## Comparing `bus-station-5.1.0.tar` & `bus_station-6.0.0.tar`

### file list

```diff
@@ -1,168 +1,160 @@
--rw-r--r--   0        0        0       48 2023-03-17 09:52:43.748455 bus-station-5.1.0/README.md
--rw-r--r--   0        0        0      977 2023-03-17 09:54:41.286836 bus-station-5.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/__init__.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/__init__.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/bus/__init__.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/bus/asynchronous/__init__.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/bus/asynchronous/distributed/__init__.py
--rw-r--r--   0        0        0     1813 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/bus/asynchronous/distributed/kombu_command_bus.py
--rw-r--r--   0        0        0     1241 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/bus/asynchronous/memory_queue_command_bus.py
--rw-r--r--   0        0        0     1208 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/bus/asynchronous/threaded_command_bus.py
--rw-r--r--   0        0        0      258 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/bus/command_bus.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/bus/synchronous/__init__.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/bus/synchronous/distributed/__init__.py
--rw-r--r--   0        0        0     1690 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/bus/synchronous/distributed/json_rpc_command_bus.py
--rw-r--r--   0        0        0     1562 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/bus/synchronous/distributed/rpyc_command_bus.py
--rw-r--r--   0        0        0     1099 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/bus/synchronous/sync_command_bus.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/bus_engine/__init__.py
--rw-r--r--   0        0        0     1334 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/bus_engine/json_rpc_command_bus_engine.py
--rw-r--r--   0        0        0     3085 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/bus_engine/kombu_command_bus_engine.py
--rw-r--r--   0        0        0     1566 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/bus_engine/memory_queue_command_bus_engine.py
--rw-r--r--   0        0        0     1252 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/bus_engine/rpyc_command_bus_engine.py
--rw-r--r--   0        0        0      253 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/command.py
--rw-r--r--   0        0        0      292 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/command_execution_failed.py
--rw-r--r--   0        0        0      379 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/command_handler.py
--rw-r--r--   0        0        0      202 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/contact_not_found_for_command.py
--rw-r--r--   0        0        0      282 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/handler_for_command_already_registered.py
--rw-r--r--   0        0        0      233 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/handler_not_found_for_command.py
--rw-r--r--   0        0        0      725 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/json_rpc_command_server.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/middleware/__init__.py
--rw-r--r--   0        0        0      607 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/middleware/command_middleware.py
--rw-r--r--   0        0        0     1078 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/middleware/command_middleware_receiver.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/middleware/implementations/__init__.py
--rw-r--r--   0        0        0     1070 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/middleware/implementations/logging_command_middleware.py
--rw-r--r--   0        0        0     1039 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/middleware/implementations/timing_command_middleware.py
--rw-r--r--   0        0        0      890 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/middleware/implementations/tracking_command_middleware.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/registry/__init__.py
--rw-r--r--   0        0        0     1880 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/registry/command_registry.py
--rw-r--r--   0        0        0     2992 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/registry/in_memory_command_registry.py
--rw-r--r--   0        0        0     3018 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/registry/redis_command_registry.py
--rw-r--r--   0        0        0      590 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/registry/remote_command_registry.py
--rw-r--r--   0        0        0      712 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/command_terminal/rpyc_command_server.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/event_terminal/__init__.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/event_terminal/bus/__init__.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/event_terminal/bus/asynchronous/__init__.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/event_terminal/bus/asynchronous/distributed/__init__.py
--rw-r--r--   0        0        0     1833 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/event_terminal/bus/asynchronous/distributed/kombu_event_bus.py
--rw-r--r--   0        0        0     1102 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/event_terminal/bus/asynchronous/memory_queue_event_bus.py
--rw-r--r--   0        0        0     1048 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/event_terminal/bus/asynchronous/threaded_event_bus.py
--rw-r--r--   0        0        0      246 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/event_terminal/bus/event_bus.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/event_terminal/bus/synchronous/__init__.py
--rw-r--r--   0        0        0      936 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/event_terminal/bus/synchronous/sync_event_bus.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/event_terminal/bus_engine/__init__.py
--rw-r--r--   0        0        0     3538 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/event_terminal/bus_engine/kombu_event_bus_engine.py
--rw-r--r--   0        0        0     1769 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/event_terminal/bus_engine/memory_queue_event_bus_engine.py
--rw-r--r--   0        0        0      289 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/event_terminal/consumer_for_event_already_registered.py
--rw-r--r--   0        0        0      238 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/event_terminal/contact_not_found_for_consumer.py
--rw-r--r--   0        0        0      249 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/event_terminal/event.py
--rw-r--r--   0        0        0      368 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/event_terminal/event_consumer.py
--rw-r--r--   0        0        0      221 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/event_terminal/event_consumer_not_found.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/event_terminal/middleware/__init__.py
--rw-r--r--   0        0        0      590 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/event_terminal/middleware/event_middleware.py
--rw-r--r--   0        0        0     1049 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/event_terminal/middleware/event_middleware_receiver.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/event_terminal/middleware/implementations/__init__.py
--rw-r--r--   0        0        0     1038 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/event_terminal/middleware/implementations/logging_event_middleware.py
--rw-r--r--   0        0        0     1012 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/event_terminal/middleware/implementations/timing_event_middleware.py
--rw-r--r--   0        0        0      864 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/event_terminal/middleware/implementations/tracking_event_middleware.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/event_terminal/registry/__init__.py
--rw-r--r--   0        0        0     1973 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/event_terminal/registry/event_registry.py
--rw-r--r--   0        0        0     4329 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/event_terminal/registry/in_memory_event_registry.py
--rw-r--r--   0        0        0     4110 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/event_terminal/registry/redis_event_registry.py
--rw-r--r--   0        0        0      726 2023-03-17 09:52:43.748455 bus-station-5.1.0/src/bus_station/event_terminal/registry/remote_event_registry.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/passengers/__init__.py
--rw-r--r--   0        0        0     1447 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/passengers/memory_queue_passenger_worker.py
--rw-r--r--   0        0        0     2187 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/passengers/passenger.py
--rw-r--r--   0        0        0      478 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/passengers/passenger_class_resolver.py
--rw-r--r--   0        0        0     2049 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/passengers/passenger_kombu_consumer.py
--rw-r--r--   0        0        0       76 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/passengers/passenger_middleware.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/passengers/passenger_record/__init__.py
--rw-r--r--   0        0        0     1798 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/passengers/passenger_record/in_memory_passenger_record_repository.py
--rw-r--r--   0        0        0     1795 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/passengers/passenger_record/passenger_record.py
--rw-r--r--   0        0        0      815 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/passengers/passenger_record/passenger_record_repository.py
--rw-r--r--   0        0        0     1954 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/passengers/passenger_record/redis_passenger_record_repository.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/passengers/reception/__init__.py
--rw-r--r--   0        0        0     1393 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/passengers/reception/passenger_middleware_receiver.py
--rw-r--r--   0        0        0      840 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/passengers/reception/passenger_receiver.py
--rw-r--r--   0        0        0     1055 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/passengers/resolve_passenger_from_bus_stop.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/passengers/serialization/__init__.py
--rw-r--r--   0        0        0      347 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/passengers/serialization/passenger_deserialization_error.py
--rw-r--r--   0        0        0      321 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/passengers/serialization/passenger_deserializer.py
--rw-r--r--   0        0        0     1016 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/passengers/serialization/passenger_json_deserializer.py
--rw-r--r--   0        0        0      822 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/passengers/serialization/passenger_json_serializer.py
--rw-r--r--   0        0        0      241 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/passengers/serialization/passenger_serializer.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/__init__.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/bus/__init__.py
--rw-r--r--   0        0        0      323 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/bus/query_bus.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/bus/synchronous/__init__.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/bus/synchronous/distributed/__init__.py
--rw-r--r--   0        0        0     2043 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/bus/synchronous/distributed/json_rpc_query_bus.py
--rw-r--r--   0        0        0     1960 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/bus/synchronous/distributed/rpyc_query_bus.py
--rw-r--r--   0        0        0     1101 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/bus/synchronous/sync_query_bus.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/bus_engine/__init__.py
--rw-r--r--   0        0        0     1204 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/bus_engine/json_rpc_query_bus_engine.py
--rw-r--r--   0        0        0     1194 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/bus_engine/rpyc_query_bus_engine.py
--rw-r--r--   0        0        0      246 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/handler_for_query_already_registered.py
--rw-r--r--   0        0        0      219 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/handler_not_found_for_query.py
--rw-r--r--   0        0        0     1483 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/json_rpc_query_server.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/middleware/__init__.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/middleware/implementations/__init__.py
--rw-r--r--   0        0        0     1261 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/middleware/implementations/logging_query_middleware.py
--rw-r--r--   0        0        0     1178 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/middleware/implementations/timing_query_middleware.py
--rw-r--r--   0        0        0     1227 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/middleware/implementations/tracking_query_middleware.py
--rw-r--r--   0        0        0      726 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/middleware/query_middleware.py
--rw-r--r--   0        0        0     1286 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/middleware/query_middleware_receiver.py
--rw-r--r--   0        0        0      249 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/query.py
--rw-r--r--   0        0        0      273 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/query_execution_failed.py
--rw-r--r--   0        0        0      442 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/query_handler.py
--rw-r--r--   0        0        0      138 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/query_response.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/registry/__init__.py
--rw-r--r--   0        0        0     2895 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/registry/in_memory_query_registry.py
--rw-r--r--   0        0        0     1811 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/registry/query_registry.py
--rw-r--r--   0        0        0     2856 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/registry/redis_query_registry.py
--rw-r--r--   0        0        0      558 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/registry/remote_query_registry.py
--rw-r--r--   0        0        0     1442 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/rpyc_query_server.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/serialization/__init__.py
--rw-r--r--   0        0        0      282 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/serialization/query_response_deserializer.py
--rw-r--r--   0        0        0      465 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/serialization/query_response_json_deserializer.py
--rw-r--r--   0        0        0      390 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/serialization/query_response_json_serializer.py
--rw-r--r--   0        0        0      267 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/query_terminal/serialization/query_response_serializer.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/shared_terminal/__init__.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/shared_terminal/broker_connection/__init__.py
--rw-r--r--   0        0        0      352 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/shared_terminal/broker_connection/broker_connection_type.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/shared_terminal/broker_connection/connection_parameters/__init__.py
--rw-r--r--   0        0        0      176 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/shared_terminal/broker_connection/connection_parameters/connection_parameters.py
--rw-r--r--   0        0        0     1249 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/shared_terminal/broker_connection/connection_parameters/rabbitmq_connection_parameters.py
--rw-r--r--   0        0        0      567 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/shared_terminal/bus.py
--rw-r--r--   0        0        0      143 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/shared_terminal/bus_stop.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/shared_terminal/bus_stop_resolver/__init__.py
--rw-r--r--   0        0        0      306 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/shared_terminal/bus_stop_resolver/bus_stop_resolver.py
--rw-r--r--   0        0        0      724 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/shared_terminal/bus_stop_resolver/in_memory_bus_stop_resolver.py
--rw-r--r--   0        0        0      845 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/shared_terminal/bus_stop_resolver/pypendency_bus_stop_resolver.py
--rw-r--r--   0        0        0      983 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/shared_terminal/distributed.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/shared_terminal/engine/__init__.py
--rw-r--r--   0        0        0      181 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/shared_terminal/engine/engine.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/shared_terminal/engine/runner/__init__.py
--rw-r--r--   0        0        0      436 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/shared_terminal/engine/runner/engine_runner.py
--rw-r--r--   0        0        0      805 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/shared_terminal/engine/runner/process_engine_runner.py
--rw-r--r--   0        0        0      241 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/shared_terminal/engine/runner/self_process_engine_runner.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/shared_terminal/factories/__init__.py
--rw-r--r--   0        0        0      381 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/shared_terminal/factories/kombu_connection_factory.py
--rw-r--r--   0        0        0      382 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/shared_terminal/factories/proxy_class_factory.py
--rw-r--r--   0        0        0      374 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/shared_terminal/fqn_getter.py
--rw-r--r--   0        0        0     2500 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/shared_terminal/json_rpc_server.py
--rw-r--r--   0        0        0      956 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/shared_terminal/kafka_topic_creator.py
--rw-r--r--   0        0        0     2044 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/shared_terminal/rpyc_server.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/tracking_terminal/__init__.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/tracking_terminal/models/__init__.py
--rw-r--r--   0        0        0      185 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/tracking_terminal/models/command_tracking.py
--rw-r--r--   0        0        0      183 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/tracking_terminal/models/event_tracking.py
--rw-r--r--   0        0        0      950 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/tracking_terminal/models/passenger_model_tracking_map.py
--rw-r--r--   0        0        0      310 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/tracking_terminal/models/passenger_tracking.py
--rw-r--r--   0        0        0      744 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/tracking_terminal/models/passenger_tracking_json_serializer.py
--rw-r--r--   0        0        0      297 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/tracking_terminal/models/passenger_tracking_serializer.py
--rw-r--r--   0        0        0      281 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/tracking_terminal/models/query_tracking.py
--rw-r--r--   0        0        0        0 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/tracking_terminal/trackers/__init__.py
--rw-r--r--   0        0        0     1400 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/tracking_terminal/trackers/kafka_passenger_tracker.py
--rw-r--r--   0        0        0     2103 2023-03-17 09:52:43.752455 bus-station-5.1.0/src/bus_station/tracking_terminal/trackers/passenger_tracker.py
--rw-r--r--   0        0        0     2817 2023-03-17 09:54:48.076002 bus-station-5.1.0/setup.py
--rw-r--r--   0        0        0      723 2023-03-17 09:54:48.076327 bus-station-5.1.0/PKG-INFO
+-rw-r--r--   0        0        0       48 2023-05-17 23:26:07.511233 bus_station-6.0.0/README.md
+-rw-r--r--   0        0        0      977 2023-05-17 23:27:47.710968 bus_station-6.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/bus_stop/__init__.py
+-rw-r--r--   0        0        0      143 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/bus_stop/bus_stop.py
+-rw-r--r--   0        0        0      692 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/bus_stop/environment.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/bus_stop/registration/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/bus_stop/registration/address/__init__.py
+-rw-r--r--   0        0        0      199 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/bus_stop/registration/address/address_not_found_for_bus_stop.py
+-rw-r--r--   0        0        0      407 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/bus_stop/registration/address/bus_stop_address_registry.py
+-rw-r--r--   0        0        0      673 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/bus_stop/registration/address/redis_bus_stop_address_registry.py
+-rw-r--r--   0        0        0     3526 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/bus_stop/registration/bus_stop_registry.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/bus_stop/registration/supervisor/__init__.py
+-rw-r--r--   0        0        0     1180 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/bus_stop/registration/supervisor/bus_stop_address_registration_supervisor.py
+-rw-r--r--   0        0        0      255 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/bus_stop/registration/supervisor/bus_stop_registration_supervisor.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/bus_stop/resolvers/__init__.py
+-rw-r--r--   0        0        0      289 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/bus_stop/resolvers/bus_stop_resolver.py
+-rw-r--r--   0        0        0      614 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/bus_stop/resolvers/in_memory_bus_stop_resolver.py
+-rw-r--r--   0        0        0      811 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/bus_stop/resolvers/pypendency_bus_stop_resolver.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/command_terminal/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/command_terminal/bus/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/command_terminal/bus/asynchronous/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/command_terminal/bus/asynchronous/distributed/__init__.py
+-rw-r--r--   0        0        0     1352 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/command_terminal/bus/asynchronous/distributed/kombu_command_bus.py
+-rw-r--r--   0        0        0      889 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/command_terminal/bus/asynchronous/memory_queue_command_bus.py
+-rw-r--r--   0        0        0     1237 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/command_terminal/bus/asynchronous/threaded_command_bus.py
+-rw-r--r--   0        0        0      258 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/command_terminal/bus/command_bus.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/command_terminal/bus/synchronous/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/command_terminal/bus/synchronous/distributed/__init__.py
+-rw-r--r--   0        0        0     2315 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/command_terminal/bus/synchronous/distributed/json_rpc_command_bus.py
+-rw-r--r--   0        0        0     2188 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/command_terminal/bus/synchronous/distributed/rpyc_command_bus.py
+-rw-r--r--   0        0        0     1128 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/command_terminal/bus/synchronous/sync_command_bus.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/command_terminal/bus_engine/__init__.py
+-rw-r--r--   0        0        0     1326 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/command_terminal/bus_engine/json_rpc_command_bus_engine.py
+-rw-r--r--   0        0        0     2747 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/command_terminal/bus_engine/kombu_command_bus_engine.py
+-rw-r--r--   0        0        0     1856 2023-05-17 23:26:07.511233 bus_station-6.0.0/src/bus_station/command_terminal/bus_engine/memory_queue_command_bus_engine.py
+-rw-r--r--   0        0        0     1266 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/command_terminal/bus_engine/rpyc_command_bus_engine.py
+-rw-r--r--   0        0        0      253 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/command_terminal/command.py
+-rw-r--r--   0        0        0      292 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/command_terminal/command_execution_failed.py
+-rw-r--r--   0        0        0      457 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/command_terminal/command_handler.py
+-rw-r--r--   0        0        0      227 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/command_terminal/command_handler_not_found.py
+-rw-r--r--   0        0        0     1510 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/command_terminal/command_handler_registry.py
+-rw-r--r--   0        0        0      233 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/command_terminal/handler_not_found_for_command.py
+-rw-r--r--   0        0        0      725 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/command_terminal/json_rpc_command_server.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/command_terminal/middleware/__init__.py
+-rw-r--r--   0        0        0      607 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/command_terminal/middleware/command_middleware.py
+-rw-r--r--   0        0        0     1078 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/command_terminal/middleware/command_middleware_receiver.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/command_terminal/middleware/implementations/__init__.py
+-rw-r--r--   0        0        0     1070 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/command_terminal/middleware/implementations/logging_command_middleware.py
+-rw-r--r--   0        0        0     1039 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/command_terminal/middleware/implementations/timing_command_middleware.py
+-rw-r--r--   0        0        0      890 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/command_terminal/middleware/implementations/tracking_command_middleware.py
+-rw-r--r--   0        0        0      712 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/command_terminal/rpyc_command_server.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/event_terminal/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/event_terminal/bus/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/event_terminal/bus/asynchronous/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/event_terminal/bus/asynchronous/distributed/__init__.py
+-rw-r--r--   0        0        0     1247 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/event_terminal/bus/asynchronous/distributed/kombu_event_bus.py
+-rw-r--r--   0        0        0     1212 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/event_terminal/bus/asynchronous/memory_queue_event_bus.py
+-rw-r--r--   0        0        0      984 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/event_terminal/bus/asynchronous/threaded_event_bus.py
+-rw-r--r--   0        0        0      246 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/event_terminal/bus/event_bus.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/event_terminal/bus/synchronous/__init__.py
+-rw-r--r--   0        0        0      872 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/event_terminal/bus/synchronous/sync_event_bus.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/event_terminal/bus_engine/__init__.py
+-rw-r--r--   0        0        0     3196 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/event_terminal/bus_engine/kombu_event_bus_engine.py
+-rw-r--r--   0        0        0     1625 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/event_terminal/bus_engine/memory_queue_event_bus_engine.py
+-rw-r--r--   0        0        0      249 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/event_terminal/event.py
+-rw-r--r--   0        0        0      446 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/event_terminal/event_consumer.py
+-rw-r--r--   0        0        0      221 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/event_terminal/event_consumer_not_found.py
+-rw-r--r--   0        0        0     1439 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/event_terminal/event_consumer_registry.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/event_terminal/middleware/__init__.py
+-rw-r--r--   0        0        0      590 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/event_terminal/middleware/event_middleware.py
+-rw-r--r--   0        0        0     1049 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/event_terminal/middleware/event_middleware_receiver.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/event_terminal/middleware/implementations/__init__.py
+-rw-r--r--   0        0        0     1038 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/event_terminal/middleware/implementations/logging_event_middleware.py
+-rw-r--r--   0        0        0     1012 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/event_terminal/middleware/implementations/timing_event_middleware.py
+-rw-r--r--   0        0        0      864 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/event_terminal/middleware/implementations/tracking_event_middleware.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/passengers/__init__.py
+-rw-r--r--   0        0        0     1440 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/passengers/memory_queue_passenger_worker.py
+-rw-r--r--   0        0        0     2319 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/passengers/passenger.py
+-rw-r--r--   0        0        0     2042 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/passengers/passenger_kombu_consumer.py
+-rw-r--r--   0        0        0     2294 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/passengers/passenger_mapper.py
+-rw-r--r--   0        0        0       76 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/passengers/passenger_middleware.py
+-rw-r--r--   0        0        0      637 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/passengers/passenger_registry.py
+-rw-r--r--   0        0        0      641 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/passengers/passenger_resolvers.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/passengers/reception/__init__.py
+-rw-r--r--   0        0        0     1386 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/passengers/reception/passenger_middleware_receiver.py
+-rw-r--r--   0        0        0      792 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/passengers/reception/passenger_receiver.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/passengers/serialization/__init__.py
+-rw-r--r--   0        0        0      347 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/passengers/serialization/passenger_deserialization_error.py
+-rw-r--r--   0        0        0      321 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/passengers/serialization/passenger_deserializer.py
+-rw-r--r--   0        0        0     1016 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/passengers/serialization/passenger_json_deserializer.py
+-rw-r--r--   0        0        0      822 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/passengers/serialization/passenger_json_serializer.py
+-rw-r--r--   0        0        0      241 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/passengers/serialization/passenger_serializer.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/query_terminal/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/query_terminal/bus/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/query_terminal/bus/query_bus.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/query_terminal/bus/synchronous/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/query_terminal/bus/synchronous/distributed/__init__.py
+-rw-r--r--   0        0        0     2671 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/query_terminal/bus/synchronous/distributed/json_rpc_query_bus.py
+-rw-r--r--   0        0        0     2580 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/query_terminal/bus/synchronous/distributed/rpyc_query_bus.py
+-rw-r--r--   0        0        0     1127 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/query_terminal/bus/synchronous/sync_query_bus.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/query_terminal/bus_engine/__init__.py
+-rw-r--r--   0        0        0     1242 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/query_terminal/bus_engine/json_rpc_query_bus_engine.py
+-rw-r--r--   0        0        0     1218 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/query_terminal/bus_engine/rpyc_query_bus_engine.py
+-rw-r--r--   0        0        0      219 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/query_terminal/handler_not_found_for_query.py
+-rw-r--r--   0        0        0     1483 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/query_terminal/json_rpc_query_server.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/query_terminal/middleware/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/query_terminal/middleware/implementations/__init__.py
+-rw-r--r--   0        0        0     1261 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/query_terminal/middleware/implementations/logging_query_middleware.py
+-rw-r--r--   0        0        0     1178 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/query_terminal/middleware/implementations/timing_query_middleware.py
+-rw-r--r--   0        0        0     1227 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/query_terminal/middleware/implementations/tracking_query_middleware.py
+-rw-r--r--   0        0        0      726 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/query_terminal/middleware/query_middleware.py
+-rw-r--r--   0        0        0     1286 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/query_terminal/middleware/query_middleware_receiver.py
+-rw-r--r--   0        0        0      249 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/query_terminal/query.py
+-rw-r--r--   0        0        0      273 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/query_terminal/query_execution_failed.py
+-rw-r--r--   0        0        0      520 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/query_terminal/query_handler.py
+-rw-r--r--   0        0        0      215 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/query_terminal/query_handler_not_found.py
+-rw-r--r--   0        0        0     1480 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/query_terminal/query_handler_registry.py
+-rw-r--r--   0        0        0      138 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/query_terminal/query_response.py
+-rw-r--r--   0        0        0     1442 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/query_terminal/rpyc_query_server.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/query_terminal/serialization/__init__.py
+-rw-r--r--   0        0        0      282 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/query_terminal/serialization/query_response_deserializer.py
+-rw-r--r--   0        0        0      465 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/query_terminal/serialization/query_response_json_deserializer.py
+-rw-r--r--   0        0        0      390 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/query_terminal/serialization/query_response_json_serializer.py
+-rw-r--r--   0        0        0      267 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/query_terminal/serialization/query_response_serializer.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/shared_terminal/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/shared_terminal/broker_connection/__init__.py
+-rw-r--r--   0        0        0      352 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/shared_terminal/broker_connection/broker_connection_type.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/shared_terminal/broker_connection/connection_parameters/__init__.py
+-rw-r--r--   0        0        0      176 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/shared_terminal/broker_connection/connection_parameters/connection_parameters.py
+-rw-r--r--   0        0        0     1249 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/shared_terminal/broker_connection/connection_parameters/rabbitmq_connection_parameters.py
+-rw-r--r--   0        0        0      695 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/shared_terminal/bus.py
+-rw-r--r--   0        0        0      438 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/shared_terminal/context.py
+-rw-r--r--   0        0        0      118 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/shared_terminal/dataclass_type.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/shared_terminal/engine/__init__.py
+-rw-r--r--   0        0        0      181 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/shared_terminal/engine/engine.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/shared_terminal/engine/runner/__init__.py
+-rw-r--r--   0        0        0      436 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/shared_terminal/engine/runner/engine_runner.py
+-rw-r--r--   0        0        0      805 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/shared_terminal/engine/runner/process_engine_runner.py
+-rw-r--r--   0        0        0      241 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/shared_terminal/engine/runner/self_process_engine_runner.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/shared_terminal/factories/__init__.py
+-rw-r--r--   0        0        0      381 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/shared_terminal/factories/kombu_connection_factory.py
+-rw-r--r--   0        0        0      545 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/shared_terminal/factories/memory_queue_factory.py
+-rw-r--r--   0        0        0      305 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/shared_terminal/fqn.py
+-rw-r--r--   0        0        0     2493 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/shared_terminal/json_rpc_server.py
+-rw-r--r--   0        0        0      956 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/shared_terminal/kafka_topic_creator.py
+-rw-r--r--   0        0        0     2037 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/shared_terminal/rpyc_server.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/tracking_terminal/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/tracking_terminal/models/__init__.py
+-rw-r--r--   0        0        0      185 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/tracking_terminal/models/command_tracking.py
+-rw-r--r--   0        0        0      183 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/tracking_terminal/models/event_tracking.py
+-rw-r--r--   0        0        0      950 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/tracking_terminal/models/passenger_model_tracking_map.py
+-rw-r--r--   0        0        0      310 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/tracking_terminal/models/passenger_tracking.py
+-rw-r--r--   0        0        0      744 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/tracking_terminal/models/passenger_tracking_json_serializer.py
+-rw-r--r--   0        0        0      297 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/tracking_terminal/models/passenger_tracking_serializer.py
+-rw-r--r--   0        0        0      281 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/tracking_terminal/models/query_tracking.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/tracking_terminal/trackers/__init__.py
+-rw-r--r--   0        0        0     1400 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/tracking_terminal/trackers/kafka_passenger_tracker.py
+-rw-r--r--   0        0        0     2096 2023-05-17 23:26:07.515233 bus_station-6.0.0/src/bus_station/tracking_terminal/trackers/passenger_tracker.py
+-rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 bus_station-6.0.0/PKG-INFO
```

### Comparing `bus-station-5.1.0/pyproject.toml` & `bus_station-6.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "bus-station"
-version = "5.1.0"
+version = "6.0.0"
 description = "A python bus station"
 readme = "README.md"
 authors = ["DeejayRevok <seryi_one@hotmail.com>"]
 
 [tool.poetry.dependencies]
 python = "~=3.10.0"
 kombu = "5.2.2"
-redis = "4.1.0"
+redis = "4.4.4"
 rpyc = "5.0.1"
 jsonrpcserver = "^5.0.6"
 jsonrpcclient = "^4.0.2"
 requests = "^2.27.1"
 pypendency = "^0.1.0"
 confluent-kafka = "^2.0.2"
 freezegun = "^1.2.2"
@@ -40,15 +40,15 @@
 [tool.isort]
 profile = "black"
 py_version=310
 line_length = 120
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "5.1.0"
+version = "6.0.0"
 tag_format = "$version"
 version_files = [
   "pyproject.toml:version"
 ]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `bus-station-5.1.0/src/bus_station/command_terminal/bus/asynchronous/distributed/kombu_command_bus.py` & `bus_station-6.0.0/src/bus_station/command_terminal/bus/asynchronous/distributed/kombu_command_bus.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 from kombu import Connection, Producer
 
 from bus_station.command_terminal.bus.command_bus import CommandBus
 from bus_station.command_terminal.command import Command
-from bus_station.command_terminal.handler_not_found_for_command import HandlerNotFoundForCommand
-from bus_station.command_terminal.registry.remote_command_registry import RemoteCommandRegistry
 from bus_station.passengers.serialization.passenger_serializer import PassengerSerializer
 
 
 class KombuCommandBus(CommandBus):
     def __init__(
         self,
         broker_connection: Connection,
         command_serializer: PassengerSerializer,
-        command_registry: RemoteCommandRegistry,
     ):
         self.__broker_connection = broker_connection
         self.__command_serializer = command_serializer
-        self.__command_registry = command_registry
         self.__producer = Producer(broker_connection.channel())
 
     def _transport(self, passenger: Command) -> None:
-        handler_queue_name = self.__command_registry.get_command_destination_contact(passenger.passenger_name())
-        if handler_queue_name is None:
-            raise HandlerNotFoundForCommand(passenger.passenger_name())
+        handler_queue_name = passenger.passenger_name()
 
         self.__publish_command(passenger, handler_queue_name)
 
     def __publish_command(self, command: Command, routing_key: str) -> None:
         serialized_command = self.__command_serializer.serialize(command)
         if self.__producer is not None:
             self.__producer.publish(
```

### Comparing `bus-station-5.1.0/src/bus_station/command_terminal/bus/asynchronous/memory_queue_command_bus.py` & `bus_station-6.0.0/src/bus_station/command_terminal/bus_engine/json_rpc_command_bus_engine.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,32 @@
-from multiprocessing import Queue
+from bus_station.command_terminal.command_handler_not_found import CommandHandlerNotFound
+from bus_station.command_terminal.command_handler_registry import CommandHandlerRegistry
+from bus_station.command_terminal.json_rpc_command_server import JsonRPCCommandServer
+from bus_station.passengers.passenger_resolvers import resolve_passenger_class_from_bus_stop
+from bus_station.shared_terminal.engine.engine import Engine
 
-from bus_station.command_terminal.bus.command_bus import CommandBus
-from bus_station.command_terminal.command import Command
-from bus_station.command_terminal.handler_not_found_for_command import HandlerNotFoundForCommand
-from bus_station.command_terminal.registry.in_memory_command_registry import InMemoryCommandRegistry
-from bus_station.passengers.serialization.passenger_serializer import PassengerSerializer
 
-
-class MemoryQueueCommandBus(CommandBus):
+class JsonRPCCommandBusEngine(Engine):
     def __init__(
         self,
-        command_serializer: PassengerSerializer,
-        command_registry: InMemoryCommandRegistry,
+        server: JsonRPCCommandServer,
+        command_handler_registry: CommandHandlerRegistry,
+        command_handler_name: str,
     ):
-        self.__command_serializer = command_serializer
-        self.__command_registry = command_registry
+        self.__server = server
+        self.__register_command_handler_in_server(command_handler_registry, command_handler_name)
+
+    def __register_command_handler_in_server(
+        self, command_handler_registry: CommandHandlerRegistry, command_handler_name: str
+    ) -> None:
+        handler = command_handler_registry.get_bus_stop_by_name(command_handler_name)
+        if handler is None:
+            raise CommandHandlerNotFound(command_handler_name)
+
+        command_type = resolve_passenger_class_from_bus_stop(handler, "handle", "command")
+        self.__server.register(command_type, handler)
+
+    def start(self) -> None:
+        self.__server.run()
 
-    def _transport(self, passenger: Command) -> None:
-        handler_queue = self.__command_registry.get_command_destination_contact(passenger.passenger_name())
-        if handler_queue is None:
-            raise HandlerNotFoundForCommand(passenger.passenger_name())
-
-        self.__put_command(handler_queue, passenger)
-
-    def __put_command(self, queue: Queue, command: Command) -> None:
-        serialized_command = self.__command_serializer.serialize(command)
-        queue.put(serialized_command)
+    def stop(self):
+        pass
```

### Comparing `bus-station-5.1.0/src/bus_station/command_terminal/bus/asynchronous/threaded_command_bus.py` & `bus_station-6.0.0/src/bus_station/command_terminal/bus_engine/rpyc_command_bus_engine.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,28 @@
-from threading import Thread
+from bus_station.command_terminal.command_handler_not_found import CommandHandlerNotFound
+from bus_station.command_terminal.command_handler_registry import CommandHandlerRegistry
+from bus_station.passengers.passenger_resolvers import resolve_passenger_class_from_bus_stop
+from bus_station.shared_terminal.engine.engine import Engine
+from bus_station.shared_terminal.rpyc_server import RPyCServer
 
-from bus_station.command_terminal.bus.command_bus import CommandBus
-from bus_station.command_terminal.command import Command
-from bus_station.command_terminal.command_handler import CommandHandler
-from bus_station.command_terminal.handler_not_found_for_command import HandlerNotFoundForCommand
-from bus_station.command_terminal.registry.in_memory_command_registry import InMemoryCommandRegistry
-from bus_station.passengers.reception.passenger_receiver import PassengerReceiver
 
-
-class ThreadedCommandBus(CommandBus):
+class RPyCCommandBusEngine(Engine):
     def __init__(
-        self, command_registry: InMemoryCommandRegistry, command_receiver: PassengerReceiver[Command, CommandHandler]
+        self, rpyc_server: RPyCServer, command_handler_registry: CommandHandlerRegistry, command_handler_name: str
     ):
-        self.__command_registry = command_registry
-        self.__command_receiver = command_receiver
+        self.__server = rpyc_server
+        self.__register_command_in_server(command_handler_registry, command_handler_name)
+
+    def __register_command_in_server(
+        self, command_handler_registry: CommandHandlerRegistry, command_handler_name: str
+    ) -> None:
+        handler = command_handler_registry.get_bus_stop_by_name(command_handler_name)
+        if handler is None:
+            raise CommandHandlerNotFound(command_handler_name)
+        command_type = resolve_passenger_class_from_bus_stop(handler, "handle", "command")
+        self.__server.register(command_type, handler)
 
-    def _transport(self, passenger: Command) -> None:
-        command_handler = self.__command_registry.get_command_destination_contact(passenger.passenger_name())
-        if command_handler is None:
-            raise HandlerNotFoundForCommand(passenger.passenger_name())
+    def start(self) -> None:
+        self.__server.run()
 
-        execution_thread = Thread(target=self.__command_receiver.receive, args=(passenger, command_handler))
-        execution_thread.start()
+    def stop(self) -> None:
+        pass
```

### Comparing `bus-station-5.1.0/src/bus_station/command_terminal/bus/synchronous/distributed/json_rpc_command_bus.py` & `bus_station-6.0.0/src/bus_station/command_terminal/bus/synchronous/distributed/rpyc_command_bus.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,47 @@
-import requests
-from jsonrpcclient import Error, parse, request
+from rpyc import Connection, connect
 
+from bus_station.bus_stop.registration.address.address_not_found_for_bus_stop import AddressNotFoundForBusStop
+from bus_station.bus_stop.registration.address.bus_stop_address_registry import BusStopAddressRegistry
 from bus_station.command_terminal.bus.command_bus import CommandBus
 from bus_station.command_terminal.command import Command
-from bus_station.command_terminal.command_execution_failed import CommandExecutionFailed
 from bus_station.command_terminal.handler_not_found_for_command import HandlerNotFoundForCommand
-from bus_station.command_terminal.registry.remote_command_registry import RemoteCommandRegistry
+from bus_station.passengers.passenger_registry import passenger_bus_stop_registry
 from bus_station.passengers.serialization.passenger_serializer import PassengerSerializer
 
 
-class JsonRPCCommandBus(CommandBus):
+class RPyCCommandBus(CommandBus):
     def __init__(
         self,
         command_serializer: PassengerSerializer,
-        command_registry: RemoteCommandRegistry,
+        address_registry: BusStopAddressRegistry,
     ):
         self.__command_serializer = command_serializer
-        self.__command_registry = command_registry
+        self.__address_registry = address_registry
 
     def _transport(self, passenger: Command) -> None:
-        handler_address = self.__command_registry.get_command_destination_contact(passenger.passenger_name())
-        if handler_address is None:
+        handler_address = self.__get_handler_address(passenger)
+
+        rpyc_client = self.__get_rpyc_client(handler_address)
+        self.__execute_command(rpyc_client, passenger)
+
+        rpyc_client.close()
+
+    def __get_handler_address(self, passenger: Command) -> str:
+        command_handler_ids = passenger_bus_stop_registry.get_bus_stops_for_passenger(passenger.passenger_name())
+        if len(command_handler_ids) == 0:
             raise HandlerNotFoundForCommand(passenger.passenger_name())
 
-        self.__execute_command(passenger, handler_address)
+        command_handler_id = next(iter(command_handler_ids))
+        handler_address = self.__address_registry.get_bus_stop_address(command_handler_id)
+        if handler_address is None:
+            raise AddressNotFoundForBusStop(command_handler_id)
 
-    def __execute_command(self, command: Command, command_handler_addr: str) -> None:
-        serialized_command = self.__command_serializer.serialize(command)
+        return handler_address
 
-        request_response = requests.post(
-            command_handler_addr, json=request(command.__class__.passenger_name(), params=(serialized_command,))
-        )
-        json_rpc_response = parse(request_response.json())
+    def __get_rpyc_client(self, handler_addr: str) -> Connection:
+        host, port = handler_addr.split(":")
+        return connect(host, port=port, config={"allow_public_attrs": True})
 
-        if isinstance(json_rpc_response, Error):
-            raise CommandExecutionFailed(command, json_rpc_response.message)
+    def __execute_command(self, client: Connection, command: Command) -> None:
+        serialized_command = self.__command_serializer.serialize(command)
+        getattr(client.root, command.passenger_name())(serialized_command)
```

### Comparing `bus-station-5.1.0/src/bus_station/command_terminal/bus/synchronous/sync_command_bus.py` & `bus_station-6.0.0/src/bus_station/command_terminal/json_rpc_command_server.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,15 @@
-from bus_station.command_terminal.bus.command_bus import CommandBus
+from typing import Type
+
 from bus_station.command_terminal.command import Command
 from bus_station.command_terminal.command_handler import CommandHandler
-from bus_station.command_terminal.handler_not_found_for_command import HandlerNotFoundForCommand
-from bus_station.command_terminal.registry.in_memory_command_registry import InMemoryCommandRegistry
-from bus_station.passengers.reception.passenger_receiver import PassengerReceiver
-
+from bus_station.shared_terminal.json_rpc_server import JsonRPCServer
 
-class SyncCommandBus(CommandBus):
-    def __init__(
-        self, command_registry: InMemoryCommandRegistry, command_receiver: PassengerReceiver[Command, CommandHandler]
-    ):
-        self.__command_registry = command_registry
-        self.__command_receiver = command_receiver
 
-    def _transport(self, passenger: Command) -> None:
-        command_handler = self.__command_registry.get_command_destination_contact(passenger.passenger_name())
-        if command_handler is None:
-            raise HandlerNotFoundForCommand(passenger.passenger_name())
-        self.__command_receiver.receive(passenger, command_handler)
+class JsonRPCCommandServer(JsonRPCServer[Command, CommandHandler]):
+    def _passenger_handler(
+        self, bus_stop: CommandHandler, passenger_class: Type[Command], serialized_passenger: str
+    ) -> None:
+        command = self._passenger_deserializer.deserialize(serialized_passenger, passenger_cls=passenger_class)
+        if not isinstance(command, Command):
+            raise TypeError("Input serialized command is not a Command")
+        self._passenger_receiver.receive(command, bus_stop)
```

### Comparing `bus-station-5.1.0/src/bus_station/command_terminal/bus_engine/json_rpc_command_bus_engine.py` & `bus_station-6.0.0/src/bus_station/command_terminal/command_handler_registry.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from bus_station.command_terminal.command import Command
-from bus_station.command_terminal.handler_not_found_for_command import HandlerNotFoundForCommand
-from bus_station.command_terminal.json_rpc_command_server import JsonRPCCommandServer
-from bus_station.command_terminal.registry.remote_command_registry import RemoteCommandRegistry
-from bus_station.passengers.resolve_passenger_from_bus_stop import resolve_passenger_from_bus_stop
-from bus_station.shared_terminal.engine.engine import Engine
+from functools import partial
+from typing import List, Optional
 
+from bus_station.bus_stop.registration.bus_stop_registry import BusStopRegistry
+from bus_station.bus_stop.registration.supervisor.bus_stop_registration_supervisor import BusStopRegistrationSupervisor
+from bus_station.bus_stop.resolvers.bus_stop_resolver import BusStopResolver
+from bus_station.command_terminal.command_handler import CommandHandler
+from bus_station.passengers.passenger_registry import passenger_bus_stop_registry
+from bus_station.passengers.passenger_resolvers import resolve_passenger_class_from_bus_stop
 
-class JsonRPCCommandBusEngine(Engine):
+
+class CommandHandlerRegistry(BusStopRegistry[CommandHandler]):
     def __init__(
         self,
-        server: JsonRPCCommandServer,
-        command_registry: RemoteCommandRegistry,
-        command_name: str,
+        bus_stop_resolver: BusStopResolver,
+        registration_supervisors: Optional[List[BusStopRegistrationSupervisor]] = None,
     ):
-        super().__init__()
-        self.__server = server
-        self.__register_command_in_server(command_registry, command_name)
-
-    def __register_command_in_server(self, command_registry: RemoteCommandRegistry, command_name: str) -> None:
-        handler = command_registry.get_command_destination(command_name)
-        if handler is None:
-            raise HandlerNotFoundForCommand(command_name)
-        command_type = resolve_passenger_from_bus_stop(handler, "handle", "command", Command)
-        self.__server.register(command_type, handler)
+        bus_stop_passenger_resolver = partial(
+            resolve_passenger_class_from_bus_stop,
+            bus_stop_handle_function_name="handle",
+            passenger_type_name="command",
+        )
+        super().__init__(bus_stop_resolver, bus_stop_passenger_resolver, registration_supervisors)
 
-    def start(self) -> None:
-        self.__server.run()
+    def get_handler_from_command(self, command_name: str) -> Optional[CommandHandler]:
+        command_handler_ids = passenger_bus_stop_registry.get_bus_stops_for_passenger(command_name)
+        if len(command_handler_ids) == 0:
+            return None
 
-    def stop(self):
-        pass
+        command_handler_id = next(iter(command_handler_ids))
+        return self._bus_stop_resolver.resolve(command_handler_id)
```

### Comparing `bus-station-5.1.0/src/bus_station/command_terminal/bus_engine/kombu_command_bus_engine.py` & `bus_station-6.0.0/src/bus_station/command_terminal/bus_engine/kombu_command_bus_engine.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,51 +1,43 @@
 from typing import ClassVar
 
 from kombu import Connection, Exchange, Queue
 from kombu.transport.base import StdChannel
 
 from bus_station.command_terminal.command import Command
 from bus_station.command_terminal.command_handler import CommandHandler
-from bus_station.command_terminal.contact_not_found_for_command import ContactNotFoundForCommand
-from bus_station.command_terminal.handler_not_found_for_command import HandlerNotFoundForCommand
-from bus_station.command_terminal.registry.remote_command_registry import RemoteCommandRegistry
+from bus_station.command_terminal.command_handler_not_found import CommandHandlerNotFound
+from bus_station.command_terminal.command_handler_registry import CommandHandlerRegistry
 from bus_station.passengers.passenger_kombu_consumer import PassengerKombuConsumer
+from bus_station.passengers.passenger_resolvers import resolve_passenger_class_from_bus_stop
 from bus_station.passengers.reception.passenger_receiver import PassengerReceiver
-from bus_station.passengers.resolve_passenger_from_bus_stop import resolve_passenger_from_bus_stop
 from bus_station.passengers.serialization.passenger_deserializer import PassengerDeserializer
 from bus_station.shared_terminal.engine.engine import Engine
 
 
 class KombuCommandBusEngine(Engine):
     __DEAD_LETTER_EXCHANGE_NAME: ClassVar = "failed_commands"
 
     def __init__(
         self,
         broker_connection: Connection,
-        command_registry: RemoteCommandRegistry,
+        command_handler_registry: CommandHandlerRegistry,
         command_receiver: PassengerReceiver[Command, CommandHandler],
         command_deserializer: PassengerDeserializer,
-        command_name: str,
+        command_handler_name: str,
     ):
-        super().__init__()
-        command_handler = command_registry.get_command_destination(command_name)
+        command_handler = command_handler_registry.get_bus_stop_by_name(command_handler_name)
         if command_handler is None:
-            raise HandlerNotFoundForCommand(command_name)
+            raise CommandHandlerNotFound(command_handler_name)
 
-        broker_connection = broker_connection
+        command_type = resolve_passenger_class_from_bus_stop(command_handler, "handle", "command")
         channel = broker_connection.channel()
         self.__create_dead_letter_exchange(channel)
 
-        command_queue_name = command_registry.get_command_destination_contact(command_name)
-        if command_queue_name is None:
-            raise ContactNotFoundForCommand(command_name)
-
-        command_queue = self.__create_command_handler_queue(command_queue_name, channel)
-
-        command_type = resolve_passenger_from_bus_stop(command_handler, "handle", "command", Command)
+        command_queue = self.__create_command_handler_queue(command_type.passenger_name(), channel)
 
         self.__command_consumer = PassengerKombuConsumer(
             broker_connection,
             command_queue,
             command_handler,
             command_type,
             command_receiver,
```

### Comparing `bus-station-5.1.0/src/bus_station/command_terminal/bus_engine/memory_queue_command_bus_engine.py` & `bus_station-6.0.0/src/bus_station/command_terminal/bus_engine/memory_queue_command_bus_engine.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from bus_station.command_terminal.command import Command
 from bus_station.command_terminal.command_handler import CommandHandler
-from bus_station.command_terminal.handler_not_found_for_command import HandlerNotFoundForCommand
-from bus_station.command_terminal.registry.command_registry import CommandRegistry
+from bus_station.command_terminal.command_handler_not_found import CommandHandlerNotFound
+from bus_station.command_terminal.command_handler_registry import CommandHandlerRegistry
 from bus_station.passengers.memory_queue_passenger_worker import MemoryQueuePassengerWorker
+from bus_station.passengers.passenger_resolvers import resolve_passenger_class_from_bus_stop
 from bus_station.passengers.reception.passenger_receiver import PassengerReceiver
 from bus_station.passengers.serialization.passenger_deserializer import PassengerDeserializer
 from bus_station.shared_terminal.engine.engine import Engine
+from bus_station.shared_terminal.factories.memory_queue_factory import memory_queue_factory
 
 
 class MemoryQueueCommandBusEngine(Engine):
     def __init__(
         self,
-        command_registry: CommandRegistry,
+        command_handler_registry: CommandHandlerRegistry,
         command_receiver: PassengerReceiver[Command, CommandHandler],
         command_deserializer: PassengerDeserializer,
-        command_name: str,
+        command_handler_name: str,
     ):
-        super().__init__()
-        command_handler = command_registry.get_command_destination(command_name)
+        command_handler = command_handler_registry.get_bus_stop_by_name(command_handler_name)
         if command_handler is None:
-            raise HandlerNotFoundForCommand(command_name)
+            raise CommandHandlerNotFound(command_handler_name)
 
-        command_queue = command_registry.get_command_destination_contact(command_name)
+        command = resolve_passenger_class_from_bus_stop(command_handler, "handle", "command")
+        command_queue = memory_queue_factory.queue_with_id(command.passenger_name())
         self.__command_worker = MemoryQueuePassengerWorker(
             command_queue, command_handler, command_receiver, command_deserializer
         )
 
     def start(self) -> None:
         try:
             self.__command_worker.work()
```

### Comparing `bus-station-5.1.0/src/bus_station/command_terminal/bus_engine/rpyc_command_bus_engine.py` & `bus_station-6.0.0/src/bus_station/command_terminal/middleware/implementations/tracking_command_middleware.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,20 @@
-from bus_station.command_terminal.command import Command
-from bus_station.command_terminal.handler_not_found_for_command import HandlerNotFoundForCommand
-from bus_station.command_terminal.registry.command_registry import CommandRegistry
-from bus_station.passengers.resolve_passenger_from_bus_stop import resolve_passenger_from_bus_stop
-from bus_station.shared_terminal.engine.engine import Engine
-from bus_station.shared_terminal.rpyc_server import RPyCServer
+from typing import Optional
 
+from bus_station.command_terminal.command import Command
+from bus_station.command_terminal.command_handler import CommandHandler
+from bus_station.command_terminal.middleware.command_middleware import CommandMiddleware
+from bus_station.tracking_terminal.trackers.passenger_tracker import PassengerTracker
 
-class RPyCCommandBusEngine(Engine):
-    def __init__(self, rpyc_server: RPyCServer, command_registry: CommandRegistry, command_name: str):
-        super().__init__()
-        self.__server = rpyc_server
-        self.__register_command_in_server(command_registry, command_name)
 
-    def __register_command_in_server(self, command_registry: CommandRegistry, command_name: str) -> None:
-        handler = command_registry.get_command_destination(command_name)
-        if handler is None:
-            raise HandlerNotFoundForCommand(command_name)
-        command_type = resolve_passenger_from_bus_stop(handler, "handle", "command", Command)
-        self.__server.register(command_type, handler)
+class TrackingCommandMiddleware(CommandMiddleware):
+    def __init__(self, passenger_tracker: PassengerTracker):
+        self.__tracker = passenger_tracker
 
-    def start(self) -> None:
-        self.__server.run()
+    def before_handle(self, passenger: Command, bus_stop: CommandHandler) -> None:
+        self.__tracker.start_tracking(passenger, bus_stop)
 
-    def stop(self) -> None:
-        pass
+    def after_handle(
+        self, passenger: Command, bus_stop: CommandHandler, handling_exception: Optional[Exception] = None
+    ) -> None:
+        success = handling_exception is None
+        self.__tracker.end_tracking(passenger, bus_stop, success)
```

### Comparing `bus-station-5.1.0/src/bus_station/command_terminal/json_rpc_command_server.py` & `bus_station-6.0.0/src/bus_station/command_terminal/rpyc_command_server.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Type
 
 from bus_station.command_terminal.command import Command
 from bus_station.command_terminal.command_handler import CommandHandler
-from bus_station.shared_terminal.json_rpc_server import JsonRPCServer
+from bus_station.shared_terminal.rpyc_server import RPyCServer
 
 
-class JsonRPCCommandServer(JsonRPCServer[Command, CommandHandler]):
+class RPyCCommandServer(RPyCServer[Command, CommandHandler]):
     def _passenger_handler(
         self, bus_stop: CommandHandler, passenger_class: Type[Command], serialized_passenger: str
     ) -> None:
         command = self._passenger_deserializer.deserialize(serialized_passenger, passenger_cls=passenger_class)
         if not isinstance(command, Command):
             raise TypeError("Input serialized command is not a Command")
         self._passenger_receiver.receive(command, bus_stop)
```

### Comparing `bus-station-5.1.0/src/bus_station/command_terminal/middleware/command_middleware.py` & `bus_station-6.0.0/src/bus_station/command_terminal/middleware/command_middleware.py`

 * *Files identical despite different names*

### Comparing `bus-station-5.1.0/src/bus_station/command_terminal/middleware/command_middleware_receiver.py` & `bus_station-6.0.0/src/bus_station/command_terminal/middleware/command_middleware_receiver.py`

 * *Files identical despite different names*

### Comparing `bus-station-5.1.0/src/bus_station/command_terminal/middleware/implementations/logging_command_middleware.py` & `bus_station-6.0.0/src/bus_station/command_terminal/middleware/implementations/logging_command_middleware.py`

 * *Files identical despite different names*

### Comparing `bus-station-5.1.0/src/bus_station/command_terminal/middleware/implementations/timing_command_middleware.py` & `bus_station-6.0.0/src/bus_station/command_terminal/middleware/implementations/timing_command_middleware.py`

 * *Files identical despite different names*

### Comparing `bus-station-5.1.0/src/bus_station/command_terminal/middleware/implementations/tracking_command_middleware.py` & `bus_station-6.0.0/src/bus_station/query_terminal/middleware/implementations/tracking_query_middleware.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,30 @@
+from dataclasses import asdict
 from typing import Optional
 
-from bus_station.command_terminal.command import Command
-from bus_station.command_terminal.command_handler import CommandHandler
-from bus_station.command_terminal.middleware.command_middleware import CommandMiddleware
+from bus_station.query_terminal.middleware.query_middleware import QueryMiddleware
+from bus_station.query_terminal.query import Query
+from bus_station.query_terminal.query_handler import QueryHandler
+from bus_station.query_terminal.query_response import QueryResponse
 from bus_station.tracking_terminal.trackers.passenger_tracker import PassengerTracker
 
 
-class TrackingCommandMiddleware(CommandMiddleware):
+class TrackingQueryMiddleware(QueryMiddleware):
     def __init__(self, passenger_tracker: PassengerTracker):
         self.__tracker = passenger_tracker
 
-    def before_handle(self, passenger: Command, bus_stop: CommandHandler) -> None:
+    def before_handle(self, passenger: Query, bus_stop: QueryHandler) -> None:
         self.__tracker.start_tracking(passenger, bus_stop)
 
     def after_handle(
-        self, passenger: Command, bus_stop: CommandHandler, handling_exception: Optional[Exception] = None
-    ) -> None:
+        self,
+        passenger: Query,
+        bus_stop: QueryHandler,
+        query_response: QueryResponse,
+        handling_exception: Optional[Exception] = None,
+    ) -> QueryResponse:
         success = handling_exception is None
-        self.__tracker.end_tracking(passenger, bus_stop, success)
+        response_data = asdict(query_response) if query_response is not None else None
+        self.__tracker.end_tracking(
+            passenger=passenger, bus_stop=bus_stop, response_data=response_data, success=success
+        )
+        return query_response
```

### Comparing `bus-station-5.1.0/src/bus_station/event_terminal/bus/asynchronous/distributed/kombu_event_bus.py` & `bus_station-6.0.0/src/bus_station/event_terminal/bus/asynchronous/distributed/kombu_event_bus.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,26 @@
 from kombu import Connection, Producer
 
 from bus_station.event_terminal.bus.event_bus import EventBus
 from bus_station.event_terminal.event import Event
-from bus_station.event_terminal.registry.remote_event_registry import RemoteEventRegistry
 from bus_station.passengers.serialization.passenger_serializer import PassengerSerializer
 
 
 class KombuEventBus(EventBus):
     def __init__(
         self,
         broker_connection: Connection,
         event_serializer: PassengerSerializer,
-        event_registry: RemoteEventRegistry,
     ):
         self.__broker_connection = broker_connection
         self.__event_serializer = event_serializer
-        self.__event_registry = event_registry
         self.__producer = Producer(broker_connection.channel())
 
     def _transport(self, passenger: Event) -> None:
-        event_exchange_names = self.__event_registry.get_event_destination_contacts(passenger.passenger_name())
-        if event_exchange_names is None:
-            return
-
-        published_exchanges = []
-        for event_exchange_name in event_exchange_names:
-            if event_exchange_name in published_exchanges:
-                continue
-            self.__publish_event(passenger, event_exchange_name)
-            published_exchanges.append(event_exchange_name)
+        self.__publish_event(passenger, passenger.passenger_name())
 
     def __publish_event(self, event: Event, event_exchange_name: str) -> None:
         serialized_event = self.__event_serializer.serialize(event)
         if self.__producer is not None:
             self.__producer.publish(
                 serialized_event,
                 exchange=event_exchange_name,
```

### Comparing `bus-station-5.1.0/src/bus_station/event_terminal/bus/asynchronous/memory_queue_event_bus.py` & `bus_station-6.0.0/src/bus_station/event_terminal/bus/asynchronous/memory_queue_event_bus.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from multiprocessing import Queue
 
 from bus_station.event_terminal.bus.event_bus import EventBus
 from bus_station.event_terminal.event import Event
-from bus_station.event_terminal.registry.in_memory_event_registry import InMemoryEventRegistry
+from bus_station.event_terminal.event_consumer_registry import EventConsumerRegistry
 from bus_station.passengers.serialization.passenger_serializer import PassengerSerializer
+from bus_station.shared_terminal.factories.memory_queue_factory import memory_queue_factory
 
 
 class MemoryQueueEventBus(EventBus):
     def __init__(
         self,
         event_serializer: PassengerSerializer,
-        event_registry: InMemoryEventRegistry,
+        event_consumer_registry: EventConsumerRegistry,
     ):
         self.__event_serializer = event_serializer
-        self.__event_registry = event_registry
+        self.__event_consumer_registry = event_consumer_registry
 
     def _transport(self, passenger: Event) -> None:
-        event_consumer_queues = self.__event_registry.get_event_destination_contacts(passenger.passenger_name())
-        if event_consumer_queues is None:
-            return
-
-        for event_queue in event_consumer_queues:
-            self.__put_event(event_queue, passenger)
+        for event_consumer in self.__event_consumer_registry.get_consumers_from_event(passenger.passenger_name()):
+            event_consumer_queue = memory_queue_factory.queue_with_id(event_consumer.bus_stop_name())
+            self.__put_event(event_consumer_queue, passenger)
 
     def __put_event(self, queue: Queue, event: Event) -> None:
         serialized_event = self.__event_serializer.serialize(event)
         queue.put(serialized_event)
```

### Comparing `bus-station-5.1.0/src/bus_station/event_terminal/bus/asynchronous/threaded_event_bus.py` & `bus_station-6.0.0/src/bus_station/event_terminal/bus/asynchronous/threaded_event_bus.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from threading import Thread
 
 from bus_station.event_terminal.bus.event_bus import EventBus
 from bus_station.event_terminal.event import Event
 from bus_station.event_terminal.event_consumer import EventConsumer
-from bus_station.event_terminal.registry.in_memory_event_registry import InMemoryEventRegistry
+from bus_station.event_terminal.event_consumer_registry import EventConsumerRegistry
 from bus_station.passengers.reception.passenger_receiver import PassengerReceiver
 
 
 class ThreadedEventBus(EventBus):
-    def __init__(self, event_registry: InMemoryEventRegistry, event_receiver: PassengerReceiver[Event, EventConsumer]):
+    def __init__(
+        self, event_consumer_registry: EventConsumerRegistry, event_receiver: PassengerReceiver[Event, EventConsumer]
+    ):
         self.__event_receiver = event_receiver
-        self.__event_registry = event_registry
+        self.__event_consumer_registry = event_consumer_registry
 
     def _transport(self, passenger: Event) -> None:
-        event_consumers = self.__event_registry.get_event_destination_contacts(passenger.passenger_name())
-        if event_consumers is None:
-            return
-
-        for event_consumer in event_consumers:
+        for event_consumer in self.__event_consumer_registry.get_consumers_from_event(passenger.passenger_name()):
             execution_thread = Thread(target=self.__event_receiver.receive, args=(passenger, event_consumer))
             execution_thread.start()
```

### Comparing `bus-station-5.1.0/src/bus_station/event_terminal/bus/synchronous/sync_event_bus.py` & `bus_station-6.0.0/src/bus_station/command_terminal/bus/asynchronous/threaded_command_bus.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,26 @@
-from bus_station.event_terminal.bus.event_bus import EventBus
-from bus_station.event_terminal.event import Event
-from bus_station.event_terminal.event_consumer import EventConsumer
-from bus_station.event_terminal.registry.in_memory_event_registry import InMemoryEventRegistry
+from threading import Thread
+
+from bus_station.command_terminal.bus.command_bus import CommandBus
+from bus_station.command_terminal.command import Command
+from bus_station.command_terminal.command_handler import CommandHandler
+from bus_station.command_terminal.command_handler_registry import CommandHandlerRegistry
+from bus_station.command_terminal.handler_not_found_for_command import HandlerNotFoundForCommand
 from bus_station.passengers.reception.passenger_receiver import PassengerReceiver
 
 
-class SyncEventBus(EventBus):
-    def __init__(self, event_registry: InMemoryEventRegistry, event_receiver: PassengerReceiver[Event, EventConsumer]):
-        self.__event_receiver = event_receiver
-        self.__event_registry = event_registry
+class ThreadedCommandBus(CommandBus):
+    def __init__(
+        self,
+        command_handler_registry: CommandHandlerRegistry,
+        command_receiver: PassengerReceiver[Command, CommandHandler],
+    ):
+        self.__command_handler_registry = command_handler_registry
+        self.__command_receiver = command_receiver
 
-    def _transport(self, passenger: Event) -> None:
-        event_consumers = self.__event_registry.get_event_destination_contacts(passenger.passenger_name())
-        if event_consumers is None:
-            return
+    def _transport(self, passenger: Command) -> None:
+        command_handler = self.__command_handler_registry.get_handler_from_command(passenger.passenger_name())
+        if command_handler is None:
+            raise HandlerNotFoundForCommand(passenger.passenger_name())
 
-        for event_consumer in event_consumers:
-            self.__event_receiver.receive(passenger, event_consumer)
+        execution_thread = Thread(target=self.__command_receiver.receive, args=(passenger, command_handler))
+        execution_thread.start()
```

### Comparing `bus-station-5.1.0/src/bus_station/event_terminal/bus_engine/kombu_event_bus_engine.py` & `bus_station-6.0.0/src/bus_station/event_terminal/bus_engine/kombu_event_bus_engine.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,51 @@
 from typing import ClassVar
 
 from kombu import Connection, Exchange, Queue
 from kombu.transport.base import StdChannel
 
-from bus_station.event_terminal.contact_not_found_for_consumer import ContactNotFoundForConsumer
 from bus_station.event_terminal.event import Event
 from bus_station.event_terminal.event_consumer import EventConsumer
 from bus_station.event_terminal.event_consumer_not_found import EventConsumerNotFound
-from bus_station.event_terminal.registry.remote_event_registry import RemoteEventRegistry
+from bus_station.event_terminal.event_consumer_registry import EventConsumerRegistry
 from bus_station.passengers.passenger_kombu_consumer import PassengerKombuConsumer
+from bus_station.passengers.passenger_resolvers import resolve_passenger_class_from_bus_stop
 from bus_station.passengers.reception.passenger_receiver import PassengerReceiver
-from bus_station.passengers.resolve_passenger_from_bus_stop import resolve_passenger_from_bus_stop
 from bus_station.passengers.serialization.passenger_deserializer import PassengerDeserializer
 from bus_station.shared_terminal.engine.engine import Engine
 
 
 class KombuEventBusEngine(Engine):
     __DEAD_LETTER_EXCHANGE_NAME: ClassVar = "failed_events"
 
     def __init__(
         self,
         broker_connection: Connection,
-        event_registry: RemoteEventRegistry,
         event_receiver: PassengerReceiver[Event, EventConsumer],
+        event_consumer_registry: EventConsumerRegistry,
         event_deserializer: PassengerDeserializer,
-        event_name: str,
         event_consumer_name: str,
     ):
-        super().__init__()
-        event_exchange_name = event_registry.get_event_destination_contact(event_name, event_consumer_name)
-        if event_exchange_name is None:
-            raise ContactNotFoundForConsumer(event_consumer_name)
-        event_consumer = event_registry.get_event_destination(event_name, event_consumer_name)
+        event_consumer = event_consumer_registry.get_bus_stop_by_name(event_consumer_name)
         if event_consumer is None:
             raise EventConsumerNotFound(event_consumer_name)
 
+        event = resolve_passenger_class_from_bus_stop(event_consumer, "consume", "event")
+
         channel = broker_connection.channel()
         self.__create_dead_letter_exchange(channel)
 
-        event_exchange = self.__create_event_consumer_exchange(event_exchange_name, channel)
+        event_exchange = self.__create_event_consumer_exchange(event.passenger_name(), channel)
         event_consumer_queue = self.__create_event_consumer_queue(event_consumer, event_exchange, channel)
 
         self.__event_consumer_consumer = PassengerKombuConsumer(
             broker_connection,
             event_consumer_queue,
             event_consumer,
-            resolve_passenger_from_bus_stop(event_consumer, "consume", "event", Event),
+            event,
             event_receiver,
             event_deserializer,
         )
 
     def start(self) -> None:
         try:
             self.__event_consumer_consumer.run()
```

### Comparing `bus-station-5.1.0/src/bus_station/event_terminal/bus_engine/memory_queue_event_bus_engine.py` & `bus_station-6.0.0/src/bus_station/event_terminal/bus_engine/memory_queue_event_bus_engine.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,32 @@
-from bus_station.event_terminal.contact_not_found_for_consumer import ContactNotFoundForConsumer
 from bus_station.event_terminal.event import Event
 from bus_station.event_terminal.event_consumer import EventConsumer
 from bus_station.event_terminal.event_consumer_not_found import EventConsumerNotFound
-from bus_station.event_terminal.registry.event_registry import EventRegistry
+from bus_station.event_terminal.event_consumer_registry import EventConsumerRegistry
 from bus_station.passengers.memory_queue_passenger_worker import MemoryQueuePassengerWorker
 from bus_station.passengers.reception.passenger_receiver import PassengerReceiver
 from bus_station.passengers.serialization.passenger_deserializer import PassengerDeserializer
 from bus_station.shared_terminal.engine.engine import Engine
+from bus_station.shared_terminal.factories.memory_queue_factory import memory_queue_factory
 
 
 class MemoryQueueEventBusEngine(Engine):
     def __init__(
         self,
-        event_registry: EventRegistry,
+        event_consumer_registry: EventConsumerRegistry,
         event_receiver: PassengerReceiver[Event, EventConsumer],
         event_deserializer: PassengerDeserializer,
-        event_name: str,
         event_consumer_name: str,
     ):
-        super().__init__()
-        event_queue = event_registry.get_event_destination_contact(event_name, event_consumer_name)
-        if event_queue is None:
-            raise ContactNotFoundForConsumer(event_consumer_name)
-        event_consumer = event_registry.get_event_destination(event_name, event_consumer_name)
+        event_consumer = event_consumer_registry.get_bus_stop_by_name(event_consumer_name)
         if event_consumer is None:
             raise EventConsumerNotFound(event_consumer_name)
 
+        event_queue = memory_queue_factory.queue_with_id(event_consumer.bus_stop_name())
+
         self.__event_worker = MemoryQueuePassengerWorker(
             event_queue, event_consumer, event_receiver, event_deserializer
         )
 
     def start(self) -> None:
         try:
             self.__event_worker.work()
```

### Comparing `bus-station-5.1.0/src/bus_station/event_terminal/middleware/event_middleware.py` & `bus_station-6.0.0/src/bus_station/event_terminal/middleware/event_middleware.py`

 * *Files identical despite different names*

### Comparing `bus-station-5.1.0/src/bus_station/event_terminal/middleware/event_middleware_receiver.py` & `bus_station-6.0.0/src/bus_station/event_terminal/middleware/event_middleware_receiver.py`

 * *Files identical despite different names*

### Comparing `bus-station-5.1.0/src/bus_station/event_terminal/middleware/implementations/logging_event_middleware.py` & `bus_station-6.0.0/src/bus_station/event_terminal/middleware/implementations/logging_event_middleware.py`

 * *Files identical despite different names*

### Comparing `bus-station-5.1.0/src/bus_station/event_terminal/middleware/implementations/timing_event_middleware.py` & `bus_station-6.0.0/src/bus_station/event_terminal/middleware/implementations/timing_event_middleware.py`

 * *Files identical despite different names*

### Comparing `bus-station-5.1.0/src/bus_station/event_terminal/middleware/implementations/tracking_event_middleware.py` & `bus_station-6.0.0/src/bus_station/event_terminal/middleware/implementations/tracking_event_middleware.py`

 * *Files identical despite different names*

### Comparing `bus-station-5.1.0/src/bus_station/passengers/memory_queue_passenger_worker.py` & `bus_station-6.0.0/src/bus_station/passengers/memory_queue_passenger_worker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from ctypes import c_bool
 from multiprocessing import Queue, Value
 from queue import Empty
 
+from bus_station.bus_stop.bus_stop import BusStop
 from bus_station.passengers.reception.passenger_receiver import PassengerReceiver
 from bus_station.passengers.serialization.passenger_deserializer import PassengerDeserializer
-from bus_station.shared_terminal.bus_stop import BusStop
 
 
 class MemoryQueuePassengerWorker:
     def __init__(
         self,
         queue: Queue,
         passenger_bus_stop: BusStop,
```

### Comparing `bus-station-5.1.0/src/bus_station/passengers/passenger_kombu_consumer.py` & `bus_station-6.0.0/src/bus_station/passengers/passenger_kombu_consumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 from kombu import Connection
 from kombu import Consumer as KombuConsumer
 from kombu import Message, Queue
 from kombu.mixins import ConsumerMixin
 from kombu.transport.base import StdChannel
 
+from bus_station.bus_stop.bus_stop import BusStop
 from bus_station.passengers.passenger import Passenger
 from bus_station.passengers.reception.passenger_receiver import PassengerReceiver
 from bus_station.passengers.serialization.passenger_deserializer import PassengerDeserializer
-from bus_station.shared_terminal.bus_stop import BusStop
 
 
 class PassengerKombuConsumer(ConsumerMixin):
     def __init__(
         self,
         connection: Connection,
         passenger_queue: Queue,
```

### Comparing `bus-station-5.1.0/src/bus_station/passengers/passenger_record/redis_passenger_record_repository.py` & `bus_station-6.0.0/src/bus_station/shared_terminal/rpyc_server.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,53 @@
-from typing import Iterable, List, Optional
-
-from redis import Redis
-
-from bus_station.passengers.passenger_record.passenger_record import PassengerRecord
-from bus_station.passengers.passenger_record.passenger_record_repository import PassengerRecordRepository
-
-
-class RedisPassengerRecordRepository(PassengerRecordRepository):
-    def __init__(self, client: Redis):
-        self.__client = client
-
-    def save(self, passenger_record: PassengerRecord[str]) -> None:
-        str_passenger_record = str(passenger_record)
-        self.__client.lpush(passenger_record.passenger_name, str_passenger_record.encode("UTF-8"))
-
-    def find_by_passenger_name(self, passenger_name: str) -> Optional[List[PassengerRecord]]:
-        redis_records = []
-        for redis_value in self.__client.lrange(passenger_name, 0, -1):
-            passenger_record = PassengerRecord.from_str(redis_value.decode("UTF-8"))
-            redis_records.append(passenger_record)
-
-        if len(redis_records) == 0:
-            return None
-        return redis_records
-
-    def find_by_passenger_name_and_destination_name(
-        self, passenger_name: str, passenger_destination_name: str
-    ) -> Optional[PassengerRecord]:
-        for redis_value in self.__client.lrange(passenger_name, 0, -1):
-            passenger_record = PassengerRecord.from_str(redis_value.decode("UTF-8"))
-            if passenger_record.destination_name == passenger_destination_name:
-                return passenger_record
-        return None
-
-    def all(self) -> Iterable[PassengerRecord]:
-        for passenger_name in self.__client.scan_iter("*"):
-            passenger_records = self.find_by_passenger_name(passenger_name)
-            if passenger_records is None:
-                continue
-            for passenger_record in passenger_records:
-                yield passenger_record
-
-    def delete_by_passenger_name(self, passenger_name: str) -> None:
-        self.__client.delete(passenger_name)
+from abc import abstractmethod
+from functools import partial
+from typing import Callable, ClassVar, Dict, Generic, Optional, Type, TypeVar
+
+from rpyc import Service, ThreadedServer
+
+from bus_station.bus_stop.bus_stop import BusStop
+from bus_station.passengers.passenger import Passenger
+from bus_station.passengers.reception.passenger_receiver import PassengerReceiver
+from bus_station.passengers.serialization.passenger_deserializer import PassengerDeserializer
+
+P = TypeVar("P", bound=Passenger)
+S = TypeVar("S", bound=BusStop)
+
+
+class RPyCServer(Generic[P, S]):
+    __EXPOSED_CALLABLE_PATTERN: ClassVar[str] = "exposed_{callable_name}"
+
+    def __init__(
+        self,
+        host: str,
+        port: int,
+        passenger_deserializer: PassengerDeserializer,
+        passenger_receiver: PassengerReceiver,
+    ):
+        self._passenger_deserializer = passenger_deserializer
+        self._passenger_receiver = passenger_receiver
+        self.__host = host
+        self.__port = port
+        self.__callables_to_expose: Dict[str, Callable] = {}
+
+    def register(self, passenger_class: Type[P], bus_stop: S) -> None:
+        exposed_callable = partial(self._passenger_handler, bus_stop, passenger_class)
+        exposed_callable_name = self.__EXPOSED_CALLABLE_PATTERN.format(callable_name=passenger_class.passenger_name())
+        self.__callables_to_expose[exposed_callable_name] = exposed_callable
+
+    def run(self) -> None:
+        rpyc_server = ThreadedServer(
+            service=self.__build_rpyc_service(),
+            hostname=self.__host,
+            port=self.__port,
+            protocol_config={"allow_public_attrs": True},
+        )
+        rpyc_server.start()
+        rpyc_server.close()
+
+    def __build_rpyc_service(self) -> Service:
+        rpyc_service_class = type("RPyCServiceClass", (Service,), self.__callables_to_expose)
+        return rpyc_service_class()
+
+    @abstractmethod
+    def _passenger_handler(self, bus_stop: S, passenger_class: Type[P], serialized_passenger: str) -> Optional[str]:
+        pass
```

### Comparing `bus-station-5.1.0/src/bus_station/passengers/reception/passenger_middleware_receiver.py` & `bus_station-6.0.0/src/bus_station/passengers/reception/passenger_middleware_receiver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABC
 from typing import Any, Generic, Iterable, List, Tuple, Type, TypeVar
 
+from bus_station.bus_stop.bus_stop import BusStop
 from bus_station.passengers.passenger import Passenger
 from bus_station.passengers.passenger_middleware import PassengerMiddleware
 from bus_station.passengers.reception.passenger_receiver import PassengerReceiver
-from bus_station.shared_terminal.bus_stop import BusStop
 
 M = TypeVar("M", bound=PassengerMiddleware)
 S = TypeVar("S", bound=BusStop)
 P = TypeVar("P", bound=Passenger)
 
 
 class PassengerMiddlewareReceiver(PassengerReceiver[P, S], Generic[P, S, M], ABC):
```

### Comparing `bus-station-5.1.0/src/bus_station/passengers/resolve_passenger_from_bus_stop.py` & `bus_station-6.0.0/src/bus_station/passengers/passenger_resolvers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,17 @@
-from typing import Type, TypeVar, get_type_hints
+from typing import Type, get_type_hints
 
-from bus_station.passengers.passenger import Passenger
-from bus_station.shared_terminal.bus_stop import BusStop
+from bus_station.bus_stop.bus_stop import BusStop
 
-P = TypeVar("P", bound=Passenger)
 
-
-def resolve_passenger_from_bus_stop(
-    bus_stop: BusStop, bus_stop_handle_function_name: str, passenger_type_name: str, expected_passenger_type: Type[P]
-) -> Type[P]:
+def resolve_passenger_class_from_bus_stop(
+    bus_stop: BusStop, bus_stop_handle_function_name: str, passenger_type_name: str
+) -> Type:
     bus_stop_handle_function = getattr(bus_stop, bus_stop_handle_function_name)
     bus_stop_handle_typing = get_type_hints(bus_stop_handle_function)
 
     if passenger_type_name not in bus_stop_handle_typing:
         raise TypeError(
             f"{bus_stop_handle_function_name} {passenger_type_name} not found for {bus_stop.bus_stop_name()}"
         )
 
-    bus_stop_passenger_type = bus_stop_handle_typing[passenger_type_name]
-    if not issubclass(bus_stop_passenger_type, expected_passenger_type):
-        raise TypeError(
-            f"Wrong type for {bus_stop_handle_function_name} {passenger_type_name} of {bus_stop.bus_stop_name()}"
-        )
-
-    return bus_stop_passenger_type
+    return bus_stop_handle_typing[passenger_type_name]
```

### Comparing `bus-station-5.1.0/src/bus_station/passengers/serialization/passenger_json_deserializer.py` & `bus_station-6.0.0/src/bus_station/passengers/serialization/passenger_json_deserializer.py`

 * *Files identical despite different names*

### Comparing `bus-station-5.1.0/src/bus_station/passengers/serialization/passenger_json_serializer.py` & `bus_station-6.0.0/src/bus_station/passengers/serialization/passenger_json_serializer.py`

 * *Files identical despite different names*

### Comparing `bus-station-5.1.0/src/bus_station/query_terminal/bus/synchronous/distributed/json_rpc_query_bus.py` & `bus_station-6.0.0/src/bus_station/query_terminal/bus/synchronous/distributed/json_rpc_query_bus.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,48 @@
 import requests
 from jsonrpcclient import Error, parse, request
 
+from bus_station.bus_stop.registration.address.address_not_found_for_bus_stop import AddressNotFoundForBusStop
+from bus_station.bus_stop.registration.address.bus_stop_address_registry import BusStopAddressRegistry
+from bus_station.passengers.passenger_registry import passenger_bus_stop_registry
 from bus_station.passengers.serialization.passenger_serializer import PassengerSerializer
 from bus_station.query_terminal.bus.query_bus import QueryBus
 from bus_station.query_terminal.handler_not_found_for_query import HandlerNotFoundForQuery
 from bus_station.query_terminal.query import Query
 from bus_station.query_terminal.query_execution_failed import QueryExecutionFailed
 from bus_station.query_terminal.query_response import QueryResponse
-from bus_station.query_terminal.registry.remote_query_registry import RemoteQueryRegistry
 from bus_station.query_terminal.serialization.query_response_deserializer import QueryResponseDeserializer
 
 
 class JsonRPCQueryBus(QueryBus):
     def __init__(
         self,
         query_serializer: PassengerSerializer,
         query_response_deserializer: QueryResponseDeserializer,
-        query_registry: RemoteQueryRegistry,
+        address_registry: BusStopAddressRegistry,
     ):
         self.__query_serializer = query_serializer
-        self.__query_registry = query_registry
+        self.__address_registry = address_registry
         self.__query_response_deserializer = query_response_deserializer
 
     def _transport(self, passenger: Query) -> QueryResponse:
-        handler_address = self.__query_registry.get_query_destination_contact(passenger.passenger_name())
-        if handler_address is None:
+        handler_address = self.__get_handler_address(passenger)
+        return self.__execute_query(passenger, handler_address)
+
+    def __get_handler_address(self, passenger: Query) -> str:
+        query_handler_ids = passenger_bus_stop_registry.get_bus_stops_for_passenger(passenger.passenger_name())
+        if len(query_handler_ids) == 0:
             raise HandlerNotFoundForQuery(passenger.passenger_name())
 
-        return self.__execute_query(passenger, handler_address)
+        query_handler_id = next(iter(query_handler_ids))
+        handler_address = self.__address_registry.get_bus_stop_address(query_handler_id)
+        if handler_address is None:
+            raise AddressNotFoundForBusStop(query_handler_id)
+
+        return handler_address
 
     def __execute_query(self, query: Query, query_handler_addr: str) -> QueryResponse:
         serialized_query = self.__query_serializer.serialize(query)
 
         request_response = requests.post(
             query_handler_addr, json=request(query.passenger_name(), params=(serialized_query,))
         )
```

### Comparing `bus-station-5.1.0/src/bus_station/query_terminal/bus/synchronous/distributed/rpyc_query_bus.py` & `bus_station-6.0.0/src/bus_station/query_terminal/bus/synchronous/distributed/rpyc_query_bus.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,51 @@
 from rpyc import Connection, connect
 
+from bus_station.bus_stop.registration.address.address_not_found_for_bus_stop import AddressNotFoundForBusStop
+from bus_station.bus_stop.registration.address.bus_stop_address_registry import BusStopAddressRegistry
+from bus_station.passengers.passenger_registry import passenger_bus_stop_registry
 from bus_station.passengers.serialization.passenger_serializer import PassengerSerializer
 from bus_station.query_terminal.bus.query_bus import QueryBus
 from bus_station.query_terminal.handler_not_found_for_query import HandlerNotFoundForQuery
 from bus_station.query_terminal.query import Query
 from bus_station.query_terminal.query_response import QueryResponse
-from bus_station.query_terminal.registry.remote_query_registry import RemoteQueryRegistry
 from bus_station.query_terminal.serialization.query_response_deserializer import QueryResponseDeserializer
 
 
 class RPyCQueryBus(QueryBus):
     def __init__(
         self,
         query_serializer: PassengerSerializer,
         query_response_deserializer: QueryResponseDeserializer,
-        query_registry: RemoteQueryRegistry,
+        address_registry: BusStopAddressRegistry,
     ):
         self.__query_serializer = query_serializer
         self.__query_response_deserializer = query_response_deserializer
-        self.__query_registry = query_registry
+        self.__address_registry = address_registry
 
     def _transport(self, passenger: Query) -> QueryResponse:
-        query_handler_addr = self.__query_registry.get_query_destination_contact(passenger.passenger_name())
-        if query_handler_addr is None:
-            raise HandlerNotFoundForQuery(passenger.passenger_name())
+        handler_address = self.__get_handler_address(passenger)
 
-        rpyc_client = self.__get_rpyc_client(query_handler_addr)
+        rpyc_client = self.__get_rpyc_client(handler_address)
         query_response = self.__execute_query(rpyc_client, passenger)
         rpyc_client.close()
         return query_response
 
+    def __get_handler_address(self, passenger: Query) -> str:
+        query_handler_ids = passenger_bus_stop_registry.get_bus_stops_for_passenger(passenger.passenger_name())
+        if len(query_handler_ids) == 0:
+            raise HandlerNotFoundForQuery(passenger.passenger_name())
+
+        query_handler_id = next(iter(query_handler_ids))
+        handler_address = self.__address_registry.get_bus_stop_address(query_handler_id)
+        if handler_address is None:
+            raise AddressNotFoundForBusStop(query_handler_id)
+
+        return handler_address
+
     def __get_rpyc_client(self, handler_addr: str) -> Connection:
         host, port = handler_addr.split(":")
         return connect(host, port=port)
 
     def __execute_query(self, client: Connection, query: Query) -> QueryResponse:
         serialized_query = self.__query_serializer.serialize(query)
         serialized_query_response = getattr(client.root, query.passenger_name())(serialized_query)
```

### Comparing `bus-station-5.1.0/src/bus_station/query_terminal/json_rpc_query_server.py` & `bus_station-6.0.0/src/bus_station/query_terminal/json_rpc_query_server.py`

 * *Files identical despite different names*

### Comparing `bus-station-5.1.0/src/bus_station/query_terminal/middleware/implementations/logging_query_middleware.py` & `bus_station-6.0.0/src/bus_station/query_terminal/middleware/implementations/logging_query_middleware.py`

 * *Files identical despite different names*

### Comparing `bus-station-5.1.0/src/bus_station/query_terminal/middleware/implementations/timing_query_middleware.py` & `bus_station-6.0.0/src/bus_station/query_terminal/middleware/implementations/timing_query_middleware.py`

 * *Files identical despite different names*

### Comparing `bus-station-5.1.0/src/bus_station/query_terminal/middleware/implementations/tracking_query_middleware.py` & `bus_station-6.0.0/src/bus_station/query_terminal/middleware/query_middleware_receiver.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-from dataclasses import asdict
-from typing import Optional
-
+from bus_station.passengers.reception.passenger_middleware_receiver import PassengerMiddlewareReceiver
 from bus_station.query_terminal.middleware.query_middleware import QueryMiddleware
 from bus_station.query_terminal.query import Query
 from bus_station.query_terminal.query_handler import QueryHandler
 from bus_station.query_terminal.query_response import QueryResponse
-from bus_station.tracking_terminal.trackers.passenger_tracker import PassengerTracker
 
 
-class TrackingQueryMiddleware(QueryMiddleware):
-    def __init__(self, passenger_tracker: PassengerTracker):
-        self.__tracker = passenger_tracker
-
-    def before_handle(self, passenger: Query, bus_stop: QueryHandler) -> None:
-        self.__tracker.start_tracking(passenger, bus_stop)
-
-    def after_handle(
-        self,
-        passenger: Query,
-        bus_stop: QueryHandler,
-        query_response: QueryResponse,
-        handling_exception: Optional[Exception] = None,
-    ) -> QueryResponse:
-        success = handling_exception is None
-        response_data = asdict(query_response) if query_response is not None else None
-        self.__tracker.end_tracking(
-            passenger=passenger, bus_stop=bus_stop, response_data=response_data, success=success
-        )
+class QueryMiddlewareReceiver(PassengerMiddlewareReceiver[Query, QueryHandler, QueryMiddleware]):
+    def _receive(self, passenger: Query, passenger_bus_stop: QueryHandler) -> QueryResponse:
+        middlewares = list(self._get_middlewares())
+        for middleware in middlewares:
+            middleware.before_handle(passenger, passenger_bus_stop)
+
+        query_response = QueryResponse(data=None)
+        handling_exception = None
+        try:
+            query_response = passenger_bus_stop.handle(passenger)
+        except Exception as ex:
+            handling_exception = ex
+
+        for middleware in reversed(middlewares):
+            query_response = middleware.after_handle(
+                passenger, passenger_bus_stop, query_response, handling_exception=handling_exception
+            )
+
+        if handling_exception is not None:
+            raise handling_exception
+
         return query_response
```

### Comparing `bus-station-5.1.0/src/bus_station/query_terminal/middleware/query_middleware.py` & `bus_station-6.0.0/src/bus_station/query_terminal/middleware/query_middleware.py`

 * *Files identical despite different names*

### Comparing `bus-station-5.1.0/src/bus_station/query_terminal/rpyc_query_server.py` & `bus_station-6.0.0/src/bus_station/query_terminal/rpyc_query_server.py`

 * *Files identical despite different names*

### Comparing `bus-station-5.1.0/src/bus_station/shared_terminal/broker_connection/connection_parameters/rabbitmq_connection_parameters.py` & `bus_station-6.0.0/src/bus_station/shared_terminal/broker_connection/connection_parameters/rabbitmq_connection_parameters.py`

 * *Files identical despite different names*

### Comparing `bus-station-5.1.0/src/bus_station/shared_terminal/bus.py` & `bus_station-6.0.0/src/bus_station/passengers/reception/passenger_receiver.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from abc import abstractmethod
 from typing import Any, Generic, Optional, TypeVar
 
+from bus_station.bus_stop.bus_stop import BusStop
 from bus_station.passengers.passenger import Passenger
-from bus_station.shared_terminal.distributed import get_distributed_id
+from bus_station.shared_terminal.context import set_context_root_passenger_id
 
+S = TypeVar("S", bound=BusStop)
 P = TypeVar("P", bound=Passenger)
 
 
-class Bus(Generic[P]):
-    def transport(self, passenger: P) -> Optional[Any]:
-        distributed_id = get_distributed_id(passenger)
-        passenger.set_distributed_id(distributed_id)
-
-        return self._transport(passenger)
+class PassengerReceiver(Generic[P, S]):
+    def receive(self, passenger: P, passenger_bus_stop: S) -> Optional[Any]:
+        set_context_root_passenger_id(passenger.passenger_id)
+
+        try:
+            return self._receive(passenger, passenger_bus_stop)
+        finally:
+            set_context_root_passenger_id(passenger.root_passenger_id)
 
     @abstractmethod
-    def _transport(self, passenger: P) -> Optional[Any]:
+    def _receive(self, passenger: P, passenger_bus_stop: S) -> Optional[Any]:
         pass
```

### Comparing `bus-station-5.1.0/src/bus_station/shared_terminal/bus_stop_resolver/pypendency_bus_stop_resolver.py` & `bus_station-6.0.0/src/bus_station/bus_stop/resolvers/pypendency_bus_stop_resolver.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from typing import Optional, TypeVar
 
 from pypendency.container import Container
 
-from bus_station.shared_terminal.bus_stop import BusStop
-from bus_station.shared_terminal.bus_stop_resolver.bus_stop_resolver import BusStopResolver
+from bus_station.bus_stop.bus_stop import BusStop
+from bus_station.bus_stop.resolvers.bus_stop_resolver import BusStopResolver
 
 S = TypeVar("S", bound=BusStop)
 
 
 class PypendencyBusStopResolver(BusStopResolver[S]):
     def __init__(self, pypendency_container: Container):
         self.__pypendency_container = pypendency_container
 
-    def resolve_from_fqn(self, bus_stop_fqn: str) -> Optional[S]:
-        resolved_instance = self.__pypendency_container.get(bus_stop_fqn)
+    def resolve(self, bus_stop_id: str) -> Optional[S]:
+        resolved_instance = self.__pypendency_container.get(bus_stop_id)
         if resolved_instance is None:
             return None
         if not issubclass(resolved_instance.__class__, BusStop):
-            raise TypeError(f"Instance resolved from {bus_stop_fqn} is not a valid BusStop")
+            raise TypeError(f"Instance resolved from {bus_stop_id} is not a valid BusStop")
         return resolved_instance  # type: ignore
```

### Comparing `bus-station-5.1.0/src/bus_station/shared_terminal/engine/runner/process_engine_runner.py` & `bus_station-6.0.0/src/bus_station/shared_terminal/engine/runner/process_engine_runner.py`

 * *Files identical despite different names*

### Comparing `bus-station-5.1.0/src/bus_station/shared_terminal/json_rpc_server.py` & `bus_station-6.0.0/src/bus_station/shared_terminal/json_rpc_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from http.server import ThreadingHTTPServer
 from typing import Callable, Dict, Generic, Optional, Type, TypeVar
 
 from jsonrpcserver import Error, Result, Success, method
 from jsonrpcserver.codes import ERROR_INTERNAL_ERROR
 from jsonrpcserver.server import RequestHandler
 
+from bus_station.bus_stop.bus_stop import BusStop
 from bus_station.passengers.passenger import Passenger
 from bus_station.passengers.reception.passenger_receiver import PassengerReceiver
 from bus_station.passengers.serialization.passenger_deserializer import PassengerDeserializer
-from bus_station.shared_terminal.bus_stop import BusStop
 
 P = TypeVar("P", bound=Passenger)
 S = TypeVar("S", bound=BusStop)
 
 
 class JsonRPCServer(Generic[P, S]):
     def __init__(
```

### Comparing `bus-station-5.1.0/src/bus_station/shared_terminal/kafka_topic_creator.py` & `bus_station-6.0.0/src/bus_station/shared_terminal/kafka_topic_creator.py`

 * *Files identical despite different names*

### Comparing `bus-station-5.1.0/src/bus_station/tracking_terminal/models/passenger_model_tracking_map.py` & `bus_station-6.0.0/src/bus_station/tracking_terminal/models/passenger_model_tracking_map.py`

 * *Files identical despite different names*

### Comparing `bus-station-5.1.0/src/bus_station/tracking_terminal/models/passenger_tracking_json_serializer.py` & `bus_station-6.0.0/src/bus_station/tracking_terminal/models/passenger_tracking_json_serializer.py`

 * *Files identical despite different names*

### Comparing `bus-station-5.1.0/src/bus_station/tracking_terminal/trackers/kafka_passenger_tracker.py` & `bus_station-6.0.0/src/bus_station/tracking_terminal/trackers/kafka_passenger_tracker.py`

 * *Files identical despite different names*

### Comparing `bus-station-5.1.0/src/bus_station/tracking_terminal/trackers/passenger_tracker.py` & `bus_station-6.0.0/src/bus_station/tracking_terminal/trackers/passenger_tracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABC, abstractmethod
 from dataclasses import asdict
 from datetime import datetime
 from typing import Any
 
+from bus_station.bus_stop.bus_stop import BusStop
 from bus_station.passengers.passenger import Passenger
-from bus_station.shared_terminal.bus_stop import BusStop
 from bus_station.tracking_terminal.models.passenger_model_tracking_map import PassengerModelTrackingMap
 from bus_station.tracking_terminal.models.passenger_tracking import PassengerTracking
 
 
 class PassengerTracker(ABC):
     def __init__(self, passenger_model_tracking_map: PassengerModelTrackingMap):
         self.__passenger_model_tracking_map = passenger_model_tracking_map
```

### Comparing `bus-station-5.1.0/PKG-INFO` & `bus_station-6.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: bus-station
-Version: 5.1.0
+Version: 6.0.0
 Summary: A python bus station
 Author: DeejayRevok
 Author-email: seryi_one@hotmail.com
 Requires-Python: >=3.10.0,<3.11.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: confluent-kafka (>=2.0.2,<3.0.0)
 Requires-Dist: freezegun (>=1.2.2,<2.0.0)
 Requires-Dist: jsonrpcclient (>=4.0.2,<5.0.0)
 Requires-Dist: jsonrpcserver (>=5.0.6,<6.0.0)
 Requires-Dist: kombu (==5.2.2)
 Requires-Dist: pypendency (>=0.1.0,<0.2.0)
-Requires-Dist: redis (==4.1.0)
+Requires-Dist: redis (==4.4.4)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: rpyc (==5.0.1)
 Description-Content-Type: text/markdown
 
 # Bus station
 Python bus pattern implementation
```

