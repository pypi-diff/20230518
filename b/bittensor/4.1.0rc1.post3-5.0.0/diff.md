# Comparing `tmp/bittensor-4.1.0rc1.post3.tar.gz` & `tmp/bittensor-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bittensor-4.1.0rc1.post3.tar", last modified: Wed May 10 19:12:58 2023, max compression
+gzip compressed data, was "bittensor-5.0.0.tar", last modified: Thu May 18 16:44:04 2023, max compression
```

## Comparing `bittensor-4.1.0rc1.post3.tar` & `bittensor-5.0.0.tar`

### file list

```diff
@@ -1,116 +1,115 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.573312 bittensor-4.1.0rc1.post3/
--rw-rw-r--   0 root         (0) root         (0)     1087 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4917 2023-05-10 19:12:58.573312 bittensor-4.1.0rc1.post3/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3369 2023-05-10 19:11:39.000000 bittensor-4.1.0rc1.post3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bin/
--rwxrwxr-x   0 root         (0) root         (0)     1297 2022-10-11 20:24:30.000000 bittensor-4.1.0rc1.post3/bin/btcli
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor/
--rw-rw-r--   0 root         (0) root         (0)    15549 2023-05-10 19:12:46.000000 bittensor-4.1.0rc1.post3/bittensor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor/_axon/
--rw-rw-r--   0 root         (0) root         (0)    17744 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_axon/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor/_cli/
--rw-rw-r--   0 root         (0) root         (0)     6688 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_cli/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3983 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_cli/cli_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor/_cli/commands/
--rw-rw-r--   0 root         (0) root         (0)      649 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_cli/commands/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    25104 2023-05-04 15:20:44.000000 bittensor-4.1.0rc1.post3/bittensor/_cli/commands/delegates.py
--rw-rw-r--   0 root         (0) root         (0)     7571 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post3/bittensor/_cli/commands/inspect.py
--rw-rw-r--   0 root         (0) root         (0)     3911 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post3/bittensor/_cli/commands/list.py
--rw-rw-r--   0 root         (0) root         (0)     7407 2023-05-10 19:11:39.000000 bittensor-4.1.0rc1.post3/bittensor/_cli/commands/metagraph.py
--rw-rw-r--   0 root         (0) root         (0)     7008 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_cli/commands/misc.py
--rw-rw-r--   0 root         (0) root         (0)    16429 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post3/bittensor/_cli/commands/overview.py
--rw-rw-r--   0 root         (0) root         (0)     7587 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post3/bittensor/_cli/commands/register.py
--rw-rw-r--   0 root         (0) root         (0)    11039 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post3/bittensor/_cli/commands/stake.py
--rw-rw-r--   0 root         (0) root         (0)     4349 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post3/bittensor/_cli/commands/transfer.py
--rw-rw-r--   0 root         (0) root         (0)    11156 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post3/bittensor/_cli/commands/unstake.py
--rw-rw-r--   0 root         (0) root         (0)     7733 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post3/bittensor/_cli/commands/utils.py
--rw-rw-r--   0 root         (0) root         (0)    17664 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post3/bittensor/_cli/commands/wallets.py
--rw-rw-r--   0 root         (0) root         (0)     4705 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post3/bittensor/_cli/commands/weights.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor/_config/
--rw-rw-r--   0 root         (0) root         (0)     6034 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_config/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5957 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_config/config_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor/_dataset/
--rw-rw-r--   0 root         (0) root         (0)    10966 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post3/bittensor/_dataset/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    27097 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post3/bittensor/_dataset/dataset_impl.py
--rw-rw-r--   0 root         (0) root         (0)     5467 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post3/bittensor/_dataset/dataset_mock.py
--rw-rw-r--   0 root         (0) root         (0)     3623 2022-10-11 20:17:46.000000 bittensor-4.1.0rc1.post3/bittensor/_dataset/thread_queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor/_dendrite/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_dendrite/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10220 2023-05-10 19:11:39.000000 bittensor-4.1.0rc1.post3/bittensor/_dendrite/dendrite.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor/_dendrite/text_prompting/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_dendrite/text_prompting/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10897 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_dendrite/text_prompting/dendrite.py
--rw-rw-r--   0 root         (0) root         (0)     5195 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_dendrite/text_prompting/dendrite_pool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor/_ipfs/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post3/bittensor/_ipfs/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2907 2023-02-21 20:04:30.000000 bittensor-4.1.0rc1.post3/bittensor/_ipfs/ipfs_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor/_keyfile/
--rw-rw-r--   0 root         (0) root         (0)     1894 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post3/bittensor/_keyfile/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    22266 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post3/bittensor/_keyfile/keyfile_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor/_logging/
--rw-rw-r--   0 root         (0) root         (0)    13107 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_logging/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor/_metagraph/
--rw-rw-r--   0 root         (0) root         (0)    12489 2023-05-10 19:11:39.000000 bittensor-4.1.0rc1.post3/bittensor/_metagraph/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor/_prometheus/
--rw-rw-r--   0 root         (0) root         (0)     8118 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post3/bittensor/_prometheus/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor/_proto/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post3/bittensor/_proto/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    37015 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_proto/bittensor_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     6201 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_proto/bittensor_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor/_serializer/
--rw-rw-r--   0 root         (0) root         (0)     6078 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_serializer/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10782 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_serializer/serializer_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor/_subtensor/
--rw-rw-r--   0 root         (0) root         (0)    14289 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_subtensor/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    26232 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_subtensor/chain_data.py
--rw-rw-r--   0 root         (0) root         (0)     2351 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post3/bittensor/_subtensor/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.573312 bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/
--rw-rw-r--   0 root         (0) root         (0)     1126 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    17164 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/delegation.py
--rw-rw-r--   0 root         (0) root         (0)    27011 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/log_utilities.py
--rw-rw-r--   0 root         (0) root         (0)     6056 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/prometheus.py
--rw-rw-r--   0 root         (0) root         (0)    14454 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/registration.py
--rw-rw-r--   0 root         (0) root         (0)    10152 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/serving.py
--rw-rw-r--   0 root         (0) root         (0)     6387 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/set_weights.py
--rw-rw-r--   0 root         (0) root         (0)    18492 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/staking.py
--rw-rw-r--   0 root         (0) root         (0)     7595 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/transfer.py
--rw-rw-r--   0 root         (0) root         (0)    15591 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/unstaking.py
--rw-rw-r--   0 root         (0) root         (0)    45559 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_subtensor/subtensor_impl.py
--rw-rw-r--   0 root         (0) root         (0)    18974 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post3/bittensor/_subtensor/subtensor_mock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.573312 bittensor-4.1.0rc1.post3/bittensor/_synapse/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_synapse/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6777 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_synapse/synapse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.573312 bittensor-4.1.0rc1.post3/bittensor/_synapse/text_prompting/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_synapse/text_prompting/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10714 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_synapse/text_prompting/miner.py
--rw-rw-r--   0 root         (0) root         (0)     7346 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_synapse/text_prompting/synapse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.573312 bittensor-4.1.0rc1.post3/bittensor/_threadpool/
--rw-rw-r--   0 root         (0) root         (0)     4517 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_threadpool/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8631 2022-11-24 17:43:32.000000 bittensor-4.1.0rc1.post3/bittensor/_threadpool/priority_thread_pool_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.573312 bittensor-4.1.0rc1.post3/bittensor/_tokenizer/
--rw-rw-r--   0 root         (0) root         (0)     2500 2022-10-11 20:17:46.000000 bittensor-4.1.0rc1.post3/bittensor/_tokenizer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.573312 bittensor-4.1.0rc1.post3/bittensor/_wallet/
--rw-rw-r--   0 root         (0) root         (0)     7293 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_wallet/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    41712 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post3/bittensor/_wallet/wallet_impl.py
--rw-rw-r--   0 root         (0) root         (0)     2287 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post3/bittensor/_wallet/wallet_mock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.573312 bittensor-4.1.0rc1.post3/bittensor/utils/
--rw-rw-r--   0 root         (0) root         (0)     8575 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post3/bittensor/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3443 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post3/bittensor/utils/_register_cuda.py
--rw-rw-r--   0 root         (0) root         (0)     8711 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post3/bittensor/utils/balance.py
--rw-rw-r--   0 root         (0) root         (0)     4457 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/utils/codes.py
--rw-rw-r--   0 root         (0) root         (0)      518 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post3/bittensor/utils/formatting.py
--rw-rw-r--   0 root         (0) root         (0)     8017 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post3/bittensor/utils/networking.py
--rw-rw-r--   0 root         (0) root         (0)    36116 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post3/bittensor/utils/registration.py
--rw-rw-r--   0 root         (0) root         (0)    33174 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post3/bittensor/utils/registratrion_old.py
--rw-rw-r--   0 root         (0) root         (0)     3373 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post3/bittensor/utils/stats.py
--rw-rw-r--   0 root         (0) root         (0)      630 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post3/bittensor/utils/test_utils.py
--rw-rw-r--   0 root         (0) root         (0)    75481 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post3/bittensor/utils/tokenizer_utils.py
--rw-rw-r--   0 root         (0) root         (0)     9986 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/utils/weight_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     4917 2023-05-10 19:12:58.000000 bittensor-4.1.0rc1.post3/bittensor.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3005 2023-05-10 19:12:58.000000 bittensor-4.1.0rc1.post3/bittensor.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-05-10 19:12:58.000000 bittensor-4.1.0rc1.post3/bittensor.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)     1044 2023-05-10 19:12:58.000000 bittensor-4.1.0rc1.post3/bittensor.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       10 2023-05-10 19:12:58.000000 bittensor-4.1.0rc1.post3/bittensor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 19:12:58.573312 bittensor-4.1.0rc1.post3/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     3436 2023-05-02 18:50:29.000000 bittensor-4.1.0rc1.post3/setup.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.288592 bittensor-5.0.0/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1087 2022-07-09 15:48:08.000000 bittensor-5.0.0/LICENSE
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     4395 2023-05-18 16:44:04.288592 bittensor-5.0.0/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3369 2023-05-18 16:31:28.000000 bittensor-5.0.0/README.md
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.280592 bittensor-5.0.0/bin/
+-rwxrwxr-x   0 eduardo   (1000) eduardo   (1000)     1297 2022-10-11 20:24:30.000000 bittensor-5.0.0/bin/btcli
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.280592 bittensor-5.0.0/bittensor/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    15485 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/__init__.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.280592 bittensor-5.0.0/bittensor/_axon/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    18031 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_axon/__init__.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_cli/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6777 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_cli/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3879 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_cli/cli_impl.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_cli/commands/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      613 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_cli/commands/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    24917 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_cli/commands/delegates.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7512 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_cli/commands/inspect.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3900 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_cli/commands/list.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7371 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_cli/commands/metagraph.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6968 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_cli/commands/misc.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    16312 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_cli/commands/overview.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7542 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_cli/commands/register.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    10946 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_cli/commands/stake.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     4312 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_cli/commands/transfer.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    11043 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_cli/commands/unstake.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7699 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_cli/commands/utils.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    17524 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_cli/commands/wallets.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_config/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5981 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_config/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5896 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_config/config_impl.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_dataset/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    10949 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_dataset/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    26660 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_dataset/dataset_impl.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5443 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_dataset/dataset_mock.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3581 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_dataset/thread_queue.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_dendrite/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_dendrite/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    10128 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_dendrite/dendrite.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_dendrite/text_prompting/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_dendrite/text_prompting/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    10806 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_dendrite/text_prompting/dendrite.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5215 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_dendrite/text_prompting/dendrite_pool.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_ipfs/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2022-07-09 15:48:08.000000 bittensor-5.0.0/bittensor/_ipfs/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2890 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_ipfs/ipfs_impl.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_keyfile/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1885 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_keyfile/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    22206 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_keyfile/keyfile_impl.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_logging/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    13062 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_logging/__init__.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_metagraph/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    12792 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_metagraph/__init__.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_prometheus/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     8080 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_prometheus/__init__.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_proto/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2022-07-09 15:48:08.000000 bittensor-5.0.0/bittensor/_proto/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    37015 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_proto/bittensor_pb2.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6201 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_proto/bittensor_pb2_grpc.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_serializer/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6062 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_serializer/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    10739 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_serializer/serializer_impl.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_subtensor/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    13432 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_subtensor/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    25954 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_subtensor/chain_data.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2344 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_subtensor/errors.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_subtensor/extrinsics/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1119 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_subtensor/extrinsics/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    17093 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_subtensor/extrinsics/delegation.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    26886 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_subtensor/extrinsics/log_utilities.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6020 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_subtensor/extrinsics/prometheus.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    14263 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_subtensor/extrinsics/registration.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    10108 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_subtensor/extrinsics/serving.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6376 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_subtensor/extrinsics/set_weights.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    18378 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_subtensor/extrinsics/staking.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7537 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_subtensor/extrinsics/transfer.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    15505 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_subtensor/extrinsics/unstaking.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    45395 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_subtensor/subtensor_impl.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    18999 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_subtensor/subtensor_mock.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_synapse/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_synapse/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6713 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_synapse/synapse.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_synapse/text_prompting/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_synapse/text_prompting/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    10680 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_synapse/text_prompting/miner.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7260 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_synapse/text_prompting/synapse.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_threadpool/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     4477 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_threadpool/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     8594 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_threadpool/priority_thread_pool_impl.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_tokenizer/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2485 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_tokenizer/__init__.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_wallet/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6891 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_wallet/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    41320 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_wallet/wallet_impl.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2286 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_wallet/wallet_mock.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.288592 bittensor-5.0.0/bittensor/utils/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     8536 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/utils/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3443 2023-04-20 18:56:12.000000 bittensor-5.0.0/bittensor/utils/_register_cuda.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     8699 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/utils/balance.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     4445 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/utils/codes.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      518 2023-04-20 18:56:12.000000 bittensor-5.0.0/bittensor/utils/formatting.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7999 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/utils/networking.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    35796 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/utils/registration.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    32876 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/utils/registratrion_old.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3351 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/utils/stats.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      630 2022-07-09 15:48:08.000000 bittensor-5.0.0/bittensor/utils/test_utils.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    75481 2023-03-23 20:47:08.000000 bittensor-5.0.0/bittensor/utils/tokenizer_utils.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     9929 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/utils/weight_utils.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.280592 bittensor-5.0.0/bittensor.egg-info/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     4395 2023-05-18 16:44:04.000000 bittensor-5.0.0/bittensor.egg-info/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2970 2023-05-18 16:44:04.000000 bittensor-5.0.0/bittensor.egg-info/SOURCES.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2023-05-18 16:44:04.000000 bittensor-5.0.0/bittensor.egg-info/dependency_links.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1044 2023-05-18 16:44:04.000000 bittensor-5.0.0/bittensor.egg-info/requires.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       10 2023-05-18 16:44:04.000000 bittensor-5.0.0/bittensor.egg-info/top_level.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2023-05-18 16:44:04.288592 bittensor-5.0.0/setup.cfg
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3429 2023-05-18 16:31:28.000000 bittensor-5.0.0/setup.py
```

### Comparing `bittensor-4.1.0rc1.post3/LICENSE` & `bittensor-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post3/PKG-INFO` & `bittensor-5.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,80 +1,15 @@
 Metadata-Version: 2.1
 Name: bittensor
-Version: 4.1.0rc1.post3
+Version: 5.0.0
 Summary: bittensor
 Home-page: https://github.com/opentensor/bittensor
 Author: bittensor.com
 Author-email: 
 License: MIT
-Description: <div align="center">
-        
-        # **Bittensor** <!-- omit in toc -->
-        [![Discord Chat](https://img.shields.io/discord/308323056592486420.svg)](https://discord.gg/bittensor)
-        [![PyPI version](https://badge.fury.io/py/bittensor.svg)](https://badge.fury.io/py/bittensor)
-        [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 
-        
-        ---
-        
-        ### Internet-scale Neural Networks <!-- omit in toc -->
-        
-        [Discord](https://discord.gg/bittensor) • [Network](https://taostats.io/) • [Research](https://drive.google.com/file/d/1VnsobL6lIAAqcA1_Tbm8AYIQscfJV4KU)
-        
-        </div>
-        
-        This repository contains Bittensor's Python API, which can be used for the following purposes:
-        
-        1. Querying the Bittensor network as a client.
-        2. Running and building Bittensor miners and validators.
-        3. Pulling network state information.
-        4. Managing TAO wallets, balances, transfers, etc.
-        
-        Bittensor is a mining network, similar to Bitcoin, that includes built-in incentives designed to encourage miners to provide value by hosting trained or training machine learning models. These models can be queried by clients seeking inference over inputs, such as token-based text generations or numerical embeddings from a large foundation model like GPT-NeoX-20B.
-        
-        Token-based incentives are designed to drive the network's growth and distribute the value generated by the network directly to the individuals producing that value, without intermediaries. The network is open to all participants, and no individual or group has full control over what is learned, who can profit from it, or who can access it.
-        
-        To learn more about Bittensor, please read our [paper](https://drive.google.com/file/d/1VnsobL6lIAAqcA1_Tbm8AYIQscfJV4KU/view).
-        
-        # Install
-        There are three ways to install Bittensor
-        
-        1. Through the installer:
-        ```
-        $ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/opentensor/bittensor/master/scripts/install.sh)"
-        ```
-        
-        2. With pip:
-        ```bash
-        $ pip3 install bittensor
-        ```
-        
-        3. From source:
-        ```
-        $ git clone https://github.com/opentensor/bittensor.git
-        $ python3 -m pip install -e bittensor/
-        ```
-        
-        ## Release
-        The release manager should follow the instructions of the [RELEASE_GUIDELINES.md](./RELEASE_GUIDELINES.md) document.
-        
-        ## License
-        The MIT License (MIT)
-        Copyright © 2021 Yuma Rao
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-        
-        
-        ## Acknowledgments
-        **learning-at-home/hivemind**
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -84,7 +19,72 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+<div align="center">
+
+# **Bittensor** <!-- omit in toc -->
+[![Discord Chat](https://img.shields.io/discord/308323056592486420.svg)](https://discord.gg/bittensor)
+[![PyPI version](https://badge.fury.io/py/bittensor.svg)](https://badge.fury.io/py/bittensor)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 
+
+---
+
+### Internet-scale Neural Networks <!-- omit in toc -->
+
+[Discord](https://discord.gg/bittensor) • [Network](https://taostats.io/) • [Research](https://drive.google.com/file/d/1VnsobL6lIAAqcA1_Tbm8AYIQscfJV4KU)
+
+</div>
+
+This repository contains Bittensor's Python API, which can be used for the following purposes:
+
+1. Querying the Bittensor network as a client.
+2. Running and building Bittensor miners and validators.
+3. Pulling network state information.
+4. Managing TAO wallets, balances, transfers, etc.
+
+Bittensor is a mining network, similar to Bitcoin, that includes built-in incentives designed to encourage miners to provide value by hosting trained or training machine learning models. These models can be queried by clients seeking inference over inputs, such as token-based text generations or numerical embeddings from a large foundation model like GPT-NeoX-20B.
+
+Token-based incentives are designed to drive the network's growth and distribute the value generated by the network directly to the individuals producing that value, without intermediaries. The network is open to all participants, and no individual or group has full control over what is learned, who can profit from it, or who can access it.
+
+To learn more about Bittensor, please read our [paper](https://drive.google.com/file/d/1VnsobL6lIAAqcA1_Tbm8AYIQscfJV4KU/view).
+
+# Install
+There are three ways to install Bittensor
+
+1. Through the installer:
+```
+$ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/opentensor/bittensor/master/scripts/install.sh)"
+```
+
+2. With pip:
+```bash
+$ pip3 install bittensor
+```
+
+3. From source:
+```
+$ git clone https://github.com/opentensor/bittensor.git
+$ python3 -m pip install -e bittensor/
+```
+
+## Release
+The release manager should follow the instructions of the [RELEASE_GUIDELINES.md](./RELEASE_GUIDELINES.md) document.
+
+## License
+The MIT License (MIT)
+Copyright © 2021 Yuma Rao
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
+
+## Acknowledgments
+**learning-at-home/hivemind**
```

### Comparing `bittensor-4.1.0rc1.post3/README.md` & `bittensor-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post3/bin/btcli` & `bittensor-5.0.0/bin/btcli`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post3/bittensor/__init__.py` & `bittensor-5.0.0/bittensor/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import torch
 from typing import Union, List, Dict
 from rich.console import Console
 from rich.traceback import install
 from prometheus_client import Info
 from langchain.llms.base import LLM
 from typing import Optional, List, Mapping, Any, Tuple
 
 import nest_asyncio
 nest_asyncio.apply()
 
 # Bittensor code and protocol version.
-__version__ = '4.1.0-rc1-3'
-version_split = __version__.split("-")[0].split(".")
+__version__ = '5.0.0'
+version_split = __version__.split(".")
 __version_as_int__ = (100 * int(version_split[0])) + (10 * int(version_split[1])) + (1 * int(version_split[2]))
 __new_signature_version__ = 360
 
 # Turn off rich console locals trace.
 from rich.traceback import install
 install(show_locals=False)
 
@@ -113,28 +113,28 @@
 
 # --- Prometheus ---
 __prometheus_version__ = "0.1.0"
 prometheus_version__split = __prometheus_version__.split(".")
 __prometheus_version__as_int__ = (100 * int(prometheus_version__split[0])) + (10 * int(prometheus_version__split[1])) + (1 * int(prometheus_version__split[2]))
 try:
     bt_promo_info = Info("bittensor_info", "Information about the installed bittensor package.")
-    bt_promo_info.info ( 
+    bt_promo_info.info (
         {
             '__version__': str(__version__),
             '__version_as_int__': str(__version_as_int__),
             '__vocab_size__': str(__vocab_size__),
             '__network_dim__': str(__network_dim__),
             '__blocktime__': str(__blocktime__),
             '__prometheus_version__': str(__prometheus_version__),
             '__prometheus_version__as_int__': str(__prometheus_version__as_int__),
-        } 
+        }
     )
-except ValueError: 
+except ValueError:
     # This can silently fail if we import bittensor twice in the same process.
-    # We simply pass over this error. 
+    # We simply pass over this error.
     pass
 
 
 # ---- Config ----
 from bittensor._config import config as config
 
 # ---- LOGGING ----
@@ -240,25 +240,25 @@
 Chattensor is a research project by Opentensor Cortex.
 Chattensor is designed to be able to assist with a wide range of tasks, from answering simple questions to providing in-depth explanations and discussions on a wide range of topics. As a language model, Chattensor is able to generate human-like text based on the input it receives, allowing it to engage in natural-sounding conversations and provide responses that are coherent and relevant to the topic at hand.
 '''
 
 default_prompting_validator_key = '5F4tQyWrhfGVcNhoqeiNsR6KjD4wMZ2kfhLj4oHYuyHbZAc3'
 
 __context_prompting_llm = None
-def prompt( 
+def prompt(
         content: Union[ str, List[str], List[Dict[ str ,str ]]],
         wallet_name: str = "default",
         hotkey: str = default_prompting_validator_key,
         subtensor_: Optional['Subtensor'] = None,
         axon_: Optional['axon_info'] = None,
         return_all: bool = False,
     ) -> str:
     global __context_prompting_llm
     if __context_prompting_llm == None:
-        __context_prompting_llm = prompting( 
+        __context_prompting_llm = prompting(
             wallet_name = wallet_name,
             hotkey = hotkey,
             subtensor_ = subtensor_,
             axon_ = axon_,
         )
     return __context_prompting_llm( content = content, return_all = return_all )
 
@@ -280,15 +280,15 @@
         super(prompting, self).__init__()
         self._hotkey = hotkey
         self._subtensor = subtensor() if subtensor_ is None else subtensor_
         if use_coldkey:
             self._keypair = wallet( name = wallet_name ).create_if_non_existent().coldkey
         else:
             self._keypair = wallet( name = wallet_name ).create_if_non_existent().hotkey
-        
+
         if axon_ is not None:
             self._axon = axon_
         else:
             self._metagraph = metagraph( 1 )
             self._axon = self._metagraph.axons[ self._metagraph.hotkeys.index( self._hotkey ) ]
         self._dendrite = text_prompting(
             keypair = self._keypair,
@@ -297,23 +297,23 @@
 
     @staticmethod
     def format_content( content: Union[ str, List[str], List[Dict[ str ,str ]]] ) -> Tuple[ List[str], List[str ]]:
         if isinstance( content, str ):
             return ['system', 'user'], [ default_prompt, content ]
         elif isinstance( content, list ):
             if isinstance( content[0], str ):
-                return ['user' for _ in content ], content 
+                return ['user' for _ in content ], content
             elif isinstance( content[0], dict ):
                 return [ dictitem[ list(dictitem.keys())[0] ] for dictitem in content ], [ dictitem[ list(dictitem.keys())[1] ] for dictitem in content ]
             else:
                 raise ValueError('content has invalid type {}'.format( type( content )))
         else:
             raise ValueError('content has invalid type {}'.format( type( content )))
-        
-    def forward( 
+
+    def forward(
             self,
             content: Union[ str, List[str], List[Dict[ str ,str ]]],
             timeout: float = 24,
             return_call: bool = False,
             return_all: bool = False,
         ) -> Union[str, List[str]]:
         roles, messages = self.format_content( content )
@@ -326,16 +326,16 @@
         else:
             return self._dendrite.multi_forward(
                 roles = roles,
                 messages = messages,
                 timeout = timeout
             ).multi_completions
 
-       
-    async def async_forward( 
+
+    async def async_forward(
             self,
             content: Union[ str, List[str], List[Dict[ str ,str ]]],
             timeout: float = 24,
             return_all: bool = False,
         ) -> Union[str, List[str]]:
         roles, messages = self.format_content( content )
         if not return_all:
@@ -348,17 +348,17 @@
             return self._dendrite.async_multi_forward(
                 roles = roles,
                 messages = messages,
                 timeout = timeout
             ).multi_completions
 
 class BittensorLLM(LLM):
-    """Wrapper around Bittensor Prompting Subnetwork. 
+    """Wrapper around Bittensor Prompting Subnetwork.
 This Python file implements the BittensorLLM class, a wrapper around the Bittensor Prompting Subnetwork for easy integration into language models. The class provides a query method to receive responses from the subnetwork for a given user message and an implementation of the _call method to return the best response. The class can be initialized with various parameters such as the wallet name and chain endpoint.
-    
+
     Example:
         .. code-block:: python
 
             from bittensor import BittensorLLM
             btllm = BittensorLLM(wallet_name="default")
     """
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_axon/__init__.py` & `bittensor-5.0.0/bittensor/_axon/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 import bittensor.utils.networking as net
 from typing import Callable, Dict, Optional, Tuple, Union
 
 class axon:
     """ Axon object for serving synapse receptors. """
 
     def info(self) -> 'axon_info':
-        """Returns the axon info object associate with this axon.""" 
+        """Returns the axon info object associate with this axon."""
         return axon_info(
             version = bittensor.__version_as_int__,
             ip = self.external_ip,
             ip_type = 4,
             port = self.external_port,
             hotkey = self.wallet.hotkey.ss58_address,
             coldkey = self.wallet.coldkeypub.ss58_address,
@@ -54,14 +54,15 @@
         metagraph: "bittensor.Metagraph",
         config: Optional["bittensor.config"] = None,
         port: Optional[int] = None,
         ip: Optional[str] = None,
         external_ip: Optional[str] = None,
         external_port: Optional[int] = None,
         max_workers: Optional[int] = None,
+        server: "grpc._server._Server" = None,
         maximum_concurrent_rpcs: Optional[int] = None,
         blacklist: Optional[Callable] = None,
     ) -> "bittensor.Axon":
         r"""Creates a new bittensor.Axon object from passed arguments.
         Args:
             config (:obj:`Optional[bittensor.Config]`, `optional`):
                 bittensor.axon.config()
@@ -119,22 +120,27 @@
         # Build interceptor.
         self.receiver_hotkey = self.wallet.hotkey.ss58_address
         self.auth_interceptor = AuthInterceptor(
             receiver_hotkey=self.receiver_hotkey, blacklist=self.blacklist
         )
 
         # Build grpc server
-        self.thread_pool = futures.ThreadPoolExecutor(max_workers=self.config.axon.max_workers)
-        self.server = grpc.server(
-            self.thread_pool,
-            interceptors=(self.auth_interceptor,),
-            maximum_concurrent_rpcs=self.config.axon.maximum_concurrent_rpcs,
-            options=[("grpc.keepalive_time_ms", 100000), ("grpc.keepalive_timeout_ms", 500000)],
-        )
-        self.server.add_insecure_port(self.full_address)
+        if server is None:
+            self.thread_pool = futures.ThreadPoolExecutor(max_workers=self.config.axon.max_workers)
+            self.server = grpc.server(
+                self.thread_pool,
+                interceptors=(self.auth_interceptor,),
+                maximum_concurrent_rpcs=self.config.axon.maximum_concurrent_rpcs,
+                options=[("grpc.keepalive_time_ms", 100000), ("grpc.keepalive_timeout_ms", 500000)],
+            )
+            self.server.add_insecure_port(self.full_address)
+        else:
+            self.server = server
+            self.thread_pool = server._state.thread_pool
+            self.server.add_insecure_port(self.full_address)
 
     @classmethod
     def config(cls) -> "bittensor.Config":
         """Get config from the argument parser
         Return: bittensor.config object
         """
         parser = argparse.ArgumentParser()
@@ -180,15 +186,15 @@
                 required=False,
                 help="""The external ip this axon broadcasts to the network to. ie. [::]""",
                 default=bittensor.defaults.axon.external_ip,
             )
             parser.add_argument(
                 "--" + prefix_str + "axon.max_workers",
                 type=int,
-                help="""The maximum number connection handler threads working simultaneously on this endpoint. 
+                help="""The maximum number connection handler threads working simultaneously on this endpoint.
                         The grpc server distributes new worker threads to service requests up to this number.""",
                 default=bittensor.defaults.axon.max_workers,
             )
             parser.add_argument(
                 "--" + prefix_str + "axon.maximum_concurrent_rpcs",
                 type=int,
                 help="""Maximum number of allowed active connections""",
@@ -254,15 +260,15 @@
             self.server.stop(grace=1)
         self.server.start()
         self.started = True
         return self
 
     def stop(self) -> "bittensor.axon":
         r"""Stop the axon grpc server."""
-        if self.server is not None:
+        if hasattr(self, "server") and self.server is not None:
             self.server.stop(grace=1)
         self.started = False
 
 
 class AuthInterceptor(grpc.ServerInterceptor):
     """Creates a new server interceptor that authenticates incoming messages from passed arguments."""
 
@@ -302,15 +308,14 @@
         r"""Attempts to parse a signature from the metadata"""
         signature = metadata.get("bittensor-signature")
         version = metadata.get('bittensor-version')
         if signature is None:
             raise Exception("Request signature missing")
         if int(version) < 370:
             raise Exception("Incorrect Version")
-        
         parts = self.parse_signature_v2(signature)
         if parts is not None:
             return parts
         raise Exception("Unknown signature format")
 
     def check_signature(
         self,
@@ -334,15 +339,15 @@
             if nonce <= previous_nonce:
                 raise Exception("Nonce is too small")
 
         if not keypair.verify(message, signature):
             raise Exception("Signature mismatch")
         self.nonces[endpoint_key] = nonce
 
-    def black_list_checking(self, hotkey: str):
+    def black_list_checking(self, hotkey: str, method: str):
         r"""Tries to call to blacklist function in the miner and checks if it should blacklist the pubkey"""
         if self.blacklist is None:
             return
 
         request_type = {
             "/Bittensor/Forward": bittensor.proto.RequestType.FORWARD,
             "/Bittensor/Backward": bittensor.proto.RequestType.BACKWARD,
@@ -350,15 +355,14 @@
         if request_type is None:
             raise Exception("Unknown request type")
 
         failed, error_message =  self.blacklist(hotkey, request_type)
         if failed:
             raise Exception(str(error_message))
 
-
     def intercept_service(self, continuation, handler_call_details):
         r"""Authentication between bittensor nodes. Intercepts messages and checks them"""
         method = handler_call_details.method
         metadata = dict(handler_call_details.invocation_metadata)
 
         try:
             (
@@ -370,15 +374,15 @@
 
             # signature checking
             self.check_signature(
                 nonce, sender_hotkey, signature, receptor_uuid
             )
 
             # blacklist checking
-            self.black_list_checking(sender_hotkey)
+            self.black_list_checking(sender_hotkey, method)
 
             return continuation(handler_call_details)
 
         except Exception as e:
             message = str(e)
             abort = lambda _, ctx: ctx.abort(grpc.StatusCode.UNAUTHENTICATED, message)
             return grpc.unary_unary_rpc_method_handler(abort)
@@ -389,41 +393,41 @@
 @dataclass
 class axon_info:
 
     version: int
     ip: str
     port: int
     ip_type: int
-    hotkey: str 
+    hotkey: str
     coldkey: str
     protocol:int = 4,
     placeholder1:int = 0,
     placeholder2:int = 0,
 
     @property
     def is_serving(self) -> bool:
         """ True if the endpoint is serving. """
         if self.ip == '0.0.0.0': return False
         else:return True
 
     def ip_str(self) -> str:
-        """ Return the whole ip as string """ 
+        """ Return the whole ip as string """
         return net.ip__str__(self.ip_type, self.ip, self.port)
 
     def __eq__ (self, other: 'axon_info'):
         if other == None: return False
         if self.version == other.version and self.ip == other.ip and self.port == other.port and self.ip_type == other.ip_type and self.coldkey == other.coldkey and self.hotkey == other.hotkey: return True
-        else: return False 
+        else: return False
 
-    def __str__(self): 
+    def __str__(self):
         return "axon_info( {}, {}, {}, {} )".format( str(self.ip_str()), str(self.hotkey), str(self.coldkey), self.version)
-    
+
     def __repr__(self):
         return self.__str__()
-        
+
     @classmethod
     def from_neuron_info(cls, neuron_info: dict ) -> 'axon_info':
         """ Converts a dictionary to an axon_info object. """
         return cls(
             version = neuron_info['axon_info']['version'],
             ip = bittensor.utils.networking.int_to_ip(int(neuron_info['axon_info']['ip'])),
             port = neuron_info['axon_info']['port'],
@@ -431,16 +435,16 @@
             hotkey = neuron_info['hotkey'],
             coldkey = neuron_info['coldkey'],
         )
 
     def to_parameter_dict( self ) -> 'torch.nn.ParameterDict':
         r""" Returns a torch tensor of the subnet info.
         """
-        return torch.nn.ParameterDict( 
+        return torch.nn.ParameterDict(
             self.__dict__
         )
-    
+
     @classmethod
     def from_parameter_dict( cls, parameter_dict: 'torch.nn.ParameterDict' ) -> 'SubnetInfo':
         r""" Returns a SubnetInfo object from a torch parameter_dict.
         """
         return cls( **dict(parameter_dict) )
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_cli/__init__.py` & `bittensor-5.0.0/bittensor/_cli/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
-Create and init the CLI class, which handles the coldkey, hotkey and money transfer 
+Create and init the CLI class, which handles the coldkey, hotkey and money transfer
 """
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 # Copyright © 2022 Opentensor Foundation
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import sys
 import argparse
 import bittensor
 from . import cli_impl
 from .commands import *
@@ -29,49 +29,48 @@
 
 # Turn off rich console locals trace.
 from rich.traceback import install
 install(show_locals=False)
 
 class cli:
     """
-    Create and init the CLI class, which handles the coldkey, hotkey and tao transfer 
+    Create and init the CLI class, which handles the coldkey, hotkey and tao transfer
     """
     def __new__(
             cls,
             config: Optional['bittensor.Config'] = None,
-            args: Optional[List[str]] = None, 
+            args: Optional[List[str]] = None,
         ) -> 'bittensor.CLI':
         r""" Creates a new bittensor.cli from passed arguments.
             Args:
-                config (:obj:`bittensor.Config`, `optional`): 
+                config (:obj:`bittensor.Config`, `optional`):
                     bittensor.cli.config()
-                args (`List[str]`, `optional`): 
+                args (`List[str]`, `optional`):
                     The arguments to parse from the command line.
         """
-        if config == None:  
+        if config == None:
             config = cli.config( args )
         cli.check_config( config )
-        
+
         return cli_impl.CLI( config = config)
-        
+
     @staticmethod
     def __create_parser__() -> 'argparse.ArgumentParser':
         """ Creates the argument parser for the bittensor cli.
         """
         parser = argparse.ArgumentParser(
             description=f"bittensor cli v{bittensor.__version__}",
             usage="btcli <command> <command args>",
             add_help=True)
 
         cmd_parsers = parser.add_subparsers(dest='command')
         ListCommand.add_args( cmd_parsers )
         StakeCommand.add_args( cmd_parsers )
         UpdateCommand.add_args( cmd_parsers )
-        InspectCommand.add_args( cmd_parsers ) 
-        WeightsCommand.add_args( cmd_parsers )
+        InspectCommand.add_args( cmd_parsers )
         UnStakeCommand.add_args( cmd_parsers )
         OverviewCommand.add_args( cmd_parsers )
         RegisterCommand.add_args( cmd_parsers )
         TransferCommand.add_args( cmd_parsers )
         NominateCommand.add_args( cmd_parsers )
         NewHotkeyCommand.add_args( cmd_parsers )
         MetagraphCommand.add_args( cmd_parsers )
@@ -84,29 +83,38 @@
         DelegateUnstakeCommand.add_args( cmd_parsers )
         ListDelegatesCommand.add_args( cmd_parsers )
         RegenColdkeypubCommand.add_args( cmd_parsers )
         RecycleRegisterCommand.add_args( cmd_parsers )
 
         return parser
 
-    @staticmethod   
+    @staticmethod
+    def config(args: List[str]) -> 'bittensor.config':
+        """ From the argument parser, add config to bittensor.executor and local config
+            Return: bittensor.config object
+        """
+        parser = cli.__create_parser__()
+
+        return parser
+
+    @staticmethod
     def config(args: List[str]) -> 'bittensor.config':
-        """ From the argument parser, add config to bittensor.executor and local config 
+        """ From the argument parser, add config to bittensor.executor and local config
             Return: bittensor.config object
         """
         parser = cli.__create_parser__()
 
         # If no arguments are passed, print help text.
         if len(args) == 0:
             parser.print_help()
             sys.exit()
 
         return bittensor.config( parser, args=args )
 
-    @staticmethod   
+    @staticmethod
     def check_config (config: 'bittensor.Config'):
         """ Check if the essential config exist under different command
         """
         if config.command == "transfer":
             TransferCommand.check_config( config )
         elif config.command == "register":
             RegisterCommand.check_config( config )
@@ -124,16 +132,14 @@
             RegenColdkeyCommand.check_config( config )
         elif config.command == "regen_coldkeypub":
             RegenColdkeypubCommand.check_config( config )
         elif config.command == "regen_hotkey":
             RegenHotkeyCommand.check_config( config )
         elif config.command == "metagraph":
             MetagraphCommand.check_config( config )
-        elif config.command == "weights":
-            WeightsCommand.check_config( config )
         elif config.command == "list":
             ListCommand.check_config( config )
         elif config.command == "inspect":
             InspectCommand.check_config( config )
         elif config.command == "update":
             UpdateCommand.check_config( config )
         elif config.command == "nominate":
@@ -150,8 +156,7 @@
             MyDelegatesCommand.check_config( config )
         elif config.command == "recycle_register":
             RecycleRegisterCommand.check_config( config )
         else:
             console.print(":cross_mark:[red]Unknown command: {}[/red]".format(config.command))
             sys.exit()
 
-
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_cli/cli_impl.py` & `bittensor-5.0.0/bittensor/_cli/cli_impl.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 
 import bittensor
 from .commands import *
 
 class CLI:
     """
-    Implementation of the CLI class, which handles the coldkey, hotkey and money transfer 
+    Implementation of the CLI class, which handles the coldkey, hotkey and money transfer
     """
     def __init__(self, config: 'bittensor.Config' ):
         r""" Initialized a bittensor.CLI object.
             Args:
-                config (:obj:`bittensor.Config`, `required`): 
+                config (:obj:`bittensor.Config`, `required`):
                     bittensor.cli.config()
         """
         # (d)efaults to True if config.no_version_checking is not set.
         if not config.get("no_version_checking", d=True):
             try:
                 bittensor.utils.version_checking()
             except:
                 raise RuntimeError("To avoid internet based version checking pass --no_version_checking while running the CLI.")
         self.config = config
 
     def run ( self ):
-        """ Execute the command from config 
+        """ Execute the command from config
         """
         if self.config.command == "transfer":
             TransferCommand.run( self )
         elif self.config.command == "register":
             RegisterCommand.run( self )
         elif self.config.command == "unstake":
             UnStakeCommand.run( self )
@@ -60,16 +60,14 @@
             RegenColdkeyCommand.run( self )
         elif self.config.command == "regen_coldkeypub":
             RegenColdkeypubCommand.run( self )
         elif self.config.command == "regen_hotkey":
             RegenHotkeyCommand.run( self )
         elif self.config.command == "metagraph":
             MetagraphCommand.run( self )
-        elif self.config.command == "weights":
-            WeightsCommand.run( self )
         elif self.config.command == "inspect":
             InspectCommand.run( self )
         elif self.config.command == 'update':
             UpdateCommand.run( self )
         elif self.config.command == 'nominate':
             NominateCommand.run( self )
         elif self.config.command == 'delegate':
@@ -80,8 +78,8 @@
             MyDelegatesCommand.run( self )
         elif self.config.command == 'list_delegates':
             ListDelegatesCommand.run( self )
         elif self.config.command == 'list_subnets':
             ListSubnetsCommand.run( self )
         elif self.config.command == 'recycle_register':
             RecycleRegisterCommand.run( self )
-        
+
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_cli/commands/__init__.py` & `bittensor-5.0.0/bittensor/_cli/commands/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,9 +4,8 @@
 from .register import RegisterCommand, RecycleRegisterCommand
 from .delegates import NominateCommand, ListDelegatesCommand, DelegateStakeCommand, DelegateUnstakeCommand, MyDelegatesCommand
 from .wallets import NewColdkeyCommand, NewHotkeyCommand, RegenColdkeyCommand, RegenColdkeypubCommand, RegenHotkeyCommand
 from .transfer import TransferCommand
 from .inspect import InspectCommand
 from .metagraph import MetagraphCommand
 from .list import ListCommand
-from .weights import WeightsCommand
 from .misc import UpdateCommand, ListSubnetsCommand
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_cli/commands/delegates.py` & `bittensor-5.0.0/bittensor/_cli/commands/delegates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # The MIT License (MIT)
 # Copyright © 2023 OpenTensor Foundation
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import sys
 import os
 import json
 import argparse
 import bittensor
@@ -128,64 +128,64 @@
 
     @staticmethod
     def run( cli ):
         '''Delegates stake to a chain delegate.'''
         config = cli.config.copy()
         wallet = bittensor.wallet( config = config )
         subtensor: bittensor.Subtensor = bittensor.subtensor( config = config )
-        subtensor.delegate( 
-            wallet = wallet, 
-            delegate_ss58 = config.get('delegate_ss58key'), 
-            amount = config.get('amount'), 
-            wait_for_inclusion = True, 
-            prompt = not config.no_prompt 
+        subtensor.delegate(
+            wallet = wallet,
+            delegate_ss58 = config.get('delegate_ss58key'),
+            amount = config.get('amount'),
+            wait_for_inclusion = True,
+            prompt = not config.no_prompt
         )
 
     @staticmethod
     def add_args( parser: argparse.ArgumentParser ):
         delegate_stake_parser = parser.add_parser(
-            'delegate', 
+            'delegate',
             help='''Delegate Stake to an account.'''
         )
-        delegate_stake_parser.add_argument( 
-            '--no_version_checking', 
-            action='store_true', 
-            help='''Set false to stop cli version checking''', 
-            default = False 
+        delegate_stake_parser.add_argument(
+            '--no_version_checking',
+            action='store_true',
+            help='''Set false to stop cli version checking''',
+            default = False
         )
         delegate_stake_parser.add_argument(
-            '--delegate_ss58key', 
+            '--delegate_ss58key',
             '--delegate_ss58',
             dest = "delegate_ss58key",
-            type = str,  
+            type = str,
             required = False,
-            help='''The ss58 address of the choosen delegate''', 
+            help='''The ss58 address of the choosen delegate''',
         )
         delegate_stake_parser.add_argument(
-            '--all', 
-            dest="stake_all", 
+            '--all',
+            dest="stake_all",
             action='store_true'
         )
         delegate_stake_parser.add_argument(
-            '--amount', 
-            dest="amount", 
-            type=float, 
+            '--amount',
+            dest="amount",
+            type=float,
             required=False
-        )        
+        )
         delegate_stake_parser.add_argument(
-            '--no_prompt', 
-            dest='no_prompt', 
-            action='store_true', 
+            '--no_prompt',
+            dest='no_prompt',
+            action='store_true',
             help='''Set true to avoid prompting the user.''',
             default=False,
         )
         bittensor.wallet.add_args( delegate_stake_parser )
         bittensor.subtensor.add_args( delegate_stake_parser )
 
-    @staticmethod   
+    @staticmethod
     def check_config( config: 'bittensor.Config' ):
         if not config.get('delegate_ss58key'):
             # Check for delegates.
             with bittensor.__console__.status(":satellite: Loading delegates..."):
                 subtensor = bittensor.subtensor( config = config )
                 delegates: List[bittensor.DelegateInfo] = subtensor.get_delegates()
                 try:
@@ -195,25 +195,25 @@
 
             if prev_delegates is None:
                 bittensor.__console__.print(":warning: [yellow]Could not fetch delegates history[/yellow]")
 
             if len(delegates) == 0:
                 console.print(":cross_mark: [red]There are no delegates on {}[/red]".format(subtensor.network))
                 sys.exit(1)
-            
+
             delegates.sort(key=lambda delegate: delegate.total_stake, reverse=True)
             show_delegates( delegates, prev_delegates = prev_delegates)
             delegate_index = Prompt.ask("Enter delegate index")
             config.delegate_ss58key = str(delegates[int(delegate_index)].hotkey_ss58)
             console.print("Selected: [yellow]{}[/yellow]".format(config.delegate_ss58key))
 
         if config.wallet.get('name') == bittensor.defaults.wallet.name and not config.no_prompt:
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
-            
+
         # Get amount.
         if not config.get('amount') and not config.get('stake_all'):
             if not Confirm.ask("Stake all Tao from account: [bold]'{}'[/bold]?".format(config.wallet.get('name', bittensor.defaults.wallet.name))):
                 amount = Prompt.ask("Enter Tao amount to stake")
                 try:
                     config.amount = float(amount)
                 except ValueError:
@@ -226,64 +226,64 @@
 
     @staticmethod
     def run( cli ):
         '''Undelegates stake from a chain delegate.'''
         config = cli.config.copy()
         wallet = bittensor.wallet( config = config )
         subtensor: bittensor.Subtensor = bittensor.subtensor( config = config )
-        subtensor.undelegate( 
-            wallet = wallet, 
-            delegate_ss58 = config.get('delegate_ss58key'), 
-            amount = config.get('amount'), 
-            wait_for_inclusion = True, 
-            prompt = not config.no_prompt 
+        subtensor.undelegate(
+            wallet = wallet,
+            delegate_ss58 = config.get('delegate_ss58key'),
+            amount = config.get('amount'),
+            wait_for_inclusion = True,
+            prompt = not config.no_prompt
         )
 
     @staticmethod
     def add_args( parser: argparse.ArgumentParser ):
         undelegate_stake_parser = parser.add_parser(
-            'undelegate', 
+            'undelegate',
             help='''Undelegate Stake from an account.'''
         )
-        undelegate_stake_parser.add_argument( 
-            '--no_version_checking', 
-            action='store_true', 
-            help='''Set false to stop cli version checking''', 
-            default = False 
+        undelegate_stake_parser.add_argument(
+            '--no_version_checking',
+            action='store_true',
+            help='''Set false to stop cli version checking''',
+            default = False
         )
         undelegate_stake_parser.add_argument(
-            '--delegate_ss58key', 
+            '--delegate_ss58key',
             '--delegate_ss58',
             dest = "delegate_ss58key",
-            type = str,  
+            type = str,
             required = False,
-            help='''The ss58 address of the choosen delegate''', 
+            help='''The ss58 address of the choosen delegate''',
         )
         undelegate_stake_parser.add_argument(
-            '--all', 
-            dest="unstake_all", 
+            '--all',
+            dest="unstake_all",
             action='store_true'
         )
         undelegate_stake_parser.add_argument(
-            '--amount', 
-            dest="amount", 
-            type=float, 
+            '--amount',
+            dest="amount",
+            type=float,
             required=False
-        )        
+        )
         undelegate_stake_parser.add_argument(
-            '--no_prompt', 
-            dest='no_prompt', 
-            action='store_true', 
+            '--no_prompt',
+            dest='no_prompt',
+            action='store_true',
             help='''Set true to avoid prompting the user.''',
             default=False,
         )
         bittensor.wallet.add_args( undelegate_stake_parser )
         bittensor.subtensor.add_args( undelegate_stake_parser )
 
-    @staticmethod   
+    @staticmethod
     def check_config( config: 'bittensor.Config' ):
         # if config.subtensor.get('network') == bittensor.defaults.subtensor.network and not config.no_prompt:
         #     config.subtensor.network = Prompt.ask("Enter subtensor network", choices=bittensor.__networks__, default = bittensor.defaults.subtensor.network)
 
         if config.wallet.get('name') == bittensor.defaults.wallet.name and not config.no_prompt:
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
@@ -300,15 +300,15 @@
 
             if prev_delegates is None:
                 bittensor.__console__.print(":warning: [yellow]Could not fetch delegates history[/yellow]")
 
             if len(delegates) == 0:
                 console.print(":cross_mark: [red]There are no delegates on {}[/red]".format(subtensor.network))
                 sys.exit(1)
-            
+
             delegates.sort(key=lambda delegate: delegate.total_stake, reverse=True)
             show_delegates( delegates, prev_delegates = prev_delegates)
             delegate_index = Prompt.ask("Enter delegate index")
             config.delegate_ss58key = str(delegates[int(delegate_index)].hotkey_ss58)
             console.print("Selected: [yellow]{}[/yellow]".format(config.delegate_ss58key))
 
         # Get amount.
@@ -336,33 +336,32 @@
             try:
                 prev_delegates = subtensor.get_delegates(max(0, subtensor.block - 1200))
             except SubstrateRequestException:
                 prev_delegates = None
 
         if prev_delegates is None:
             bittensor.__console__.print(":warning: [yellow]Could not fetch delegates history[/yellow]")
-        
         show_delegates( delegates, prev_delegates = prev_delegates, width = cli.config.get('width', None) )
 
     @staticmethod
     def add_args( parser: argparse.ArgumentParser ):
         list_delegates_parser = parser.add_parser(
-            'list_delegates', 
+            'list_delegates',
             help='''List all delegates on the network'''
         )
         list_delegates_parser.add_argument(
-            '--no_prompt', 
-            dest='no_prompt', 
-            action='store_true', 
+            '--no_prompt',
+            dest='no_prompt',
+            action='store_true',
             help='''Set true to avoid prompting the user.''',
             default=False,
         )
         bittensor.subtensor.add_args( list_delegates_parser )
 
-    @staticmethod   
+    @staticmethod
     def check_config( config: 'bittensor.Config' ):
         pass
 
 
 
 class NominateCommand:
 
@@ -392,37 +391,37 @@
                 bittensor.__console__.print("Could not became a delegate on [white]{}[/white]".format(subtensor.network))
                 return
             bittensor.__console__.print("Successfully became a delegate on [white]{}[/white]".format(subtensor.network))
 
     @staticmethod
     def add_args( parser: argparse.ArgumentParser ):
         nominate_parser = parser.add_parser(
-            'nominate', 
+            'nominate',
             help='''Become a delegate on the network'''
         )
         nominate_parser.add_argument(
-            '--no_prompt', 
-            dest='no_prompt', 
-            action='store_true', 
+            '--no_prompt',
+            dest='no_prompt',
+            action='store_true',
             help='''Set true to avoid prompting the user.''',
             default=False,
         )
         bittensor.wallet.add_args( nominate_parser )
         bittensor.subtensor.add_args( nominate_parser )
 
-    @staticmethod   
+    @staticmethod
     def check_config( config: 'bittensor.Config' ):
         if config.wallet.get('name') == bittensor.defaults.wallet.name and not config.no_prompt:
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
 
         if config.wallet.get('hotkey') == bittensor.defaults.wallet.hotkey and not config.no_prompt:
             hotkey = Prompt.ask("Enter hotkey name", default = bittensor.defaults.wallet.hotkey)
             config.wallet.hotkey = str(hotkey)
-      
+
 
 class MyDelegatesCommand:
 
     @staticmethod
     def run( cli ):
         '''Delegates stake to a chain delegate.'''
         config = cli.config.copy()
@@ -453,31 +452,30 @@
             my_delegates = {} # hotkey, amount
             for delegate in delegates:
                 for coldkey_addr, staked in delegate[0].nominators:
                     if coldkey_addr == wallet.coldkeypub.ss58_address and staked.tao > 0:
                         my_delegates[ delegate[0].hotkey_ss58 ] = staked
 
             delegates.sort(key=lambda delegate: delegate[0].total_stake, reverse=True)
-            
             registered_delegate_info: Optional[DelegatesDetails] = get_delegates_details(url = bittensor.__delegates_details_url__)
             if registered_delegate_info is None:
                 bittensor.__console__.print( ':warning:[yellow]Could not get delegate info from chain.[/yellow]')
                 registered_delegate_info = {}
 
             for i, delegate in enumerate( delegates ):
                 owner_stake = next(
                     map(lambda x: x[1], # get stake
                         filter(lambda x: x[0] == delegate[0].owner_ss58, delegate[0].nominators) # filter for owner
                     ),
                     bittensor.Balance.from_rao(0) # default to 0 if no owner stake.
                 )
                 if delegate[0].hotkey_ss58 in registered_delegate_info:
-                    delegate_name = registered_delegate_info[delegate[0].hotkey_ss58]['name']
-                    delegate_url = registered_delegate_info[delegate[0].hotkey_ss58]['url']
-                    delegate_description =  registered_delegate_info[delegate[0].hotkey_ss58]['description']
+                    delegate_name = registered_delegate_info[delegate[0].hotkey_ss58].name
+                    delegate_url = registered_delegate_info[delegate[0].hotkey_ss58].url
+                    delegate_description =  registered_delegate_info[delegate[0].hotkey_ss58].description
                 else:
                     delegate_name = ''
                     delegate_url = ''
                     delegate_description = ''
 
                 if delegate[0].hotkey_ss58 in my_delegates:
                     table.add_row(
@@ -498,41 +496,40 @@
                     )
 
         bittensor.__console__.print(table)
 
     @staticmethod
     def add_args( parser: argparse.ArgumentParser ):
         delegate_stake_parser = parser.add_parser(
-            'my_delegates', 
+            'my_delegates',
             help='''Show all delegates where I am delegating a positive amount of stake'''
         )
-        delegate_stake_parser.add_argument( 
-            '--no_version_checking', 
-            action='store_true', 
-            help='''Set false to stop cli version checking''', 
-            default = False 
-        )
-        delegate_stake_parser.add_argument( 
-            '--all', 
-            action='store_true', 
-            help='''Check all coldkey wallets.''', 
-            default = False 
+        delegate_stake_parser.add_argument(
+            '--no_version_checking',
+            action='store_true',
+            help='''Set false to stop cli version checking''',
+            default = False
+        )
+        delegate_stake_parser.add_argument(
+            '--all',
+            action='store_true',
+            help='''Check all coldkey wallets.''',
+            default = False
         )
         delegate_stake_parser.add_argument(
-            '--no_prompt', 
-            dest='no_prompt', 
-            action='store_true', 
+            '--no_prompt',
+            dest='no_prompt',
+            action='store_true',
             help='''Set true to avoid prompting the user.''',
             default=False,
         )
         bittensor.wallet.add_args( delegate_stake_parser )
         bittensor.subtensor.add_args( delegate_stake_parser )
 
-    @staticmethod   
+    @staticmethod
     def check_config( config: 'bittensor.Config' ):
         if not config.get( 'all', d=None ) and config.wallet.get('name') == bittensor.defaults.wallet.name and not config.no_prompt:
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
 
 
 
-
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_cli/commands/inspect.py` & `bittensor-5.0.0/bittensor/_cli/commands/inspect.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import json
 import argparse
 import bittensor
 from tqdm import tqdm
 from rich.table import Table
@@ -128,40 +128,40 @@
                             '',
                             '',
                             str( netuid ),
                             str( neuron.hotkey ),
                             str( neuron.stake ),
                             str( bittensor.Balance.from_tao(neuron.emission) )
                         )
-               
+
         bittensor.__console__.print(table)
-            
-                
+
+
 
     @staticmethod
     def check_config( config: 'bittensor.Config' ):
         if not config.get( 'all', d=None ) and config.wallet.get('name') == bittensor.defaults.wallet.name and not config.no_prompt:
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
 
     @staticmethod
     def add_args( parser: argparse.ArgumentParser ):
         inspect_parser = parser.add_parser(
-            'inspect', 
+            'inspect',
             help='''Inspect a wallet (cold, hot) pair'''
         )
-        inspect_parser.add_argument( 
-            '--all', 
-            action='store_true', 
-            help='''Check all coldkey wallets.''', 
-            default = False 
+        inspect_parser.add_argument(
+            '--all',
+            action='store_true',
+            help='''Check all coldkey wallets.''',
+            default = False
         )
         inspect_parser.add_argument(
-            '--no_prompt', 
-            dest='no_prompt', 
-            action='store_true', 
+            '--no_prompt',
+            dest='no_prompt',
+            action='store_true',
             help='''Set true to avoid prompting the user.''',
             default=False,
         )
         inspect_parser.add_argument( '--no_version_checking', action='store_true', help='''Set false to stop cli version checking''', default = False )
         bittensor.wallet.add_args( inspect_parser )
         bittensor.subtensor.add_args( inspect_parser )
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_cli/commands/list.py` & `bittensor-5.0.0/bittensor/_cli/commands/list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import os
 import argparse
 import bittensor
 from rich import print
 from rich.tree import Tree
@@ -70,20 +70,20 @@
     @staticmethod
     def check_config( config: 'bittensor.Config' ):
         pass
 
     @staticmethod
     def add_args( parser: argparse.ArgumentParser ):
         list_parser = parser.add_parser(
-            'list', 
+            'list',
             help='''List wallets'''
         )
         list_parser.add_argument(
-            '--no_prompt', 
-            dest='no_prompt', 
-            action='store_true', 
+            '--no_prompt',
+            dest='no_prompt',
+            action='store_true',
             help='''Set true to avoid prompting the user.''',
             default=False,
         )
         list_parser.add_argument( '--no_version_checking', action='store_true', help='''Set false to stop cli version checking''', default = False )
         bittensor.wallet.add_args( list_parser )
         bittensor.subtensor.add_args( list_parser )
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_cli/commands/metagraph.py` & `bittensor-5.0.0/bittensor/_cli/commands/metagraph.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import argparse
 import bittensor
 from rich.prompt import Prompt
 from rich.table import Table
 from .utils import check_netuid_set
@@ -32,53 +32,53 @@
         console.print(":satellite: Syncing with chain: [white]{}[/white] ...".format(cli.config.subtensor.network))
         metagraph: bittensor.metagraph = subtensor.metagraph( netuid = cli.config.netuid )
         metagraph.save()
         difficulty = subtensor.difficulty( cli.config.netuid )
         subnet_emission = bittensor.Balance.from_tao(subtensor.get_emission_value_by_subnet(cli.config.netuid))
         total_issuance = bittensor.Balance.from_tao(subtensor.total_issuance())
 
-        TABLE_DATA = [] 
+        TABLE_DATA = []
         total_stake = 0.0
         total_rank = 0.0
         total_validator_trust = 0.0
         total_trust = 0.0
         total_consensus = 0.0
         total_incentive = 0.0
         total_dividends = 0.0
-        total_emission = 0  
+        total_emission = 0
         for uid in metagraph.uids:
             neuron = metagraph.neurons[uid]
             ep = metagraph.axons[uid]
             row = [
-                str(neuron.uid), 
+                str(neuron.uid),
                 '{:.5f}'.format( metagraph.total_stake[uid]),
                 '{:.5f}'.format( metagraph.ranks[uid]),
-                '{:.5f}'.format( metagraph.trust[uid]), 
+                '{:.5f}'.format( metagraph.trust[uid]),
                 '{:.5f}'.format( metagraph.consensus[uid]),
                 '{:.5f}'.format( metagraph.incentive[uid]),
                 '{:.5f}'.format( metagraph.dividends[uid]),
                 '{}'.format( int(metagraph.emission[uid] * 1000000000)),
                 '{:.5f}'.format( metagraph.validator_trust[uid]),
                 '*' if metagraph.validator_permit[uid] else '',
                 str((metagraph.block.item() - metagraph.last_update[uid].item())),
                 str( metagraph.active[uid].item() ),
-                ep.ip + ':' + str(ep.port) if ep.is_serving else '[yellow]none[/yellow]', 
+                ep.ip + ':' + str(ep.port) if ep.is_serving else '[yellow]none[/yellow]',
                 ep.hotkey[:10],
                 ep.coldkey[:10]
             ]
             total_stake += metagraph.total_stake[uid]
             total_rank += metagraph.ranks[uid]
             total_validator_trust += metagraph.validator_trust[uid]
             total_trust += metagraph.trust[uid]
             total_consensus += metagraph.consensus[uid]
             total_incentive += metagraph.incentive[uid]
             total_dividends += metagraph.dividends[uid]
             total_emission += int(metagraph.emission[uid] * 1000000000)
             TABLE_DATA.append(row)
-        total_neurons = len(metagraph.uids)                
+        total_neurons = len(metagraph.uids)
         table = Table(show_footer=False)
         table.title = (
             "[white]Metagraph: net: {}:{}, block: {}, N: {}/{}, stake: {}, issuance: {}, difficulty: {}".format(subtensor.network, metagraph.netuid, metagraph.block.item(), sum(metagraph.active.tolist()), metagraph.n.item(), bittensor.Balance.from_tao(total_stake), total_issuance, difficulty )
         )
         table.add_column("[overline white]UID",  str(total_neurons), footer_style = "overline white", style='yellow')
         table.add_column("[overline white]STAKE(\u03C4)", '\u03C4{:.5f}'.format(total_stake), footer_style = "overline white", justify='right', style='green', no_wrap=True)
         table.add_column("[overline white]RANK", '{:.5f}'.format(total_rank), footer_style = "overline white", justify='right', style='green', no_wrap=True)
@@ -87,15 +87,15 @@
         table.add_column("[overline white]INCENTIVE", '{:.5f}'.format(total_incentive), footer_style = "overline white", justify='right', style='green', no_wrap=True)
         table.add_column("[overline white]DIVIDENDS", '{:.5f}'.format(total_dividends), footer_style = "overline white", justify='right', style='green', no_wrap=True)
         table.add_column("[overline white]EMISSION(\u03C1)", '\u03C1{}'.format(int(total_emission)), footer_style = "overline white", justify='right', style='green', no_wrap=True)
         table.add_column("[overline white]VTRUST", '{:.5f}'.format(total_validator_trust), footer_style = "overline white", justify='right', style='green', no_wrap=True)
         table.add_column("[overline white]VAL", justify='right', style='green', no_wrap=True)
         table.add_column("[overline white]UPDATED", justify='right', no_wrap=True)
         table.add_column("[overline white]ACTIVE", justify='right', style='green', no_wrap=True)
-        table.add_column("[overline white]AXON", justify='left', style='dim blue', no_wrap=True) 
+        table.add_column("[overline white]AXON", justify='left', style='dim blue', no_wrap=True)
         table.add_column("[overline white]HOTKEY", style='dim blue', no_wrap=False)
         table.add_column("[overline white]COLDKEY", style='dim purple', no_wrap=False)
         table.show_footer = True
 
         for row in TABLE_DATA:
             table.add_row(*row)
         table.box = None
@@ -106,26 +106,26 @@
     @staticmethod
     def check_config( config: 'bittensor.Config' ):
         check_netuid_set( config, subtensor = bittensor.subtensor( config = config ) )
 
     @staticmethod
     def add_args( parser: argparse.ArgumentParser ):
         metagraph_parser = parser.add_parser(
-            'metagraph', 
+            'metagraph',
             help='''Metagraph commands'''
         )
         metagraph_parser.add_argument(
-            '--netuid', 
-            dest='netuid', 
+            '--netuid',
+            dest='netuid',
             type=int,
             help='''Set the netuid to get the metagraph of''',
             default=False,
         )
         metagraph_parser.add_argument(
-            '--no_prompt', 
-            dest='no_prompt', 
-            action='store_true', 
+            '--no_prompt',
+            dest='no_prompt',
+            action='store_true',
             help='''Set true to avoid prompting the user.''',
             default=False,
         )
         metagraph_parser.add_argument( '--no_version_checking', action='store_true', help='''Set false to stop cli version checking''', default = False )
         bittensor.subtensor.add_args( metagraph_parser )
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_cli/commands/misc.py` & `bittensor-5.0.0/bittensor/_cli/commands/misc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import os
 import sys
 import argparse
 import bittensor
 from typing import List
@@ -43,23 +43,23 @@
         #     model = Prompt.ask('Enter miner name', choices = list(bittensor.neurons.__text_neurons__.keys()), default = 'core_server')
         #     config.model = model
 
     @staticmethod
     def add_args( parser: argparse.ArgumentParser ):
         pass
         # help_parser = parser.add_parser(
-        #     'help', 
+        #     'help',
         #     add_help=False,
         #     help='''Displays the help '''
         # )
         # help_parser.add_argument(
-        #     '--model', 
-        #     type=str, 
-        #     choices= list(bittensor.neurons.__text_neurons__.keys()), 
-        #     default='None', 
+        #     '--model',
+        #     type=str,
+        #     choices= list(bittensor.neurons.__text_neurons__.keys()),
+        #     default='None',
         # )
         # help_parser.add_argument( '--no_version_checking', action='store_true', help='''Set false to stop cli version checking''', default = False )
         # bittensor.subtensor.add_args( help_parser )
 
 class UpdateCommand:
     @staticmethod
     def run (cli):
@@ -72,22 +72,22 @@
         if not config.no_prompt:
             answer = Prompt.ask('This will update the local bittensor package', choices = ['Y','N'], default = 'Y')
             config.answer = answer
 
     @staticmethod
     def add_args( parser: argparse.ArgumentParser ):
         update_parser = parser.add_parser(
-            'update', 
+            'update',
             add_help=False,
             help='''Update bittensor '''
         )
         update_parser.add_argument(
-            '--no_prompt', 
-            dest='no_prompt', 
-            action='store_true', 
+            '--no_prompt',
+            dest='no_prompt',
+            action='store_true',
             help='''Set true to skip prompt from update.''',
             default=False,
         )
         update_parser.add_argument( '--no_version_checking', action='store_true', help='''Set false to stop cli version checking''', default = False )
         bittensor.subtensor.add_args( update_parser )
 
 class ListSubnetsCommand:
@@ -127,32 +127,31 @@
         #table.add_column("[overline white]BATCH SIZE", style='white')
         #table.add_column("[overline white]SEQ_LEN", style='white')
         table.add_column("[overline white]TEMPO", style='white', justify='center')
         #table.add_column("[overline white]MODALITY", style='white')
         table.add_column("[overline white]CON_REQ", style='white', justify='center')
         table.add_column("[overline white]EMISSION", style='white', justify='center') # sums to 100%
         table.add_column("[overline white]BURN(\u03C4)", style='white')
-        
+
         for row in rows:
             table.add_row(*row)
 
         bittensor.__console__.print(table)
 
     @staticmethod
     def check_config( config: 'bittensor.Config' ):
         pass
-    
+
     @staticmethod
     def add_args( parser: argparse.ArgumentParser ):
         list_subnets_parser = parser.add_parser(
-            'list_subnets', 
+            'list_subnets',
             help='''List all subnets on the network'''
         )
         list_subnets_parser.add_argument(
-            '--no_prompt', 
-            dest='no_prompt', 
-            action='store_true', 
+            '--no_prompt',
+            dest='no_prompt',
+            action='store_true',
             help='''Set true to avoid prompting the user.''',
             default=False,
         )
         bittensor.subtensor.add_args( list_subnets_parser )
-
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_cli/commands/overview.py` & `bittensor-5.0.0/bittensor/_cli/commands/overview.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import argparse
 import bittensor
 from tqdm import tqdm
 from fuzzywuzzy import fuzz
 from rich.align import Align
@@ -35,15 +35,15 @@
         """
         console = bittensor.__console__
         wallet = bittensor.wallet( config = cli.config )
         subtensor: 'bittensor.Subtensor' = bittensor.subtensor( config = cli.config )
 
         all_hotkeys = []
         total_balance = bittensor.Balance(0)
-        
+
         # We are printing for every coldkey.
         if cli.config.get( 'all', d=None ):
             cold_wallets = get_coldkey_wallets_for_path(cli.config.wallet.path)
             for cold_wallet in tqdm(cold_wallets, desc="Pulling balances"):
                 if cold_wallet.coldkeypub_file.exists_on_device() and not cold_wallet.coldkeypub_file.is_encrypted():
                     total_balance = total_balance + subtensor.get_balance( cold_wallet.coldkeypub.ss58_address )
             all_hotkeys = get_all_wallets_for_path( cli.config.wallet.path )
@@ -68,25 +68,25 @@
                 all_hotkeys = [hotkey for hotkey in all_hotkeys if hotkey.hotkey_str not in cli.config.hotkeys]
 
         # Check we have keys to display.
         if len(all_hotkeys) == 0:
             console.print("[red]No wallets found.[/red]")
             return
 
-        # Pull neuron info for all keys.            
+        # Pull neuron info for all keys.
         neurons: Dict[str, List[bittensor.NeuronInfoLite, bittensor.Wallet]] = {}
         block = subtensor.block
 
         netuids = subtensor.get_all_subnet_netuids()
         if cli.config.netuid != []:
             netuids = [netuid for netuid in netuids if netuid in cli.config.netuid]
         for netuid in netuids:
             neurons[str(netuid)] = []
         netuids_copy = netuids.copy()
-        
+
         with console.status(":satellite: Syncing with chain: [white]{}[/white] ...".format(cli.config.subtensor.get('network', bittensor.defaults.subtensor.network))):
             for netuid in tqdm(netuids_copy, desc="Checking each subnet"):
                 all_neurons: List[bittensor.NeuronInfoLite] = subtensor.neurons_lite( netuid = netuid )
                 # Map the hotkeys to uids
                 hotkey_to_neurons = {n.hotkey: n.uid for n in all_neurons}
                 for hot_wallet in all_hotkeys:
                     uid = hotkey_to_neurons.get(hot_wallet.hotkey.ss58_address)
@@ -113,22 +113,22 @@
         # Generate rows per netuid
         hotkeys_seen = set()
         total_neurons = 0
         total_stake = 0.0
         for netuid in netuids:
             subnet_tempo = subtensor.tempo(netuid=netuid)
             last_subnet = netuid == netuids[-1]
-            TABLE_DATA = []  
+            TABLE_DATA = []
             total_rank = 0.0
             total_trust = 0.0
             total_consensus = 0.0
             total_validator_trust = 0.0
             total_incentive = 0.0
             total_dividends = 0.0
-            total_emission = 0   
+            total_emission = 0
 
             for nn, hotwallet in neurons[str(netuid)]:
                 nn: bittensor.NeuronInfoLite
                 uid = nn.uid
                 active = nn.active
                 stake = nn.total_stake.tao
                 rank = nn.rank
@@ -139,30 +139,30 @@
                 dividends = nn.dividends
                 emission = int(nn.emission / (subnet_tempo + 1) * 1e9)
                 last_update = int(block -  nn.last_update)
                 validator_permit = nn.validator_permit
                 row = [
                     hotwallet.name,
                     hotwallet.hotkey_str,
-                    str(uid), 
-                    str(active), 
+                    str(uid),
+                    str(active),
                     '{:.5f}'.format(stake),
-                    '{:.5f}'.format(rank), 
-                    '{:.5f}'.format(trust), 
+                    '{:.5f}'.format(rank),
+                    '{:.5f}'.format(trust),
                     '{:.5f}'.format(consensus),
                     '{:.5f}'.format(incentive),
                     '{:.5f}'.format(dividends),
                     '{:_}'.format(emission),
                     '{:.5f}'.format(validator_trust),
                     '*' if validator_permit else '',
                     str(last_update),
-                    bittensor.utils.networking.int_to_ip( nn.axon_info.ip) + ':' + str(nn.axon_info.port) if nn.axon_info.port != 0 else '[yellow]none[/yellow]', 
+                    bittensor.utils.networking.int_to_ip( nn.axon_info.ip) + ':' + str(nn.axon_info.port) if nn.axon_info.port != 0 else '[yellow]none[/yellow]',
                     nn.hotkey
                 ]
-               
+
                 total_rank += rank
                 total_trust += trust
                 total_consensus += consensus
                 total_incentive += incentive
                 total_dividends += dividends
                 total_emission += emission
                 total_validator_trust += validator_trust
@@ -197,15 +197,15 @@
             table.add_column("[overline white]CONSENSUS", '{:.5f}'.format(total_consensus), footer_style = "overline white", justify='right', style='green', no_wrap=True)
             table.add_column("[overline white]INCENTIVE", '{:.5f}'.format(total_incentive), footer_style = "overline white", justify='right', style='green', no_wrap=True)
             table.add_column("[overline white]DIVIDENDS", '{:.5f}'.format(total_dividends), footer_style = "overline white", justify='right', style='green', no_wrap=True)
             table.add_column("[overline white]EMISSION(\u03C1)", '\u03C1{:_}'.format(total_emission), footer_style = "overline white", justify='right', style='green', no_wrap=True)
             table.add_column("[overline white]VTRUST", '{:.5f}'.format(total_validator_trust), footer_style="overline white", justify='right', style='green', no_wrap=True)
             table.add_column("[overline white]VPERMIT", justify='right', no_wrap=True)
             table.add_column("[overline white]UPDATED", justify='right', no_wrap=True)
-            table.add_column("[overline white]AXON", justify='left', style='dim blue', no_wrap=True) 
+            table.add_column("[overline white]AXON", justify='left', style='dim blue', no_wrap=True)
             table.add_column("[overline white]HOTKEY_SS58", style='dim blue', no_wrap=False)
             table.show_footer = True
 
             sort_by: Optional[str] = cli.config.get('sort_by', None)
             sort_order: Optional[str] = cli.config.get('sort_order', None)
 
             if sort_by is not None and sort_by != "":
@@ -217,19 +217,19 @@
                     # Fuzzy match the column name. Default to the first column.
                     column_name = column.header.lower().replace('[overline white]', '')
                     match_ratio = fuzz.ratio(sort_by.lower(), column_name)
                     # Finds the best matching column
                     if  match_ratio > highest_matching_ratio:
                         highest_matching_ratio = match_ratio
                         column_to_sort_by = index
-                
+
                 if sort_order.lower() in { 'desc', 'descending', 'reverse'}:
                     # Sort descending if the sort_order matches desc, descending, or reverse
                     sort_descending = True
-                
+
                 def overview_sort_function(row):
                     data = row[column_to_sort_by]
                     # Try to convert to number if possible
                     try:
                         data = float(data)
                     except ValueError:
                         pass
@@ -250,41 +250,41 @@
 
         # Print the entire table/grid
         console.print(grid, width=cli.config.get('width', None))
 
     @staticmethod
     def add_args( parser: argparse.ArgumentParser ):
         overview_parser = parser.add_parser(
-            'overview', 
+            'overview',
             help='''Show registered account overview.'''
         )
         overview_parser.add_argument(
-            '--no_prompt', 
-            dest='no_prompt', 
-            action='store_true', 
+            '--no_prompt',
+            dest='no_prompt',
+            action='store_true',
             help='''Set true to avoid prompting the user.''',
             default=False,
         )
         overview_parser.add_argument(
-            '--all', 
-            dest='all', 
-            action='store_true', 
+            '--all',
+            dest='all',
+            action='store_true',
             help='''View overview for all wallets.''',
             default=False,
         )
         overview_parser.add_argument(
-            '--width', 
-            dest='width', 
+            '--width',
+            dest='width',
             action='store',
-            type=int, 
+            type=int,
             help='''Set the output width of the overview. Defaults to automatic width from terminal.''',
             default=None,
         )
         overview_parser.add_argument(
-            '--sort_by', 
+            '--sort_by',
             '--wallet.sort_by',
             dest='sort_by',
             required=False,
             action='store',
             default="",
             type=str,
             help='''Sort the hotkeys by the specified column title (e.g. name, uid, axon).'''
@@ -316,30 +316,29 @@
             '--wallet.all_hotkeys',
             required=False,
             action='store_true',
             default=False,
             help='''To specify all hotkeys. Specifying hotkeys will exclude them from this all.'''
         )
         overview_parser.add_argument(
-            '--netuid', 
-            dest='netuid', 
+            '--netuid',
+            dest='netuid',
             type=int,
             nargs='*',
             help='''Set the netuid(s) to filter by.''',
             default=[],
         )
-        overview_parser.add_argument( '--no_version_checking', action='store_true', help='''Set false to stop cli version checking''', default = False )  
+        overview_parser.add_argument( '--no_version_checking', action='store_true', help='''Set false to stop cli version checking''', default = False )
         bittensor.wallet.add_args( overview_parser )
         bittensor.subtensor.add_args( overview_parser )
 
-    @staticmethod   
+    @staticmethod
     def check_config( config: 'bittensor.Config' ):
         if config.wallet.get('name') == bittensor.defaults.wallet.name  and not config.no_prompt and not config.get( 'all', d=None ):
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
 
         if config.netuid != []:
             if not isinstance(config.netuid, list):
                 config.netuid = [int(config.netuid)]
             else:
                 config.netuid = [int(netuid) for netuid in config.netuid]
-
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_cli/commands/register.py` & `bittensor-5.0.0/bittensor/_cli/commands/register.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import sys
 import argparse
 import bittensor
 from rich.prompt import Prompt, Confirm
 from .utils import check_netuid_set, check_for_cuda_reg_config
@@ -49,41 +49,41 @@
             log_verbose = cli.config.subtensor.register.get('verbose', bittensor.defaults.subtensor.register.verbose),
         )
 
 
     @staticmethod
     def add_args( parser: argparse.ArgumentParser ):
         register_parser = parser.add_parser(
-            'register', 
+            'register',
             help='''Register a wallet to a network.'''
         )
-        register_parser.add_argument( 
-            '--no_version_checking', 
-            action='store_true', 
-            help='''Set false to stop cli version checking''', 
-            default = False 
+        register_parser.add_argument(
+            '--no_version_checking',
+            action='store_true',
+            help='''Set false to stop cli version checking''',
+            default = False
         )
         register_parser.add_argument(
-            '--no_prompt', 
-            dest='no_prompt', 
-            action='store_true', 
+            '--no_prompt',
+            dest='no_prompt',
+            action='store_true',
             help='''Set true to avoid prompting the user.''',
             default=False,
         )
         register_parser.add_argument(
             '--netuid',
             type=int,
             help='netuid for subnet to serve this neuron on',
             default=argparse.SUPPRESS,
         )
 
         bittensor.wallet.add_args( register_parser )
         bittensor.subtensor.add_args( register_parser )
 
-    @staticmethod   
+    @staticmethod
     def check_config( config: 'bittensor.Config' ):
         check_netuid_set( config, subtensor = bittensor.subtensor( config = config ) )
 
         if config.wallet.get('name') == bittensor.defaults.wallet.name and not config.no_prompt:
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
 
@@ -115,59 +115,58 @@
         if balance < current_recycle:
             bittensor.__console__.print(f"[red]Insufficient balance {balance} to register neuron. Current recycle is {current_recycle} TAO[/red]")
             sys.exit(1)
 
         if not cli.config.no_prompt:
             if Confirm.ask(f"Your balance is: [bold green]{balance}[/bold green]\nThe cost to register by recycle is [bold red]{current_recycle}[/bold red]\nDo you want to continue?", default = False) == False:
                 sys.exit(1)
-        
+
         subtensor.burned_register(
             wallet = wallet,
             netuid = cli.config.netuid,
             prompt = not cli.config.no_prompt
         )
 
 
     @staticmethod
     def add_args( parser: argparse.ArgumentParser ):
         recycle_register_parser = parser.add_parser(
-            'recycle_register', 
+            'recycle_register',
             help='''Register a wallet to a network.'''
         )
-        recycle_register_parser.add_argument( 
-            '--no_version_checking', 
-            action='store_true', 
-            help='''Set false to stop cli version checking''', 
-            default = False 
+        recycle_register_parser.add_argument(
+            '--no_version_checking',
+            action='store_true',
+            help='''Set false to stop cli version checking''',
+            default = False
         )
         recycle_register_parser.add_argument(
-            '--no_prompt', 
-            dest='no_prompt', 
-            action='store_true', 
+            '--no_prompt',
+            dest='no_prompt',
+            action='store_true',
             help='''Set true to avoid prompting the user.''',
             default=False,
         )
         recycle_register_parser.add_argument(
             '--netuid',
             type=int,
             help='netuid for subnet to serve this neuron on',
             default=argparse.SUPPRESS,
         )
 
         bittensor.wallet.add_args( recycle_register_parser )
         bittensor.subtensor.add_args( recycle_register_parser )
 
-    @staticmethod   
+    @staticmethod
     def check_config( config: 'bittensor.Config' ):
         if config.subtensor.get('network') == bittensor.defaults.subtensor.network and not config.no_prompt:
             config.subtensor.network = Prompt.ask("Enter subtensor network", choices=bittensor.__networks__, default = bittensor.defaults.subtensor.network)
 
         check_netuid_set( config, subtensor = bittensor.subtensor( config = config ) )
 
         if config.wallet.get('name') == bittensor.defaults.wallet.name and not config.no_prompt:
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
 
         if config.wallet.get('hotkey') == bittensor.defaults.wallet.hotkey and not config.no_prompt:
             hotkey = Prompt.ask("Enter hotkey name", default = bittensor.defaults.wallet.hotkey)
             config.wallet.hotkey = str(hotkey)
-
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_cli/commands/stake.py` & `bittensor-5.0.0/bittensor/_cli/commands/stake.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import sys
 import argparse
 import bittensor
 from tqdm import tqdm
 from rich.prompt import Confirm
@@ -31,15 +31,15 @@
     @staticmethod
     def run( cli ):
         r""" Stake token of amount to hotkey(s).
         """
         config = cli.config.copy()
         wallet = bittensor.wallet( config = config )
         subtensor: bittensor.Subtensor = bittensor.subtensor( config = config )
-        
+
         # Get the hotkey_names (if any) and the hotkey_ss58s.
         hotkeys_to_stake_to: List[Tuple[Optional[str], str]] = []
         if config.get('all_hotkeys'):
             # Stake to all hotkeys.
             all_hotkeys: List[bittensor.wallet] = get_hotkey_wallets_for_wallet( wallet = wallet )
             # Get the hotkeys to exclude. (d)efault to no exclusions.
             hotkeys_to_exclude: List[str] = cli.config.get('hotkeys', d=[])
@@ -71,18 +71,18 @@
                 wallet_ = bittensor.wallet( config = config, hotkey = hotkey_ss58_or_name )
                 hotkeys_to_stake_to = [ (wallet_.hotkey_str, wallet_.hotkey.ss58_address ) ]
         else:
             # Only config.wallet.hotkey is specified.
             #  so we stake to that single hotkey.
             assert config.wallet.hotkey is not None
             hotkeys_to_stake_to = [ (None, bittensor.wallet( config = config ).hotkey.ss58_address) ]
-        
+
         # Get coldkey balance
         wallet_balance: Balance = subtensor.get_balance( wallet.coldkeypub.ss58_address )
-        final_hotkeys: List[Tuple[str, str]] = [] 
+        final_hotkeys: List[Tuple[str, str]] = []
         final_amounts: List[Union[float, Balance]] = []
         for hotkey in tqdm(hotkeys_to_stake_to):
             hotkey: Tuple[Optional[str], str] # (hotkey_name (or None), hotkey_ss58)
             if not subtensor.is_hotkey_registered_any( hotkey_ss58 = hotkey[1] ):
                 # Hotkey is not registered.
                 if (len(hotkeys_to_stake_to) == 1):
                     # Only one hotkey, error
@@ -102,15 +102,15 @@
 
                 # If the max_stake is greater than the current wallet balance, stake the entire balance.
                 stake_amount_tao: float = min(stake_amount_tao, wallet_balance.tao)
                 if stake_amount_tao <= 0.00001: # Threshold because of fees, might create a loop otherwise
                     # Skip hotkey if max_stake is less than current stake.
                     continue
                 wallet_balance = Balance.from_tao(wallet_balance.tao - stake_amount_tao)
-            
+
                 if wallet_balance.tao < 0:
                     # No more balance to stake.
                     break
 
             final_amounts.append(stake_amount_tao)
             final_hotkeys.append(hotkey) # add both the name and the ss58 address.
 
@@ -123,32 +123,32 @@
         if not config.no_prompt:
             if not Confirm.ask(f"Do you want to stake to the following keys from {wallet.name}:\n" + \
                     "".join([
                         f"    [bold white]- {hotkey[0] + ':' if hotkey[0] else ''}{hotkey[1]}: {f'{amount} {bittensor.__tao_symbol__}' if amount else 'All'}[/bold white]\n" for hotkey, amount in zip(final_hotkeys, final_amounts)
                     ])
                 ):
                 return None
-        
+
         if len(final_hotkeys) == 1:
             # do regular stake
             return subtensor.add_stake( wallet=wallet, hotkey_ss58 = final_hotkeys[0][1], amount = None if config.get('stake_all') else final_amounts[0], wait_for_inclusion = True, prompt = not config.no_prompt )
 
         subtensor.add_stake_multiple( wallet = wallet, hotkey_ss58s=[hotkey_ss58 for _, hotkey_ss58 in final_hotkeys], amounts =  None if config.get('stake_all') else final_amounts, wait_for_inclusion = True, prompt = False )
 
 
-    @classmethod   
+    @classmethod
     def check_config( cls, config: 'bittensor.Config' ):
         if config.wallet.get('name') == bittensor.defaults.wallet.name and not config.no_prompt:
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
 
         if config.wallet.get('hotkey') == bittensor.defaults.wallet.hotkey and not config.no_prompt and not config.get('all_hotkeys') and not config.get('hotkeys'):
             hotkey = Prompt.ask("Enter hotkey name", default = bittensor.defaults.wallet.hotkey)
             config.wallet.hotkey = str(hotkey)
-                    
+
         # Get amount.
         if not config.get('amount') and not config.get('stake_all') and not config.get('max_stake'):
             if not Confirm.ask("Stake all Tao from account: [bold]'{}'[/bold]?".format(config.wallet.get('name', bittensor.defaults.wallet.name))):
                 amount = Prompt.ask("Enter Tao amount to stake")
                 try:
                     config.amount = float(amount)
                 except ValueError:
@@ -156,53 +156,53 @@
                     sys.exit()
             else:
                 config.stake_all = True
 
     @classmethod
     def add_args( cls, parser: argparse.ArgumentParser ):
         stake_parser = parser.add_parser(
-            'stake', 
+            'stake',
             help='''Stake to your hotkey accounts.'''
         )
-        stake_parser.add_argument( 
-            '--no_version_checking', 
-            action='store_true', 
-            help='''Set false to stop cli version checking''', 
-            default = False 
+        stake_parser.add_argument(
+            '--no_version_checking',
+            action='store_true',
+            help='''Set false to stop cli version checking''',
+            default = False
         )
         stake_parser.add_argument(
-            '--all', 
-            dest="stake_all", 
+            '--all',
+            dest="stake_all",
             action='store_true'
         )
         stake_parser.add_argument(
-            '--uid', 
-            dest="uid", 
-            type=int, 
+            '--uid',
+            dest="uid",
+            type=int,
             required=False
         )
         stake_parser.add_argument(
-            '--amount', 
-            dest="amount", 
-            type=float, 
+            '--amount',
+            dest="amount",
+            type=float,
             required=False
-        )        
+        )
         stake_parser.add_argument(
-            '--max_stake', 
+            '--max_stake',
             dest="max_stake",
             type=float,
             required=False,
             action='store',
             default=None,
             help='''Specify the maximum amount of Tao to have staked in each hotkey.'''
         )
         stake_parser.add_argument(
-            '--no_prompt', 
-            dest='no_prompt', 
-            action='store_true', 
+            '--no_prompt',
+            dest='no_prompt',
+            action='store_true',
             help='''Set true to avoid prompting the user.''',
             default=False,
         )
         stake_parser.add_argument(
             '--hotkeys',
             '--exclude_hotkeys',
             '--wallet.hotkeys',
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_cli/commands/transfer.py` & `bittensor-5.0.0/bittensor/_cli/commands/transfer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 # Copyright © 2022 Opentensor Foundation
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import sys
 import argparse
 import bittensor
 from rich.prompt import Prompt
 console = bittensor.__console__
@@ -48,15 +48,15 @@
         # Get current balance and print to user.
         if not config.no_prompt:
             wallet = bittensor.wallet( config )
             subtensor = bittensor.subtensor( config )
             with bittensor.__console__.status(":satellite: Checking Balance..."):
                 account_balance = subtensor.get_balance( wallet.coldkeypub.ss58_address )
                 bittensor.__console__.print("Balance: [green]{}[/green]".format(account_balance))
-                    
+
         # Get amount.
         if not config.get('amount'):
             if not config.no_prompt:
                 amount = Prompt.ask("Enter TAO amount to transfer")
                 try:
                     config.amount = float(amount)
                 except ValueError:
@@ -65,32 +65,32 @@
             else:
                 console.print(":cross_mark:[red] Invalid TAO amount[/red] [bold white]{}[/bold white]".format(amount))
                 sys.exit(1)
 
     @staticmethod
     def add_args( parser: argparse.ArgumentParser ):
         transfer_parser = parser.add_parser(
-            'transfer', 
+            'transfer',
             help='''Transfer Tao between accounts.'''
         )
         transfer_parser.add_argument( '--no_version_checking', action='store_true', help='''Set false to stop cli version checking''', default = False )
         transfer_parser.add_argument(
-            '--dest', 
-            dest="dest", 
-            type=str, 
+            '--dest',
+            dest="dest",
+            type=str,
             required=False
         )
         transfer_parser.add_argument(
-            '--amount', 
-            dest="amount", 
-            type=float, 
+            '--amount',
+            dest="amount",
+            type=float,
             required=False
         )
         transfer_parser.add_argument(
-            '--no_prompt', 
-            dest='no_prompt', 
-            action='store_true', 
+            '--no_prompt',
+            dest='no_prompt',
+            action='store_true',
             help='''Set true to avoid prompting the user.''',
             default=False,
         )
         bittensor.wallet.add_args( transfer_parser )
         bittensor.subtensor.add_args( transfer_parser )
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_cli/commands/unstake.py` & `bittensor-5.0.0/bittensor/_cli/commands/unstake.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import sys
 import bittensor
 from tqdm import tqdm
 from rich.prompt import Confirm, Prompt
 from bittensor.utils.balance import Balance
 from typing import List, Union, Optional, Dict, Tuple
 from .utils import get_hotkey_wallets_for_wallet
 console = bittensor.__console__
 
 class UnStakeCommand:
 
-    @classmethod   
-    def check_config( cls, config: 'bittensor.Config' ):        
+    @classmethod
+    def check_config( cls, config: 'bittensor.Config' ):
         if config.wallet.get('name') == bittensor.defaults.wallet.name and not config.no_prompt:
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
 
         if not config.get('hotkey_ss58address') and config.wallet.get('hotkey') == bittensor.defaults.wallet.hotkey and not config.no_prompt and not config.get('all_hotkeys') and not config.get('hotkeys'):
             hotkey = Prompt.ask("Enter hotkey name", default = bittensor.defaults.wallet.hotkey)
             config.wallet.hotkey = str(hotkey)
-                    
+
         # Get amount.
         if not config.get('hotkey_ss58address') and not config.get('amount') and not config.get('unstake_all') and not config.get('max_stake'):
             hotkeys: str = ''
             if config.get('all_hotkeys'):
                 hotkeys = "all hotkeys"
             elif config.get('hotkeys'):
                 hotkeys = str(config.hotkeys).replace('[', '').replace(']', '')
@@ -55,54 +55,54 @@
                     sys.exit()
             else:
                 config.unstake_all = True
 
     @staticmethod
     def add_args( command_parser ):
         unstake_parser = command_parser.add_parser(
-            'unstake', 
+            'unstake',
             help='''Unstake from hotkey accounts.'''
         )
-        unstake_parser.add_argument( 
-            '--no_version_checking', 
-            action='store_true', 
-            help='''Set false to stop cli version checking''', 
-            default = False 
+        unstake_parser.add_argument(
+            '--no_version_checking',
+            action='store_true',
+            help='''Set false to stop cli version checking''',
+            default = False
         )
         unstake_parser.add_argument(
-            '--all', 
-            dest="unstake_all", 
+            '--all',
+            dest="unstake_all",
             action='store_true',
             default=False,
         )
         unstake_parser.add_argument(
-            '--amount', 
-            dest="amount", 
-            type=float, 
+            '--amount',
+            dest="amount",
+            type=float,
             required=False
         )
         unstake_parser.add_argument(
-            '--hotkey_ss58address', 
-            dest="hotkey_ss58address", 
-            type=str, 
+            '--hotkey_ss58address',
+            dest="hotkey_ss58address",
+            type=str,
             required=False
         )
         unstake_parser.add_argument(
-            '--max_stake', 
+            '--max_stake',
             dest="max_stake",
             type=float,
             required=False,
             action='store',
             default=None,
             help='''Specify the maximum amount of Tao to have staked in each hotkey.'''
         )
         unstake_parser.add_argument(
-            '--no_prompt', 
-            dest='no_prompt', 
-            action='store_true', 
+            '--no_prompt',
+            dest='no_prompt',
+            action='store_true',
             help='''Set true to avoid prompting the user.''',
             default=False,
         )
         unstake_parser.add_argument(
             '--hotkeys',
             '--exclude_hotkeys',
             '--wallet.hotkeys',
@@ -124,32 +124,32 @@
         )
         bittensor.wallet.add_args( unstake_parser )
         bittensor.subtensor.add_args( unstake_parser )
 
     @staticmethod
     def run( cli ):
         r""" Unstake token of amount from hotkey(s).
-        """        
+        """
         config = cli.config.copy()
         wallet = bittensor.wallet( config = config )
         subtensor: bittensor.Subtensor = bittensor.subtensor( config = cli.config )
-        
+
         # Get the hotkey_names (if any) and the hotkey_ss58s.
         hotkeys_to_unstake_from: List[Tuple[Optional[str], str]] = []
         if cli.config.get('hotkey_ss58address'):
             # Stake to specific hotkey.
             hotkeys_to_unstake_from = [(None, cli.config.get('hotkey_ss58address'))]
         elif cli.config.get('all_hotkeys'):
             # Stake to all hotkeys.
             all_hotkeys: List[bittensor.wallet] = get_hotkey_wallets_for_wallet( wallet = wallet )
             # Get the hotkeys to exclude. (d)efault to no exclusions.
             hotkeys_to_exclude: List[str] = cli.config.get('hotkeys', d=[])
             # Exclude hotkeys that are specified.
             hotkeys_to_unstake_from = [
-                (wallet.hotkey_str, wallet.hotkey.ss58_address) for wallet in all_hotkeys 
+                (wallet.hotkey_str, wallet.hotkey.ss58_address) for wallet in all_hotkeys
                     if wallet.hotkey_str not in hotkeys_to_exclude
             ] # definitely wallets
 
         elif cli.config.get('hotkeys'):
             # Stake to specific hotkeys.
             for hotkey_ss58_or_hotkey_name in cli.config.get('hotkeys'):
                 if bittensor.utils.is_valid_ss58_address( hotkey_ss58_or_hotkey_name ):
@@ -171,37 +171,37 @@
                 wallet_ = bittensor.wallet( config = cli.config, hotkey = hotkey_ss58_or_name )
                 hotkeys_to_unstake_from = [ (wallet_.hotkey_str, wallet_.hotkey.ss58_address ) ]
         else:
             # Only cli.config.wallet.hotkey is specified.
             #  so we stake to that single hotkey.
             assert cli.config.wallet.hotkey is not None
             hotkeys_to_unstake_from = [ (None, bittensor.wallet( config = cli.config ).hotkey.ss58_address) ]
-        
-        final_hotkeys: List[Tuple[str, str]] = [] 
+
+        final_hotkeys: List[Tuple[str, str]] = []
         final_amounts: List[Union[float, Balance]] = []
         for hotkey in tqdm(hotkeys_to_unstake_from):
             hotkey: Tuple[Optional[str], str] # (hotkey_name (or None), hotkey_ss58)
             unstake_amount_tao: float = cli.config.get('amount') # The amount specified to unstake.
             hotkey_stake: Balance = subtensor.get_stake_for_coldkey_and_hotkey( hotkey_ss58 = hotkey[1], coldkey_ss58 = wallet.coldkeypub.ss58_address )
             if unstake_amount_tao == None:
                 unstake_amount_tao = hotkey_stake.tao
             if cli.config.get('max_stake'):
                 # Get the current stake of the hotkey from this coldkey.
-                unstake_amount_tao: float = hotkey_stake.tao - cli.config.get('max_stake')   
-                cli.config.amount = unstake_amount_tao  
+                unstake_amount_tao: float = hotkey_stake.tao - cli.config.get('max_stake')
+                cli.config.amount = unstake_amount_tao
                 if unstake_amount_tao < 0:
                     # Skip if max_stake is greater than current stake.
                     continue
             else:
                 if unstake_amount_tao is not None:
                     # There is a specified amount to unstake.
                     if unstake_amount_tao > hotkey_stake.tao:
                         # Skip if the specified amount is greater than the current stake.
                         continue
-            
+
             final_amounts.append(unstake_amount_tao)
             final_hotkeys.append(hotkey) # add both the name and the ss58 address.
 
         if len(final_hotkeys) == 0:
             # No hotkeys to unstake from.
             bittensor.__console__.print("Not enough stake to unstake from any hotkeys or max_stake is more than current stake.")
             return None
@@ -210,20 +210,20 @@
         if not cli.config.no_prompt:
             if not Confirm.ask(f"Do you want to unstake from the following keys to {wallet.name}:\n" + \
                     "".join([
                         f"    [bold white]- {hotkey[0] + ':' if hotkey[0] else ''}{hotkey[1]}: {f'{amount} {bittensor.__tao_symbol__}' if amount else 'All'}[/bold white]\n" for hotkey, amount in zip(final_hotkeys, final_amounts)
                     ])
                 ):
                 return None
-        
+
         if len(final_hotkeys) == 1:
             # do regular unstake
-            return subtensor.unstake( 
-                wallet=wallet, 
-                hotkey_ss58 = final_hotkeys[0][1], 
-                amount = None if cli.config.get('unstake_all') else final_amounts[0], 
-                wait_for_inclusion = True, 
-                prompt = not cli.config.no_prompt 
+            return subtensor.unstake(
+                wallet=wallet,
+                hotkey_ss58 = final_hotkeys[0][1],
+                amount = None if cli.config.get('unstake_all') else final_amounts[0],
+                wait_for_inclusion = True,
+                prompt = not cli.config.no_prompt
             )
 
         subtensor.unstake_multiple( wallet = wallet, hotkey_ss58s=[hotkey_ss58 for _, hotkey_ss58 in final_hotkeys], amounts =  None if cli.config.get('unstake_all') else final_amounts, wait_for_inclusion = True, prompt = False )
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_cli/commands/utils.py` & `bittensor-5.0.0/bittensor/_cli/commands/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import sys
 import os
 import torch
 import bittensor
 from typing import List, Dict, Any, Optional
 from rich.prompt import Confirm, Prompt, PromptBase
 import requests
 from dataclasses import dataclass
 console = bittensor.__console__
 
 class IntListPrompt(PromptBase):
     """ Prompt for a list of integers. """
-    
+
     def check_choice( self, value: str ) -> bool:
         assert self.choices is not None
         # check if value is a valid choice or all the values in a list of ints are valid choices
         return value == "All" or \
             value in self.choices or \
             all( val.strip() in self.choices for val in value.replace(',', ' ').split( ))
 
@@ -48,15 +48,15 @@
         if config.get('netuid', 'notset') == 'notset':
             if not config.no_prompt:
                 netuid = IntListPrompt.ask("Enter netuid", choices=all_netuids, default=str(all_netuids[0]))
             else:
                 netuid = str(bittensor.defaults.netuid) if not allow_none else 'None'
         else:
             netuid = config.netuid
-            
+
         if isinstance(netuid, str) and netuid.lower() in ['none'] and allow_none:
             config.netuid = None
         else:
             try:
                 config.netuid = int(netuid)
             except ValueError:
                 raise ValueError('netuid must be an integer or "None" (if applicable)')
@@ -90,15 +90,15 @@
                         dev_id = [int(dev_id.strip()) for dev_id in dev_id.replace(',', ' ').split()]
                     except ValueError:
                         console.log(":cross_mark:[red]Invalid GPU device[/red] [bold white]{}[/bold white]\nAvailable CUDA devices:{}".format(dev_id, choices_str))
                         sys.exit(1)
                 config.subtensor.register.cuda.dev_id = dev_id
         else:
             # flag was not set, use default value.
-            if config.subtensor.register.cuda.get('use_cuda') is None: 
+            if config.subtensor.register.cuda.get('use_cuda') is None:
                 config.subtensor.register.cuda.use_cuda = bittensor.defaults.subtensor.register.cuda.use_cuda
 
 def get_hotkey_wallets_for_wallet( wallet ) -> List['bittensor.wallet']:
     hotkey_wallets = []
     hotkeys_path = wallet.path + '/' + wallet.name + '/hotkeys'
     try:
         hotkey_files = next(os.walk(os.path.expanduser(hotkeys_path)))[2]
@@ -144,23 +144,22 @@
             url=json['url'],
             description=json['description'],
             signature=json['signature'],
         )
 
 def _get_delegates_details_from_github(requests_get, url: str) -> Dict[str, DelegatesDetails]:
     response = requests_get(url)
-    
 
     if response.status_code == 200:
         all_delegates: Dict[str, Any] = response.json()
         all_delegates_details = {}
         for delegate_hotkey, delegates_details in all_delegates.items():
             all_delegates_details[delegate_hotkey] = DelegatesDetails.from_json(delegates_details)
         return all_delegates_details
     else:
         return {}
-    
-def get_delegates_details(url: str) -> Optional[Dict[str, DelegatesDetails]]: 
+
+def get_delegates_details(url: str) -> Optional[Dict[str, DelegatesDetails]]:
     try:
         return _get_delegates_details_from_github(requests.get, url)
     except Exception:
         return None # Fail silently
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_cli/commands/wallets.py` & `bittensor-5.0.0/bittensor/_cli/commands/wallets.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import argparse
 import bittensor
 import os
 import sys
 from rich.prompt import Prompt
@@ -32,54 +32,53 @@
         json_password: Optional[str] = None
         if cli.config.get('json'):
             file_name: str = cli.config.get('json')
             if not os.path.exists(file_name) or not os.path.isfile(file_name):
                 raise ValueError('File {} does not exist'.format(file_name))
             with open(cli.config.get('json'), 'r') as f:
                 json_str = f.read()
-            
+
             # Password can be "", assume if None
             json_password = cli.config.get('json_password', "")
 
         wallet.regenerate_coldkey( mnemonic = cli.config.mnemonic, seed = cli.config.seed, json = (json_str, json_password), use_password = cli.config.use_password, overwrite = cli.config.overwrite_coldkey )
-   
+
     @staticmethod
     def check_config( config: 'bittensor.Config' ):
         if config.wallet.get('name') == bittensor.defaults.wallet.name  and not config.no_prompt:
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
-        
         if config.mnemonic == None and config.get( 'seed', d=None ) == None and config.get( 'json', d=None ) == None:
             prompt_answer = Prompt.ask("Enter mnemonic, seed, or json file location")
             if prompt_answer.startswith("0x"):
                 config.seed = prompt_answer
             elif len(prompt_answer.split(" ")) > 1:
                 config.mnemonic = prompt_answer
             else:
                 config.json = prompt_answer
 
         if config.get( 'json', d=None ) and config.get( 'json_password', d=None ) == None:
             config.json_password = Prompt.ask("Enter json backup password", password=True)
-    
+
     @staticmethod
     def add_args( parser: argparse.ArgumentParser ):
         regen_coldkey_parser = parser.add_parser(
             'regen_coldkey',
             help='''Regenerates a coldkey from a passed value'''
         )
         regen_coldkey_parser.add_argument( '--no_version_checking', action='store_true', help='''Set false to stop cli version checking''', default = False )
         regen_coldkey_parser.add_argument(
-            "--mnemonic", 
-            required=False, 
-            nargs="+", 
+            "--mnemonic",
+            required=False,
+            nargs="+",
             help='Mnemonic used to regen your key i.e. horse cart dog ...'
         )
         regen_coldkey_parser.add_argument(
-            "--seed", 
-            required=False,  
+            "--seed",
+            required=False,
             default=None,
             help='Seed hex string used to regen your key i.e. 0x1234...'
         )
         regen_coldkey_parser.add_argument(
             "--json",
             required=False,
             default=None,
@@ -88,30 +87,30 @@
         regen_coldkey_parser.add_argument(
             "--json_password",
             required=False,
             default=None,
             help='''Password to decrypt the json file.'''
         )
         regen_coldkey_parser.add_argument(
-            '--use_password', 
-            dest='use_password', 
-            action='store_true', 
+            '--use_password',
+            dest='use_password',
+            action='store_true',
             help='''Set true to protect the generated bittensor key with a password.''',
             default=True,
         )
         regen_coldkey_parser.add_argument(
-            '--no_password', 
-            dest='use_password', 
-            action='store_false', 
+            '--no_password',
+            dest='use_password',
+            action='store_false',
             help='''Set off protects the generated bittensor key with a password.''',
         )
         regen_coldkey_parser.add_argument(
-            '--no_prompt', 
-            dest='no_prompt', 
-            action='store_true', 
+            '--no_prompt',
+            dest='no_prompt',
+            action='store_true',
             help='''Set true to avoid prompting the user.''',
             default=False,
         )
         regen_coldkey_parser.add_argument(
             '--overwrite_coldkey',
             default=False,
             action='store_false',
@@ -122,15 +121,15 @@
 
 
 class RegenColdkeypubCommand:
     def run ( cli ):
         r""" Creates a new coldkeypub under this wallet."""
         wallet = bittensor.wallet(config = cli.config)
         wallet.regenerate_coldkeypub( ss58_address=cli.config.get('ss58_address'), public_key=cli.config.get('public_key_hex'), overwrite = cli.config.overwrite_coldkeypub )
-    
+
     @staticmethod
     def check_config( config: 'bittensor.Config' ):
         if config.wallet.get('name') == bittensor.defaults.wallet.name  and not config.no_prompt:
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
         if config.ss58_address == None and config.public_key_hex == None:
             prompt_answer = Prompt.ask("Enter the ss58_address or the public key in hex")
@@ -146,35 +145,35 @@
         regen_coldkeypub_parser = parser.add_parser(
             'regen_coldkeypub',
             help='''Regenerates a coldkeypub from the public part of the coldkey.'''
         )
         regen_coldkeypub_parser.add_argument( '--no_version_checking', action='store_true', help='''Set false to stop cli version checking''', default = False )
         regen_coldkeypub_parser.add_argument(
             "--public_key",
-            "--pubkey", 
+            "--pubkey",
             dest="public_key_hex",
             required=False,
-            default=None, 
+            default=None,
             type=str,
             help='The public key (in hex) of the coldkey to regen e.g. 0x1234 ...'
         )
         regen_coldkeypub_parser.add_argument(
-            "--ss58_address", 
+            "--ss58_address",
             "--addr",
             "--ss58",
             dest="ss58_address",
-            required=False,  
+            required=False,
             default=None,
             type=str,
             help='The ss58 address of the coldkey to regen e.g. 5ABCD ...'
         )
         regen_coldkeypub_parser.add_argument(
-            '--no_prompt', 
-            dest='no_prompt', 
-            action='store_true', 
+            '--no_prompt',
+            dest='no_prompt',
+            action='store_true',
             help='''Set true to avoid prompting the user.''',
             default=False,
         )
         regen_coldkeypub_parser.add_argument(
             '--overwrite_coldkeypub',
             default=False,
             action='store_true',
@@ -193,30 +192,29 @@
         json_password: Optional[str] = None
         if cli.config.get('json'):
             file_name: str = cli.config.get('json')
             if not os.path.exists(file_name) or not os.path.isfile(file_name):
                 raise ValueError('File {} does not exist'.format(file_name))
             with open(cli.config.get('json'), 'r') as f:
                 json_str = f.read()
-            
+
             # Password can be "", assume if None
             json_password = cli.config.get('json_password', "")
 
         wallet.regenerate_hotkey( mnemonic = cli.config.mnemonic, seed=cli.config.seed, json = (json_str, json_password), use_password = cli.config.use_password, overwrite = cli.config.overwrite_hotkey)
-    
+
     @staticmethod
     def check_config( config: 'bittensor.Config' ):
         if config.wallet.get('name') == bittensor.defaults.wallet.name  and not config.no_prompt:
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
 
         if config.wallet.get('hotkey') == bittensor.defaults.wallet.hotkey and not config.no_prompt:
             hotkey = Prompt.ask("Enter hotkey name", default = bittensor.defaults.wallet.hotkey)
             config.wallet.hotkey = str(hotkey)
-        
         if config.mnemonic == None and config.get( 'seed', d=None ) == None and config.get( 'json', d=None ) == None:
             prompt_answer = Prompt.ask("Enter mnemonic, seed, or json file location")
             if prompt_answer.startswith("0x"):
                 config.seed = prompt_answer
             elif len(prompt_answer.split(" ")) > 1:
                 config.mnemonic = prompt_answer
             else:
@@ -229,22 +227,22 @@
     def add_args( parser: argparse.ArgumentParser ):
         regen_hotkey_parser = parser.add_parser(
             'regen_hotkey',
             help='''Regenerates a hotkey from a passed mnemonic'''
         )
         regen_hotkey_parser.add_argument( '--no_version_checking', action='store_true', help='''Set false to stop cli version checking''', default = False )
         regen_hotkey_parser.add_argument(
-            "--mnemonic", 
-            required=False, 
-            nargs="+", 
+            "--mnemonic",
+            required=False,
+            nargs="+",
             help='Mnemonic used to regen your key i.e. horse cart dog ...'
         )
         regen_hotkey_parser.add_argument(
-            "--seed", 
-            required=False,  
+            "--seed",
+            required=False,
             default=None,
             help='Seed hex string used to regen your key i.e. 0x1234...'
         )
         regen_hotkey_parser.add_argument(
             "--json",
             required=False,
             default=None,
@@ -253,51 +251,51 @@
         regen_hotkey_parser.add_argument(
             "--json_password",
             required=False,
             default=None,
             help='''Password to decrypt the json file.'''
         )
         regen_hotkey_parser.add_argument(
-            '--use_password', 
-            dest='use_password', 
-            action='store_true', 
+            '--use_password',
+            dest='use_password',
+            action='store_true',
             help='''Set true to protect the generated bittensor key with a password.''',
             default=False
         )
         regen_hotkey_parser.add_argument(
-            '--no_password', 
-            dest='use_password', 
-            action='store_false', 
+            '--no_password',
+            dest='use_password',
+            action='store_false',
             help='''Set off protects the generated bittensor key with a password.'''
         )
         regen_hotkey_parser.add_argument(
-            '--no_prompt', 
-            dest='no_prompt', 
-            action='store_true', 
+            '--no_prompt',
+            dest='no_prompt',
+            action='store_true',
             help='''Set true to avoid prompting the user.''',
             default=False,
         )
         regen_hotkey_parser.add_argument(
             '--overwrite_hotkey',
             dest='overwrite_hotkey',
             action='store_true',
             default=False,
             help='''Overwrite the old hotkey with the newly generated hotkey'''
         )
         bittensor.wallet.add_args( regen_hotkey_parser )
         bittensor.subtensor.add_args( regen_hotkey_parser )
-    
+
 
 
 class NewHotkeyCommand:
 
     def run( cli ):
         """ Creates a new hotke under this wallet."""
         wallet = bittensor.wallet(config = cli.config)
-        wallet.create_new_hotkey( n_words = cli.config.n_words, use_password = cli.config.use_password, overwrite = cli.config.overwrite_hotkey)   
+        wallet.create_new_hotkey( n_words = cli.config.n_words, use_password = cli.config.use_password, overwrite = cli.config.overwrite_hotkey)
 
     @staticmethod
     def check_config( config: 'bittensor.Config' ):
         if config.wallet.get('name') == bittensor.defaults.wallet.name  and not config.no_prompt:
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
 
@@ -305,93 +303,93 @@
             hotkey = Prompt.ask("Enter hotkey name", default = bittensor.defaults.wallet.hotkey)
             config.wallet.hotkey = str(hotkey)
 
     @staticmethod
     def add_args( parser: argparse.ArgumentParser ):
         new_hotkey_parser = parser.add_parser( 'new_hotkey',  help='''Creates a new hotkey (for running a miner) under the specified path.''')
         new_hotkey_parser.add_argument( '--no_version_checking', action='store_true', help='''Set false to stop cli version checking''', default = False )
-        new_hotkey_parser.add_argument( '--n_words', 
-            type=int, 
-            choices=[12,15,18,21,24], 
-            default=12, 
+        new_hotkey_parser.add_argument( '--n_words',
+            type=int,
+            choices=[12,15,18,21,24],
+            default=12,
             help='''The number of words representing the mnemonic. i.e. horse cart dog ... x 24'''
         )
         new_hotkey_parser.add_argument(
-            '--use_password', 
-            dest='use_password', 
-            action='store_true', 
+            '--use_password',
+            dest='use_password',
+            action='store_true',
             help='''Set true to protect the generated bittensor key with a password.''',
             default=False
         )
         new_hotkey_parser.add_argument(
-            '--no_password', 
-            dest='use_password', 
-            action='store_false', 
+            '--no_password',
+            dest='use_password',
+            action='store_false',
             help='''Set off protects the generated bittensor key with a password.'''
         )
         new_hotkey_parser.add_argument(
-            '--no_prompt', 
-            dest='no_prompt', 
-            action='store_true', 
+            '--no_prompt',
+            dest='no_prompt',
+            action='store_true',
             help='''Set true to avoid prompting the user.''',
             default=False,
         )
         new_hotkey_parser.add_argument(
             '--overwrite_hotkey',
             action='store_false',
             default=False,
             help='''Overwrite the old hotkey with the newly generated hotkey'''
         )
-        bittensor.wallet.add_args( new_hotkey_parser ) 
+        bittensor.wallet.add_args( new_hotkey_parser )
         bittensor.subtensor.add_args( new_hotkey_parser )
 
 
 class NewColdkeyCommand:
     def run ( cli ):
         r""" Creates a new coldkey under this wallet."""
         wallet = bittensor.wallet(config = cli.config)
-        wallet.create_new_coldkey( n_words = cli.config.n_words, use_password = cli.config.use_password, overwrite = cli.config.overwrite_coldkey)   
+        wallet.create_new_coldkey( n_words = cli.config.n_words, use_password = cli.config.use_password, overwrite = cli.config.overwrite_coldkey)
 
     @staticmethod
     def check_config( config: 'bittensor.Config' ):
         if config.wallet.get('name') == bittensor.defaults.wallet.name  and not config.no_prompt:
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
 
     @staticmethod
     def add_args( parser: argparse.ArgumentParser ):
         new_coldkey_parser = parser.add_parser(
-            'new_coldkey', 
+            'new_coldkey',
             help='''Creates a new coldkey (for containing balance) under the specified path. '''
         )
         new_coldkey_parser.add_argument( '--no_version_checking', action='store_true', help='''Set false to stop cli version checking''', default = False )
         new_coldkey_parser.add_argument(
-            '--n_words', 
-            type=int, 
-            choices=[12,15,18,21,24], 
-            default=12, 
+            '--n_words',
+            type=int,
+            choices=[12,15,18,21,24],
+            default=12,
             help='''The number of words representing the mnemonic. i.e. horse cart dog ... x 24'''
         )
         new_coldkey_parser.add_argument(
-            '--use_password', 
-            dest='use_password', 
-            action='store_true', 
+            '--use_password',
+            dest='use_password',
+            action='store_true',
             help='''Set true to protect the generated bittensor key with a password.''',
             default=True,
         )
         new_coldkey_parser.add_argument(
-            '--no_password', 
-            dest='use_password', 
-            action='store_false', 
+            '--no_password',
+            dest='use_password',
+            action='store_false',
             help='''Set off protects the generated bittensor key with a password.'''
         )
         new_coldkey_parser.add_argument(
-            '--no_prompt', 
-            dest='no_prompt', 
-            action='store_true', 
+            '--no_prompt',
+            dest='no_prompt',
+            action='store_true',
             help='''Set true to avoid prompting the user.''',
             default=False,
         )
         new_coldkey_parser.add_argument(
             '--overwrite_coldkey',
             action='store_false',
             default=False,
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_config/__init__.py` & `bittensor-5.0.0/bittensor/_config/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
 Create and init the config class, which manages the config of different bittensor modules.
 """
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 # Copyright © 2022 Opentensor Foundation
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import os
 import sys
 from argparse import ArgumentParser, Namespace
 from typing import List, Optional
 
 import bittensor
 import yaml
 from loguru import logger
 
 from . import config_impl
 
 logger = logger.opt(colors=True)
-    
+
 class config:
     """
     Create and init the config class, which manages the config of different bittensor modules.
     """
     class InvalidConfigFile(Exception):
         """ In place of YAMLError
         """
@@ -79,15 +79,15 @@
             config_file_path = None
 
         # Parse args not strict
         params = cls.__parse_args__(args=args, parser=parser, strict=False)
 
         # 2. Optionally check for --strict, if stict we will parse the args strictly.
         strict = params.strict
-                        
+
         if config_file_path != None:
             config_file_path = os.path.expanduser(config_file_path)
             try:
                 with open(config_file_path) as f:
                     params_config = yaml.safe_load(f)
                     print('Loading config defaults from: {}'.format(config_file_path))
                     parser.set_defaults(**params_config)
@@ -95,26 +95,26 @@
                 print('Error in loading: {} using default parser settings'.format(e))
 
         # 2. Continue with loading in params.
         params = cls.__parse_args__(args=args, parser=parser, strict=strict)
 
         _config = config_impl.Config()
 
-        # Splits params on dot syntax i.e neuron.axon_port            
+        # Splits params on dot syntax i.e neuron.axon_port
         for arg_key, arg_val in params.__dict__.items():
             split_keys = arg_key.split('.')
             head = _config
             keys = split_keys
             while len(keys) > 1:
                 if hasattr(head, keys[0]):
-                    head = getattr(head, keys[0])  
-                    keys = keys[1:]   
+                    head = getattr(head, keys[0])
+                    keys = keys[1:]
                 else:
                     head[keys[0]] = config_impl.Config()
-                    head = head[keys[0]] 
+                    head = head[keys[0]]
                     keys = keys[1:]
             if len(keys) == 1:
                 head[keys[0]] = arg_val
 
         return _config
 
     @staticmethod
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_config/config_impl.py` & `bittensor-5.0.0/bittensor/_config/config_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
 Implementation of the config class, which manages the config of different bittensor modules.
 """
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 # Copyright © 2022 Opentensor Foundation
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import yaml
 import json
 import pandas
 import bittensor
 from munch import Munch
@@ -33,15 +33,15 @@
     def __init__(self, loaded_config = None ):
         super().__init__()
         if loaded_config:
             raise NotImplementedError('Function load_from_relative_path is not fully implemented.')
 
     def __repr__(self) -> str:
         return self.__str__()
-    
+
     def __str__(self) -> str:
         return "\n" + yaml.dump(self.toDict())
 
     def to_string(self, items) -> str:
         """ Get string from items
         """
         return "\n" + yaml.dump(items.toDict())
@@ -71,23 +71,23 @@
             prometheus_info.info(formatted_info)
         except ValueError:
             # The user called this function twice in the same session.
             # TODO(const): need a way of distinguishing the various config items.
             bittensor.__console__.print("The config has already been added to prometheus.", highlight=True)
 
     def to_defaults(self):
-        try: 
+        try:
             if 'axon' in self.keys():
                 bittensor.defaults.axon.port = self.axon.port
                 bittensor.defaults.axon.ip = self.axon.ip
                 bittensor.defaults.axon.external_port = self.axon.external_port
                 bittensor.defaults.axon.external_ip = self.axon.external_ip
                 bittensor.defaults.axon.max_workers = self.axon.max_workers
                 bittensor.defaults.axon.maximum_concurrent_rpcs = self.axon.maximum_concurrent_rpcs
-            
+
             if 'dataset' in self.keys():
                 bittensor.defaults.dataset.batch_size = self.dataset.batch_size
                 bittensor.defaults.dataset.block_size = self.dataset.block_size
                 bittensor.defaults.dataset.num_batches = self.dataset.num_batches
                 bittensor.defaults.dataset.num_workers = self.dataset.num_workers
                 bittensor.defaults.dataset.dataset_names = self.dataset.dataset_names
                 bittensor.defaults.dataset.data_dir = self.dataset.data_dir
@@ -95,28 +95,28 @@
                 bittensor.defaults.dataset.max_datasets = self.dataset.max_datasets
 
             if  'logging' in self.keys():
                 bittensor.defaults.logging.debug = self.logging.debug
                 bittensor.defaults.logging.trace = self.logging.trace
                 bittensor.defaults.logging.record_log = self.logging.record_log
                 bittensor.defaults.logging.logging_dir = self.logging.logging_dir
-            
+
             if 'subtensor' in self.keys():
                 bittensor.defaults.subtensor.network = self.subtensor.network
                 bittensor.defaults.subtensor.chain_endpoint = self.subtensor.chain_endpoint
-            
+
             if 'threadpool' in self.keys():
                 bittensor.defaults.threadpool.max_workers = self.threadpool.max_workers
-                bittensor.defaults.threadpool.maxsize = self.threadpool.maxsize 
+                bittensor.defaults.threadpool.maxsize = self.threadpool.maxsize
 
             if 'wallet' in self.keys():
                 bittensor.defaults.wallet.name = self.wallet.name
                 bittensor.defaults.wallet.hotkey = self.wallet.hotkey
                 bittensor.defaults.wallet.path = self.wallet.path
-            
+
             if 'wandb' in self.keys():
                 bittensor.defaults.wandb.name = self.wandb.name
                 bittensor.defaults.wandb.project = self.wandb.project
                 bittensor.defaults.wandb.tags = self.wandb.tags
                 bittensor.defaults.wandb.run_group = self.wandb.run_group
                 bittensor.defaults.wandb.directory = self.wandb.directory
                 bittensor.defaults.wandb.offline = self.wandb.offline
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_dataset/__init__.py` & `bittensor-5.0.0/bittensor/_dataset/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,19 +26,19 @@
 
 import bittensor
 from . import dataset_impl
 from . import dataset_mock
 
 class dataset:
     """ Factory class for the GenesisTextDataset class or the mocked GenesisTextDataset
-    The GenesisTextDataset downloads text data from the bittensor mountain dataset. 
+    The GenesisTextDataset downloads text data from the bittensor mountain dataset.
     The class makes http requests to bittensor's IPFS backend server which contains the full dataset.
     By default, the GenesisTextDataset class will return a fully functioning pytorch dataloader.
 
-    Examples:: 
+    Examples::
             >>> dataset = bittensor.dataset(batch_size = 10, block_size=20)
             >>> # data.shape[batch_size, block_size]
             >>> data = next(dataset)
     """
     def __new__(
             cls,
             config: 'bittensor.config' = None,
@@ -50,35 +50,35 @@
             no_tokenizer: bool=None,
             num_batches: int = None,
             _mock:bool=None,
             dataset_name: list = None, # For backwards compatibility
         ):
         r""" Create and init the GenesisTextDataset class, which handles dataloading from ipfs.
             Args:
-                config (:obj:`bittensor.Config`, `optional`): 
+                config (:obj:`bittensor.Config`, `optional`):
                     bittensor.dataset.config()
                 block_size (:obj:`int`, `optional`):
                     Number of text items to pull for each example.
                 batch_size (:obj:`int`, `optional`):
                     Batch size.
                 num_workers (:obj:`int`, `optional`):
                     Number of workers for data loader.
                 dataset_names (:obj:`list`,`str`, `optional`):
-                    Which datasets to use (ArXiv, BookCorpus2, Books3, DMMathematics, EnronEmails, EuroParl, 
+                    Which datasets to use (ArXiv, BookCorpus2, Books3, DMMathematics, EnronEmails, EuroParl,
                     Gutenberg_PG, HackerNews, NIHExPorter, OpenSubtitles, PhilPapers, UbuntuIRC, YoutubeSubtitles)).
                 save_dataset (:obj:`bool`, `optional`):
                     Save the downloaded dataset or not.
                 no_tokenizer (:obj:`bool`, `optional`):
                     To return non-tokenized text (EXPERIMENTAL, DO NOT USE)
                 num_batches (:obj:`int`, `optional`):
                     The number of batches of data to prepare for the dataloader.
                 _mock (:obj:`bool`, `optional`):
-                    For testing, if true the dataset if filled with fake text data.  
-        """   
-        if config == None: 
+                    For testing, if true the dataset if filled with fake text data.
+        """
+        if config == None:
             config = dataset.config()
         config = copy.deepcopy( config )
         config.dataset.block_size = block_size if block_size != None else config.dataset.block_size
         config.dataset.batch_size = batch_size if batch_size != None else config.dataset.batch_size
         config.dataset.num_workers = num_workers if num_workers != None else config.dataset.num_workers
         config.dataset.dataset_names = dataset_names if dataset_names != None else config.dataset.dataset_names
         config.dataset.save_dataset = save_dataset if save_dataset != None else config.dataset.save_dataset
@@ -118,15 +118,15 @@
 
     @classmethod
     def mock(cls):
         return dataset( _mock = True, dataset_names = ['Books3'])
 
     @classmethod
     def config(cls) -> 'bittensor.Config':
-        """ Get config from the argument parser 
+        """ Get config from the argument parser
             Return: bittensor.config object
         """
         parser = argparse.ArgumentParser()
         dataset.add_args( parser )
         return bittensor.config( parser )
 
     @classmethod
@@ -147,24 +147,24 @@
             parser.add_argument('--' + prefix_str + 'dataset.num_batches', type=int, help='The number of data to download each time(measured by the number of batches).', default=bittensor.defaults.dataset.num_batches)
             parser.add_argument('--' + prefix_str + 'dataset._mock', action='store_true', help='To turn on dataset mocking for testing purposes.', default=False)
 
         except argparse.ArgumentError:
             # re-parsing arguments.
             pass
 
-    @classmethod   
+    @classmethod
     def help(cls):
         """ Print help to stdout
         """
         parser = argparse.ArgumentParser()
         cls.add_args( parser )
         print (cls.__new__.__doc__)
         parser.print_help()
 
-    @classmethod   
+    @classmethod
     def add_defaults(cls, defaults):
         """ Adds parser defaults to object from enviroment variables.
         """
         defaults.dataset = bittensor.Config()
         defaults.dataset.batch_size = os.getenv('BT_DATASET_BATCH_SIZE') if os.getenv('BT_DATASET_BATCH_SIZE') != None else 10
         defaults.dataset.block_size = os.getenv('BT_DATASET_BLOCK_SIZE') if os.getenv('BT_DATASET_BLOCK_SIZE') != None else 20
         defaults.dataset.num_workers = os.getenv('BT_DATASET_NUM_WORKERS') if os.getenv('BT_DATASET_NUM_WORKERS') != None else 0
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_dataset/dataset_impl.py` & `bittensor-5.0.0/bittensor/_dataset/dataset_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,22 +40,22 @@
 logger = logger.opt(colors=True)
 
 
 class Dataset:
     """ Implementation for the dataset class, which handles dataloading from ipfs
     """
     def __init__(self):
-        
+
         # Used to retrieve directory contentx
-        self.dataset_dir = 'http://global.ipfs.opentensor.ai/api/v0/cat' 
+        self.dataset_dir = 'http://global.ipfs.opentensor.ai/api/v0/cat'
         self.text_dir = 'http://global.ipfs.opentensor.ai/api/v0/object/get'
         self.mountain_hash = 'QmSdDg6V9dgpdAFtActs75Qfc36qJtm9y8a7yrQ1rHm7ZX'
         # Used when current corpus has been exhausted
         self.refresh_corpus = False
-        
+
 
     @staticmethod
     def requests_retry_session(
             retries=1,
             backoff_factor=0.5,
             status_forcelist=(104, 500, 502, 504),
             session=None,
@@ -85,27 +85,27 @@
         session.mount('https://', adapter)
         return session
 
     def get_ipfs_directory(self, address: str, file_meta: dict, action: str = 'post', timeout : int = 180):
         r"""Connects to IPFS gateway and retrieves directory.
         Args:
             address: (:type:`str`, required):
-                The target address of the request. 
+                The target address of the request.
             params: (:type:`tuple`, optional):
                 The arguments of the request. eg. (('arg', dataset_hash),)
             action: (:type:`str`, optional):
                 POST or GET.
             timeout: (:type:`int`, optional):
-                Timeout for getting the server's response. 
+                Timeout for getting the server's response.
         Returns:
             dict: A dictionary of the files inside of the genesis_datasets and their hashes.
         """
         session = requests.Session()
         session.params.update((('arg', file_meta['Hash']), ))
-        
+
         try:
             if action == 'get':
                 response = self.requests_retry_session(session=session).get(address, timeout=timeout)
             elif action == 'post':
                 response = self.requests_retry_session(session=session).post(address, timeout=timeout)
 
         except Exception as E:
@@ -119,26 +119,26 @@
         """
 
     def __getitem__(self, idx):
         """ Returns the next batch from the dataset.
         """
 
 class GenesisTextDataset( Dataset ):
-    """ One kind of dataset that caters for the data from ipfs 
+    """ One kind of dataset that caters for the data from ipfs
     """
     def __init__(
         self,
         block_size,
         batch_size,
         num_workers,
         dataset_names,
         data_dir,
         save_dataset,
         max_datasets,
-        no_tokenizer, 
+        no_tokenizer,
         num_batches,
     ):
         super().__init__()
         self.block_size = block_size
         self.batch_size = batch_size
         self.num_workers = num_workers
         self.tokenizer = bittensor.tokenizer( version = bittensor.__version__ )
@@ -170,15 +170,15 @@
 
         # Used to refresh corpus if we've exhausted the whole dataset
         self.refresh_corpus = True
 
         self.build_hash_table()
 
         os.makedirs(os.path.expanduser(data_dir), exist_ok=True)
-            
+
         self.data_queue = ThreadQueue(
             producer_target = self.reserve_multiple_data,
             producer_arg = (self.num_batches, ),
             buffer_size = 1
         )
 
     def __del__(self):
@@ -188,18 +188,18 @@
         self.data_queue.close()
 
     def get_folder_size(self, folder):
         r""" Get the size (in byte) of a folder inside the data_dir.
         Args:
             folder (str):
                 The name of the folder
-        
+
         Returns:
             total_size (int):
-                The memory size of the folder (in byte). 
+                The memory size of the folder (in byte).
         """
         total_size = 0
         full_path = os.path.expanduser(os.path.join(self.data_dir, folder))
         for dirpath, dirnames, filenames in os.walk(full_path):
             for f in filenames:
                 fp = os.path.join(dirpath, f)
                 # skip if it is symbolic link
@@ -211,102 +211,102 @@
     def load_hash(self, file_meta):
         r""" Load a hash from disk.
         Args:
             file_meta (dict of str: int):
                 Specify the details of the dataset in the format of {'Name': , 'Hash':}.
 
         Returns:
-            text (str): 
-                The text in the file.                
+            text (str):
+                The text in the file.
         """
 
         full_path = os.path.expanduser(os.path.join(self.data_dir, file_meta['Folder'], file_meta['Hash']))
         if os.path.exists(full_path):
             try:
                 with open(full_path, mode='r') as f:
                     text = f.read()
 
                 logger.success("Loaded from disk:".ljust(20) + "<blue>{}</blue>".format(file_meta['Name']))
             except Exception:
                 logger.success("Could not load from disk:".ljust(20) + "<blue>{}</blue>".format(file_meta['Name']))
                 pass
 
             return text
-        
+
         return None
 
     def save_hash(self, file_meta, text):
         r""" Save a hash to disk.
         Args:
             file_meta (dict of str: int):
                 Specify the details of the dataset in the format of {'Name': , 'Hash':}.
-            text (str): 
+            text (str):
                 The string to save to the file.
-        
+
         Returns:
             text (str):
-                The text in the file.                
+                The text in the file.
         """
         folder_path = os.path.expanduser(os.path.join(self.data_dir, file_meta['Folder']))
         full_path = os.path.expanduser(os.path.join(self.data_dir, file_meta['Folder'], file_meta['Hash']))
         if not os.path.exists(folder_path):
             os.makedirs(folder_path)
         try:
             with open(full_path, mode = 'w+') as f:
                 f.write(text)
                 logger.success("Saved:".ljust(20) + "<blue>{}</blue>".format(file_meta['Name']))
             return True
-        
+
         except Exception as E:
             logger.warning("Save failed:".ljust(20) + "<blue>{}</blue>".format(file_meta['Name']))
             return False
 
     def get_text(self, file_meta):
         r""" Either load a file from disk or download it from IPFS
         Args:
             file_meta (dict of str: int):
                 Specify the details of the file in the format of {'Name': , 'Hash':}.
 
         Return:
             text (str):
-                The text that we get from the file (from disk or IPFS).     
+                The text that we get from the file (from disk or IPFS).
         """
         text = None
         response = self.get_ipfs_directory(self.text_dir, file_meta)
         if (response != None) and (response.status_code == 200):
             try:
                 text = json.loads(response.text)['Data']
             except json.decoder.JSONDecodeError:
                 text = response.text
 
             self.IPFS_fails = 0
-            
+
             if self.save_dataset and self.dataset_hashes[file_meta['Folder']]['Size'] < self.backup_dataset_cap_size:
                 self.save_hash( file_meta, text )
                 self.dataset_hashes[file_meta['Folder']]['Size'] += file_meta['Size']
-            
+
         else:
             logger.warning("Failed to get text".ljust(20) + "<blue>{}</blue>".format(file_meta['Name']))
             self.IPFS_fails += 1
-            
-        return text 
+
+        return text
 
     def get_dataset(self , file_meta):
         r""" Either load a dataset, which is a list of hashes, from disk or download it from IPFS
         Args:
             file_meta (dict of str: int):
                 Specify the details of the dataset in the format of {'Name': , 'Hash':}.
 
         Return:
             hashes (list):
-                The hashes from the dataset downloaded from disk or IPFS.     
+                The hashes from the dataset downloaded from disk or IPFS.
         """
         # --- Load text from path
         logger.success( f"Getting dataset: {file_meta['Name']}" )
-        
+
         hashes = self.load_hash(file_meta)
 
         if hashes != None:
             hashes = json.loads(hashes)
 
         # --- If couldnt load from path, download text.
         else:
@@ -314,116 +314,116 @@
             if (response != None) and (response.status_code == 200):
                 self.IPFS_fails = 0
                 hashes = response.json()
 
                 # --- Save text if the save_dataset flag is on.
                 if self.save_dataset :
                     self.save_hash(file_meta, json.dumps(response.json()) )
-                    
+
             else:
                 self.IPFS_fails += 1
                 logger.warning("Failed to get dataset".ljust(20) + "<blue>{}</blue>".format(file_meta['Name']))
                 return None
 
         if hashes == None:
             return None
         else:
             for h in hashes:
                 h['Folder'] = file_meta['Name']
-            return hashes 
+            return hashes
 
     def get_hashes_from_dataset(self):
         r""" Getting directories .
         Where a directory could be leading to a data file or a directory file.
 
         Returns:
             directories (:type:`list`, `required`)
                 A list of directory.
-                    directory: Map{ Name: str, Hash: str, Size: int }: 
+                    directory: Map{ Name: str, Hash: str, Size: int }:
                         A random directory that lead to a datafile.
         """
         def get_hashes(dataset_meta):
             if self.IPFS_fails > self.IPFS_fails_max:
                 sub_directories = json.loads(self.load_hash(dataset_meta))
                 for sub_directory in sub_directories:
                     sub_directory['Folder'] = dataset_meta['Name']
             else:
                 sub_directories = self.get_dataset(dataset_meta)
 
             if sub_directories != None:
                 return sub_directories
 
             return []
-        
+
         directories = []
         self.IPFS_fails = 0
-        
+
         if self.dataset_names == ['default']:
             i = 0
             dataset_hashes = list(self.dataset_hashes.values())
             random.shuffle(dataset_hashes)
-            
-            for dataset_hash in dataset_hashes: 
+
+            for dataset_hash in dataset_hashes:
                 dataset_meta = {'Folder': 'mountain', 'Name': dataset_hash['Name'], 'Hash': dataset_hash['Hash']}
                 directories += get_hashes(dataset_meta)
                 i += 1
                 if i >= self.max_datasets:
                     break
-                    
+
         else:
             for key in self.dataset_names:
                 if key in self.dataset_hashes.keys():
-                    dataset_meta = {'Folder': 'mountain','Name': key, 'Hash': self.dataset_hashes[key]['Hash'] }  
+                    dataset_meta = {'Folder': 'mountain','Name': key, 'Hash': self.dataset_hashes[key]['Hash'] }
                     directories += get_hashes(dataset_meta)
 
                 else:
                     logger.error('Incorrect dataset name:'.ljust(20) + " <red>{}</red>.".format(key)+' Must be one of the following {}'.format(bittensor.__datasets__))
 
         if len(directories) == 0:
             logger.error('Could not get any directory from IPFS or local.')
             directories = None
-          
+
         return directories
 
     def get_root_text_hash(self, file_meta):
         r"""
         With recursion, from the given directory, get a directory that leads to a datafile.
 
         Args:
-            directory: Map{ Name: str, Hash: str, Size: int }: 
+            directory: Map{ Name: str, Hash: str, Size: int }:
                 The original directory to look up a datafile for.
 
         Returns:
-            directory: Map{ Name: str, Hash: str, Size: int }: 
+            directory: Map{ Name: str, Hash: str, Size: int }:
                 A random directory that lead to a datafile.
         """
         # --- If the size of directory is small, it is leads to data file, return the data file.
         if file_meta['Size'] <= self.datafile_size_bound:
             return file_meta
 
         # --- Else, the directory leads to more directories, return a random data file within the directories.
         else:
             response = self.get_ipfs_directory(self.text_dir, file_meta)
             # --- Return none if the request failed.
             if (response == None) or (response.status_code != 200):
                 logger.warning("Failed to retrieve directory, ignoring directory:".ljust(20) + "<blue>{}</blue>".format(file_meta))
                 return None
-            
+
             # --- Pick a random sub_directory, run recursion until we have found a data file
             else:
                 sub_directories = response.json()
                 if sub_directories and 'Links' in sub_directories.keys() and len(sub_directories['Links']) >= 1:
                     random_sub_directory = random.choice(sub_directories['Links'])
 
-                    # --- Fill the name of the random_sub_directory if it is empty. 
+                    # --- Fill the name of the random_sub_directory if it is empty.
                     if random_sub_directory['Name'] == '':
                         random_sub_directory['Name'] = file_meta['Name']
                         random_sub_directory['Folder'] = file_meta['Folder']
 
-                    
+
                     return self.get_root_text_hash(random_sub_directory)
                 else:
                     logger.warning("Directory seems empty, ignoring directory:".ljust(20) + "<blue>{}</blue>". format(file_meta))
         return None
 
     def get_text_from_local(self, min_data_len):
 
@@ -435,47 +435,47 @@
         else:
             folders_avail = []
             for dataset_name in self.dataset_names:
                 if dataset_name in folders:
                     folders_avail.append(dataset_name)
             random.shuffle(folders_avail)
 
-        files = [] 
+        files = []
         for folder in folders_avail:
             file_names = os.listdir(os.path.expanduser(os.path.join(self.data_dir, folder)))
             sub_files = [{'Name': file_name,'Folder': folder, 'Hash': file_name} for file_name in file_names]
             files += sub_files
 
         random.shuffle(files)
         data_corpus = []
         total_dataset_len = 0
 
         for text_file in files:
             # --- Get text from the datafile directory
             text = self.load_hash(text_file)
 
             if text != None:
-                text_list = text.split() 
+                text_list = text.split()
                 data_corpus.extend(text_list)
                 total_dataset_len += len(text_list)
-            
+
             if (total_dataset_len > min_data_len) :
                 break
 
         return data_corpus
 
     def construct_text_corpus(self, min_data_len = 0):
         """ Main function for generating the text data.
         1. Get directories from a random dataset_hash (dataset_hash is the result from calling pin/ls).
-        2. Pick a random directory and get the directory that would lead to a datafile.    
+        2. Pick a random directory and get the directory that would lead to a datafile.
         3. Get text from the directory.
         4. Repeat 2,3 until we have reached the min data length
 
         Returns:
-            text: str: 
+            text: str:
                 Contents of the text data.
         """
         self.IPFS_fails = 0
         data_corpus = []
         try:
             # --- Get directories from a random dataset_hash
             directories = list(self.get_hashes_from_dataset())
@@ -493,22 +493,22 @@
                 n_workers = cpu_count() if self.num_workers == 0 else self.num_workers
                 with concurrent.futures.ThreadPoolExecutor(max_workers=n_workers) as executor:
                     while (total_dataset_len < min_data_len) and (self.IPFS_fails <= self.IPFS_fails_max):
                         future_map = {}
                         for idx, call_arg in enumerate(directories[:n_workers]):
                             future = executor.submit(self.get_text, call_arg)
                             future_map[future] = call_arg
-                        
+
                         for i, future in enumerate(concurrent.futures.as_completed(future_map)):
                             text = future.result()
                             if text is not None:
                                 text_list = text.split()
                                 data_corpus.extend(text_list)
                                 total_dataset_len += len(text_list)
-                        
+
                         logger.success("Loaded from IPFS".ljust(20) + f"<yellow>{ round(total_dataset_len / min_data_len * 100) }%</yellow>  " + "<blue>{}</blue>".format([file_meta['Name'] for file_meta in directories[:n_workers]]))
                         directories = directories[n_workers:]
 
             else:
                 logger.error("It appears the directory is empty... Restart your miner to try again.")
 
         except Exception as e:
@@ -518,60 +518,60 @@
         if len(data_corpus) == 0:
             logger.error("Fail to construct any text from IPFS, getting from local instead.")
             data_corpus = self.get_text_from_local(min_data_len)
 
         return data_corpus
 
     def reserve_multiple_data(self, epoch_length = 100, multiples = 2):
-        r""" Make sure the reserved data meet the multiple, 
+        r""" Make sure the reserved data meet the multiple,
         If not, then keep constructing text corpus.
         Arg:
-            epoch_length (int, optional): 
+            epoch_length (int, optional):
                 A dataloader for a subset of the dataset of epoch_length is returned.
-            
+
             multiples (int, optional):
                 The number of dataloader that the data_reserved should be able to create.
 
-        Return: 
+        Return:
             success (bool):
                 If we have got the data ready.
         """
         logger.success(f"Reserving data with multiples: {multiples}")
         data_size = epoch_length * self.batch_size * self.block_size
-        
+
         while len(self.data_reserved) < data_size * multiples :
             self.data_reserved += self.construct_text_corpus(min_data_len = data_size)
 
         logger.success(f"Dataset download completed, {multiples} copy of data reserved")
         return True
 
     def set_data_size(self, batch_size, block_size):
         r""" Update the size of data (batch_size, block_size) that we need.
 
-        Args: 
+        Args:
             batch_size(int, required):
                 The batch_size of data that should be produced by dataloader.
 
             block_size(int, required):
-                The block_size of data that should be produced by dataloader. 
+                The block_size of data that should be produced by dataloader.
         """
         def check_valid(size):
             r""" Check if the size is a valid positive intiget, if not, return False.
             """
             if size <= 0 or (not isinstance(size, int)):
                 return False
             else:
                 return True
 
         old_batch_size = self.batch_size
         old_block_size = self.block_size
-        
+
         if check_valid(batch_size):
             self.batch_size = batch_size
-        
+
         if check_valid(block_size):
             self.block_size = block_size
 
         # empty the queue
         while not self.data_queue.queue.empty():
             self.data_queue.queue.get()
 
@@ -580,15 +580,15 @@
 
         logger.success(f"Updated data size: batch_size: {old_batch_size} --> {self.batch_size}, block_size: {old_block_size} --> {self.block_size}")
 
     def dataloader(self, epoch_length = 100):
         r""" Creates a torch dataloader out of a subclass of this class.
 
         Args:
-            epoch_length (int, optional): 
+            epoch_length (int, optional):
                 A dataloader for a subset of the dataset of epoch_length is returned.
 
         Returns:
             torch.utils.data.dataloader.DataLoader: Pytorch dataloader.
         """
         logger.success(f"Getting a new Dataloader")
         data_size = epoch_length * self.batch_size * self.block_size
@@ -601,40 +601,40 @@
 
         # Datalaoder calls self._getitem_ functions until the self.data uses up, and group the result by batch size
         return DataLoader(self,
                     shuffle=True,
                     batch_size=self.batch_size,
                     num_workers=self.num_workers,
                     drop_last=True)
-    
+
     def set_dataset_iterator(self):
-        r""" Get a new dataset that is ready from the queue. The result would be updated to self.__infinite_dataset_iterator__ . 
+        r""" Get a new dataset that is ready from the queue. The result would be updated to self.__infinite_dataset_iterator__ .
         """
-        success = False 
+        success = False
         while not success:
             if not self.data_queue.queue.empty() :
                 ready = self.data_queue.queue.get() # the queue stores a bool ready signal
                 dataset = self.dataloader(self.num_batches)
                 if dataset:
                     self.__infinite_dataset_iterator = iter([input for input in dataset])
                     success = True
             else:
                 time.sleep(2)
 
         return
 
     def __next__(self):
-        """Returns the next element from the dataset. 
+        """Returns the next element from the dataset.
         """
         if self.__infinite_dataset_iterator == None:
             self.set_dataset_iterator()
 
         try:
             return next(self.__infinite_dataset_iterator)
-        
+
         except StopIteration:
             self.set_dataset_iterator()
             return next(self.__infinite_dataset_iterator)
 
     def __len__(self):
         """Returns number of samples (blocks) of dataset
 
@@ -666,24 +666,24 @@
 
     def build_hash_table(self):
         self.IPFS_fails = 0
         self.dataset_hashes = {}
         response = None
 
         mountain_meta = {'Name': 'mountain', 'Folder': 'meta_data', 'Hash': self.mountain_hash}
-        
+
         while response == None:
             self.IPFS_fails += 1
             response = self.get_ipfs_directory(self.text_dir, mountain_meta)
-            
+
             if response:
                 dataset_hashes = response.json()['Links']
                 if self.save_dataset:
                     self.save_hash(mountain_meta, json.dumps(dataset_hashes) )
-            
+
             if self.IPFS_fails > self.IPFS_fails_max and response == None:
                 dataset_hashes = json.loads(self.load_hash(mountain_meta))
                 break
 
         for i in dataset_hashes:
             name = i['Name'][:-4]
             dataset_meta = {'Name': name, 'Hash': i['Hash'], 'Size': self.get_folder_size(name) }
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_dataset/dataset_mock.py` & `bittensor-5.0.0/bittensor/_dataset/dataset_mock.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,30 +59,30 @@
 
     def close(self):
         pass
 
     def __del__(self):
         self.close()
 
-    def construct_text_corpus(self, min_data_len = 0):         
+    def construct_text_corpus(self, min_data_len = 0):
         data_corpus = []
         total_dataset_len = 0
         i = 0
         while (total_dataset_len < min_data_len):
             text = "lorem ipsum data is not here this is super fake but maybe you could still learn from it?"
-            text_list = text.split() 
+            text_list = text.split()
             data_corpus.extend(text_list)
             total_dataset_len += len(text_list)
             i += 1
         return data_corpus
 
     def _fill_data(self, epoch_length:int = 100):
         data_size = epoch_length * self.batch_size * self.block_size
-        
-        # Make sure the data remained is at least as big as data_size 
+
+        # Make sure the data remained is at least as big as data_size
         while len(self.data_remained) < (data_size) :
             self.data_remained += self.construct_text_corpus(min_data_len = data_size)
 
         self.data = self.data_remained[:data_size]
         del self.data_remained[:data_size]
 
     def dataloader(self, epoch_length = 100):
@@ -98,17 +98,17 @@
         """
         self._fill_data(epoch_length)
         return DataLoader(self,
                     shuffle=True,
                     batch_size=self.batch_size,
                     num_workers=self.num_workers,
                     drop_last=True)
-    
+
     def __next__(self):
-        """Returns the next element from the dataset. 
+        """Returns the next element from the dataset.
         """
         if self.__infinite_dataset_iterator == None:
             self.__infinite_dataset_iterator = iter(list(self.dataloader()))
         try:
             return next(self.__infinite_dataset_iterator)
         except StopIteration:
             self.__infinite_dataset_iterator = iter(list(self.dataloader()))
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_dataset/thread_queue.py` & `bittensor-5.0.0/bittensor/_dataset/thread_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,29 +24,29 @@
     r""" This producer thread runs in backgraound to fill the queue with the result of the target function.
     """
     def __init__(self, queue, target, arg, name=None):
         r"""Initialization.
         Args:
             queue (:obj:`queue.Queue`, `required`)
                 The queue to be filled.
-                
+
             target (:obj:`function`, `required`)
                 The target function to run when the queue is not full.
 
             arg (:type:`tuple`, `required`)
                 The arguments to be passed to the target function.
 
             name (:type:`str`, `optional`)
-                The name of this threading object. 
+                The name of this threading object.
         """
         super(ProducerThread,self).__init__()
         self.name = name
         self.target = target
         self.arg = arg
-        self.queue = queue 
+        self.queue = queue
         self._stop_event = threading.Event()
 
     def run(self):
         r""" Work of the thread. Keep checking if the queue is full, if it is not full, run the target function to fill the queue.
         """
         while not self.stopped():
             if not self.queue.full():
@@ -62,17 +62,17 @@
         return self._stop_event.is_set()
 
 class ThreadQueue():
     r""" Manages the queue the producer thread that monitor and fills the queue.
     """
     def __init__(self, producer_target, producer_arg, buffer_size = 2):
         """ Setup the queue and start the producer thread.
-        
+
         Args:
-                
+
             producer_target (:obj:`function`, `required`)
                 The target function to run when the queue is not full.
 
             producer_arg (:type:`tuple`, `required`)
                 The arguments to be passed to the target function.
 
             buffer_size (:type:`int`, `optional`)
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_dendrite/dendrite.py` & `bittensor-5.0.0/bittensor/_dendrite/dendrite.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import uuid
 import grpc
 import time
 import torch
 import asyncio
@@ -31,134 +31,136 @@
 class DendriteCall( ABC ):
     """ Base class for all dendrite calls."""
 
     is_forward: bool
     name: str
 
     def __init__(
-            self, 
+            self,
             dendrite: 'bittensor.Dendrite',
             timeout: float = bittensor.__blocktime__
         ):
         self.dendrite = dendrite
         self.completed = False
         self.timeout = timeout
         self.start_time = time.time()
-        self.src_hotkey = self.dendrite.keypair.ss58_address 
+        self.src_hotkey = self.dendrite.keypair.ss58_address
         self.src_version = bittensor.__version_as_int__
         self.dest_hotkey = self.dendrite.axon_info.hotkey
-        self.dest_version = self.dendrite.axon_info.version  
+        self.dest_version = self.dendrite.axon_info.version
         self.return_code: bittensor.proto.ReturnCode = bittensor.proto.ReturnCode.Success
         self.return_message: str = 'Success'
 
-    def __repr__(self) -> str: 
+    def __repr__(self) -> str:
         return f"DendriteCall( {bittensor.utils.codes.code_to_string(self.return_code)}, to:{self.dest_hotkey[:4]} + ... + {self.dest_hotkey[-4:]}, msg:{self.return_message})"
-    
-    def __str__(self) -> str: 
+
+    def __str__(self) -> str:
         return self.__repr__()
 
     @abstractmethod
     def get_callable(self) -> Callable: ...
 
     @abstractmethod
     def get_inputs_shape(self) -> torch.Size: ...
-    
+
     @abstractmethod
     def get_outputs_shape(self) -> torch.Size: ...
 
     @abstractmethod
     def get_request_proto(self) -> object: ...
 
     def _get_request_proto(self) -> object:
-        request_proto = self.get_request_proto()    
+        request_proto = self.get_request_proto()
         request_proto.version = self.src_version
         request_proto.timeout = self.timeout
         request_proto.hotkey = self.src_hotkey
         return request_proto
-    
+
     @abstractmethod
     def apply_response_proto( self, response_proto: object ): ...
 
     def _apply_response_proto( self, response_proto: object ):
         self.apply_response_proto( response_proto )
         try: self.return_message = response_proto.return_message
         except: pass
         try: self.return_code = response_proto.return_code
         except: pass
-    
+
     def end(self):
         self.end_time = time.time()
         self.elapsed = self.end_time - self.start_time
         self.completed = True
 
     @property
     def did_timeout( self ) -> bool: return self.return_code == bittensor.proto.ReturnCode.Timeout
     @property
     def is_success( self ) -> bool: return self.return_code == bittensor.proto.ReturnCode.Success
-    @property 
+    @property
     def did_fail( self ) -> bool: return not self.is_success
 
     def log_outbound(self):
         bittensor.logging.rpc_log(
-            axon = False, 
-            forward = self.is_forward, 
-            is_response = False, 
-            code = self.return_code, 
-            call_time = 0, 
-            pubkey = self.dest_hotkey, 
+            axon = False,
+            forward = self.is_forward,
+            is_response = False,
+            code = self.return_code,
+            call_time = 0,
+            pubkey = self.dest_hotkey,
             uid = self.dendrite.uid,
-            inputs = self.get_inputs_shape(), 
+            inputs = self.get_inputs_shape(),
             outputs = self.get_outputs_shape(),
             message = self.return_message,
             synapse = self.name,
         )
 
     def log_inbound(self):
-        bittensor.logging.rpc_log( 
-            axon = False, 
-            forward = self.is_forward, 
-            is_response = True, 
-            code = self.return_code, 
+        bittensor.logging.rpc_log(
+            axon = False,
+            forward = self.is_forward,
+            is_response = True,
+            code = self.return_code,
             call_time = self.elapsed,
-            pubkey = self.dest_hotkey, 
-            uid = self.dendrite.uid, 
+            pubkey = self.dest_hotkey,
+            uid = self.dendrite.uid,
             inputs = self.get_inputs_shape(),
             outputs = self.get_outputs_shape(),
             message = self.return_message,
             synapse = self.name
-        )      
+        )
 
 class Dendrite( ABC, torch.nn.Module ):
     def __init__(
             self,
             keypair: Union[ 'bittensor.Wallet', 'bittensor.Keypair'],
-            axon: Union[ 'bittensor.axon_info', 'bittensor.axon' ], 
+            axon: Union[ 'bittensor.axon_info', 'bittensor.axon' ],
             uid : int = 0,
-            grpc_options: List[Tuple[str,object]] = 
+            ip: str = None,
+            grpc_options: List[Tuple[str,object]] =
                     [('grpc.max_send_message_length', -1),
                      ('grpc.max_receive_message_length', -1),
                      ('grpc.keepalive_time_ms', 100000) ]
         ):
         """ Dendrite abstract class
             Args:
                 keypair (:obj:`Union[ 'bittensor.Wallet', 'bittensor.Keypair']`, `required`):
                     bittensor keypair used for signing messages.
-                axon (:obj:Union[`bittensor.axon_info`, 'bittensor.axon'], `required`):   
+                axon (:obj:Union[`bittensor.axon_info`, 'bittensor.axon'], `required`):
                     bittensor axon object or its info used to create the connection.
                 grpc_options (:obj:`List[Tuple[str,object]]`, `optional`):
                     grpc options to pass through to channel.
         """
         super(Dendrite, self).__init__()
         self.uuid = str(uuid.uuid1())
         self.uid = uid
+        self.ip = ip
         self.keypair = keypair.hotkey if isinstance( keypair, bittensor.Wallet ) else keypair
         self.axon_info = axon.info() if isinstance( axon, bittensor.axon ) else axon
-        if self.axon_info.ip == bittensor.utils.networking.get_external_ip(): 
+        if self.axon_info.ip == self.ip:
             self.endpoint_str = "localhost:" + str(self.axon_info.port)
-        else: 
+        else:
             self.endpoint_str = self.axon_info.ip + ':' + str(self.axon_info.port)
         self.channel = grpc.aio.insecure_channel( self.endpoint_str, options = grpc_options )
         self.state_dict = _common.CYGRPC_CONNECTIVITY_STATE_TO_CHANNEL_CONNECTIVITY
         self.loop = asyncio.get_event_loop()
 
     async def apply( self, dendrite_call: 'DendriteCall' ) -> DendriteCall:
         """ Applies a dendrite call to the endpoint.
@@ -186,64 +188,64 @@
             bittensor.logging.trace( 'Dendrite.apply() received response from: {}'.format( self.axon_info.hotkey ) )
 
         # Request failed with GRPC code.
         except grpc.RpcError as rpc_error_call:
             dendrite_call.return_code = rpc_error_call.code()
             dendrite_call.return_message = 'GRPC error code: {}, details: {}'.format( rpc_error_call.code(), str(rpc_error_call.details()) )
             bittensor.logging.trace( 'Dendrite.apply() rpc error: {}'.format( dendrite_call.return_message ) )
-    
+
         # Catch timeout errors.
         except asyncio.TimeoutError:
             dendrite_call.return_code = bittensor.proto.ReturnCode.Timeout
             dendrite_call.return_message = 'GRPC request timeout after: {}s'.format( dendrite_call.timeout)
             bittensor.logging.trace( 'Denrite.apply() timeout error: {}'.format( dendrite_call.return_message ) )
 
         except Exception as e:
             # Catch unknown errors.
             dendrite_call.return_code = bittensor.proto.ReturnCode.UnknownException
-            dendrite_call.return_message = str(e)   
+            dendrite_call.return_message = str(e)
             bittensor.logging.trace( 'Dendrite.apply() unknown error: {}'.format( dendrite_call.return_message ) )
 
         finally:
-            dendrite_call.end()         
-            dendrite_call.log_inbound()  
+            dendrite_call.end()
+            dendrite_call.log_inbound()
             return dendrite_call
 
-    def __exit__ ( self ): 
+    def __exit__ ( self ):
         self.__del__()
 
-    def close ( self ): 
+    def close ( self ):
         self.__exit__()
 
     def __del__ ( self ):
         try:
             result = self.channel._channel.check_connectivity_state(True)
-            if self.state_dict[result] != self.state_dict[result].SHUTDOWN: 
+            if self.state_dict[result] != self.state_dict[result].SHUTDOWN:
                 self.loop.run_until_complete ( self.channel.close() )
         except:
             pass
 
-    def nonce ( self ): 
+    def nonce ( self ):
         return time.monotonic_ns()
 
     def sign(self) -> str:
         """ Creates a signature for the dendrite and returns it as a string."""
         nonce = f"{self.nonce()}"
         sender_hotkey = self.keypair.ss58_address
         receiver_hotkey = self.axon_info.hotkey
         message = f"{nonce}.{sender_hotkey}.{receiver_hotkey}.{self.uuid}"
         signature = f"0x{self.keypair.sign(message).hex()}"
         return ".".join([nonce, sender_hotkey, signature, self.uuid])
-        
+
     def state ( self ):
         """ Returns the state of the dendrite channel."""
-        try: 
+        try:
             return self.state_dict[self.channel._channel.check_connectivity_state(True)]
         except ValueError:
             return "Channel closed"
 
 
 
-    
 
-    
-    
+
+
+
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_dendrite/text_prompting/dendrite.py` & `bittensor-5.0.0/bittensor/_dendrite/text_prompting/dendrite.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,27 +37,27 @@
         super().__init__( dendrite = dendrite, timeout = timeout )
         self.messages = messages
         self.roles = roles
         self.packed_messages = [json.dumps({"role": role, "content": message}) for role, message in zip(self.roles, self.messages)]
 
     def __repr__(self) -> str:
         return f"DendriteForwardCall( {bittensor.utils.codes.code_to_string(self.return_code)}, to: {self.dest_hotkey[:4]}...{self.dest_hotkey[-4:]}, msg: {self.return_message}, completion: {self.completion.strip()})"
-    
+
     def __str__(self) -> str: return self.__repr__()
-    
+
     def get_callable( self ) -> Callable:
         return bittensor.grpc.TextPromptingStub( self.dendrite.channel ).Forward
 
     def get_request_proto( self ) -> bittensor.proto.ForwardTextPromptingRequest:
         return bittensor.ForwardTextPromptingRequest( timeout = self.timeout, messages = self.packed_messages )
-    
+
     def apply_response_proto( self, response_proto: bittensor.ForwardTextPromptingResponse ):
         self.completion = response_proto.response
-        
-    def get_inputs_shape(self) -> torch.Size: 
+
+    def get_inputs_shape(self) -> torch.Size:
         return torch.Size( [len(message) for message in self.packed_messages] )
 
     def get_outputs_shape(self) -> torch.Size:
         return torch.Size([ len(self.completion) ] )
 
     def backward( self, reward: float, timeout: float = None ) -> 'DendriteBackwardCall':
         return self.dendrite.backward(
@@ -94,38 +94,38 @@
         super().__init__( dendrite = dendrite, timeout = timeout )
         self.messages = messages
         self.roles = roles
         self.packed_messages = [json.dumps({"role": role, "content": message}) for role, message in zip(self.roles, self.messages)]
 
     def __repr__(self) -> str:
         return f"MultiDendriteForwardCall( {bittensor.utils.codes.code_to_string(self.return_code)}, to: {self.dest_hotkey[:4]}...{self.dest_hotkey[-4:]}, msg: {self.return_message}, n_completion: {len(self.multi_completions)})"
-    
+
     def __str__(self) -> str: return self.__repr__()
-    
+
     def get_callable( self ) -> Callable:
         return bittensor.grpc.TextPromptingStub( self.dendrite.channel ).MultiForward
 
     def get_request_proto( self ) -> bittensor.proto.MultiForwardTextPromptingRequest:
         return bittensor.MultiForwardTextPromptingRequest( timeout = self.timeout, messages = self.packed_messages )
-    
+
     def apply_response_proto( self, response_proto: bittensor.MultiForwardTextPromptingResponse ):
         self.multi_completions = response_proto.multi_completions
-        
-    def get_inputs_shape(self) -> torch.Size: 
+
+    def get_inputs_shape(self) -> torch.Size:
         return torch.Size( [len(message) for message in self.packed_messages] )
 
     def get_outputs_shape(self) -> torch.Size:
         return torch.Size([ len(self.multi_completions) ] )
-    
-    
+
+
 class DendriteBackwardCall( bittensor.DendriteCall ):
 
     name: str = "text_prompting_backward"
     is_forward: bool = False
-    
+
     def __init__(
         self,
         dendrite: 'bittensor.TextPromptingDendrite',
         completion: str,
         messages: List[str],
         roles: List[str],
         rewards: Union[ List[float], torch.FloatTensor ],
@@ -136,26 +136,26 @@
         self.roles = roles
         self.completion = completion
         self.rewards = rewards if not isinstance( rewards, torch.FloatTensor ) else rewards.tolist()
         self.packed_messages = [ json.dumps({"role": role, "content": message}) for role, message in zip(self.roles, self.messages)]
 
     def __repr__(self) -> str:
         return f"DendriteBackwardCall( {bittensor.utils.codes.code_to_string(self.return_code)}, to: {self.dest_hotkey[:4]}...{self.dest_hotkey[-4:]}, msg: {self.return_message} )"
-    
+
     def __str__(self) -> str: return self.__repr__()
 
     def get_callable( self ) -> Callable:
         return bittensor.grpc.TextPromptingStub( self.dendrite.channel ).Backward
 
     def get_request_proto( self ) -> bittensor.proto.BackwardTextPromptingRequest:
         return bittensor.BackwardTextPromptingRequest( messages = self.packed_messages, response = self.completion, rewards = self.rewards, timeout = self.timeout )
-    
+
     def apply_response_proto( self, response_proto: bittensor.ForwardTextPromptingResponse ):
         pass
-        
+
     def get_inputs_shape(self) -> torch.Size:
         return torch.Size( [len(message) for message in self.packed_messages] )
 
     def get_outputs_shape(self) -> torch.Size:
         return torch.Size( [0] )
 
 
@@ -168,32 +168,32 @@
             self,
             roles: List[ str ] ,
             messages: List[ str ],
             timeout: float = bittensor.__blocktime__,
             return_call:bool = True,
         ) -> Union[ str, DendriteForwardCall ]:
         forward_call = DendriteForwardCall(
-            dendrite = self, 
+            dendrite = self,
             messages = messages,
             roles = roles,
             timeout = timeout,
         )
         response_call = self.loop.run_until_complete( self.apply( dendrite_call = forward_call ) )
         if return_call: return response_call
         else: return response_call.completion
-    
+
     async def async_forward(
         self,
         roles: List[ str ],
         messages: List[ str ],
         timeout: float = bittensor.__blocktime__,
         return_call: bool = True,
     ) -> Union[ str, DendriteForwardCall ]:
         forward_call = DendriteForwardCall(
-            dendrite = self, 
+            dendrite = self,
             messages = messages,
             roles = roles,
             timeout = timeout,
         )
         forward_call = await self.apply( dendrite_call = forward_call )
         if return_call: return forward_call
         else: return forward_call.completion
@@ -202,32 +202,32 @@
             self,
             roles: List[ str ] ,
             messages: List[ str ],
             timeout: float = bittensor.__blocktime__,
             return_call:bool = True,
         ) -> Union[ str, DendriteForwardCall ]:
         forward_call = MultiDendriteForwardCall(
-            dendrite = self, 
+            dendrite = self,
             messages = messages,
             roles = roles,
             timeout = timeout,
         )
         response_call = self.loop.run_until_complete( self.apply( dendrite_call = forward_call ) )
         if return_call: return response_call
         else: return response_call.multi_completions
-    
+
     async def async_multi_forward(
         self,
         roles: List[ str ],
         messages: List[ str ],
         timeout: float = bittensor.__blocktime__,
         return_call: bool = True,
     ) -> Union[ str, DendriteForwardCall ]:
         forward_call = MultiDendriteForwardCall(
-            dendrite = self, 
+            dendrite = self,
             messages = messages,
             roles = roles,
             timeout = timeout,
         )
         forward_call = await self.apply( dendrite_call = forward_call )
         if return_call: return forward_call
         else: return forward_call.multi_completions
@@ -250,24 +250,24 @@
         )
         return self.loop.run_until_complete( self.apply( dendrite_call = backward_call ) )
 
     async def async_backward(
         self,
         roles: List[ str ],
         messages: List[ str ],
-        completion: str,        
+        completion: str,
         rewards: Union[ List[ float], torch.FloatTensor ],
         timeout: float = bittensor.__blocktime__,
     ) -> DendriteBackwardCall:
         backward_call = DendriteBackwardCall(
             dendrite = self,
             completion = completion,
             messages = messages,
             roles = roles,
             rewards = rewards,
             timeout = timeout,
         )
-        return await self.apply( dendrite_call = backward_call ) 
+        return await self.apply( dendrite_call = backward_call )
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_dendrite/text_prompting/dendrite_pool.py` & `bittensor-5.0.0/bittensor/_dendrite/text_prompting/dendrite_pool.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,102 +21,103 @@
 import asyncio
 import bittensor
 from typing import Callable, List, Dict, Union
 
 class TextPromptingDendritePool( torch.nn.Module ):
 
     def __init__(
-            self, 
+            self,
             keypair: Union[ 'bittensor.Wallet', 'bittensor.Keypair'],
-            metagraph: 'bittensor.metagraph', 
+            metagraph: 'bittensor.metagraph',
         ):
         super(TextPromptingDendritePool, self).__init__()
         self.metagraph = metagraph
         self.keypair = keypair
-        self.dendrites = [ bittensor.text_prompting( axon = axon, keypair = self.keypair, uid = uid ) for uid, axon in enumerate(self.metagraph.axons) ]
+        self.ip = bittensor.utils.networking.get_external_ip()
+        self.dendrites = [ bittensor.text_prompting( axon = axon, keypair = self.keypair, uid = uid, ip = self.ip) for uid, axon in enumerate(self.metagraph.axons) ]
         self.loop = asyncio.get_event_loop()
         self.priority_threadpool = bittensor.prioritythreadpool(max_workers = 1)
 
     def backward( self,
             forward_calls: List[ 'DendriteForwardCall' ],
             rewards: Union[ List[ float ], torch.FloatTensor ],
             timeout: float = 12.0,
             priority: int = 1,
         ):
         def _backward():
-            self.loop.run_until_complete( 
+            self.loop.run_until_complete(
                 self.async_backward (
                     forward_calls = forward_calls,
                     timeout = timeout,
-                ) 
+                )
             )
         future = self.priority_threadpool.submit(
             _backward,
             priority = priority
         )
         return future.result()
 
     async def async_backward(self,
             forward_calls: List[ 'DendriteForwardCall' ],
             rewards: Union[ List[ float ], torch.FloatTensor ] ,
             timeout: float = 12.0
         ):
         rewards = rewards if not isinstance( rewards, torch.Tensor ) else rewards.tolist()
         async def query():
-            coroutines = [ forward_calls.async_backward( reward ) for call, reward in list(zip( forward_calls, rewards )) ]                
+            coroutines = [ forward_calls.async_backward( reward ) for call, reward in list(zip( forward_calls, rewards )) ]
             all_responses = await asyncio.gather( *coroutines )
             return all_responses
         await query()
 
-    def forward( 
-            self, 
-            roles: Union[ str, List[str] ], 
+    def forward(
+            self,
+            roles: Union[ str, List[str] ],
             messages: Union[ str, List[str] ],
-            uids: Union[ torch.LongTensor, List[int] ] = None, 
+            uids: Union[ torch.LongTensor, List[int] ] = None,
             return_call:bool = True,
             timeout: float = 12,
             priority: int = 1,
         ) -> List['DendriteForwardCall']:
         def _forward():
             bittensor.logging.trace( 'dendrite pool: forward: _forward: start')
             return self.loop.run_until_complete(
                 self.async_forward (
                     messages = messages,
                     roles = roles,
                     uids = uids,
                     return_call = return_call,
                     timeout = timeout,
-                ) 
+                )
             )
         future = self.priority_threadpool.submit(
             _forward,
             priority = priority
         )
         return future.result()
 
-    async def async_forward( 
-            self, 
+    async def async_forward(
+            self,
             roles: Union[ str, List[str] ],
             messages: Union[ str, List[str] ],
-            uids: Union[ torch.LongTensor, List[int] ] = None, 
+            uids: Union[ torch.LongTensor, List[int] ] = None,
             return_call:bool = True,
-            timeout: float = 12 
-        ) -> List['DendriteForwardCall']:      
+            timeout: float = 12
+        ) -> List['DendriteForwardCall']:
         # We optionally set the uids to all if uids is None.
         if uids is None: uids = range( self.metagraph.n.item() )
         if isinstance( uids, torch.Tensor ): uids = uids.tolist()
         # The following asyncio defintion queries a single endpoint with the message
         # prompt and returns the response.
         async def call_single_uid( uid: int ) -> str:
-            return await self.dendrites[uid].async_forward( 
-                roles = roles, 
+            return await self.dendrites[uid].async_forward(
+                roles = roles,
                 messages = messages,
-                return_call = return_call, 
-                timeout = timeout 
+                return_call = return_call,
+                timeout = timeout
             )
         # The following asyncio definition gathers the responses
         # from multiple coroutines for each uid.
         async def query():
-            coroutines = [ call_single_uid( uid ) for uid in uids ]                
+            coroutines = [ call_single_uid( uid ) for uid in uids ]
             all_responses = await asyncio.gather(*coroutines)
             return all_responses
-        return await query() 
+        return await query()
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_ipfs/ipfs_impl.py` & `bittensor-5.0.0/bittensor/_ipfs/ipfs_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 from requests.packages.urllib3.util.retry import Retry
 import requests
 
 class Ipfs():
     """ Implementation for the dataset class, which handles dataloading from ipfs
     """
     def __init__(self):
-        
+
         # Used to retrieve directory contentx
-        self.cat = 'http://global.ipfs.opentensor.ai/api/v0/cat' 
+        self.cat = 'http://global.ipfs.opentensor.ai/api/v0/cat'
         self.node_get = 'http://global.ipfs.opentensor.ai/api/v0/object/get'
         self.ipns_resolve = 'http://global.ipfs.opentensor.ai/api/v0/name/resolve'
 
         self.mountain_hash = 'QmSdDg6V9dgpdAFtActs75Qfc36qJtm9y8a7yrQ1rHm7ZX'
         self.latest_neurons_ipns = "k51qzi5uqu5di1eoe0o91g32tbfsgikva6mvz0jw0414zhxzhiakana67shoh7"
         self.historical_neurons_ipns = "k51qzi5uqu5dhf5yxm3kqw9hyrv28q492p3t32s23059z911a23l30ai6ziceh"
         # Used when current corpus has been exhausted
         self.refresh_corpus = False
-        
+
 
     @staticmethod
     def requests_retry_session(
             retries=1,
             backoff_factor=0.5,
             status_forcelist=(104, 500, 502, 504),
             session=None,
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_keyfile/__init__.py` & `bittensor-5.0.0/bittensor/_keyfile/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import bittensor
 from . import keyfile_impl
 
 class keyfile (object):
     """ Factory for a bittensor on device keypair
     """
-    def __new__( 
-        cls, 
+    def __new__(
+        cls,
         path: str = None,
         _mock: bool = False
     ) -> 'bittensor.Keyfile':
         r""" Initialize a bittensor on device keypair interface.
 
             Args:
                 path (required=False, default: ~/.bittensor/wallets/default/coldkey ):
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_keyfile/keyfile_impl.py` & `bittensor-5.0.0/bittensor/_keyfile/keyfile_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import os
 import base64
 import json
 import stat
 import getpass
@@ -50,15 +50,15 @@
     """
     json_data = {
         'accountId': "0x" + keypair.public_key.hex() if keypair.public_key != None else None,
         'publicKey': "0x" + keypair.public_key.hex()  if keypair.public_key != None else None,
         'secretPhrase': keypair.mnemonic if keypair.mnemonic != None else None,
         'secretSeed': "0x" + \
             # If bytes -> str
-            ( keypair.seed_hex if isinstance(keypair.seed_hex, str) else keypair.seed_hex.hex() ) 
+            ( keypair.seed_hex if isinstance(keypair.seed_hex, str) else keypair.seed_hex.hex() )
                 # If None -> None
                 if keypair.seed_hex != None else None,
         'ss58Address': keypair.ss58_address if keypair.ss58_address != None else None
     }
     data = json.dumps( json_data ).encode()
     return data
 
@@ -184,15 +184,15 @@
             password ( bool, optional ):
                 It set, uses this password to encrypt data.
         Returns:
             encrytped_data (bytes):
                 Ansible encrypted data.
     """
     password = ask_password_to_encrypt() if password == None else password
-    console = bittensor.__console__;             
+    console = bittensor.__console__;
     with console.status(":locked_with_key: Encrypting key..."):
         vault = Vault( password )
     return vault.vault.encrypt ( keyfile_data )
 
 
 def get_coldkey_password_from_environment(coldkey_name: str) -> Optional[str]:
 
@@ -221,32 +221,32 @@
                 Raised if the file is corrupted or if the password is incorrect.
     """
     if coldkey_name is not None and password is None:
         password = get_coldkey_password_from_environment(coldkey_name)
 
     try:
         password = getpass.getpass("Enter password to unlock key: ") if password is None else password
-        console = bittensor.__console__;             
+        console = bittensor.__console__;
         with console.status(":key: Decrypting key..."):
             # Ansible decrypt.
             if keyfile_data_is_encrypted_ansible( keyfile_data ):
                 vault = Vault( password )
                 try:
                     decrypted_keyfile_data = vault.load( keyfile_data )
                 except AnsibleVaultError:
                     raise KeyFileError('Invalid password')
             # Legacy decrypt.
             elif keyfile_data_is_encrypted_legacy( keyfile_data ):
                 __SALT = b"Iguesscyborgslikemyselfhaveatendencytobeparanoidaboutourorigins"
                 kdf = PBKDF2HMAC(algorithm=hashes.SHA256(), salt=__SALT, length=32, iterations=10000000, backend=default_backend())
                 key = base64.urlsafe_b64encode(kdf.derive(password.encode()))
                 cipher_suite = Fernet(key)
-                decrypted_keyfile_data = cipher_suite.decrypt( keyfile_data )   
+                decrypted_keyfile_data = cipher_suite.decrypt( keyfile_data )
             # Unknown.
-            else: 
+            else:
                 raise KeyFileError( "Keyfile data: {} is corrupt".format( keyfile_data ))
 
     except (InvalidSignature, InvalidKey, InvalidToken):
         raise KeyFileError('Invalid password')
 
     if not isinstance(decrypted_keyfile_data, bytes):
         decrypted_keyfile_data = json.dumps( decrypted_keyfile_data ).encode()
@@ -277,36 +277,36 @@
                 password ( str, optional ):
                     Optional password used to decrypt file. If None, asks for user input.
             Returns:
                 keypair (bittensor.Keypair):
                     Keypair stored under path.
             Raises:
                 KeyFileError:
-                    Raised if the file does not exists, is not readable, writable 
+                    Raised if the file does not exists, is not readable, writable
                     corrupted, or if the password is incorrect.
         """
         return self.get_keypair()
 
     @property
     def data( self ) -> bytes:
         """ Returns keyfile data under path.
             Returns:
-                keyfile_data (bytes):   
+                keyfile_data (bytes):
                     Keyfile data stored under path.
             Raises:
                 KeyFileError:
                     Raised if the file does not exists, is not readable, or writable.
         """
         return self._read_keyfile_data_from_file()
 
     @property
     def keyfile_data( self ) -> bytes:
         """ Returns keyfile data under path.
             Returns:
-                keyfile_data (bytes):   
+                keyfile_data (bytes):
                     Keyfile data stored under path.
             Raises:
                 KeyFileError:
                     Raised if the file does not exists, is not readable, or writable.
         """
         return self._read_keyfile_data_from_file()
 
@@ -337,28 +337,28 @@
                 password ( str, optional ):
                     Optional password used to decrypt file. If None, asks for user input.
             Returns:
                 keypair (bittensor.Keypair):
                     Keypair stored under path.
             Raises:
                 KeyFileError:
-                    Raised if the file does not exists, is not readable, writable 
+                    Raised if the file does not exists, is not readable, writable
                     corrupted, or if the password is incorrect.
         """
         keyfile_data = self._read_keyfile_data_from_file()
         if keyfile_data_is_encrypted( keyfile_data ):
             keyfile_data = decrypt_keyfile_data(keyfile_data, password, coldkey_name=self.name)
         return deserialize_keypair_from_keyfile_data( keyfile_data )
 
     def make_dirs( self ):
         """ Makes directories for path.
         """
         directory = os.path.dirname( self.path )
         if not os.path.exists( directory ):
-            os.makedirs( directory ) 
+            os.makedirs( directory )
 
     def exists_on_device( self ) -> bool:
         """ Returns true if the file exists on the device.
             Returns:
                 on_device (bool):
                     True if the file is on device.
         """
@@ -414,38 +414,38 @@
                     Raised if the file does not exists, is not readable, writable.
         """
         if not self.exists_on_device():
             raise KeyFileError( "Keyfile at: {} is not a file".format( self.path ))
         if not self.is_readable():
             raise KeyFileError( "Keyfile at: {} is not readable".format( self.path ))
         if not self.is_writable():
-            raise KeyFileError( "Keyfile at: {} is not writeable".format( self.path ) ) 
+            raise KeyFileError( "Keyfile at: {} is not writeable".format( self.path ) )
         keyfile_data = self._read_keyfile_data_from_file()
         if not keyfile_data_is_encrypted( keyfile_data ):
             as_keypair = deserialize_keypair_from_keyfile_data( keyfile_data )
             keyfile_data = serialized_keypair_to_keyfile_data( as_keypair )
             keyfile_data = encrypt_keyfile_data( keyfile_data, password )
         self._write_keyfile_data_to_file( keyfile_data, overwrite = True )
 
     def decrypt( self, password: str = None):
         """ Decrypts file under path.
             Args:
                 password: (str, optional):
                     Optional password for decryption. Otherwise asks for user input.
             Raises:
                 KeyFileError:
-                    Raised if the file does not exists, is not readable, writable 
+                    Raised if the file does not exists, is not readable, writable
                     corrupted, or if the password is incorrect.
         """
         if not self.exists_on_device():
             raise KeyFileError( "Keyfile at: {} is not a file".format( self.path ))
         if not self.is_readable():
             raise KeyFileError( "Keyfile at: {} is not readable".format( self.path ))
         if not self.is_writable():
-            raise KeyFileError( "No write access for {}".format( self.path ) ) 
+            raise KeyFileError( "No write access for {}".format( self.path ) )
         keyfile_data = self._read_keyfile_data_from_file()
         if keyfile_data_is_encrypted( keyfile_data ):
             keyfile_data = decrypt_keyfile_data(keyfile_data, password, coldkey_name=self.name)
         as_keypair = deserialize_keypair_from_keyfile_data( keyfile_data )
         keyfile_data = serialized_keypair_to_keyfile_data( as_keypair )
         self._write_keyfile_data_to_file( keyfile_data, overwrite = True )
 
@@ -476,15 +476,15 @@
             Raises:
                 KeyFileError:
                     Raised if the file is not writable or the user returns No to overwrite prompt.
         """
         # Check overwrite.
         if self.exists_on_device() and not overwrite:
             if not self._may_overwrite():
-                raise KeyFileError( "Keyfile at: {} is not writeable".format( self.path ) ) 
+                raise KeyFileError( "Keyfile at: {} is not writeable".format( self.path ) )
         with open(self.path, "wb") as keyfile:
             keyfile.write( keyfile_data )
         # Set file permissions.
         os.chmod(self.path, stat.S_IRUSR | stat.S_IWUSR)
 
 
 class MockKeyfile( object ):
@@ -512,15 +512,15 @@
 
     @property
     def data( self ) -> bytes:
         return bytes(self._mock_data)
 
     @property
     def keyfile_data( self ) -> bytes:
-        return bytes( self._mock_data) 
+        return bytes( self._mock_data)
 
     def set_keypair ( self, keypair: 'bittensor.Keypair', encrypt: bool = True, overwrite: bool = False, password:str = None):
         self._mock_keypair = keypair
         self._mock_data = serialized_keypair_to_keyfile_data( self._mock_keypair )
 
     def get_keypair(self, password: str = None) -> 'bittensor.Keypair':
         return self._mock_keypair
@@ -551,8 +551,7 @@
 
 
 
 
 
 
 
-
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_logging/__init__.py` & `bittensor-5.0.0/bittensor/_logging/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,29 +53,29 @@
             debug: bool = None,
             trace: bool = None,
             record_log: bool = None,
             logging_dir: str = None,
         ):
         r""" Instantiate bittensor logging system backend.
             Args:
-                config (:obj:`bittensor.Config`, `optional`): 
+                config (:obj:`bittensor.Config`, `optional`):
                     bittensor.logging.config()
                 debug (:obj:`bool`, `optional`):
                     Turn on debug.
                 trace (:obj:`bool`, `optional`):
                     Turn on trace.
                 record_log (:obj:`bool`, `optional`):
                     If true, logs are saved to loggind dir.
                 logging_dir (:obj:`str`, `optional`):
-                    Directory where logs are sunk. 
-        """   
+                    Directory where logs are sunk.
+        """
 
         cls.__has_been_inited__ = True
 
-        if config == None: 
+        if config == None:
             config = logging.config()
         config = copy.deepcopy(config)
         config.logging.debug = debug if debug != None else config.logging.debug
         config.logging.trace = trace if trace != None else config.logging.trace
         config.logging.record_log = record_log if record_log != None else config.logging.record_log
         config.logging.logging_dir = logging_dir if logging_dir != None else config.logging.logging_dir
 
@@ -125,15 +125,15 @@
         """ Get config from the argument parser
             Return: bittensor.config object
         """
         parser = argparse.ArgumentParser()
         logging.add_args( parser )
         return bittensor.config( parser )
 
-    @classmethod   
+    @classmethod
     def help(cls):
         """ Print help to stdout
         """
         parser = argparse.ArgumentParser()
         cls.add_args( parser )
         print (cls.__new__.__doc__)
         parser.print_help()
@@ -148,15 +148,15 @@
             parser.add_argument('--' + prefix_str + 'logging.trace', action='store_true', help='''Turn on bittensor trace level information''', default = bittensor.defaults.logging.trace )
             parser.add_argument('--' + prefix_str + 'logging.record_log', action='store_true', help='''Turns on logging to file.''', default = bittensor.defaults.logging.record_log )
             parser.add_argument('--' + prefix_str + 'logging.logging_dir', type=str, help='Logging default root directory.', default = bittensor.defaults.logging.logging_dir )
         except argparse.ArgumentError:
             # re-parsing arguments.
             pass
 
-    @classmethod   
+    @classmethod
     def add_defaults(cls, defaults):
         """ Adds parser defaults to object from enviroment variables.
         """
         defaults.logging = bittensor.Config()
         defaults.logging.debug = os.getenv('BT_LOGGING_DEBUG') if os.getenv('BT_LOGGING_DEBUG') != None else False
         defaults.logging.trace = os.getenv('BT_LOGGING_TRACE') if os.getenv('BT_LOGGING_DEBUG') != None else False
         defaults.logging.record_log = os.getenv('BT_LOGGING_RECORD_LOG') if os.getenv('BT_LOGGING_RECORD_LOG') != None else False
@@ -166,23 +166,23 @@
     def check_config( cls, config: 'bittensor.Config' ):
         """ Check config
         """
         assert config.logging
 
     @classmethod
     def set_debug(cls, debug_on: bool = True ):
-        """ Set debug for the specific cls class 
+        """ Set debug for the specific cls class
         """
         if not cls.__has_been_inited__:
             cls()
         cls.__debug_on__ = debug_on
 
     @classmethod
     def set_trace(cls, trace_on: bool = True):
-        """ Set trace back for the specific cls class 
+        """ Set trace back for the specific cls class
         """
         if not cls.__has_been_inited__:
             cls()
         cls.__trace_on__ = trace_on
 
     @classmethod
     def get_level( cls ) -> int:
@@ -209,43 +209,43 @@
         """ Log with different format according to record['extra']
         """
         extra = record['extra']
         if 'rpc' in extra:
             return "<blue>{time:YYYY-MM-DD HH:mm:ss.SSS}</blue> | " + extra['code_str'] + " | {extra[prefix]} | {extra[direction]} | {extra[arrow]} | {extra[uid_str]} | {extra[inputs]} | {extra[call_time]} | {extra[key_str]} | {extra[rpc_message]} | {extra[synapse]} \n"
         else:
             return "<blue>{time:YYYY-MM-DD HH:mm:ss.SSS}</blue> | <level>{level: ^16}</level> | {message}\n"
-   
+
     @classmethod
     def log_save_formatter(cls, record):
         extra = record['extra']
         if 'rpc' in extra:
             return "{time:YYYY-MM-DD HH:mm:ss.SSS} | " + extra['code_str'] + " | {extra[prefix]} | {extra[direction]} | {extra[arrow]} | {extra[uid_str]} | {extra[inputs]} | {extra[call_time]} | {extra[key_str]} | {extra[rpc_message]} \n"
         else:
             if cls.__trace_on__:
                 return "{time:YYYY-MM-DD HH:mm:ss.SSS} | <level>{level: ^16}</level> | <cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan> | {message}\n"
             else:
                 return "{time:YYYY-MM-DD HH:mm:ss.SSS} | <level>{level: ^16}</level> | {message}\n"
 
 
     @classmethod
-    def rpc_log( 
-                 cls, 
+    def rpc_log(
+                 cls,
                  axon: bool,
                  forward: bool,
                  is_response: bool,
                  code:int,
-                 call_time: float, 
-                 pubkey: str, 
-                 uid: int = None, 
-                 inputs:list = None, 
-                 outputs:list = None, 
+                 call_time: float,
+                 pubkey: str,
+                 uid: int = None,
+                 inputs:list = None,
+                 outputs:list = None,
                  message:str = '',
                  synapse:'bittensor.Synapse' = None
         ):
-        """ Debug logging for the communication between endpoints with axon/dendrite 
+        """ Debug logging for the communication between endpoints with axon/dendrite
         """
 
         if axon:
             prefix = "Synapse"
         else:
             prefix = "Dendrite"
         prefix = prefix.center(len('Dendrite'))
@@ -256,15 +256,15 @@
             direction = "Backward"
         direction = direction.center(len('Backward'))
 
         if is_response:
             arrow = "<---"
         else:
             arrow = "--->"
-        
+
         key_str = "{}".format( pubkey )
         call_time_str = "{:.2f}s".format(call_time).center(6)
 
         if uid != None:
             uid_str = str(uid).center(5)
         else:
             uid_str = "-".center(5)
@@ -280,25 +280,25 @@
             inputs = str(list(inputs)) if inputs != None else '[x]'
         inputs = inputs.center(15)
 
         if synapse != None:
             synapse = codes.code_to_synapse(synapse)
 
         rpc_message = message if message != None else 'None'
-        logger.debug( 
-                    'rpc', 
-                    rpc=True, 
-                    prefix=prefix, 
-                    direction=direction, 
-                    arrow=arrow, 
-                    call_time = call_time_str, 
-                    uid_str=uid_str, 
-                    key_str=key_str, 
-                    code_str=code_str, 
-                    inputs = inputs, 
+        logger.debug(
+                    'rpc',
+                    rpc=True,
+                    prefix=prefix,
+                    direction=direction,
+                    arrow=arrow,
+                    call_time = call_time_str,
+                    uid_str=uid_str,
+                    key_str=key_str,
+                    code_str=code_str,
+                    inputs = inputs,
                     rpc_message = rpc_message,
                     synapse = synapse
         )
 
     @classmethod
     def _format( cls, prefix:object, sufix:object = None ):
         """ Format logging message
@@ -313,15 +313,15 @@
         else:
             sufix = ""
         log_msg = str( prefix ).ljust(30) + str( sufix )
         return _remove_loguru_ansi_directive( log_msg )
 
     @classmethod
     def success( cls, prefix:object, sufix:object = None ):
-        """ Success logging 
+        """ Success logging
         """
         if not cls.__has_been_inited__: cls()
         logger.success( cls._format( prefix, sufix ) )
 
     @classmethod
     def warning( cls, prefix:object, sufix:object = None ):
         """ Warning logging
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_metagraph/__init__.py` & `bittensor-5.0.0/bittensor/_metagraph/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,61 +1,56 @@
 """ Maintains chain state as a torch.nn.Module.
 """
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import os
-import json
 import torch
 import bittensor
 
-import torch.nn.functional as f
-import bittensor.utils.networking as net
-
 from os import listdir
-from os.path import isfile, join
-from bittensor import Balance
-from typing import List, Optional, Dict, Union
+from os.path import join
+from typing import List, Optional
 
 
 # Return directory path from network and netuid
-def get_save_dir(  network: str, netuid: int ) -> str: 
+def get_save_dir(  network: str, netuid: int ) -> str:
     return os.path.expanduser(f"~/.bittensor/metagraphs/network-{str(network)}/netuid-{str(netuid)}/")
 
 def latest_block_path( dir_path: str ) -> int:
         latest_block = -1
         latest_file_full_path = None
         for filename in listdir(dir_path):
             full_path_filename = os.path.expanduser(join(dir_path, filename))
             try:
                 block_number = int(filename.split('-')[1].split('.')[0])
                 if block_number > latest_block:
                     latest_block = block_number
                     latest_file_full_path = full_path_filename
             except Exception as e:
                 pass
-        if not latest_file_full_path: 
+        if not latest_file_full_path:
             raise ValueError( f"Metagraph not found at: {dir_path}" )
         else:
             return latest_file_full_path
-        
+
 class metagraph( torch.nn.Module ):
 
     @property
     def S(self) -> torch.FloatTensor: return self.total_stake
     @property
     def R(self) -> torch.FloatTensor: return self.ranks
     @property
@@ -78,20 +73,20 @@
     def hotkeys( self ) -> List[str]: return [ axon.hotkey for axon in self.axons ]
     @property
     def coldkeys( self ) -> List[str]: return [ axon.coldkey for axon in self.axons ]
     @property
     def addresses( self ) -> List[str]: return [ axon.ip_str() for axon in self.axons ]
 
     def __str__(self): return "Metagraph(netuid:{}, n:{}, block:{}, network:{})".format(self.netuid, self.n.item(), self.block.item(), self.network)
-        
+
     def __repr__(self): return self.__str__()
 
     def metadata(self) -> dict: return {"netuid": self.netuid, "n": self.n.item(), "block": self.block.item(), "network": self.network, "version": bittensor.__version__ }
 
-    def __init__(self, netuid: int, network: str = 'finney', lite:bool = True, sync: bool = True ) -> 'metagraph':    
+    def __init__(self, netuid: int, network: str = 'finney', lite: bool = True, sync: bool = True ) -> 'metagraph':
         super(metagraph, self).__init__()
         self.netuid = netuid
         self.network = network
         self.version = torch.nn.Parameter( torch.tensor( [ bittensor.__version_as_int__ ], dtype=torch.int64), requires_grad=False )
         self.n = torch.nn.Parameter( torch.tensor( [0], dtype=torch.int64), requires_grad = False )
         self.block = torch.nn.Parameter( torch.tensor( [0], dtype=torch.int64), requires_grad = False )
         self.stake = torch.nn.Parameter( torch.tensor( [], dtype=torch.float32 ), requires_grad=False )
@@ -136,45 +131,53 @@
         self.validator_trust = torch.nn.Parameter( torch.tensor( [ neuron.validator_trust for neuron in self.neurons ], dtype=torch.float32 ), requires_grad=False )
         self.total_stake = torch.nn.Parameter( torch.tensor( [ neuron.total_stake.tao for neuron in self.neurons ], dtype=torch.float32 ), requires_grad=False )
         self.stake = torch.nn.Parameter( torch.tensor( [ neuron.stake for neuron in self.neurons ], dtype=torch.float32 ), requires_grad=False )
         self.axons = [ n.axon_info for n in self.neurons ]
         if not lite:
             weights_array = []
             for n in self.neurons:
-                w_uids, w_weights = zip(*n.weights)
-                weights_array.append( bittensor.utils.weight_utils.convert_weight_uids_and_vals_to_tensor( len(self.neurons), w_uids, w_weights ).tolist() )
-            self.weights = torch.nn.Parameter( torch.stack( weights_array ), requires_grad=False )
+                if len(n.weights) == 0:
+                    weights_array.append( torch.zeros( len( self.neurons ) ) )
+                else:
+                    w_uids, w_weights = zip(*n.weights)
+                    weights_array.append( bittensor.utils.weight_utils.convert_weight_uids_and_vals_to_tensor( len(self.neurons), w_uids, w_weights ) )
+            self.weights = torch.nn.Parameter( torch.stack( weights_array ), requires_grad=False ) if len( weights_array ) else torch.nn.Parameter()
+            if len(weights_array) == 0:
+                bittensor.logging.warning("Empty weights_array on metagraph.sync(). The 'weights' tensor is empty.")
         if not lite:
             bonds_array = []
             for n in self.neurons:
-                b_uids, b_bonds = zip(*n.bonds)
-                bonds_array.append( bittensor.utils.weight_utils.convert_bond_uids_and_vals_to_tensor( len(self.neurons), b_uids, b_bonds ).tolist() )
-            self.bonds = torch.nn.Parameter( torch.stack( bonds_array ), requires_grad=False )
+                if len(n.bonds) == 0:
+                    bonds_array.append( torch.zeros( len( self.neurons ) ) )
+                else:
+                    b_uids, b_bonds = zip(*n.bonds)
+                    bonds_array.append( bittensor.utils.weight_utils.convert_bond_uids_and_vals_to_tensor( len(self.neurons), b_uids, b_bonds ) )
+            self.bonds = torch.nn.Parameter( torch.stack( bonds_array ), requires_grad=False ) if len( bonds_array ) else torch.nn.Parameter()
+            if len(bonds_array) == 0:
+                bittensor.logging.warning("Empty bonds_array on metagraph.sync(). The 'bonds' tensor is empty.")
 
     def save( self ) -> 'metagraph':
         r""" Saves this metagraph object's state_dict under bittensor root dir."""
         save_directory = get_save_dir( self.network, self.netuid  )
         os.makedirs( save_directory, exist_ok=True )
         graph_file = save_directory + f'/block-{self.block.item()}.pt'
         state_dict = self.state_dict()
         state_dict['axons'] = self.axons
-        torch.save(state_dict, graph_file) 
+        torch.save(state_dict, graph_file)
         state_dict = torch.load( graph_file )
         return self
 
     def load( self ) -> 'metagraph':
         r""" Loads this metagraph object's state_dict from bittensor root dir. """
         self.load_from_path( get_save_dir( self.network, self.netuid ) )
-    
+
     def load_from_path( self, dir_path:str ) -> 'metagraph':
         r""" Loads this metagraph object with state_dict under the specified path."""
         graph_file = latest_block_path( dir_path )
         state_dict = torch.load( graph_file )
-        # self.info = bittensor.SubnetInfo.from_parameter_dict( state_dict['info'] ) if 'info' in state_dict else None
-        # self.version = torch.nn.Parameter( state_dict['version'], requires_grad=False )
         self.n = torch.nn.Parameter( state_dict['n'], requires_grad=False )
         self.block = torch.nn.Parameter( state_dict['block'], requires_grad=False )
         self.uids = torch.nn.Parameter( state_dict['uids'], requires_grad=False )
         self.stake = torch.nn.Parameter( state_dict['stake'], requires_grad=False )
         self.total_stake = torch.nn.Parameter( state_dict['total_stake'], requires_grad=False )
         self.ranks = torch.nn.Parameter( state_dict['ranks'], requires_grad=False )
         self.trust = torch.nn.Parameter( state_dict['trust'], requires_grad=False )
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_prometheus/__init__.py` & `bittensor-5.0.0/bittensor/_prometheus/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
 Create and init the config class, which manages the config of different bittensor modules.
 """
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import os
 import argparse
 import bittensor
 from typing import List, Callable, Union
 from prometheus_client import start_http_server
@@ -41,15 +41,15 @@
         def __str__(self):
             return self.value
 
     # Prometheus Global state.
     port: int = None
     started: bool = False
 
-    def __new__( 
+    def __new__(
         cls,
         wallet: 'bittensor.wallet',
         netuid: int,
         config: 'bittensor.config' = None,
         port: int = None,
         level: Union[str, "prometheus.level"] = None,
         network: str = None,
@@ -65,46 +65,46 @@
                     network uid to serve on.
                 config (:obj:`bittensor.Config`, `optional`, defaults to bittensor.prometheus.config()):
                     A config namespace object created by calling bittensor.prometheus.config()
                 port (:obj:`int`, `optional`, defaults to bittensor.defaults.prometheus.port ):
                     The port to run the prometheus DB on, this uniquely identifies the prometheus DB.
                 level (:obj:`prometheus.level`, `optional`, defaults to bittensor.defaults.prometheus.level ):
                     Prometheus logging level. If OFF, the prometheus DB is not initialized.
-                subtensor (:obj:`bittensor.Subtensor`, `optional`): 
+                subtensor (:obj:`bittensor.Subtensor`, `optional`):
                     Chain connection through which to serve.
                 network (default='local', type=str)
                     If subtensor is not set, uses this network flag to create the subtensor connection.
                 chain_endpoint (default=None, type=str)
                     Overrides the network argument if not set.
         """
         if config == None:
             config = prometheus.config()
 
         if isinstance(level, prometheus.level):
             level = level.name # Convert ENUM to str.
 
-        if subtensor == None: subtensor = bittensor.subtensor( network = network, chain_endpoint = chain_endpoint) 
-        
+        if subtensor == None: subtensor = bittensor.subtensor( network = network, chain_endpoint = chain_endpoint)
+
         config.prometheus.port = port if port != None else config.prometheus.port
         config.prometheus.level = level if level != None else config.prometheus.level
 
         if isinstance(config.prometheus.level, str):
             config.prometheus.level = config.prometheus.level.upper() # Convert str to upper case.
-        
+
         cls.check_config( config )
 
         return cls.serve(
             cls,
             wallet = wallet,
             netuid = netuid,
             subtensor = subtensor,
             port = config.prometheus.port,
             level = config.prometheus.level,
         )
-        
+
     def serve(cls, wallet, subtensor, netuid, port, level) -> bool:
         if level == prometheus.level.OFF.name: # If prometheus is off, return true.
             logger.success('Prometheus:'.ljust(20) + '<red>OFF</red>')
             return True
         else:
             # Serve prometheus. Not OFF
             serve_success = subtensor.serve_prometheus(
@@ -146,22 +146,22 @@
 
     @classmethod
     def add_args(cls, parser: argparse.ArgumentParser, prefix: str = None ):
         """ Accept specific arguments from parser
         """
         prefix_str = '' if prefix == None else prefix + '.'
         try:
-            parser.add_argument('--' + prefix_str + 'prometheus.port',  type=int, required=False, default = bittensor.defaults.prometheus.port, 
+            parser.add_argument('--' + prefix_str + 'prometheus.port',  type=int, required=False, default = bittensor.defaults.prometheus.port,
                 help='''Prometheus serving port.''')
             parser.add_argument(
-                '--' + prefix_str + 'prometheus.level', 
+                '--' + prefix_str + 'prometheus.level',
                 required = False,
-                type = str, 
+                type = str,
                 choices = [l.name for l in list(prometheus.level)],
-                default = bittensor.defaults.prometheus.level, 
+                default = bittensor.defaults.prometheus.level,
                 help = '''Prometheus logging level. <OFF | INFO | DEBUG>''')
         except argparse.ArgumentError as e:
             pass
 
     @classmethod
     def add_defaults(cls, defaults):
         """ Adds parser defaults to object from enviroment variables.
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_proto/bittensor_pb2.py` & `bittensor-5.0.0/bittensor/_proto/bittensor_pb2.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_proto/bittensor_pb2_grpc.py` & `bittensor-5.0.0/bittensor/_proto/bittensor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_serializer/__init__.py` & `bittensor-5.0.0/bittensor/_serializer/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """ An interface for serializing and deserializing bittensor tensors"""
 
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import torch
 import numpy as np
 import bittensor
 from typing import Tuple, List, Union, Optional
 
@@ -34,29 +34,29 @@
         """ Raised during deserialization """
 
     class NoSerializerForEnum (Exception):
         """ Raised if there is no serializer for the passed type """
 
     class SerializationTypeNotImplementedException (Exception):
         """ Raised if serialization/deserialization is not implemented for the passed object type """
-    
+
     def __new__(cls, serializer_type: bittensor.proto.Serializer = bittensor.proto.Serializer.MSGPACK ) -> 'bittensor.Serializer':
-        r"""Returns the correct serializer object for the passed Serializer enum. 
+        r"""Returns the correct serializer object for the passed Serializer enum.
 
             Args:
-                serializer_type (:obj:`bittensor.proto.Serializer`, `required`): 
+                serializer_type (:obj:`bittensor.proto.Serializer`, `required`):
                     The serializer_type ENUM from bittensor.proto.
 
             Returns:
-                Serializer: (obj: `bittensor.Serializer`, `required`): 
+                Serializer: (obj: `bittensor.Serializer`, `required`):
                     The bittensor serializer/deserialzer for the passed type.
 
             Raises:
-                NoSerializerForEnum: (Exception): 
-                    Raised if the passed there is no serialzier for the passed type. 
+                NoSerializerForEnum: (Exception):
+                    Raised if the passed there is no serialzier for the passed type.
         """
         # WARNING: the pickle serializer is not safe. Should be removed in future verions.
         # if serializer_type == bittensor.proto.Serializer.PICKLE:
         #     return PyTorchPickleSerializer()
         if serializer_type == bittensor.proto.Serializer.MSGPACK:
             return serializer_impl.MSGPackSerializer()
         elif serializer_type == bittensor.proto.Serializer.CMPPACK:
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_serializer/serializer_impl.py` & `bittensor-5.0.0/bittensor/_serializer/serializer_impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """ An interface for serializing and deserializing bittensor tensors"""
 
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import torch
 import msgpack
 import msgpack_numpy
 from typing import Tuple, List, Union, Optional
 
@@ -36,32 +36,32 @@
         torch_proto = bittensor.proto.Tensor(version= bittensor.__version_as_int__)
         return torch_proto
 
     def serialize (self, tensor_obj: object, from_type: int = bittensor.proto.TensorType.TORCH ) -> bittensor.proto.Tensor:
         """Serializes a torch object to bittensor.proto.Tensor wire format.
 
         Args:
-            tensor_obj (:obj:`object`, `required`): 
+            tensor_obj (:obj:`object`, `required`):
                 general tensor object i.e. torch.Tensor or tensorflow.Tensor
 
-            from_type (`obj`: bittensor.proto.TensorType, `Optional`): 
+            from_type (`obj`: bittensor.proto.TensorType, `Optional`):
                 Serialization from this type. i.e. bittensor.proto.TensorType.TORCH or bittensor.proto.TensorType.TENSORFLOW
 
         Returns:
-            tensor_pb2: (obj: `bittensor.proto.Tensor`, `Optional`): 
-                Serialized tensor as bittensor.proto.proto. 
+            tensor_pb2: (obj: `bittensor.proto.Tensor`, `Optional`):
+                Serialized tensor as bittensor.proto.proto.
 
         Raises:
             SerializationTypeNotImplementedException (Exception):
                 Raised if the serializer does not implement the conversion between the passed type and a bittensor.proto.Tensor
 
-            SerializationException: (Exception): 
+            SerializationException: (Exception):
                 Raised when the subclass serialization throws an error for the passed object.
         """
-        # TODO (const): add deserialization types for torch -> tensorflow 
+        # TODO (const): add deserialization types for torch -> tensorflow
         if from_type == bittensor.proto.TensorType.TORCH:
             return self.serialize_from_torch( torch_tensor = tensor_obj )
 
         elif from_type == bittensor.proto.TensorType.NUMPY:
             return self.serialize_from_numpy( numpy_tensor = tensor_obj )
 
         elif from_type == bittensor.proto.TensorType.TENSORFLOW:
@@ -72,32 +72,32 @@
 
         raise NotImplementedError
 
     def deserialize (self, tensor_pb2: bittensor.proto.Tensor, to_type: int = bittensor.proto.TensorType.TORCH ) -> object:
         """Serializes a torch object to bittensor.proto.Tensor wire format.
 
         Args:
-            tensor_pb2 (`obj`: bittensor.proto.Tensor, `required`): 
-                Serialized tensor as bittensor.proto.proto. 
+            tensor_pb2 (`obj`: bittensor.proto.Tensor, `required`):
+                Serialized tensor as bittensor.proto.proto.
 
-            to_type (`obj`: bittensor.proto.TensorType, `required`): 
+            to_type (`obj`: bittensor.proto.TensorType, `required`):
                 Deserialization to this type. i.e. bittensor.proto.TensorType.TORCH or bittensor.proto.TensorType.TENSORFLOW
 
         Returns:
-            tensor_obj (:obj:`torch.FloatTensor`, `required`): 
+            tensor_obj (:obj:`torch.FloatTensor`, `required`):
                 tensor object of type from_type in bittensor.proto.TensorType
 
         Raises:
             SerializationTypeNotImplementedException (Exception):
                 Raised if the serializer does not implement the conversion between the pb2 and the passed type.
-          
-            DeserializationException: (Exception): 
+
+            DeserializationException: (Exception):
                 Raised when the subclass deserializer throws an error for the passed object.
         """
-        # TODO (const): add deserialization types for torch -> tensorflow 
+        # TODO (const): add deserialization types for torch -> tensorflow
         if to_type == bittensor.proto.TensorType.TORCH:
             return self.deserialize_to_torch( tensor_pb2 )
 
         elif to_type == bittensor.proto.TensorType.NUMPY:
             return self.deserialize_to_numpy( tensor_pb2 )
 
         elif to_type == bittensor.proto.TensorType.TENSORFLOW:
@@ -109,15 +109,15 @@
     def serialize_from_tensorflow( self, tensorflow_tensor: torch.Tensor ) -> bittensor.proto.Tensor:
         """ tensorflow -> bittensor.proto.Tensor """
         raise bittensor.serializer.SerializationTypeNotImplementedException
 
     def serialize_from_torch( self, torch_tensor: torch.Tensor ) -> bittensor.proto.Tensor:
         """ torch -> bittensor.proto.Tensor """
         raise bittensor.serializer.SerializationTypeNotImplementedException
-    
+
     def serialize_from_numpy( self, numpy_tensor: torch.Tensor ) -> bittensor.proto.Tensor:
         """ numpy -> bittensor.proto.Tensor """
         raise bittensor.serializer.SerializationTypeNotImplementedException
 
     def deserialize_to_torch( self, tensor_pb2: bittensor.proto.Tensor ) -> torch.Tensor:
         """ bittensor.proto.Tensor -> torch """
         raise bittensor.serializer.SerializationTypeNotImplementedException
@@ -134,19 +134,19 @@
 class MSGPackSerializer( Serializer ):
     """ Make conversion between torch and bittensor.proto.torch
     """
     def serialize_from_torch( self, torch_tensor: torch.Tensor ) -> bittensor.proto.Tensor:
         """ Serializes a torch.Tensor to an bittensor Tensor proto.
 
         Args:
-            torch_tensor (torch.Tensor): 
+            torch_tensor (torch.Tensor):
                 Torch tensor to serialize.
         Returns:
-            bittensor.proto.Tensor: 
-                The serialized torch tensor as bittensor.proto.proto. 
+            bittensor.proto.Tensor:
+                The serialized torch tensor as bittensor.proto.proto.
         """
         dtype = bittensor.serializer.torch_dtype_to_bittensor_dtype(torch_tensor.dtype)
         shape = list(torch_tensor.shape)
         torch_numpy = torch_tensor.cpu().detach().numpy().copy()
         data_buffer = msgpack.packb(torch_numpy, default=msgpack_numpy.encode)
         torch_proto = bittensor.proto.Tensor (
                                     version = bittensor.__version_as_int__,
@@ -159,19 +159,19 @@
                                 )
         return torch_proto
 
     def deserialize_to_torch(self, torch_proto: bittensor.proto.Tensor) -> torch.Tensor:
         """Deserializes an bittensor.proto.Tensor to a torch.Tensor object.
 
         Args:
-            torch_proto (bittensor.proto.Tensor): 
+            torch_proto (bittensor.proto.Tensor):
                 Proto containing torch tensor to derserialize.
 
         Returns:
-            torch.Tensor: 
+            torch.Tensor:
                 Deserialized torch tensor.
         """
         dtype = bittensor.serializer.bittensor_dtype_to_torch_dtype(torch_proto.dtype)
         shape = tuple(torch_proto.shape)
         numpy_object = msgpack.unpackb(torch_proto.buffer, object_hook=msgpack_numpy.decode).copy()
         torch_object = torch.as_tensor(numpy_object).view(shape).requires_grad_(torch_proto.requires_grad)
         return torch_object.type(dtype)
@@ -180,19 +180,19 @@
 class CMPPackSerializer( Serializer ):
     """ Make conversion between torch and bittensor.proto.torch in float16
     """
     def serialize_from_torch(self, torch_tensor: torch.Tensor ) -> bittensor.proto.Tensor:
         """ Serializes a torch.Tensor to an bittensor Tensor proto in float16
 
         Args:
-            torch_tensor (torch.Tensor): 
+            torch_tensor (torch.Tensor):
                 Torch tensor to serialize.
         Returns:
-            bittensor.proto.Tensor: 
-                The serialized torch tensor as bittensor.proto.proto. 
+            bittensor.proto.Tensor:
+                The serialized torch tensor as bittensor.proto.proto.
         """
         dtype = bittensor.serializer.torch_dtype_to_bittensor_dtype(torch_tensor.dtype)
         shape = list(torch_tensor.shape)
         torch_numpy = torch_tensor.cpu().detach().half().numpy().copy()
         data_buffer = msgpack.packb(torch_numpy, default=msgpack_numpy.encode)
         torch_proto = bittensor.proto.Tensor (
                                     version = bittensor.__version_as_int__,
@@ -205,19 +205,19 @@
                                 )
         return torch_proto
 
     def deserialize_to_torch(self, torch_proto: bittensor.proto.Tensor) -> torch.Tensor:
         """Deserializes an bittensor.proto.Tensor to a torch.Tensor object.
 
         Args:
-            torch_proto (bittensor.proto.Tensor): 
+            torch_proto (bittensor.proto.Tensor):
                 Proto containing torch tensor to derserialize.
 
         Returns:
-            torch.Tensor: 
+            torch.Tensor:
                 Deserialized torch tensor.
         """
         dtype = bittensor.serializer.bittensor_dtype_to_torch_dtype(torch_proto.dtype)
         shape = tuple(torch_proto.shape)
         numpy_object = msgpack.unpackb(torch_proto.buffer, object_hook=msgpack_numpy.decode).copy()
         torch_object = torch.as_tensor(numpy_object).view(shape).requires_grad_(torch_proto.requires_grad)
         return torch_object.type(dtype)
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_subtensor/__init__.py` & `bittensor-5.0.0/bittensor/_subtensor/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 # Copyright © 2023 Opentensor Foundation
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 
 import os
 import copy
 import argparse
 import bittensor
@@ -32,124 +32,108 @@
 GLOBAL_SUBTENSOR_MOCK_PROCESS_NAME = 'node-subtensor'
 
 class subtensor:
     """Factory Class for both bittensor.Subtensor and Mock_Subtensor Classes
 
     The Subtensor class handles interactions with the substrate subtensor chain.
     By default, the Subtensor class connects to the Finney which serves as the main bittensor network.
-    
     """
-    
+
     def __new__(
-            cls, 
+            cls,
             config: 'bittensor.config' = None,
             network: str = None,
             chain_endpoint: str = None,
             _mock: bool = None,
         ) -> 'bittensor.Subtensor':
         r""" Initializes a subtensor chain interface.
             Args:
-                config (:obj:`bittensor.Config`, `optional`): 
+                config (:obj:`bittensor.Config`, `optional`):
                     bittensor.subtensor.config()
                 network (default='local', type=str)
                     The subtensor network flag. The likely choices are:
                             -- local (local running network)
                             -- finney (main network)
                             -- mock (mock network for testing.)
-                    If this option is set it overloads subtensor.chain_endpoint with 
+                    If this option is set it overloads subtensor.chain_endpoint with
                     an entry point node from that network.
                 chain_endpoint (default=None, type=str)
                     The subtensor endpoint flag. If set, overrides the network argument.
                 _mock (bool, `optional`):
                     Returned object is mocks the underlying chain connection.
         """
         if config == None: config = subtensor.config()
         config = copy.deepcopy( config )
 
         # Returns a mocked connection with a background chain connection.
         config.subtensor._mock = _mock if _mock != None else config.subtensor._mock
         if config.subtensor._mock == True or network == 'mock' or config.subtensor.get('network', bittensor.defaults.subtensor.network) == 'mock':
             config.subtensor._mock = True
             return subtensor_mock.mock_subtensor.mock()
-        
+
         # Determine config.subtensor.chain_endpoint and config.subtensor.network config.
         # If chain_endpoint is set, we override the network flag, otherwise, the chain_endpoint is assigned by the network.
         # Argument importance: chain_endpoint > network > config.subtensor.chain_endpoint > config.subtensor.network
-       
+
         # Select using chain_endpoint arg.
         if chain_endpoint != None:
             config.subtensor.chain_endpoint = chain_endpoint
             if network != None:
                 config.subtensor.network = network
             else:
                 config.subtensor.network = config.subtensor.get('network', bittensor.defaults.subtensor.network)
-            
+
         # Select using network arg.
         elif network != None:
             config.subtensor.chain_endpoint = subtensor.determine_chain_endpoint( network )
             config.subtensor.network = network
-            
+
         # Select using config.subtensor.chain_endpoint
         elif config.subtensor.chain_endpoint != None:
             config.subtensor.chain_endpoint = config.subtensor.chain_endpoint
             config.subtensor.network = config.subtensor.get('network', bittensor.defaults.subtensor.network)
-         
+
         # Select using config.subtensor.network
         elif config.subtensor.get('network', bittensor.defaults.subtensor.network) != None:
             config.subtensor.chain_endpoint = subtensor.determine_chain_endpoint( config.subtensor.get('network', bittensor.defaults.subtensor.network) )
             config.subtensor.network = config.subtensor.get('network', bittensor.defaults.subtensor.network)
-            
+
         # Fallback to defaults.
         else:
             config.subtensor.chain_endpoint = subtensor.determine_chain_endpoint( bittensor.defaults.subtensor.network )
             config.subtensor.network = bittensor.defaults.subtensor.network
-        
+
         # make sure it's wss:// or ws://
         # If it's bellagene (parachain testnet) then it has to be wss
         endpoint_url: str = config.subtensor.chain_endpoint
-        
+
         # make sure formatting is good
         endpoint_url = bittensor.utils.networking.get_formatted_ws_endpoint_url(endpoint_url)
-        
-        
 
         subtensor.check_config( config )
         network = config.subtensor.get('network', bittensor.defaults.subtensor.network)
-        if network == 'nakamoto':
-            substrate = SubstrateInterface(
-                ss58_format = bittensor.__ss58_format__,
-                use_remote_preset=True,
-                url = endpoint_url,
-            )
-            # Use nakamoto-specific subtensor.
-            return Nakamoto_subtensor( 
-                substrate = substrate,
-                network = config.subtensor.get('network', bittensor.defaults.subtensor.network),
-                chain_endpoint = config.subtensor.chain_endpoint,
-            )
-        else:
-            substrate = SubstrateInterface(
-                ss58_format = bittensor.__ss58_format__,
-                use_remote_preset=True,
-                url = endpoint_url,
-                type_registry=bittensor.__type_registry__
-            )
-            return subtensor_impl.Subtensor( 
-                substrate = substrate,
-                network = config.subtensor.get('network', bittensor.defaults.subtensor.network),
-                chain_endpoint = config.subtensor.chain_endpoint,
-            )
+        substrate = SubstrateInterface(
+            ss58_format = bittensor.__ss58_format__,
+            use_remote_preset=True,
+            url = endpoint_url,
+            type_registry=bittensor.__type_registry__
+        )
+        return subtensor_impl.Subtensor(
+            substrate = substrate,
+            network = config.subtensor.get('network', bittensor.defaults.subtensor.network),
+            chain_endpoint = config.subtensor.chain_endpoint,
+        )
 
-    @staticmethod   
+    @staticmethod
     def config() -> 'bittensor.Config':
         parser = argparse.ArgumentParser()
         subtensor.add_args( parser )
         return bittensor.config( parser )
 
-    @classmethod   
+    @classmethod
     def help(cls):
         """ Print help to stdout
         """
         parser = argparse.ArgumentParser()
         cls.add_args( parser )
         print (cls.__new__.__doc__)
         parser.print_help()
@@ -159,27 +143,27 @@
         prefix_str = '' if prefix == None else prefix + '.'
         try:
             parser.add_argument('--' + prefix_str + 'subtensor.network', default = bittensor.defaults.subtensor.network, type=str,
                                 help='''The subtensor network flag. The likely choices are:
                                         -- finney (main network)
                                         -- local (local running network)
                                         -- mock (creates a mock connection (for testing))
-                                    If this option is set it overloads subtensor.chain_endpoint with 
+                                    If this option is set it overloads subtensor.chain_endpoint with
                                     an entry point node from that network.
                                     ''')
-            parser.add_argument('--' + prefix_str + 'subtensor.chain_endpoint', default = bittensor.defaults.subtensor.chain_endpoint, type=str, 
+            parser.add_argument('--' + prefix_str + 'subtensor.chain_endpoint', default = bittensor.defaults.subtensor.chain_endpoint, type=str,
                                 help='''The subtensor endpoint flag. If set, overrides the --network flag.
-                                    ''')       
+                                    ''')
             parser.add_argument('--' + prefix_str + 'subtensor._mock', action='store_true', help='To turn on subtensor mocking for testing purposes.', default=bittensor.defaults.subtensor._mock)
             # registration args. Used for register and re-register and anything that calls register.
             parser.add_argument('--' + prefix_str + 'subtensor.register.num_processes', '-n', dest=prefix_str + 'subtensor.register.num_processes', help="Number of processors to use for registration", type=int, default=bittensor.defaults.subtensor.register.num_processes)
             parser.add_argument('--' + prefix_str + 'subtensor.register.update_interval', '--' + prefix_str + 'subtensor.register.cuda.update_interval', '--' + prefix_str + 'cuda.update_interval', '-u', help="The number of nonces to process before checking for next block during registration", type=int, default=bittensor.defaults.subtensor.register.update_interval)
             parser.add_argument('--' + prefix_str + 'subtensor.register.no_output_in_place', '--' + prefix_str + 'no_output_in_place', dest="subtensor.register.output_in_place", help="Whether to not ouput the registration statistics in-place. Set flag to disable output in-place.", action='store_false', required=False, default=bittensor.defaults.subtensor.register.output_in_place)
             parser.add_argument('--' + prefix_str + 'subtensor.register.verbose', help="Whether to ouput the registration statistics verbosely.", action='store_true', required=False, default=bittensor.defaults.subtensor.register.verbose)
-            
+
             ## Registration args for CUDA registration.
             parser.add_argument( '--' + prefix_str + 'subtensor.register.cuda.use_cuda', '--' + prefix_str + 'cuda', '--' + prefix_str + 'cuda.use_cuda', default=argparse.SUPPRESS, help='''Set flag to use CUDA to register.''', action="store_true", required=False )
             parser.add_argument( '--' + prefix_str + 'subtensor.register.cuda.no_cuda', '--' + prefix_str + 'no_cuda', '--' + prefix_str + 'cuda.no_cuda', dest=prefix_str + 'subtensor.register.cuda.use_cuda', default=argparse.SUPPRESS, help='''Set flag to not use CUDA for registration''', action="store_false", required=False )
 
             parser.add_argument( '--' + prefix_str + 'subtensor.register.cuda.dev_id', '--' + prefix_str + 'cuda.dev_id',  type=int, nargs='+', default=argparse.SUPPRESS, help='''Set the CUDA device id(s). Goes by the order of speed. (i.e. 0 is the fastest).''', required=False )
             parser.add_argument( '--' + prefix_str + 'subtensor.register.cuda.TPB', '--' + prefix_str + 'cuda.TPB', type=int, default=bittensor.defaults.subtensor.register.cuda.TPB, help='''Set the number of Threads Per Block for CUDA.''', required=False )
 
@@ -203,17 +187,17 @@
         defaults.subtensor.register.verbose = False
 
         defaults.subtensor.register.cuda = bittensor.Config()
         defaults.subtensor.register.cuda.dev_id = [0]
         defaults.subtensor.register.cuda.use_cuda = False
         defaults.subtensor.register.cuda.TPB = 256
 
-        
 
-    @staticmethod   
+
+    @staticmethod
     def check_config( config: 'bittensor.Config' ):
         assert config.subtensor
         #assert config.subtensor.network != None
         if config.subtensor.get('register') and config.subtensor.register.get('cuda'):
             assert all((isinstance(x, int) or isinstance(x, str) and x.isnumeric() ) for x in config.subtensor.register.cuda.get('dev_id', []))
 
             if config.subtensor.register.cuda.get('use_cuda', bittensor.defaults.subtensor.register.cuda.use_cuda):
@@ -224,21 +208,18 @@
 
                 if not is_cuda_available():
                     raise RuntimeError('CUDA registration is enabled but no CUDA devices are detected.')
 
 
     @staticmethod
     def determine_chain_endpoint(network: str):
-        if network == "nakamoto":
-            # Main network.
-            return bittensor.__nakamoto_entrypoint__
-        elif network == "finney": 
+        if network == "finney":
             # Kiru Finney stagin network.
             return bittensor.__finney_entrypoint__
-        elif network == "nobunaga": 
+        elif network == "nobunaga":
             # Staging network.
             return bittensor.__nobunaga_entrypoint__
         elif network == "bellagene":
             # Parachain test net
             return bittensor.__bellagene_entrypoint__
         elif network == "local":
             # Local chain.
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_subtensor/chain_data.py` & `bittensor-5.0.0/bittensor/_subtensor/chain_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # The MIT License (MIT)
 # Copyright © 2023 Opentensor Foundation
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 from dataclasses import dataclass
 from typing import List, Tuple, Dict, Optional, Any
 import bittensor
 from bittensor import Balance
 import torch
@@ -135,15 +135,15 @@
                 ["block", "u64"],
                 ["version", "u32"],
                 ["ip", "u128"],
                 ["port", "u16"],
                 ["ip_type", "u8"],
             ],
         },
-    }   
+    }
 }
 
 class ChainDataType(Enum):
     NeuronInfo = 1
     SubnetInfo = 2
     DelegateInfo = 3
     NeuronInfoLite = 4
@@ -183,15 +183,15 @@
     r"""
     Dataclass for neuron metadata.
     """
     hotkey: str
     coldkey: str
     uid: int
     netuid: int
-    active: int    
+    active: int
     stake: Balance
     # mapping of coldkey to amount staked to this Neuron
     stake_dict: Dict[str, Balance]
     total_stake: Balance
     rank: float
     emission: float
     incentive: float
@@ -227,35 +227,35 @@
         neuron_info_decoded['trust'] = bittensor.utils.U16_NORMALIZED_FLOAT(neuron_info_decoded['trust'])
         neuron_info_decoded['validator_trust'] = bittensor.utils.U16_NORMALIZED_FLOAT(neuron_info_decoded['validator_trust'])
         neuron_info_decoded['dividends'] = bittensor.utils.U16_NORMALIZED_FLOAT(neuron_info_decoded['dividends'])
         neuron_info_decoded['prometheus_info'] = PrometheusInfo.fix_decoded_values(neuron_info_decoded['prometheus_info'])
         neuron_info_decoded['axon_info'] = bittensor.axon_info.from_neuron_info( neuron_info_decoded )
 
         return cls(**neuron_info_decoded)
-    
+
     @classmethod
     def from_vec_u8(cls, vec_u8: List[int]) -> 'NeuronInfo':
         r""" Returns a NeuronInfo object from a vec_u8.
         """
         if len(vec_u8) == 0:
             return NeuronInfo._null_neuron()
-        
+
         decoded = from_scale_encoding(vec_u8, ChainDataType.NeuronInfo)
         if decoded is None:
             return NeuronInfo._null_neuron()
-        
+
         decoded = NeuronInfo.fix_decoded_values(decoded)
 
         return decoded
-    
+
     @classmethod
     def list_from_vec_u8(cls, vec_u8: List[int]) -> List['NeuronInfo']:
         r""" Returns a list of NeuronInfo objects from a vec_u8.
         """
-        
+
         decoded_list = from_scale_encoding(vec_u8, ChainDataType.NeuronInfo, is_vec=True)
         if decoded_list is None:
             return []
 
         decoded_list = [NeuronInfo.fix_decoded_values(decoded) for decoded in decoded_list]
         return decoded_list
 
@@ -302,27 +302,27 @@
             neuron.rank = neuron.rank / U16_MAX
             neuron.trust = neuron.trust / U16_MAX
             neuron.consensus = neuron.consensus / U16_MAX
             neuron.validator_trust = neuron.validator_trust / U16_MAX
             neuron.incentive = neuron.incentive / U16_MAX
             neuron.dividends = neuron.dividends / U16_MAX
             neuron.emission = neuron.emission / RAOPERTAO
-                
+
             return neuron
-        
+
 @dataclass
 class NeuronInfoLite:
     r"""
     Dataclass for neuron metadata, but without the weights and bonds.
     """
     hotkey: str
     coldkey: str
     uid: int
     netuid: int
-    active: int    
+    active: int
     stake: Balance
     # mapping of coldkey to amount staked to this Neuron
     stake_dict: Dict[str, Balance]
     total_stake: Balance
     rank: float
     emission: float
     incentive: float
@@ -358,35 +358,35 @@
         neuron_info_decoded['consensus'] = bittensor.utils.U16_NORMALIZED_FLOAT(neuron_info_decoded['consensus'])
         neuron_info_decoded['trust'] = bittensor.utils.U16_NORMALIZED_FLOAT(neuron_info_decoded['trust'])
         neuron_info_decoded['validator_trust'] = bittensor.utils.U16_NORMALIZED_FLOAT(neuron_info_decoded['validator_trust'])
         neuron_info_decoded['dividends'] = bittensor.utils.U16_NORMALIZED_FLOAT(neuron_info_decoded['dividends'])
         neuron_info_decoded['prometheus_info'] = PrometheusInfo.fix_decoded_values(neuron_info_decoded['prometheus_info'])
         neuron_info_decoded['axon_info'] = bittensor.axon_info.from_neuron_info(neuron_info_decoded)
         return cls(**neuron_info_decoded)
-    
+
     @classmethod
     def from_vec_u8(cls, vec_u8: List[int]) -> 'NeuronInfoLite':
         r""" Returns a NeuronInfoLite object from a vec_u8.
         """
         if len(vec_u8) == 0:
             return NeuronInfoLite._null_neuron()
-        
+
         decoded = from_scale_encoding(vec_u8, ChainDataType.NeuronInfoLite)
         if decoded is None:
             return NeuronInfoLite._null_neuron()
-        
+
         decoded = NeuronInfoLite.fix_decoded_values(decoded)
 
         return decoded
-    
+
     @classmethod
     def list_from_vec_u8(cls, vec_u8: List[int]) -> List['NeuronInfoLite']:
         r""" Returns a list of NeuronInfoLite objects from a vec_u8.
         """
-        
+
         decoded_list = from_scale_encoding(vec_u8, ChainDataType.NeuronInfoLite, is_vec=True)
         if decoded_list is None:
             return []
 
         decoded_list = [NeuronInfoLite.fix_decoded_values(decoded) for decoded in decoded_list]
         return decoded_list
 
@@ -433,15 +433,15 @@
             neuron.rank = neuron.rank / U16_MAX
             neuron.trust = neuron.trust / U16_MAX
             neuron.consensus = neuron.consensus / U16_MAX
             neuron.validator_trust = neuron.validator_trust / U16_MAX
             neuron.incentive = neuron.incentive / U16_MAX
             neuron.dividends = neuron.dividends / U16_MAX
             neuron.emission = neuron.emission / RAOPERTAO
-                
+
             return neuron
 
 @dataclass
 class axon_info:
     r"""
     Dataclass for axon info.
     """
@@ -455,15 +455,15 @@
     placeholder2: int
 
     @classmethod
     def fix_decoded_values(cls, axon_info_decoded: Dict) -> 'axon_info':
         r""" Returns an axon_info object from an axon_info_decoded dictionary.
         """
         axon_info_decoded['ip'] = bittensor.utils.networking.int_to_ip(int(axon_info_decoded['ip']))
-                                                                       
+
         return cls(**axon_info_decoded)
 
 @dataclass
 class PrometheusInfo:
     r"""
     Dataclass for prometheus info.
     """
@@ -474,15 +474,15 @@
     ip_type: int
 
     @classmethod
     def fix_decoded_values(cls, prometheus_info_decoded: Dict) -> 'PrometheusInfo':
         r""" Returns a PrometheusInfo object from a prometheus_info_decoded dictionary.
         """
         prometheus_info_decoded['ip'] = bittensor.utils.networking.int_to_ip(int(prometheus_info_decoded['ip']))
-        
+
         return cls(**prometheus_info_decoded)
 @dataclass
 class DelegateInfo:
     r"""
     Dataclass for delegate info.
     """
     hotkey_ss58: str # Hotkey of delegate
@@ -495,15 +495,15 @@
     return_per_1000: bittensor.Balance # Return per 1000 tao of the delegate over a day
     total_daily_return: bittensor.Balance # Total daily return of the delegate
 
     @classmethod
     def fix_decoded_values(cls, decoded: Any) -> 'DelegateInfo':
         r""" Fixes the decoded values.
         """
-        
+
         return cls(
             hotkey_ss58 = ss58_encode(decoded['delegate_ss58'], bittensor.__ss58_format__),
             owner_ss58 = ss58_encode(decoded['owner_ss58'], bittensor.__ss58_format__),
             take = bittensor.utils.U16_NORMALIZED_FLOAT(decoded['take']),
             nominators = [
                 (ss58_encode(nom[0], bittensor.__ss58_format__), Balance.from_rao(nom[1]))
                 for nom in decoded['nominators']
@@ -517,47 +517,47 @@
 
     @classmethod
     def from_vec_u8(cls, vec_u8: List[int]) -> Optional['DelegateInfo']:
         r""" Returns a DelegateInfo object from a vec_u8.
         """
         if len(vec_u8) == 0:
             return None
-        
+
         decoded = from_scale_encoding(vec_u8, ChainDataType.DelegateInfo)
 
         if decoded is None:
             return None
-        
+
         decoded = DelegateInfo.fix_decoded_values(decoded)
 
         return decoded
-    
+
     @classmethod
     def list_from_vec_u8(cls, vec_u8: List[int]) -> List['DelegateInfo']:
         r""" Returns a list of DelegateInfo objects from a vec_u8.
         """
         decoded = from_scale_encoding(vec_u8, ChainDataType.DelegateInfo, is_vec=True)
 
         if decoded is None:
             return []
-        
+
         decoded = [DelegateInfo.fix_decoded_values(d) for d in decoded]
 
         return decoded
-    
+
     @classmethod
     def delegated_list_from_vec_u8(cls, vec_u8: List[int]) -> List[Tuple['DelegateInfo', Balance]]:
         r""" Returns a list of Tuples of DelegateInfo objects, and Balance, from a vec_u8.
         This is the list of delegates that the user has delegated to, and the amount of stake delegated.
         """
         decoded = from_scale_encoding(vec_u8, ChainDataType.DelegatedInfo, is_vec=True)
 
         if decoded is None:
             return []
-        
+
         decoded = [(DelegateInfo.fix_decoded_values(d), Balance.from_rao(s)) for d, s in decoded]
 
         return decoded
 
 @dataclass
 class SubnetInfo:
     r"""
@@ -594,26 +594,26 @@
         if len(vec_u8) == 0:
             return None
 
         decoded = from_scale_encoding(vec_u8, ChainDataType.SubnetInfo)
 
         if decoded is None:
             return None
-        
+
         return SubnetInfo.fix_decoded_values(decoded)
-    
+
     @classmethod
     def list_from_vec_u8(cls, vec_u8: List[int]) -> List['SubnetInfo']:
         r""" Returns a list of SubnetInfo objects from a vec_u8.
         """
         decoded = from_scale_encoding(vec_u8, ChainDataType.SubnetInfo, is_vec=True, is_option=True)
 
         if decoded is None:
             return []
-        
+
         decoded = [SubnetInfo.fix_decoded_values(d) for d in decoded]
 
         return decoded
 
     @classmethod
     def fix_decoded_values(cls, decoded: Dict) -> 'SubnetInfo':
         r""" Returns a SubnetInfo object from a decoded SubnetInfo dictionary.
@@ -640,20 +640,20 @@
             modality = decoded['network_modality'],
             connection_requirements = {
                 str(int(netuid)): bittensor.utils.U16_NORMALIZED_FLOAT(int(req)) for netuid, req in decoded['network_connect']
             },
             emission_value= decoded['emission_values'],
             burn = Balance.from_rao(decoded['burn'])
         )
-    
+
     def to_parameter_dict( self ) -> 'torch.nn.ParameterDict':
         r""" Returns a torch tensor of the subnet info.
         """
-        return torch.nn.ParameterDict( 
+        return torch.nn.ParameterDict(
             self.__dict__
         )
-    
+
     @classmethod
     def from_parameter_dict( cls, parameter_dict: 'torch.nn.ParameterDict' ) -> 'SubnetInfo':
         r""" Returns a SubnetInfo object from a torch parameter_dict.
         """
         return cls( **dict(parameter_dict) )
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_subtensor/errors.py` & `bittensor-5.0.0/bittensor/_subtensor/errors.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # The MIT License (MIT)
 # Copyright © 2023 Opentensor Foundation
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 class ChainError(BaseException):
     r""" Base error for any chain related errors.
     """
     pass
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/__init__.py` & `bittensor-5.0.0/bittensor/_subtensor/extrinsics/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # The MIT License (MIT)
 # Copyright © 2023 Opentensor Foundation
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/delegation.py` & `bittensor-5.0.0/bittensor/_subtensor/extrinsics/delegation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 
-            
+
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 # Copyright © 2023 Opentensor Foundation
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import bittensor
 from ..errors import *
 from rich.prompt import Confirm
 from typing import List, Dict, Union, Optional
 from bittensor.utils.balance import Balance
 from .staking import __do_add_stake_single
 
 from loguru import logger
 logger = logger.opt(colors=True)
 
-def nominate_extrinsic( 
+def nominate_extrinsic(
     subtensor: 'bittensor.Subtensor',
-    wallet: 'bittensor.Wallet', 
-    wait_for_finalization: bool = False, 
-    wait_for_inclusion: bool = True 
+    wallet: 'bittensor.Wallet',
+    wait_for_finalization: bool = False,
+    wait_for_inclusion: bool = True
 ) -> bool:
     r""" Becomes a delegate for the hotkey.
     Args:
         wallet ( bittensor.Wallet ):
             The wallet to become a delegate for.
     Returns:
         success (bool):
@@ -79,28 +79,28 @@
         except Exception as e:
             bittensor.__console__.print(":cross_mark: [red]Failed[/red]: error:{}".format(e))
             bittensor.logging.warning(  prefix = 'Set weights', sufix = '<red>Failed: </red>' + str(e) )
             return False
 
     if response.is_success:
         return True
-    
+
     return False
 
 def do_delegation(
-        subtensor: 'bittensor.Subtensor', 
+        subtensor: 'bittensor.Subtensor',
         wallet: 'bittensor.wallet',
         delegate_ss58: str,
-        amount: 'bittensor.Balance', 
+        amount: 'bittensor.Balance',
         wait_for_inclusion: bool = True,
         wait_for_finalization: bool = False,
     ) -> bool:
     with subtensor.substrate as substrate:
         call = substrate.compose_call(
-        call_module='SubtensorModule', 
+        call_module='SubtensorModule',
         call_function='add_stake',
         call_params={
             'hotkey': delegate_ss58,
             'amount_staked': amount.rao
             }
         )
         extrinsic = substrate.create_signed_extrinsic( call = call, keypair = wallet.coldkey )
@@ -111,24 +111,24 @@
         response.process_events()
         if response.is_success:
             return True
         else:
             raise StakeError(response.error_message)
 
 def do_undelegation(
-        subtensor: 'bittensor.Subtensor', 
+        subtensor: 'bittensor.Subtensor',
         wallet: 'bittensor.wallet',
         delegate_ss58: str,
-        amount: 'bittensor.Balance', 
+        amount: 'bittensor.Balance',
         wait_for_inclusion: bool = True,
         wait_for_finalization: bool = False,
     ) -> bool:
     with subtensor.substrate as substrate:
         call = substrate.compose_call(
-        call_module='SubtensorModule', 
+        call_module='SubtensorModule',
         call_function='remove_stake',
         call_params={
             'hotkey': delegate_ss58,
             'amount_unstaked': amount.rao
             }
         )
         extrinsic = substrate.create_signed_extrinsic( call = call, keypair = wallet.coldkey )
@@ -140,41 +140,41 @@
         if response.is_success:
             return True
         else:
             raise StakeError(response.error_message)
 
 
 def delegate_extrinsic(
-        subtensor: 'bittensor.Subtensor', 
+        subtensor: 'bittensor.Subtensor',
         wallet: 'bittensor.wallet',
         delegate_ss58: Optional[str] = None,
-        amount: Union[Balance, float] = None, 
+        amount: Union[Balance, float] = None,
         wait_for_inclusion: bool = True,
         wait_for_finalization: bool = False,
         prompt: bool = False,
     ) -> bool:
     r""" Delegates the specified amount of stake to the passed delegate.
     Args:
         wallet (bittensor.wallet):
             Bittensor wallet object.
         delegate_ss58 (Optional[str]):
             ss58 address of the delegate.
         amount (Union[Balance, float]):
             Amount to stake as bittensor balance, or float interpreted as Tao.
         wait_for_inclusion (bool):
-            If set, waits for the extrinsic to enter a block before returning true, 
-            or returns false if the extrinsic fails to enter the block within the timeout.   
+            If set, waits for the extrinsic to enter a block before returning true,
+            or returns false if the extrinsic fails to enter the block within the timeout.
         wait_for_finalization (bool):
             If set, waits for the extrinsic to be finalized on the chain before returning true,
             or returns false if the extrinsic fails to be finalized within the timeout.
         prompt (bool):
             If true, the call waits for confirmation from the user before proceeding.
     Returns:
         success (bool):
-            flag is true if extrinsic was finalized or uncluded in the block. 
+            flag is true if extrinsic was finalized or uncluded in the block.
             If we did not wait for finalization / inclusion, the response is true.
 
     Raises:
         NotRegisteredError:
             If the wallet is not registered on the chain.
         NotDelegateError:
             If the hotkey is not a delegate on the chain.
@@ -205,15 +205,15 @@
     else:
         staking_balance = staking_balance
 
     # Check enough balance to stake.
     if staking_balance > my_prev_coldkey_balance:
         bittensor.__console__.print(":cross_mark: [red]Not enough balance[/red]:[bold white]\n  balance:{}\n  amount: {}\n  coldkey: {}[/bold white]".format(my_prev_coldkey_balance, staking_balance, wallet.name))
         return False
-            
+
     # Ask before moving on.
     if prompt:
         if not Confirm.ask("Do you want to delegate:[bold white]\n  amount: {}\n  to: {}\n owner: {}[/bold white]".format( staking_balance, delegate_ss58, delegate_owner) ):
             return False
 
     try:
         with bittensor.__console__.status(":satellite: Staking to: [bold white]{}[/bold white] ...".format(subtensor.network)):
@@ -253,41 +253,41 @@
         bittensor.__console__.print(":cross_mark: [red]Hotkey: {} is not registered.[/red]".format(wallet.hotkey_str))
         return False
     except StakeError as e:
         bittensor.__console__.print(":cross_mark: [red]Stake Error: {}[/red]".format(e))
         return False
 
 def undelegate_extrinsic(
-        subtensor: 'bittensor.Subtensor', 
+        subtensor: 'bittensor.Subtensor',
         wallet: 'bittensor.wallet',
         delegate_ss58: Optional[str] = None,
-        amount: Union[Balance, float] = None, 
+        amount: Union[Balance, float] = None,
         wait_for_inclusion: bool = True,
         wait_for_finalization: bool = False,
         prompt: bool = False,
     ) -> bool:
     r""" Un-delegates stake from the passed delegate.
     Args:
         wallet (bittensor.wallet):
             Bittensor wallet object.
         delegate_ss58 (Optional[str]):
             ss58 address of the delegate.
         amount (Union[Balance, float]):
             Amount to unstake as bittensor balance, or float interpreted as Tao.
         wait_for_inclusion (bool):
-            If set, waits for the extrinsic to enter a block before returning true, 
-            or returns false if the extrinsic fails to enter the block within the timeout.   
+            If set, waits for the extrinsic to enter a block before returning true,
+            or returns false if the extrinsic fails to enter the block within the timeout.
         wait_for_finalization (bool):
             If set, waits for the extrinsic to be finalized on the chain before returning true,
             or returns false if the extrinsic fails to be finalized within the timeout.
         prompt (bool):
             If true, the call waits for confirmation from the user before proceeding.
     Returns:
         success (bool):
-            flag is true if extrinsic was finalized or uncluded in the block. 
+            flag is true if extrinsic was finalized or uncluded in the block.
             If we did not wait for finalization / inclusion, the response is true.
 
     Raises:
         NotRegisteredError:
             If the wallet is not registered on the chain.
         NotDelegateError:
             If the hotkey is not a delegate on the chain.
@@ -314,15 +314,15 @@
     else:
         unstaking_balance = amount
 
     # Check enough stake to unstake.
     if unstaking_balance > my_prev_delegated_stake:
         bittensor.__console__.print(":cross_mark: [red]Not enough delegated stake[/red]:[bold white]\n  stake:{}\n  amount: {}\n coldkey: {}[/bold white]".format(my_prev_delegated_stake, unstaking_balance, wallet.name))
         return False
-            
+
     # Ask before moving on.
     if prompt:
         if not Confirm.ask("Do you want to un-delegate:[bold white]\n  amount: {}\n  from: {}\n  owner: {}[/bold white]".format( unstaking_balance, delegate_ss58, delegate_owner) ):
             return False
 
     try:
         with bittensor.__console__.status(":satellite: Unstaking from: [bold white]{}[/bold white] ...".format(subtensor.network)):
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/log_utilities.py` & `bittensor-5.0.0/bittensor/_subtensor/extrinsics/log_utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 import datetime
 from prometheus_client import Counter, Gauge, Histogram, Summary, Info
 import bittensor
 
 class ValidatorLogger:
     r"""
     Logger object for handling all logging function specific to validator.
-    Including console log styling, console table print and prometheus. 
-    
-    Args: 
-            config (:obj:`bittensor.Config`, `optional`): 
+    Including console log styling, console table print and prometheus.
+
+    Args:
+            config (:obj:`bittensor.Config`, `optional`):
                 bittensor.server.config()
     """
     def __init__(self, config = None):
         # Neuron stats recorded by validator neuron/nucleus
         #   [Column_name, key_name, format_string, rich_style]  # description
         self.config = config
         self.neuron_stats_columns = [
@@ -59,24 +59,24 @@
         ]
         # console_width (:obj:`int`, `required`):
         #     Config console width for table print.
         self.console_width = self.config.get('width', None) if self.config else None
         self.prometheus = ValidatorPrometheus(config)
 
     def print_response_table(
-        self, 
-        batch_predictions: List, 
-        stats: Dict, 
-        sort_col: str, 
-        task_repeat: int = 4, 
+        self,
+        batch_predictions: List,
+        stats: Dict,
+        sort_col: str,
+        task_repeat: int = 4,
         tasks_per_server: int = 3
     ):
-        r""" 
+        r"""
         Prints the query response table: top prediction probabilities and texts for batch tasks.
-        
+
             Args:
                 batch_predictions (:obj:`List[Union[str, Dict{torch.Tensor, str}]]`, `required`):
                     Predictions in string per task per uid. In the format of [(task, {uid, "prob: phrase" })] of length batch size.
                 stats (:obj:`Dict{Dict}`, `required`):
                     Statistics per endpoint for this batch. In the format of {uid, {statistics}}.
                 sort_col (:type:`str`, `required`):
                     Column name used for sorting. Options from self.neuron_stats_columns[:, 1].
@@ -140,29 +140,29 @@
                 except MarkupError as e:
                     print(e)
                 else:
                     if i == len(sort) - 1:
                         print()
 
     def print_synergy_table(
-        self, 
-        stats: Dict, 
+        self,
+        stats: Dict,
         syn_loss_diff: Dict ,
-        sort_col: str, 
+        sort_col: str,
     ):
-        r""" 
+        r"""
         Prints the synergy loss diff matrix with pairwise loss reduction due to synergy (original loss on diagonal).
-            
+
             Args:
                 stats (:obj:`Dict{Dict}`, `required`):
                     Statistics per endpoint for this batch. In the format of {uid, {statistics}}.
                 syn_loss_diff (:obj:`Dict`, `required`):
                     Dictionary table of pairwise synergies as loss reductions, with direct loss on diagonal.
                 sort_col (:type:`str`, `required`):
-                    Column name used for sorting. Options from self.neuron_stats_columns[:, 1]. 
+                    Column name used for sorting. Options from self.neuron_stats_columns[:, 1].
         """
         sort = sorted([(uid, s[sort_col]) for uid, s in stats.items() if sort_col in s],
                     reverse='loss' not in sort_col, key=lambda _row: _row[1])
         uid_col = self.neuron_stats_columns[0]  # [Column_name, key_name, format_string, rich_style]
         columns = [uid_col] + [[f'{s[0]}', '', '{:.2f}', ''] for s in sort]
         rows = [[uid_col[2].format(s[0])] +
                 [('[bright_cyan]{:.2f}[/bright_cyan]' if t == s else
@@ -180,25 +180,25 @@
             table.add_row(*row)
 
         if len(rows):
             rich_print(table)
             print()
 
     def print_stats_table(
-        self, 
-        stats: Dict, 
-        sort_col: str, 
-        title: str, 
-        caption: str, 
+        self,
+        stats: Dict,
+        sort_col: str,
+        title: str,
+        caption: str,
         mark_uids=None
     ):
-        r""" 
+        r"""
         Gathers data and constructs neuron statistics table and prints it.
 
-            Args: 
+            Args:
                 stats (:obj:`Dict{Dict}`, `required`):
                     Statistics per endpoint for this batch. In the format of {uid, {statistics}}.
                 sort_col (:type:`str`, `required`):
                     Column name used for sorting. Options from self.neuron_stats_columns[:, 1].
                 title (:type:`str`, `required`):
                     Title of the table.
                 caption (:type:`str`, `required`):
@@ -240,24 +240,24 @@
         for row in rows:
             table.add_row(*[txt for txt, val in row])
 
         # === Print table ===
         rich_print(table)
 
     def print_synapse_table(
-        self, 
-        name: str, 
-        stats: Dict, 
-        sort_col: str, 
+        self,
+        name: str,
+        stats: Dict,
+        sort_col: str,
         start_time: time.time
     ):
-        r""" 
+        r"""
         Prints the evaluation of the neuron responses to the validator request
-            
-            Args: 
+
+            Args:
                 stats (:obj:`Dict{Dict}`, `required`):
                     Statistics per endpoint for this batch. In the format of {uid, {statistics}}.
                 sort_col (:type:`str`, `required`):
                     Column name used for sorting. Options from self.neuron_stats_columns[:, 1].
                 name (:obj:`str`, `required`):
                     Name of synapse for the title of the table.
                 start_time (:obj:`time.time`, `required`):
@@ -273,51 +273,51 @@
 
     def print_weights_table(
             self,
             min_allowed_weights: int,
             max_weight_limit: int,
             neuron_stats: Dict,
             title: str,
-            metagraph_n: int, 
-            sample_uids: torch.Tensor, 
-            sample_weights: torch.Tensor, 
-            include_uids: List = None, 
+            metagraph_n: int,
+            sample_uids: torch.Tensor,
+            sample_weights: torch.Tensor,
+            include_uids: List = None,
             num_rows: int = None
         ):
-        r""" 
+        r"""
         Prints weights table given sample_uids and sample_weights.
-        
+
             Args:
                 min_allowed_weights (:type:`int`, `required`):
                     subtensor minimum allowed weight to set.
                 max_weight_limit (:type:`int`, `required`):
                     subtensor maximum allowed weight to set.
                 neuron_stats (:obj:`Dict{Dict}`, `required`):
                     Statistics per endpoint for this batch. In the format of {uid, {statistics}}.
                 title (:type:`str`, `required`):
                     Title of the table.
                 metagraph_n (:type:`int`, `required`):
                     Total number of uids in the metagraph.
                 sample_uids (:obj:`torch.Tensor`, `required`):
-                    Uids to set weight for. 
+                    Uids to set weight for.
                 sample_weights (:obj:`torch.Tensor`, `required`):
-                    Weights to set uids for. 
-                include_uids (:type:`list`, `optional`): 
+                    Weights to set uids for.
+                include_uids (:type:`list`, `optional`):
                     Set of uids to inculde in the table.
-                num_rows (:type:`int`, `optional`): 
+                num_rows (:type:`int`, `optional`):
                     Total number of uids to print in total.
         """
         # === Weight table ===
         # Prints exponential moving average statistics of valid neurons and latest weights
         _neuron_stats = {}
         uid_weights = []  # (uid, weight) tuples for sorting to find top/bottom weights
         unvalidated = []
 
         if len(sample_weights) == 0:
-            return 
+            return
 
         for uid, weight in zip(sample_uids.tolist(), sample_weights.tolist()):
             if uid in neuron_stats:
                 _neuron_stats[uid] = {k: v for k, v in neuron_stats[uid].items()}
                 _neuron_stats[uid]['weight'] = weight
                 uid_weights += [(uid, weight)]
             else:
@@ -342,19 +342,19 @@
                     f'sum:{sample_weights.sum().item():.2g} '
                     f'[white] max:[bold]{sample_weights.max().item():.4g}[/bold] / '
                     f'min:[bold]{sample_weights.min().item():.4g}[/bold] [/white] '
                     f'\[{max_weight_limit:.4g} allowed]',  # caption
                     mark_uids=include_uids)
 
     def print_console_validator_identifier(
-        self, 
-        uid: int, 
-        wallet: 'bittensor.Wallet', 
+        self,
+        uid: int,
+        wallet: 'bittensor.Wallet',
         external_ip: str,
-    ):  
+    ):
         r""" Console print for validator identifier.
         """
 
         # validator identifier status console message (every 25 validation steps)
         rich_print(f"[white not bold]{datetime.datetime.now():%Y-%m-%d %H:%M:%S}[/white not bold]{' ' * 4} | "
         f"{f'[bright_white]core_validator[/bright_white]'.center(16 + len('[bright_white][/bright_white]'))} | "
         f"UID [cyan]{uid}[/cyan] "
@@ -362,43 +362,43 @@
         f"[white not bold]cold:[bold]{wallet.name}[/bold]:"
         f"[bright_white not bold]{wallet.coldkeypub.ss58_address}[/bright_white not bold] "
         f"[dim white]/[/dim white] "
         f"hot:[bold]{wallet.hotkey_str}[/bold]:"
         f"[bright_white not bold]{wallet.hotkey.ss58_address}[/bright_white not bold][/white not bold]")
 
     def print_console_metagraph_status(
-        self, 
-        uid: int, 
-        metagraph: 'bittensor.Metagraph', 
-        current_block: int, 
-        start_block: int, 
+        self,
+        uid: int,
+        metagraph: 'bittensor.Metagraph',
+        current_block: int,
+        start_block: int,
         network: str,
         netuid: int
     ):
-        r""" Console print for current validator's metagraph status. 
+        r""" Console print for current validator's metagraph status.
         """
         # validator update status console message
         rich_print(f"[white not bold]{datetime.datetime.now():%Y-%m-%d %H:%M:%S}[/white not bold]{' ' * 4} | "
         f"{f'UID [bright_cyan]{uid}[/bright_cyan]'.center(16 + len('[bright_cyan][/bright_cyan]'))} | "
         f'Updated [yellow]{current_block - metagraph.last_update[uid]}[/yellow] [dim]blocks ago[/dim] | '
         f'Dividends [green not bold]{metagraph.dividends[uid]:.5f}[/green not bold] | '
         f'Stake \u03C4[magenta not bold]{metagraph.total_stake[uid]:.5f}[/magenta not bold] '
         f'[dim](retrieved [yellow]{current_block - start_block}[/yellow] blocks ago from {network})[/dim]')
 
     def print_console_query_summary(
-        self, 
-        current_block: int, 
+        self,
+        current_block: int,
         start_block: int,
-        blocks_per_epoch: int, 
-        epoch_steps: int, 
+        blocks_per_epoch: int,
+        epoch_steps: int,
         epoch: int,
-        responsive_uids: List, 
-        queried_uids: List, 
-        step_time: float, 
-        epoch_responsive_uids: Set, 
+        responsive_uids: List,
+        queried_uids: List,
+        step_time: float,
+        epoch_responsive_uids: Set,
         epoch_queried_uids: Set
     ):
         r""" Console print for query summary.
         """
         rich_print(f"[white not bold]{datetime.datetime.now():%Y-%m-%d %H:%M:%S}[/white not bold]{' ' * 4} | "
         f"{f'[magenta dim not bold]#{current_block}[/magenta dim not bold]'.center(16 + len('[magenta dim not bold][/magenta dim not bold]'))} | "
         f'[green not bold]{current_block - start_block}[/green not bold]/'
@@ -410,17 +410,17 @@
         f'[[yellow]{step_time:.3g}[/yellow]s] '
         f'[dim white not bold][green]{len(epoch_responsive_uids)}[/green]/'
         f'{len(epoch_queried_uids)}[/dim white not bold]')
 
     def print_console_subtensor_weight(
         self,
         sample_weights: torch.Tensor,
-        epoch_responsive_uids: Set, 
-        epoch_queried_uids: Set, 
-        max_weight_limit: float, 
+        epoch_responsive_uids: Set,
+        epoch_queried_uids: Set,
+        max_weight_limit: float,
         epoch_start_time: time.time,
     ):
         r""" Console print for weight setting to subtensor.
         """
 
         rich_print(f"[white not bold]{datetime.datetime.now():%Y-%m-%d %H:%M:%S}[/white not bold]{' ' * 4} | "
         f"{f'[bright_white]Set weights[/bright_white]'.center(16 + len('[bright_white][/bright_white]'))} | "
@@ -433,76 +433,76 @@
         f'[white] max:[bold]{sample_weights.max().item():.4g}[/bold] / '
         f'min:[bold]{sample_weights.min().item():.4g}[/bold] [/white] '
         f'\[{max_weight_limit:.4g} allowed]')
 
 class ValidatorPrometheus:
     r"""
     Prometheis logging object for validator.
-        Args: 
-            config (:obj:`bittensor.Config`, `optional`): 
+        Args:
+            config (:obj:`bittensor.Config`, `optional`):
                 bittensor.server.config()
-    """ 
+    """
     def __init__(self, config):
         self.config = config
         self.info = Info("neuron_info", "Info sumamries for the running server-miner.")
         self.gauges = Gauge('validator_gauges', 'Gauges for the running validator.', ['validator_gauges_name'])
         self.counters = Counter('validator_counters', 'Counters for the running validator.', ['validator_counters_name'])
         self.step_time = Histogram('validator_step_time', 'Validator step time histogram.', buckets=list(range(0, 2 * bittensor.__blocktime__, 1)))
 
     def log_run_info(
-        self, 
-        parameters: torch.nn.parameter.Parameter, 
-        uid: int, 
-        network: str, 
+        self,
+        parameters: torch.nn.parameter.Parameter,
+        uid: int,
+        network: str,
         wallet: 'bittensor.Wallet'
     ):
-        r""" Set up prometheus running info. 
+        r""" Set up prometheus running info.
         """
 
         self.gauges.labels( "model_size_params" ).set( sum(p.numel() for p in parameters) )
         self.gauges.labels( "model_size_bytes" ).set( sum(p.element_size() * p.nelement() for p in parameters) )
         self.info.info({
             'type': "core_validator",
             'uid': str(uid),
             'network': network,
             'coldkey': str(wallet.coldkeypub.ss58_address),
             'hotkey': str(wallet.hotkey.ss58_address),
         })
 
     def log_epoch_start(
-        self, 
-        current_block: int, 
-        batch_size: int, 
-        sequence_length: int, 
-        validation_len: int, 
-        min_allowed_weights: int, 
-        blocks_per_epoch: int, 
+        self,
+        current_block: int,
+        batch_size: int,
+        sequence_length: int,
+        validation_len: int,
+        min_allowed_weights: int,
+        blocks_per_epoch: int,
         epochs_until_reset: int
     ):
-        r""" All prometheus logging at the start of epoch. 
+        r""" All prometheus logging at the start of epoch.
         """
         self.gauges.labels("current_block").set( current_block )
         self.gauges.labels("batch_size").set( batch_size )
         self.gauges.labels("sequence_length").set( sequence_length )
         self.gauges.labels("validation_len").set( validation_len )
         self.gauges.labels("min_allowed_weights").set( min_allowed_weights )
         self.gauges.labels("blocks_per_epoch").set( blocks_per_epoch )
         self.gauges.labels("epochs_until_reset").set( epochs_until_reset )
         self.gauges.labels("scaling_law_power").set( self.config.nucleus.scaling_law_power )
         self.gauges.labels("synergy_scaling_law_power").set( self.config.nucleus.synergy_scaling_law_power )
         self.gauges.labels("epoch_steps").set(0)
-    
+
     def log_step(
         self,
         current_block: int,
         last_update: int,
         step_time: int,
         loss: int
     ):
-        r""" All prometheus logging at the each validation step. 
+        r""" All prometheus logging at the each validation step.
         """
         self.gauges.labels("global_step").inc()
         self.gauges.labels("epoch_steps").inc()
         self.gauges.labels("current_block").set(current_block)
         self.gauges.labels("last_updated").set( current_block - last_update )
         self.step_time.observe( step_time )
         self.gauges.labels('step_time').set( step_time )
@@ -510,15 +510,15 @@
 
     def log_epoch_end(
         self,
         uid: int,
         metagraph: 'bittensor.Metagraph',
         current_block: int,
     ):
-        r""" All prometheus logging at the end of epoch. 
+        r""" All prometheus logging at the end of epoch.
         """
         self.gauges.labels("epoch").inc()
         self.gauges.labels("set_weights").inc()
         self.gauges.labels('set_weights_block').set(current_block)
         self.gauges.labels("stake").set( metagraph.total_stake[uid] )
         self.gauges.labels("rank").set( metagraph.ranks[uid] )
         self.gauges.labels("trust").set( metagraph.trust[uid] )
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/prometheus.py` & `bittensor-5.0.0/bittensor/_subtensor/extrinsics/prometheus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 # Copyright © 2023 Opentensor Foundation
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 import bittensor
 
 import json
 from rich.prompt import Confirm
 import bittensor.utils.networking as net
 from ..errors import *
 
 def prometheus_extrinsic(
     subtensor: 'bittensor.Subtensor',
     wallet: 'bittensor.wallet',
-    port: int, 
+    port: int,
     netuid: int,
     ip: int = None,
     wait_for_inclusion: bool = False,
     wait_for_finalization = True,
 ) -> bool:
     r""" Subscribes an bittensor endpoint to the substensor chain.
     Args:
@@ -40,40 +40,40 @@
         ip (str):
             endpoint host port i.e. 192.122.31.4
         port (int):
             endpoint port number i.e. 9221
         netuid (int):
             network uid to serve on.
         wait_for_inclusion (bool):
-            if set, waits for the extrinsic to enter a block before returning true, 
-            or returns false if the extrinsic fails to enter the block within the timeout.   
+            if set, waits for the extrinsic to enter a block before returning true,
+            or returns false if the extrinsic fails to enter the block within the timeout.
         wait_for_finalization (bool):
             if set, waits for the extrinsic to be finalized on the chain before returning true,
             or returns false if the extrinsic fails to be finalized within the timeout.
     Returns:
         success (bool):
-            flag is true if extrinsic was finalized or uncluded in the block. 
+            flag is true if extrinsic was finalized or uncluded in the block.
             If we did not wait for finalization / inclusion, the response is true.
     """
-        
+
     # ---- Get external ip ----
     if ip == None:
         try:
             external_ip = net.get_external_ip()
             bittensor.__console__.print(":white_heavy_check_mark: [green]Found external ip: {}[/green]".format( external_ip ))
             bittensor.logging.success(prefix = 'External IP', sufix = '<blue>{}</blue>'.format( external_ip ))
         except Exception as E:
             raise RuntimeError('Unable to attain your external ip. Check your internet connection. error: {}'.format(E)) from E
     else:
         external_ip = ip
 
     call_params={
-        'version': bittensor.__version_as_int__, 
-        'ip': net.ip_to_int(external_ip), 
-        'port': port, 
+        'version': bittensor.__version_as_int__,
+        'ip': net.ip_to_int(external_ip),
+        'port': port,
         'ip_type': net.ip_version(external_ip),
     }
 
     with bittensor.__console__.status(":satellite: Checking Prometheus..."):
         neuron = subtensor.get_neuron_for_pubkey_and_subnet( wallet.hotkey.ss58_address, netuid = netuid )
         neuron_up_to_date = not neuron.is_null and call_params == {
             'version': neuron.prometheus_info.version,
@@ -91,15 +91,15 @@
             f"[green not bold] port: [/green not bold][white not bold]{neuron.prometheus_info.port}[/white not bold] | "
             f"[green not bold] version: [/green not bold][white not bold]{neuron.prometheus_info.version}[/white not bold] |"
         )
 
 
         bittensor.__console__.print(":white_heavy_check_mark: [white]Prometheus already served.[/white]".format( external_ip ))
         return True
-    
+
     # Add netuid, not in prometheus_info
     call_params['netuid'] = netuid
 
     with bittensor.__console__.status(":satellite: Serving prometheus on: [white]{}:{}[/white] ...".format(subtensor.network, netuid)):
         with subtensor.substrate as substrate:
             call = substrate.compose_call(
                 call_module='SubtensorModule',
@@ -116,8 +116,7 @@
                     ))
                     return True
                 else:
                     bittensor.__console__.print(':cross_mark: [green]Failed to serve prometheus[/green] error: {}'.format(response.error_message))
                     return False
             else:
                 return True
-
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/registration.py` & `bittensor-5.0.0/bittensor/_subtensor/extrinsics/registration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 # Copyright © 2023 Opentensor Foundation
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import bittensor
 
 import torch
 import time
 from rich.prompt import Confirm
@@ -46,16 +46,16 @@
     r""" Registers the wallet to chain.
     Args:
         wallet (bittensor.wallet):
             bittensor wallet object.
         netuid (int):
             The netuid of the subnet to register on.
         wait_for_inclusion (bool):
-            If set, waits for the extrinsic to enter a block before returning true, 
-            or returns false if the extrinsic fails to enter the block within the timeout.   
+            If set, waits for the extrinsic to enter a block before returning true,
+            or returns false if the extrinsic fails to enter the block within the timeout.
         wait_for_finalization (bool):
             If set, waits for the extrinsic to be finalized on the chain before returning true,
             or returns false if the extrinsic fails to be finalized within the timeout.
         prompt (bool):
             If true, the call waits for confirmation from the user before proceeding.
         max_allowed_attempts (int):
             Maximum number of attempts to register the wallet.
@@ -69,30 +69,30 @@
             The number of processes to use to register.
         update_interval (int):
             The number of nonces to solve between updates.
         log_verbose (bool):
             If true, the registration process will log more information.
     Returns:
         success (bool):
-            flag is true if extrinsic was finalized or uncluded in the block. 
+            flag is true if extrinsic was finalized or uncluded in the block.
             If we did not wait for finalization / inclusion, the response is true.
     """
     if not subtensor.subnet_exists( netuid ):
         bittensor.__console__.print(":cross_mark: [red]Failed[/red]: error: [bold white]subnet:{}[/bold white] does not exist.".format(netuid))
         return False
 
     with bittensor.__console__.status(f":satellite: Checking Account on [bold]subnet:{netuid}[/bold]..."):
         neuron = subtensor.get_neuron_for_pubkey_and_subnet( wallet.hotkey.ss58_address, netuid = netuid )
         if not neuron.is_null:
             bittensor.__console__.print(
             ':white_heavy_check_mark: [green]Already Registered[/green]:\n'\
             'uid: [bold white]{}[/bold white]\n' \
             'netuid: [bold white]{}[/bold white]\n' \
             'hotkey: [bold white]{}[/bold white]\n' \
-            'coldkey: [bold white]{}[/bold white]' 
+            'coldkey: [bold white]{}[/bold white]'
             .format(neuron.uid, neuron.netuid, neuron.hotkey, neuron.coldkey))
             return True
 
     if prompt:
         if not Confirm.ask("Continue Registration?\n  hotkey:     [bold white]{}[/bold white]\n  coldkey:    [bold white]{}[/bold white]\n  network:    [bold white]{}[/bold white]".format( wallet.hotkey.ss58_address, wallet.coldkeypub.ss58_address, subtensor.network ) ):
             return False
 
@@ -112,53 +112,53 @@
 
         # pow failed
         if not pow_result:
             # might be registered already on this subnet
             if (wallet.is_registered( subtensor = subtensor, netuid = netuid )):
                 bittensor.__console__.print(f":white_heavy_check_mark: [green]Already registered on netuid:{netuid}[/green]")
                 return True
-            
+
         # pow successful, proceed to submit pow to chain for registration
         else:
             with bittensor.__console__.status(":satellite: Submitting POW..."):
                 # check if pow result is still valid
                 while not pow_result.is_stale(subtensor=subtensor):
                     with subtensor.substrate as substrate:
                         # create extrinsic call
-                        call = substrate.compose_call( 
-                            call_module='SubtensorModule',  
-                            call_function='register', 
-                            call_params={ 
+                        call = substrate.compose_call(
+                            call_module='SubtensorModule',
+                            call_function='register',
+                            call_params={
                                 'netuid': netuid,
-                                'block_number': pow_result.block_number, 
-                                'nonce': pow_result.nonce, 
+                                'block_number': pow_result.block_number,
+                                'nonce': pow_result.nonce,
                                 'work': [int(byte_) for byte_ in pow_result.seal],
-                                'hotkey': wallet.hotkey.ss58_address, 
+                                'hotkey': wallet.hotkey.ss58_address,
                                 'coldkey': wallet.coldkeypub.ss58_address,
-                            } 
+                            }
                         )
                         extrinsic = substrate.create_signed_extrinsic( call = call, keypair = wallet.hotkey )
                         response = substrate.submit_extrinsic( extrinsic, wait_for_inclusion=wait_for_inclusion, wait_for_finalization=wait_for_finalization )
-                        
+
                         # We only wait here if we expect finalization.
                         if not wait_for_finalization and not wait_for_inclusion:
                             bittensor.__console__.print(":white_heavy_check_mark: [green]Sent[/green]")
                             return True
-                        
+
                         # process if registration successful, try again if pow is still valid
                         response.process_events()
                         if not response.is_success:
                             if 'key is already registered' in response.error_message:
                                 # Error meant that the key is already registered.
                                 bittensor.__console__.print(f":white_heavy_check_mark: [green]Already Registered on [bold]subnet:{netuid}[/bold][/green]")
                                 return True
 
                             bittensor.__console__.print(":cross_mark: [red]Failed[/red]: error:{}".format(response.error_message))
                             time.sleep(0.5)
-                        
+
                         # Successful registration, final check for neuron and pubkey
                         else:
                             bittensor.__console__.print(":satellite: Checking Balance...")
                             is_registered = wallet.is_registered( subtensor = subtensor, netuid = netuid )
                             if is_registered:
                                 bittensor.__console__.print(":white_heavy_check_mark: [green]Registered[/green]")
                                 return True
@@ -167,24 +167,24 @@
                                 bittensor.__console__.print(":cross_mark: [red]Unknown error. Neuron not found.[/red]")
                                 continue
                 else:
                     # Exited loop because pow is no longer valid.
                     bittensor.__console__.print( "[red]POW is stale.[/red]" )
                     # Try again.
                     continue
-                    
+
         if attempts < max_allowed_attempts:
             #Failed registration, retry pow
             attempts += 1
             bittensor.__console__.print( ":satellite: Failed registration, retrying pow ...({}/{})".format(attempts, max_allowed_attempts))
         else:
             # Failed to register after max attempts.
             bittensor.__console__.print( "[red]No more attempts.[/red]" )
-            return False 
-        
+            return False
+
 
 def burned_register_extrinsic (
     subtensor: 'bittensor.Subtensor',
     wallet: 'bittensor.Wallet',
     netuid: int,
     wait_for_inclusion: bool = False,
     wait_for_finalization: bool = True,
@@ -193,24 +193,24 @@
     r""" Registers the wallet to chain by recycling TAO.
     Args:
         wallet (bittensor.wallet):
             bittensor wallet object.
         netuid (int):
             The netuid of the subnet to register on.
         wait_for_inclusion (bool):
-            If set, waits for the extrinsic to enter a block before returning true, 
-            or returns false if the extrinsic fails to enter the block within the timeout.   
+            If set, waits for the extrinsic to enter a block before returning true,
+            or returns false if the extrinsic fails to enter the block within the timeout.
         wait_for_finalization (bool):
             If set, waits for the extrinsic to be finalized on the chain before returning true,
             or returns false if the extrinsic fails to be finalized within the timeout.
         prompt (bool):
             If true, the call waits for confirmation from the user before proceeding.
     Returns:
         success (bool):
-            flag is true if extrinsic was finalized or uncluded in the block. 
+            flag is true if extrinsic was finalized or uncluded in the block.
             If we did not wait for finalization / inclusion, the response is true.
     """
     if not subtensor.subnet_exists( netuid ):
         bittensor.__console__.print(":cross_mark: [red]Failed[/red]: error: [bold white]subnet:{}[/bold white] does not exist.".format(netuid))
         return False
 
     wallet.coldkey # unlock coldkey
@@ -222,48 +222,48 @@
         burn_amount = subtensor.burn( netuid = netuid )
         if not neuron.is_null:
             bittensor.__console__.print(
             ':white_heavy_check_mark: [green]Already Registered[/green]:\n'\
             'uid: [bold white]{}[/bold white]\n' \
             'netuid: [bold white]{}[/bold white]\n' \
             'hotkey: [bold white]{}[/bold white]\n' \
-            'coldkey: [bold white]{}[/bold white]' 
+            'coldkey: [bold white]{}[/bold white]'
             .format(neuron.uid, neuron.netuid, neuron.hotkey, neuron.coldkey))
             return True
-        
+
     if prompt:
         # Prompt user for confirmation.
         if not Confirm.ask( f"Recycle {burn_amount} to register on subnet:{netuid}?" ):
             return False
 
     with bittensor.__console__.status(":satellite: Recycling TAO for Registration..."):
        with subtensor.substrate as substrate:
             # create extrinsic call
-            call = substrate.compose_call( 
-                call_module='SubtensorModule',  
-                call_function='burned_register', 
-                call_params={ 
+            call = substrate.compose_call(
+                call_module='SubtensorModule',
+                call_function='burned_register',
+                call_params={
                     'netuid': netuid,
                     'hotkey': wallet.hotkey.ss58_address
-                } 
+                }
             )
             extrinsic = substrate.create_signed_extrinsic( call = call, keypair = wallet.coldkey )
             response = substrate.submit_extrinsic( extrinsic, wait_for_inclusion=wait_for_inclusion, wait_for_finalization=wait_for_finalization )
-            
+
             # We only wait here if we expect finalization.
             if not wait_for_finalization and not wait_for_inclusion:
                 bittensor.__console__.print(":white_heavy_check_mark: [green]Sent[/green]")
                 return True
-            
+
             # process if registration successful, try again if pow is still valid
             response.process_events()
             if not response.is_success:
                 bittensor.__console__.print(":cross_mark: [red]Failed[/red]: error:{}".format(response.error_message))
                 time.sleep(0.5)
-            
+
             # Successful registration, final check for neuron and pubkey
             else:
                 bittensor.__console__.print(":satellite: Checking Balance...")
                 block = subtensor.get_current_block()
                 new_balance = subtensor.get_balance( wallet.coldkeypub.ss58_address, block = block )
 
                 bittensor.__console__.print("Balance:\n  [blue]{}[/blue] :arrow_right: [green]{}[/green]".format( old_balance, new_balance ))
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/serving.py` & `bittensor-5.0.0/bittensor/_subtensor/extrinsics/serving.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 # Copyright © 2023 Opentensor Foundation
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 import bittensor
 
 import json
 from rich.prompt import Confirm
 import bittensor.utils.networking as net
 from ..errors import *
 
 def serve_extrinsic (
     subtensor: 'bittensor.Subtensor',
     wallet: 'bittensor.wallet',
-    ip: str, 
-    port: int, 
-    protocol: int, 
+    ip: str,
+    port: int,
+    protocol: int,
     netuid: int,
     placeholder1: int = 0,
     placeholder2: int = 0,
     wait_for_inclusion: bool = False,
     wait_for_finalization = True,
     prompt: bool = False,
 ) -> bool:
@@ -40,32 +40,32 @@
         wallet (bittensor.wallet):
             bittensor wallet object.
         ip (str):
             endpoint host port i.e. 192.122.31.4
         port (int):
             endpoint port number i.e. 9221
         protocol (int):
-            int representation of the protocol 
+            int representation of the protocol
         netuid (int):
             network uid to serve on.
         placeholder1 (int):
             placeholder for future use.
         placeholder2 (int):
             placeholder for future use.
         wait_for_inclusion (bool):
-            if set, waits for the extrinsic to enter a block before returning true, 
-            or returns false if the extrinsic fails to enter the block within the timeout.   
+            if set, waits for the extrinsic to enter a block before returning true,
+            or returns false if the extrinsic fails to enter the block within the timeout.
         wait_for_finalization (bool):
             if set, waits for the extrinsic to be finalized on the chain before returning true,
             or returns false if the extrinsic fails to be finalized within the timeout.
         prompt (bool):
             If true, the call waits for confirmation from the user before proceeding.
     Returns:
         success (bool):
-            flag is true if extrinsic was finalized or uncluded in the block. 
+            flag is true if extrinsic was finalized or uncluded in the block.
             If we did not wait for finalization / inclusion, the response is true.
     """
     # Decrypt hotkey
     wallet.hotkey
     params = {
         'version': bittensor.__version_as_int__,
         'ip': net.ip_to_int(ip),
@@ -148,31 +148,31 @@
     wait_for_inclusion: bool = False,
     wait_for_finalization: bool = True,
     prompt: bool = False,
 ) -> bool:
     r""" Serves the axon to the network.
     Args:
         netuid ( int ):
-            The netuid being served on. 
+            The netuid being served on.
         axon (bittensor.Axon):
             Axon to serve.
-        use_upnpc (:type:bool, `optional`): 
-            If true, the axon attempts port forward through your router before 
-            subscribing.                
+        use_upnpc (:type:bool, `optional`):
+            If true, the axon attempts port forward through your router before
+            subscribing.
         wait_for_inclusion (bool):
-            If set, waits for the extrinsic to enter a block before returning true, 
-            or returns false if the extrinsic fails to enter the block within the timeout.   
+            If set, waits for the extrinsic to enter a block before returning true,
+            or returns false if the extrinsic fails to enter the block within the timeout.
         wait_for_finalization (bool):
             If set, waits for the extrinsic to be finalized on the chain before returning true,
             or returns false if the extrinsic fails to be finalized within the timeout.
         prompt (bool):
             If true, the call waits for confirmation from the user before proceeding.
     Returns:
         success (bool):
-            flag is true if extrinsic was finalized or uncluded in the block. 
+            flag is true if extrinsic was finalized or uncluded in the block.
             If we did not wait for finalization / inclusion, the response is true.
     """
     axon.wallet.hotkey
     axon.wallet.coldkeypub
 
     # ---- Setup UPNPC ----
     if use_upnpc:
@@ -194,15 +194,15 @@
             external_ip = net.get_external_ip()
             bittensor.__console__.print(":white_heavy_check_mark: [green]Found external ip: {}[/green]".format( external_ip ))
             bittensor.logging.success(prefix = 'External IP', sufix = '<blue>{}</blue>'.format( external_ip ))
         except Exception as E:
             raise RuntimeError('Unable to attain your external ip. Check your internet connection. error: {}'.format(E)) from E
     else:
         external_ip = axon.external_ip
-    
+
     # ---- Subscribe to chain ----
     serve_success = subtensor.serve(
             wallet = axon.wallet,
             ip = external_ip,
             port = external_port,
             netuid = netuid,
             protocol = 4,
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/set_weights.py` & `bittensor-5.0.0/bittensor/_subtensor/extrinsics/set_weights.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 # Copyright © 2023 Opentensor Foundation
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import bittensor
 
 import torch
 from rich.prompt import Confirm
 from typing import Union
@@ -117,9 +117,9 @@
 
     # TODO( devs ): this code is dead.
     if response.is_success:
         bittensor.__console__.print("Set weights:\n[bold white]  weights: {}\n  uids: {}[/bold white ]".format( [float(v/4294967295) for v in weight_vals], weight_uids ))
         message = '<green>Success: </green>' + f'Set {len(uids)} weights, top 5 weights' + str(list(zip(uids.tolist()[:5], [round (w,4) for w in weights.tolist()[:5]] )))
         logger.debug('Set weights:'.ljust(20) +  message)
         return True
-    
+
     return False
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/staking.py` & `bittensor-5.0.0/bittensor/_subtensor/extrinsics/staking.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,93 +1,93 @@
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 # Copyright © 2023 Opentensor Foundation
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import bittensor
 
 from rich.prompt import Confirm
 from time import sleep
 from typing import List, Dict, Union, Optional
 from bittensor.utils.balance import Balance
 from ..errors import *
 
 def add_stake_extrinsic(
-        subtensor: 'bittensor.Subtensor', 
+        subtensor: 'bittensor.Subtensor',
         wallet: 'bittensor.wallet',
         hotkey_ss58: Optional[str] = None,
-        amount: Union[Balance, float] = None, 
+        amount: Union[Balance, float] = None,
         wait_for_inclusion: bool = True,
         wait_for_finalization: bool = False,
         prompt: bool = False,
     ) -> bool:
     r""" Adds the specified amount of stake to passed hotkey uid.
     Args:
         wallet (bittensor.wallet):
             Bittensor wallet object.
         hotkey_ss58 (Optional[str]):
             ss58 address of the hotkey account to stake to
             defaults to the wallet's hotkey.
         amount (Union[Balance, float]):
             Amount to stake as bittensor balance, or float interpreted as Tao.
         wait_for_inclusion (bool):
-            If set, waits for the extrinsic to enter a block before returning true, 
-            or returns false if the extrinsic fails to enter the block within the timeout.   
+            If set, waits for the extrinsic to enter a block before returning true,
+            or returns false if the extrinsic fails to enter the block within the timeout.
         wait_for_finalization (bool):
             If set, waits for the extrinsic to be finalized on the chain before returning true,
             or returns false if the extrinsic fails to be finalized within the timeout.
         prompt (bool):
             If true, the call waits for confirmation from the user before proceeding.
     Returns:
         success (bool):
-            flag is true if extrinsic was finalized or uncluded in the block. 
+            flag is true if extrinsic was finalized or uncluded in the block.
             If we did not wait for finalization / inclusion, the response is true.
 
     Raises:
         NotRegisteredError:
             If the wallet is not registered on the chain.
         NotDelegateError:
             If the hotkey is not a delegate on the chain.
     """
     # Decrypt keys,
     wallet.coldkey
 
     # Default to wallet's own hotkey if the value is not passed.
     if hotkey_ss58 is None:
-        hotkey_ss58 = wallet.hotkey.ss58_address 
+        hotkey_ss58 = wallet.hotkey.ss58_address
 
     # Flag to indicate if we are using the wallet's own hotkey.
     own_hotkey: bool
 
     with bittensor.__console__.status(":satellite: Syncing with chain: [white]{}[/white] ...".format(subtensor.network)):
         old_balance = subtensor.get_balance( wallet.coldkeypub.ss58_address )
         # Get hotkey owner
         hotkey_owner = subtensor.get_hotkey_owner( hotkey_ss58 )
         own_hotkey = (wallet.coldkeypub.ss58_address == hotkey_owner)
         if not own_hotkey:
             # This is not the wallet's own hotkey so we are delegating.
             if not subtensor.is_hotkey_delegate( hotkey_ss58 ):
                 raise NotDelegateError("Hotkey: {} is not a delegate.".format(hotkey_ss58))
-            
+
             # Get hotkey take
             hotkey_take = subtensor.get_delegate_take( hotkey_ss58 )
-        
+
         # Get current stake
         old_stake = subtensor.get_stake_for_coldkey_and_hotkey( coldkey_ss58=wallet.coldkeypub.ss58_address, hotkey_ss58=hotkey_ss58 )
 
     # Convert to bittensor.Balance
     if amount == None:
         # Stake it all.
         staking_balance = bittensor.Balance.from_tao( old_balance.tao )
@@ -102,15 +102,15 @@
     else:
         staking_balance = staking_balance
 
     # Check enough to stake.
     if staking_balance > old_balance:
         bittensor.__console__.print(":cross_mark: [red]Not enough stake[/red]:[bold white]\n  balance:{}\n  amount: {}\n  coldkey: {}[/bold white]".format(old_balance, staking_balance, wallet.name))
         return False
-            
+
     # Ask before moving on.
     if prompt:
         if not own_hotkey:
             # We are delegating.
             if not Confirm.ask("Do you want to delegate:[bold white]\n  amount: {}\n  to: {}\n  take: {}\n  owner: {}[/bold white]".format( staking_balance, wallet.hotkey_str, hotkey_take, hotkey_owner) ):
                 return False
         else:
@@ -156,47 +156,47 @@
         return False
     except StakeError as e:
         bittensor.__console__.print(":cross_mark: [red]Stake Error: {}[/red]".format(e))
         return False
 
 
 def add_stake_multiple_extrinsic (
-        subtensor: 'bittensor.Subtensor', 
+        subtensor: 'bittensor.Subtensor',
         wallet: 'bittensor.wallet',
         hotkey_ss58s: List[str],
-        amounts: List[Union[Balance, float]] = None, 
+        amounts: List[Union[Balance, float]] = None,
         wait_for_inclusion: bool = True,
         wait_for_finalization: bool = False,
         prompt: bool = False,
     ) -> bool:
     r""" Adds stake to each hotkey_ss58 in the list, using each amount, from a common coldkey.
     Args:
         wallet (bittensor.wallet):
             Bittensor wallet object for the coldkey.
         hotkey_ss58s (List[str]):
             List of hotkeys to stake to.
         amounts (List[Union[Balance, float]]):
             List of amounts to stake. If None, stake all to the first hotkey.
         wait_for_inclusion (bool):
-            if set, waits for the extrinsic to enter a block before returning true, 
-            or returns false if the extrinsic fails to enter the block within the timeout.   
+            if set, waits for the extrinsic to enter a block before returning true,
+            or returns false if the extrinsic fails to enter the block within the timeout.
         wait_for_finalization (bool):
             if set, waits for the extrinsic to be finalized on the chain before returning true,
             or returns false if the extrinsic fails to be finalized within the timeout.
         prompt (bool):
             If true, the call waits for confirmation from the user before proceeding.
     Returns:
         success (bool):
             flag is true if extrinsic was finalized or included in the block.
             flag is true if any wallet was staked.
             If we did not wait for finalization / inclusion, the response is true.
     """
     if not isinstance(hotkey_ss58s, list) or not all(isinstance(hotkey_ss58, str) for hotkey_ss58 in hotkey_ss58s):
         raise TypeError("hotkey_ss58s must be a list of str")
-    
+
     if len(hotkey_ss58s) == 0:
         return True
 
     if amounts is not None and len(amounts) != len(hotkey_ss58s):
         raise ValueError("amounts must be a list of the same length as hotkey_ss58s")
 
     if amounts is not None and not all(isinstance(amount, (Balance, float)) for amount in amounts):
@@ -235,15 +235,15 @@
         # Staking less than 1000 rao to the wallets.
         pass
     else:
         # Staking more than 1000 rao to the wallets.
         ## Reduce the amount to stake to each wallet to keep the balance above 1000 rao.
         percent_reduction = 1 - (1000 / total_staking_rao)
         amounts = [Balance.from_tao(amount.tao * percent_reduction) for amount in amounts]
-    
+
     successful_stakes = 0
     for idx, (hotkey_ss58, amount, old_stake) in enumerate(zip(hotkey_ss58s, amounts, old_stakes)):
         staking_all = False
         # Convert to bittensor.Balance
         if amount == None:
             # Stake it all.
             staking_balance = bittensor.Balance.from_tao( old_balance.tao )
@@ -253,15 +253,15 @@
             assert isinstance(amount, bittensor.Balance)
             staking_balance = amount
 
         # Check enough to stake
         if staking_balance > old_balance:
             bittensor.__console__.print(":cross_mark: [red]Not enough balance[/red]: [green]{}[/green] to stake: [blue]{}[/blue] from coldkey: [white]{}[/white]".format(old_balance, staking_balance, wallet.name))
             continue
-                        
+
         # Ask before moving on.
         if prompt:
             if not Confirm.ask("Do you want to stake:\n[bold white]  amount: {}\n  hotkey: {}[/bold white ]?".format( staking_balance, wallet.hotkey_str) ):
                 continue
 
         try:
             staking_response: bool = __do_add_stake_single(
@@ -311,76 +311,75 @@
 
         except NotRegisteredError as e:
             bittensor.__console__.print(":cross_mark: [red]Hotkey: {} is not registered.[/red]".format(hotkey_ss58))
             continue
         except StakeError as e:
             bittensor.__console__.print(":cross_mark: [red]Stake Error: {}[/red]".format(e))
             continue
-            
-    
+
+
     if successful_stakes != 0:
         with bittensor.__console__.status(":satellite: Checking Balance on: ([white]{}[/white] ...".format(subtensor.network)):
             new_balance = subtensor.get_balance( wallet.coldkeypub.ss58_address )
         bittensor.__console__.print("Balance: [blue]{}[/blue] :arrow_right: [green]{}[/green]".format( old_balance, new_balance ))
         return True
 
     return False
 
 def __do_add_stake_single(
-        subtensor: 'bittensor.Subtensor', 
+        subtensor: 'bittensor.Subtensor',
         wallet: 'bittensor.wallet',
         hotkey_ss58: str,
-        amount: 'bittensor.Balance', 
+        amount: 'bittensor.Balance',
         wait_for_inclusion: bool = True,
         wait_for_finalization: bool = False,
     ) -> bool:
     r"""
     Executes a stake call to the chain using the wallet and amount specified.
     Args:
         wallet (bittensor.wallet):
             Bittensor wallet object.
         hotkey_ss58 (str):
             Hotkey to stake to.
         amount (bittensor.Balance):
             Amount to stake as bittensor balance object.
         wait_for_inclusion (bool):
-            If set, waits for the extrinsic to enter a block before returning true, 
-            or returns false if the extrinsic fails to enter the block within the timeout.   
+            If set, waits for the extrinsic to enter a block before returning true,
+            or returns false if the extrinsic fails to enter the block within the timeout.
         wait_for_finalization (bool):
             If set, waits for the extrinsic to be finalized on the chain before returning true,
             or returns false if the extrinsic fails to be finalized within the timeout.
         prompt (bool):
             If true, the call waits for confirmation from the user before proceeding.
     Returns:
         success (bool):
-            flag is true if extrinsic was finalized or uncluded in the block. 
+            flag is true if extrinsic was finalized or uncluded in the block.
             If we did not wait for finalization / inclusion, the response is true.
     Raises:
         StakeError:
             If the extrinsic fails to be finalized or included in the block.
         NotDelegateError:
             If the hotkey is not a delegate.
         NotRegisteredError:
             If the hotkey is not registered in any subnets.
 
     """
     # Decrypt keys,
     wallet.coldkey
-    
     hotkey_owner = subtensor.get_hotkey_owner( hotkey_ss58 )
     own_hotkey = (wallet.coldkeypub.ss58_address == hotkey_owner)
     if not own_hotkey:
         # We are delegating.
         # Verify that the hotkey is a delegate.
         if not subtensor.is_hotkey_delegate( hotkey_ss58 = hotkey_ss58 ):
             raise NotDelegateError("Hotkey: {} is not a delegate.".format(hotkey_ss58))
 
     with subtensor.substrate as substrate:
         call = substrate.compose_call(
-        call_module='SubtensorModule', 
+        call_module='SubtensorModule',
         call_function='add_stake',
         call_params={
             'hotkey': hotkey_ss58,
             'amount_staked': amount.rao
             }
         )
         extrinsic = substrate.create_signed_extrinsic( call = call, keypair = wallet.coldkey )
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/transfer.py` & `bittensor-5.0.0/bittensor/_subtensor/extrinsics/transfer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,64 +1,64 @@
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 # Copyright © 2023 Opentensor Foundation
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import bittensor
 
 from rich.prompt import Confirm
 from typing import List, Dict, Union
 from bittensor.utils.balance import Balance
 from bittensor.utils import is_valid_bittensor_address_or_public_key
 from ..errors import *
 
 def transfer_extrinsic(
         subtensor: 'bittensor.Subtensor',
         wallet: 'bittensor.wallet',
-        dest: str, 
-        amount: Union[Balance, float], 
+        dest: str,
+        amount: Union[Balance, float],
         wait_for_inclusion: bool = True,
         wait_for_finalization: bool = False,
         keep_alive: bool = True,
         prompt: bool = False,
     ) -> bool:
     r""" Transfers funds from this wallet to the destination public key address
     Args:
         wallet (bittensor.wallet):
             Bittensor wallet object to make transfer from.
         dest (str, ss58_address or ed25519):
-            Destination public key address of reciever. 
+            Destination public key address of reciever.
         amount (Union[Balance, int]):
             Amount to stake as bittensor balance, or float interpreted as Tao.
         wait_for_inclusion (bool):
-            If set, waits for the extrinsic to enter a block before returning true, 
-            or returns false if the extrinsic fails to enter the block within the timeout.   
+            If set, waits for the extrinsic to enter a block before returning true,
+            or returns false if the extrinsic fails to enter the block within the timeout.
         wait_for_finalization (bool):
             If set, waits for the extrinsic to be finalized on the chain before returning true,
             or returns false if the extrinsic fails to be finalized within the timeout.
         keep_alive (bool):
             If set, keeps the account alive by keeping the balance above the existential deposit.
         prompt (bool):
             If true, the call waits for confirmation from the user before proceeding.
     Returns:
         success (bool):
-            Flag is true if extrinsic was finalized or uncluded in the block. 
+            Flag is true if extrinsic was finalized or uncluded in the block.
             If we did not wait for finalization / inclusion, the response is true.
     """
     # Validate destination address.
     if not is_valid_bittensor_address_or_public_key( dest ):
         bittensor.__console__.print(":cross_mark: [red]Invalid destination address[/red]:[bold white]\n  {}[/bold white]".format(dest))
         return False
 
@@ -83,29 +83,29 @@
 
     with bittensor.__console__.status(":satellite: Transferring..."):
         with subtensor.substrate as substrate:
             call = substrate.compose_call(
                 call_module='Balances',
                 call_function='transfer',
                 call_params={
-                    'dest': dest, 
+                    'dest': dest,
                     'value': transfer_balance.rao
                 }
             )
 
             try:
                 payment_info = substrate.get_payment_info( call = call, keypair = wallet.coldkey )
             except Exception as e:
                 bittensor.__console__.print(":cross_mark: [red]Failed to get payment info[/red]:[bold white]\n  {}[/bold white]".format(e))
                 payment_info = {
-                    'partialFee': 2e7, # assume  0.02 Tao 
+                    'partialFee': 2e7, # assume  0.02 Tao
                 }
 
             fee = bittensor.Balance.from_rao( payment_info['partialFee'] )
-    
+
     if not keep_alive:
         # Check if the transfer should keep_alive the account
         existential_deposit = bittensor.Balance(0)
 
     # Check if we have enough balance.
     if account_balance < (transfer_balance + fee + existential_deposit):
         bittensor.__console__.print(":cross_mark: [red]Not enough balance[/red]:[bold white]\n  balance: {}\n  amount: {}\n  for fee: {}[/bold white]".format( account_balance, transfer_balance, fee ))
@@ -118,15 +118,15 @@
 
     with bittensor.__console__.status(":satellite: Transferring..."):
         with subtensor.substrate as substrate:
             call = substrate.compose_call(
                 call_module='Balances',
                 call_function='transfer',
                 call_params={
-                    'dest': dest, 
+                    'dest': dest,
                     'value': transfer_balance.rao
                 }
             )
             extrinsic = substrate.create_signed_extrinsic( call = call, keypair = wallet.coldkey )
             response = substrate.submit_extrinsic( extrinsic, wait_for_inclusion = wait_for_inclusion, wait_for_finalization = wait_for_finalization )
             # We only wait here if we expect finalization.
             if not wait_for_finalization and not wait_for_inclusion:
@@ -135,22 +135,22 @@
 
             # Otherwise continue with finalization.
             response.process_events()
             if response.is_success:
                 bittensor.__console__.print(":white_heavy_check_mark: [green]Finalized[/green]")
                 block_hash = response.block_hash
                 bittensor.__console__.print("[green]Block Hash: {}[/green]".format( block_hash ))
-                
+
                 explorer_url = bittensor.utils.get_explorer_url_for_network( subtensor.network, block_hash, bittensor.__network_explorer_map__ )
                 if explorer_url is not None:
                     bittensor.__console__.print("[green]Explorer Link: {}[/green]".format( explorer_url ))
-                
+
             else:
                 bittensor.__console__.print(":cross_mark: [red]Failed[/red]: error:{}".format(response.error_message))
 
     if response.is_success:
         with bittensor.__console__.status(":satellite: Checking Balance..."):
             new_balance = subtensor.get_balance( wallet.coldkey.ss58_address )
             bittensor.__console__.print("Balance:\n  [blue]{}[/blue] :arrow_right: [green]{}[/green]".format(account_balance, new_balance))
             return True
-    
+
     return False
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/unstaking.py` & `bittensor-5.0.0/bittensor/_subtensor/extrinsics/unstaking.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 # Copyright © 2023 Opentensor Foundation
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import bittensor
 
 from rich.prompt import Confirm
 from time import sleep
 from typing import List, Dict, Union, Optional
 from bittensor.utils.balance import Balance
-from ..errors import * 
+from ..errors import *
 
 def __do_remove_stake_single(
     subtensor: 'bittensor.Subtensor',
     wallet: 'bittensor.wallet',
     hotkey_ss58: str,
-    amount: 'bittensor.Balance', 
+    amount: 'bittensor.Balance',
     wait_for_inclusion: bool = True,
     wait_for_finalization: bool = False,
 ) -> bool:
     r"""
     Executes an unstake call to the chain using the wallet and amount specified.
     Args:
         wallet (bittensor.wallet):
             Bittensor wallet object.
         hotkey_ss58 (str):
             Hotkey address to unstake from.
         amount (bittensor.Balance):
             Amount to unstake as bittensor balance object.
         wait_for_inclusion (bool):
-            If set, waits for the extrinsic to enter a block before returning true, 
-            or returns false if the extrinsic fails to enter the block within the timeout.   
+            If set, waits for the extrinsic to enter a block before returning true,
+            or returns false if the extrinsic fails to enter the block within the timeout.
         wait_for_finalization (bool):
             If set, waits for the extrinsic to be finalized on the chain before returning true,
             or returns false if the extrinsic fails to be finalized within the timeout.
         prompt (bool):
             If true, the call waits for confirmation from the user before proceeding.
     Returns:
         success (bool):
-            flag is true if extrinsic was finalized or uncluded in the block. 
+            flag is true if extrinsic was finalized or uncluded in the block.
             If we did not wait for finalization / inclusion, the response is true.
     Raises:
         StakeError:
             If the extrinsic fails to be finalized or included in the block.
         NotRegisteredError:
             If the hotkey is not registered in any subnets.
 
     """
     # Decrypt keys,
     wallet.coldkey
 
     with subtensor.substrate as substrate:
         call = substrate.compose_call(
-        call_module='SubtensorModule', 
+        call_module='SubtensorModule',
         call_function='remove_stake',
         call_params={
             'hotkey': hotkey_ss58,
             'amount_unstaked': amount.rao
             }
         )
         extrinsic = substrate.create_signed_extrinsic( call = call, keypair = wallet.coldkey )
@@ -84,49 +84,49 @@
         else:
             raise StakeError(response.error_message)
 
 def unstake_extrinsic (
         subtensor: 'bittensor.Subtensor',
         wallet: 'bittensor.wallet',
         hotkey_ss58: Optional[str] = None,
-        amount: Union[Balance, float] = None, 
-        wait_for_inclusion:bool = True, 
+        amount: Union[Balance, float] = None,
+        wait_for_inclusion:bool = True,
         wait_for_finalization:bool = False,
         prompt: bool = False,
     ) -> bool:
     r""" Removes stake into the wallet coldkey from the specified hotkey uid.
     Args:
         wallet (bittensor.wallet):
             bittensor wallet object.
         hotkey_ss58 (Optional[str]):
             ss58 address of the hotkey to unstake from.
             by default, the wallet hotkey is used.
         amount (Union[Balance, float]):
             Amount to stake as bittensor balance, or float interpreted as tao.
         wait_for_inclusion (bool):
-            if set, waits for the extrinsic to enter a block before returning true, 
-            or returns false if the extrinsic fails to enter the block within the timeout.   
+            if set, waits for the extrinsic to enter a block before returning true,
+            or returns false if the extrinsic fails to enter the block within the timeout.
         wait_for_finalization (bool):
             if set, waits for the extrinsic to be finalized on the chain before returning true,
             or returns false if the extrinsic fails to be finalized within the timeout.
         prompt (bool):
             If true, the call waits for confirmation from the user before proceeding.
     Returns:
         success (bool):
-            flag is true if extrinsic was finalized or uncluded in the block. 
+            flag is true if extrinsic was finalized or uncluded in the block.
             If we did not wait for finalization / inclusion, the response is true.
     """
     # Decrypt keys,
     wallet.coldkey
 
     if hotkey_ss58 is None:
         hotkey_ss58 = wallet.hotkey.ss58_address # Default to wallet's own hotkey.
 
     with bittensor.__console__.status(":satellite: Syncing with chain: [white]{}[/white] ...".format(subtensor.network)):
-        old_balance = subtensor.get_balance( wallet.coldkeypub.ss58_address )        
+        old_balance = subtensor.get_balance( wallet.coldkeypub.ss58_address )
         old_stake = subtensor.get_stake_for_coldkey_and_hotkey( coldkey_ss58 = wallet.coldkeypub.ss58_address, hotkey_ss58 = hotkey_ss58 )
 
     # Convert to bittensor.Balance
     if amount == None:
         # Unstake it all.
         unstaking_balance = old_stake
     elif not isinstance(amount, bittensor.Balance ):
@@ -135,21 +135,21 @@
         unstaking_balance = amount
 
     # Check enough to unstake.
     stake_on_uid = old_stake
     if unstaking_balance > stake_on_uid:
         bittensor.__console__.print(":cross_mark: [red]Not enough stake[/red]: [green]{}[/green] to unstake: [blue]{}[/blue] from hotkey: [white]{}[/white]".format(stake_on_uid, unstaking_balance, wallet.hotkey_str))
         return False
-    
+
     # Ask before moving on.
     if prompt:
         if not Confirm.ask("Do you want to unstake:\n[bold white]  amount: {}\n  hotkey: {}[/bold white ]?".format( unstaking_balance, wallet.hotkey_str) ):
             return False
 
-    
+
     try:
         with bittensor.__console__.status(":satellite: Unstaking from chain: [white]{}[/white] ...".format(subtensor.network)):
             staking_response: bool = __do_remove_stake_single(
                 subtensor = subtensor,
                 wallet = wallet,
                 hotkey_ss58 = hotkey_ss58,
                 amount = unstaking_balance,
@@ -176,49 +176,49 @@
 
     except NotRegisteredError as e:
         bittensor.__console__.print(":cross_mark: [red]Hotkey: {} is not registered.[/red]".format(wallet.hotkey_str))
         return False
     except StakeError as e:
         bittensor.__console__.print(":cross_mark: [red]Stake Error: {}[/red]".format(e))
         return False
-        
+
 def unstake_multiple_extrinsic (
         subtensor: 'bittensor.Subtensor',
         wallet: 'bittensor.wallet',
         hotkey_ss58s: List[str],
-        amounts: List[Union[Balance, float]] = None, 
-        wait_for_inclusion: bool = True, 
+        amounts: List[Union[Balance, float]] = None,
+        wait_for_inclusion: bool = True,
         wait_for_finalization: bool = False,
         prompt: bool = False,
     ) -> bool:
     r""" Removes stake from each hotkey_ss58 in the list, using each amount, to a common coldkey.
     Args:
         wallet (bittensor.wallet):
             The wallet with the coldkey to unstake to.
         hotkey_ss58s (List[str]):
             List of hotkeys to unstake from.
         amounts (List[Union[Balance, float]]):
             List of amounts to unstake. If None, unstake all.
         wait_for_inclusion (bool):
-            if set, waits for the extrinsic to enter a block before returning true, 
-            or returns false if the extrinsic fails to enter the block within the timeout.   
+            if set, waits for the extrinsic to enter a block before returning true,
+            or returns false if the extrinsic fails to enter the block within the timeout.
         wait_for_finalization (bool):
             if set, waits for the extrinsic to be finalized on the chain before returning true,
             or returns false if the extrinsic fails to be finalized within the timeout.
         prompt (bool):
             If true, the call waits for confirmation from the user before proceeding.
     Returns:
         success (bool):
             flag is true if extrinsic was finalized or included in the block.
             flag is true if any wallet was unstaked.
             If we did not wait for finalization / inclusion, the response is true.
     """
     if not isinstance(hotkey_ss58s, list) or not all(isinstance(hotkey_ss58, str) for hotkey_ss58 in hotkey_ss58s):
         raise TypeError("hotkey_ss58s must be a list of str")
-    
+
     if len(hotkey_ss58s) == 0:
         return True
 
     if amounts is not None and len(amounts) != len(hotkey_ss58s):
         raise ValueError("amounts must be a list of the same length as hotkey_ss58s")
 
     if amounts is not None and not all(isinstance(amount, (Balance, float)) for amount in amounts):
@@ -257,20 +257,20 @@
             unstaking_balance = amount
 
         # Check enough to unstake.
         stake_on_uid = old_stake
         if unstaking_balance > stake_on_uid:
             bittensor.__console__.print(":cross_mark: [red]Not enough stake[/red]: [green]{}[/green] to unstake: [blue]{}[/blue] from hotkey: [white]{}[/white]".format(stake_on_uid, unstaking_balance, wallet.hotkey_str))
             continue
-      
+
         # Ask before moving on.
         if prompt:
             if not Confirm.ask("Do you want to unstake:\n[bold white]  amount: {}\n  hotkey: {}[/bold white ]?".format( unstaking_balance, wallet.hotkey_str) ):
                 continue
-        
+
         try:
             with bittensor.__console__.status(":satellite: Unstaking from chain: [white]{}[/white] ...".format(subtensor.network)):
                 staking_response: bool = __do_remove_stake_single(
                     subtensor = subtensor,
                     wallet = wallet,
                     hotkey_ss58 = hotkey_ss58,
                     amount = unstaking_balance,
@@ -305,16 +305,16 @@
 
         except NotRegisteredError as e:
             bittensor.__console__.print(":cross_mark: [red]{} is not registered.[/red]".format(hotkey_ss58))
             continue
         except StakeError as e:
             bittensor.__console__.print(":cross_mark: [red]Stake Error: {}[/red]".format(e))
             continue
-            
-    
+
+
     if successful_unstakes != 0:
         with bittensor.__console__.status(":satellite: Checking Balance on: ([white]{}[/white] ...".format(subtensor.network)):
             new_balance = subtensor.get_balance( wallet.coldkeypub.ss58_address )
         bittensor.__console__.print("Balance: [blue]{}[/blue] :arrow_right: [green]{}[/green]".format( old_balance, new_balance ))
         return True
 
     return False
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_subtensor/subtensor_impl.py` & `bittensor-5.0.0/bittensor/_subtensor/subtensor_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 # Copyright © 2023 Opentensor Foundation
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 # Imports
 import torch
 import bittensor
 import scalecodec
 from retry import retry
@@ -42,30 +42,30 @@
 from loguru import logger
 logger = logger.opt(colors=True)
 
 class Subtensor:
     """
     Handles interactions with the subtensor chain.
     """
-    def __init__( 
-        self, 
+    def __init__(
+        self,
         substrate: 'SubstrateInterface',
         network: str,
         chain_endpoint: str,
     ):
         r""" Initializes a subtensor chain interface.
             Args:
-                substrate (:obj:`SubstrateInterface`, `required`): 
+                substrate (:obj:`SubstrateInterface`, `required`):
                     substrate websocket client.
                 network (default='local', type=str)
                     The subtensor network flag. The likely choices are:
                             -- local (local running network)
                             -- nobunaga (staging network)
-                            -- nakamoto (main network)
-                    If this option is set it overloads subtensor.chain_endpoint with 
+                            -- finney (main network)
+                    If this option is set it overloads subtensor.chain_endpoint with
                     an entry point node from that network.
                 chain_endpoint (default=None, type=str)
                     The subtensor endpoint flag. If set, overrides the network argument.
         """
         self.network = network
         self.chain_endpoint = chain_endpoint
         self.substrate = substrate
@@ -80,65 +80,65 @@
 
     def __repr__(self) -> str:
         return self.__str__()
 
     #####################
     #### Delegation #####
     #####################
-    def nominate( 
+    def nominate(
         self,
-        wallet: 'bittensor.Wallet', 
-        wait_for_finalization: bool = False, 
-        wait_for_inclusion: bool = True 
+        wallet: 'bittensor.Wallet',
+        wait_for_finalization: bool = False,
+        wait_for_inclusion: bool = True
     ) -> bool:
         """ Becomes a delegate for the hotkey."""
-        return nominate_extrinsic( 
-            subtensor = self, 
-            wallet = wallet, 
+        return nominate_extrinsic(
+            subtensor = self,
+            wallet = wallet,
             wait_for_finalization = wait_for_finalization,
             wait_for_inclusion = wait_for_inclusion
         )
 
     def delegate(
-        self, 
+        self,
         wallet: 'bittensor.wallet',
         delegate_ss58: Optional[str] = None,
-        amount: Union[Balance, float] = None, 
+        amount: Union[Balance, float] = None,
         wait_for_inclusion: bool = True,
         wait_for_finalization: bool = False,
         prompt: bool = False,
     ) -> bool:
         """ Adds the specified amount of stake to the passed delegate using the passed wallet. """
-        return delegate_extrinsic( 
-            subtensor = self, 
+        return delegate_extrinsic(
+            subtensor = self,
             wallet = wallet,
-            delegate_ss58 = delegate_ss58, 
-            amount = amount, 
+            delegate_ss58 = delegate_ss58,
+            amount = amount,
             wait_for_inclusion = wait_for_inclusion,
-            wait_for_finalization = wait_for_finalization, 
+            wait_for_finalization = wait_for_finalization,
             prompt = prompt
         )
 
     def undelegate(
-        self, 
+        self,
         wallet: 'bittensor.wallet',
         delegate_ss58: Optional[str] = None,
-        amount: Union[Balance, float] = None, 
+        amount: Union[Balance, float] = None,
         wait_for_inclusion: bool = True,
         wait_for_finalization: bool = False,
         prompt: bool = False,
     ) -> bool:
         """ Removes the specified amount of stake from the passed delegate using the passed wallet. """
-        return undelegate_extrinsic( 
-            subtensor = self, 
+        return undelegate_extrinsic(
+            subtensor = self,
             wallet = wallet,
-            delegate_ss58 = delegate_ss58, 
-            amount = amount, 
+            delegate_ss58 = delegate_ss58,
+            amount = amount,
             wait_for_inclusion = wait_for_inclusion,
-            wait_for_finalization = wait_for_finalization, 
+            wait_for_finalization = wait_for_finalization,
             prompt = prompt
         )
 
     #####################
     #### Set Weights ####
     #####################
     def set_weights(
@@ -148,15 +148,15 @@
         uids: Union[torch.LongTensor, list],
         weights: Union[torch.FloatTensor, list],
         version_key: int = bittensor.__version_as_int__,
         wait_for_inclusion:bool = False,
         wait_for_finalization:bool = False,
         prompt:bool = False
     ) -> bool:
-        return set_weights_extrinsic( 
+        return set_weights_extrinsic(
             subtensor=self,
             wallet=wallet,
             netuid=netuid,
             uids=uids,
             weights=weights,
             version_key=version_key,
             wait_for_inclusion=wait_for_inclusion,
@@ -180,109 +180,109 @@
         dev_id: Union[List[int], int] = 0,
         TPB: int = 256,
         num_processes: Optional[int] = None,
         update_interval: Optional[int] = None,
         log_verbose: bool = False,
     ) -> bool:
         """ Registers the wallet to chain."""
-        return register_extrinsic( 
-            subtensor = self, 
-            wallet = wallet, 
-            netuid = netuid, 
-            wait_for_inclusion = wait_for_inclusion, 
-            wait_for_finalization = wait_for_finalization, 
+        return register_extrinsic(
+            subtensor = self,
+            wallet = wallet,
+            netuid = netuid,
+            wait_for_inclusion = wait_for_inclusion,
+            wait_for_finalization = wait_for_finalization,
             prompt = prompt,
             max_allowed_attempts = max_allowed_attempts,
             output_in_place = output_in_place,
             cuda = cuda,
             dev_id = dev_id,
             TPB = TPB,
             num_processes = num_processes,
             update_interval = update_interval,
             log_verbose = log_verbose,
         )
-    
+
     def burned_register (
         self,
         wallet: 'bittensor.Wallet',
         netuid: int,
         wait_for_inclusion: bool = False,
         wait_for_finalization: bool = True,
         prompt: bool = False
     ) -> bool:
         """ Registers the wallet to chain by recycling TAO."""
-        return burned_register_extrinsic( 
-            subtensor = self, 
-            wallet = wallet, 
-            netuid = netuid, 
-            wait_for_inclusion = wait_for_inclusion, 
-            wait_for_finalization = wait_for_finalization, 
+        return burned_register_extrinsic(
+            subtensor = self,
+            wallet = wallet,
+            netuid = netuid,
+            wait_for_inclusion = wait_for_inclusion,
+            wait_for_finalization = wait_for_finalization,
             prompt = prompt
         )
 
     ##################
     #### Transfer ####
     ##################
     def transfer(
         self,
         wallet: 'bittensor.wallet',
-        dest: str, 
-        amount: Union[Balance, float], 
+        dest: str,
+        amount: Union[Balance, float],
         wait_for_inclusion: bool = True,
         wait_for_finalization: bool = False,
         prompt: bool = False,
     ) -> bool:
         """ Transfers funds from this wallet to the destination public key address"""
         return transfer_extrinsic(
             subtensor = self,
             wallet = wallet,
             dest = dest,
             amount = amount,
             wait_for_inclusion = wait_for_inclusion,
             wait_for_finalization = wait_for_finalization,
             prompt = prompt
         )
-    
+
     def get_existential_deposit(
         self,
         block: Optional[int] = None,
     ) -> Optional[Balance]:
         """ Returns the existential deposit for the chain. """
         result = self.query_constant(
             module_name='Balances',
             constant_name='ExistentialDeposit',
             block = block,
         )
-        
+
         if result is None:
             return None
-        
+
         return Balance.from_rao(result.value)
 
     #################
     #### Serving ####
     #################
     def serve (
         self,
         wallet: 'bittensor.wallet',
-        ip: str, 
-        port: int, 
-        protocol: int, 
+        ip: str,
+        port: int,
+        protocol: int,
         netuid: int,
         placeholder1: int = 0,
         placeholder2: int = 0,
         wait_for_inclusion: bool = False,
         wait_for_finalization = True,
         prompt: bool = False,
     ) -> bool:
         return serve_extrinsic( self, wallet, ip, port, protocol, netuid , placeholder1, placeholder2, wait_for_inclusion, wait_for_finalization)
 
     def serve_axon (
         self,
-        netuid: int, 
+        netuid: int,
         axon: 'bittensor.Axon',
         use_upnpc: bool = False,
         wait_for_inclusion: bool = False,
         wait_for_finalization: bool = True,
         prompt: bool = False,
     ) -> bool:
         return serve_axon_extrinsic( self, netuid, axon, use_upnpc, wait_for_inclusion, wait_for_finalization)
@@ -296,68 +296,68 @@
         wait_for_finalization: bool = True,
     ) -> bool:
         return prometheus_extrinsic( self, wallet = wallet, port = port, netuid = netuid, wait_for_inclusion = wait_for_inclusion, wait_for_finalization = wait_for_finalization)
     #################
     #### Staking ####
     #################
     def add_stake(
-        self, 
+        self,
         wallet: 'bittensor.wallet',
         hotkey_ss58: Optional[str] = None,
-        amount: Union[Balance, float] = None, 
+        amount: Union[Balance, float] = None,
         wait_for_inclusion: bool = True,
         wait_for_finalization: bool = False,
         prompt: bool = False,
     ) -> bool:
         """ Adds the specified amount of stake to passed hotkey uid. """
-        return add_stake_extrinsic( 
-            subtensor = self, 
+        return add_stake_extrinsic(
+            subtensor = self,
             wallet = wallet,
-            hotkey_ss58 = hotkey_ss58, 
-            amount = amount, 
+            hotkey_ss58 = hotkey_ss58,
+            amount = amount,
             wait_for_inclusion = wait_for_inclusion,
-            wait_for_finalization = wait_for_finalization, 
+            wait_for_finalization = wait_for_finalization,
             prompt = prompt
         )
 
     def add_stake_multiple (
-        self, 
+        self,
         wallet: 'bittensor.wallet',
         hotkey_ss58s: List[str],
-        amounts: List[Union[Balance, float]] = None, 
+        amounts: List[Union[Balance, float]] = None,
         wait_for_inclusion: bool = True,
         wait_for_finalization: bool = False,
         prompt: bool = False,
     ) -> bool:
         """ Adds stake to each hotkey_ss58 in the list, using each amount, from a common coldkey."""
         return add_stake_multiple_extrinsic( self, wallet, hotkey_ss58s, amounts, wait_for_inclusion, wait_for_finalization, prompt)
 
     ###################
     #### Unstaking ####
     ###################
     def unstake_multiple (
         self,
         wallet: 'bittensor.wallet',
         hotkey_ss58s: List[str],
-        amounts: List[Union[Balance, float]] = None, 
-        wait_for_inclusion: bool = True, 
+        amounts: List[Union[Balance, float]] = None,
+        wait_for_inclusion: bool = True,
         wait_for_finalization: bool = False,
         prompt: bool = False,
     ) -> bool:
         """ Removes stake from each hotkey_ss58 in the list, using each amount, to a common coldkey. """
         return unstake_multiple_extrinsic( self, wallet, hotkey_ss58s, amounts, wait_for_inclusion, wait_for_finalization, prompt)
 
-   
+
 
     def unstake (
         self,
         wallet: 'bittensor.wallet',
         hotkey_ss58: Optional[str] = None,
-        amount: Union[Balance, float] = None, 
-        wait_for_inclusion:bool = True, 
+        amount: Union[Balance, float] = None,
+        wait_for_inclusion:bool = True,
         wait_for_finalization:bool = False,
         prompt: bool = False,
     ) -> bool:
         """ Removes stake into the wallet coldkey from the specified hotkey uid."""
         return unstake_extrinsic( self, wallet, hotkey_ss58, amount, wait_for_inclusion, wait_for_finalization, prompt )
 
 
@@ -386,27 +386,27 @@
                 return substrate.query_map(
                     module='SubtensorModule',
                     storage_function = name,
                     params = params,
                     block_hash = None if block == None else substrate.get_block_hash(block)
                 )
         return make_substrate_call_with_retry()
-    
+
     """ Gets a constant from subtensor with module_name, constant_name, and block. """
     def query_constant( self, module_name: str, constant_name: str, block: Optional[int] = None ) -> Optional[object]:
         @retry(delay=2, tries=3, backoff=2, max_delay=4)
         def make_substrate_call_with_retry():
             with self.substrate as substrate:
                 return substrate.get_constant(
                     module_name=module_name,
                     constant_name=constant_name,
                     block_hash = None if block == None else substrate.get_block_hash(block)
                 )
         return make_substrate_call_with_retry()
-      
+
     #####################################
     #### Hyper parameter calls. ####
     #####################################
 
     """ Returns network Rho hyper parameter """
     def rho (self, netuid: int, block: Optional[int] = None ) -> Optional[int]:
         if not self.subnet_exists( netuid, block ): return None
@@ -417,15 +417,15 @@
         if not self.subnet_exists( netuid, block ): return None
         return U16_NORMALIZED_FLOAT( self.query_subtensor( "Kappa", block, [netuid] ).value )
 
     """ Returns network Difficulty hyper parameter """
     def difficulty (self, netuid: int, block: Optional[int] = None ) -> Optional[int]:
         if not self.subnet_exists( netuid, block ): return None
         return self.query_subtensor( "Difficulty", block, [netuid] ).value
-    
+
     """ Returns network Burn hyper parameter """
     def burn (self, netuid: int, block: Optional[int] = None ) -> Optional[bittensor.Balance]:
         if not self.subnet_exists( netuid, block ): return None
         return bittensor.Balance.from_rao( self.query_subtensor( "Burn", block, [netuid] ).value )
 
     """ Returns network ImmunityPeriod hyper parameter """
     def immunity_period (self, netuid: int, block: Optional[int] = None ) -> Optional[int]:
@@ -467,15 +467,15 @@
         if not self.subnet_exists( netuid, block ): return None
         return U16_NORMALIZED_FLOAT( self.query_subtensor("ValidatorExcludeQuantile", block, [netuid] ).value )
 
     """ Returns network MaxAllowedValidators hyper parameter """
     def max_allowed_validators(self, netuid: int, block: Optional[int] = None) -> Optional[int]:
         if not self.subnet_exists( netuid, block ): return None
         return self.query_subtensor( 'MaxAllowedValidators', block, [netuid] ).value
-        
+
     """ Returns network MinAllowedWeights hyper parameter """
     def min_allowed_weights (self, netuid: int, block: Optional[int] = None ) -> Optional[int]:
         if not self.subnet_exists( netuid, block ): return None
         return self.query_subtensor("MinAllowedWeights", block, [netuid] ).value
 
     """ Returns network MaxWeightsLimit hyper parameter """
     def max_weight_limit (self, netuid: int, block: Optional[int] = None ) -> Optional[float]:
@@ -541,15 +541,15 @@
         if self.does_hotkey_exist( hotkey_ss58, block ):
             return self.query_subtensor( 'Owner', block, [hotkey_ss58 ] ).value
         else:
             return None
 
     """ Returns the axon information for this hotkey account """
     def get_axon_info( self, hotkey_ss58: str, block: Optional[int] = None ) -> Optional[axon_info]:
-        result = self.query_subtensor( 'Axons', block, [hotkey_ss58 ] )        
+        result = self.query_subtensor( 'Axons', block, [hotkey_ss58 ] )
         if result != None:
             return axon_info(
                 ip = bittensor.utils.networking.ip_from_int( result.value.ip ),
                 ip_type = result.value.ip_type,
                 port = result.value.port,
                 protocol = result.value.protocol,
                 version = result.value.version,
@@ -557,15 +557,15 @@
                 placeholder2 = result.value.placeholder2,
             )
         else:
             return None
 
     """ Returns the prometheus information for this hotkey account """
     def get_prometheus_info( self, hotkey_ss58: str, block: Optional[int] = None ) -> Optional[axon_info]:
-        result = self.query_subtensor( 'Prometheus', block, [hotkey_ss58 ] )        
+        result = self.query_subtensor( 'Prometheus', block, [hotkey_ss58 ] )
         if result != None:
             return PrometheusInfo (
                 ip = bittensor.utils.networking.ip_from_int( result.value.ip ),
                 ip_type = result.value.ip_type,
                 port = result.value.port,
                 version = result.value.version,
                 block = result.value.block,
@@ -594,36 +594,39 @@
 
     def serving_rate_limit (self, block: Optional[int] = None ) -> Optional[int]:
         return self.query_subtensor( "ServingRateLimit", block ).value
     
     def tx_rate_limit (self, block: Optional[int] = None ) -> Optional[int]:
         return self.query_subtensor( "TxRateLimit", block ).value
 
+    def tx_rate_limit (self, block: Optional[int] = None ) -> Optional[int]:
+        return self.query_subtensor( "TxRateLimit", block ).value
+
     #####################################
     #### Network Parameters ####
     #####################################
 
     def subnet_exists( self, netuid: int, block: Optional[int] = None ) -> bool:
-        return self.query_subtensor( 'NetworksAdded', block, [netuid] ).value  
+        return self.query_subtensor( 'NetworksAdded', block, [netuid] ).value
 
     def get_all_subnet_netuids( self, block: Optional[int] = None ) -> List[int]:
         subnet_netuids = []
         result = self.query_map_subtensor( 'NetworksAdded', block )
         if result.records:
-            for netuid, exists in result:  
+            for netuid, exists in result:
                 if exists:
                     subnet_netuids.append( netuid.value )
-            
+
         return subnet_netuids
 
     def get_total_subnets( self, block: Optional[int] = None ) -> int:
-        return self.query_subtensor( 'TotalNetworks', block ).value      
+        return self.query_subtensor( 'TotalNetworks', block ).value
 
     def get_subnet_modality( self, netuid: int, block: Optional[int] = None ) -> Optional[int]:
-        return self.query_subtensor( 'NetworkModality', block, [netuid] ).value   
+        return self.query_subtensor( 'NetworkModality', block, [netuid] ).value
 
     def get_subnet_connection_requirement( self, netuid_0: int, netuid_1: int, block: Optional[int] = None) -> Optional[int]:
         return self.query_subtensor( 'NetworkConnect', block, [netuid_0, netuid_1] ).value
 
     def get_emission_value_by_subnet( self, netuid: int, block: Optional[int] = None ) -> Optional[float]:
         return bittensor.Balance.from_rao( self.query_subtensor( 'EmissionValues', block, [ netuid ] ).value )
 
@@ -654,55 +657,55 @@
                 params = []
                 if block_hash:
                     params = params + [block_hash]
                 return substrate.rpc_request(
                     method="subnetInfo_getSubnetsInfo", # custom rpc method
                     params=params
                 )
-        
+
         json_body = make_substrate_call_with_retry()
         result = json_body['result']
 
         if result in (None, []):
             return []
-        
+
         return SubnetInfo.list_from_vec_u8( result )
 
     def get_subnet_info( self, netuid: int, block: Optional[int] = None ) -> Optional[SubnetInfo]:
         @retry(delay=2, tries=3, backoff=2, max_delay=4)
         def make_substrate_call_with_retry():
             with self.substrate as substrate:
                 block_hash = None if block == None else substrate.get_block_hash( block )
                 params = [netuid]
                 if block_hash:
                     params = params + [block_hash]
                 return substrate.rpc_request(
                     method="subnetInfo_getSubnetInfo", # custom rpc method
                     params=params
                 )
-        
+
         json_body = make_substrate_call_with_retry()
         result = json_body['result']
 
         if result in (None, []):
             return None
-        
+
         return SubnetInfo.from_vec_u8( result )
-        
+
     ####################
     #### Nomination ####
     ####################
     def is_hotkey_delegate( self, hotkey_ss58: str ) -> bool:
         return hotkey_ss58 in [ info.hotkey_ss58 for info in self.get_delegates() ]
 
     def get_delegate_take( self, hotkey_ss58: str, block: Optional[int] = None ) -> Optional[float]:
         return U16_NORMALIZED_FLOAT( self.query_subtensor( 'Delegates', block, [ hotkey_ss58 ] ).value )
 
     def get_nominators_for_hotkey( self, hotkey_ss58: str, block: Optional[int] = None ) -> List[Tuple[str, Balance]]:
-        result = self.query_map_subtensor( 'Stake', block, [ hotkey_ss58 ] ) 
+        result = self.query_map_subtensor( 'Stake', block, [ hotkey_ss58 ] )
         if result.records:
             return [(record[0].value, record[1].value) for record in result.records]
         else:
             return 0
 
     def get_delegate_by_hotkey( self, hotkey_ss58: str, block: Optional[int] = None ) -> Optional[DelegateInfo]:
         @retry(delay=2, tries=3, backoff=2, max_delay=4)
@@ -720,15 +723,15 @@
         hotkey_bytes: bytes = bittensor.utils.ss58_address_to_bytes( hotkey_ss58 )
         encoded_hotkey: List[int] = [ int( byte ) for byte in hotkey_bytes ]
         json_body = make_substrate_call_with_retry(encoded_hotkey)
         result = json_body['result']
 
         if result in (None, []):
             return None
-            
+
         return DelegateInfo.from_vec_u8( result )
 
     def get_delegates( self, block: Optional[int] = None ) -> List[DelegateInfo]:
         @retry(delay=2, tries=3, backoff=2, max_delay=4)
         def make_substrate_call_with_retry():
             with self.substrate as substrate:
                 block_hash = None if block == None else substrate.get_block_hash( block )
@@ -742,15 +745,15 @@
         json_body = make_substrate_call_with_retry()
         result = json_body['result']
 
         if result in (None, []):
             return []
 
         return DelegateInfo.list_from_vec_u8( result )
-    
+
     def get_delegated( self, coldkey_ss58: str, block: Optional[int] = None ) -> List[Tuple[DelegateInfo, Balance]]:
         """ Returns the list of delegates that a given coldkey is staked to.
         """
         @retry(delay=2, tries=3, backoff=2, max_delay=4)
         def make_substrate_call_with_retry(encoded_coldkey: List[int]):
             with self.substrate as substrate:
                 block_hash = None if block == None else substrate.get_block_hash( block )
@@ -775,51 +778,51 @@
 
     ########################################
     #### Neuron information per subnet ####
     ########################################
 
     def is_hotkey_registered_any( self, hotkey_ss58: str, block: Optional[int] = None) -> bool:
         return len( self.get_netuids_for_hotkey( hotkey_ss58, block) ) > 0
-    
+
     def is_hotkey_registered_on_subnet( self, hotkey_ss58: str, netuid: int, block: Optional[int] = None) -> bool:
         return self.get_uid_for_hotkey_on_subnet( hotkey_ss58, netuid, block ) != None
 
     def is_hotkey_registered( self, hotkey_ss58: str, netuid: int, block: Optional[int] = None) -> bool:
         return self.get_uid_for_hotkey_on_subnet( hotkey_ss58, netuid, block ) != None
 
     def get_uid_for_hotkey_on_subnet( self, hotkey_ss58: str, netuid: int, block: Optional[int] = None) -> int:
-        return self.query_subtensor( 'Uids', block, [ netuid, hotkey_ss58 ] ).value  
+        return self.query_subtensor( 'Uids', block, [ netuid, hotkey_ss58 ] ).value
 
     def get_all_uids_for_hotkey( self, hotkey_ss58: str, block: Optional[int] = None) -> List[int]:
         return [ self.get_uid_for_hotkey_on_subnet( hotkey_ss58, netuid, block) for netuid in self.get_netuids_for_hotkey( hotkey_ss58, block)]
 
     def get_netuids_for_hotkey( self, hotkey_ss58: str, block: Optional[int] = None) -> List[int]:
-        result = self.query_map_subtensor( 'IsNetworkMember', block, [ hotkey_ss58 ] )   
+        result = self.query_map_subtensor( 'IsNetworkMember', block, [ hotkey_ss58 ] )
         netuids = []
         for netuid, is_member in result.records:
             if is_member:
                 netuids.append( netuid.value )
         return netuids
 
     def get_neuron_for_pubkey_and_subnet( self, hotkey_ss58: str, netuid: int, block: Optional[int] = None ) -> Optional[NeuronInfo]:
         return self.neuron_for_uid( self.get_uid_for_hotkey_on_subnet(hotkey_ss58, netuid, block=block), netuid, block = block)
 
     def get_all_neurons_for_pubkey( self, hotkey_ss58: str, block: Optional[int] = None ) -> List[NeuronInfo]:
-        netuids = self.get_netuids_for_hotkey( hotkey_ss58, block) 
-        uids = [self.get_uid_for_hotkey_on_subnet(hotkey_ss58, net) for net in netuids] 
+        netuids = self.get_netuids_for_hotkey( hotkey_ss58, block)
+        uids = [self.get_uid_for_hotkey_on_subnet(hotkey_ss58, net) for net in netuids]
         return [self.neuron_for_uid( uid, net ) for uid, net in list(zip(uids, netuids))]
 
     def neuron_has_validator_permit( self, uid: int, netuid: int, block: Optional[int] = None ) -> Optional[bool]:
         return self.query_subtensor( 'ValidatorPermit', block, [ netuid, uid ] ).value
 
-    def neuron_for_wallet( self, wallet: 'bittensor.Wallet', netuid = int, block: Optional[int] = None ) -> Optional[NeuronInfo]: 
+    def neuron_for_wallet( self, wallet: 'bittensor.Wallet', netuid = int, block: Optional[int] = None ) -> Optional[NeuronInfo]:
         return self.get_neuron_for_pubkey_and_subnet ( wallet.hotkey.ss58_address, netuid = netuid, block = block )
 
-    def neuron_for_uid( self, uid: int, netuid: int, block: Optional[int] = None ) -> Optional[NeuronInfo]: 
-        r""" Returns a list of neuron from the chain. 
+    def neuron_for_uid( self, uid: int, netuid: int, block: Optional[int] = None ) -> Optional[NeuronInfo]:
+        r""" Returns a list of neuron from the chain.
         Args:
             uid ( int ):
                 The uid of the neuron to query for.
             netuid ( int ):
                 The uid of the network to query for.
             block ( int ):
                 The neuron at a particular block
@@ -840,19 +843,19 @@
                     params=params
                 )
         json_body = make_substrate_call_with_retry()
         result = json_body['result']
 
         if result in (None, []):
             return NeuronInfo._null_neuron()
-        
-        return NeuronInfo.from_vec_u8( result ) 
 
-    def neurons(self, netuid: int, block: Optional[int] = None ) -> List[NeuronInfo]: 
-        r""" Returns a list of neuron from the chain. 
+        return NeuronInfo.from_vec_u8( result )
+
+    def neurons(self, netuid: int, block: Optional[int] = None ) -> List[NeuronInfo]:
+        r""" Returns a list of neuron from the chain.
         Args:
             netuid ( int ):
                 The netuid of the subnet to pull neurons from.
             block ( Optional[int] ):
                 block to sync from.
         Returns:
             neuron (List[NeuronInfo]):
@@ -865,25 +868,25 @@
                 params = [netuid]
                 if block_hash:
                     params = params + [block_hash]
                 return substrate.rpc_request(
                     method="neuronInfo_getNeurons", # custom rpc method
                     params=params
                 )
-        
+
         json_body = make_substrate_call_with_retry()
         result = json_body['result']
 
         if result in (None, []):
             return []
-        
+
         return NeuronInfo.list_from_vec_u8( result )
-    
-    def neuron_for_uid_lite( self, uid: int, netuid: int, block: Optional[int] = None ) -> Optional[NeuronInfoLite]: 
-        r""" Returns a list of neuron lite from the chain. 
+
+    def neuron_for_uid_lite( self, uid: int, netuid: int, block: Optional[int] = None ) -> Optional[NeuronInfoLite]:
+        r""" Returns a list of neuron lite from the chain.
         Args:
             uid ( int ):
                 The uid of the neuron to query for.
             netuid ( int ):
                 The uid of the network to query for.
             block ( int ):
                 The neuron at a particular block
@@ -894,29 +897,29 @@
         if uid == None: return NeuronInfoLite._null_neuron()
         @retry(delay=2, tries=3, backoff=2, max_delay=4)
         def make_substrate_call_with_retry():
             with self.substrate as substrate:
                 block_hash = None if block == None else substrate.get_block_hash( block )
                 params = [netuid, uid]
                 if block_hash:
-                    params = params + [block_hash] 
+                    params = params + [block_hash]
                 return substrate.rpc_request(
                     method="neuronInfo_getNeuronLite", # custom rpc method
                     params=params
                 )
         json_body = make_substrate_call_with_retry()
         result = json_body['result']
 
         if result in (None, []):
             return NeuronInfoLite._null_neuron()
-        
-        return NeuronInfoLite.from_vec_u8( result ) 
 
-    def neurons_lite(self, netuid: int, block: Optional[int] = None ) -> List[NeuronInfoLite]: 
-        r""" Returns a list of neuron lite from the chain. 
+        return NeuronInfoLite.from_vec_u8( result )
+
+    def neurons_lite(self, netuid: int, block: Optional[int] = None ) -> List[NeuronInfoLite]:
+        r""" Returns a list of neuron lite from the chain.
         Args:
             netuid ( int ):
                 The netuid of the subnet to pull neurons from.
             block ( Optional[int] ):
                 block to sync from.
         Returns:
             neuron (List[NeuronInfoLite]):
@@ -929,42 +932,42 @@
                 params = [netuid]
                 if block_hash:
                     params = params + [block_hash]
                 return substrate.rpc_request(
                     method="neuronInfo_getNeuronsLite", # custom rpc method
                     params=params
                 )
-        
+
         json_body = make_substrate_call_with_retry()
         result = json_body['result']
 
         if result in (None, []):
             return []
-        
+
         return NeuronInfoLite.list_from_vec_u8( result )
 
     def metagraph( self, netuid: int, lite: bool = True ) -> 'bittensor.Metagraph':
         r""" Returns the metagraph for the subnet.
         Args:
             netuid ( int ):
                 The network uid of the subnet to query.
             lite (bool, default=True):
                 If true, returns a metagraph using the lite sync (no weights, no bonds)
         Returns:
             metagraph ( `bittensor.Metagraph` ):
                 The metagraph for the subnet at the block.
-        """        
+        """
         return bittensor.metagraph( network = self.network, netuid = netuid, lite = lite )
 
     ################
     #### Transfer ##
     ################
 
 
-    
+
 
     ################
     #### Legacy ####
     ################
 
     def get_balance(self, address: str, block: int = None) -> Balance:
         r""" Returns the token balance for the passed ss58_address address
@@ -992,15 +995,15 @@
         return Balance( result.value['data']['free'] )
 
     def get_current_block(self) -> int:
         r""" Returns the current block number on the chain.
         Returns:
             block_number (int):
                 Current chain blocknumber.
-        """        
+        """
         @retry(delay=2, tries=3, backoff=2, max_delay=4)
         def make_substrate_call_with_retry():
             with self.substrate as substrate:
                 return substrate.get_block_number(None)
         return make_substrate_call_with_retry()
 
     def get_balances(self, block: int = None) -> Dict[str, Balance]:
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_subtensor/subtensor_mock.py` & `bittensor-5.0.0/bittensor/_subtensor/subtensor_mock.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # The MIT License (MIT)
 # Copyright © 2022 Opentensor Foundation
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 from substrateinterface import SubstrateInterface, Keypair
 from scalecodec import GenericCall
 import psutil
 import subprocess
 from sys import platform
@@ -32,21 +32,21 @@
     "runtime_id": 2,
     "types": {
         "Balance": "u64",
         "NeuronMetadataOf": {
             "type": "struct",
             "type_mapping": [
                 ["version", "u32"],
-                ["ip", "u128"], 
-                ["port", "u16"], 
-                ["ip_type", "u8"], 
-                ["uid", "u32"], 
-                ["modality", "u8"], 
-                ["hotkey", "AccountId"], 
-                ["coldkey", "AccountId"], 
+                ["ip", "u128"],
+                ["port", "u16"],
+                ["ip_type", "u8"],
+                ["uid", "u32"],
+                ["modality", "u8"],
+                ["hotkey", "AccountId"],
+                ["coldkey", "AccountId"],
                 ["active", "bool"],
                 ["last_update", "u64"],
                 ["validator_permit", "bool"],
                 ["stake", "u64"],
                 ["rank", "u16"],
                 ["trust", "u16"],
                 ["consensus", "u16"],
@@ -86,15 +86,15 @@
         substrate = SubstrateInterface(
             ss58_format = bittensor.__ss58_format__,
             type_registry_preset='substrate-node-template',
             type_registry = __type_registery__,
             url = "ws://{}".format('localhost:{}'.format(port)),
             use_remote_preset=True
         )
-        subtensor = Mock_Subtensor( 
+        subtensor = Mock_Subtensor(
             substrate = substrate,
             network = 'mock',
             chain_endpoint = 'localhost:{}'.format(port),
 
             # Is mocked, optionally has owned process for ref counting.
             _is_mocked = True,
             _owned_mock_subtensor_process = _owned_mock_subtensor_process
@@ -128,35 +128,35 @@
         r""" Creates a global mocked subtensor process running in the backgroun with name GLOBAL_SUBTENSOR_MOCK_PROCESS_NAME.
         """
         try:
             operating_system = "OSX" if platform == "darwin" else "Linux"
             path_root = "./tests/mock_subtensor"
             path = "{}/bin/{}/{}".format(path_root, operating_system, GLOBAL_SUBTENSOR_MOCK_PROCESS_NAME)
             path_to_spec = "{}/specs/local_raw.json".format(path_root)
-            
+
             ws_port = int(bittensor.__mock_entrypoint__.split(':')[1])
             print(f'MockSub ws_port: {ws_port}')
-            
+
             command_args = [ path ] + f'--chain {path_to_spec} --base-path {bittensor.__mock_chain_db__}_{pid} --execution native --ws-max-connections 1000 --no-mdns --rpc-cors all'.split(' ') + \
                 f'--port {int(bittensor.get_random_unused_port())} --rpc-port {int(bittensor.get_random_unused_port())} --ws-port {ws_port}'.split(' ') + \
                 '--validator --alice'.split(' ')
-            
+
             print ('Starting subtensor process with command: {}'.format(command_args))
-            
+
             _mock_subtensor_process = subprocess.Popen(
                 command_args,
                 close_fds=True, shell=False, stdout=subprocess.PIPE, stderr=subprocess.PIPE )
-            
+
             # Wait for the process to start. Check for errors.
             try:
                 # Timeout is okay.
                 error_code = _mock_subtensor_process.wait(timeout=12)
             except subprocess.TimeoutExpired:
                 error_code = None
-            
+
             if error_code is not None:
                 # Get the error message.
                 error_message = _mock_subtensor_process.stderr.read().decode('utf-8')
                 raise RuntimeError( 'Failed to start mocked subtensor process: {}'.format(error_code), error_message )
 
             print ('Starting subtensor process with pid {} and name {}'.format(_mock_subtensor_process.pid, GLOBAL_SUBTENSOR_MOCK_PROCESS_NAME))
 
@@ -164,28 +164,28 @@
             while errored:
                 errored = False
                 try:
                     _ = requests.get('http://localhost:{}'.format(ws_port))
                 except requests.exceptions.ConnectionError as e:
                     errored = True
                     time.sleep(0.5) # Wait for the process to start.
-            
+
             return _mock_subtensor_process
         except Exception as e:
             raise RuntimeError( 'Failed to start mocked subtensor process: {}'.format(e) )
 
 
 class Mock_Subtensor(subtensor_impl.Subtensor):
     """
     Handles interactions with the subtensor chain.
     """
     sudo_keypair: Keypair = Keypair.create_from_uri('//Alice') # Alice is the sudo keypair for the mock chain.
-    
-    def __init__( 
-        self, 
+
+    def __init__(
+        self,
         _is_mocked: bool,
         _owned_mock_subtensor_process: object,
         **kwargs,
     ):
         r""" Initializes a subtensor chain interface.
             Args:
                 _owned_mock_subtensor_process (Used for testing):
@@ -204,30 +204,30 @@
             return "MockSubtensor({}, PID:{})".format( self.chain_endpoint, self._owned_mock_subtensor_process.pid)
         else:
             # Mocked but does not own process.
             return "MockSubtensor({})".format( self.chain_endpoint)
 
     def __del__(self):
         self.optionally_kill_owned_mock_instance()
-    
+
     def __exit__(self):
         pass
-    
+
     def optionally_kill_owned_mock_instance(self):
         r""" If this subtensor instance owns the mock process, it kills the process.
         """
         if self._owned_mock_subtensor_process != None:
             try:
                 self._owned_mock_subtensor_process.terminate()
                 self._owned_mock_subtensor_process.kill()
                 os.system("kill %i" % self._owned_mock_subtensor_process.pid)
                 time.sleep(2) # Buffer to ensure the processes actually die
             except Exception as e:
                 print(f"failed to kill owned mock instance: {e}")
-                # Occasionally 
+                # Occasionally
                 pass
 
     def wrap_sudo(self, call: GenericCall) -> GenericCall:
         r""" Wraps a call in a sudo call.
         """
         return self.substrate.compose_call(
             call_module='Sudo',
@@ -244,15 +244,15 @@
             balance = balance.rao
         elif isinstance(balance, float):
             balance = int(balance * bittensor.utils.RAOPERTAO)
         elif isinstance(balance, int):
             pass
         else:
             raise ValueError('Invalid type for balance: {}'.format(type(balance)))
-        
+
         with self.substrate as substrate:
             call = substrate.compose_call(
                     call_module='Balances',
                     call_function='set_balance',
                     call_params = {
                         'who': ss58_address,
                         'new_free': balance,
@@ -266,15 +266,14 @@
             response = substrate.submit_extrinsic( extrinsic, wait_for_inclusion = True, wait_for_finalization = True )
 
             response.process_events()
             if response.is_success:
                 return True, None
             else:
                 return False, response.error_message
-            
     def sudo_set_tx_rate_limit(self, netuid: int, tx_rate_limit: int, wait_for_inclusion: bool = True, wait_for_finalization: bool = True ) -> Tuple[bool, Optional[str]]:
         r""" Sets the tx rate limit of the subnet in the mock chain using the sudo key.
         """
         with self.substrate as substrate:
             call = substrate.compose_call(
                     call_module='SubtensorModule',
                     call_function='sudo_set_tx_rate_limit',
@@ -287,21 +286,19 @@
             wrapped_call = self.wrap_sudo(call)
 
             extrinsic = substrate.create_signed_extrinsic( call = wrapped_call, keypair = self.sudo_keypair )
             response = substrate.submit_extrinsic( extrinsic, wait_for_inclusion = wait_for_inclusion, wait_for_finalization = wait_for_finalization )
 
             if not wait_for_finalization:
                 return True, None
-            
             response.process_events()
             if response.is_success:
                 return True, None
             else:
                 return False, response.error_message
-        
     def sudo_set_difficulty(self, netuid: int, difficulty: int, wait_for_inclusion: bool = True, wait_for_finalization: bool = True ) -> Tuple[bool, Optional[str]]:
         r""" Sets the difficulty of the mock chain using the sudo key.
         """
         with self.substrate as substrate:
             call = substrate.compose_call(
                     call_module='SubtensorModule',
                     call_function='sudo_set_difficulty',
@@ -314,21 +311,24 @@
             wrapped_call = self.wrap_sudo(call)
 
             extrinsic = substrate.create_signed_extrinsic( call = wrapped_call, keypair = self.sudo_keypair )
             response = substrate.submit_extrinsic( extrinsic, wait_for_inclusion = wait_for_inclusion, wait_for_finalization = wait_for_finalization )
 
             if not wait_for_finalization:
                 return True, None
+
+            if not wait_for_finalization:
+                return True, None
             
             response.process_events()
             if response.is_success:
                 return True, None
             else:
                 return False, response.error_message
-            
+
     def sudo_set_max_difficulty(self, netuid: int, max_difficulty: int, wait_for_inclusion: bool = True, wait_for_finalization: bool = True ) -> Tuple[bool, Optional[str]]:
         r""" Sets the max difficulty of the mock chain using the sudo key.
         """
         with self.substrate as substrate:
             call = substrate.compose_call(
                     call_module='SubtensorModule',
                     call_function='sudo_set_max_difficulty',
@@ -341,15 +341,15 @@
             wrapped_call = self.wrap_sudo(call)
 
             extrinsic = substrate.create_signed_extrinsic( call = wrapped_call, keypair = self.sudo_keypair )
             response = substrate.submit_extrinsic( extrinsic, wait_for_inclusion = wait_for_inclusion, wait_for_finalization = wait_for_finalization )
 
             if not wait_for_finalization:
                 return True, None
-            
+
             response.process_events()
             if response.is_success:
                 return True, None
             else:
                 return False, response.error_message
 
     def sudo_set_min_difficulty(self, netuid: int, min_difficulty: int, wait_for_inclusion: bool = True, wait_for_finalization: bool = True ) -> Tuple[bool, Optional[str]]:
@@ -368,15 +368,15 @@
             wrapped_call = self.wrap_sudo(call)
 
             extrinsic = substrate.create_signed_extrinsic( call = wrapped_call, keypair = self.sudo_keypair )
             response = substrate.submit_extrinsic( extrinsic, wait_for_inclusion = wait_for_inclusion, wait_for_finalization = wait_for_finalization )
 
             if not wait_for_finalization:
                 return True, None
-            
+
             response.process_events()
             if response.is_success:
                 return True, None
             else:
                 return False, response.error_message
 
     def sudo_add_network(self, netuid: int, tempo: int = 0, modality: int = 0, wait_for_inclusion: bool = True, wait_for_finalization: bool = True ) -> Tuple[bool, Optional[str]]:
@@ -396,21 +396,23 @@
             wrapped_call = self.wrap_sudo(call)
 
             extrinsic = substrate.create_signed_extrinsic( call = wrapped_call, keypair = self.sudo_keypair )
             response = substrate.submit_extrinsic( extrinsic, wait_for_inclusion = wait_for_inclusion, wait_for_finalization = wait_for_finalization )
 
             if not wait_for_finalization:
                 return True, None
+
+            if not wait_for_finalization:
+                return True, None
             
             response.process_events()
             if response.is_success:
                 return True, None
             else:
                 return False, response.error_message
-            
     def sudo_register(self, netuid: int, hotkey: str, coldkey: str, stake: int = 0, balance: int = 0, wait_for_inclusion: bool = True, wait_for_finalization: bool = True ) -> Tuple[bool, Optional[str]]:
         r""" Registers a neuron to the subnet using sudo.
         """
         with self.substrate as substrate:
             call = substrate.compose_call(
                     call_module='SubtensorModule',
                     call_function='sudo_register',
@@ -426,13 +428,16 @@
             wrapped_call = self.wrap_sudo(call)
 
             extrinsic = substrate.create_signed_extrinsic( call = wrapped_call, keypair = self.sudo_keypair )
             response = substrate.submit_extrinsic( extrinsic, wait_for_inclusion = wait_for_inclusion, wait_for_finalization = wait_for_finalization )
 
             if not wait_for_finalization:
                 return True, None
+
+            if not wait_for_finalization:
+                return True, None
             
             response.process_events()
             if response.is_success:
                 return True, None
             else:
                 return False, response.error_message
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_synapse/synapse.py` & `bittensor-5.0.0/bittensor/_synapse/synapse.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,106 +24,106 @@
 from typing import Union, Optional, Callable, List, Dict, Tuple
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 
 @dataclass
 class SynapseCall( ABC ):
     """ Base class for all synapse calls."""
-    
+
     is_forward: bool # If it is an forward of backward
     name: str # The name of the call.
 
     def __init__(
         self,
         synapse: 'bittensor.Synapse',
         request_proto: object
     ):
         self.completed = False
         self.start_time = time.time()
         self.timeout = request_proto.timeout
         self.src_version = request_proto.version
         self.src_hotkey = request_proto.hotkey
         self.dest_hotkey = synapse.axon.wallet.hotkey.ss58_address
-        self.dest_version = bittensor.__version_as_int__ 
+        self.dest_version = bittensor.__version_as_int__
         self.return_code: bittensor.proto.ReturnCode = bittensor.proto.ReturnCode.Success
         self.return_message: str = 'Success'
         self.priority: float = 0
 
     def __repr__(self) -> str:
         return f"SynapseCall( from: {self.src_hotkey}, forward: {self.is_forward}, start: {self.start_time}, timeout: {self.timeout}, priority: {self.priority}, completed: {self.completed})"
-    
+
     def __str__(self) -> str: return self.__repr__()
 
     @abstractmethod
-    def get_inputs_shape( self ) -> torch.Size: ...    
+    def get_inputs_shape( self ) -> torch.Size: ...
 
     @abstractmethod
-    def get_outputs_shape( self ) -> torch.Size: ...     
+    def get_outputs_shape( self ) -> torch.Size: ...
 
     @abstractmethod
     def get_response_proto( self ) -> object: ...
 
     def _get_response_proto( self ) -> object:
         proto = self.get_response_proto()
         proto.return_code = self.return_code
         proto.return_message = self.return_message
         return proto
 
     @abstractmethod
     def apply( self ): ...
 
-    def _apply( self ): 
+    def _apply( self ):
         # TODO(const): measure apply time.
         self.apply()
 
     def end(self):
         self.end_time = time.time()
         self.elapsed = self.end_time - self.start_time
         self.completed = True
 
     def log_outbound( self ):
         bittensor.logging.rpc_log(
-            axon = True, 
-            forward = self.is_forward, 
-            is_response = False, 
-            code = self.return_code, 
-            call_time = 0, 
-            pubkey = self.src_hotkey, 
+            axon = True,
+            forward = self.is_forward,
+            is_response = False,
+            code = self.return_code,
+            call_time = 0,
+            pubkey = self.src_hotkey,
             uid = None,
-            inputs = self.get_outputs_shape(), 
+            inputs = self.get_outputs_shape(),
             outputs = self.get_outputs_shape(),
             message = self.return_message,
             synapse = self.name,
         )
 
     def log_inbound( self ):
-        bittensor.logging.rpc_log( 
-            axon = True, 
-            forward = self.is_forward, 
-            is_response = True, 
-            code = self.return_code, 
-            call_time = self.elapsed if self.completed else 0, 
-            pubkey = self.src_hotkey, 
-            uid = None, 
+        bittensor.logging.rpc_log(
+            axon = True,
+            forward = self.is_forward,
+            is_response = True,
+            code = self.return_code,
+            call_time = self.elapsed if self.completed else 0,
+            pubkey = self.src_hotkey,
+            uid = None,
             inputs = self.get_inputs_shape(),
             outputs = self.get_inputs_shape(),
             message = self.return_message,
             synapse = self.name
-        )      
+        )
 
 class Synapse( ABC ):
     name: str
 
     def __init__( self, axon: bittensor.axon ):
         self.axon = axon
 
     @abstractmethod
     def blacklist( self, call: SynapseCall ) -> Union[ Tuple[bool, str], bool ]: ...
 
-    def _blacklist( self, call: SynapseCall ) -> Union[ bool, str ]: 
+    def _blacklist( self, call: SynapseCall ) -> Union[ bool, str ]:
         blacklist = self.blacklist( call )
         if isinstance( blacklist, tuple ): return blacklist
         elif isinstance( blacklist, bool ): return blacklist, "no reason specified"
         else:
             raise ValueError('Blacklist response had type {} expected one of bool or Tuple[bool, str]'.format( blacklist ))
 
     @abstractmethod
@@ -136,15 +136,15 @@
 
             # Check blacklist.
             blacklist, reason = self._blacklist( call )
             if blacklist:
                 call.return_code = bittensor.proto.ReturnCode.Blacklisted
                 call.return_message = reason
                 bittensor.logging.info( 'Synapse: {} blacklisted call: {} reason: {}'.format( self.name, call, reason) )
-            
+
             # Make call.
             else:
                 # Queue the forward call with priority.
                 call.priority = self.priority( call )
                 future = self.axon.priority_threadpool.submit(
                     call._apply,
                     priority = call.priority,
@@ -167,9 +167,8 @@
 
         # Finally return the call.
         finally:
             bittensor.logging.trace( 'Synapse: {} finalize call {}'.format( self.name, call ) )
             call.end()
             call.log_outbound()
             return call._get_response_proto()
-        
-   
+
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_synapse/text_prompting/miner.py` & `bittensor-5.0.0/bittensor/_synapse/text_prompting/miner.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,35 +44,35 @@
     def blacklist( self, forward_call: "bittensor.TextPromptingForwardCall" ) -> Union[ Tuple[bool, str], bool ]:
         # Check for registration
         def registration_check():
             is_registered = forward_call.src_hotkey in self.metagraph.hotkeys
             if not is_registered:
                 if self.config.neuron.blacklist.allow_non_registered: return False, 'passed blacklist'
                 else: return True, 'pubkey not registered'
-        
+
         # Blacklist based on stake.
         def stake_check() -> bool:
             default_stake = self.config.neuron.blacklist.default_stake
             if default_stake <= 0.0:
                 return False, 'passed blacklist'
             uid = self.metagraph.hotkeys.index(forward_call.src_hotkey)
-            if self.metagraph.S[uid].item() < default_stake: 
+            if self.metagraph.S[uid].item() < default_stake:
                 bittensor.logging.debug( "Blacklisted. Stake too low.")
                 return True, 'Stake too low.'
             else: return False, 'passed blacklist'
 
         # Optionally blacklist based on checks.
         try:
             registration_check()
             stake_check()
             return False, 'passed blacklist'
         except Exception as e:
             bittensor.logging.warning( "Blacklisted. Error in `registration_check` or `stake_check()" )
             return True, 'Error in `registration_check` or `stake_check()'
-        
+
     @abstractmethod
     def forward( self, messages: List[Dict[str, str]] ) -> str:
         ...
 
     @classmethod
     @abstractmethod
     def check_config( cls, config: 'bittensor.Config' ):
@@ -106,54 +106,54 @@
         if not os.path.exists( config.neuron.full_path ):
             os.makedirs( config.neuron.full_path )
 
     @classmethod
     def add_super_args( cls, parser: argparse.ArgumentParser ):
         cls.add_args(parser)
         parser.add_argument(
-            '--netuid', 
-            type = int, 
-            help = 'Subnet netuid', 
+            '--netuid',
+            type = int,
+            help = 'Subnet netuid',
             default = 41
         )
         parser.add_argument(
-            '--neuron.name', 
+            '--neuron.name',
             type = str,
             help = 'Trials for this miner go in miner.root / (wallet_cold - wallet_hot) / miner.name ',
             default = 'openai_prompting_miner'
         )
         parser.add_argument(
-            '--neuron.blocks_per_epoch', 
-            type = str, 
+            '--neuron.blocks_per_epoch',
+            type = str,
             help = 'Blocks until the miner sets weights on chain',
             default = 100
         )
         parser.add_argument(
-            '--neuron.no_set_weights', 
-            action = 'store_true', 
+            '--neuron.no_set_weights',
+            action = 'store_true',
             help = 'If True, the model does not set weights.',
             default = False
         )
         parser.add_argument(
-            '--neuron.max_batch_size', 
-            type = int, 
+            '--neuron.max_batch_size',
+            type = int,
             help = 'The maximum batch size for forward requests.',
             default = -1
         )
         parser.add_argument(
-            '--neuron.max_sequence_len', 
-            type = int, 
+            '--neuron.max_sequence_len',
+            type = int,
             help = 'The maximum sequence length for forward requests.',
             default = -1
         )
         parser.add_argument(
-            '--neuron.blacklist.hotkeys', 
-            type = str, 
-            required = False, 
-            nargs = '*', 
+            '--neuron.blacklist.hotkeys',
+            type = str,
+            required = False,
+            nargs = '*',
             action = 'store',
             help = 'To blacklist certain hotkeys', default=[]
         )
         parser.add_argument(
             '--neuron.blacklist.allow_non_registered',
             action = 'store_true',
             help = 'If True, the miner will allow non-registered hotkeys to mine.',
@@ -184,15 +184,15 @@
         self.config = copy.deepcopy( config )
         self.super_check_config( self.config )
         self.config.to_defaults()
         bittensor.logging( config = self.config, logging_dir = self.config.neuron.full_path )
         self.subtensor = bittensor.subtensor( self.config )
         self.wallet = bittensor.wallet( self.config )
         self.metagraph = self.subtensor.metagraph( self.config.netuid )
-        self.axon = bittensor.axon( 
+        self.axon = bittensor.axon(
             wallet = self.wallet,
             metagraph = self.metagraph,
             config = self.config,
         )
         class Synapse( bittensor.TextPromptingSynapse ):
             def priority( _, forward_call: "bittensor.TextPromptingForwardCall" ) -> float:
                 return self.priority( forward_call )
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_synapse/text_prompting/synapse.py` & `bittensor-5.0.0/bittensor/_synapse/text_prompting/synapse.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,105 +25,105 @@
 
 
 class SynapseForwardMulti( bittensor.SynapseCall ):
     name: str = "text_prompting_forward_multi"
     is_forward: bool = True
     multi_completions: List[ str ] = [""]
 
-    def __init__( 
-            self, 
-            synapse: "TextPromptingSynapseMulti", 
+    def __init__(
+            self,
+            synapse: "TextPromptingSynapseMulti",
             request_proto: bittensor.proto.MultiForwardTextPromptingRequest,
             multi_forward_callback: Callable,
         ):
         super().__init__( synapse = synapse, request_proto = request_proto )
         self.messages: List[ Dict[str, str] ] = request_proto.messages
         self.formatted_messages = [ json.loads(message) for message in self.messages ]
         self.multi_forward_callback = multi_forward_callback
 
     def apply( self ):
         bittensor.logging.trace( "SynapseForward.apply()" )
         self.multi_completions = self.multi_forward_callback( messages = self.formatted_messages )
         bittensor.logging.trace( "SynapseForward.apply() = ", self.multi_completions )
 
-    def get_response_proto( self ) -> bittensor.proto.MultiForwardTextPromptingResponse: 
+    def get_response_proto( self ) -> bittensor.proto.MultiForwardTextPromptingResponse:
         bittensor.logging.trace( "SynapseForward.get_response_proto()")
         return bittensor.MultiForwardTextPromptingResponse( multi_completions = self.multi_completions )
-            
-    def get_inputs_shape(self) -> Union[torch.Size, None]: 
+
+    def get_inputs_shape(self) -> Union[torch.Size, None]:
         bittensor.logging.trace( "SynapseForward.get_inputs_shape()" )
         return torch.Size( [ len(message) for message in self.messages ] )
-    
-    def get_outputs_shape(self) -> Union[torch.Size, None]: 
+
+    def get_outputs_shape(self) -> Union[torch.Size, None]:
         bittensor.logging.trace( "SynapseForward.get_outputs_shape()" )
         return torch.Size( [ len(self.multi_completions) ]  )
 
 class SynapseForward( bittensor.SynapseCall ):
     name: str = "text_prompting_forward"
     is_forward: bool = True
     completion: str = ""
 
-    def __init__( 
-            self, 
-            synapse: "TextPromptingSynapse", 
+    def __init__(
+            self,
+            synapse: "TextPromptingSynapse",
             request_proto: bittensor.proto.ForwardTextPromptingRequest,
             forward_callback: Callable,
         ):
         super().__init__( synapse = synapse, request_proto = request_proto )
         self.messages = request_proto.messages
         self.formatted_messages = [ json.loads(message) for message in self.messages ]
         self.forward_callback = forward_callback
 
     def apply( self ):
         bittensor.logging.trace( "SynapseForward.apply()" )
         self.completion = self.forward_callback( messages = self.formatted_messages )
         bittensor.logging.trace( "SynapseForward.apply() = ", self.completion )
 
-    def get_response_proto( self ) -> bittensor.proto.ForwardTextPromptingResponse: 
+    def get_response_proto( self ) -> bittensor.proto.ForwardTextPromptingResponse:
         bittensor.logging.trace( "SynapseForward.get_response_proto()" )
         return bittensor.ForwardTextPromptingResponse( response = self.completion )
-    
-    def get_inputs_shape(self) -> Union[torch.Size, None]: 
+
+    def get_inputs_shape(self) -> Union[torch.Size, None]:
         bittensor.logging.trace( "SynapseForward.get_inputs_shape()" )
         return torch.Size( [ len(message) for message in self.messages ] )
-    
-    def get_outputs_shape(self) -> Union[torch.Size, None]: 
+
+    def get_outputs_shape(self) -> Union[torch.Size, None]:
         bittensor.logging.trace( "SynapseForward.get_outputs_shape()" )
         return torch.Size( [ len(self.completion) ]  )
-    
+
 class SynapseBackward( bittensor.SynapseCall ):
     name: str = "text_prompting_backward"
     is_forward: bool = False
 
-    def __init__( 
-            self, 
-            synapse: "TextPromptingSynapse", 
+    def __init__(
+            self,
+            synapse: "TextPromptingSynapse",
             request_proto: bittensor.proto.BackwardTextPromptingRequest,
             backward_callback: Callable,
         ):
         super().__init__( synapse = synapse, request_proto = request_proto )
         self.formatted_messages = [ message for message in request_proto.messages ]
         self.formatted_rewards = torch.tensor( [ request_proto.rewards ], dtype = torch.float32 )
         self.completion = request_proto.response
         self.backward_callback = backward_callback
 
     def apply( self ):
         self.backward_callback(
             rewards = self.formatted_rewards,
             messages = self.formatted_messages,
             response = self.completion,
-        )    
-    
-    def get_response_proto( self ) -> bittensor.proto.BackwardTextPromptingResponse: 
+        )
+
+    def get_response_proto( self ) -> bittensor.proto.BackwardTextPromptingResponse:
         return bittensor.BackwardTextPromptingResponse( )
 
-    def get_inputs_shape(self) -> torch.Size: 
+    def get_inputs_shape(self) -> torch.Size:
         return torch.Size( [ len(message) for message in self.formatted_messages ] )
-    
-    def get_outputs_shape(self) -> torch.Size: 
+
+    def get_outputs_shape(self) -> torch.Size:
         return torch.Size( [ 0 ] )
 
 
 class TextPromptingSynapse( bittensor.Synapse, bittensor.grpc.TextPromptingServicer ):
     name: str = "text_prompting_synapse"
 
     def __init__(self, axon: "bittensor.axon" ):
@@ -138,19 +138,19 @@
 
     @abstractmethod
     def backward( self, messages: List[Dict[str, str]], response: str, rewards: torch.FloatTensor ) -> str: ...
 
     def Forward( self, request: bittensor.proto.ForwardTextPromptingRequest, context: grpc.ServicerContext ) -> bittensor.proto.ForwardTextPromptingResponse:
         call = SynapseForward( self, request, self.forward )
         bittensor.logging.trace( 'Forward: {} '.format( call ) )
-        return self.apply( call = call ) 
+        return self.apply( call = call )
 
     def MultiForward( self, request: bittensor.proto.MultiForwardTextPromptingRequest, context: grpc.ServicerContext ) -> bittensor.proto.MultiForwardTextPromptingResponse:
         call = SynapseForwardMulti( self, request, self.multi_forward )
         bittensor.logging.trace( 'MultiForward: {} '.format( call ) )
-        return self.apply( call = call ) 
-                         
+        return self.apply( call = call )
+
     def Backward( self, request: bittensor.proto.BackwardTextPromptingRequest, context: grpc.ServicerContext ) -> bittensor.proto.BackwardTextPromptingResponse:
         call = SynapseBackward( self, request, self.backward )
         bittensor.logging.trace( 'Backward: {}'.format( call ) )
-        return self.apply( call = call ) 
+        return self.apply( call = call )
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_threadpool/__init__.py` & `bittensor-5.0.0/bittensor/_threadpool/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """ Factory method for creating priority threadpool
 """
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import os
 import argparse
 import copy
 import bittensor
 from . import priority_thread_pool_impl
@@ -30,22 +30,22 @@
             cls,
             config: 'bittensor.config' = None,
             max_workers: int = None,
             maxsize: int = None,
         ):
         r""" Initializes a priority thread pool.
             Args:
-                config (:obj:`bittensor.Config`, `optional`): 
+                config (:obj:`bittensor.Config`, `optional`):
                     bittensor.subtensor.config()
                 max_workers (default=10, type=int)
 .                   The maximum number of threads in thread pool
                 maxsize (default=-1, type=int)
                     The maximum number of tasks in the priority queue
-        """        
-        if config == None: 
+        """
+        if config == None:
             config = prioritythreadpool.config()
         config = copy.deepcopy( config )
         config.priority.max_workers = max_workers if max_workers != None else config.priority.max_workers
         config.priority.maxsize = maxsize if maxsize != None else config.priority.maxsize
 
         prioritythreadpool.check_config( config )
         return priority_thread_pool_impl.PriorityThreadPoolExecutor(maxsize = config.priority.maxsize, max_workers = config.priority.max_workers)
@@ -53,45 +53,45 @@
     @classmethod
     def add_args(cls, parser: argparse.ArgumentParser, prefix: str = None ):
         """ Accept specific arguments from parser
         """
         prefix_str = '' if prefix == None else prefix + '.'
         try:
             parser.add_argument('--' + prefix_str + 'priority.max_workers', type = int, help='''maximum number of threads in thread pool''', default = bittensor.defaults.priority.max_workers)
-            parser.add_argument('--' + prefix_str + 'priority.maxsize', type=int, help='''maximum size of tasks in priority queue''', default = bittensor.defaults.priority.maxsize)  
+            parser.add_argument('--' + prefix_str + 'priority.maxsize', type=int, help='''maximum size of tasks in priority queue''', default = bittensor.defaults.priority.maxsize)
         except argparse.ArgumentError:
             # re-parsing arguments.
             pass
 
-    @classmethod   
+    @classmethod
     def help(cls):
         """ Print help to stdout
         """
         parser = argparse.ArgumentParser()
         cls.add_args( parser )
         print (cls.__new__.__doc__)
         parser.print_help()
 
-    @classmethod   
+    @classmethod
     def add_defaults(cls, defaults):
         """ Adds parser defaults to object from enviroment variables.
         """
         defaults.priority = bittensor.Config()
         defaults.priority = bittensor.Config()
         defaults.priority.max_workers = os.getenv('BT_PRIORITY_MAX_WORKERS') if os.getenv('BT_PRIORITY_MAX_WORKERS') != None else 5
         defaults.priority.maxsize = os.getenv('BT_PRIORITY_MAXSIZE') if os.getenv('BT_PRIORITY_MAXSIZE') != None else 10
-    
-    @classmethod   
+
+    @classmethod
     def config(cls) -> 'bittensor.Config':
         """ Get config from the argument parser
-            Return: bittensor.config object 
+            Return: bittensor.config object
         """
         parser = argparse.ArgumentParser()
         prioritythreadpool.add_args( parser )
         return bittensor.config( parser )
-    
-    @classmethod   
+
+    @classmethod
     def check_config(cls, config: 'bittensor.Config' ):
         """ Check config for threadpool worker number and size
         """
         assert isinstance(config.priority.max_workers, int), 'priority.max_workers must be a int'
         assert isinstance(config.priority.maxsize, int), 'priority.maxsize must be a int'
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_threadpool/priority_thread_pool_impl.py` & `bittensor-5.0.0/bittensor/_threadpool/priority_thread_pool_impl.py`

 * *Files 8% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             if priority == sys.maxsize:
                 del item
             elif item is not None:
                 item.run()
                 # Delete references to object. See issue16284
                 del item
                 continue
-                
+
             executor = executor_reference()
             # Exit if:
             #   - The interpreter is shutting down OR
             #   - The executor that owns the worker has been collected OR
             #   - The executor that owns the worker has been shutdown.
             if _shutdown or executor is None or executor._shutdown:
                 # Flag the executor as shutting down as early as possible if it
@@ -107,15 +107,15 @@
 class BrokenThreadPool(_base.BrokenExecutor):
     """
     Raised when a worker thread in a ThreadPoolExecutor failed initializing.
     """
 
 
 class PriorityThreadPoolExecutor(_base.Executor):
-    """ Base threadpool executor with a priority queue 
+    """ Base threadpool executor with a priority queue
     """
     # Used to assign unique thread names when thread_name_prefix is not supplied.
     _counter = itertools.count().__next__
 
     def __init__(self, maxsize = -1, max_workers=None, thread_name_prefix='',
                  initializer=None, initargs=()):
         """Initializes a new ThreadPoolExecutor instance.
@@ -166,15 +166,15 @@
             priority = kwargs.get('priority', random.randint(0, 1000000))
             if priority == 0:
                 priority = random.randint(1, 100)
             eplison = random.uniform(0,0.01) * priority
             start_time = time.time()
             if 'priority' in kwargs:
                 del kwargs['priority']
-            
+
 
             f = _base.Future()
             w = _WorkItem(f, fn, start_time, args, kwargs)
             self._work_queue.put((-float(priority + eplison), w), block=False)
             self._adjust_thread_count()
             return f
     submit.__doc__ = _base.Executor.submit.__doc__
@@ -217,15 +217,15 @@
                 if work_item is not None:
                     work_item.future.set_exception(BrokenThreadPool(self._broken))
 
     def shutdown(self, wait=True):
         with self._shutdown_lock:
             self._shutdown = True
             self._work_queue.put(NULL_ENTRY)
-        
+
         if wait:
             for t in self._threads:
                 try:
                     t.join(timeout=2)
                 except Exception:
                     pass
     shutdown.__doc__ = _base.Executor.shutdown.__doc__
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_tokenizer/__init__.py` & `bittensor-5.0.0/bittensor/_tokenizer/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """ Implementation of the bittensor tokenizer
 """
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 from transformers import AutoTokenizer
 import bittensor
 from bittensor.utils.tokenizer_utils import prep_tokenizer
 
 
@@ -32,15 +32,15 @@
             version = bittensor.__version__
         if version not in cls.cached_tokenizer_for_version:
             _tokenizer = cls.get_tokenizer_for_version( version )
             cls.cached_tokenizer_for_version[ version ] = _tokenizer
         else:
             _tokenizer = cls.cached_tokenizer_for_version[ version ]
         return _tokenizer
-        
+
     # Tokenizer
     # NOTE (const): tokenizers are guaranteed to improve and expand as time progresses. We version the tokenizer here.
     # neurons must be aware that versions will increase and be ready to convert between tokenizers.
     # TODO (const): Add functionality to allow tokenizer conversion. i.e. for input token conversion.
     @classmethod
     def get_tokenizer_for_version( cls, version = bittensor.__version__ ):
         """ Return the GPT2 tokenizer with bittersor's special tokens
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_wallet/__init__.py` & `bittensor-5.0.0/bittensor/_wallet/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import argparse
 import copy
 from distutils.util import strtobool
 import os
 
@@ -28,83 +28,76 @@
     """ Create and init wallet that stores hot and coldkey
     """
     @classmethod
     def mock(cls) -> 'bittensor.Wallet':
         return wallet( name='mock' )
 
     def __new__(
-            cls, 
+            cls,
             config: 'bittensor.Config' = None,
             name: str = None,
             hotkey: str = None,
             path: str = None,
             _mock: bool = None
         ) -> 'bittensor.Wallet':
         r""" Init bittensor wallet object containing a hot and coldkey.
 
             Args:
-                config (:obj:`bittensor.Config`, `optional`): 
+                config (:obj:`bittensor.Config`, `optional`):
                     bittensor.wallet.config()
                 name (required=False, default='default'):
                     The name of the wallet to unlock for running bittensor
                 hotkey (required=False, default='default'):
                     The name of hotkey used to running the miner.
                 path (required=False, default='~/.bittensor/wallets/'):
                     The path to your bittensor wallets
                 _mock (required=False, default=False):
                     If true creates a mock wallet with random keys.
         """
-        if config == None: 
+        if config == None:
             config = wallet.config()
         config = copy.deepcopy( config )
         config.wallet.name = name if name != None else config.wallet.name
         config.wallet.hotkey = hotkey if hotkey != None else config.wallet.hotkey
         config.wallet.path = path if path != None else config.wallet.path
         config.wallet._mock = _mock if _mock != None else config.wallet._mock
         wallet.check_config( config )
         # Allows mocking from the command line.
         if config.wallet.get('name', bittensor.defaults.wallet.name) == 'mock' or config.wallet._mock:
             config.wallet._mock = True
             _mock = True
 
             return wallet_mock.Wallet_mock(
-                name = config.wallet.get('name', bittensor.defaults.wallet.name), 
-                hotkey = config.wallet.get('hotkey', bittensor.defaults.wallet.hotkey), 
+                name = config.wallet.get('name', bittensor.defaults.wallet.name),
+                hotkey = config.wallet.get('hotkey', bittensor.defaults.wallet.hotkey),
                 path = config.wallet.path,
                 _mock = True,
                 config = config
             )
 
         network = config.get('subtensor.network', bittensor.defaults.subtensor.network)
-        if network == 'nakamoto':
-            return naka_wallet(
-                name = config.wallet.get('name', bittensor.defaults.wallet.name), 
-                hotkey = config.wallet.get('hotkey', bittensor.defaults.wallet.hotkey), 
-                path = config.wallet.path,
-                config = config
-            )
-        else:
-            # Default to finney.
-            return wallet_impl.Wallet(
-                name = config.wallet.get('name', bittensor.defaults.wallet.name), 
-                hotkey = config.wallet.get('hotkey', bittensor.defaults.wallet.hotkey), 
-                path = config.wallet.path,
-                config = config
-            )
 
-    @classmethod   
+        # Default to finney.
+        return wallet_impl.Wallet(
+            name = config.wallet.get('name', bittensor.defaults.wallet.name),
+            hotkey = config.wallet.get('hotkey', bittensor.defaults.wallet.hotkey),
+            path = config.wallet.path,
+            config = config
+        )
+
+    @classmethod
     def config(cls) -> 'bittensor.Config':
         """ Get config from the argument parser
         Return: bittensor.config object
         """
         parser = argparse.ArgumentParser()
         wallet.add_args( parser )
         return bittensor.config( parser )
 
-    @classmethod   
+    @classmethod
     def help(cls):
         """ Print help to stdout
         """
         parser = argparse.ArgumentParser()
         cls.add_args( parser )
         print (cls.__new__.__doc__)
         parser.print_help()
@@ -115,33 +108,33 @@
         """
         prefix_str = '' if prefix == None else prefix + '.'
         try:
             parser.add_argument('--' + prefix_str + 'wallet.name', required=False, default=bittensor.defaults.wallet.name, help='''The name of the wallet to unlock for running bittensor (name mock is reserved for mocking this wallet)''')
             parser.add_argument('--' + prefix_str + 'wallet.hotkey', required=False, default=bittensor.defaults.wallet.hotkey, help='''The name of wallet's hotkey.''')
             parser.add_argument('--' + prefix_str + 'wallet.path', required=False, default=bittensor.defaults.wallet.path, help='''The path to your bittensor wallets''')
             parser.add_argument('--' + prefix_str + 'wallet._mock', action='store_true', default=bittensor.defaults.wallet._mock, help='To turn on wallet mocking for testing purposes.')
-        
+
             parser.add_argument('--' + prefix_str + 'wallet.reregister', required=False, action='store', default=bittensor.defaults.wallet.reregister, type=strtobool, help='''Whether to reregister the wallet if it is not already registered.''')
 
         except argparse.ArgumentError as e:
             pass
 
-    @classmethod   
+    @classmethod
     def add_defaults(cls, defaults):
         """ Adds parser defaults to object from enviroment variables.
         """
         defaults.wallet = bittensor.Config()
         defaults.wallet.name = os.getenv('BT_WALLET_NAME') if os.getenv('BT_WALLET_NAME') != None else 'default'
         defaults.wallet.hotkey = os.getenv('BT_WALLET_HOTKEY') if os.getenv('BT_WALLET_HOTKEY') != None else 'default'
         defaults.wallet.path = os.getenv('BT_WALLET_PATH') if os.getenv('BT_WALLET_PATH') != None else '~/.bittensor/wallets/'
         defaults.wallet._mock = os.getenv('BT_WALLET_MOCK') if os.getenv('BT_WALLET_MOCK') != None else False
         # Defaults for registration
         defaults.wallet.reregister = True
 
-    @classmethod   
+    @classmethod
     def check_config(cls, config: 'bittensor.Config' ):
         """ Check config for wallet name/hotkey/path/hotkeys/sort_by
         """
         assert 'wallet' in config
         assert isinstance(config.wallet.get('name', bittensor.defaults.wallet.name), str)
         assert isinstance(config.wallet.get('hotkey', bittensor.defaults.wallet.hotkey), str ) or config.wallet.get('hotkey', bittensor.defaults.wallet.hotkey) == None
         assert isinstance(config.wallet.path, str)
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_wallet/wallet_impl.py` & `bittensor-5.0.0/bittensor/_wallet/wallet_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """ Implementation of the wallet class, which manages balances with staking and transfer. Also manages hotkey and coldkey.
 """
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import os
 import sys
 from types import SimpleNamespace
 from typing import Optional, Union, List, Tuple, Dict, overload
 
@@ -39,49 +39,49 @@
     print ("The mnemonic to the new {} is:\n\n{}\n".format(key_type, mnemonic_green))
     print ("You can use the mnemonic to recreate the key in case it gets lost. The command to use to regenerate the key using this mnemonic is:")
     print("btcli regen_{} --mnemonic {}".format(key_type, mnemonic))
     print('')
 
 class Wallet():
     """
-    Bittensor wallet maintenance class. Each wallet contains a coldkey and a hotkey. 
+    Bittensor wallet maintenance class. Each wallet contains a coldkey and a hotkey.
     The coldkey is the user's primary key for holding stake in their wallet
     and is the only way that users can access Tao. Coldkeys can hold tokens and should be encrypted on your device.
     The coldkey must be used to stake and unstake funds from a running node. The hotkey, on the other hand, is only used
-    for suscribing and setting weights from running code. Hotkeys are linked to coldkeys through the metagraph. 
+    for suscribing and setting weights from running code. Hotkeys are linked to coldkeys through the metagraph.
     """
-    def __init__( 
+    def __init__(
         self,
         name:str,
         path:str,
         hotkey:str,
         config: 'bittensor.Config' = None,
     ):
         r""" Init bittensor wallet object containing a hot and coldkey.
             Args:
                 name (required=True, default='default):
                     The name of the wallet to unlock for running bittensor
                 hotkey (required=True, default='default):
                     The name of hotkey used to running the miner.
                 path (required=True, default='~/.bittensor/wallets/'):
                     The path to your bittensor wallets
-                config (:obj:`bittensor.Config`, `optional`): 
+                config (:obj:`bittensor.Config`, `optional`):
                     bittensor.wallet.config()
         """
         self.name = name
         self.path = path
         self.hotkey_str = hotkey
         self._hotkey = None
         self._coldkey = None
         self._coldkeypub = None
         self.config = config
 
     def __str__(self):
         return "Wallet ({}, {}, {})".format(self.name, self.hotkey_str, self.path)
-    
+
     def __repr__(self):
         return self.__str__()
 
     def neuron(self, netuid: int) -> Optional['bittensor.NeuronInfo']:
         return self.get_neuron(netuid=netuid)
 
     def trust(self, netuid: int) -> Optional[float]:
@@ -165,38 +165,35 @@
                     The network uid to check for registration.
                     Default is None, which checks any subnetwork.
             Return:
                 is_registered (bool):
                     Is the wallet registered on the chain.
         """
         if subtensor == None: subtensor = bittensor.subtensor(self.config)
-        if subtensor.network == 'nakamoto':
-            neuron = subtensor.neuron_for_pubkey( ss58_hotkey = self.hotkey.ss58_address )
-            return not neuron.is_null
+
+        # default to finney
+        if netuid == None:
+            return subtensor.is_hotkey_registered_any( self.hotkey.ss58_address )
         else:
-            # default to finney
-            if netuid == None:
-                return subtensor.is_hotkey_registered_any( self.hotkey.ss58_address )
-            else:
-                return subtensor.is_hotkey_registered_on_subnet( self.hotkey.ss58_address, netuid = netuid )
-        
+            return subtensor.is_hotkey_registered_on_subnet( self.hotkey.ss58_address, netuid = netuid )
+
 
     def get_neuron ( self, netuid: int, subtensor: Optional['bittensor.Subtensor'] = None ) -> Optional['bittensor.NeuronInfo'] :
         """ Returns this wallet's neuron information from subtensor.
             Args:
                 netuid (int):
                     The network uid of the subnet to query.
                 subtensor( Optional['bittensor.Subtensor'] ):
                     Bittensor subtensor connection. Overrides with defaults if None.
             Return:
                 neuron (Union[ NeuronInfo, None ]):
                     neuron account on the chain or None if you are not registered.
         """
         if subtensor == None: subtensor = bittensor.subtensor()
-        if not self.is_registered(netuid = netuid, subtensor=subtensor): 
+        if not self.is_registered(netuid = netuid, subtensor=subtensor):
             print(colored('This wallet is not registered. Call wallet.register() before this function.','red'))
             return None
         neuron = subtensor.neuron_for_wallet( self, netuid = netuid )
         return neuron
 
     def get_uid ( self, netuid: int, subtensor: Optional['bittensor.Subtensor'] = None ) -> int:
         """ Returns this wallet's hotkey uid or -1 if the hotkey is not subscribed.
@@ -206,15 +203,15 @@
                 subtensor( Optional['bittensor.Subtensor'] ):
                     Bittensor subtensor connection. Overrides with defaults if None.
             Return:
                 uid (int):
                     Network uid or -1 if you are not registered.
         """
         if subtensor == None: subtensor = bittensor.subtensor()
-        if not self.is_registered(netuid = netuid, subtensor=subtensor): 
+        if not self.is_registered(netuid = netuid, subtensor=subtensor):
             print(colored('This wallet is not registered. Call wallet.register() before this function.','red'))
             return -1
         neuron = self.get_neuron(netuid = netuid, subtensor = subtensor)
         if neuron.is_null:
             return -1
         else:
             return neuron.uid
@@ -229,15 +226,15 @@
                     Stake account balance.
         """
         if subtensor == None: subtensor = bittensor.subtensor()
         stake = subtensor.get_stake_for_coldkey_and_hotkey( hotkey_ss58 = self.hotkey.ss58_address, coldkey_ss58 = self.coldkeypub.ss58_address )
         if not stake: # Not registered.
             print(colored('This wallet is not registered. Call wallet.register() before this function.','red'))
             return bittensor.Balance(0)
-        
+
         return stake
 
     def get_balance( self, subtensor: Optional['bittensor.Subtensor'] = None ) -> 'bittensor.Balance':
         """ Returns this wallet's coldkey balance from passed subtensor connection.
             Args:
                 subtensor( Optional['bittensor.Subtensor'] ):
                     Bittensor subtensor connection. Overrides with defaults if None.
@@ -259,22 +256,22 @@
         """ Re-register this wallet on the chain.
             Args:
                 netuid (int):
                     The network uid of the subnet to register on.
                 subtensor( Optional['bittensor.Subtensor'] ):
                     Bittensor subtensor connection. Overrides with defaults if None.
                 wait_for_inclusion (bool):
-                    if set, waits for the extrinsic to enter a block before returning true, 
-                    or returns false if the extrinsic fails to enter the block within the timeout.   
+                    if set, waits for the extrinsic to enter a block before returning true,
+                    or returns false if the extrinsic fails to enter the block within the timeout.
                 wait_for_finalization (bool):
                     if set, waits for the extrinsic to be finalized on the chain before returning true,
                     or returns false if the extrinsic fails to be finalized within the timeout.
                 prompt (bool):
                     If true, the call waits for confirmation from the user before proceeding.
-                
+
             Return:
                 wallet (bittensor.Wallet):
                     This wallet.
         """
         if subtensor == None:
             subtensor = bittensor.subtensor()
         if not self.is_registered(netuid = netuid, subtensor=subtensor):
@@ -295,18 +292,18 @@
                 wait_for_finalization = wait_for_finalization,
                 output_in_place = self.config.subtensor.register.get('output_in_place', bittensor.defaults.subtensor.register.output_in_place),
                 log_verbose = self.config.subtensor.register.get('verbose', bittensor.defaults.subtensor.register.verbose),
             )
 
         return self
 
-    def register ( 
-            self, 
+    def register (
+            self,
             netuid: int,
-            subtensor: Optional['bittensor.Subtensor'] = None, 
+            subtensor: Optional['bittensor.Subtensor'] = None,
             wait_for_inclusion: bool = False,
             wait_for_finalization: bool = True,
             prompt: bool = False,
             max_allowed_attempts: int = 3,
             cuda: bool = False,
             dev_id: int = 0,
             TPB: int = 256,
@@ -318,16 +315,16 @@
         """ Registers the wallet to chain.
         Args:
             netuid (int):
                 The network uid of the subnet to register on.
             subtensor( Optional['bittensor.Subtensor'] ):
                 Bittensor subtensor connection. Overrides with defaults if None.
             wait_for_inclusion (bool):
-                If set, waits for the extrinsic to enter a block before returning true, 
-                or returns false if the extrinsic fails to enter the block within the timeout.   
+                If set, waits for the extrinsic to enter a block before returning true,
+                or returns false if the extrinsic fails to enter the block within the timeout.
             wait_for_finalization (bool):
                 If set, waits for the extrinsic to be finalized on the chain before returning true,
                 or returns false if the extrinsic fails to be finalized within the timeout.
             prompt (bool):
                 If true, the call waits for confirmation from the user before proceeding.
             max_allowed_attempts (int):
                 Maximum number of attempts to register the wallet.
@@ -343,15 +340,15 @@
                 The number of nonces to solve between updates.
             output_in_place (bool):
                 If true, the registration output is printed in-place.
             log_verbose (bool):
                 If true, the registration output is more verbose.
         Returns:
             success (bool):
-                flag is true if extrinsic was finalized or uncluded in the block. 
+                flag is true if extrinsic was finalized or uncluded in the block.
                 If we did not wait for finalization / inclusion, the response is true.
         """
         # Get chain connection.
         if subtensor == None: subtensor = bittensor.subtensor()
         subtensor.register(
             wallet = self,
             wait_for_inclusion = wait_for_inclusion,
@@ -362,107 +359,107 @@
             dev_id=dev_id,
             TPB=TPB,
             num_processes=num_processes,
             update_interval=update_interval,
             log_verbose=log_verbose,
             netuid = netuid,
         )
-        
+
         return self
 
-    def add_stake( self, 
-        amount: Union[float, bittensor.Balance] = None, 
+    def add_stake( self,
+        amount: Union[float, bittensor.Balance] = None,
         wait_for_inclusion: bool = False,
         wait_for_finalization: bool = True,
         subtensor: Optional['bittensor.Subtensor'] = None,
         prompt: bool = False
     ) -> bool:
         """ Stakes tokens from this wallet's coldkey onto it's hotkey.
             Args:
                 amount_tao (float):
                     amount of tao to stake or bittensor balance object. If None, stakes all available balance.
                 wait_for_inclusion (bool):
-                    if set, waits for the extrinsic to enter a block before returning true, 
-                    or returns false if the extrinsic fails to enter the block within the timeout.   
+                    if set, waits for the extrinsic to enter a block before returning true,
+                    or returns false if the extrinsic fails to enter the block within the timeout.
                 wait_for_finalization (bool):
                     if set, waits for the extrinsic to be finalized on the chain before returning true,
                     or returns false if the extrinsic fails to be finalized within the timeout.
                 subtensor( `bittensor.Subtensor` ):
                     Bittensor subtensor connection. Overrides with defaults if None.
                 prompt (bool):
                     If true, the call waits for confirmation from the user before proceeding.
             Returns:
                 success (bool):
-                    flag is true if extrinsic was finalized or uncluded in the block. 
+                    flag is true if extrinsic was finalized or uncluded in the block.
                     If we did not wait for finalization / inclusion, the response is true.
         """
         if subtensor == None: subtensor = bittensor.subtensor()
         return subtensor.add_stake( wallet = self, amount = amount, wait_for_inclusion = wait_for_inclusion, wait_for_finalization = wait_for_finalization, prompt=prompt )
 
-    def remove_stake( self, 
-        amount: Union[float, bittensor.Balance] = None, 
+    def remove_stake( self,
+        amount: Union[float, bittensor.Balance] = None,
         wait_for_inclusion: bool = False,
         wait_for_finalization: bool = True,
         subtensor: Optional['bittensor.Subtensor'] = None,
         prompt: bool = False,
     ) -> bool:
         """ Removes stake from this wallet's hotkey and moves them onto it's coldkey balance.
             Args:
                 amount_tao (float):
                     amount of tao to unstake or bittensor balance object. If None, unstakes all available hotkey balance.
                 wait_for_inclusion (bool):
-                    if set, waits for the extrinsic to enter a block before returning true, 
-                    or returns false if the extrinsic fails to enter the block within the timeout.   
+                    if set, waits for the extrinsic to enter a block before returning true,
+                    or returns false if the extrinsic fails to enter the block within the timeout.
                 wait_for_finalization (bool):
                     if set, waits for the extrinsic to be finalized on the chain before returning true,
                     or returns false if the extrinsic fails to be finalized within the timeout.
                 subtensor( `bittensor.Subtensor` ):
                     Bittensor subtensor connection. Overrides with defaults if None.
                 prompt (bool):
                     If true, the call waits for confirmation from the user before proceeding.
             Returns:
                 success (bool):
-                    flag is true if extrinsic was finalized or uncluded in the block. 
+                    flag is true if extrinsic was finalized or uncluded in the block.
                     If we did not wait for finalization / inclusion, the response is true.
         """
         if subtensor == None: subtensor = bittensor.subtensor()
         return subtensor.unstake( wallet = self, amount = amount, wait_for_inclusion = wait_for_inclusion, wait_for_finalization = wait_for_finalization, prompt=prompt )
 
-    def transfer( 
-        self, 
+    def transfer(
+        self,
         dest:str,
-        amount: Union[float, bittensor.Balance] , 
+        amount: Union[float, bittensor.Balance] ,
         wait_for_inclusion: bool = False,
         wait_for_finalization: bool = True,
         subtensor: Optional['bittensor.Subtensor'] = None,
         prompt: bool = False,
     ) -> bool:
         """ Transfers Tao from this wallet's coldkey to the destination address.
             Args:
                 dest (`type`:str, required):
-                    The destination address either encoded as a ss58 or ed255 public-key string of 
+                    The destination address either encoded as a ss58 or ed255 public-key string of
                     secondary account.
                 amount (float, required):
                     amount of tao to transfer or a bittensor balance object.
                 wait_for_inclusion (bool):
-                    if set, waits for the extrinsic to enter a block before returning true, 
-                    or returns false if the extrinsic fails to enter the block within the timeout.   
+                    if set, waits for the extrinsic to enter a block before returning true,
+                    or returns false if the extrinsic fails to enter the block within the timeout.
                 wait_for_finalization (bool):
                     if set, waits for the extrinsic to be finalized on the chain before returning true,
                     or returns false if the extrinsic fails to be finalized within the timeout.
                 subtensor( `bittensor.Subtensor` ):
                     Bittensor subtensor connection. Overrides with defaults if None.
                 prompt (bool):
                     If true, the call waits for confirmation from the user before proceeding.
             Returns:
                 success (bool):
-                    flag is true if extrinsic was finalized or uncluded in the block. 
+                    flag is true if extrinsic was finalized or uncluded in the block.
                     If we did not wait for finalization / inclusion, the response is true.
         """
-        if subtensor == None: subtensor = bittensor.subtensor() 
+        if subtensor == None: subtensor = bittensor.subtensor()
         return subtensor.transfer( wallet = self, dest = dest, amount = amount, wait_for_inclusion = wait_for_inclusion, wait_for_finalization = wait_for_finalization, prompt=prompt )
 
     def create_if_non_existent( self, coldkey_use_password:bool = True, hotkey_use_password:bool = False) -> 'Wallet':
         """ Checks for existing coldkeypub and hotkeys and creates them if non-existent.
         """
         return self.create(coldkey_use_password, hotkey_use_password)
 
@@ -561,110 +558,110 @@
             Raises:
                 KeyFileError: Raised if the file is corrupt of non-existent.
                 CryptoKeyError: Raised if the user enters an incorrect password for an encrypted keyfile.
         """
         if self._coldkeypub == None:
             self._coldkeypub = self.coldkeypub_file.keypair
         return self._coldkeypub
-            
+
     def create_coldkey_from_uri(self, uri:str, use_password: bool = True, overwrite:bool = False) -> 'Wallet':
         """ Creates coldkey from suri string, optionally encrypts it with the user's inputed password.
             Args:
                 uri: (str, required):
                     URI string to use i.e. /Alice or /Bob
                 use_password (bool, optional):
                     Is the created key password protected.
-                overwrite (bool, optional): 
+                overwrite (bool, optional):
                     Will this operation overwrite the coldkey under the same path <wallet path>/<wallet name>/coldkey
             Returns:
                 wallet (bittensor.Wallet):
                     this object with newly created coldkey.
         """
         keypair = Keypair.create_from_uri( uri )
         display_mnemonic_msg( keypair, "coldkey" )
         self.set_coldkey( keypair, encrypt = use_password, overwrite = overwrite)
         self.set_coldkeypub( keypair, overwrite = overwrite)
         return self
 
-    def create_hotkey_from_uri( self, uri:str, use_password: bool = False, overwrite:bool = False) -> 'Wallet':  
+    def create_hotkey_from_uri( self, uri:str, use_password: bool = False, overwrite:bool = False) -> 'Wallet':
         """ Creates hotkey from suri string, optionally encrypts it with the user's inputed password.
             Args:
                 uri: (str, required):
                     URI string to use i.e. /Alice or /Bob
                 use_password (bool, optional):
                     Is the created key password protected.
-                overwrite (bool, optional): 
+                overwrite (bool, optional):
                     Will this operation overwrite the hotkey under the same path <wallet path>/<wallet name>/hotkeys/<hotkey>
             Returns:
                 wallet (bittensor.Wallet):
                     this object with newly created hotkey.
         """
         keypair = Keypair.create_from_uri( uri )
         display_mnemonic_msg( keypair, "hotkey" )
         self.set_hotkey( keypair, encrypt=use_password, overwrite = overwrite)
         return self
 
-    def new_coldkey( self, n_words:int = 12, use_password: bool = True, overwrite:bool = False) -> 'Wallet':  
+    def new_coldkey( self, n_words:int = 12, use_password: bool = True, overwrite:bool = False) -> 'Wallet':
         """ Creates a new coldkey, optionally encrypts it with the user's inputed password and saves to disk.
             Args:
                 n_words: (int, optional):
                     Number of mnemonic words to use.
                 use_password (bool, optional):
                     Is the created key password protected.
-                overwrite (bool, optional): 
+                overwrite (bool, optional):
                     Will this operation overwrite the coldkey under the same path <wallet path>/<wallet name>/coldkey
             Returns:
                 wallet (bittensor.Wallet):
                     this object with newly created coldkey.
         """
         self.create_new_coldkey( n_words, use_password, overwrite )
 
-    def create_new_coldkey( self, n_words:int = 12, use_password: bool = True, overwrite:bool = False) -> 'Wallet':  
+    def create_new_coldkey( self, n_words:int = 12, use_password: bool = True, overwrite:bool = False) -> 'Wallet':
         """ Creates a new coldkey, optionally encrypts it with the user's inputed password and saves to disk.
             Args:
                 n_words: (int, optional):
                     Number of mnemonic words to use.
                 use_password (bool, optional):
                     Is the created key password protected.
-                overwrite (bool, optional): 
+                overwrite (bool, optional):
                     Will this operation overwrite the coldkey under the same path <wallet path>/<wallet name>/coldkey
             Returns:
                 wallet (bittensor.Wallet):
                     this object with newly created coldkey.
         """
         mnemonic = Keypair.generate_mnemonic( n_words)
         keypair = Keypair.create_from_mnemonic(mnemonic)
         display_mnemonic_msg( keypair, "coldkey" )
         self.set_coldkey( keypair, encrypt = use_password, overwrite = overwrite)
         self.set_coldkeypub( keypair, overwrite = overwrite)
         return self
 
-    def new_hotkey( self, n_words:int = 12, use_password: bool = False, overwrite:bool = False) -> 'Wallet':  
+    def new_hotkey( self, n_words:int = 12, use_password: bool = False, overwrite:bool = False) -> 'Wallet':
         """ Creates a new hotkey, optionally encrypts it with the user's inputed password and saves to disk.
             Args:
                 n_words: (int, optional):
                     Number of mnemonic words to use.
                 use_password (bool, optional):
                     Is the created key password protected.
-                overwrite (bool, optional): 
+                overwrite (bool, optional):
                     Will this operation overwrite the hotkey under the same path <wallet path>/<wallet name>/hotkeys/<hotkey>
             Returns:
                 wallet (bittensor.Wallet):
                     this object with newly created hotkey.
         """
         self.create_new_hotkey( n_words, use_password, overwrite )
 
-    def create_new_hotkey( self, n_words:int = 12, use_password: bool = False, overwrite:bool = False) -> 'Wallet':  
+    def create_new_hotkey( self, n_words:int = 12, use_password: bool = False, overwrite:bool = False) -> 'Wallet':
         """ Creates a new hotkey, optionally encrypts it with the user's inputed password and saves to disk.
             Args:
                 n_words: (int, optional):
                     Number of mnemonic words to use.
                 use_password (bool, optional):
                     Is the created key password protected.
-                overwrite (bool, optional): 
+                overwrite (bool, optional):
                     Will this operation overwrite the hotkey under the same path <wallet path>/<wallet name>/hotkeys/<hotkey>
             Returns:
                 wallet (bittensor.Wallet):
                     this object with newly created hotkey.
         """
         mnemonic = Keypair.generate_mnemonic( n_words)
         keypair = Keypair.create_from_mnemonic(mnemonic)
@@ -681,21 +678,21 @@
                 public_key: (str | bytes, optional):
                     Public key as hex string or bytes.
                 overwrite (bool, optional) (default: False):
                     Will this operation overwrite the coldkeypub (if exists) under the same path <wallet path>/<wallet name>/coldkeypub
             Returns:
                 wallet (bittensor.Wallet):
                     newly re-generated Wallet with coldkeypub.
-            
+
         """
         if ss58_address is None and public_key is None:
             raise ValueError("Either ss58_address or public_key must be passed")
 
         if not is_valid_bittensor_address_or_public_key( ss58_address if ss58_address is not None else public_key ):
-            raise ValueError(f"Invalid {'ss58_address' if ss58_address is not None else 'public_key'}") 
+            raise ValueError(f"Invalid {'ss58_address' if ss58_address is not None else 'public_key'}")
 
         if ss58_address is not None:
             ss58_format = bittensor.utils.get_ss58_format( ss58_address )
             keypair = Keypair(ss58_address=ss58_address, public_key=public_key, ss58_format=ss58_format)
         else:
             keypair = Keypair(ss58_address=ss58_address, public_key=public_key, ss58_format=bittensor.__ss58_format__)
 
@@ -747,30 +744,30 @@
                     Key mnemonic as list of words or string space separated words.
                 seed: (str, optional):
                     Seed as hex string.
                 json: (Tuple[Union[str, Dict], str], optional):
                     Restore from encrypted JSON backup as (json_data: Union[str, Dict], passphrase: str)
                 use_password (bool, optional):
                     Is the created key password protected.
-                overwrite (bool, optional): 
+                overwrite (bool, optional):
                     Will this operation overwrite the coldkey under the same path <wallet path>/<wallet name>/coldkey
             Returns:
                 wallet (bittensor.Wallet):
                     this object with newly created coldkey.
 
             Note: uses priority order: mnemonic > seed > json
         """
         if len(kwargs) == 0:
             raise ValueError("Must pass either mnemonic, seed, or json")
-        
+
         # Get from kwargs
         mnemonic = kwargs.get('mnemonic', None)
         seed = kwargs.get('seed', None)
         json = kwargs.get('json', None)
-        
+
         if mnemonic is None and seed is None and json is None:
             raise ValueError("Must pass either mnemonic, seed, or json")
         if mnemonic is not None:
             if isinstance( mnemonic, str): mnemonic = mnemonic.split()
             if len(mnemonic) not in [12,15,18,21,24]:
                 raise ValueError("Mnemonic has invalid size. This should be 12,15,18,21 or 24 words")
             keypair = Keypair.create_from_mnemonic(" ".join(mnemonic), ss58_format=bittensor.__ss58_format__ )
@@ -780,18 +777,18 @@
         else:
             # json is not None
             if not isinstance(json, tuple) or len(json) != 2 or not isinstance(json[0], (str, dict)) or not isinstance(json[1], str):
                 raise ValueError("json must be a tuple of (json_data: str | Dict, passphrase: str)")
 
             json_data, passphrase = json
             keypair = Keypair.create_from_encrypted_json( json_data, passphrase, ss58_format=bittensor.__ss58_format__ )
-            
+
         self.set_coldkey( keypair, encrypt = use_password, overwrite = overwrite)
         self.set_coldkeypub( keypair, overwrite = overwrite)
-        return self 
+        return self
 
     # Short name for regenerate_coldkey
     regen_coldkey = regenerate_coldkey
 
     @overload
     def regenerate_hotkey(
             self,
@@ -831,23 +828,23 @@
                     Key mnemonic as list of words or string space separated words.
                 seed: (str, optional):
                     Seed as hex string.
                 json: (Tuple[Union[str, Dict], str], optional):
                     Restore from encrypted JSON backup as (json_data: Union[str, Dict], passphrase: str)
                 use_password (bool, optional):
                     Is the created key password protected.
-                overwrite (bool, optional): 
+                overwrite (bool, optional):
                     Will this operation overwrite the hotkey under the same path <wallet path>/<wallet name>/hotkeys/<hotkey>
             Returns:
                 wallet (bittensor.Wallet):
                     this object with newly created hotkey.
         """
         if len(kwargs) == 0:
             raise ValueError("Must pass either mnemonic, seed, or json")
-        
+
         # Get from kwargs
         mnemonic = kwargs.get('mnemonic', None)
         seed = kwargs.get('seed', None)
         json = kwargs.get('json', None)
 
         if mnemonic is None and seed is None and json is None:
             raise ValueError("Must pass either mnemonic, seed, or json")
@@ -863,13 +860,13 @@
             # json is not None
             if not isinstance(json, tuple) or len(json) != 2 or not isinstance(json[0], (str, dict)) or not isinstance(json[1], str):
                 raise ValueError("json must be a tuple of (json_data: str | Dict, passphrase: str)")
 
             json_data, passphrase = json
             keypair = Keypair.create_from_encrypted_json( json_data, passphrase, ss58_format=bittensor.__ss58_format__ )
 
-        
+
         self.set_hotkey( keypair, encrypt=use_password, overwrite = overwrite)
-        return self 
-    
+        return self
+
     # Short name for regenerate_hotkey
     regen_hotkey = regenerate_hotkey
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/_wallet/wallet_mock.py` & `bittensor-5.0.0/bittensor/_wallet/wallet_mock.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import bittensor
 
 class Wallet_mock(wallet_impl.Wallet):
     """
     Mocked Version of the bittensor wallet class, meant to be used for testing
     """
-    def __init__( 
+    def __init__(
         self,
         _mock:bool,
         **kwargs,
     ):
         r""" Init bittensor wallet object containing a hot and coldkey.
             Args:
                 _mock (required=True, default=False):
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/utils/__init__.py` & `bittensor-5.0.0/bittensor/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 from substrateinterface.utils import ss58
 from .registration import create_pow
 
 RAOPERTAO = 1e9
 U16_MAX = 65535
 U64_MAX = 18446744073709551615
 
-def indexed_values_to_dataframe ( 
+def indexed_values_to_dataframe (
         prefix: Union[str, int],
-        index: Union[list, torch.LongTensor], 
+        index: Union[list, torch.LongTensor],
         values: Union[list, torch.Tensor],
         filter_zeros: bool = False
     ) -> 'pandas.DataFrame':
     # Type checking.
     if not isinstance(prefix, str) and not isinstance(prefix, numbers.Number):
         raise ValueError('Passed prefix must have type str or Number')
     if isinstance(prefix, numbers.Number):
@@ -46,15 +46,15 @@
 def unbiased_topk( values, k, dim=0, sorted = True, largest = True):
     r""" Selects topk as in torch.topk but does not bias lower indices when values are equal.
         Args:
             values: (torch.Tensor)
                 Values to index into.
             k: (int):
                 Number to take.
-            
+
         Return:
             topk: (torch.Tensor):
                 topk k values.
             indices: (torch.LongTensor)
                 indices of the topk values.
     """
     permutation = torch.randperm(values.shape[ dim ])
@@ -91,17 +91,17 @@
 def is_valid_ed25519_pubkey( public_key: Union[str, bytes] ) -> bool:
     """
     Checks if the given public_key is a valid ed25519 key.
 
     Args:
         public_key(Union[str, bytes]): The public_key to check.
 
-    Returns:    
+    Returns:
         True if the public_key is a valid ed25519 key, False otherwise.
-    
+
     """
     try:
         if isinstance( public_key, str ):
             if len(public_key) != 64 and len(public_key) != 66:
                 raise ValueError( "a public_key should be 64 or 66 characters" )
         elif isinstance( public_key, bytes ):
             if len(public_key) != 32:
@@ -181,57 +181,57 @@
 def get_explorer_root_url_by_network_from_map(network: str, network_map: Dict[str, str]) -> Optional[str]:
     r"""
     Returns the explorer root url for the given network name from the given network map.
 
     Args:
         network(str): The network to get the explorer url for.
         network_map(Dict[str, str]): The network map to get the explorer url from.
-    
+
     Returns:
         The explorer url for the given network.
         Or None if the network is not in the network map.
     """
     explorer_url: Optional[str] = None
     if network in network_map:
         explorer_url = network_map[network]
 
     return explorer_url
-    
+
 
 def get_explorer_url_for_network(network: str, block_hash: str, network_map: Dict[str, str]) -> Optional[str]:
     r"""
     Returns the explorer url for the given block hash and network.
 
     Args:
         network(str): The network to get the explorer url for.
         block_hash(str): The block hash to get the explorer url for.
         network_map(Dict[str, str]): The network map to get the explorer url from.
-    
+
     Returns:
         The explorer url for the given block hash and network.
         Or None if the network is not known.
     """
 
     explorer_url: Optional[str] = None
     # Will be None if the network is not known. i.e. not in network_map
     explorer_root_url: Optional[str] = get_explorer_root_url_by_network_from_map(network, network_map)
 
     if explorer_root_url is not None:
         # We are on a known network.
         explorer_url = "{root_url}/query/{block_hash}".format( root_url=explorer_root_url, block_hash = block_hash )
-    
+
     return explorer_url
 
 def ss58_address_to_bytes(ss58_address: str) -> bytes:
     """Converts a ss58 address to a bytes object."""
     account_id_hex: str = scalecodec.ss58_decode(ss58_address, bittensor.__ss58_format__)
     return bytes.fromhex(account_id_hex)
 
 def U16_NORMALIZED_FLOAT( x: int ) -> float:
-    return float( x ) / float( U16_MAX ) 
+    return float( x ) / float( U16_MAX )
 
 def U64_NORMALIZED_FLOAT( x: int ) -> float:
     return float( x ) / float( U64_MAX )
 
 def u8_key_to_ss58(u8_key: List[int]) -> str:
     r"""
     Converts a u8-encoded account key to an ss58 address.
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/utils/_register_cuda.py` & `bittensor-5.0.0/bittensor/utils/_register_cuda.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post3/bittensor/utils/balance.py` & `bittensor-5.0.0/bittensor/utils/balance.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
     def __repr__(self):
         return self.__str__()
 
     def __eq__(self, other: Union[int, float, "Balance"]):
         if other is None:
             return False
-            
+
         if hasattr(other, "rao"):
             return self.rao == other.rao
         else:
             try:
                 # Attempt to cast to int from rao
                 other_rao = int(other)
                 return self.rao == other_rao
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/utils/codes.py` & `bittensor-5.0.0/bittensor/utils/codes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 """ utils for rpc log, convert return code to string with color for the log
 """
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 from loguru import logger
-import bittensor 
+import bittensor
 
 logger = logger.opt(colors=True)
 
 def code_to_string( code: 'bittensor.proto.ReturnCode' ) -> str:
     """ Return code -> string
     """
-    if code == 0: 
+    if code == 0:
         return 'NoReturn'
-    elif code == 1: 
+    elif code == 1:
         return 'Success'
     elif code == 2:
         return 'Timeout'
     elif code == 3:
         return 'Backoff'
     elif code == 4:
         return 'Unavailable'
@@ -79,17 +79,17 @@
         return 'Blacklisted'
     else:
         return 'UnknownCode'
 
 def code_to_loguru_color( code: 'bittensor.proto.ReturnCode' ) -> str:
     """ Return code -> loguru color
     """
-    if code == 0: 
+    if code == 0:
         return 'red'
-    elif code == 1: 
+    elif code == 1:
         return 'green'
     elif code == 2:
         return 'yellow'
     elif code == 3:
         return 'yellow'
     elif code == 4:
         return 'red'
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/utils/formatting.py` & `bittensor-5.0.0/bittensor/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post3/bittensor/utils/networking.py` & `bittensor-5.0.0/bittensor/utils/networking.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-""" Utils for handling local network with ip and ports. 
+""" Utils for handling local network with ip and ports.
 """
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import os
 import urllib
 import json
 import miniupnpc
 import netaddr
 import requests
 
 from loguru import logger
 
 def int_to_ip(int_val: int) -> str:
-    r""" Maps an integer to a unique ip-string 
+    r""" Maps an integer to a unique ip-string
         Args:
             int_val  (:type:`int128`, `required`):
                 The integer representation of an ip. Must be in the range (0, 3.4028237e+38).
 
         Returns:
             str_val (:tyep:`str`, `required):
                 The string representation of an ip. Of form *.*.*.* for ipv4 or *::*:*:*:* for ipv6
 
         Raises:
             netaddr.core.AddrFormatError (Exception):
                 Raised when the passed int_vals is not a valid ip int value.
     """
     return str(netaddr.IPAddress(int_val))
- 
+
 def ip_to_int(str_val: str) -> int:
     r""" Maps an ip-string to a unique integer.
         arg:
             str_val (:tyep:`str`, `required):
                 The string representation of an ip. Of form *.*.*.* for ipv4 or *::*:*:*:* for ipv6
 
         Returns:
@@ -116,33 +116,33 @@
         external_ip = json.loads(process.read())['ip']
         process.close()
         assert isinstance(ip_to_int(external_ip), int)
         return str(external_ip)
     except Exception:
         pass
 
-    # --- Try myip.dnsomatic 
+    # --- Try myip.dnsomatic
     try:
         process = os.popen('curl -s myip.dnsomatic.com')
         external_ip  = process.readline()
         process.close()
         assert isinstance(ip_to_int(external_ip), int)
         return str(external_ip)
     except Exception:
-        pass    
+        pass
 
-    # --- Try urllib ipv6 
+    # --- Try urllib ipv6
     try:
         external_ip = urllib.request.urlopen('https://ident.me').read().decode('utf8')
         assert isinstance(ip_to_int(external_ip), int)
         return str(external_ip)
     except Exception:
         pass
 
-    # --- Try Wikipedia 
+    # --- Try Wikipedia
     try:
         external_ip = requests.get('https://www.wikipedia.org').headers['X-Client-IP']
         assert isinstance(ip_to_int(external_ip), int)
         return str(external_ip)
     except Exception:
         pass
 
@@ -152,15 +152,15 @@
 class UPNPCException(Exception):
     """ Raised when trying to perform a port mapping on your router. """
 
 
 def upnpc_create_port_map(port: int):
     r""" Creates a upnpc port map on your router from passed external_port to local port.
 
-        Args: 
+        Args:
             port (int, `required`):
                 The local machine port to map from your external port.
 
         Return:
             external_port (int, `required`):
                 The external port mapped to the local port on your machine.
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/utils/registration.py` & `bittensor-5.0.0/bittensor/utils/registration.py`

 * *Files 5% similar despite different names*

```diff
@@ -127,26 +127,24 @@
         self.curr_diff = curr_diff
         self.check_block = check_block
         self.stopEvent = stopEvent
         self.limit = limit
 
     def run(self):
         raise NotImplementedError("_SolverBase is an abstract class")
-    
     @staticmethod
     def create_shared_memory() -> Tuple[multiprocessing.Array, multiprocessing.Value, multiprocessing.Array]:
         """Creates shared memory for the solver processes to use.
         """
         curr_block = multiprocessing.Array('h', 32, lock=True) # byte array
         curr_block_num = multiprocessing.Value('i', 0, lock=True) # int
         curr_diff = multiprocessing.Array('Q', [0, 0], lock=True) # [high, low]
 
         return curr_block, curr_block_num, curr_diff
 
-
 class _Solver(_SolverBase):
     def run(self):
         block_number: int
         block_and_hotkey_hash_bytes: bytes
         block_difficulty: int
         nonce_limit = int(math.pow(2,64)) - 1
 
@@ -157,26 +155,26 @@
             if self.newBlockEvent.is_set():
                 with self.check_block:
                     block_number = self.curr_block_num.value
                     block_and_hotkey_hash_bytes = bytes(self.curr_block)
                     block_difficulty = _registration_diff_unpack(self.curr_diff)
 
                 self.newBlockEvent.clear()
-                
+
             # Do a block of nonces
             solution = _solve_for_nonce_block(nonce_start, nonce_end, block_and_hotkey_hash_bytes, block_difficulty, self.limit, block_number)
             if solution is not None:
                 self.solution_queue.put(solution)
 
             try:
                 # Send time
                 self.finished_queue.put_nowait(self.proc_num)
             except Full:
                 pass
-                
+
             nonce_start = random.randint( 0, nonce_limit )
             nonce_start = nonce_start % nonce_limit
             nonce_end = nonce_start + self.update_interval
 
 
 class _CUDASolver(_SolverBase):
     dev_id: int
@@ -199,53 +197,54 @@
             if self.newBlockEvent.is_set():
                 with self.check_block:
                     block_number = self.curr_block_num.value
                     block_and_hotkey_hash_bytes = bytes(self.curr_block)
                     block_difficulty = _registration_diff_unpack(self.curr_diff)
 
                 self.newBlockEvent.clear()
-                
+
             # Do a block of nonces
             solution = _solve_for_nonce_block_cuda(nonce_start, self.update_interval, block_and_hotkey_hash_bytes, block_difficulty, self.limit, block_number, self.dev_id, self.TPB)
             if solution is not None:
                 self.solution_queue.put(solution)
 
             try:
                 # Signal that a nonce_block was finished using queue
                 # send our proc_num
                 self.finished_queue.put(self.proc_num)
             except Full:
                 pass
-            
+
             # increase nonce by number of nonces processed
-            nonce_start += self.update_interval * self.TPB 
+            nonce_start += self.update_interval * self.TPB
             nonce_start = nonce_start % nonce_limit
 
 
 def _solve_for_nonce_block_cuda(nonce_start: int, update_interval: int, block_and_hotkey_hash_bytes: bytes, difficulty: int, limit: int, block_number: int, dev_id: int, TPB: int) -> Optional[POWSolution]:
     """Tries to solve the POW on a CUDA device for a block of nonces (nonce_start, nonce_start + update_interval * TPB"""
     solution, seal = solve_cuda(
                     nonce_start,
                     update_interval,
                     TPB,
-                    block_and_hotkey_hash_bytes, 
-                    difficulty, 
+                    block_and_hotkey_hash_bytes,
+                    difficulty,
                     limit,
                     dev_id)
     
 
+
     if (solution != -1):
         # Check if solution is valid (i.e. not -1)
         return POWSolution(solution, block_number, difficulty, seal)
 
     return None
 
 
 def _solve_for_nonce_block(nonce_start: int, nonce_end: int, block_and_hotkey_hash_bytes: bytes, difficulty: int, limit: int, block_number: int) -> Optional[POWSolution]:
-    """Tries to solve the POW for a block of nonces (nonce_start, nonce_end)""" 
+    """Tries to solve the POW for a block of nonces (nonce_start, nonce_end)"""
     for nonce in range(nonce_start, nonce_end):
         # Create seal.
         seal = _create_seal_hash(block_and_hotkey_hash_bytes, nonce)
 
         # Check if seal meets difficulty
         if _seal_meets_difficulty(seal, difficulty, limit):
             # Found a solution, save it.
@@ -298,29 +297,29 @@
     time_average: float
     time_spent: float
     hash_rate_perpetual: float
     hash_rate: float
     difficulty: int
     block_number: int
     block_hash: bytes
-    
+
 
 class RegistrationStatisticsLogger:
     """Logs statistics for a registration."""
     console: rich_console.Console
-    status: Optional[rich_status.Status] 
+    status: Optional[rich_status.Status]
 
     def __init__( self, console: rich_console.Console, output_in_place: bool = True) -> None:
         self.console = console
-        
+
         if output_in_place:
             self.status = self.console.status("Solving")
         else:
             self.status = None
-        
+
     def start( self ) -> None:
         if self.status is not None:
             self.status.start()
 
     def stop( self ) -> None:
         if self.status is not None:
             self.status.stop()
@@ -368,41 +367,40 @@
         n_samples: int
             The number of samples of the hash_rate to keep for the EWMA
         alpha_: float
             The alpha for the EWMA for the hash_rate calculation
         log_verbose: bool
             If true, prints more verbose logging of the registration metrics.
     Note: The hash rate is calculated as an exponentially weighted moving average in order to make the measure more robust.
-    Note: 
+    Note:
     - We can also modify the update interval to do smaller blocks of work,
         while still updating the block information after a different number of nonces,
         to increase the transparency of the process while still keeping the speed.
     """
     if num_processes == None:
         # get the number of allowed processes for this process
         num_processes = min(1, get_cpu_count())
 
     if update_interval is None:
         update_interval = 50_000
-        
+
     limit = int(math.pow(2,256)) - 1
 
     curr_block, curr_block_num, curr_diff = _Solver.create_shared_memory()
 
     # Establish communication queues
     ## See the _Solver class for more information on the queues.
     stopEvent = multiprocessing.Event()
     stopEvent.clear()
 
     solution_queue = multiprocessing.Queue()
     finished_queues = [multiprocessing.Queue() for _ in range(num_processes)]
     check_block = multiprocessing.Lock()
 
     hotkey_bytes = wallet.hotkey.public_key
-    
     # Start consumers
     solvers = [ _Solver(i, num_processes, update_interval, finished_queues[i], solution_queue, stopEvent, curr_block, curr_block_num, curr_diff, check_block, limit)
                 for i in range(num_processes) ]
 
     # Get first block
     block_number, difficulty, block_hash = _get_block_with_retry(subtensor = subtensor, netuid = netuid)
 
@@ -410,45 +408,45 @@
     old_block_number = block_number
     # Set to current block
     _update_curr_block(curr_diff, curr_block, curr_block_num, block_number, block_bytes, difficulty, hotkey_bytes, check_block)
 
     # Set new block events for each solver to start at the initial block
     for worker in solvers:
         worker.newBlockEvent.set()
-    
+
     for worker in solvers:
         worker.start() # start the solver processes
 
     start_time = time.time() # time that the registration started
     time_last = start_time # time that the last work blocks completed
-    
+
     curr_stats = RegistrationStatistics(
         time_spent_total = 0.0,
         time_average = 0.0,
         rounds_total = 0,
         time_spent = 0.0,
         hash_rate_perpetual = 0.0,
         hash_rate = 0.0,
         difficulty = difficulty,
         block_number = block_number,
         block_hash = block_hash
     )
 
     start_time_perpetual = time.time()
-    
+
 
     console = bittensor.__console__
     logger = RegistrationStatisticsLogger(console, output_in_place)
     logger.start()
 
     solution = None
 
     hash_rates = [0] * n_samples # The last n true hash_rates
     weights = [alpha_ ** i for i in range(n_samples)] # weights decay by alpha
-    
+
     while not wallet.is_registered(netuid = netuid, subtensor = subtensor):
         # Wait until a solver finds a solution
         try:
             solution = solution_queue.get(block=True, timeout=0.25)
             if solution is not None:
                 break
         except Empty:
@@ -465,29 +463,29 @@
             curr_block=curr_block,
             curr_block_num=curr_block_num,
             curr_stats=curr_stats,
             update_curr_block=_update_curr_block,
             check_block=check_block,
             solvers=solvers
         )
-                
+
         num_time = 0
         for finished_queue in finished_queues:
             try:
                 proc_num = finished_queue.get(timeout=0.1)
                 num_time += 1
 
             except Empty:
                 continue
-        
+
         time_now = time.time() # get current time
         time_since_last = time_now - time_last # get time since last work block(s)
         if num_time > 0 and time_since_last > 0.0:
             # create EWMA of the hash_rate to make measure more robust
-        
+
             hash_rate_ = (num_time * update_interval) / time_since_last
             hash_rates.append(hash_rate_)
             hash_rates.pop(0) # remove the 0th data point
             curr_stats.hash_rate = sum([hash_rates[i]*weights[i] for i in range(n_samples)])/(sum(weights))
 
             # update time last to now
             time_last = time_now
@@ -524,19 +522,19 @@
 
     Args:
         subtensor (:obj:`bittensor.Subtensor`, `required`):
             The subtensor object to use to get the block number, difficulty, and block hash.
 
         netuid (:obj:`int`, `required`):
             The netuid of the network to get the block number, difficulty, and block hash from.
-        
+
     Returns:
         block_number (:obj:`int`):
             The current block number.
-        
+
         difficulty (:obj:`int`):
             The current difficulty of the subnet.
 
         block_hash (:obj:`bytes`):
             The current block hash.
 
     Raises:
@@ -666,15 +664,15 @@
         dev_id = [0]
 
     if update_interval is None:
         update_interval = 50_000
 
     if not torch.cuda.is_available():
         raise Exception("CUDA not available")
-        
+
     limit = int(math.pow(2,256)) - 1
 
     # Set mp start to use spawn so CUDA doesn't complain
     with _UsingSpawnStartMethod(force=True):
         curr_block, curr_block_num, curr_diff = _CUDASolver.create_shared_memory()
 
         ## Create a worker per CUDA device
@@ -684,39 +682,38 @@
         stopEvent = multiprocessing.Event()
         stopEvent.clear()
         solution_queue = multiprocessing.Queue()
         finished_queues = [multiprocessing.Queue() for _ in range(num_processes)]
         check_block = multiprocessing.Lock()
 
         hotkey_bytes = wallet.hotkey.public_key
-        
         # Start workers
         solvers = [ _CUDASolver(i, num_processes, update_interval, finished_queues[i], solution_queue, stopEvent, curr_block, curr_block_num, curr_diff, check_block, limit, dev_id[i], TPB)
                     for i in range(num_processes) ]
 
 
         # Get first block
         block_number, difficulty, block_hash = _get_block_with_retry(subtensor = subtensor, netuid = netuid)
 
         block_bytes = bytes.fromhex(block_hash[2:])
         old_block_number = block_number
-        
+
         # Set to current block
         _update_curr_block(curr_diff, curr_block, curr_block_num, block_number, block_bytes, difficulty, hotkey_bytes, check_block)
 
         # Set new block events for each solver to start at the initial block
         for worker in solvers:
             worker.newBlockEvent.set()
-        
+
         for worker in solvers:
             worker.start() # start the solver processes
-        
+
         start_time = time.time() # time that the registration started
         time_last = start_time # time that the last work blocks completed
-        
+
         curr_stats = RegistrationStatistics(
             time_spent_total = 0.0,
             time_average = 0.0,
             rounds_total = 0,
             time_spent = 0.0,
             hash_rate_perpetual = 0.0,
             hash_rate = 0.0, # EWMA hash_rate (H/s)
@@ -740,67 +737,67 @@
             try:
                 solution = solution_queue.get(block=True, timeout=0.15)
                 if solution is not None:
                     break
             except Empty:
                 # No solution found, try again
                 pass
-            
+
             # check for new block
             old_block_number = _check_for_newest_block_and_update(
                 subtensor = subtensor,
                 netuid = netuid,
                 hotkey_bytes = hotkey_bytes,
                 curr_diff=curr_diff,
                 curr_block=curr_block,
                 curr_block_num=curr_block_num,
                 old_block_number=old_block_number,
                 curr_stats=curr_stats,
                 update_curr_block=_update_curr_block,
                 check_block=check_block,
                 solvers=solvers
             )
-                    
+
             num_time = 0
             # Get times for each solver
             for finished_queue in finished_queues:
                 try:
                     proc_num = finished_queue.get(timeout=0.1)
                     num_time += 1
-            
+
                 except Empty:
                     continue
-            
+
             time_now = time.time() # get current time
             time_since_last = time_now - time_last # get time since last work block(s)
             if num_time > 0 and time_since_last > 0.0:
                 # create EWMA of the hash_rate to make measure more robust
-            
+
                 hash_rate_ = (num_time * TPB * update_interval) / time_since_last
                 hash_rates.append(hash_rate_)
                 hash_rates.pop(0) # remove the 0th data point
                 curr_stats.hash_rate = sum([hash_rates[i]*weights[i] for i in range(n_samples)])/(sum(weights))
 
                 # update time last to now
                 time_last = time_now
 
                 curr_stats.time_average = (curr_stats.time_average*curr_stats.rounds_total + curr_stats.time_spent)/(curr_stats.rounds_total+num_time)
                 curr_stats.rounds_total += num_time
-            
+
             # Update stats
             curr_stats.time_spent = time_since_last
             new_time_spent_total = time_now - start_time_perpetual
             curr_stats.hash_rate_perpetual = (curr_stats.rounds_total * (TPB * update_interval))/ new_time_spent_total
             curr_stats.time_spent_total = new_time_spent_total
 
             # Update the logger
             logger.update(curr_stats, verbose=log_verbose)
-        
+
         # exited while, found_solution contains the nonce or wallet is registered
-        
+
         stopEvent.set() # stop all other processes
         logger.stop()
 
         # terminate and wait for all solvers to exit
         _terminate_workers_and_wait_for_exit(solvers)
 
         return solution
@@ -847,19 +844,19 @@
         num_processes (:obj:`int`, `optional`, defaults to :obj:`None`):
             The number of processes to use when solving the proof of work.
             If None, then the number of processes is equal to the number of
                 CPU cores.
         update_interval (:obj:`int`, `optional`, defaults to :obj:`None`):
             The number of nonces to run before checking for a new block.
         log_verbose (:obj:`bool`, `optional`, defaults to :obj:`False`):
-            If true, prints the progress of the proof of work more verbosely.   
+            If true, prints the progress of the proof of work more verbosely.
     Returns:
         :obj:`Optional[Dict[str, Any]]`: The proof of work solution or None if
             the wallet is already registered or there is a different error.
-    
+
     Raises:
         :obj:`ValueError`: If the subnet does not exist.
     """
     if not subtensor.subnet_exists(netuid = netuid):
         raise ValueError(f'Subnet {netuid} does not exist')
 
     if cuda:
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/utils/registratrion_old.py` & `bittensor-5.0.0/bittensor/utils/registratrion_old.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     return hex_chunks
 
 
 def u8_list_to_hex( values: list ):
     total = 0
     for val in reversed(values):
         total = (total << 8) + val
-    return total 
+    return total
 
 
 def create_seal_hash( block_hash:bytes, nonce:int ) -> bytes:
     block_bytes = block_hash.encode('utf-8')[2:]
     nonce_bytes = binascii.hexlify(nonce.to_bytes(8, 'little'))
     pre_seal = nonce_bytes + block_bytes
     seal_sh256 = hashlib.sha256( bytearray(hex_bytes_to_u8_list(pre_seal)) ).digest()
@@ -51,21 +51,21 @@
     seal_number = int.from_bytes(seal, "big")
     product = seal_number * difficulty
     limit = int(math.pow(2,256))- 1
     if product > limit:
         return False
     else:
         return True
-    
+
 
 def solve_for_difficulty( block_hash, difficulty ):
     meets = False
     nonce = -1
     while not meets:
-        nonce += 1 
+        nonce += 1
         seal = create_seal_hash( block_hash, nonce )
         meets = seal_meets_difficulty( seal, difficulty )
         if nonce > 1:
             break
     return nonce, seal
 
 
@@ -190,26 +190,26 @@
             if self.newBlockEvent.is_set():
                 with self.check_block:
                     block_number = self.curr_block_num.value
                     block_bytes = bytes(self.curr_block)
                     block_difficulty = registration_diff_unpack(self.curr_diff)
 
                 self.newBlockEvent.clear()
-                
+
             # Do a block of nonces
             solution = solve_for_nonce_block(self, nonce_start, nonce_end, block_bytes, block_difficulty, self.limit, block_number)
             if solution is not None:
                 self.solution_queue.put(solution)
 
             try:
                 # Send time
                 self.finished_queue.put_nowait(self.proc_num)
             except Full:
                 pass
-                
+
             nonce_start = random.randint( 0, nonce_limit )
             nonce_start = nonce_start % nonce_limit
             nonce_end = nonce_start + self.update_interval
 
 
 class CUDASolver(SolverBase):
     dev_id: int
@@ -232,52 +232,52 @@
             if self.newBlockEvent.is_set():
                 with self.check_block:
                     block_number = self.curr_block_num.value
                     block_bytes = bytes(self.curr_block)
                     block_difficulty = registration_diff_unpack(self.curr_diff)
 
                 self.newBlockEvent.clear()
-                
+
             # Do a block of nonces
             solution = solve_for_nonce_block_cuda(self, nonce_start, self.update_interval, block_bytes, block_difficulty, self.limit, block_number, self.dev_id, self.TPB)
             if solution is not None:
                 self.solution_queue.put(solution)
 
             try:
                 # Signal that a nonce_block was finished using queue
                 # send our proc_num
                 self.finished_queue.put(self.proc_num)
             except Full:
                 pass
-            
+
             # increase nonce by number of nonces processed
-            nonce_start += self.update_interval * self.TPB 
+            nonce_start += self.update_interval * self.TPB
             nonce_start = nonce_start % nonce_limit
 
 
 def solve_for_nonce_block_cuda(solver: CUDASolver, nonce_start: int, update_interval: int, block_bytes: bytes, difficulty: int, limit: int, block_number: int, dev_id: int, TPB: int) -> Optional[POWSolution]:
     """Tries to solve the POW on a CUDA device for a block of nonces (nonce_start, nonce_start + update_interval * TPB"""
     solution, seal = solve_cuda(
                     nonce_start,
                     update_interval,
                     TPB,
-                    block_bytes, 
-                    difficulty, 
+                    block_bytes,
+                    difficulty,
                     limit,
                     dev_id)
 
     if (solution != -1):
         # Check if solution is valid (i.e. not -1)
         return POWSolution(solution, block_number, difficulty, seal)
 
     return None
 
 
 def solve_for_nonce_block(solver: Solver, nonce_start: int, nonce_end: int, block_bytes: bytes, difficulty: int, limit: int, block_number: int) -> Optional[POWSolution]:
-    """Tries to solve the POW for a block of nonces (nonce_start, nonce_end)""" 
+    """Tries to solve the POW for a block of nonces (nonce_start, nonce_end)"""
     for nonce in range(nonce_start, nonce_end):
         # Create seal.
         nonce_bytes = binascii.hexlify(nonce.to_bytes(8, 'little'))
         pre_seal = nonce_bytes + block_bytes
         seal_sh256 = hashlib.sha256( bytearray(hex_bytes_to_u8_list(pre_seal)) ).digest()
         kec = keccak.new(digest_bits=256)
         seal = kec.update( seal_sh256 ).digest()
@@ -326,29 +326,29 @@
     time_average: float
     time_spent: float
     hash_rate_perpetual: float
     hash_rate: float
     difficulty: int
     block_number: int
     block_hash: bytes
-    
+
 
 class RegistrationStatisticsLogger:
     """Logs statistics for a registration."""
     console: rich_console.Console
-    status: Optional[rich_status.Status] 
+    status: Optional[rich_status.Status]
 
     def __init__( self, console: rich_console.Console, output_in_place: bool = True) -> None:
         self.console = console
-        
+
         if output_in_place:
             self.status = self.console.status("Solving")
         else:
             self.status = None
-        
+
     def start( self ) -> None:
         if self.status is not None:
             self.status.start()
 
     def stop( self ) -> None:
         if self.status is not None:
             self.status.stop()
@@ -394,41 +394,41 @@
         n_samples: int
             The number of samples of the hash_rate to keep for the EWMA
         alpha_: float
             The alpha for the EWMA for the hash_rate calculation
         log_verbose: bool
             If true, prints more verbose logging of the registration metrics.
     Note: The hash rate is calculated as an exponentially weighted moving average in order to make the measure more robust.
-    Note: 
+    Note:
     - We can also modify the update interval to do smaller blocks of work,
         while still updating the block information after a different number of nonces,
         to increase the transparency of the process while still keeping the speed.
     """
     if num_processes == None:
         # get the number of allowed processes for this process
         num_processes = min(1, get_cpu_count())
 
     if update_interval is None:
         update_interval = 50_000
-        
+
     limit = int(math.pow(2,256)) - 1
 
     curr_block = multiprocessing.Array('h', 64, lock=True) # byte array
     curr_block_num = multiprocessing.Value('i', 0, lock=True) # int
     curr_diff = multiprocessing.Array('Q', [0, 0], lock=True) # [high, low]
 
     # Establish communication queues
     ## See the Solver class for more information on the queues.
     stopEvent = multiprocessing.Event()
     stopEvent.clear()
 
     solution_queue = multiprocessing.Queue()
     finished_queues = [multiprocessing.Queue() for _ in range(num_processes)]
     check_block = multiprocessing.Lock()
-    
+
     # Start consumers
     solvers = [ Solver(i, num_processes, update_interval, finished_queues[i], solution_queue, stopEvent, curr_block, curr_block_num, curr_diff, check_block, limit)
                 for i in range(num_processes) ]
 
     # Get first block
     block_number = subtensor.get_current_block()
     difficulty = subtensor.difficulty
@@ -439,45 +439,45 @@
     old_block_number = block_number
     # Set to current block
     update_curr_block(curr_diff, curr_block, curr_block_num, block_number, block_bytes, difficulty, check_block)
 
     # Set new block events for each solver to start at the initial block
     for worker in solvers:
         worker.newBlockEvent.set()
-    
+
     for worker in solvers:
         worker.start() # start the solver processes
 
     start_time = time.time() # time that the registration started
     time_last = start_time # time that the last work blocks completed
-    
+
     curr_stats = RegistrationStatistics(
         time_spent_total = 0.0,
         time_average = 0.0,
         rounds_total = 0,
         time_spent = 0.0,
         hash_rate_perpetual = 0.0,
         hash_rate = 0.0,
         difficulty = difficulty,
         block_number = block_number,
         block_hash = block_hash
     )
 
     start_time_perpetual = time.time()
-    
+
 
     console = bittensor.__console__
     logger = RegistrationStatisticsLogger(console, output_in_place)
     logger.start()
 
     solution = None
 
     hash_rates = [0] * n_samples # The last n true hash_rates
     weights = [alpha_ ** i for i in range(n_samples)] # weights decay by alpha
-    
+
     while not wallet.is_registered(subtensor):
         # Wait until a solver finds a solution
         try:
             solution = solution_queue.get(block=True, timeout=0.25)
             if solution is not None:
                 break
         except Empty:
@@ -492,29 +492,29 @@
             curr_block=curr_block,
             curr_block_num=curr_block_num,
             curr_stats=curr_stats,
             update_curr_block=update_curr_block,
             check_block=check_block,
             solvers=solvers
         )
-                
+
         num_time = 0
         for finished_queue in finished_queues:
             try:
                 proc_num = finished_queue.get(timeout=0.1)
                 num_time += 1
 
             except Empty:
                 continue
-        
+
         time_now = time.time() # get current time
         time_since_last = time_now - time_last # get time since last work block(s)
         if num_time > 0 and time_since_last > 0.0:
             # create EWMA of the hash_rate to make measure more robust
-        
+
             hash_rate_ = (num_time * update_interval) / time_since_last
             hash_rates.append(hash_rate_)
             hash_rates.pop(0) # remove the 0th data point
             curr_stats.hash_rate = sum([hash_rates[i]*weights[i] for i in range(n_samples)])/(sum(weights))
 
             # update time last to now
             time_last = time_now
@@ -660,15 +660,15 @@
         dev_id = [0]
 
     if update_interval is None:
         update_interval = 50_000
 
     if not torch.cuda.is_available():
         raise Exception("CUDA not available")
-        
+
     limit = int(math.pow(2,256)) - 1
 
     # Set mp start to use spawn so CUDA doesn't complain
     with UsingSpawnStartMethod(force=True):
         curr_block = multiprocessing.Array('h', 64, lock=True) # byte array
         curr_block_num = multiprocessing.Value('i', 0, lock=True) # int
         curr_diff = multiprocessing.Array('Q', [0, 0], lock=True) # [high, low]
@@ -678,42 +678,42 @@
 
         # Establish communication queues
         stopEvent = multiprocessing.Event()
         stopEvent.clear()
         solution_queue = multiprocessing.Queue()
         finished_queues = [multiprocessing.Queue() for _ in range(num_processes)]
         check_block = multiprocessing.Lock()
-        
+
         # Start workers
         solvers = [ CUDASolver(i, num_processes, update_interval, finished_queues[i], solution_queue, stopEvent, curr_block, curr_block_num, curr_diff, check_block, limit, dev_id[i], TPB)
                     for i in range(num_processes) ]
 
 
         # Get first block
         block_number = subtensor.get_current_block()
         difficulty = subtensor.difficulty
         block_hash = subtensor.substrate.get_block_hash( block_number )
         while block_hash == None:
             block_hash = subtensor.substrate.get_block_hash( block_number )
         block_bytes = block_hash.encode('utf-8')[2:]
         old_block_number = block_number
-        
+
         # Set to current block
         update_curr_block(curr_diff, curr_block, curr_block_num, block_number, block_bytes, difficulty, check_block)
 
         # Set new block events for each solver to start at the initial block
         for worker in solvers:
             worker.newBlockEvent.set()
-        
+
         for worker in solvers:
             worker.start() # start the solver processes
-        
+
         start_time = time.time() # time that the registration started
         time_last = start_time # time that the last work blocks completed
-        
+
         curr_stats = RegistrationStatistics(
             time_spent_total = 0.0,
             time_average = 0.0,
             rounds_total = 0,
             time_spent = 0.0,
             hash_rate_perpetual = 0.0,
             hash_rate = 0.0, # EWMA hash_rate (H/s)
@@ -737,65 +737,65 @@
             try:
                 solution = solution_queue.get(block=True, timeout=0.15)
                 if solution is not None:
                     break
             except Empty:
                 # No solution found, try again
                 pass
-            
+
             # check for new block
             old_block_number = check_for_newest_block_and_update(
                 subtensor = subtensor,
                 curr_diff=curr_diff,
                 curr_block=curr_block,
                 curr_block_num=curr_block_num,
                 old_block_number=old_block_number,
                 curr_stats=curr_stats,
                 update_curr_block=update_curr_block,
                 check_block=check_block,
                 solvers=solvers
             )
-                    
+
             num_time = 0
             # Get times for each solver
             for finished_queue in finished_queues:
                 try:
                     proc_num = finished_queue.get(timeout=0.1)
                     num_time += 1
-            
+
                 except Empty:
                     continue
-            
+
             time_now = time.time() # get current time
             time_since_last = time_now - time_last # get time since last work block(s)
             if num_time > 0 and time_since_last > 0.0:
                 # create EWMA of the hash_rate to make measure more robust
-            
+
                 hash_rate_ = (num_time * TPB * update_interval) / time_since_last
                 hash_rates.append(hash_rate_)
                 hash_rates.pop(0) # remove the 0th data point
                 curr_stats.hash_rate = sum([hash_rates[i]*weights[i] for i in range(n_samples)])/(sum(weights))
 
                 # update time last to now
                 time_last = time_now
 
                 curr_stats.time_average = (curr_stats.time_average*curr_stats.rounds_total + curr_stats.time_spent)/(curr_stats.rounds_total+num_time)
                 curr_stats.rounds_total += num_time
-            
+
             # Update stats
             curr_stats.time_spent = time_since_last
             new_time_spent_total = time_now - start_time_perpetual
             curr_stats.hash_rate_perpetual = (curr_stats.rounds_total * (TPB * update_interval))/ new_time_spent_total
             curr_stats.time_spent_total = new_time_spent_total
 
             # Update the logger
             logger.update(curr_stats, verbose=log_verbose)
-        
+
         # exited while, found_solution contains the nonce or wallet is registered
-        
+
         stopEvent.set() # stop all other processes
         logger.stop()
 
         # terminate and wait for all solvers to exit
         terminate_workers_and_wait_for_exit(solvers)
 
         return solution
@@ -824,12 +824,12 @@
         )
     else:
         solution: POWSolution = solve_for_difficulty_fast( subtensor, wallet, output_in_place=output_in_place, \
             num_processes=num_processes, update_interval=update_interval, log_verbose=log_verbose
         )
 
     return None if solution is None else {
-        'nonce': solution.nonce, 
+        'nonce': solution.nonce,
         'difficulty': solution.difficulty,
-        'block_number': solution.block_number, 
+        'block_number': solution.block_number,
         'work': binascii.hexlify(solution.seal)
     }
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/utils/stats.py` & `bittensor-5.0.0/bittensor/utils/stats.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 """ A exponential moving average that updates values based on time since last update.
 """
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import time
 
 class timed_rolling_avg():
     """ A exponential moving average that updates values based on time since last update.
     """
     def __init__(self, initial_value, alpha):
         self.value = initial_value
         self.alpha = alpha
         self.last_update = time.time()
 
     def update(self, new_value):
-        """ Update self.value (the moving average) with the new_value 
+        """ Update self.value (the moving average) with the new_value
         """
         now = time.time()
         time_delta = now - self.last_update
         self.last_update = now
         new_value = new_value / time_delta
         self.value = (1 - self.alpha) * self.value + self.alpha * new_value
 
@@ -41,44 +41,44 @@
     """
     def __init__(self, initial_value=0, alpha=0.1):
         self.value = initial_value
         self.alpha = alpha
         self.last_update = None
 
     def event(self, amount):
-        """ Update self.value (the moving average) with the new_value 
+        """ Update self.value (the moving average) with the new_value
         """
         if self.last_update == None:
             self.last_update = time.time()
         else:
             now = time.time()
             time_delta = now - self.last_update
             self.last_update = now
             new_value = amount / time_delta
             self.value = (1 - self.alpha) * self.value + self.alpha * new_value
 
     def get(self) -> float:
         return float(self.value)
 
-        
+
 class EventsPerSecondRollingAverage():
     """ A exponential moving average that counts the number of events per second.
     """
     def __init__(self, initial_value, alpha):
         self.value = initial_value
         self.alpha = alpha
         self.last_update = None
 
     def event(self):
-        """ Update self.value (the moving average) with the new_value 
+        """ Update self.value (the moving average) with the new_value
         """
         if self.last_update == None:
             self.last_update = time.time()
         else:
             now = time.time()
             time_delta = now - self.last_update
             self.last_update = now
             new_value = 1 / time_delta
             self.value = (1 - self.alpha) * self.value + self.alpha * new_value
-    
+
     def get(self) -> float:
         return float(self.value)
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor/utils/test_utils.py` & `bittensor-5.0.0/bittensor/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post3/bittensor/utils/tokenizer_utils.py` & `bittensor-5.0.0/bittensor/utils/tokenizer_utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post3/bittensor/utils/weight_utils.py` & `bittensor-5.0.0/bittensor/utils/weight_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """ Conversion for weight between chain representation and torch tensor
 """
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import torch
 import bittensor
 from typing import Tuple, List
 
 U32_MAX = 4294967295
@@ -26,40 +26,40 @@
 
 def normalize_max_weight(  x: torch.FloatTensor, limit:float = 0.1 ) -> 'torch.FloatTensor':
     r""" Normalizes the tensor x so that sum(x) = 1 and the max value is not greater than the limit.
         Args:
             x (:obj:`torch.FloatTensor`):
                 Tensor to be max_value normalized.
             limit: float:
-                Max value after normalization.     
+                Max value after normalization.
         Returns:
             y (:obj:`torch.FloatTensor`):
                 Normalized x tensor.
     """
     epsilon = 1e-7 #For numerical stability after normalization
-    
+
     weights =  x.clone()
     values, _ = torch.sort(weights)
 
     if x.sum() == 0 or len(x)*limit <= 1:
         return torch.ones_like(x)/x.size(0)
     else:
         estimation = values/values.sum()
-        
+
         if estimation.max() <= limit:
             return weights/weights.sum()
 
         # Find the cumlative sum and sorted tensor
         cumsum = torch.cumsum(estimation,0)
 
         # Determine the index of cutoff
         estimation_sum = torch.tensor([(len(values)-i-1)*estimation[i] for i in range(len(values))])
         n_values = (estimation/(estimation_sum+cumsum+epsilon)<limit).sum()
 
-        # Determine the cutoff based on the index        
+        # Determine the cutoff based on the index
         cutoff_scale = (limit*cumsum[n_values-1]-epsilon)/(1-(limit*(len(estimation)-n_values)))
         cutoff= cutoff_scale*values.sum()
 
         # Applying the cutoff
         weights[weights > cutoff] = cutoff
 
         y = weights/weights.sum()
@@ -98,15 +98,15 @@
                 Tensor of bonds.
         Returns:
             row_bonds ( torch.FloatTensor ):
                 Converted row bonds.
     """
     row_bonds = torch.zeros( [ n ], dtype=torch.int64 )
     for uid_j, bij in list(zip( uids, bonds )):
-        row_bonds[ uid_j ] = int( bij ) 
+        row_bonds[ uid_j ] = int( bij )
     return row_bonds
 
 def convert_weights_and_uids_for_emit( uids: torch.LongTensor, weights: torch.FloatTensor ) -> Tuple[List[int], List[int]]:
     r""" Converts weights into integer u32 representation that sum to MAX_INT_WEIGHT.
         Args:
             uids (:obj:`torch.LongTensor,`):
                 Tensor of uids as destinations for passed weights.
@@ -137,59 +137,59 @@
     weight_uids = []
     for i, (weight_i, uid_i) in enumerate(list(zip(weights, uids))):
         uint16_val = round(float(weight_i) * int(U16_MAX))  # convert to int representation.
 
         # Filter zeros
         if uint16_val != 0: # Filter zeros
             weight_vals.append( uint16_val )
-            weight_uids.append( uid_i ) 
+            weight_uids.append( uid_i )
 
     return weight_uids, weight_vals
 
 
-def process_weights_for_netuid( 
+def process_weights_for_netuid(
         uids,
-        weights: torch.Tensor, 
-        netuid: int, 
-        subtensor: 'bittensor.subtensor', 
+        weights: torch.Tensor,
+        netuid: int,
+        subtensor: 'bittensor.subtensor',
         metagraph: 'bittensor.metagraph' = None,
     ) -> torch.FloatTensor:
     bittensor.logging.debug( 'process_weights_for_netuid()' )
     bittensor.logging.debug( 'weights', weights )
     bittensor.logging.debug( 'netuid', netuid )
     bittensor.logging.debug( 'subtensor', subtensor )
     bittensor.logging.debug( 'metagraph', metagraph )
 
     # Get latest metagraph from chain if metagraph is None.
     if metagraph == None:
         metagraph = subtensor.metagraph( netuid )
 
     # Cast weights to floats.
-    if not isinstance( weights, torch.FloatTensor ): 
+    if not isinstance( weights, torch.FloatTensor ):
         weights = weights.type( torch.float32 )
 
     # Network configuration parameters from an subtensor.
     # These parameters determine the range of acceptable weights for each neuron.
     quantile = subtensor.validator_exclude_quantile( netuid = netuid )
     min_allowed_weights = subtensor.min_allowed_weights( netuid = netuid )
-    max_weight_limit = subtensor.max_weight_limit( netuid = netuid ) 
+    max_weight_limit = subtensor.max_weight_limit( netuid = netuid )
     bittensor.logging.debug( 'quantile', quantile )
     bittensor.logging.debug( 'min_allowed_weights', min_allowed_weights )
     bittensor.logging.debug( 'max_weight_limit', max_weight_limit )
 
     # Find all non zero weights.
-    non_zero_weight_idx = torch.argwhere( weights > 0 ).squeeze( dim = 1 )  
+    non_zero_weight_idx = torch.argwhere( weights > 0 ).squeeze( dim = 1 )
     non_zero_weight_uids = uids[ non_zero_weight_idx ]
-    non_zero_weights = weights[ non_zero_weight_idx ]  
+    non_zero_weights = weights[ non_zero_weight_idx ]
     if non_zero_weights.numel() == 0 or metagraph.n < min_allowed_weights:
         bittensor.logging.warning( 'No non-zero weights returning all ones.' )
         final_weights = torch.ones( ( metagraph.n ) ) / metagraph.n
         bittensor.logging.debug( 'final_weights', final_weights )
         return torch.tensor( list( range( len( final_weights ) ) ) ), final_weights
-    
+
     elif non_zero_weights.numel() < min_allowed_weights:
         bittensor.logging.warning( 'No non-zero weights less then min allowed weight, returning all ones.' )
         # ( const ): Should this be torch.zeros( ( metagraph.n ) ) to reset everyone to build up weight?
         weights = torch.ones( ( metagraph.n ) ) * 1e-5 # creating minimum even non-zero weights
         weights[non_zero_weight_idx] += non_zero_weights
         bittensor.logging.debug( 'final_weights', weights )
         normalized_weights = bittensor.utils.weight_utils.normalize_max_weight(
@@ -197,24 +197,24 @@
             limit = max_weight_limit
         )
         return torch.tensor( list( range( len( normalized_weights ) ) ) ), normalized_weights
 
     bittensor.logging.debug( 'non_zero_weights', non_zero_weights )
 
     # Compute the exclude quantile and find the weights in the lowest quantile
-    max_exclude = max( 0,len( non_zero_weights ) - min_allowed_weights) / len( non_zero_weights )  
-    exclude_quantile = min([ quantile , max_exclude ]) 
-    lowest_quantile = non_zero_weights.quantile( exclude_quantile ) 
+    max_exclude = max( 0,len( non_zero_weights ) - min_allowed_weights) / len( non_zero_weights )
+    exclude_quantile = min([ quantile , max_exclude ])
+    lowest_quantile = non_zero_weights.quantile( exclude_quantile )
     bittensor.logging.debug( 'max_exclude', max_exclude )
-    bittensor.logging.debug( 'exclude_quantile', exclude_quantile )   
+    bittensor.logging.debug( 'exclude_quantile', exclude_quantile )
     bittensor.logging.debug( 'lowest_quantile', lowest_quantile )
 
     # Exclude all weights below the allowed quantile.
-    non_zero_weight_uids = non_zero_weight_uids[lowest_quantile <= non_zero_weights] 
-    non_zero_weights = non_zero_weights[ lowest_quantile <= non_zero_weights ] 
+    non_zero_weight_uids = non_zero_weight_uids[lowest_quantile <= non_zero_weights]
+    non_zero_weights = non_zero_weights[ lowest_quantile <= non_zero_weights ]
     bittensor.logging.debug( 'non_zero_weight_uids', non_zero_weight_uids )
     bittensor.logging.debug( 'non_zero_weights', non_zero_weights )
 
     # Normalize weights and return.
     normalized_weights = bittensor.utils.weight_utils.normalize_max_weight(
         x = non_zero_weights,
         limit = max_weight_limit
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor.egg-info/PKG-INFO` & `bittensor-5.0.0/bittensor.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,80 +1,15 @@
 Metadata-Version: 2.1
 Name: bittensor
-Version: 4.1.0rc1.post3
+Version: 5.0.0
 Summary: bittensor
 Home-page: https://github.com/opentensor/bittensor
 Author: bittensor.com
 Author-email: 
 License: MIT
-Description: <div align="center">
-        
-        # **Bittensor** <!-- omit in toc -->
-        [![Discord Chat](https://img.shields.io/discord/308323056592486420.svg)](https://discord.gg/bittensor)
-        [![PyPI version](https://badge.fury.io/py/bittensor.svg)](https://badge.fury.io/py/bittensor)
-        [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 
-        
-        ---
-        
-        ### Internet-scale Neural Networks <!-- omit in toc -->
-        
-        [Discord](https://discord.gg/bittensor) • [Network](https://taostats.io/) • [Research](https://drive.google.com/file/d/1VnsobL6lIAAqcA1_Tbm8AYIQscfJV4KU)
-        
-        </div>
-        
-        This repository contains Bittensor's Python API, which can be used for the following purposes:
-        
-        1. Querying the Bittensor network as a client.
-        2. Running and building Bittensor miners and validators.
-        3. Pulling network state information.
-        4. Managing TAO wallets, balances, transfers, etc.
-        
-        Bittensor is a mining network, similar to Bitcoin, that includes built-in incentives designed to encourage miners to provide value by hosting trained or training machine learning models. These models can be queried by clients seeking inference over inputs, such as token-based text generations or numerical embeddings from a large foundation model like GPT-NeoX-20B.
-        
-        Token-based incentives are designed to drive the network's growth and distribute the value generated by the network directly to the individuals producing that value, without intermediaries. The network is open to all participants, and no individual or group has full control over what is learned, who can profit from it, or who can access it.
-        
-        To learn more about Bittensor, please read our [paper](https://drive.google.com/file/d/1VnsobL6lIAAqcA1_Tbm8AYIQscfJV4KU/view).
-        
-        # Install
-        There are three ways to install Bittensor
-        
-        1. Through the installer:
-        ```
-        $ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/opentensor/bittensor/master/scripts/install.sh)"
-        ```
-        
-        2. With pip:
-        ```bash
-        $ pip3 install bittensor
-        ```
-        
-        3. From source:
-        ```
-        $ git clone https://github.com/opentensor/bittensor.git
-        $ python3 -m pip install -e bittensor/
-        ```
-        
-        ## Release
-        The release manager should follow the instructions of the [RELEASE_GUIDELINES.md](./RELEASE_GUIDELINES.md) document.
-        
-        ## License
-        The MIT License (MIT)
-        Copyright © 2021 Yuma Rao
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-        
-        
-        ## Acknowledgments
-        **learning-at-home/hivemind**
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -84,7 +19,72 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+<div align="center">
+
+# **Bittensor** <!-- omit in toc -->
+[![Discord Chat](https://img.shields.io/discord/308323056592486420.svg)](https://discord.gg/bittensor)
+[![PyPI version](https://badge.fury.io/py/bittensor.svg)](https://badge.fury.io/py/bittensor)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 
+
+---
+
+### Internet-scale Neural Networks <!-- omit in toc -->
+
+[Discord](https://discord.gg/bittensor) • [Network](https://taostats.io/) • [Research](https://drive.google.com/file/d/1VnsobL6lIAAqcA1_Tbm8AYIQscfJV4KU)
+
+</div>
+
+This repository contains Bittensor's Python API, which can be used for the following purposes:
+
+1. Querying the Bittensor network as a client.
+2. Running and building Bittensor miners and validators.
+3. Pulling network state information.
+4. Managing TAO wallets, balances, transfers, etc.
+
+Bittensor is a mining network, similar to Bitcoin, that includes built-in incentives designed to encourage miners to provide value by hosting trained or training machine learning models. These models can be queried by clients seeking inference over inputs, such as token-based text generations or numerical embeddings from a large foundation model like GPT-NeoX-20B.
+
+Token-based incentives are designed to drive the network's growth and distribute the value generated by the network directly to the individuals producing that value, without intermediaries. The network is open to all participants, and no individual or group has full control over what is learned, who can profit from it, or who can access it.
+
+To learn more about Bittensor, please read our [paper](https://drive.google.com/file/d/1VnsobL6lIAAqcA1_Tbm8AYIQscfJV4KU/view).
+
+# Install
+There are three ways to install Bittensor
+
+1. Through the installer:
+```
+$ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/opentensor/bittensor/master/scripts/install.sh)"
+```
+
+2. With pip:
+```bash
+$ pip3 install bittensor
+```
+
+3. From source:
+```
+$ git clone https://github.com/opentensor/bittensor.git
+$ python3 -m pip install -e bittensor/
+```
+
+## Release
+The release manager should follow the instructions of the [RELEASE_GUIDELINES.md](./RELEASE_GUIDELINES.md) document.
+
+## License
+The MIT License (MIT)
+Copyright © 2021 Yuma Rao
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
+
+## Acknowledgments
+**learning-at-home/hivemind**
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor.egg-info/SOURCES.txt` & `bittensor-5.0.0/bittensor.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 bittensor/_cli/commands/overview.py
 bittensor/_cli/commands/register.py
 bittensor/_cli/commands/stake.py
 bittensor/_cli/commands/transfer.py
 bittensor/_cli/commands/unstake.py
 bittensor/_cli/commands/utils.py
 bittensor/_cli/commands/wallets.py
-bittensor/_cli/commands/weights.py
 bittensor/_config/__init__.py
 bittensor/_config/config_impl.py
 bittensor/_dataset/__init__.py
 bittensor/_dataset/dataset_impl.py
 bittensor/_dataset/dataset_mock.py
 bittensor/_dataset/thread_queue.py
 bittensor/_dendrite/__init__.py
```

### Comparing `bittensor-4.1.0rc1.post3/bittensor.egg-info/requires.txt` & `bittensor-5.0.0/bittensor.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-ansible_vault>=2.1
 argparse==1.4.0
-backoff==2.1.0
 base58==2.0.1
+backoff==2.1.0
 certifi==2020.11.8
 cryptography==39.0.0
-datasets==2.12.0
+idna==2.10
+jinja2==3.0
 fuzzywuzzy==0.18.0
 google-api-python-client==2.7.0
-grpcio-tools==1.42.0
+python-levenshtein==0.12.1
 grpcio==1.42.0
+grpcio-tools==1.42.0
 hypothesis==6.47.4
-idna==2.10
-jinja2==3.0
-jsonschema[format-nongpl]<=4.17.0,>=4.14.0
-langchain>=0.0.132
 loguru==0.6.0
-markupsafe==2.0.1
-miniupnpc==2.0.2
-msgpack-numpy==0.4.7.1
 msgpack==1.0.4
+msgpack-numpy==0.4.7.1
+miniupnpc==2.0.2
 munch==2.5.0
 nest_asyncio==1.5.6
 netaddr==0.8.0
-numpy==1.21.6
 pandas==1.5.2
+psutil==5.9.4
 password_strength==0.0.3.post2
-prometheus_client==0.14.1
 protobuf==3.19.5
-psutil==5.9.4
-py-bip39-bindings<1,>=0.1.9
-py-ed25519-bindings<2,>=1.0
-py-sr25519-bindings<1,>=0.1.4
+prometheus_client==0.14.1
 pycryptodome==3.11.0
-python-levenshtein==0.12.1
+py-sr25519-bindings<1,>=0.1.4
+py-ed25519-bindings<2,>=1.0
+py-bip39-bindings<1,>=0.1.9
 pyyaml==6.0
-qqdm==0.0.7
-requests==2.25.0
-retry==0.9.2
 rich==12.5.1
+retry==0.9.2
+requests==2.25.0
 scalecodec==1.2.0
 sentencepiece==0.1.97
-substrate-interface==1.5.0
 termcolor==2.1.1
 torch==1.13.1
-tqdm==4.64.1
 transformers>=4.20.1
+numpy==1.21.6
 wheel==0.37.1
+tqdm==4.64.1
+qqdm==0.0.7
+ansible_vault>=2.1
+substrate-interface==1.5.0
+jsonschema[format-nongpl]<=4.17.0,>=4.14.0
+markupsafe==2.0.1
+langchain>=0.0.132
+datasets==2.12.0
 
 [dev]
-coveralls==3.3.1
-ddt==1.6.0
-pytest-cov==4.0.0
-pytest-rerunfailures==10.2
+pytest==7.2.0
 pytest-split==0.8.0
 pytest-xdist==3.0.2
-pytest==7.2.0
+pytest-rerunfailures==10.2
+coveralls==3.3.1
+pytest-cov==4.0.0
+ddt==1.6.0
```

### Comparing `bittensor-4.1.0rc1.post3/setup.py` & `bittensor-5.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
-# documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
-# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+# THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+# OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 from setuptools import setup, find_packages
 from pkg_resources import parse_requirements
 from os import path
 from io import open
 import codecs
```

