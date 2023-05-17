# Comparing `tmp/redvox-3.4.1.tar.gz` & `tmp/redvox-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redvox-3.4.1.tar", last modified: Fri Apr 28 20:37:47 2023, max compression
+gzip compressed data, was "redvox-3.4.2.tar", last modified: Wed May 17 22:37:40 2023, max compression
```

## Comparing `redvox-3.4.1.tar` & `redvox-3.4.2.tar`

### file list

```diff
@@ -1,161 +1,153 @@
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.406221 redvox-3.4.1/
--rw-r--r--   0 opq       (1000) opq       (1000)    11343 2023-04-28 19:34:15.000000 redvox-3.4.1/LICENSE
--rw-r--r--   0 opq       (1000) opq       (1000)    13906 2023-04-28 20:37:47.406221 redvox-3.4.1/PKG-INFO
--rw-rw-r--   0 opq       (1000) opq       (1000)      517 2021-06-14 20:37:56.000000 redvox-3.4.1/README.md
--rw-r--r--   0 opq       (1000) opq       (1000)     1375 2023-04-28 19:34:15.000000 redvox-3.4.1/pyproject.toml
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.390222 redvox-3.4.1/redvox/
--rw-r--r--   0 opq       (1000) opq       (1000)      815 2023-04-28 20:36:50.000000 redvox-3.4.1/redvox/__init__.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.391222 redvox-3.4.1/redvox/api1000/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/__init__.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.392222 redvox-3.4.1/redvox/api1000/common/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/common/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    20204 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/common/common.py
--rw-r--r--   0 opq       (1000) opq       (1000)     1050 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/common/decorators.py
--rw-r--r--   0 opq       (1000) opq       (1000)     5359 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/common/generic.py
--rw-r--r--   0 opq       (1000) opq       (1000)      875 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/common/lz4.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2570 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/common/mapping.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2237 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/common/metadata.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2435 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/common/typing.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2114 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/errors.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.393222 redvox-3.4.1/redvox/api1000/gui/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/gui/__init__.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     4672 2021-04-14 19:22:20.000000 redvox-3.4.1/redvox/api1000/gui/image_viewer.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.393222 redvox-3.4.1/redvox/api1000/proto/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/proto/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    41044 2023-04-28 19:34:15.000000 redvox-3.4.1/redvox/api1000/proto/redvox_api_m_pb2.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.393222 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)     5639 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/event_streams.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.394222 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    11949 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/audio.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.394222 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/derived/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/derived/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    14890 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/derived/movement.py
--rw-r--r--   0 opq       (1000) opq       (1000)     7398 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/image.py
--rw-r--r--   0 opq       (1000) opq       (1000)    40936 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/location.py
--rw-r--r--   0 opq       (1000) opq       (1000)    42236 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/sensors.py
--rw-r--r--   0 opq       (1000) opq       (1000)     3425 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/single.py
--rw-r--r--   0 opq       (1000) opq       (1000)     5576 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/xyz.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    50437 2022-04-19 20:47:15.000000 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/station_information.py
--rw-r--r--   0 opq       (1000) opq       (1000)    19060 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/timing_information.py
--rw-r--r--   0 opq       (1000) opq       (1000)    21971 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/wrapped_packet.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.396222 redvox-3.4.1/redvox/api900/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    17514 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/concat.py
--rw-r--r--   0 opq       (1000) opq       (1000)      494 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/constants.py
--rw-r--r--   0 opq       (1000) opq       (1000)     1689 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/deprecation.py
--rw-r--r--   0 opq       (1000) opq       (1000)      351 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/exceptions.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.396222 redvox-3.4.1/redvox/api900/lib/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/lib/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)     7970 2023-04-28 19:34:15.000000 redvox-3.4.1/redvox/api900/lib/api900_pb2.py
--rw-r--r--   0 opq       (1000) opq       (1000)    43091 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/location_analyzer.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2597 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/migrations.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.396222 redvox-3.4.1/redvox/api900/qa/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/qa/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2813 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/qa/gap_detection.py
--rw-r--r--   0 opq       (1000) opq       (1000)    16939 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/reader.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    17096 2021-06-07 23:35:09.000000 redvox-3.4.1/redvox/api900/reader_utils.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.398222 redvox-3.4.1/redvox/api900/sensors/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2113 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/accelerometer_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2298 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/barometer_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2665 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/evenly_sampled_channel.py
--rw-r--r--   0 opq       (1000) opq       (1000)     6283 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/evenly_sampled_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     1989 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/gyroscope_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     4854 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/image_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2264 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/infrared_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)    16540 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/interleaved_channel.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2261 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/light_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)    10051 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/location_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2022 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/magnetometer_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     3209 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/microphone_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     4655 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/time_synchronization_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     3536 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/unevenly_sampled_channel.py
--rw-r--r--   0 opq       (1000) opq       (1000)     6619 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/unevenly_sampled_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     5907 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/sensors/xyz_unevenly_sampled_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     1128 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/stat_utils.py
--rw-r--r--   0 opq       (1000) opq       (1000)     8780 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/summarize.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.398222 redvox-3.4.1/redvox/api900/timesync/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/timesync/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    27606 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/timesync/api900_timesync.py
--rw-r--r--   0 opq       (1000) opq       (1000)    13824 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/timesync/tri_message_stats.py
--rw-r--r--   0 opq       (1000) opq       (1000)     1537 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/types.py
--rw-r--r--   0 opq       (1000) opq       (1000)    54392 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/api900/wrapped_redvox_packet.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.399222 redvox-3.4.1/redvox/cli/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/cli/__init__.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    22678 2021-04-14 19:22:20.000000 redvox-3.4.1/redvox/cli/cli.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     6683 2021-06-07 23:35:09.000000 redvox-3.4.1/redvox/cli/conversions.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     1797 2021-04-14 19:22:20.000000 redvox-3.4.1/redvox/cli/data_req.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.401222 redvox-3.4.1/redvox/cloud/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/cloud/__init__.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     2267 2021-04-06 18:15:12.000000 redvox-3.4.1/redvox/cloud/api.py
--rw-r--r--   0 opq       (1000) opq       (1000)   142063 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/cloud/api_m_fqns.py
--rw-r--r--   0 opq       (1000) opq       (1000)     4334 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/cloud/auth_api.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    27215 2022-04-20 20:36:13.000000 redvox-3.4.1/redvox/cloud/client.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     5905 2021-09-16 19:39:56.000000 redvox-3.4.1/redvox/cloud/config.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     6088 2021-04-14 19:22:20.000000 redvox-3.4.1/redvox/cloud/data_api.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     3829 2021-09-16 19:39:56.000000 redvox-3.4.1/redvox/cloud/data_client.py
--rw-r--r--   0 opq       (1000) opq       (1000)     3094 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/cloud/data_io.py
--rw-r--r--   0 opq       (1000) opq       (1000)      487 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/cloud/errors.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    18946 2022-04-20 20:36:13.000000 redvox-3.4.1/redvox/cloud/metadata_api.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     3770 2021-04-14 23:45:25.000000 redvox-3.4.1/redvox/cloud/query_timing_correction.py
--rw-rw-r--   0 opq       (1000) opq       (1000)      902 2022-04-20 20:36:13.000000 redvox-3.4.1/redvox/cloud/routes.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     4262 2021-04-14 23:45:25.000000 redvox-3.4.1/redvox/cloud/station_stats.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     7707 2022-06-01 22:08:00.000000 redvox-3.4.1/redvox/cloud/subscription.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.406221 redvox-3.4.1/redvox/common/
--rw-r--r--   0 opq       (1000) opq       (1000)      195 2021-03-29 23:26:30.000000 redvox-3.4.1/redvox/common/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    55240 2022-09-30 02:01:56.000000 redvox-3.4.1/redvox/common/api_conversions.py
--rw-r--r--   0 opq       (1000) opq       (1000)    23044 2023-04-25 00:47:07.000000 redvox-3.4.1/redvox/common/api_reader.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     5527 2022-04-19 20:47:15.000000 redvox-3.4.1/redvox/common/api_reader_dw.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    12875 2021-06-07 23:35:09.000000 redvox-3.4.1/redvox/common/api_reader_old.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     1173 2021-04-20 02:39:13.000000 redvox-3.4.1/redvox/common/constants.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     4126 2021-07-07 20:00:14.000000 redvox-3.4.1/redvox/common/cross_stats.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    44341 2022-06-29 18:15:55.000000 redvox-3.4.1/redvox/common/data_window.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     8246 2022-04-19 20:47:15.000000 redvox-3.4.1/redvox/common/data_window_configuration.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     6208 2022-01-03 23:28:51.000000 redvox-3.4.1/redvox/common/data_window_configuration_old.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    12571 2022-04-19 20:47:15.000000 redvox-3.4.1/redvox/common/data_window_io.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    31911 2022-01-03 23:28:51.000000 redvox-3.4.1/redvox/common/data_window_old.py
--rw-r--r--   0 opq       (1000) opq       (1000)    16785 2023-04-25 00:47:07.000000 redvox-3.4.1/redvox/common/date_time_utils.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     3250 2022-04-19 20:47:15.000000 redvox-3.4.1/redvox/common/errors.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    39791 2022-06-29 18:15:55.000000 redvox-3.4.1/redvox/common/event_stream.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     3397 2022-04-19 20:47:15.000000 redvox-3.4.1/redvox/common/event_stream_io.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    14254 2022-01-03 23:28:51.000000 redvox-3.4.1/redvox/common/file_statistics.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    22168 2022-04-19 20:47:15.000000 redvox-3.4.1/redvox/common/gap_and_pad_utils.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    22503 2022-01-03 23:28:51.000000 redvox-3.4.1/redvox/common/gap_and_pad_utils_old.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.406221 redvox-3.4.1/redvox/common/gui/
--rw-rw-r--   0 opq       (1000) opq       (1000)        0 2021-04-14 19:22:20.000000 redvox-3.4.1/redvox/common/gui/__init__.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    16251 2021-04-14 23:46:42.000000 redvox-3.4.1/redvox/common/gui/cloud_data_retrieval.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    56743 2022-06-29 18:15:55.000000 redvox-3.4.1/redvox/common/io.py
--rw-r--r--   0 opq       (1000) opq       (1000)    25612 2023-04-25 00:47:07.000000 redvox-3.4.1/redvox/common/offset_model.py
--rw-r--r--   0 opq       (1000) opq       (1000)    27554 2023-04-25 00:47:07.000000 redvox-3.4.1/redvox/common/packet_to_pyarrow.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     5022 2022-01-03 23:28:51.000000 redvox-3.4.1/redvox/common/parallel_utils.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     1256 2022-06-29 18:15:55.000000 redvox-3.4.1/redvox/common/run_me.py
--rw-r--r--   0 opq       (1000) opq       (1000)    94299 2023-04-25 00:47:07.000000 redvox-3.4.1/redvox/common/sensor_data.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    44259 2022-01-03 23:28:51.000000 redvox-3.4.1/redvox/common/sensor_data_old.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     1206 2022-01-03 23:28:51.000000 redvox-3.4.1/redvox/common/sensor_io.py
--rw-r--r--   0 opq       (1000) opq       (1000)    18349 2023-04-25 00:47:07.000000 redvox-3.4.1/redvox/common/sensor_reader_utils.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    55914 2022-01-03 23:28:51.000000 redvox-3.4.1/redvox/common/sensor_reader_utils_old.py
--rw-r--r--   0 opq       (1000) opq       (1000)     3352 2023-04-25 00:47:07.000000 redvox-3.4.1/redvox/common/session_io.py
--rw-r--r--   0 opq       (1000) opq       (1000)    44577 2023-04-25 00:47:07.000000 redvox-3.4.1/redvox/common/session_model.py
--rw-r--r--   0 opq       (1000) opq       (1000)    14986 2023-04-25 00:47:07.000000 redvox-3.4.1/redvox/common/session_model_utils.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    66786 2022-06-29 18:15:55.000000 redvox-3.4.1/redvox/common/station.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     1679 2022-04-19 20:47:15.000000 redvox-3.4.1/redvox/common/station_io.py
--rw-r--r--   0 opq       (1000) opq       (1000)     4515 2023-04-25 00:47:07.000000 redvox-3.4.1/redvox/common/station_model.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    42555 2022-01-03 23:28:51.000000 redvox-3.4.1/redvox/common/station_old.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    23699 2022-06-29 18:15:55.000000 redvox-3.4.1/redvox/common/station_utils.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     4002 2022-01-03 23:28:51.000000 redvox-3.4.1/redvox/common/stats_helper.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    24492 2022-04-19 20:47:15.000000 redvox-3.4.1/redvox/common/timesync.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     1295 2022-04-19 20:47:15.000000 redvox-3.4.1/redvox/common/timesync_io.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    35537 2022-01-03 23:28:51.000000 redvox-3.4.1/redvox/common/timesync_old.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    14138 2022-01-03 23:28:51.000000 redvox-3.4.1/redvox/common/tri_message_stats.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     1867 2021-07-07 20:00:14.000000 redvox-3.4.1/redvox/common/versioning.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2483 2022-09-30 02:01:51.000000 redvox-3.4.1/redvox/settings.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 20:37:47.391222 redvox-3.4.1/redvox.egg-info/
--rw-r--r--   0 opq       (1000) opq       (1000)    13906 2023-04-28 20:37:47.000000 redvox-3.4.1/redvox.egg-info/PKG-INFO
--rw-r--r--   0 opq       (1000) opq       (1000)     4767 2023-04-28 20:37:47.000000 redvox-3.4.1/redvox.egg-info/SOURCES.txt
--rw-r--r--   0 opq       (1000) opq       (1000)        1 2023-04-28 20:37:47.000000 redvox-3.4.1/redvox.egg-info/dependency_links.txt
--rw-r--r--   0 opq       (1000) opq       (1000)       51 2023-04-28 20:37:47.000000 redvox-3.4.1/redvox.egg-info/entry_points.txt
--rw-r--r--   0 opq       (1000) opq       (1000)      386 2023-04-28 20:37:47.000000 redvox-3.4.1/redvox.egg-info/requires.txt
--rw-r--r--   0 opq       (1000) opq       (1000)        7 2023-04-28 20:37:47.000000 redvox-3.4.1/redvox.egg-info/top_level.txt
--rw-r--r--   0 opq       (1000) opq       (1000)       38 2023-04-28 20:37:47.407221 redvox-3.4.1/setup.cfg
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.942336 redvox-3.4.2/
+-rw-r--r--   0 tyler      (501) staff       (20)    11343 2023-04-28 20:38:30.000000 redvox-3.4.2/LICENSE
+-rw-r--r--   0 tyler      (501) staff       (20)    13906 2023-05-17 22:37:40.941757 redvox-3.4.2/PKG-INFO
+-rw-r--r--   0 tyler      (501) staff       (20)      517 2021-06-16 20:22:36.000000 redvox-3.4.2/README.md
+-rw-r--r--   0 tyler      (501) staff       (20)     1375 2023-04-28 20:38:30.000000 redvox-3.4.2/pyproject.toml
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.812976 redvox-3.4.2/redvox/
+-rw-r--r--   0 tyler      (501) staff       (20)      728 2023-05-17 22:14:20.000000 redvox-3.4.2/redvox/__init__.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.816955 redvox-3.4.2/redvox/api1000/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/__init__.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.823528 redvox-3.4.2/redvox/api1000/common/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/common/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    20204 2021-03-31 23:04:52.000000 redvox-3.4.2/redvox/api1000/common/common.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1050 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/common/decorators.py
+-rw-r--r--   0 tyler      (501) staff       (20)     5359 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/common/generic.py
+-rw-r--r--   0 tyler      (501) staff       (20)      875 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/common/lz4.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2570 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/common/mapping.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2237 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/common/metadata.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2435 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/common/typing.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2114 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/errors.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.824720 redvox-3.4.2/redvox/api1000/gui/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/gui/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4672 2021-04-09 20:02:21.000000 redvox-3.4.2/redvox/api1000/gui/image_viewer.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.826033 redvox-3.4.2/redvox/api1000/proto/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/proto/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    39434 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/api1000/proto/redvox_api_m_pb2.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.830873 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     5639 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/event_streams.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.838024 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    11949 2021-03-31 23:04:52.000000 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/audio.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.839433 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/derived/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/derived/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    14890 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/derived/movement.py
+-rw-r--r--   0 tyler      (501) staff       (20)     7398 2021-03-31 23:04:52.000000 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/image.py
+-rw-r--r--   0 tyler      (501) staff       (20)    40936 2021-03-31 23:04:52.000000 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/location.py
+-rw-r--r--   0 tyler      (501) staff       (20)    42236 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/sensors.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3425 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/single.py
+-rw-r--r--   0 tyler      (501) staff       (20)     5576 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/xyz.py
+-rw-r--r--   0 tyler      (501) staff       (20)    50437 2022-12-15 01:35:54.000000 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/station_information.py
+-rw-r--r--   0 tyler      (501) staff       (20)    19060 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/timing_information.py
+-rw-r--r--   0 tyler      (501) staff       (20)    21971 2021-03-31 23:04:52.000000 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/wrapped_packet.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.854994 redvox-3.4.2/redvox/api900/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    17514 2021-03-31 23:04:52.000000 redvox-3.4.2/redvox/api900/concat.py
+-rw-r--r--   0 tyler      (501) staff       (20)      494 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/constants.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1689 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/deprecation.py
+-rw-r--r--   0 tyler      (501) staff       (20)      351 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/exceptions.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.857067 redvox-3.4.2/redvox/api900/lib/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/lib/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     7591 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/api900/lib/api900_pb2.py
+-rw-r--r--   0 tyler      (501) staff       (20)    43091 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/location_analyzer.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2597 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/migrations.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.858404 redvox-3.4.2/redvox/api900/qa/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/qa/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2813 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/qa/gap_detection.py
+-rw-r--r--   0 tyler      (501) staff       (20)    16939 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/reader.py
+-rw-r--r--   0 tyler      (501) staff       (20)    17096 2021-06-01 21:32:52.000000 redvox-3.4.2/redvox/api900/reader_utils.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.874601 redvox-3.4.2/redvox/api900/sensors/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2113 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/accelerometer_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2298 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/barometer_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2665 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/evenly_sampled_channel.py
+-rw-r--r--   0 tyler      (501) staff       (20)     6283 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/evenly_sampled_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1989 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/gyroscope_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4854 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/image_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2264 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/infrared_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)    16540 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/interleaved_channel.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2261 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/light_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)    10051 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/location_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2022 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/magnetometer_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3209 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/microphone_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4655 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/time_synchronization_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3536 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/unevenly_sampled_channel.py
+-rw-r--r--   0 tyler      (501) staff       (20)     6619 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/unevenly_sampled_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)     5907 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/xyz_unevenly_sampled_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1128 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/stat_utils.py
+-rw-r--r--   0 tyler      (501) staff       (20)     8780 2021-03-31 23:04:52.000000 redvox-3.4.2/redvox/api900/summarize.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.880006 redvox-3.4.2/redvox/api900/timesync/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/timesync/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    27606 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/timesync/api900_timesync.py
+-rw-r--r--   0 tyler      (501) staff       (20)    13824 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/timesync/tri_message_stats.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1537 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/types.py
+-rw-r--r--   0 tyler      (501) staff       (20)    54392 2021-03-31 23:04:52.000000 redvox-3.4.2/redvox/api900/wrapped_redvox_packet.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.886577 redvox-3.4.2/redvox/cli/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/cli/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    22678 2021-04-09 20:02:21.000000 redvox-3.4.2/redvox/cli/cli.py
+-rw-r--r--   0 tyler      (501) staff       (20)     6683 2021-06-01 21:32:52.000000 redvox-3.4.2/redvox/cli/conversions.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1797 2021-04-09 20:02:21.000000 redvox-3.4.2/redvox/cli/data_req.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.902033 redvox-3.4.2/redvox/cloud/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/cloud/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2267 2021-04-06 01:58:10.000000 redvox-3.4.2/redvox/cloud/api.py
+-rw-r--r--   0 tyler      (501) staff       (20)   142063 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/cloud/api_m_fqns.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4334 2021-03-31 23:04:52.000000 redvox-3.4.2/redvox/cloud/auth_api.py
+-rw-r--r--   0 tyler      (501) staff       (20)    27215 2022-12-15 01:35:54.000000 redvox-3.4.2/redvox/cloud/client.py
+-rw-r--r--   0 tyler      (501) staff       (20)     5905 2022-12-15 01:35:54.000000 redvox-3.4.2/redvox/cloud/config.py
+-rw-r--r--   0 tyler      (501) staff       (20)     6088 2021-04-09 20:02:21.000000 redvox-3.4.2/redvox/cloud/data_api.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3829 2022-12-15 01:35:54.000000 redvox-3.4.2/redvox/cloud/data_client.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3094 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/cloud/data_io.py
+-rw-r--r--   0 tyler      (501) staff       (20)      487 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/cloud/errors.py
+-rw-r--r--   0 tyler      (501) staff       (20)    18946 2022-12-15 01:35:54.000000 redvox-3.4.2/redvox/cloud/metadata_api.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3770 2021-04-14 22:44:11.000000 redvox-3.4.2/redvox/cloud/query_timing_correction.py
+-rw-r--r--   0 tyler      (501) staff       (20)      902 2022-12-15 01:35:54.000000 redvox-3.4.2/redvox/cloud/routes.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4262 2021-04-14 22:44:11.000000 redvox-3.4.2/redvox/cloud/station_stats.py
+-rw-r--r--   0 tyler      (501) staff       (20)     7707 2022-12-15 01:35:54.000000 redvox-3.4.2/redvox/cloud/subscription.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.939383 redvox-3.4.2/redvox/common/
+-rw-r--r--   0 tyler      (501) staff       (20)      195 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/common/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    55240 2023-01-05 19:44:31.000000 redvox-3.4.2/redvox/common/api_conversions.py
+-rw-r--r--   0 tyler      (501) staff       (20)    23092 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/common/api_reader.py
+-rw-r--r--   0 tyler      (501) staff       (20)     5532 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/common/api_reader_dw.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1173 2021-04-19 23:26:28.000000 redvox-3.4.2/redvox/common/constants.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4126 2021-06-29 20:11:21.000000 redvox-3.4.2/redvox/common/cross_stats.py
+-rw-r--r--   0 tyler      (501) staff       (20)    44735 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/common/data_window.py
+-rw-r--r--   0 tyler      (501) staff       (20)     8246 2022-12-15 01:35:54.000000 redvox-3.4.2/redvox/common/data_window_configuration.py
+-rw-r--r--   0 tyler      (501) staff       (20)     7301 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/common/data_window_io.py
+-rw-r--r--   0 tyler      (501) staff       (20)    16785 2023-01-05 19:44:31.000000 redvox-3.4.2/redvox/common/date_time_utils.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3250 2022-12-15 01:35:54.000000 redvox-3.4.2/redvox/common/errors.py
+-rw-r--r--   0 tyler      (501) staff       (20)    41765 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/common/event_stream.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3397 2022-12-15 01:35:54.000000 redvox-3.4.2/redvox/common/event_stream_io.py
+-rw-r--r--   0 tyler      (501) staff       (20)    13655 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/common/file_statistics.py
+-rw-r--r--   0 tyler      (501) staff       (20)    17695 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/common/gap_and_pad_utils.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.940659 redvox-3.4.2/redvox/common/gui/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-04-09 20:02:21.000000 redvox-3.4.2/redvox/common/gui/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    16251 2021-04-15 01:00:48.000000 redvox-3.4.2/redvox/common/gui/cloud_data_retrieval.py
+-rw-r--r--   0 tyler      (501) staff       (20)    56756 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/common/io.py
+-rw-r--r--   0 tyler      (501) staff       (20)    26136 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/common/offset_model.py
+-rw-r--r--   0 tyler      (501) staff       (20)    27551 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/common/packet_to_pyarrow.py
+-rw-r--r--   0 tyler      (501) staff       (20)     5022 2022-12-15 01:35:54.000000 redvox-3.4.2/redvox/common/parallel_utils.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1256 2022-12-15 01:35:54.000000 redvox-3.4.2/redvox/common/run_me.py
+-rw-r--r--   0 tyler      (501) staff       (20)    94611 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/common/sensor_data.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1206 2022-12-15 01:35:54.000000 redvox-3.4.2/redvox/common/sensor_io.py
+-rw-r--r--   0 tyler      (501) staff       (20)    18349 2023-01-05 19:44:31.000000 redvox-3.4.2/redvox/common/sensor_reader_utils.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3352 2023-01-05 19:44:31.000000 redvox-3.4.2/redvox/common/session_io.py
+-rw-r--r--   0 tyler      (501) staff       (20)    44873 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/common/session_model.py
+-rw-r--r--   0 tyler      (501) staff       (20)    14986 2023-01-05 19:44:31.000000 redvox-3.4.2/redvox/common/session_model_utils.py
+-rw-r--r--   0 tyler      (501) staff       (20)    69098 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/common/station.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1679 2022-12-15 01:35:54.000000 redvox-3.4.2/redvox/common/station_io.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4549 2023-04-26 02:27:01.000000 redvox-3.4.2/redvox/common/station_model.py
+-rw-r--r--   0 tyler      (501) staff       (20)    18151 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/common/station_utils.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4002 2022-12-15 01:35:54.000000 redvox-3.4.2/redvox/common/stats_helper.py
+-rw-r--r--   0 tyler      (501) staff       (20)    21477 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/common/timesync.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1295 2022-12-15 01:35:54.000000 redvox-3.4.2/redvox/common/timesync_io.py
+-rw-r--r--   0 tyler      (501) staff       (20)    14257 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/common/tri_message_stats.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1867 2021-06-29 20:11:21.000000 redvox-3.4.2/redvox/common/versioning.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2205 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/settings.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.815924 redvox-3.4.2/redvox.egg-info/
+-rw-r--r--   0 tyler      (501) staff       (20)    13906 2023-05-17 22:37:40.000000 redvox-3.4.2/redvox.egg-info/PKG-INFO
+-rw-r--r--   0 tyler      (501) staff       (20)     4483 2023-05-17 22:37:40.000000 redvox-3.4.2/redvox.egg-info/SOURCES.txt
+-rw-r--r--   0 tyler      (501) staff       (20)        1 2023-05-17 22:37:40.000000 redvox-3.4.2/redvox.egg-info/dependency_links.txt
+-rw-r--r--   0 tyler      (501) staff       (20)       51 2023-05-17 22:37:40.000000 redvox-3.4.2/redvox.egg-info/entry_points.txt
+-rw-r--r--   0 tyler      (501) staff       (20)      386 2023-05-17 22:37:40.000000 redvox-3.4.2/redvox.egg-info/requires.txt
+-rw-r--r--   0 tyler      (501) staff       (20)        7 2023-05-17 22:37:40.000000 redvox-3.4.2/redvox.egg-info/top_level.txt
+-rw-r--r--   0 tyler      (501) staff       (20)       38 2023-05-17 22:37:40.942487 redvox-3.4.2/setup.cfg
```

### Comparing `redvox-3.4.1/LICENSE` & `redvox-3.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/PKG-INFO` & `redvox-3.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redvox
-Version: 3.4.1
+Version: 3.4.2
 Summary: Library for working with RedVox files. 
 Author-email: "RedVox, Inc" <support@redvox.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `redvox-3.4.1/README.md` & `redvox-3.4.2/README.md`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/pyproject.toml` & `redvox-3.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/__init__.py` & `redvox-3.4.2/redvox/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Provides library level metadata and constants.
 """
 
 NAME: str = "redvox"
-VERSION: str = "3.4.1"
+VERSION: str = "3.4.2"
 
 
 def version() -> str:
     """Returns the version number of this library."""
     return VERSION
 
 
@@ -23,9 +23,8 @@
     import redvox.settings
 
     print()
     print(f"version: {VERSION}")
     print(f"parallelism enabled: {redvox.settings.is_parallelism_enabled()}")
     print(f"native extra enabled: {redvox.settings.is_native_extra_enabled()}")
     print(f"gui extra enabled: {redvox.settings.is_gui_extra_enabled()}")
-    print(f"protobuf cpp backend enabled: {redvox.settings.is_cpp_backend_enabled()}")
     print()
```

### Comparing `redvox-3.4.1/redvox/api1000/common/common.py` & `redvox-3.4.2/redvox/api1000/common/common.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api1000/common/decorators.py` & `redvox-3.4.2/redvox/api1000/common/decorators.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api1000/common/generic.py` & `redvox-3.4.2/redvox/api1000/common/generic.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api1000/common/lz4.py` & `redvox-3.4.2/redvox/api1000/common/lz4.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api1000/common/mapping.py` & `redvox-3.4.2/redvox/api1000/common/mapping.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api1000/common/metadata.py` & `redvox-3.4.2/redvox/api1000/common/metadata.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api1000/common/typing.py` & `redvox-3.4.2/redvox/api1000/common/typing.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api1000/errors.py` & `redvox-3.4.2/redvox/api1000/errors.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api1000/gui/image_viewer.py` & `redvox-3.4.2/redvox/api1000/gui/image_viewer.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api1000/proto/redvox_api_m_pb2.py` & `redvox-3.4.2/redvox/api1000/proto/redvox_api_m_pb2.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-SUB_API: float = 10.0
+SUB_API: float = 10.0  # redvox-api-1000 -> build_protos.sh -> insert_sub_api.py on 2022-07-07 00:07:12.686182
 
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: redvox_api_m.proto
+# source: src/redvox_api_m/redvox_api_m.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12redvox_api_m.proto\x12\x0credvox_api_m\"\xecs\n\rRedvoxPacketM\x12\x0b\n\x03\x61pi\x18\x01 \x01(\x02\x12\x0f\n\x07sub_api\x18\x02 \x01(\x02\x12K\n\x13station_information\x18\x03 \x01(\x0b\x32..redvox_api_m.RedvoxPacketM.StationInformation\x12I\n\x12timing_information\x18\x04 \x01(\x0b\x32-.redvox_api_m.RedvoxPacketM.TimingInformation\x12\x34\n\x07sensors\x18\x05 \x01(\x0b\x32#.redvox_api_m.RedvoxPacketM.Sensors\x12>\n\revent_streams\x18\x06 \x03(\x0b\x32\'.redvox_api_m.RedvoxPacketM.EventStream\x12;\n\x08metadata\x18\x07 \x03(\x0b\x32).redvox_api_m.RedvoxPacketM.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xd1$\n\x12StationInformation\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04uuid\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0f\n\x07\x61uth_id\x18\x04 \x01(\t\x12\x0c\n\x04make\x18\x05 \x01(\t\x12\r\n\x05model\x18\x06 \x01(\t\x12\x41\n\x02os\x18\x07 \x01(\x0e\x32\x35.redvox_api_m.RedvoxPacketM.StationInformation.OsType\x12\x12\n\nos_version\x18\x08 \x01(\t\x12\x13\n\x0b\x61pp_version\x18\t \x01(\t\x12\x12\n\nis_private\x18\n \x01(\x08\x12P\n\x0c\x61pp_settings\x18\x0b \x01(\x0b\x32:.redvox_api_m.RedvoxPacketM.StationInformation.AppSettings\x12V\n\x0fstation_metrics\x18\x0c \x01(\x0b\x32=.redvox_api_m.RedvoxPacketM.StationInformation.StationMetrics\x12P\n\x0cservice_urls\x18\r \x01(\x0b\x32:.redvox_api_m.RedvoxPacketM.StationInformation.ServiceUrls\x12N\n\x08metadata\x18\x0e \x03(\x0b\x32<.redvox_api_m.RedvoxPacketM.StationInformation.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xe1\x01\n\x0bServiceUrls\x12\x13\n\x0b\x61uth_server\x18\x01 \x01(\t\x12\x14\n\x0csynch_server\x18\x02 \x01(\t\x12\x1a\n\x12\x61\x63quisition_server\x18\x03 \x01(\t\x12Z\n\x08metadata\x18\x04 \x03(\x0b\x32H.redvox_api_m.RedvoxPacketM.StationInformation.ServiceUrls.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xf9\x0c\n\x0eStationMetrics\x12=\n\ntimestamps\x18\x01 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.TimingPayload\x12_\n\x0cnetwork_type\x18\x02 \x03(\x0e\x32I.redvox_api_m.RedvoxPacketM.StationInformation.StationMetrics.NetworkType\x12j\n\x12\x63\x65ll_service_state\x18\x03 \x03(\x0e\x32N.redvox_api_m.RedvoxPacketM.StationInformation.StationMetrics.CellServiceState\x12\x43\n\x10network_strength\x18\x04 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12>\n\x0btemperature\x18\x05 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12:\n\x07\x62\x61ttery\x18\x06 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12\x42\n\x0f\x62\x61ttery_current\x18\x07 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12@\n\ravailable_ram\x18\x08 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12\x41\n\x0e\x61vailable_disk\x18\t \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12\x42\n\x0f\x63pu_utilization\x18\n \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12]\n\x0bpower_state\x18\x0b \x03(\x0e\x32H.redvox_api_m.RedvoxPacketM.StationInformation.StationMetrics.PowerState\x12\x62\n\x0ewifi_wake_lock\x18\x0c \x03(\x0e\x32J.redvox_api_m.RedvoxPacketM.StationInformation.StationMetrics.WifiWakeLock\x12_\n\x0cscreen_state\x18\r \x03(\x0e\x32I.redvox_api_m.RedvoxPacketM.StationInformation.StationMetrics.ScreenState\x12\x44\n\x11screen_brightness\x18\x0e \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12]\n\x08metadata\x18\x0f \x03(\x0b\x32K.redvox_api_m.RedvoxPacketM.StationInformation.StationMetrics.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"U\n\x0bNetworkType\x12\x13\n\x0fUNKNOWN_NETWORK\x10\x00\x12\x0e\n\nNO_NETWORK\x10\x01\x12\x08\n\x04WIFI\x10\x02\x12\x0c\n\x08\x43\x45LLULAR\x10\x03\x12\t\n\x05WIRED\x10\x04\"C\n\x0cWifiWakeLock\x12\x08\n\x04NONE\x10\x00\x12\r\n\tHIGH_PERF\x10\x01\x12\x0f\n\x0bLOW_LATENCY\x10\x02\x12\t\n\x05OTHER\x10\x03\"^\n\x10\x43\x65llServiceState\x12\x0b\n\x07UNKNOWN\x10\x00\x12\r\n\tEMERGENCY\x10\x01\x12\x0b\n\x07NOMINAL\x10\x02\x12\x12\n\x0eOUT_OF_SERVICE\x10\x03\x12\r\n\tPOWER_OFF\x10\x04\"O\n\nPowerState\x12\x17\n\x13UNKNOWN_POWER_STATE\x10\x00\x12\r\n\tUNPLUGGED\x10\x01\x12\x0c\n\x08\x43HARGING\x10\x02\x12\x0b\n\x07\x43HARGED\x10\x03\"F\n\x0bScreenState\x12\x18\n\x14UNKNOWN_SCREEN_STATE\x10\x00\x12\x06\n\x02ON\x10\x01\x12\x07\n\x03OFF\x10\x02\x12\x0c\n\x08HEADLESS\x10\x03\x1a\xe9\x0f\n\x0b\x41ppSettings\x12i\n\x13\x61udio_sampling_rate\x18\x01 \x01(\x0e\x32L.redvox_api_m.RedvoxPacketM.StationInformation.AppSettings.AudioSamplingRate\x12\x1a\n\x12samples_per_window\x18\x02 \x01(\x02\x12i\n\x13\x61udio_source_tuning\x18\x03 \x01(\x0e\x32L.redvox_api_m.RedvoxPacketM.StationInformation.AppSettings.AudioSourceTuning\x12h\n\x18\x61\x64\x64itional_input_sensors\x18\x04 \x03(\x0e\x32\x46.redvox_api_m.RedvoxPacketM.StationInformation.AppSettings.InputSensor\x12\x1c\n\x14\x61utomatically_record\x18\x05 \x01(\x08\x12\x1a\n\x12launch_at_power_up\x18\x06 \x01(\x08\x12\x12\n\nstation_id\x18\x07 \x01(\t\x12\x1b\n\x13station_description\x18\x08 \x01(\t\x12\x16\n\x0epush_to_server\x18\t \x01(\x08\x12\x1f\n\x17publish_data_as_private\x18\n \x01(\x08\x12\x1b\n\x13scramble_audio_data\x18\x0b \x01(\x08\x12\x18\n\x10provide_backfill\x18\x0c \x01(\x08\x12\x1f\n\x17remove_sensor_dc_offset\x18\r \x01(\x08\x12Z\n\x0b\x66\x66t_overlap\x18\x0e \x01(\x0e\x32\x45.redvox_api_m.RedvoxPacketM.StationInformation.AppSettings.FftOverlap\x12#\n\x1buse_custom_time_sync_server\x18\x0f \x01(\x08\x12\x1c\n\x14time_sync_server_url\x18\x10 \x01(\t\x12\x1e\n\x16use_custom_data_server\x18\x11 \x01(\x08\x12\x17\n\x0f\x64\x61ta_server_url\x18\x12 \x01(\t\x12\x1e\n\x16use_custom_auth_server\x18\x13 \x01(\x08\x12\x17\n\x0f\x61uth_server_url\x18\x14 \x01(\t\x12\x1e\n\x16\x61uto_delete_data_files\x18\x15 \x01(\x08\x12\x1f\n\x17storage_space_allowance\x18\x16 \x01(\x02\x12$\n\x1cuse_sd_card_for_data_storage\x18\x17 \x01(\x08\x12\x1d\n\x15use_location_services\x18\x18 \x01(\x08\x12\x14\n\x0cuse_latitude\x18\x19 \x01(\x01\x12\x15\n\ruse_longitude\x18\x1a \x01(\x01\x12\x14\n\x0cuse_altitude\x18\x1b \x01(\x02\x12P\n\x0cmetrics_rate\x18\x1c \x01(\x0e\x32:.redvox_api_m.RedvoxPacketM.StationInformation.MetricsRate\x12Z\n\x08metadata\x18\x1d \x03(\x0b\x32H.redvox_api_m.RedvoxPacketM.StationInformation.AppSettings.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"I\n\nFftOverlap\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0e\n\nPERCENT_25\x10\x01\x12\x0e\n\nPERCENT_50\x10\x02\x12\x0e\n\nPERCENT_75\x10\x03\"n\n\x11\x41udioSamplingRate\x12\x19\n\x15UNKNOWN_SAMPLING_RATE\x10\x00\x12\t\n\x05HZ_80\x10\x01\x12\n\n\x06HZ_800\x10\x02\x12\x0b\n\x07HZ_8000\x10\x03\x12\x0c\n\x08HZ_16000\x10\x04\x12\x0c\n\x08HZ_48000\x10\x05\"f\n\x11\x41udioSourceTuning\x12\x12\n\x0eUNKNOWN_TUNING\x10\x00\x12\x15\n\x11INFRASOUND_TUNING\x10\x01\x12\x14\n\x10LOW_AUDIO_TUNING\x10\x02\x12\x10\n\x0c\x41UDIO_TUNING\x10\x03\"\xa5\x03\n\x0bInputSensor\x12\x12\n\x0eUNKNOWN_SENSOR\x10\x00\x12\x11\n\rACCELEROMETER\x10\x01\x12\x16\n\x12\x41\x43\x43\x45LEROMETER_FAST\x10\x02\x12\x17\n\x13\x41MBIENT_TEMPERATURE\x10\x03\x12\t\n\x05\x41UDIO\x10\x04\x12\x14\n\x10\x43OMPRESSED_AUDIO\x10\x05\x12\x0b\n\x07GRAVITY\x10\x06\x12\r\n\tGYROSCOPE\x10\x07\x12\x12\n\x0eGYROSCOPE_FAST\x10\x08\x12\x14\n\x10IMAGE_PER_SECOND\x10\t\x12\x14\n\x10IMAGE_PER_PACKET\x10\n\x12\t\n\x05LIGHT\x10\x0b\x12\x17\n\x13LINEAR_ACCELERATION\x10\x0c\x12\x0c\n\x08LOCATION\x10\r\x12\x10\n\x0cMAGNETOMETER\x10\x0e\x12\x15\n\x11MAGNETOMETER_FAST\x10\x0f\x12\x0f\n\x0bORIENTATION\x10\x10\x12\x0c\n\x08PRESSURE\x10\x11\x12\r\n\tPROXIMITY\x10\x12\x12\x15\n\x11RELATIVE_HUMIDITY\x10\x13\x12\x13\n\x0fROTATION_VECTOR\x10\x14\x12\x0c\n\x08VELOCITY\x10\x15\"O\n\x06OsType\x12\x0e\n\nUNKNOWN_OS\x10\x00\x12\x0b\n\x07\x41NDROID\x10\x01\x12\x07\n\x03IOS\x10\x02\x12\x07\n\x03OSX\x10\x03\x12\t\n\x05LINUX\x10\x04\x12\x0b\n\x07WINDOWS\x10\x05\"D\n\x0bMetricsRate\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x13\n\x0fONCE_PER_SECOND\x10\x01\x12\x13\n\x0fONCE_PER_PACKET\x10\x02\x1a\xc0\x07\n\x11TimingInformation\x12!\n\x19packet_start_os_timestamp\x18\x01 \x01(\x01\x12#\n\x1bpacket_start_mach_timestamp\x18\x02 \x01(\x01\x12\x1f\n\x17packet_end_os_timestamp\x18\x03 \x01(\x01\x12!\n\x19packet_end_mach_timestamp\x18\x04 \x01(\x01\x12,\n$server_acquisition_arrival_timestamp\x18\x05 \x01(\x01\x12 \n\x18\x61pp_start_mach_timestamp\x18\x06 \x01(\x01\x12T\n\x0fsynch_exchanges\x18\x07 \x03(\x0b\x32;.redvox_api_m.RedvoxPacketM.TimingInformation.SynchExchange\x12\x14\n\x0c\x62\x65st_latency\x18\x08 \x01(\x02\x12\x13\n\x0b\x62\x65st_offset\x18\t \x01(\x02\x12\r\n\x05score\x18\n \x01(\x02\x12U\n\x0cscore_method\x18\x0b \x01(\x0e\x32?.redvox_api_m.RedvoxPacketM.TimingInformation.TimingScoreMethod\x12.\n\x04unit\x18\x0c \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12M\n\x08metadata\x18\r \x03(\x0b\x32;.redvox_api_m.RedvoxPacketM.TimingInformation.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x95\x02\n\rSynchExchange\x12\n\n\x02\x61\x31\x18\x01 \x01(\x01\x12\n\n\x02\x61\x32\x18\x02 \x01(\x01\x12\n\n\x02\x61\x33\x18\x03 \x01(\x01\x12\n\n\x02\x62\x31\x18\x04 \x01(\x01\x12\n\n\x02\x62\x32\x18\x05 \x01(\x01\x12\n\n\x02\x62\x33\x18\x06 \x01(\x01\x12.\n\x04unit\x18\x07 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12[\n\x08metadata\x18\x08 \x03(\x0b\x32I.redvox_api_m.RedvoxPacketM.TimingInformation.SynchExchange.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\" \n\x11TimingScoreMethod\x12\x0b\n\x07UNKNOWN\x10\x00\x1a\xa8\x30\n\x07Sensors\x12>\n\raccelerometer\x18\x01 \x01(\x0b\x32\'.redvox_api_m.RedvoxPacketM.Sensors.Xyz\x12G\n\x13\x61mbient_temperature\x18\x02 \x01(\x0b\x32*.redvox_api_m.RedvoxPacketM.Sensors.Single\x12\x38\n\x05\x61udio\x18\x03 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.Sensors.Audio\x12M\n\x10\x63ompressed_audio\x18\x04 \x01(\x0b\x32\x33.redvox_api_m.RedvoxPacketM.Sensors.CompressedAudio\x12\x38\n\x07gravity\x18\x05 \x01(\x0b\x32\'.redvox_api_m.RedvoxPacketM.Sensors.Xyz\x12:\n\tgyroscope\x18\x06 \x01(\x0b\x32\'.redvox_api_m.RedvoxPacketM.Sensors.Xyz\x12\x38\n\x05image\x18\x07 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.Sensors.Image\x12\x39\n\x05light\x18\x08 \x01(\x0b\x32*.redvox_api_m.RedvoxPacketM.Sensors.Single\x12\x44\n\x13linear_acceleration\x18\t \x01(\x0b\x32\'.redvox_api_m.RedvoxPacketM.Sensors.Xyz\x12>\n\x08location\x18\n \x01(\x0b\x32,.redvox_api_m.RedvoxPacketM.Sensors.Location\x12=\n\x0cmagnetometer\x18\x0b \x01(\x0b\x32\'.redvox_api_m.RedvoxPacketM.Sensors.Xyz\x12<\n\x0borientation\x18\x0c \x01(\x0b\x32\'.redvox_api_m.RedvoxPacketM.Sensors.Xyz\x12<\n\x08pressure\x18\r \x01(\x0b\x32*.redvox_api_m.RedvoxPacketM.Sensors.Single\x12=\n\tproximity\x18\x0e \x01(\x0b\x32*.redvox_api_m.RedvoxPacketM.Sensors.Single\x12\x45\n\x11relative_humidity\x18\x0f \x01(\x0b\x32*.redvox_api_m.RedvoxPacketM.Sensors.Single\x12@\n\x0frotation_vector\x18\x10 \x01(\x0b\x32\'.redvox_api_m.RedvoxPacketM.Sensors.Xyz\x12\x39\n\x08velocity\x18\x11 \x01(\x0b\x32\'.redvox_api_m.RedvoxPacketM.Sensors.Xyz\x12\x43\n\x08metadata\x18\x12 \x03(\x0b\x32\x31.redvox_api_m.RedvoxPacketM.Sensors.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xd3\x02\n\x05\x41udio\x12\x1a\n\x12sensor_description\x18\x01 \x01(\t\x12\x1e\n\x16\x66irst_sample_timestamp\x18\x02 \x01(\x01\x12\x13\n\x0bsample_rate\x18\x03 \x01(\x02\x12\x19\n\x11\x62its_of_precision\x18\x04 \x01(\x02\x12\x14\n\x0cis_scrambled\x18\x05 \x01(\x08\x12\x10\n\x08\x65ncoding\x18\x06 \x01(\t\x12:\n\x07samples\x18\x07 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12I\n\x08metadata\x18\x08 \x03(\x0b\x32\x37.redvox_api_m.RedvoxPacketM.Sensors.Audio.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x8d\x03\n\x0f\x43ompressedAudio\x12\x1a\n\x12sensor_description\x18\x01 \x01(\t\x12\x1e\n\x16\x66irst_sample_timestamp\x18\x02 \x01(\x01\x12\x13\n\x0bsample_rate\x18\x03 \x01(\x02\x12\x14\n\x0cis_scrambled\x18\x04 \x01(\x08\x12\x13\n\x0b\x61udio_bytes\x18\x05 \x01(\x0c\x12S\n\x0b\x61udio_codec\x18\x06 \x01(\x0e\x32>.redvox_api_m.RedvoxPacketM.Sensors.CompressedAudio.AudioCodec\x12S\n\x08metadata\x18\x07 \x03(\x0b\x32\x41.redvox_api_m.RedvoxPacketM.Sensors.CompressedAudio.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"#\n\nAudioCodec\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04\x46LAC\x10\x01\x1a\x9c\x02\n\x06Single\x12\x1a\n\x12sensor_description\x18\x01 \x01(\t\x12=\n\ntimestamps\x18\x02 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.TimingPayload\x12:\n\x07samples\x18\x03 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12J\n\x08metadata\x18\x04 \x03(\x0b\x32\x38.redvox_api_m.RedvoxPacketM.Sensors.Single.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xd6\x18\n\x08Location\x12\x1a\n\x12sensor_description\x18\x01 \x01(\t\x12=\n\ntimestamps\x18\x02 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.TimingPayload\x12\x41\n\x0etimestamps_gps\x18\x03 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.TimingPayload\x12I\n\x10latitude_samples\x18\x04 \x01(\x0b\x32/.redvox_api_m.RedvoxPacketM.DoubleSamplePayload\x12J\n\x11longitude_samples\x18\x05 \x01(\x0b\x32/.redvox_api_m.RedvoxPacketM.DoubleSamplePayload\x12\x43\n\x10\x61ltitude_samples\x18\x06 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12@\n\rspeed_samples\x18\x07 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12\x42\n\x0f\x62\x65\x61ring_samples\x18\x08 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12N\n\x1bhorizontal_accuracy_samples\x18\t \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12L\n\x19vertical_accuracy_samples\x18\n \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12I\n\x16speed_accuracy_samples\x18\x0b \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12K\n\x18\x62\x65\x61ring_accuracy_samples\x18\x0c \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12U\n\x12last_best_location\x18\r \x01(\x0b\x32\x39.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation\x12X\n\x15overall_best_location\x18\x0e \x01(\x0b\x32\x39.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation\x12$\n\x1clocation_permissions_granted\x18\x0f \x01(\x08\x12#\n\x1blocation_services_requested\x18\x10 \x01(\x08\x12!\n\x19location_services_enabled\x18\x11 \x01(\x08\x12Y\n\x12location_providers\x18\x12 \x03(\x0e\x32=.redvox_api_m.RedvoxPacketM.Sensors.Location.LocationProvider\x12L\n\x08metadata\x18\x13 \x03(\x0b\x32:.redvox_api_m.RedvoxPacketM.Sensors.Location.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xcf\r\n\x0c\x42\x65stLocation\x12m\n\x1clatitude_longitude_timestamp\x18\x01 \x01(\x0b\x32G.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation.BestTimestamp\x12\x63\n\x12\x61ltitude_timestamp\x18\x02 \x01(\x0b\x32G.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation.BestTimestamp\x12`\n\x0fspeed_timestamp\x18\x03 \x01(\x0b\x32G.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation.BestTimestamp\x12\x62\n\x11\x62\x65\x61ring_timestamp\x18\x04 \x01(\x0b\x32G.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation.BestTimestamp\x12\x41\n\x17latitude_longitude_unit\x18\x05 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x37\n\raltitude_unit\x18\x06 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x34\n\nspeed_unit\x18\x07 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x36\n\x0c\x62\x65\x61ring_unit\x18\x08 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12@\n\x16vertical_accuracy_unit\x18\t \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x42\n\x18horizontal_accuracy_unit\x18\n \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12=\n\x13speed_accuracy_unit\x18\x0b \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12?\n\x15\x62\x65\x61ring_accuracy_unit\x18\x0c \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x10\n\x08latitude\x18\r \x01(\x01\x12\x11\n\tlongitude\x18\x0e \x01(\x01\x12\x10\n\x08\x61ltitude\x18\x0f \x01(\x02\x12\r\n\x05speed\x18\x10 \x01(\x02\x12\x0f\n\x07\x62\x65\x61ring\x18\x11 \x01(\x02\x12\x19\n\x11vertical_accuracy\x18\x12 \x01(\x02\x12\x1b\n\x13horizontal_accuracy\x18\x13 \x01(\x02\x12\x16\n\x0espeed_accuracy\x18\x14 \x01(\x02\x12\x18\n\x10\x62\x65\x61ring_accuracy\x18\x15 \x01(\x02\x12\r\n\x05score\x18\x16 \x01(\x02\x12]\n\x06method\x18\x17 \x01(\x0e\x32M.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation.LocationScoreMethod\x12X\n\x11location_provider\x18\x18 \x01(\x0e\x32=.redvox_api_m.RedvoxPacketM.Sensors.Location.LocationProvider\x12Y\n\x08metadata\x18\x19 \x03(\x0b\x32G.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xf4\x01\n\rBestTimestamp\x12.\n\x04unit\x18\x01 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x0c\n\x04mach\x18\x02 \x01(\x01\x12\x0b\n\x03gps\x18\x03 \x01(\x01\x12g\n\x08metadata\x18\x04 \x03(\x0b\x32U.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation.BestTimestamp.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\")\n\x13LocationScoreMethod\x12\x12\n\x0eUNKNOWN_METHOD\x10\x00\"I\n\x10LocationProvider\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04NONE\x10\x01\x12\x08\n\x04USER\x10\x02\x12\x07\n\x03GPS\x10\x03\x12\x0b\n\x07NETWORK\x10\x04\x1a\x94\x03\n\x03Xyz\x12\x1a\n\x12sensor_description\x18\x01 \x01(\t\x12=\n\ntimestamps\x18\x02 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.TimingPayload\x12<\n\tx_samples\x18\x03 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12<\n\ty_samples\x18\x04 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12<\n\tz_samples\x18\x05 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12G\n\x08metadata\x18\x06 \x03(\x0b\x32\x35.redvox_api_m.RedvoxPacketM.Sensors.Xyz.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xf0\x02\n\x05Image\x12\x1a\n\x12sensor_description\x18\x01 \x01(\t\x12=\n\ntimestamps\x18\x02 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.TimingPayload\x12\x0f\n\x07samples\x18\x03 \x03(\x0c\x12I\n\x0bimage_codec\x18\x04 \x01(\x0e\x32\x34.redvox_api_m.RedvoxPacketM.Sensors.Image.ImageCodec\x12I\n\x08metadata\x18\x05 \x03(\x0b\x32\x37.redvox_api_m.RedvoxPacketM.Sensors.Image.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"4\n\nImageCodec\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03PNG\x10\x01\x12\x07\n\x03JPG\x10\x02\x12\x07\n\x03\x42MP\x10\x03\x1a\xf2\x07\n\x0b\x45ventStream\x12\x0c\n\x04name\x18\x01 \x01(\t\x12=\n\ntimestamps\x18\x02 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.TimingPayload\x12=\n\x06\x65vents\x18\x03 \x03(\x0b\x32-.redvox_api_m.RedvoxPacketM.EventStream.Event\x12G\n\x08metadata\x18\x04 \x03(\x0b\x32\x35.redvox_api_m.RedvoxPacketM.EventStream.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xdc\x05\n\x05\x45vent\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12X\n\x0estring_payload\x18\x02 \x03(\x0b\x32@.redvox_api_m.RedvoxPacketM.EventStream.Event.StringPayloadEntry\x12Z\n\x0fnumeric_payload\x18\x03 \x03(\x0b\x32\x41.redvox_api_m.RedvoxPacketM.EventStream.Event.NumericPayloadEntry\x12Z\n\x0f\x62oolean_payload\x18\x04 \x03(\x0b\x32\x41.redvox_api_m.RedvoxPacketM.EventStream.Event.BooleanPayloadEntry\x12T\n\x0c\x62yte_payload\x18\x05 \x03(\x0b\x32>.redvox_api_m.RedvoxPacketM.EventStream.Event.BytePayloadEntry\x12M\n\x08metadata\x18\x06 \x03(\x0b\x32;.redvox_api_m.RedvoxPacketM.EventStream.Event.MetadataEntry\x1a\x34\n\x12StringPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x35\n\x13NumericPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01:\x02\x38\x01\x1a\x35\n\x13\x42ooleanPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x08:\x02\x38\x01\x1a\x32\n\x10\x42ytePayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x94\x02\n\rSamplePayload\x12.\n\x04unit\x18\x01 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x0e\n\x06values\x18\x02 \x03(\x02\x12G\n\x10value_statistics\x18\x03 \x01(\x0b\x32-.redvox_api_m.RedvoxPacketM.SummaryStatistics\x12I\n\x08metadata\x18\x04 \x03(\x0b\x32\x37.redvox_api_m.RedvoxPacketM.SamplePayload.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xa0\x02\n\x13\x44oubleSamplePayload\x12.\n\x04unit\x18\x01 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x0e\n\x06values\x18\x02 \x03(\x01\x12G\n\x10value_statistics\x18\x03 \x01(\x0b\x32-.redvox_api_m.RedvoxPacketM.SummaryStatistics\x12O\n\x08metadata\x18\x04 \x03(\x0b\x32=.redvox_api_m.RedvoxPacketM.DoubleSamplePayload.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xd1\x02\n\rTimingPayload\x12.\n\x04unit\x18\x01 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x12\n\ntimestamps\x18\x02 \x03(\x01\x12K\n\x14timestamp_statistics\x18\x03 \x01(\x0b\x32-.redvox_api_m.RedvoxPacketM.SummaryStatistics\x12\x18\n\x10mean_sample_rate\x18\x04 \x01(\x02\x12\x19\n\x11stdev_sample_rate\x18\x05 \x01(\x02\x12I\n\x08metadata\x18\x06 \x03(\x0b\x32\x37.redvox_api_m.RedvoxPacketM.TimingPayload.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xf5\x01\n\x11SummaryStatistics\x12\r\n\x05\x63ount\x18\x01 \x01(\x01\x12\x0c\n\x04mean\x18\x02 \x01(\x01\x12\x1a\n\x12standard_deviation\x18\x03 \x01(\x01\x12\x0b\n\x03min\x18\x04 \x01(\x01\x12\x0b\n\x03max\x18\x05 \x01(\x01\x12\r\n\x05range\x18\x06 \x01(\x01\x12M\n\x08metadata\x18\x07 \x03(\x0b\x32;.redvox_api_m.RedvoxPacketM.SummaryStatistics.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x83\x03\n\x04Unit\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x1d\n\x19METERS_PER_SECOND_SQUARED\x10\x01\x12\x0e\n\nKILOPASCAL\x10\x02\x12\x16\n\x12RADIANS_PER_SECOND\x10\x03\x12\x13\n\x0f\x44\x45\x43IMAL_DEGREES\x10\x04\x12\n\n\x06METERS\x10\x05\x12\x15\n\x11METERS_PER_SECOND\x10\x06\x12\x0e\n\nMICROTESLA\x10\x07\x12\x19\n\x15LSB_PLUS_MINUS_COUNTS\x10\x08\x12!\n\x1dMICROSECONDS_SINCE_UNIX_EPOCH\x10\t\x12\x0b\n\x07\x44\x45\x43IBEL\x10\n\x12\x13\n\x0f\x44\x45GREES_CELSIUS\x10\x0b\x12\x08\n\x04\x42YTE\x10\x0c\x12\x0e\n\nPERCENTAGE\x10\r\x12\x0b\n\x07RADIANS\x10\x0e\x12\x10\n\x0cMICROAMPERES\x10\x0f\x12\x0f\n\x0b\x43\x45NTIMETERS\x10\x10\x12\x15\n\x11NORMALIZED_COUNTS\x10\x11\x12\x07\n\x03LUX\x10\x12\x12\x0c\n\x08UNITLESS\x10\x13\x12\x07\n\x03PCM\x10\x14\"\xac\x01\n\x16\x45ncryptedRedvoxPacketM\x12\x0e\n\x06header\x18\x01 \x01(\x0c\x12\x0e\n\x06packet\x18\x02 \x01(\x0c\x1ar\n\x06Header\x12\x12\n\nstation_id\x18\x01 \x01(\t\x12\x14\n\x0cstation_uuid\x18\x02 \x01(\t\x12\x12\n\nauth_token\x18\x03 \x01(\t\x12\x16\n\x0e\x66irebase_token\x18\x04 \x01(\t\x12\x12\n\nauth_email\x18\x05 \x01(\t\"\x89\x01\n\x12\x41\x63quisitionRequest\x12\x12\n\nauth_token\x18\x01 \x01(\t\x12\x16\n\x0e\x66irebase_token\x18\x02 \x01(\t\x12\x10\n\x08\x63hecksum\x18\x03 \x01(\x03\x12\x14\n\x0cis_encrypted\x18\x04 \x01(\x08\x12\x0f\n\x07payload\x18\x05 \x01(\x0c\x12\x0e\n\x06seq_id\x18\x06 \x01(\x03\"\xf5\x01\n\x13\x41\x63quisitionResponse\x12\x45\n\rresponse_type\x18\x01 \x01(\x0e\x32..redvox_api_m.AcquisitionResponse.ResponseType\x12\x10\n\x08\x63hecksum\x18\x02 \x01(\x03\x12\x0f\n\x07\x64\x65tails\x18\x03 \x01(\t\x12\x0e\n\x06resend\x18\x04 \x01(\x08\x12\x0e\n\x06seq_id\x18\x05 \x01(\x03\"T\n\x0cResponseType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x06\n\x02OK\x10\x01\x12\x0e\n\nAUTH_ERROR\x10\x02\x12\x0e\n\nDATA_ERROR\x10\x03\x12\x0f\n\x0bOTHER_ERROR\x10\x04\"\\\n\x0cSynchRequest\x12\x12\n\nstation_id\x18\x01 \x01(\t\x12\x14\n\x0cstation_uuid\x18\x02 \x01(\t\x12\x0e\n\x06seq_id\x18\x03 \x01(\r\x12\x12\n\nsub_seq_id\x18\x04 \x01(\r\"\x85\x01\n\rSynchResponse\x12\x12\n\nstation_id\x18\x01 \x01(\t\x12\x14\n\x0cstation_uuid\x18\x02 \x01(\t\x12\x0e\n\x06seq_id\x18\x03 \x01(\r\x12\x12\n\nsub_seq_id\x18\x04 \x01(\r\x12\x12\n\nrecv_ts_us\x18\x05 \x01(\x04\x12\x12\n\nsend_ts_us\x18\x06 \x01(\x04\x42\x10\n\x0eio.redvox.apisb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#src/redvox_api_m/redvox_api_m.proto\x12\x0credvox_api_m\"\xecs\n\rRedvoxPacketM\x12\x0b\n\x03\x61pi\x18\x01 \x01(\x02\x12\x0f\n\x07sub_api\x18\x02 \x01(\x02\x12K\n\x13station_information\x18\x03 \x01(\x0b\x32..redvox_api_m.RedvoxPacketM.StationInformation\x12I\n\x12timing_information\x18\x04 \x01(\x0b\x32-.redvox_api_m.RedvoxPacketM.TimingInformation\x12\x34\n\x07sensors\x18\x05 \x01(\x0b\x32#.redvox_api_m.RedvoxPacketM.Sensors\x12>\n\revent_streams\x18\x06 \x03(\x0b\x32\'.redvox_api_m.RedvoxPacketM.EventStream\x12;\n\x08metadata\x18\x07 \x03(\x0b\x32).redvox_api_m.RedvoxPacketM.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xd1$\n\x12StationInformation\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04uuid\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0f\n\x07\x61uth_id\x18\x04 \x01(\t\x12\x0c\n\x04make\x18\x05 \x01(\t\x12\r\n\x05model\x18\x06 \x01(\t\x12\x41\n\x02os\x18\x07 \x01(\x0e\x32\x35.redvox_api_m.RedvoxPacketM.StationInformation.OsType\x12\x12\n\nos_version\x18\x08 \x01(\t\x12\x13\n\x0b\x61pp_version\x18\t \x01(\t\x12\x12\n\nis_private\x18\n \x01(\x08\x12P\n\x0c\x61pp_settings\x18\x0b \x01(\x0b\x32:.redvox_api_m.RedvoxPacketM.StationInformation.AppSettings\x12V\n\x0fstation_metrics\x18\x0c \x01(\x0b\x32=.redvox_api_m.RedvoxPacketM.StationInformation.StationMetrics\x12P\n\x0cservice_urls\x18\r \x01(\x0b\x32:.redvox_api_m.RedvoxPacketM.StationInformation.ServiceUrls\x12N\n\x08metadata\x18\x0e \x03(\x0b\x32<.redvox_api_m.RedvoxPacketM.StationInformation.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xe1\x01\n\x0bServiceUrls\x12\x13\n\x0b\x61uth_server\x18\x01 \x01(\t\x12\x14\n\x0csynch_server\x18\x02 \x01(\t\x12\x1a\n\x12\x61\x63quisition_server\x18\x03 \x01(\t\x12Z\n\x08metadata\x18\x04 \x03(\x0b\x32H.redvox_api_m.RedvoxPacketM.StationInformation.ServiceUrls.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xf9\x0c\n\x0eStationMetrics\x12=\n\ntimestamps\x18\x01 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.TimingPayload\x12_\n\x0cnetwork_type\x18\x02 \x03(\x0e\x32I.redvox_api_m.RedvoxPacketM.StationInformation.StationMetrics.NetworkType\x12j\n\x12\x63\x65ll_service_state\x18\x03 \x03(\x0e\x32N.redvox_api_m.RedvoxPacketM.StationInformation.StationMetrics.CellServiceState\x12\x43\n\x10network_strength\x18\x04 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12>\n\x0btemperature\x18\x05 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12:\n\x07\x62\x61ttery\x18\x06 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12\x42\n\x0f\x62\x61ttery_current\x18\x07 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12@\n\ravailable_ram\x18\x08 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12\x41\n\x0e\x61vailable_disk\x18\t \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12\x42\n\x0f\x63pu_utilization\x18\n \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12]\n\x0bpower_state\x18\x0b \x03(\x0e\x32H.redvox_api_m.RedvoxPacketM.StationInformation.StationMetrics.PowerState\x12\x62\n\x0ewifi_wake_lock\x18\x0c \x03(\x0e\x32J.redvox_api_m.RedvoxPacketM.StationInformation.StationMetrics.WifiWakeLock\x12_\n\x0cscreen_state\x18\r \x03(\x0e\x32I.redvox_api_m.RedvoxPacketM.StationInformation.StationMetrics.ScreenState\x12\x44\n\x11screen_brightness\x18\x0e \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12]\n\x08metadata\x18\x0f \x03(\x0b\x32K.redvox_api_m.RedvoxPacketM.StationInformation.StationMetrics.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"U\n\x0bNetworkType\x12\x13\n\x0fUNKNOWN_NETWORK\x10\x00\x12\x0e\n\nNO_NETWORK\x10\x01\x12\x08\n\x04WIFI\x10\x02\x12\x0c\n\x08\x43\x45LLULAR\x10\x03\x12\t\n\x05WIRED\x10\x04\"C\n\x0cWifiWakeLock\x12\x08\n\x04NONE\x10\x00\x12\r\n\tHIGH_PERF\x10\x01\x12\x0f\n\x0bLOW_LATENCY\x10\x02\x12\t\n\x05OTHER\x10\x03\"^\n\x10\x43\x65llServiceState\x12\x0b\n\x07UNKNOWN\x10\x00\x12\r\n\tEMERGENCY\x10\x01\x12\x0b\n\x07NOMINAL\x10\x02\x12\x12\n\x0eOUT_OF_SERVICE\x10\x03\x12\r\n\tPOWER_OFF\x10\x04\"O\n\nPowerState\x12\x17\n\x13UNKNOWN_POWER_STATE\x10\x00\x12\r\n\tUNPLUGGED\x10\x01\x12\x0c\n\x08\x43HARGING\x10\x02\x12\x0b\n\x07\x43HARGED\x10\x03\"F\n\x0bScreenState\x12\x18\n\x14UNKNOWN_SCREEN_STATE\x10\x00\x12\x06\n\x02ON\x10\x01\x12\x07\n\x03OFF\x10\x02\x12\x0c\n\x08HEADLESS\x10\x03\x1a\xe9\x0f\n\x0b\x41ppSettings\x12i\n\x13\x61udio_sampling_rate\x18\x01 \x01(\x0e\x32L.redvox_api_m.RedvoxPacketM.StationInformation.AppSettings.AudioSamplingRate\x12\x1a\n\x12samples_per_window\x18\x02 \x01(\x02\x12i\n\x13\x61udio_source_tuning\x18\x03 \x01(\x0e\x32L.redvox_api_m.RedvoxPacketM.StationInformation.AppSettings.AudioSourceTuning\x12h\n\x18\x61\x64\x64itional_input_sensors\x18\x04 \x03(\x0e\x32\x46.redvox_api_m.RedvoxPacketM.StationInformation.AppSettings.InputSensor\x12\x1c\n\x14\x61utomatically_record\x18\x05 \x01(\x08\x12\x1a\n\x12launch_at_power_up\x18\x06 \x01(\x08\x12\x12\n\nstation_id\x18\x07 \x01(\t\x12\x1b\n\x13station_description\x18\x08 \x01(\t\x12\x16\n\x0epush_to_server\x18\t \x01(\x08\x12\x1f\n\x17publish_data_as_private\x18\n \x01(\x08\x12\x1b\n\x13scramble_audio_data\x18\x0b \x01(\x08\x12\x18\n\x10provide_backfill\x18\x0c \x01(\x08\x12\x1f\n\x17remove_sensor_dc_offset\x18\r \x01(\x08\x12Z\n\x0b\x66\x66t_overlap\x18\x0e \x01(\x0e\x32\x45.redvox_api_m.RedvoxPacketM.StationInformation.AppSettings.FftOverlap\x12#\n\x1buse_custom_time_sync_server\x18\x0f \x01(\x08\x12\x1c\n\x14time_sync_server_url\x18\x10 \x01(\t\x12\x1e\n\x16use_custom_data_server\x18\x11 \x01(\x08\x12\x17\n\x0f\x64\x61ta_server_url\x18\x12 \x01(\t\x12\x1e\n\x16use_custom_auth_server\x18\x13 \x01(\x08\x12\x17\n\x0f\x61uth_server_url\x18\x14 \x01(\t\x12\x1e\n\x16\x61uto_delete_data_files\x18\x15 \x01(\x08\x12\x1f\n\x17storage_space_allowance\x18\x16 \x01(\x02\x12$\n\x1cuse_sd_card_for_data_storage\x18\x17 \x01(\x08\x12\x1d\n\x15use_location_services\x18\x18 \x01(\x08\x12\x14\n\x0cuse_latitude\x18\x19 \x01(\x01\x12\x15\n\ruse_longitude\x18\x1a \x01(\x01\x12\x14\n\x0cuse_altitude\x18\x1b \x01(\x02\x12P\n\x0cmetrics_rate\x18\x1c \x01(\x0e\x32:.redvox_api_m.RedvoxPacketM.StationInformation.MetricsRate\x12Z\n\x08metadata\x18\x1d \x03(\x0b\x32H.redvox_api_m.RedvoxPacketM.StationInformation.AppSettings.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"I\n\nFftOverlap\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0e\n\nPERCENT_25\x10\x01\x12\x0e\n\nPERCENT_50\x10\x02\x12\x0e\n\nPERCENT_75\x10\x03\"n\n\x11\x41udioSamplingRate\x12\x19\n\x15UNKNOWN_SAMPLING_RATE\x10\x00\x12\t\n\x05HZ_80\x10\x01\x12\n\n\x06HZ_800\x10\x02\x12\x0b\n\x07HZ_8000\x10\x03\x12\x0c\n\x08HZ_16000\x10\x04\x12\x0c\n\x08HZ_48000\x10\x05\"f\n\x11\x41udioSourceTuning\x12\x12\n\x0eUNKNOWN_TUNING\x10\x00\x12\x15\n\x11INFRASOUND_TUNING\x10\x01\x12\x14\n\x10LOW_AUDIO_TUNING\x10\x02\x12\x10\n\x0c\x41UDIO_TUNING\x10\x03\"\xa5\x03\n\x0bInputSensor\x12\x12\n\x0eUNKNOWN_SENSOR\x10\x00\x12\x11\n\rACCELEROMETER\x10\x01\x12\x16\n\x12\x41\x43\x43\x45LEROMETER_FAST\x10\x02\x12\x17\n\x13\x41MBIENT_TEMPERATURE\x10\x03\x12\t\n\x05\x41UDIO\x10\x04\x12\x14\n\x10\x43OMPRESSED_AUDIO\x10\x05\x12\x0b\n\x07GRAVITY\x10\x06\x12\r\n\tGYROSCOPE\x10\x07\x12\x12\n\x0eGYROSCOPE_FAST\x10\x08\x12\x14\n\x10IMAGE_PER_SECOND\x10\t\x12\x14\n\x10IMAGE_PER_PACKET\x10\n\x12\t\n\x05LIGHT\x10\x0b\x12\x17\n\x13LINEAR_ACCELERATION\x10\x0c\x12\x0c\n\x08LOCATION\x10\r\x12\x10\n\x0cMAGNETOMETER\x10\x0e\x12\x15\n\x11MAGNETOMETER_FAST\x10\x0f\x12\x0f\n\x0bORIENTATION\x10\x10\x12\x0c\n\x08PRESSURE\x10\x11\x12\r\n\tPROXIMITY\x10\x12\x12\x15\n\x11RELATIVE_HUMIDITY\x10\x13\x12\x13\n\x0fROTATION_VECTOR\x10\x14\x12\x0c\n\x08VELOCITY\x10\x15\"O\n\x06OsType\x12\x0e\n\nUNKNOWN_OS\x10\x00\x12\x0b\n\x07\x41NDROID\x10\x01\x12\x07\n\x03IOS\x10\x02\x12\x07\n\x03OSX\x10\x03\x12\t\n\x05LINUX\x10\x04\x12\x0b\n\x07WINDOWS\x10\x05\"D\n\x0bMetricsRate\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x13\n\x0fONCE_PER_SECOND\x10\x01\x12\x13\n\x0fONCE_PER_PACKET\x10\x02\x1a\xc0\x07\n\x11TimingInformation\x12!\n\x19packet_start_os_timestamp\x18\x01 \x01(\x01\x12#\n\x1bpacket_start_mach_timestamp\x18\x02 \x01(\x01\x12\x1f\n\x17packet_end_os_timestamp\x18\x03 \x01(\x01\x12!\n\x19packet_end_mach_timestamp\x18\x04 \x01(\x01\x12,\n$server_acquisition_arrival_timestamp\x18\x05 \x01(\x01\x12 \n\x18\x61pp_start_mach_timestamp\x18\x06 \x01(\x01\x12T\n\x0fsynch_exchanges\x18\x07 \x03(\x0b\x32;.redvox_api_m.RedvoxPacketM.TimingInformation.SynchExchange\x12\x14\n\x0c\x62\x65st_latency\x18\x08 \x01(\x02\x12\x13\n\x0b\x62\x65st_offset\x18\t \x01(\x02\x12\r\n\x05score\x18\n \x01(\x02\x12U\n\x0cscore_method\x18\x0b \x01(\x0e\x32?.redvox_api_m.RedvoxPacketM.TimingInformation.TimingScoreMethod\x12.\n\x04unit\x18\x0c \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12M\n\x08metadata\x18\r \x03(\x0b\x32;.redvox_api_m.RedvoxPacketM.TimingInformation.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x95\x02\n\rSynchExchange\x12\n\n\x02\x61\x31\x18\x01 \x01(\x01\x12\n\n\x02\x61\x32\x18\x02 \x01(\x01\x12\n\n\x02\x61\x33\x18\x03 \x01(\x01\x12\n\n\x02\x62\x31\x18\x04 \x01(\x01\x12\n\n\x02\x62\x32\x18\x05 \x01(\x01\x12\n\n\x02\x62\x33\x18\x06 \x01(\x01\x12.\n\x04unit\x18\x07 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12[\n\x08metadata\x18\x08 \x03(\x0b\x32I.redvox_api_m.RedvoxPacketM.TimingInformation.SynchExchange.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\" \n\x11TimingScoreMethod\x12\x0b\n\x07UNKNOWN\x10\x00\x1a\xa8\x30\n\x07Sensors\x12>\n\raccelerometer\x18\x01 \x01(\x0b\x32\'.redvox_api_m.RedvoxPacketM.Sensors.Xyz\x12G\n\x13\x61mbient_temperature\x18\x02 \x01(\x0b\x32*.redvox_api_m.RedvoxPacketM.Sensors.Single\x12\x38\n\x05\x61udio\x18\x03 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.Sensors.Audio\x12M\n\x10\x63ompressed_audio\x18\x04 \x01(\x0b\x32\x33.redvox_api_m.RedvoxPacketM.Sensors.CompressedAudio\x12\x38\n\x07gravity\x18\x05 \x01(\x0b\x32\'.redvox_api_m.RedvoxPacketM.Sensors.Xyz\x12:\n\tgyroscope\x18\x06 \x01(\x0b\x32\'.redvox_api_m.RedvoxPacketM.Sensors.Xyz\x12\x38\n\x05image\x18\x07 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.Sensors.Image\x12\x39\n\x05light\x18\x08 \x01(\x0b\x32*.redvox_api_m.RedvoxPacketM.Sensors.Single\x12\x44\n\x13linear_acceleration\x18\t \x01(\x0b\x32\'.redvox_api_m.RedvoxPacketM.Sensors.Xyz\x12>\n\x08location\x18\n \x01(\x0b\x32,.redvox_api_m.RedvoxPacketM.Sensors.Location\x12=\n\x0cmagnetometer\x18\x0b \x01(\x0b\x32\'.redvox_api_m.RedvoxPacketM.Sensors.Xyz\x12<\n\x0borientation\x18\x0c \x01(\x0b\x32\'.redvox_api_m.RedvoxPacketM.Sensors.Xyz\x12<\n\x08pressure\x18\r \x01(\x0b\x32*.redvox_api_m.RedvoxPacketM.Sensors.Single\x12=\n\tproximity\x18\x0e \x01(\x0b\x32*.redvox_api_m.RedvoxPacketM.Sensors.Single\x12\x45\n\x11relative_humidity\x18\x0f \x01(\x0b\x32*.redvox_api_m.RedvoxPacketM.Sensors.Single\x12@\n\x0frotation_vector\x18\x10 \x01(\x0b\x32\'.redvox_api_m.RedvoxPacketM.Sensors.Xyz\x12\x39\n\x08velocity\x18\x11 \x01(\x0b\x32\'.redvox_api_m.RedvoxPacketM.Sensors.Xyz\x12\x43\n\x08metadata\x18\x12 \x03(\x0b\x32\x31.redvox_api_m.RedvoxPacketM.Sensors.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xd3\x02\n\x05\x41udio\x12\x1a\n\x12sensor_description\x18\x01 \x01(\t\x12\x1e\n\x16\x66irst_sample_timestamp\x18\x02 \x01(\x01\x12\x13\n\x0bsample_rate\x18\x03 \x01(\x02\x12\x19\n\x11\x62its_of_precision\x18\x04 \x01(\x02\x12\x14\n\x0cis_scrambled\x18\x05 \x01(\x08\x12\x10\n\x08\x65ncoding\x18\x06 \x01(\t\x12:\n\x07samples\x18\x07 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12I\n\x08metadata\x18\x08 \x03(\x0b\x32\x37.redvox_api_m.RedvoxPacketM.Sensors.Audio.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x8d\x03\n\x0f\x43ompressedAudio\x12\x1a\n\x12sensor_description\x18\x01 \x01(\t\x12\x1e\n\x16\x66irst_sample_timestamp\x18\x02 \x01(\x01\x12\x13\n\x0bsample_rate\x18\x03 \x01(\x02\x12\x14\n\x0cis_scrambled\x18\x04 \x01(\x08\x12\x13\n\x0b\x61udio_bytes\x18\x05 \x01(\x0c\x12S\n\x0b\x61udio_codec\x18\x06 \x01(\x0e\x32>.redvox_api_m.RedvoxPacketM.Sensors.CompressedAudio.AudioCodec\x12S\n\x08metadata\x18\x07 \x03(\x0b\x32\x41.redvox_api_m.RedvoxPacketM.Sensors.CompressedAudio.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"#\n\nAudioCodec\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04\x46LAC\x10\x01\x1a\x9c\x02\n\x06Single\x12\x1a\n\x12sensor_description\x18\x01 \x01(\t\x12=\n\ntimestamps\x18\x02 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.TimingPayload\x12:\n\x07samples\x18\x03 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12J\n\x08metadata\x18\x04 \x03(\x0b\x32\x38.redvox_api_m.RedvoxPacketM.Sensors.Single.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xd6\x18\n\x08Location\x12\x1a\n\x12sensor_description\x18\x01 \x01(\t\x12=\n\ntimestamps\x18\x02 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.TimingPayload\x12\x41\n\x0etimestamps_gps\x18\x03 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.TimingPayload\x12I\n\x10latitude_samples\x18\x04 \x01(\x0b\x32/.redvox_api_m.RedvoxPacketM.DoubleSamplePayload\x12J\n\x11longitude_samples\x18\x05 \x01(\x0b\x32/.redvox_api_m.RedvoxPacketM.DoubleSamplePayload\x12\x43\n\x10\x61ltitude_samples\x18\x06 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12@\n\rspeed_samples\x18\x07 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12\x42\n\x0f\x62\x65\x61ring_samples\x18\x08 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12N\n\x1bhorizontal_accuracy_samples\x18\t \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12L\n\x19vertical_accuracy_samples\x18\n \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12I\n\x16speed_accuracy_samples\x18\x0b \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12K\n\x18\x62\x65\x61ring_accuracy_samples\x18\x0c \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12U\n\x12last_best_location\x18\r \x01(\x0b\x32\x39.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation\x12X\n\x15overall_best_location\x18\x0e \x01(\x0b\x32\x39.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation\x12$\n\x1clocation_permissions_granted\x18\x0f \x01(\x08\x12#\n\x1blocation_services_requested\x18\x10 \x01(\x08\x12!\n\x19location_services_enabled\x18\x11 \x01(\x08\x12Y\n\x12location_providers\x18\x12 \x03(\x0e\x32=.redvox_api_m.RedvoxPacketM.Sensors.Location.LocationProvider\x12L\n\x08metadata\x18\x13 \x03(\x0b\x32:.redvox_api_m.RedvoxPacketM.Sensors.Location.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xcf\r\n\x0c\x42\x65stLocation\x12m\n\x1clatitude_longitude_timestamp\x18\x01 \x01(\x0b\x32G.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation.BestTimestamp\x12\x63\n\x12\x61ltitude_timestamp\x18\x02 \x01(\x0b\x32G.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation.BestTimestamp\x12`\n\x0fspeed_timestamp\x18\x03 \x01(\x0b\x32G.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation.BestTimestamp\x12\x62\n\x11\x62\x65\x61ring_timestamp\x18\x04 \x01(\x0b\x32G.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation.BestTimestamp\x12\x41\n\x17latitude_longitude_unit\x18\x05 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x37\n\raltitude_unit\x18\x06 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x34\n\nspeed_unit\x18\x07 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x36\n\x0c\x62\x65\x61ring_unit\x18\x08 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12@\n\x16vertical_accuracy_unit\x18\t \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x42\n\x18horizontal_accuracy_unit\x18\n \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12=\n\x13speed_accuracy_unit\x18\x0b \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12?\n\x15\x62\x65\x61ring_accuracy_unit\x18\x0c \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x10\n\x08latitude\x18\r \x01(\x01\x12\x11\n\tlongitude\x18\x0e \x01(\x01\x12\x10\n\x08\x61ltitude\x18\x0f \x01(\x02\x12\r\n\x05speed\x18\x10 \x01(\x02\x12\x0f\n\x07\x62\x65\x61ring\x18\x11 \x01(\x02\x12\x19\n\x11vertical_accuracy\x18\x12 \x01(\x02\x12\x1b\n\x13horizontal_accuracy\x18\x13 \x01(\x02\x12\x16\n\x0espeed_accuracy\x18\x14 \x01(\x02\x12\x18\n\x10\x62\x65\x61ring_accuracy\x18\x15 \x01(\x02\x12\r\n\x05score\x18\x16 \x01(\x02\x12]\n\x06method\x18\x17 \x01(\x0e\x32M.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation.LocationScoreMethod\x12X\n\x11location_provider\x18\x18 \x01(\x0e\x32=.redvox_api_m.RedvoxPacketM.Sensors.Location.LocationProvider\x12Y\n\x08metadata\x18\x19 \x03(\x0b\x32G.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xf4\x01\n\rBestTimestamp\x12.\n\x04unit\x18\x01 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x0c\n\x04mach\x18\x02 \x01(\x01\x12\x0b\n\x03gps\x18\x03 \x01(\x01\x12g\n\x08metadata\x18\x04 \x03(\x0b\x32U.redvox_api_m.RedvoxPacketM.Sensors.Location.BestLocation.BestTimestamp.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\")\n\x13LocationScoreMethod\x12\x12\n\x0eUNKNOWN_METHOD\x10\x00\"I\n\x10LocationProvider\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04NONE\x10\x01\x12\x08\n\x04USER\x10\x02\x12\x07\n\x03GPS\x10\x03\x12\x0b\n\x07NETWORK\x10\x04\x1a\x94\x03\n\x03Xyz\x12\x1a\n\x12sensor_description\x18\x01 \x01(\t\x12=\n\ntimestamps\x18\x02 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.TimingPayload\x12<\n\tx_samples\x18\x03 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12<\n\ty_samples\x18\x04 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12<\n\tz_samples\x18\x05 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.SamplePayload\x12G\n\x08metadata\x18\x06 \x03(\x0b\x32\x35.redvox_api_m.RedvoxPacketM.Sensors.Xyz.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xf0\x02\n\x05Image\x12\x1a\n\x12sensor_description\x18\x01 \x01(\t\x12=\n\ntimestamps\x18\x02 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.TimingPayload\x12\x0f\n\x07samples\x18\x03 \x03(\x0c\x12I\n\x0bimage_codec\x18\x04 \x01(\x0e\x32\x34.redvox_api_m.RedvoxPacketM.Sensors.Image.ImageCodec\x12I\n\x08metadata\x18\x05 \x03(\x0b\x32\x37.redvox_api_m.RedvoxPacketM.Sensors.Image.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"4\n\nImageCodec\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03PNG\x10\x01\x12\x07\n\x03JPG\x10\x02\x12\x07\n\x03\x42MP\x10\x03\x1a\xf2\x07\n\x0b\x45ventStream\x12\x0c\n\x04name\x18\x01 \x01(\t\x12=\n\ntimestamps\x18\x02 \x01(\x0b\x32).redvox_api_m.RedvoxPacketM.TimingPayload\x12=\n\x06\x65vents\x18\x03 \x03(\x0b\x32-.redvox_api_m.RedvoxPacketM.EventStream.Event\x12G\n\x08metadata\x18\x04 \x03(\x0b\x32\x35.redvox_api_m.RedvoxPacketM.EventStream.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xdc\x05\n\x05\x45vent\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12X\n\x0estring_payload\x18\x02 \x03(\x0b\x32@.redvox_api_m.RedvoxPacketM.EventStream.Event.StringPayloadEntry\x12Z\n\x0fnumeric_payload\x18\x03 \x03(\x0b\x32\x41.redvox_api_m.RedvoxPacketM.EventStream.Event.NumericPayloadEntry\x12Z\n\x0f\x62oolean_payload\x18\x04 \x03(\x0b\x32\x41.redvox_api_m.RedvoxPacketM.EventStream.Event.BooleanPayloadEntry\x12T\n\x0c\x62yte_payload\x18\x05 \x03(\x0b\x32>.redvox_api_m.RedvoxPacketM.EventStream.Event.BytePayloadEntry\x12M\n\x08metadata\x18\x06 \x03(\x0b\x32;.redvox_api_m.RedvoxPacketM.EventStream.Event.MetadataEntry\x1a\x34\n\x12StringPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x35\n\x13NumericPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01:\x02\x38\x01\x1a\x35\n\x13\x42ooleanPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x08:\x02\x38\x01\x1a\x32\n\x10\x42ytePayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x94\x02\n\rSamplePayload\x12.\n\x04unit\x18\x01 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x0e\n\x06values\x18\x02 \x03(\x02\x12G\n\x10value_statistics\x18\x03 \x01(\x0b\x32-.redvox_api_m.RedvoxPacketM.SummaryStatistics\x12I\n\x08metadata\x18\x04 \x03(\x0b\x32\x37.redvox_api_m.RedvoxPacketM.SamplePayload.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xa0\x02\n\x13\x44oubleSamplePayload\x12.\n\x04unit\x18\x01 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x0e\n\x06values\x18\x02 \x03(\x01\x12G\n\x10value_statistics\x18\x03 \x01(\x0b\x32-.redvox_api_m.RedvoxPacketM.SummaryStatistics\x12O\n\x08metadata\x18\x04 \x03(\x0b\x32=.redvox_api_m.RedvoxPacketM.DoubleSamplePayload.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xd1\x02\n\rTimingPayload\x12.\n\x04unit\x18\x01 \x01(\x0e\x32 .redvox_api_m.RedvoxPacketM.Unit\x12\x12\n\ntimestamps\x18\x02 \x03(\x01\x12K\n\x14timestamp_statistics\x18\x03 \x01(\x0b\x32-.redvox_api_m.RedvoxPacketM.SummaryStatistics\x12\x18\n\x10mean_sample_rate\x18\x04 \x01(\x02\x12\x19\n\x11stdev_sample_rate\x18\x05 \x01(\x02\x12I\n\x08metadata\x18\x06 \x03(\x0b\x32\x37.redvox_api_m.RedvoxPacketM.TimingPayload.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xf5\x01\n\x11SummaryStatistics\x12\r\n\x05\x63ount\x18\x01 \x01(\x01\x12\x0c\n\x04mean\x18\x02 \x01(\x01\x12\x1a\n\x12standard_deviation\x18\x03 \x01(\x01\x12\x0b\n\x03min\x18\x04 \x01(\x01\x12\x0b\n\x03max\x18\x05 \x01(\x01\x12\r\n\x05range\x18\x06 \x01(\x01\x12M\n\x08metadata\x18\x07 \x03(\x0b\x32;.redvox_api_m.RedvoxPacketM.SummaryStatistics.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x83\x03\n\x04Unit\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x1d\n\x19METERS_PER_SECOND_SQUARED\x10\x01\x12\x0e\n\nKILOPASCAL\x10\x02\x12\x16\n\x12RADIANS_PER_SECOND\x10\x03\x12\x13\n\x0f\x44\x45\x43IMAL_DEGREES\x10\x04\x12\n\n\x06METERS\x10\x05\x12\x15\n\x11METERS_PER_SECOND\x10\x06\x12\x0e\n\nMICROTESLA\x10\x07\x12\x19\n\x15LSB_PLUS_MINUS_COUNTS\x10\x08\x12!\n\x1dMICROSECONDS_SINCE_UNIX_EPOCH\x10\t\x12\x0b\n\x07\x44\x45\x43IBEL\x10\n\x12\x13\n\x0f\x44\x45GREES_CELSIUS\x10\x0b\x12\x08\n\x04\x42YTE\x10\x0c\x12\x0e\n\nPERCENTAGE\x10\r\x12\x0b\n\x07RADIANS\x10\x0e\x12\x10\n\x0cMICROAMPERES\x10\x0f\x12\x0f\n\x0b\x43\x45NTIMETERS\x10\x10\x12\x15\n\x11NORMALIZED_COUNTS\x10\x11\x12\x07\n\x03LUX\x10\x12\x12\x0c\n\x08UNITLESS\x10\x13\x12\x07\n\x03PCM\x10\x14\"\xac\x01\n\x16\x45ncryptedRedvoxPacketM\x12\x0e\n\x06header\x18\x01 \x01(\x0c\x12\x0e\n\x06packet\x18\x02 \x01(\x0c\x1ar\n\x06Header\x12\x12\n\nstation_id\x18\x01 \x01(\t\x12\x14\n\x0cstation_uuid\x18\x02 \x01(\t\x12\x12\n\nauth_token\x18\x03 \x01(\t\x12\x16\n\x0e\x66irebase_token\x18\x04 \x01(\t\x12\x12\n\nauth_email\x18\x05 \x01(\t\"\x89\x01\n\x12\x41\x63quisitionRequest\x12\x12\n\nauth_token\x18\x01 \x01(\t\x12\x16\n\x0e\x66irebase_token\x18\x02 \x01(\t\x12\x10\n\x08\x63hecksum\x18\x03 \x01(\x03\x12\x14\n\x0cis_encrypted\x18\x04 \x01(\x08\x12\x0f\n\x07payload\x18\x05 \x01(\x0c\x12\x0e\n\x06seq_id\x18\x06 \x01(\x03\"\xf5\x01\n\x13\x41\x63quisitionResponse\x12\x45\n\rresponse_type\x18\x01 \x01(\x0e\x32..redvox_api_m.AcquisitionResponse.ResponseType\x12\x10\n\x08\x63hecksum\x18\x02 \x01(\x03\x12\x0f\n\x07\x64\x65tails\x18\x03 \x01(\t\x12\x0e\n\x06resend\x18\x04 \x01(\x08\x12\x0e\n\x06seq_id\x18\x05 \x01(\x03\"T\n\x0cResponseType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x06\n\x02OK\x10\x01\x12\x0e\n\nAUTH_ERROR\x10\x02\x12\x0e\n\nDATA_ERROR\x10\x03\x12\x0f\n\x0bOTHER_ERROR\x10\x04\"\\\n\x0cSynchRequest\x12\x12\n\nstation_id\x18\x01 \x01(\t\x12\x14\n\x0cstation_uuid\x18\x02 \x01(\t\x12\x0e\n\x06seq_id\x18\x03 \x01(\r\x12\x12\n\nsub_seq_id\x18\x04 \x01(\r\"\x85\x01\n\rSynchResponse\x12\x12\n\nstation_id\x18\x01 \x01(\t\x12\x14\n\x0cstation_uuid\x18\x02 \x01(\t\x12\x0e\n\x06seq_id\x18\x03 \x01(\r\x12\x12\n\nsub_seq_id\x18\x04 \x01(\r\x12\x12\n\nrecv_ts_us\x18\x05 \x01(\x04\x12\x12\n\nsend_ts_us\x18\x06 \x01(\x04\x42\x10\n\x0eio.redvox.apisb\x06proto3')
 
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'redvox_api_m_pb2', _globals)
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'src.redvox_api_m.redvox_api_m_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\016io.redvox.apis'
   _REDVOXPACKETM_METADATAENTRY._options = None
   _REDVOXPACKETM_METADATAENTRY._serialized_options = b'8\001'
   _REDVOXPACKETM_STATIONINFORMATION_METADATAENTRY._options = None
@@ -72,152 +71,152 @@
   _REDVOXPACKETM_SAMPLEPAYLOAD_METADATAENTRY._serialized_options = b'8\001'
   _REDVOXPACKETM_DOUBLESAMPLEPAYLOAD_METADATAENTRY._options = None
   _REDVOXPACKETM_DOUBLESAMPLEPAYLOAD_METADATAENTRY._serialized_options = b'8\001'
   _REDVOXPACKETM_TIMINGPAYLOAD_METADATAENTRY._options = None
   _REDVOXPACKETM_TIMINGPAYLOAD_METADATAENTRY._serialized_options = b'8\001'
   _REDVOXPACKETM_SUMMARYSTATISTICS_METADATAENTRY._options = None
   _REDVOXPACKETM_SUMMARYSTATISTICS_METADATAENTRY._serialized_options = b'8\001'
-  _globals['_REDVOXPACKETM']._serialized_start=37
-  _globals['_REDVOXPACKETM']._serialized_end=14865
-  _globals['_REDVOXPACKETM_METADATAENTRY']._serialized_start=415
-  _globals['_REDVOXPACKETM_METADATAENTRY']._serialized_end=462
-  _globals['_REDVOXPACKETM_STATIONINFORMATION']._serialized_start=465
-  _globals['_REDVOXPACKETM_STATIONINFORMATION']._serialized_end=5154
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_METADATAENTRY']._serialized_start=415
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_METADATAENTRY']._serialized_end=462
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_SERVICEURLS']._serialized_start=1090
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_SERVICEURLS']._serialized_end=1315
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_SERVICEURLS_METADATAENTRY']._serialized_start=415
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_SERVICEURLS_METADATAENTRY']._serialized_end=462
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS']._serialized_start=1318
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS']._serialized_end=2975
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_METADATAENTRY']._serialized_start=415
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_METADATAENTRY']._serialized_end=462
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_NETWORKTYPE']._serialized_start=2572
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_NETWORKTYPE']._serialized_end=2657
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_WIFIWAKELOCK']._serialized_start=2659
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_WIFIWAKELOCK']._serialized_end=2726
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_CELLSERVICESTATE']._serialized_start=2728
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_CELLSERVICESTATE']._serialized_end=2822
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_POWERSTATE']._serialized_start=2824
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_POWERSTATE']._serialized_end=2903
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_SCREENSTATE']._serialized_start=2905
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_SCREENSTATE']._serialized_end=2975
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS']._serialized_start=2978
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS']._serialized_end=5003
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_METADATAENTRY']._serialized_start=415
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_METADATAENTRY']._serialized_end=462
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_FFTOVERLAP']._serialized_start=4290
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_FFTOVERLAP']._serialized_end=4363
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_AUDIOSAMPLINGRATE']._serialized_start=4365
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_AUDIOSAMPLINGRATE']._serialized_end=4475
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_AUDIOSOURCETUNING']._serialized_start=4477
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_AUDIOSOURCETUNING']._serialized_end=4579
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_INPUTSENSOR']._serialized_start=4582
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_INPUTSENSOR']._serialized_end=5003
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_OSTYPE']._serialized_start=5005
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_OSTYPE']._serialized_end=5084
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_METRICSRATE']._serialized_start=5086
-  _globals['_REDVOXPACKETM_STATIONINFORMATION_METRICSRATE']._serialized_end=5154
-  _globals['_REDVOXPACKETM_TIMINGINFORMATION']._serialized_start=5157
-  _globals['_REDVOXPACKETM_TIMINGINFORMATION']._serialized_end=6117
-  _globals['_REDVOXPACKETM_TIMINGINFORMATION_METADATAENTRY']._serialized_start=415
-  _globals['_REDVOXPACKETM_TIMINGINFORMATION_METADATAENTRY']._serialized_end=462
-  _globals['_REDVOXPACKETM_TIMINGINFORMATION_SYNCHEXCHANGE']._serialized_start=5806
-  _globals['_REDVOXPACKETM_TIMINGINFORMATION_SYNCHEXCHANGE']._serialized_end=6083
-  _globals['_REDVOXPACKETM_TIMINGINFORMATION_SYNCHEXCHANGE_METADATAENTRY']._serialized_start=415
-  _globals['_REDVOXPACKETM_TIMINGINFORMATION_SYNCHEXCHANGE_METADATAENTRY']._serialized_end=462
-  _globals['_REDVOXPACKETM_TIMINGINFORMATION_TIMINGSCOREMETHOD']._serialized_start=6085
-  _globals['_REDVOXPACKETM_TIMINGINFORMATION_TIMINGSCOREMETHOD']._serialized_end=6117
-  _globals['_REDVOXPACKETM_SENSORS']._serialized_start=6120
-  _globals['_REDVOXPACKETM_SENSORS']._serialized_end=12304
-  _globals['_REDVOXPACKETM_SENSORS_METADATAENTRY']._serialized_start=415
-  _globals['_REDVOXPACKETM_SENSORS_METADATAENTRY']._serialized_end=462
-  _globals['_REDVOXPACKETM_SENSORS_AUDIO']._serialized_start=7339
-  _globals['_REDVOXPACKETM_SENSORS_AUDIO']._serialized_end=7678
-  _globals['_REDVOXPACKETM_SENSORS_AUDIO_METADATAENTRY']._serialized_start=415
-  _globals['_REDVOXPACKETM_SENSORS_AUDIO_METADATAENTRY']._serialized_end=462
-  _globals['_REDVOXPACKETM_SENSORS_COMPRESSEDAUDIO']._serialized_start=7681
-  _globals['_REDVOXPACKETM_SENSORS_COMPRESSEDAUDIO']._serialized_end=8078
-  _globals['_REDVOXPACKETM_SENSORS_COMPRESSEDAUDIO_METADATAENTRY']._serialized_start=415
-  _globals['_REDVOXPACKETM_SENSORS_COMPRESSEDAUDIO_METADATAENTRY']._serialized_end=462
-  _globals['_REDVOXPACKETM_SENSORS_COMPRESSEDAUDIO_AUDIOCODEC']._serialized_start=8043
-  _globals['_REDVOXPACKETM_SENSORS_COMPRESSEDAUDIO_AUDIOCODEC']._serialized_end=8078
-  _globals['_REDVOXPACKETM_SENSORS_SINGLE']._serialized_start=8081
-  _globals['_REDVOXPACKETM_SENSORS_SINGLE']._serialized_end=8365
-  _globals['_REDVOXPACKETM_SENSORS_SINGLE_METADATAENTRY']._serialized_start=415
-  _globals['_REDVOXPACKETM_SENSORS_SINGLE_METADATAENTRY']._serialized_end=462
-  _globals['_REDVOXPACKETM_SENSORS_LOCATION']._serialized_start=8368
-  _globals['_REDVOXPACKETM_SENSORS_LOCATION']._serialized_end=11526
-  _globals['_REDVOXPACKETM_SENSORS_LOCATION_METADATAENTRY']._serialized_start=415
-  _globals['_REDVOXPACKETM_SENSORS_LOCATION_METADATAENTRY']._serialized_end=462
-  _globals['_REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION']._serialized_start=9708
-  _globals['_REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION']._serialized_end=11451
-  _globals['_REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION_METADATAENTRY']._serialized_start=415
-  _globals['_REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION_METADATAENTRY']._serialized_end=462
-  _globals['_REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION_BESTTIMESTAMP']._serialized_start=11164
-  _globals['_REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION_BESTTIMESTAMP']._serialized_end=11408
-  _globals['_REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION_BESTTIMESTAMP_METADATAENTRY']._serialized_start=415
-  _globals['_REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION_BESTTIMESTAMP_METADATAENTRY']._serialized_end=462
-  _globals['_REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION_LOCATIONSCOREMETHOD']._serialized_start=11410
-  _globals['_REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION_LOCATIONSCOREMETHOD']._serialized_end=11451
-  _globals['_REDVOXPACKETM_SENSORS_LOCATION_LOCATIONPROVIDER']._serialized_start=11453
-  _globals['_REDVOXPACKETM_SENSORS_LOCATION_LOCATIONPROVIDER']._serialized_end=11526
-  _globals['_REDVOXPACKETM_SENSORS_XYZ']._serialized_start=11529
-  _globals['_REDVOXPACKETM_SENSORS_XYZ']._serialized_end=11933
-  _globals['_REDVOXPACKETM_SENSORS_XYZ_METADATAENTRY']._serialized_start=415
-  _globals['_REDVOXPACKETM_SENSORS_XYZ_METADATAENTRY']._serialized_end=462
-  _globals['_REDVOXPACKETM_SENSORS_IMAGE']._serialized_start=11936
-  _globals['_REDVOXPACKETM_SENSORS_IMAGE']._serialized_end=12304
-  _globals['_REDVOXPACKETM_SENSORS_IMAGE_METADATAENTRY']._serialized_start=415
-  _globals['_REDVOXPACKETM_SENSORS_IMAGE_METADATAENTRY']._serialized_end=462
-  _globals['_REDVOXPACKETM_SENSORS_IMAGE_IMAGECODEC']._serialized_start=12252
-  _globals['_REDVOXPACKETM_SENSORS_IMAGE_IMAGECODEC']._serialized_end=12304
-  _globals['_REDVOXPACKETM_EVENTSTREAM']._serialized_start=12307
-  _globals['_REDVOXPACKETM_EVENTSTREAM']._serialized_end=13317
-  _globals['_REDVOXPACKETM_EVENTSTREAM_METADATAENTRY']._serialized_start=415
-  _globals['_REDVOXPACKETM_EVENTSTREAM_METADATAENTRY']._serialized_end=462
-  _globals['_REDVOXPACKETM_EVENTSTREAM_EVENT']._serialized_start=12585
-  _globals['_REDVOXPACKETM_EVENTSTREAM_EVENT']._serialized_end=13317
-  _globals['_REDVOXPACKETM_EVENTSTREAM_EVENT_STRINGPAYLOADENTRY']._serialized_start=13054
-  _globals['_REDVOXPACKETM_EVENTSTREAM_EVENT_STRINGPAYLOADENTRY']._serialized_end=13106
-  _globals['_REDVOXPACKETM_EVENTSTREAM_EVENT_NUMERICPAYLOADENTRY']._serialized_start=13108
-  _globals['_REDVOXPACKETM_EVENTSTREAM_EVENT_NUMERICPAYLOADENTRY']._serialized_end=13161
-  _globals['_REDVOXPACKETM_EVENTSTREAM_EVENT_BOOLEANPAYLOADENTRY']._serialized_start=13163
-  _globals['_REDVOXPACKETM_EVENTSTREAM_EVENT_BOOLEANPAYLOADENTRY']._serialized_end=13216
-  _globals['_REDVOXPACKETM_EVENTSTREAM_EVENT_BYTEPAYLOADENTRY']._serialized_start=13218
-  _globals['_REDVOXPACKETM_EVENTSTREAM_EVENT_BYTEPAYLOADENTRY']._serialized_end=13268
-  _globals['_REDVOXPACKETM_EVENTSTREAM_EVENT_METADATAENTRY']._serialized_start=415
-  _globals['_REDVOXPACKETM_EVENTSTREAM_EVENT_METADATAENTRY']._serialized_end=462
-  _globals['_REDVOXPACKETM_SAMPLEPAYLOAD']._serialized_start=13320
-  _globals['_REDVOXPACKETM_SAMPLEPAYLOAD']._serialized_end=13596
-  _globals['_REDVOXPACKETM_SAMPLEPAYLOAD_METADATAENTRY']._serialized_start=415
-  _globals['_REDVOXPACKETM_SAMPLEPAYLOAD_METADATAENTRY']._serialized_end=462
-  _globals['_REDVOXPACKETM_DOUBLESAMPLEPAYLOAD']._serialized_start=13599
-  _globals['_REDVOXPACKETM_DOUBLESAMPLEPAYLOAD']._serialized_end=13887
-  _globals['_REDVOXPACKETM_DOUBLESAMPLEPAYLOAD_METADATAENTRY']._serialized_start=415
-  _globals['_REDVOXPACKETM_DOUBLESAMPLEPAYLOAD_METADATAENTRY']._serialized_end=462
-  _globals['_REDVOXPACKETM_TIMINGPAYLOAD']._serialized_start=13890
-  _globals['_REDVOXPACKETM_TIMINGPAYLOAD']._serialized_end=14227
-  _globals['_REDVOXPACKETM_TIMINGPAYLOAD_METADATAENTRY']._serialized_start=415
-  _globals['_REDVOXPACKETM_TIMINGPAYLOAD_METADATAENTRY']._serialized_end=462
-  _globals['_REDVOXPACKETM_SUMMARYSTATISTICS']._serialized_start=14230
-  _globals['_REDVOXPACKETM_SUMMARYSTATISTICS']._serialized_end=14475
-  _globals['_REDVOXPACKETM_SUMMARYSTATISTICS_METADATAENTRY']._serialized_start=415
-  _globals['_REDVOXPACKETM_SUMMARYSTATISTICS_METADATAENTRY']._serialized_end=462
-  _globals['_REDVOXPACKETM_UNIT']._serialized_start=14478
-  _globals['_REDVOXPACKETM_UNIT']._serialized_end=14865
-  _globals['_ENCRYPTEDREDVOXPACKETM']._serialized_start=14868
-  _globals['_ENCRYPTEDREDVOXPACKETM']._serialized_end=15040
-  _globals['_ENCRYPTEDREDVOXPACKETM_HEADER']._serialized_start=14926
-  _globals['_ENCRYPTEDREDVOXPACKETM_HEADER']._serialized_end=15040
-  _globals['_ACQUISITIONREQUEST']._serialized_start=15043
-  _globals['_ACQUISITIONREQUEST']._serialized_end=15180
-  _globals['_ACQUISITIONRESPONSE']._serialized_start=15183
-  _globals['_ACQUISITIONRESPONSE']._serialized_end=15428
-  _globals['_ACQUISITIONRESPONSE_RESPONSETYPE']._serialized_start=15344
-  _globals['_ACQUISITIONRESPONSE_RESPONSETYPE']._serialized_end=15428
-  _globals['_SYNCHREQUEST']._serialized_start=15430
-  _globals['_SYNCHREQUEST']._serialized_end=15522
-  _globals['_SYNCHRESPONSE']._serialized_start=15525
-  _globals['_SYNCHRESPONSE']._serialized_end=15658
+  _REDVOXPACKETM._serialized_start=54
+  _REDVOXPACKETM._serialized_end=14882
+  _REDVOXPACKETM_METADATAENTRY._serialized_start=432
+  _REDVOXPACKETM_METADATAENTRY._serialized_end=479
+  _REDVOXPACKETM_STATIONINFORMATION._serialized_start=482
+  _REDVOXPACKETM_STATIONINFORMATION._serialized_end=5171
+  _REDVOXPACKETM_STATIONINFORMATION_METADATAENTRY._serialized_start=432
+  _REDVOXPACKETM_STATIONINFORMATION_METADATAENTRY._serialized_end=479
+  _REDVOXPACKETM_STATIONINFORMATION_SERVICEURLS._serialized_start=1107
+  _REDVOXPACKETM_STATIONINFORMATION_SERVICEURLS._serialized_end=1332
+  _REDVOXPACKETM_STATIONINFORMATION_SERVICEURLS_METADATAENTRY._serialized_start=432
+  _REDVOXPACKETM_STATIONINFORMATION_SERVICEURLS_METADATAENTRY._serialized_end=479
+  _REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS._serialized_start=1335
+  _REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS._serialized_end=2992
+  _REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_METADATAENTRY._serialized_start=432
+  _REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_METADATAENTRY._serialized_end=479
+  _REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_NETWORKTYPE._serialized_start=2589
+  _REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_NETWORKTYPE._serialized_end=2674
+  _REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_WIFIWAKELOCK._serialized_start=2676
+  _REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_WIFIWAKELOCK._serialized_end=2743
+  _REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_CELLSERVICESTATE._serialized_start=2745
+  _REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_CELLSERVICESTATE._serialized_end=2839
+  _REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_POWERSTATE._serialized_start=2841
+  _REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_POWERSTATE._serialized_end=2920
+  _REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_SCREENSTATE._serialized_start=2922
+  _REDVOXPACKETM_STATIONINFORMATION_STATIONMETRICS_SCREENSTATE._serialized_end=2992
+  _REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS._serialized_start=2995
+  _REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS._serialized_end=5020
+  _REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_METADATAENTRY._serialized_start=432
+  _REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_METADATAENTRY._serialized_end=479
+  _REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_FFTOVERLAP._serialized_start=4307
+  _REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_FFTOVERLAP._serialized_end=4380
+  _REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_AUDIOSAMPLINGRATE._serialized_start=4382
+  _REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_AUDIOSAMPLINGRATE._serialized_end=4492
+  _REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_AUDIOSOURCETUNING._serialized_start=4494
+  _REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_AUDIOSOURCETUNING._serialized_end=4596
+  _REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_INPUTSENSOR._serialized_start=4599
+  _REDVOXPACKETM_STATIONINFORMATION_APPSETTINGS_INPUTSENSOR._serialized_end=5020
+  _REDVOXPACKETM_STATIONINFORMATION_OSTYPE._serialized_start=5022
+  _REDVOXPACKETM_STATIONINFORMATION_OSTYPE._serialized_end=5101
+  _REDVOXPACKETM_STATIONINFORMATION_METRICSRATE._serialized_start=5103
+  _REDVOXPACKETM_STATIONINFORMATION_METRICSRATE._serialized_end=5171
+  _REDVOXPACKETM_TIMINGINFORMATION._serialized_start=5174
+  _REDVOXPACKETM_TIMINGINFORMATION._serialized_end=6134
+  _REDVOXPACKETM_TIMINGINFORMATION_METADATAENTRY._serialized_start=432
+  _REDVOXPACKETM_TIMINGINFORMATION_METADATAENTRY._serialized_end=479
+  _REDVOXPACKETM_TIMINGINFORMATION_SYNCHEXCHANGE._serialized_start=5823
+  _REDVOXPACKETM_TIMINGINFORMATION_SYNCHEXCHANGE._serialized_end=6100
+  _REDVOXPACKETM_TIMINGINFORMATION_SYNCHEXCHANGE_METADATAENTRY._serialized_start=432
+  _REDVOXPACKETM_TIMINGINFORMATION_SYNCHEXCHANGE_METADATAENTRY._serialized_end=479
+  _REDVOXPACKETM_TIMINGINFORMATION_TIMINGSCOREMETHOD._serialized_start=6102
+  _REDVOXPACKETM_TIMINGINFORMATION_TIMINGSCOREMETHOD._serialized_end=6134
+  _REDVOXPACKETM_SENSORS._serialized_start=6137
+  _REDVOXPACKETM_SENSORS._serialized_end=12321
+  _REDVOXPACKETM_SENSORS_METADATAENTRY._serialized_start=432
+  _REDVOXPACKETM_SENSORS_METADATAENTRY._serialized_end=479
+  _REDVOXPACKETM_SENSORS_AUDIO._serialized_start=7356
+  _REDVOXPACKETM_SENSORS_AUDIO._serialized_end=7695
+  _REDVOXPACKETM_SENSORS_AUDIO_METADATAENTRY._serialized_start=432
+  _REDVOXPACKETM_SENSORS_AUDIO_METADATAENTRY._serialized_end=479
+  _REDVOXPACKETM_SENSORS_COMPRESSEDAUDIO._serialized_start=7698
+  _REDVOXPACKETM_SENSORS_COMPRESSEDAUDIO._serialized_end=8095
+  _REDVOXPACKETM_SENSORS_COMPRESSEDAUDIO_METADATAENTRY._serialized_start=432
+  _REDVOXPACKETM_SENSORS_COMPRESSEDAUDIO_METADATAENTRY._serialized_end=479
+  _REDVOXPACKETM_SENSORS_COMPRESSEDAUDIO_AUDIOCODEC._serialized_start=8060
+  _REDVOXPACKETM_SENSORS_COMPRESSEDAUDIO_AUDIOCODEC._serialized_end=8095
+  _REDVOXPACKETM_SENSORS_SINGLE._serialized_start=8098
+  _REDVOXPACKETM_SENSORS_SINGLE._serialized_end=8382
+  _REDVOXPACKETM_SENSORS_SINGLE_METADATAENTRY._serialized_start=432
+  _REDVOXPACKETM_SENSORS_SINGLE_METADATAENTRY._serialized_end=479
+  _REDVOXPACKETM_SENSORS_LOCATION._serialized_start=8385
+  _REDVOXPACKETM_SENSORS_LOCATION._serialized_end=11543
+  _REDVOXPACKETM_SENSORS_LOCATION_METADATAENTRY._serialized_start=432
+  _REDVOXPACKETM_SENSORS_LOCATION_METADATAENTRY._serialized_end=479
+  _REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION._serialized_start=9725
+  _REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION._serialized_end=11468
+  _REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION_METADATAENTRY._serialized_start=432
+  _REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION_METADATAENTRY._serialized_end=479
+  _REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION_BESTTIMESTAMP._serialized_start=11181
+  _REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION_BESTTIMESTAMP._serialized_end=11425
+  _REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION_BESTTIMESTAMP_METADATAENTRY._serialized_start=432
+  _REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION_BESTTIMESTAMP_METADATAENTRY._serialized_end=479
+  _REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION_LOCATIONSCOREMETHOD._serialized_start=11427
+  _REDVOXPACKETM_SENSORS_LOCATION_BESTLOCATION_LOCATIONSCOREMETHOD._serialized_end=11468
+  _REDVOXPACKETM_SENSORS_LOCATION_LOCATIONPROVIDER._serialized_start=11470
+  _REDVOXPACKETM_SENSORS_LOCATION_LOCATIONPROVIDER._serialized_end=11543
+  _REDVOXPACKETM_SENSORS_XYZ._serialized_start=11546
+  _REDVOXPACKETM_SENSORS_XYZ._serialized_end=11950
+  _REDVOXPACKETM_SENSORS_XYZ_METADATAENTRY._serialized_start=432
+  _REDVOXPACKETM_SENSORS_XYZ_METADATAENTRY._serialized_end=479
+  _REDVOXPACKETM_SENSORS_IMAGE._serialized_start=11953
+  _REDVOXPACKETM_SENSORS_IMAGE._serialized_end=12321
+  _REDVOXPACKETM_SENSORS_IMAGE_METADATAENTRY._serialized_start=432
+  _REDVOXPACKETM_SENSORS_IMAGE_METADATAENTRY._serialized_end=479
+  _REDVOXPACKETM_SENSORS_IMAGE_IMAGECODEC._serialized_start=12269
+  _REDVOXPACKETM_SENSORS_IMAGE_IMAGECODEC._serialized_end=12321
+  _REDVOXPACKETM_EVENTSTREAM._serialized_start=12324
+  _REDVOXPACKETM_EVENTSTREAM._serialized_end=13334
+  _REDVOXPACKETM_EVENTSTREAM_METADATAENTRY._serialized_start=432
+  _REDVOXPACKETM_EVENTSTREAM_METADATAENTRY._serialized_end=479
+  _REDVOXPACKETM_EVENTSTREAM_EVENT._serialized_start=12602
+  _REDVOXPACKETM_EVENTSTREAM_EVENT._serialized_end=13334
+  _REDVOXPACKETM_EVENTSTREAM_EVENT_STRINGPAYLOADENTRY._serialized_start=13071
+  _REDVOXPACKETM_EVENTSTREAM_EVENT_STRINGPAYLOADENTRY._serialized_end=13123
+  _REDVOXPACKETM_EVENTSTREAM_EVENT_NUMERICPAYLOADENTRY._serialized_start=13125
+  _REDVOXPACKETM_EVENTSTREAM_EVENT_NUMERICPAYLOADENTRY._serialized_end=13178
+  _REDVOXPACKETM_EVENTSTREAM_EVENT_BOOLEANPAYLOADENTRY._serialized_start=13180
+  _REDVOXPACKETM_EVENTSTREAM_EVENT_BOOLEANPAYLOADENTRY._serialized_end=13233
+  _REDVOXPACKETM_EVENTSTREAM_EVENT_BYTEPAYLOADENTRY._serialized_start=13235
+  _REDVOXPACKETM_EVENTSTREAM_EVENT_BYTEPAYLOADENTRY._serialized_end=13285
+  _REDVOXPACKETM_EVENTSTREAM_EVENT_METADATAENTRY._serialized_start=432
+  _REDVOXPACKETM_EVENTSTREAM_EVENT_METADATAENTRY._serialized_end=479
+  _REDVOXPACKETM_SAMPLEPAYLOAD._serialized_start=13337
+  _REDVOXPACKETM_SAMPLEPAYLOAD._serialized_end=13613
+  _REDVOXPACKETM_SAMPLEPAYLOAD_METADATAENTRY._serialized_start=432
+  _REDVOXPACKETM_SAMPLEPAYLOAD_METADATAENTRY._serialized_end=479
+  _REDVOXPACKETM_DOUBLESAMPLEPAYLOAD._serialized_start=13616
+  _REDVOXPACKETM_DOUBLESAMPLEPAYLOAD._serialized_end=13904
+  _REDVOXPACKETM_DOUBLESAMPLEPAYLOAD_METADATAENTRY._serialized_start=432
+  _REDVOXPACKETM_DOUBLESAMPLEPAYLOAD_METADATAENTRY._serialized_end=479
+  _REDVOXPACKETM_TIMINGPAYLOAD._serialized_start=13907
+  _REDVOXPACKETM_TIMINGPAYLOAD._serialized_end=14244
+  _REDVOXPACKETM_TIMINGPAYLOAD_METADATAENTRY._serialized_start=432
+  _REDVOXPACKETM_TIMINGPAYLOAD_METADATAENTRY._serialized_end=479
+  _REDVOXPACKETM_SUMMARYSTATISTICS._serialized_start=14247
+  _REDVOXPACKETM_SUMMARYSTATISTICS._serialized_end=14492
+  _REDVOXPACKETM_SUMMARYSTATISTICS_METADATAENTRY._serialized_start=432
+  _REDVOXPACKETM_SUMMARYSTATISTICS_METADATAENTRY._serialized_end=479
+  _REDVOXPACKETM_UNIT._serialized_start=14495
+  _REDVOXPACKETM_UNIT._serialized_end=14882
+  _ENCRYPTEDREDVOXPACKETM._serialized_start=14885
+  _ENCRYPTEDREDVOXPACKETM._serialized_end=15057
+  _ENCRYPTEDREDVOXPACKETM_HEADER._serialized_start=14943
+  _ENCRYPTEDREDVOXPACKETM_HEADER._serialized_end=15057
+  _ACQUISITIONREQUEST._serialized_start=15060
+  _ACQUISITIONREQUEST._serialized_end=15197
+  _ACQUISITIONRESPONSE._serialized_start=15200
+  _ACQUISITIONRESPONSE._serialized_end=15445
+  _ACQUISITIONRESPONSE_RESPONSETYPE._serialized_start=15361
+  _ACQUISITIONRESPONSE_RESPONSETYPE._serialized_end=15445
+  _SYNCHREQUEST._serialized_start=15447
+  _SYNCHREQUEST._serialized_end=15539
+  _SYNCHRESPONSE._serialized_start=15542
+  _SYNCHRESPONSE._serialized_end=15675
 # @@protoc_insertion_point(module_scope)
```

### Comparing `redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/event_streams.py` & `redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/event_streams.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/audio.py` & `redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/audio.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/derived/movement.py` & `redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/derived/movement.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/image.py` & `redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/image.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/location.py` & `redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/location.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/sensors.py` & `redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/sensors.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/single.py` & `redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/single.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/sensors/xyz.py` & `redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/xyz.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/station_information.py` & `redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/station_information.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/timing_information.py` & `redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/timing_information.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api1000/wrapped_redvox_packet/wrapped_packet.py` & `redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/wrapped_packet.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api900/concat.py` & `redvox-3.4.2/redvox/api900/concat.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api900/deprecation.py` & `redvox-3.4.2/redvox/api900/deprecation.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api900/lib/api900_pb2.py` & `redvox-3.4.2/redvox/api900/lib/api900_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,45 +11,44 @@
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0c\x61pi900.proto\"\xf5\x05\n\x0cRedvoxPacket\x12\x0b\n\x03\x61pi\x18\x01 \x01(\r\x12\x0c\n\x04uuid\x18\x02 \x01(\t\x12\x11\n\tredvox_id\x18\x03 \x01(\t\x12\x1b\n\x13\x61uthenticated_email\x18\x04 \x01(\t\x12\x1c\n\x14\x61uthentication_token\x18\x05 \x01(\t\x12\x16\n\x0e\x66irebase_token\x18\x17 \x01(\t\x12\x15\n\ris_backfilled\x18\x06 \x01(\x08\x12\x12\n\nis_private\x18\x07 \x01(\x08\x12\x14\n\x0cis_scrambled\x18\x08 \x01(\x08\x12\x13\n\x0b\x64\x65vice_make\x18\t \x01(\t\x12\x14\n\x0c\x64\x65vice_model\x18\n \x01(\t\x12\x11\n\tdevice_os\x18\x0b \x01(\t\x12\x19\n\x11\x64\x65vice_os_version\x18\x0c \x01(\t\x12\x13\n\x0b\x61pp_version\x18\r \x01(\t\x12\x1d\n\x15\x62\x61ttery_level_percent\x18\x18 \x01(\x02\x12\x1c\n\x14\x64\x65vice_temperature_c\x18\x19 \x01(\x02\x12\x1a\n\x12\x61\x63quisition_server\x18\x0e \x01(\t\x12#\n\x1btime_synchronization_server\x18\x0f \x01(\t\x12\x1d\n\x15\x61uthentication_server\x18\x10 \x01(\t\x12\x37\n/app_file_start_timestamp_epoch_microseconds_utc\x18\x11 \x01(\x03\x12(\n app_file_start_timestamp_machine\x18\x12 \x01(\x03\x12/\n\'server_timestamp_epoch_microseconds_utc\x18\x13 \x01(\x03\x12\x36\n\x17\x65venly_sampled_channels\x18\x14 \x03(\x0b\x32\x15.EvenlySampledChannel\x12:\n\x19unevenly_sampled_channels\x18\x15 \x03(\x0b\x32\x17.UnevenlySampledChannel\x12\x10\n\x08metadata\x18\x16 \x03(\t\"\x1f\n\x0cInt32Payload\x12\x0f\n\x07payload\x18\x01 \x03(\x05\" \n\rUInt32Payload\x12\x0f\n\x07payload\x18\x01 \x03(\r\"\x1f\n\x0cInt64Payload\x12\x0f\n\x07payload\x18\x01 \x03(\x03\" \n\rUInt64Payload\x12\x0f\n\x07payload\x18\x01 \x03(\x04\"!\n\x0e\x46loat32Payload\x12\x0f\n\x07payload\x18\x01 \x03(\x02\"!\n\x0e\x46loat64Payload\x12\x0f\n\x07payload\x18\x01 \x03(\x01\"\x8c\x02\n\x0b\x42ytePayload\x12\x35\n\x0f\x62ytePayloadType\x18\x01 \x01(\x0e\x32\x1c.BytePayload.BytePayloadType\x12\x0f\n\x07payload\x18\x02 \x01(\x0c\"\xb4\x01\n\x0f\x42ytePayloadType\x12\t\n\x05\x42YTES\x10\x00\x12\t\n\x05UINT8\x10\x01\x12\x0b\n\x07UNINT16\x10\x02\x12\x0b\n\x07UNINT24\x10\x03\x12\n\n\x06UINT32\x10\x04\x12\n\n\x06UINT64\x10\x05\x12\x08\n\x04INT8\x10\x06\x12\t\n\x05INT16\x10\x07\x12\t\n\x05INT24\x10\x08\x12\t\n\x05INT32\x10\t\x12\t\n\x05INT64\x10\n\x12\x0b\n\x07\x46LOAT32\x10\x0b\x12\x0b\n\x07\x46LOAT64\x10\x0c\x12\t\n\x05OTHER\x10\r\"\x9e\x04\n\x14\x45venlySampledChannel\x12#\n\rchannel_types\x18\x01 \x03(\x0e\x32\x0c.ChannelType\x12\x13\n\x0bsensor_name\x18\x02 \x01(\t\x12\x16\n\x0esample_rate_hz\x18\x03 \x01(\x01\x12\x35\n-first_sample_timestamp_epoch_microseconds_utc\x18\x04 \x01(\x03\x12$\n\x0c\x62yte_payload\x18\x05 \x01(\x0b\x32\x0c.BytePayloadH\x00\x12(\n\x0euint32_payload\x18\x06 \x01(\x0b\x32\x0e.UInt32PayloadH\x00\x12(\n\x0euint64_payload\x18\x07 \x01(\x0b\x32\x0e.UInt64PayloadH\x00\x12&\n\rint32_payload\x18\x08 \x01(\x0b\x32\r.Int32PayloadH\x00\x12&\n\rint64_payload\x18\t \x01(\x0b\x32\r.Int64PayloadH\x00\x12*\n\x0f\x66loat32_payload\x18\n \x01(\x0b\x32\x0f.Float32PayloadH\x00\x12*\n\x0f\x66loat64_payload\x18\x0b \x01(\x0b\x32\x0f.Float64PayloadH\x00\x12\x13\n\x0bvalue_means\x18\x0c \x03(\x01\x12\x12\n\nvalue_stds\x18\r \x03(\x01\x12\x15\n\rvalue_medians\x18\x0e \x03(\x01\x12\x10\n\x08metadata\x18\x0f \x03(\tB\t\n\x07payload\"\xd1\x04\n\x16UnevenlySampledChannel\x12#\n\rchannel_types\x18\x01 \x03(\x0e\x32\x0c.ChannelType\x12\x13\n\x0bsensor_name\x18\x02 \x01(\t\x12#\n\x1btimestamps_microseconds_utc\x18\x03 \x03(\x03\x12$\n\x0c\x62yte_payload\x18\x04 \x01(\x0b\x32\x0c.BytePayloadH\x00\x12(\n\x0euint32_payload\x18\x05 \x01(\x0b\x32\x0e.UInt32PayloadH\x00\x12(\n\x0euint64_payload\x18\x06 \x01(\x0b\x32\x0e.UInt64PayloadH\x00\x12&\n\rint32_payload\x18\x07 \x01(\x0b\x32\r.Int32PayloadH\x00\x12&\n\rint64_payload\x18\x08 \x01(\x0b\x32\r.Int64PayloadH\x00\x12*\n\x0f\x66loat32_payload\x18\t \x01(\x0b\x32\x0f.Float32PayloadH\x00\x12*\n\x0f\x66loat64_payload\x18\n \x01(\x0b\x32\x0f.Float64PayloadH\x00\x12\x1c\n\x14sample_interval_mean\x18\x0b \x01(\x01\x12\x1b\n\x13sample_interval_std\x18\x0c \x01(\x01\x12\x1e\n\x16sample_interval_median\x18\r \x01(\x01\x12\x13\n\x0bvalue_means\x18\x0e \x03(\x01\x12\x12\n\nvalue_stds\x18\x0f \x03(\x01\x12\x15\n\rvalue_medians\x18\x10 \x03(\x01\x12\x10\n\x08metadata\x18\x11 \x03(\tB\t\n\x07payload\"\xd7\x01\n\x14RedvoxPacketResponse\x12(\n\x04type\x18\x01 \x01(\x0e\x32\x1a.RedvoxPacketResponse.Type\x12\x10\n\x08\x63hecksum\x18\x02 \x01(\x03\x12+\n\x06\x65rrors\x18\x03 \x03(\x0e\x32\x1b.RedvoxPacketResponse.Error\x12\x10\n\x08metadata\x18\x04 \x03(\t\"\x19\n\x04Type\x12\x06\n\x02OK\x10\x00\x12\t\n\x05\x45RROR\x10\x01\")\n\x05\x45rror\x12\x15\n\x11NOT_AUTHENTICATED\x10\x00\x12\t\n\x05OTHER\x10\x01*\x97\x03\n\x0b\x43hannelType\x12\x0e\n\nMICROPHONE\x10\x00\x12\r\n\tBAROMETER\x10\x01\x12\x0c\n\x08LATITUDE\x10\x02\x12\r\n\tLONGITUDE\x10\x03\x12\t\n\x05SPEED\x10\x04\x12\x0c\n\x08\x41LTITUDE\x10\x05\x12\x0e\n\nRESERVED_0\x10\x06\x12\x0e\n\nRESERVED_1\x10\x07\x12\x0e\n\nRESERVED_2\x10\x08\x12\x18\n\x14TIME_SYNCHRONIZATION\x10\t\x12\x0c\n\x08\x41\x43\x43URACY\x10\n\x12\x13\n\x0f\x41\x43\x43\x45LEROMETER_X\x10\x0b\x12\x13\n\x0f\x41\x43\x43\x45LEROMETER_Y\x10\x0c\x12\x13\n\x0f\x41\x43\x43\x45LEROMETER_Z\x10\r\x12\x12\n\x0eMAGNETOMETER_X\x10\x0e\x12\x12\n\x0eMAGNETOMETER_Y\x10\x0f\x12\x12\n\x0eMAGNETOMETER_Z\x10\x10\x12\x0f\n\x0bGYROSCOPE_X\x10\x11\x12\x0f\n\x0bGYROSCOPE_Y\x10\x12\x12\x0f\n\x0bGYROSCOPE_Z\x10\x13\x12\t\n\x05OTHER\x10\x14\x12\t\n\x05LIGHT\x10\x15\x12\t\n\x05IMAGE\x10\x16\x12\x0c\n\x08INFRARED\x10\x17\x42\x10\n\x0eio.redvox.apisb\x06proto3')
 
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'api900_pb2', _globals)
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'api900_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\016io.redvox.apis'
-  _globals['_CHANNELTYPE']._serialized_start=2611
-  _globals['_CHANNELTYPE']._serialized_end=3018
-  _globals['_REDVOXPACKET']._serialized_start=17
-  _globals['_REDVOXPACKET']._serialized_end=774
-  _globals['_INT32PAYLOAD']._serialized_start=776
-  _globals['_INT32PAYLOAD']._serialized_end=807
-  _globals['_UINT32PAYLOAD']._serialized_start=809
-  _globals['_UINT32PAYLOAD']._serialized_end=841
-  _globals['_INT64PAYLOAD']._serialized_start=843
-  _globals['_INT64PAYLOAD']._serialized_end=874
-  _globals['_UINT64PAYLOAD']._serialized_start=876
-  _globals['_UINT64PAYLOAD']._serialized_end=908
-  _globals['_FLOAT32PAYLOAD']._serialized_start=910
-  _globals['_FLOAT32PAYLOAD']._serialized_end=943
-  _globals['_FLOAT64PAYLOAD']._serialized_start=945
-  _globals['_FLOAT64PAYLOAD']._serialized_end=978
-  _globals['_BYTEPAYLOAD']._serialized_start=981
-  _globals['_BYTEPAYLOAD']._serialized_end=1249
-  _globals['_BYTEPAYLOAD_BYTEPAYLOADTYPE']._serialized_start=1069
-  _globals['_BYTEPAYLOAD_BYTEPAYLOADTYPE']._serialized_end=1249
-  _globals['_EVENLYSAMPLEDCHANNEL']._serialized_start=1252
-  _globals['_EVENLYSAMPLEDCHANNEL']._serialized_end=1794
-  _globals['_UNEVENLYSAMPLEDCHANNEL']._serialized_start=1797
-  _globals['_UNEVENLYSAMPLEDCHANNEL']._serialized_end=2390
-  _globals['_REDVOXPACKETRESPONSE']._serialized_start=2393
-  _globals['_REDVOXPACKETRESPONSE']._serialized_end=2608
-  _globals['_REDVOXPACKETRESPONSE_TYPE']._serialized_start=2540
-  _globals['_REDVOXPACKETRESPONSE_TYPE']._serialized_end=2565
-  _globals['_REDVOXPACKETRESPONSE_ERROR']._serialized_start=2567
-  _globals['_REDVOXPACKETRESPONSE_ERROR']._serialized_end=2608
+  _CHANNELTYPE._serialized_start=2611
+  _CHANNELTYPE._serialized_end=3018
+  _REDVOXPACKET._serialized_start=17
+  _REDVOXPACKET._serialized_end=774
+  _INT32PAYLOAD._serialized_start=776
+  _INT32PAYLOAD._serialized_end=807
+  _UINT32PAYLOAD._serialized_start=809
+  _UINT32PAYLOAD._serialized_end=841
+  _INT64PAYLOAD._serialized_start=843
+  _INT64PAYLOAD._serialized_end=874
+  _UINT64PAYLOAD._serialized_start=876
+  _UINT64PAYLOAD._serialized_end=908
+  _FLOAT32PAYLOAD._serialized_start=910
+  _FLOAT32PAYLOAD._serialized_end=943
+  _FLOAT64PAYLOAD._serialized_start=945
+  _FLOAT64PAYLOAD._serialized_end=978
+  _BYTEPAYLOAD._serialized_start=981
+  _BYTEPAYLOAD._serialized_end=1249
+  _BYTEPAYLOAD_BYTEPAYLOADTYPE._serialized_start=1069
+  _BYTEPAYLOAD_BYTEPAYLOADTYPE._serialized_end=1249
+  _EVENLYSAMPLEDCHANNEL._serialized_start=1252
+  _EVENLYSAMPLEDCHANNEL._serialized_end=1794
+  _UNEVENLYSAMPLEDCHANNEL._serialized_start=1797
+  _UNEVENLYSAMPLEDCHANNEL._serialized_end=2390
+  _REDVOXPACKETRESPONSE._serialized_start=2393
+  _REDVOXPACKETRESPONSE._serialized_end=2608
+  _REDVOXPACKETRESPONSE_TYPE._serialized_start=2540
+  _REDVOXPACKETRESPONSE_TYPE._serialized_end=2565
+  _REDVOXPACKETRESPONSE_ERROR._serialized_start=2567
+  _REDVOXPACKETRESPONSE_ERROR._serialized_end=2608
 # @@protoc_insertion_point(module_scope)
```

### Comparing `redvox-3.4.1/redvox/api900/location_analyzer.py` & `redvox-3.4.2/redvox/api900/location_analyzer.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api900/migrations.py` & `redvox-3.4.2/redvox/api900/migrations.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api900/qa/gap_detection.py` & `redvox-3.4.2/redvox/api900/qa/gap_detection.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api900/reader.py` & `redvox-3.4.2/redvox/api900/reader.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api900/reader_utils.py` & `redvox-3.4.2/redvox/api900/reader_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api900/sensors/accelerometer_sensor.py` & `redvox-3.4.2/redvox/api900/sensors/accelerometer_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api900/sensors/barometer_sensor.py` & `redvox-3.4.2/redvox/api900/sensors/barometer_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api900/sensors/evenly_sampled_channel.py` & `redvox-3.4.2/redvox/api900/sensors/evenly_sampled_channel.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api900/sensors/evenly_sampled_sensor.py` & `redvox-3.4.2/redvox/api900/sensors/evenly_sampled_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api900/sensors/gyroscope_sensor.py` & `redvox-3.4.2/redvox/api900/sensors/gyroscope_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api900/sensors/image_sensor.py` & `redvox-3.4.2/redvox/api900/sensors/image_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api900/sensors/infrared_sensor.py` & `redvox-3.4.2/redvox/api900/sensors/infrared_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api900/sensors/interleaved_channel.py` & `redvox-3.4.2/redvox/api900/sensors/interleaved_channel.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api900/sensors/light_sensor.py` & `redvox-3.4.2/redvox/api900/sensors/light_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api900/sensors/location_sensor.py` & `redvox-3.4.2/redvox/api900/sensors/location_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api900/sensors/magnetometer_sensor.py` & `redvox-3.4.2/redvox/api900/sensors/magnetometer_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api900/sensors/microphone_sensor.py` & `redvox-3.4.2/redvox/api900/sensors/microphone_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api900/sensors/time_synchronization_sensor.py` & `redvox-3.4.2/redvox/api900/sensors/time_synchronization_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api900/sensors/unevenly_sampled_channel.py` & `redvox-3.4.2/redvox/api900/sensors/unevenly_sampled_channel.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api900/sensors/unevenly_sampled_sensor.py` & `redvox-3.4.2/redvox/api900/sensors/unevenly_sampled_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api900/sensors/xyz_unevenly_sampled_sensor.py` & `redvox-3.4.2/redvox/api900/sensors/xyz_unevenly_sampled_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api900/stat_utils.py` & `redvox-3.4.2/redvox/api900/stat_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api900/summarize.py` & `redvox-3.4.2/redvox/api900/summarize.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api900/timesync/api900_timesync.py` & `redvox-3.4.2/redvox/api900/timesync/api900_timesync.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api900/timesync/tri_message_stats.py` & `redvox-3.4.2/redvox/api900/timesync/tri_message_stats.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api900/types.py` & `redvox-3.4.2/redvox/api900/types.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/api900/wrapped_redvox_packet.py` & `redvox-3.4.2/redvox/api900/wrapped_redvox_packet.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/cli/cli.py` & `redvox-3.4.2/redvox/cli/cli.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/cli/conversions.py` & `redvox-3.4.2/redvox/cli/conversions.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/cli/data_req.py` & `redvox-3.4.2/redvox/cli/data_req.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/cloud/api.py` & `redvox-3.4.2/redvox/cloud/api.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/cloud/api_m_fqns.py` & `redvox-3.4.2/redvox/cloud/api_m_fqns.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/cloud/auth_api.py` & `redvox-3.4.2/redvox/cloud/auth_api.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/cloud/client.py` & `redvox-3.4.2/redvox/cloud/client.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/cloud/config.py` & `redvox-3.4.2/redvox/cloud/config.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/cloud/data_api.py` & `redvox-3.4.2/redvox/cloud/data_api.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/cloud/data_client.py` & `redvox-3.4.2/redvox/cloud/data_client.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/cloud/data_io.py` & `redvox-3.4.2/redvox/cloud/data_io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/cloud/metadata_api.py` & `redvox-3.4.2/redvox/cloud/metadata_api.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/cloud/query_timing_correction.py` & `redvox-3.4.2/redvox/cloud/query_timing_correction.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/cloud/routes.py` & `redvox-3.4.2/redvox/cloud/routes.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/cloud/station_stats.py` & `redvox-3.4.2/redvox/cloud/station_stats.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/cloud/subscription.py` & `redvox-3.4.2/redvox/cloud/subscription.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/common/api_conversions.py` & `redvox-3.4.2/redvox/common/api_conversions.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/common/api_reader.py` & `redvox-3.4.2/redvox/common/api_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,31 +222,31 @@
         timing_offsets: Optional[om.TimingOffsets] = om.compute_offsets(stats)
 
         # punt if duration or other important values are invalid or if the latency array was empty
         if timing_offsets is None:
             return [station_index]
 
         # if our filtered files do not encompass the request even when the packet times are updated
-        # try getting 1.5 times the difference of the expected start/end and the start/end of the data
+        # try getting the difference of the expected start/end and the start/end of the data plus one packet
         insufficient_str = ""
         if (self.filter.start_dt and timing_offsets.adjusted_start > self.filter.start_dt) or \
                 (self.filter.end_dt and timing_offsets.adjusted_start >= self.filter.end_dt):
             insufficient_str += f" {self.filter.start_dt} (start)"
             new_end = self.filter.start_dt - self.filter.start_dt_buf
-            new_start = new_end - 1.5 * (timing_offsets.adjusted_start - self.filter.start_dt)
+            new_start = new_end - (timing_offsets.adjusted_start - self.filter.start_dt + stats[0].packet_duration)
             new_index = self._redo_index(set(station_index.summarize().station_ids()), new_start, new_end)
             if new_index:
                 station_index.append(new_index.entries)
                 stats.extend(fs.extract_stats(new_index))
 
         if (self.filter.end_dt and timing_offsets.adjusted_end < self.filter.end_dt) or \
                 (self.filter.start_dt and timing_offsets.adjusted_end <= self.filter.start_dt):
             insufficient_str += f" {self.filter.end_dt} (end)"
             new_start = self.filter.end_dt + self.filter.end_dt_buf
-            new_end = new_start + 1.5 * (self.filter.end_dt - timing_offsets.adjusted_end)
+            new_end = new_start + (self.filter.end_dt - timing_offsets.adjusted_end + stats[0].packet_duration)
             new_index = self._redo_index(set(station_index.summarize().station_ids()), new_start, new_end)
             if new_index:
                 station_index.append(new_index.entries)
                 stats.extend(fs.extract_stats(new_index))
 
         if len(insufficient_str) > 0:
             self.errors.append(f"Data for {station_index.summarize().station_ids()} exists, "
```

### Comparing `redvox-3.4.1/redvox/common/api_reader_dw.py` & `redvox-3.4.2/redvox/common/api_reader_dw.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,26 +62,25 @@
         split_list = self._split_workload(findex)
         use_temp_dir = True if len(split_list) > 1 else False
 
         if len(split_list) > 0:
             if self.debug and use_temp_dir:
                 print("Writing data to disk; this may take a few minutes to complete.")
             stpa = Station.create_from_indexes(split_list,
+                                               correct_timestamps=self.correct_timestamps,
                                                use_model_correction=self.use_model_correction,
                                                base_out_dir=self.dw_base_dir,
                                                use_temp_dir=use_temp_dir
                                                )
             if self.debug:
                 print(f"station {stpa.id()} files read: {len(findex.entries)}")
                 if len(split_list) > 1:
                     print(f"required making {len(split_list)} smaller segments due to memory restraints")
             if self.dw_save_mode == io.FileSystemSaveMode.MEM and use_temp_dir:
                 self.dw_save_mode = io.FileSystemSaveMode.TEMP
-            if self.correct_timestamps:
-                stpa.set_correct_timestamps()
             return stpa
         self.errors.append("No files found to create station.")
         return Station()
 
     def get_stations(self, pool: Optional[multiprocessing.pool.Pool] = None) -> List[Station]:
         """
         :return: a list of stations read by the ApiReader
```

### Comparing `redvox-3.4.1/redvox/common/constants.py` & `redvox-3.4.2/redvox/common/constants.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/common/cross_stats.py` & `redvox-3.4.2/redvox/common/cross_stats.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/common/data_window.py` & `redvox-3.4.2/redvox/common/data_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from redvox.common.date_time_utils import (
     datetime_to_epoch_microseconds_utc as us_dt,
 )
 from redvox.common import io
 from redvox.common import data_window_io as dw_io
 from redvox.common.data_window_configuration import DataWindowConfigFile
 from redvox.common.parallel_utils import maybe_parallel_map
-from redvox.common.station import Station
+from redvox.common.station import Station, STATION_ID_LENGTH
 from redvox.common.sensor_data import SensorType, SensorData
 from redvox.common.api_reader_dw import ApiReaderDw
 from redvox.common import gap_and_pad_utils as gpu
 from redvox.common.errors import RedVoxExceptions
 
 DEFAULT_START_BUFFER_TD: timedelta = timedelta(minutes=2.0)  # default padding to start time of data
 DEFAULT_END_BUFFER_TD: timedelta = timedelta(minutes=2.0)  # default padding to end time of data
@@ -113,14 +113,16 @@
         return EventOrigin(data_dict["provider"], data_dict["latitude"], data_dict["latitude_std"],
                            data_dict["longitude"], data_dict["longitude_std"], data_dict["altitude"],
                            data_dict["altitude_std"], data_dict["event_radius_m"])
 
 
 class DataWindowConfig:
     """
+    Configuration of DataWindow properties
+
     Properties:
         input_dir: str, the directory that contains all the data.  REQUIRED
 
         structured_layout: bool, if True, the input_dir contains specially named and organized
         directories of data.  Default True
 
         start_datetime: optional datetime, start datetime of the window.
@@ -246,15 +248,18 @@
                                 data_dict["apply_correction"], data_dict["use_model_correction"],
                                 gpu.DataPointCreationMode(data_dict["copy_edge_points"])
                                 )
 
 
 class DataWindow:
     """
-    Holds the data for a given time window; adds interpolated timestamps to fill gaps and pad start and end values
+    Holds the data for a given time window; adds interpolated timestamps to fill gaps and pad the start and end values
+    If a start time is given, data starting from that time will be included.
+    If an end time is given, data up to but not including that time will be included.
+    Refer to the DataWindowConfig class for more details on DataWindow parameters.
 
     Properties:
         event_name: str, name of the DataWindow.  defaults to "dw"
 
         event_origin: Optional EventOrigin which describes the physical location and radius of the
         origin event.  Default empty EventOrigin (no valid data)
 
@@ -764,28 +769,28 @@
             if not s.has_audio_sensor():
                 remove.append(s.get_key())
         if len(remove) > 0:
             self._stations = [s for s in self._stations if s.get_key() not in remove]
 
     def _check_valid_ids(self):
         """
-        if there are stations, searches the station_ids for any ids not in the data collected
+        if there are stations, searches the config's station_ids for any ids not in the data collected
         and creates an error message for each id requested but has no data
         if there are no stations, creates a single error message declaring no data found
         """
         if len(self._stations) < 1 and self._config.station_ids:
             if len(self._config.station_ids) > 1:
                 add_ids = f"for all stations {self._config.station_ids} "
             else:
                 add_ids = ""
             self._errors.append(f"No data matching criteria {add_ids}in {self._config.input_dir}"
                                 f"\nPlease adjust parameters of DataWindow")
         elif len(self._stations) > 0 and self._config.station_ids:
             for ids in self._config.station_ids:
-                if ids.zfill(10) not in [i.id() for i in self._stations]:
+                if ids.zfill(STATION_ID_LENGTH) not in [i.id() for i in self._stations]:
                     self._errors.append(
                         f"Requested {ids} but there is no data to read for that station"
                     )
 
     def create_window_in_sensors(
             self, station: Station, start_datetime: Optional[dtu.datetime] = None,
             end_datetime: Optional[dtu.datetime] = None
@@ -804,15 +809,14 @@
             start_datetime = dtu.datetime_to_epoch_microseconds_utc(start_datetime)
         else:
             start_datetime = 0
         if end_datetime:
             end_datetime = dtu.datetime_to_epoch_microseconds_utc(end_datetime)
         else:
             end_datetime = dtu.datetime_to_epoch_microseconds_utc(dtu.datetime.max)
-        # process events?
         self.process_sensor(station.audio_sensor(), station.id(), start_datetime, end_datetime)
         if station.has_audio_data():
             for sensor in [s for s in station.data() if s.type() != SensorType.AUDIO]:
                 self.process_sensor(sensor, station.id(), station.audio_sensor().first_data_timestamp(),
                                     station.audio_sensor().last_data_timestamp())
             # recalculate metadata
             station.update_first_and_last_data_timestamps()
@@ -856,14 +860,15 @@
             # check if all the samples have been cut off
             is_audio = sensor.type() == SensorType.AUDIO
             if end_index <= start_index:
                 self._errors.append(
                     f"Data window for {station_id} {'Audio' if is_audio else sensor.type().name} "
                     f"sensor has truncated all data points"
                 )
+                # adjust data window to match the conditions of the remaining data
                 if is_audio:
                     sensor.empty_data_table()
                 elif last_before_start is not None and first_after_end is None:
                     first_entry = sensor.pyarrow_table().slice(last_before_start, 1).to_pydict()
                     first_entry["timestamps"] = [start_date_timestamp]
                     sensor.write_pyarrow_table(pa.Table.from_pydict(first_entry))
                 elif last_before_start is None and first_after_end is not None:
```

### Comparing `redvox-3.4.1/redvox/common/data_window_configuration.py` & `redvox-3.4.2/redvox/common/data_window_configuration.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/common/data_window_io.py` & `redvox-3.4.2/redvox/common/data_window_io.py`

 * *Files 25% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from redvox.common.date_time_utils import (
     datetime_to_epoch_microseconds_utc as us_dt,
 )
 
 
 if TYPE_CHECKING:
     from redvox.common.data_window import DataWindow, DataWindowConfig
-    from redvox.common.data_window_old import DataWindow as DwOld
 
 
 class DataWindowOutputType(enum.Enum):
     """
     Type of file to create when exporting DataWindow
     """
 
@@ -118,156 +117,14 @@
 @dataclass
 class DataWindowSerializationResult:
     path: str
     serialized_bytes: int
     compressed_bytes: int
 
 
-def serialize_data_window_old(
-        data_window: "DwOld",
-        base_dir: str = ".",
-        file_name: Optional[str] = None,
-        compression_factor: int = 4,
-) -> Path:
-    """
-    Serializes and compresses a DataWindow to a file.
-
-    :param data_window: The data window to serialize and compress.
-    :param base_dir: The base directory to write the serialized file to (default=.).
-    :param file_name: The optional file name. If None, a default filename with the following format is used:
-                      [start_ts]_[end_ts]_[num_stations].pkl.lz4
-    :param compression_factor: A value between 1 and 12. Higher values provide better compression, but take longer.
-                               (default=4).
-    :return: The path to the written file.
-    """
-
-    _file_name: str = (
-        file_name
-        if file_name is not None
-        else f"{int(data_window.start_datetime.timestamp())}"
-             f"_{int(data_window.end_datetime.timestamp())}"
-             f"_{len(data_window.station_ids)}.pkl.lz4"
-    )
-
-    file_path: Path = Path(base_dir).joinpath(_file_name)
-
-    with lz4.frame.open(
-            file_path, "wb", compression_level=compression_factor
-    ) as compressed_out:
-        pickle.dump(data_window, compressed_out)
-        compressed_out.flush()
-        return file_path.resolve(False)
-
-
-def deserialize_data_window_old(path: str) -> "DwOld":
-    """
-    Decompresses and deserializes a DataWindow written to disk.
-
-    :param path: Path to the serialized and compressed data window.
-    :return: An instance of a DataWindow.
-    """
-    with lz4.frame.open(path, "rb") as compressed_in:
-        return pickle.load(compressed_in)
-
-
-def json_file_to_data_window_old(base_dir: str, file_name: str) -> Dict:
-    """
-    load a data window from json written to disk
-
-    :param base_dir: directory where json file is saved
-    :param file_name: name of json file to load
-    :return: a dictionary representing a json-ified data window
-    """
-    with open(Path(base_dir).joinpath(file_name), "r") as r_f:
-        return json_to_dict(r_f.read())
-
-
-def data_window_to_json_old(
-        data_win: "DwOld",
-        base_dir: str = ".",
-        file_name: Optional[str] = None,
-        compression_format: str = "lz4",
-) -> str:
-    """
-    Converts a data window to json format
-
-    :param data_win: the data window object to convert
-    :param base_dir: the base directory to write the data file to
-    :param file_name: the data object's optional base file name.  Do not include a file extension.
-                        If None, a default file name is created using this format:
-                        [start_ts]_[end_ts]_[num_stations].[compression_type]
-    :param compression_format: the compression format to use.  default lz4
-    :return: The path to the written file
-    """
-    _file_name: str = (
-        file_name
-        if file_name is not None
-        else f"{int(data_win.start_datetime.timestamp())}"
-             f"_{int(data_win.end_datetime.timestamp())}"
-             f"_{len(data_win.station_ids)}"
-    )
-    base_dir = os.path.join(base_dir, "dw")
-    if not os.path.exists(base_dir):
-        os.makedirs(base_dir)
-    if compression_format == "lz4":
-        _ = str(
-            serialize_data_window_old(
-                data_win, base_dir, _file_name + ".pkl.lz4"
-            ).resolve()
-        )
-    else:
-        dfp = os.path.join(base_dir, _file_name + ".pkl")
-        with open(dfp, "wb") as compressed_out:
-            pickle.dump(data_win, compressed_out)
-    data_win_dict = {
-        "start_datetime": us_dt(data_win.start_datetime)
-        if data_win.start_datetime
-        else None,
-        "end_datetime": us_dt(data_win.end_datetime) if data_win.end_datetime else None,
-        "station_ids": list(data_win.station_ids),
-        "compression_format": compression_format,
-        "file_name": _file_name,
-    }
-    return json.dumps(data_win_dict)
-
-
-def data_window_to_json_file_old(
-        data_window: "DwOld",
-        base_dir: str = ".",
-        file_name: Optional[str] = None,
-        compression_format: str = "lz4",
-) -> Path:
-    """
-    Converts a data window to json format.
-
-    :param data_window: the data window object to convert
-    :param base_dir: the base directory to write the json file to
-    :param file_name: the optional base file name.  Do not include a file extension.
-                        If None, a default file name is created using this format:
-                        [start_ts]_[end_ts]_[num_stations].json
-    :param compression_format: the type of compression to use.  default lz4
-    :return: The path to the written file
-    """
-    _file_name: str = (
-        file_name
-        if file_name is not None
-        else f"{int(data_window.start_datetime.timestamp())}"
-             f"_{int(data_window.end_datetime.timestamp())}"
-             f"_{len(data_window.station_ids)}"
-    )
-    file_path: Path = Path(base_dir).joinpath(f"{_file_name}.json")
-    with open(file_path, "w") as f_p:
-        f_p.write(
-            data_window_to_json_old(
-                data_window, base_dir, file_name, compression_format
-            )
-        )
-        return file_path.resolve(False)
-
-
 def data_window_as_json(
         data_window: "DataWindow"
 ) -> str:
     """
     Converts the DataWindow's metadata into a JSON dictionary
 
     :param data_window: The data window to convert
```

### Comparing `redvox-3.4.1/redvox/common/date_time_utils.py` & `redvox-3.4.2/redvox/common/date_time_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/common/errors.py` & `redvox-3.4.2/redvox/common/errors.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/common/event_stream.py` & `redvox-3.4.2/redvox/common/event_stream.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             self._data = get_empty_event_data_dict()
 
     def __repr__(self):
         return f"name: {self.name}, " \
                f"timestamp: {self._timestamp}, " \
                f"uncorrected_timestamp: {self._uncorrected_timestamp}, " \
                f"schema: {self.get_schema()}, " \
-               f"save_mode: {self._fs_writer.save_mode().value}"
+               f"save_mode: {self._fs_writer.save_mode()}"
 
     def __str__(self):
         return f"name: {self.name}, " \
                f"timestamp: {self._timestamp}, " \
                f"uncorrected_timestamp: {self._uncorrected_timestamp}, " \
                f"schema: {self.__schema_as_str()}"
 
@@ -429,14 +429,27 @@
                                     otherwise uses the best offset (model's intercept value).  Default False
         """
         if self.is_timestamp_corrected():
             self._errors.append("Timestamps already corrected!")
         else:
             self._timestamp = offset_model.update_time(self._timestamp, use_model_function)
 
+    def original_timestamps(self, offset_model: om.OffsetModel, use_model_function: bool = False):
+        """
+        undo the update to the timestamp of the Event
+
+        :param offset_model: model used to update the timestamps
+        :param use_model_function: if True, use the model's slope function to update the timestamps.
+                                    otherwise uses the best offset (model's intercept value).  Default False
+        """
+        if not self.is_timestamp_corrected():
+            self._errors.append("Timestamps already not corrected!")
+        else:
+            self._timestamp = offset_model.get_original_time(self._timestamp, use_model_function)
+
     def default_json_file_name(self) -> str:
         """
         :return: default event json file name (event_[event.name]): note there is no extension
         """
         return f"event_{self.name}"
 
     def is_save_to_disk(self) -> bool:
@@ -795,25 +808,27 @@
         :return: idealized event sample hop rate in hz
         """
         return self.input_sample_rate / self.samples_per_hop
 
     def create_event_window(self, start: float = -np.inf, end: float = np.inf):
         """
         removes any event in the stream that doesn't match start <= event < end
+        adds empty events to beginning and end of data (as long as the corresponding input values are not infinity)
         default start is negative infinity, default end is infinity
         all times in microseconds since epoch UTC
 
         :param start: inclusive start time of events to keep
         :param end: exclusive end time of events to keep
         """
         self.events = [s for s in self.events if start <= s.get_timestamp() < end]
         if self.num_events() > 0:
-            if start < self.events[0].get_timestamp():
+            if start < self.events[0].get_timestamp() and not np.isinf(start):
                 self.events.insert(0, Event(start, self.name))
-            self.events.append(Event(end, self.name))
+            if not np.isinf(end):
+                self.events.append(Event(end - 1, self.name))
 
     def get_file_names(self) -> List[str]:
         """
         :return: the names of the files which store the event data
         """
         return [e.file_name() for e in self.events]
 
@@ -852,14 +867,25 @@
         :param offset_model: model used to update the timestamps
         :param use_model_function: if True, use the model's slope function to update the timestamps.
                                     otherwise uses the best offset (model's intercept value).  Default False
         """
         for evnt in self.events:
             evnt.update_timestamps(offset_model, use_model_function)
 
+    def original_timestamps(self, offset_model: om.OffsetModel, use_model_function: bool = False):
+        """
+        undo the update to the timestamps in the data
+
+        :param offset_model: model used to update the timestamps
+        :param use_model_function: if True, use the model's slope function to update the timestamps.
+                                    otherwise uses the best offset (model's intercept value).  Default False
+        """
+        for evnt in self.events:
+            evnt.original_timestamps(offset_model, use_model_function)
+
     @staticmethod
     def from_json_dict(json_dict: dict) -> "EventStream":
         """
         :param json_dict: json dict to parse
         :return: EventStream from json dict
         """
         if "name" in json_dict.keys():
@@ -1043,14 +1069,25 @@
         :param offset_model: model used to update the timestamps
         :param use_model_function: if True, use the model's slope function to update the timestamps.
                                     otherwise uses the best offset (model's intercept value).  Default False
         """
         for evnt in self.streams:
             evnt.update_timestamps(offset_model, use_model_function)
 
+    def original_timestamps(self, offset_model: om.OffsetModel, use_model_function: bool = False):
+        """
+        undo the update to the timestamps in the data
+
+        :param offset_model: model used to update the timestamps
+        :param use_model_function: if True, use the model's slope function to update the timestamps.
+                                    otherwise uses the best offset (model's intercept value).  Default False
+        """
+        for evnt in self.streams:
+            evnt.original_timestamps(offset_model, use_model_function)
+
     @staticmethod
     def from_json_file(file_dir: str, file_name: str) -> "EventStreams":
         """
         :param file_dir: full path to containing directory for the file
         :param file_name: name of file to load data from
         :return: EventStreams from json file
         """
```

### Comparing `redvox-3.4.1/redvox/common/event_stream_io.py` & `redvox-3.4.2/redvox/common/event_stream_io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/common/file_statistics.py` & `redvox-3.4.2/redvox/common/file_statistics.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Any, Callable, Iterator, List, Optional, Tuple, TYPE_CHECKING, Union
 import math
 import multiprocessing
 from multiprocessing.pool import Pool
 
 import numpy as np
 
-from redvox.common.timesync_old import TimeSyncData
+from redvox.common.timesync import TimeSync
 from redvox.common.parallel_utils import maybe_parallel_map
 
 # noinspection Mypy
 if TYPE_CHECKING:
     from redvox.api1000.wrapped_redvox_packet.sensors.audio import Audio
     from redvox.api1000.wrapped_redvox_packet.sensors.location import Location
     from redvox.api1000.wrapped_redvox_packet.sensors.sensors import Sensors
@@ -211,26 +211,22 @@
         :return: An instance of StationStat.
         """
         mtz: Optional[float] = packet.mach_time_zero()
 
         best_offset = packet.best_offset()
         best_latency = packet.best_latency()
         if packet.has_time_synchronization_sensor():
-            tsd = TimeSyncData(
-                packet.redvox_id(),
+            tsd = TimeSync(
                 time_sync_exchanges_list=list(
                     packet.time_synchronization_sensor().payload_values()
-                ),
-                packet_start_timestamp=packet.app_file_start_timestamp_machine(),
-                packet_end_timestamp=packet.end_timestamp_us_utc(),
-                server_acquisition_timestamp=packet.server_timestamp_epoch_microseconds_utc(),
+                )
             )
             if not best_offset or not best_latency:
-                best_offset = tsd.best_offset
-                best_latency = tsd.best_latency
+                best_offset = tsd.best_offset()
+                best_latency = tsd.best_latency()
             best_latency_timestamp = tsd.get_best_latency_timestamp()
         else:
             best_latency_timestamp = np.nan
 
         # noinspection Mypy
         return StationStat(
             packet.redvox_id(),
@@ -279,24 +275,20 @@
                     else None
                 )
                 gps_timestamps.append(GpsDateTime(us2dt(ts), gps_ts))
 
         best_offset = timing_info.get_best_offset()
         best_latency = timing_info.get_best_latency()
         if len(timing_info.get_synch_exchange_array()) > 0:
-            tsd = TimeSyncData(
-                station_info.get_id(),
-                time_sync_exchanges_list=timing_info.get_synch_exchange_array(),
-                packet_start_timestamp=timing_info.get_packet_start_mach_timestamp(),
-                packet_end_timestamp=timing_info.get_packet_end_mach_timestamp(),
-                server_acquisition_timestamp=timing_info.get_server_acquisition_arrival_timestamp(),
+            tsd = TimeSync(
+                time_sync_exchanges_list=timing_info.get_synch_exchange_array()
             )
             if not best_offset or not best_latency:
-                best_offset = tsd.best_offset
-                best_latency = tsd.best_latency
+                best_offset = tsd.best_offset()
+                best_latency = tsd.best_latency()
             best_latency_timestamp = tsd.get_best_latency_timestamp()
         else:
             best_latency_timestamp = np.nan
 
         return StationStat(
             station_info.get_id(),
             station_info.get_uuid(),
```

### Comparing `redvox-3.4.1/redvox/common/gap_and_pad_utils.py` & `redvox-3.4.2/redvox/common/gap_and_pad_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 from typing import List, Tuple, Optional, Dict
 import enum
 from math import modf
 from dataclasses import dataclass, field
 
 from dataclasses_json import dataclass_json
 import numpy as np
@@ -12,16 +13,14 @@
 from redvox.common.errors import RedVoxExceptions
 from redvox.api1000.wrapped_redvox_packet.sensors.audio import AudioCodec
 from redvox.api1000.wrapped_redvox_packet.sensors.location import LocationProvider
 from redvox.api1000.wrapped_redvox_packet.sensors.image import ImageCodec
 from redvox.api1000.wrapped_redvox_packet.station_information import \
     NetworkType, PowerState, CellServiceState, WifiWakeLock, ScreenState
 
-# default maximum number of points required to brute force calculating gap timestamps
-DEFAULT_MAX_BRUTE_FORCE_GAP_TIMESTAMPS: int = 5000
 # percent of packet duration/sample rate required for gap to be considered a whole unit
 DEFAULT_GAP_UPPER_LIMIT: float = 0.8
 # percent of packet duration/sample rate required for gap to be considered nothing
 DEFAULT_GAP_LOWER_LIMIT: float = 0.02
 # columns for audio table
 AUDIO_DF_COLUMNS = ["timestamps", "unaltered_timestamps", "microphone"]
 # columns that cannot be interpolated
@@ -44,32 +43,14 @@
     @staticmethod
     def list_names() -> List[str]:
         return [n.name for n in DataPointCreationMode]
 
 
 @dataclass_json
 @dataclass
-class GapPadResult:
-    """
-    The result of filling gaps or padding a time series
-    """
-    result: Optional[pa.Table] = None
-    gaps: List[Tuple[float, float]] = field(default_factory=lambda: [])
-    errors: RedVoxExceptions = field(default_factory=lambda: RedVoxExceptions("GapPadResult"))
-
-    def add_error(self, error: str):
-        """
-        add an error to the result
-        :param error: error message to add
-        """
-        self.errors.append(error)
-
-
-@dataclass_json
-@dataclass
 class AudioWithGaps:
     """
     Represents methods of reconstructing audio data with or without gaps in it
 
     Properties:
         sample_interval_micros: microseconds between sample points
 
@@ -91,15 +72,16 @@
         result_array = [[], [], []]
         for m in self.metadata:
             timestamps = calc_evenly_sampled_timestamps(m[0], m[1].num_rows, self.sample_interval_micros)
             result_array[0].extend(timestamps)
             result_array[1].extend(timestamps)
             result_array[2].extend(m[1]["microphone"].to_numpy())
         for gs, ge in self.gaps:
-            num_samples = int((ge - gs) / self.sample_interval_micros) - 1
+            fractional, whole = modf((ge - gs) / self.sample_interval_micros)
+            num_samples = int((whole - 1) if fractional < DEFAULT_GAP_LOWER_LIMIT else whole)
             timestamps = calc_evenly_sampled_timestamps(gs + self.sample_interval_micros, num_samples,
                                                         self.sample_interval_micros)
             gap_array = [timestamps, np.full(len(timestamps), np.nan)]
             result_array[0].extend(gap_array[0])
             result_array[1].extend(gap_array[0])
             result_array[2].extend(gap_array[1])
         ptable = pa.Table.from_pydict(dict(zip(AUDIO_DF_COLUMNS, result_array)))
@@ -161,36 +143,39 @@
     return return_gaps
 
 
 def fill_gaps(
         arrow_df: pa.Table,
         gaps: List[Tuple[float, float]],
         sample_interval_micros: float,
-        copy: bool = False
+        fill_mode: str = "nan"
 ) -> Tuple[pa.Table, List[Tuple[float, float]]]:
     """
     fills gaps in the table with np.nan or interpolated values by interpolating timestamps based on the
     calculated sample interval
 
     :param arrow_df: pyarrow table with data.  first column is "timestamps"
     :param gaps: list of tuples of known non-inclusive start and end timestamps of the gaps
     :param sample_interval_micros: known sample interval of the data points
-    :param copy: if True, copy the data points, otherwise interpolate from edges, default False
+    :param fill_mode: must be one of: "nan", "interpolate", or "copy".  Other inputs result in "nan".  Default "nan".
+                        Will convert input to lowercase.
     :return: table without gaps and the list of gaps
     """
     # extract the necessary information to compute gap size and gap timestamps
     data_time_stamps = arrow_df["timestamps"].to_numpy()
     if len(data_time_stamps) > 1:
         data_duration = data_time_stamps[-1] - data_time_stamps[0]
         expected_samples = (np.floor(data_duration / sample_interval_micros)
                             + (1 if data_duration % sample_interval_micros >=
                                sample_interval_micros * DEFAULT_GAP_UPPER_LIMIT else 0)) + 1
         if expected_samples > len(data_time_stamps):
-            if copy:
+            if fill_mode.lower() == "copy":
                 pcm = DataPointCreationMode["COPY"]
+            elif fill_mode.lower() == "interpolate":
+                pcm = DataPointCreationMode["INTERPOLATE"]
             else:
                 pcm = DataPointCreationMode["NAN"]
             # make it safe to alter the gap values
             my_gaps = check_gap_list(gaps, data_time_stamps[0], data_time_stamps[-1])
             for gap in my_gaps:
                 # if timestamps are around gaps, we have to update the values
                 before_start = np.argwhere([t <= gap[0] for t in data_time_stamps])
@@ -216,121 +201,49 @@
                     arrow_df = add_data_points_to_df(arrow_df, after_end, -sample_interval_micros,
                                                      num_new_points, pcm)
         indic = pc.sort_indices(arrow_df, sort_keys=[("timestamps", "ascending")])
         return arrow_df.take(indic), gaps
     return arrow_df, gaps
 
 
-def fill_audio_gaps2(
+def fill_audio_gaps(
         packet_data: List[Tuple[float, pa.Table]],
         sample_interval_micros: float,
-        gap_upper_limit: float = DEFAULT_GAP_UPPER_LIMIT,
         gap_lower_limit: float = DEFAULT_GAP_LOWER_LIMIT
 ) -> AudioWithGaps:
     """
     fills gaps in the table with np.nan by interpolating timestamps based on the expected sample interval
       * ignores gaps with duration less than or equal to packet length * gap_lower_limit
-      * converts gaps with duration greater than or equal to packet length * gap_upper_limit into a multiple of
-        packet length
 
     :param packet_data: list of tuples, each tuple containing two pieces of packet information:
                         packet_start_timestamps; float of packet start timestamp in microseconds
                         and audio_data; pa.Table of data points
     :param sample_interval_micros: sample interval in microseconds
-    :param gap_upper_limit: percentage of packet length required to confirm gap is at least 1 packet,
-                            default DEFAULT_GAP_UPPER_LIMIT
     :param gap_lower_limit: percentage of packet length required to disregard gap, default DEFAULT_GAP_LOWER_LIMIT
-    :return: list of timestamps of the non-inclusive start and end of the gaps
+    :return: AudioWithGaps object that contains a list of timestamps of the non-inclusive start and end of the gaps
+                and other information to recreate the audio record
     """
     last_data_timestamp = packet_data[0][0]
     gaps = []
     result = AudioWithGaps(sample_interval_micros, packet_data)
     for packet in packet_data:
         samples_in_packet = packet[1].num_rows
         start_ts = packet[0]
         packet_length = sample_interval_micros * samples_in_packet
         # check if start_ts is close to the last timestamp in data_timestamps
         last_timestamp_diff = start_ts - last_data_timestamp
         if last_timestamp_diff > gap_lower_limit * packet_length:
-            fractional_packet, num_packets = modf(last_timestamp_diff /
-                                                  (samples_in_packet * sample_interval_micros))
-            if fractional_packet >= gap_upper_limit and num_packets < 1:
-                num_samples = samples_in_packet * (num_packets + 1)
-            else:
-                num_samples = np.max([np.floor((fractional_packet + num_packets) * samples_in_packet), 1])
-            gap_start = last_data_timestamp
-            last_data_timestamp += (num_samples + 1) * sample_interval_micros
+            gap_start = last_data_timestamp - sample_interval_micros
+            last_data_timestamp = start_ts
             gaps.append((gap_start, last_data_timestamp))
         elif last_timestamp_diff < -gap_lower_limit * packet_length:
             result.add_error(f"Packet start timestamp: {dtu.microseconds_to_seconds(start_ts)} "
                              f"is before last timestamp of previous "
-                             f"packet: {dtu.microseconds_to_seconds(last_data_timestamp)}")
-        last_data_timestamp += (samples_in_packet + 1) * sample_interval_micros
-    result.gaps = gaps
-    return result
-
-
-def fill_audio_gaps(
-        packet_data: List[Tuple[float, pa.Table]],
-        sample_interval_micros: float,
-        gap_upper_limit: float = DEFAULT_GAP_UPPER_LIMIT,
-        gap_lower_limit: float = DEFAULT_GAP_LOWER_LIMIT
-) -> GapPadResult:
-    """
-    fills gaps in the table with np.nan by interpolating timestamps based on the expected sample interval
-      * ignores gaps with duration less than or equal to packet length * gap_lower_limit
-      * converts gaps with duration greater than or equal to packet length * gap_upper_limit into a multiple of
-        packet length
-
-    :param packet_data: list of tuples, each tuple containing two pieces of packet information:
-                        packet_start_timestamps; float of packet start timestamp in microseconds
-                        and audio_data; pa.Table of data points
-    :param sample_interval_micros: sample interval in microseconds
-    :param gap_upper_limit: percentage of packet length required to confirm gap is at least 1 packet,
-                            default DEFAULT_GAP_UPPER_LIMIT
-    :param gap_lower_limit: percentage of packet length required to disregard gap, default DEFAULT_GAP_LOWER_LIMIT
-    :return: table without gaps and the list of timestamps of the non-inclusive start and end of the gaps
-    """
-    result_array = [[], [], []]
-    last_data_timestamp: Optional[float] = None
-    gaps = []
-    result = GapPadResult()
-    for packet in packet_data:
-        samples_in_packet = packet[1].num_rows
-        start_ts = packet[0]
-        packet_length = sample_interval_micros * samples_in_packet
-        if last_data_timestamp:
-            last_data_timestamp += sample_interval_micros
-            # check if start_ts is close to the last timestamp in data_timestamps
-            last_timestamp_diff = start_ts - last_data_timestamp
-            if last_timestamp_diff > gap_lower_limit * packet_length:
-                fractional_packet, num_packets = modf(last_timestamp_diff /
-                                                      (samples_in_packet * sample_interval_micros))
-                if fractional_packet >= gap_upper_limit:
-                    num_samples = samples_in_packet * (num_packets + 1)
-                else:
-                    num_samples = np.max([np.floor((fractional_packet + num_packets) * samples_in_packet), 1])
-                gap_ts = calc_evenly_sampled_timestamps(last_data_timestamp, num_samples, sample_interval_micros)
-                gap_array = [gap_ts, np.full(len(gap_ts), np.nan)]
-                start_ts = gap_ts[-1] + sample_interval_micros
-                gaps.append((last_data_timestamp, start_ts))
-                result_array[0].extend(gap_array[0])
-                result_array[1].extend(gap_array[0])
-                result_array[2].extend(gap_array[1])
-            elif last_timestamp_diff < -gap_lower_limit * packet_length:
-                result.add_error(f"Packet start timestamp: {dtu.microseconds_to_seconds(start_ts)} "
-                                 f"is before last timestamp of previous "
-                                 f"packet: {dtu.microseconds_to_seconds(last_data_timestamp)}")
-                # return result
-        estimated_ts = calc_evenly_sampled_timestamps(start_ts, samples_in_packet, sample_interval_micros)
-        last_data_timestamp = estimated_ts[-1]
-        result_array[0].extend(estimated_ts)
-        result_array[1].extend(estimated_ts)
-        result_array[2].extend(packet[1]["microphone"].to_numpy())
-    result.result = pa.Table.from_pydict(dict(zip(AUDIO_DF_COLUMNS, result_array)))
+                             f"packet: {dtu.microseconds_to_seconds(last_data_timestamp - sample_interval_micros)}")
+        last_data_timestamp += samples_in_packet * sample_interval_micros
     result.gaps = gaps
     return result
 
 
 def add_data_points_to_df(data_table: pa.Table,
                           start_index: int,
                           sample_interval_micros: float,
@@ -386,18 +299,20 @@
                 non_numeric_diff = non_numeric_start
             else:
                 non_numeric_diff = non_numeric_end
             numeric_diff = numeric_end - numeric_start
             numeric_diff = \
                 (numeric_diff / numeric_diff["timestamps"]) * \
                 (new_timestamps - numeric_start) + numeric_start
-            # merge dicts (python 3.5 to 3.8)
-            empty_df = pa.Table.from_pydict({**numeric_diff, **non_numeric_diff})
-            # merge dicts (python 3.9):
-            # empty_df = pa.Table.from_pydict(numeric_diff | non_numeric_diff)
+            if sys.version_info[0] > 3 or (sys.version_info[0] == 3 and sys.version_info[1] >= 9):
+                # merge dicts (python 3.9):
+                empty_df = pa.Table.from_pydict(numeric_diff | non_numeric_diff)
+            else:
+                # merge dicts (python 3.5 to 3.8)
+                empty_df = pa.Table.from_pydict({**numeric_diff, **non_numeric_diff})
         else:
             # add nans and defaults
             empty_dict: Dict[str, List] = {}
             for k in data_table.schema.names:
                 empty_dict[k] = []
             for column_index in data_table.schema.names:
                 if column_index == "timestamps":
```

### Comparing `redvox-3.4.1/redvox/common/gui/cloud_data_retrieval.py` & `redvox-3.4.2/redvox/common/gui/cloud_data_retrieval.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/common/io.py` & `redvox-3.4.2/redvox/common/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,17 +262,16 @@
         """
         :return: full path to json file
         """
         return Path(self.save_dir()).joinpath(self.json_file_name())
 
     def create_dir(self):
         """
-        if saving to disk, remove the directory if it exists,
-        then create an empty directory to save things into
-        if saving to temp dir, remove any files in the temp dir
+        if saving to disk, remove the directory if it exists, then create an empty directory to save things into
+        if saving to temp dir, remove any files in the temp dir before saving to dir
         """
         if self.is_use_disk():
             if os.path.exists(self.save_dir()):
                 remove_dir_contents(Path(self.save_dir()))
             else:
                 os.makedirs(self.save_dir())
         elif self.is_use_temp():
```

### Comparing `redvox-3.4.1/redvox/common/offset_model.py` & `redvox-3.4.2/redvox/common/offset_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -333,14 +333,26 @@
         :param use_model_function: if True, use the slope of the model if it's not 0.  default True
         :return: updated list of timestamps
         """
         if use_model_function and self.slope != 0.0:
             return [self.update_time(t) for t in timestamps]
         return [t + self.intercept for t in timestamps]
 
+    def get_original_time(self, time: float, use_model_function: bool = True) -> float:
+        """
+        reverse the updated time to the unaltered value
+
+        :param time: time to update
+        :param use_model_function: if True, use the slope of the model, otherwise use the intercept.  default True
+        :return: unaltered, original time
+        """
+        if use_model_function:
+            return (self.slope * self.start_time + time - self.intercept) / (1 + self.slope)
+        return time - self.intercept
+
 
 # Method to get number of bins
 def get_bins_per_5min(start_time: float, end_time: float) -> int:
     """
     Calculates number of bins needed for roughly 5 minute bins.
         k_bins = int((end_time - start_time) / (300 * 1e6) + 1)
     :param start_time: the time used to compute the intercept (offset) and time bins; use start time of first packet
```

### Comparing `redvox-3.4.1/redvox/common/packet_to_pyarrow.py` & `redvox-3.4.2/redvox/common/packet_to_pyarrow.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,17 +199,17 @@
         pckt_info = []
         audio_lst = self.get_audio()
         frst_audio = audio_lst[0]
         use_mem = frst_audio.check_data()
         for adl in audio_lst:
             pckt_info.append((int(adl.start), adl.data()))
 
-        audio_data = gpu.fill_audio_gaps2(pckt_info,
-                                          dtu.seconds_to_microseconds(1 / frst_audio.srate_hz)
-                                          )
+        audio_data = gpu.fill_audio_gaps(pckt_info,
+                                         dtu.seconds_to_microseconds(1 / frst_audio.srate_hz)
+                                         )
         tbl = audio_data.create_timestamps()
         frst_audio = PyarrowSummary(frst_audio.name, frst_audio.stype, frst_audio.start, frst_audio.srate_hz,
                                     frst_audio.fdir, tbl.num_rows, frst_audio.smint_s, frst_audio.sstd_s,
                                     tbl)
         if not use_mem:
             frst_audio.write_data(True)
```

### Comparing `redvox-3.4.1/redvox/common/parallel_utils.py` & `redvox-3.4.2/redvox/common/parallel_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/common/run_me.py` & `redvox-3.4.2/redvox/common/run_me.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/common/sensor_data.py` & `redvox-3.4.2/redvox/common/sensor_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
             return SensorType.VELOCITY
         else:
             return SensorType.UNKNOWN_SENSOR
 
 
 class SensorData:
     """
-    Generic RedvoxSensor class for API-independent analysis
+    Generic Redvox Sensor class for API-independent analysis
 
     Properties:
         name: string, name of sensor.  REQUIRED
 
     Protected:
         _type: SensorType, enumerated type of sensor, default UNKNOWN_SENSOR
 
@@ -300,15 +300,15 @@
                                         original values, default False
         :param calculate_stats: if True, calculate sample_rate, sample_interval_s, and sample_interval_std_s
                                 default False
         :param use_offset_model_for_correction: if True, use an offset model to correct timestamps, otherwise
                                                 use the best known offset.  default False
         :param save_data: if True, save the data of the sensor to disk, otherwise use a temporary dir.  default False
         :param use_temp_dir: if True, save the data using a temporary directory.  default False
-        :return: RedvoxSensor object
+        :return: SensorData object
         """
         result = SensorData(sensor_name,
                             ds.dataset(data_path, format="parquet", exclude_invalid_files=True).to_table(),
                             sensor_type, sample_rate_hz, sample_interval_s, sample_interval_std_s,
                             is_sample_rate_fixed, are_timestamps_altered, calculate_stats,
                             use_offset_model_for_correction, save_data, data_path, use_temp_dir=use_temp_dir)
         return result
@@ -346,38 +346,38 @@
                                 default False
         :param use_offset_model_for_correction: if True, use an offset model to correct timestamps, otherwise
                                                 use the best known offset.  default False
         :param save_data: if True, save the data of the sensor to disk, otherwise use a temporary dir.  default False
         :param arrow_dir: directory to save pyarrow table, default "" (current dir).  default temporary dir if not
                             saving data
         :param use_temp_dir: If True, use a temporary directory to save the data.  default False
-        :return: RedvoxSensor object
+        :return: SensorData object
         """
         return SensorData(sensor_name, pa.Table.from_pydict(sensor_data), sensor_type, sample_rate_hz,
                           sample_interval_s, sample_interval_std_s, is_sample_rate_fixed, are_timestamps_altered,
                           calculate_stats, use_offset_model_for_correction, save_data, arrow_dir,
                           use_temp_dir=use_temp_dir)
 
     def save(self, file_name: Optional[str] = None) -> Optional[Path]:
         """
-        Saves the RedvoxSensor to disk.  Does nothing if saving is not enabled
+        Saves the sensor to disk.  Does nothing if saving is not enabled
 
-        :param file_name: Optional file name to save RedvoxSensor as.  Do not include a file extension.  Default None
+        :param file_name: Optional file name to save as.  Do not include a file extension.  Default None
                             If None, a default file name is created using this format:
                             [sensor_type]_[first_timestamp].json
         :return: The path to the saved file or None if unable to save.
         """
         if self._fs_writer.is_save_disk():
             return self.to_json_file(file_name)
         return None
 
     def load(self, in_dir: str) -> "SensorData":
         """
         :param in_dir: structured directory with json metadata file to load
-        :return: RedvoxSensor using data from files
+        :return: SensorData using data from files
         """
         file = io.get_json_file(in_dir)
         if file is None:
             st = SensorData("LoadError")
             st.append_error("File to load Sensor not found.")
             return self
         else:
@@ -482,15 +482,15 @@
     def write_pyarrow_table(self, table: pa.Table, update_file_name: Optional[bool] = True):
         """
         saves the pyarrow table to disk or to memory.
 
         * if there is no data or there is no column named timestamps in the table, an error will be created
         * if writing to disk, uses a default filename: {sensor_type}_{first_timestamp}.parquet
         * uses the directory defined by self.save_dir().  Creates the directory if it doesn't exist and removes any
-        existing parquet files from the directory if it exists
+          existing parquet files from the directory if it exists
 
         :param table: the table to write
         :param update_file_name: if True, updates the file name to match the new data.  Default True
         """
         if table.num_rows < 1 or "timestamps" not in table.schema.names:
             self._errors.append("Attempted to write invalid table.")
         elif self._fs_writer.is_save_disk():
@@ -603,15 +603,15 @@
         data = pc.take(ptable, pc.sort_indices(ptable, sort_keys=[("timestamps", order)]))
         self.write_pyarrow_table(data)
 
     def organize_and_update_stats(self, ptable: pa.Table) -> "SensorData":
         """
         sorts the data by timestamps, then if the sample rate is not fixed, recalculates the sample rate, interval,
             and interval std dev.  If there is only one value, sets the sample rate, interval, and interval std dev
-            to np.nan.  Updates the RedvoxSensor object with the new values
+            to np.nan.  Updates self with the new values
 
         :param ptable: pyarrow table to update
         :return: updated version of self
         """
         self.sort_by_data_timestamps(ptable)
         if not self._is_sample_rate_fixed:
             if self.num_samples() > 1:
@@ -632,39 +632,39 @@
                 self._sample_interval_std_s = np.nan
                 self._sample_rate_hz = np.nan
         return self
 
     def append_sensor(self, new_sensor: "SensorData", recalculate_stats: bool = False) -> "SensorData":
         """
         append the new data to the sensor, update the sensor's stats on demand if it doesn't have a fixed
-            sample rate, then return the updated RedvoxSensor object
+            sample rate, then return the updated object
 
         :param new_sensor: sensor containing data to add to the calling sensor
         :param recalculate_stats: if True and the sensor does not have a fixed sample rate, sort the timestamps,
                                     recalculate the sample rate, interval, and interval std dev, default False
-        :return: the updated RedvoxSensor object
+        :return: the updated object
         """
         _arrow: pa.Table = pa.concat_tables([self.pyarrow_table(), new_sensor.pyarrow_table()])
         if recalculate_stats and not self._is_sample_rate_fixed:
             self.organize_and_update_stats(_arrow)
         else:
             self.write_pyarrow_table(_arrow)
         return self
 
     def append_data(
             self, new_data: List[np.array], recalculate_stats: bool = False
     ) -> "SensorData":
         """
         append the new data to the dataframe, update the sensor's stats on demand if it doesn't have a fixed
-            sample rate, then return the updated RedvoxSensor object
+            sample rate, then return the updated object
 
         :param new_data: list of arrays containing data to add to the sensor's dataframe
         :param recalculate_stats: if True and the sensor does not have a fixed sample rate, sort the timestamps,
                                     recalculate the sample rate, interval, and interval std dev, default False
-        :return: the updated RedvoxSensor object
+        :return: the updated object
         """
         _arrow = pa.concat_tables([self.pyarrow_table(),
                                    pa.Table.from_arrays(arrays=[pa.array(s) for s in new_data],
                                                         names=self.data_channels())])
         if recalculate_stats and not self._is_sample_rate_fixed:
             self.organize_and_update_stats(_arrow)
         else:
@@ -807,37 +807,45 @@
         """
         slope = dtu.seconds_to_microseconds(self._sample_interval_s) * (1 + offset_model.slope) \
             if self._use_offset_model else dtu.seconds_to_microseconds(self._sample_interval_s)
         if self._type == SensorType.AUDIO:
             # use the model to update the first timestamp or add the best offset (model's intercept value)
             timestamps = pa.array(
                 calc_evenly_sampled_timestamps(
-                    offset_model.update_time(self.first_data_timestamp(), self._use_offset_model),
+                    offset_model.update_time(self.unaltered_data_timestamps()[0], self._use_offset_model),
                     self.num_samples(),
                     slope))
         else:
-            timestamps = pa.array(offset_model.update_timestamps(self.data_timestamps(),
+            timestamps = pa.array(offset_model.update_timestamps(self.unaltered_data_timestamps(),
                                                                  self._use_offset_model))
         # old_name = self.full_path()
         self.write_pyarrow_table(self.pyarrow_table().set_column(0, "timestamps", timestamps))
         # self.set_file_name()
         # os.rename(old_name, self.full_path())
         time_diffs = np.floor(np.diff(self.data_timestamps()))
         if len(time_diffs) > 1:
             self._sample_interval_s = dtu.microseconds_to_seconds(slope)
             if self._sample_interval_s > 0:
                 self._sample_rate_hz = 1 / self._sample_interval_s
                 self._sample_interval_std_s = dtu.microseconds_to_seconds(float(np.std(time_diffs)))
         self._timestamps_altered = True
 
+    def set_original_timestamps(self):
+        """
+        converts all timestamps in the sensor to the original values from the data
+        """
+        timestamps = self.unaltered_data_timestamps()
+        self.write_pyarrow_table(self.pyarrow_table().set_column(0, "timestamps", timestamps))
+        self._timestamps_altered = False
+
     def interpolate(self, interpolate_timestamp: float, first_point: int, second_point: int = 0,
                     copy: bool = True) -> pa.Table:
         """
-        interpolates two points at the intercept value.  the two points must be consecutive in the data.
-        data channels that can't be interpolated are set to np.nan.
+        interpolates two points at the chosen timestamp.  If copy is true, copies the values of the closest point,
+        otherwise interpolates any numerical value.  Non-numeric values are set to a copy of the closest point.
 
         :param interpolate_timestamp: timestamp to interpolate other values
         :param first_point: index of first point
         :param second_point: delta to second point, default 0 (same as first point)
         :param copy: if True, copies the values of the first point, otherwise uses the interpolated value.
                         Default True
         :return: pyarrow Table of interpolated points
@@ -907,15 +915,15 @@
     @staticmethod
     def from_json_file(file_dir: str, file_name: Optional[str] = None) -> "SensorData":
         """
         convert contents of json file to Sensor
 
         :param file_dir: full path to containing directory for the file
         :param file_name: optional name of file and extension to load data from; if not specified, finds the first one
-        :return: RedvoxSensor object
+        :return: SensorData object
         """
         if file_name is None:
             file_name = io.get_json_file(file_dir)
             if file_name is None:
                 result = SensorData("Empty")
                 result.append_error("JSON file to load Sensor from not found.")
                 return result
@@ -1042,15 +1050,15 @@
                                 default False
         :param use_offset_model_for_correction: if True, use an offset model to correct timestamps, otherwise
                                                 use the best known offset.  default False
         :param save_data: if True, save the data of the sensor to disk, otherwise use a temporary dir.  default False
         :param base_dir: directory to save pyarrow table, default "." (current dir).  internally uses a temporary
                             dir if not saving data
         :param use_temp_dir: if True, save the data using a temporary directory.  default False
-        :return: RedvoxSensor object
+        :return: SensorData object
         """
         return SensorData(sensor_name, data.create_timestamps(),
                           SensorType.AUDIO, sample_rate_hz, sample_interval_s, sample_interval_std_s,
                           is_sample_rate_fixed, are_timestamps_altered, calculate_stats,
                           use_offset_model_for_correction, save_data, base_dir, use_temp_dir=use_temp_dir)
 
     def get_microphone_data(self) -> np.array:
```

### Comparing `redvox-3.4.1/redvox/common/sensor_io.py` & `redvox-3.4.2/redvox/common/sensor_io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/common/sensor_reader_utils.py` & `redvox-3.4.2/redvox/common/sensor_reader_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/common/session_io.py` & `redvox-3.4.2/redvox/common/session_io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/common/session_model.py` & `redvox-3.4.2/redvox/common/session_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,17 +145,18 @@
         if _has_sensor(packet, s):
             result.append(s)
     return result
 
 
 class SessionModel:
     """
-    SessionModel is designed to summarize an operational period of a station.  SessionModel can be sealed, which means
-    no more data will be received for the model, and the properties of the SessionModel are valid and the best
-    available.  WARNING: Only seal a SessionModel when you are certain the session being modeled is finished.
+    SessionModel is designed to summarize an operational period of a station.  Summaries do not include data from
+    sensors, and only if necessary is limited amounts of data stored within the model.  SessionModel can be sealed,
+    which means no more data will be received for the model, and the properties of the SessionModel are valid and the
+    best available.  WARNING: Only seal a SessionModel when you are certain the session being modeled is finished.
 
     Timestamps are in microseconds since epoch UTC
 
     Latitude and Longitude are in degrees
 
     Altitude is in meters
 
@@ -169,14 +170,24 @@
     presented by this class
 
     Protected:
         _session_version: str, the version of the SessionModel.
 
         _sensors: Dict[str, float], The name of sensors and their mean sample rate as a dictionary.
 
+        _first_timesync_data: CircularQueue, container for the first 15 points of timesync data;
+        timestamp, latency, offset.  Default empty
+
+        _last_timesync_data: CircularQueue, container for the last 15 points of timesync data.  Default empty
+
+        _first_gps_data: CircularQueue, container for the first 15 points of GPS offset data; timestamp and offset.
+        Default empty
+
+        _last_gps_data: CircularQueue, container for the last 15 points of GPS offset data.  Default empty
+
         _errors: RedVoxExceptions, Contains any errors found when creating the model.
 
         _sdk_version: str, the version of the SDK used to create the model.
 
     Properties:
         id: str, id of the station.  Default ""
 
@@ -215,29 +226,21 @@
 
         num_timesync_points: int, the number of timesync data points.  Default 0
 
         mean_latency: float, mean latency of the model.  Default np.nan
 
         mean_offset: float, mean offset of the model.  Default np.nan
 
-        _first_timesync_data: CircularQueue, container for the first 15 points of timesync data;
-        timestamp, latency, offset.  Default empty
-
-        _last_timesync_data: CircularQueue, container for the last 15 points of timesync data.  Default empty
+        offset_model: OffsetModel with which the user can calculate corrected timestamps.  Default empty OffsetModel
 
         num_gps_points: int, the number of gps data points.  Default 0
 
         gps_offset: optional tuple of float, the slope and intercept (in that order) of the gps timing calculations.
         Default None
 
-        _first_gps_data: CircularQueue, container for the first 15 points of GPS offset data; timestamp and offset.
-        Default empty
-
-        _last_gps_data: CircularQueue, container for the last 15 points of GPS offset data.  Default empty
-
         is_sealed: bool, if True, the SessionModel will not accept any more data.  This means the offset model and gps
         offset values are the best they can be, given the available data.  Default False
     """
     def __init__(self,
                  station_id: str = "",
                  uuid: str = "",
                  start_timestamp: float = np.nan,
@@ -246,15 +249,15 @@
                  make: str = "",
                  model: str = "",
                  station_description: str = "",
                  app_name: str = "Redvox",
                  sensors: Optional[Dict] = None
                  ):
         """
-        Initialize a SessionModel with non-sensor related metadata.  This function uses only the most basic information
+        Initialize a SessionModel with general status metadata.  This function uses only the most basic information
         to create the SessionModel; use these other functions if you already have some form of data to read:
 
         Use function create_from_packet() instead of this if you already have a packet to read from.
 
         Use function create_from_stream() instead of this if you already have several packets to read from.
 
         Use function load() instead of this if you already have a session_model.json to read from.
@@ -424,15 +427,15 @@
             result["last_timesync_data"] = self._last_timesync_data.as_dict()
             result["first_gps_data"] = self._first_gps_data.as_dict()
             result["last_gps_data"] = self._last_gps_data.as_dict()
         return result
 
     def default_json_file_name(self) -> str:
         """
-        :return: Default filename as [id]_[startdate], with startdate as integer of microseconds
+        :return: Default filename as [id]_[start_date], with start_date as integer of microseconds
                     since epoch UTC.  File extension NOT included.
         """
         return f"{self.id}_{0 if np.isnan(self.start_date) else int(self.start_date)}"
 
     @staticmethod
     def from_json_dict(json_dict: dict) -> "SessionModel":
         """
@@ -658,14 +661,15 @@
             self.mean_latency = \
                 (self.mean_latency * self.num_packets + packet_best_latency) / (self.num_packets + 1)
             self.mean_offset = \
                 (self.mean_offset * self.num_packets + packet_best_offset) / (self.num_packets + 1)
             _ts_offsets = ts.offsets().flatten()
             _ts_timestamps = ts.get_device_exchanges_timestamps()
             _ts_latencies = ts.latencies().flatten()
+            # add data to the appropriate circular queue
             if self._first_timesync_data.is_full():
                 for i in range(len(_ts_timestamps)):
                     self._last_timesync_data.add((_ts_timestamps[i], _ts_latencies[i], _ts_offsets[i]))
             else:
                 for i in range(len(_ts_timestamps)):
                     self._first_timesync_data.add((_ts_timestamps[i], _ts_latencies[i], _ts_offsets[i]), True)
```

### Comparing `redvox-3.4.1/redvox/common/session_model_utils.py` & `redvox-3.4.2/redvox/common/session_model_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/common/station.py` & `redvox-3.4.2/redvox/common/station.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Defines generic station objects for API-independent analysis
 all timestamps are integers in microseconds unless otherwise stated
-Utilizes WrappedRedvoxPacketM (API M data packets) as the format of the data due to their versatility
+Utilizes RedvoxPacketM (API M data packets) as the format of the data due to their versatility
 """
 from typing import List, Optional, Tuple
 import os
 from pathlib import Path
 
 import numpy as np
 import pyarrow.dataset as ds
@@ -21,23 +21,27 @@
 from redvox.common import packet_to_pyarrow as ptp
 from redvox.common import gap_and_pad_utils as gpu
 from redvox.common.date_time_utils import datetime_from_epoch_microseconds_utc,\
     seconds_to_microseconds as s_to_us
 from redvox.common.event_stream import EventStreams
 
 
+STATION_ID_LENGTH = 10  # the length of a station ID string
+
+
 class Station:
     """
     generic station for api-independent stuff; uses API M as the core data object since its quite versatile
     In order for a list of data to be a station, all of the data packets must:
         * Have the same station id
         * Have the same station uuid
         * Have the same start date
         * Have the same audio sample rate
         * Have the same metadata
+    Generally speaking, stations can be uniquely identified with a minimum of three values: id, uuid, and start date
     Properties:
         _data: list of sensor data associated with the station, default empty list
 
         _metadata: StationMetadata consistent across all packets, default empty StationMetadata
 
         _packet_metadata: list of StationPacketMetadata that changes from packet to packet, default empty list
 
@@ -374,15 +378,15 @@
     def _load_metadata_from_packet(self, packet: api_m.RedvoxPacketM):
         """
         sets metadata that applies to the entire station from a single packet
 
         :param packet: API-M redvox packet to load metadata from
         """
         # self.id = packet.station_information.id
-        self._id = packet.station_information.id.zfill(10)
+        self._id = packet.station_information.id.zfill(STATION_ID_LENGTH)
         self._uuid = packet.station_information.uuid
         self._start_date = packet.timing_information.app_start_mach_timestamp
         if self._start_date < 0:
             self._errors.append(
                 f"Station {self._id} has station start date before epoch.  "
                 f"Station start date reset to np.nan"
             )
@@ -563,14 +567,20 @@
         if sensor_type in self.get_station_sensor_types():
             raise ValueError(
                 f"Cannot add sensor type ({sensor_type.name}) that already exists in packet!"
             )
         else:
             self._data.append(sensor)
 
+    def get_num_packets(self) -> int:
+        """
+        :return: number of packets used to create station
+        """
+        return len(self._packet_metadata)
+
     def get_mean_packet_duration(self) -> float:
         """
         :return: mean duration of packets in microseconds
         """
         return float(
             np.mean(
                 [tsd.packet_end_mach_timestamp - tsd.packet_start_mach_timestamp for tsd in self._packet_metadata]
@@ -581,15 +591,15 @@
         """
         calculate the mean number of audio samples per packet using the
           number of audio sensor's data points and the number of packets
 
         :return: mean number of audio samples per packet
         """
         # noinspection Mypy
-        return self.audio_sensor().num_samples() / len(self._packet_metadata)
+        return self.audio_sensor().num_samples() / self.get_num_packets()
 
     def has_timesync_data(self) -> bool:
         """
         :return: True if there is timesync data for the station
         """
         return self._timesync_data.num_tri_messages() > 0
 
@@ -1348,25 +1358,25 @@
                         data_table = pa.concat_tables([data_table, sdata[i].data()])
                 data_table = self._fix_sensor_data(snr, data_table)
                 if np.isnan(sdata[0].srate_hz):
                     timestamps = data_table["timestamps"].to_numpy()
                     d, g = gpu.fill_gaps(
                         data_table,
                         self._gaps,
-                        float(np.mean(np.diff(timestamps))) if len(timestamps) > 1 else np.nan, True)
+                        float(np.mean(np.diff(timestamps))) if len(timestamps) > 1 else np.nan, "copy")
                     new_sensor = sd.SensorData(
                         sensor_name=sdata[0].name, sensor_data=d, gaps=g, save_data=self._fs_writer.is_save_disk(),
                         sensor_type=snr, calculate_stats=True, is_sample_rate_fixed=False,
                         use_offset_model_for_correction=self._use_model_correction,
                         base_dir=self.get_save_dir_sensor(sdata[0].stype))
                 else:
                     d, g = gpu.fill_gaps(
                         data_table,
                         self._gaps,
-                        s_to_us(sdata[0].smint_s), True)
+                        s_to_us(sdata[0].smint_s), "copy")
                     new_sensor = sd.SensorData(
                             sensor_name=sdata[0].name, sensor_data=d, gaps=g, save_data=self._fs_writer.is_save_disk(),
                             sensor_type=snr, sample_rate_hz=sdata[0].srate_hz, sample_interval_s=1/sdata[0].srate_hz,
                             sample_interval_std_s=0., is_sample_rate_fixed=True,
                             use_offset_model_for_correction=self._use_model_correction,
                             base_dir=self.get_save_dir_sensor(sdata[0].stype))
                 self._data.append(new_sensor.class_from_type())
@@ -1374,14 +1384,16 @@
             self._errors.append("Audio Sensor expected, but does not exist.")
 
     def _app_version_major(self) -> Tuple[int, int]:
         """
         :return: tuple of app version to 2 significant version numbers (i.e: version number x.y.z returns x and y)
         """
         nums = self.metadata().app_version.split(".")
+        if self.metadata().os == st_utils.OsType["IOS"]:
+            nums[1] = nums[1].split(" ")[0]
         return int(nums[0]), int(nums[1])
 
     def metadata(self) -> st_utils.StationMetadata:
         """
         :return: station metadata
         """
         return self._metadata
@@ -1564,14 +1576,47 @@
             self.update_first_and_last_data_timestamps()
             self._timesync_data.arrow_file = f"timesync_{0 if np.isnan(self._start_date) else int(self._start_date)}"
             self._is_timestamps_updated = True
         else:
             self._errors.append("Attempted to correct timestamps, but correction not enabled.")
         return self
 
+    def undo_update_timestamps(self) -> "Station":
+        """
+        undoes non-sensor timestamp updates of the timestamps in the station using the offset model
+        sensors already have unaltered timestamps
+        """
+        if not self._is_timestamps_updated:
+            self._errors.append("Timestamps already not corrected!")
+        else:
+            self._start_date = self._timesync_data.offset_model().get_original_time(
+                self._start_date, self._use_model_correction
+            )
+            if self._fs_writer.file_name != self._get_id_key():
+                if self._fs_writer.is_save_disk():
+                    old_name = self.save_dir()
+                    self.set_save_dir(self._fs_writer.base_dir)
+                    if old_name != "." and os.path.exists(old_name):
+                        os.rename(old_name, self.save_dir())
+                else:
+                    self._fs_writer.file_name = self._get_id_key()
+            for sensor in self._data:
+                sensor.set_original_timestamps()
+            for packet in self._packet_metadata:
+                packet.original_timestamps(self._timesync_data.offset_model(), self._use_model_correction)
+            for g in range(len(self._gaps)):
+                self._gaps[g] = (self._timesync_data.offset_model().get_original_time(self._gaps[g][0]),
+                                 self._timesync_data.offset_model().get_original_time(self._gaps[g][1]))
+            if hasattr(self, "_event_data"):
+                self._event_data.original_timestamps(self._timesync_data.offset_model(), self.use_model_correction())
+            self.update_first_and_last_data_timestamps()
+            self._timesync_data.arrow_file = f"timesync_{0 if np.isnan(self._start_date) else int(self._start_date)}"
+            self._is_timestamps_updated = True
+        return self
+
     def as_dict(self) -> dict:
         """
         :return: station as dictionary
         """
         return {
             "id": self._id,
             "uuid": self._uuid,
```

### Comparing `redvox-3.4.1/redvox/common/station_io.py` & `redvox-3.4.2/redvox/common/station_io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/common/station_model.py` & `redvox-3.4.2/redvox/common/station_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,17 +77,19 @@
         if self.id == session.id and self.uuid == session.uuid:
             self.num_sessions += 1
             if self.start_date > session.start_date:
                 self.start_date = session.start_date
             if self.end_date < session.last_data_timestamp:
                 self.end_date = session.last_data_timestamp
             first_timestamp = np.nan if np.isnan(session.first_data_timestamp) \
-                else datetime_from_epoch_microseconds_utc(session.first_data_timestamp).strftime('%Y-%m-%dT%H:%M:%S.%fZ')
+                else datetime_from_epoch_microseconds_utc(
+                session.first_data_timestamp).strftime('%Y-%m-%dT%H:%M:%S.%fZ')
             last_timestamp = np.nan if np.isnan(session.last_data_timestamp) \
-                else datetime_from_epoch_microseconds_utc(session.last_data_timestamp).strftime('%Y-%m-%dT%H:%M:%S.%fZ')
+                else datetime_from_epoch_microseconds_utc(
+                session.last_data_timestamp).strftime('%Y-%m-%dT%H:%M:%S.%fZ')
             self.changelog.append(f"session from {first_timestamp}: {last_timestamp}")
 
     @staticmethod
     def create_from_session(session: SessionModel) -> "StationModel":
         """
         Create StationModel from a single session
```

### Comparing `redvox-3.4.1/redvox/common/station_utils.py` & `redvox-3.4.2/redvox/common/station_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,29 +5,27 @@
 from dataclasses import dataclass
 from typing import Tuple, Optional, List, Dict
 
 import numpy as np
 
 from redvox.common.offset_model import OffsetModel
 from redvox.api1000.wrapped_redvox_packet.station_information import OsType
-from redvox.api1000.wrapped_redvox_packet.wrapped_packet import WrappedRedvoxPacketM
 from redvox.api1000.wrapped_redvox_packet.timing_information import TimingScoreMethod
 from redvox.common.errors import RedVoxExceptions
-# from redvox.api1000.wrapped_redvox_packet import event_streams as es
 import redvox.api1000.proto.redvox_api_m_pb2 as api_m
 
 
 def validate_station_key_list(
     data_packets: List[api_m.RedvoxPacketM], errors: RedVoxExceptions
 ) -> bool:
     """
     Checks for consistency in the data packets.  Returns False if discrepancies are found.
     If debug is True, will output the discrepancies.
 
-    :param data_packets: list of WrappedRedvoxPacketM to look at
+    :param data_packets: list of RedvoxPacketM to look at
     :param errors: RedVoxExceptions detailing errors found while validating
     :return: True if no discrepancies found.  False otherwise
     """
     my_errors = RedVoxExceptions("StationKeyValidation")
     if len(data_packets) < 2:
         return True
     j: np.ndarray = np.transpose(
@@ -153,20 +151,20 @@
         app_version: str, station app version, default empty string
         is_private: bool, is station data private, default False
         packet_duration_s: float, duration of the packet in seconds, default np.nan
         station_description: str, description of the station, default empty string
         other_metadata: dict, str: str of other metadata from the packet, default empty list
     """
 
-    def __init__(self, app: str, packet: Optional[api_m.RedvoxPacketM] = None):
+    def __init__(self, app: str = "", packet: Optional[api_m.RedvoxPacketM] = None):
         """
         initialize the metadata
 
         :param app: app name
-        :param packet: Optional WrappedRedvoxPacketM to read data from
+        :param packet: Optional RedvoxPacketM to read data from
         """
         self.app = app
         self.other_metadata = {}
         if packet:
             self.api = packet.api
             self.sub_api = packet.sub_api
             self.make = packet.station_information.make
@@ -273,86 +271,14 @@
         result.is_private = md_dict["is_private"]
         result.packet_duration_s = md_dict["packet_duration_s"]
         result.station_description = md_dict["station_description"]
         result.other_metadata = md_dict["other_metadata"]
         return result
 
 
-class StationMetadataWrapped:
-    """
-    A container for all the packet metadata consistent across all packets
-    Properties:
-        api: float, api version, default np.nan
-        sub_api: float, sub api version, default np.nan
-        make: str, station make, default empty string
-        model: str, station model, default empty string
-        os: OsType enum, station OS, default OsType.UNKNOWN_OS
-        os_version: str, station OS version, default empty string
-        app: str, station app, default empty string
-        app_version: str, station app version, default empty string
-        is_private: bool, is station data private, default False
-        packet_duration_s: float, duration of the packet in seconds, default np.nan
-        station_description: str, description of the station, default empty string
-        other_metadata: dict, str: str of other metadata from the packet, default empty list
-    """
-
-    def __init__(self, app: str, packet: Optional[WrappedRedvoxPacketM] = None):
-        """
-        initialize the metadata
-
-        :param app: app name
-        :param packet: Optional WrappedRedvoxPacketM to read data from
-        """
-        self.app = app
-        self.other_metadata = {}
-        if packet:
-            self.api = packet.get_api()
-            self.sub_api = packet.get_sub_api()
-            self.make = packet.get_station_information().get_make()
-            self.model = packet.get_station_information().get_model()
-            self.os = packet.get_station_information().get_os()
-            self.os_version = packet.get_station_information().get_os_version()
-            self.app_version = packet.get_station_information().get_app_version()
-            self.is_private = packet.get_station_information().get_is_private()
-            self.packet_duration_s = packet.get_packet_duration_s()
-            self.station_description = (
-                packet.get_station_information().get_description()
-            )
-        else:
-            self.api = np.nan
-            self.sub_api = np.nan
-            self.make = ""
-            self.model = ""
-            self.os = OsType.UNKNOWN_OS
-            self.os_version = ""
-            self.app_version = ""
-            self.is_private = False
-            self.packet_duration_s = np.nan
-            self.station_description = ""
-
-    def validate_metadata(self, other_metadata: "StationMetadataWrapped") -> bool:
-        """
-        :param other_metadata: another StationMetadata object to compare
-        :return: True if other_metadata is equal to the calling metadata
-        """
-        return (
-                self.app == other_metadata.app
-                and self.api == other_metadata.api
-                and self.sub_api == other_metadata.sub_api
-                and self.make == other_metadata.make
-                and self.model == other_metadata.model
-                and self.os == other_metadata.os
-                and self.os_version == other_metadata.os_version
-                and self.app_version == other_metadata.app_version
-                and self.is_private == other_metadata.is_private
-                and self.packet_duration_s == other_metadata.packet_duration_s
-                and self.station_description == other_metadata.station_description
-        )
-
-
 class StationPacketMetadata:
     """
     A container for all the packet metadata that isn't consistent across all packets
 
     Properties:
         packet_start_mach_timestamp: float, machine timestamp of packet start in microseconds since epoch UTC,
         default np.nan
@@ -374,15 +300,15 @@
         other_metadata: dict, str: str of other metadata from the packet, default empty list
     """
 
     def __init__(self, packet: Optional[api_m.RedvoxPacketM] = None):
         """
         initialize the metadata
 
-        :param packet: Optional WrappedRedvoxPacketM to read data from
+        :param packet: Optional RedvoxPacketM to read data from
         """
         self.other_metadata = {}
         if packet:
             self.packet_start_mach_timestamp = (
                 packet.timing_information.packet_start_mach_timestamp
             )
             self.packet_end_mach_timestamp = (
@@ -433,14 +359,27 @@
                                     otherwise use best offset (model's intercept value).  default True
         """
         self.packet_start_mach_timestamp = om.update_time(self.packet_start_mach_timestamp, use_model_function)
         self.packet_end_mach_timestamp = om.update_time(self.packet_end_mach_timestamp, use_model_function)
         self.packet_start_os_timestamp = om.update_time(self.packet_start_os_timestamp, use_model_function)
         self.packet_end_os_timestamp = om.update_time(self.packet_end_os_timestamp, use_model_function)
 
+    def original_timestamps(self, om: OffsetModel, use_model_function: bool = True):
+        """
+        undo the updates to the timestamps in the metadata using the offset model
+
+        :param om: OffsetModel to apply to data
+        :param use_model_function: if True, use the offset model's correction function to correct time,
+                                    otherwise use best offset (model's intercept value).  default True
+        """
+        self.packet_start_mach_timestamp = om.get_original_time(self.packet_start_mach_timestamp, use_model_function)
+        self.packet_end_mach_timestamp = om.get_original_time(self.packet_end_mach_timestamp, use_model_function)
+        self.packet_start_os_timestamp = om.get_original_time(self.packet_start_os_timestamp, use_model_function)
+        self.packet_end_os_timestamp = om.get_original_time(self.packet_end_os_timestamp, use_model_function)
+
     def as_dict(self) -> dict:
         """
         :return: dictionary representation of the packet metadata
         """
         return {
             "packet_start_mach_timestamp": self.packet_start_mach_timestamp,
             "packet_end_mach_timestamp": self.packet_end_mach_timestamp,
@@ -466,64 +405,7 @@
         result.packet_end_os_timestamp = pmd_dict["packet_end_os_timestamp"]
         result.server_packet_receive_timestamp = pmd_dict["server_packet_receive_timestamp"]
         result.timing_info_score = pmd_dict["timing_info_score"]
         result.timing_score_method = TimingScoreMethod[pmd_dict["timing_score_method"]
                                                        if "timing_score_method" in pmd_dict.keys()
                                                        else "UNKNOWN"]
         return result
-
-
-class StationPacketMetadataWrapped:
-    """
-    A container for all the packet metadata that isn't consistent across all packets
-    Properties:
-        packet_start_mach_timestamp: float, machine timestamp of packet start in microseconds since epoch UTC
-        packet_end_mach_timestamp: float, machine timestamp of packet end in microseconds since epoch UTC
-        packet_start_os_timestamp: float, os timestamp of packet start in microseconds since epoch UTC
-        packet_end_os_timestamp: float, os timestamp of packet end in microseconds since epoch UTC
-        timing_info_score: float, quality of timing information
-        timing_score_method: TimingScoreMethod, method used to determine timing score
-        other_metadata: dict, str: str of other metadata from the packet
-    """
-
-    def __init__(self, packet: Optional[WrappedRedvoxPacketM] = None):
-        """
-        initialize the metadata
-
-        :param packet: Optional WrappedRedvoxPacketM to read data from
-        """
-        self.other_metadata = {}
-        if packet:
-            self.packet_start_mach_timestamp = (
-                packet.get_timing_information().get_packet_start_mach_timestamp()
-            )
-            self.packet_end_mach_timestamp = (
-                packet.get_timing_information().get_packet_end_mach_timestamp()
-            )
-            self.packet_start_os_timestamp = (
-                packet.get_timing_information().get_packet_start_os_timestamp()
-            )
-            self.packet_end_os_timestamp = (
-                packet.get_timing_information().get_packet_end_os_timestamp()
-            )
-            self.timing_info_score = packet.get_timing_information().get_score()
-            self.timing_score_method = TimingScoreMethod(packet.get_timing_information().get_score_method())
-        else:
-            self.packet_start_mach_timestamp = np.nan
-            self.packet_end_mach_timestamp = np.nan
-            self.packet_start_os_timestamp = np.nan
-            self.packet_end_os_timestamp = np.nan
-            self.timing_info_score = np.nan
-            self.timing_score_method = TimingScoreMethod["UNKNOWN"]
-
-    def update_timestamps(self, om: OffsetModel, use_model_function: bool = True):
-        """
-        updates the timestamps in the metadata using the offset model
-
-        :param om: OffsetModel to apply to data
-        :param use_model_function: if True, use the offset model's correction function to correct time,
-                                    otherwise use best offset (model's intercept value).  default True
-        """
-        self.packet_start_mach_timestamp = om.update_time(self.packet_start_mach_timestamp, use_model_function)
-        self.packet_end_mach_timestamp = om.update_time(self.packet_end_mach_timestamp, use_model_function)
-        self.packet_start_os_timestamp = om.update_time(self.packet_start_os_timestamp, use_model_function)
-        self.packet_end_os_timestamp = om.update_time(self.packet_end_os_timestamp, use_model_function)
```

### Comparing `redvox-3.4.1/redvox/common/stats_helper.py` & `redvox-3.4.2/redvox/common/stats_helper.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/common/timesync.py` & `redvox-3.4.2/redvox/common/timesync.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         _offset_std: float, standard deviation of offsets, default np.nan
 
         _data_start: float, start timestamp of the data, default np.nan
 
         _data_end: float, end timestamp of the data, default np.nan
 
         _best_latency_index: int, index in latencies/sync exchanges array that contains the best latency,
-        default -1
+        default np.nan
 
         _best_msg_array_index: int, indicates which latency array has the best latency.
         Must be 1 or 3, other values are invalid.  Default 0
 
         _offset_model: OffsetModel, used to correct timestamps.
 
         _arrow_dir: str, directory to save arrow file in, default "." (current dir)
@@ -79,15 +79,15 @@
             latency_std: float = np.nan,
             offsets: Optional[np.ndarray] = None,
             best_offset: float = 0.0,
             mean_offset: float = np.nan,
             offset_std: float = np.nan,
             data_start: float = np.nan,
             data_end: float = np.nan,
-            best_latency_index: Optional[int] = None,
+            best_latency_index: int = np.nan,
             best_array_index: int = 0,
             arrow_dir: str = ".",
             arrow_file_name: str = "timesync"
     ):
         """
         Initialize properties
 
@@ -98,15 +98,15 @@
         :param latency_std: the standard deviation of all latencies, default np.nan
         :param offsets: optional arrays of offsets from exchanges; must be two equal length arrays, default None
         :param best_offset: the best offset of the packet, default 0.0
         :param mean_offset: the mean of all offsets, default np.nan
         :param offset_std: the standard deviation of all offsets, default np.nan
         :param data_start: the start timestamp of the data, default np.nan
         :param data_end: the end timestamp of the data, default np.nan
-        :param best_latency_index: optional index of best latency in latencies array, default None
+        :param best_latency_index: index of best latency in latencies array, default np.nan
         :param best_array_index: index of best latency array; must be either 1 (first array) or 3 (second array),
                                     any other value is invalid, default 0
         :param arrow_dir: directory to save timesync data in, default "."
         :param arrow_file_name: name of file to save timesync data as.  do not include extensions.  default "timesync"
         """
         self._latencies: np.ndarray = latencies
         self._best_latency: float = best_latency
@@ -128,15 +128,20 @@
             self._best_exchange_index_list = []
             self._offset_model: OffsetModel = OffsetModel.empty_model()
         else:
             self._time_sync_exchanges_list = np.transpose([
                 time_sync_exchanges_list[i: i + 6]
                 for i in range(0, len(time_sync_exchanges_list), 6)
             ])
-            self._stats_from_exchanges()
+            if self._latencies is None:
+                if not np.isnan(self._data_start):
+                    self._data_start = self.get_exchange_timestamps(4)[0]
+                if not np.isnan(self._data_end):
+                    self._data_end = self.get_exchange_timestamps(5)[-1]
+                self._stats_from_exchanges()
 
     def __repr__(self):
         return f"best_latency_index: {self._best_latency_index}, " \
                f"best_latency: {self._best_latency}, " \
                f"mean_latency: {self._mean_latency}, " \
                f"latency_std: {self._latency_std}, " \
                f"best_offset: {self._best_offset}, " \
@@ -246,60 +251,65 @@
             self._offsets = np.array(([], []))
             self._best_latency = np.nan
             self._mean_latency = np.nan
             self._latency_std = np.nan
             self._best_offset = 0
             self._mean_offset = np.nan
             self._offset_std = np.nan
-            self._best_latency_index = -1
+            self._best_latency_index = np.nan
             self._best_msg_array_index = 0
             self._offset_model = OffsetModel.empty_model()
             self._best_exchange_index_list = []
-        elif self._latencies is None:
+        else:
             # compute tri message data from time sync exchanges
             tse = tms.TriMessageStats(
                 "",
                 np.array(self._time_sync_exchanges_list[0]),
                 np.array(self._time_sync_exchanges_list[1]),
                 np.array(self._time_sync_exchanges_list[2]),
                 np.array(self._time_sync_exchanges_list[3]),
                 np.array(self._time_sync_exchanges_list[4]),
                 np.array(self._time_sync_exchanges_list[5]),
             )
             self._latencies = np.array((tse.latency1, tse.latency3))
-            if self._offsets is None:
-                self._offsets = np.array((tse.offset1, tse.offset3))
-            # Compute the statistics for latency and offset
-            if np.isnan(self._mean_latency):
-                self._mean_latency = np.mean([*self._latencies[0], *self._latencies[1]])
-            if np.isnan(self._latency_std):
-                self._latency_std = np.std([*self._latencies[0], *self._latencies[1]])
-            if np.isnan(self._mean_offset):
-                self._mean_offset = np.mean([*self._offsets[0], *self._offsets[1]])
-            if np.isnan(self._offset_std):
-                self._offset_std = np.std([*self._offsets[0], *self._offsets[1]])
-            self._best_exchange_index_list = tse.best_latency_per_exchange_index_array
-            self._best_latency_index = tse.best_latency_index
-            self._best_msg_array_index = tse.best_latency_array_index
-            # if best_latency is np.nan, set to best computed latency
-            if np.isnan(self._best_latency):
-                self._best_latency = tse.best_latency
-                self._best_offset = tse.best_offset
-            # if best_offset is still default value, use the best computed offset
-            elif self._best_offset == 0:
-                self._best_offset = tse.best_offset
+            self._offsets = np.array((tse.offset1, tse.offset3))
             if not np.isnan(self._data_start) and not np.isnan(self._data_end):
                 self._offset_model = OffsetModel(self._latencies.flatten(), self._offsets.flatten(),
                                                  self.get_device_exchanges_timestamps(),
                                                  self._data_start, self._data_end)
+                # Compute the statistics for latency using the model
+                self._mean_latency = self._offset_model.mean_latency
+                self._latency_std = self._offset_model.std_dev_latency
+            else:
+                self._offset_model = OffsetModel.empty_model()
+                # Compute the statistics for latency using the exchanges
+                self._mean_latency = np.mean([*self._latencies[0], *self._latencies[1]])
+                self._latency_std = np.std([*self._latencies[0], *self._latencies[1]])
+            # compute the rest of the statistics
+            self._mean_offset = np.mean([*self._offsets[0], *self._offsets[1]])
+            self._offset_std = np.std([*self._offsets[0], *self._offsets[1]])
+            self._best_latency_index = tse.best_latency_index
+            self._best_msg_array_index = tse.best_latency_array_index
+            self._best_latency = tse.best_latency
+            self._best_offset = tse.best_offset
+            self._best_exchange_index_list = tse.best_latency_per_exchange_index_array
+
+    def process_exchanges(self, force: bool = False):
+        """
+        Use the sync exchanges to compute the time sync stats (latencies, best latency, offsets, etc).
+
+        :param force: if True, will overwrite any existing values.
+        """
+        if self._latencies is None or force:
+            self._stats_from_exchanges()
 
     def get_exchange_timestamps(self, index: int) -> np.array:
         """
-        :param index: index of timestamps to return.  0, 1, 2 are server timestamps.  3, 4, 5 are device
-                        any value not from 0 to 5 will be converted to 0
+        :param index: index of timestamps to return.  0, 1, 2 are server timestamps.  3, 4, 5 are device.
+                        Any value not from 0 to 5 will be converted to 0
         :return: timestamps from the chosen index.
         """
         if index < 0 or index > 5:
             index = 0
         return self._time_sync_exchanges_list[index]
 
     def get_device_exchanges_timestamps(self) -> np.array:
@@ -314,20 +324,20 @@
         """
         return np.size(self._time_sync_exchanges_list, 1)
 
     def get_best_latency_timestamp(self) -> float:
         """
         :return: timestamp of best latency, or np.nan if no best latency.
         """
-        if self._best_msg_array_index == 1:
-            return self._time_sync_exchanges_list[3][self._best_latency_index]
-        elif self._best_msg_array_index == 3:
-            return self._time_sync_exchanges_list[5][self._best_latency_index]
-        else:
-            return np.nan
+        if not np.isnan(self._best_latency_index):
+            if self._best_msg_array_index == 1:
+                return self._time_sync_exchanges_list[3][self._best_latency_index]
+            elif self._best_msg_array_index == 3:
+                return self._time_sync_exchanges_list[5][self._best_latency_index]
+        return np.nan
 
     def append_timesync_arrow(self, new_data: "TimeSync"):
         """
         adds timesync data from new_data to current
 
         :param new_data: another TimeSyncArrow object
         """
@@ -347,38 +357,15 @@
             self._data_start = new_data._data_start
         elif not np.isnan(new_data._data_start):
             self._data_start = np.min([self._data_start, new_data._data_start])
         if np.isnan(self._data_end):
             self._data_end = new_data._data_end
         elif not np.isnan(new_data._data_end):
             self._data_end = np.max([self._data_end, new_data._data_end])
-        if len(self._time_sync_exchanges_list[0]) > 0:
-            tse = tms.TriMessageStats(
-                "",
-                np.array(self._time_sync_exchanges_list[0]),
-                np.array(self._time_sync_exchanges_list[1]),
-                np.array(self._time_sync_exchanges_list[2]),
-                np.array(self._time_sync_exchanges_list[3]),
-                np.array(self._time_sync_exchanges_list[4]),
-                np.array(self._time_sync_exchanges_list[5]),
-            )
-            self._latencies = np.array((tse.latency1, tse.latency3))
-            self._offsets = np.array((tse.offset1, tse.offset3))
-            self._mean_latency = np.mean([*self._latencies[0], *self._latencies[1]])
-            self._latency_std = np.std([*self._latencies[0], *self._latencies[1]])
-            self._mean_offset = np.mean([*self._offsets[0], *self._offsets[1]])
-            self._offset_std = np.std([*self._offsets[0], *self._offsets[1]])
-            self._best_latency_index = tse.best_latency_index
-            self._best_msg_array_index = tse.best_latency_array_index
-            self._best_latency = tse.best_latency
-            self._best_offset = tse.best_offset
-            self._best_exchange_index_list = tse.best_latency_per_exchange_index_array
-            self._offset_model = OffsetModel(self._latencies.flatten(), self._offsets.flatten(),
-                                             self.get_device_exchanges_timestamps(),
-                                             self._data_start, self._data_end)
+        self._stats_from_exchanges()
 
     def from_raw_packets(self, packets: List[Union[RedvoxPacketM, RedvoxPacket]]) -> 'TimeSync':
         """
         converts packets into TimeSyncData objects, then performs analysis
 
         :param packets: list of RedvoxPacketM and RedvoxPacket to convert
         :return: modified version of self
@@ -406,51 +393,15 @@
                     if api900_pb2.TIME_SYNCHRONIZATION in ch.channel_types:
                         all_exchanges.extend(util_900.extract_payload(ch))
 
         if len(all_exchanges) > 0:
             self._time_sync_exchanges_list = np.transpose([
                 all_exchanges[i: i + 6] for i in range(0, len(all_exchanges), 6)
             ])
-            tse = tms.TriMessageStats(
-                "",
-                np.array(self._time_sync_exchanges_list[0]),
-                np.array(self._time_sync_exchanges_list[1]),
-                np.array(self._time_sync_exchanges_list[2]),
-                np.array(self._time_sync_exchanges_list[3]),
-                np.array(self._time_sync_exchanges_list[4]),
-                np.array(self._time_sync_exchanges_list[5]),
-            )
-            self._latencies = np.array((tse.latency1, tse.latency3))
-            self._offsets = np.array((tse.offset1, tse.offset3))
-            # Compute the statistics for latency and offset
-            self._mean_latency = np.mean([*self._latencies[0], *self._latencies[1]])
-            self._latency_std = np.std([*self._latencies[0], *self._latencies[1]])
-            self._mean_offset = np.mean([*self._offsets[0], *self._offsets[1]])
-            self._offset_std = np.std([*self._offsets[0], *self._offsets[1]])
-            self._best_latency_index = tse.best_latency_index
-            self._best_msg_array_index = tse.best_latency_array_index
-            self._best_latency = tse.best_latency
-            self._best_offset = tse.best_offset
-            self._best_exchange_index_list = tse.best_latency_per_exchange_index_array
-            self._offset_model = OffsetModel(self._latencies.flatten(), self._offsets.flatten(),
-                                             self.get_device_exchanges_timestamps(),
-                                             self._data_start, self._data_end)
-        else:
-            self._latencies = np.array(([], []))
-            self._offsets = np.array(([], []))
-            self._best_latency = np.nan
-            self._mean_latency = np.nan
-            self._latency_std = np.nan
-            self._best_offset = 0
-            self._mean_offset = np.nan
-            self._offset_std = np.nan
-            self._best_latency_index = -1
-            self._best_msg_array_index = 0
-            self._best_exchange_index_list = []
-            self._offset_model = OffsetModel.empty_model()
+            self._stats_from_exchanges()
         return self
 
     def sync_exchanges(self) -> np.ndarray:
         """
         :return: time sync exchanges
         """
         return self._time_sync_exchanges_list
@@ -485,17 +436,17 @@
 
     def latency_std(self) -> float:
         """
         :return: standard deviation of latency
         """
         return self._latency_std
 
-    def best_latency_index(self) -> float:
+    def best_latency_index(self) -> int:
         """
-        :return: index/position of best latency
+        :return: index/position of best latency or np.nan if no best latency exists
         """
         return self._best_latency_index
 
     def best_latency_per_exchange(self) -> np.array:
         """
         :return: the best latency per sync exchange as a numpy array
         """
```

### Comparing `redvox-3.4.1/redvox/common/timesync_io.py` & `redvox-3.4.2/redvox/common/timesync_io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/common/tri_message_stats.py` & `redvox-3.4.2/redvox/common/tri_message_stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,18 +18,19 @@
     ALL timestamps in microseconds
     Properties:
         packet_id: an identifier for the packet that contains the data.  Used for reporting purposes
         latency1: latencies measured by timestamps 1 and 2
         latency3: latencies measured by timestamps 2 and 3
         offset1: offsets measured by timestamps 1 and 2
         offset3: offsets measured by timestamps 2 and 3
-        best_latency: minimum latency that meets all criteria
-        best_offset: best offset that meets all criteria
-        best_latency_array_index: index in latency array with best latency
-        best_latency_index: index of which latency array has the best latency
+        best_latency: minimum latency that meets all criteria, default np.nan
+        best_offset: best offset that meets all criteria, default 0.0
+        best_latency_array_index: index of which latency array has the best latency, valid values are either 1 or 3,
+                                    all other values are invalid, default 0
+        best_latency_index: index in latency array with best latency, default None
         best_latency_per_exchange_index_array: the index of which latency array has the best latency, per each exchange
         num_messages: number of tri-message exchanges
     """
 
     def __init__(
         self,
         packet_id: Union[str, int],
@@ -59,18 +60,18 @@
         )
         self.latency1: np.ndarray = latencies_tuple[0]
         self.latency3: np.ndarray = latencies_tuple[1]
         offsets_tuple: Tuple[np.ndarray, np.ndarray] = offsets(a1, a2, a3, b1, b2, b3)
         self.offset1: np.ndarray = offsets_tuple[0]
         self.offset3: np.ndarray = offsets_tuple[1]
 
-        self.best_latency: Optional[float] = np.nan
-        self.best_latency_array_index: Optional[int] = None
+        self.best_latency: float = np.nan
+        self.best_latency_array_index: int = 0
         self.best_latency_index: Optional[int] = None
-        self.best_offset: Optional[float] = 0.0
+        self.best_offset: float = 0.0
 
         self.find_best_latency()
         self.find_best_offset()
         self.best_latency_per_exchange_index_array: List[int] = self.find_best_exchange_latencies_index()
 
     def find_best_latency(self) -> None:
         """
```

### Comparing `redvox-3.4.1/redvox/common/versioning.py` & `redvox-3.4.2/redvox/common/versioning.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.1/redvox/settings.py` & `redvox-3.4.2/redvox/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -68,16 +68,7 @@
     :return: True if the native extra is enabled, False otherwise
     """
     try:
         import redvox_native
         return True
     except ModuleNotFoundError:
         return False
-
-
-def is_cpp_backend_enabled() -> bool:
-    """
-    :return: True if the protobuf CPP backend is enabled, False otherwise
-    """
-    # noinspection PyUnresolvedReferences
-    from google.protobuf.internal import api_implementation
-    return api_implementation.Type() == "cpp"
```

### Comparing `redvox-3.4.1/redvox.egg-info/PKG-INFO` & `redvox-3.4.2/redvox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redvox
-Version: 3.4.1
+Version: 3.4.2
 Summary: Library for working with RedVox files. 
 Author-email: "RedVox, Inc" <support@redvox.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `redvox-3.4.1/redvox.egg-info/SOURCES.txt` & `redvox-3.4.2/redvox.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -93,48 +93,40 @@
 redvox/cloud/routes.py
 redvox/cloud/station_stats.py
 redvox/cloud/subscription.py
 redvox/common/__init__.py
 redvox/common/api_conversions.py
 redvox/common/api_reader.py
 redvox/common/api_reader_dw.py
-redvox/common/api_reader_old.py
 redvox/common/constants.py
 redvox/common/cross_stats.py
 redvox/common/data_window.py
 redvox/common/data_window_configuration.py
-redvox/common/data_window_configuration_old.py
 redvox/common/data_window_io.py
-redvox/common/data_window_old.py
 redvox/common/date_time_utils.py
 redvox/common/errors.py
 redvox/common/event_stream.py
 redvox/common/event_stream_io.py
 redvox/common/file_statistics.py
 redvox/common/gap_and_pad_utils.py
-redvox/common/gap_and_pad_utils_old.py
 redvox/common/io.py
 redvox/common/offset_model.py
 redvox/common/packet_to_pyarrow.py
 redvox/common/parallel_utils.py
 redvox/common/run_me.py
 redvox/common/sensor_data.py
-redvox/common/sensor_data_old.py
 redvox/common/sensor_io.py
 redvox/common/sensor_reader_utils.py
-redvox/common/sensor_reader_utils_old.py
 redvox/common/session_io.py
 redvox/common/session_model.py
 redvox/common/session_model_utils.py
 redvox/common/station.py
 redvox/common/station_io.py
 redvox/common/station_model.py
-redvox/common/station_old.py
 redvox/common/station_utils.py
 redvox/common/stats_helper.py
 redvox/common/timesync.py
 redvox/common/timesync_io.py
-redvox/common/timesync_old.py
 redvox/common/tri_message_stats.py
 redvox/common/versioning.py
 redvox/common/gui/__init__.py
 redvox/common/gui/cloud_data_retrieval.py
```

