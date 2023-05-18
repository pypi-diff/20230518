# Comparing `tmp/vega_sim-0.67.0.tar.gz` & `tmp/vega_sim-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vega_sim-0.67.0.tar", max compression
+gzip compressed data, was "vega_sim-1.0.1.tar", max compression
```

## Comparing `vega_sim-0.67.0.tar` & `vega_sim-1.0.1.tar`

### file list

```diff
@@ -1,201 +1,200 @@
--rw-r--r--   0        0        0     1061 2023-01-18 18:32:34.428593 vega_sim-0.67.0/LICENSE
--rw-r--r--   0        0        0     1513 2023-01-18 18:32:34.504598 vega_sim-0.67.0/pyproject.toml
--rw-r--r--   0        0        0      201 2023-01-18 18:32:34.508598 vega_sim-0.67.0/vega_sim/__init__.py
--rw-r--r--   0        0        0        0 2023-01-18 18:32:34.508598 vega_sim-0.67.0/vega_sim/api/__init__.py
--rw-r--r--   0        0        0    42705 2023-01-18 18:32:34.508598 vega_sim-0.67.0/vega_sim/api/data.py
--rw-r--r--   0        0        0    18457 2023-01-18 18:32:34.508598 vega_sim-0.67.0/vega_sim/api/data_raw.py
--rw-r--r--   0        0        0      548 2023-01-18 18:32:34.508598 vega_sim-0.67.0/vega_sim/api/faucet.py
--rw-r--r--   0        0        0    20026 2023-01-18 18:32:34.508598 vega_sim-0.67.0/vega_sim/api/governance.py
--rw-r--r--   0        0        0     4806 2023-01-18 18:32:34.508598 vega_sim-0.67.0/vega_sim/api/helpers.py
--rw-r--r--   0        0        0    12265 2023-01-18 18:32:34.508598 vega_sim-0.67.0/vega_sim/api/market.py
--rw-r--r--   0        0        0    21610 2023-01-18 18:32:34.508598 vega_sim-0.67.0/vega_sim/api/trading.py
--rw-r--r--   0        0        0      122 2023-01-18 18:32:34.508598 vega_sim-0.67.0/vega_sim/constants.py
--rw-r--r--   0        0        0       48 2023-01-18 18:32:34.508598 vega_sim-0.67.0/vega_sim/environment/__init__.py
--rw-r--r--   0        0        0     2912 2023-01-18 18:32:34.508598 vega_sim-0.67.0/vega_sim/environment/agent.py
--rw-r--r--   0        0        0    17598 2023-01-18 18:32:34.508598 vega_sim-0.67.0/vega_sim/environment/environment.py
--rw-r--r--   0        0        0        0 2023-01-18 18:32:34.508598 vega_sim-0.67.0/vega_sim/grpc/__init__.py
--rw-r--r--   0        0        0     1287 2023-01-18 18:32:34.508598 vega_sim-0.67.0/vega_sim/grpc/client.py
--rw-r--r--   0        0        0    15115 2023-01-18 18:32:34.508598 vega_sim-0.67.0/vega_sim/network_service.py
--rw-r--r--   0        0        0    23584 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/null_service.py
--rw-r--r--   0        0        0        0 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/parameter_test/__init__.py
--rw-r--r--   0        0        0        0 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/parameter_test/parameter/__init__.py
--rw-r--r--   0        0        0     3024 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/parameter_test/parameter/configs.py
--rw-r--r--   0        0        0     6666 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/parameter_test/parameter/experiment.py
--rw-r--r--   0        0        0    12833 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/parameter_test/parameter/loggers.py
--rw-r--r--   0        0        0      636 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/parameter_test/run.py
--rw-r--r--   0        0        0       63 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/__init__.py
--rw-r--r--   0        0        0     4736 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/blockexplorer/blockexplorer_pb2.py
--rw-r--r--   0        0        0     6533 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/blockexplorer/blockexplorer_pb2_grpc.py
--rw-r--r--   0        0        0       37 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/data_node/__init__.py
--rw-r--r--   0        0        0       35 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/data_node/api/__init__.py
--rw-r--r--   0        0        0      164 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/data_node/api/v2/__init__.py
--rw-r--r--   0        0        0    91412 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/data_node/api/v2/trading_data_pb2.py
--rw-r--r--   0        0        0   165777 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/data_node/api/v2/trading_data_pb2_grpc.py
--rw-r--r--   0        0        0     1075 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/vega/__init__.py
--rw-r--r--   0        0        0       35 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/vega/api/__init__.py
--rw-r--r--   0        0        0      247 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/vega/api/v1/__init__.py
--rw-r--r--   0        0        0    14310 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/vega/api/v1/core_pb2.py
--rw-r--r--   0        0        0    18874 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/vega/api/v1/core_pb2_grpc.py
--rw-r--r--   0        0        0     8685 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/vega/api/v1/corestate_pb2.py
--rw-r--r--   0        0        0    22498 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/vega/api/v1/corestate_pb2_grpc.py
--rw-r--r--   0        0        0     3114 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/vega/assets_pb2.py
--rw-r--r--   0        0        0      158 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/vega/assets_pb2_grpc.py
--rw-r--r--   0        0        0     7056 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/vega/chain_events_pb2.py
--rw-r--r--   0        0        0      158 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/vega/chain_events_pb2_grpc.py
--rw-r--r--   0        0        0       35 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/vega/checkpoint/__init__.py
--rw-r--r--   0        0        0      152 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/vega/checkpoint/v1/__init__.py
--rw-r--r--   0        0        0    10934 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/vega/checkpoint/v1/checkpoint_pb2.py
--rw-r--r--   0        0        0      158 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/vega/checkpoint/v1/checkpoint_pb2_grpc.py
--rw-r--r--   0        0        0       35 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/vega/commands/__init__.py
--rw-r--r--   0        0        0      700 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/vega/commands/v1/__init__.py
--rw-r--r--   0        0        0     7606 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/vega/commands/v1/commands_pb2.py
--rw-r--r--   0        0        0      158 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/vega/commands/v1/commands_pb2_grpc.py
--rw-r--r--   0        0        0     1624 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/vega/commands/v1/data_pb2.py
--rw-r--r--   0        0        0      158 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/vega/commands/v1/data_pb2_grpc.py
--rw-r--r--   0        0        0     1297 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/vega/commands/v1/signature_pb2.py
--rw-r--r--   0        0        0      158 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/vega/commands/v1/signature_pb2_grpc.py
--rw-r--r--   0        0        0     5944 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/vega/commands/v1/transaction_pb2.py
--rw-r--r--   0        0        0      158 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/vega/commands/v1/transaction_pb2_grpc.py
--rw-r--r--   0        0        0     6658 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/vega/commands/v1/validator_commands_pb2.py
--rw-r--r--   0        0        0      158 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/vega/commands/v1/validator_commands_pb2_grpc.py
--rw-r--r--   0        0        0       35 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/vega/data/__init__.py
--rw-r--r--   0        0        0      217 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/vega/data/v1/__init__.py
--rw-r--r--   0        0        0     2449 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/vega/data/v1/data_pb2.py
--rw-r--r--   0        0        0      158 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/vega/data/v1/data_pb2_grpc.py
--rw-r--r--   0        0        0     2569 2023-01-18 18:32:34.512598 vega_sim-0.67.0/vega_sim/proto/vega/data/v1/spec_pb2.py
--rw-r--r--   0        0        0      158 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/proto/vega/data/v1/spec_pb2_grpc.py
--rw-r--r--   0        0        0     3491 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/proto/vega/data_source_pb2.py
--rw-r--r--   0        0        0      158 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/proto/vega/data_source_pb2_grpc.py
--rw-r--r--   0        0        0       35 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/proto/vega/events/__init__.py
--rw-r--r--   0        0        0      128 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/proto/vega/events/v1/__init__.py
--rw-r--r--   0        0        0    32800 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/proto/vega/events/v1/events_pb2.py
--rw-r--r--   0        0        0      158 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/proto/vega/events/v1/events_pb2_grpc.py
--rw-r--r--   0        0        0    13029 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/proto/vega/governance_pb2.py
--rw-r--r--   0        0        0      158 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/proto/vega/governance_pb2_grpc.py
--rw-r--r--   0        0        0     9271 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/proto/vega/markets_pb2.py
--rw-r--r--   0        0        0      158 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/proto/vega/markets_pb2_grpc.py
--rw-r--r--   0        0        0     1560 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/proto/vega/oracle_pb2.py
--rw-r--r--   0        0        0      158 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/proto/vega/oracle_pb2_grpc.py
--rw-r--r--   0        0        0       35 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/proto/vega/snapshot/__init__.py
--rw-r--r--   0        0        0      140 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/proto/vega/snapshot/v1/__init__.py
--rw-r--r--   0        0        0    48155 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/proto/vega/snapshot/v1/snapshot_pb2.py
--rw-r--r--   0        0        0      158 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/proto/vega/snapshot/v1/snapshot_pb2_grpc.py
--rw-r--r--   0        0        0    37238 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/proto/vega/vega_pb2.py
--rw-r--r--   0        0        0      158 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/proto/vega/vega_pb2_grpc.py
--rw-r--r--   0        0        0       35 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/proto/vega/wallet/__init__.py
--rw-r--r--   0        0        0      128 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/proto/vega/wallet/v1/__init__.py
--rw-r--r--   0        0        0     4847 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/proto/vega/wallet/v1/wallet_pb2.py
--rw-r--r--   0        0        0      158 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/proto/vega/wallet/v1/wallet_pb2_grpc.py
--rw-r--r--   0        0        0        0 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/quant/__init__.py
--rw-r--r--   0        0        0     2961 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/quant/quant.py
--rw-r--r--   0        0        0       29 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/reinforcement/.gitignore
--rw-r--r--   0        0        0        0 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/reinforcement/__init__.py
--rw-r--r--   0        0        0        0 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/reinforcement/agents/__init__.py
--rw-r--r--   0        0        0     8337 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/reinforcement/agents/learning_agent.py
--rw-r--r--   0        0        0    13518 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/reinforcement/agents/learning_agent_MO.py
--rw-r--r--   0        0        0    19063 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/reinforcement/agents/learning_agent_MO_with_vol.py
--rw-r--r--   0        0        0    13097 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/reinforcement/agents/learning_agent_heuristic.py
--rw-r--r--   0        0        0     4757 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/reinforcement/agents/simple_agent.py
--rw-r--r--   0        0        0      925 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/reinforcement/distributions.py
--rw-r--r--   0        0        0        0 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/reinforcement/full_market_sim/__init__.py
--rw-r--r--   0        0        0      608 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/reinforcement/full_market_sim/environments.py
--rw-r--r--   0        0        0        0 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/reinforcement/full_market_sim/utils/__init__.py
--rw-r--r--   0        0        0     4458 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/reinforcement/full_market_sim/utils/create_csv.py
--rw-r--r--   0        0        0     1932 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/reinforcement/full_market_sim/utils/external_assetprice.py
--rw-r--r--   0        0        0     4782 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/reinforcement/full_market_sim/utils/logdata.py
--rw-r--r--   0        0        0     4810 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/reinforcement/full_market_sim/utils/strategy.py
--rw-r--r--   0        0        0      662 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/reinforcement/helpers.py
--rw-r--r--   0        0        0     2996 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/reinforcement/la_market_state.py
--rw-r--r--   0        0        0     4244 2023-01-18 18:32:34.516598 vega_sim-0.67.0/vega_sim/reinforcement/networks.py
--rw-r--r--   0        0        0     4016 2023-01-18 18:32:34.520599 vega_sim-0.67.0/vega_sim/reinforcement/plot.py
--rw-r--r--   0        0        0     8917 2023-01-18 18:32:34.520599 vega_sim-0.67.0/vega_sim/reinforcement/run_rl_agent.py
--rw-r--r--   0        0        0     2446 2023-01-18 18:32:34.520599 vega_sim-0.67.0/vega_sim/reinforcement/run_simple_agent.py
--rw-r--r--   0        0        0      505 2023-01-18 18:32:34.520599 vega_sim-0.67.0/vega_sim/reinforcement/theory_intro/Bibliography.bib
--rw-r--r--   0        0        0    13970 2023-01-18 18:32:34.520599 vega_sim-0.67.0/vega_sim/reinforcement/theory_intro/RL.tex
--rw-r--r--   0        0        0    36669 2023-01-18 18:32:34.520599 vega_sim-0.67.0/vega_sim/reinforcement/theory_intro/images/RL.png
--rw-r--r--   0        0        0    29521 2023-01-18 18:32:34.520599 vega_sim-0.67.0/vega_sim/reinforcement/theory_intro/images/RL_inv.png
--rw-r--r--   0        0        0    39266 2023-01-18 18:32:34.520599 vega_sim-0.67.0/vega_sim/reinforcement/theory_intro/images/logo.png
--rw-r--r--   0        0        0    52831 2023-01-18 18:32:34.520599 vega_sim-0.67.0/vega_sim/reinforcement/theory_intro/images/logo_inv.png
--rw-r--r--   0        0        0        0 2023-01-18 18:32:34.520599 vega_sim-0.67.0/vega_sim/replay/__init__.py
--rw-r--r--   0        0        0     1386 2023-01-18 18:32:34.520599 vega_sim-0.67.0/vega_sim/replay/replay.py
--rw-r--r--   0        0        0        0 2023-01-18 18:32:34.520599 vega_sim-0.67.0/vega_sim/scenario/__init__.py
--rw-r--r--   0        0        0     2372 2023-01-18 18:32:34.520599 vega_sim-0.67.0/vega_sim/scenario/adhoc.py
--rw-r--r--   0        0        0        0 2023-01-18 18:32:34.520599 vega_sim-0.67.0/vega_sim/scenario/common/__init__.py
--rw-r--r--   0        0        0    94738 2023-01-18 18:32:34.520599 vega_sim-0.67.0/vega_sim/scenario/common/agents.py
--rw-r--r--   0        0        0     7797 2023-01-18 18:32:34.520599 vega_sim-0.67.0/vega_sim/scenario/common/utils/ideal_mm_models.py
--rw-r--r--   0        0        0     5680 2023-01-18 18:32:34.520599 vega_sim-0.67.0/vega_sim/scenario/common/utils/price_process.py
--rw-r--r--   0        0        0      779 2023-01-18 18:32:34.520599 vega_sim-0.67.0/vega_sim/scenario/comprehensive_market/agents.py
--rw-r--r--   0        0        0    13045 2023-01-18 18:32:34.520599 vega_sim-0.67.0/vega_sim/scenario/comprehensive_market/scenario.py
--rw-r--r--   0        0        0     5408 2023-01-18 18:32:34.520599 vega_sim-0.67.0/vega_sim/scenario/configurable_market/agents.py
--rw-r--r--   0        0        0     8649 2023-01-18 18:32:34.520599 vega_sim-0.67.0/vega_sim/scenario/configurable_market/scenario.py
--rw-r--r--   0        0        0      238 2023-01-18 18:32:34.520599 vega_sim-0.67.0/vega_sim/scenario/constants.py
--rw-r--r--   0        0        0        0 2023-01-18 18:32:34.520599 vega_sim-0.67.0/vega_sim/scenario/curve_market_maker/__init__.py
--rw-r--r--   0        0        0    11394 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/scenario/curve_market_maker/scenario.py
--rw-r--r--   0        0        0        0 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/scenario/hedged_market_maker/__init__.py
--rw-r--r--   0        0        0      827 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/scenario/hedged_market_maker/agents.py
--rw-r--r--   0        0        0    19200 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/scenario/hedged_market_maker/scenario.py
--rw-r--r--   0        0        0        0 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/scenario/ideal_market_maker/__init__.py
--rw-r--r--   0        0        0    31546 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/scenario/ideal_market_maker/agents.py
--rw-r--r--   0        0        0     3160 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/scenario/ideal_market_maker/environments.py
--rw-r--r--   0        0        0     8680 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/scenario/ideal_market_maker/scenario.py
--rw-r--r--   0        0        0        0 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/scenario/ideal_market_maker/utils/__init__.py
--rw-r--r--   0        0        0     4782 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/scenario/ideal_market_maker/utils/log_data.py
--rw-r--r--   0        0        0     4819 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/scenario/ideal_market_maker/utils/strategy.py
--rw-r--r--   0        0        0        0 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/scenario/ideal_market_maker_v2/__init__.py
--rw-r--r--   0        0        0    11501 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/scenario/ideal_market_maker_v2/agents.py
--rw-r--r--   0        0        0     9917 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/scenario/ideal_market_maker_v2/scenario.py
--rw-r--r--   0        0        0        0 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/scenario/ideal_market_maker_v2/utils/__init__.py
--rw-r--r--   0        0        0     4819 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/scenario/ideal_market_maker_v2/utils/strategy.py
--rw-r--r--   0        0        0     1687 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/scenario/market_crash/price_process.py
--rw-r--r--   0        0        0     9790 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/scenario/market_crash/scenario.py
--rw-r--r--   0        0        0     2091 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/scenario/multi_market/agents.py
--rw-r--r--   0        0        0    21436 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/scenario/multi_market/scenario.py
--rw-r--r--   0        0        0     9608 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/scenario/parameter_experiment/scenario.py
--rw-r--r--   0        0        0     6749 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/scenario/registry.py
--rw-r--r--   0        0        0     2976 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/scenario/scenario.py
--rw-r--r--   0        0        0    82885 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/service.py
--rw-r--r--   0        0        0        0 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/tools/__init__.py
--rw-r--r--   0        0        0     7082 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/tools/scenario_output.py
--rw-r--r--   0        0        0     5728 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/tools/scenario_plots.py
--rw-r--r--   0        0        0     7148 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/vegahome/config/data-node/config.toml
--rw-r--r--   0        0        0      277 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/vegahome/config/faucet/config.toml
--rw-r--r--   0        0        0     3968 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/vegahome/config/node/config.toml
--rw-r--r--   0        0        0      312 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/vegahome/config/node/wallets.encrypted
--rw-r--r--   0        0        0      321 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/vegahome/config/wallet-service/networks/local.toml
--rw-r--r--   0        0        0      586 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/vegahome/data/faucet/wallets/vega.1639051237294446827
--rw-r--r--   0        0        0      586 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/vegahome/data/faucet/wallets/vega.1641976836892788243
--rw-r--r--   0        0        0      586 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977214518086643
--rw-r--r--   0        0        0      586 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977270881740938
--rw-r--r--   0        0        0      586 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977376563008654
--rw-r--r--   0        0        0      586 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977471442889253
--rw-r--r--   0        0        0      586 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977537535784009
--rw-r--r--   0        0        0      586 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977956797580358
--rw-r--r--   0        0        0      586 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/vegahome/data/faucet/wallets/vega.1641978034856367487
--rw-r--r--   0        0        0      586 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/vegahome/data/faucet/wallets/vega.1643100690865690276
--rw-r--r--   0        0        0      491 2023-01-18 18:32:34.524599 vega_sim-0.67.0/vega_sim/vegahome/data/node/wallets/ethereum/UTC--2021-12-09T12-00-28.751280926Z--b6ea7744971f455bbd754a97e8e05ea13dc1a033
--rw-r--r--   0        0        0      491 2023-01-18 18:32:34.528599 vega_sim-0.67.0/vega_sim/vegahome/data/node/wallets/ethereum/UTC--2022-01-12T08-54-28.446104867Z--d1b7ef68bb457b47837c6e81da24455be7a8be0d
--rw-r--r--   0        0        0      491 2023-01-18 18:32:34.528599 vega_sim-0.67.0/vega_sim/vegahome/data/node/wallets/ethereum/UTC--2022-01-12T08-57-18.522457076Z--dc699ecdab1705ebe83b60345060b6b7620263a3
--rw-r--r--   0        0        0      491 2023-01-18 18:32:34.528599 vega_sim-0.67.0/vega_sim/vegahome/data/node/wallets/ethereum/UTC--2022-01-12T08-58-36.643184436Z--760895ae7f813d685b048336fac88625441d6aa7
--rw-r--r--   0        0        0      491 2023-01-18 18:32:34.528599 vega_sim-0.67.0/vega_sim/vegahome/data/node/wallets/ethereum/UTC--2022-01-12T08-59-08.359696969Z--9e5beec6e56b28ccbd02864840b0f1e0125e42ce
--rw-r--r--   0        0        0      586 2023-01-18 18:32:34.528599 vega_sim-0.67.0/vega_sim/vegahome/data/node/wallets/vega/vega.1639051228296308758
--rw-r--r--   0        0        0      586 2023-01-18 18:32:34.528599 vega_sim-0.67.0/vega_sim/vegahome/data/node/wallets/vega/vega.1641977668033624243
--rw-r--r--   0        0        0      586 2023-01-18 18:32:34.528599 vega_sim-0.67.0/vega_sim/vegahome/data/node/wallets/vega/vega.1641977838095755067
--rw-r--r--   0        0        0      586 2023-01-18 18:32:34.528599 vega_sim-0.67.0/vega_sim/vegahome/data/node/wallets/vega/vega.1641977916225009082
--rw-r--r--   0        0        0      586 2023-01-18 18:32:34.528599 vega_sim-0.67.0/vega_sim/vegahome/data/node/wallets/vega/vega.1641977947934016124
--rw-r--r--   0        0        0       46 2023-01-18 18:32:34.528599 vega_sim-0.67.0/vega_sim/vegahome/data/priv_validator_state.json
--rw-r--r--   0        0        0     3243 2023-01-18 18:32:34.528599 vega_sim-0.67.0/vega_sim/vegahome/data/wallet-service/rsa-keys/private.pem
--rw-r--r--   0        0        0      800 2023-01-18 18:32:34.528599 vega_sim-0.67.0/vega_sim/vegahome/data/wallet-service/rsa-keys/public.pem
--rwxr-xr-x   0        0        0      621 2023-01-18 18:32:34.528599 vega_sim-0.67.0/vega_sim/vegahome/data/wallets/1RkMQOfoswtvmoiXrL1U
--rw-r--r--   0        0        0      609 2023-01-18 18:32:34.528599 vega_sim-0.67.0/vega_sim/vegahome/data/wallets/AcZ6sIcH
--rw-r--r--   0        0        0      621 2023-01-18 18:32:34.528599 vega_sim-0.67.0/vega_sim/vegahome/data/wallets/lLK8PvgpGBOwap3v1DdY
--rw-r--r--   0        0        0      609 2023-01-18 18:32:34.528599 vega_sim-0.67.0/vega_sim/vegahome/data/wallets/oq8YJHWE
--rwxr-xr-x   0        0        0      621 2023-01-18 18:32:34.528599 vega_sim-0.67.0/vega_sim/vegahome/data/wallets/xztnaIYwkocQNKbm5zG0
--rwxr-xr-x   0        0        0      621 2023-01-18 18:32:34.528599 vega_sim-0.67.0/vega_sim/vegahome/data/wallets/yxuEAf5rJFFgsNv5dCGn
--rw-r--r--   0        0        0     7023 2023-01-18 18:32:34.528599 vega_sim-0.67.0/vega_sim/vegahome/genesis.json
--rw-r--r--   0        0        0        3 2023-01-18 18:32:34.528599 vega_sim-0.67.0/vega_sim/vegahome/passphrase-file
--rw-r--r--   0        0        0        0 2023-01-18 18:32:34.528599 vega_sim-0.67.0/vega_sim/wallet/__init__.py
--rw-r--r--   0        0        0     1724 2023-01-18 18:32:34.528599 vega_sim-0.67.0/vega_sim/wallet/base.py
--rw-r--r--   0        0        0     7615 2023-01-18 18:32:34.528599 vega_sim-0.67.0/vega_sim/wallet/slim_wallet.py
--rw-r--r--   0        0        0     5974 2023-01-18 18:32:34.528599 vega_sim-0.67.0/vega_sim/wallet/vega_wallet.py
--rw-r--r--   0        0        0     3543 1970-01-01 00:00:00.000000 vega_sim-0.67.0/setup.py
--rw-r--r--   0        0        0     1632 1970-01-01 00:00:00.000000 vega_sim-0.67.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-02-24 15:57:56.653695 vega_sim-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1516 2023-02-24 15:57:56.717695 vega_sim-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      224 2023-02-24 15:57:56.721695 vega_sim-1.0.1/vega_sim/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-24 15:57:56.721695 vega_sim-1.0.1/vega_sim/api/__init__.py
+-rw-r--r--   0        0        0    43662 2023-02-24 15:57:56.721695 vega_sim-1.0.1/vega_sim/api/data.py
+-rw-r--r--   0        0        0    19960 2023-02-24 15:57:56.721695 vega_sim-1.0.1/vega_sim/api/data_raw.py
+-rw-r--r--   0        0        0      548 2023-02-24 15:57:56.721695 vega_sim-1.0.1/vega_sim/api/faucet.py
+-rw-r--r--   0        0        0    20160 2023-02-24 15:57:56.721695 vega_sim-1.0.1/vega_sim/api/governance.py
+-rw-r--r--   0        0        0     4806 2023-02-24 15:57:56.721695 vega_sim-1.0.1/vega_sim/api/helpers.py
+-rw-r--r--   0        0        0    12265 2023-02-24 15:57:56.721695 vega_sim-1.0.1/vega_sim/api/market.py
+-rw-r--r--   0        0        0    21663 2023-02-24 15:57:56.721695 vega_sim-1.0.1/vega_sim/api/trading.py
+-rw-r--r--   0        0        0      122 2023-02-24 15:57:56.721695 vega_sim-1.0.1/vega_sim/constants.py
+-rw-r--r--   0        0        0       48 2023-02-24 15:57:56.721695 vega_sim-1.0.1/vega_sim/environment/__init__.py
+-rw-r--r--   0        0        0     2609 2023-02-24 15:57:56.721695 vega_sim-1.0.1/vega_sim/environment/agent.py
+-rw-r--r--   0        0        0    23928 2023-02-24 15:57:56.721695 vega_sim-1.0.1/vega_sim/environment/environment.py
+-rw-r--r--   0        0        0        0 2023-02-24 15:57:56.721695 vega_sim-1.0.1/vega_sim/grpc/__init__.py
+-rw-r--r--   0        0        0     1287 2023-02-24 15:57:56.721695 vega_sim-1.0.1/vega_sim/grpc/client.py
+-rw-r--r--   0        0        0    15886 2023-02-24 15:57:56.721695 vega_sim-1.0.1/vega_sim/local_data_cache.py
+-rw-r--r--   0        0        0    17839 2023-02-24 15:57:56.721695 vega_sim-1.0.1/vega_sim/network_service.py
+-rw-r--r--   0        0        0    25761 2023-02-24 15:57:56.721695 vega_sim-1.0.1/vega_sim/null_service.py
+-rw-r--r--   0        0        0        0 2023-02-24 15:57:56.721695 vega_sim-1.0.1/vega_sim/parameter_test/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-24 15:57:56.721695 vega_sim-1.0.1/vega_sim/parameter_test/parameter/__init__.py
+-rw-r--r--   0        0        0     3026 2023-02-24 15:57:56.721695 vega_sim-1.0.1/vega_sim/parameter_test/parameter/configs.py
+-rw-r--r--   0        0        0     6665 2023-02-24 15:57:56.721695 vega_sim-1.0.1/vega_sim/parameter_test/parameter/experiment.py
+-rw-r--r--   0        0        0    13545 2023-02-24 15:57:56.721695 vega_sim-1.0.1/vega_sim/parameter_test/parameter/loggers.py
+-rw-r--r--   0        0        0      636 2023-02-24 15:57:56.721695 vega_sim-1.0.1/vega_sim/parameter_test/run.py
+-rw-r--r--   0        0        0       63 2023-02-24 15:57:56.721695 vega_sim-1.0.1/vega_sim/proto/__init__.py
+-rw-r--r--   0        0        0     4747 2023-02-24 15:57:56.721695 vega_sim-1.0.1/vega_sim/proto/blockexplorer/blockexplorer_pb2.py
+-rw-r--r--   0        0        0     6533 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/blockexplorer/blockexplorer_pb2_grpc.py
+-rw-r--r--   0        0        0       37 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/data_node/__init__.py
+-rw-r--r--   0        0        0       35 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/data_node/api/__init__.py
+-rw-r--r--   0        0        0      164 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/data_node/api/v2/__init__.py
+-rw-r--r--   0        0        0    94610 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/data_node/api/v2/trading_data_pb2.py
+-rw-r--r--   0        0        0   171942 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/data_node/api/v2/trading_data_pb2_grpc.py
+-rw-r--r--   0        0        0     1075 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/__init__.py
+-rw-r--r--   0        0        0       35 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/api/__init__.py
+-rw-r--r--   0        0        0      247 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/api/v1/__init__.py
+-rw-r--r--   0        0        0    14923 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/api/v1/core_pb2.py
+-rw-r--r--   0        0        0    18874 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/api/v1/core_pb2_grpc.py
+-rw-r--r--   0        0        0     8686 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/api/v1/corestate_pb2.py
+-rw-r--r--   0        0        0    22499 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/api/v1/corestate_pb2_grpc.py
+-rw-r--r--   0        0        0     3113 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/assets_pb2.py
+-rw-r--r--   0        0        0      158 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/assets_pb2_grpc.py
+-rw-r--r--   0        0        0     7055 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/chain_events_pb2.py
+-rw-r--r--   0        0        0      158 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/chain_events_pb2_grpc.py
+-rw-r--r--   0        0        0       35 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/checkpoint/__init__.py
+-rw-r--r--   0        0        0      152 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/checkpoint/v1/__init__.py
+-rw-r--r--   0        0        0    10933 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/checkpoint/v1/checkpoint_pb2.py
+-rw-r--r--   0        0        0      158 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/checkpoint/v1/checkpoint_pb2_grpc.py
+-rw-r--r--   0        0        0       35 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/commands/__init__.py
+-rw-r--r--   0        0        0      700 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/commands/v1/__init__.py
+-rw-r--r--   0        0        0     8086 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/commands/v1/commands_pb2.py
+-rw-r--r--   0        0        0      158 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/commands/v1/commands_pb2_grpc.py
+-rw-r--r--   0        0        0     1623 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/commands/v1/data_pb2.py
+-rw-r--r--   0        0        0      158 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/commands/v1/data_pb2_grpc.py
+-rw-r--r--   0        0        0     1296 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/commands/v1/signature_pb2.py
+-rw-r--r--   0        0        0      158 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/commands/v1/signature_pb2_grpc.py
+-rw-r--r--   0        0        0     5943 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/commands/v1/transaction_pb2.py
+-rw-r--r--   0        0        0      158 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/commands/v1/transaction_pb2_grpc.py
+-rw-r--r--   0        0        0     6339 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/commands/v1/validator_commands_pb2.py
+-rw-r--r--   0        0        0      158 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/commands/v1/validator_commands_pb2_grpc.py
+-rw-r--r--   0        0        0       35 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/data/__init__.py
+-rw-r--r--   0        0        0      217 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/data/v1/__init__.py
+-rw-r--r--   0        0        0     2448 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/data/v1/data_pb2.py
+-rw-r--r--   0        0        0      158 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/data/v1/data_pb2_grpc.py
+-rw-r--r--   0        0        0     2568 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/data/v1/spec_pb2.py
+-rw-r--r--   0        0        0      158 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/data/v1/spec_pb2_grpc.py
+-rw-r--r--   0        0        0     3490 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/data_source_pb2.py
+-rw-r--r--   0        0        0      158 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0       35 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/events/__init__.py
+-rw-r--r--   0        0        0      128 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/events/v1/__init__.py
+-rw-r--r--   0        0        0    33189 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/events/v1/events_pb2.py
+-rw-r--r--   0        0        0      158 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/events/v1/events_pb2_grpc.py
+-rw-r--r--   0        0        0    13475 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/governance_pb2.py
+-rw-r--r--   0        0        0      158 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/governance_pb2_grpc.py
+-rw-r--r--   0        0        0     9423 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/markets_pb2.py
+-rw-r--r--   0        0        0      158 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/markets_pb2_grpc.py
+-rw-r--r--   0        0        0     1559 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/oracle_pb2.py
+-rw-r--r--   0        0        0      158 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/oracle_pb2_grpc.py
+-rw-r--r--   0        0        0       35 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/snapshot/__init__.py
+-rw-r--r--   0        0        0      140 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/snapshot/v1/__init__.py
+-rw-r--r--   0        0        0    48154 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/snapshot/v1/snapshot_pb2.py
+-rw-r--r--   0        0        0      158 2023-02-24 15:57:56.725695 vega_sim-1.0.1/vega_sim/proto/vega/snapshot/v1/snapshot_pb2_grpc.py
+-rw-r--r--   0        0        0    37665 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/proto/vega/vega_pb2.py
+-rw-r--r--   0        0        0      158 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/proto/vega/vega_pb2_grpc.py
+-rw-r--r--   0        0        0       35 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/proto/vega/wallet/__init__.py
+-rw-r--r--   0        0        0      128 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/proto/vega/wallet/v1/__init__.py
+-rw-r--r--   0        0        0     4846 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/proto/vega/wallet/v1/wallet_pb2.py
+-rw-r--r--   0        0        0      158 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/proto/vega/wallet/v1/wallet_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/quant/__init__.py
+-rw-r--r--   0        0        0     2961 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/quant/quant.py
+-rw-r--r--   0        0        0       29 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/reinforcement/.gitignore
+-rw-r--r--   0        0        0        0 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/reinforcement/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/reinforcement/agents/__init__.py
+-rw-r--r--   0        0        0     8259 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/reinforcement/agents/learning_agent.py
+-rw-r--r--   0        0        0    13440 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/reinforcement/agents/learning_agent_MO.py
+-rw-r--r--   0        0        0    18985 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/reinforcement/agents/learning_agent_MO_with_vol.py
+-rw-r--r--   0        0        0    13019 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/reinforcement/agents/learning_agent_heuristic.py
+-rw-r--r--   0        0        0     4754 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/reinforcement/agents/simple_agent.py
+-rw-r--r--   0        0        0      925 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/reinforcement/distributions.py
+-rw-r--r--   0        0        0        0 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/reinforcement/full_market_sim/__init__.py
+-rw-r--r--   0        0        0      608 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/reinforcement/full_market_sim/environments.py
+-rw-r--r--   0        0        0        0 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/reinforcement/full_market_sim/utils/__init__.py
+-rw-r--r--   0        0        0     4458 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/reinforcement/full_market_sim/utils/create_csv.py
+-rw-r--r--   0        0        0     1932 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/reinforcement/full_market_sim/utils/external_assetprice.py
+-rw-r--r--   0        0        0     4782 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/reinforcement/full_market_sim/utils/logdata.py
+-rw-r--r--   0        0        0     4809 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/reinforcement/full_market_sim/utils/strategy.py
+-rw-r--r--   0        0        0      662 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/reinforcement/helpers.py
+-rw-r--r--   0        0        0     2996 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/reinforcement/la_market_state.py
+-rw-r--r--   0        0        0     4243 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/reinforcement/networks.py
+-rw-r--r--   0        0        0     4015 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/reinforcement/plot.py
+-rw-r--r--   0        0        0     9630 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/reinforcement/run_rl_agent.py
+-rw-r--r--   0        0        0     2446 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/reinforcement/run_simple_agent.py
+-rw-r--r--   0        0        0      505 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/reinforcement/theory_intro/Bibliography.bib
+-rw-r--r--   0        0        0    13970 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/reinforcement/theory_intro/RL.tex
+-rw-r--r--   0        0        0    36669 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/reinforcement/theory_intro/images/RL.png
+-rw-r--r--   0        0        0    29521 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/reinforcement/theory_intro/images/RL_inv.png
+-rw-r--r--   0        0        0    39266 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/reinforcement/theory_intro/images/logo.png
+-rw-r--r--   0        0        0    52831 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/reinforcement/theory_intro/images/logo_inv.png
+-rw-r--r--   0        0        0        0 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/replay/__init__.py
+-rw-r--r--   0        0        0     1386 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/replay/replay.py
+-rw-r--r--   0        0        0        0 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/scenario/__init__.py
+-rw-r--r--   0        0        0     2260 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/scenario/adhoc.py
+-rw-r--r--   0        0        0        0 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/scenario/common/__init__.py
+-rw-r--r--   0        0        0    97893 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/scenario/common/agents.py
+-rw-r--r--   0        0        0     7797 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/scenario/common/utils/ideal_mm_models.py
+-rw-r--r--   0        0        0     6107 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/scenario/common/utils/price_process.py
+-rw-r--r--   0        0        0      779 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/scenario/comprehensive_market/agents.py
+-rw-r--r--   0        0        0    12572 2023-02-24 15:57:56.729695 vega_sim-1.0.1/vega_sim/scenario/comprehensive_market/scenario.py
+-rw-r--r--   0        0        0     5296 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/scenario/configurable_market/agents.py
+-rw-r--r--   0        0        0     8149 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/scenario/configurable_market/scenario.py
+-rw-r--r--   0        0        0      249 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/scenario/constants.py
+-rw-r--r--   0        0        0        0 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/scenario/curve_market_maker/__init__.py
+-rw-r--r--   0        0        0    11025 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/scenario/curve_market_maker/scenario.py
+-rw-r--r--   0        0        0        0 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/scenario/hedged_market_maker/__init__.py
+-rw-r--r--   0        0        0      827 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/scenario/hedged_market_maker/agents.py
+-rw-r--r--   0        0        0    18488 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/scenario/hedged_market_maker/scenario.py
+-rw-r--r--   0        0        0        0 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/scenario/ideal_market_maker/__init__.py
+-rw-r--r--   0        0        0    31515 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/scenario/ideal_market_maker/agents.py
+-rw-r--r--   0        0        0     3160 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/scenario/ideal_market_maker/environments.py
+-rw-r--r--   0        0        0     8680 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/scenario/ideal_market_maker/scenario.py
+-rw-r--r--   0        0        0        0 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/scenario/ideal_market_maker/utils/__init__.py
+-rw-r--r--   0        0        0     4782 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/scenario/ideal_market_maker/utils/log_data.py
+-rw-r--r--   0        0        0     4818 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/scenario/ideal_market_maker/utils/strategy.py
+-rw-r--r--   0        0        0        0 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/scenario/ideal_market_maker_v2/__init__.py
+-rw-r--r--   0        0        0    11478 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/scenario/ideal_market_maker_v2/agents.py
+-rw-r--r--   0        0        0     9525 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/scenario/ideal_market_maker_v2/scenario.py
+-rw-r--r--   0        0        0        0 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/scenario/ideal_market_maker_v2/utils/__init__.py
+-rw-r--r--   0        0        0     4818 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/scenario/ideal_market_maker_v2/utils/strategy.py
+-rw-r--r--   0        0        0     1687 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/scenario/market_crash/price_process.py
+-rw-r--r--   0        0        0     9288 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/scenario/market_crash/scenario.py
+-rw-r--r--   0        0        0     1948 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/scenario/multi_market/agents.py
+-rw-r--r--   0        0        0    20142 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/scenario/multi_market/scenario.py
+-rw-r--r--   0        0        0    10779 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/scenario/parameter_experiment/scenario.py
+-rw-r--r--   0        0        0        0 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/scenario/realtime_market/__init__.py
+-rw-r--r--   0        0        0     4646 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/scenario/realtime_market/scenario.py
+-rw-r--r--   0        0        0     6767 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/scenario/registry.py
+-rw-r--r--   0        0        0     2938 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/scenario/scenario.py
+-rw-r--r--   0        0        0    80762 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/service.py
+-rw-r--r--   0        0        0        0 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/tools/__init__.py
+-rw-r--r--   0        0        0     2011 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/tools/load_binaries.py
+-rw-r--r--   0        0        0     7082 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/tools/scenario_output.py
+-rw-r--r--   0        0        0     5728 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/tools/scenario_plots.py
+-rw-r--r--   0        0        0     2658 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/vegahome/config/data-node/config.toml
+-rw-r--r--   0        0        0      277 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/vegahome/config/faucet/config.toml
+-rw-r--r--   0        0        0     3968 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/vegahome/config/node/config.toml
+-rw-r--r--   0        0        0      312 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/vegahome/config/node/wallets.encrypted
+-rw-r--r--   0        0        0      114 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/vegahome/config/wallet-service/config.toml
+-rw-r--r--   0        0        0      321 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/vegahome/config/wallet-service/networks/local.toml
+-rw-r--r--   0        0        0      586 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/vegahome/data/faucet/wallets/vega.1639051237294446827
+-rw-r--r--   0        0        0      586 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/vegahome/data/faucet/wallets/vega.1641976836892788243
+-rw-r--r--   0        0        0      586 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977214518086643
+-rw-r--r--   0        0        0      586 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977270881740938
+-rw-r--r--   0        0        0      586 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977376563008654
+-rw-r--r--   0        0        0      586 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977471442889253
+-rw-r--r--   0        0        0      586 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977537535784009
+-rw-r--r--   0        0        0      586 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977956797580358
+-rw-r--r--   0        0        0      586 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/vegahome/data/faucet/wallets/vega.1641978034856367487
+-rw-r--r--   0        0        0      586 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/vegahome/data/faucet/wallets/vega.1643100690865690276
+-rw-r--r--   0        0        0      491 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/vegahome/data/node/wallets/ethereum/UTC--2021-12-09T12-00-28.751280926Z--b6ea7744971f455bbd754a97e8e05ea13dc1a033
+-rw-r--r--   0        0        0      491 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/vegahome/data/node/wallets/ethereum/UTC--2022-01-12T08-54-28.446104867Z--d1b7ef68bb457b47837c6e81da24455be7a8be0d
+-rw-r--r--   0        0        0      491 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/vegahome/data/node/wallets/ethereum/UTC--2022-01-12T08-57-18.522457076Z--dc699ecdab1705ebe83b60345060b6b7620263a3
+-rw-r--r--   0        0        0      491 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/vegahome/data/node/wallets/ethereum/UTC--2022-01-12T08-58-36.643184436Z--760895ae7f813d685b048336fac88625441d6aa7
+-rw-r--r--   0        0        0      491 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/vegahome/data/node/wallets/ethereum/UTC--2022-01-12T08-59-08.359696969Z--9e5beec6e56b28ccbd02864840b0f1e0125e42ce
+-rw-r--r--   0        0        0      586 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/vegahome/data/node/wallets/vega/vega.1639051228296308758
+-rw-r--r--   0        0        0      586 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/vegahome/data/node/wallets/vega/vega.1641977668033624243
+-rw-r--r--   0        0        0      586 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/vegahome/data/node/wallets/vega/vega.1641977838095755067
+-rw-r--r--   0        0        0      586 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/vegahome/data/node/wallets/vega/vega.1641977916225009082
+-rw-r--r--   0        0        0      586 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/vegahome/data/node/wallets/vega/vega.1641977947934016124
+-rw-r--r--   0        0        0       46 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/vegahome/data/priv_validator_state.json
+-rw-r--r--   0        0        0     3243 2023-02-24 15:57:56.733695 vega_sim-1.0.1/vega_sim/vegahome/data/wallet-service/rsa-keys/private.pem
+-rw-r--r--   0        0        0      800 2023-02-24 15:57:56.737695 vega_sim-1.0.1/vega_sim/vegahome/data/wallet-service/rsa-keys/public.pem
+-rw-r--r--   0        0        0     7023 2023-02-24 15:57:56.737695 vega_sim-1.0.1/vega_sim/vegahome/genesis.json
+-rw-r--r--   0        0        0        3 2023-02-24 15:57:56.737695 vega_sim-1.0.1/vega_sim/vegahome/passphrase-file
+-rw-r--r--   0        0        0        0 2023-02-24 15:57:56.737695 vega_sim-1.0.1/vega_sim/wallet/__init__.py
+-rw-r--r--   0        0        0     1552 2023-02-24 15:57:56.737695 vega_sim-1.0.1/vega_sim/wallet/base.py
+-rw-r--r--   0        0        0     6796 2023-02-24 15:57:56.737695 vega_sim-1.0.1/vega_sim/wallet/slim_wallet.py
+-rw-r--r--   0        0        0     9025 2023-02-24 15:57:56.737695 vega_sim-1.0.1/vega_sim/wallet/vega_wallet.py
+-rw-r--r--   0        0        0     3589 1970-01-01 00:00:00.000000 vega_sim-1.0.1/setup.py
+-rw-r--r--   0        0        0     1631 1970-01-01 00:00:00.000000 vega_sim-1.0.1/PKG-INFO
```

### Comparing `vega_sim-0.67.0/LICENSE` & `vega_sim-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/pyproject.toml` & `vega_sim-1.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "vega_sim"
 description = "Simulator for running self-contained Vega chain on local PC"
 authors = ["Tom McLean <tom@vegaprotocol.io>"]
 license = "MIT"
-version = "0.67.0"
+version = "1.0.1"
 
 [tool.setuptools]
 zip-safe = false
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.11"
 requests = "^2.28.0"
@@ -29,25 +29,29 @@
 grpc-gateway-protoc-gen-openapiv2 = "^0.1.0"
 plotly = {version = "^5.10.0", optional = true}
 TA-Lib = {version = "^0.4.25", optional = true}
 python-dotenv = "^0.21.0"
 deprecated = "^1.2.13"
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.3.0"
+black = "^23.1.0"
 pytest = "^7.1.2"
 requests-mock = "^1.9.3"
 flake8 = "^4.0.1"
 Jinja2 = "^3.1.2"
 nbmake = "^1.3.2"
 matplotlib = "^3.5.2"
 pytest-xdist = "^2.5.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
+
+
+
+
 [tool.poetry.extras]
 learning = ["matplotlib", "tqdm", "torch"]
 jupyter = ["jupyterlab", "jupyter", "matplotlib", "plotly", "ipywidgets"]
 profile = ["snakeviz", "pytest-profiling"]
 agents = ["TA-Lib"]
```

### Comparing `vega_sim-0.67.0/vega_sim/api/data.py` & `vega_sim-1.0.1/vega_sim/api/data.py`

 * *Files 11% similar despite different names*

```diff
@@ -67,14 +67,15 @@
         "party_id",
         "market_id",
         "open_volume",
         "realised_pnl",
         "unrealised_pnl",
         "average_entry_price",
         "updated_at",
+        "loss_socialisation_amount",
     ],
 )
 Transfer = namedtuple(
     "Transfer",
     [
         "id",
         "party_from",
@@ -104,14 +105,30 @@
         "asset",
         "timestamp",
     ],
 )
 
 
 @dataclass
+class DecimalSpec:
+    position_decimals: Optional[int] = None
+    price_decimals: Optional[int] = None
+    asset_decimals: Optional[int] = None
+
+
+@dataclass
+class LedgerEntry:
+    from_account: vega_protos.vega.AccountDetails
+    to_account: vega_protos.vega.AccountDetails
+    amount: str
+    transfer_type: vega_protos.vega.TransferType
+    timestamp: int
+
+
+@dataclass
 class AggregatedLedgerEntry:
     timestamp: int
     quantity: float
     transfer_type: vega_protos.vega.TransferType
     asset_id: str
     from_account_type: vega_protos.vega.AccountType
     to_account_type: vega_protos.vega.AccountType
@@ -136,15 +153,15 @@
 @dataclass
 class Fee:
     maker_fee: float
     infrastructure_fee: float
     liquidity_fee: float
 
 
-@dataclass
+@dataclass(frozen=True)
 class Trade:
     id: str
     market_id: str
     price: float
     size: float
     buyer: str
     seller: str
@@ -155,145 +172,174 @@
     trade_type: vega_protos.vega.Trade.Type
     buyer_fee: Fee
     seller_fee: Fee
     buyer_auction_batch: int
     seller_auction_batch: int
 
 
+def _ledger_entry_from_proto(
+    ledger_entry,
+    asset_decimals: int,
+) -> LedgerEntry:
+    return LedgerEntry(
+        from_account=ledger_entry.from_account,
+        to_account=ledger_entry.to_account,
+        amount=num_from_padded_int(ledger_entry.amount, asset_decimals),
+        transfer_type=ledger_entry.type,
+        timestamp=ledger_entry.timestamp,
+    )
+
+
 def _aggregated_ledger_entry_from_proto(
     ledger_entry: data_node_protos_v2.trading_data.AggregatedLedgerEntry,
-    asset_decimals: int,
+    decimal_spec: DecimalSpec,
 ) -> AggregatedLedgerEntry:
     return AggregatedLedgerEntry(
         timestamp=ledger_entry.timestamp,
-        quantity=num_from_padded_int(ledger_entry.quantity, asset_decimals),
+        quantity=num_from_padded_int(
+            ledger_entry.quantity, decimal_spec.asset_decimals
+        ),
         transfer_type=ledger_entry.transfer_type,
         asset_id=ledger_entry.asset_id,
         from_account_type=ledger_entry.from_account_type,
         to_account_type=ledger_entry.to_account_type,
         from_account_party_id=ledger_entry.from_account_party_id,
         to_account_party_id=ledger_entry.to_account_party_id,
         from_account_market_id=ledger_entry.from_account_market_id,
         to_account_market_id=ledger_entry.to_account_market_id,
     )
 
 
 def _trade_from_proto(
     trade: vega_protos.vega.Trade,
-    price_decimals: int,
-    position_decimals: int,
-    asset_decimals: int,
+    decimal_spec: DecimalSpec,
 ) -> Trade:
     return Trade(
         id=trade.id,
         market_id=trade.market_id,
-        price=num_from_padded_int(trade.price, price_decimals),
-        size=num_from_padded_int(trade.size, position_decimals),
+        price=num_from_padded_int(trade.price, decimal_spec.price_decimals),
+        size=num_from_padded_int(trade.size, decimal_spec.position_decimals),
         buyer=trade.buyer,
         seller=trade.seller,
         aggressor=trade.aggressor,
         buy_order=trade.buy_order,
         sell_order=trade.sell_order,
         timestamp=trade.timestamp,
         trade_type=trade.type,
         buyer_fee=Fee(
-            maker_fee=num_from_padded_int(trade.buyer_fee.maker_fee, asset_decimals),
+            maker_fee=num_from_padded_int(
+                trade.buyer_fee.maker_fee, decimal_spec.asset_decimals
+            ),
             infrastructure_fee=num_from_padded_int(
-                trade.buyer_fee.infrastructure_fee, asset_decimals
+                trade.buyer_fee.infrastructure_fee, decimal_spec.asset_decimals
             ),
             liquidity_fee=num_from_padded_int(
-                trade.buyer_fee.liquidity_fee, asset_decimals
+                trade.buyer_fee.liquidity_fee, decimal_spec.asset_decimals
             ),
         ),
         seller_fee=Fee(
-            maker_fee=num_from_padded_int(trade.seller_fee.maker_fee, asset_decimals),
+            maker_fee=num_from_padded_int(
+                trade.seller_fee.maker_fee, decimal_spec.asset_decimals
+            ),
             infrastructure_fee=num_from_padded_int(
-                trade.seller_fee.infrastructure_fee, asset_decimals
+                trade.seller_fee.infrastructure_fee, decimal_spec.asset_decimals
             ),
             liquidity_fee=num_from_padded_int(
-                trade.seller_fee.liquidity_fee, asset_decimals
+                trade.seller_fee.liquidity_fee, decimal_spec.asset_decimals
             ),
         ),
         buyer_auction_batch=trade.buyer_auction_batch,
         seller_auction_batch=trade.seller_auction_batch,
     )
 
 
 def _margin_level_from_proto(
-    margin_level: vega_protos.vega.MarginLevels, asset_decimals: int
+    margin_level: vega_protos.vega.MarginLevels, decimal_spec: DecimalSpec
 ) -> MarginLevels:
     return MarginLevels(
         maintenance_margin=num_from_padded_int(
-            margin_level.maintenance_margin, asset_decimals
+            margin_level.maintenance_margin, decimal_spec.asset_decimals
+        ),
+        search_level=num_from_padded_int(
+            margin_level.search_level, decimal_spec.asset_decimals
+        ),
+        initial_margin=num_from_padded_int(
+            margin_level.initial_margin, decimal_spec.asset_decimals
         ),
-        search_level=num_from_padded_int(margin_level.search_level, asset_decimals),
-        initial_margin=num_from_padded_int(margin_level.initial_margin, asset_decimals),
         collateral_release_level=num_from_padded_int(
-            margin_level.collateral_release_level, asset_decimals
+            margin_level.collateral_release_level, decimal_spec.asset_decimals
         ),
         party_id=margin_level.party_id,
         market_id=margin_level.market_id,
         asset=margin_level.asset,
         timestamp=margin_level.timestamp,
     )
 
 
 def _order_from_proto(
-    order: vega_protos.vega.Order, price_decimals: int, position_decimals: int
+    order: vega_protos.vega.Order,
+    decimal_spec: DecimalSpec,
 ) -> Order:
     return Order(
         id=order.id,
-        price=num_from_padded_int(order.price, price_decimals),
-        size=num_from_padded_int(order.size, position_decimals),
+        price=num_from_padded_int(order.price, decimal_spec.price_decimals),
+        size=num_from_padded_int(order.size, decimal_spec.position_decimals),
         reference=order.reference,
         side=order.side,
         status=order.status,
-        remaining=num_from_padded_int(order.remaining, position_decimals),
+        remaining=num_from_padded_int(order.remaining, decimal_spec.position_decimals),
         time_in_force=order.time_in_force,
         order_type=order.type,
         created_at=order.created_at,
         expires_at=order.expires_at,
         party_id=order.party_id,
         updated_at=order.updated_at,
         version=order.version,
         market_id=order.market_id,
     )
 
 
 def _position_from_proto(
     position: vega_protos.vega.Position,
-    position_decimals: int,
-    asset_decimals: int,
-    price_decimals: int,
+    decimal_spec: DecimalSpec,
 ) -> Position:
     return Position(
         party_id=position.party_id,
         market_id=position.market_id,
-        open_volume=num_from_padded_int(position.open_volume, position_decimals),
-        realised_pnl=num_from_padded_int(position.realised_pnl, asset_decimals),
-        unrealised_pnl=num_from_padded_int(position.unrealised_pnl, asset_decimals),
+        open_volume=num_from_padded_int(
+            position.open_volume, decimal_spec.position_decimals
+        ),
+        realised_pnl=num_from_padded_int(
+            position.realised_pnl, decimal_spec.asset_decimals
+        ),
+        unrealised_pnl=num_from_padded_int(
+            position.unrealised_pnl, decimal_spec.asset_decimals
+        ),
         average_entry_price=num_from_padded_int(
-            position.average_entry_price, price_decimals
+            position.average_entry_price, decimal_spec.price_decimals
+        ),
+        loss_socialisation_amount=num_from_padded_int(
+            position.loss_socialisation_amount,
+            decimal_spec.asset_decimals,
         ),
         updated_at=position.updated_at,
     )
 
 
 def _transfer_from_proto(
-    transfer: vega_protos.vega.Transfer,
-    asset_decimals: int,
+    transfer: vega_protos.vega.Transfer, decimal_spec: DecimalSpec
 ) -> Transfer:
     return Transfer(
         id=transfer.id,
         party_from=getattr(transfer, "from"),
         from_account_type=transfer.from_account_type,
         party_to=transfer.to,
         to_account_type=transfer.to_account_type,
         asset=transfer.asset,
-        amount=num_from_padded_int(transfer.amount, asset_decimals),
+        amount=num_from_padded_int(transfer.amount, decimal_spec.asset_decimals),
         reference=transfer.reference,
         status=transfer.status,
         timestamp=transfer.timestamp,
         reason=transfer.reason,
         one_off=transfer.one_off,
         recurring=transfer.recurring,
     )
@@ -354,17 +400,19 @@
                 data_client=data_client,
             )
             asset_decimals_map[pos.market_id] = int(asset_info.details.decimals)
 
         # Convert raw proto into a market-sim Position object
         positions[pos.market_id] = _position_from_proto(
             position=pos,
-            price_decimals=market_price_decimals_map[pos.market_id],
-            position_decimals=market_position_decimals_map[pos.market_id],
-            asset_decimals=asset_decimals_map[market_to_asset_map[pos.market_id]],
+            decimal_spec=DecimalSpec(
+                price_decimals=market_price_decimals_map[pos.market_id],
+                position_decimals=market_position_decimals_map[pos.market_id],
+                asset_decimals=asset_decimals_map[market_to_asset_map[pos.market_id]],
+            ),
         )
 
     if market_id is None:
         return positions
     else:
         return positions[market_id]
 
@@ -531,17 +579,18 @@
             str, The ID of the market requested
         data_client:
             VegaTradingDataClientV2, an instantiated gRPC data client
 
     Returns:
         int, The number of decimal places the market uses
     """
-    return data_raw.market_info(
+    res = data_raw.market_info(
         market_id=market_id, data_client=data_client
     ).decimal_places
+    return res
 
 
 def market_position_decimals(
     market_id: str,
     data_client: vac.VegaTradingDataClientV2,
 ) -> int:
     """Returns the number of decimal places a specified market uses for position units.
@@ -579,19 +628,24 @@
     ).details.decimals
 
 
 def best_prices(
     market_id: str,
     data_client: vac.VegaTradingDataClientV2,
     price_decimals: Optional[int] = None,
+    market_data: Optional[vega_protos.vega.MarketData] = None,
 ) -> Tuple[float, float]:
     """
     Output the best static bid price and best static ask price in current market.
     """
-    mkt_data = data_raw.market_data(market_id=market_id, data_client=data_client)
+    mkt_data = (
+        market_data
+        if market_data is not None
+        else data_raw.market_data(market_id=market_id, data_client=data_client)
+    )
     mkt_price_dp = (
         price_decimals
         if price_decimals is not None
         else market_price_decimals(market_id=market_id, data_client=data_client)
     )
 
     return (
@@ -600,19 +654,24 @@
     )
 
 
 def price_bounds(
     market_id: str,
     data_client: vac.VegaTradingDataClientV2,
     price_decimals: Optional[int] = None,
+    market_data: Optional[vega_protos.vega.MarketData] = None,
 ) -> Tuple[Optional[float], Optional[float]]:
     """
     Output the tightest price bounds in current market.
     """
-    mkt_data = data_raw.market_data(market_id=market_id, data_client=data_client)
+    mkt_data = (
+        market_data
+        if market_data is not None
+        else data_raw.market_data(market_id=market_id, data_client=data_client)
+    )
     mkt_price_dp = (
         price_decimals
         if price_decimals is not None
         else market_price_decimals(market_id=market_id, data_client=data_client)
     )
 
     lower_bounds = [
@@ -719,16 +778,18 @@
             )
             mkt_price_dp[order.market_id] = market_price_decimals(
                 market_id=order.market_id, data_client=data_client
             )
 
         converted_order = _order_from_proto(
             order,
-            price_decimals=mkt_price_dp[order.market_id],
-            position_decimals=mkt_pos_dp[order.market_id],
+            decimal_spec=DecimalSpec(
+                price_decimals=mkt_price_dp[order.market_id],
+                position_decimals=mkt_pos_dp[order.market_id],
+            ),
         )
         output_orders.append(converted_order)
     return output_orders
 
 
 def all_orders(
     market_id: str,
@@ -774,16 +835,18 @@
                 market_id=order.market_id, data_client=data_client
             )
 
         if open_only and order.status != vega_protos.vega.Order.Status.STATUS_ACTIVE:
             continue
         converted_order = _order_from_proto(
             order,
-            price_decimals=mkt_price_dp[order.market_id],
-            position_decimals=mkt_pos_dp[order.market_id],
+            DecimalSpec(
+                price_decimals=mkt_price_dp[order.market_id],
+                position_decimals=mkt_pos_dp[order.market_id],
+            ),
         )
         output_orders.append(converted_order)
     return output_orders
 
 
 def order_book_by_market(
     market_id: str,
@@ -888,104 +951,14 @@
 
     return MarketDepth(
         buys=[_price_level_from_raw(level) for level in mkt_depth.buy],
         sells=[_price_level_from_raw(level) for level in mkt_depth.sell],
     )
 
 
-def order_subscription(
-    data_client: vac.VegaCoreClient,
-    trading_data_client: vac.VegaTradingDataClientV2,
-    market_id: Optional[str] = None,
-    party_id: Optional[str] = None,
-) -> Iterable[Order]:
-    """Subscribe to a stream of Order updates from the data-node.
-    The stream of orders returned from this function is an iterable which
-    does not end and will continue to tick another order update whenever
-    one is received.
-
-    Args:
-        market_id:
-            Optional[str], If provided, only update orders from this market
-        party_id:
-            Optional[str], If provided, only update orders from this party
-    Returns:
-        Iterable[Order], Infinite iterable of order updates
-    """
-
-    order_stream = data_raw.observe_event_bus(
-        data_client=data_client,
-        type=[events_protos.BUS_EVENT_TYPE_ORDER],
-    )
-
-    def _order_gen(
-        order_stream: Iterable[vega_protos.api.v1.core.ObserveEventBusResponse],
-    ) -> Iterable[Order]:
-        mkt_pos_dp = {}
-        mkt_price_dp = {}
-        try:
-            for order_list in order_stream:
-                for bus_event in order_list.events:
-                    order = bus_event.order
-                    if order.market_id not in mkt_pos_dp:
-                        mkt_pos_dp[order.market_id] = market_position_decimals(
-                            market_id=order.market_id, data_client=trading_data_client
-                        )
-                        mkt_price_dp[order.market_id] = market_price_decimals(
-                            market_id=order.market_id, data_client=trading_data_client
-                        )
-                    yield _order_from_proto(
-                        order,
-                        mkt_price_dp[order.market_id],
-                        mkt_pos_dp[order.market_id],
-                    )
-        except Exception as _:
-            logger.info("Order subscription closed")
-            return
-
-    return _order_gen(order_stream=order_stream)
-
-
-def transfer_subscription(
-    data_client: vac.VegaCoreClient,
-    trading_data_client: vac.VegaTradingDataClientV2,
-    market_id: Optional[str] = None,
-    party_id: Optional[str] = None,
-) -> Iterable[Order]:
-    transfer_stream = data_raw.observe_event_bus(
-        data_client=data_client,
-        type=[events_protos.BUS_EVENT_TYPE_TRANSFER],
-        market_id=market_id,
-        party_id=party_id,
-    )
-
-    def _transfer_gen(
-        transfer_stream: Iterable[vega_protos.api.v1.core.ObserveEventBusResponse],
-    ) -> Iterable[Transfer]:
-        asset_dp = {}
-        try:
-            for transfer_list in transfer_stream:
-                for bus_event in transfer_list.events:
-                    transfer = bus_event.transfer
-                    if transfer.asset not in asset_dp:
-                        asset_dp[transfer.asset] = get_asset_decimals(
-                            asset_id=transfer.asset,
-                            data_client=trading_data_client,
-                        )
-                    yield _transfer_from_proto(
-                        transfer=transfer,
-                        asset_decimals=asset_dp[transfer.asset],
-                    )
-        except Exception as _:
-            logger.info("Transfer subscription closed")
-            return
-
-    return _transfer_gen(transfer_stream=transfer_stream)
-
-
 def has_liquidity_provision(
     data_client: vac.VegaTradingDataClientV2,
     market_id: str,
     party_id: str,
 ) -> bool:
     lip = data_raw.liquidity_provisions(
         data_client=data_client, market_id=market_id, party_id=party_id
@@ -1014,15 +987,17 @@
     res_margins = []
     for margin in margins:
         if margin.asset not in asset_dp:
             asset_dp[margin.asset] = get_asset_decimals(
                 asset_id=margin.asset, data_client=data_client
             )
         res_margins.append(
-            _margin_level_from_proto(margin, asset_decimals=asset_dp[margin.asset])
+            _margin_level_from_proto(
+                margin, DecimalSpec(asset_decimals=asset_dp[margin.asset])
+            )
         )
     return res_margins
 
 
 def get_trades(
     data_client: vac.VegaTradingDataClientV2,
     market_id: str,
@@ -1058,17 +1033,19 @@
                     market_id=market_id, data_client=data_client
                 ).tradable_instrument.instrument.future.settlement_asset,
                 data_client=data_client,
             )
         res_trades.append(
             _trade_from_proto(
                 trade,
-                price_decimals=market_price_decimals_map[trade.market_id],
-                position_decimals=market_position_decimals_map[trade.market_id],
-                asset_decimals=market_asset_decimals_map[trade.market_id],
+                DecimalSpec(
+                    price_decimals=market_price_decimals_map[trade.market_id],
+                    position_decimals=market_position_decimals_map[trade.market_id],
+                    asset_decimals=market_asset_decimals_map[trade.market_id],
+                ),
             )
         )
     return res_trades
 
 
 def ping(data_client: vac.VegaTradingDataClientV2):
     return data_client.Ping(data_node_protos_v2.trading_data.PingRequest())
@@ -1100,108 +1077,84 @@
         direction=direction,
     )
 
     asset_dp = {}
     res_transfers = []
 
     for transfer in transfers:
+        if transfer.status == events_protos.Transfer.Status.STATUS_REJECTED:
+            continue
+
         if transfer.asset not in asset_dp:
             asset_dp[transfer.asset] = get_asset_decimals(
                 asset_id=transfer.asset, data_client=data_client
             )
-
         res_transfers.append(
             _transfer_from_proto(
-                transfer=transfer, asset_decimals=asset_dp[transfer.asset]
+                transfer=transfer,
+                decimal_spec=DecimalSpec(asset_decimals=asset_dp[transfer.asset]),
             )
         )
 
     return res_transfers
 
 
-def trades_subscription(
-    data_client: vac.VegaCoreClient,
-    trading_data_client: vac.VegaTradingDataClientV2,
-) -> Iterable[Trade]:
-    """Subscribe to a stream of Order updates from the data-node.
-    The stream of orders returned from this function is an iterable which
-    does not end and will continue to tick another order update whenever
-    one is received.
-
-    Returns:
-        Iterable[Trade], Infinite iterable of trade updates
-    """
-
-    trade_stream = data_raw.observe_event_bus(
-        data_client=data_client,
-        type=[events_protos.BUS_EVENT_TYPE_TRADE],
-    )
-
-    return _stream_gen(
-        stream=trade_stream,
-        trading_data_client=trading_data_client,
-        extraction_fn=lambda evt: evt.trade,
-        conversion_fn=_trade_from_proto,
-    )
-
-
-def _stream_gen(
-    stream: Iterable[vega_protos.api.v1.core.ObserveEventBusResponse],
-    trading_data_client: vac.VegaTradingDataClientV2,
+def _stream_handler(
+    stream_item: vega_protos.api.v1.core.ObserveEventBusResponse,
     extraction_fn: Callable[[vega_protos.events.v1.events.BusEvent], T],
     conversion_fn: Callable[[T, int, int, int], S],
-) -> Iterable[S]:
-    mkt_pos_dp = {}
-    mkt_price_dp = {}
-    mkt_asset_dp = {}
-    try:
-        for stream_event_list in stream:
-            for bus_event in stream_event_list.events:
-                event = extraction_fn(bus_event)
-                if event.market_id not in mkt_pos_dp:
-                    mkt_pos_dp[event.market_id] = market_position_decimals(
-                        market_id=event.market_id, data_client=trading_data_client
-                    )
-                    mkt_price_dp[event.market_id] = market_price_decimals(
-                        market_id=event.market_id, data_client=trading_data_client
-                    )
-                    mkt_asset_dp[event.market_id] = get_asset_decimals(
-                        asset_id=data_raw.market_info(
-                            market_id=event.market_id, data_client=trading_data_client
-                        ).tradable_instrument.instrument.future.settlement_asset,
-                        data_client=trading_data_client,
-                    )
-                yield conversion_fn(
-                    event,
-                    mkt_price_dp[event.market_id],
-                    mkt_pos_dp[event.market_id],
-                    mkt_asset_dp[event.market_id],
-                )
-    except:
-        logger.info("Order subscription closed")
-        return
+    mkt_pos_dp: Optional[Dict[str, int]] = None,
+    mkt_price_dp: Optional[Dict[str, int]] = None,
+    mkt_to_asset: Optional[Dict[str, str]] = None,
+    asset_dp: Optional[Dict[str, int]] = None,
+) -> S:
+    mkt_pos_dp = mkt_pos_dp if mkt_pos_dp is not None else {}
+    mkt_price_dp = mkt_price_dp if mkt_price_dp is not None else {}
+    mkt_to_asset = mkt_to_asset if mkt_to_asset is not None else {}
+    asset_dp = asset_dp if asset_dp is not None else {}
+
+    event = extraction_fn(stream_item)
+
+    market_id = getattr(event, "market_id", None)
+    asset_decimals = asset_dp.get(getattr(event, "asset", mkt_to_asset.get(market_id)))
+
+    return conversion_fn(
+        event,
+        DecimalSpec(
+            price_decimals=mkt_price_dp[market_id] if market_id is not None else None,
+            position_decimals=mkt_pos_dp[market_id] if market_id is not None else None,
+            asset_decimals=asset_decimals,
+        ),
+    )
 
 
 def get_liquidity_fee_shares(
     data_client: vac.VegaTradingDataClientV2,
     market_id: str,
     party_id: Optional[str] = None,
+    market_data: Optional[vega_protos.vega.MarketData] = None,
 ) -> Union[Dict, float]:
     """Gets the current liquidity fee share for each party or a specified party.
 
     Args:
         data_client (vac.VegaTradingDataClientV2):
             An instantiated gRPC data client
         market_id (str):
             Id of market to get liquidity fee shares from.
         party_id (Optional[str], optional):
             Id of party to get liquidity fee shares for. Defaults to None.
+        market_data (Optional[vega_protos.markets.MarketData]):
+            Market data to use. If not passed, loads from data node
     """
 
-    market_data = data_raw.market_data(data_client=data_client, market_id=market_id)
+    market_data = (
+        market_data
+        if market_data is not None
+        else data_raw.market_data(data_client=data_client, market_id=market_id)
+    )
 
     # Calculate share of fees for each LP
     shares = {
         lp.party: float(lp.equity_like_share) * float(lp.average_score)
         for lp in market_data.liquidity_provider_fee_share
     }
     total_shares = sum(shares.values())
@@ -1295,11 +1248,103 @@
         if entry.asset_id not in asset_decimals_map:
             asset_decimals_map[entry.asset_id] = get_asset_decimals(
                 asset_id=entry.asset_id,
                 data_client=data_client,
             )
         ledger_entries.append(
             _aggregated_ledger_entry_from_proto(
-                entry, asset_decimals=asset_decimals_map[entry.asset_id]
+                entry, DecimalSpec(asset_decimals=asset_decimals_map[entry.asset_id])
             )
         )
     return ledger_entries
+
+
+def trades_subscription_handler(
+    stream: Iterable[vega_protos.api.v1.core.ObserveEventBusResponse],
+    mkt_pos_dp: Optional[Dict[str, int]] = None,
+    mkt_price_dp: Optional[Dict[str, int]] = None,
+    mkt_to_asset: Optional[Dict[str, str]] = None,
+    asset_dp: Optional[Dict[str, int]] = None,
+) -> Trade:
+    """Subscribe to a stream of Order updates from the data-node.
+    The stream of orders returned from this function is an iterable which
+    does not end and will continue to tick another order update whenever
+    one is received.
+
+    Returns:
+        Iterable[Trade], Infinite iterable of trade updates
+    """
+    return _stream_handler(
+        stream_item=stream,
+        extraction_fn=lambda evt: evt.trade,
+        conversion_fn=_trade_from_proto,
+        mkt_pos_dp=mkt_pos_dp,
+        mkt_price_dp=mkt_price_dp,
+        mkt_to_asset=mkt_to_asset,
+        asset_dp=asset_dp,
+    )
+
+
+def order_subscription_handler(
+    stream: Iterable[vega_protos.api.v1.core.ObserveEventBusResponse],
+    mkt_pos_dp: Optional[Dict[str, int]] = None,
+    mkt_price_dp: Optional[Dict[str, int]] = None,
+    mkt_to_asset: Optional[Dict[str, str]] = None,
+    asset_dp: Optional[Dict[str, int]] = None,
+) -> Order:
+    """Subscribe to a stream of Order updates from the data-node.
+    The stream of orders returned from this function is an iterable which
+    does not end and will continue to tick another order update whenever
+    one is received.
+
+    Args:
+        market_id:
+            Optional[str], If provided, only update orders from this market
+        party_id:
+            Optional[str], If provided, only update orders from this party
+    Returns:
+        Iterable[Order], Infinite iterable of order updates
+    """
+    return _stream_handler(
+        stream_item=stream,
+        extraction_fn=lambda evt: evt.order,
+        conversion_fn=_order_from_proto,
+        mkt_pos_dp=mkt_pos_dp,
+        mkt_price_dp=mkt_price_dp,
+        mkt_to_asset=mkt_to_asset,
+        asset_dp=asset_dp,
+    )
+
+
+def transfer_subscription_handler(
+    stream: Iterable[vega_protos.api.v1.core.ObserveEventBusResponse],
+    mkt_pos_dp: Optional[Dict[str, int]] = None,
+    mkt_price_dp: Optional[Dict[str, int]] = None,
+    mkt_to_asset: Optional[Dict[str, str]] = None,
+    asset_dp: Optional[Dict[str, int]] = None,
+) -> Transfer:
+    return _stream_handler(
+        stream_item=stream,
+        extraction_fn=lambda evt: evt.transfer,
+        conversion_fn=_transfer_from_proto,
+        mkt_pos_dp=mkt_pos_dp,
+        mkt_price_dp=mkt_price_dp,
+        mkt_to_asset=mkt_to_asset,
+        asset_dp=asset_dp,
+    )
+
+
+def ledger_entries_subscription_handler(
+    stream_item: vega_protos.api.v1.core.ObserveEventBusResponse,
+    asset_dp: Optional[Dict[str, int]] = None,
+) -> Iterable[LedgerEntry]:
+    ledger_entries = []
+    for ledger_movement in stream_item.ledger_movements.ledger_movements:
+        for ledger_entry in ledger_movement.entries:
+            asset_id = ledger_entry.from_account.asset_id
+            ledger_entries.append(
+                _ledger_entry_from_proto(
+                    ledger_entry,
+                    asset_decimals=asset_dp[asset_id],
+                )
+            )
+    return ledger_entries
```

### Comparing `vega_sim-0.67.0/vega_sim/api/data_raw.py` & `vega_sim-1.0.1/vega_sim/api/data_raw.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from __future__ import annotations
 
-import datetime
+import logging
 from collections import namedtuple
 from typing import Callable, Iterable, List, Optional, TypeVar, Union
+import datetime
 
 import vega_sim.grpc.client as vac
 import vega_sim.proto.data_node.api.v2 as data_node_protos_v2
 import vega_sim.proto.vega as vega_protos
 import vega_sim.proto.vega.events.v1.events_pb2 as events_protos
 
+logger = logging.getLogger(__name__)
+
 MarketAccount = namedtuple("MarketAccount", ["insurance", "liquidity_fee"])
 
 T = TypeVar("T")
 S = TypeVar("S")
 U = TypeVar("U")
 
 
@@ -160,14 +163,35 @@
     Output market info.
     """
     return data_client.GetLatestMarketData(
         data_node_protos_v2.trading_data.GetLatestMarketDataRequest(market_id=market_id)
     ).market_data
 
 
+def market_data_history(
+    market_id: str,
+    start: datetime.datetime,
+    end: datetime.datetime,
+    data_client: vac.VegaTradingDataClientV2,
+) -> List[vega_protos.vega.MarketData]:
+    """
+    Output market data history.
+    """
+
+    return unroll_v2_pagination(
+        base_request=data_node_protos_v2.trading_data.GetMarketDataHistoryByIDRequest(
+            market_id=market_id,
+            start_timestamp=int(start.timestamp() * 1e9),
+            end_timestamp=int(end.timestamp() * 1e9),
+        ),
+        request_func=lambda x: data_client.GetMarketDataHistoryByID(x).market_data,
+        extraction_func=lambda res: [i.node for i in res.edges],
+    )
+
+
 def infrastructure_fee_accounts(
     asset_id: str,
     data_client: vac.VegaTradingDataClientV2,
 ) -> List[vega_protos.vega.Account]:
     """
     Output infrastructure fee accounts
     """
@@ -524,7 +548,31 @@
         )
 
     return unroll_v2_pagination(
         base_request=base_request,
         request_func=lambda x: data_client.ListLedgerEntries(x).ledger_entries,
         extraction_func=lambda res: [i.node for i in res.edges],
     )
+
+
+def market_data_subscription(
+    data_client: vac.VegaCoreClient,
+    market_id: Optional[str] = None,
+) -> Iterable[vega_protos.vega.MarketData]:
+    data_stream = observe_event_bus(
+        data_client=data_client,
+        type=[events_protos.BUS_EVENT_TYPE_MARKET_DATA],
+        market_id=market_id,
+    )
+
+    def _data_gen(
+        data_stream: Iterable[vega_protos.api.v1.core.ObserveEventBusResponse],
+    ) -> Iterable[vega_protos.vega.MarketData]:
+        try:
+            for market_data in data_stream:
+                for market_data_event in market_data.events:
+                    yield market_data_event.market_data
+        except Exception:
+            logger.info("Order subscription closed")
+            return
+
+    return _data_gen(data_stream=data_stream)
```

### Comparing `vega_sim-0.67.0/vega_sim/api/faucet.py` & `vega_sim-1.0.1/vega_sim/api/faucet.py`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/api/governance.py` & `vega_sim-1.0.1/vega_sim/api/governance.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,27 +73,29 @@
     ).timestamp
     return int(blockchain_time / 1e9)
 
 
 def propose_market_from_config(
     data_client: vac.VegaTradingDataClientV2,
     wallet: Wallet,
-    proposal_wallet_name: str,
+    proposal_key_name: str,
     market_config: MarketConfig,
     closing_time: str,
     enactment_time: str,
     time_forward_fn: Optional[Callable[[], None]] = None,
     governance_asset: Optional[str] = "VOTE",
-    proposal_key_name: Optional[str] = None,
+    proposal_wallet_name: Optional[str] = None,
 ) -> str:
     # Make sure Vega network has governance asset
     vote_asset_id = find_asset_id(
         governance_asset, raise_on_missing=True, data_client=data_client
     )
-    pub_key = wallet.public_key(proposal_wallet_name, proposal_key_name)
+    pub_key = wallet.public_key(
+        wallet_name=proposal_wallet_name, name=proposal_key_name
+    )
 
     # Request accounts for party and check governance asset balance
     party_accounts = data_raw.list_accounts(
         data_client=data_client, asset_id=vote_asset_id, party_id=pub_key
     )
 
     voting_balance = 0
@@ -127,15 +129,15 @@
         data_client=data_client,
         time_forward_fn=time_forward_fn,
     ).proposal.id
 
 
 def propose_future_market(
     market_name: str,
-    wallet_name: str,
+    key_name: str,
     wallet: Wallet,
     settlement_asset_id: str,
     data_client: vac.VegaTradingDataClientV2,
     termination_pub_key: str,
     governance_asset: str = "VOTE",
     future_asset: str = "BTC",
     position_decimals: Optional[int] = None,
@@ -144,15 +146,15 @@
     enactment_time: Optional[int] = None,
     risk_model: Optional[vega_protos.markets.LogNormalRiskModel] = None,
     time_forward_fn: Optional[Callable[[], None]] = None,
     price_monitoring_parameters: Optional[
         vega_protos.markets.PriceMonitoringParameters
     ] = None,
     lp_price_range: float = 1,
-    key_name: Optional[str] = None,
+    wallet_name: Optional[str] = None,
 ) -> str:
     """Propose a future market as specified user.
 
     Args:
         market_name:
             str, name of the market
         wallet_name:
@@ -194,15 +196,15 @@
     Returns:
         str, the ID of the future market proposal on chain
     """
     # Make sure Vega network has governance asset
     vote_asset_id = find_asset_id(
         governance_asset, raise_on_missing=True, data_client=data_client
     )
-    pub_key = wallet.public_key(wallet_name, key_name)
+    pub_key = wallet.public_key(wallet_name=wallet_name, name=key_name)
 
     # Request accounts for party and check governance asset balance
     party_accounts = data_raw.list_accounts(
         data_client=data_client, asset_id=vote_asset_id, party_id=pub_key
     )
 
     voting_balance = 0
@@ -280,17 +282,17 @@
                         settlement_data_property=f"price.{future_asset}.value",
                         trading_termination_property="trading.terminated",
                     ),
                 ),
             ),
             lp_price_range=str(lp_price_range),
             decimal_places=price_decimals,
-            position_decimal_places=0
-            if position_decimals is None
-            else position_decimals,
+            position_decimal_places=(
+                0 if position_decimals is None else position_decimals
+            ),
             metadata=[
                 f"base:{future_asset}",
             ],
             liquidity_monitoring_parameters=vega_protos.markets.LiquidityMonitoringParameters(
                 target_stake_parameters=vega_protos.markets.TargetStakeParameters(
                     time_window=3600, scaling_factor=1
                 ),
@@ -319,24 +321,24 @@
         key_name=key_name,
     ).proposal.id
 
 
 def propose_network_parameter_change(
     parameter: str,
     value: str,
-    wallet_name: str,
+    key_name: str,
     wallet: Wallet,
     closing_time: Optional[int] = None,
     enactment_time: Optional[int] = None,
     data_client: Optional[vac.VegaTradingDataClientV2] = None,
     time_forward_fn: Optional[Callable[[], None]] = None,
-    key_name: Optional[str] = None,
+    wallet_name: Optional[str] = None,
 ):
     network_param_update = _build_generic_proposal(
-        pub_key=wallet.public_key(wallet_name, key_name),
+        pub_key=wallet.public_key(wallet_name=wallet_name, name=key_name),
         data_client=data_client,
         closing_time=closing_time,
         enactment_time=enactment_time,
     )
     network_param_update.terms.update_network_parameter.CopyFrom(
         vega_protos.governance.UpdateNetworkParameter(
             changes=vega_protos.vega.NetworkParameter(key=parameter, value=value)
@@ -350,84 +352,85 @@
         time_forward_fn=time_forward_fn,
         key_name=key_name,
     ).proposal.id
 
 
 def propose_market_update(
     market_id: str,
-    wallet_name: str,
+    key_name: str,
     wallet: Wallet,
     market_update: vega_protos.governance.UpdateMarketConfiguration,
     closing_time: Optional[int] = None,
     enactment_time: Optional[int] = None,
     data_client: Optional[vac.VegaTradingDataClientV2] = None,
     time_forward_fn: Optional[Callable[[], None]] = None,
-    key_name: Optional[str] = None,
+    wallet_name: Optional[str] = None,
 ) -> str:
     network_param_update = _build_generic_proposal(
-        pub_key=wallet.public_key(wallet_name, key_name),
+        pub_key=wallet.public_key(wallet_name=wallet_name, name=key_name),
         data_client=data_client,
         closing_time=closing_time,
         enactment_time=enactment_time,
     )
     network_param_update.terms.update_market.CopyFrom(
         vega_protos.governance.UpdateMarket(market_id=market_id, changes=market_update)
     )
 
     return _make_and_wait_for_proposal(
         wallet_name=wallet_name,
+        key_name=key_name,
         wallet=wallet,
         proposal=network_param_update,
         data_client=data_client,
         time_forward_fn=time_forward_fn,
     ).proposal.id
 
 
 def approve_proposal(
-    wallet_name: str,
+    key_name: str,
     proposal_id: str,
     wallet: Wallet,
-    key_name: Optional[str] = None,
+    wallet_name: Optional[str] = None,
 ):
     wallet.submit_transaction(
         transaction=commands_protos.commands.VoteSubmission(
             value=vega_protos.governance.Vote.Value.VALUE_YES, proposal_id=proposal_id
         ),
-        name=wallet_name,
+        wallet_name=wallet_name,
         transaction_type="vote_submission",
         key_name=key_name,
     )
 
 
 def propose_asset(
-    wallet_name: str,
+    key_name: str,
     wallet: Wallet,
     name: str,
     symbol: str,
     decimals: int,
     data_client: vac.VegaTradingDataClientV2,
     quantum: int = 1,
     max_faucet_amount: int = 10e9,
     closing_time: Optional[int] = None,
     enactment_time: Optional[int] = None,
     validation_time: Optional[int] = None,
     time_forward_fn: Optional[Callable[[], None]] = None,
-    key_name: Optional[str] = None,
+    wallet_name: Optional[str] = None,
 ) -> str:
     asset_detail = vega_protos.assets.AssetDetails(
         name=name,
         symbol=symbol,
         decimals=decimals,
         quantum=str(int(quantum)),
         builtin_asset=vega_protos.assets.BuiltinAsset(
             max_faucet_amount_mint=str(int(max_faucet_amount))
         ),
     )
     proposal = _build_generic_proposal(
-        pub_key=wallet.public_key(wallet_name, key_name),
+        pub_key=wallet.public_key(wallet_name=wallet_name, name=key_name),
         data_client=data_client,
         closing_time=closing_time,
         enactment_time=enactment_time,
     )
     proposal.terms.validation_timestamp = (
         validation_time
         if validation_time is not None
@@ -480,24 +483,24 @@
         rationale=vega_protos.governance.ProposalRationale(
             description="Making a proposal", title="This is a proposal"
         ),
     )
 
 
 def _make_and_wait_for_proposal(
-    wallet_name: str,
+    key_name: str,
     wallet: Wallet,
     proposal: commands_protos.commands.ProposalSubmission,
     data_client: vac.VegaTradingDataClientV2,
     time_forward_fn: Optional[Callable[[], None]] = None,
-    key_name: Optional[str] = None,
+    wallet_name: Optional[str] = None,
 ) -> ProposalSubmission:
     wallet.submit_transaction(
         transaction=proposal,
-        name=wallet_name,
+        wallet_name=wallet_name,
         transaction_type="proposal_submission",
         key_name=key_name,
     )
     logger.debug("Waiting for proposal acceptance")
 
     # Allow one failure, forward once more
     try:
@@ -522,19 +525,19 @@
             f" {enum_to_str(vega_protos.governance.ProposalError, proposal.proposal.reason)}."
             f" Any further info: {proposal.proposal.error_details}"
         )
     return proposal
 
 
 def settle_oracle(
-    wallet_name: str,
+    key_name: str,
     wallet: Wallet,
     settlement_price: float,
     oracle_name: str,
-    key_name: Optional[str] = None,
+    wallet_name: Optional[str] = None,
 ) -> None:
     """
     Settle the market and send settlement price.
 
     Args:
         login_token:
             str, the login token for the wallet authorised to send
@@ -543,30 +546,30 @@
             str, the public key for the wallet authorised to send
              termination/settlement oracle signals
         settlement_price:
             float, final settlement price for the asset
         oracle_name:
             str, the name of the oracle to settle
         key_name:
-            Optional[str], key name stored in metadata. Defaults to None.
+            str, key name stored in metadata.
 
     """
 
     # Use oracle feed to terminate market
     payload = {"trading.terminated": "true"}
     payload = json.dumps(payload).encode()
 
     oracle_submission = commands_protos.data.OracleDataSubmission(
         payload=payload,
         source=commands_protos.data.OracleDataSubmission.OracleSource.ORACLE_SOURCE_JSON,
     )
 
     wallet.submit_transaction(
         transaction=oracle_submission,
-        name=wallet_name,
+        wallet_name=wallet_name,
         transaction_type="oracle_data_submission",
         key_name=key_name,
     )
 
     # use oracle to settle market
     payload = {oracle_name: str(settlement_price)}
     payload = json.dumps(payload).encode()
@@ -574,11 +577,11 @@
     oracle_submission = commands_protos.data.OracleDataSubmission(
         payload=payload,
         source=commands_protos.data.OracleDataSubmission.OracleSource.ORACLE_SOURCE_JSON,
     )
 
     wallet.submit_transaction(
         transaction=oracle_submission,
-        name=wallet_name,
+        wallet_name=wallet_name,
         transaction_type="oracle_data_submission",
         key_name=key_name,
     )
```

### Comparing `vega_sim-0.67.0/vega_sim/api/helpers.py` & `vega_sim-1.0.1/vega_sim/api/helpers.py`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/api/market.py` & `vega_sim-1.0.1/vega_sim/api/market.py`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/api/trading.py` & `vega_sim-1.0.1/vega_sim/api/trading.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         pegged_order=pegged_order,
     )
 
     # Sign the transaction with an order submission command
     # Note: Setting propagate to true will also submit to a Vega node
     wallet.submit_transaction(
         transaction=order_data,
-        name=wallet_name,
+        wallet_name=wallet_name,
         transaction_type="order_submission",
         key_name=key_name,
     )
 
     logger.debug(f"Submitted Order on {side} at price {price}.")
 
     if wait:
@@ -217,15 +217,15 @@
         time_in_force=time_in_force,
         pegged_offset=pegged_offset,
         pegged_reference=pegged_reference,
     )
 
     wallet.submit_transaction(
         transaction=order_data,
-        name=wallet_name,
+        wallet_name=wallet_name,
         transaction_type="order_amendment",
         key_name=key_name,
     )
     logger.debug(f"Submitted Order amendment for {order_id}.")
 
 
 def cancel_order(
@@ -252,15 +252,15 @@
     order_data = order_cancellation(
         order_id=order_id,
         market_id=market_id,
     )
 
     wallet.submit_transaction(
         transaction=order_data,
-        name=wallet_name,
+        wallet_name=wallet_name,
         transaction_type="order_cancellation",
         key_name=key_name,
     )
 
     logger.debug(f"Cancelled order {order_id} on market {market_id}")
 
 
@@ -376,15 +376,15 @@
                 proportion=spec[2],
             )
             for spec in sell_specs
         ],
     )
     wallet.submit_transaction(
         transaction=submission,
-        name=wallet_name,
+        wallet_name=wallet_name,
         transaction_type=submission_name,
         key_name=key_name,
     )
     logger.debug(f"Submitted liquidity on market {market_id}")
 
 
 def pegged_order(
@@ -608,20 +608,21 @@
 
     command = vega_protos.commands.v1.commands.BatchMarketInstructions(
         submissions=submissions, amendments=amendments, cancellations=cancellations
     )
 
     wallet.submit_transaction(
         transaction=command,
-        name=wallet_name,
+        wallet_name=wallet_name,
         transaction_type="batch_market_instructions",
         key_name=key_name,
     )
     logger.debug(
-        f"Submitted a batch of {len(cancellations)} cancellation, {len(amendments)} amendment, and {len(submissions)} submission instructions."
+        f"Submitted a batch of {len(cancellations)} cancellation,"
+        f" {len(amendments)} amendment, and {len(submissions)} submission instructions."
     )
 
 
 def transfer(
     wallet: Wallet,
     wallet_name: str,
     key_name: str,
@@ -630,15 +631,14 @@
     to_account_type: vega_protos.vega.AccountType,
     asset: str,
     amount: str,
     reference: Optional[str] = None,
     one_off: Optional[vega_protos.commands.v1.commands.OneOffTransfer] = None,
     recurring: Optional[vega_protos.commands.v1.commands.RecurringTransfer] = None,
 ):
-
     command = vega_protos.commands.v1.commands.Transfer(
         from_account_type=from_account_type,
         to=to,
         to_account_type=to_account_type,
         asset=asset,
         amount=amount,
     )
@@ -656,13 +656,13 @@
         command.recurring.CopyFrom(recurring)
 
     else:
         command.one_off.CopyFrom(one_off)
 
     wallet.submit_transaction(
         transaction=command,
-        name=wallet_name,
+        wallet_name=wallet_name,
         transaction_type="transfer",
         key_name=key_name,
     )
 
     logger.debug(f"Submitted a transfer.")
```

### Comparing `vega_sim-0.67.0/vega_sim/environment/agent.py` & `vega_sim-1.0.1/vega_sim/environment/agent.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     def __init__(self, tag: Optional[str] = None):
         self.tag = tag
 
     def step(self, vega: VegaService):
         pass
 
     def initialise(
-        self, vega: VegaService, create_wallet: bool = False, mint_wallet: bool = False
+        self, vega: VegaService, create_key: bool = False, mint_key: bool = False
     ):
         self.vega = vega
 
     def finalise(self):
         pass
 
     def _update_state(self, current_step: int):
@@ -38,59 +38,53 @@
     def name_from_tag(cls, tag: Optional[str] = None) -> str:
         return cls.NAME_BASE + (f"_{tag}" if tag is not None else "")
 
 
 class AgentWithWallet(Agent):
     def __init__(
         self,
-        wallet_name: str,
-        wallet_pass: str,
+        key_name: str,
         tag: Optional[str] = None,
-        key_name: Optional[str] = None,
+        wallet_name: Optional[str] = None,
         state_update_freq: Optional[int] = None,
     ):
         """Agent for use in environments as specified in environment.py.
         To extend, the crucial function to implement is the step function which will
         be called on each timestep in the simulation.
 
         Additionally, the initialise function can be added to. This function is called
         once before the main simulation and can be used to creat assets, set up markets,
         faucet assets to the agent etc.
 
         Args:
-            wallet_name:
-                str, The name to use for this agent's wallet
+            key_name:
+                str, Name of key in wallet for agent to use.
             wallet_pass:
                 str, The password which this agent uses to log in to the wallet
             tag:
                 str, optional, additional tag to add to agent's wallet name
-            key_name:
-                str, optional, Name of key in wallet for agent to use. Defaults
-                to value in the environment variable "VEGA_DEFAULT_KEY_NAME".
+            wallet_name:
+                str, optional, The name to use for this agent's wallet
         """
         super().__init__(tag=tag)
         self.wallet_name = wallet_name
-        self.wallet_pass = wallet_pass
         self.key_name = key_name
 
         self.state_update_freq = state_update_freq
 
     def step(self):
         pass
 
-    def initialise(self, vega: VegaService, create_wallet: bool = True):
+    def initialise(self, vega: VegaService, create_key: bool = True):
         super().initialise(vega=vega)
-        if create_wallet:
-            self.vega.create_wallet(
-                name=self.wallet_name,
-                passphrase=self.wallet_pass,
-                key_name=self.key_name,
+        if create_key:
+            self.vega.create_key(
+                wallet_name=self.wallet_name,
+                name=self.key_name,
             )
-        else:
-            self.vega.login(name=self.wallet_name, passphrase=self.wallet_pass)
 
 
 class StateAgentWithWallet(AgentWithWallet):
     def step(self, vega_state: VegaState):
         super().step()
```

### Comparing `vega_sim-0.67.0/vega_sim/environment/environment.py` & `vega_sim-1.0.1/vega_sim/environment/environment.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,16 +39,20 @@
 
 MarketState = namedtuple(
     "MarketState",
     [
         "state",
         "trading_mode",
         "midprice",
+        "best_bid_price",
+        "best_ask_price",
+        "min_valid_price",
+        "max_valid_price",
         "orders",
-    ],  # "order_book"]
+    ],
 )
 
 
 class MarketEnvironment:
     def __init__(
         self,
         agents: List[Agent],
@@ -141,33 +145,34 @@
                 block_duration=f"{int(self.block_length_seconds)}s",
                 use_full_vega_wallet=False,
             ) as vega:
                 return self._run(vega, pause_at_completion=pause_at_completion)
         else:
             return self._run(self._vega, pause_at_completion=pause_at_completion)
 
-    def _start_order_monitoring(self, vega: VegaService):
-
+    def _start_live_feeds(self, vega: VegaService):
         # Get lists of unique market_ids and party_ids to observe
         market_ids = list(
             {
                 vega.find_market_id(name=agent.market_name)
                 for agent in self.agents
                 if hasattr(agent, "market_name")
             }
         )
         party_ids = list(
             {
-                vega.wallet.public_key(agent.wallet_name, agent.key_name)
+                vega.wallet.public_key(
+                    wallet_name=agent.wallet_name, name=agent.key_name
+                )
                 for agent in self.agents
-                if hasattr(agent, "wallet_name")
+                if hasattr(agent, "key_name")
             }
         )
         # Start order monitoring only observing scenario markets and parties
-        vega.start_order_monitoring(market_ids=market_ids, party_ids=party_ids)
+        vega.data_cache.start_live_feeds(market_ids=market_ids, party_ids=party_ids)
 
     def _run(
         self,
         vega: VegaServiceNull,
         pause_at_completion: bool = False,
     ) -> None:
         """Run the simulation with specified agents.
@@ -186,16 +191,14 @@
         start = datetime.datetime.now()
 
         for agent in self.agents:
             agent.initialise(vega=vega)
             if self.transactions_per_block > 1:
                 vega.wait_fn(1)
 
-        self._start_order_monitoring(vega=vega)
-
         start_time = vega.get_blockchain_time()
         for i in range(self.n_steps):
             self.step(vega)
 
             # Ensure core is caught up
             core_catchup_start = datetime.datetime.now()
             vega.wait_for_core_catchup()
@@ -327,25 +330,38 @@
         )
 
         self.state_func = (
             state_func if state_func is not None else self._default_state_extraction
         )
 
     def _default_state_extraction(self, vega: VegaService) -> VegaState:
+        if not hasattr(self, "market_decimals_cache"):
+            self.market_decimals_cache = {}
         market_state = {}
         order_status = vega.order_status_from_feed(live_only=True)
-        for market in vega.all_markets():
-            market_info = vega.market_info(market_id=market.id)
-            market_data = vega.market_data(market_id=market.id)
-            market_state[market.id] = MarketState(
-                state=market_info.state,
-                trading_mode=market_info.trading_mode,
+        for (
+            market_id,
+            market_data,
+        ) in vega.data_cache.market_data_from_feed_store.items():
+            if market_id not in self.market_decimals_cache:
+                self.market_decimals_cache[market_id] = vega.market_info(
+                    market_id=market_id
+                ).decimal_places
+            market_state[market_data.market] = MarketState(
+                state=market_data.market_state,
+                trading_mode=market_data.market_trading_mode,
                 midprice=float(market_data.mid_price)
-                / 10 ** int(market_info.decimal_places),
-                orders=order_status.get(market.id, {}),
+                / 10 ** int(self.market_decimals_cache[market_id]),
+                best_bid_price=float(market_data.best_bid_price)
+                / 10 ** self.market_decimals_cache[market_id],
+                best_ask_price=float(market_data.best_offer_price)
+                / 10 ** self.market_decimals_cache[market_id],
+                min_valid_price=vega.price_bounds(market_id=market_id)[0],
+                max_valid_price=vega.price_bounds(market_id=market_id)[1],
+                orders=order_status.get(market_data.market, {}),
             )
 
         return VegaState(network_state=(), market_state=market_state)
 
     def step(self, vega: VegaService) -> None:
         vega.wait_for_datanode_sync()
         state = self.state_func(vega)
@@ -381,48 +397,62 @@
         self.state_func = (
             state_func if state_func is not None else self._default_state_extraction
         )
 
         self.raise_datanode_errors = raise_datanode_errors
         self.raise_step_errors = raise_step_errors
 
-    def run(self):
+    def run(
+        self,
+        run_with_console: bool = False,
+        pause_at_completion: bool = False,
+    ):
         if self._vega is None:
             with VegaServiceNetwork(
                 use_full_vega_wallet=True,
                 run_with_wallet=True,
-                run_with_console=True,
+                run_with_console=run_with_console,
             ) as vega:
                 return self._run(vega)
         else:
-            return self._run(self._vega)
+            return self._run(self._vega, pause_at_completion=pause_at_completion)
 
-    def _run(self, vega: VegaServiceNetwork) -> None:
+    def _run(
+        self,
+        vega: VegaServiceNetwork,
+        pause_at_completion: bool = False,
+    ) -> None:
         # Initial datanode connection check
         vega.check_datanode(raise_on_error=self.raise_datanode_errors)
 
         # Initialise agents without minting assets
         for agent in self.agents:
-            agent.initialise(vega=vega, create_wallet=False, mint_wallet=False)
+            agent.initialise(vega=vega, create_key=False, mint_key=False)
 
-        self._start_order_monitoring(vega=vega)
+        self._start_live_feeds(vega=vega)
 
         i = 0
         # A negative self.n_steps will loop indefinitely
         while i != self.n_steps:
             vega.check_datanode(raise_on_error=self.raise_datanode_errors)
 
             i += 1
             self.step(vega)
 
             time.sleep(self.step_length_seconds)
 
         for agent in self.agents:
             agent.finalise()
 
+        if pause_at_completion:
+            input(
+                "Environment run completed. Pausing to allow inspection of state."
+                " Press Enter to continue"
+            )
+
     def step(self, vega: VegaServiceNetwork) -> None:
         t = time.time()
         state = self.state_func(vega)
         logging.debug(f"Get state took {time.time() - t} seconds.")
         for agent in (
             sorted(self.agents, key=lambda _: self.random_state.random())
             if self.random_agent_ordering
@@ -432,7 +462,127 @@
                 agent.step(state)
             except Exception as e:
                 msg = f"Agent '{agent.key_name}' failed to step."
                 if self.raise_step_errors:
                     raise e(msg)
                 else:
                     logging.warning(msg)
+
+
+class RealtimeMarketEnvironment(MarketEnvironmentWithState):
+    def __init__(
+        self,
+        agents: List[StateAgent],
+        random_agent_ordering: bool = True,
+        state_func: Optional[Callable[[VegaService], VegaState]] = None,
+        transactions_per_block: int = 1,
+        block_length_seconds: int = 1,
+        step_length_seconds: int = 1,
+        vega_service: Optional[VegaServiceNull] = None,
+        pause_every_n_steps: Optional[int] = None,
+        random_state: np.random.RandomState = None,
+    ):
+        """Set up a Vega protocol environment with some specified agents.
+        Handles the entire Vega setup and environment lifetime process, allowing the
+        user to focus on building the Agents themselves.
+
+        Once an environment has been created, calling the 'run' function will
+        run a complete simulation of the environment lifecycle. The realtime environment
+        aims to progress at a slower state, and so instead of running through all
+        actions and steps as fast as possible will sleep a configurable amount of
+        time between each block. Runs forever until cancelled.
+
+
+        Args:
+            agents:
+                List[StateAgent], a list of instantiated Agent objects which will
+                    interact with the environment
+            random_agent_ordering:
+                bool, default True, In each step, whether the order of agent
+                    steps should be randomised. If False, the order of agents
+                    passed in will be used
+            transactions_per_block:
+                int, default 1, How many transactions should be contained
+                    for each block in the Vega chain. Often this is best set
+                    as the maximum number of actions agents can take per step
+                    to ensure they all happen 'at the same time' per step.
+            block_length_seconds:
+                int, default 1, How many seconds each block on the Vega chain
+                    represents
+            step_length_seconds:
+                Optional[int], default None, How many seconds each step is
+                    taken to represent.
+                    After each round of actions, if time has not advanced at least
+                    this much we will be forwarded to that far in the future
+                    (minus however long the actions did take).
+                    e.g. for a step_length_seconds = 60 if all actions take up 10s
+                    we will forward 50s at the end.
+            vega_service:
+                optional, VegaServiceNull, If passed will use this precreated vega
+                    service instead of creating one internally.
+            pause_every_n_steps:
+                Optional[int], default None, If passed, simulation will pause every
+                    time the passed number of steps elapses waiting on user to press
+                    return. Allows inspection of the simulation at given frequency
+        """
+        super().__init__(
+            agents=agents,
+            n_steps=0,
+            random_agent_ordering=random_agent_ordering,
+            transactions_per_block=transactions_per_block,
+            block_length_seconds=block_length_seconds,
+            step_length_seconds=step_length_seconds,
+            vega_service=vega_service,
+            pause_every_n_steps=pause_every_n_steps,
+            random_state=random_state,
+            state_func=(
+                state_func if state_func is not None else self._default_state_extraction
+            ),
+        )
+
+    def step(self, vega: VegaService) -> None:
+        state = self.state_func(vega)
+        vega.wait_fn(1)
+        for agent in (
+            sorted(self.agents, key=lambda _: self.random_state.random())
+            if self.random_agent_ordering
+            else self.agents
+        ):
+            agent.step(state)
+
+    def _run(
+        self,
+        vega: VegaServiceNull,
+        pause_at_completion: bool = False,
+    ) -> None:
+        """Run the simulation with specified agents.
+
+        Args:
+            pause_at_completion:
+                bool, default False, If True will pause with a keypress-prompt
+                    once the simulation has completed, allowing the final state
+                    to be inspected, either via code or the Console
+        """
+        logger.info(f"Running wallet at: {vega.wallet_url}")
+        logger.info(
+            f"Running graphql at: http://localhost:{vega.data_node_graphql_port}"
+        )
+
+        for agent in self.agents:
+            agent.initialise(vega=vega)
+            if self.transactions_per_block > 1:
+                vega.wait_fn(1)
+
+        i = 1
+        while True:
+            i += 1
+            self.step(vega)
+
+            if (
+                self._pause_every_n_steps is not None
+                and i % self._pause_every_n_steps == 0
+            ):
+                input(
+                    f"Environment run at step {i}. Pausing to allow inspection of"
+                    " state. Press Enter to continue"
+                )
+            time.sleep(self.step_length_seconds)
```

### Comparing `vega_sim-0.67.0/vega_sim/grpc/client.py` & `vega_sim-1.0.1/vega_sim/grpc/client.py`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/network_service.py` & `vega_sim-1.0.1/vega_sim/network_service.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,21 @@
 This module contains functions and classes for the creation of the
 VegaServiceNetwork class. A VegaServiceNetwork object can be used to
 communicate with either a public or internal Vega network and run a
 Vega Wallet service for communication with the chosen Vega network.
 The VegaServiceNetwork inherits properties and methods from the VegaService
 class. Inherited methods can be used to communicate with the Vega datanode
 and Vega wallet services. Redundant properties and methods are overwritten.
+
+A vegawallet executable should either be in PATH whilst executing, or 
+the VEGA_WALLET_PATH environment variable set to a location of a wallet.
+
+Similarly, specify VEGA_NETWORK_CONFIG for the path to the network config
+of your chosen network
+
 Example:
 
     For an example, try running the below command. It will create a
     VegaServiceNetwork object, the relevant services and try sending some
     commands.
 
         $ python -m vega_sim.network_service
@@ -67,19 +74,20 @@
 
     Raises:
         ValueError:
             If no file exists at the specified path.
     """
 
     if not path.exists(network_config_path):
-        raise ValueError(f"No network config file at the specified path.")
+        raise ValueError("No network config file at the specified path.")
+
+    vega_wallet_path = environ.get("VEGA_WALLET_PATH", "vegawallet")
 
     args = [
-        "vega",
-        "wallet",
+        vega_wallet_path,
         "network",
         "import",
         "--from-file",
         network_config_path,
         "--force",
     ]
 
@@ -97,18 +105,18 @@
     log_dir: Optional[str] = None,
 ):
     processes = []
 
     tmp_vega_dir = tempfile.mkdtemp(prefix="vega-sim-") if log_dir is None else log_dir
 
     if run_with_wallet:
+        vega_wallet_path = environ.get("VEGA_WALLET_PATH", "vegawallet")
         vegaWalletProcess = _popen_process(
             popen_args=[
-                "vega",
-                "wallet",
+                vega_wallet_path,
                 "service",
                 "run",
                 "--network",
                 network,
                 "--automatic-consent",
                 "--no-version-check",
             ],
@@ -153,50 +161,139 @@
         return_code = process.poll()
         if return_code is not None:
             continue
         time.sleep(5)
         process.kill()
 
 
+def _find_network_config_toml(
+    network: Network, config_path: Optional[str] = None
+) -> Optional[str]:
+    search_paths = (
+        [config_path]
+        if config_path is not None
+        else [
+            path.join(
+                getcwd(),
+                "vega_sim",
+                "bin",
+                "networks-internal",
+                network.name.lower(),
+            ),
+            path.join(
+                getcwd(),
+                "vega_sim",
+                "bin",
+                "networks",
+                network.name.lower(),
+            ),
+        ]
+    )
+    for search_path in search_paths:
+        full_path = path.join(
+            search_path,
+            f"{network.value}.toml",
+        )
+
+        if path.exists(full_path):
+            return full_path
+
+
 class VegaServiceNetwork(VegaService):
     """Class for handling services for communicating with a Vega network."""
 
     def __init__(
         self,
         network: Network,
         run_with_wallet: bool = True,
         run_with_console: bool = True,
-        start_live_feeds: bool = True,
+        vega_console_path: Optional[str] = None,
+        network_config_path: Optional[str] = None,
+        wallet_path: Optional[str] = None,
+        vega_home_path: Optional[str] = None,
+        wallet_token_path: Optional[str] = None,
     ):
         """Method initialises the class.
 
         Args:
             network (Network):
                 Defines which network to connect service to.
             run_with_wallet (bool, optional):
                 Defines whether to start a wallet process.
             run_with_console (bool, optional):
                 Defines whether to start a console process.
+            vega_console_path (str, optional):
+                Path to the directory containing console files if
+                wishing to run a local console
+            network_config_path (str, optional):
+                Path to the directory containing network config files.
+                If not passed will search first the environment variable
+                VEGA_NETWORK_CONFIG then two default paths.
+                Note: Only needed if creating keys
+            vega_home_path (str, optional):
+                Path to the directory containing wallet binary. Otherwise
+                uses VEGA_HOME environment variable.
+                Note: Only needed if creating keys
+            wallet_token_path (str, optional):
+                Path to the json file containing wallet tokens. Otherwise
+                uses VEGA_WALLET_TOKEN environment variable.
         """
 
         # Run init method inherited from VegaService with network arguments.
         super().__init__(can_control_time=False, warn_on_raw_data_access=False)
 
         self.network = network
         self.run_with_wallet = run_with_wallet
         self.run_with_console = run_with_console
-        self._start_live_feeds = start_live_feeds
 
         self._wallet = None
         self._wallet_url = None
         self._data_node_grpc_url = None
         self._data_node_query_url = None
         self._network_config = None
 
-        self.vega_console_path = path.join(vega_bin_path, "console")
+        self.vega_console_path = (
+            vega_console_path
+            if vega_console_path is not None
+            else path.join(vega_bin_path, "console")
+        )
+        self._base_network_config_path = (
+            network_config_path
+            if network_config_path is not None
+            else environ.get("VEGA_NETWORK_CONFIG")
+        )
+
+        self._wallet_path = (
+            wallet_path
+            if wallet_path is not None
+            else environ.get("VEGA_WALLET_PATH", "vegawallet")
+        )
+
+        self._vega_home = (
+            vega_home_path if vega_home_path is not None else environ.get("VEGA_HOME")
+        )
+
+        self._token_path = (
+            wallet_token_path
+            if wallet_token_path is not None
+            else environ.get("VEGA_WALLET_TOKEN")
+        )
+        if self._token_path is None:
+            raise Exception(
+                "Either path to tokens JSON must be passed to wallet class or"
+                " VEGA_WALLET_TOKEN environment variable set"
+            )
+
+        self._network_config_path = _find_network_config_toml(
+            network=self.network, config_path=self._base_network_config_path
+        )
+        if self._network_config_path is None:
+            raise ValueError(
+                f"ERROR! {self.network.name.lower()} network config could not be found"
+            )
 
         self.log_dir = tempfile.mkdtemp(prefix="vega-sim-")
 
     def __enter__(self):
         """Defines behaviour when class entered by a with statement."""
         self.start()
 
@@ -227,17 +324,14 @@
         if self.run_with_console:
             logger.info(
                 "Vega Running. Console launched at"
                 f" http://localhost:{vega_console_port}"
             )
             webbrowser.open(f"http://localhost:{vega_console_port}/", new=2)
 
-        if self._start_live_feeds:
-            self.start_order_monitoring()
-
     def stop(self) -> None:
         super().stop()
         if self.proc is None:
             logger.info("Stop called but nothing to stop")
         else:
             self.proc.terminate()
 
@@ -268,44 +362,16 @@
             "Parent method overridden as VegaNetworkService incapable of controlling"
             " time."
         )
 
     @property
     def network_config(self) -> dict:
         if self._network_config is None:
-            public_path = path.join(
-                getcwd(),
-                "vega_sim",
-                "bin",
-                "networks-internal",
-                self.network.name.lower(),
-                f"{self.network.value}.toml",
-            )
-            internal_path = path.join(
-                getcwd(),
-                "vega_sim",
-                "bin",
-                "networks",
-                self.network.name.lower(),
-                f"{self.network.value}.toml",
-            )
-
-            if path.exists(public_path):
-                self._network_config = toml.load(public_path)
-                add_network_config(public_path)
-
-            elif path.exists(internal_path):
-                self._network_config = toml.load(internal_path)
-                add_network_config(internal_path)
-
-            else:
-                raise ValueError(
-                    f"ERROR! {self.network.name.lower()} network does not exist"
-                )
-
+            self._network_config = toml.load(self._network_config_path)
+            add_network_config(self._network_config_path)
         return self._network_config
 
     @property
     def data_node_grpc_url(self) -> str:
         if self._data_node_grpc_url is None:
             url = self.network_config["API"]["GRPC"]["Hosts"][0]
             self._data_node_grpc_url = f"{url.split(':')[0]}:{DATA_NODE_GRPC_PORT}"
@@ -325,15 +391,20 @@
                 f"http://{self.network_config['Host']}:{self.network_config['Port']}"
             )
         return self._wallet_url
 
     @property
     def wallet(self) -> Wallet:
         if self._wallet is None:
-            self._wallet = VegaWallet(self.wallet_url)
+            self._wallet = VegaWallet.from_json(
+                self._token_path,
+                self.wallet_url,
+                wallet_path=self._wallet_path,
+                vega_home_dir=self._vega_home,
+            )
         return self._wallet
 
     @property
     def core_state_client(self) -> None:
         logging.debug(
             (
                 "Parent property overridden as VegaNetworkService does not need a core"
```

### Comparing `vega_sim-0.67.0/vega_sim/null_service.py` & `vega_sim-1.0.1/vega_sim/null_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 from __future__ import annotations
 
 import atexit
 import functools
-from io import BufferedWriter
 import logging
 import multiprocessing
 import os
 import shutil
 import signal
 import socket
 import subprocess
 import tempfile
 import time
 import webbrowser
 from collections import namedtuple
 from contextlib import closing
 from enum import Enum, auto
+from io import BufferedWriter
 from os import path
 from typing import Dict, List, Optional, Set
 
 import requests
 import toml
 from urllib3.exceptions import MaxRetryError
 
 from vega_sim import vega_bin_path, vega_home_path
 from vega_sim.service import VegaService
-from vega_sim.wallet.base import Wallet
-from vega_sim.wallet.slim_wallet import (
-    SlimWallet,
-)
+from vega_sim.tools.load_binaries import download_binaries
+from vega_sim.wallet.base import DEFAULT_WALLET_NAME, Wallet
+from vega_sim.wallet.slim_wallet import SlimWallet
 from vega_sim.wallet.vega_wallet import VegaWallet
 
 logger = logging.getLogger(__name__)
 
 PortUpdateConfig = namedtuple(
     "PortUpdateConfig", ["file_path", "config_path", "key", "val_func"]
 )
@@ -100,14 +99,20 @@
     Ports.FAUCET: [
         PortUpdateConfig(
             ("config", "faucet", "config.toml"), [], "Port", lambda port: port
         ),
     ],
     Ports.WALLET: [
         PortUpdateConfig(
+            ("config", "wallet-service", "config.toml"),
+            ["Server"],
+            "Port",
+            lambda port: port,
+        ),
+        PortUpdateConfig(
             ("config", "wallet-service", "networks", "local.toml"),
             [],
             "Port",
             lambda port: port,
         ),
     ],
     Ports.VEGA_NODE: [
@@ -334,14 +339,24 @@
     logger.info(f"Running NullChain from vegahome of {tmp_vega_dir}")
     if port_config.get(Ports.DATA_NODE_GRAPHQL):
         logger.info(
             f"Launching GraphQL node at port {port_config.get(Ports.DATA_NODE_GRAPHQL)}"
         )
     if port_config.get(Ports.CONSOLE):
         logger.info(f"Launching Console at port {port_config.get(Ports.CONSOLE)}")
+    if port_config.get(Ports.DATA_NODE_REST):
+        logger.info(
+            f"Launching Datanode REST at port {port_config.get(Ports.DATA_NODE_REST)}"
+        )
+    if port_config.get(Ports.DATA_NODE_GRPC):
+        logger.info(
+            f"Launching Datanode GRPC at port {port_config.get(Ports.DATA_NODE_GRPC)}"
+        )
+    if port_config.get(Ports.CORE_GRPC):
+        logger.info(f"Launching Core GRPC at port {port_config.get(Ports.CORE_GRPC)}")
 
     dest_dir = f"{tmp_vega_dir}/vegahome"
     shutil.copytree(vega_home_path, dest_dir)
     for dirpath, _, filenames in os.walk(dest_dir):
         os.utime(dirpath, None)
         for file in filenames:
             os.utime(os.path.join(dirpath, file), None)
@@ -424,22 +439,52 @@
                 break
             except (
                 MaxRetryError,
                 requests.exceptions.ConnectionError,
                 requests.exceptions.HTTPError,
             ):
                 time.sleep(0.1)
+
+        subprocess.Popen(
+            [
+                vega_wallet_path,
+                "api-token",
+                "init",
+                f"--home={tmp_vega_home}",
+                f"--passphrase-file={tmp_vega_home}/passphrase-file",
+            ],
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+        )
+
+        subprocess.Popen(
+            [
+                vega_wallet_path,
+                "api-token",
+                "generate",
+                "--home=" + tmp_vega_home,
+                "--tokens-passphrase-file=" + tmp_vega_home + "/passphrase-file",
+                "--wallet-passphrase-file=" + tmp_vega_home + "/passphrase-file",
+                "--wallet-name=" + DEFAULT_WALLET_NAME,
+                "--description=" + DEFAULT_WALLET_NAME,
+            ],
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+        )
+
         wallet_args = [
             vega_wallet_path,
             "service",
             "run",
             "--network",
             "local",
             "--home=" + tmp_vega_home,
             "--automatic-consent",
+            "--load-tokens",
+            "--tokens-passphrase-file=" + tmp_vega_home + "/passphrase-file",
         ]
 
         vegaWalletProcess = _popen_process(
             wallet_args,
             dir_root=tmp_vega_dir,
             log_name="vegawallet",
         )
@@ -517,27 +562,32 @@
         run_with_console: bool = False,
         run_wallet_with_token_dapp: bool = False,
         port_config: Optional[Dict[Ports, int]] = None,
         warn_on_raw_data_access: bool = True,
         transactions_per_block: int = 1,
         seconds_per_block: int = 1,
         use_full_vega_wallet: bool = False,
-        start_live_feeds: bool = True,
         retain_log_files: bool = False,
         launch_graphql: bool = False,
         store_transactions: bool = True,
         replay_from_path: Optional[str] = None,
+        listen_for_high_volume_stream_updates: bool = False,
+        check_for_binaries: bool = False,
     ):
         super().__init__(
             can_control_time=True,
             warn_on_raw_data_access=warn_on_raw_data_access,
             seconds_per_block=seconds_per_block,
+            listen_for_high_volume_stream_updates=listen_for_high_volume_stream_updates,
         )
         self.retain_log_files = retain_log_files
 
+        self._using_all_custom_paths = all(
+            [x is not None for x in [vega_path, data_node_path, vega_wallet_path]]
+        )
         self.vega_path = vega_path or path.join(vega_bin_path, "vega")
         self.data_node_path = data_node_path or path.join(vega_bin_path, "data-node")
         self.vega_wallet_path = vega_wallet_path or path.join(
             vega_bin_path, "vegawallet"
         )
         self.vega_console_path = vega_console_path or path.join(
             vega_bin_path, "console"
@@ -551,17 +601,17 @@
 
         self._wallet = None
         self._use_full_vega_wallet = use_full_vega_wallet
         self.store_transactions = store_transactions
 
         self.log_dir = tempfile.mkdtemp(prefix="vega-sim-")
 
-        self._start_live_feeds = start_live_feeds
         self.launch_graphql = launch_graphql
         self.replay_from_path = replay_from_path
+        self.check_for_binaries = check_for_binaries
 
         if port_config is None:
             self._assign_ports()
         else:
             for key, name in self.PORT_TO_FIELD_MAP.items():
                 setattr(self, name, port_config[key])
 
@@ -580,21 +630,26 @@
         self.forward(f"{int(wait_multiple * self.seconds_per_block)}s")
         self.wait_for_core_catchup()
 
     @property
     def wallet(self) -> Wallet:
         if self._wallet is None:
             if self._use_full_vega_wallet:
-                self._wallet = VegaWallet(self.wallet_url)
+                self._wallet = VegaWallet(
+                    self.wallet_url,
+                    wallet_path=self.vega_wallet_path,
+                    vega_home_dir=path.join(self.log_dir, "vegahome"),
+                    passphrase_file_path=path.join(
+                        self.log_dir, "vegahome", "passphrase-file"
+                    ),
+                )
             else:
                 self._wallet = SlimWallet(
                     self.core_client,
-                    full_wallet=VegaWallet(self.wallet_url)
-                    if self.run_with_console
-                    else None,
+                    full_wallet=None,
                     log_dir=self.log_dir,
                 )
         return self._wallet
 
     def _assign_ports(self):
         self.wallet_port = 0
         self.data_node_rest_port = 0
@@ -627,28 +682,31 @@
             Ports.VEGA_NODE: self.vega_node_port,
             Ports.CORE_GRPC: self.vega_node_grpc_port,
             Ports.CORE_REST: self.vega_node_rest_port,
             Ports.CONSOLE: self.console_port,
         }
 
     def start(self, block_on_startup: bool = True) -> None:
+        if self.check_for_binaries and not self._using_all_custom_paths:
+            download_binaries()
+
         ctx = multiprocessing.get_context()
         port_config = self._generate_port_config()
         self.proc = ctx.Process(
             target=manage_vega_processes,
             kwargs={
                 "vega_path": self.vega_path,
                 "data_node_path": self.data_node_path,
                 "vega_wallet_path": self.vega_wallet_path,
                 "vega_console_path": self.vega_console_path,
                 "run_with_console": self.run_with_console,
                 "port_config": port_config,
                 "transactions_per_block": self.transactions_per_block,
                 "block_duration": f"{int(self.seconds_per_block)}s",
-                "run_wallet": self._use_full_vega_wallet or self.run_with_console,
+                "run_wallet": self._use_full_vega_wallet,
                 "retain_log_files": self.retain_log_files,
                 "log_dir": self.log_dir,
                 "store_transactions": self.store_transactions,
                 "replay_from_path": self.replay_from_path,
             },
         )
         self.proc.start()
@@ -666,17 +724,17 @@
                 try:
                     requests.get(
                         f"http://localhost:{self.data_node_rest_port}/time"
                     ).raise_for_status()
                     requests.get(
                         f"http://localhost:{self.vega_node_rest_port}/blockchain/height"
                     ).raise_for_status()
-                    if self.run_with_console or self._use_full_vega_wallet:
+                    if self._use_full_vega_wallet:
                         requests.get(
-                            f"http://localhost:{self.wallet_port}/api/v1/status"
+                            f"http://localhost:{self.wallet_port}/api/v2/health"
                         ).raise_for_status()
 
                     started = True
                     break
                 except (
                     MaxRetryError,
                     requests.exceptions.ConnectionError,
@@ -692,17 +750,14 @@
             webbrowser.open(f"http://localhost:{port_config[Ports.CONSOLE]}/", new=2)
 
         if self.launch_graphql:
             webbrowser.open(
                 f"http://localhost:{port_config[Ports.DATA_NODE_GRAPHQL]}/", new=2
             )
 
-        if self._start_live_feeds:
-            self.start_live_feeds()
-
     # Class internal as at some point the host may vary as well as the port
     @staticmethod
     def _build_url(port: int, prefix: str = "http://"):
         return f"{prefix}localhost:{port}"
 
     def stop(self) -> None:
         super().stop()
```

### Comparing `vega_sim-0.67.0/vega_sim/parameter_test/parameter/configs.py` & `vega_sim-1.0.1/vega_sim/parameter_test/parameter/configs.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     ],
 )
 
 TAU_SCALING_FACTOR = SingleParameterExperiment(
     name="TauScalingFactor",
     parameter_type="network",
     parameter_to_vary="market.liquidity.probabilityOfTrading.tau.scaling",
-    values=["1", "10", "100"],
+    values=["10", "100", "1000"],
     scenario=ParameterExperiment(
         state_extraction_fn=ideal_market_maker_single_data_extraction(
             additional_data_fns=[
                 tau_scaling_additional_data,
                 target_stake_additional_data,
                 limit_order_book,
             ]
@@ -83,13 +83,12 @@
     },
     data_extraction=[
         (FILE_PATTERN, BASE_IDEAL_MM_CSV_HEADERS),
         (FILE_PATTERN_LOB, LOB_CSV_HEADERS),
     ],
 )
 
-
 CONFIGS = [
     TARGET_STAKE_SCALING_FACTOR,
     TAU_SCALING_FACTOR,
     BOND_PENALTY_PARAMETER,
 ]
```

### Comparing `vega_sim-0.67.0/vega_sim/parameter_test/parameter/experiment.py` & `vega_sim-1.0.1/vega_sim/parameter_test/parameter/experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     with VegaServiceNull(
         warn_on_raw_data_access=False,
         retain_log_files=True,
         run_with_console=False,
         transactions_per_block=100,
         use_full_vega_wallet=False,
     ) as vega:
-        vega.create_wallet(*PARAMETER_AMEND_WALLET)
+        vega.create_key(PARAMETER_AMEND_WALLET[0])
         vega.mint(
             PARAMETER_AMEND_WALLET[0],
             asset="VOTE",
             amount=1e4,
         )
 
         # Update additional network parameters and the parameter to vary if running a
```

### Comparing `vega_sim-0.67.0/vega_sim/parameter_test/parameter/loggers.py` & `vega_sim-1.0.1/vega_sim/parameter_test/parameter/loggers.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,16 @@
     "LP: Relative Return",
     "LP: Annualised Relative Return",
     "LP: RealisedPnl",
     "LP: UnrealisedPnl",
     "LP: Position",
     "LP: Bid",
     "LP: Ask",
+    "LP: Received Liquidity Fees",
+    "LP: Liquidity Fee Shares",
     "External Midprice",
     "Midprice",
     "Markprice",
     "LP: entry price",
     "InsurancePool",
     "LiquifeeAccount",
     "InfrafeeAccount",
@@ -93,14 +95,31 @@
     general_lp, margin_lp, bond_lp = vega.party_account(
         wallet_name=mm_agent.wallet_name,
         asset_id=mm_agent.asset_id,
         market_id=mm_agent.market_id,
         key_name=mm_agent.key_name,
     )
 
+    received_liquidity_fees_lp = 0
+    for ledger_entry in vega.list_ledger_entries(
+        to_party_ids=[
+            vega.wallet.public_key(
+                wallet_name=mm_agent.wallet_name, name=mm_agent.key_name
+            )
+        ],
+        transfer_types=[14],
+    ):
+        received_liquidity_fees_lp += ledger_entry.quantity
+
+    liquidity_fee_shares = vega.get_liquidity_fee_shares(
+        market_id=mm_agent.market_id,
+        wallet_name=mm_agent.wallet_name,
+        key_name=mm_agent.key_name,
+    )
+
     position = vega.positions_by_market(
         wallet_name=mm_agent.wallet_name,
         market_id=mm_agent.market_id,
         key_name=mm_agent.key_name,
     )
     if position is None:
         realised_pnl_lp = 0
@@ -186,14 +205,16 @@
         "LP: Position": inventory_lp,
         "LP: Bid": -round(mm_agent.bid_depth, mm_agent.mdp)
         if mm_agent.bid_depth is not None
         else None,
         "LP: Ask": round(mm_agent.ask_depth, mm_agent.mdp)
         if mm_agent.ask_depth is not None
         else None,
+        "LP: Received Liquidity Fees": received_liquidity_fees_lp,
+        "LP: Liquidity Fee Shares": liquidity_fee_shares,
         "External Midprice": mm_agent.price_process[mm_agent.current_step - 1]
         if hasattr(mm_agent, "price_process")
         else None,
         "Midprice": mid_price,
         "Markprice": markprice,
         "LP: entry price": entry_price,
         "InsurancePool": insurance,
```

### Comparing `vega_sim-0.67.0/vega_sim/parameter_test/run.py` & `vega_sim-1.0.1/vega_sim/parameter_test/run.py`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/proto/blockexplorer/blockexplorer_pb2.py` & `vega_sim-1.0.1/vega_sim/proto/blockexplorer/blockexplorer_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,25 +20,24 @@
 )
 from protoc_gen_openapiv2.options import (
     annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2,
 )
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n!blockexplorer/blockexplorer.proto\x12\x14\x62lockexplorer.api.v1\x1a"vega/commands/v1/transaction.proto\x1a vega/commands/v1/signature.proto\x1a.protoc-gen-openapiv2/options/annotations.proto"\r\n\x0bInfoRequest"I\n\x0cInfoResponse\x12\x18\n\x07version\x18\x01 \x01(\tR\x07version\x12\x1f\n\x0b\x63ommit_hash\x18\x02 \x01(\tR\ncommitHash"+\n\x15GetTransactionRequest\x12\x12\n\x04hash\x18\x01 \x01(\tR\x04hash"]\n\x16GetTransactionResponse\x12\x43\n\x0btransaction\x18\x01 \x01(\x0b\x32!.blockexplorer.api.v1.TransactionR\x0btransaction"\x8e\x02\n\x17ListTransactionsRequest\x12\x14\n\x05limit\x18\x01 \x01(\rR\x05limit\x12\x1b\n\x06\x62\x65\x66ore\x18\x02 \x01(\tH\x00R\x06\x62\x65\x66ore\x88\x01\x01\x12\x19\n\x05\x61\x66ter\x18\x03 \x01(\tH\x01R\x05\x61\x66ter\x88\x01\x01\x12T\n\x07\x66ilters\x18\x04 \x03(\x0b\x32:.blockexplorer.api.v1.ListTransactionsRequest.FiltersEntryR\x07\x66ilters\x1a:\n\x0c\x46iltersEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x42\t\n\x07_beforeB\x08\n\x06_after"a\n\x18ListTransactionsResponse\x12\x45\n\x0ctransactions\x18\x03 \x03(\x0b\x32!.blockexplorer.api.v1.TransactionR\x0ctransactions"\xc2\x02\n\x0bTransaction\x12\x14\n\x05\x62lock\x18\x01 \x01(\x04R\x05\x62lock\x12\x14\n\x05index\x18\x02 \x01(\rR\x05index\x12\x12\n\x04hash\x18\x03 \x01(\tR\x04hash\x12\x1c\n\tsubmitter\x18\x04 \x01(\tR\tsubmitter\x12\x12\n\x04type\x18\x05 \x01(\tR\x04type\x12\x12\n\x04\x63ode\x18\x06 \x01(\rR\x04\x63ode\x12\x16\n\x06\x63ursor\x18\x07 \x01(\tR\x06\x63ursor\x12\x35\n\x07\x63ommand\x18\x08 \x01(\x0b\x32\x1b.vega.commands.v1.InputDataR\x07\x63ommand\x12\x39\n\tsignature\x18\t \x01(\x0b\x32\x1b.vega.commands.v1.SignatureR\tsignature\x12\x19\n\x05\x65rror\x18\n \x01(\tH\x00R\x05\x65rror\x88\x01\x01\x42\x08\n\x06_error2\xc9\x02\n\x14\x42lockExplorerService\x12m\n\x0eGetTransaction\x12+.blockexplorer.api.v1.GetTransactionRequest\x1a,.blockexplorer.api.v1.GetTransactionResponse"\x00\x12s\n\x10ListTransactions\x12-.blockexplorer.api.v1.ListTransactionsRequest\x1a..blockexplorer.api.v1.ListTransactionsResponse"\x00\x12M\n\x04Info\x12!.blockexplorer.api.v1.InfoRequest\x1a".blockexplorer.api.v1.InfoResponseBxZ5code.vegaprotocol.io/vega/protos/blockexplorer/api/v1\x92\x41>\x12#\n\x18Vega block explorer APIs2\x07v0.67.0\x1a\x13lb.testnet.vega.xyz*\x02\x01\x02\x62\x06proto3'
+    b'\n!blockexplorer/blockexplorer.proto\x12\x14\x62lockexplorer.api.v1\x1a"vega/commands/v1/transaction.proto\x1a vega/commands/v1/signature.proto\x1a.protoc-gen-openapiv2/options/annotations.proto"\r\n\x0bInfoRequest"I\n\x0cInfoResponse\x12\x18\n\x07version\x18\x01 \x01(\tR\x07version\x12\x1f\n\x0b\x63ommit_hash\x18\x02 \x01(\tR\ncommitHash"+\n\x15GetTransactionRequest\x12\x12\n\x04hash\x18\x01 \x01(\tR\x04hash"]\n\x16GetTransactionResponse\x12\x43\n\x0btransaction\x18\x01 \x01(\x0b\x32!.blockexplorer.api.v1.TransactionR\x0btransaction"\x8e\x02\n\x17ListTransactionsRequest\x12\x14\n\x05limit\x18\x01 \x01(\rR\x05limit\x12\x1b\n\x06\x62\x65\x66ore\x18\x02 \x01(\tH\x00R\x06\x62\x65\x66ore\x88\x01\x01\x12\x19\n\x05\x61\x66ter\x18\x03 \x01(\tH\x01R\x05\x61\x66ter\x88\x01\x01\x12T\n\x07\x66ilters\x18\x04 \x03(\x0b\x32:.blockexplorer.api.v1.ListTransactionsRequest.FiltersEntryR\x07\x66ilters\x1a:\n\x0c\x46iltersEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x42\t\n\x07_beforeB\x08\n\x06_after"a\n\x18ListTransactionsResponse\x12\x45\n\x0ctransactions\x18\x03 \x03(\x0b\x32!.blockexplorer.api.v1.TransactionR\x0ctransactions"\xc2\x02\n\x0bTransaction\x12\x14\n\x05\x62lock\x18\x01 \x01(\x04R\x05\x62lock\x12\x14\n\x05index\x18\x02 \x01(\rR\x05index\x12\x12\n\x04hash\x18\x03 \x01(\tR\x04hash\x12\x1c\n\tsubmitter\x18\x04 \x01(\tR\tsubmitter\x12\x12\n\x04type\x18\x05 \x01(\tR\x04type\x12\x12\n\x04\x63ode\x18\x06 \x01(\rR\x04\x63ode\x12\x16\n\x06\x63ursor\x18\x07 \x01(\tR\x06\x63ursor\x12\x35\n\x07\x63ommand\x18\x08 \x01(\x0b\x32\x1b.vega.commands.v1.InputDataR\x07\x63ommand\x12\x39\n\tsignature\x18\t \x01(\x0b\x32\x1b.vega.commands.v1.SignatureR\tsignature\x12\x19\n\x05\x65rror\x18\n \x01(\tH\x00R\x05\x65rror\x88\x01\x01\x42\x08\n\x06_error2\xc9\x02\n\x14\x42lockExplorerService\x12m\n\x0eGetTransaction\x12+.blockexplorer.api.v1.GetTransactionRequest\x1a,.blockexplorer.api.v1.GetTransactionResponse"\x00\x12s\n\x10ListTransactions\x12-.blockexplorer.api.v1.ListTransactionsRequest\x1a..blockexplorer.api.v1.ListTransactionsResponse"\x00\x12M\n\x04Info\x12!.blockexplorer.api.v1.InfoRequest\x1a".blockexplorer.api.v1.InfoResponseB|Z5code.vegaprotocol.io/vega/protos/blockexplorer/api/v1\x92\x41\x42\x12\'\n\x18Vega block explorer APIs2\x0bv0.68.0-dev\x1a\x13lb.testnet.vega.xyz*\x02\x01\x02\x62\x06proto3'
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(
     DESCRIPTOR, "blockexplorer.blockexplorer_pb2", globals()
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
-    DESCRIPTOR._serialized_options = b"Z5code.vegaprotocol.io/vega/protos/blockexplorer/api/v1\222A>\022#\n\030Vega block explorer APIs2\007v0.67.0\032\023lb.testnet.vega.xyz*\002\001\002"
+    DESCRIPTOR._serialized_options = b"Z5code.vegaprotocol.io/vega/protos/blockexplorer/api/v1\222AB\022'\n\030Vega block explorer APIs2\013v0.68.0-dev\032\023lb.testnet.vega.xyz*\002\001\002"
     _LISTTRANSACTIONSREQUEST_FILTERSENTRY._options = None
     _LISTTRANSACTIONSREQUEST_FILTERSENTRY._serialized_options = b"8\001"
     _INFOREQUEST._serialized_start = 177
     _INFOREQUEST._serialized_end = 190
     _INFORESPONSE._serialized_start = 192
     _INFORESPONSE._serialized_end = 265
     _GETTRANSACTIONREQUEST._serialized_start = 267
```

### Comparing `vega_sim-0.67.0/vega_sim/proto/blockexplorer/blockexplorer_pb2_grpc.py` & `vega_sim-1.0.1/vega_sim/proto/blockexplorer/blockexplorer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/proto/data_node/api/v2/trading_data_pb2.py` & `vega_sim-1.0.1/vega_sim/proto/data_node/api/v2/trading_data_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,35 +23,42 @@
 )
 from protoc_gen_openapiv2.options import (
     annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2,
 )
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n#data-node/api/v2/trading_data.proto\x12\x0f\x64\x61tanode.api.v2\x1a\x0fvega/vega.proto\x1a\x15vega/governance.proto\x1a\x12vega/markets.proto\x1a\x11vega/assets.proto\x1a\x11vega/oracle.proto\x1a\x1bvega/events/v1/events.proto\x1a)vega/commands/v1/validator_commands.proto\x1a.protoc-gen-openapiv2/options/annotations.proto"\\\n\x10OffsetPagination\x12\x12\n\x04skip\x18\x01 \x01(\x04R\x04skip\x12\x14\n\x05limit\x18\x02 \x01(\x04R\x05limit\x12\x1e\n\ndescending\x18\x03 \x01(\x08R\ndescending"\xd9\x01\n\nPagination\x12\x19\n\x05\x66irst\x18\x01 \x01(\x05H\x00R\x05\x66irst\x88\x01\x01\x12\x19\n\x05\x61\x66ter\x18\x02 \x01(\tH\x01R\x05\x61\x66ter\x88\x01\x01\x12\x17\n\x04last\x18\x03 \x01(\x05H\x02R\x04last\x88\x01\x01\x12\x1b\n\x06\x62\x65\x66ore\x18\x04 \x01(\tH\x03R\x06\x62\x65\x66ore\x88\x01\x01\x12&\n\x0cnewest_first\x18\x05 \x01(\x08H\x04R\x0bnewestFirst\x88\x01\x01\x42\x08\n\x06_firstB\x08\n\x06_afterB\x07\n\x05_lastB\t\n\x07_beforeB\x0f\n\r_newest_first"\x9c\x01\n\x08PageInfo\x12"\n\rhas_next_page\x18\x01 \x01(\x08R\x0bhasNextPage\x12*\n\x11has_previous_page\x18\x02 \x01(\x08R\x0fhasPreviousPage\x12!\n\x0cstart_cursor\x18\x03 \x01(\tR\x0bstartCursor\x12\x1d\n\nend_cursor\x18\x04 \x01(\tR\tendCursor"\x9a\x01\n\x0e\x41\x63\x63ountBalance\x12\x14\n\x05owner\x18\x02 \x01(\tR\x05owner\x12\x18\n\x07\x62\x61lance\x18\x03 \x01(\tR\x07\x62\x61lance\x12\x14\n\x05\x61sset\x18\x04 \x01(\tR\x05\x61sset\x12\x1b\n\tmarket_id\x18\x05 \x01(\tR\x08marketId\x12%\n\x04type\x18\x06 \x01(\x0e\x32\x11.vega.AccountTypeR\x04type"\x9e\x01\n\x13ListAccountsRequest\x12\x36\n\x06\x66ilter\x18\x01 \x01(\x0b\x32\x1e.datanode.api.v2.AccountFilterR\x06\x66ilter\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"W\n\x14ListAccountsResponse\x12?\n\x08\x61\x63\x63ounts\x18\x01 \x01(\x0b\x32#.datanode.api.v2.AccountsConnectionR\x08\x61\x63\x63ounts"\x80\x01\n\x12\x41\x63\x63ountsConnection\x12\x32\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1c.datanode.api.v2.AccountEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"Z\n\x0b\x41\x63\x63ountEdge\x12\x33\n\x04node\x18\x01 \x01(\x0b\x32\x1f.datanode.api.v2.AccountBalanceR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x8d\x01\n\x16ObserveAccountsRequest\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x14\n\x05\x61sset\x18\x03 \x01(\tR\x05\x61sset\x12%\n\x04type\x18\x04 \x01(\x0e\x32\x11.vega.AccountTypeR\x04type"\xa6\x01\n\x17ObserveAccountsResponse\x12\x42\n\x08snapshot\x18\x01 \x01(\x0b\x32$.datanode.api.v2.AccountSnapshotPageH\x00R\x08snapshot\x12;\n\x07updates\x18\x02 \x01(\x0b\x32\x1f.datanode.api.v2.AccountUpdatesH\x00R\x07updatesB\n\n\x08response"o\n\x13\x41\x63\x63ountSnapshotPage\x12;\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.AccountBalanceR\x08\x61\x63\x63ounts\x12\x1b\n\tlast_page\x18\x02 \x01(\x08R\x08lastPage"M\n\x0e\x41\x63\x63ountUpdates\x12;\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.AccountBalanceR\x08\x61\x63\x63ounts"\r\n\x0bInfoRequest"I\n\x0cInfoResponse\x12\x18\n\x07version\x18\x01 \x01(\tR\x07version\x12\x1f\n\x0b\x63ommit_hash\x18\x02 \x01(\tR\ncommitHash"W\n\x0fGetOrderRequest\x12\x19\n\x08order_id\x18\x01 \x01(\tR\x07orderId\x12\x1d\n\x07version\x18\x02 \x01(\x05H\x00R\x07version\x88\x01\x01\x42\n\n\x08_version"5\n\x10GetOrderResponse\x12!\n\x05order\x18\x01 \x01(\x0b\x32\x0b.vega.OrderR\x05order"\xd1\x01\n\x0bOrderFilter\x12.\n\x08statuses\x18\x01 \x03(\x0e\x32\x12.vega.Order.StatusR\x08statuses\x12&\n\x05types\x18\x02 \x03(\x0e\x32\x10.vega.Order.TypeR\x05types\x12=\n\x0etime_in_forces\x18\x03 \x03(\x0e\x32\x17.vega.Order.TimeInForceR\x0ctimeInForces\x12+\n\x11\x65xclude_liquidity\x18\x04 \x01(\x08R\x10\x65xcludeLiquidity"\xb7\x03\n\x11ListOrdersRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12 \n\tmarket_id\x18\x02 \x01(\tH\x01R\x08marketId\x88\x01\x01\x12!\n\treference\x18\x03 \x01(\tH\x02R\treference\x88\x01\x01\x12@\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x03R\npagination\x88\x01\x01\x12 \n\tlive_only\x18\x05 \x01(\x08H\x04R\x08liveOnly\x88\x01\x01\x12>\n\ndate_range\x18\x06 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x05R\tdateRange\x88\x01\x01\x12\x39\n\x06\x66ilter\x18\x07 \x01(\x0b\x32\x1c.datanode.api.v2.OrderFilterH\x06R\x06\x66ilter\x88\x01\x01\x42\x0b\n\t_party_idB\x0c\n\n_market_idB\x0c\n\n_referenceB\r\n\x0b_paginationB\x0c\n\n_live_onlyB\r\n\x0b_date_rangeB\t\n\x07_filter"N\n\x12ListOrdersResponse\x12\x38\n\x06orders\x18\x01 \x01(\x0b\x32 .datanode.api.v2.OrderConnectionR\x06orders"\x86\x01\n\x18ListOrderVersionsRequest\x12\x19\n\x08order_id\x18\x01 \x01(\tR\x07orderId\x12@\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"U\n\x19ListOrderVersionsResponse\x12\x38\n\x06orders\x18\x01 \x01(\x0b\x32 .datanode.api.v2.OrderConnectionR\x06orders"\xbb\x01\n\x14ObserveOrdersRequest\x12 \n\tmarket_id\x18\x01 \x01(\tH\x00R\x08marketId\x88\x01\x01\x12\x1e\n\x08party_id\x18\x02 \x01(\tH\x01R\x07partyId\x88\x01\x01\x12\x30\n\x11\x65xclude_liquidity\x18\x03 \x01(\x08H\x02R\x10\x65xcludeLiquidity\x88\x01\x01\x42\x0c\n\n_market_idB\x0b\n\t_party_idB\x14\n\x12_exclude_liquidity"\xa0\x01\n\x15ObserveOrdersResponse\x12@\n\x08snapshot\x18\x01 \x01(\x0b\x32".datanode.api.v2.OrderSnapshotPageH\x00R\x08snapshot\x12\x39\n\x07updates\x18\x02 \x01(\x0b\x32\x1d.datanode.api.v2.OrderUpdatesH\x00R\x07updatesB\n\n\x08response"U\n\x11OrderSnapshotPage\x12#\n\x06orders\x18\x01 \x03(\x0b\x32\x0b.vega.OrderR\x06orders\x12\x1b\n\tlast_page\x18\x02 \x01(\x08R\x08lastPage"3\n\x0cOrderUpdates\x12#\n\x06orders\x18\x01 \x03(\x0b\x32\x0b.vega.OrderR\x06orders"\x9f\x01\n\x14ListPositionsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"Z\n\x15ListPositionsResponse\x12\x41\n\tpositions\x18\x01 \x01(\x0b\x32#.datanode.api.v2.PositionConnectionR\tpositions"J\n\x0cPositionEdge\x12"\n\x04node\x18\x01 \x01(\x0b\x32\x0e.vega.PositionR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x81\x01\n\x12PositionConnection\x12\x33\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1d.datanode.api.v2.PositionEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"v\n\x17ObservePositionsRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12 \n\tmarket_id\x18\x02 \x01(\tH\x01R\x08marketId\x88\x01\x01\x42\x0b\n\t_party_idB\x0c\n\n_market_id"\xa9\x01\n\x18ObservePositionsResponse\x12\x43\n\x08snapshot\x18\x01 \x01(\x0b\x32%.datanode.api.v2.PositionSnapshotPageH\x00R\x08snapshot\x12<\n\x07updates\x18\x02 \x01(\x0b\x32 .datanode.api.v2.PositionUpdatesH\x00R\x07updatesB\n\n\x08response"a\n\x14PositionSnapshotPage\x12,\n\tpositions\x18\x01 \x03(\x0b\x32\x0e.vega.PositionR\tpositions\x12\x1b\n\tlast_page\x18\x02 \x01(\x08R\x08lastPage"?\n\x0fPositionUpdates\x12,\n\tpositions\x18\x01 \x03(\x0b\x32\x0e.vega.PositionR\tpositions"\xa3\x02\n\x11LedgerEntryFilter\x12\x37\n\x18\x63lose_on_account_filters\x18\x01 \x01(\x08R\x15\x63loseOnAccountFilters\x12N\n\x13\x66rom_account_filter\x18\x02 \x01(\x0b\x32\x1e.datanode.api.v2.AccountFilterR\x11\x66romAccountFilter\x12J\n\x11to_account_filter\x18\x03 \x01(\x0b\x32\x1e.datanode.api.v2.AccountFilterR\x0ftoAccountFilter\x12\x39\n\x0etransfer_types\x18\x05 \x03(\x0e\x32\x12.vega.TransferTypeR\rtransferTypes"\xd9\x05\n\x15\x41ggregatedLedgerEntry\x12\x1c\n\ttimestamp\x18\x02 \x01(\x03R\ttimestamp\x12\x1a\n\x08quantity\x18\x03 \x01(\tR\x08quantity\x12\x37\n\rtransfer_type\x18\x04 \x01(\x0e\x32\x12.vega.TransferTypeR\x0ctransferType\x12\x1e\n\x08\x61sset_id\x18\x05 \x01(\tH\x00R\x07\x61ssetId\x88\x01\x01\x12=\n\x11\x66rom_account_type\x18\x06 \x01(\x0e\x32\x11.vega.AccountTypeR\x0f\x66romAccountType\x12\x39\n\x0fto_account_type\x18\x07 \x01(\x0e\x32\x11.vega.AccountTypeR\rtoAccountType\x12\x36\n\x15\x66rom_account_party_id\x18\x08 \x01(\tH\x01R\x12\x66romAccountPartyId\x88\x01\x01\x12\x32\n\x13to_account_party_id\x18\t \x01(\tH\x02R\x10toAccountPartyId\x88\x01\x01\x12\x38\n\x16\x66rom_account_market_id\x18\n \x01(\tH\x03R\x13\x66romAccountMarketId\x88\x01\x01\x12\x34\n\x14to_account_market_id\x18\x0b \x01(\tH\x04R\x11toAccountMarketId\x88\x01\x01\x12\x30\n\x14\x66rom_account_balance\x18\x0c \x01(\tR\x12\x66romAccountBalance\x12,\n\x12to_account_balance\x18\r \x01(\tR\x10toAccountBalanceB\x0b\n\t_asset_idB\x18\n\x16_from_account_party_idB\x16\n\x14_to_account_party_idB\x19\n\x17_from_account_market_idB\x17\n\x15_to_account_market_idJ\x04\x08\x01\x10\x02"\xf6\x01\n\x18ListLedgerEntriesRequest\x12:\n\x06\x66ilter\x18\x01 \x01(\x0b\x32".datanode.api.v2.LedgerEntryFilterR\x06\x66ilter\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x03 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"\xf2\x01\n\x1a\x45xportLedgerEntriesRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x19\n\x08\x61sset_id\x18\x02 \x01(\tR\x07\x61ssetId\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x04 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"v\n\x19ListLedgerEntriesResponse\x12Y\n\x0eledger_entries\x18\x01 \x01(\x0b\x32\x32.datanode.api.v2.AggregatedLedgerEntriesConnectionR\rledgerEntries"i\n\x1b\x45xportLedgerEntriesResponse\x12\x12\n\x04\x64\x61ta\x18\x01 \x01(\x0cR\x04\x64\x61ta\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"q\n\x1b\x41ggregatedLedgerEntriesEdge\x12:\n\x04node\x18\x01 \x01(\x0b\x32&.datanode.api.v2.AggregatedLedgerEntryR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x9f\x01\n!AggregatedLedgerEntriesConnection\x12\x42\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32,.datanode.api.v2.AggregatedLedgerEntriesEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xf3\x01\n\x19ListBalanceChangesRequest\x12\x36\n\x06\x66ilter\x18\x01 \x01(\x0b\x32\x1e.datanode.api.v2.AccountFilterR\x06\x66ilter\x12@\n\npagination\x18\x05 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x06 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"f\n\x1aListBalanceChangesResponse\x12H\n\x08\x62\x61lances\x18\x01 \x01(\x0b\x32,.datanode.api.v2.AggregatedBalanceConnectionR\x08\x62\x61lances"\xac\x02\n\x18GetBalanceHistoryRequest\x12\x36\n\x06\x66ilter\x18\x01 \x01(\x0b\x32\x1e.datanode.api.v2.AccountFilterR\x06\x66ilter\x12\x38\n\x08group_by\x18\x02 \x03(\x0e\x32\x1d.datanode.api.v2.AccountFieldR\x07groupBy\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x04 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"e\n\x19GetBalanceHistoryResponse\x12H\n\x08\x62\x61lances\x18\x01 \x01(\x0b\x32,.datanode.api.v2.AggregatedBalanceConnectionR\x08\x62\x61lances"g\n\x15\x41ggregatedBalanceEdge\x12\x36\n\x04node\x18\x01 \x01(\x0b\x32".datanode.api.v2.AggregatedBalanceR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x93\x01\n\x1b\x41ggregatedBalanceConnection\x12<\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32&.datanode.api.v2.AggregatedBalanceEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x9e\x01\n\rAccountFilter\x12\x19\n\x08\x61sset_id\x18\x01 \x01(\tR\x07\x61ssetId\x12\x1b\n\tparty_ids\x18\x02 \x03(\tR\x08partyIds\x12\x1d\n\nmarket_ids\x18\x03 \x03(\tR\tmarketIds\x12\x36\n\raccount_types\x18\x04 \x03(\x0e\x32\x11.vega.AccountTypeR\x0c\x61\x63\x63ountTypes"\xa1\x02\n\x11\x41ggregatedBalance\x12\x1c\n\ttimestamp\x18\x01 \x01(\x03R\ttimestamp\x12\x18\n\x07\x62\x61lance\x18\x02 \x01(\tR\x07\x62\x61lance\x12\x1e\n\x08party_id\x18\x04 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12\x1e\n\x08\x61sset_id\x18\x05 \x01(\tH\x01R\x07\x61ssetId\x88\x01\x01\x12 \n\tmarket_id\x18\x06 \x01(\tH\x02R\x08marketId\x88\x01\x01\x12\x39\n\x0c\x61\x63\x63ount_type\x18\x07 \x01(\x0e\x32\x11.vega.AccountTypeH\x03R\x0b\x61\x63\x63ountType\x88\x01\x01\x42\x0b\n\t_party_idB\x0b\n\t_asset_idB\x0c\n\n_market_idB\x0f\n\r_account_type";\n\x1aObserveMarketsDepthRequest\x12\x1d\n\nmarket_ids\x18\x01 \x03(\tR\tmarketIds"S\n\x1bObserveMarketsDepthResponse\x12\x34\n\x0cmarket_depth\x18\x01 \x03(\x0b\x32\x11.vega.MarketDepthR\x0bmarketDepth"B\n!ObserveMarketsDepthUpdatesRequest\x12\x1d\n\nmarket_ids\x18\x01 \x03(\tR\tmarketIds"U\n"ObserveMarketsDepthUpdatesResponse\x12/\n\x06update\x18\x01 \x03(\x0b\x32\x17.vega.MarketDepthUpdateR\x06update":\n\x19ObserveMarketsDataRequest\x12\x1d\n\nmarket_ids\x18\x01 \x03(\tR\tmarketIds"O\n\x1aObserveMarketsDataResponse\x12\x31\n\x0bmarket_data\x18\x01 \x03(\x0b\x32\x10.vega.MarketDataR\nmarketData"j\n\x1bGetLatestMarketDepthRequest\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12 \n\tmax_depth\x18\x02 \x01(\x04H\x00R\x08maxDepth\x88\x01\x01\x42\x0c\n\n_max_depth"\xda\x01\n\x1cGetLatestMarketDepthResponse\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12"\n\x03\x62uy\x18\x02 \x03(\x0b\x32\x10.vega.PriceLevelR\x03\x62uy\x12$\n\x04sell\x18\x03 \x03(\x0b\x32\x10.vega.PriceLevelR\x04sell\x12*\n\nlast_trade\x18\x04 \x01(\x0b\x32\x0b.vega.TradeR\tlastTrade\x12\'\n\x0fsequence_number\x18\x05 \x01(\x04R\x0esequenceNumber"\x1d\n\x1bListLatestMarketDataRequest"S\n\x1cListLatestMarketDataResponse\x12\x33\n\x0cmarkets_data\x18\x01 \x03(\x0b\x32\x10.vega.MarketDataR\x0bmarketsData"9\n\x1aGetLatestMarketDataRequest\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId"P\n\x1bGetLatestMarketDataResponse\x12\x31\n\x0bmarket_data\x18\x01 \x01(\x0b\x32\x10.vega.MarketDataR\nmarketData"\xfc\x02\n\x1fGetMarketDataHistoryByIDRequest\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12,\n\x0fstart_timestamp\x18\x02 \x01(\x03H\x00R\x0estartTimestamp\x88\x01\x01\x12(\n\rend_timestamp\x18\x03 \x01(\x03H\x01R\x0c\x65ndTimestamp\x88\x01\x01\x12@\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x02R\npagination\x88\x01\x01\x12W\n\x11offset_pagination\x18\x05 \x01(\x0b\x32!.datanode.api.v2.OffsetPaginationB\x02\x18\x01H\x03R\x10offsetPagination\x88\x01\x01\x42\x12\n\x10_start_timestampB\x10\n\x0e_end_timestampB\r\n\x0b_paginationB\x14\n\x12_offset_pagination"j\n GetMarketDataHistoryByIDResponse\x12\x46\n\x0bmarket_data\x18\x01 \x01(\x0b\x32%.datanode.api.v2.MarketDataConnectionR\nmarketData"N\n\x0eMarketDataEdge\x12$\n\x04node\x18\x01 \x01(\x0b\x32\x10.vega.MarketDataR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x85\x01\n\x14MarketDataConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.MarketDataEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo":\n\x1bMarketsDataSubscribeRequest\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId"Q\n\x1cMarketsDataSubscribeResponse\x12\x31\n\x0bmarket_data\x18\x01 \x03(\x0b\x32\x10.vega.MarketDataR\nmarketData"\xd1\x01\n\x14ListTransfersRequest\x12\x1b\n\x06pubkey\x18\x01 \x01(\tH\x00R\x06pubkey\x88\x01\x01\x12@\n\tdirection\x18\x02 \x01(\x0e\x32".datanode.api.v2.TransferDirectionR\tdirection\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\t\n\x07_pubkeyB\r\n\x0b_pagination"Z\n\x15ListTransfersResponse\x12\x41\n\ttransfers\x18\x01 \x01(\x0b\x32#.datanode.api.v2.TransferConnectionR\ttransfers"T\n\x0cTransferEdge\x12,\n\x04node\x18\x01 \x01(\x0b\x32\x18.vega.events.v1.TransferR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x81\x01\n\x12TransferConnection\x12\x33\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1d.datanode.api.v2.TransferEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x19\n\x17GetNetworkLimitsRequest"G\n\x18GetNetworkLimitsResponse\x12+\n\x06limits\x18\x01 \x01(\x0b\x32\x13.vega.NetworkLimitsR\x06limits"9\n\x1aListCandleIntervalsRequest\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId"M\n\x12IntervalToCandleId\x12\x1a\n\x08interval\x18\x01 \x01(\tR\x08interval\x12\x1b\n\tcandle_id\x18\x02 \x01(\tR\x08\x63\x61ndleId"u\n\x1bListCandleIntervalsResponse\x12V\n\x15interval_to_candle_id\x18\x01 \x03(\x0b\x32#.datanode.api.v2.IntervalToCandleIdR\x12intervalToCandleId"\xa7\x01\n\x06\x43\x61ndle\x12\x14\n\x05start\x18\x01 \x01(\x03R\x05start\x12\x1f\n\x0blast_update\x18\x02 \x01(\x03R\nlastUpdate\x12\x12\n\x04high\x18\x03 \x01(\tR\x04high\x12\x10\n\x03low\x18\x04 \x01(\tR\x03low\x12\x12\n\x04open\x18\x05 \x01(\tR\x04open\x12\x14\n\x05\x63lose\x18\x06 \x01(\tR\x05\x63lose\x12\x16\n\x06volume\x18\x07 \x01(\x04R\x06volume"7\n\x18ObserveCandleDataRequest\x12\x1b\n\tcandle_id\x18\x01 \x01(\tR\x08\x63\x61ndleId"L\n\x19ObserveCandleDataResponse\x12/\n\x06\x63\x61ndle\x18\x01 \x01(\x0b\x32\x17.datanode.api.v2.CandleR\x06\x63\x61ndle"\xfb\x01\n\x15ListCandleDataRequest\x12\x1b\n\tcandle_id\x18\x01 \x01(\tR\x08\x63\x61ndleId\x12%\n\x0e\x66rom_timestamp\x18\x02 \x01(\x03R\rfromTimestamp\x12!\n\x0cto_timestamp\x18\x03 \x01(\x03R\x0btoTimestamp\x12*\n\x08interval\x18\x04 \x01(\x0e\x32\x0e.vega.IntervalR\x08interval\x12@\n\npagination\x18\x05 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"Y\n\x16ListCandleDataResponse\x12?\n\x07\x63\x61ndles\x18\x01 \x01(\x0b\x32%.datanode.api.v2.CandleDataConnectionR\x07\x63\x61ndles"Q\n\nCandleEdge\x12+\n\x04node\x18\x01 \x01(\x0b\x32\x17.datanode.api.v2.CandleR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x81\x01\n\x14\x43\x61ndleDataConnection\x12\x31\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1b.datanode.api.v2.CandleEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xc6\x01\n\x10ListVotesRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12$\n\x0bproposal_id\x18\x02 \x01(\tH\x01R\nproposalId\x88\x01\x01\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x02R\npagination\x88\x01\x01\x42\x0b\n\t_party_idB\x0e\n\x0c_proposal_idB\r\n\x0b_pagination"J\n\x11ListVotesResponse\x12\x35\n\x05votes\x18\x01 \x01(\x0b\x32\x1f.datanode.api.v2.VoteConnectionR\x05votes"B\n\x08VoteEdge\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\n.vega.VoteR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"y\n\x0eVoteConnection\x12/\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x19.datanode.api.v2.VoteEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"x\n\x13ObserveVotesRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12$\n\x0bproposal_id\x18\x02 \x01(\tH\x01R\nproposalId\x88\x01\x01\x42\x0b\n\t_party_idB\x0e\n\x0c_proposal_id"6\n\x14ObserveVotesResponse\x12\x1e\n\x04vote\x18\x01 \x01(\x0b\x32\n.vega.VoteR\x04vote"\xbd\x01\n*ListERC20MultiSigSignerAddedBundlesRequest\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1c\n\tsubmitter\x18\x02 \x01(\tR\tsubmitter\x12\x1b\n\tepoch_seq\x18\x03 \x01(\tR\x08\x65pochSeq\x12;\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationR\npagination"|\n+ListERC20MultiSigSignerAddedBundlesResponse\x12M\n\x07\x62undles\x18\x01 \x01(\x0b\x32\x33.datanode.api.v2.ERC20MultiSigSignerAddedConnectionR\x07\x62undles"t\n\x1c\x45RC20MultiSigSignerAddedEdge\x12<\n\x04node\x18\x01 \x01(\x0b\x32(.vega.events.v1.ERC20MultiSigSignerAddedR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x81\x01\n"ERC20MultiSigSignerAddedBundleEdge\x12\x43\n\x04node\x18\x01 \x01(\x0b\x32/.datanode.api.v2.ERC20MultiSigSignerAddedBundleR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\xa7\x01\n"ERC20MultiSigSignerAddedConnection\x12I\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x33.datanode.api.v2.ERC20MultiSigSignerAddedBundleEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xce\x01\n\x1e\x45RC20MultiSigSignerAddedBundle\x12\x1d\n\nnew_signer\x18\x01 \x01(\tR\tnewSigner\x12\x1c\n\tsubmitter\x18\x02 \x01(\tR\tsubmitter\x12\x14\n\x05nonce\x18\x04 \x01(\tR\x05nonce\x12\x1c\n\ttimestamp\x18\x05 \x01(\x03R\ttimestamp\x12\x1e\n\nsignatures\x18\x06 \x01(\tR\nsignatures\x12\x1b\n\tepoch_seq\x18\x03 \x01(\tR\x08\x65pochSeq"\xbf\x01\n,ListERC20MultiSigSignerRemovedBundlesRequest\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1c\n\tsubmitter\x18\x02 \x01(\tR\tsubmitter\x12\x1b\n\tepoch_seq\x18\x03 \x01(\tR\x08\x65pochSeq\x12;\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationR\npagination"\x80\x01\n-ListERC20MultiSigSignerRemovedBundlesResponse\x12O\n\x07\x62undles\x18\x01 \x01(\x0b\x32\x35.datanode.api.v2.ERC20MultiSigSignerRemovedConnectionR\x07\x62undles"x\n\x1e\x45RC20MultiSigSignerRemovedEdge\x12>\n\x04node\x18\x01 \x01(\x0b\x32*.vega.events.v1.ERC20MultiSigSignerRemovedR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x85\x01\n$ERC20MultiSigSignerRemovedBundleEdge\x12\x45\n\x04node\x18\x01 \x01(\x0b\x32\x31.datanode.api.v2.ERC20MultiSigSignerRemovedBundleR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\xab\x01\n$ERC20MultiSigSignerRemovedConnection\x12K\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x35.datanode.api.v2.ERC20MultiSigSignerRemovedBundleEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xd0\x01\n ERC20MultiSigSignerRemovedBundle\x12\x1d\n\nold_signer\x18\x01 \x01(\tR\toldSigner\x12\x1c\n\tsubmitter\x18\x02 \x01(\tR\tsubmitter\x12\x14\n\x05nonce\x18\x04 \x01(\tR\x05nonce\x12\x1c\n\ttimestamp\x18\x05 \x01(\x03R\ttimestamp\x12\x1e\n\nsignatures\x18\x06 \x01(\tR\nsignatures\x12\x1b\n\tepoch_seq\x18\x07 \x01(\tR\x08\x65pochSeq";\n\x1eGetERC20ListAssetBundleRequest\x12\x19\n\x08\x61sset_id\x18\x01 \x01(\tR\x07\x61ssetId"\x9e\x01\n\x1fGetERC20ListAssetBundleResponse\x12!\n\x0c\x61sset_source\x18\x01 \x01(\tR\x0b\x61ssetSource\x12"\n\rvega_asset_id\x18\x02 \x01(\tR\x0bvegaAssetId\x12\x14\n\x05nonce\x18\x03 \x01(\tR\x05nonce\x12\x1e\n\nsignatures\x18\x04 \x01(\tR\nsignatures"F\n#GetERC20SetAssetLimitsBundleRequest\x12\x1f\n\x0bproposal_id\x18\x01 \x01(\tR\nproposalId"\xe8\x01\n$GetERC20SetAssetLimitsBundleResponse\x12!\n\x0c\x61sset_source\x18\x01 \x01(\tR\x0b\x61ssetSource\x12"\n\rvega_asset_id\x18\x02 \x01(\tR\x0bvegaAssetId\x12\x14\n\x05nonce\x18\x03 \x01(\tR\x05nonce\x12%\n\x0elifetime_limit\x18\x04 \x01(\tR\rlifetimeLimit\x12\x1c\n\tthreshold\x18\x05 \x01(\tR\tthreshold\x12\x1e\n\nsignatures\x18\x06 \x01(\tR\nsignatures"H\n!GetERC20WithdrawalApprovalRequest\x12#\n\rwithdrawal_id\x18\x01 \x01(\tR\x0cwithdrawalId"\xde\x01\n"GetERC20WithdrawalApprovalResponse\x12!\n\x0c\x61sset_source\x18\x01 \x01(\tR\x0b\x61ssetSource\x12\x16\n\x06\x61mount\x18\x02 \x01(\tR\x06\x61mount\x12\x14\n\x05nonce\x18\x04 \x01(\tR\x05nonce\x12\x1e\n\nsignatures\x18\x05 \x01(\tR\nsignatures\x12%\n\x0etarget_address\x18\x06 \x01(\tR\rtargetAddress\x12\x1a\n\x08\x63reation\x18\x07 \x01(\x03R\x08\x63reationJ\x04\x08\x03\x10\x04"2\n\x13GetLastTradeRequest\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId"9\n\x14GetLastTradeResponse\x12!\n\x05trade\x18\x01 \x01(\x0b\x32\x0b.vega.TradeR\x05trade"\xbd\x02\n\x11ListTradesRequest\x12 \n\tmarket_id\x18\x01 \x01(\tH\x00R\x08marketId\x88\x01\x01\x12\x1e\n\x08order_id\x18\x02 \x01(\tH\x01R\x07orderId\x88\x01\x01\x12\x1e\n\x08party_id\x18\x03 \x01(\tH\x02R\x07partyId\x88\x01\x01\x12@\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x03R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x05 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x04R\tdateRange\x88\x01\x01\x42\x0c\n\n_market_idB\x0b\n\t_order_idB\x0b\n\t_party_idB\r\n\x0b_paginationB\r\n\x0b_date_range"N\n\x12ListTradesResponse\x12\x38\n\x06trades\x18\x01 \x01(\x0b\x32 .datanode.api.v2.TradeConnectionR\x06trades"{\n\x0fTradeConnection\x12\x30\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1a.datanode.api.v2.TradeEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"D\n\tTradeEdge\x12\x1f\n\x04node\x18\x01 \x01(\x0b\x32\x0b.vega.TradeR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"s\n\x14ObserveTradesRequest\x12 \n\tmarket_id\x18\x01 \x01(\tH\x00R\x08marketId\x88\x01\x01\x12\x1e\n\x08party_id\x18\x02 \x01(\tH\x01R\x07partyId\x88\x01\x01\x42\x0c\n\n_market_idB\x0b\n\t_party_id"<\n\x15ObserveTradesResponse\x12#\n\x06trades\x18\x01 \x03(\x0b\x32\x0b.vega.TradeR\x06trades"<\n\x14GetOracleSpecRequest\x12$\n\x0eoracle_spec_id\x18\x01 \x01(\tR\x0coracleSpecId"J\n\x15GetOracleSpecResponse\x12\x31\n\x0boracle_spec\x18\x01 \x01(\x0b\x32\x10.vega.OracleSpecR\noracleSpec"i\n\x16ListOracleSpecsRequest\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"d\n\x17ListOracleSpecsResponse\x12I\n\x0coracle_specs\x18\x01 \x01(\x0b\x32&.datanode.api.v2.OracleSpecsConnectionR\x0boracleSpecs"\xa6\x01\n\x15ListOracleDataRequest\x12)\n\x0eoracle_spec_id\x18\x01 \x01(\tH\x00R\x0coracleSpecId\x88\x01\x01\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\x11\n\x0f_oracle_spec_idB\r\n\x0b_pagination"`\n\x16ListOracleDataResponse\x12\x46\n\x0boracle_data\x18\x01 \x01(\x0b\x32%.datanode.api.v2.OracleDataConnectionR\noracleData"N\n\x0eOracleSpecEdge\x12$\n\x04node\x18\x01 \x01(\x0b\x32\x10.vega.OracleSpecR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x86\x01\n\x15OracleSpecsConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.OracleSpecEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"N\n\x0eOracleDataEdge\x12$\n\x04node\x18\x01 \x01(\x0b\x32\x10.vega.OracleDataR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x85\x01\n\x14OracleDataConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.OracleDataEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"/\n\x10GetMarketRequest\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId"9\n\x11GetMarketResponse\x12$\n\x06market\x18\x01 \x01(\x0b\x32\x0c.vega.MarketR\x06market"e\n\x12ListMarketsRequest\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"R\n\x13ListMarketsResponse\x12;\n\x07markets\x18\x01 \x01(\x0b\x32!.datanode.api.v2.MarketConnectionR\x07markets"F\n\nMarketEdge\x12 \n\x04node\x18\x01 \x01(\x0b\x32\x0c.vega.MarketR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"}\n\x10MarketConnection\x12\x31\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1b.datanode.api.v2.MarketEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo",\n\x0fGetPartyRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId"5\n\x10GetPartyResponse\x12!\n\x05party\x18\x01 \x01(\x0b\x32\x0b.vega.PartyR\x05party"l\n\x12ListPartiesRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12;\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationR\npagination"Q\n\x13ListPartiesResponse\x12:\n\x07parties\x18\x01 \x01(\x0b\x32 .datanode.api.v2.PartyConnectionR\x07parties"D\n\tPartyEdge\x12\x1f\n\x04node\x18\x01 \x01(\x0b\x32\x0b.vega.PartyR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"{\n\x0fPartyConnection\x12\x30\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1a.datanode.api.v2.PartyEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"D\n\tOrderEdge\x12\x1f\n\x04node\x18\x01 \x01(\x0b\x32\x0b.vega.OrderR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x8e\x01\n\x17ListMarginLevelsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12;\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationR\npagination"b\n\x18ListMarginLevelsResponse\x12\x46\n\rmargin_levels\x18\x01 \x01(\x0b\x32!.datanode.api.v2.MarginConnectionR\x0cmarginLevels"g\n\x1aObserveMarginLevelsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12 \n\tmarket_id\x18\x02 \x01(\tH\x00R\x08marketId\x88\x01\x01\x42\x0c\n\n_market_id"V\n\x1bObserveMarginLevelsResponse\x12\x37\n\rmargin_levels\x18\x01 \x01(\x0b\x32\x12.vega.MarginLevelsR\x0cmarginLevels"{\n\x0fOrderConnection\x12\x30\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1a.datanode.api.v2.OrderEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"L\n\nMarginEdge\x12&\n\x04node\x18\x01 \x01(\x0b\x32\x12.vega.MarginLevelsR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"}\n\x10MarginConnection\x12\x31\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1b.datanode.api.v2.MarginEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xad\x01\n\x12ListRewardsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x1e\n\x08\x61sset_id\x18\x02 \x01(\tH\x00R\x07\x61ssetId\x88\x01\x01\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\x0b\n\t_asset_idB\r\n\x0b_pagination"S\n\x13ListRewardsResponse\x12<\n\x07rewards\x18\x01 \x01(\x0b\x32".datanode.api.v2.RewardsConnectionR\x07rewards"F\n\nRewardEdge\x12 \n\x04node\x18\x01 \x01(\x0b\x32\x0c.vega.RewardR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"~\n\x11RewardsConnection\x12\x31\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1b.datanode.api.v2.RewardEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xc7\x01\n\x1aListRewardSummariesRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12\x1e\n\x08\x61sset_id\x18\x02 \x01(\tH\x01R\x07\x61ssetId\x88\x01\x01\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x02R\npagination\x88\x01\x01\x42\x0b\n\t_party_idB\x0b\n\t_asset_idB\r\n\x0b_pagination"P\n\x1bListRewardSummariesResponse\x12\x31\n\tsummaries\x18\x01 \x03(\x0b\x32\x13.vega.RewardSummaryR\tsummaries"\xd2\x01\n\x1fListEpochRewardSummariesRequest\x12"\n\nfrom_epoch\x18\x01 \x01(\x04H\x00R\tfromEpoch\x88\x01\x01\x12\x1e\n\x08to_epoch\x18\x02 \x01(\x04H\x01R\x07toEpoch\x88\x01\x01\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x02R\npagination\x88\x01\x01\x42\r\n\x0b_from_epochB\x0b\n\t_to_epochB\r\n\x0b_pagination"o\n ListEpochRewardSummariesResponse\x12K\n\tsummaries\x18\x01 \x01(\x0b\x32-.datanode.api.v2.EpochRewardSummaryConnectionR\tsummaries"\x95\x01\n\x1c\x45pochRewardSummaryConnection\x12=\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\'.datanode.api.v2.EpochRewardSummaryEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"^\n\x16\x45pochRewardSummaryEdge\x12,\n\x04node\x18\x01 \x01(\x0b\x32\x18.vega.EpochRewardSummaryR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"q\n\x15ObserveRewardsRequest\x12\x1e\n\x08\x61sset_id\x18\x01 \x01(\tH\x00R\x07\x61ssetId\x88\x01\x01\x12\x1e\n\x08party_id\x18\x02 \x01(\tH\x01R\x07partyId\x88\x01\x01\x42\x0b\n\t_asset_idB\x0b\n\t_party_id">\n\x16ObserveRewardsResponse\x12$\n\x06reward\x18\x01 \x01(\x0b\x32\x0c.vega.RewardR\x06reward"#\n\x11GetDepositRequest\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id"=\n\x12GetDepositResponse\x12\'\n\x07\x64\x65posit\x18\x01 \x01(\x0b\x32\r.vega.DepositR\x07\x64\x65posit"\xd0\x01\n\x13ListDepositsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x03 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"W\n\x14ListDepositsResponse\x12?\n\x08\x64\x65posits\x18\x01 \x01(\x0b\x32#.datanode.api.v2.DepositsConnectionR\x08\x64\x65posits"H\n\x0b\x44\x65positEdge\x12!\n\x04node\x18\x01 \x01(\x0b\x32\r.vega.DepositR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x80\x01\n\x12\x44\x65positsConnection\x12\x32\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1c.datanode.api.v2.DepositEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"&\n\x14GetWithdrawalRequest\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id"I\n\x15GetWithdrawalResponse\x12\x30\n\nwithdrawal\x18\x01 \x01(\x0b\x32\x10.vega.WithdrawalR\nwithdrawal"\xd3\x01\n\x16ListWithdrawalsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x03 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"c\n\x17ListWithdrawalsResponse\x12H\n\x0bwithdrawals\x18\x01 \x01(\x0b\x32&.datanode.api.v2.WithdrawalsConnectionR\x0bwithdrawals"N\n\x0eWithdrawalEdge\x12$\n\x04node\x18\x01 \x01(\x0b\x32\x10.vega.WithdrawalR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x86\x01\n\x15WithdrawalsConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.WithdrawalEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo",\n\x0fGetAssetRequest\x12\x19\n\x08\x61sset_id\x18\x01 \x01(\tR\x07\x61ssetId"5\n\x10GetAssetResponse\x12!\n\x05\x61sset\x18\x01 \x01(\x0b\x32\x0b.vega.AssetR\x05\x61sset"\x91\x01\n\x11ListAssetsRequest\x12\x1e\n\x08\x61sset_id\x18\x01 \x01(\tH\x00R\x07\x61ssetId\x88\x01\x01\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\x0b\n\t_asset_idB\r\n\x0b_pagination"O\n\x12ListAssetsResponse\x12\x39\n\x06\x61ssets\x18\x01 \x01(\x0b\x32!.datanode.api.v2.AssetsConnectionR\x06\x61ssets"D\n\tAssetEdge\x12\x1f\n\x04node\x18\x01 \x01(\x0b\x32\x0b.vega.AssetR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"|\n\x10\x41ssetsConnection\x12\x30\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1a.datanode.api.v2.AssetEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xff\x01\n\x1eListLiquidityProvisionsRequest\x12 \n\tmarket_id\x18\x01 \x01(\tH\x00R\x08marketId\x88\x01\x01\x12\x1e\n\x08party_id\x18\x02 \x01(\tH\x01R\x07partyId\x88\x01\x01\x12!\n\treference\x18\x03 \x01(\tH\x02R\treference\x88\x01\x01\x12@\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x03R\npagination\x88\x01\x01\x42\x0c\n\n_market_idB\x0b\n\t_party_idB\x0c\n\n_referenceB\r\n\x0b_pagination"\x84\x01\n\x1fListLiquidityProvisionsResponse\x12\x61\n\x14liquidity_provisions\x18\x01 \x01(\x0b\x32..datanode.api.v2.LiquidityProvisionsConnectionR\x13liquidityProvisions"_\n\x17LiquidityProvisionsEdge\x12,\n\x04node\x18\x01 \x01(\x0b\x32\x18.vega.LiquidityProvisionR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x97\x01\n\x1dLiquidityProvisionsConnection\x12>\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32(.datanode.api.v2.LiquidityProvisionsEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x80\x01\n!ObserveLiquidityProvisionsRequest\x12 \n\tmarket_id\x18\x01 \x01(\tH\x00R\x08marketId\x88\x01\x01\x12\x1e\n\x08party_id\x18\x02 \x01(\tH\x01R\x07partyId\x88\x01\x01\x42\x0c\n\n_market_idB\x0b\n\t_party_id"q\n"ObserveLiquidityProvisionsResponse\x12K\n\x14liquidity_provisions\x18\x01 \x03(\x0b\x32\x18.vega.LiquidityProvisionR\x13liquidityProvisions"\x81\x01\n\x18GetGovernanceDataRequest\x12$\n\x0bproposal_id\x18\x01 \x01(\tH\x00R\nproposalId\x88\x01\x01\x12!\n\treference\x18\x02 \x01(\tH\x01R\treference\x88\x01\x01\x42\x0e\n\x0c_proposal_idB\x0c\n\n_reference"E\n\x19GetGovernanceDataResponse\x12(\n\x04\x64\x61ta\x18\x01 \x01(\x0b\x32\x14.vega.GovernanceDataR\x04\x64\x61ta"\xfa\x04\n\x19ListGovernanceDataRequest\x12@\n\x0eproposal_state\x18\x01 \x01(\x0e\x32\x14.vega.Proposal.StateH\x00R\rproposalState\x88\x01\x01\x12Y\n\rproposal_type\x18\x02 \x01(\x0e\x32/.datanode.api.v2.ListGovernanceDataRequest.TypeH\x01R\x0cproposalType\x88\x01\x01\x12/\n\x11proposer_party_id\x18\x03 \x01(\tH\x02R\x0fproposerPartyId\x88\x01\x01\x12\x32\n\x12proposal_reference\x18\x04 \x01(\tH\x03R\x11proposalReference\x88\x01\x01\x12@\n\npagination\x18\x05 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x04R\npagination\x88\x01\x01"\xb7\x01\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0c\n\x08TYPE_ALL\x10\x01\x12\x13\n\x0fTYPE_NEW_MARKET\x10\x02\x12\x16\n\x12TYPE_UPDATE_MARKET\x10\x03\x12\x1b\n\x17TYPE_NETWORK_PARAMETERS\x10\x04\x12\x12\n\x0eTYPE_NEW_ASSET\x10\x05\x12\x16\n\x12TYPE_NEW_FREE_FORM\x10\x06\x12\x15\n\x11TYPE_UPDATE_ASSET\x10\x07\x42\x11\n\x0f_proposal_stateB\x10\n\x0e_proposal_typeB\x14\n\x12_proposer_party_idB\x15\n\x13_proposal_referenceB\r\n\x0b_pagination"g\n\x1aListGovernanceDataResponse\x12I\n\nconnection\x18\x01 \x01(\x0b\x32).datanode.api.v2.GovernanceDataConnectionR\nconnection"V\n\x12GovernanceDataEdge\x12(\n\x04node\x18\x01 \x01(\x0b\x32\x14.vega.GovernanceDataR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x8d\x01\n\x18GovernanceDataConnection\x12\x39\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32#.datanode.api.v2.GovernanceDataEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"G\n\x18ObserveGovernanceRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x42\x0b\n\t_party_id"E\n\x19ObserveGovernanceResponse\x12(\n\x04\x64\x61ta\x18\x01 \x01(\x0b\x32\x14.vega.GovernanceDataR\x04\x64\x61ta"\xed\x01\n\x16ListDelegationsRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12\x1c\n\x07node_id\x18\x02 \x01(\tH\x01R\x06nodeId\x88\x01\x01\x12\x1e\n\x08\x65poch_id\x18\x03 \x01(\tH\x02R\x07\x65pochId\x88\x01\x01\x12@\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x03R\npagination\x88\x01\x01\x42\x0b\n\t_party_idB\n\n\x08_node_idB\x0b\n\t_epoch_idB\r\n\x0b_pagination"c\n\x17ListDelegationsResponse\x12H\n\x0b\x64\x65legations\x18\x01 \x01(\x0b\x32&.datanode.api.v2.DelegationsConnectionR\x0b\x64\x65legations"N\n\x0e\x44\x65legationEdge\x12$\n\x04node\x18\x01 \x01(\x0b\x32\x10.vega.DelegationR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x86\x01\n\x15\x44\x65legationsConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.DelegationEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"r\n\x19ObserveDelegationsRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12\x1c\n\x07node_id\x18\x02 \x01(\tH\x01R\x06nodeId\x88\x01\x01\x42\x0b\n\t_party_idB\n\n\x08_node_id"N\n\x1aObserveDelegationsResponse\x12\x30\n\ndelegation\x18\x01 \x01(\x0b\x32\x10.vega.DelegationR\ndelegation"\x17\n\x15GetNetworkDataRequest"E\n\x16GetNetworkDataResponse\x12+\n\tnode_data\x18\x01 \x01(\x0b\x32\x0e.vega.NodeDataR\x08nodeData" \n\x0eGetNodeRequest\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id"1\n\x0fGetNodeResponse\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\n.vega.NodeR\x04node"\x93\x01\n\x10ListNodesRequest\x12 \n\tepoch_seq\x18\x01 \x01(\x04H\x00R\x08\x65pochSeq\x88\x01\x01\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\x0c\n\n_epoch_seqB\r\n\x0b_pagination"K\n\x11ListNodesResponse\x12\x36\n\x05nodes\x18\x01 \x01(\x0b\x32 .datanode.api.v2.NodesConnectionR\x05nodes"B\n\x08NodeEdge\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\n.vega.NodeR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"z\n\x0fNodesConnection\x12/\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x19.datanode.api.v2.NodeEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"|\n\x19ListNodeSignaturesRequest\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"g\n\x1aListNodeSignaturesResponse\x12I\n\nsignatures\x18\x01 \x01(\x0b\x32).datanode.api.v2.NodeSignaturesConnectionR\nsignatures"`\n\x11NodeSignatureEdge\x12\x33\n\x04node\x18\x01 \x01(\x0b\x32\x1f.vega.commands.v1.NodeSignatureR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x8c\x01\n\x18NodeSignaturesConnection\x12\x38\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32".datanode.api.v2.NodeSignatureEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"-\n\x0fGetEpochRequest\x12\x13\n\x02id\x18\x01 \x01(\x04H\x00R\x02id\x88\x01\x01\x42\x05\n\x03_id"5\n\x10GetEpochResponse\x12!\n\x05\x65poch\x18\x01 \x01(\x0b\x32\x0b.vega.EpochR\x05\x65poch"[\n\x12\x45stimateFeeRequest\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x14\n\x05price\x18\x02 \x01(\tR\x05price\x12\x12\n\x04size\x18\x03 \x01(\x04R\x04size"2\n\x13\x45stimateFeeResponse\x12\x1b\n\x03\x66\x65\x65\x18\x02 \x01(\x0b\x32\t.vega.FeeR\x03\x66\x65\x65"\xbf\x01\n\x15\x45stimateMarginRequest\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x1e\n\x04side\x18\x03 \x01(\x0e\x32\n.vega.SideR\x04side\x12$\n\x04type\x18\x04 \x01(\x0e\x32\x10.vega.Order.TypeR\x04type\x12\x12\n\x04size\x18\x05 \x01(\x04R\x04size\x12\x14\n\x05price\x18\x06 \x01(\tR\x05price"Q\n\x16\x45stimateMarginResponse\x12\x37\n\rmargin_levels\x18\x02 \x01(\x0b\x32\x12.vega.MarginLevelsR\x0cmarginLevels"o\n\x1cListNetworkParametersRequest\x12@\n\npagination\x18\x01 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"{\n\x1dListNetworkParametersResponse\x12Z\n\x12network_parameters\x18\x01 \x01(\x0b\x32+.datanode.api.v2.NetworkParameterConnectionR\x11networkParameters".\n\x1aGetNetworkParameterRequest\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key"b\n\x1bGetNetworkParameterResponse\x12\x43\n\x11network_parameter\x18\x01 \x01(\x0b\x32\x16.vega.NetworkParameterR\x10networkParameter"Z\n\x14NetworkParameterEdge\x12*\n\x04node\x18\x01 \x01(\x0b\x32\x16.vega.NetworkParameterR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x91\x01\n\x1aNetworkParameterConnection\x12;\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32%.datanode.api.v2.NetworkParameterEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"Z\n\nCheckpoint\x12\x12\n\x04hash\x18\x01 \x01(\tR\x04hash\x12\x1d\n\nblock_hash\x18\x02 \x01(\tR\tblockHash\x12\x19\n\x08\x61t_block\x18\x03 \x01(\x04R\x07\x61tBlock"i\n\x16ListCheckpointsRequest\x12@\n\npagination\x18\x01 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"c\n\x17ListCheckpointsResponse\x12H\n\x0b\x63heckpoints\x18\x01 \x01(\x0b\x32&.datanode.api.v2.CheckpointsConnectionR\x0b\x63heckpoints"Y\n\x0e\x43heckpointEdge\x12/\n\x04node\x18\x01 \x01(\x0b\x32\x1b.datanode.api.v2.CheckpointR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x86\x01\n\x15\x43heckpointsConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.CheckpointEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"}\n\x0fGetStakeRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"\x94\x01\n\x10GetStakeResponse\x12\x36\n\x17\x63urrent_stake_available\x18\x01 \x01(\tR\x15\x63urrentStakeAvailable\x12H\n\x0estake_linkings\x18\x02 \x01(\x0b\x32!.datanode.api.v2.StakesConnectionR\rstakeLinkings"\\\n\x10StakeLinkingEdge\x12\x30\n\x04node\x18\x01 \x01(\x0b\x32\x1c.vega.events.v1.StakeLinkingR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x83\x01\n\x10StakesConnection\x12\x37\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32!.datanode.api.v2.StakeLinkingEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"4\n\x15GetRiskFactorsRequest\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId"K\n\x16GetRiskFactorsResponse\x12\x31\n\x0brisk_factor\x18\x01 \x01(\x0b\x32\x10.vega.RiskFactorR\nriskFactor"\xa1\x01\n\x16ObserveEventBusRequest\x12\x30\n\x04type\x18\x01 \x03(\x0e\x32\x1c.vega.events.v1.BusEventTypeR\x04type\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x03 \x01(\tR\x07partyId\x12\x1d\n\nbatch_size\x18\x04 \x01(\x03R\tbatchSize"K\n\x17ObserveEventBusResponse\x12\x30\n\x06\x65vents\x18\x01 \x03(\x0b\x32\x18.vega.events.v1.BusEventR\x06\x65vents"\x1f\n\x1dObserveLedgerMovementsRequest"_\n\x1eObserveLedgerMovementsResponse\x12=\n\x0fledger_movement\x18\x01 \x01(\x0b\x32\x14.vega.LedgerMovementR\x0eledgerMovement"\x94\x01\n\x17ListKeyRotationsRequest\x12\x1c\n\x07node_id\x18\x01 \x01(\tH\x00R\x06nodeId\x88\x01\x01\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\n\n\x08_node_idB\r\n\x0b_pagination"`\n\x18ListKeyRotationsResponse\x12\x44\n\trotations\x18\x01 \x01(\x0b\x32&.datanode.api.v2.KeyRotationConnectionR\trotations"Z\n\x0fKeyRotationEdge\x12/\n\x04node\x18\x01 \x01(\x0b\x32\x1b.vega.events.v1.KeyRotationR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x87\x01\n\x15KeyRotationConnection\x12\x36\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32 .datanode.api.v2.KeyRotationEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x9c\x01\n\x1fListEthereumKeyRotationsRequest\x12\x1c\n\x07node_id\x18\x01 \x01(\tH\x00R\x06nodeId\x88\x01\x01\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\n\n\x08_node_idB\r\n\x0b_pagination"x\n ListEthereumKeyRotationsResponse\x12T\n\rkey_rotations\x18\x01 \x01(\x0b\x32/.datanode.api.v2.EthereumKeyRotationsConnectionR\x0ckeyRotations"\x98\x01\n\x1e\x45thereumKeyRotationsConnection\x12>\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32(.datanode.api.v2.EthereumKeyRotationEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"j\n\x17\x45thereumKeyRotationEdge\x12\x37\n\x04node\x18\x01 \x01(\x0b\x32#.vega.events.v1.EthereumKeyRotationR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x14\n\x12GetVegaTimeRequest"3\n\x13GetVegaTimeResponse\x12\x1c\n\ttimestamp\x18\x01 \x01(\x03R\ttimestamp"\x89\x01\n\tDateRange\x12,\n\x0fstart_timestamp\x18\x01 \x01(\x03H\x00R\x0estartTimestamp\x88\x01\x01\x12(\n\rend_timestamp\x18\x02 \x01(\x03H\x01R\x0c\x65ndTimestamp\x88\x01\x01\x42\x12\n\x10_start_timestampB\x10\n\x0e_end_timestamp"!\n\x1fGetProtocolUpgradeStatusRequest"8\n GetProtocolUpgradeStatusResponse\x12\x14\n\x05ready\x18\x01 \x01(\x08R\x05ready"\x83\x02\n#ListProtocolUpgradeProposalsRequest\x12J\n\x06status\x18\x01 \x01(\x0e\x32-.vega.events.v1.ProtocolUpgradeProposalStatusH\x00R\x06status\x88\x01\x01\x12$\n\x0b\x61pproved_by\x18\x02 \x01(\tH\x01R\napprovedBy\x88\x01\x01\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x02R\npagination\x88\x01\x01\x42\t\n\x07_statusB\x0e\n\x0c_approved_byB\r\n\x0b_pagination"\x98\x01\n$ListProtocolUpgradeProposalsResponse\x12p\n\x1aprotocol_upgrade_proposals\x18\x01 \x01(\x0b\x32\x32.datanode.api.v2.ProtocolUpgradeProposalConnectionR\x18protocolUpgradeProposals"\x9f\x01\n!ProtocolUpgradeProposalConnection\x12\x42\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32,.datanode.api.v2.ProtocolUpgradeProposalEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"o\n\x1bProtocolUpgradeProposalEdge\x12\x38\n\x04node\x18\x01 \x01(\x0b\x32$.vega.events.v1.ProtocolUpgradeEventR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"k\n\x18ListCoreSnapshotsRequest\x12@\n\npagination\x18\x01 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"k\n\x19ListCoreSnapshotsResponse\x12N\n\x0e\x63ore_snapshots\x18\x01 \x01(\x0b\x32\'.datanode.api.v2.CoreSnapshotConnectionR\rcoreSnapshots"\x89\x01\n\x16\x43oreSnapshotConnection\x12\x37\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32!.datanode.api.v2.CoreSnapshotEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"`\n\x10\x43oreSnapshotEdge\x12\x34\n\x04node\x18\x01 \x01(\x0b\x32 .vega.events.v1.CoreSnapshotDataR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\xd6\x01\n\x0eHistorySegment\x12\x1f\n\x0b\x66rom_height\x18\x01 \x01(\x03R\nfromHeight\x12\x1b\n\tto_height\x18\x02 \x01(\x03R\x08toHeight\x12\x19\n\x08\x63hain_id\x18\x03 \x01(\tR\x07\x63hainId\x12,\n\x12history_segment_id\x18\x04 \x01(\tR\x10historySegmentId\x12=\n\x1bprevious_history_segment_id\x18\x05 \x01(\tR\x18previousHistorySegmentId"+\n)GetMostRecentNetworkHistorySegmentRequest"\x84\x01\n*GetMostRecentNetworkHistorySegmentResponse\x12\x39\n\x07segment\x18\x01 \x01(\x0b\x32\x1f.datanode.api.v2.HistorySegmentR\x07segment\x12\x1b\n\tswarm_key\x18\x02 \x01(\tR\x08swarmKey"&\n$ListAllNetworkHistorySegmentsRequest"d\n%ListAllNetworkHistorySegmentsResponse\x12;\n\x08segments\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.HistorySegmentR\x08segments"-\n+GetActiveNetworkHistoryPeerAddressesRequest"Q\n,GetActiveNetworkHistoryPeerAddressesResponse\x12!\n\x0cip_addresses\x18\x01 \x03(\tR\x0bipAddresses"\r\n\x0bPingRequest"\x0e\n\x0cPingResponse*\xaa\x01\n\x10LedgerEntryField\x12"\n\x1eLEDGER_ENTRY_FIELD_UNSPECIFIED\x10\x00\x12&\n"LEDGER_ENTRY_FIELD_ACCOUNT_FROM_ID\x10\x01\x12$\n LEDGER_ENTRY_FIELD_ACCOUNT_TO_ID\x10\x02\x12$\n LEDGER_ENTRY_FIELD_TRANSFER_TYPE\x10\x03*\xb0\x01\n\x0c\x41\x63\x63ountField\x12\x1d\n\x19\x41\x43\x43OUNT_FIELD_UNSPECIFIED\x10\x00\x12\x14\n\x10\x41\x43\x43OUNT_FIELD_ID\x10\x01\x12\x1a\n\x16\x41\x43\x43OUNT_FIELD_PARTY_ID\x10\x02\x12\x1a\n\x16\x41\x43\x43OUNT_FIELD_ASSET_ID\x10\x03\x12\x1b\n\x17\x41\x43\x43OUNT_FIELD_MARKET_ID\x10\x04\x12\x16\n\x12\x41\x43\x43OUNT_FIELD_TYPE\x10\x05*\xad\x01\n\x11TransferDirection\x12"\n\x1eTRANSFER_DIRECTION_UNSPECIFIED\x10\x00\x12$\n TRANSFER_DIRECTION_TRANSFER_FROM\x10\x01\x12"\n\x1eTRANSFER_DIRECTION_TRANSFER_TO\x10\x02\x12*\n&TRANSFER_DIRECTION_TRANSFER_TO_OR_FROM\x10\x03\x32\xd6\x46\n\x12TradingDataService\x12[\n\x0cListAccounts\x12$.datanode.api.v2.ListAccountsRequest\x1a%.datanode.api.v2.ListAccountsResponse\x12\x66\n\x0fObserveAccounts\x12\'.datanode.api.v2.ObserveAccountsRequest\x1a(.datanode.api.v2.ObserveAccountsResponse0\x01\x12\x43\n\x04Info\x12\x1c.datanode.api.v2.InfoRequest\x1a\x1d.datanode.api.v2.InfoResponse\x12O\n\x08GetOrder\x12 .datanode.api.v2.GetOrderRequest\x1a!.datanode.api.v2.GetOrderResponse\x12U\n\nListOrders\x12".datanode.api.v2.ListOrdersRequest\x1a#.datanode.api.v2.ListOrdersResponse\x12j\n\x11ListOrderVersions\x12).datanode.api.v2.ListOrderVersionsRequest\x1a*.datanode.api.v2.ListOrderVersionsResponse\x12`\n\rObserveOrders\x12%.datanode.api.v2.ObserveOrdersRequest\x1a&.datanode.api.v2.ObserveOrdersResponse0\x01\x12^\n\rListPositions\x12%.datanode.api.v2.ListPositionsRequest\x1a&.datanode.api.v2.ListPositionsResponse\x12i\n\x10ObservePositions\x12(.datanode.api.v2.ObservePositionsRequest\x1a).datanode.api.v2.ObservePositionsResponse0\x01\x12l\n\x11ListLedgerEntries\x12).datanode.api.v2.ListLedgerEntriesRequest\x1a*.datanode.api.v2.ListLedgerEntriesResponse"\x00\x12r\n\x13\x45xportLedgerEntries\x12+.datanode.api.v2.ExportLedgerEntriesRequest\x1a,.datanode.api.v2.ExportLedgerEntriesResponse"\x00\x12o\n\x12ListBalanceChanges\x12*.datanode.api.v2.ListBalanceChangesRequest\x1a+.datanode.api.v2.ListBalanceChangesResponse"\x00\x12p\n\x13GetLatestMarketData\x12+.datanode.api.v2.GetLatestMarketDataRequest\x1a,.datanode.api.v2.GetLatestMarketDataResponse\x12s\n\x14ListLatestMarketData\x12,.datanode.api.v2.ListLatestMarketDataRequest\x1a-.datanode.api.v2.ListLatestMarketDataResponse\x12s\n\x14GetLatestMarketDepth\x12,.datanode.api.v2.GetLatestMarketDepthRequest\x1a-.datanode.api.v2.GetLatestMarketDepthResponse\x12r\n\x13ObserveMarketsDepth\x12+.datanode.api.v2.ObserveMarketsDepthRequest\x1a,.datanode.api.v2.ObserveMarketsDepthResponse0\x01\x12\x87\x01\n\x1aObserveMarketsDepthUpdates\x12\x32.datanode.api.v2.ObserveMarketsDepthUpdatesRequest\x1a\x33.datanode.api.v2.ObserveMarketsDepthUpdatesResponse0\x01\x12o\n\x12ObserveMarketsData\x12*.datanode.api.v2.ObserveMarketsDataRequest\x1a+.datanode.api.v2.ObserveMarketsDataResponse0\x01\x12\x7f\n\x18GetMarketDataHistoryByID\x12\x30.datanode.api.v2.GetMarketDataHistoryByIDRequest\x1a\x31.datanode.api.v2.GetMarketDataHistoryByIDResponse\x12^\n\rListTransfers\x12%.datanode.api.v2.ListTransfersRequest\x1a&.datanode.api.v2.ListTransfersResponse\x12g\n\x10GetNetworkLimits\x12(.datanode.api.v2.GetNetworkLimitsRequest\x1a).datanode.api.v2.GetNetworkLimitsResponse\x12\x61\n\x0eListCandleData\x12&.datanode.api.v2.ListCandleDataRequest\x1a\'.datanode.api.v2.ListCandleDataResponse\x12l\n\x11ObserveCandleData\x12).datanode.api.v2.ObserveCandleDataRequest\x1a*.datanode.api.v2.ObserveCandleDataResponse0\x01\x12p\n\x13ListCandleIntervals\x12+.datanode.api.v2.ListCandleIntervalsRequest\x1a,.datanode.api.v2.ListCandleIntervalsResponse\x12R\n\tListVotes\x12!.datanode.api.v2.ListVotesRequest\x1a".datanode.api.v2.ListVotesResponse\x12]\n\x0cObserveVotes\x12$.datanode.api.v2.ObserveVotesRequest\x1a%.datanode.api.v2.ObserveVotesResponse0\x01\x12\xa0\x01\n#ListERC20MultiSigSignerAddedBundles\x12;.datanode.api.v2.ListERC20MultiSigSignerAddedBundlesRequest\x1a<.datanode.api.v2.ListERC20MultiSigSignerAddedBundlesResponse\x12\xa6\x01\n%ListERC20MultiSigSignerRemovedBundles\x12=.datanode.api.v2.ListERC20MultiSigSignerRemovedBundlesRequest\x1a>.datanode.api.v2.ListERC20MultiSigSignerRemovedBundlesResponse\x12|\n\x17GetERC20ListAssetBundle\x12/.datanode.api.v2.GetERC20ListAssetBundleRequest\x1a\x30.datanode.api.v2.GetERC20ListAssetBundleResponse\x12\x8b\x01\n\x1cGetERC20SetAssetLimitsBundle\x12\x34.datanode.api.v2.GetERC20SetAssetLimitsBundleRequest\x1a\x35.datanode.api.v2.GetERC20SetAssetLimitsBundleResponse\x12\x85\x01\n\x1aGetERC20WithdrawalApproval\x12\x32.datanode.api.v2.GetERC20WithdrawalApprovalRequest\x1a\x33.datanode.api.v2.GetERC20WithdrawalApprovalResponse\x12[\n\x0cGetLastTrade\x12$.datanode.api.v2.GetLastTradeRequest\x1a%.datanode.api.v2.GetLastTradeResponse\x12U\n\nListTrades\x12".datanode.api.v2.ListTradesRequest\x1a#.datanode.api.v2.ListTradesResponse\x12`\n\rObserveTrades\x12%.datanode.api.v2.ObserveTradesRequest\x1a&.datanode.api.v2.ObserveTradesResponse0\x01\x12^\n\rGetOracleSpec\x12%.datanode.api.v2.GetOracleSpecRequest\x1a&.datanode.api.v2.GetOracleSpecResponse\x12\x64\n\x0fListOracleSpecs\x12\'.datanode.api.v2.ListOracleSpecsRequest\x1a(.datanode.api.v2.ListOracleSpecsResponse\x12\x61\n\x0eListOracleData\x12&.datanode.api.v2.ListOracleDataRequest\x1a\'.datanode.api.v2.ListOracleDataResponse\x12R\n\tGetMarket\x12!.datanode.api.v2.GetMarketRequest\x1a".datanode.api.v2.GetMarketResponse\x12X\n\x0bListMarkets\x12#.datanode.api.v2.ListMarketsRequest\x1a$.datanode.api.v2.ListMarketsResponse\x12O\n\x08GetParty\x12 .datanode.api.v2.GetPartyRequest\x1a!.datanode.api.v2.GetPartyResponse\x12X\n\x0bListParties\x12#.datanode.api.v2.ListPartiesRequest\x1a$.datanode.api.v2.ListPartiesResponse\x12g\n\x10ListMarginLevels\x12(.datanode.api.v2.ListMarginLevelsRequest\x1a).datanode.api.v2.ListMarginLevelsResponse\x12r\n\x13ObserveMarginLevels\x12+.datanode.api.v2.ObserveMarginLevelsRequest\x1a,.datanode.api.v2.ObserveMarginLevelsResponse0\x01\x12X\n\x0bListRewards\x12#.datanode.api.v2.ListRewardsRequest\x1a$.datanode.api.v2.ListRewardsResponse\x12p\n\x13ListRewardSummaries\x12+.datanode.api.v2.ListRewardSummariesRequest\x1a,.datanode.api.v2.ListRewardSummariesResponse\x12\x7f\n\x18ListEpochRewardSummaries\x12\x30.datanode.api.v2.ListEpochRewardSummariesRequest\x1a\x31.datanode.api.v2.ListEpochRewardSummariesResponse\x12\x63\n\x0eObserveRewards\x12&.datanode.api.v2.ObserveRewardsRequest\x1a\'.datanode.api.v2.ObserveRewardsResponse0\x01\x12U\n\nGetDeposit\x12".datanode.api.v2.GetDepositRequest\x1a#.datanode.api.v2.GetDepositResponse\x12[\n\x0cListDeposits\x12$.datanode.api.v2.ListDepositsRequest\x1a%.datanode.api.v2.ListDepositsResponse\x12^\n\rGetWithdrawal\x12%.datanode.api.v2.GetWithdrawalRequest\x1a&.datanode.api.v2.GetWithdrawalResponse\x12\x64\n\x0fListWithdrawals\x12\'.datanode.api.v2.ListWithdrawalsRequest\x1a(.datanode.api.v2.ListWithdrawalsResponse\x12O\n\x08GetAsset\x12 .datanode.api.v2.GetAssetRequest\x1a!.datanode.api.v2.GetAssetResponse\x12U\n\nListAssets\x12".datanode.api.v2.ListAssetsRequest\x1a#.datanode.api.v2.ListAssetsResponse\x12|\n\x17ListLiquidityProvisions\x12/.datanode.api.v2.ListLiquidityProvisionsRequest\x1a\x30.datanode.api.v2.ListLiquidityProvisionsResponse\x12\x87\x01\n\x1aObserveLiquidityProvisions\x12\x32.datanode.api.v2.ObserveLiquidityProvisionsRequest\x1a\x33.datanode.api.v2.ObserveLiquidityProvisionsResponse0\x01\x12j\n\x11GetGovernanceData\x12).datanode.api.v2.GetGovernanceDataRequest\x1a*.datanode.api.v2.GetGovernanceDataResponse\x12m\n\x12ListGovernanceData\x12*.datanode.api.v2.ListGovernanceDataRequest\x1a+.datanode.api.v2.ListGovernanceDataResponse\x12l\n\x11ObserveGovernance\x12).datanode.api.v2.ObserveGovernanceRequest\x1a*.datanode.api.v2.ObserveGovernanceResponse0\x01\x12\x64\n\x0fListDelegations\x12\'.datanode.api.v2.ListDelegationsRequest\x1a(.datanode.api.v2.ListDelegationsResponse\x12o\n\x12ObserveDelegations\x12*.datanode.api.v2.ObserveDelegationsRequest\x1a+.datanode.api.v2.ObserveDelegationsResponse0\x01\x12\x61\n\x0eGetNetworkData\x12&.datanode.api.v2.GetNetworkDataRequest\x1a\'.datanode.api.v2.GetNetworkDataResponse\x12L\n\x07GetNode\x12\x1f.datanode.api.v2.GetNodeRequest\x1a .datanode.api.v2.GetNodeResponse\x12R\n\tListNodes\x12!.datanode.api.v2.ListNodesRequest\x1a".datanode.api.v2.ListNodesResponse\x12m\n\x12ListNodeSignatures\x12*.datanode.api.v2.ListNodeSignaturesRequest\x1a+.datanode.api.v2.ListNodeSignaturesResponse\x12O\n\x08GetEpoch\x12 .datanode.api.v2.GetEpochRequest\x1a!.datanode.api.v2.GetEpochResponse\x12X\n\x0b\x45stimateFee\x12#.datanode.api.v2.EstimateFeeRequest\x1a$.datanode.api.v2.EstimateFeeResponse\x12\x61\n\x0e\x45stimateMargin\x12&.datanode.api.v2.EstimateMarginRequest\x1a\'.datanode.api.v2.EstimateMarginResponse\x12v\n\x15ListNetworkParameters\x12-.datanode.api.v2.ListNetworkParametersRequest\x1a..datanode.api.v2.ListNetworkParametersResponse\x12p\n\x13GetNetworkParameter\x12+.datanode.api.v2.GetNetworkParameterRequest\x1a,.datanode.api.v2.GetNetworkParameterResponse\x12\x64\n\x0fListCheckpoints\x12\'.datanode.api.v2.ListCheckpointsRequest\x1a(.datanode.api.v2.ListCheckpointsResponse\x12O\n\x08GetStake\x12 .datanode.api.v2.GetStakeRequest\x1a!.datanode.api.v2.GetStakeResponse\x12\x61\n\x0eGetRiskFactors\x12&.datanode.api.v2.GetRiskFactorsRequest\x1a\'.datanode.api.v2.GetRiskFactorsResponse\x12h\n\x0fObserveEventBus\x12\'.datanode.api.v2.ObserveEventBusRequest\x1a(.datanode.api.v2.ObserveEventBusResponse(\x01\x30\x01\x12{\n\x16ObserveLedgerMovements\x12..datanode.api.v2.ObserveLedgerMovementsRequest\x1a/.datanode.api.v2.ObserveLedgerMovementsResponse0\x01\x12g\n\x10ListKeyRotations\x12(.datanode.api.v2.ListKeyRotationsRequest\x1a).datanode.api.v2.ListKeyRotationsResponse\x12\x7f\n\x18ListEthereumKeyRotations\x12\x30.datanode.api.v2.ListEthereumKeyRotationsRequest\x1a\x31.datanode.api.v2.ListEthereumKeyRotationsResponse\x12X\n\x0bGetVegaTime\x12#.datanode.api.v2.GetVegaTimeRequest\x1a$.datanode.api.v2.GetVegaTimeResponse\x12\x7f\n\x18GetProtocolUpgradeStatus\x12\x30.datanode.api.v2.GetProtocolUpgradeStatusRequest\x1a\x31.datanode.api.v2.GetProtocolUpgradeStatusResponse\x12\x8b\x01\n\x1cListProtocolUpgradeProposals\x12\x34.datanode.api.v2.ListProtocolUpgradeProposalsRequest\x1a\x35.datanode.api.v2.ListProtocolUpgradeProposalsResponse\x12j\n\x11ListCoreSnapshots\x12).datanode.api.v2.ListCoreSnapshotsRequest\x1a*.datanode.api.v2.ListCoreSnapshotsResponse\x12\x9d\x01\n"GetMostRecentNetworkHistorySegment\x12:.datanode.api.v2.GetMostRecentNetworkHistorySegmentRequest\x1a;.datanode.api.v2.GetMostRecentNetworkHistorySegmentResponse\x12\x8e\x01\n\x1dListAllNetworkHistorySegments\x12\x35.datanode.api.v2.ListAllNetworkHistorySegmentsRequest\x1a\x36.datanode.api.v2.ListAllNetworkHistorySegmentsResponse\x12\xa3\x01\n$GetActiveNetworkHistoryPeerAddresses\x12<.datanode.api.v2.GetActiveNetworkHistoryPeerAddressesRequest\x1a=.datanode.api.v2.GetActiveNetworkHistoryPeerAddressesResponse\x12\x43\n\x04Ping\x12\x1c.datanode.api.v2.PingRequest\x1a\x1d.datanode.api.v2.PingResponseB}Z1code.vegaprotocol.io/vega/protos/data-node/api/v2\x92\x41G\x12\x1e\n\x13Vega data node APIs2\x07v0.67.0\x1a!lb.testnet.vega.xyz/datanode/rest*\x02\x01\x02\x62\x06proto3'
+    b'\n#data-node/api/v2/trading_data.proto\x12\x0f\x64\x61tanode.api.v2\x1a\x0fvega/vega.proto\x1a\x15vega/governance.proto\x1a\x12vega/markets.proto\x1a\x11vega/assets.proto\x1a\x11vega/oracle.proto\x1a\x1bvega/events/v1/events.proto\x1a)vega/commands/v1/validator_commands.proto\x1a.protoc-gen-openapiv2/options/annotations.proto"\\\n\x10OffsetPagination\x12\x12\n\x04skip\x18\x01 \x01(\x04R\x04skip\x12\x14\n\x05limit\x18\x02 \x01(\x04R\x05limit\x12\x1e\n\ndescending\x18\x03 \x01(\x08R\ndescending"\xd9\x01\n\nPagination\x12\x19\n\x05\x66irst\x18\x01 \x01(\x05H\x00R\x05\x66irst\x88\x01\x01\x12\x19\n\x05\x61\x66ter\x18\x02 \x01(\tH\x01R\x05\x61\x66ter\x88\x01\x01\x12\x17\n\x04last\x18\x03 \x01(\x05H\x02R\x04last\x88\x01\x01\x12\x1b\n\x06\x62\x65\x66ore\x18\x04 \x01(\tH\x03R\x06\x62\x65\x66ore\x88\x01\x01\x12&\n\x0cnewest_first\x18\x05 \x01(\x08H\x04R\x0bnewestFirst\x88\x01\x01\x42\x08\n\x06_firstB\x08\n\x06_afterB\x07\n\x05_lastB\t\n\x07_beforeB\x0f\n\r_newest_first"\x9c\x01\n\x08PageInfo\x12"\n\rhas_next_page\x18\x01 \x01(\x08R\x0bhasNextPage\x12*\n\x11has_previous_page\x18\x02 \x01(\x08R\x0fhasPreviousPage\x12!\n\x0cstart_cursor\x18\x03 \x01(\tR\x0bstartCursor\x12\x1d\n\nend_cursor\x18\x04 \x01(\tR\tendCursor"\x9a\x01\n\x0e\x41\x63\x63ountBalance\x12\x14\n\x05owner\x18\x02 \x01(\tR\x05owner\x12\x18\n\x07\x62\x61lance\x18\x03 \x01(\tR\x07\x62\x61lance\x12\x14\n\x05\x61sset\x18\x04 \x01(\tR\x05\x61sset\x12\x1b\n\tmarket_id\x18\x05 \x01(\tR\x08marketId\x12%\n\x04type\x18\x06 \x01(\x0e\x32\x11.vega.AccountTypeR\x04type"\x9e\x01\n\x13ListAccountsRequest\x12\x36\n\x06\x66ilter\x18\x01 \x01(\x0b\x32\x1e.datanode.api.v2.AccountFilterR\x06\x66ilter\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"W\n\x14ListAccountsResponse\x12?\n\x08\x61\x63\x63ounts\x18\x01 \x01(\x0b\x32#.datanode.api.v2.AccountsConnectionR\x08\x61\x63\x63ounts"\x80\x01\n\x12\x41\x63\x63ountsConnection\x12\x32\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1c.datanode.api.v2.AccountEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"Z\n\x0b\x41\x63\x63ountEdge\x12\x33\n\x04node\x18\x01 \x01(\x0b\x32\x1f.datanode.api.v2.AccountBalanceR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x8d\x01\n\x16ObserveAccountsRequest\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x14\n\x05\x61sset\x18\x03 \x01(\tR\x05\x61sset\x12%\n\x04type\x18\x04 \x01(\x0e\x32\x11.vega.AccountTypeR\x04type"\xa6\x01\n\x17ObserveAccountsResponse\x12\x42\n\x08snapshot\x18\x01 \x01(\x0b\x32$.datanode.api.v2.AccountSnapshotPageH\x00R\x08snapshot\x12;\n\x07updates\x18\x02 \x01(\x0b\x32\x1f.datanode.api.v2.AccountUpdatesH\x00R\x07updatesB\n\n\x08response"o\n\x13\x41\x63\x63ountSnapshotPage\x12;\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.AccountBalanceR\x08\x61\x63\x63ounts\x12\x1b\n\tlast_page\x18\x02 \x01(\x08R\x08lastPage"M\n\x0e\x41\x63\x63ountUpdates\x12;\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.AccountBalanceR\x08\x61\x63\x63ounts"\r\n\x0bInfoRequest"I\n\x0cInfoResponse\x12\x18\n\x07version\x18\x01 \x01(\tR\x07version\x12\x1f\n\x0b\x63ommit_hash\x18\x02 \x01(\tR\ncommitHash"W\n\x0fGetOrderRequest\x12\x19\n\x08order_id\x18\x01 \x01(\tR\x07orderId\x12\x1d\n\x07version\x18\x02 \x01(\x05H\x00R\x07version\x88\x01\x01\x42\n\n\x08_version"5\n\x10GetOrderResponse\x12!\n\x05order\x18\x01 \x01(\x0b\x32\x0b.vega.OrderR\x05order"\xd1\x01\n\x0bOrderFilter\x12.\n\x08statuses\x18\x01 \x03(\x0e\x32\x12.vega.Order.StatusR\x08statuses\x12&\n\x05types\x18\x02 \x03(\x0e\x32\x10.vega.Order.TypeR\x05types\x12=\n\x0etime_in_forces\x18\x03 \x03(\x0e\x32\x17.vega.Order.TimeInForceR\x0ctimeInForces\x12+\n\x11\x65xclude_liquidity\x18\x04 \x01(\x08R\x10\x65xcludeLiquidity"\xb7\x03\n\x11ListOrdersRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12 \n\tmarket_id\x18\x02 \x01(\tH\x01R\x08marketId\x88\x01\x01\x12!\n\treference\x18\x03 \x01(\tH\x02R\treference\x88\x01\x01\x12@\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x03R\npagination\x88\x01\x01\x12 \n\tlive_only\x18\x05 \x01(\x08H\x04R\x08liveOnly\x88\x01\x01\x12>\n\ndate_range\x18\x06 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x05R\tdateRange\x88\x01\x01\x12\x39\n\x06\x66ilter\x18\x07 \x01(\x0b\x32\x1c.datanode.api.v2.OrderFilterH\x06R\x06\x66ilter\x88\x01\x01\x42\x0b\n\t_party_idB\x0c\n\n_market_idB\x0c\n\n_referenceB\r\n\x0b_paginationB\x0c\n\n_live_onlyB\r\n\x0b_date_rangeB\t\n\x07_filter"N\n\x12ListOrdersResponse\x12\x38\n\x06orders\x18\x01 \x01(\x0b\x32 .datanode.api.v2.OrderConnectionR\x06orders"\x86\x01\n\x18ListOrderVersionsRequest\x12\x19\n\x08order_id\x18\x01 \x01(\tR\x07orderId\x12@\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"U\n\x19ListOrderVersionsResponse\x12\x38\n\x06orders\x18\x01 \x01(\x0b\x32 .datanode.api.v2.OrderConnectionR\x06orders"\xbb\x01\n\x14ObserveOrdersRequest\x12 \n\tmarket_id\x18\x01 \x01(\tH\x00R\x08marketId\x88\x01\x01\x12\x1e\n\x08party_id\x18\x02 \x01(\tH\x01R\x07partyId\x88\x01\x01\x12\x30\n\x11\x65xclude_liquidity\x18\x03 \x01(\x08H\x02R\x10\x65xcludeLiquidity\x88\x01\x01\x42\x0c\n\n_market_idB\x0b\n\t_party_idB\x14\n\x12_exclude_liquidity"\xa0\x01\n\x15ObserveOrdersResponse\x12@\n\x08snapshot\x18\x01 \x01(\x0b\x32".datanode.api.v2.OrderSnapshotPageH\x00R\x08snapshot\x12\x39\n\x07updates\x18\x02 \x01(\x0b\x32\x1d.datanode.api.v2.OrderUpdatesH\x00R\x07updatesB\n\n\x08response"U\n\x11OrderSnapshotPage\x12#\n\x06orders\x18\x01 \x03(\x0b\x32\x0b.vega.OrderR\x06orders\x12\x1b\n\tlast_page\x18\x02 \x01(\x08R\x08lastPage"3\n\x0cOrderUpdates\x12#\n\x06orders\x18\x01 \x03(\x0b\x32\x0b.vega.OrderR\x06orders"\xa3\x01\n\x14ListPositionsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01:\x02\x18\x01\x42\r\n\x0b_pagination"^\n\x15ListPositionsResponse\x12\x41\n\tpositions\x18\x01 \x01(\x0b\x32#.datanode.api.v2.PositionConnectionR\tpositions:\x02\x18\x01"M\n\x0fPositionsFilter\x12\x1b\n\tparty_ids\x18\x01 \x03(\tR\x08partyIds\x12\x1d\n\nmarket_ids\x18\x02 \x03(\tR\tmarketIds"\xa4\x01\n\x17ListAllPositionsRequest\x12\x38\n\x06\x66ilter\x18\x01 \x01(\x0b\x32 .datanode.api.v2.PositionsFilterR\x06\x66ilter\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"]\n\x18ListAllPositionsResponse\x12\x41\n\tpositions\x18\x01 \x01(\x0b\x32#.datanode.api.v2.PositionConnectionR\tpositions"J\n\x0cPositionEdge\x12"\n\x04node\x18\x01 \x01(\x0b\x32\x0e.vega.PositionR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x81\x01\n\x12PositionConnection\x12\x33\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1d.datanode.api.v2.PositionEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"v\n\x17ObservePositionsRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12 \n\tmarket_id\x18\x02 \x01(\tH\x01R\x08marketId\x88\x01\x01\x42\x0b\n\t_party_idB\x0c\n\n_market_id"\xa9\x01\n\x18ObservePositionsResponse\x12\x43\n\x08snapshot\x18\x01 \x01(\x0b\x32%.datanode.api.v2.PositionSnapshotPageH\x00R\x08snapshot\x12<\n\x07updates\x18\x02 \x01(\x0b\x32 .datanode.api.v2.PositionUpdatesH\x00R\x07updatesB\n\n\x08response"a\n\x14PositionSnapshotPage\x12,\n\tpositions\x18\x01 \x03(\x0b\x32\x0e.vega.PositionR\tpositions\x12\x1b\n\tlast_page\x18\x02 \x01(\x08R\x08lastPage"?\n\x0fPositionUpdates\x12,\n\tpositions\x18\x01 \x03(\x0b\x32\x0e.vega.PositionR\tpositions"\xa3\x02\n\x11LedgerEntryFilter\x12\x37\n\x18\x63lose_on_account_filters\x18\x01 \x01(\x08R\x15\x63loseOnAccountFilters\x12N\n\x13\x66rom_account_filter\x18\x02 \x01(\x0b\x32\x1e.datanode.api.v2.AccountFilterR\x11\x66romAccountFilter\x12J\n\x11to_account_filter\x18\x03 \x01(\x0b\x32\x1e.datanode.api.v2.AccountFilterR\x0ftoAccountFilter\x12\x39\n\x0etransfer_types\x18\x05 \x03(\x0e\x32\x12.vega.TransferTypeR\rtransferTypes"\xd9\x05\n\x15\x41ggregatedLedgerEntry\x12\x1c\n\ttimestamp\x18\x02 \x01(\x03R\ttimestamp\x12\x1a\n\x08quantity\x18\x03 \x01(\tR\x08quantity\x12\x37\n\rtransfer_type\x18\x04 \x01(\x0e\x32\x12.vega.TransferTypeR\x0ctransferType\x12\x1e\n\x08\x61sset_id\x18\x05 \x01(\tH\x00R\x07\x61ssetId\x88\x01\x01\x12=\n\x11\x66rom_account_type\x18\x06 \x01(\x0e\x32\x11.vega.AccountTypeR\x0f\x66romAccountType\x12\x39\n\x0fto_account_type\x18\x07 \x01(\x0e\x32\x11.vega.AccountTypeR\rtoAccountType\x12\x36\n\x15\x66rom_account_party_id\x18\x08 \x01(\tH\x01R\x12\x66romAccountPartyId\x88\x01\x01\x12\x32\n\x13to_account_party_id\x18\t \x01(\tH\x02R\x10toAccountPartyId\x88\x01\x01\x12\x38\n\x16\x66rom_account_market_id\x18\n \x01(\tH\x03R\x13\x66romAccountMarketId\x88\x01\x01\x12\x34\n\x14to_account_market_id\x18\x0b \x01(\tH\x04R\x11toAccountMarketId\x88\x01\x01\x12\x30\n\x14\x66rom_account_balance\x18\x0c \x01(\tR\x12\x66romAccountBalance\x12,\n\x12to_account_balance\x18\r \x01(\tR\x10toAccountBalanceB\x0b\n\t_asset_idB\x18\n\x16_from_account_party_idB\x16\n\x14_to_account_party_idB\x19\n\x17_from_account_market_idB\x17\n\x15_to_account_market_idJ\x04\x08\x01\x10\x02"\xf6\x01\n\x18ListLedgerEntriesRequest\x12:\n\x06\x66ilter\x18\x01 \x01(\x0b\x32".datanode.api.v2.LedgerEntryFilterR\x06\x66ilter\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x03 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"\xf2\x01\n\x1a\x45xportLedgerEntriesRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x19\n\x08\x61sset_id\x18\x02 \x01(\tR\x07\x61ssetId\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x04 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"v\n\x19ListLedgerEntriesResponse\x12Y\n\x0eledger_entries\x18\x01 \x01(\x0b\x32\x32.datanode.api.v2.AggregatedLedgerEntriesConnectionR\rledgerEntries"i\n\x1b\x45xportLedgerEntriesResponse\x12\x12\n\x04\x64\x61ta\x18\x01 \x01(\x0cR\x04\x64\x61ta\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"q\n\x1b\x41ggregatedLedgerEntriesEdge\x12:\n\x04node\x18\x01 \x01(\x0b\x32&.datanode.api.v2.AggregatedLedgerEntryR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x9f\x01\n!AggregatedLedgerEntriesConnection\x12\x42\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32,.datanode.api.v2.AggregatedLedgerEntriesEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xf3\x01\n\x19ListBalanceChangesRequest\x12\x36\n\x06\x66ilter\x18\x01 \x01(\x0b\x32\x1e.datanode.api.v2.AccountFilterR\x06\x66ilter\x12@\n\npagination\x18\x05 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x06 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"f\n\x1aListBalanceChangesResponse\x12H\n\x08\x62\x61lances\x18\x01 \x01(\x0b\x32,.datanode.api.v2.AggregatedBalanceConnectionR\x08\x62\x61lances"\xac\x02\n\x18GetBalanceHistoryRequest\x12\x36\n\x06\x66ilter\x18\x01 \x01(\x0b\x32\x1e.datanode.api.v2.AccountFilterR\x06\x66ilter\x12\x38\n\x08group_by\x18\x02 \x03(\x0e\x32\x1d.datanode.api.v2.AccountFieldR\x07groupBy\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x04 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"e\n\x19GetBalanceHistoryResponse\x12H\n\x08\x62\x61lances\x18\x01 \x01(\x0b\x32,.datanode.api.v2.AggregatedBalanceConnectionR\x08\x62\x61lances"g\n\x15\x41ggregatedBalanceEdge\x12\x36\n\x04node\x18\x01 \x01(\x0b\x32".datanode.api.v2.AggregatedBalanceR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x93\x01\n\x1b\x41ggregatedBalanceConnection\x12<\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32&.datanode.api.v2.AggregatedBalanceEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x9e\x01\n\rAccountFilter\x12\x19\n\x08\x61sset_id\x18\x01 \x01(\tR\x07\x61ssetId\x12\x1b\n\tparty_ids\x18\x02 \x03(\tR\x08partyIds\x12\x1d\n\nmarket_ids\x18\x03 \x03(\tR\tmarketIds\x12\x36\n\raccount_types\x18\x04 \x03(\x0e\x32\x11.vega.AccountTypeR\x0c\x61\x63\x63ountTypes"\xa1\x02\n\x11\x41ggregatedBalance\x12\x1c\n\ttimestamp\x18\x01 \x01(\x03R\ttimestamp\x12\x18\n\x07\x62\x61lance\x18\x02 \x01(\tR\x07\x62\x61lance\x12\x1e\n\x08party_id\x18\x04 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12\x1e\n\x08\x61sset_id\x18\x05 \x01(\tH\x01R\x07\x61ssetId\x88\x01\x01\x12 \n\tmarket_id\x18\x06 \x01(\tH\x02R\x08marketId\x88\x01\x01\x12\x39\n\x0c\x61\x63\x63ount_type\x18\x07 \x01(\x0e\x32\x11.vega.AccountTypeH\x03R\x0b\x61\x63\x63ountType\x88\x01\x01\x42\x0b\n\t_party_idB\x0b\n\t_asset_idB\x0c\n\n_market_idB\x0f\n\r_account_type";\n\x1aObserveMarketsDepthRequest\x12\x1d\n\nmarket_ids\x18\x01 \x03(\tR\tmarketIds"S\n\x1bObserveMarketsDepthResponse\x12\x34\n\x0cmarket_depth\x18\x01 \x03(\x0b\x32\x11.vega.MarketDepthR\x0bmarketDepth"B\n!ObserveMarketsDepthUpdatesRequest\x12\x1d\n\nmarket_ids\x18\x01 \x03(\tR\tmarketIds"U\n"ObserveMarketsDepthUpdatesResponse\x12/\n\x06update\x18\x01 \x03(\x0b\x32\x17.vega.MarketDepthUpdateR\x06update":\n\x19ObserveMarketsDataRequest\x12\x1d\n\nmarket_ids\x18\x01 \x03(\tR\tmarketIds"O\n\x1aObserveMarketsDataResponse\x12\x31\n\x0bmarket_data\x18\x01 \x03(\x0b\x32\x10.vega.MarketDataR\nmarketData"j\n\x1bGetLatestMarketDepthRequest\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12 \n\tmax_depth\x18\x02 \x01(\x04H\x00R\x08maxDepth\x88\x01\x01\x42\x0c\n\n_max_depth"\xda\x01\n\x1cGetLatestMarketDepthResponse\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12"\n\x03\x62uy\x18\x02 \x03(\x0b\x32\x10.vega.PriceLevelR\x03\x62uy\x12$\n\x04sell\x18\x03 \x03(\x0b\x32\x10.vega.PriceLevelR\x04sell\x12*\n\nlast_trade\x18\x04 \x01(\x0b\x32\x0b.vega.TradeR\tlastTrade\x12\'\n\x0fsequence_number\x18\x05 \x01(\x04R\x0esequenceNumber"\x1d\n\x1bListLatestMarketDataRequest"S\n\x1cListLatestMarketDataResponse\x12\x33\n\x0cmarkets_data\x18\x01 \x03(\x0b\x32\x10.vega.MarketDataR\x0bmarketsData"9\n\x1aGetLatestMarketDataRequest\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId"P\n\x1bGetLatestMarketDataResponse\x12\x31\n\x0bmarket_data\x18\x01 \x01(\x0b\x32\x10.vega.MarketDataR\nmarketData"\xfc\x02\n\x1fGetMarketDataHistoryByIDRequest\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12,\n\x0fstart_timestamp\x18\x02 \x01(\x03H\x00R\x0estartTimestamp\x88\x01\x01\x12(\n\rend_timestamp\x18\x03 \x01(\x03H\x01R\x0c\x65ndTimestamp\x88\x01\x01\x12@\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x02R\npagination\x88\x01\x01\x12W\n\x11offset_pagination\x18\x05 \x01(\x0b\x32!.datanode.api.v2.OffsetPaginationB\x02\x18\x01H\x03R\x10offsetPagination\x88\x01\x01\x42\x12\n\x10_start_timestampB\x10\n\x0e_end_timestampB\r\n\x0b_paginationB\x14\n\x12_offset_pagination"j\n GetMarketDataHistoryByIDResponse\x12\x46\n\x0bmarket_data\x18\x01 \x01(\x0b\x32%.datanode.api.v2.MarketDataConnectionR\nmarketData"N\n\x0eMarketDataEdge\x12$\n\x04node\x18\x01 \x01(\x0b\x32\x10.vega.MarketDataR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x85\x01\n\x14MarketDataConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.MarketDataEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo":\n\x1bMarketsDataSubscribeRequest\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId"Q\n\x1cMarketsDataSubscribeResponse\x12\x31\n\x0bmarket_data\x18\x01 \x03(\x0b\x32\x10.vega.MarketDataR\nmarketData"\xd1\x01\n\x14ListTransfersRequest\x12\x1b\n\x06pubkey\x18\x01 \x01(\tH\x00R\x06pubkey\x88\x01\x01\x12@\n\tdirection\x18\x02 \x01(\x0e\x32".datanode.api.v2.TransferDirectionR\tdirection\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\t\n\x07_pubkeyB\r\n\x0b_pagination"Z\n\x15ListTransfersResponse\x12\x41\n\ttransfers\x18\x01 \x01(\x0b\x32#.datanode.api.v2.TransferConnectionR\ttransfers"T\n\x0cTransferEdge\x12,\n\x04node\x18\x01 \x01(\x0b\x32\x18.vega.events.v1.TransferR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x81\x01\n\x12TransferConnection\x12\x33\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1d.datanode.api.v2.TransferEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x19\n\x17GetNetworkLimitsRequest"G\n\x18GetNetworkLimitsResponse\x12+\n\x06limits\x18\x01 \x01(\x0b\x32\x13.vega.NetworkLimitsR\x06limits"9\n\x1aListCandleIntervalsRequest\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId"M\n\x12IntervalToCandleId\x12\x1a\n\x08interval\x18\x01 \x01(\tR\x08interval\x12\x1b\n\tcandle_id\x18\x02 \x01(\tR\x08\x63\x61ndleId"u\n\x1bListCandleIntervalsResponse\x12V\n\x15interval_to_candle_id\x18\x01 \x03(\x0b\x32#.datanode.api.v2.IntervalToCandleIdR\x12intervalToCandleId"\xa7\x01\n\x06\x43\x61ndle\x12\x14\n\x05start\x18\x01 \x01(\x03R\x05start\x12\x1f\n\x0blast_update\x18\x02 \x01(\x03R\nlastUpdate\x12\x12\n\x04high\x18\x03 \x01(\tR\x04high\x12\x10\n\x03low\x18\x04 \x01(\tR\x03low\x12\x12\n\x04open\x18\x05 \x01(\tR\x04open\x12\x14\n\x05\x63lose\x18\x06 \x01(\tR\x05\x63lose\x12\x16\n\x06volume\x18\x07 \x01(\x04R\x06volume"7\n\x18ObserveCandleDataRequest\x12\x1b\n\tcandle_id\x18\x01 \x01(\tR\x08\x63\x61ndleId"L\n\x19ObserveCandleDataResponse\x12/\n\x06\x63\x61ndle\x18\x01 \x01(\x0b\x32\x17.datanode.api.v2.CandleR\x06\x63\x61ndle"\xfb\x01\n\x15ListCandleDataRequest\x12\x1b\n\tcandle_id\x18\x01 \x01(\tR\x08\x63\x61ndleId\x12%\n\x0e\x66rom_timestamp\x18\x02 \x01(\x03R\rfromTimestamp\x12!\n\x0cto_timestamp\x18\x03 \x01(\x03R\x0btoTimestamp\x12*\n\x08interval\x18\x04 \x01(\x0e\x32\x0e.vega.IntervalR\x08interval\x12@\n\npagination\x18\x05 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"Y\n\x16ListCandleDataResponse\x12?\n\x07\x63\x61ndles\x18\x01 \x01(\x0b\x32%.datanode.api.v2.CandleDataConnectionR\x07\x63\x61ndles"Q\n\nCandleEdge\x12+\n\x04node\x18\x01 \x01(\x0b\x32\x17.datanode.api.v2.CandleR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x81\x01\n\x14\x43\x61ndleDataConnection\x12\x31\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1b.datanode.api.v2.CandleEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xc6\x01\n\x10ListVotesRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12$\n\x0bproposal_id\x18\x02 \x01(\tH\x01R\nproposalId\x88\x01\x01\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x02R\npagination\x88\x01\x01\x42\x0b\n\t_party_idB\x0e\n\x0c_proposal_idB\r\n\x0b_pagination"J\n\x11ListVotesResponse\x12\x35\n\x05votes\x18\x01 \x01(\x0b\x32\x1f.datanode.api.v2.VoteConnectionR\x05votes"B\n\x08VoteEdge\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\n.vega.VoteR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"y\n\x0eVoteConnection\x12/\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x19.datanode.api.v2.VoteEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"x\n\x13ObserveVotesRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12$\n\x0bproposal_id\x18\x02 \x01(\tH\x01R\nproposalId\x88\x01\x01\x42\x0b\n\t_party_idB\x0e\n\x0c_proposal_id"6\n\x14ObserveVotesResponse\x12\x1e\n\x04vote\x18\x01 \x01(\x0b\x32\n.vega.VoteR\x04vote"\xbd\x01\n*ListERC20MultiSigSignerAddedBundlesRequest\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1c\n\tsubmitter\x18\x02 \x01(\tR\tsubmitter\x12\x1b\n\tepoch_seq\x18\x03 \x01(\tR\x08\x65pochSeq\x12;\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationR\npagination"|\n+ListERC20MultiSigSignerAddedBundlesResponse\x12M\n\x07\x62undles\x18\x01 \x01(\x0b\x32\x33.datanode.api.v2.ERC20MultiSigSignerAddedConnectionR\x07\x62undles"t\n\x1c\x45RC20MultiSigSignerAddedEdge\x12<\n\x04node\x18\x01 \x01(\x0b\x32(.vega.events.v1.ERC20MultiSigSignerAddedR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x81\x01\n"ERC20MultiSigSignerAddedBundleEdge\x12\x43\n\x04node\x18\x01 \x01(\x0b\x32/.datanode.api.v2.ERC20MultiSigSignerAddedBundleR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\xa7\x01\n"ERC20MultiSigSignerAddedConnection\x12I\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x33.datanode.api.v2.ERC20MultiSigSignerAddedBundleEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xce\x01\n\x1e\x45RC20MultiSigSignerAddedBundle\x12\x1d\n\nnew_signer\x18\x01 \x01(\tR\tnewSigner\x12\x1c\n\tsubmitter\x18\x02 \x01(\tR\tsubmitter\x12\x14\n\x05nonce\x18\x04 \x01(\tR\x05nonce\x12\x1c\n\ttimestamp\x18\x05 \x01(\x03R\ttimestamp\x12\x1e\n\nsignatures\x18\x06 \x01(\tR\nsignatures\x12\x1b\n\tepoch_seq\x18\x03 \x01(\tR\x08\x65pochSeq"\xbf\x01\n,ListERC20MultiSigSignerRemovedBundlesRequest\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1c\n\tsubmitter\x18\x02 \x01(\tR\tsubmitter\x12\x1b\n\tepoch_seq\x18\x03 \x01(\tR\x08\x65pochSeq\x12;\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationR\npagination"\x80\x01\n-ListERC20MultiSigSignerRemovedBundlesResponse\x12O\n\x07\x62undles\x18\x01 \x01(\x0b\x32\x35.datanode.api.v2.ERC20MultiSigSignerRemovedConnectionR\x07\x62undles"x\n\x1e\x45RC20MultiSigSignerRemovedEdge\x12>\n\x04node\x18\x01 \x01(\x0b\x32*.vega.events.v1.ERC20MultiSigSignerRemovedR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x85\x01\n$ERC20MultiSigSignerRemovedBundleEdge\x12\x45\n\x04node\x18\x01 \x01(\x0b\x32\x31.datanode.api.v2.ERC20MultiSigSignerRemovedBundleR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\xab\x01\n$ERC20MultiSigSignerRemovedConnection\x12K\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x35.datanode.api.v2.ERC20MultiSigSignerRemovedBundleEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xd0\x01\n ERC20MultiSigSignerRemovedBundle\x12\x1d\n\nold_signer\x18\x01 \x01(\tR\toldSigner\x12\x1c\n\tsubmitter\x18\x02 \x01(\tR\tsubmitter\x12\x14\n\x05nonce\x18\x04 \x01(\tR\x05nonce\x12\x1c\n\ttimestamp\x18\x05 \x01(\x03R\ttimestamp\x12\x1e\n\nsignatures\x18\x06 \x01(\tR\nsignatures\x12\x1b\n\tepoch_seq\x18\x07 \x01(\tR\x08\x65pochSeq";\n\x1eGetERC20ListAssetBundleRequest\x12\x19\n\x08\x61sset_id\x18\x01 \x01(\tR\x07\x61ssetId"\x9e\x01\n\x1fGetERC20ListAssetBundleResponse\x12!\n\x0c\x61sset_source\x18\x01 \x01(\tR\x0b\x61ssetSource\x12"\n\rvega_asset_id\x18\x02 \x01(\tR\x0bvegaAssetId\x12\x14\n\x05nonce\x18\x03 \x01(\tR\x05nonce\x12\x1e\n\nsignatures\x18\x04 \x01(\tR\nsignatures"F\n#GetERC20SetAssetLimitsBundleRequest\x12\x1f\n\x0bproposal_id\x18\x01 \x01(\tR\nproposalId"\xe8\x01\n$GetERC20SetAssetLimitsBundleResponse\x12!\n\x0c\x61sset_source\x18\x01 \x01(\tR\x0b\x61ssetSource\x12"\n\rvega_asset_id\x18\x02 \x01(\tR\x0bvegaAssetId\x12\x14\n\x05nonce\x18\x03 \x01(\tR\x05nonce\x12%\n\x0elifetime_limit\x18\x04 \x01(\tR\rlifetimeLimit\x12\x1c\n\tthreshold\x18\x05 \x01(\tR\tthreshold\x12\x1e\n\nsignatures\x18\x06 \x01(\tR\nsignatures"H\n!GetERC20WithdrawalApprovalRequest\x12#\n\rwithdrawal_id\x18\x01 \x01(\tR\x0cwithdrawalId"\xde\x01\n"GetERC20WithdrawalApprovalResponse\x12!\n\x0c\x61sset_source\x18\x01 \x01(\tR\x0b\x61ssetSource\x12\x16\n\x06\x61mount\x18\x02 \x01(\tR\x06\x61mount\x12\x14\n\x05nonce\x18\x04 \x01(\tR\x05nonce\x12\x1e\n\nsignatures\x18\x05 \x01(\tR\nsignatures\x12%\n\x0etarget_address\x18\x06 \x01(\tR\rtargetAddress\x12\x1a\n\x08\x63reation\x18\x07 \x01(\x03R\x08\x63reationJ\x04\x08\x03\x10\x04"2\n\x13GetLastTradeRequest\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId"9\n\x14GetLastTradeResponse\x12!\n\x05trade\x18\x01 \x01(\x0b\x32\x0b.vega.TradeR\x05trade"\xbd\x02\n\x11ListTradesRequest\x12 \n\tmarket_id\x18\x01 \x01(\tH\x00R\x08marketId\x88\x01\x01\x12\x1e\n\x08order_id\x18\x02 \x01(\tH\x01R\x07orderId\x88\x01\x01\x12\x1e\n\x08party_id\x18\x03 \x01(\tH\x02R\x07partyId\x88\x01\x01\x12@\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x03R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x05 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x04R\tdateRange\x88\x01\x01\x42\x0c\n\n_market_idB\x0b\n\t_order_idB\x0b\n\t_party_idB\r\n\x0b_paginationB\r\n\x0b_date_range"N\n\x12ListTradesResponse\x12\x38\n\x06trades\x18\x01 \x01(\x0b\x32 .datanode.api.v2.TradeConnectionR\x06trades"{\n\x0fTradeConnection\x12\x30\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1a.datanode.api.v2.TradeEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"D\n\tTradeEdge\x12\x1f\n\x04node\x18\x01 \x01(\x0b\x32\x0b.vega.TradeR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"s\n\x14ObserveTradesRequest\x12 \n\tmarket_id\x18\x01 \x01(\tH\x00R\x08marketId\x88\x01\x01\x12\x1e\n\x08party_id\x18\x02 \x01(\tH\x01R\x07partyId\x88\x01\x01\x42\x0c\n\n_market_idB\x0b\n\t_party_id"<\n\x15ObserveTradesResponse\x12#\n\x06trades\x18\x01 \x03(\x0b\x32\x0b.vega.TradeR\x06trades"<\n\x14GetOracleSpecRequest\x12$\n\x0eoracle_spec_id\x18\x01 \x01(\tR\x0coracleSpecId"J\n\x15GetOracleSpecResponse\x12\x31\n\x0boracle_spec\x18\x01 \x01(\x0b\x32\x10.vega.OracleSpecR\noracleSpec"i\n\x16ListOracleSpecsRequest\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"d\n\x17ListOracleSpecsResponse\x12I\n\x0coracle_specs\x18\x01 \x01(\x0b\x32&.datanode.api.v2.OracleSpecsConnectionR\x0boracleSpecs"\xa6\x01\n\x15ListOracleDataRequest\x12)\n\x0eoracle_spec_id\x18\x01 \x01(\tH\x00R\x0coracleSpecId\x88\x01\x01\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\x11\n\x0f_oracle_spec_idB\r\n\x0b_pagination"`\n\x16ListOracleDataResponse\x12\x46\n\x0boracle_data\x18\x01 \x01(\x0b\x32%.datanode.api.v2.OracleDataConnectionR\noracleData"N\n\x0eOracleSpecEdge\x12$\n\x04node\x18\x01 \x01(\x0b\x32\x10.vega.OracleSpecR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x86\x01\n\x15OracleSpecsConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.OracleSpecEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"N\n\x0eOracleDataEdge\x12$\n\x04node\x18\x01 \x01(\x0b\x32\x10.vega.OracleDataR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x85\x01\n\x14OracleDataConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.OracleDataEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"/\n\x10GetMarketRequest\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId"9\n\x11GetMarketResponse\x12$\n\x06market\x18\x01 \x01(\x0b\x32\x0c.vega.MarketR\x06market"\xa7\x01\n\x12ListMarketsRequest\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12,\n\x0finclude_settled\x18\x03 \x01(\x08H\x01R\x0eincludeSettled\x88\x01\x01\x42\r\n\x0b_paginationB\x12\n\x10_include_settled"R\n\x13ListMarketsResponse\x12;\n\x07markets\x18\x01 \x01(\x0b\x32!.datanode.api.v2.MarketConnectionR\x07markets"F\n\nMarketEdge\x12 \n\x04node\x18\x01 \x01(\x0b\x32\x0c.vega.MarketR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"}\n\x10MarketConnection\x12\x31\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1b.datanode.api.v2.MarketEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo",\n\x0fGetPartyRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId"5\n\x10GetPartyResponse\x12!\n\x05party\x18\x01 \x01(\x0b\x32\x0b.vega.PartyR\x05party"l\n\x12ListPartiesRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12;\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationR\npagination"Q\n\x13ListPartiesResponse\x12:\n\x07parties\x18\x01 \x01(\x0b\x32 .datanode.api.v2.PartyConnectionR\x07parties"D\n\tPartyEdge\x12\x1f\n\x04node\x18\x01 \x01(\x0b\x32\x0b.vega.PartyR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"{\n\x0fPartyConnection\x12\x30\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1a.datanode.api.v2.PartyEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"D\n\tOrderEdge\x12\x1f\n\x04node\x18\x01 \x01(\x0b\x32\x0b.vega.OrderR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x8e\x01\n\x17ListMarginLevelsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12;\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationR\npagination"b\n\x18ListMarginLevelsResponse\x12\x46\n\rmargin_levels\x18\x01 \x01(\x0b\x32!.datanode.api.v2.MarginConnectionR\x0cmarginLevels"g\n\x1aObserveMarginLevelsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12 \n\tmarket_id\x18\x02 \x01(\tH\x00R\x08marketId\x88\x01\x01\x42\x0c\n\n_market_id"V\n\x1bObserveMarginLevelsResponse\x12\x37\n\rmargin_levels\x18\x01 \x01(\x0b\x32\x12.vega.MarginLevelsR\x0cmarginLevels"{\n\x0fOrderConnection\x12\x30\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1a.datanode.api.v2.OrderEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"L\n\nMarginEdge\x12&\n\x04node\x18\x01 \x01(\x0b\x32\x12.vega.MarginLevelsR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"}\n\x10MarginConnection\x12\x31\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1b.datanode.api.v2.MarginEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x8d\x02\n\x12ListRewardsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x1e\n\x08\x61sset_id\x18\x02 \x01(\tH\x00R\x07\x61ssetId\x88\x01\x01\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x12"\n\nfrom_epoch\x18\x04 \x01(\x04H\x02R\tfromEpoch\x88\x01\x01\x12\x1e\n\x08to_epoch\x18\x05 \x01(\x04H\x03R\x07toEpoch\x88\x01\x01\x42\x0b\n\t_asset_idB\r\n\x0b_paginationB\r\n\x0b_from_epochB\x0b\n\t_to_epoch"S\n\x13ListRewardsResponse\x12<\n\x07rewards\x18\x01 \x01(\x0b\x32".datanode.api.v2.RewardsConnectionR\x07rewards"F\n\nRewardEdge\x12 \n\x04node\x18\x01 \x01(\x0b\x32\x0c.vega.RewardR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"~\n\x11RewardsConnection\x12\x31\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1b.datanode.api.v2.RewardEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xc7\x01\n\x1aListRewardSummariesRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12\x1e\n\x08\x61sset_id\x18\x02 \x01(\tH\x01R\x07\x61ssetId\x88\x01\x01\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x02R\npagination\x88\x01\x01\x42\x0b\n\t_party_idB\x0b\n\t_asset_idB\r\n\x0b_pagination"P\n\x1bListRewardSummariesResponse\x12\x31\n\tsummaries\x18\x01 \x03(\x0b\x32\x13.vega.RewardSummaryR\tsummaries"\xb1\x01\n\x13RewardSummaryFilter\x12\x1b\n\tasset_ids\x18\x01 \x03(\tR\x08\x61ssetIds\x12\x1d\n\nmarket_ids\x18\x02 \x03(\tR\tmarketIds\x12"\n\nfrom_epoch\x18\x03 \x01(\x04H\x00R\tfromEpoch\x88\x01\x01\x12\x1e\n\x08to_epoch\x18\x04 \x01(\x04H\x01R\x07toEpoch\x88\x01\x01\x42\r\n\x0b_from_epochB\x0b\n\t_to_epoch"\xb0\x01\n\x1fListEpochRewardSummariesRequest\x12<\n\x06\x66ilter\x18\x01 \x01(\x0b\x32$.datanode.api.v2.RewardSummaryFilterR\x06\x66ilter\x12@\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"o\n ListEpochRewardSummariesResponse\x12K\n\tsummaries\x18\x01 \x01(\x0b\x32-.datanode.api.v2.EpochRewardSummaryConnectionR\tsummaries"\x95\x01\n\x1c\x45pochRewardSummaryConnection\x12=\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\'.datanode.api.v2.EpochRewardSummaryEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"^\n\x16\x45pochRewardSummaryEdge\x12,\n\x04node\x18\x01 \x01(\x0b\x32\x18.vega.EpochRewardSummaryR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"q\n\x15ObserveRewardsRequest\x12\x1e\n\x08\x61sset_id\x18\x01 \x01(\tH\x00R\x07\x61ssetId\x88\x01\x01\x12\x1e\n\x08party_id\x18\x02 \x01(\tH\x01R\x07partyId\x88\x01\x01\x42\x0b\n\t_asset_idB\x0b\n\t_party_id">\n\x16ObserveRewardsResponse\x12$\n\x06reward\x18\x01 \x01(\x0b\x32\x0c.vega.RewardR\x06reward"#\n\x11GetDepositRequest\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id"=\n\x12GetDepositResponse\x12\'\n\x07\x64\x65posit\x18\x01 \x01(\x0b\x32\r.vega.DepositR\x07\x64\x65posit"\xd0\x01\n\x13ListDepositsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x03 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"W\n\x14ListDepositsResponse\x12?\n\x08\x64\x65posits\x18\x01 \x01(\x0b\x32#.datanode.api.v2.DepositsConnectionR\x08\x64\x65posits"H\n\x0b\x44\x65positEdge\x12!\n\x04node\x18\x01 \x01(\x0b\x32\r.vega.DepositR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x80\x01\n\x12\x44\x65positsConnection\x12\x32\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1c.datanode.api.v2.DepositEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"&\n\x14GetWithdrawalRequest\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id"I\n\x15GetWithdrawalResponse\x12\x30\n\nwithdrawal\x18\x01 \x01(\x0b\x32\x10.vega.WithdrawalR\nwithdrawal"\xd3\x01\n\x16ListWithdrawalsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x03 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"c\n\x17ListWithdrawalsResponse\x12H\n\x0bwithdrawals\x18\x01 \x01(\x0b\x32&.datanode.api.v2.WithdrawalsConnectionR\x0bwithdrawals"N\n\x0eWithdrawalEdge\x12$\n\x04node\x18\x01 \x01(\x0b\x32\x10.vega.WithdrawalR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x86\x01\n\x15WithdrawalsConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.WithdrawalEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo",\n\x0fGetAssetRequest\x12\x19\n\x08\x61sset_id\x18\x01 \x01(\tR\x07\x61ssetId"5\n\x10GetAssetResponse\x12!\n\x05\x61sset\x18\x01 \x01(\x0b\x32\x0b.vega.AssetR\x05\x61sset"\x91\x01\n\x11ListAssetsRequest\x12\x1e\n\x08\x61sset_id\x18\x01 \x01(\tH\x00R\x07\x61ssetId\x88\x01\x01\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\x0b\n\t_asset_idB\r\n\x0b_pagination"O\n\x12ListAssetsResponse\x12\x39\n\x06\x61ssets\x18\x01 \x01(\x0b\x32!.datanode.api.v2.AssetsConnectionR\x06\x61ssets"D\n\tAssetEdge\x12\x1f\n\x04node\x18\x01 \x01(\x0b\x32\x0b.vega.AssetR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"|\n\x10\x41ssetsConnection\x12\x30\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1a.datanode.api.v2.AssetEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xff\x01\n\x1eListLiquidityProvisionsRequest\x12 \n\tmarket_id\x18\x01 \x01(\tH\x00R\x08marketId\x88\x01\x01\x12\x1e\n\x08party_id\x18\x02 \x01(\tH\x01R\x07partyId\x88\x01\x01\x12!\n\treference\x18\x03 \x01(\tH\x02R\treference\x88\x01\x01\x12@\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x03R\npagination\x88\x01\x01\x42\x0c\n\n_market_idB\x0b\n\t_party_idB\x0c\n\n_referenceB\r\n\x0b_pagination"\x84\x01\n\x1fListLiquidityProvisionsResponse\x12\x61\n\x14liquidity_provisions\x18\x01 \x01(\x0b\x32..datanode.api.v2.LiquidityProvisionsConnectionR\x13liquidityProvisions"_\n\x17LiquidityProvisionsEdge\x12,\n\x04node\x18\x01 \x01(\x0b\x32\x18.vega.LiquidityProvisionR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x97\x01\n\x1dLiquidityProvisionsConnection\x12>\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32(.datanode.api.v2.LiquidityProvisionsEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x80\x01\n!ObserveLiquidityProvisionsRequest\x12 \n\tmarket_id\x18\x01 \x01(\tH\x00R\x08marketId\x88\x01\x01\x12\x1e\n\x08party_id\x18\x02 \x01(\tH\x01R\x07partyId\x88\x01\x01\x42\x0c\n\n_market_idB\x0b\n\t_party_id"q\n"ObserveLiquidityProvisionsResponse\x12K\n\x14liquidity_provisions\x18\x01 \x03(\x0b\x32\x18.vega.LiquidityProvisionR\x13liquidityProvisions"\x81\x01\n\x18GetGovernanceDataRequest\x12$\n\x0bproposal_id\x18\x01 \x01(\tH\x00R\nproposalId\x88\x01\x01\x12!\n\treference\x18\x02 \x01(\tH\x01R\treference\x88\x01\x01\x42\x0e\n\x0c_proposal_idB\x0c\n\n_reference"E\n\x19GetGovernanceDataResponse\x12(\n\x04\x64\x61ta\x18\x01 \x01(\x0b\x32\x14.vega.GovernanceDataR\x04\x64\x61ta"\xfa\x04\n\x19ListGovernanceDataRequest\x12@\n\x0eproposal_state\x18\x01 \x01(\x0e\x32\x14.vega.Proposal.StateH\x00R\rproposalState\x88\x01\x01\x12Y\n\rproposal_type\x18\x02 \x01(\x0e\x32/.datanode.api.v2.ListGovernanceDataRequest.TypeH\x01R\x0cproposalType\x88\x01\x01\x12/\n\x11proposer_party_id\x18\x03 \x01(\tH\x02R\x0fproposerPartyId\x88\x01\x01\x12\x32\n\x12proposal_reference\x18\x04 \x01(\tH\x03R\x11proposalReference\x88\x01\x01\x12@\n\npagination\x18\x05 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x04R\npagination\x88\x01\x01"\xb7\x01\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0c\n\x08TYPE_ALL\x10\x01\x12\x13\n\x0fTYPE_NEW_MARKET\x10\x02\x12\x16\n\x12TYPE_UPDATE_MARKET\x10\x03\x12\x1b\n\x17TYPE_NETWORK_PARAMETERS\x10\x04\x12\x12\n\x0eTYPE_NEW_ASSET\x10\x05\x12\x16\n\x12TYPE_NEW_FREE_FORM\x10\x06\x12\x15\n\x11TYPE_UPDATE_ASSET\x10\x07\x42\x11\n\x0f_proposal_stateB\x10\n\x0e_proposal_typeB\x14\n\x12_proposer_party_idB\x15\n\x13_proposal_referenceB\r\n\x0b_pagination"g\n\x1aListGovernanceDataResponse\x12I\n\nconnection\x18\x01 \x01(\x0b\x32).datanode.api.v2.GovernanceDataConnectionR\nconnection"V\n\x12GovernanceDataEdge\x12(\n\x04node\x18\x01 \x01(\x0b\x32\x14.vega.GovernanceDataR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x8d\x01\n\x18GovernanceDataConnection\x12\x39\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32#.datanode.api.v2.GovernanceDataEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"G\n\x18ObserveGovernanceRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x42\x0b\n\t_party_id"E\n\x19ObserveGovernanceResponse\x12(\n\x04\x64\x61ta\x18\x01 \x01(\x0b\x32\x14.vega.GovernanceDataR\x04\x64\x61ta"\xed\x01\n\x16ListDelegationsRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12\x1c\n\x07node_id\x18\x02 \x01(\tH\x01R\x06nodeId\x88\x01\x01\x12\x1e\n\x08\x65poch_id\x18\x03 \x01(\tH\x02R\x07\x65pochId\x88\x01\x01\x12@\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x03R\npagination\x88\x01\x01\x42\x0b\n\t_party_idB\n\n\x08_node_idB\x0b\n\t_epoch_idB\r\n\x0b_pagination"c\n\x17ListDelegationsResponse\x12H\n\x0b\x64\x65legations\x18\x01 \x01(\x0b\x32&.datanode.api.v2.DelegationsConnectionR\x0b\x64\x65legations"N\n\x0e\x44\x65legationEdge\x12$\n\x04node\x18\x01 \x01(\x0b\x32\x10.vega.DelegationR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x86\x01\n\x15\x44\x65legationsConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.DelegationEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"r\n\x19ObserveDelegationsRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12\x1c\n\x07node_id\x18\x02 \x01(\tH\x01R\x06nodeId\x88\x01\x01\x42\x0b\n\t_party_idB\n\n\x08_node_id"N\n\x1aObserveDelegationsResponse\x12\x30\n\ndelegation\x18\x01 \x01(\x0b\x32\x10.vega.DelegationR\ndelegation"\x17\n\x15GetNetworkDataRequest"E\n\x16GetNetworkDataResponse\x12+\n\tnode_data\x18\x01 \x01(\x0b\x32\x0e.vega.NodeDataR\x08nodeData" \n\x0eGetNodeRequest\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id"1\n\x0fGetNodeResponse\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\n.vega.NodeR\x04node"\x93\x01\n\x10ListNodesRequest\x12 \n\tepoch_seq\x18\x01 \x01(\x04H\x00R\x08\x65pochSeq\x88\x01\x01\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\x0c\n\n_epoch_seqB\r\n\x0b_pagination"K\n\x11ListNodesResponse\x12\x36\n\x05nodes\x18\x01 \x01(\x0b\x32 .datanode.api.v2.NodesConnectionR\x05nodes"B\n\x08NodeEdge\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\n.vega.NodeR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"z\n\x0fNodesConnection\x12/\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x19.datanode.api.v2.NodeEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"|\n\x19ListNodeSignaturesRequest\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"g\n\x1aListNodeSignaturesResponse\x12I\n\nsignatures\x18\x01 \x01(\x0b\x32).datanode.api.v2.NodeSignaturesConnectionR\nsignatures"`\n\x11NodeSignatureEdge\x12\x33\n\x04node\x18\x01 \x01(\x0b\x32\x1f.vega.commands.v1.NodeSignatureR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x8c\x01\n\x18NodeSignaturesConnection\x12\x38\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32".datanode.api.v2.NodeSignatureEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"-\n\x0fGetEpochRequest\x12\x13\n\x02id\x18\x01 \x01(\x04H\x00R\x02id\x88\x01\x01\x42\x05\n\x03_id"5\n\x10GetEpochResponse\x12!\n\x05\x65poch\x18\x01 \x01(\x0b\x32\x0b.vega.EpochR\x05\x65poch"[\n\x12\x45stimateFeeRequest\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x14\n\x05price\x18\x02 \x01(\tR\x05price\x12\x12\n\x04size\x18\x03 \x01(\x04R\x04size"2\n\x13\x45stimateFeeResponse\x12\x1b\n\x03\x66\x65\x65\x18\x02 \x01(\x0b\x32\t.vega.FeeR\x03\x66\x65\x65"\xbf\x01\n\x15\x45stimateMarginRequest\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x1e\n\x04side\x18\x03 \x01(\x0e\x32\n.vega.SideR\x04side\x12$\n\x04type\x18\x04 \x01(\x0e\x32\x10.vega.Order.TypeR\x04type\x12\x12\n\x04size\x18\x05 \x01(\x04R\x04size\x12\x14\n\x05price\x18\x06 \x01(\tR\x05price"Q\n\x16\x45stimateMarginResponse\x12\x37\n\rmargin_levels\x18\x02 \x01(\x0b\x32\x12.vega.MarginLevelsR\x0cmarginLevels"o\n\x1cListNetworkParametersRequest\x12@\n\npagination\x18\x01 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"{\n\x1dListNetworkParametersResponse\x12Z\n\x12network_parameters\x18\x01 \x01(\x0b\x32+.datanode.api.v2.NetworkParameterConnectionR\x11networkParameters".\n\x1aGetNetworkParameterRequest\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key"b\n\x1bGetNetworkParameterResponse\x12\x43\n\x11network_parameter\x18\x01 \x01(\x0b\x32\x16.vega.NetworkParameterR\x10networkParameter"Z\n\x14NetworkParameterEdge\x12*\n\x04node\x18\x01 \x01(\x0b\x32\x16.vega.NetworkParameterR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x91\x01\n\x1aNetworkParameterConnection\x12;\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32%.datanode.api.v2.NetworkParameterEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"Z\n\nCheckpoint\x12\x12\n\x04hash\x18\x01 \x01(\tR\x04hash\x12\x1d\n\nblock_hash\x18\x02 \x01(\tR\tblockHash\x12\x19\n\x08\x61t_block\x18\x03 \x01(\x04R\x07\x61tBlock"i\n\x16ListCheckpointsRequest\x12@\n\npagination\x18\x01 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"c\n\x17ListCheckpointsResponse\x12H\n\x0b\x63heckpoints\x18\x01 \x01(\x0b\x32&.datanode.api.v2.CheckpointsConnectionR\x0b\x63heckpoints"Y\n\x0e\x43heckpointEdge\x12/\n\x04node\x18\x01 \x01(\x0b\x32\x1b.datanode.api.v2.CheckpointR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x86\x01\n\x15\x43heckpointsConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.CheckpointEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"}\n\x0fGetStakeRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"\x94\x01\n\x10GetStakeResponse\x12\x36\n\x17\x63urrent_stake_available\x18\x01 \x01(\tR\x15\x63urrentStakeAvailable\x12H\n\x0estake_linkings\x18\x02 \x01(\x0b\x32!.datanode.api.v2.StakesConnectionR\rstakeLinkings"\\\n\x10StakeLinkingEdge\x12\x30\n\x04node\x18\x01 \x01(\x0b\x32\x1c.vega.events.v1.StakeLinkingR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x83\x01\n\x10StakesConnection\x12\x37\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32!.datanode.api.v2.StakeLinkingEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"4\n\x15GetRiskFactorsRequest\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId"K\n\x16GetRiskFactorsResponse\x12\x31\n\x0brisk_factor\x18\x01 \x01(\x0b\x32\x10.vega.RiskFactorR\nriskFactor"\xa1\x01\n\x16ObserveEventBusRequest\x12\x30\n\x04type\x18\x01 \x03(\x0e\x32\x1c.vega.events.v1.BusEventTypeR\x04type\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x03 \x01(\tR\x07partyId\x12\x1d\n\nbatch_size\x18\x04 \x01(\x03R\tbatchSize"K\n\x17ObserveEventBusResponse\x12\x30\n\x06\x65vents\x18\x01 \x03(\x0b\x32\x18.vega.events.v1.BusEventR\x06\x65vents"\x1f\n\x1dObserveLedgerMovementsRequest"_\n\x1eObserveLedgerMovementsResponse\x12=\n\x0fledger_movement\x18\x01 \x01(\x0b\x32\x14.vega.LedgerMovementR\x0eledgerMovement"\x94\x01\n\x17ListKeyRotationsRequest\x12\x1c\n\x07node_id\x18\x01 \x01(\tH\x00R\x06nodeId\x88\x01\x01\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\n\n\x08_node_idB\r\n\x0b_pagination"`\n\x18ListKeyRotationsResponse\x12\x44\n\trotations\x18\x01 \x01(\x0b\x32&.datanode.api.v2.KeyRotationConnectionR\trotations"Z\n\x0fKeyRotationEdge\x12/\n\x04node\x18\x01 \x01(\x0b\x32\x1b.vega.events.v1.KeyRotationR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x87\x01\n\x15KeyRotationConnection\x12\x36\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32 .datanode.api.v2.KeyRotationEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x9c\x01\n\x1fListEthereumKeyRotationsRequest\x12\x1c\n\x07node_id\x18\x01 \x01(\tH\x00R\x06nodeId\x88\x01\x01\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\n\n\x08_node_idB\r\n\x0b_pagination"x\n ListEthereumKeyRotationsResponse\x12T\n\rkey_rotations\x18\x01 \x01(\x0b\x32/.datanode.api.v2.EthereumKeyRotationsConnectionR\x0ckeyRotations"\x98\x01\n\x1e\x45thereumKeyRotationsConnection\x12>\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32(.datanode.api.v2.EthereumKeyRotationEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"j\n\x17\x45thereumKeyRotationEdge\x12\x37\n\x04node\x18\x01 \x01(\x0b\x32#.vega.events.v1.EthereumKeyRotationR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x14\n\x12GetVegaTimeRequest"3\n\x13GetVegaTimeResponse\x12\x1c\n\ttimestamp\x18\x01 \x01(\x03R\ttimestamp"\x89\x01\n\tDateRange\x12,\n\x0fstart_timestamp\x18\x01 \x01(\x03H\x00R\x0estartTimestamp\x88\x01\x01\x12(\n\rend_timestamp\x18\x02 \x01(\x03H\x01R\x0c\x65ndTimestamp\x88\x01\x01\x42\x12\n\x10_start_timestampB\x10\n\x0e_end_timestamp"!\n\x1fGetProtocolUpgradeStatusRequest"8\n GetProtocolUpgradeStatusResponse\x12\x14\n\x05ready\x18\x01 \x01(\x08R\x05ready"\x83\x02\n#ListProtocolUpgradeProposalsRequest\x12J\n\x06status\x18\x01 \x01(\x0e\x32-.vega.events.v1.ProtocolUpgradeProposalStatusH\x00R\x06status\x88\x01\x01\x12$\n\x0b\x61pproved_by\x18\x02 \x01(\tH\x01R\napprovedBy\x88\x01\x01\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x02R\npagination\x88\x01\x01\x42\t\n\x07_statusB\x0e\n\x0c_approved_byB\r\n\x0b_pagination"\x98\x01\n$ListProtocolUpgradeProposalsResponse\x12p\n\x1aprotocol_upgrade_proposals\x18\x01 \x01(\x0b\x32\x32.datanode.api.v2.ProtocolUpgradeProposalConnectionR\x18protocolUpgradeProposals"\x9f\x01\n!ProtocolUpgradeProposalConnection\x12\x42\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32,.datanode.api.v2.ProtocolUpgradeProposalEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"o\n\x1bProtocolUpgradeProposalEdge\x12\x38\n\x04node\x18\x01 \x01(\x0b\x32$.vega.events.v1.ProtocolUpgradeEventR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"k\n\x18ListCoreSnapshotsRequest\x12@\n\npagination\x18\x01 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"k\n\x19ListCoreSnapshotsResponse\x12N\n\x0e\x63ore_snapshots\x18\x01 \x01(\x0b\x32\'.datanode.api.v2.CoreSnapshotConnectionR\rcoreSnapshots"\x89\x01\n\x16\x43oreSnapshotConnection\x12\x37\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32!.datanode.api.v2.CoreSnapshotEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"`\n\x10\x43oreSnapshotEdge\x12\x34\n\x04node\x18\x01 \x01(\x0b\x32 .vega.events.v1.CoreSnapshotDataR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\xbb\x01\n\x0eHistorySegment\x12\x1f\n\x0b\x66rom_height\x18\x01 \x01(\x03R\nfromHeight\x12\x1b\n\tto_height\x18\x02 \x01(\x03R\x08toHeight\x12,\n\x12history_segment_id\x18\x03 \x01(\tR\x10historySegmentId\x12=\n\x1bprevious_history_segment_id\x18\x04 \x01(\tR\x18previousHistorySegmentId"+\n)GetMostRecentNetworkHistorySegmentRequest"\x8d\x01\n*GetMostRecentNetworkHistorySegmentResponse\x12\x39\n\x07segment\x18\x01 \x01(\x0b\x32\x1f.datanode.api.v2.HistorySegmentR\x07segment\x12$\n\x0eswarm_key_seed\x18\x02 \x01(\tR\x0cswarmKeySeed"&\n$ListAllNetworkHistorySegmentsRequest"d\n%ListAllNetworkHistorySegmentsResponse\x12;\n\x08segments\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.HistorySegmentR\x08segments"-\n+GetActiveNetworkHistoryPeerAddressesRequest"Q\n,GetActiveNetworkHistoryPeerAddressesResponse\x12!\n\x0cip_addresses\x18\x01 \x03(\tR\x0bipAddresses"\x1d\n\x1bNetworkHistoryStatusRequest"\xad\x01\n\x1cNetworkHistoryStatusResponse\x12!\n\x0cipfs_address\x18\x01 \x01(\tR\x0bipfsAddress\x12\x1b\n\tswarm_key\x18\x02 \x01(\tR\x08swarmKey\x12$\n\x0eswarm_key_seed\x18\x03 \x01(\tR\x0cswarmKeySeed\x12\'\n\x0f\x63onnected_peers\x18\x05 \x03(\tR\x0e\x63onnectedPeers"%\n#NetworkHistoryBootstrapPeersRequest"O\n$NetworkHistoryBootstrapPeersResponse\x12\'\n\x0f\x62ootstrap_peers\x18\x01 \x03(\tR\x0e\x62ootstrapPeers"\r\n\x0bPingRequest"\x0e\n\x0cPingResponse*\xaa\x01\n\x10LedgerEntryField\x12"\n\x1eLEDGER_ENTRY_FIELD_UNSPECIFIED\x10\x00\x12&\n"LEDGER_ENTRY_FIELD_ACCOUNT_FROM_ID\x10\x01\x12$\n LEDGER_ENTRY_FIELD_ACCOUNT_TO_ID\x10\x02\x12$\n LEDGER_ENTRY_FIELD_TRANSFER_TYPE\x10\x03*\xb0\x01\n\x0c\x41\x63\x63ountField\x12\x1d\n\x19\x41\x43\x43OUNT_FIELD_UNSPECIFIED\x10\x00\x12\x14\n\x10\x41\x43\x43OUNT_FIELD_ID\x10\x01\x12\x1a\n\x16\x41\x43\x43OUNT_FIELD_PARTY_ID\x10\x02\x12\x1a\n\x16\x41\x43\x43OUNT_FIELD_ASSET_ID\x10\x03\x12\x1b\n\x17\x41\x43\x43OUNT_FIELD_MARKET_ID\x10\x04\x12\x16\n\x12\x41\x43\x43OUNT_FIELD_TYPE\x10\x05*\xad\x01\n\x11TransferDirection\x12"\n\x1eTRANSFER_DIRECTION_UNSPECIFIED\x10\x00\x12$\n TRANSFER_DIRECTION_TRANSFER_FROM\x10\x01\x12"\n\x1eTRANSFER_DIRECTION_TRANSFER_TO\x10\x02\x12*\n&TRANSFER_DIRECTION_TRANSFER_TO_OR_FROM\x10\x03\x32\xc7I\n\x12TradingDataService\x12[\n\x0cListAccounts\x12$.datanode.api.v2.ListAccountsRequest\x1a%.datanode.api.v2.ListAccountsResponse\x12\x66\n\x0fObserveAccounts\x12\'.datanode.api.v2.ObserveAccountsRequest\x1a(.datanode.api.v2.ObserveAccountsResponse0\x01\x12\x43\n\x04Info\x12\x1c.datanode.api.v2.InfoRequest\x1a\x1d.datanode.api.v2.InfoResponse\x12O\n\x08GetOrder\x12 .datanode.api.v2.GetOrderRequest\x1a!.datanode.api.v2.GetOrderResponse\x12U\n\nListOrders\x12".datanode.api.v2.ListOrdersRequest\x1a#.datanode.api.v2.ListOrdersResponse\x12j\n\x11ListOrderVersions\x12).datanode.api.v2.ListOrderVersionsRequest\x1a*.datanode.api.v2.ListOrderVersionsResponse\x12`\n\rObserveOrders\x12%.datanode.api.v2.ObserveOrdersRequest\x1a&.datanode.api.v2.ObserveOrdersResponse0\x01\x12\x63\n\rListPositions\x12%.datanode.api.v2.ListPositionsRequest\x1a&.datanode.api.v2.ListPositionsResponse"\x03\x88\x02\x01\x12g\n\x10ListAllPositions\x12(.datanode.api.v2.ListAllPositionsRequest\x1a).datanode.api.v2.ListAllPositionsResponse\x12i\n\x10ObservePositions\x12(.datanode.api.v2.ObservePositionsRequest\x1a).datanode.api.v2.ObservePositionsResponse0\x01\x12l\n\x11ListLedgerEntries\x12).datanode.api.v2.ListLedgerEntriesRequest\x1a*.datanode.api.v2.ListLedgerEntriesResponse"\x00\x12r\n\x13\x45xportLedgerEntries\x12+.datanode.api.v2.ExportLedgerEntriesRequest\x1a,.datanode.api.v2.ExportLedgerEntriesResponse"\x00\x12o\n\x12ListBalanceChanges\x12*.datanode.api.v2.ListBalanceChangesRequest\x1a+.datanode.api.v2.ListBalanceChangesResponse"\x00\x12p\n\x13GetLatestMarketData\x12+.datanode.api.v2.GetLatestMarketDataRequest\x1a,.datanode.api.v2.GetLatestMarketDataResponse\x12s\n\x14ListLatestMarketData\x12,.datanode.api.v2.ListLatestMarketDataRequest\x1a-.datanode.api.v2.ListLatestMarketDataResponse\x12s\n\x14GetLatestMarketDepth\x12,.datanode.api.v2.GetLatestMarketDepthRequest\x1a-.datanode.api.v2.GetLatestMarketDepthResponse\x12r\n\x13ObserveMarketsDepth\x12+.datanode.api.v2.ObserveMarketsDepthRequest\x1a,.datanode.api.v2.ObserveMarketsDepthResponse0\x01\x12\x87\x01\n\x1aObserveMarketsDepthUpdates\x12\x32.datanode.api.v2.ObserveMarketsDepthUpdatesRequest\x1a\x33.datanode.api.v2.ObserveMarketsDepthUpdatesResponse0\x01\x12o\n\x12ObserveMarketsData\x12*.datanode.api.v2.ObserveMarketsDataRequest\x1a+.datanode.api.v2.ObserveMarketsDataResponse0\x01\x12\x7f\n\x18GetMarketDataHistoryByID\x12\x30.datanode.api.v2.GetMarketDataHistoryByIDRequest\x1a\x31.datanode.api.v2.GetMarketDataHistoryByIDResponse\x12^\n\rListTransfers\x12%.datanode.api.v2.ListTransfersRequest\x1a&.datanode.api.v2.ListTransfersResponse\x12g\n\x10GetNetworkLimits\x12(.datanode.api.v2.GetNetworkLimitsRequest\x1a).datanode.api.v2.GetNetworkLimitsResponse\x12\x61\n\x0eListCandleData\x12&.datanode.api.v2.ListCandleDataRequest\x1a\'.datanode.api.v2.ListCandleDataResponse\x12l\n\x11ObserveCandleData\x12).datanode.api.v2.ObserveCandleDataRequest\x1a*.datanode.api.v2.ObserveCandleDataResponse0\x01\x12p\n\x13ListCandleIntervals\x12+.datanode.api.v2.ListCandleIntervalsRequest\x1a,.datanode.api.v2.ListCandleIntervalsResponse\x12R\n\tListVotes\x12!.datanode.api.v2.ListVotesRequest\x1a".datanode.api.v2.ListVotesResponse\x12]\n\x0cObserveVotes\x12$.datanode.api.v2.ObserveVotesRequest\x1a%.datanode.api.v2.ObserveVotesResponse0\x01\x12\xa0\x01\n#ListERC20MultiSigSignerAddedBundles\x12;.datanode.api.v2.ListERC20MultiSigSignerAddedBundlesRequest\x1a<.datanode.api.v2.ListERC20MultiSigSignerAddedBundlesResponse\x12\xa6\x01\n%ListERC20MultiSigSignerRemovedBundles\x12=.datanode.api.v2.ListERC20MultiSigSignerRemovedBundlesRequest\x1a>.datanode.api.v2.ListERC20MultiSigSignerRemovedBundlesResponse\x12|\n\x17GetERC20ListAssetBundle\x12/.datanode.api.v2.GetERC20ListAssetBundleRequest\x1a\x30.datanode.api.v2.GetERC20ListAssetBundleResponse\x12\x8b\x01\n\x1cGetERC20SetAssetLimitsBundle\x12\x34.datanode.api.v2.GetERC20SetAssetLimitsBundleRequest\x1a\x35.datanode.api.v2.GetERC20SetAssetLimitsBundleResponse\x12\x85\x01\n\x1aGetERC20WithdrawalApproval\x12\x32.datanode.api.v2.GetERC20WithdrawalApprovalRequest\x1a\x33.datanode.api.v2.GetERC20WithdrawalApprovalResponse\x12[\n\x0cGetLastTrade\x12$.datanode.api.v2.GetLastTradeRequest\x1a%.datanode.api.v2.GetLastTradeResponse\x12U\n\nListTrades\x12".datanode.api.v2.ListTradesRequest\x1a#.datanode.api.v2.ListTradesResponse\x12`\n\rObserveTrades\x12%.datanode.api.v2.ObserveTradesRequest\x1a&.datanode.api.v2.ObserveTradesResponse0\x01\x12^\n\rGetOracleSpec\x12%.datanode.api.v2.GetOracleSpecRequest\x1a&.datanode.api.v2.GetOracleSpecResponse\x12\x64\n\x0fListOracleSpecs\x12\'.datanode.api.v2.ListOracleSpecsRequest\x1a(.datanode.api.v2.ListOracleSpecsResponse\x12\x61\n\x0eListOracleData\x12&.datanode.api.v2.ListOracleDataRequest\x1a\'.datanode.api.v2.ListOracleDataResponse\x12R\n\tGetMarket\x12!.datanode.api.v2.GetMarketRequest\x1a".datanode.api.v2.GetMarketResponse\x12X\n\x0bListMarkets\x12#.datanode.api.v2.ListMarketsRequest\x1a$.datanode.api.v2.ListMarketsResponse\x12O\n\x08GetParty\x12 .datanode.api.v2.GetPartyRequest\x1a!.datanode.api.v2.GetPartyResponse\x12X\n\x0bListParties\x12#.datanode.api.v2.ListPartiesRequest\x1a$.datanode.api.v2.ListPartiesResponse\x12g\n\x10ListMarginLevels\x12(.datanode.api.v2.ListMarginLevelsRequest\x1a).datanode.api.v2.ListMarginLevelsResponse\x12r\n\x13ObserveMarginLevels\x12+.datanode.api.v2.ObserveMarginLevelsRequest\x1a,.datanode.api.v2.ObserveMarginLevelsResponse0\x01\x12X\n\x0bListRewards\x12#.datanode.api.v2.ListRewardsRequest\x1a$.datanode.api.v2.ListRewardsResponse\x12p\n\x13ListRewardSummaries\x12+.datanode.api.v2.ListRewardSummariesRequest\x1a,.datanode.api.v2.ListRewardSummariesResponse\x12\x7f\n\x18ListEpochRewardSummaries\x12\x30.datanode.api.v2.ListEpochRewardSummariesRequest\x1a\x31.datanode.api.v2.ListEpochRewardSummariesResponse\x12\x63\n\x0eObserveRewards\x12&.datanode.api.v2.ObserveRewardsRequest\x1a\'.datanode.api.v2.ObserveRewardsResponse0\x01\x12U\n\nGetDeposit\x12".datanode.api.v2.GetDepositRequest\x1a#.datanode.api.v2.GetDepositResponse\x12[\n\x0cListDeposits\x12$.datanode.api.v2.ListDepositsRequest\x1a%.datanode.api.v2.ListDepositsResponse\x12^\n\rGetWithdrawal\x12%.datanode.api.v2.GetWithdrawalRequest\x1a&.datanode.api.v2.GetWithdrawalResponse\x12\x64\n\x0fListWithdrawals\x12\'.datanode.api.v2.ListWithdrawalsRequest\x1a(.datanode.api.v2.ListWithdrawalsResponse\x12O\n\x08GetAsset\x12 .datanode.api.v2.GetAssetRequest\x1a!.datanode.api.v2.GetAssetResponse\x12U\n\nListAssets\x12".datanode.api.v2.ListAssetsRequest\x1a#.datanode.api.v2.ListAssetsResponse\x12|\n\x17ListLiquidityProvisions\x12/.datanode.api.v2.ListLiquidityProvisionsRequest\x1a\x30.datanode.api.v2.ListLiquidityProvisionsResponse\x12\x87\x01\n\x1aObserveLiquidityProvisions\x12\x32.datanode.api.v2.ObserveLiquidityProvisionsRequest\x1a\x33.datanode.api.v2.ObserveLiquidityProvisionsResponse0\x01\x12j\n\x11GetGovernanceData\x12).datanode.api.v2.GetGovernanceDataRequest\x1a*.datanode.api.v2.GetGovernanceDataResponse\x12m\n\x12ListGovernanceData\x12*.datanode.api.v2.ListGovernanceDataRequest\x1a+.datanode.api.v2.ListGovernanceDataResponse\x12l\n\x11ObserveGovernance\x12).datanode.api.v2.ObserveGovernanceRequest\x1a*.datanode.api.v2.ObserveGovernanceResponse0\x01\x12\x64\n\x0fListDelegations\x12\'.datanode.api.v2.ListDelegationsRequest\x1a(.datanode.api.v2.ListDelegationsResponse\x12o\n\x12ObserveDelegations\x12*.datanode.api.v2.ObserveDelegationsRequest\x1a+.datanode.api.v2.ObserveDelegationsResponse0\x01\x12\x61\n\x0eGetNetworkData\x12&.datanode.api.v2.GetNetworkDataRequest\x1a\'.datanode.api.v2.GetNetworkDataResponse\x12L\n\x07GetNode\x12\x1f.datanode.api.v2.GetNodeRequest\x1a .datanode.api.v2.GetNodeResponse\x12R\n\tListNodes\x12!.datanode.api.v2.ListNodesRequest\x1a".datanode.api.v2.ListNodesResponse\x12m\n\x12ListNodeSignatures\x12*.datanode.api.v2.ListNodeSignaturesRequest\x1a+.datanode.api.v2.ListNodeSignaturesResponse\x12O\n\x08GetEpoch\x12 .datanode.api.v2.GetEpochRequest\x1a!.datanode.api.v2.GetEpochResponse\x12X\n\x0b\x45stimateFee\x12#.datanode.api.v2.EstimateFeeRequest\x1a$.datanode.api.v2.EstimateFeeResponse\x12\x61\n\x0e\x45stimateMargin\x12&.datanode.api.v2.EstimateMarginRequest\x1a\'.datanode.api.v2.EstimateMarginResponse\x12v\n\x15ListNetworkParameters\x12-.datanode.api.v2.ListNetworkParametersRequest\x1a..datanode.api.v2.ListNetworkParametersResponse\x12p\n\x13GetNetworkParameter\x12+.datanode.api.v2.GetNetworkParameterRequest\x1a,.datanode.api.v2.GetNetworkParameterResponse\x12\x64\n\x0fListCheckpoints\x12\'.datanode.api.v2.ListCheckpointsRequest\x1a(.datanode.api.v2.ListCheckpointsResponse\x12O\n\x08GetStake\x12 .datanode.api.v2.GetStakeRequest\x1a!.datanode.api.v2.GetStakeResponse\x12\x61\n\x0eGetRiskFactors\x12&.datanode.api.v2.GetRiskFactorsRequest\x1a\'.datanode.api.v2.GetRiskFactorsResponse\x12h\n\x0fObserveEventBus\x12\'.datanode.api.v2.ObserveEventBusRequest\x1a(.datanode.api.v2.ObserveEventBusResponse(\x01\x30\x01\x12{\n\x16ObserveLedgerMovements\x12..datanode.api.v2.ObserveLedgerMovementsRequest\x1a/.datanode.api.v2.ObserveLedgerMovementsResponse0\x01\x12g\n\x10ListKeyRotations\x12(.datanode.api.v2.ListKeyRotationsRequest\x1a).datanode.api.v2.ListKeyRotationsResponse\x12\x7f\n\x18ListEthereumKeyRotations\x12\x30.datanode.api.v2.ListEthereumKeyRotationsRequest\x1a\x31.datanode.api.v2.ListEthereumKeyRotationsResponse\x12X\n\x0bGetVegaTime\x12#.datanode.api.v2.GetVegaTimeRequest\x1a$.datanode.api.v2.GetVegaTimeResponse\x12\x7f\n\x18GetProtocolUpgradeStatus\x12\x30.datanode.api.v2.GetProtocolUpgradeStatusRequest\x1a\x31.datanode.api.v2.GetProtocolUpgradeStatusResponse\x12\x8b\x01\n\x1cListProtocolUpgradeProposals\x12\x34.datanode.api.v2.ListProtocolUpgradeProposalsRequest\x1a\x35.datanode.api.v2.ListProtocolUpgradeProposalsResponse\x12j\n\x11ListCoreSnapshots\x12).datanode.api.v2.ListCoreSnapshotsRequest\x1a*.datanode.api.v2.ListCoreSnapshotsResponse\x12\x9d\x01\n"GetMostRecentNetworkHistorySegment\x12:.datanode.api.v2.GetMostRecentNetworkHistorySegmentRequest\x1a;.datanode.api.v2.GetMostRecentNetworkHistorySegmentResponse\x12\x8e\x01\n\x1dListAllNetworkHistorySegments\x12\x35.datanode.api.v2.ListAllNetworkHistorySegmentsRequest\x1a\x36.datanode.api.v2.ListAllNetworkHistorySegmentsResponse\x12\xa3\x01\n$GetActiveNetworkHistoryPeerAddresses\x12<.datanode.api.v2.GetActiveNetworkHistoryPeerAddressesRequest\x1a=.datanode.api.v2.GetActiveNetworkHistoryPeerAddressesResponse\x12s\n\x14NetworkHistoryStatus\x12,.datanode.api.v2.NetworkHistoryStatusRequest\x1a-.datanode.api.v2.NetworkHistoryStatusResponse\x12\x8b\x01\n\x1cNetworkHistoryBootstrapPeers\x12\x34.datanode.api.v2.NetworkHistoryBootstrapPeersRequest\x1a\x35.datanode.api.v2.NetworkHistoryBootstrapPeersResponse\x12\x43\n\x04Ping\x12\x1c.datanode.api.v2.PingRequest\x1a\x1d.datanode.api.v2.PingResponseB\x81\x01Z1code.vegaprotocol.io/vega/protos/data-node/api/v2\x92\x41K\x12"\n\x13Vega data node APIs2\x0bv0.68.0-dev\x1a!lb.testnet.vega.xyz/datanode/rest*\x02\x01\x02\x62\x06proto3'
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(
     DESCRIPTOR, "data_node.api.v2.trading_data_pb2", globals()
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
-    DESCRIPTOR._serialized_options = b"Z1code.vegaprotocol.io/vega/protos/data-node/api/v2\222AG\022\036\n\023Vega data node APIs2\007v0.67.0\032!lb.testnet.vega.xyz/datanode/rest*\002\001\002"
+    DESCRIPTOR._serialized_options = b'Z1code.vegaprotocol.io/vega/protos/data-node/api/v2\222AK\022"\n\023Vega data node APIs2\013v0.68.0-dev\032!lb.testnet.vega.xyz/datanode/rest*\002\001\002'
+    _LISTPOSITIONSREQUEST._options = None
+    _LISTPOSITIONSREQUEST._serialized_options = b"\030\001"
+    _LISTPOSITIONSRESPONSE._options = None
+    _LISTPOSITIONSRESPONSE._serialized_options = b"\030\001"
     _GETMARKETDATAHISTORYBYIDREQUEST.fields_by_name["offset_pagination"]._options = None
     _GETMARKETDATAHISTORYBYIDREQUEST.fields_by_name[
         "offset_pagination"
     ]._serialized_options = b"\030\001"
-    _LEDGERENTRYFIELD._serialized_start = 31916
-    _LEDGERENTRYFIELD._serialized_end = 32086
-    _ACCOUNTFIELD._serialized_start = 32089
-    _ACCOUNTFIELD._serialized_end = 32265
-    _TRANSFERDIRECTION._serialized_start = 32268
-    _TRANSFERDIRECTION._serialized_end = 32441
+    _TRADINGDATASERVICE.methods_by_name["ListPositions"]._options = None
+    _TRADINGDATASERVICE.methods_by_name[
+        "ListPositions"
+    ]._serialized_options = b"\210\002\001"
+    _LEDGERENTRYFIELD._serialized_start = 32883
+    _LEDGERENTRYFIELD._serialized_end = 33053
+    _ACCOUNTFIELD._serialized_start = 33056
+    _ACCOUNTFIELD._serialized_end = 33232
+    _TRANSFERDIRECTION._serialized_start = 33235
+    _TRANSFERDIRECTION._serialized_end = 33408
     _OFFSETPAGINATION._serialized_start = 274
     _OFFSETPAGINATION._serialized_end = 366
     _PAGINATION._serialized_start = 369
     _PAGINATION._serialized_end = 586
     _PAGEINFO._serialized_start = 589
     _PAGEINFO._serialized_end = 745
     _ACCOUNTBALANCE._serialized_start = 748
@@ -95,489 +102,505 @@
     _OBSERVEORDERSRESPONSE._serialized_start = 3265
     _OBSERVEORDERSRESPONSE._serialized_end = 3425
     _ORDERSNAPSHOTPAGE._serialized_start = 3427
     _ORDERSNAPSHOTPAGE._serialized_end = 3512
     _ORDERUPDATES._serialized_start = 3514
     _ORDERUPDATES._serialized_end = 3565
     _LISTPOSITIONSREQUEST._serialized_start = 3568
-    _LISTPOSITIONSREQUEST._serialized_end = 3727
-    _LISTPOSITIONSRESPONSE._serialized_start = 3729
-    _LISTPOSITIONSRESPONSE._serialized_end = 3819
-    _POSITIONEDGE._serialized_start = 3821
-    _POSITIONEDGE._serialized_end = 3895
-    _POSITIONCONNECTION._serialized_start = 3898
-    _POSITIONCONNECTION._serialized_end = 4027
-    _OBSERVEPOSITIONSREQUEST._serialized_start = 4029
-    _OBSERVEPOSITIONSREQUEST._serialized_end = 4147
-    _OBSERVEPOSITIONSRESPONSE._serialized_start = 4150
-    _OBSERVEPOSITIONSRESPONSE._serialized_end = 4319
-    _POSITIONSNAPSHOTPAGE._serialized_start = 4321
-    _POSITIONSNAPSHOTPAGE._serialized_end = 4418
-    _POSITIONUPDATES._serialized_start = 4420
-    _POSITIONUPDATES._serialized_end = 4483
-    _LEDGERENTRYFILTER._serialized_start = 4486
-    _LEDGERENTRYFILTER._serialized_end = 4777
-    _AGGREGATEDLEDGERENTRY._serialized_start = 4780
-    _AGGREGATEDLEDGERENTRY._serialized_end = 5509
-    _LISTLEDGERENTRIESREQUEST._serialized_start = 5512
-    _LISTLEDGERENTRIESREQUEST._serialized_end = 5758
-    _EXPORTLEDGERENTRIESREQUEST._serialized_start = 5761
-    _EXPORTLEDGERENTRIESREQUEST._serialized_end = 6003
-    _LISTLEDGERENTRIESRESPONSE._serialized_start = 6005
-    _LISTLEDGERENTRIESRESPONSE._serialized_end = 6123
-    _EXPORTLEDGERENTRIESRESPONSE._serialized_start = 6125
-    _EXPORTLEDGERENTRIESRESPONSE._serialized_end = 6230
-    _AGGREGATEDLEDGERENTRIESEDGE._serialized_start = 6232
-    _AGGREGATEDLEDGERENTRIESEDGE._serialized_end = 6345
-    _AGGREGATEDLEDGERENTRIESCONNECTION._serialized_start = 6348
-    _AGGREGATEDLEDGERENTRIESCONNECTION._serialized_end = 6507
-    _LISTBALANCECHANGESREQUEST._serialized_start = 6510
-    _LISTBALANCECHANGESREQUEST._serialized_end = 6753
-    _LISTBALANCECHANGESRESPONSE._serialized_start = 6755
-    _LISTBALANCECHANGESRESPONSE._serialized_end = 6857
-    _GETBALANCEHISTORYREQUEST._serialized_start = 6860
-    _GETBALANCEHISTORYREQUEST._serialized_end = 7160
-    _GETBALANCEHISTORYRESPONSE._serialized_start = 7162
-    _GETBALANCEHISTORYRESPONSE._serialized_end = 7263
-    _AGGREGATEDBALANCEEDGE._serialized_start = 7265
-    _AGGREGATEDBALANCEEDGE._serialized_end = 7368
-    _AGGREGATEDBALANCECONNECTION._serialized_start = 7371
-    _AGGREGATEDBALANCECONNECTION._serialized_end = 7518
-    _ACCOUNTFILTER._serialized_start = 7521
-    _ACCOUNTFILTER._serialized_end = 7679
-    _AGGREGATEDBALANCE._serialized_start = 7682
-    _AGGREGATEDBALANCE._serialized_end = 7971
-    _OBSERVEMARKETSDEPTHREQUEST._serialized_start = 7973
-    _OBSERVEMARKETSDEPTHREQUEST._serialized_end = 8032
-    _OBSERVEMARKETSDEPTHRESPONSE._serialized_start = 8034
-    _OBSERVEMARKETSDEPTHRESPONSE._serialized_end = 8117
-    _OBSERVEMARKETSDEPTHUPDATESREQUEST._serialized_start = 8119
-    _OBSERVEMARKETSDEPTHUPDATESREQUEST._serialized_end = 8185
-    _OBSERVEMARKETSDEPTHUPDATESRESPONSE._serialized_start = 8187
-    _OBSERVEMARKETSDEPTHUPDATESRESPONSE._serialized_end = 8272
-    _OBSERVEMARKETSDATAREQUEST._serialized_start = 8274
-    _OBSERVEMARKETSDATAREQUEST._serialized_end = 8332
-    _OBSERVEMARKETSDATARESPONSE._serialized_start = 8334
-    _OBSERVEMARKETSDATARESPONSE._serialized_end = 8413
-    _GETLATESTMARKETDEPTHREQUEST._serialized_start = 8415
-    _GETLATESTMARKETDEPTHREQUEST._serialized_end = 8521
-    _GETLATESTMARKETDEPTHRESPONSE._serialized_start = 8524
-    _GETLATESTMARKETDEPTHRESPONSE._serialized_end = 8742
-    _LISTLATESTMARKETDATAREQUEST._serialized_start = 8744
-    _LISTLATESTMARKETDATAREQUEST._serialized_end = 8773
-    _LISTLATESTMARKETDATARESPONSE._serialized_start = 8775
-    _LISTLATESTMARKETDATARESPONSE._serialized_end = 8858
-    _GETLATESTMARKETDATAREQUEST._serialized_start = 8860
-    _GETLATESTMARKETDATAREQUEST._serialized_end = 8917
-    _GETLATESTMARKETDATARESPONSE._serialized_start = 8919
-    _GETLATESTMARKETDATARESPONSE._serialized_end = 8999
-    _GETMARKETDATAHISTORYBYIDREQUEST._serialized_start = 9002
-    _GETMARKETDATAHISTORYBYIDREQUEST._serialized_end = 9382
-    _GETMARKETDATAHISTORYBYIDRESPONSE._serialized_start = 9384
-    _GETMARKETDATAHISTORYBYIDRESPONSE._serialized_end = 9490
-    _MARKETDATAEDGE._serialized_start = 9492
-    _MARKETDATAEDGE._serialized_end = 9570
-    _MARKETDATACONNECTION._serialized_start = 9573
-    _MARKETDATACONNECTION._serialized_end = 9706
-    _MARKETSDATASUBSCRIBEREQUEST._serialized_start = 9708
-    _MARKETSDATASUBSCRIBEREQUEST._serialized_end = 9766
-    _MARKETSDATASUBSCRIBERESPONSE._serialized_start = 9768
-    _MARKETSDATASUBSCRIBERESPONSE._serialized_end = 9849
-    _LISTTRANSFERSREQUEST._serialized_start = 9852
-    _LISTTRANSFERSREQUEST._serialized_end = 10061
-    _LISTTRANSFERSRESPONSE._serialized_start = 10063
-    _LISTTRANSFERSRESPONSE._serialized_end = 10153
-    _TRANSFEREDGE._serialized_start = 10155
-    _TRANSFEREDGE._serialized_end = 10239
-    _TRANSFERCONNECTION._serialized_start = 10242
-    _TRANSFERCONNECTION._serialized_end = 10371
-    _GETNETWORKLIMITSREQUEST._serialized_start = 10373
-    _GETNETWORKLIMITSREQUEST._serialized_end = 10398
-    _GETNETWORKLIMITSRESPONSE._serialized_start = 10400
-    _GETNETWORKLIMITSRESPONSE._serialized_end = 10471
-    _LISTCANDLEINTERVALSREQUEST._serialized_start = 10473
-    _LISTCANDLEINTERVALSREQUEST._serialized_end = 10530
-    _INTERVALTOCANDLEID._serialized_start = 10532
-    _INTERVALTOCANDLEID._serialized_end = 10609
-    _LISTCANDLEINTERVALSRESPONSE._serialized_start = 10611
-    _LISTCANDLEINTERVALSRESPONSE._serialized_end = 10728
-    _CANDLE._serialized_start = 10731
-    _CANDLE._serialized_end = 10898
-    _OBSERVECANDLEDATAREQUEST._serialized_start = 10900
-    _OBSERVECANDLEDATAREQUEST._serialized_end = 10955
-    _OBSERVECANDLEDATARESPONSE._serialized_start = 10957
-    _OBSERVECANDLEDATARESPONSE._serialized_end = 11033
-    _LISTCANDLEDATAREQUEST._serialized_start = 11036
-    _LISTCANDLEDATAREQUEST._serialized_end = 11287
-    _LISTCANDLEDATARESPONSE._serialized_start = 11289
-    _LISTCANDLEDATARESPONSE._serialized_end = 11378
-    _CANDLEEDGE._serialized_start = 11380
-    _CANDLEEDGE._serialized_end = 11461
-    _CANDLEDATACONNECTION._serialized_start = 11464
-    _CANDLEDATACONNECTION._serialized_end = 11593
-    _LISTVOTESREQUEST._serialized_start = 11596
-    _LISTVOTESREQUEST._serialized_end = 11794
-    _LISTVOTESRESPONSE._serialized_start = 11796
-    _LISTVOTESRESPONSE._serialized_end = 11870
-    _VOTEEDGE._serialized_start = 11872
-    _VOTEEDGE._serialized_end = 11938
-    _VOTECONNECTION._serialized_start = 11940
-    _VOTECONNECTION._serialized_end = 12061
-    _OBSERVEVOTESREQUEST._serialized_start = 12063
-    _OBSERVEVOTESREQUEST._serialized_end = 12183
-    _OBSERVEVOTESRESPONSE._serialized_start = 12185
-    _OBSERVEVOTESRESPONSE._serialized_end = 12239
-    _LISTERC20MULTISIGSIGNERADDEDBUNDLESREQUEST._serialized_start = 12242
-    _LISTERC20MULTISIGSIGNERADDEDBUNDLESREQUEST._serialized_end = 12431
-    _LISTERC20MULTISIGSIGNERADDEDBUNDLESRESPONSE._serialized_start = 12433
-    _LISTERC20MULTISIGSIGNERADDEDBUNDLESRESPONSE._serialized_end = 12557
-    _ERC20MULTISIGSIGNERADDEDEDGE._serialized_start = 12559
-    _ERC20MULTISIGSIGNERADDEDEDGE._serialized_end = 12675
-    _ERC20MULTISIGSIGNERADDEDBUNDLEEDGE._serialized_start = 12678
-    _ERC20MULTISIGSIGNERADDEDBUNDLEEDGE._serialized_end = 12807
-    _ERC20MULTISIGSIGNERADDEDCONNECTION._serialized_start = 12810
-    _ERC20MULTISIGSIGNERADDEDCONNECTION._serialized_end = 12977
-    _ERC20MULTISIGSIGNERADDEDBUNDLE._serialized_start = 12980
-    _ERC20MULTISIGSIGNERADDEDBUNDLE._serialized_end = 13186
-    _LISTERC20MULTISIGSIGNERREMOVEDBUNDLESREQUEST._serialized_start = 13189
-    _LISTERC20MULTISIGSIGNERREMOVEDBUNDLESREQUEST._serialized_end = 13380
-    _LISTERC20MULTISIGSIGNERREMOVEDBUNDLESRESPONSE._serialized_start = 13383
-    _LISTERC20MULTISIGSIGNERREMOVEDBUNDLESRESPONSE._serialized_end = 13511
-    _ERC20MULTISIGSIGNERREMOVEDEDGE._serialized_start = 13513
-    _ERC20MULTISIGSIGNERREMOVEDEDGE._serialized_end = 13633
-    _ERC20MULTISIGSIGNERREMOVEDBUNDLEEDGE._serialized_start = 13636
-    _ERC20MULTISIGSIGNERREMOVEDBUNDLEEDGE._serialized_end = 13769
-    _ERC20MULTISIGSIGNERREMOVEDCONNECTION._serialized_start = 13772
-    _ERC20MULTISIGSIGNERREMOVEDCONNECTION._serialized_end = 13943
-    _ERC20MULTISIGSIGNERREMOVEDBUNDLE._serialized_start = 13946
-    _ERC20MULTISIGSIGNERREMOVEDBUNDLE._serialized_end = 14154
-    _GETERC20LISTASSETBUNDLEREQUEST._serialized_start = 14156
-    _GETERC20LISTASSETBUNDLEREQUEST._serialized_end = 14215
-    _GETERC20LISTASSETBUNDLERESPONSE._serialized_start = 14218
-    _GETERC20LISTASSETBUNDLERESPONSE._serialized_end = 14376
-    _GETERC20SETASSETLIMITSBUNDLEREQUEST._serialized_start = 14378
-    _GETERC20SETASSETLIMITSBUNDLEREQUEST._serialized_end = 14448
-    _GETERC20SETASSETLIMITSBUNDLERESPONSE._serialized_start = 14451
-    _GETERC20SETASSETLIMITSBUNDLERESPONSE._serialized_end = 14683
-    _GETERC20WITHDRAWALAPPROVALREQUEST._serialized_start = 14685
-    _GETERC20WITHDRAWALAPPROVALREQUEST._serialized_end = 14757
-    _GETERC20WITHDRAWALAPPROVALRESPONSE._serialized_start = 14760
-    _GETERC20WITHDRAWALAPPROVALRESPONSE._serialized_end = 14982
-    _GETLASTTRADEREQUEST._serialized_start = 14984
-    _GETLASTTRADEREQUEST._serialized_end = 15034
-    _GETLASTTRADERESPONSE._serialized_start = 15036
-    _GETLASTTRADERESPONSE._serialized_end = 15093
-    _LISTTRADESREQUEST._serialized_start = 15096
-    _LISTTRADESREQUEST._serialized_end = 15413
-    _LISTTRADESRESPONSE._serialized_start = 15415
-    _LISTTRADESRESPONSE._serialized_end = 15493
-    _TRADECONNECTION._serialized_start = 15495
-    _TRADECONNECTION._serialized_end = 15618
-    _TRADEEDGE._serialized_start = 15620
-    _TRADEEDGE._serialized_end = 15688
-    _OBSERVETRADESREQUEST._serialized_start = 15690
-    _OBSERVETRADESREQUEST._serialized_end = 15805
-    _OBSERVETRADESRESPONSE._serialized_start = 15807
-    _OBSERVETRADESRESPONSE._serialized_end = 15867
-    _GETORACLESPECREQUEST._serialized_start = 15869
-    _GETORACLESPECREQUEST._serialized_end = 15929
-    _GETORACLESPECRESPONSE._serialized_start = 15931
-    _GETORACLESPECRESPONSE._serialized_end = 16005
-    _LISTORACLESPECSREQUEST._serialized_start = 16007
-    _LISTORACLESPECSREQUEST._serialized_end = 16112
-    _LISTORACLESPECSRESPONSE._serialized_start = 16114
-    _LISTORACLESPECSRESPONSE._serialized_end = 16214
-    _LISTORACLEDATAREQUEST._serialized_start = 16217
-    _LISTORACLEDATAREQUEST._serialized_end = 16383
-    _LISTORACLEDATARESPONSE._serialized_start = 16385
-    _LISTORACLEDATARESPONSE._serialized_end = 16481
-    _ORACLESPECEDGE._serialized_start = 16483
-    _ORACLESPECEDGE._serialized_end = 16561
-    _ORACLESPECSCONNECTION._serialized_start = 16564
-    _ORACLESPECSCONNECTION._serialized_end = 16698
-    _ORACLEDATAEDGE._serialized_start = 16700
-    _ORACLEDATAEDGE._serialized_end = 16778
-    _ORACLEDATACONNECTION._serialized_start = 16781
-    _ORACLEDATACONNECTION._serialized_end = 16914
-    _GETMARKETREQUEST._serialized_start = 16916
-    _GETMARKETREQUEST._serialized_end = 16963
-    _GETMARKETRESPONSE._serialized_start = 16965
-    _GETMARKETRESPONSE._serialized_end = 17022
-    _LISTMARKETSREQUEST._serialized_start = 17024
-    _LISTMARKETSREQUEST._serialized_end = 17125
-    _LISTMARKETSRESPONSE._serialized_start = 17127
-    _LISTMARKETSRESPONSE._serialized_end = 17209
-    _MARKETEDGE._serialized_start = 17211
-    _MARKETEDGE._serialized_end = 17281
-    _MARKETCONNECTION._serialized_start = 17283
-    _MARKETCONNECTION._serialized_end = 17408
-    _GETPARTYREQUEST._serialized_start = 17410
-    _GETPARTYREQUEST._serialized_end = 17454
-    _GETPARTYRESPONSE._serialized_start = 17456
-    _GETPARTYRESPONSE._serialized_end = 17509
-    _LISTPARTIESREQUEST._serialized_start = 17511
-    _LISTPARTIESREQUEST._serialized_end = 17619
-    _LISTPARTIESRESPONSE._serialized_start = 17621
-    _LISTPARTIESRESPONSE._serialized_end = 17702
-    _PARTYEDGE._serialized_start = 17704
-    _PARTYEDGE._serialized_end = 17772
-    _PARTYCONNECTION._serialized_start = 17774
-    _PARTYCONNECTION._serialized_end = 17897
-    _ORDEREDGE._serialized_start = 17899
-    _ORDEREDGE._serialized_end = 17967
-    _LISTMARGINLEVELSREQUEST._serialized_start = 17970
-    _LISTMARGINLEVELSREQUEST._serialized_end = 18112
-    _LISTMARGINLEVELSRESPONSE._serialized_start = 18114
-    _LISTMARGINLEVELSRESPONSE._serialized_end = 18212
-    _OBSERVEMARGINLEVELSREQUEST._serialized_start = 18214
-    _OBSERVEMARGINLEVELSREQUEST._serialized_end = 18317
-    _OBSERVEMARGINLEVELSRESPONSE._serialized_start = 18319
-    _OBSERVEMARGINLEVELSRESPONSE._serialized_end = 18405
-    _ORDERCONNECTION._serialized_start = 18407
-    _ORDERCONNECTION._serialized_end = 18530
-    _MARGINEDGE._serialized_start = 18532
-    _MARGINEDGE._serialized_end = 18608
-    _MARGINCONNECTION._serialized_start = 18610
-    _MARGINCONNECTION._serialized_end = 18735
-    _LISTREWARDSREQUEST._serialized_start = 18738
-    _LISTREWARDSREQUEST._serialized_end = 18911
-    _LISTREWARDSRESPONSE._serialized_start = 18913
-    _LISTREWARDSRESPONSE._serialized_end = 18996
-    _REWARDEDGE._serialized_start = 18998
-    _REWARDEDGE._serialized_end = 19068
-    _REWARDSCONNECTION._serialized_start = 19070
-    _REWARDSCONNECTION._serialized_end = 19196
-    _LISTREWARDSUMMARIESREQUEST._serialized_start = 19199
-    _LISTREWARDSUMMARIESREQUEST._serialized_end = 19398
-    _LISTREWARDSUMMARIESRESPONSE._serialized_start = 19400
-    _LISTREWARDSUMMARIESRESPONSE._serialized_end = 19480
-    _LISTEPOCHREWARDSUMMARIESREQUEST._serialized_start = 19483
-    _LISTEPOCHREWARDSUMMARIESREQUEST._serialized_end = 19693
-    _LISTEPOCHREWARDSUMMARIESRESPONSE._serialized_start = 19695
-    _LISTEPOCHREWARDSUMMARIESRESPONSE._serialized_end = 19806
-    _EPOCHREWARDSUMMARYCONNECTION._serialized_start = 19809
-    _EPOCHREWARDSUMMARYCONNECTION._serialized_end = 19958
-    _EPOCHREWARDSUMMARYEDGE._serialized_start = 19960
-    _EPOCHREWARDSUMMARYEDGE._serialized_end = 20054
-    _OBSERVEREWARDSREQUEST._serialized_start = 20056
-    _OBSERVEREWARDSREQUEST._serialized_end = 20169
-    _OBSERVEREWARDSRESPONSE._serialized_start = 20171
-    _OBSERVEREWARDSRESPONSE._serialized_end = 20233
-    _GETDEPOSITREQUEST._serialized_start = 20235
-    _GETDEPOSITREQUEST._serialized_end = 20270
-    _GETDEPOSITRESPONSE._serialized_start = 20272
-    _GETDEPOSITRESPONSE._serialized_end = 20333
-    _LISTDEPOSITSREQUEST._serialized_start = 20336
-    _LISTDEPOSITSREQUEST._serialized_end = 20544
-    _LISTDEPOSITSRESPONSE._serialized_start = 20546
-    _LISTDEPOSITSRESPONSE._serialized_end = 20633
-    _DEPOSITEDGE._serialized_start = 20635
-    _DEPOSITEDGE._serialized_end = 20707
-    _DEPOSITSCONNECTION._serialized_start = 20710
-    _DEPOSITSCONNECTION._serialized_end = 20838
-    _GETWITHDRAWALREQUEST._serialized_start = 20840
-    _GETWITHDRAWALREQUEST._serialized_end = 20878
-    _GETWITHDRAWALRESPONSE._serialized_start = 20880
-    _GETWITHDRAWALRESPONSE._serialized_end = 20953
-    _LISTWITHDRAWALSREQUEST._serialized_start = 20956
-    _LISTWITHDRAWALSREQUEST._serialized_end = 21167
-    _LISTWITHDRAWALSRESPONSE._serialized_start = 21169
-    _LISTWITHDRAWALSRESPONSE._serialized_end = 21268
-    _WITHDRAWALEDGE._serialized_start = 21270
-    _WITHDRAWALEDGE._serialized_end = 21348
-    _WITHDRAWALSCONNECTION._serialized_start = 21351
-    _WITHDRAWALSCONNECTION._serialized_end = 21485
-    _GETASSETREQUEST._serialized_start = 21487
-    _GETASSETREQUEST._serialized_end = 21531
-    _GETASSETRESPONSE._serialized_start = 21533
-    _GETASSETRESPONSE._serialized_end = 21586
-    _LISTASSETSREQUEST._serialized_start = 21589
-    _LISTASSETSREQUEST._serialized_end = 21734
-    _LISTASSETSRESPONSE._serialized_start = 21736
-    _LISTASSETSRESPONSE._serialized_end = 21815
-    _ASSETEDGE._serialized_start = 21817
-    _ASSETEDGE._serialized_end = 21885
-    _ASSETSCONNECTION._serialized_start = 21887
-    _ASSETSCONNECTION._serialized_end = 22011
-    _LISTLIQUIDITYPROVISIONSREQUEST._serialized_start = 22014
-    _LISTLIQUIDITYPROVISIONSREQUEST._serialized_end = 22269
-    _LISTLIQUIDITYPROVISIONSRESPONSE._serialized_start = 22272
-    _LISTLIQUIDITYPROVISIONSRESPONSE._serialized_end = 22404
-    _LIQUIDITYPROVISIONSEDGE._serialized_start = 22406
-    _LIQUIDITYPROVISIONSEDGE._serialized_end = 22501
-    _LIQUIDITYPROVISIONSCONNECTION._serialized_start = 22504
-    _LIQUIDITYPROVISIONSCONNECTION._serialized_end = 22655
-    _OBSERVELIQUIDITYPROVISIONSREQUEST._serialized_start = 22658
-    _OBSERVELIQUIDITYPROVISIONSREQUEST._serialized_end = 22786
-    _OBSERVELIQUIDITYPROVISIONSRESPONSE._serialized_start = 22788
-    _OBSERVELIQUIDITYPROVISIONSRESPONSE._serialized_end = 22901
-    _GETGOVERNANCEDATAREQUEST._serialized_start = 22904
-    _GETGOVERNANCEDATAREQUEST._serialized_end = 23033
-    _GETGOVERNANCEDATARESPONSE._serialized_start = 23035
-    _GETGOVERNANCEDATARESPONSE._serialized_end = 23104
-    _LISTGOVERNANCEDATAREQUEST._serialized_start = 23107
-    _LISTGOVERNANCEDATAREQUEST._serialized_end = 23741
-    _LISTGOVERNANCEDATAREQUEST_TYPE._serialized_start = 23461
-    _LISTGOVERNANCEDATAREQUEST_TYPE._serialized_end = 23644
-    _LISTGOVERNANCEDATARESPONSE._serialized_start = 23743
-    _LISTGOVERNANCEDATARESPONSE._serialized_end = 23846
-    _GOVERNANCEDATAEDGE._serialized_start = 23848
-    _GOVERNANCEDATAEDGE._serialized_end = 23934
-    _GOVERNANCEDATACONNECTION._serialized_start = 23937
-    _GOVERNANCEDATACONNECTION._serialized_end = 24078
-    _OBSERVEGOVERNANCEREQUEST._serialized_start = 24080
-    _OBSERVEGOVERNANCEREQUEST._serialized_end = 24151
-    _OBSERVEGOVERNANCERESPONSE._serialized_start = 24153
-    _OBSERVEGOVERNANCERESPONSE._serialized_end = 24222
-    _LISTDELEGATIONSREQUEST._serialized_start = 24225
-    _LISTDELEGATIONSREQUEST._serialized_end = 24462
-    _LISTDELEGATIONSRESPONSE._serialized_start = 24464
-    _LISTDELEGATIONSRESPONSE._serialized_end = 24563
-    _DELEGATIONEDGE._serialized_start = 24565
-    _DELEGATIONEDGE._serialized_end = 24643
-    _DELEGATIONSCONNECTION._serialized_start = 24646
-    _DELEGATIONSCONNECTION._serialized_end = 24780
-    _OBSERVEDELEGATIONSREQUEST._serialized_start = 24782
-    _OBSERVEDELEGATIONSREQUEST._serialized_end = 24896
-    _OBSERVEDELEGATIONSRESPONSE._serialized_start = 24898
-    _OBSERVEDELEGATIONSRESPONSE._serialized_end = 24976
-    _GETNETWORKDATAREQUEST._serialized_start = 24978
-    _GETNETWORKDATAREQUEST._serialized_end = 25001
-    _GETNETWORKDATARESPONSE._serialized_start = 25003
-    _GETNETWORKDATARESPONSE._serialized_end = 25072
-    _GETNODEREQUEST._serialized_start = 25074
-    _GETNODEREQUEST._serialized_end = 25106
-    _GETNODERESPONSE._serialized_start = 25108
-    _GETNODERESPONSE._serialized_end = 25157
-    _LISTNODESREQUEST._serialized_start = 25160
-    _LISTNODESREQUEST._serialized_end = 25307
-    _LISTNODESRESPONSE._serialized_start = 25309
-    _LISTNODESRESPONSE._serialized_end = 25384
-    _NODEEDGE._serialized_start = 25386
-    _NODEEDGE._serialized_end = 25452
-    _NODESCONNECTION._serialized_start = 25454
-    _NODESCONNECTION._serialized_end = 25576
-    _LISTNODESIGNATURESREQUEST._serialized_start = 25578
-    _LISTNODESIGNATURESREQUEST._serialized_end = 25702
-    _LISTNODESIGNATURESRESPONSE._serialized_start = 25704
-    _LISTNODESIGNATURESRESPONSE._serialized_end = 25807
-    _NODESIGNATUREEDGE._serialized_start = 25809
-    _NODESIGNATUREEDGE._serialized_end = 25905
-    _NODESIGNATURESCONNECTION._serialized_start = 25908
-    _NODESIGNATURESCONNECTION._serialized_end = 26048
-    _GETEPOCHREQUEST._serialized_start = 26050
-    _GETEPOCHREQUEST._serialized_end = 26095
-    _GETEPOCHRESPONSE._serialized_start = 26097
-    _GETEPOCHRESPONSE._serialized_end = 26150
-    _ESTIMATEFEEREQUEST._serialized_start = 26152
-    _ESTIMATEFEEREQUEST._serialized_end = 26243
-    _ESTIMATEFEERESPONSE._serialized_start = 26245
-    _ESTIMATEFEERESPONSE._serialized_end = 26295
-    _ESTIMATEMARGINREQUEST._serialized_start = 26298
-    _ESTIMATEMARGINREQUEST._serialized_end = 26489
-    _ESTIMATEMARGINRESPONSE._serialized_start = 26491
-    _ESTIMATEMARGINRESPONSE._serialized_end = 26572
-    _LISTNETWORKPARAMETERSREQUEST._serialized_start = 26574
-    _LISTNETWORKPARAMETERSREQUEST._serialized_end = 26685
-    _LISTNETWORKPARAMETERSRESPONSE._serialized_start = 26687
-    _LISTNETWORKPARAMETERSRESPONSE._serialized_end = 26810
-    _GETNETWORKPARAMETERREQUEST._serialized_start = 26812
-    _GETNETWORKPARAMETERREQUEST._serialized_end = 26858
-    _GETNETWORKPARAMETERRESPONSE._serialized_start = 26860
-    _GETNETWORKPARAMETERRESPONSE._serialized_end = 26958
-    _NETWORKPARAMETEREDGE._serialized_start = 26960
-    _NETWORKPARAMETEREDGE._serialized_end = 27050
-    _NETWORKPARAMETERCONNECTION._serialized_start = 27053
-    _NETWORKPARAMETERCONNECTION._serialized_end = 27198
-    _CHECKPOINT._serialized_start = 27200
-    _CHECKPOINT._serialized_end = 27290
-    _LISTCHECKPOINTSREQUEST._serialized_start = 27292
-    _LISTCHECKPOINTSREQUEST._serialized_end = 27397
-    _LISTCHECKPOINTSRESPONSE._serialized_start = 27399
-    _LISTCHECKPOINTSRESPONSE._serialized_end = 27498
-    _CHECKPOINTEDGE._serialized_start = 27500
-    _CHECKPOINTEDGE._serialized_end = 27589
-    _CHECKPOINTSCONNECTION._serialized_start = 27592
-    _CHECKPOINTSCONNECTION._serialized_end = 27726
-    _GETSTAKEREQUEST._serialized_start = 27728
-    _GETSTAKEREQUEST._serialized_end = 27853
-    _GETSTAKERESPONSE._serialized_start = 27856
-    _GETSTAKERESPONSE._serialized_end = 28004
-    _STAKELINKINGEDGE._serialized_start = 28006
-    _STAKELINKINGEDGE._serialized_end = 28098
-    _STAKESCONNECTION._serialized_start = 28101
-    _STAKESCONNECTION._serialized_end = 28232
-    _GETRISKFACTORSREQUEST._serialized_start = 28234
-    _GETRISKFACTORSREQUEST._serialized_end = 28286
-    _GETRISKFACTORSRESPONSE._serialized_start = 28288
-    _GETRISKFACTORSRESPONSE._serialized_end = 28363
-    _OBSERVEEVENTBUSREQUEST._serialized_start = 28366
-    _OBSERVEEVENTBUSREQUEST._serialized_end = 28527
-    _OBSERVEEVENTBUSRESPONSE._serialized_start = 28529
-    _OBSERVEEVENTBUSRESPONSE._serialized_end = 28604
-    _OBSERVELEDGERMOVEMENTSREQUEST._serialized_start = 28606
-    _OBSERVELEDGERMOVEMENTSREQUEST._serialized_end = 28637
-    _OBSERVELEDGERMOVEMENTSRESPONSE._serialized_start = 28639
-    _OBSERVELEDGERMOVEMENTSRESPONSE._serialized_end = 28734
-    _LISTKEYROTATIONSREQUEST._serialized_start = 28737
-    _LISTKEYROTATIONSREQUEST._serialized_end = 28885
-    _LISTKEYROTATIONSRESPONSE._serialized_start = 28887
-    _LISTKEYROTATIONSRESPONSE._serialized_end = 28983
-    _KEYROTATIONEDGE._serialized_start = 28985
-    _KEYROTATIONEDGE._serialized_end = 29075
-    _KEYROTATIONCONNECTION._serialized_start = 29078
-    _KEYROTATIONCONNECTION._serialized_end = 29213
-    _LISTETHEREUMKEYROTATIONSREQUEST._serialized_start = 29216
-    _LISTETHEREUMKEYROTATIONSREQUEST._serialized_end = 29372
-    _LISTETHEREUMKEYROTATIONSRESPONSE._serialized_start = 29374
-    _LISTETHEREUMKEYROTATIONSRESPONSE._serialized_end = 29494
-    _ETHEREUMKEYROTATIONSCONNECTION._serialized_start = 29497
-    _ETHEREUMKEYROTATIONSCONNECTION._serialized_end = 29649
-    _ETHEREUMKEYROTATIONEDGE._serialized_start = 29651
-    _ETHEREUMKEYROTATIONEDGE._serialized_end = 29757
-    _GETVEGATIMEREQUEST._serialized_start = 29759
-    _GETVEGATIMEREQUEST._serialized_end = 29779
-    _GETVEGATIMERESPONSE._serialized_start = 29781
-    _GETVEGATIMERESPONSE._serialized_end = 29832
-    _DATERANGE._serialized_start = 29835
-    _DATERANGE._serialized_end = 29972
-    _GETPROTOCOLUPGRADESTATUSREQUEST._serialized_start = 29974
-    _GETPROTOCOLUPGRADESTATUSREQUEST._serialized_end = 30007
-    _GETPROTOCOLUPGRADESTATUSRESPONSE._serialized_start = 30009
-    _GETPROTOCOLUPGRADESTATUSRESPONSE._serialized_end = 30065
-    _LISTPROTOCOLUPGRADEPROPOSALSREQUEST._serialized_start = 30068
-    _LISTPROTOCOLUPGRADEPROPOSALSREQUEST._serialized_end = 30327
-    _LISTPROTOCOLUPGRADEPROPOSALSRESPONSE._serialized_start = 30330
-    _LISTPROTOCOLUPGRADEPROPOSALSRESPONSE._serialized_end = 30482
-    _PROTOCOLUPGRADEPROPOSALCONNECTION._serialized_start = 30485
-    _PROTOCOLUPGRADEPROPOSALCONNECTION._serialized_end = 30644
-    _PROTOCOLUPGRADEPROPOSALEDGE._serialized_start = 30646
-    _PROTOCOLUPGRADEPROPOSALEDGE._serialized_end = 30757
-    _LISTCORESNAPSHOTSREQUEST._serialized_start = 30759
-    _LISTCORESNAPSHOTSREQUEST._serialized_end = 30866
-    _LISTCORESNAPSHOTSRESPONSE._serialized_start = 30868
-    _LISTCORESNAPSHOTSRESPONSE._serialized_end = 30975
-    _CORESNAPSHOTCONNECTION._serialized_start = 30978
-    _CORESNAPSHOTCONNECTION._serialized_end = 31115
-    _CORESNAPSHOTEDGE._serialized_start = 31117
-    _CORESNAPSHOTEDGE._serialized_end = 31213
-    _HISTORYSEGMENT._serialized_start = 31216
-    _HISTORYSEGMENT._serialized_end = 31430
-    _GETMOSTRECENTNETWORKHISTORYSEGMENTREQUEST._serialized_start = 31432
-    _GETMOSTRECENTNETWORKHISTORYSEGMENTREQUEST._serialized_end = 31475
-    _GETMOSTRECENTNETWORKHISTORYSEGMENTRESPONSE._serialized_start = 31478
-    _GETMOSTRECENTNETWORKHISTORYSEGMENTRESPONSE._serialized_end = 31610
-    _LISTALLNETWORKHISTORYSEGMENTSREQUEST._serialized_start = 31612
-    _LISTALLNETWORKHISTORYSEGMENTSREQUEST._serialized_end = 31650
-    _LISTALLNETWORKHISTORYSEGMENTSRESPONSE._serialized_start = 31652
-    _LISTALLNETWORKHISTORYSEGMENTSRESPONSE._serialized_end = 31752
-    _GETACTIVENETWORKHISTORYPEERADDRESSESREQUEST._serialized_start = 31754
-    _GETACTIVENETWORKHISTORYPEERADDRESSESREQUEST._serialized_end = 31799
-    _GETACTIVENETWORKHISTORYPEERADDRESSESRESPONSE._serialized_start = 31801
-    _GETACTIVENETWORKHISTORYPEERADDRESSESRESPONSE._serialized_end = 31882
-    _PINGREQUEST._serialized_start = 31884
-    _PINGREQUEST._serialized_end = 31897
-    _PINGRESPONSE._serialized_start = 31899
-    _PINGRESPONSE._serialized_end = 31913
-    _TRADINGDATASERVICE._serialized_start = 32444
-    _TRADINGDATASERVICE._serialized_end = 41490
+    _LISTPOSITIONSREQUEST._serialized_end = 3731
+    _LISTPOSITIONSRESPONSE._serialized_start = 3733
+    _LISTPOSITIONSRESPONSE._serialized_end = 3827
+    _POSITIONSFILTER._serialized_start = 3829
+    _POSITIONSFILTER._serialized_end = 3906
+    _LISTALLPOSITIONSREQUEST._serialized_start = 3909
+    _LISTALLPOSITIONSREQUEST._serialized_end = 4073
+    _LISTALLPOSITIONSRESPONSE._serialized_start = 4075
+    _LISTALLPOSITIONSRESPONSE._serialized_end = 4168
+    _POSITIONEDGE._serialized_start = 4170
+    _POSITIONEDGE._serialized_end = 4244
+    _POSITIONCONNECTION._serialized_start = 4247
+    _POSITIONCONNECTION._serialized_end = 4376
+    _OBSERVEPOSITIONSREQUEST._serialized_start = 4378
+    _OBSERVEPOSITIONSREQUEST._serialized_end = 4496
+    _OBSERVEPOSITIONSRESPONSE._serialized_start = 4499
+    _OBSERVEPOSITIONSRESPONSE._serialized_end = 4668
+    _POSITIONSNAPSHOTPAGE._serialized_start = 4670
+    _POSITIONSNAPSHOTPAGE._serialized_end = 4767
+    _POSITIONUPDATES._serialized_start = 4769
+    _POSITIONUPDATES._serialized_end = 4832
+    _LEDGERENTRYFILTER._serialized_start = 4835
+    _LEDGERENTRYFILTER._serialized_end = 5126
+    _AGGREGATEDLEDGERENTRY._serialized_start = 5129
+    _AGGREGATEDLEDGERENTRY._serialized_end = 5858
+    _LISTLEDGERENTRIESREQUEST._serialized_start = 5861
+    _LISTLEDGERENTRIESREQUEST._serialized_end = 6107
+    _EXPORTLEDGERENTRIESREQUEST._serialized_start = 6110
+    _EXPORTLEDGERENTRIESREQUEST._serialized_end = 6352
+    _LISTLEDGERENTRIESRESPONSE._serialized_start = 6354
+    _LISTLEDGERENTRIESRESPONSE._serialized_end = 6472
+    _EXPORTLEDGERENTRIESRESPONSE._serialized_start = 6474
+    _EXPORTLEDGERENTRIESRESPONSE._serialized_end = 6579
+    _AGGREGATEDLEDGERENTRIESEDGE._serialized_start = 6581
+    _AGGREGATEDLEDGERENTRIESEDGE._serialized_end = 6694
+    _AGGREGATEDLEDGERENTRIESCONNECTION._serialized_start = 6697
+    _AGGREGATEDLEDGERENTRIESCONNECTION._serialized_end = 6856
+    _LISTBALANCECHANGESREQUEST._serialized_start = 6859
+    _LISTBALANCECHANGESREQUEST._serialized_end = 7102
+    _LISTBALANCECHANGESRESPONSE._serialized_start = 7104
+    _LISTBALANCECHANGESRESPONSE._serialized_end = 7206
+    _GETBALANCEHISTORYREQUEST._serialized_start = 7209
+    _GETBALANCEHISTORYREQUEST._serialized_end = 7509
+    _GETBALANCEHISTORYRESPONSE._serialized_start = 7511
+    _GETBALANCEHISTORYRESPONSE._serialized_end = 7612
+    _AGGREGATEDBALANCEEDGE._serialized_start = 7614
+    _AGGREGATEDBALANCEEDGE._serialized_end = 7717
+    _AGGREGATEDBALANCECONNECTION._serialized_start = 7720
+    _AGGREGATEDBALANCECONNECTION._serialized_end = 7867
+    _ACCOUNTFILTER._serialized_start = 7870
+    _ACCOUNTFILTER._serialized_end = 8028
+    _AGGREGATEDBALANCE._serialized_start = 8031
+    _AGGREGATEDBALANCE._serialized_end = 8320
+    _OBSERVEMARKETSDEPTHREQUEST._serialized_start = 8322
+    _OBSERVEMARKETSDEPTHREQUEST._serialized_end = 8381
+    _OBSERVEMARKETSDEPTHRESPONSE._serialized_start = 8383
+    _OBSERVEMARKETSDEPTHRESPONSE._serialized_end = 8466
+    _OBSERVEMARKETSDEPTHUPDATESREQUEST._serialized_start = 8468
+    _OBSERVEMARKETSDEPTHUPDATESREQUEST._serialized_end = 8534
+    _OBSERVEMARKETSDEPTHUPDATESRESPONSE._serialized_start = 8536
+    _OBSERVEMARKETSDEPTHUPDATESRESPONSE._serialized_end = 8621
+    _OBSERVEMARKETSDATAREQUEST._serialized_start = 8623
+    _OBSERVEMARKETSDATAREQUEST._serialized_end = 8681
+    _OBSERVEMARKETSDATARESPONSE._serialized_start = 8683
+    _OBSERVEMARKETSDATARESPONSE._serialized_end = 8762
+    _GETLATESTMARKETDEPTHREQUEST._serialized_start = 8764
+    _GETLATESTMARKETDEPTHREQUEST._serialized_end = 8870
+    _GETLATESTMARKETDEPTHRESPONSE._serialized_start = 8873
+    _GETLATESTMARKETDEPTHRESPONSE._serialized_end = 9091
+    _LISTLATESTMARKETDATAREQUEST._serialized_start = 9093
+    _LISTLATESTMARKETDATAREQUEST._serialized_end = 9122
+    _LISTLATESTMARKETDATARESPONSE._serialized_start = 9124
+    _LISTLATESTMARKETDATARESPONSE._serialized_end = 9207
+    _GETLATESTMARKETDATAREQUEST._serialized_start = 9209
+    _GETLATESTMARKETDATAREQUEST._serialized_end = 9266
+    _GETLATESTMARKETDATARESPONSE._serialized_start = 9268
+    _GETLATESTMARKETDATARESPONSE._serialized_end = 9348
+    _GETMARKETDATAHISTORYBYIDREQUEST._serialized_start = 9351
+    _GETMARKETDATAHISTORYBYIDREQUEST._serialized_end = 9731
+    _GETMARKETDATAHISTORYBYIDRESPONSE._serialized_start = 9733
+    _GETMARKETDATAHISTORYBYIDRESPONSE._serialized_end = 9839
+    _MARKETDATAEDGE._serialized_start = 9841
+    _MARKETDATAEDGE._serialized_end = 9919
+    _MARKETDATACONNECTION._serialized_start = 9922
+    _MARKETDATACONNECTION._serialized_end = 10055
+    _MARKETSDATASUBSCRIBEREQUEST._serialized_start = 10057
+    _MARKETSDATASUBSCRIBEREQUEST._serialized_end = 10115
+    _MARKETSDATASUBSCRIBERESPONSE._serialized_start = 10117
+    _MARKETSDATASUBSCRIBERESPONSE._serialized_end = 10198
+    _LISTTRANSFERSREQUEST._serialized_start = 10201
+    _LISTTRANSFERSREQUEST._serialized_end = 10410
+    _LISTTRANSFERSRESPONSE._serialized_start = 10412
+    _LISTTRANSFERSRESPONSE._serialized_end = 10502
+    _TRANSFEREDGE._serialized_start = 10504
+    _TRANSFEREDGE._serialized_end = 10588
+    _TRANSFERCONNECTION._serialized_start = 10591
+    _TRANSFERCONNECTION._serialized_end = 10720
+    _GETNETWORKLIMITSREQUEST._serialized_start = 10722
+    _GETNETWORKLIMITSREQUEST._serialized_end = 10747
+    _GETNETWORKLIMITSRESPONSE._serialized_start = 10749
+    _GETNETWORKLIMITSRESPONSE._serialized_end = 10820
+    _LISTCANDLEINTERVALSREQUEST._serialized_start = 10822
+    _LISTCANDLEINTERVALSREQUEST._serialized_end = 10879
+    _INTERVALTOCANDLEID._serialized_start = 10881
+    _INTERVALTOCANDLEID._serialized_end = 10958
+    _LISTCANDLEINTERVALSRESPONSE._serialized_start = 10960
+    _LISTCANDLEINTERVALSRESPONSE._serialized_end = 11077
+    _CANDLE._serialized_start = 11080
+    _CANDLE._serialized_end = 11247
+    _OBSERVECANDLEDATAREQUEST._serialized_start = 11249
+    _OBSERVECANDLEDATAREQUEST._serialized_end = 11304
+    _OBSERVECANDLEDATARESPONSE._serialized_start = 11306
+    _OBSERVECANDLEDATARESPONSE._serialized_end = 11382
+    _LISTCANDLEDATAREQUEST._serialized_start = 11385
+    _LISTCANDLEDATAREQUEST._serialized_end = 11636
+    _LISTCANDLEDATARESPONSE._serialized_start = 11638
+    _LISTCANDLEDATARESPONSE._serialized_end = 11727
+    _CANDLEEDGE._serialized_start = 11729
+    _CANDLEEDGE._serialized_end = 11810
+    _CANDLEDATACONNECTION._serialized_start = 11813
+    _CANDLEDATACONNECTION._serialized_end = 11942
+    _LISTVOTESREQUEST._serialized_start = 11945
+    _LISTVOTESREQUEST._serialized_end = 12143
+    _LISTVOTESRESPONSE._serialized_start = 12145
+    _LISTVOTESRESPONSE._serialized_end = 12219
+    _VOTEEDGE._serialized_start = 12221
+    _VOTEEDGE._serialized_end = 12287
+    _VOTECONNECTION._serialized_start = 12289
+    _VOTECONNECTION._serialized_end = 12410
+    _OBSERVEVOTESREQUEST._serialized_start = 12412
+    _OBSERVEVOTESREQUEST._serialized_end = 12532
+    _OBSERVEVOTESRESPONSE._serialized_start = 12534
+    _OBSERVEVOTESRESPONSE._serialized_end = 12588
+    _LISTERC20MULTISIGSIGNERADDEDBUNDLESREQUEST._serialized_start = 12591
+    _LISTERC20MULTISIGSIGNERADDEDBUNDLESREQUEST._serialized_end = 12780
+    _LISTERC20MULTISIGSIGNERADDEDBUNDLESRESPONSE._serialized_start = 12782
+    _LISTERC20MULTISIGSIGNERADDEDBUNDLESRESPONSE._serialized_end = 12906
+    _ERC20MULTISIGSIGNERADDEDEDGE._serialized_start = 12908
+    _ERC20MULTISIGSIGNERADDEDEDGE._serialized_end = 13024
+    _ERC20MULTISIGSIGNERADDEDBUNDLEEDGE._serialized_start = 13027
+    _ERC20MULTISIGSIGNERADDEDBUNDLEEDGE._serialized_end = 13156
+    _ERC20MULTISIGSIGNERADDEDCONNECTION._serialized_start = 13159
+    _ERC20MULTISIGSIGNERADDEDCONNECTION._serialized_end = 13326
+    _ERC20MULTISIGSIGNERADDEDBUNDLE._serialized_start = 13329
+    _ERC20MULTISIGSIGNERADDEDBUNDLE._serialized_end = 13535
+    _LISTERC20MULTISIGSIGNERREMOVEDBUNDLESREQUEST._serialized_start = 13538
+    _LISTERC20MULTISIGSIGNERREMOVEDBUNDLESREQUEST._serialized_end = 13729
+    _LISTERC20MULTISIGSIGNERREMOVEDBUNDLESRESPONSE._serialized_start = 13732
+    _LISTERC20MULTISIGSIGNERREMOVEDBUNDLESRESPONSE._serialized_end = 13860
+    _ERC20MULTISIGSIGNERREMOVEDEDGE._serialized_start = 13862
+    _ERC20MULTISIGSIGNERREMOVEDEDGE._serialized_end = 13982
+    _ERC20MULTISIGSIGNERREMOVEDBUNDLEEDGE._serialized_start = 13985
+    _ERC20MULTISIGSIGNERREMOVEDBUNDLEEDGE._serialized_end = 14118
+    _ERC20MULTISIGSIGNERREMOVEDCONNECTION._serialized_start = 14121
+    _ERC20MULTISIGSIGNERREMOVEDCONNECTION._serialized_end = 14292
+    _ERC20MULTISIGSIGNERREMOVEDBUNDLE._serialized_start = 14295
+    _ERC20MULTISIGSIGNERREMOVEDBUNDLE._serialized_end = 14503
+    _GETERC20LISTASSETBUNDLEREQUEST._serialized_start = 14505
+    _GETERC20LISTASSETBUNDLEREQUEST._serialized_end = 14564
+    _GETERC20LISTASSETBUNDLERESPONSE._serialized_start = 14567
+    _GETERC20LISTASSETBUNDLERESPONSE._serialized_end = 14725
+    _GETERC20SETASSETLIMITSBUNDLEREQUEST._serialized_start = 14727
+    _GETERC20SETASSETLIMITSBUNDLEREQUEST._serialized_end = 14797
+    _GETERC20SETASSETLIMITSBUNDLERESPONSE._serialized_start = 14800
+    _GETERC20SETASSETLIMITSBUNDLERESPONSE._serialized_end = 15032
+    _GETERC20WITHDRAWALAPPROVALREQUEST._serialized_start = 15034
+    _GETERC20WITHDRAWALAPPROVALREQUEST._serialized_end = 15106
+    _GETERC20WITHDRAWALAPPROVALRESPONSE._serialized_start = 15109
+    _GETERC20WITHDRAWALAPPROVALRESPONSE._serialized_end = 15331
+    _GETLASTTRADEREQUEST._serialized_start = 15333
+    _GETLASTTRADEREQUEST._serialized_end = 15383
+    _GETLASTTRADERESPONSE._serialized_start = 15385
+    _GETLASTTRADERESPONSE._serialized_end = 15442
+    _LISTTRADESREQUEST._serialized_start = 15445
+    _LISTTRADESREQUEST._serialized_end = 15762
+    _LISTTRADESRESPONSE._serialized_start = 15764
+    _LISTTRADESRESPONSE._serialized_end = 15842
+    _TRADECONNECTION._serialized_start = 15844
+    _TRADECONNECTION._serialized_end = 15967
+    _TRADEEDGE._serialized_start = 15969
+    _TRADEEDGE._serialized_end = 16037
+    _OBSERVETRADESREQUEST._serialized_start = 16039
+    _OBSERVETRADESREQUEST._serialized_end = 16154
+    _OBSERVETRADESRESPONSE._serialized_start = 16156
+    _OBSERVETRADESRESPONSE._serialized_end = 16216
+    _GETORACLESPECREQUEST._serialized_start = 16218
+    _GETORACLESPECREQUEST._serialized_end = 16278
+    _GETORACLESPECRESPONSE._serialized_start = 16280
+    _GETORACLESPECRESPONSE._serialized_end = 16354
+    _LISTORACLESPECSREQUEST._serialized_start = 16356
+    _LISTORACLESPECSREQUEST._serialized_end = 16461
+    _LISTORACLESPECSRESPONSE._serialized_start = 16463
+    _LISTORACLESPECSRESPONSE._serialized_end = 16563
+    _LISTORACLEDATAREQUEST._serialized_start = 16566
+    _LISTORACLEDATAREQUEST._serialized_end = 16732
+    _LISTORACLEDATARESPONSE._serialized_start = 16734
+    _LISTORACLEDATARESPONSE._serialized_end = 16830
+    _ORACLESPECEDGE._serialized_start = 16832
+    _ORACLESPECEDGE._serialized_end = 16910
+    _ORACLESPECSCONNECTION._serialized_start = 16913
+    _ORACLESPECSCONNECTION._serialized_end = 17047
+    _ORACLEDATAEDGE._serialized_start = 17049
+    _ORACLEDATAEDGE._serialized_end = 17127
+    _ORACLEDATACONNECTION._serialized_start = 17130
+    _ORACLEDATACONNECTION._serialized_end = 17263
+    _GETMARKETREQUEST._serialized_start = 17265
+    _GETMARKETREQUEST._serialized_end = 17312
+    _GETMARKETRESPONSE._serialized_start = 17314
+    _GETMARKETRESPONSE._serialized_end = 17371
+    _LISTMARKETSREQUEST._serialized_start = 17374
+    _LISTMARKETSREQUEST._serialized_end = 17541
+    _LISTMARKETSRESPONSE._serialized_start = 17543
+    _LISTMARKETSRESPONSE._serialized_end = 17625
+    _MARKETEDGE._serialized_start = 17627
+    _MARKETEDGE._serialized_end = 17697
+    _MARKETCONNECTION._serialized_start = 17699
+    _MARKETCONNECTION._serialized_end = 17824
+    _GETPARTYREQUEST._serialized_start = 17826
+    _GETPARTYREQUEST._serialized_end = 17870
+    _GETPARTYRESPONSE._serialized_start = 17872
+    _GETPARTYRESPONSE._serialized_end = 17925
+    _LISTPARTIESREQUEST._serialized_start = 17927
+    _LISTPARTIESREQUEST._serialized_end = 18035
+    _LISTPARTIESRESPONSE._serialized_start = 18037
+    _LISTPARTIESRESPONSE._serialized_end = 18118
+    _PARTYEDGE._serialized_start = 18120
+    _PARTYEDGE._serialized_end = 18188
+    _PARTYCONNECTION._serialized_start = 18190
+    _PARTYCONNECTION._serialized_end = 18313
+    _ORDEREDGE._serialized_start = 18315
+    _ORDEREDGE._serialized_end = 18383
+    _LISTMARGINLEVELSREQUEST._serialized_start = 18386
+    _LISTMARGINLEVELSREQUEST._serialized_end = 18528
+    _LISTMARGINLEVELSRESPONSE._serialized_start = 18530
+    _LISTMARGINLEVELSRESPONSE._serialized_end = 18628
+    _OBSERVEMARGINLEVELSREQUEST._serialized_start = 18630
+    _OBSERVEMARGINLEVELSREQUEST._serialized_end = 18733
+    _OBSERVEMARGINLEVELSRESPONSE._serialized_start = 18735
+    _OBSERVEMARGINLEVELSRESPONSE._serialized_end = 18821
+    _ORDERCONNECTION._serialized_start = 18823
+    _ORDERCONNECTION._serialized_end = 18946
+    _MARGINEDGE._serialized_start = 18948
+    _MARGINEDGE._serialized_end = 19024
+    _MARGINCONNECTION._serialized_start = 19026
+    _MARGINCONNECTION._serialized_end = 19151
+    _LISTREWARDSREQUEST._serialized_start = 19154
+    _LISTREWARDSREQUEST._serialized_end = 19423
+    _LISTREWARDSRESPONSE._serialized_start = 19425
+    _LISTREWARDSRESPONSE._serialized_end = 19508
+    _REWARDEDGE._serialized_start = 19510
+    _REWARDEDGE._serialized_end = 19580
+    _REWARDSCONNECTION._serialized_start = 19582
+    _REWARDSCONNECTION._serialized_end = 19708
+    _LISTREWARDSUMMARIESREQUEST._serialized_start = 19711
+    _LISTREWARDSUMMARIESREQUEST._serialized_end = 19910
+    _LISTREWARDSUMMARIESRESPONSE._serialized_start = 19912
+    _LISTREWARDSUMMARIESRESPONSE._serialized_end = 19992
+    _REWARDSUMMARYFILTER._serialized_start = 19995
+    _REWARDSUMMARYFILTER._serialized_end = 20172
+    _LISTEPOCHREWARDSUMMARIESREQUEST._serialized_start = 20175
+    _LISTEPOCHREWARDSUMMARIESREQUEST._serialized_end = 20351
+    _LISTEPOCHREWARDSUMMARIESRESPONSE._serialized_start = 20353
+    _LISTEPOCHREWARDSUMMARIESRESPONSE._serialized_end = 20464
+    _EPOCHREWARDSUMMARYCONNECTION._serialized_start = 20467
+    _EPOCHREWARDSUMMARYCONNECTION._serialized_end = 20616
+    _EPOCHREWARDSUMMARYEDGE._serialized_start = 20618
+    _EPOCHREWARDSUMMARYEDGE._serialized_end = 20712
+    _OBSERVEREWARDSREQUEST._serialized_start = 20714
+    _OBSERVEREWARDSREQUEST._serialized_end = 20827
+    _OBSERVEREWARDSRESPONSE._serialized_start = 20829
+    _OBSERVEREWARDSRESPONSE._serialized_end = 20891
+    _GETDEPOSITREQUEST._serialized_start = 20893
+    _GETDEPOSITREQUEST._serialized_end = 20928
+    _GETDEPOSITRESPONSE._serialized_start = 20930
+    _GETDEPOSITRESPONSE._serialized_end = 20991
+    _LISTDEPOSITSREQUEST._serialized_start = 20994
+    _LISTDEPOSITSREQUEST._serialized_end = 21202
+    _LISTDEPOSITSRESPONSE._serialized_start = 21204
+    _LISTDEPOSITSRESPONSE._serialized_end = 21291
+    _DEPOSITEDGE._serialized_start = 21293
+    _DEPOSITEDGE._serialized_end = 21365
+    _DEPOSITSCONNECTION._serialized_start = 21368
+    _DEPOSITSCONNECTION._serialized_end = 21496
+    _GETWITHDRAWALREQUEST._serialized_start = 21498
+    _GETWITHDRAWALREQUEST._serialized_end = 21536
+    _GETWITHDRAWALRESPONSE._serialized_start = 21538
+    _GETWITHDRAWALRESPONSE._serialized_end = 21611
+    _LISTWITHDRAWALSREQUEST._serialized_start = 21614
+    _LISTWITHDRAWALSREQUEST._serialized_end = 21825
+    _LISTWITHDRAWALSRESPONSE._serialized_start = 21827
+    _LISTWITHDRAWALSRESPONSE._serialized_end = 21926
+    _WITHDRAWALEDGE._serialized_start = 21928
+    _WITHDRAWALEDGE._serialized_end = 22006
+    _WITHDRAWALSCONNECTION._serialized_start = 22009
+    _WITHDRAWALSCONNECTION._serialized_end = 22143
+    _GETASSETREQUEST._serialized_start = 22145
+    _GETASSETREQUEST._serialized_end = 22189
+    _GETASSETRESPONSE._serialized_start = 22191
+    _GETASSETRESPONSE._serialized_end = 22244
+    _LISTASSETSREQUEST._serialized_start = 22247
+    _LISTASSETSREQUEST._serialized_end = 22392
+    _LISTASSETSRESPONSE._serialized_start = 22394
+    _LISTASSETSRESPONSE._serialized_end = 22473
+    _ASSETEDGE._serialized_start = 22475
+    _ASSETEDGE._serialized_end = 22543
+    _ASSETSCONNECTION._serialized_start = 22545
+    _ASSETSCONNECTION._serialized_end = 22669
+    _LISTLIQUIDITYPROVISIONSREQUEST._serialized_start = 22672
+    _LISTLIQUIDITYPROVISIONSREQUEST._serialized_end = 22927
+    _LISTLIQUIDITYPROVISIONSRESPONSE._serialized_start = 22930
+    _LISTLIQUIDITYPROVISIONSRESPONSE._serialized_end = 23062
+    _LIQUIDITYPROVISIONSEDGE._serialized_start = 23064
+    _LIQUIDITYPROVISIONSEDGE._serialized_end = 23159
+    _LIQUIDITYPROVISIONSCONNECTION._serialized_start = 23162
+    _LIQUIDITYPROVISIONSCONNECTION._serialized_end = 23313
+    _OBSERVELIQUIDITYPROVISIONSREQUEST._serialized_start = 23316
+    _OBSERVELIQUIDITYPROVISIONSREQUEST._serialized_end = 23444
+    _OBSERVELIQUIDITYPROVISIONSRESPONSE._serialized_start = 23446
+    _OBSERVELIQUIDITYPROVISIONSRESPONSE._serialized_end = 23559
+    _GETGOVERNANCEDATAREQUEST._serialized_start = 23562
+    _GETGOVERNANCEDATAREQUEST._serialized_end = 23691
+    _GETGOVERNANCEDATARESPONSE._serialized_start = 23693
+    _GETGOVERNANCEDATARESPONSE._serialized_end = 23762
+    _LISTGOVERNANCEDATAREQUEST._serialized_start = 23765
+    _LISTGOVERNANCEDATAREQUEST._serialized_end = 24399
+    _LISTGOVERNANCEDATAREQUEST_TYPE._serialized_start = 24119
+    _LISTGOVERNANCEDATAREQUEST_TYPE._serialized_end = 24302
+    _LISTGOVERNANCEDATARESPONSE._serialized_start = 24401
+    _LISTGOVERNANCEDATARESPONSE._serialized_end = 24504
+    _GOVERNANCEDATAEDGE._serialized_start = 24506
+    _GOVERNANCEDATAEDGE._serialized_end = 24592
+    _GOVERNANCEDATACONNECTION._serialized_start = 24595
+    _GOVERNANCEDATACONNECTION._serialized_end = 24736
+    _OBSERVEGOVERNANCEREQUEST._serialized_start = 24738
+    _OBSERVEGOVERNANCEREQUEST._serialized_end = 24809
+    _OBSERVEGOVERNANCERESPONSE._serialized_start = 24811
+    _OBSERVEGOVERNANCERESPONSE._serialized_end = 24880
+    _LISTDELEGATIONSREQUEST._serialized_start = 24883
+    _LISTDELEGATIONSREQUEST._serialized_end = 25120
+    _LISTDELEGATIONSRESPONSE._serialized_start = 25122
+    _LISTDELEGATIONSRESPONSE._serialized_end = 25221
+    _DELEGATIONEDGE._serialized_start = 25223
+    _DELEGATIONEDGE._serialized_end = 25301
+    _DELEGATIONSCONNECTION._serialized_start = 25304
+    _DELEGATIONSCONNECTION._serialized_end = 25438
+    _OBSERVEDELEGATIONSREQUEST._serialized_start = 25440
+    _OBSERVEDELEGATIONSREQUEST._serialized_end = 25554
+    _OBSERVEDELEGATIONSRESPONSE._serialized_start = 25556
+    _OBSERVEDELEGATIONSRESPONSE._serialized_end = 25634
+    _GETNETWORKDATAREQUEST._serialized_start = 25636
+    _GETNETWORKDATAREQUEST._serialized_end = 25659
+    _GETNETWORKDATARESPONSE._serialized_start = 25661
+    _GETNETWORKDATARESPONSE._serialized_end = 25730
+    _GETNODEREQUEST._serialized_start = 25732
+    _GETNODEREQUEST._serialized_end = 25764
+    _GETNODERESPONSE._serialized_start = 25766
+    _GETNODERESPONSE._serialized_end = 25815
+    _LISTNODESREQUEST._serialized_start = 25818
+    _LISTNODESREQUEST._serialized_end = 25965
+    _LISTNODESRESPONSE._serialized_start = 25967
+    _LISTNODESRESPONSE._serialized_end = 26042
+    _NODEEDGE._serialized_start = 26044
+    _NODEEDGE._serialized_end = 26110
+    _NODESCONNECTION._serialized_start = 26112
+    _NODESCONNECTION._serialized_end = 26234
+    _LISTNODESIGNATURESREQUEST._serialized_start = 26236
+    _LISTNODESIGNATURESREQUEST._serialized_end = 26360
+    _LISTNODESIGNATURESRESPONSE._serialized_start = 26362
+    _LISTNODESIGNATURESRESPONSE._serialized_end = 26465
+    _NODESIGNATUREEDGE._serialized_start = 26467
+    _NODESIGNATUREEDGE._serialized_end = 26563
+    _NODESIGNATURESCONNECTION._serialized_start = 26566
+    _NODESIGNATURESCONNECTION._serialized_end = 26706
+    _GETEPOCHREQUEST._serialized_start = 26708
+    _GETEPOCHREQUEST._serialized_end = 26753
+    _GETEPOCHRESPONSE._serialized_start = 26755
+    _GETEPOCHRESPONSE._serialized_end = 26808
+    _ESTIMATEFEEREQUEST._serialized_start = 26810
+    _ESTIMATEFEEREQUEST._serialized_end = 26901
+    _ESTIMATEFEERESPONSE._serialized_start = 26903
+    _ESTIMATEFEERESPONSE._serialized_end = 26953
+    _ESTIMATEMARGINREQUEST._serialized_start = 26956
+    _ESTIMATEMARGINREQUEST._serialized_end = 27147
+    _ESTIMATEMARGINRESPONSE._serialized_start = 27149
+    _ESTIMATEMARGINRESPONSE._serialized_end = 27230
+    _LISTNETWORKPARAMETERSREQUEST._serialized_start = 27232
+    _LISTNETWORKPARAMETERSREQUEST._serialized_end = 27343
+    _LISTNETWORKPARAMETERSRESPONSE._serialized_start = 27345
+    _LISTNETWORKPARAMETERSRESPONSE._serialized_end = 27468
+    _GETNETWORKPARAMETERREQUEST._serialized_start = 27470
+    _GETNETWORKPARAMETERREQUEST._serialized_end = 27516
+    _GETNETWORKPARAMETERRESPONSE._serialized_start = 27518
+    _GETNETWORKPARAMETERRESPONSE._serialized_end = 27616
+    _NETWORKPARAMETEREDGE._serialized_start = 27618
+    _NETWORKPARAMETEREDGE._serialized_end = 27708
+    _NETWORKPARAMETERCONNECTION._serialized_start = 27711
+    _NETWORKPARAMETERCONNECTION._serialized_end = 27856
+    _CHECKPOINT._serialized_start = 27858
+    _CHECKPOINT._serialized_end = 27948
+    _LISTCHECKPOINTSREQUEST._serialized_start = 27950
+    _LISTCHECKPOINTSREQUEST._serialized_end = 28055
+    _LISTCHECKPOINTSRESPONSE._serialized_start = 28057
+    _LISTCHECKPOINTSRESPONSE._serialized_end = 28156
+    _CHECKPOINTEDGE._serialized_start = 28158
+    _CHECKPOINTEDGE._serialized_end = 28247
+    _CHECKPOINTSCONNECTION._serialized_start = 28250
+    _CHECKPOINTSCONNECTION._serialized_end = 28384
+    _GETSTAKEREQUEST._serialized_start = 28386
+    _GETSTAKEREQUEST._serialized_end = 28511
+    _GETSTAKERESPONSE._serialized_start = 28514
+    _GETSTAKERESPONSE._serialized_end = 28662
+    _STAKELINKINGEDGE._serialized_start = 28664
+    _STAKELINKINGEDGE._serialized_end = 28756
+    _STAKESCONNECTION._serialized_start = 28759
+    _STAKESCONNECTION._serialized_end = 28890
+    _GETRISKFACTORSREQUEST._serialized_start = 28892
+    _GETRISKFACTORSREQUEST._serialized_end = 28944
+    _GETRISKFACTORSRESPONSE._serialized_start = 28946
+    _GETRISKFACTORSRESPONSE._serialized_end = 29021
+    _OBSERVEEVENTBUSREQUEST._serialized_start = 29024
+    _OBSERVEEVENTBUSREQUEST._serialized_end = 29185
+    _OBSERVEEVENTBUSRESPONSE._serialized_start = 29187
+    _OBSERVEEVENTBUSRESPONSE._serialized_end = 29262
+    _OBSERVELEDGERMOVEMENTSREQUEST._serialized_start = 29264
+    _OBSERVELEDGERMOVEMENTSREQUEST._serialized_end = 29295
+    _OBSERVELEDGERMOVEMENTSRESPONSE._serialized_start = 29297
+    _OBSERVELEDGERMOVEMENTSRESPONSE._serialized_end = 29392
+    _LISTKEYROTATIONSREQUEST._serialized_start = 29395
+    _LISTKEYROTATIONSREQUEST._serialized_end = 29543
+    _LISTKEYROTATIONSRESPONSE._serialized_start = 29545
+    _LISTKEYROTATIONSRESPONSE._serialized_end = 29641
+    _KEYROTATIONEDGE._serialized_start = 29643
+    _KEYROTATIONEDGE._serialized_end = 29733
+    _KEYROTATIONCONNECTION._serialized_start = 29736
+    _KEYROTATIONCONNECTION._serialized_end = 29871
+    _LISTETHEREUMKEYROTATIONSREQUEST._serialized_start = 29874
+    _LISTETHEREUMKEYROTATIONSREQUEST._serialized_end = 30030
+    _LISTETHEREUMKEYROTATIONSRESPONSE._serialized_start = 30032
+    _LISTETHEREUMKEYROTATIONSRESPONSE._serialized_end = 30152
+    _ETHEREUMKEYROTATIONSCONNECTION._serialized_start = 30155
+    _ETHEREUMKEYROTATIONSCONNECTION._serialized_end = 30307
+    _ETHEREUMKEYROTATIONEDGE._serialized_start = 30309
+    _ETHEREUMKEYROTATIONEDGE._serialized_end = 30415
+    _GETVEGATIMEREQUEST._serialized_start = 30417
+    _GETVEGATIMEREQUEST._serialized_end = 30437
+    _GETVEGATIMERESPONSE._serialized_start = 30439
+    _GETVEGATIMERESPONSE._serialized_end = 30490
+    _DATERANGE._serialized_start = 30493
+    _DATERANGE._serialized_end = 30630
+    _GETPROTOCOLUPGRADESTATUSREQUEST._serialized_start = 30632
+    _GETPROTOCOLUPGRADESTATUSREQUEST._serialized_end = 30665
+    _GETPROTOCOLUPGRADESTATUSRESPONSE._serialized_start = 30667
+    _GETPROTOCOLUPGRADESTATUSRESPONSE._serialized_end = 30723
+    _LISTPROTOCOLUPGRADEPROPOSALSREQUEST._serialized_start = 30726
+    _LISTPROTOCOLUPGRADEPROPOSALSREQUEST._serialized_end = 30985
+    _LISTPROTOCOLUPGRADEPROPOSALSRESPONSE._serialized_start = 30988
+    _LISTPROTOCOLUPGRADEPROPOSALSRESPONSE._serialized_end = 31140
+    _PROTOCOLUPGRADEPROPOSALCONNECTION._serialized_start = 31143
+    _PROTOCOLUPGRADEPROPOSALCONNECTION._serialized_end = 31302
+    _PROTOCOLUPGRADEPROPOSALEDGE._serialized_start = 31304
+    _PROTOCOLUPGRADEPROPOSALEDGE._serialized_end = 31415
+    _LISTCORESNAPSHOTSREQUEST._serialized_start = 31417
+    _LISTCORESNAPSHOTSREQUEST._serialized_end = 31524
+    _LISTCORESNAPSHOTSRESPONSE._serialized_start = 31526
+    _LISTCORESNAPSHOTSRESPONSE._serialized_end = 31633
+    _CORESNAPSHOTCONNECTION._serialized_start = 31636
+    _CORESNAPSHOTCONNECTION._serialized_end = 31773
+    _CORESNAPSHOTEDGE._serialized_start = 31775
+    _CORESNAPSHOTEDGE._serialized_end = 31871
+    _HISTORYSEGMENT._serialized_start = 31874
+    _HISTORYSEGMENT._serialized_end = 32061
+    _GETMOSTRECENTNETWORKHISTORYSEGMENTREQUEST._serialized_start = 32063
+    _GETMOSTRECENTNETWORKHISTORYSEGMENTREQUEST._serialized_end = 32106
+    _GETMOSTRECENTNETWORKHISTORYSEGMENTRESPONSE._serialized_start = 32109
+    _GETMOSTRECENTNETWORKHISTORYSEGMENTRESPONSE._serialized_end = 32250
+    _LISTALLNETWORKHISTORYSEGMENTSREQUEST._serialized_start = 32252
+    _LISTALLNETWORKHISTORYSEGMENTSREQUEST._serialized_end = 32290
+    _LISTALLNETWORKHISTORYSEGMENTSRESPONSE._serialized_start = 32292
+    _LISTALLNETWORKHISTORYSEGMENTSRESPONSE._serialized_end = 32392
+    _GETACTIVENETWORKHISTORYPEERADDRESSESREQUEST._serialized_start = 32394
+    _GETACTIVENETWORKHISTORYPEERADDRESSESREQUEST._serialized_end = 32439
+    _GETACTIVENETWORKHISTORYPEERADDRESSESRESPONSE._serialized_start = 32441
+    _GETACTIVENETWORKHISTORYPEERADDRESSESRESPONSE._serialized_end = 32522
+    _NETWORKHISTORYSTATUSREQUEST._serialized_start = 32524
+    _NETWORKHISTORYSTATUSREQUEST._serialized_end = 32553
+    _NETWORKHISTORYSTATUSRESPONSE._serialized_start = 32556
+    _NETWORKHISTORYSTATUSRESPONSE._serialized_end = 32729
+    _NETWORKHISTORYBOOTSTRAPPEERSREQUEST._serialized_start = 32731
+    _NETWORKHISTORYBOOTSTRAPPEERSREQUEST._serialized_end = 32768
+    _NETWORKHISTORYBOOTSTRAPPEERSRESPONSE._serialized_start = 32770
+    _NETWORKHISTORYBOOTSTRAPPEERSRESPONSE._serialized_end = 32849
+    _PINGREQUEST._serialized_start = 32851
+    _PINGREQUEST._serialized_end = 32864
+    _PINGRESPONSE._serialized_start = 32866
+    _PINGRESPONSE._serialized_end = 32880
+    _TRADINGDATASERVICE._serialized_start = 33411
+    _TRADINGDATASERVICE._serialized_end = 42826
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-0.67.0/vega_sim/proto/data_node/api/v2/trading_data_pb2_grpc.py` & `vega_sim-1.0.1/vega_sim/proto/data_node/api/v2/trading_data_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,19 @@
             response_deserializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ObserveOrdersResponse.FromString,
         )
         self.ListPositions = channel.unary_unary(
             "/datanode.api.v2.TradingDataService/ListPositions",
             request_serializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ListPositionsRequest.SerializeToString,
             response_deserializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ListPositionsResponse.FromString,
         )
+        self.ListAllPositions = channel.unary_unary(
+            "/datanode.api.v2.TradingDataService/ListAllPositions",
+            request_serializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ListAllPositionsRequest.SerializeToString,
+            response_deserializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ListAllPositionsResponse.FromString,
+        )
         self.ObservePositions = channel.unary_stream(
             "/datanode.api.v2.TradingDataService/ObservePositions",
             request_serializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ObservePositionsRequest.SerializeToString,
             response_deserializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ObservePositionsResponse.FromString,
         )
         self.ListLedgerEntries = channel.unary_unary(
             "/datanode.api.v2.TradingDataService/ListLedgerEntries",
@@ -427,14 +432,24 @@
             response_deserializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ListAllNetworkHistorySegmentsResponse.FromString,
         )
         self.GetActiveNetworkHistoryPeerAddresses = channel.unary_unary(
             "/datanode.api.v2.TradingDataService/GetActiveNetworkHistoryPeerAddresses",
             request_serializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.GetActiveNetworkHistoryPeerAddressesRequest.SerializeToString,
             response_deserializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.GetActiveNetworkHistoryPeerAddressesResponse.FromString,
         )
+        self.NetworkHistoryStatus = channel.unary_unary(
+            "/datanode.api.v2.TradingDataService/NetworkHistoryStatus",
+            request_serializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.NetworkHistoryStatusRequest.SerializeToString,
+            response_deserializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.NetworkHistoryStatusResponse.FromString,
+        )
+        self.NetworkHistoryBootstrapPeers = channel.unary_unary(
+            "/datanode.api.v2.TradingDataService/NetworkHistoryBootstrapPeers",
+            request_serializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.NetworkHistoryBootstrapPeersRequest.SerializeToString,
+            response_deserializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.NetworkHistoryBootstrapPeersResponse.FromString,
+        )
         self.Ping = channel.unary_unary(
             "/datanode.api.v2.TradingDataService/Ping",
             request_serializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.PingRequest.SerializeToString,
             response_deserializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.PingResponse.FromString,
         )
 
 
@@ -503,14 +518,24 @@
         Subscribe to a stream of orders
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ListPositions(self, request, context):
+        """Positions (deprecated)
+
+        Get a list of positions by party (public key) using cursor based pagination
+        Deprecated: use ListAllPositions instead
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details("Method not implemented!")
+        raise NotImplementedError("Method not implemented!")
+
+    def ListAllPositions(self, request, context):
         """Positions
 
         Get a list of positions by party (public key) using cursor based pagination
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
@@ -524,16 +549,16 @@
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ListLedgerEntries(self, request, context):
         """Ledger entries
 
         Get ledger entries by asset, market, party, account type, transfer type within the given date range.
-        This query requests and sums number of the ledger entries of a given subset of accounts, specified via the 'filter' argument.
-        It returns a timeseries (implemented as a list of AggregateLedgerEntry structs), with a row for every time
+        This query requests and sums the number of ledger entries from a given subset of accounts, specified via the 'filter' argument.
+        It returns a time series (implemented as a list of AggregateLedgerEntry structs), with a row for every time
         the summed ledger entries of the set of specified accounts changes.
         Listed queries should be limited to a single party from each side only. If no or more than one parties are provided
         for sending and receiving accounts - the query returns error.
 
         Entries can be queried by:
         - listing ledger entries with filtering on the sending account (market_id, asset_id, account_type)
         - listing ledger entries with filtering on the receiving account (market_id, asset_id, account_type)
@@ -936,15 +961,15 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ListAssets(self, request, context):
         """Assets list
 
-        Get a list of assets using cusor based pagination
+        Get a list of assets using cursor based pagination
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ListLiquidityProvisions(self, request, context):
         """Liquidity Provisions list
@@ -1219,14 +1244,34 @@
 
         List the addresses of all active network history peers
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
+    def NetworkHistoryStatus(self, request, context):
+        """Network history status
+
+        Retrieves information about the current state of network history
+        Response contains the network history status
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details("Method not implemented!")
+        raise NotImplementedError("Method not implemented!")
+
+    def NetworkHistoryBootstrapPeers(self, request, context):
+        """Network history bootstrap peers
+
+        Retrieves the nodes bootstrap peers
+        Response contains the bootstrap peers
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details("Method not implemented!")
+        raise NotImplementedError("Method not implemented!")
+
     def Ping(self, request, context):
         """Ping
 
         Ping the data node
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
@@ -1271,14 +1316,19 @@
             response_serializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ObserveOrdersResponse.SerializeToString,
         ),
         "ListPositions": grpc.unary_unary_rpc_method_handler(
             servicer.ListPositions,
             request_deserializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ListPositionsRequest.FromString,
             response_serializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ListPositionsResponse.SerializeToString,
         ),
+        "ListAllPositions": grpc.unary_unary_rpc_method_handler(
+            servicer.ListAllPositions,
+            request_deserializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ListAllPositionsRequest.FromString,
+            response_serializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ListAllPositionsResponse.SerializeToString,
+        ),
         "ObservePositions": grpc.unary_stream_rpc_method_handler(
             servicer.ObservePositions,
             request_deserializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ObservePositionsRequest.FromString,
             response_serializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ObservePositionsResponse.SerializeToString,
         ),
         "ListLedgerEntries": grpc.unary_unary_rpc_method_handler(
             servicer.ListLedgerEntries,
@@ -1646,14 +1696,24 @@
             response_serializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ListAllNetworkHistorySegmentsResponse.SerializeToString,
         ),
         "GetActiveNetworkHistoryPeerAddresses": grpc.unary_unary_rpc_method_handler(
             servicer.GetActiveNetworkHistoryPeerAddresses,
             request_deserializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.GetActiveNetworkHistoryPeerAddressesRequest.FromString,
             response_serializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.GetActiveNetworkHistoryPeerAddressesResponse.SerializeToString,
         ),
+        "NetworkHistoryStatus": grpc.unary_unary_rpc_method_handler(
+            servicer.NetworkHistoryStatus,
+            request_deserializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.NetworkHistoryStatusRequest.FromString,
+            response_serializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.NetworkHistoryStatusResponse.SerializeToString,
+        ),
+        "NetworkHistoryBootstrapPeers": grpc.unary_unary_rpc_method_handler(
+            servicer.NetworkHistoryBootstrapPeers,
+            request_deserializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.NetworkHistoryBootstrapPeersRequest.FromString,
+            response_serializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.NetworkHistoryBootstrapPeersResponse.SerializeToString,
+        ),
         "Ping": grpc.unary_unary_rpc_method_handler(
             servicer.Ping,
             request_deserializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.PingRequest.FromString,
             response_serializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.PingResponse.SerializeToString,
         ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
@@ -1895,14 +1955,43 @@
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
+    def ListAllPositions(
+        request,
+        target,
+        options=(),
+        channel_credentials=None,
+        call_credentials=None,
+        insecure=False,
+        compression=None,
+        wait_for_ready=None,
+        timeout=None,
+        metadata=None,
+    ):
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            "/datanode.api.v2.TradingDataService/ListAllPositions",
+            data__node_dot_api_dot_v2_dot_trading__data__pb2.ListAllPositionsRequest.SerializeToString,
+            data__node_dot_api_dot_v2_dot_trading__data__pb2.ListAllPositionsResponse.FromString,
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+        )
+
+    @staticmethod
     def ObservePositions(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
@@ -4066,14 +4155,72 @@
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
+            metadata,
+        )
+
+    @staticmethod
+    def NetworkHistoryStatus(
+        request,
+        target,
+        options=(),
+        channel_credentials=None,
+        call_credentials=None,
+        insecure=False,
+        compression=None,
+        wait_for_ready=None,
+        timeout=None,
+        metadata=None,
+    ):
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            "/datanode.api.v2.TradingDataService/NetworkHistoryStatus",
+            data__node_dot_api_dot_v2_dot_trading__data__pb2.NetworkHistoryStatusRequest.SerializeToString,
+            data__node_dot_api_dot_v2_dot_trading__data__pb2.NetworkHistoryStatusResponse.FromString,
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+        )
+
+    @staticmethod
+    def NetworkHistoryBootstrapPeers(
+        request,
+        target,
+        options=(),
+        channel_credentials=None,
+        call_credentials=None,
+        insecure=False,
+        compression=None,
+        wait_for_ready=None,
+        timeout=None,
+        metadata=None,
+    ):
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            "/datanode.api.v2.TradingDataService/NetworkHistoryBootstrapPeers",
+            data__node_dot_api_dot_v2_dot_trading__data__pb2.NetworkHistoryBootstrapPeersRequest.SerializeToString,
+            data__node_dot_api_dot_v2_dot_trading__data__pb2.NetworkHistoryBootstrapPeersResponse.FromString,
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
             metadata,
         )
 
     @staticmethod
     def Ping(
         request,
         target,
```

### Comparing `vega_sim-0.67.0/vega_sim/proto/vega/__init__.py` & `vega_sim-1.0.1/vega_sim/proto/vega/__init__.py`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/proto/vega/api/v1/core_pb2.py` & `vega_sim-1.0.1/vega_sim/proto/vega/api/v1/core_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,23 +19,22 @@
 )
 from protoc_gen_openapiv2.options import (
     annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2,
 )
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x16vega/api/v1/core.proto\x12\x0bvega.api.v1\x1a\x0fvega/vega.proto\x1a\x1bvega/events/v1/events.proto\x1a"vega/commands/v1/transaction.proto\x1a.protoc-gen-openapiv2/options/annotations.proto"i\n\x1aPropagateChainEventRequest\x12\x14\n\x05\x65vent\x18\x01 \x01(\x0cR\x05\x65vent\x12\x17\n\x07pub_key\x18\x02 \x01(\tR\x06pubKey\x12\x1c\n\tsignature\x18\x03 \x01(\x0cR\tsignature"7\n\x1bPropagateChainEventResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success"\xd7\x01\n\x18SubmitTransactionRequest\x12-\n\x02tx\x18\x01 \x01(\x0b\x32\x1d.vega.commands.v1.TransactionR\x02tx\x12>\n\x04type\x18\x02 \x01(\x0e\x32*.vega.api.v1.SubmitTransactionRequest.TypeR\x04type"L\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0e\n\nTYPE_ASYNC\x10\x01\x12\r\n\tTYPE_SYNC\x10\x02\x12\x0f\n\x0bTYPE_COMMIT\x10\x03"\xa0\x01\n\x19SubmitTransactionResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12\x17\n\x07tx_hash\x18\x02 \x01(\tR\x06txHash\x12\x12\n\x04\x63ode\x18\x03 \x01(\rR\x04\x63ode\x12\x12\n\x04\x64\x61ta\x18\x04 \x01(\tR\x04\x64\x61ta\x12\x10\n\x03log\x18\x05 \x01(\tR\x03log\x12\x16\n\x06height\x18\x06 \x01(\x03R\x06height"H\n\x17\x43heckTransactionRequest\x12-\n\x02tx\x18\x01 \x01(\x0b\x32\x1d.vega.commands.v1.TransactionR\x02tx"\xbc\x01\n\x18\x43heckTransactionResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12\x12\n\x04\x63ode\x18\x02 \x01(\rR\x04\x63ode\x12\x1d\n\ngas_wanted\x18\x03 \x01(\x03R\tgasWanted\x12\x19\n\x08gas_used\x18\x04 \x01(\x03R\x07gasUsed\x12\x12\n\x04\x64\x61ta\x18\x05 \x01(\tR\x04\x64\x61ta\x12\x10\n\x03log\x18\x06 \x01(\tR\x03log\x12\x12\n\x04info\x18\x07 \x01(\tR\x04info"\xbe\x01\n\x1bSubmitRawTransactionRequest\x12\x0e\n\x02tx\x18\x01 \x01(\x0cR\x02tx\x12\x41\n\x04type\x18\x02 \x01(\x0e\x32-.vega.api.v1.SubmitRawTransactionRequest.TypeR\x04type"L\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0e\n\nTYPE_ASYNC\x10\x01\x12\r\n\tTYPE_SYNC\x10\x02\x12\x0f\n\x0bTYPE_COMMIT\x10\x03"\xa3\x01\n\x1cSubmitRawTransactionResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12\x17\n\x07tx_hash\x18\x02 \x01(\tR\x06txHash\x12\x12\n\x04\x63ode\x18\x03 \x01(\rR\x04\x63ode\x12\x12\n\x04\x64\x61ta\x18\x04 \x01(\tR\x04\x64\x61ta\x12\x10\n\x03log\x18\x05 \x01(\tR\x03log\x12\x16\n\x06height\x18\x06 \x01(\x03R\x06height",\n\x1a\x43heckRawTransactionRequest\x12\x0e\n\x02tx\x18\x01 \x01(\x0cR\x02tx"\xbf\x01\n\x1b\x43heckRawTransactionResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12\x12\n\x04\x63ode\x18\x02 \x01(\rR\x04\x63ode\x12\x1d\n\ngas_wanted\x18\x03 \x01(\x03R\tgasWanted\x12\x19\n\x08gas_used\x18\x04 \x01(\x03R\x07gasUsed\x12\x12\n\x04\x64\x61ta\x18\x05 \x01(\tR\x04\x64\x61ta\x12\x10\n\x03log\x18\x06 \x01(\tR\x03log\x12\x12\n\x04info\x18\x07 \x01(\tR\x04info"\x14\n\x12GetVegaTimeRequest"3\n\x13GetVegaTimeResponse\x12\x1c\n\ttimestamp\x18\x01 \x01(\x03R\ttimestamp"\xa1\x01\n\x16ObserveEventBusRequest\x12\x30\n\x04type\x18\x01 \x03(\x0e\x32\x1c.vega.events.v1.BusEventTypeR\x04type\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x03 \x01(\tR\x07partyId\x12\x1d\n\nbatch_size\x18\x04 \x01(\x03R\tbatchSize"K\n\x17ObserveEventBusResponse\x12\x30\n\x06\x65vents\x18\x01 \x03(\x0b\x32\x18.vega.events.v1.BusEventR\x06\x65vents"\x13\n\x11StatisticsRequest"M\n\x12StatisticsResponse\x12\x37\n\nstatistics\x18\x01 \x01(\x0b\x32\x17.vega.api.v1.StatisticsR\nstatistics"\xfb\x0b\n\nStatistics\x12!\n\x0c\x62lock_height\x18\x01 \x01(\x04R\x0b\x62lockHeight\x12%\n\x0e\x62\x61\x63klog_length\x18\x02 \x01(\x04R\rbacklogLength\x12\x1f\n\x0btotal_peers\x18\x03 \x01(\x04R\ntotalPeers\x12!\n\x0cgenesis_time\x18\x04 \x01(\tR\x0bgenesisTime\x12!\n\x0c\x63urrent_time\x18\x05 \x01(\tR\x0b\x63urrentTime\x12\x1b\n\tvega_time\x18\x06 \x01(\tR\x08vegaTime\x12)\n\x06status\x18\x07 \x01(\x0e\x32\x11.vega.ChainStatusR\x06status\x12 \n\x0ctx_per_block\x18\x08 \x01(\x04R\ntxPerBlock\x12(\n\x10\x61verage_tx_bytes\x18\t \x01(\x04R\x0e\x61verageTxBytes\x12\x37\n\x18\x61verage_orders_per_block\x18\n \x01(\x04R\x15\x61verageOrdersPerBlock\x12*\n\x11trades_per_second\x18\x0b \x01(\x04R\x0ftradesPerSecond\x12*\n\x11orders_per_second\x18\x0c \x01(\x04R\x0fordersPerSecond\x12#\n\rtotal_markets\x18\r \x01(\x04R\x0ctotalMarkets\x12*\n\x11total_amend_order\x18\x10 \x01(\x04R\x0ftotalAmendOrder\x12,\n\x12total_cancel_order\x18\x11 \x01(\x04R\x10totalCancelOrder\x12,\n\x12total_create_order\x18\x12 \x01(\x04R\x10totalCreateOrder\x12!\n\x0ctotal_orders\x18\x13 \x01(\x04R\x0btotalOrders\x12!\n\x0ctotal_trades\x18\x14 \x01(\x04R\x0btotalTrades\x12/\n\x13order_subscriptions\x18\x15 \x01(\rR\x12orderSubscriptions\x12/\n\x13trade_subscriptions\x18\x16 \x01(\rR\x12tradeSubscriptions\x12\x31\n\x14\x63\x61ndle_subscriptions\x18\x17 \x01(\rR\x13\x63\x61ndleSubscriptions\x12<\n\x1amarket_depth_subscriptions\x18\x18 \x01(\rR\x18marketDepthSubscriptions\x12\x37\n\x17positions_subscriptions\x18\x19 \x01(\rR\x16positionsSubscriptions\x12\x33\n\x15\x61\x63\x63ount_subscriptions\x18\x1a \x01(\rR\x14\x61\x63\x63ountSubscriptions\x12:\n\x19market_data_subscriptions\x18\x1b \x01(\rR\x17marketDataSubscriptions\x12(\n\x10\x61pp_version_hash\x18\x1c \x01(\tR\x0e\x61ppVersionHash\x12\x1f\n\x0b\x61pp_version\x18\x1d \x01(\tR\nappVersion\x12#\n\rchain_version\x18\x1e \x01(\tR\x0c\x63hainVersion\x12%\n\x0e\x62lock_duration\x18\x1f \x01(\x04R\rblockDuration\x12\x16\n\x06uptime\x18  \x01(\tR\x06uptime\x12\x19\n\x08\x63hain_id\x18! \x01(\tR\x07\x63hainId\x12K\n"market_depth_updates_subscriptions\x18" \x01(\rR\x1fmarketDepthUpdatesSubscriptions\x12\x1d\n\nblock_hash\x18# \x01(\tR\tblockHash\x12\x1b\n\tepoch_seq\x18$ \x01(\x04R\x08\x65pochSeq\x12(\n\x10\x65poch_start_time\x18% \x01(\tR\x0e\x65pochStartTime\x12*\n\x11\x65poch_expiry_time\x18& \x01(\tR\x0f\x65pochExpiryTime"\x18\n\x16LastBlockHeightRequest"\x91\x03\n\x17LastBlockHeightResponse\x12\x16\n\x06height\x18\x01 \x01(\x04R\x06height\x12\x12\n\x04hash\x18\x02 \x01(\tR\x04hash\x12\x33\n\x16spam_pow_hash_function\x18\x03 \x01(\tR\x13spamPowHashFunction\x12.\n\x13spam_pow_difficulty\x18\x04 \x01(\rR\x11spamPowDifficulty\x12\x41\n\x1espam_pow_number_of_past_blocks\x18\x05 \x01(\rR\x19spamPowNumberOfPastBlocks\x12\x42\n\x1fspam_pow_number_of_tx_per_block\x18\x06 \x01(\rR\x19spamPowNumberOfTxPerBlock\x12\x43\n\x1espam_pow_increasing_difficulty\x18\x07 \x01(\x08R\x1bspamPowIncreasingDifficulty\x12\x19\n\x08\x63hain_id\x18\x08 \x01(\tR\x07\x63hainId"5\n\x18GetSpamStatisticsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId"\x94\x01\n\rSpamStatistic\x12&\n\x0f\x63ount_for_epoch\x18\x01 \x01(\x04R\rcountForEpoch\x12"\n\rmax_for_epoch\x18\x02 \x01(\x04R\x0bmaxForEpoch\x12&\n\x0c\x62\x61nned_until\x18\x04 \x01(\tH\x00R\x0b\x62\x61nnedUntil\x88\x01\x01\x42\x0f\n\r_banned_until"\xb1\x01\n\x12VoteSpamStatistics\x12>\n\nstatistics\x18\x01 \x03(\x0b\x32\x1e.vega.api.v1.VoteSpamStatisticR\nstatistics\x12"\n\rmax_for_epoch\x18\x02 \x01(\x04R\x0bmaxForEpoch\x12&\n\x0c\x62\x61nned_until\x18\x03 \x01(\tH\x00R\x0b\x62\x61nnedUntil\x88\x01\x01\x42\x0f\n\r_banned_until"\x87\x01\n\x11VoteSpamStatistic\x12\x1a\n\x08proposal\x18\x01 \x01(\tR\x08proposal\x12&\n\x0f\x63ount_for_epoch\x18\x02 \x01(\x04R\rcountForEpoch\x12.\n\x13min_tokens_required\x18\x03 \x01(\tR\x11minTokensRequired"\xf1\x01\n\rPoWBlockState\x12!\n\x0c\x62lock_height\x18\x01 \x01(\x04R\x0b\x62lockHeight\x12\x1d\n\nblock_hash\x18\x02 \x01(\tR\tblockHash\x12+\n\x11transactions_seen\x18\x03 \x01(\x04R\x10transactionsSeen\x12\x34\n\x13\x65xpected_difficulty\x18\x04 \x01(\x04H\x00R\x12\x65xpectedDifficulty\x88\x01\x01\x12#\n\rhash_function\x18\x05 \x01(\tR\x0chashFunctionB\x16\n\x14_expected_difficulty"\x86\x01\n\x0cPoWStatistic\x12=\n\x0c\x62lock_states\x18\x01 \x03(\x0b\x32\x1a.vega.api.v1.PoWBlockStateR\x0b\x62lockStates\x12&\n\x0c\x62\x61nned_until\x18\x02 \x01(\tH\x00R\x0b\x62\x61nnedUntil\x88\x01\x01\x42\x0f\n\r_banned_until"\xf1\x02\n\x0eSpamStatistics\x12\x38\n\tproposals\x18\x01 \x01(\x0b\x32\x1a.vega.api.v1.SpamStatisticR\tproposals\x12<\n\x0b\x64\x65legations\x18\x02 \x01(\x0b\x32\x1a.vega.api.v1.SpamStatisticR\x0b\x64\x65legations\x12\x38\n\ttransfers\x18\x03 \x01(\x0b\x32\x1a.vega.api.v1.SpamStatisticR\ttransfers\x12I\n\x12node_announcements\x18\x04 \x01(\x0b\x32\x1a.vega.api.v1.SpamStatisticR\x11nodeAnnouncements\x12\x35\n\x05votes\x18\x05 \x01(\x0b\x32\x1f.vega.api.v1.VoteSpamStatisticsR\x05votes\x12+\n\x03pow\x18\x06 \x01(\x0b\x32\x19.vega.api.v1.PoWStatisticR\x03pow"s\n\x19GetSpamStatisticsResponse\x12\x19\n\x08\x63hain_id\x18\x01 \x01(\tR\x07\x63hainId\x12;\n\nstatistics\x18\x02 \x01(\x0b\x32\x1b.vega.api.v1.SpamStatisticsR\nstatistics2\xd8\x07\n\x0b\x43oreService\x12\x62\n\x11SubmitTransaction\x12%.vega.api.v1.SubmitTransactionRequest\x1a&.vega.api.v1.SubmitTransactionResponse\x12h\n\x13PropagateChainEvent\x12\'.vega.api.v1.PropagateChainEventRequest\x1a(.vega.api.v1.PropagateChainEventResponse\x12M\n\nStatistics\x12\x1e.vega.api.v1.StatisticsRequest\x1a\x1f.vega.api.v1.StatisticsResponse\x12\\\n\x0fLastBlockHeight\x12#.vega.api.v1.LastBlockHeightRequest\x1a$.vega.api.v1.LastBlockHeightResponse\x12P\n\x0bGetVegaTime\x12\x1f.vega.api.v1.GetVegaTimeRequest\x1a .vega.api.v1.GetVegaTimeResponse\x12`\n\x0fObserveEventBus\x12#.vega.api.v1.ObserveEventBusRequest\x1a$.vega.api.v1.ObserveEventBusResponse(\x01\x30\x01\x12k\n\x14SubmitRawTransaction\x12(.vega.api.v1.SubmitRawTransactionRequest\x1a).vega.api.v1.SubmitRawTransactionResponse\x12_\n\x10\x43heckTransaction\x12$.vega.api.v1.CheckTransactionRequest\x1a%.vega.api.v1.CheckTransactionResponse\x12h\n\x13\x43heckRawTransaction\x12\'.vega.api.v1.CheckRawTransactionRequest\x1a(.vega.api.v1.CheckRawTransactionResponse\x12\x62\n\x11GetSpamStatistics\x12%.vega.api.v1.GetSpamStatisticsRequest\x1a&.vega.api.v1.GetSpamStatisticsResponseBeZ,code.vegaprotocol.io/vega/protos/vega/api/v1\x92\x41\x34\x12\x19\n\x0eVega core APIs2\x07v0.67.0\x1a\x13lb.testnet.vega.xyz*\x02\x01\x02\x62\x06proto3'
+    b'\n\x16vega/api/v1/core.proto\x12\x0bvega.api.v1\x1a\x0fvega/vega.proto\x1a\x1bvega/events/v1/events.proto\x1a"vega/commands/v1/transaction.proto\x1a.protoc-gen-openapiv2/options/annotations.proto"i\n\x1aPropagateChainEventRequest\x12\x14\n\x05\x65vent\x18\x01 \x01(\x0cR\x05\x65vent\x12\x17\n\x07pub_key\x18\x02 \x01(\tR\x06pubKey\x12\x1c\n\tsignature\x18\x03 \x01(\x0cR\tsignature"7\n\x1bPropagateChainEventResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success"\xd7\x01\n\x18SubmitTransactionRequest\x12-\n\x02tx\x18\x01 \x01(\x0b\x32\x1d.vega.commands.v1.TransactionR\x02tx\x12>\n\x04type\x18\x02 \x01(\x0e\x32*.vega.api.v1.SubmitTransactionRequest.TypeR\x04type"L\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0e\n\nTYPE_ASYNC\x10\x01\x12\r\n\tTYPE_SYNC\x10\x02\x12\x0f\n\x0bTYPE_COMMIT\x10\x03"\xa0\x01\n\x19SubmitTransactionResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12\x17\n\x07tx_hash\x18\x02 \x01(\tR\x06txHash\x12\x12\n\x04\x63ode\x18\x03 \x01(\rR\x04\x63ode\x12\x12\n\x04\x64\x61ta\x18\x04 \x01(\tR\x04\x64\x61ta\x12\x10\n\x03log\x18\x05 \x01(\tR\x03log\x12\x16\n\x06height\x18\x06 \x01(\x03R\x06height"H\n\x17\x43heckTransactionRequest\x12-\n\x02tx\x18\x01 \x01(\x0b\x32\x1d.vega.commands.v1.TransactionR\x02tx"\xbc\x01\n\x18\x43heckTransactionResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12\x12\n\x04\x63ode\x18\x02 \x01(\rR\x04\x63ode\x12\x1d\n\ngas_wanted\x18\x03 \x01(\x03R\tgasWanted\x12\x19\n\x08gas_used\x18\x04 \x01(\x03R\x07gasUsed\x12\x12\n\x04\x64\x61ta\x18\x05 \x01(\tR\x04\x64\x61ta\x12\x10\n\x03log\x18\x06 \x01(\tR\x03log\x12\x12\n\x04info\x18\x07 \x01(\tR\x04info"\xbe\x01\n\x1bSubmitRawTransactionRequest\x12\x0e\n\x02tx\x18\x01 \x01(\x0cR\x02tx\x12\x41\n\x04type\x18\x02 \x01(\x0e\x32-.vega.api.v1.SubmitRawTransactionRequest.TypeR\x04type"L\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0e\n\nTYPE_ASYNC\x10\x01\x12\r\n\tTYPE_SYNC\x10\x02\x12\x0f\n\x0bTYPE_COMMIT\x10\x03"\xa3\x01\n\x1cSubmitRawTransactionResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12\x17\n\x07tx_hash\x18\x02 \x01(\tR\x06txHash\x12\x12\n\x04\x63ode\x18\x03 \x01(\rR\x04\x63ode\x12\x12\n\x04\x64\x61ta\x18\x04 \x01(\tR\x04\x64\x61ta\x12\x10\n\x03log\x18\x05 \x01(\tR\x03log\x12\x16\n\x06height\x18\x06 \x01(\x03R\x06height",\n\x1a\x43heckRawTransactionRequest\x12\x0e\n\x02tx\x18\x01 \x01(\x0cR\x02tx"\xbf\x01\n\x1b\x43heckRawTransactionResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12\x12\n\x04\x63ode\x18\x02 \x01(\rR\x04\x63ode\x12\x1d\n\ngas_wanted\x18\x03 \x01(\x03R\tgasWanted\x12\x19\n\x08gas_used\x18\x04 \x01(\x03R\x07gasUsed\x12\x12\n\x04\x64\x61ta\x18\x05 \x01(\tR\x04\x64\x61ta\x12\x10\n\x03log\x18\x06 \x01(\tR\x03log\x12\x12\n\x04info\x18\x07 \x01(\tR\x04info"\x14\n\x12GetVegaTimeRequest"3\n\x13GetVegaTimeResponse\x12\x1c\n\ttimestamp\x18\x01 \x01(\x03R\ttimestamp"\xa1\x01\n\x16ObserveEventBusRequest\x12\x30\n\x04type\x18\x01 \x03(\x0e\x32\x1c.vega.events.v1.BusEventTypeR\x04type\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x03 \x01(\tR\x07partyId\x12\x1d\n\nbatch_size\x18\x04 \x01(\x03R\tbatchSize"K\n\x17ObserveEventBusResponse\x12\x30\n\x06\x65vents\x18\x01 \x03(\x0b\x32\x18.vega.events.v1.BusEventR\x06\x65vents"\x13\n\x11StatisticsRequest"M\n\x12StatisticsResponse\x12\x37\n\nstatistics\x18\x01 \x01(\x0b\x32\x17.vega.api.v1.StatisticsR\nstatistics"\xc8\x0c\n\nStatistics\x12!\n\x0c\x62lock_height\x18\x01 \x01(\x04R\x0b\x62lockHeight\x12%\n\x0e\x62\x61\x63klog_length\x18\x02 \x01(\x04R\rbacklogLength\x12\x1f\n\x0btotal_peers\x18\x03 \x01(\x04R\ntotalPeers\x12!\n\x0cgenesis_time\x18\x04 \x01(\tR\x0bgenesisTime\x12!\n\x0c\x63urrent_time\x18\x05 \x01(\tR\x0b\x63urrentTime\x12\x1b\n\tvega_time\x18\x06 \x01(\tR\x08vegaTime\x12)\n\x06status\x18\x07 \x01(\x0e\x32\x11.vega.ChainStatusR\x06status\x12 \n\x0ctx_per_block\x18\x08 \x01(\x04R\ntxPerBlock\x12(\n\x10\x61verage_tx_bytes\x18\t \x01(\x04R\x0e\x61verageTxBytes\x12\x37\n\x18\x61verage_orders_per_block\x18\n \x01(\x04R\x15\x61verageOrdersPerBlock\x12*\n\x11trades_per_second\x18\x0b \x01(\x04R\x0ftradesPerSecond\x12*\n\x11orders_per_second\x18\x0c \x01(\x04R\x0fordersPerSecond\x12#\n\rtotal_markets\x18\r \x01(\x04R\x0ctotalMarkets\x12*\n\x11total_amend_order\x18\x10 \x01(\x04R\x0ftotalAmendOrder\x12,\n\x12total_cancel_order\x18\x11 \x01(\x04R\x10totalCancelOrder\x12,\n\x12total_create_order\x18\x12 \x01(\x04R\x10totalCreateOrder\x12!\n\x0ctotal_orders\x18\x13 \x01(\x04R\x0btotalOrders\x12!\n\x0ctotal_trades\x18\x14 \x01(\x04R\x0btotalTrades\x12/\n\x13order_subscriptions\x18\x15 \x01(\rR\x12orderSubscriptions\x12/\n\x13trade_subscriptions\x18\x16 \x01(\rR\x12tradeSubscriptions\x12\x31\n\x14\x63\x61ndle_subscriptions\x18\x17 \x01(\rR\x13\x63\x61ndleSubscriptions\x12<\n\x1amarket_depth_subscriptions\x18\x18 \x01(\rR\x18marketDepthSubscriptions\x12\x37\n\x17positions_subscriptions\x18\x19 \x01(\rR\x16positionsSubscriptions\x12\x33\n\x15\x61\x63\x63ount_subscriptions\x18\x1a \x01(\rR\x14\x61\x63\x63ountSubscriptions\x12:\n\x19market_data_subscriptions\x18\x1b \x01(\rR\x17marketDataSubscriptions\x12(\n\x10\x61pp_version_hash\x18\x1c \x01(\tR\x0e\x61ppVersionHash\x12\x1f\n\x0b\x61pp_version\x18\x1d \x01(\tR\nappVersion\x12#\n\rchain_version\x18\x1e \x01(\tR\x0c\x63hainVersion\x12%\n\x0e\x62lock_duration\x18\x1f \x01(\x04R\rblockDuration\x12\x16\n\x06uptime\x18  \x01(\tR\x06uptime\x12\x19\n\x08\x63hain_id\x18! \x01(\tR\x07\x63hainId\x12K\n"market_depth_updates_subscriptions\x18" \x01(\rR\x1fmarketDepthUpdatesSubscriptions\x12\x1d\n\nblock_hash\x18# \x01(\tR\tblockHash\x12\x1b\n\tepoch_seq\x18$ \x01(\x04R\x08\x65pochSeq\x12(\n\x10\x65poch_start_time\x18% \x01(\tR\x0e\x65pochStartTime\x12*\n\x11\x65poch_expiry_time\x18& \x01(\tR\x0f\x65pochExpiryTime\x12\x1f\n\x0b\x65vent_count\x18\' \x01(\x04R\neventCount\x12*\n\x11\x65vents_per_second\x18( \x01(\x04R\x0f\x65ventsPerSecond"\x18\n\x16LastBlockHeightRequest"\x91\x03\n\x17LastBlockHeightResponse\x12\x16\n\x06height\x18\x01 \x01(\x04R\x06height\x12\x12\n\x04hash\x18\x02 \x01(\tR\x04hash\x12\x33\n\x16spam_pow_hash_function\x18\x03 \x01(\tR\x13spamPowHashFunction\x12.\n\x13spam_pow_difficulty\x18\x04 \x01(\rR\x11spamPowDifficulty\x12\x41\n\x1espam_pow_number_of_past_blocks\x18\x05 \x01(\rR\x19spamPowNumberOfPastBlocks\x12\x42\n\x1fspam_pow_number_of_tx_per_block\x18\x06 \x01(\rR\x19spamPowNumberOfTxPerBlock\x12\x43\n\x1espam_pow_increasing_difficulty\x18\x07 \x01(\x08R\x1bspamPowIncreasingDifficulty\x12\x19\n\x08\x63hain_id\x18\x08 \x01(\tR\x07\x63hainId"5\n\x18GetSpamStatisticsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId"\xc4\x01\n\rSpamStatistic\x12&\n\x0f\x63ount_for_epoch\x18\x01 \x01(\x04R\rcountForEpoch\x12"\n\rmax_for_epoch\x18\x02 \x01(\x04R\x0bmaxForEpoch\x12&\n\x0c\x62\x61nned_until\x18\x04 \x01(\tH\x00R\x0b\x62\x61nnedUntil\x88\x01\x01\x12.\n\x13min_tokens_required\x18\x05 \x01(\tR\x11minTokensRequiredB\x0f\n\r_banned_until"\xb1\x01\n\x12VoteSpamStatistics\x12>\n\nstatistics\x18\x01 \x03(\x0b\x32\x1e.vega.api.v1.VoteSpamStatisticR\nstatistics\x12"\n\rmax_for_epoch\x18\x02 \x01(\x04R\x0bmaxForEpoch\x12&\n\x0c\x62\x61nned_until\x18\x03 \x01(\tH\x00R\x0b\x62\x61nnedUntil\x88\x01\x01\x42\x0f\n\r_banned_until"\x87\x01\n\x11VoteSpamStatistic\x12\x1a\n\x08proposal\x18\x01 \x01(\tR\x08proposal\x12&\n\x0f\x63ount_for_epoch\x18\x02 \x01(\x04R\rcountForEpoch\x12.\n\x13min_tokens_required\x18\x03 \x01(\tR\x11minTokensRequired"\xe8\x02\n\rPoWBlockState\x12!\n\x0c\x62lock_height\x18\x01 \x01(\x04R\x0b\x62lockHeight\x12\x1d\n\nblock_hash\x18\x02 \x01(\tR\tblockHash\x12+\n\x11transactions_seen\x18\x03 \x01(\x04R\x10transactionsSeen\x12\x34\n\x13\x65xpected_difficulty\x18\x04 \x01(\x04H\x00R\x12\x65xpectedDifficulty\x88\x01\x01\x12#\n\rhash_function\x18\x05 \x01(\tR\x0chashFunction\x12\x1e\n\ndifficulty\x18\x06 \x01(\x04R\ndifficulty\x12 \n\x0ctx_per_block\x18\x07 \x01(\x04R\ntxPerBlock\x12\x33\n\x15increasing_difficulty\x18\x08 \x01(\x08R\x14increasingDifficultyB\x16\n\x14_expected_difficulty"\xb9\x01\n\x0cPoWStatistic\x12=\n\x0c\x62lock_states\x18\x01 \x03(\x0b\x32\x1a.vega.api.v1.PoWBlockStateR\x0b\x62lockStates\x12&\n\x0c\x62\x61nned_until\x18\x02 \x01(\tH\x00R\x0b\x62\x61nnedUntil\x88\x01\x01\x12\x31\n\x15number_of_past_blocks\x18\x03 \x01(\x04R\x12numberOfPastBlocksB\x0f\n\r_banned_until"\xd5\x03\n\x0eSpamStatistics\x12\x38\n\tproposals\x18\x01 \x01(\x0b\x32\x1a.vega.api.v1.SpamStatisticR\tproposals\x12<\n\x0b\x64\x65legations\x18\x02 \x01(\x0b\x32\x1a.vega.api.v1.SpamStatisticR\x0b\x64\x65legations\x12\x38\n\ttransfers\x18\x03 \x01(\x0b\x32\x1a.vega.api.v1.SpamStatisticR\ttransfers\x12I\n\x12node_announcements\x18\x04 \x01(\x0b\x32\x1a.vega.api.v1.SpamStatisticR\x11nodeAnnouncements\x12\x35\n\x05votes\x18\x05 \x01(\x0b\x32\x1f.vega.api.v1.VoteSpamStatisticsR\x05votes\x12+\n\x03pow\x18\x06 \x01(\x0b\x32\x19.vega.api.v1.PoWStatisticR\x03pow\x12\x45\n\x10issue_signatures\x18\x07 \x01(\x0b\x32\x1a.vega.api.v1.SpamStatisticR\x0fissueSignatures\x12\x1b\n\tepoch_seq\x18\x08 \x01(\x04R\x08\x65pochSeq"s\n\x19GetSpamStatisticsResponse\x12\x19\n\x08\x63hain_id\x18\x01 \x01(\tR\x07\x63hainId\x12;\n\nstatistics\x18\x02 \x01(\x0b\x32\x1b.vega.api.v1.SpamStatisticsR\nstatistics2\xd8\x07\n\x0b\x43oreService\x12\x62\n\x11SubmitTransaction\x12%.vega.api.v1.SubmitTransactionRequest\x1a&.vega.api.v1.SubmitTransactionResponse\x12h\n\x13PropagateChainEvent\x12\'.vega.api.v1.PropagateChainEventRequest\x1a(.vega.api.v1.PropagateChainEventResponse\x12M\n\nStatistics\x12\x1e.vega.api.v1.StatisticsRequest\x1a\x1f.vega.api.v1.StatisticsResponse\x12\\\n\x0fLastBlockHeight\x12#.vega.api.v1.LastBlockHeightRequest\x1a$.vega.api.v1.LastBlockHeightResponse\x12P\n\x0bGetVegaTime\x12\x1f.vega.api.v1.GetVegaTimeRequest\x1a .vega.api.v1.GetVegaTimeResponse\x12`\n\x0fObserveEventBus\x12#.vega.api.v1.ObserveEventBusRequest\x1a$.vega.api.v1.ObserveEventBusResponse(\x01\x30\x01\x12k\n\x14SubmitRawTransaction\x12(.vega.api.v1.SubmitRawTransactionRequest\x1a).vega.api.v1.SubmitRawTransactionResponse\x12_\n\x10\x43heckTransaction\x12$.vega.api.v1.CheckTransactionRequest\x1a%.vega.api.v1.CheckTransactionResponse\x12h\n\x13\x43heckRawTransaction\x12\'.vega.api.v1.CheckRawTransactionRequest\x1a(.vega.api.v1.CheckRawTransactionResponse\x12\x62\n\x11GetSpamStatistics\x12%.vega.api.v1.GetSpamStatisticsRequest\x1a&.vega.api.v1.GetSpamStatisticsResponseBiZ,code.vegaprotocol.io/vega/protos/vega/api/v1\x92\x41\x38\x12\x1d\n\x0eVega core APIs2\x0bv0.68.0-dev\x1a\x13lb.testnet.vega.xyz*\x02\x01\x02\x62\x06proto3'
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "vega.api.v1.core_pb2", globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
-    DESCRIPTOR._serialized_options = b"Z,code.vegaprotocol.io/vega/protos/vega/api/v1\222A4\022\031\n\016Vega core APIs2\007v0.67.0\032\023lb.testnet.vega.xyz*\002\001\002"
+    DESCRIPTOR._serialized_options = b"Z,code.vegaprotocol.io/vega/protos/vega/api/v1\222A8\022\035\n\016Vega core APIs2\013v0.68.0-dev\032\023lb.testnet.vega.xyz*\002\001\002"
     _PROPAGATECHAINEVENTREQUEST._serialized_start = 169
     _PROPAGATECHAINEVENTREQUEST._serialized_end = 274
     _PROPAGATECHAINEVENTRESPONSE._serialized_start = 276
     _PROPAGATECHAINEVENTRESPONSE._serialized_end = 331
     _SUBMITTRANSACTIONREQUEST._serialized_start = 334
     _SUBMITTRANSACTIONREQUEST._serialized_end = 549
     _SUBMITTRANSACTIONREQUEST_TYPE._serialized_start = 473
@@ -65,31 +64,31 @@
     _OBSERVEEVENTBUSRESPONSE._serialized_start = 1817
     _OBSERVEEVENTBUSRESPONSE._serialized_end = 1892
     _STATISTICSREQUEST._serialized_start = 1894
     _STATISTICSREQUEST._serialized_end = 1913
     _STATISTICSRESPONSE._serialized_start = 1915
     _STATISTICSRESPONSE._serialized_end = 1992
     _STATISTICS._serialized_start = 1995
-    _STATISTICS._serialized_end = 3526
-    _LASTBLOCKHEIGHTREQUEST._serialized_start = 3528
-    _LASTBLOCKHEIGHTREQUEST._serialized_end = 3552
-    _LASTBLOCKHEIGHTRESPONSE._serialized_start = 3555
-    _LASTBLOCKHEIGHTRESPONSE._serialized_end = 3956
-    _GETSPAMSTATISTICSREQUEST._serialized_start = 3958
-    _GETSPAMSTATISTICSREQUEST._serialized_end = 4011
-    _SPAMSTATISTIC._serialized_start = 4014
-    _SPAMSTATISTIC._serialized_end = 4162
-    _VOTESPAMSTATISTICS._serialized_start = 4165
-    _VOTESPAMSTATISTICS._serialized_end = 4342
-    _VOTESPAMSTATISTIC._serialized_start = 4345
-    _VOTESPAMSTATISTIC._serialized_end = 4480
-    _POWBLOCKSTATE._serialized_start = 4483
-    _POWBLOCKSTATE._serialized_end = 4724
-    _POWSTATISTIC._serialized_start = 4727
-    _POWSTATISTIC._serialized_end = 4861
-    _SPAMSTATISTICS._serialized_start = 4864
-    _SPAMSTATISTICS._serialized_end = 5233
-    _GETSPAMSTATISTICSRESPONSE._serialized_start = 5235
-    _GETSPAMSTATISTICSRESPONSE._serialized_end = 5350
-    _CORESERVICE._serialized_start = 5353
-    _CORESERVICE._serialized_end = 6337
+    _STATISTICS._serialized_end = 3603
+    _LASTBLOCKHEIGHTREQUEST._serialized_start = 3605
+    _LASTBLOCKHEIGHTREQUEST._serialized_end = 3629
+    _LASTBLOCKHEIGHTRESPONSE._serialized_start = 3632
+    _LASTBLOCKHEIGHTRESPONSE._serialized_end = 4033
+    _GETSPAMSTATISTICSREQUEST._serialized_start = 4035
+    _GETSPAMSTATISTICSREQUEST._serialized_end = 4088
+    _SPAMSTATISTIC._serialized_start = 4091
+    _SPAMSTATISTIC._serialized_end = 4287
+    _VOTESPAMSTATISTICS._serialized_start = 4290
+    _VOTESPAMSTATISTICS._serialized_end = 4467
+    _VOTESPAMSTATISTIC._serialized_start = 4470
+    _VOTESPAMSTATISTIC._serialized_end = 4605
+    _POWBLOCKSTATE._serialized_start = 4608
+    _POWBLOCKSTATE._serialized_end = 4968
+    _POWSTATISTIC._serialized_start = 4971
+    _POWSTATISTIC._serialized_end = 5156
+    _SPAMSTATISTICS._serialized_start = 5159
+    _SPAMSTATISTICS._serialized_end = 5628
+    _GETSPAMSTATISTICSRESPONSE._serialized_start = 5630
+    _GETSPAMSTATISTICSRESPONSE._serialized_end = 5745
+    _CORESERVICE._serialized_start = 5748
+    _CORESERVICE._serialized_end = 6732
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-0.67.0/vega_sim/proto/vega/api/v1/core_pb2_grpc.py` & `vega_sim-1.0.1/vega_sim/proto/vega/api/v1/core_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/proto/vega/api/v1/corestate_pb2.py` & `vega_sim-1.0.1/vega_sim/proto/vega/api/v1/corestate_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,25 +19,24 @@
 from ...events.v1 import events_pb2 as vega_dot_events_dot_v1_dot_events__pb2
 from protoc_gen_openapiv2.options import (
     annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2,
 )
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x1bvega/api/v1/corestate.proto\x12\x0bvega.api.v1\x1a\x11vega/assets.proto\x1a\x15vega/governance.proto\x1a\x12vega/markets.proto\x1a\x0fvega/vega.proto\x1a\x1bvega/events/v1/events.proto\x1a.protoc-gen-openapiv2/options/annotations.proto"{\n\x07\x41\x63\x63ount\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x16\n\x06market\x18\x02 \x01(\tR\x06market\x12\x18\n\x07\x62\x61lance\x18\x03 \x01(\tR\x07\x62\x61lance\x12\x14\n\x05\x61sset\x18\x05 \x01(\tR\x05\x61sset\x12\x12\n\x04type\x18\x06 \x01(\tR\x04type"C\n\x13ListAccountsRequest\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x16\n\x06market\x18\x02 \x01(\tR\x06market"H\n\x14ListAccountsResponse\x12\x30\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32\x14.vega.api.v1.AccountR\x08\x61\x63\x63ounts")\n\x11ListAssetsRequest\x12\x14\n\x05\x61sset\x18\x01 \x01(\tR\x05\x61sset"9\n\x12ListAssetsResponse\x12#\n\x06\x61ssets\x18\x01 \x03(\x0b\x32\x0b.vega.AssetR\x06\x61ssets"R\n\x1cListNetworkParametersRequest\x12\x32\n\x15network_parameter_key\x18\x01 \x01(\tR\x13networkParameterKey"f\n\x1dListNetworkParametersResponse\x12\x45\n\x12network_parameters\x18\x01 \x03(\x0b\x32\x16.vega.NetworkParameterR\x11networkParameters"\x1a\n\x18ListNetworkLimitsRequest"W\n\x19ListNetworkLimitsResponse\x12:\n\x0enetwork_limits\x18\x01 \x01(\x0b\x32\x13.vega.NetworkLimitsR\rnetworkLimits"\x14\n\x12ListPartiesRequest"<\n\x13ListPartiesResponse\x12%\n\x07parties\x18\x01 \x03(\x0b\x32\x0b.vega.PartyR\x07parties"\x17\n\x15ListValidatorsRequest"Y\n\x16ListValidatorsResponse\x12?\n\nvalidators\x18\x01 \x03(\x0b\x32\x1f.vega.events.v1.ValidatorUpdateR\nvalidators",\n\x12ListMarketsRequest\x12\x16\n\x06market\x18\x01 \x01(\tR\x06market"=\n\x13ListMarketsResponse\x12&\n\x07markets\x18\x01 \x03(\x0b\x32\x0c.vega.MarketR\x07markets"N\n\x14ListProposalsRequest\x12\x1a\n\x08proposal\x18\x01 \x01(\tR\x08proposal\x12\x1a\n\x08proposer\x18\x02 \x01(\tR\x08proposer"E\n\x15ListProposalsResponse\x12,\n\tproposals\x18\x01 \x03(\x0b\x32\x0e.vega.ProposalR\tproposals"0\n\x16ListMarketsDataRequest\x12\x16\n\x06market\x18\x01 \x01(\tR\x06market"N\n\x17ListMarketsDataResponse\x12\x33\n\x0cmarkets_data\x18\x01 \x03(\x0b\x32\x10.vega.MarketDataR\x0bmarketsData"D\n\x10ListVotesRequest\x12\x1a\n\x08proposal\x18\x01 \x01(\tR\x08proposal\x12\x14\n\x05party\x18\x02 \x01(\tR\x05party"5\n\x11ListVotesResponse\x12 \n\x05votes\x18\x01 \x03(\x0b\x32\n.vega.VoteR\x05votes"\x9f\x01\n\nPartyStake\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x36\n\x17\x63urrent_stake_available\x18\x02 \x01(\tR\x15\x63urrentStakeAvailable\x12\x43\n\x0estake_linkings\x18\x03 \x03(\x0b\x32\x1c.vega.events.v1.StakeLinkingR\rstakeLinkings"/\n\x17ListPartiesStakeRequest\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party"X\n\x18ListPartiesStakeResponse\x12<\n\rparties_stake\x18\x01 \x03(\x0b\x32\x17.vega.api.v1.PartyStakeR\x0cpartiesStake"_\n\x16ListDelegationsRequest\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x12\n\x04node\x18\x02 \x01(\tR\x04node\x12\x1b\n\tepoch_seq\x18\x03 \x01(\tR\x08\x65pochSeq"M\n\x17ListDelegationsResponse\x12\x32\n\x0b\x64\x65legations\x18\x01 \x03(\x0b\x32\x10.vega.DelegationR\x0b\x64\x65legations2\xca\x08\n\x10\x43oreStateService\x12S\n\x0cListAccounts\x12 .vega.api.v1.ListAccountsRequest\x1a!.vega.api.v1.ListAccountsResponse\x12M\n\nListAssets\x12\x1e.vega.api.v1.ListAssetsRequest\x1a\x1f.vega.api.v1.ListAssetsResponse\x12n\n\x15ListNetworkParameters\x12).vega.api.v1.ListNetworkParametersRequest\x1a*.vega.api.v1.ListNetworkParametersResponse\x12\x62\n\x11ListNetworkLimits\x12%.vega.api.v1.ListNetworkLimitsRequest\x1a&.vega.api.v1.ListNetworkLimitsResponse\x12P\n\x0bListParties\x12\x1f.vega.api.v1.ListPartiesRequest\x1a .vega.api.v1.ListPartiesResponse\x12Y\n\x0eListValidators\x12".vega.api.v1.ListValidatorsRequest\x1a#.vega.api.v1.ListValidatorsResponse\x12P\n\x0bListMarkets\x12\x1f.vega.api.v1.ListMarketsRequest\x1a .vega.api.v1.ListMarketsResponse\x12V\n\rListProposals\x12!.vega.api.v1.ListProposalsRequest\x1a".vega.api.v1.ListProposalsResponse\x12\\\n\x0fListMarketsData\x12#.vega.api.v1.ListMarketsDataRequest\x1a$.vega.api.v1.ListMarketsDataResponse\x12J\n\tListVotes\x12\x1d.vega.api.v1.ListVotesRequest\x1a\x1e.vega.api.v1.ListVotesResponse\x12_\n\x10ListPartiesStake\x12$.vega.api.v1.ListPartiesStakeRequest\x1a%.vega.api.v1.ListPartiesStakeResponse\x12\\\n\x0fListDelegations\x12#.vega.api.v1.ListDelegationsRequest\x1a$.vega.api.v1.ListDelegationsResponseBkZ,code.vegaprotocol.io/vega/protos/vega/api/v1\x92\x41:\x12\x1f\n\x14Vega core state APIs2\x07v0.67.0\x1a\x13lb.testnet.vega.xyz*\x02\x01\x02\x62\x06proto3'
+    b'\n\x1bvega/api/v1/corestate.proto\x12\x0bvega.api.v1\x1a\x11vega/assets.proto\x1a\x15vega/governance.proto\x1a\x12vega/markets.proto\x1a\x0fvega/vega.proto\x1a\x1bvega/events/v1/events.proto\x1a.protoc-gen-openapiv2/options/annotations.proto"{\n\x07\x41\x63\x63ount\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x16\n\x06market\x18\x02 \x01(\tR\x06market\x12\x18\n\x07\x62\x61lance\x18\x03 \x01(\tR\x07\x62\x61lance\x12\x14\n\x05\x61sset\x18\x05 \x01(\tR\x05\x61sset\x12\x12\n\x04type\x18\x06 \x01(\tR\x04type"C\n\x13ListAccountsRequest\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x16\n\x06market\x18\x02 \x01(\tR\x06market"H\n\x14ListAccountsResponse\x12\x30\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32\x14.vega.api.v1.AccountR\x08\x61\x63\x63ounts")\n\x11ListAssetsRequest\x12\x14\n\x05\x61sset\x18\x01 \x01(\tR\x05\x61sset"9\n\x12ListAssetsResponse\x12#\n\x06\x61ssets\x18\x01 \x03(\x0b\x32\x0b.vega.AssetR\x06\x61ssets"R\n\x1cListNetworkParametersRequest\x12\x32\n\x15network_parameter_key\x18\x01 \x01(\tR\x13networkParameterKey"f\n\x1dListNetworkParametersResponse\x12\x45\n\x12network_parameters\x18\x01 \x03(\x0b\x32\x16.vega.NetworkParameterR\x11networkParameters"\x1a\n\x18ListNetworkLimitsRequest"W\n\x19ListNetworkLimitsResponse\x12:\n\x0enetwork_limits\x18\x01 \x01(\x0b\x32\x13.vega.NetworkLimitsR\rnetworkLimits"\x14\n\x12ListPartiesRequest"<\n\x13ListPartiesResponse\x12%\n\x07parties\x18\x01 \x03(\x0b\x32\x0b.vega.PartyR\x07parties"\x17\n\x15ListValidatorsRequest"Y\n\x16ListValidatorsResponse\x12?\n\nvalidators\x18\x01 \x03(\x0b\x32\x1f.vega.events.v1.ValidatorUpdateR\nvalidators",\n\x12ListMarketsRequest\x12\x16\n\x06market\x18\x01 \x01(\tR\x06market"=\n\x13ListMarketsResponse\x12&\n\x07markets\x18\x01 \x03(\x0b\x32\x0c.vega.MarketR\x07markets"N\n\x14ListProposalsRequest\x12\x1a\n\x08proposal\x18\x01 \x01(\tR\x08proposal\x12\x1a\n\x08proposer\x18\x02 \x01(\tR\x08proposer"E\n\x15ListProposalsResponse\x12,\n\tproposals\x18\x01 \x03(\x0b\x32\x0e.vega.ProposalR\tproposals"0\n\x16ListMarketsDataRequest\x12\x16\n\x06market\x18\x01 \x01(\tR\x06market"N\n\x17ListMarketsDataResponse\x12\x33\n\x0cmarkets_data\x18\x01 \x03(\x0b\x32\x10.vega.MarketDataR\x0bmarketsData"D\n\x10ListVotesRequest\x12\x1a\n\x08proposal\x18\x01 \x01(\tR\x08proposal\x12\x14\n\x05party\x18\x02 \x01(\tR\x05party"5\n\x11ListVotesResponse\x12 \n\x05votes\x18\x01 \x03(\x0b\x32\n.vega.VoteR\x05votes"\x9f\x01\n\nPartyStake\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x36\n\x17\x63urrent_stake_available\x18\x02 \x01(\tR\x15\x63urrentStakeAvailable\x12\x43\n\x0estake_linkings\x18\x03 \x03(\x0b\x32\x1c.vega.events.v1.StakeLinkingR\rstakeLinkings"/\n\x17ListPartiesStakeRequest\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party"X\n\x18ListPartiesStakeResponse\x12<\n\rparties_stake\x18\x01 \x03(\x0b\x32\x17.vega.api.v1.PartyStakeR\x0cpartiesStake"_\n\x16ListDelegationsRequest\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x12\n\x04node\x18\x02 \x01(\tR\x04node\x12\x1b\n\tepoch_seq\x18\x03 \x01(\tR\x08\x65pochSeq"M\n\x17ListDelegationsResponse\x12\x32\n\x0b\x64\x65legations\x18\x01 \x03(\x0b\x32\x10.vega.DelegationR\x0b\x64\x65legations2\xca\x08\n\x10\x43oreStateService\x12S\n\x0cListAccounts\x12 .vega.api.v1.ListAccountsRequest\x1a!.vega.api.v1.ListAccountsResponse\x12M\n\nListAssets\x12\x1e.vega.api.v1.ListAssetsRequest\x1a\x1f.vega.api.v1.ListAssetsResponse\x12n\n\x15ListNetworkParameters\x12).vega.api.v1.ListNetworkParametersRequest\x1a*.vega.api.v1.ListNetworkParametersResponse\x12\x62\n\x11ListNetworkLimits\x12%.vega.api.v1.ListNetworkLimitsRequest\x1a&.vega.api.v1.ListNetworkLimitsResponse\x12P\n\x0bListParties\x12\x1f.vega.api.v1.ListPartiesRequest\x1a .vega.api.v1.ListPartiesResponse\x12Y\n\x0eListValidators\x12".vega.api.v1.ListValidatorsRequest\x1a#.vega.api.v1.ListValidatorsResponse\x12P\n\x0bListMarkets\x12\x1f.vega.api.v1.ListMarketsRequest\x1a .vega.api.v1.ListMarketsResponse\x12V\n\rListProposals\x12!.vega.api.v1.ListProposalsRequest\x1a".vega.api.v1.ListProposalsResponse\x12\\\n\x0fListMarketsData\x12#.vega.api.v1.ListMarketsDataRequest\x1a$.vega.api.v1.ListMarketsDataResponse\x12J\n\tListVotes\x12\x1d.vega.api.v1.ListVotesRequest\x1a\x1e.vega.api.v1.ListVotesResponse\x12_\n\x10ListPartiesStake\x12$.vega.api.v1.ListPartiesStakeRequest\x1a%.vega.api.v1.ListPartiesStakeResponse\x12\\\n\x0fListDelegations\x12#.vega.api.v1.ListDelegationsRequest\x1a$.vega.api.v1.ListDelegationsResponseBoZ,code.vegaprotocol.io/vega/protos/vega/api/v1\x92\x41>\x12#\n\x14Vega core state APIs2\x0bv0.68.0-dev\x1a\x13lb.testnet.vega.xyz*\x02\x01\x02\x62\x06proto3'
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(
     DESCRIPTOR, "vega.api.v1.corestate_pb2", globals()
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
-    DESCRIPTOR._serialized_options = b"Z,code.vegaprotocol.io/vega/protos/vega/api/v1\222A:\022\037\n\024Vega core state APIs2\007v0.67.0\032\023lb.testnet.vega.xyz*\002\001\002"
+    DESCRIPTOR._serialized_options = b"Z,code.vegaprotocol.io/vega/protos/vega/api/v1\222A>\022#\n\024Vega core state APIs2\013v0.68.0-dev\032\023lb.testnet.vega.xyz*\002\001\002"
     _ACCOUNT._serialized_start = 200
     _ACCOUNT._serialized_end = 323
     _LISTACCOUNTSREQUEST._serialized_start = 325
     _LISTACCOUNTSREQUEST._serialized_end = 392
     _LISTACCOUNTSRESPONSE._serialized_start = 394
     _LISTACCOUNTSRESPONSE._serialized_end = 466
     _LISTASSETSREQUEST._serialized_start = 468
```

### Comparing `vega_sim-0.67.0/vega_sim/proto/vega/api/v1/corestate_pb2_grpc.py` & `vega_sim-1.0.1/vega_sim/proto/vega/api/v1/corestate_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ListNetworkParameters(self, request, context):
         """Network parameters list
 
-        Return a list of network paramters
+        Return a list of network parameters
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ListNetworkLimits(self, request, context):
         """Network limits list
```

### Comparing `vega_sim-0.67.0/vega_sim/proto/vega/assets_pb2.py` & `vega_sim-1.0.1/vega_sim/proto/vega/assets_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
     b'\n\x11vega/assets.proto\x12\x04vega"\xed\x01\n\x05\x41sset\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12,\n\x07\x64\x65tails\x18\x02 \x01(\x0b\x32\x12.vega.AssetDetailsR\x07\x64\x65tails\x12*\n\x06status\x18\x03 \x01(\x0e\x32\x12.vega.Asset.StatusR\x06status"z\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x13\n\x0fSTATUS_PROPOSED\x10\x01\x12\x13\n\x0fSTATUS_REJECTED\x10\x02\x12\x1a\n\x16STATUS_PENDING_LISTING\x10\x03\x12\x12\n\x0eSTATUS_ENABLED\x10\x04"\xe0\x01\n\x0c\x41ssetDetails\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x16\n\x06symbol\x18\x02 \x01(\tR\x06symbol\x12\x1a\n\x08\x64\x65\x63imals\x18\x04 \x01(\x04R\x08\x64\x65\x63imals\x12\x18\n\x07quantum\x18\x05 \x01(\tR\x07quantum\x12\x39\n\rbuiltin_asset\x18\x65 \x01(\x0b\x32\x12.vega.BuiltinAssetH\x00R\x0c\x62uiltinAsset\x12#\n\x05\x65rc20\x18\x66 \x01(\x0b\x32\x0b.vega.ERC20H\x00R\x05\x65rc20B\x08\n\x06sourceJ\x04\x08\x03\x10\x04"C\n\x0c\x42uiltinAsset\x12\x33\n\x16max_faucet_amount_mint\x18\x01 \x01(\tR\x13maxFaucetAmountMint"\x88\x01\n\x05\x45RC20\x12)\n\x10\x63ontract_address\x18\x01 \x01(\tR\x0f\x63ontractAddress\x12%\n\x0elifetime_limit\x18\x02 \x01(\tR\rlifetimeLimit\x12-\n\x12withdraw_threshold\x18\x03 \x01(\tR\x11withdrawThreshold"{\n\x12\x41ssetDetailsUpdate\x12\x18\n\x07quantum\x18\x05 \x01(\tR\x07quantum\x12)\n\x05\x65rc20\x18\x65 \x01(\x0b\x32\x11.vega.ERC20UpdateH\x00R\x05\x65rc20B\x08\n\x06sourceJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05"c\n\x0b\x45RC20Update\x12%\n\x0elifetime_limit\x18\x01 \x01(\tR\rlifetimeLimit\x12-\n\x12withdraw_threshold\x18\x02 \x01(\tR\x11withdrawThresholdB\'Z%code.vegaprotocol.io/vega/protos/vegab\x06proto3'
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "vega.assets_pb2", globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b"Z%code.vegaprotocol.io/vega/protos/vega"
     _ASSET._serialized_start = 28
     _ASSET._serialized_end = 265
     _ASSET_STATUS._serialized_start = 143
     _ASSET_STATUS._serialized_end = 265
     _ASSETDETAILS._serialized_start = 268
```

### Comparing `vega_sim-0.67.0/vega_sim/proto/vega/chain_events_pb2.py` & `vega_sim-1.0.1/vega_sim/proto/vega/chain_events_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
     b'\n\x17vega/chain_events.proto\x12\x04vega"l\n\x13\x42uiltinAssetDeposit\x12"\n\rvega_asset_id\x18\x01 \x01(\tR\x0bvegaAssetId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount"o\n\x16\x42uiltinAssetWithdrawal\x12"\n\rvega_asset_id\x18\x01 \x01(\tR\x0bvegaAssetId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount"\x96\x01\n\x11\x42uiltinAssetEvent\x12\x36\n\x07\x64\x65posit\x18\xe9\x07 \x01(\x0b\x32\x19.vega.BuiltinAssetDepositH\x00R\x07\x64\x65posit\x12?\n\nwithdrawal\x18\xea\x07 \x01(\x0b\x32\x1c.vega.BuiltinAssetWithdrawalH\x00R\nwithdrawalB\x08\n\x06\x61\x63tion"W\n\x0e\x45RC20AssetList\x12"\n\rvega_asset_id\x18\x01 \x01(\tR\x0bvegaAssetId\x12!\n\x0c\x61sset_source\x18\x02 \x01(\tR\x0b\x61ssetSource"6\n\x10\x45RC20AssetDelist\x12"\n\rvega_asset_id\x18\x01 \x01(\tR\x0bvegaAssetId"\xcd\x01\n\x17\x45RC20AssetLimitsUpdated\x12"\n\rvega_asset_id\x18\x01 \x01(\tR\x0bvegaAssetId\x12\x36\n\x17source_ethereum_address\x18\x02 \x01(\tR\x15sourceEthereumAddress\x12\'\n\x0flifetime_limits\x18\x03 \x01(\tR\x0elifetimeLimits\x12-\n\x12withdraw_threshold\x18\x04 \x01(\tR\x11withdrawThreshold"\xaa\x01\n\x0c\x45RC20Deposit\x12"\n\rvega_asset_id\x18\x01 \x01(\tR\x0bvegaAssetId\x12\x36\n\x17source_ethereum_address\x18\x02 \x01(\tR\x15sourceEthereumAddress\x12&\n\x0ftarget_party_id\x18\x03 \x01(\tR\rtargetPartyId\x12\x16\n\x06\x61mount\x18\x04 \x01(\tR\x06\x61mount"\x96\x01\n\x0f\x45RC20Withdrawal\x12"\n\rvega_asset_id\x18\x01 \x01(\tR\x0bvegaAssetId\x12\x36\n\x17target_ethereum_address\x18\x02 \x01(\tR\x15targetEthereumAddress\x12\'\n\x0freference_nonce\x18\x03 \x01(\tR\x0ereferenceNonce"\xcb\x03\n\nERC20Event\x12\x14\n\x05index\x18\x01 \x01(\x04R\x05index\x12\x14\n\x05\x62lock\x18\x02 \x01(\x04R\x05\x62lock\x12\x36\n\nasset_list\x18\xe9\x07 \x01(\x0b\x32\x14.vega.ERC20AssetListH\x00R\tassetList\x12<\n\x0c\x61sset_delist\x18\xea\x07 \x01(\x0b\x32\x16.vega.ERC20AssetDelistH\x00R\x0b\x61ssetDelist\x12/\n\x07\x64\x65posit\x18\xeb\x07 \x01(\x0b\x32\x12.vega.ERC20DepositH\x00R\x07\x64\x65posit\x12\x38\n\nwithdrawal\x18\xec\x07 \x01(\x0b\x32\x15.vega.ERC20WithdrawalH\x00R\nwithdrawal\x12R\n\x14\x61sset_limits_updated\x18\xed\x07 \x01(\x0b\x32\x1d.vega.ERC20AssetLimitsUpdatedH\x00R\x12\x61ssetLimitsUpdated\x12(\n\x0e\x62ridge_stopped\x18\xee\x07 \x01(\x08H\x00R\rbridgeStopped\x12(\n\x0e\x62ridge_resumed\x18\xef\x07 \x01(\x08H\x00R\rbridgeResumedB\x08\n\x06\x61\x63tion"f\n\x10\x45RC20SignerAdded\x12\x1d\n\nnew_signer\x18\x01 \x01(\tR\tnewSigner\x12\x14\n\x05nonce\x18\x02 \x01(\tR\x05nonce\x12\x1d\n\nblock_time\x18\x03 \x01(\x03R\tblockTime"h\n\x12\x45RC20SignerRemoved\x12\x1d\n\nold_signer\x18\x01 \x01(\tR\toldSigner\x12\x14\n\x05nonce\x18\x02 \x01(\tR\x05nonce\x12\x1d\n\nblock_time\x18\x03 \x01(\x03R\tblockTime"m\n\x11\x45RC20ThresholdSet\x12#\n\rnew_threshold\x18\x01 \x01(\rR\x0cnewThreshold\x12\x14\n\x05nonce\x18\x02 \x01(\tR\x05nonce\x12\x1d\n\nblock_time\x18\x03 \x01(\x03R\tblockTime"\x8d\x02\n\x12\x45RC20MultiSigEvent\x12\x14\n\x05index\x18\x01 \x01(\x04R\x05index\x12\x14\n\x05\x62lock\x18\x02 \x01(\x04R\x05\x62lock\x12<\n\x0csigner_added\x18\xe9\x07 \x01(\x0b\x32\x16.vega.ERC20SignerAddedH\x00R\x0bsignerAdded\x12\x42\n\x0esigner_removed\x18\xea\x07 \x01(\x0b\x32\x18.vega.ERC20SignerRemovedH\x00R\rsignerRemoved\x12?\n\rthreshold_set\x18\xeb\x07 \x01(\x0b\x32\x17.vega.ERC20ThresholdSetH\x00R\x0cthresholdSetB\x08\n\x06\x61\x63tion"\x80\x02\n\x0cStakingEvent\x12\x14\n\x05index\x18\x01 \x01(\x04R\x05index\x12\x14\n\x05\x62lock\x18\x02 \x01(\x04R\x05\x62lock\x12@\n\x0fstake_deposited\x18\xe9\x07 \x01(\x0b\x32\x14.vega.StakeDepositedH\x00R\x0estakeDeposited\x12:\n\rstake_removed\x18\xea\x07 \x01(\x0b\x32\x12.vega.StakeRemovedH\x00R\x0cstakeRemoved\x12<\n\x0ctotal_supply\x18\xeb\x07 \x01(\x0b\x32\x16.vega.StakeTotalSupplyH\x00R\x0btotalSupplyB\x08\n\x06\x61\x63tion"\x9a\x01\n\x0eStakeDeposited\x12)\n\x10\x65thereum_address\x18\x01 \x01(\tR\x0f\x65thereumAddress\x12&\n\x0fvega_public_key\x18\x02 \x01(\tR\rvegaPublicKey\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x1d\n\nblock_time\x18\x04 \x01(\x03R\tblockTime"\x98\x01\n\x0cStakeRemoved\x12)\n\x10\x65thereum_address\x18\x01 \x01(\tR\x0f\x65thereumAddress\x12&\n\x0fvega_public_key\x18\x02 \x01(\tR\rvegaPublicKey\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x1d\n\nblock_time\x18\x04 \x01(\x03R\tblockTime"Z\n\x10StakeTotalSupply\x12#\n\rtoken_address\x18\x01 \x01(\tR\x0ctokenAddress\x12!\n\x0ctotal_supply\x18\x02 \x01(\tR\x0btotalSupplyB\'Z%code.vegaprotocol.io/vega/protos/vegab\x06proto3'
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "vega.chain_events_pb2", globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b"Z%code.vegaprotocol.io/vega/protos/vega"
     _BUILTINASSETDEPOSIT._serialized_start = 33
     _BUILTINASSETDEPOSIT._serialized_end = 141
     _BUILTINASSETWITHDRAWAL._serialized_start = 143
     _BUILTINASSETWITHDRAWAL._serialized_end = 254
     _BUILTINASSETEVENT._serialized_start = 257
```

### Comparing `vega_sim-0.67.0/vega_sim/proto/vega/checkpoint/v1/checkpoint_pb2.py` & `vega_sim-1.0.1/vega_sim/proto/vega/checkpoint/v1/checkpoint_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(
     DESCRIPTOR, "vega.checkpoint.v1.checkpoint_pb2", globals()
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = (
         b"Z3code.vegaprotocol.io/vega/protos/vega/checkpoint/v1"
     )
     _CHECKPOINTSTATE._serialized_start = 147
     _CHECKPOINTSTATE._serialized_end = 206
     _CHECKPOINT._serialized_start = 209
```

### Comparing `vega_sim-0.67.0/vega_sim/proto/vega/commands/v1/__init__.py` & `vega_sim-1.0.1/vega_sim/proto/vega/commands/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/proto/vega/commands/v1/commands_pb2.py` & `vega_sim-1.0.1/vega_sim/proto/vega/commands/v1/commands_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,58 +10,62 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from ... import governance_pb2 as vega_dot_governance__pb2
 from ... import vega_pb2 as vega_dot_vega__pb2
+from ...commands.v1 import (
+    validator_commands_pb2 as vega_dot_commands_dot_v1_dot_validator__commands__pb2,
+)
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x1fvega/commands/v1/commands.proto\x12\x10vega.commands.v1\x1a\x15vega/governance.proto\x1a\x0fvega/vega.proto"\xeb\x01\n\x17\x42\x61tchMarketInstructions\x12I\n\rcancellations\x18\x01 \x03(\x0b\x32#.vega.commands.v1.OrderCancellationR\rcancellations\x12@\n\namendments\x18\x02 \x03(\x0b\x32 .vega.commands.v1.OrderAmendmentR\namendments\x12\x43\n\x0bsubmissions\x18\x03 \x03(\x0b\x32!.vega.commands.v1.OrderSubmissionR\x0bsubmissions"\xce\x02\n\x0fOrderSubmission\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x14\n\x05price\x18\x02 \x01(\tR\x05price\x12\x12\n\x04size\x18\x03 \x01(\x04R\x04size\x12\x1e\n\x04side\x18\x04 \x01(\x0e\x32\n.vega.SideR\x04side\x12;\n\rtime_in_force\x18\x05 \x01(\x0e\x32\x17.vega.Order.TimeInForceR\x0btimeInForce\x12\x1d\n\nexpires_at\x18\x06 \x01(\x03R\texpiresAt\x12$\n\x04type\x18\x07 \x01(\x0e\x32\x10.vega.Order.TypeR\x04type\x12\x1c\n\treference\x18\x08 \x01(\tR\treference\x12\x34\n\x0cpegged_order\x18\t \x01(\x0b\x32\x11.vega.PeggedOrderR\x0bpeggedOrder"K\n\x11OrderCancellation\x12\x19\n\x08order_id\x18\x01 \x01(\tR\x07orderId\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId"\xe3\x02\n\x0eOrderAmendment\x12\x19\n\x08order_id\x18\x01 \x01(\tR\x07orderId\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x19\n\x05price\x18\x03 \x01(\tH\x00R\x05price\x88\x01\x01\x12\x1d\n\nsize_delta\x18\x04 \x01(\x03R\tsizeDelta\x12"\n\nexpires_at\x18\x05 \x01(\x03H\x01R\texpiresAt\x88\x01\x01\x12;\n\rtime_in_force\x18\x06 \x01(\x0e\x32\x17.vega.Order.TimeInForceR\x0btimeInForce\x12#\n\rpegged_offset\x18\x07 \x01(\tR\x0cpeggedOffset\x12@\n\x10pegged_reference\x18\x08 \x01(\x0e\x32\x15.vega.PeggedReferenceR\x0fpeggedReferenceB\x08\n\x06_priceB\r\n\x0b_expires_at"\xee\x01\n\x1cLiquidityProvisionSubmission\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12+\n\x11\x63ommitment_amount\x18\x02 \x01(\tR\x10\x63ommitmentAmount\x12\x10\n\x03\x66\x65\x65\x18\x03 \x01(\tR\x03\x66\x65\x65\x12*\n\x05sells\x18\x04 \x03(\x0b\x32\x14.vega.LiquidityOrderR\x05sells\x12(\n\x04\x62uys\x18\x05 \x03(\x0b\x32\x14.vega.LiquidityOrderR\x04\x62uys\x12\x1c\n\treference\x18\x06 \x01(\tR\treference"=\n\x1eLiquidityProvisionCancellation\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId"\xed\x01\n\x1bLiquidityProvisionAmendment\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12+\n\x11\x63ommitment_amount\x18\x02 \x01(\tR\x10\x63ommitmentAmount\x12\x10\n\x03\x66\x65\x65\x18\x03 \x01(\tR\x03\x66\x65\x65\x12*\n\x05sells\x18\x04 \x03(\x0b\x32\x14.vega.LiquidityOrderR\x05sells\x12(\n\x04\x62uys\x18\x05 \x03(\x0b\x32\x14.vega.LiquidityOrderR\x04\x62uys\x12\x1c\n\treference\x18\x06 \x01(\tR\treference"g\n\x12WithdrawSubmission\x12\x16\n\x06\x61mount\x18\x01 \x01(\tR\x06\x61mount\x12\x14\n\x05\x61sset\x18\x02 \x01(\tR\x05\x61sset\x12#\n\x03\x65xt\x18\x03 \x01(\x0b\x32\x11.vega.WithdrawExtR\x03\x65xt"\x94\x01\n\x12ProposalSubmission\x12\x1c\n\treference\x18\x01 \x01(\tR\treference\x12)\n\x05terms\x18\x02 \x01(\x0b\x32\x13.vega.ProposalTermsR\x05terms\x12\x35\n\trationale\x18\x03 \x01(\x0b\x32\x17.vega.ProposalRationaleR\trationale"Y\n\x0eVoteSubmission\x12\x1f\n\x0bproposal_id\x18\x01 \x01(\tR\nproposalId\x12&\n\x05value\x18\x02 \x01(\x0e\x32\x10.vega.Vote.ValueR\x05value"E\n\x12\x44\x65legateSubmission\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x16\n\x06\x61mount\x18\x02 \x01(\tR\x06\x61mount"\xe2\x01\n\x14UndelegateSubmission\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x16\n\x06\x61mount\x18\x02 \x01(\tR\x06\x61mount\x12\x45\n\x06method\x18\x03 \x01(\x0e\x32-.vega.commands.v1.UndelegateSubmission.MethodR\x06method"R\n\x06Method\x12\x16\n\x12METHOD_UNSPECIFIED\x10\x00\x12\x0e\n\nMETHOD_NOW\x10\x01\x12\x1a\n\x16METHOD_AT_END_OF_EPOCH\x10\x02"\x04\x08\x03\x10\x03"\xea\x02\n\x08Transfer\x12=\n\x11\x66rom_account_type\x18\x01 \x01(\x0e\x32\x11.vega.AccountTypeR\x0f\x66romAccountType\x12\x0e\n\x02to\x18\x02 \x01(\tR\x02to\x12\x39\n\x0fto_account_type\x18\x03 \x01(\x0e\x32\x11.vega.AccountTypeR\rtoAccountType\x12\x14\n\x05\x61sset\x18\x04 \x01(\tR\x05\x61sset\x12\x16\n\x06\x61mount\x18\x05 \x01(\tR\x06\x61mount\x12\x1c\n\treference\x18\x06 \x01(\tR\treference\x12;\n\x07one_off\x18\x65 \x01(\x0b\x32 .vega.commands.v1.OneOffTransferH\x00R\x06oneOff\x12\x43\n\trecurring\x18\x66 \x01(\x0b\x32#.vega.commands.v1.RecurringTransferH\x00R\trecurringB\x06\n\x04kind"/\n\x0eOneOffTransfer\x12\x1d\n\ndeliver_on\x18\x01 \x01(\x03R\tdeliverOn"\xc1\x01\n\x11RecurringTransfer\x12\x1f\n\x0bstart_epoch\x18\x01 \x01(\x04R\nstartEpoch\x12 \n\tend_epoch\x18\x02 \x01(\x04H\x00R\x08\x65ndEpoch\x88\x01\x01\x12\x16\n\x06\x66\x61\x63tor\x18\x03 \x01(\tR\x06\x66\x61\x63tor\x12\x43\n\x11\x64ispatch_strategy\x18\x04 \x01(\x0b\x32\x16.vega.DispatchStrategyR\x10\x64ispatchStrategyB\x0c\n\n_end_epoch"1\n\x0e\x43\x61ncelTransfer\x12\x1f\n\x0btransfer_id\x18\x01 \x01(\tR\ntransferIdB3Z1code.vegaprotocol.io/vega/protos/vega/commands/v1b\x06proto3'
+    b'\n\x1fvega/commands/v1/commands.proto\x12\x10vega.commands.v1\x1a\x15vega/governance.proto\x1a\x0fvega/vega.proto\x1a)vega/commands/v1/validator_commands.proto"\xeb\x01\n\x17\x42\x61tchMarketInstructions\x12I\n\rcancellations\x18\x01 \x03(\x0b\x32#.vega.commands.v1.OrderCancellationR\rcancellations\x12@\n\namendments\x18\x02 \x03(\x0b\x32 .vega.commands.v1.OrderAmendmentR\namendments\x12\x43\n\x0bsubmissions\x18\x03 \x03(\x0b\x32!.vega.commands.v1.OrderSubmissionR\x0bsubmissions"\xce\x02\n\x0fOrderSubmission\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x14\n\x05price\x18\x02 \x01(\tR\x05price\x12\x12\n\x04size\x18\x03 \x01(\x04R\x04size\x12\x1e\n\x04side\x18\x04 \x01(\x0e\x32\n.vega.SideR\x04side\x12;\n\rtime_in_force\x18\x05 \x01(\x0e\x32\x17.vega.Order.TimeInForceR\x0btimeInForce\x12\x1d\n\nexpires_at\x18\x06 \x01(\x03R\texpiresAt\x12$\n\x04type\x18\x07 \x01(\x0e\x32\x10.vega.Order.TypeR\x04type\x12\x1c\n\treference\x18\x08 \x01(\tR\treference\x12\x34\n\x0cpegged_order\x18\t \x01(\x0b\x32\x11.vega.PeggedOrderR\x0bpeggedOrder"K\n\x11OrderCancellation\x12\x19\n\x08order_id\x18\x01 \x01(\tR\x07orderId\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId"\xe3\x02\n\x0eOrderAmendment\x12\x19\n\x08order_id\x18\x01 \x01(\tR\x07orderId\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x19\n\x05price\x18\x03 \x01(\tH\x00R\x05price\x88\x01\x01\x12\x1d\n\nsize_delta\x18\x04 \x01(\x03R\tsizeDelta\x12"\n\nexpires_at\x18\x05 \x01(\x03H\x01R\texpiresAt\x88\x01\x01\x12;\n\rtime_in_force\x18\x06 \x01(\x0e\x32\x17.vega.Order.TimeInForceR\x0btimeInForce\x12#\n\rpegged_offset\x18\x07 \x01(\tR\x0cpeggedOffset\x12@\n\x10pegged_reference\x18\x08 \x01(\x0e\x32\x15.vega.PeggedReferenceR\x0fpeggedReferenceB\x08\n\x06_priceB\r\n\x0b_expires_at"\xee\x01\n\x1cLiquidityProvisionSubmission\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12+\n\x11\x63ommitment_amount\x18\x02 \x01(\tR\x10\x63ommitmentAmount\x12\x10\n\x03\x66\x65\x65\x18\x03 \x01(\tR\x03\x66\x65\x65\x12*\n\x05sells\x18\x04 \x03(\x0b\x32\x14.vega.LiquidityOrderR\x05sells\x12(\n\x04\x62uys\x18\x05 \x03(\x0b\x32\x14.vega.LiquidityOrderR\x04\x62uys\x12\x1c\n\treference\x18\x06 \x01(\tR\treference"=\n\x1eLiquidityProvisionCancellation\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId"\xed\x01\n\x1bLiquidityProvisionAmendment\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12+\n\x11\x63ommitment_amount\x18\x02 \x01(\tR\x10\x63ommitmentAmount\x12\x10\n\x03\x66\x65\x65\x18\x03 \x01(\tR\x03\x66\x65\x65\x12*\n\x05sells\x18\x04 \x03(\x0b\x32\x14.vega.LiquidityOrderR\x05sells\x12(\n\x04\x62uys\x18\x05 \x03(\x0b\x32\x14.vega.LiquidityOrderR\x04\x62uys\x12\x1c\n\treference\x18\x06 \x01(\tR\treference"g\n\x12WithdrawSubmission\x12\x16\n\x06\x61mount\x18\x01 \x01(\tR\x06\x61mount\x12\x14\n\x05\x61sset\x18\x02 \x01(\tR\x05\x61sset\x12#\n\x03\x65xt\x18\x03 \x01(\x0b\x32\x11.vega.WithdrawExtR\x03\x65xt"\x94\x01\n\x12ProposalSubmission\x12\x1c\n\treference\x18\x01 \x01(\tR\treference\x12)\n\x05terms\x18\x02 \x01(\x0b\x32\x13.vega.ProposalTermsR\x05terms\x12\x35\n\trationale\x18\x03 \x01(\x0b\x32\x17.vega.ProposalRationaleR\trationale"Y\n\x0eVoteSubmission\x12\x1f\n\x0bproposal_id\x18\x01 \x01(\tR\nproposalId\x12&\n\x05value\x18\x02 \x01(\x0e\x32\x10.vega.Vote.ValueR\x05value"E\n\x12\x44\x65legateSubmission\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x16\n\x06\x61mount\x18\x02 \x01(\tR\x06\x61mount"\xe2\x01\n\x14UndelegateSubmission\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x16\n\x06\x61mount\x18\x02 \x01(\tR\x06\x61mount\x12\x45\n\x06method\x18\x03 \x01(\x0e\x32-.vega.commands.v1.UndelegateSubmission.MethodR\x06method"R\n\x06Method\x12\x16\n\x12METHOD_UNSPECIFIED\x10\x00\x12\x0e\n\nMETHOD_NOW\x10\x01\x12\x1a\n\x16METHOD_AT_END_OF_EPOCH\x10\x02"\x04\x08\x03\x10\x03"\xea\x02\n\x08Transfer\x12=\n\x11\x66rom_account_type\x18\x01 \x01(\x0e\x32\x11.vega.AccountTypeR\x0f\x66romAccountType\x12\x0e\n\x02to\x18\x02 \x01(\tR\x02to\x12\x39\n\x0fto_account_type\x18\x03 \x01(\x0e\x32\x11.vega.AccountTypeR\rtoAccountType\x12\x14\n\x05\x61sset\x18\x04 \x01(\tR\x05\x61sset\x12\x16\n\x06\x61mount\x18\x05 \x01(\tR\x06\x61mount\x12\x1c\n\treference\x18\x06 \x01(\tR\treference\x12;\n\x07one_off\x18\x65 \x01(\x0b\x32 .vega.commands.v1.OneOffTransferH\x00R\x06oneOff\x12\x43\n\trecurring\x18\x66 \x01(\x0b\x32#.vega.commands.v1.RecurringTransferH\x00R\trecurringB\x06\n\x04kind"/\n\x0eOneOffTransfer\x12\x1d\n\ndeliver_on\x18\x01 \x01(\x03R\tdeliverOn"\xc1\x01\n\x11RecurringTransfer\x12\x1f\n\x0bstart_epoch\x18\x01 \x01(\x04R\nstartEpoch\x12 \n\tend_epoch\x18\x02 \x01(\x04H\x00R\x08\x65ndEpoch\x88\x01\x01\x12\x16\n\x06\x66\x61\x63tor\x18\x03 \x01(\tR\x06\x66\x61\x63tor\x12\x43\n\x11\x64ispatch_strategy\x18\x04 \x01(\x0b\x32\x16.vega.DispatchStrategyR\x10\x64ispatchStrategyB\x0c\n\n_end_epoch"1\n\x0e\x43\x61ncelTransfer\x12\x1f\n\x0btransfer_id\x18\x01 \x01(\tR\ntransferId"\x94\x01\n\x0fIssueSignatures\x12\x1c\n\tsubmitter\x18\x01 \x01(\tR\tsubmitter\x12\x37\n\x04kind\x18\x02 \x01(\x0e\x32#.vega.commands.v1.NodeSignatureKindR\x04kind\x12*\n\x11validator_node_id\x18\x03 \x01(\tR\x0fvalidatorNodeIdB3Z1code.vegaprotocol.io/vega/protos/vega/commands/v1b\x06proto3'
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(
     DESCRIPTOR, "vega.commands.v1.commands_pb2", globals()
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = (
         b"Z1code.vegaprotocol.io/vega/protos/vega/commands/v1"
     )
-    _BATCHMARKETINSTRUCTIONS._serialized_start = 94
-    _BATCHMARKETINSTRUCTIONS._serialized_end = 329
-    _ORDERSUBMISSION._serialized_start = 332
-    _ORDERSUBMISSION._serialized_end = 666
-    _ORDERCANCELLATION._serialized_start = 668
-    _ORDERCANCELLATION._serialized_end = 743
-    _ORDERAMENDMENT._serialized_start = 746
-    _ORDERAMENDMENT._serialized_end = 1101
-    _LIQUIDITYPROVISIONSUBMISSION._serialized_start = 1104
-    _LIQUIDITYPROVISIONSUBMISSION._serialized_end = 1342
-    _LIQUIDITYPROVISIONCANCELLATION._serialized_start = 1344
-    _LIQUIDITYPROVISIONCANCELLATION._serialized_end = 1405
-    _LIQUIDITYPROVISIONAMENDMENT._serialized_start = 1408
-    _LIQUIDITYPROVISIONAMENDMENT._serialized_end = 1645
-    _WITHDRAWSUBMISSION._serialized_start = 1647
-    _WITHDRAWSUBMISSION._serialized_end = 1750
-    _PROPOSALSUBMISSION._serialized_start = 1753
-    _PROPOSALSUBMISSION._serialized_end = 1901
-    _VOTESUBMISSION._serialized_start = 1903
-    _VOTESUBMISSION._serialized_end = 1992
-    _DELEGATESUBMISSION._serialized_start = 1994
-    _DELEGATESUBMISSION._serialized_end = 2063
-    _UNDELEGATESUBMISSION._serialized_start = 2066
-    _UNDELEGATESUBMISSION._serialized_end = 2292
-    _UNDELEGATESUBMISSION_METHOD._serialized_start = 2210
-    _UNDELEGATESUBMISSION_METHOD._serialized_end = 2292
-    _TRANSFER._serialized_start = 2295
-    _TRANSFER._serialized_end = 2657
-    _ONEOFFTRANSFER._serialized_start = 2659
-    _ONEOFFTRANSFER._serialized_end = 2706
-    _RECURRINGTRANSFER._serialized_start = 2709
-    _RECURRINGTRANSFER._serialized_end = 2902
-    _CANCELTRANSFER._serialized_start = 2904
-    _CANCELTRANSFER._serialized_end = 2953
+    _BATCHMARKETINSTRUCTIONS._serialized_start = 137
+    _BATCHMARKETINSTRUCTIONS._serialized_end = 372
+    _ORDERSUBMISSION._serialized_start = 375
+    _ORDERSUBMISSION._serialized_end = 709
+    _ORDERCANCELLATION._serialized_start = 711
+    _ORDERCANCELLATION._serialized_end = 786
+    _ORDERAMENDMENT._serialized_start = 789
+    _ORDERAMENDMENT._serialized_end = 1144
+    _LIQUIDITYPROVISIONSUBMISSION._serialized_start = 1147
+    _LIQUIDITYPROVISIONSUBMISSION._serialized_end = 1385
+    _LIQUIDITYPROVISIONCANCELLATION._serialized_start = 1387
+    _LIQUIDITYPROVISIONCANCELLATION._serialized_end = 1448
+    _LIQUIDITYPROVISIONAMENDMENT._serialized_start = 1451
+    _LIQUIDITYPROVISIONAMENDMENT._serialized_end = 1688
+    _WITHDRAWSUBMISSION._serialized_start = 1690
+    _WITHDRAWSUBMISSION._serialized_end = 1793
+    _PROPOSALSUBMISSION._serialized_start = 1796
+    _PROPOSALSUBMISSION._serialized_end = 1944
+    _VOTESUBMISSION._serialized_start = 1946
+    _VOTESUBMISSION._serialized_end = 2035
+    _DELEGATESUBMISSION._serialized_start = 2037
+    _DELEGATESUBMISSION._serialized_end = 2106
+    _UNDELEGATESUBMISSION._serialized_start = 2109
+    _UNDELEGATESUBMISSION._serialized_end = 2335
+    _UNDELEGATESUBMISSION_METHOD._serialized_start = 2253
+    _UNDELEGATESUBMISSION_METHOD._serialized_end = 2335
+    _TRANSFER._serialized_start = 2338
+    _TRANSFER._serialized_end = 2700
+    _ONEOFFTRANSFER._serialized_start = 2702
+    _ONEOFFTRANSFER._serialized_end = 2749
+    _RECURRINGTRANSFER._serialized_start = 2752
+    _RECURRINGTRANSFER._serialized_end = 2945
+    _CANCELTRANSFER._serialized_start = 2947
+    _CANCELTRANSFER._serialized_end = 2996
+    _ISSUESIGNATURES._serialized_start = 2999
+    _ISSUESIGNATURES._serialized_end = 3147
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-0.67.0/vega_sim/proto/vega/commands/v1/data_pb2.py` & `vega_sim-1.0.1/vega_sim/proto/vega/commands/v1/data_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(
     DESCRIPTOR, "vega.commands.v1.data_pb2", globals()
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = (
         b"Z1code.vegaprotocol.io/vega/protos/vega/commands/v1"
     )
     _ORACLEDATASUBMISSION._serialized_start = 50
     _ORACLEDATASUBMISSION._serialized_end = 277
     _ORACLEDATASUBMISSION_ORACLESOURCE._serialized_start = 177
```

### Comparing `vega_sim-0.67.0/vega_sim/proto/vega/commands/v1/signature_pb2.py` & `vega_sim-1.0.1/vega_sim/proto/vega/commands/v1/signature_pb2.py`

 * *Files identical despite different names*

```diff
@@ -17,15 +17,14 @@
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(
     DESCRIPTOR, "vega.commands.v1.signature_pb2", globals()
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = (
         b"Z1code.vegaprotocol.io/vega/protos/vega/commands/v1"
     )
     _SIGNATURE._serialized_start = 54
     _SIGNATURE._serialized_end = 133
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-0.67.0/vega_sim/proto/vega/commands/v1/transaction_pb2.py` & `vega_sim-1.0.1/vega_sim/proto/vega/commands/v1/transaction_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(
     DESCRIPTOR, "vega.commands.v1.transaction_pb2", globals()
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = (
         b"Z1code.vegaprotocol.io/vega/protos/vega/commands/v1"
     )
     _TXVERSION._serialized_start = 2876
     _TXVERSION._serialized_end = 2959
     _INPUTDATA._serialized_start = 196
```

### Comparing `vega_sim-0.67.0/vega_sim/proto/vega/commands/v1/validator_commands_pb2.py` & `vega_sim-1.0.1/vega_sim/proto/vega/commands/v1/validator_commands_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,29 +14,28 @@
 
 from ... import vega_pb2 as vega_dot_vega__pb2
 from ... import chain_events_pb2 as vega_dot_chain__events__pb2
 from ...commands.v1 import signature_pb2 as vega_dot_commands_dot_v1_dot_signature__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n)vega/commands/v1/validator_commands.proto\x12\x10vega.commands.v1\x1a\x0fvega/vega.proto\x1a\x17vega/chain_events.proto\x1a vega/commands/v1/signature.proto"\xbd\x01\n\x12ValidatorHeartbeat\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12J\n\x12\x65thereum_signature\x18\x02 \x01(\x0b\x32\x1b.vega.commands.v1.SignatureR\x11\x65thereumSignature\x12\x42\n\x0evega_signature\x18\x03 \x01(\x0b\x32\x1b.vega.commands.v1.SignatureR\rvegaSignature"\x80\x04\n\x0c\x41nnounceNode\x12 \n\x0cvega_pub_key\x18\x01 \x01(\tR\nvegaPubKey\x12)\n\x10\x65thereum_address\x18\x02 \x01(\tR\x0f\x65thereumAddress\x12"\n\rchain_pub_key\x18\x03 \x01(\tR\x0b\x63hainPubKey\x12\x19\n\x08info_url\x18\x04 \x01(\tR\x07infoUrl\x12\x18\n\x07\x63ountry\x18\x05 \x01(\tR\x07\x63ountry\x12\x0e\n\x02id\x18\x06 \x01(\tR\x02id\x12\x12\n\x04name\x18\x07 \x01(\tR\x04name\x12\x1d\n\navatar_url\x18\x08 \x01(\tR\tavatarUrl\x12+\n\x12vega_pub_key_index\x18\t \x01(\rR\x0fvegaPubKeyIndex\x12\x1d\n\nfrom_epoch\x18\n \x01(\x04R\tfromEpoch\x12J\n\x12\x65thereum_signature\x18\x0b \x01(\x0b\x32\x1b.vega.commands.v1.SignatureR\x11\x65thereumSignature\x12\x42\n\x0evega_signature\x18\x0c \x01(\x0b\x32\x1b.vega.commands.v1.SignatureR\rvegaSignature\x12+\n\x11submitter_address\x18\r \x01(\tR\x10submitterAddress"\xc0\x03\n\x08NodeVote\x12\x1c\n\treference\x18\x02 \x01(\tR\treference\x12\x33\n\x04type\x18\x03 \x01(\x0e\x32\x1f.vega.commands.v1.NodeVote.TypeR\x04type"\xda\x02\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x18\n\x14TYPE_STAKE_DEPOSITED\x10\x01\x12\x16\n\x12TYPE_STAKE_REMOVED\x10\x02\x12\x18\n\x14TYPE_FUNDS_DEPOSITED\x10\x03\x12\x15\n\x11TYPE_SIGNER_ADDED\x10\x04\x12\x17\n\x13TYPE_SIGNER_REMOVED\x10\x05\x12\x17\n\x13TYPE_BRIDGE_STOPPED\x10\x06\x12\x17\n\x13TYPE_BRIDGE_RESUMED\x10\x07\x12\x15\n\x11TYPE_ASSET_LISTED\x10\x08\x12\x17\n\x13TYPE_LIMITS_UPDATED\x10\t\x12\x1b\n\x17TYPE_STAKE_TOTAL_SUPPLY\x10\n\x12\x1d\n\x19TYPE_SIGNER_THRESHOLD_SET\x10\x0b\x12"\n\x1eTYPE_GOVERNANCE_VALIDATE_ASSET\x10\x0cJ\x04\x08\x01\x10\x02"j\n\rNodeSignature\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x10\n\x03sig\x18\x02 \x01(\x0cR\x03sig\x12\x37\n\x04kind\x18\x03 \x01(\x0e\x32#.vega.commands.v1.NodeSignatureKindR\x04kind"\xb1\x02\n\nChainEvent\x12\x13\n\x05tx_id\x18\x01 \x01(\tR\x04txId\x12\x14\n\x05nonce\x18\x02 \x01(\x04R\x05nonce\x12\x34\n\x07\x62uiltin\x18\xe9\x07 \x01(\x0b\x32\x17.vega.BuiltinAssetEventH\x00R\x07\x62uiltin\x12)\n\x05\x65rc20\x18\xea\x07 \x01(\x0b\x32\x10.vega.ERC20EventH\x00R\x05\x65rc20\x12:\n\rstaking_event\x18\xed\x07 \x01(\x0b\x32\x12.vega.StakingEventH\x00R\x0cstakingEvent\x12\x42\n\x0e\x65rc20_multisig\x18\xee\x07 \x01(\x0b\x32\x18.vega.ERC20MultiSigEventH\x00R\rerc20MultisigB\x07\n\x05\x65ventJ\x06\x08\xeb\x07\x10\xec\x07J\x06\x08\xec\x07\x10\xed\x07"\xb4\x01\n\x13KeyRotateSubmission\x12)\n\x11new_pub_key_index\x18\x01 \x01(\rR\x0enewPubKeyIndex\x12!\n\x0ctarget_block\x18\x02 \x01(\x04R\x0btargetBlock\x12\x1e\n\x0bnew_pub_key\x18\x03 \x01(\tR\tnewPubKey\x12/\n\x14\x63urrent_pub_key_hash\x18\x04 \x01(\tR\x11\x63urrentPubKeyHash"\x83\x02\n\x1b\x45thereumKeyRotateSubmission\x12!\n\x0ctarget_block\x18\x01 \x01(\x04R\x0btargetBlock\x12\x1f\n\x0bnew_address\x18\x02 \x01(\tR\nnewAddress\x12\'\n\x0f\x63urrent_address\x18\x03 \x01(\tR\x0e\x63urrentAddress\x12+\n\x11submitter_address\x18\x04 \x01(\tR\x10submitterAddress\x12J\n\x12\x65thereum_signature\x18\x05 \x01(\x0b\x32\x1b.vega.commands.v1.SignatureR\x11\x65thereumSignature"M\n\x15StateVariableProposal\x12\x34\n\x08proposal\x18\x01 \x01(\x0b\x32\x18.vega.StateValueProposalR\x08proposal"u\n\x17ProtocolUpgradeProposal\x12\x30\n\x14upgrade_block_height\x18\x01 \x01(\x04R\x12upgradeBlockHeight\x12(\n\x10vega_release_tag\x18\x02 \x01(\tR\x0evegaReleaseTag"\x94\x01\n\x0fIssueSignatures\x12\x1c\n\tsubmitter\x18\x01 \x01(\tR\tsubmitter\x12\x37\n\x04kind\x18\x02 \x01(\x0e\x32#.vega.commands.v1.NodeSignatureKindR\x04kind\x12*\n\x11validator_node_id\x18\x03 \x01(\tR\x0fvalidatorNodeId*\x97\x02\n\x11NodeSignatureKind\x12#\n\x1fNODE_SIGNATURE_KIND_UNSPECIFIED\x10\x00\x12!\n\x1dNODE_SIGNATURE_KIND_ASSET_NEW\x10\x01\x12(\n$NODE_SIGNATURE_KIND_ASSET_WITHDRAWAL\x10\x02\x12\x33\n/NODE_SIGNATURE_KIND_ERC20_MULTISIG_SIGNER_ADDED\x10\x03\x12\x35\n1NODE_SIGNATURE_KIND_ERC20_MULTISIG_SIGNER_REMOVED\x10\x04\x12$\n NODE_SIGNATURE_KIND_ASSET_UPDATE\x10\x05\x42\x33Z1code.vegaprotocol.io/vega/protos/vega/commands/v1b\x06proto3'
+    b'\n)vega/commands/v1/validator_commands.proto\x12\x10vega.commands.v1\x1a\x0fvega/vega.proto\x1a\x17vega/chain_events.proto\x1a vega/commands/v1/signature.proto"\xbd\x01\n\x12ValidatorHeartbeat\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12J\n\x12\x65thereum_signature\x18\x02 \x01(\x0b\x32\x1b.vega.commands.v1.SignatureR\x11\x65thereumSignature\x12\x42\n\x0evega_signature\x18\x03 \x01(\x0b\x32\x1b.vega.commands.v1.SignatureR\rvegaSignature"\x80\x04\n\x0c\x41nnounceNode\x12 \n\x0cvega_pub_key\x18\x01 \x01(\tR\nvegaPubKey\x12)\n\x10\x65thereum_address\x18\x02 \x01(\tR\x0f\x65thereumAddress\x12"\n\rchain_pub_key\x18\x03 \x01(\tR\x0b\x63hainPubKey\x12\x19\n\x08info_url\x18\x04 \x01(\tR\x07infoUrl\x12\x18\n\x07\x63ountry\x18\x05 \x01(\tR\x07\x63ountry\x12\x0e\n\x02id\x18\x06 \x01(\tR\x02id\x12\x12\n\x04name\x18\x07 \x01(\tR\x04name\x12\x1d\n\navatar_url\x18\x08 \x01(\tR\tavatarUrl\x12+\n\x12vega_pub_key_index\x18\t \x01(\rR\x0fvegaPubKeyIndex\x12\x1d\n\nfrom_epoch\x18\n \x01(\x04R\tfromEpoch\x12J\n\x12\x65thereum_signature\x18\x0b \x01(\x0b\x32\x1b.vega.commands.v1.SignatureR\x11\x65thereumSignature\x12\x42\n\x0evega_signature\x18\x0c \x01(\x0b\x32\x1b.vega.commands.v1.SignatureR\rvegaSignature\x12+\n\x11submitter_address\x18\r \x01(\tR\x10submitterAddress"\xc0\x03\n\x08NodeVote\x12\x1c\n\treference\x18\x02 \x01(\tR\treference\x12\x33\n\x04type\x18\x03 \x01(\x0e\x32\x1f.vega.commands.v1.NodeVote.TypeR\x04type"\xda\x02\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x18\n\x14TYPE_STAKE_DEPOSITED\x10\x01\x12\x16\n\x12TYPE_STAKE_REMOVED\x10\x02\x12\x18\n\x14TYPE_FUNDS_DEPOSITED\x10\x03\x12\x15\n\x11TYPE_SIGNER_ADDED\x10\x04\x12\x17\n\x13TYPE_SIGNER_REMOVED\x10\x05\x12\x17\n\x13TYPE_BRIDGE_STOPPED\x10\x06\x12\x17\n\x13TYPE_BRIDGE_RESUMED\x10\x07\x12\x15\n\x11TYPE_ASSET_LISTED\x10\x08\x12\x17\n\x13TYPE_LIMITS_UPDATED\x10\t\x12\x1b\n\x17TYPE_STAKE_TOTAL_SUPPLY\x10\n\x12\x1d\n\x19TYPE_SIGNER_THRESHOLD_SET\x10\x0b\x12"\n\x1eTYPE_GOVERNANCE_VALIDATE_ASSET\x10\x0cJ\x04\x08\x01\x10\x02"j\n\rNodeSignature\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x10\n\x03sig\x18\x02 \x01(\x0cR\x03sig\x12\x37\n\x04kind\x18\x03 \x01(\x0e\x32#.vega.commands.v1.NodeSignatureKindR\x04kind"\xb1\x02\n\nChainEvent\x12\x13\n\x05tx_id\x18\x01 \x01(\tR\x04txId\x12\x14\n\x05nonce\x18\x02 \x01(\x04R\x05nonce\x12\x34\n\x07\x62uiltin\x18\xe9\x07 \x01(\x0b\x32\x17.vega.BuiltinAssetEventH\x00R\x07\x62uiltin\x12)\n\x05\x65rc20\x18\xea\x07 \x01(\x0b\x32\x10.vega.ERC20EventH\x00R\x05\x65rc20\x12:\n\rstaking_event\x18\xed\x07 \x01(\x0b\x32\x12.vega.StakingEventH\x00R\x0cstakingEvent\x12\x42\n\x0e\x65rc20_multisig\x18\xee\x07 \x01(\x0b\x32\x18.vega.ERC20MultiSigEventH\x00R\rerc20MultisigB\x07\n\x05\x65ventJ\x06\x08\xeb\x07\x10\xec\x07J\x06\x08\xec\x07\x10\xed\x07"\xb4\x01\n\x13KeyRotateSubmission\x12)\n\x11new_pub_key_index\x18\x01 \x01(\rR\x0enewPubKeyIndex\x12!\n\x0ctarget_block\x18\x02 \x01(\x04R\x0btargetBlock\x12\x1e\n\x0bnew_pub_key\x18\x03 \x01(\tR\tnewPubKey\x12/\n\x14\x63urrent_pub_key_hash\x18\x04 \x01(\tR\x11\x63urrentPubKeyHash"\x83\x02\n\x1b\x45thereumKeyRotateSubmission\x12!\n\x0ctarget_block\x18\x01 \x01(\x04R\x0btargetBlock\x12\x1f\n\x0bnew_address\x18\x02 \x01(\tR\nnewAddress\x12\'\n\x0f\x63urrent_address\x18\x03 \x01(\tR\x0e\x63urrentAddress\x12+\n\x11submitter_address\x18\x04 \x01(\tR\x10submitterAddress\x12J\n\x12\x65thereum_signature\x18\x05 \x01(\x0b\x32\x1b.vega.commands.v1.SignatureR\x11\x65thereumSignature"M\n\x15StateVariableProposal\x12\x34\n\x08proposal\x18\x01 \x01(\x0b\x32\x18.vega.StateValueProposalR\x08proposal"u\n\x17ProtocolUpgradeProposal\x12\x30\n\x14upgrade_block_height\x18\x01 \x01(\x04R\x12upgradeBlockHeight\x12(\n\x10vega_release_tag\x18\x02 \x01(\tR\x0evegaReleaseTag*\x97\x02\n\x11NodeSignatureKind\x12#\n\x1fNODE_SIGNATURE_KIND_UNSPECIFIED\x10\x00\x12!\n\x1dNODE_SIGNATURE_KIND_ASSET_NEW\x10\x01\x12(\n$NODE_SIGNATURE_KIND_ASSET_WITHDRAWAL\x10\x02\x12\x33\n/NODE_SIGNATURE_KIND_ERC20_MULTISIG_SIGNER_ADDED\x10\x03\x12\x35\n1NODE_SIGNATURE_KIND_ERC20_MULTISIG_SIGNER_REMOVED\x10\x04\x12$\n NODE_SIGNATURE_KIND_ASSET_UPDATE\x10\x05\x42\x33Z1code.vegaprotocol.io/vega/protos/vega/commands/v1b\x06proto3'
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(
     DESCRIPTOR, "vega.commands.v1.validator_commands_pb2", globals()
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = (
         b"Z1code.vegaprotocol.io/vega/protos/vega/commands/v1"
     )
-    _NODESIGNATUREKIND._serialized_start = 2508
-    _NODESIGNATUREKIND._serialized_end = 2787
+    _NODESIGNATUREKIND._serialized_start = 2357
+    _NODESIGNATUREKIND._serialized_end = 2636
     _VALIDATORHEARTBEAT._serialized_start = 140
     _VALIDATORHEARTBEAT._serialized_end = 329
     _ANNOUNCENODE._serialized_start = 332
     _ANNOUNCENODE._serialized_end = 844
     _NODEVOTE._serialized_start = 847
     _NODEVOTE._serialized_end = 1295
     _NODEVOTE_TYPE._serialized_start = 943
@@ -49,10 +48,8 @@
     _KEYROTATESUBMISSION._serialized_end = 1894
     _ETHEREUMKEYROTATESUBMISSION._serialized_start = 1897
     _ETHEREUMKEYROTATESUBMISSION._serialized_end = 2156
     _STATEVARIABLEPROPOSAL._serialized_start = 2158
     _STATEVARIABLEPROPOSAL._serialized_end = 2235
     _PROTOCOLUPGRADEPROPOSAL._serialized_start = 2237
     _PROTOCOLUPGRADEPROPOSAL._serialized_end = 2354
-    _ISSUESIGNATURES._serialized_start = 2357
-    _ISSUESIGNATURES._serialized_end = 2505
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-0.67.0/vega_sim/proto/vega/data/v1/data_pb2.py` & `vega_sim-1.0.1/vega_sim/proto/vega/data/v1/data_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
     b'\n\x17vega/data/v1/data.proto\x12\x0cvega.data.v1"&\n\nETHAddress\x12\x18\n\x07\x61\x64\x64ress\x18\x01 \x01(\tR\x07\x61\x64\x64ress"\x1a\n\x06PubKey\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key"\x80\x01\n\x06Signer\x12/\n\x07pub_key\x18\x01 \x01(\x0b\x32\x14.vega.data.v1.PubKeyH\x00R\x06pubKey\x12;\n\x0b\x65th_address\x18\x02 \x01(\x0b\x32\x18.vega.data.v1.ETHAddressH\x00R\nethAddressB\x08\n\x06signer"\x87\x01\n\x08Property\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value\x12\x37\n\x15number_decimal_places\x18\x03 \x01(\x04H\x00R\x13numberDecimalPlaces\x88\x01\x01\x42\x18\n\x16_number_decimal_places"\xaf\x01\n\x04\x44\x61ta\x12.\n\x07signers\x18\x01 \x03(\x0b\x32\x14.vega.data.v1.SignerR\x07signers\x12*\n\x04\x64\x61ta\x18\x02 \x03(\x0b\x32\x16.vega.data.v1.PropertyR\x04\x64\x61ta\x12(\n\x10matched_spec_ids\x18\x03 \x03(\tR\x0ematchedSpecIds\x12!\n\x0c\x62roadcast_at\x18\x04 \x01(\x03R\x0b\x62roadcastAt"6\n\x0c\x45xternalData\x12&\n\x04\x64\x61ta\x18\x01 \x01(\x0b\x32\x12.vega.data.v1.DataR\x04\x64\x61taB/Z-code.vegaprotocol.io/vega/protos/vega/data/v1b\x06proto3'
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "vega.data.v1.data_pb2", globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b"Z-code.vegaprotocol.io/vega/protos/vega/data/v1"
     _ETHADDRESS._serialized_start = 41
     _ETHADDRESS._serialized_end = 79
     _PUBKEY._serialized_start = 81
     _PUBKEY._serialized_end = 107
     _SIGNER._serialized_start = 110
```

### Comparing `vega_sim-0.67.0/vega_sim/proto/vega/data/v1/spec_pb2.py` & `vega_sim-1.0.1/vega_sim/proto/vega/data/v1/spec_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
     b'\n\x17vega/data/v1/spec.proto\x12\x0cvega.data.v1"n\n\x06\x46ilter\x12+\n\x03key\x18\x01 \x01(\x0b\x32\x19.vega.data.v1.PropertyKeyR\x03key\x12\x37\n\nconditions\x18\x02 \x03(\x0b\x32\x17.vega.data.v1.ConditionR\nconditions"\xb2\x02\n\x0bPropertyKey\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x32\n\x04type\x18\x02 \x01(\x0e\x32\x1e.vega.data.v1.PropertyKey.TypeR\x04type\x12\x37\n\x15number_decimal_places\x18\x03 \x01(\x04H\x00R\x13numberDecimalPlaces\x88\x01\x01"\x87\x01\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0e\n\nTYPE_EMPTY\x10\x01\x12\x10\n\x0cTYPE_INTEGER\x10\x02\x12\x0f\n\x0bTYPE_STRING\x10\x03\x12\x10\n\x0cTYPE_BOOLEAN\x10\x04\x12\x10\n\x0cTYPE_DECIMAL\x10\x05\x12\x12\n\x0eTYPE_TIMESTAMP\x10\x06\x42\x18\n\x16_number_decimal_places"\x93\x02\n\tCondition\x12<\n\x08operator\x18\x01 \x01(\x0e\x32 .vega.data.v1.Condition.OperatorR\x08operator\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value"\xb1\x01\n\x08Operator\x12\x18\n\x14OPERATOR_UNSPECIFIED\x10\x00\x12\x13\n\x0fOPERATOR_EQUALS\x10\x01\x12\x19\n\x15OPERATOR_GREATER_THAN\x10\x02\x12"\n\x1eOPERATOR_GREATER_THAN_OR_EQUAL\x10\x03\x12\x16\n\x12OPERATOR_LESS_THAN\x10\x04\x12\x1f\n\x1bOPERATOR_LESS_THAN_OR_EQUAL\x10\x05\x42/Z-code.vegaprotocol.io/vega/protos/vega/data/v1b\x06proto3'
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "vega.data.v1.spec_pb2", globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b"Z-code.vegaprotocol.io/vega/protos/vega/data/v1"
     _FILTER._serialized_start = 41
     _FILTER._serialized_end = 151
     _PROPERTYKEY._serialized_start = 154
     _PROPERTYKEY._serialized_end = 460
     _PROPERTYKEY_TYPE._serialized_start = 299
```

### Comparing `vega_sim-0.67.0/vega_sim/proto/vega/data_source_pb2.py` & `vega_sim-1.0.1/vega_sim/proto/vega/data_source_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
     b'\n\x16vega/data_source.proto\x12\x04vega\x1a\x17vega/data/v1/spec.proto\x1a\x17vega/data/v1/data.proto"\xa9\x01\n\x14\x44\x61taSourceDefinition\x12@\n\x08internal\x18\x01 \x01(\x0b\x32".vega.DataSourceDefinitionInternalH\x00R\x08internal\x12@\n\x08\x65xternal\x18\x02 \x01(\x0b\x32".vega.DataSourceDefinitionExternalH\x00R\x08\x65xternalB\r\n\x0bsource_type"Z\n\x1f\x44\x61taSourceSpecConfigurationTime\x12\x37\n\nconditions\x18\x01 \x03(\x0b\x32\x17.vega.data.v1.ConditionR\nconditions"j\n\x1c\x44\x61taSourceDefinitionInternal\x12;\n\x04time\x18\x01 \x01(\x0b\x32%.vega.DataSourceSpecConfigurationTimeH\x00R\x04timeB\r\n\x0bsource_type"j\n\x1c\x44\x61taSourceDefinitionExternal\x12;\n\x06oracle\x18\x01 \x01(\x0b\x32!.vega.DataSourceSpecConfigurationH\x00R\x06oracleB\r\n\x0bsource_type"}\n\x1b\x44\x61taSourceSpecConfiguration\x12.\n\x07signers\x18\x01 \x03(\x0b\x32\x14.vega.data.v1.SignerR\x07signers\x12.\n\x07\x66ilters\x18\x02 \x03(\x0b\x32\x14.vega.data.v1.FilterR\x07\x66ilters"\x90\x02\n\x0e\x44\x61taSourceSpec\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1d\n\ncreated_at\x18\x02 \x01(\x03R\tcreatedAt\x12\x1d\n\nupdated_at\x18\x03 \x01(\x03R\tupdatedAt\x12.\n\x04\x64\x61ta\x18\x04 \x01(\x0b\x32\x1a.vega.DataSourceDefinitionR\x04\x64\x61ta\x12\x33\n\x06status\x18\x05 \x01(\x0e\x32\x1b.vega.DataSourceSpec.StatusR\x06status"K\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x11\n\rSTATUS_ACTIVE\x10\x01\x12\x16\n\x12STATUS_DEACTIVATED\x10\x02"B\n\x16\x45xternalDataSourceSpec\x12(\n\x04spec\x18\x01 \x01(\x0b\x32\x14.vega.DataSourceSpecR\x04specB\'Z%code.vegaprotocol.io/vega/protos/vegab\x06proto3'
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "vega.data_source_pb2", globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b"Z%code.vegaprotocol.io/vega/protos/vega"
     _DATASOURCEDEFINITION._serialized_start = 83
     _DATASOURCEDEFINITION._serialized_end = 252
     _DATASOURCESPECCONFIGURATIONTIME._serialized_start = 254
     _DATASOURCESPECCONFIGURATIONTIME._serialized_end = 344
     _DATASOURCEDEFINITIONINTERNAL._serialized_start = 346
```

### Comparing `vega_sim-0.67.0/vega_sim/proto/vega/events/v1/events_pb2.py` & `vega_sim-1.0.1/vega_sim/proto/vega/events/v1/events_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,31 +21,30 @@
 from ...commands.v1 import data_pb2 as vega_dot_commands_dot_v1_dot_data__pb2
 from ...commands.v1 import (
     validator_commands_pb2 as vega_dot_commands_dot_v1_dot_validator__commands__pb2,
 )
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x1bvega/events/v1/events.proto\x12\x0evega.events.v1\x1a\x12vega/markets.proto\x1a\x11vega/assets.proto\x1a\x15vega/governance.proto\x1a\x0fvega/vega.proto\x1a\x11vega/oracle.proto\x1a\x1fvega/commands/v1/commands.proto\x1a\x1bvega/commands/v1/data.proto\x1a)vega/commands/v1/validator_commands.proto"\xee\x01\n\x18\x45RC20MultiSigSignerAdded\x12!\n\x0csignature_id\x18\x01 \x01(\tR\x0bsignatureId\x12!\n\x0cvalidator_id\x18\x02 \x01(\tR\x0bvalidatorId\x12\x1c\n\ttimestamp\x18\x03 \x01(\x03R\ttimestamp\x12\x1d\n\nnew_signer\x18\x04 \x01(\tR\tnewSigner\x12\x1c\n\tsubmitter\x18\x05 \x01(\tR\tsubmitter\x12\x14\n\x05nonce\x18\x06 \x01(\tR\x05nonce\x12\x1b\n\tepoch_seq\x18\x07 \x01(\tR\x08\x65pochSeq"f\n#ERC20MultiSigSignerRemovedSubmitter\x12!\n\x0csignature_id\x18\x01 \x01(\tR\x0bsignatureId\x12\x1c\n\tsubmitter\x18\x02 \x01(\tR\tsubmitter"\x97\x02\n\x1a\x45RC20MultiSigSignerRemoved\x12\x66\n\x14signature_submitters\x18\x01 \x03(\x0b\x32\x33.vega.events.v1.ERC20MultiSigSignerRemovedSubmitterR\x13signatureSubmitters\x12!\n\x0cvalidator_id\x18\x02 \x01(\tR\x0bvalidatorId\x12\x1c\n\ttimestamp\x18\x03 \x01(\x03R\ttimestamp\x12\x1d\n\nold_signer\x18\x04 \x01(\tR\toldSigner\x12\x14\n\x05nonce\x18\x05 \x01(\tR\x05nonce\x12\x1b\n\tepoch_seq\x18\x06 \x01(\tR\x08\x65pochSeq"\x90\x05\n\x08Transfer\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04\x66rom\x18\x02 \x01(\tR\x04\x66rom\x12=\n\x11\x66rom_account_type\x18\x03 \x01(\x0e\x32\x11.vega.AccountTypeR\x0f\x66romAccountType\x12\x0e\n\x02to\x18\x04 \x01(\tR\x02to\x12\x39\n\x0fto_account_type\x18\x05 \x01(\x0e\x32\x11.vega.AccountTypeR\rtoAccountType\x12\x14\n\x05\x61sset\x18\x06 \x01(\tR\x05\x61sset\x12\x16\n\x06\x61mount\x18\x07 \x01(\tR\x06\x61mount\x12\x1c\n\treference\x18\x08 \x01(\tR\treference\x12\x37\n\x06status\x18\t \x01(\x0e\x32\x1f.vega.events.v1.Transfer.StatusR\x06status\x12\x1c\n\ttimestamp\x18\n \x01(\x03R\ttimestamp\x12\x1b\n\x06reason\x18\x0b \x01(\tH\x01R\x06reason\x88\x01\x01\x12\x39\n\x07one_off\x18\x65 \x01(\x0b\x32\x1e.vega.events.v1.OneOffTransferH\x00R\x06oneOff\x12\x41\n\trecurring\x18\x66 \x01(\x0b\x32!.vega.events.v1.RecurringTransferH\x00R\trecurring"\x84\x01\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x12\n\x0eSTATUS_PENDING\x10\x01\x12\x0f\n\x0bSTATUS_DONE\x10\x02\x12\x13\n\x0fSTATUS_REJECTED\x10\x03\x12\x12\n\x0eSTATUS_STOPPED\x10\x04\x12\x14\n\x10STATUS_CANCELLED\x10\x05\x42\x06\n\x04kindB\t\n\x07_reason"/\n\x0eOneOffTransfer\x12\x1d\n\ndeliver_on\x18\x01 \x01(\x03R\tdeliverOn"\xc1\x01\n\x11RecurringTransfer\x12\x1f\n\x0bstart_epoch\x18\x01 \x01(\x04R\nstartEpoch\x12 \n\tend_epoch\x18\x02 \x01(\x04H\x00R\x08\x65ndEpoch\x88\x01\x01\x12\x16\n\x06\x66\x61\x63tor\x18\x03 \x01(\tR\x06\x66\x61\x63tor\x12\x43\n\x11\x64ispatch_strategy\x18\x04 \x01(\x0b\x32\x16.vega.DispatchStrategyR\x10\x64ispatchStrategyB\x0c\n\n_end_epoch"\xb4\x04\n\x0cStakeLinking\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x35\n\x04type\x18\x02 \x01(\x0e\x32!.vega.events.v1.StakeLinking.TypeR\x04type\x12\x0e\n\x02ts\x18\x03 \x01(\x03R\x02ts\x12\x14\n\x05party\x18\x04 \x01(\tR\x05party\x12\x16\n\x06\x61mount\x18\x05 \x01(\tR\x06\x61mount\x12;\n\x06status\x18\x06 \x01(\x0e\x32#.vega.events.v1.StakeLinking.StatusR\x06status\x12!\n\x0c\x66inalized_at\x18\x07 \x01(\x03R\x0b\x66inalizedAt\x12\x17\n\x07tx_hash\x18\x08 \x01(\tR\x06txHash\x12!\n\x0c\x62lock_height\x18\t \x01(\x04R\x0b\x62lockHeight\x12\x1d\n\nblock_time\x18\n \x01(\x03R\tblockTime\x12\x1b\n\tlog_index\x18\x0b \x01(\x04R\x08logIndex\x12)\n\x10\x65thereum_address\x18\x0c \x01(\tR\x0f\x65thereumAddress"<\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\r\n\tTYPE_LINK\x10\x01\x12\x0f\n\x0bTYPE_UNLINK\x10\x02"^\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x12\n\x0eSTATUS_PENDING\x10\x01\x12\x13\n\x0fSTATUS_ACCEPTED\x10\x02\x12\x13\n\x0fSTATUS_REJECTED\x10\x03"\xd3\x02\n\x18\x45RC20MultiSigSignerEvent\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x41\n\x04type\x18\x02 \x01(\x0e\x32-.vega.events.v1.ERC20MultiSigSignerEvent.TypeR\x04type\x12\x16\n\x06signer\x18\x03 \x01(\tR\x06signer\x12\x14\n\x05nonce\x18\x04 \x01(\tR\x05nonce\x12\x1d\n\nblock_time\x18\x05 \x01(\x03R\tblockTime\x12\x17\n\x07tx_hash\x18\x06 \x01(\tR\x06txHash\x12\x1b\n\tlog_index\x18\x07 \x01(\x04R\x08logIndex\x12!\n\x0c\x62lock_number\x18\x08 \x01(\x04R\x0b\x62lockNumber">\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0e\n\nTYPE_ADDED\x10\x01\x12\x10\n\x0cTYPE_REMOVED\x10\x02"\xe3\x01\n\x1e\x45RC20MultiSigThresholdSetEvent\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12#\n\rnew_threshold\x18\x02 \x01(\rR\x0cnewThreshold\x12\x14\n\x05nonce\x18\x03 \x01(\tR\x05nonce\x12\x1d\n\nblock_time\x18\x04 \x01(\x03R\tblockTime\x12\x17\n\x07tx_hash\x18\x05 \x01(\tR\x06txHash\x12\x1b\n\tlog_index\x18\x06 \x01(\x04R\x08logIndex\x12!\n\x0c\x62lock_number\x18\x07 \x01(\x04R\x0b\x62lockNumber"g\n\x0f\x43heckpointEvent\x12\x12\n\x04hash\x18\x01 \x01(\tR\x04hash\x12\x1d\n\nblock_hash\x18\x02 \x01(\tR\tblockHash\x12!\n\x0c\x62lock_height\x18\x03 \x01(\x04R\x0b\x62lockHeight"-\n\x10StreamStartEvent\x12\x19\n\x08\x63hain_id\x18\x01 \x01(\tR\x07\x63hainId"\x82\x02\n\x11RewardPayoutEvent\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x1b\n\tepoch_seq\x18\x02 \x01(\tR\x08\x65pochSeq\x12\x14\n\x05\x61sset\x18\x03 \x01(\tR\x05\x61sset\x12\x16\n\x06\x61mount\x18\x04 \x01(\tR\x06\x61mount\x12\x35\n\x17percent_of_total_reward\x18\x05 \x01(\tR\x14percentOfTotalReward\x12\x1c\n\ttimestamp\x18\x06 \x01(\x03R\ttimestamp\x12\x1f\n\x0breward_type\x18\x07 \x01(\tR\nrewardType\x12\x16\n\x06market\x18\x08 \x01(\tR\x06market"\xd6\x02\n\x13ValidatorScoreEvent\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1b\n\tepoch_seq\x18\x02 \x01(\tR\x08\x65pochSeq\x12\'\n\x0fvalidator_score\x18\x03 \x01(\tR\x0evalidatorScore\x12)\n\x10normalised_score\x18\x04 \x01(\tR\x0fnormalisedScore\x12\x33\n\x15validator_performance\x18\x05 \x01(\tR\x14validatorPerformance\x12.\n\x13raw_validator_score\x18\x06 \x01(\tR\x11rawValidatorScore\x12)\n\x10validator_status\x18\x07 \x01(\tR\x0fvalidatorStatus\x12%\n\x0emultisig_score\x18\x08 \x01(\tR\rmultisigScore"|\n\x16\x44\x65legationBalanceEvent\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x17\n\x07node_id\x18\x02 \x01(\tR\x06nodeId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x1b\n\tepoch_seq\x18\x04 \x01(\tR\x08\x65pochSeq"D\n\x0bMarketEvent\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x18\n\x07payload\x18\x02 \x01(\tR\x07payload"\xed\x10\n\x11TransactionResult\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x16\n\x06status\x18\x02 \x01(\x08R\x06status\x12\x12\n\x04hash\x18\x03 \x01(\tR\x04hash\x12N\n\x10order_submission\x18\x65 \x01(\x0b\x32!.vega.commands.v1.OrderSubmissionH\x00R\x0forderSubmission\x12K\n\x0forder_amendment\x18\x66 \x01(\x0b\x32 .vega.commands.v1.OrderAmendmentH\x00R\x0eorderAmendment\x12T\n\x12order_cancellation\x18g \x01(\x0b\x32#.vega.commands.v1.OrderCancellationH\x00R\x11orderCancellation\x12\x42\n\x08proposal\x18h \x01(\x0b\x32$.vega.commands.v1.ProposalSubmissionH\x00R\x08proposal\x12K\n\x0fvote_submission\x18i \x01(\x0b\x32 .vega.commands.v1.VoteSubmissionH\x00R\x0evoteSubmission\x12v\n\x1eliquidity_provision_submission\x18j \x01(\x0b\x32..vega.commands.v1.LiquidityProvisionSubmissionH\x00R\x1cliquidityProvisionSubmission\x12W\n\x13withdraw_submission\x18k \x01(\x0b\x32$.vega.commands.v1.WithdrawSubmissionH\x00R\x12withdrawSubmission\x12W\n\x13\x64\x65legate_submission\x18l \x01(\x0b\x32$.vega.commands.v1.DelegateSubmissionH\x00R\x12\x64\x65legateSubmission\x12]\n\x15undelegate_submission\x18m \x01(\x0b\x32&.vega.commands.v1.UndelegateSubmissionH\x00R\x14undelegateSubmission\x12|\n liquidity_provision_cancellation\x18o \x01(\x0b\x32\x30.vega.commands.v1.LiquidityProvisionCancellationH\x00R\x1eliquidityProvisionCancellation\x12s\n\x1dliquidity_provision_amendment\x18p \x01(\x0b\x32-.vega.commands.v1.LiquidityProvisionAmendmentH\x00R\x1bliquidityProvisionAmendment\x12\x38\n\x08transfer\x18q \x01(\x0b\x32\x1a.vega.commands.v1.TransferH\x00R\x08transfer\x12K\n\x0f\x63\x61ncel_transfer\x18r \x01(\x0b\x32 .vega.commands.v1.CancelTransferH\x00R\x0e\x63\x61ncelTransfer\x12\x45\n\rannounce_node\x18s \x01(\x0b\x32\x1e.vega.commands.v1.AnnounceNodeH\x00R\x0c\x61nnounceNode\x12^\n\x16oracle_data_submission\x18t \x01(\x0b\x32&.vega.commands.v1.OracleDataSubmissionH\x00R\x14oracleDataSubmission\x12g\n\x19protocol_upgrade_proposal\x18u \x01(\x0b\x32).vega.commands.v1.ProtocolUpgradeProposalH\x00R\x17protocolUpgradeProposal\x12N\n\x10issue_signatures\x18v \x01(\x0b\x32!.vega.commands.v1.IssueSignaturesH\x00R\x0fissueSignatures\x12g\n\x19\x62\x61tch_market_instructions\x18w \x01(\x0b\x32).vega.commands.v1.BatchMarketInstructionsH\x00R\x17\x62\x61tchMarketInstructions\x12[\n\x15key_rotate_submission\x18x \x01(\x0b\x32%.vega.commands.v1.KeyRotateSubmissionH\x00R\x13keyRotateSubmission\x12t\n\x1e\x65thereum_key_rotate_submission\x18y \x01(\x0b\x32-.vega.commands.v1.EthereumKeyRotateSubmissionH\x00R\x1b\x65thereumKeyRotateSubmission\x12M\n\x07success\x18\xe9\x07 \x01(\x0b\x32\x30.vega.events.v1.TransactionResult.SuccessDetailsH\x01R\x07success\x12M\n\x07\x66\x61ilure\x18\xea\x07 \x01(\x0b\x32\x30.vega.events.v1.TransactionResult.FailureDetailsH\x01R\x07\x66\x61ilure\x1a\x10\n\x0eSuccessDetails\x1a&\n\x0e\x46\x61ilureDetails\x12\x14\n\x05\x65rror\x18\x01 \x01(\tR\x05\x65rrorB\r\n\x0btransactionB\x07\n\x05\x65xtra"\xa7\r\n\x0cTxErrorEvent\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x17\n\x07\x65rr_msg\x18\x02 \x01(\tR\x06\x65rrMsg\x12N\n\x10order_submission\x18\x65 \x01(\x0b\x32!.vega.commands.v1.OrderSubmissionH\x00R\x0forderSubmission\x12K\n\x0forder_amendment\x18\x66 \x01(\x0b\x32 .vega.commands.v1.OrderAmendmentH\x00R\x0eorderAmendment\x12T\n\x12order_cancellation\x18g \x01(\x0b\x32#.vega.commands.v1.OrderCancellationH\x00R\x11orderCancellation\x12\x42\n\x08proposal\x18h \x01(\x0b\x32$.vega.commands.v1.ProposalSubmissionH\x00R\x08proposal\x12K\n\x0fvote_submission\x18i \x01(\x0b\x32 .vega.commands.v1.VoteSubmissionH\x00R\x0evoteSubmission\x12v\n\x1eliquidity_provision_submission\x18j \x01(\x0b\x32..vega.commands.v1.LiquidityProvisionSubmissionH\x00R\x1cliquidityProvisionSubmission\x12W\n\x13withdraw_submission\x18k \x01(\x0b\x32$.vega.commands.v1.WithdrawSubmissionH\x00R\x12withdrawSubmission\x12W\n\x13\x64\x65legate_submission\x18l \x01(\x0b\x32$.vega.commands.v1.DelegateSubmissionH\x00R\x12\x64\x65legateSubmission\x12]\n\x15undelegate_submission\x18m \x01(\x0b\x32&.vega.commands.v1.UndelegateSubmissionH\x00R\x14undelegateSubmission\x12|\n liquidity_provision_cancellation\x18o \x01(\x0b\x32\x30.vega.commands.v1.LiquidityProvisionCancellationH\x00R\x1eliquidityProvisionCancellation\x12s\n\x1dliquidity_provision_amendment\x18p \x01(\x0b\x32-.vega.commands.v1.LiquidityProvisionAmendmentH\x00R\x1bliquidityProvisionAmendment\x12\x38\n\x08transfer\x18q \x01(\x0b\x32\x1a.vega.commands.v1.TransferH\x00R\x08transfer\x12K\n\x0f\x63\x61ncel_transfer\x18r \x01(\x0b\x32 .vega.commands.v1.CancelTransferH\x00R\x0e\x63\x61ncelTransfer\x12\x45\n\rannounce_node\x18s \x01(\x0b\x32\x1e.vega.commands.v1.AnnounceNodeH\x00R\x0c\x61nnounceNode\x12^\n\x16oracle_data_submission\x18t \x01(\x0b\x32&.vega.commands.v1.OracleDataSubmissionH\x00R\x14oracleDataSubmission\x12g\n\x19protocol_upgrade_proposal\x18u \x01(\x0b\x32).vega.commands.v1.ProtocolUpgradeProposalH\x00R\x17protocolUpgradeProposal\x12N\n\x10issue_signatures\x18v \x01(\x0b\x32!.vega.commands.v1.IssueSignaturesH\x00R\x0fissueSignatures\x12g\n\x19\x62\x61tch_market_instructions\x18w \x01(\x0b\x32).vega.commands.v1.BatchMarketInstructionsH\x00R\x17\x62\x61tchMarketInstructionsB\r\n\x0btransactionJ\x04\x08n\x10o"*\n\nTimeUpdate\x12\x1c\n\ttimestamp\x18\x01 \x01(\x03R\ttimestamp"\xa4\x01\n\nEpochEvent\x12\x10\n\x03seq\x18\x01 \x01(\x04R\x03seq\x12)\n\x06\x61\x63tion\x18\x02 \x01(\x0e\x32\x11.vega.EpochActionR\x06\x61\x63tion\x12\x1d\n\nstart_time\x18\x03 \x01(\x03R\tstartTime\x12\x1f\n\x0b\x65xpire_time\x18\x04 \x01(\x03R\nexpireTime\x12\x19\n\x08\x65nd_time\x18\x05 \x01(\x03R\x07\x65ndTime"R\n\x0fLedgerMovements\x12?\n\x10ledger_movements\x18\x01 \x03(\x0b\x32\x14.vega.LedgerMovementR\x0fledgerMovements"\x88\x01\n\x12PositionResolution\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x1e\n\ndistressed\x18\x02 \x01(\x03R\ndistressed\x12\x16\n\x06\x63losed\x18\x03 \x01(\x03R\x06\x63losed\x12\x1d\n\nmark_price\x18\x04 \x01(\tR\tmarkPrice"c\n\x11LossSocialization\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount"^\n\x0fTradeSettlement\x12\x12\n\x04size\x18\x01 \x01(\x03R\x04size\x12\x14\n\x05price\x18\x02 \x01(\tR\x05price\x12!\n\x0cmarket_price\x18\x03 \x01(\tR\x0bmarketPrice"\xd5\x01\n\x0eSettlePosition\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x14\n\x05price\x18\x03 \x01(\tR\x05price\x12L\n\x11trade_settlements\x18\x04 \x03(\x0b\x32\x1f.vega.events.v1.TradeSettlementR\x10tradeSettlements\x12\'\n\x0fposition_factor\x18\x05 \x01(\tR\x0epositionFactor"j\n\x0cSettleMarket\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x14\n\x05price\x18\x02 \x01(\tR\x05price\x12\'\n\x0fposition_factor\x18\x03 \x01(\tR\x0epositionFactor"\xf6\x01\n\x12PositionStateEvent\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x12\n\x04size\x18\x03 \x01(\x03R\x04size\x12%\n\x0epotential_buys\x18\x04 \x01(\x03R\rpotentialBuys\x12\'\n\x0fpotential_sells\x18\x05 \x01(\x03R\x0epotentialSells\x12 \n\x0cvw_buy_price\x18\x06 \x01(\tR\nvwBuyPrice\x12"\n\rvw_sell_price\x18\x07 \x01(\tR\x0bvwSellPrice"x\n\x10SettleDistressed\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x16\n\x06margin\x18\x03 \x01(\tR\x06margin\x12\x14\n\x05price\x18\x04 \x01(\tR\x05price"0\n\nMarketTick\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04time\x18\x02 \x01(\x03R\x04time"\x85\x02\n\x0c\x41uctionEvent\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\'\n\x0fopening_auction\x18\x02 \x01(\x08R\x0eopeningAuction\x12\x14\n\x05leave\x18\x03 \x01(\x08R\x05leave\x12\x14\n\x05start\x18\x04 \x01(\x03R\x05start\x12\x10\n\x03\x65nd\x18\x05 \x01(\x03R\x03\x65nd\x12.\n\x07trigger\x18\x06 \x01(\x0e\x32\x14.vega.AuctionTriggerR\x07trigger\x12\x41\n\x11\x65xtension_trigger\x18\x07 \x01(\x0e\x32\x14.vega.AuctionTriggerR\x10\x65xtensionTrigger"\xa9\x03\n\x0fValidatorUpdate\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12 \n\x0cvega_pub_key\x18\x02 \x01(\tR\nvegaPubKey\x12)\n\x10\x65thereum_address\x18\x03 \x01(\tR\x0f\x65thereumAddress\x12\x1c\n\ntm_pub_key\x18\x04 \x01(\tR\x08tmPubKey\x12\x19\n\x08info_url\x18\x05 \x01(\tR\x07infoUrl\x12\x18\n\x07\x63ountry\x18\x06 \x01(\tR\x07\x63ountry\x12\x12\n\x04name\x18\x07 \x01(\tR\x04name\x12\x1d\n\navatar_url\x18\x08 \x01(\tR\tavatarUrl\x12+\n\x12vega_pub_key_index\x18\t \x01(\rR\x0fvegaPubKeyIndex\x12\x14\n\x05\x61\x64\x64\x65\x64\x18\n \x01(\x08R\x05\x61\x64\x64\x65\x64\x12\x1d\n\nfrom_epoch\x18\x0b \x01(\x04R\tfromEpoch\x12+\n\x11submitter_address\x18\x0c \x01(\tR\x10submitterAddress\x12\x1b\n\tepoch_seq\x18\r \x01(\x04R\x08\x65pochSeq"\xb2\x02\n\x15ValidatorRankingEvent\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1f\n\x0bstake_score\x18\x02 \x01(\tR\nstakeScore\x12+\n\x11performance_score\x18\x03 \x01(\tR\x10performanceScore\x12#\n\rranking_score\x18\x04 \x01(\tR\x0crankingScore\x12\'\n\x0fprevious_status\x18\x05 \x01(\tR\x0epreviousStatus\x12\x1f\n\x0bnext_status\x18\x06 \x01(\tR\nnextStatus\x12\x1b\n\tepoch_seq\x18\x07 \x01(\tR\x08\x65pochSeq\x12&\n\x0ftm_voting_power\x18\x08 \x01(\rR\rtmVotingPower"\x89\x01\n\x0bKeyRotation\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1e\n\x0bold_pub_key\x18\x02 \x01(\tR\toldPubKey\x12\x1e\n\x0bnew_pub_key\x18\x03 \x01(\tR\tnewPubKey\x12!\n\x0c\x62lock_height\x18\x04 \x01(\x04R\x0b\x62lockHeight"\x93\x01\n\x13\x45thereumKeyRotation\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1f\n\x0bold_address\x18\x02 \x01(\tR\noldAddress\x12\x1f\n\x0bnew_address\x18\x03 \x01(\tR\nnewAddress\x12!\n\x0c\x62lock_height\x18\x04 \x01(\x04R\x0b\x62lockHeight"\xd7\x01\n\x14ProtocolUpgradeEvent\x12\x30\n\x14upgrade_block_height\x18\x01 \x01(\x04R\x12upgradeBlockHeight\x12(\n\x10vega_release_tag\x18\x02 \x01(\tR\x0evegaReleaseTag\x12\x1c\n\tapprovers\x18\x03 \x03(\tR\tapprovers\x12\x45\n\x06status\x18\x04 \x01(\x0e\x32-.vega.events.v1.ProtocolUpgradeProposalStatusR\x06status"K\n\x08StateVar\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x19\n\x08\x65vent_id\x18\x02 \x01(\tR\x07\x65ventId\x12\x14\n\x05state\x18\x03 \x01(\tR\x05state"V\n\nBeginBlock\x12\x16\n\x06height\x18\x01 \x01(\x04R\x06height\x12\x1c\n\ttimestamp\x18\x02 \x01(\x03R\ttimestamp\x12\x12\n\x04hash\x18\x03 \x01(\tR\x04hash""\n\x08\x45ndBlock\x12\x16\n\x06height\x18\x01 \x01(\x04R\x06height"D\n\x16ProtocolUpgradeStarted\x12*\n\x11last_block_height\x18\x01 \x01(\x04R\x0flastBlockHeight"J\n\x1cProtocolUpgradeDataNodeReady\x12*\n\x11last_block_height\x18\x01 \x01(\x04R\x0flastBlockHeight"\xad\x01\n\x10\x43oreSnapshotData\x12!\n\x0c\x62lock_height\x18\x01 \x01(\x04R\x0b\x62lockHeight\x12\x1d\n\nblock_hash\x18\x02 \x01(\tR\tblockHash\x12!\n\x0c\x63ore_version\x18\x03 \x01(\tR\x0b\x63oreVersion\x12\x34\n\x16protocol_upgrade_block\x18\x04 \x01(\x08R\x14protocolUpgradeBlock"\xc2\x1f\n\x08\x42usEvent\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x14\n\x05\x62lock\x18\x02 \x01(\tR\x05\x62lock\x12\x30\n\x04type\x18\x03 \x01(\x0e\x32\x1c.vega.events.v1.BusEventTypeR\x04type\x12=\n\x0btime_update\x18\x65 \x01(\x0b\x32\x1a.vega.events.v1.TimeUpdateH\x00R\ntimeUpdate\x12L\n\x10ledger_movements\x18\x66 \x01(\x0b\x32\x1f.vega.events.v1.LedgerMovementsH\x00R\x0fledgerMovements\x12U\n\x13position_resolution\x18g \x01(\x0b\x32".vega.events.v1.PositionResolutionH\x00R\x12positionResolution\x12#\n\x05order\x18h \x01(\x0b\x32\x0b.vega.OrderH\x00R\x05order\x12)\n\x07\x61\x63\x63ount\x18i \x01(\x0b\x32\r.vega.AccountH\x00R\x07\x61\x63\x63ount\x12#\n\x05party\x18j \x01(\x0b\x32\x0b.vega.PartyH\x00R\x05party\x12#\n\x05trade\x18k \x01(\x0b\x32\x0b.vega.TradeH\x00R\x05trade\x12\x39\n\rmargin_levels\x18l \x01(\x0b\x32\x12.vega.MarginLevelsH\x00R\x0cmarginLevels\x12,\n\x08proposal\x18m \x01(\x0b\x32\x0e.vega.ProposalH\x00R\x08proposal\x12 \n\x04vote\x18n \x01(\x0b\x32\n.vega.VoteH\x00R\x04vote\x12\x33\n\x0bmarket_data\x18o \x01(\x0b\x32\x10.vega.MarketDataH\x00R\nmarketData\x12H\n\x0enode_signature\x18p \x01(\x0b\x32\x1f.vega.commands.v1.NodeSignatureH\x00R\rnodeSignature\x12R\n\x12loss_socialization\x18q \x01(\x0b\x32!.vega.events.v1.LossSocializationH\x00R\x11lossSocialization\x12I\n\x0fsettle_position\x18r \x01(\x0b\x32\x1e.vega.events.v1.SettlePositionH\x00R\x0esettlePosition\x12O\n\x11settle_distressed\x18s \x01(\x0b\x32 .vega.events.v1.SettleDistressedH\x00R\x10settleDistressed\x12\x35\n\x0emarket_created\x18t \x01(\x0b\x32\x0c.vega.MarketH\x00R\rmarketCreated\x12#\n\x05\x61sset\x18u \x01(\x0b\x32\x0b.vega.AssetH\x00R\x05\x61sset\x12=\n\x0bmarket_tick\x18v \x01(\x0b\x32\x1a.vega.events.v1.MarketTickH\x00R\nmarketTick\x12\x32\n\nwithdrawal\x18w \x01(\x0b\x32\x10.vega.WithdrawalH\x00R\nwithdrawal\x12)\n\x07\x64\x65posit\x18x \x01(\x0b\x32\r.vega.DepositH\x00R\x07\x64\x65posit\x12\x38\n\x07\x61uction\x18y \x01(\x0b\x32\x1c.vega.events.v1.AuctionEventH\x00R\x07\x61uction\x12\x33\n\x0brisk_factor\x18z \x01(\x0b\x32\x10.vega.RiskFactorH\x00R\nriskFactor\x12\x45\n\x11network_parameter\x18{ \x01(\x0b\x32\x16.vega.NetworkParameterH\x00R\x10networkParameter\x12K\n\x13liquidity_provision\x18| \x01(\x0b\x32\x18.vega.LiquidityProvisionH\x00R\x12liquidityProvision\x12\x35\n\x0emarket_updated\x18} \x01(\x0b\x32\x0c.vega.MarketH\x00R\rmarketUpdated\x12\x33\n\x0boracle_spec\x18~ \x01(\x0b\x32\x10.vega.OracleSpecH\x00R\noracleSpec\x12\x33\n\x0boracle_data\x18\x7f \x01(\x0b\x32\x10.vega.OracleDataH\x00R\noracleData\x12X\n\x12\x64\x65legation_balance\x18\x81\x01 \x01(\x0b\x32&.vega.events.v1.DelegationBalanceEventH\x00R\x11\x64\x65legationBalance\x12O\n\x0fvalidator_score\x18\x82\x01 \x01(\x0b\x32#.vega.events.v1.ValidatorScoreEventH\x00R\x0evalidatorScore\x12>\n\x0b\x65poch_event\x18\x83\x01 \x01(\x0b\x32\x1a.vega.events.v1.EpochEventH\x00R\nepochEvent\x12M\n\x10validator_update\x18\x84\x01 \x01(\x0b\x32\x1f.vega.events.v1.ValidatorUpdateH\x00R\x0fvalidatorUpdate\x12\x44\n\rstake_linking\x18\x85\x01 \x01(\x0b\x32\x1c.vega.events.v1.StakeLinkingH\x00R\x0cstakeLinking\x12I\n\rreward_payout\x18\x86\x01 \x01(\x0b\x32!.vega.events.v1.RewardPayoutEventH\x00R\x0crewardPayout\x12\x42\n\ncheckpoint\x18\x87\x01 \x01(\x0b\x32\x1f.vega.events.v1.CheckpointEventH\x00R\ncheckpoint\x12\x41\n\x0ckey_rotation\x18\x88\x01 \x01(\x0b\x32\x1b.vega.events.v1.KeyRotationH\x00R\x0bkeyRotation\x12\x38\n\tstate_var\x18\x89\x01 \x01(\x0b\x32\x18.vega.events.v1.StateVarH\x00R\x08stateVar\x12=\n\x0enetwork_limits\x18\x8a\x01 \x01(\x0b\x32\x13.vega.NetworkLimitsH\x00R\rnetworkLimits\x12\x37\n\x08transfer\x18\x8b\x01 \x01(\x0b\x32\x18.vega.events.v1.TransferH\x00R\x08transfer\x12M\n\rranking_event\x18\x8c\x01 \x01(\x0b\x32%.vega.events.v1.ValidatorRankingEventH\x00R\x0crankingEvent\x12j\n\x1b\x65rc20_multisig_signer_event\x18\x8d\x01 \x01(\x0b\x32(.vega.events.v1.ERC20MultiSigSignerEventH\x00R\x18\x65rc20MultisigSignerEvent\x12}\n"erc20_multisig_set_threshold_event\x18\x8e\x01 \x01(\x0b\x32..vega.events.v1.ERC20MultiSigThresholdSetEventH\x00R\x1e\x65rc20MultisigSetThresholdEvent\x12j\n\x1b\x65rc20_multisig_signer_added\x18\x8f\x01 \x01(\x0b\x32(.vega.events.v1.ERC20MultiSigSignerAddedH\x00R\x18\x65rc20MultisigSignerAdded\x12p\n\x1d\x65rc20_multisig_signer_removed\x18\x90\x01 \x01(\x0b\x32*.vega.events.v1.ERC20MultiSigSignerRemovedH\x00R\x1a\x65rc20MultisigSignerRemoved\x12W\n\x14position_state_event\x18\x91\x01 \x01(\x0b\x32".vega.events.v1.PositionStateEventH\x00R\x12positionStateEvent\x12Z\n\x15\x65thereum_key_rotation\x18\x92\x01 \x01(\x0b\x32#.vega.events.v1.EthereumKeyRotationH\x00R\x13\x65thereumKeyRotation\x12]\n\x16protocol_upgrade_event\x18\x93\x01 \x01(\x0b\x32$.vega.events.v1.ProtocolUpgradeEventH\x00R\x14protocolUpgradeEvent\x12>\n\x0b\x62\x65gin_block\x18\x94\x01 \x01(\x0b\x32\x1a.vega.events.v1.BeginBlockH\x00R\nbeginBlock\x12\x38\n\tend_block\x18\x95\x01 \x01(\x0b\x32\x18.vega.events.v1.EndBlockH\x00R\x08\x65ndBlock\x12\x63\n\x18protocol_upgrade_started\x18\x96\x01 \x01(\x0b\x32&.vega.events.v1.ProtocolUpgradeStartedH\x00R\x16protocolUpgradeStarted\x12\x44\n\rsettle_market\x18\x97\x01 \x01(\x0b\x32\x1c.vega.events.v1.SettleMarketH\x00R\x0csettleMarket\x12S\n\x12transaction_result\x18\x98\x01 \x01(\x0b\x32!.vega.events.v1.TransactionResultH\x00R\x11transactionResult\x12S\n\x13\x63ore_snapshot_event\x18\x99\x01 \x01(\x0b\x32 .vega.events.v1.CoreSnapshotDataH\x00R\x11\x63oreSnapshotEvent\x12w\n protocol_upgrade_data_node_ready\x18\x9a\x01 \x01(\x0b\x32,.vega.events.v1.ProtocolUpgradeDataNodeReadyH\x00R\x1cprotocolUpgradeDataNodeReady\x12\x36\n\x06market\x18\xe9\x07 \x01(\x0b\x32\x1b.vega.events.v1.MarketEventH\x00R\x06market\x12\x41\n\x0ctx_err_event\x18\xd1\x0f \x01(\x0b\x32\x1c.vega.events.v1.TxErrorEventH\x00R\ntxErrEvent\x12\x18\n\x07version\x18\x04 \x01(\rR\x07version\x12\x19\n\x08\x63hain_id\x18\x05 \x01(\tR\x07\x63hainId\x12\x17\n\x07tx_hash\x18\x06 \x01(\tR\x06txHashB\x07\n\x05\x65vent*\xdd\x01\n\x1dProtocolUpgradeProposalStatus\x12\x30\n,PROTOCOL_UPGRADE_PROPOSAL_STATUS_UNSPECIFIED\x10\x00\x12,\n(PROTOCOL_UPGRADE_PROPOSAL_STATUS_PENDING\x10\x01\x12-\n)PROTOCOL_UPGRADE_PROPOSAL_STATUS_APPROVED\x10\x02\x12-\n)PROTOCOL_UPGRADE_PROPOSAL_STATUS_REJECTED\x10\x03*\xf5\x0f\n\x0c\x42usEventType\x12\x1e\n\x1a\x42US_EVENT_TYPE_UNSPECIFIED\x10\x00\x12\x16\n\x12\x42US_EVENT_TYPE_ALL\x10\x01\x12\x1e\n\x1a\x42US_EVENT_TYPE_TIME_UPDATE\x10\x02\x12#\n\x1f\x42US_EVENT_TYPE_LEDGER_MOVEMENTS\x10\x03\x12&\n"BUS_EVENT_TYPE_POSITION_RESOLUTION\x10\x04\x12\x18\n\x14\x42US_EVENT_TYPE_ORDER\x10\x05\x12\x1a\n\x16\x42US_EVENT_TYPE_ACCOUNT\x10\x06\x12\x18\n\x14\x42US_EVENT_TYPE_PARTY\x10\x07\x12\x18\n\x14\x42US_EVENT_TYPE_TRADE\x10\x08\x12 \n\x1c\x42US_EVENT_TYPE_MARGIN_LEVELS\x10\t\x12\x1b\n\x17\x42US_EVENT_TYPE_PROPOSAL\x10\n\x12\x17\n\x13\x42US_EVENT_TYPE_VOTE\x10\x0b\x12\x1e\n\x1a\x42US_EVENT_TYPE_MARKET_DATA\x10\x0c\x12!\n\x1d\x42US_EVENT_TYPE_NODE_SIGNATURE\x10\r\x12%\n!BUS_EVENT_TYPE_LOSS_SOCIALIZATION\x10\x0e\x12"\n\x1e\x42US_EVENT_TYPE_SETTLE_POSITION\x10\x0f\x12$\n BUS_EVENT_TYPE_SETTLE_DISTRESSED\x10\x10\x12!\n\x1d\x42US_EVENT_TYPE_MARKET_CREATED\x10\x11\x12\x18\n\x14\x42US_EVENT_TYPE_ASSET\x10\x12\x12\x1e\n\x1a\x42US_EVENT_TYPE_MARKET_TICK\x10\x13\x12\x1d\n\x19\x42US_EVENT_TYPE_WITHDRAWAL\x10\x14\x12\x1a\n\x16\x42US_EVENT_TYPE_DEPOSIT\x10\x15\x12\x1a\n\x16\x42US_EVENT_TYPE_AUCTION\x10\x16\x12\x1e\n\x1a\x42US_EVENT_TYPE_RISK_FACTOR\x10\x17\x12$\n BUS_EVENT_TYPE_NETWORK_PARAMETER\x10\x18\x12&\n"BUS_EVENT_TYPE_LIQUIDITY_PROVISION\x10\x19\x12!\n\x1d\x42US_EVENT_TYPE_MARKET_UPDATED\x10\x1a\x12\x1e\n\x1a\x42US_EVENT_TYPE_ORACLE_SPEC\x10\x1b\x12\x1e\n\x1a\x42US_EVENT_TYPE_ORACLE_DATA\x10\x1c\x12%\n!BUS_EVENT_TYPE_DELEGATION_BALANCE\x10\x1d\x12"\n\x1e\x42US_EVENT_TYPE_VALIDATOR_SCORE\x10\x1e\x12\x1f\n\x1b\x42US_EVENT_TYPE_EPOCH_UPDATE\x10\x1f\x12#\n\x1f\x42US_EVENT_TYPE_VALIDATOR_UPDATE\x10 \x12 \n\x1c\x42US_EVENT_TYPE_STAKE_LINKING\x10!\x12&\n"BUS_EVENT_TYPE_REWARD_PAYOUT_EVENT\x10"\x12\x1d\n\x19\x42US_EVENT_TYPE_CHECKPOINT\x10#\x12\x1f\n\x1b\x42US_EVENT_TYPE_STREAM_START\x10$\x12\x1f\n\x1b\x42US_EVENT_TYPE_KEY_ROTATION\x10%\x12\x1c\n\x18\x42US_EVENT_TYPE_STATE_VAR\x10&\x12!\n\x1d\x42US_EVENT_TYPE_NETWORK_LIMITS\x10\'\x12\x1b\n\x17\x42US_EVENT_TYPE_TRANSFER\x10(\x12$\n BUS_EVENT_TYPE_VALIDATOR_RANKING\x10)\x12/\n+BUS_EVENT_TYPE_ERC20_MULTI_SIG_SIGNER_EVENT\x10*\x12\x30\n,BUS_EVENT_TYPE_ERC20_MULTI_SIG_SET_THRESHOLD\x10+\x12/\n+BUS_EVENT_TYPE_ERC20_MULTI_SIG_SIGNER_ADDED\x10,\x12\x31\n-BUS_EVENT_TYPE_ERC20_MULTI_SIG_SIGNER_REMOVED\x10-\x12!\n\x1d\x42US_EVENT_TYPE_POSITION_STATE\x10.\x12(\n$BUS_EVENT_TYPE_ETHEREUM_KEY_ROTATION\x10/\x12,\n(BUS_EVENT_TYPE_PROTOCOL_UPGRADE_PROPOSAL\x10\x30\x12\x1e\n\x1a\x42US_EVENT_TYPE_BEGIN_BLOCK\x10\x31\x12\x1c\n\x18\x42US_EVENT_TYPE_END_BLOCK\x10\x32\x12+\n\'BUS_EVENT_TYPE_PROTOCOL_UPGRADE_STARTED\x10\x33\x12 \n\x1c\x42US_EVENT_TYPE_SETTLE_MARKET\x10\x34\x12%\n!BUS_EVENT_TYPE_TRANSACTION_RESULT\x10\x35\x12!\n\x1d\x42US_EVENT_TYPE_SNAPSHOT_TAKEN\x10\x36\x12\x33\n/BUS_EVENT_TYPE_PROTOCOL_UPGRADE_DATA_NODE_READY\x10\x37\x12\x19\n\x15\x42US_EVENT_TYPE_MARKET\x10\x65\x12\x1c\n\x17\x42US_EVENT_TYPE_TX_ERROR\x10\xc9\x01\x42\x31Z/code.vegaprotocol.io/vega/protos/vega/events/v1b\x06proto3'
+    b'\n\x1bvega/events/v1/events.proto\x12\x0evega.events.v1\x1a\x12vega/markets.proto\x1a\x11vega/assets.proto\x1a\x15vega/governance.proto\x1a\x0fvega/vega.proto\x1a\x11vega/oracle.proto\x1a\x1fvega/commands/v1/commands.proto\x1a\x1bvega/commands/v1/data.proto\x1a)vega/commands/v1/validator_commands.proto"\xee\x01\n\x18\x45RC20MultiSigSignerAdded\x12!\n\x0csignature_id\x18\x01 \x01(\tR\x0bsignatureId\x12!\n\x0cvalidator_id\x18\x02 \x01(\tR\x0bvalidatorId\x12\x1c\n\ttimestamp\x18\x03 \x01(\x03R\ttimestamp\x12\x1d\n\nnew_signer\x18\x04 \x01(\tR\tnewSigner\x12\x1c\n\tsubmitter\x18\x05 \x01(\tR\tsubmitter\x12\x14\n\x05nonce\x18\x06 \x01(\tR\x05nonce\x12\x1b\n\tepoch_seq\x18\x07 \x01(\tR\x08\x65pochSeq"f\n#ERC20MultiSigSignerRemovedSubmitter\x12!\n\x0csignature_id\x18\x01 \x01(\tR\x0bsignatureId\x12\x1c\n\tsubmitter\x18\x02 \x01(\tR\tsubmitter"\x97\x02\n\x1a\x45RC20MultiSigSignerRemoved\x12\x66\n\x14signature_submitters\x18\x01 \x03(\x0b\x32\x33.vega.events.v1.ERC20MultiSigSignerRemovedSubmitterR\x13signatureSubmitters\x12!\n\x0cvalidator_id\x18\x02 \x01(\tR\x0bvalidatorId\x12\x1c\n\ttimestamp\x18\x03 \x01(\x03R\ttimestamp\x12\x1d\n\nold_signer\x18\x04 \x01(\tR\toldSigner\x12\x14\n\x05nonce\x18\x05 \x01(\tR\x05nonce\x12\x1b\n\tepoch_seq\x18\x06 \x01(\tR\x08\x65pochSeq"\x90\x05\n\x08Transfer\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04\x66rom\x18\x02 \x01(\tR\x04\x66rom\x12=\n\x11\x66rom_account_type\x18\x03 \x01(\x0e\x32\x11.vega.AccountTypeR\x0f\x66romAccountType\x12\x0e\n\x02to\x18\x04 \x01(\tR\x02to\x12\x39\n\x0fto_account_type\x18\x05 \x01(\x0e\x32\x11.vega.AccountTypeR\rtoAccountType\x12\x14\n\x05\x61sset\x18\x06 \x01(\tR\x05\x61sset\x12\x16\n\x06\x61mount\x18\x07 \x01(\tR\x06\x61mount\x12\x1c\n\treference\x18\x08 \x01(\tR\treference\x12\x37\n\x06status\x18\t \x01(\x0e\x32\x1f.vega.events.v1.Transfer.StatusR\x06status\x12\x1c\n\ttimestamp\x18\n \x01(\x03R\ttimestamp\x12\x1b\n\x06reason\x18\x0b \x01(\tH\x01R\x06reason\x88\x01\x01\x12\x39\n\x07one_off\x18\x65 \x01(\x0b\x32\x1e.vega.events.v1.OneOffTransferH\x00R\x06oneOff\x12\x41\n\trecurring\x18\x66 \x01(\x0b\x32!.vega.events.v1.RecurringTransferH\x00R\trecurring"\x84\x01\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x12\n\x0eSTATUS_PENDING\x10\x01\x12\x0f\n\x0bSTATUS_DONE\x10\x02\x12\x13\n\x0fSTATUS_REJECTED\x10\x03\x12\x12\n\x0eSTATUS_STOPPED\x10\x04\x12\x14\n\x10STATUS_CANCELLED\x10\x05\x42\x06\n\x04kindB\t\n\x07_reason"/\n\x0eOneOffTransfer\x12\x1d\n\ndeliver_on\x18\x01 \x01(\x03R\tdeliverOn"\xc1\x01\n\x11RecurringTransfer\x12\x1f\n\x0bstart_epoch\x18\x01 \x01(\x04R\nstartEpoch\x12 \n\tend_epoch\x18\x02 \x01(\x04H\x00R\x08\x65ndEpoch\x88\x01\x01\x12\x16\n\x06\x66\x61\x63tor\x18\x03 \x01(\tR\x06\x66\x61\x63tor\x12\x43\n\x11\x64ispatch_strategy\x18\x04 \x01(\x0b\x32\x16.vega.DispatchStrategyR\x10\x64ispatchStrategyB\x0c\n\n_end_epoch"\xb4\x04\n\x0cStakeLinking\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x35\n\x04type\x18\x02 \x01(\x0e\x32!.vega.events.v1.StakeLinking.TypeR\x04type\x12\x0e\n\x02ts\x18\x03 \x01(\x03R\x02ts\x12\x14\n\x05party\x18\x04 \x01(\tR\x05party\x12\x16\n\x06\x61mount\x18\x05 \x01(\tR\x06\x61mount\x12;\n\x06status\x18\x06 \x01(\x0e\x32#.vega.events.v1.StakeLinking.StatusR\x06status\x12!\n\x0c\x66inalized_at\x18\x07 \x01(\x03R\x0b\x66inalizedAt\x12\x17\n\x07tx_hash\x18\x08 \x01(\tR\x06txHash\x12!\n\x0c\x62lock_height\x18\t \x01(\x04R\x0b\x62lockHeight\x12\x1d\n\nblock_time\x18\n \x01(\x03R\tblockTime\x12\x1b\n\tlog_index\x18\x0b \x01(\x04R\x08logIndex\x12)\n\x10\x65thereum_address\x18\x0c \x01(\tR\x0f\x65thereumAddress"<\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\r\n\tTYPE_LINK\x10\x01\x12\x0f\n\x0bTYPE_UNLINK\x10\x02"^\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x12\n\x0eSTATUS_PENDING\x10\x01\x12\x13\n\x0fSTATUS_ACCEPTED\x10\x02\x12\x13\n\x0fSTATUS_REJECTED\x10\x03"\xd3\x02\n\x18\x45RC20MultiSigSignerEvent\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x41\n\x04type\x18\x02 \x01(\x0e\x32-.vega.events.v1.ERC20MultiSigSignerEvent.TypeR\x04type\x12\x16\n\x06signer\x18\x03 \x01(\tR\x06signer\x12\x14\n\x05nonce\x18\x04 \x01(\tR\x05nonce\x12\x1d\n\nblock_time\x18\x05 \x01(\x03R\tblockTime\x12\x17\n\x07tx_hash\x18\x06 \x01(\tR\x06txHash\x12\x1b\n\tlog_index\x18\x07 \x01(\x04R\x08logIndex\x12!\n\x0c\x62lock_number\x18\x08 \x01(\x04R\x0b\x62lockNumber">\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0e\n\nTYPE_ADDED\x10\x01\x12\x10\n\x0cTYPE_REMOVED\x10\x02"\xe3\x01\n\x1e\x45RC20MultiSigThresholdSetEvent\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12#\n\rnew_threshold\x18\x02 \x01(\rR\x0cnewThreshold\x12\x14\n\x05nonce\x18\x03 \x01(\tR\x05nonce\x12\x1d\n\nblock_time\x18\x04 \x01(\x03R\tblockTime\x12\x17\n\x07tx_hash\x18\x05 \x01(\tR\x06txHash\x12\x1b\n\tlog_index\x18\x06 \x01(\x04R\x08logIndex\x12!\n\x0c\x62lock_number\x18\x07 \x01(\x04R\x0b\x62lockNumber"g\n\x0f\x43heckpointEvent\x12\x12\n\x04hash\x18\x01 \x01(\tR\x04hash\x12\x1d\n\nblock_hash\x18\x02 \x01(\tR\tblockHash\x12!\n\x0c\x62lock_height\x18\x03 \x01(\x04R\x0b\x62lockHeight"-\n\x10StreamStartEvent\x12\x19\n\x08\x63hain_id\x18\x01 \x01(\tR\x07\x63hainId"\x82\x02\n\x11RewardPayoutEvent\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x1b\n\tepoch_seq\x18\x02 \x01(\tR\x08\x65pochSeq\x12\x14\n\x05\x61sset\x18\x03 \x01(\tR\x05\x61sset\x12\x16\n\x06\x61mount\x18\x04 \x01(\tR\x06\x61mount\x12\x35\n\x17percent_of_total_reward\x18\x05 \x01(\tR\x14percentOfTotalReward\x12\x1c\n\ttimestamp\x18\x06 \x01(\x03R\ttimestamp\x12\x1f\n\x0breward_type\x18\x07 \x01(\tR\nrewardType\x12\x16\n\x06market\x18\x08 \x01(\tR\x06market"\xd6\x02\n\x13ValidatorScoreEvent\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1b\n\tepoch_seq\x18\x02 \x01(\tR\x08\x65pochSeq\x12\'\n\x0fvalidator_score\x18\x03 \x01(\tR\x0evalidatorScore\x12)\n\x10normalised_score\x18\x04 \x01(\tR\x0fnormalisedScore\x12\x33\n\x15validator_performance\x18\x05 \x01(\tR\x14validatorPerformance\x12.\n\x13raw_validator_score\x18\x06 \x01(\tR\x11rawValidatorScore\x12)\n\x10validator_status\x18\x07 \x01(\tR\x0fvalidatorStatus\x12%\n\x0emultisig_score\x18\x08 \x01(\tR\rmultisigScore"|\n\x16\x44\x65legationBalanceEvent\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x17\n\x07node_id\x18\x02 \x01(\tR\x06nodeId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x1b\n\tepoch_seq\x18\x04 \x01(\tR\x08\x65pochSeq"D\n\x0bMarketEvent\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x18\n\x07payload\x18\x02 \x01(\tR\x07payload"\xed\x10\n\x11TransactionResult\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x16\n\x06status\x18\x02 \x01(\x08R\x06status\x12\x12\n\x04hash\x18\x03 \x01(\tR\x04hash\x12N\n\x10order_submission\x18\x65 \x01(\x0b\x32!.vega.commands.v1.OrderSubmissionH\x00R\x0forderSubmission\x12K\n\x0forder_amendment\x18\x66 \x01(\x0b\x32 .vega.commands.v1.OrderAmendmentH\x00R\x0eorderAmendment\x12T\n\x12order_cancellation\x18g \x01(\x0b\x32#.vega.commands.v1.OrderCancellationH\x00R\x11orderCancellation\x12\x42\n\x08proposal\x18h \x01(\x0b\x32$.vega.commands.v1.ProposalSubmissionH\x00R\x08proposal\x12K\n\x0fvote_submission\x18i \x01(\x0b\x32 .vega.commands.v1.VoteSubmissionH\x00R\x0evoteSubmission\x12v\n\x1eliquidity_provision_submission\x18j \x01(\x0b\x32..vega.commands.v1.LiquidityProvisionSubmissionH\x00R\x1cliquidityProvisionSubmission\x12W\n\x13withdraw_submission\x18k \x01(\x0b\x32$.vega.commands.v1.WithdrawSubmissionH\x00R\x12withdrawSubmission\x12W\n\x13\x64\x65legate_submission\x18l \x01(\x0b\x32$.vega.commands.v1.DelegateSubmissionH\x00R\x12\x64\x65legateSubmission\x12]\n\x15undelegate_submission\x18m \x01(\x0b\x32&.vega.commands.v1.UndelegateSubmissionH\x00R\x14undelegateSubmission\x12|\n liquidity_provision_cancellation\x18o \x01(\x0b\x32\x30.vega.commands.v1.LiquidityProvisionCancellationH\x00R\x1eliquidityProvisionCancellation\x12s\n\x1dliquidity_provision_amendment\x18p \x01(\x0b\x32-.vega.commands.v1.LiquidityProvisionAmendmentH\x00R\x1bliquidityProvisionAmendment\x12\x38\n\x08transfer\x18q \x01(\x0b\x32\x1a.vega.commands.v1.TransferH\x00R\x08transfer\x12K\n\x0f\x63\x61ncel_transfer\x18r \x01(\x0b\x32 .vega.commands.v1.CancelTransferH\x00R\x0e\x63\x61ncelTransfer\x12\x45\n\rannounce_node\x18s \x01(\x0b\x32\x1e.vega.commands.v1.AnnounceNodeH\x00R\x0c\x61nnounceNode\x12^\n\x16oracle_data_submission\x18t \x01(\x0b\x32&.vega.commands.v1.OracleDataSubmissionH\x00R\x14oracleDataSubmission\x12g\n\x19protocol_upgrade_proposal\x18u \x01(\x0b\x32).vega.commands.v1.ProtocolUpgradeProposalH\x00R\x17protocolUpgradeProposal\x12N\n\x10issue_signatures\x18v \x01(\x0b\x32!.vega.commands.v1.IssueSignaturesH\x00R\x0fissueSignatures\x12g\n\x19\x62\x61tch_market_instructions\x18w \x01(\x0b\x32).vega.commands.v1.BatchMarketInstructionsH\x00R\x17\x62\x61tchMarketInstructions\x12[\n\x15key_rotate_submission\x18x \x01(\x0b\x32%.vega.commands.v1.KeyRotateSubmissionH\x00R\x13keyRotateSubmission\x12t\n\x1e\x65thereum_key_rotate_submission\x18y \x01(\x0b\x32-.vega.commands.v1.EthereumKeyRotateSubmissionH\x00R\x1b\x65thereumKeyRotateSubmission\x12M\n\x07success\x18\xe9\x07 \x01(\x0b\x32\x30.vega.events.v1.TransactionResult.SuccessDetailsH\x01R\x07success\x12M\n\x07\x66\x61ilure\x18\xea\x07 \x01(\x0b\x32\x30.vega.events.v1.TransactionResult.FailureDetailsH\x01R\x07\x66\x61ilure\x1a\x10\n\x0eSuccessDetails\x1a&\n\x0e\x46\x61ilureDetails\x12\x14\n\x05\x65rror\x18\x01 \x01(\tR\x05\x65rrorB\r\n\x0btransactionB\x07\n\x05\x65xtra"\xa7\r\n\x0cTxErrorEvent\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x17\n\x07\x65rr_msg\x18\x02 \x01(\tR\x06\x65rrMsg\x12N\n\x10order_submission\x18\x65 \x01(\x0b\x32!.vega.commands.v1.OrderSubmissionH\x00R\x0forderSubmission\x12K\n\x0forder_amendment\x18\x66 \x01(\x0b\x32 .vega.commands.v1.OrderAmendmentH\x00R\x0eorderAmendment\x12T\n\x12order_cancellation\x18g \x01(\x0b\x32#.vega.commands.v1.OrderCancellationH\x00R\x11orderCancellation\x12\x42\n\x08proposal\x18h \x01(\x0b\x32$.vega.commands.v1.ProposalSubmissionH\x00R\x08proposal\x12K\n\x0fvote_submission\x18i \x01(\x0b\x32 .vega.commands.v1.VoteSubmissionH\x00R\x0evoteSubmission\x12v\n\x1eliquidity_provision_submission\x18j \x01(\x0b\x32..vega.commands.v1.LiquidityProvisionSubmissionH\x00R\x1cliquidityProvisionSubmission\x12W\n\x13withdraw_submission\x18k \x01(\x0b\x32$.vega.commands.v1.WithdrawSubmissionH\x00R\x12withdrawSubmission\x12W\n\x13\x64\x65legate_submission\x18l \x01(\x0b\x32$.vega.commands.v1.DelegateSubmissionH\x00R\x12\x64\x65legateSubmission\x12]\n\x15undelegate_submission\x18m \x01(\x0b\x32&.vega.commands.v1.UndelegateSubmissionH\x00R\x14undelegateSubmission\x12|\n liquidity_provision_cancellation\x18o \x01(\x0b\x32\x30.vega.commands.v1.LiquidityProvisionCancellationH\x00R\x1eliquidityProvisionCancellation\x12s\n\x1dliquidity_provision_amendment\x18p \x01(\x0b\x32-.vega.commands.v1.LiquidityProvisionAmendmentH\x00R\x1bliquidityProvisionAmendment\x12\x38\n\x08transfer\x18q \x01(\x0b\x32\x1a.vega.commands.v1.TransferH\x00R\x08transfer\x12K\n\x0f\x63\x61ncel_transfer\x18r \x01(\x0b\x32 .vega.commands.v1.CancelTransferH\x00R\x0e\x63\x61ncelTransfer\x12\x45\n\rannounce_node\x18s \x01(\x0b\x32\x1e.vega.commands.v1.AnnounceNodeH\x00R\x0c\x61nnounceNode\x12^\n\x16oracle_data_submission\x18t \x01(\x0b\x32&.vega.commands.v1.OracleDataSubmissionH\x00R\x14oracleDataSubmission\x12g\n\x19protocol_upgrade_proposal\x18u \x01(\x0b\x32).vega.commands.v1.ProtocolUpgradeProposalH\x00R\x17protocolUpgradeProposal\x12N\n\x10issue_signatures\x18v \x01(\x0b\x32!.vega.commands.v1.IssueSignaturesH\x00R\x0fissueSignatures\x12g\n\x19\x62\x61tch_market_instructions\x18w \x01(\x0b\x32).vega.commands.v1.BatchMarketInstructionsH\x00R\x17\x62\x61tchMarketInstructionsB\r\n\x0btransactionJ\x04\x08n\x10o"*\n\nTimeUpdate\x12\x1c\n\ttimestamp\x18\x01 \x01(\x03R\ttimestamp"\xa4\x01\n\nEpochEvent\x12\x10\n\x03seq\x18\x01 \x01(\x04R\x03seq\x12)\n\x06\x61\x63tion\x18\x02 \x01(\x0e\x32\x11.vega.EpochActionR\x06\x61\x63tion\x12\x1d\n\nstart_time\x18\x03 \x01(\x03R\tstartTime\x12\x1f\n\x0b\x65xpire_time\x18\x04 \x01(\x03R\nexpireTime\x12\x19\n\x08\x65nd_time\x18\x05 \x01(\x03R\x07\x65ndTime"R\n\x0fLedgerMovements\x12?\n\x10ledger_movements\x18\x01 \x03(\x0b\x32\x14.vega.LedgerMovementR\x0fledgerMovements"\x88\x01\n\x12PositionResolution\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x1e\n\ndistressed\x18\x02 \x01(\x03R\ndistressed\x12\x16\n\x06\x63losed\x18\x03 \x01(\x03R\x06\x63losed\x12\x1d\n\nmark_price\x18\x04 \x01(\tR\tmarkPrice"c\n\x11LossSocialization\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount"^\n\x0fTradeSettlement\x12\x12\n\x04size\x18\x01 \x01(\x03R\x04size\x12\x14\n\x05price\x18\x02 \x01(\tR\x05price\x12!\n\x0cmarket_price\x18\x03 \x01(\tR\x0bmarketPrice"\xd5\x01\n\x0eSettlePosition\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x14\n\x05price\x18\x03 \x01(\tR\x05price\x12L\n\x11trade_settlements\x18\x04 \x03(\x0b\x32\x1f.vega.events.v1.TradeSettlementR\x10tradeSettlements\x12\'\n\x0fposition_factor\x18\x05 \x01(\tR\x0epositionFactor"j\n\x0cSettleMarket\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x14\n\x05price\x18\x02 \x01(\tR\x05price\x12\'\n\x0fposition_factor\x18\x03 \x01(\tR\x0epositionFactor"\xf6\x01\n\x12PositionStateEvent\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x12\n\x04size\x18\x03 \x01(\x03R\x04size\x12%\n\x0epotential_buys\x18\x04 \x01(\x03R\rpotentialBuys\x12\'\n\x0fpotential_sells\x18\x05 \x01(\x03R\x0epotentialSells\x12 \n\x0cvw_buy_price\x18\x06 \x01(\tR\nvwBuyPrice\x12"\n\rvw_sell_price\x18\x07 \x01(\tR\x0bvwSellPrice"x\n\x10SettleDistressed\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x16\n\x06margin\x18\x03 \x01(\tR\x06margin\x12\x14\n\x05price\x18\x04 \x01(\tR\x05price"I\n\x10\x44istressedOrders\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x18\n\x07parties\x18\x02 \x03(\tR\x07parties"0\n\nMarketTick\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04time\x18\x02 \x01(\x03R\x04time"\x85\x02\n\x0c\x41uctionEvent\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\'\n\x0fopening_auction\x18\x02 \x01(\x08R\x0eopeningAuction\x12\x14\n\x05leave\x18\x03 \x01(\x08R\x05leave\x12\x14\n\x05start\x18\x04 \x01(\x03R\x05start\x12\x10\n\x03\x65nd\x18\x05 \x01(\x03R\x03\x65nd\x12.\n\x07trigger\x18\x06 \x01(\x0e\x32\x14.vega.AuctionTriggerR\x07trigger\x12\x41\n\x11\x65xtension_trigger\x18\x07 \x01(\x0e\x32\x14.vega.AuctionTriggerR\x10\x65xtensionTrigger"\xa9\x03\n\x0fValidatorUpdate\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12 \n\x0cvega_pub_key\x18\x02 \x01(\tR\nvegaPubKey\x12)\n\x10\x65thereum_address\x18\x03 \x01(\tR\x0f\x65thereumAddress\x12\x1c\n\ntm_pub_key\x18\x04 \x01(\tR\x08tmPubKey\x12\x19\n\x08info_url\x18\x05 \x01(\tR\x07infoUrl\x12\x18\n\x07\x63ountry\x18\x06 \x01(\tR\x07\x63ountry\x12\x12\n\x04name\x18\x07 \x01(\tR\x04name\x12\x1d\n\navatar_url\x18\x08 \x01(\tR\tavatarUrl\x12+\n\x12vega_pub_key_index\x18\t \x01(\rR\x0fvegaPubKeyIndex\x12\x14\n\x05\x61\x64\x64\x65\x64\x18\n \x01(\x08R\x05\x61\x64\x64\x65\x64\x12\x1d\n\nfrom_epoch\x18\x0b \x01(\x04R\tfromEpoch\x12+\n\x11submitter_address\x18\x0c \x01(\tR\x10submitterAddress\x12\x1b\n\tepoch_seq\x18\r \x01(\x04R\x08\x65pochSeq"\xb2\x02\n\x15ValidatorRankingEvent\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1f\n\x0bstake_score\x18\x02 \x01(\tR\nstakeScore\x12+\n\x11performance_score\x18\x03 \x01(\tR\x10performanceScore\x12#\n\rranking_score\x18\x04 \x01(\tR\x0crankingScore\x12\'\n\x0fprevious_status\x18\x05 \x01(\tR\x0epreviousStatus\x12\x1f\n\x0bnext_status\x18\x06 \x01(\tR\nnextStatus\x12\x1b\n\tepoch_seq\x18\x07 \x01(\tR\x08\x65pochSeq\x12&\n\x0ftm_voting_power\x18\x08 \x01(\rR\rtmVotingPower"\x89\x01\n\x0bKeyRotation\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1e\n\x0bold_pub_key\x18\x02 \x01(\tR\toldPubKey\x12\x1e\n\x0bnew_pub_key\x18\x03 \x01(\tR\tnewPubKey\x12!\n\x0c\x62lock_height\x18\x04 \x01(\x04R\x0b\x62lockHeight"\x93\x01\n\x13\x45thereumKeyRotation\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1f\n\x0bold_address\x18\x02 \x01(\tR\noldAddress\x12\x1f\n\x0bnew_address\x18\x03 \x01(\tR\nnewAddress\x12!\n\x0c\x62lock_height\x18\x04 \x01(\x04R\x0b\x62lockHeight"\xd7\x01\n\x14ProtocolUpgradeEvent\x12\x30\n\x14upgrade_block_height\x18\x01 \x01(\x04R\x12upgradeBlockHeight\x12(\n\x10vega_release_tag\x18\x02 \x01(\tR\x0evegaReleaseTag\x12\x1c\n\tapprovers\x18\x03 \x03(\tR\tapprovers\x12\x45\n\x06status\x18\x04 \x01(\x0e\x32-.vega.events.v1.ProtocolUpgradeProposalStatusR\x06status"K\n\x08StateVar\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x19\n\x08\x65vent_id\x18\x02 \x01(\tR\x07\x65ventId\x12\x14\n\x05state\x18\x03 \x01(\tR\x05state"V\n\nBeginBlock\x12\x16\n\x06height\x18\x01 \x01(\x04R\x06height\x12\x1c\n\ttimestamp\x18\x02 \x01(\x03R\ttimestamp\x12\x12\n\x04hash\x18\x03 \x01(\tR\x04hash""\n\x08\x45ndBlock\x12\x16\n\x06height\x18\x01 \x01(\x04R\x06height"D\n\x16ProtocolUpgradeStarted\x12*\n\x11last_block_height\x18\x01 \x01(\x04R\x0flastBlockHeight"J\n\x1cProtocolUpgradeDataNodeReady\x12*\n\x11last_block_height\x18\x01 \x01(\x04R\x0flastBlockHeight"\xad\x01\n\x10\x43oreSnapshotData\x12!\n\x0c\x62lock_height\x18\x01 \x01(\x04R\x0b\x62lockHeight\x12\x1d\n\nblock_hash\x18\x02 \x01(\tR\tblockHash\x12!\n\x0c\x63ore_version\x18\x03 \x01(\tR\x0b\x63oreVersion\x12\x34\n\x16protocol_upgrade_block\x18\x04 \x01(\x08R\x14protocolUpgradeBlock"\x94 \n\x08\x42usEvent\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x14\n\x05\x62lock\x18\x02 \x01(\tR\x05\x62lock\x12\x30\n\x04type\x18\x03 \x01(\x0e\x32\x1c.vega.events.v1.BusEventTypeR\x04type\x12=\n\x0btime_update\x18\x65 \x01(\x0b\x32\x1a.vega.events.v1.TimeUpdateH\x00R\ntimeUpdate\x12L\n\x10ledger_movements\x18\x66 \x01(\x0b\x32\x1f.vega.events.v1.LedgerMovementsH\x00R\x0fledgerMovements\x12U\n\x13position_resolution\x18g \x01(\x0b\x32".vega.events.v1.PositionResolutionH\x00R\x12positionResolution\x12#\n\x05order\x18h \x01(\x0b\x32\x0b.vega.OrderH\x00R\x05order\x12)\n\x07\x61\x63\x63ount\x18i \x01(\x0b\x32\r.vega.AccountH\x00R\x07\x61\x63\x63ount\x12#\n\x05party\x18j \x01(\x0b\x32\x0b.vega.PartyH\x00R\x05party\x12#\n\x05trade\x18k \x01(\x0b\x32\x0b.vega.TradeH\x00R\x05trade\x12\x39\n\rmargin_levels\x18l \x01(\x0b\x32\x12.vega.MarginLevelsH\x00R\x0cmarginLevels\x12,\n\x08proposal\x18m \x01(\x0b\x32\x0e.vega.ProposalH\x00R\x08proposal\x12 \n\x04vote\x18n \x01(\x0b\x32\n.vega.VoteH\x00R\x04vote\x12\x33\n\x0bmarket_data\x18o \x01(\x0b\x32\x10.vega.MarketDataH\x00R\nmarketData\x12H\n\x0enode_signature\x18p \x01(\x0b\x32\x1f.vega.commands.v1.NodeSignatureH\x00R\rnodeSignature\x12R\n\x12loss_socialization\x18q \x01(\x0b\x32!.vega.events.v1.LossSocializationH\x00R\x11lossSocialization\x12I\n\x0fsettle_position\x18r \x01(\x0b\x32\x1e.vega.events.v1.SettlePositionH\x00R\x0esettlePosition\x12O\n\x11settle_distressed\x18s \x01(\x0b\x32 .vega.events.v1.SettleDistressedH\x00R\x10settleDistressed\x12\x35\n\x0emarket_created\x18t \x01(\x0b\x32\x0c.vega.MarketH\x00R\rmarketCreated\x12#\n\x05\x61sset\x18u \x01(\x0b\x32\x0b.vega.AssetH\x00R\x05\x61sset\x12=\n\x0bmarket_tick\x18v \x01(\x0b\x32\x1a.vega.events.v1.MarketTickH\x00R\nmarketTick\x12\x32\n\nwithdrawal\x18w \x01(\x0b\x32\x10.vega.WithdrawalH\x00R\nwithdrawal\x12)\n\x07\x64\x65posit\x18x \x01(\x0b\x32\r.vega.DepositH\x00R\x07\x64\x65posit\x12\x38\n\x07\x61uction\x18y \x01(\x0b\x32\x1c.vega.events.v1.AuctionEventH\x00R\x07\x61uction\x12\x33\n\x0brisk_factor\x18z \x01(\x0b\x32\x10.vega.RiskFactorH\x00R\nriskFactor\x12\x45\n\x11network_parameter\x18{ \x01(\x0b\x32\x16.vega.NetworkParameterH\x00R\x10networkParameter\x12K\n\x13liquidity_provision\x18| \x01(\x0b\x32\x18.vega.LiquidityProvisionH\x00R\x12liquidityProvision\x12\x35\n\x0emarket_updated\x18} \x01(\x0b\x32\x0c.vega.MarketH\x00R\rmarketUpdated\x12\x33\n\x0boracle_spec\x18~ \x01(\x0b\x32\x10.vega.OracleSpecH\x00R\noracleSpec\x12\x33\n\x0boracle_data\x18\x7f \x01(\x0b\x32\x10.vega.OracleDataH\x00R\noracleData\x12X\n\x12\x64\x65legation_balance\x18\x81\x01 \x01(\x0b\x32&.vega.events.v1.DelegationBalanceEventH\x00R\x11\x64\x65legationBalance\x12O\n\x0fvalidator_score\x18\x82\x01 \x01(\x0b\x32#.vega.events.v1.ValidatorScoreEventH\x00R\x0evalidatorScore\x12>\n\x0b\x65poch_event\x18\x83\x01 \x01(\x0b\x32\x1a.vega.events.v1.EpochEventH\x00R\nepochEvent\x12M\n\x10validator_update\x18\x84\x01 \x01(\x0b\x32\x1f.vega.events.v1.ValidatorUpdateH\x00R\x0fvalidatorUpdate\x12\x44\n\rstake_linking\x18\x85\x01 \x01(\x0b\x32\x1c.vega.events.v1.StakeLinkingH\x00R\x0cstakeLinking\x12I\n\rreward_payout\x18\x86\x01 \x01(\x0b\x32!.vega.events.v1.RewardPayoutEventH\x00R\x0crewardPayout\x12\x42\n\ncheckpoint\x18\x87\x01 \x01(\x0b\x32\x1f.vega.events.v1.CheckpointEventH\x00R\ncheckpoint\x12\x41\n\x0ckey_rotation\x18\x88\x01 \x01(\x0b\x32\x1b.vega.events.v1.KeyRotationH\x00R\x0bkeyRotation\x12\x38\n\tstate_var\x18\x89\x01 \x01(\x0b\x32\x18.vega.events.v1.StateVarH\x00R\x08stateVar\x12=\n\x0enetwork_limits\x18\x8a\x01 \x01(\x0b\x32\x13.vega.NetworkLimitsH\x00R\rnetworkLimits\x12\x37\n\x08transfer\x18\x8b\x01 \x01(\x0b\x32\x18.vega.events.v1.TransferH\x00R\x08transfer\x12M\n\rranking_event\x18\x8c\x01 \x01(\x0b\x32%.vega.events.v1.ValidatorRankingEventH\x00R\x0crankingEvent\x12j\n\x1b\x65rc20_multisig_signer_event\x18\x8d\x01 \x01(\x0b\x32(.vega.events.v1.ERC20MultiSigSignerEventH\x00R\x18\x65rc20MultisigSignerEvent\x12}\n"erc20_multisig_set_threshold_event\x18\x8e\x01 \x01(\x0b\x32..vega.events.v1.ERC20MultiSigThresholdSetEventH\x00R\x1e\x65rc20MultisigSetThresholdEvent\x12j\n\x1b\x65rc20_multisig_signer_added\x18\x8f\x01 \x01(\x0b\x32(.vega.events.v1.ERC20MultiSigSignerAddedH\x00R\x18\x65rc20MultisigSignerAdded\x12p\n\x1d\x65rc20_multisig_signer_removed\x18\x90\x01 \x01(\x0b\x32*.vega.events.v1.ERC20MultiSigSignerRemovedH\x00R\x1a\x65rc20MultisigSignerRemoved\x12W\n\x14position_state_event\x18\x91\x01 \x01(\x0b\x32".vega.events.v1.PositionStateEventH\x00R\x12positionStateEvent\x12Z\n\x15\x65thereum_key_rotation\x18\x92\x01 \x01(\x0b\x32#.vega.events.v1.EthereumKeyRotationH\x00R\x13\x65thereumKeyRotation\x12]\n\x16protocol_upgrade_event\x18\x93\x01 \x01(\x0b\x32$.vega.events.v1.ProtocolUpgradeEventH\x00R\x14protocolUpgradeEvent\x12>\n\x0b\x62\x65gin_block\x18\x94\x01 \x01(\x0b\x32\x1a.vega.events.v1.BeginBlockH\x00R\nbeginBlock\x12\x38\n\tend_block\x18\x95\x01 \x01(\x0b\x32\x18.vega.events.v1.EndBlockH\x00R\x08\x65ndBlock\x12\x63\n\x18protocol_upgrade_started\x18\x96\x01 \x01(\x0b\x32&.vega.events.v1.ProtocolUpgradeStartedH\x00R\x16protocolUpgradeStarted\x12\x44\n\rsettle_market\x18\x97\x01 \x01(\x0b\x32\x1c.vega.events.v1.SettleMarketH\x00R\x0csettleMarket\x12S\n\x12transaction_result\x18\x98\x01 \x01(\x0b\x32!.vega.events.v1.TransactionResultH\x00R\x11transactionResult\x12S\n\x13\x63ore_snapshot_event\x18\x99\x01 \x01(\x0b\x32 .vega.events.v1.CoreSnapshotDataH\x00R\x11\x63oreSnapshotEvent\x12w\n protocol_upgrade_data_node_ready\x18\x9a\x01 \x01(\x0b\x32,.vega.events.v1.ProtocolUpgradeDataNodeReadyH\x00R\x1cprotocolUpgradeDataNodeReady\x12P\n\x11\x64istressed_orders\x18\x9b\x01 \x01(\x0b\x32 .vega.events.v1.DistressedOrdersH\x00R\x10\x64istressedOrders\x12\x36\n\x06market\x18\xe9\x07 \x01(\x0b\x32\x1b.vega.events.v1.MarketEventH\x00R\x06market\x12\x41\n\x0ctx_err_event\x18\xd1\x0f \x01(\x0b\x32\x1c.vega.events.v1.TxErrorEventH\x00R\ntxErrEvent\x12\x18\n\x07version\x18\x04 \x01(\rR\x07version\x12\x19\n\x08\x63hain_id\x18\x05 \x01(\tR\x07\x63hainId\x12\x17\n\x07tx_hash\x18\x06 \x01(\tR\x06txHashB\x07\n\x05\x65vent*\xdd\x01\n\x1dProtocolUpgradeProposalStatus\x12\x30\n,PROTOCOL_UPGRADE_PROPOSAL_STATUS_UNSPECIFIED\x10\x00\x12,\n(PROTOCOL_UPGRADE_PROPOSAL_STATUS_PENDING\x10\x01\x12-\n)PROTOCOL_UPGRADE_PROPOSAL_STATUS_APPROVED\x10\x02\x12-\n)PROTOCOL_UPGRADE_PROPOSAL_STATUS_REJECTED\x10\x03*\xa2\x10\n\x0c\x42usEventType\x12\x1e\n\x1a\x42US_EVENT_TYPE_UNSPECIFIED\x10\x00\x12\x16\n\x12\x42US_EVENT_TYPE_ALL\x10\x01\x12\x1e\n\x1a\x42US_EVENT_TYPE_TIME_UPDATE\x10\x02\x12#\n\x1f\x42US_EVENT_TYPE_LEDGER_MOVEMENTS\x10\x03\x12&\n"BUS_EVENT_TYPE_POSITION_RESOLUTION\x10\x04\x12\x18\n\x14\x42US_EVENT_TYPE_ORDER\x10\x05\x12\x1a\n\x16\x42US_EVENT_TYPE_ACCOUNT\x10\x06\x12\x18\n\x14\x42US_EVENT_TYPE_PARTY\x10\x07\x12\x18\n\x14\x42US_EVENT_TYPE_TRADE\x10\x08\x12 \n\x1c\x42US_EVENT_TYPE_MARGIN_LEVELS\x10\t\x12\x1b\n\x17\x42US_EVENT_TYPE_PROPOSAL\x10\n\x12\x17\n\x13\x42US_EVENT_TYPE_VOTE\x10\x0b\x12\x1e\n\x1a\x42US_EVENT_TYPE_MARKET_DATA\x10\x0c\x12!\n\x1d\x42US_EVENT_TYPE_NODE_SIGNATURE\x10\r\x12%\n!BUS_EVENT_TYPE_LOSS_SOCIALIZATION\x10\x0e\x12"\n\x1e\x42US_EVENT_TYPE_SETTLE_POSITION\x10\x0f\x12$\n BUS_EVENT_TYPE_SETTLE_DISTRESSED\x10\x10\x12!\n\x1d\x42US_EVENT_TYPE_MARKET_CREATED\x10\x11\x12\x18\n\x14\x42US_EVENT_TYPE_ASSET\x10\x12\x12\x1e\n\x1a\x42US_EVENT_TYPE_MARKET_TICK\x10\x13\x12\x1d\n\x19\x42US_EVENT_TYPE_WITHDRAWAL\x10\x14\x12\x1a\n\x16\x42US_EVENT_TYPE_DEPOSIT\x10\x15\x12\x1a\n\x16\x42US_EVENT_TYPE_AUCTION\x10\x16\x12\x1e\n\x1a\x42US_EVENT_TYPE_RISK_FACTOR\x10\x17\x12$\n BUS_EVENT_TYPE_NETWORK_PARAMETER\x10\x18\x12&\n"BUS_EVENT_TYPE_LIQUIDITY_PROVISION\x10\x19\x12!\n\x1d\x42US_EVENT_TYPE_MARKET_UPDATED\x10\x1a\x12\x1e\n\x1a\x42US_EVENT_TYPE_ORACLE_SPEC\x10\x1b\x12\x1e\n\x1a\x42US_EVENT_TYPE_ORACLE_DATA\x10\x1c\x12%\n!BUS_EVENT_TYPE_DELEGATION_BALANCE\x10\x1d\x12"\n\x1e\x42US_EVENT_TYPE_VALIDATOR_SCORE\x10\x1e\x12\x1f\n\x1b\x42US_EVENT_TYPE_EPOCH_UPDATE\x10\x1f\x12#\n\x1f\x42US_EVENT_TYPE_VALIDATOR_UPDATE\x10 \x12 \n\x1c\x42US_EVENT_TYPE_STAKE_LINKING\x10!\x12&\n"BUS_EVENT_TYPE_REWARD_PAYOUT_EVENT\x10"\x12\x1d\n\x19\x42US_EVENT_TYPE_CHECKPOINT\x10#\x12\x1f\n\x1b\x42US_EVENT_TYPE_STREAM_START\x10$\x12\x1f\n\x1b\x42US_EVENT_TYPE_KEY_ROTATION\x10%\x12\x1c\n\x18\x42US_EVENT_TYPE_STATE_VAR\x10&\x12!\n\x1d\x42US_EVENT_TYPE_NETWORK_LIMITS\x10\'\x12\x1b\n\x17\x42US_EVENT_TYPE_TRANSFER\x10(\x12$\n BUS_EVENT_TYPE_VALIDATOR_RANKING\x10)\x12/\n+BUS_EVENT_TYPE_ERC20_MULTI_SIG_SIGNER_EVENT\x10*\x12\x30\n,BUS_EVENT_TYPE_ERC20_MULTI_SIG_SET_THRESHOLD\x10+\x12/\n+BUS_EVENT_TYPE_ERC20_MULTI_SIG_SIGNER_ADDED\x10,\x12\x31\n-BUS_EVENT_TYPE_ERC20_MULTI_SIG_SIGNER_REMOVED\x10-\x12!\n\x1d\x42US_EVENT_TYPE_POSITION_STATE\x10.\x12(\n$BUS_EVENT_TYPE_ETHEREUM_KEY_ROTATION\x10/\x12,\n(BUS_EVENT_TYPE_PROTOCOL_UPGRADE_PROPOSAL\x10\x30\x12\x1e\n\x1a\x42US_EVENT_TYPE_BEGIN_BLOCK\x10\x31\x12\x1c\n\x18\x42US_EVENT_TYPE_END_BLOCK\x10\x32\x12+\n\'BUS_EVENT_TYPE_PROTOCOL_UPGRADE_STARTED\x10\x33\x12 \n\x1c\x42US_EVENT_TYPE_SETTLE_MARKET\x10\x34\x12%\n!BUS_EVENT_TYPE_TRANSACTION_RESULT\x10\x35\x12!\n\x1d\x42US_EVENT_TYPE_SNAPSHOT_TAKEN\x10\x36\x12\x33\n/BUS_EVENT_TYPE_PROTOCOL_UPGRADE_DATA_NODE_READY\x10\x37\x12+\n\'BUS_EVENT_TYPE_DISTRESSED_ORDERS_CLOSED\x10\x38\x12\x19\n\x15\x42US_EVENT_TYPE_MARKET\x10\x65\x12\x1c\n\x17\x42US_EVENT_TYPE_TX_ERROR\x10\xc9\x01\x42\x31Z/code.vegaprotocol.io/vega/protos/vega/events/v1b\x06proto3'
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(
     DESCRIPTOR, "vega.events.v1.events_pb2", globals()
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = (
         b"Z/code.vegaprotocol.io/vega/protos/vega/events/v1"
     )
-    _PROTOCOLUPGRADEPROPOSALSTATUS._serialized_start = 15186
-    _PROTOCOLUPGRADEPROPOSALSTATUS._serialized_end = 15407
-    _BUSEVENTTYPE._serialized_start = 15410
-    _BUSEVENTTYPE._serialized_end = 17447
+    _PROTOCOLUPGRADEPROPOSALSTATUS._serialized_start = 15343
+    _PROTOCOLUPGRADEPROPOSALSTATUS._serialized_end = 15564
+    _BUSEVENTTYPE._serialized_start = 15567
+    _BUSEVENTTYPE._serialized_end = 17649
     _ERC20MULTISIGSIGNERADDED._serialized_start = 251
     _ERC20MULTISIGSIGNERADDED._serialized_end = 489
     _ERC20MULTISIGSIGNERREMOVEDSUBMITTER._serialized_start = 491
     _ERC20MULTISIGSIGNERREMOVEDSUBMITTER._serialized_end = 593
     _ERC20MULTISIGSIGNERREMOVED._serialized_start = 596
     _ERC20MULTISIGSIGNERREMOVED._serialized_end = 875
     _TRANSFER._serialized_start = 878
@@ -104,36 +103,38 @@
     _SETTLEPOSITION._serialized_end = 8585
     _SETTLEMARKET._serialized_start = 8587
     _SETTLEMARKET._serialized_end = 8693
     _POSITIONSTATEEVENT._serialized_start = 8696
     _POSITIONSTATEEVENT._serialized_end = 8942
     _SETTLEDISTRESSED._serialized_start = 8944
     _SETTLEDISTRESSED._serialized_end = 9064
-    _MARKETTICK._serialized_start = 9066
-    _MARKETTICK._serialized_end = 9114
-    _AUCTIONEVENT._serialized_start = 9117
-    _AUCTIONEVENT._serialized_end = 9378
-    _VALIDATORUPDATE._serialized_start = 9381
-    _VALIDATORUPDATE._serialized_end = 9806
-    _VALIDATORRANKINGEVENT._serialized_start = 9809
-    _VALIDATORRANKINGEVENT._serialized_end = 10115
-    _KEYROTATION._serialized_start = 10118
-    _KEYROTATION._serialized_end = 10255
-    _ETHEREUMKEYROTATION._serialized_start = 10258
-    _ETHEREUMKEYROTATION._serialized_end = 10405
-    _PROTOCOLUPGRADEEVENT._serialized_start = 10408
-    _PROTOCOLUPGRADEEVENT._serialized_end = 10623
-    _STATEVAR._serialized_start = 10625
-    _STATEVAR._serialized_end = 10700
-    _BEGINBLOCK._serialized_start = 10702
-    _BEGINBLOCK._serialized_end = 10788
-    _ENDBLOCK._serialized_start = 10790
-    _ENDBLOCK._serialized_end = 10824
-    _PROTOCOLUPGRADESTARTED._serialized_start = 10826
-    _PROTOCOLUPGRADESTARTED._serialized_end = 10894
-    _PROTOCOLUPGRADEDATANODEREADY._serialized_start = 10896
-    _PROTOCOLUPGRADEDATANODEREADY._serialized_end = 10970
-    _CORESNAPSHOTDATA._serialized_start = 10973
-    _CORESNAPSHOTDATA._serialized_end = 11146
-    _BUSEVENT._serialized_start = 11149
-    _BUSEVENT._serialized_end = 15183
+    _DISTRESSEDORDERS._serialized_start = 9066
+    _DISTRESSEDORDERS._serialized_end = 9139
+    _MARKETTICK._serialized_start = 9141
+    _MARKETTICK._serialized_end = 9189
+    _AUCTIONEVENT._serialized_start = 9192
+    _AUCTIONEVENT._serialized_end = 9453
+    _VALIDATORUPDATE._serialized_start = 9456
+    _VALIDATORUPDATE._serialized_end = 9881
+    _VALIDATORRANKINGEVENT._serialized_start = 9884
+    _VALIDATORRANKINGEVENT._serialized_end = 10190
+    _KEYROTATION._serialized_start = 10193
+    _KEYROTATION._serialized_end = 10330
+    _ETHEREUMKEYROTATION._serialized_start = 10333
+    _ETHEREUMKEYROTATION._serialized_end = 10480
+    _PROTOCOLUPGRADEEVENT._serialized_start = 10483
+    _PROTOCOLUPGRADEEVENT._serialized_end = 10698
+    _STATEVAR._serialized_start = 10700
+    _STATEVAR._serialized_end = 10775
+    _BEGINBLOCK._serialized_start = 10777
+    _BEGINBLOCK._serialized_end = 10863
+    _ENDBLOCK._serialized_start = 10865
+    _ENDBLOCK._serialized_end = 10899
+    _PROTOCOLUPGRADESTARTED._serialized_start = 10901
+    _PROTOCOLUPGRADESTARTED._serialized_end = 10969
+    _PROTOCOLUPGRADEDATANODEREADY._serialized_start = 10971
+    _PROTOCOLUPGRADEDATANODEREADY._serialized_end = 11045
+    _CORESNAPSHOTDATA._serialized_start = 11048
+    _CORESNAPSHOTDATA._serialized_end = 11221
+    _BUSEVENT._serialized_start = 11224
+    _BUSEVENT._serialized_end = 15340
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-0.67.0/vega_sim/proto/vega/governance_pb2.py` & `vega_sim-1.0.1/vega_sim/proto/vega/governance_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,65 +15,64 @@
 from . import markets_pb2 as vega_dot_markets__pb2
 from . import vega_pb2 as vega_dot_vega__pb2
 from . import assets_pb2 as vega_dot_assets__pb2
 from . import data_source_pb2 as vega_dot_data__source__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x15vega/governance.proto\x12\x04vega\x1a\x12vega/markets.proto\x1a\x0fvega/vega.proto\x1a\x11vega/assets.proto\x1a\x16vega/data_source.proto"\x95\x03\n\rFutureProduct\x12)\n\x10settlement_asset\x18\x01 \x01(\tR\x0fsettlementAsset\x12\x1d\n\nquote_name\x18\x02 \x01(\tR\tquoteName\x12i\n$data_source_spec_for_settlement_data\x18\x03 \x01(\x0b\x32\x1a.vega.DataSourceDefinitionR\x1f\x64\x61taSourceSpecForSettlementData\x12q\n(data_source_spec_for_trading_termination\x18\x04 \x01(\x0b\x32\x1a.vega.DataSourceDefinitionR#dataSourceSpecForTradingTermination\x12\\\n\x18\x64\x61ta_source_spec_binding\x18\x05 \x01(\x0b\x32#.vega.DataSourceSpecToFutureBindingR\x15\x64\x61taSourceSpecBinding"{\n\x17InstrumentConfiguration\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x12\n\x04\x63ode\x18\x02 \x01(\tR\x04\x63ode\x12-\n\x06\x66uture\x18\x64 \x01(\x0b\x32\x13.vega.FutureProductH\x00R\x06\x66utureB\t\n\x07product"\xc7\x04\n\x16NewMarketConfiguration\x12=\n\ninstrument\x18\x01 \x01(\x0b\x32\x1d.vega.InstrumentConfigurationR\ninstrument\x12%\n\x0e\x64\x65\x63imal_places\x18\x02 \x01(\x04R\rdecimalPlaces\x12\x1a\n\x08metadata\x18\x03 \x03(\tR\x08metadata\x12_\n\x1bprice_monitoring_parameters\x18\x04 \x01(\x0b\x32\x1f.vega.PriceMonitoringParametersR\x19priceMonitoringParameters\x12k\n\x1fliquidity_monitoring_parameters\x18\x05 \x01(\x0b\x32#.vega.LiquidityMonitoringParametersR\x1dliquidityMonitoringParameters\x12\x31\n\x06simple\x18\x64 \x01(\x0b\x32\x17.vega.SimpleModelParamsH\x00R\x06simple\x12\x39\n\nlog_normal\x18\x65 \x01(\x0b\x32\x18.vega.LogNormalRiskModelH\x00R\tlogNormal\x12\x36\n\x17position_decimal_places\x18\x06 \x01(\x03R\x15positionDecimalPlaces\x12$\n\x0elp_price_range\x18\x08 \x01(\tR\x0clpPriceRangeB\x11\n\x0frisk_parameters"C\n\tNewMarket\x12\x36\n\x07\x63hanges\x18\x01 \x01(\x0b\x32\x1c.vega.NewMarketConfigurationR\x07\x63hanges"f\n\x0cUpdateMarket\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x39\n\x07\x63hanges\x18\x02 \x01(\x0b\x32\x1f.vega.UpdateMarketConfigurationR\x07\x63hanges"\xf1\x03\n\x19UpdateMarketConfiguration\x12\x43\n\ninstrument\x18\x01 \x01(\x0b\x32#.vega.UpdateInstrumentConfigurationR\ninstrument\x12\x1a\n\x08metadata\x18\x02 \x03(\tR\x08metadata\x12_\n\x1bprice_monitoring_parameters\x18\x03 \x01(\x0b\x32\x1f.vega.PriceMonitoringParametersR\x19priceMonitoringParameters\x12k\n\x1fliquidity_monitoring_parameters\x18\x04 \x01(\x0b\x32#.vega.LiquidityMonitoringParametersR\x1dliquidityMonitoringParameters\x12\x31\n\x06simple\x18\x64 \x01(\x0b\x32\x17.vega.SimpleModelParamsH\x00R\x06simple\x12\x39\n\nlog_normal\x18\x65 \x01(\x0b\x32\x18.vega.LogNormalRiskModelH\x00R\tlogNormal\x12$\n\x0elp_price_range\x18\x05 \x01(\tR\x0clpPriceRangeB\x11\n\x0frisk_parameters"s\n\x1dUpdateInstrumentConfiguration\x12\x12\n\x04\x63ode\x18\x01 \x01(\tR\x04\x63ode\x12\x33\n\x06\x66uture\x18\x64 \x01(\x0b\x32\x19.vega.UpdateFutureProductH\x00R\x06\x66utureB\t\n\x07product"\xf0\x02\n\x13UpdateFutureProduct\x12\x1d\n\nquote_name\x18\x01 \x01(\tR\tquoteName\x12i\n$data_source_spec_for_settlement_data\x18\x02 \x01(\x0b\x32\x1a.vega.DataSourceDefinitionR\x1f\x64\x61taSourceSpecForSettlementData\x12q\n(data_source_spec_for_trading_termination\x18\x03 \x01(\x0b\x32\x1a.vega.DataSourceDefinitionR#dataSourceSpecForTradingTermination\x12\\\n\x18\x64\x61ta_source_spec_binding\x18\x04 \x01(\x0b\x32#.vega.DataSourceSpecToFutureBindingR\x15\x64\x61taSourceSpecBinding"J\n\x16UpdateNetworkParameter\x12\x30\n\x07\x63hanges\x18\x01 \x01(\x0b\x32\x16.vega.NetworkParameterR\x07\x63hanges"8\n\x08NewAsset\x12,\n\x07\x63hanges\x18\x01 \x01(\x0b\x32\x12.vega.AssetDetailsR\x07\x63hanges"\\\n\x0bUpdateAsset\x12\x19\n\x08\x61sset_id\x18\x01 \x01(\tR\x07\x61ssetId\x12\x32\n\x07\x63hanges\x18\x02 \x01(\x0b\x32\x18.vega.AssetDetailsUpdateR\x07\x63hanges"\r\n\x0bNewFreeform"\x90\x04\n\rProposalTerms\x12+\n\x11\x63losing_timestamp\x18\x01 \x01(\x03R\x10\x63losingTimestamp\x12/\n\x13\x65nactment_timestamp\x18\x02 \x01(\x03R\x12\x65nactmentTimestamp\x12\x31\n\x14validation_timestamp\x18\x03 \x01(\x03R\x13validationTimestamp\x12\x39\n\rupdate_market\x18\x65 \x01(\x0b\x32\x12.vega.UpdateMarketH\x00R\x0cupdateMarket\x12\x30\n\nnew_market\x18\x66 \x01(\x0b\x32\x0f.vega.NewMarketH\x00R\tnewMarket\x12X\n\x18update_network_parameter\x18g \x01(\x0b\x32\x1c.vega.UpdateNetworkParameterH\x00R\x16updateNetworkParameter\x12-\n\tnew_asset\x18h \x01(\x0b\x32\x0e.vega.NewAssetH\x00R\x08newAsset\x12\x36\n\x0cnew_freeform\x18i \x01(\x0b\x32\x11.vega.NewFreeformH\x00R\x0bnewFreeform\x12\x36\n\x0cupdate_asset\x18j \x01(\x0b\x32\x11.vega.UpdateAssetH\x00R\x0bupdateAssetB\x08\n\x06\x63hange"W\n\x11ProposalRationale\x12 \n\x0b\x64\x65scription\x18\x01 \x01(\tR\x0b\x64\x65scription\x12\x14\n\x05title\x18\x04 \x01(\tR\x05titleJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04"\x86\x03\n\x0eGovernanceData\x12*\n\x08proposal\x18\x01 \x01(\x0b\x32\x0e.vega.ProposalR\x08proposal\x12\x1c\n\x03yes\x18\x02 \x03(\x0b\x32\n.vega.VoteR\x03yes\x12\x1a\n\x02no\x18\x03 \x03(\x0b\x32\n.vega.VoteR\x02no\x12?\n\tyes_party\x18\x04 \x03(\x0b\x32".vega.GovernanceData.YesPartyEntryR\x08yesParty\x12<\n\x08no_party\x18\x05 \x03(\x0b\x32!.vega.GovernanceData.NoPartyEntryR\x07noParty\x1aG\n\rYesPartyEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12 \n\x05value\x18\x02 \x01(\x0b\x32\n.vega.VoteR\x05value:\x02\x38\x01\x1a\x46\n\x0cNoPartyEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12 \n\x05value\x18\x02 \x01(\x0b\x32\n.vega.VoteR\x05value:\x02\x38\x01"\x9a\x07\n\x08Proposal\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1c\n\treference\x18\x02 \x01(\tR\treference\x12\x19\n\x08party_id\x18\x03 \x01(\tR\x07partyId\x12*\n\x05state\x18\x04 \x01(\x0e\x32\x14.vega.Proposal.StateR\x05state\x12\x1c\n\ttimestamp\x18\x05 \x01(\x03R\ttimestamp\x12)\n\x05terms\x18\x06 \x01(\x0b\x32\x13.vega.ProposalTermsR\x05terms\x12\x30\n\x06reason\x18\x07 \x01(\x0e\x32\x13.vega.ProposalErrorH\x00R\x06reason\x88\x01\x01\x12(\n\rerror_details\x18\x08 \x01(\tH\x01R\x0c\x65rrorDetails\x88\x01\x01\x12\x35\n\trationale\x18\t \x01(\x0b\x32\x17.vega.ProposalRationaleR\trationale\x12\x35\n\x16required_participation\x18\n \x01(\tR\x15requiredParticipation\x12+\n\x11required_majority\x18\x0b \x01(\tR\x10requiredMajority\x12^\n)required_liquidity_provider_participation\x18\x0c \x01(\tH\x02R&requiredLiquidityProviderParticipation\x88\x01\x01\x12T\n$required_liquidity_provider_majority\x18\r \x01(\tH\x03R!requiredLiquidityProviderMajority\x88\x01\x01"\xae\x01\n\x05State\x12\x15\n\x11STATE_UNSPECIFIED\x10\x00\x12\x10\n\x0cSTATE_FAILED\x10\x01\x12\x0e\n\nSTATE_OPEN\x10\x02\x12\x10\n\x0cSTATE_PASSED\x10\x03\x12\x12\n\x0eSTATE_REJECTED\x10\x04\x12\x12\n\x0eSTATE_DECLINED\x10\x05\x12\x11\n\rSTATE_ENACTED\x10\x06\x12\x1f\n\x1bSTATE_WAITING_FOR_NODE_VOTE\x10\x07\x42\t\n\x07_reasonB\x10\n\x0e_error_detailsB,\n*_required_liquidity_provider_participationB\'\n%_required_liquidity_provider_majority"\x91\x03\n\x04Vote\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12&\n\x05value\x18\x02 \x01(\x0e\x32\x10.vega.Vote.ValueR\x05value\x12\x1f\n\x0bproposal_id\x18\x03 \x01(\tR\nproposalId\x12\x1c\n\ttimestamp\x18\x04 \x01(\x03R\ttimestamp\x12\x43\n\x1etotal_governance_token_balance\x18\x05 \x01(\tR\x1btotalGovernanceTokenBalance\x12\x41\n\x1dtotal_governance_token_weight\x18\x06 \x01(\tR\x1atotalGovernanceTokenWeight\x12\x42\n\x1etotal_equity_like_share_weight\x18\x07 \x01(\tR\x1atotalEquityLikeShareWeight";\n\x05Value\x12\x15\n\x11VALUE_UNSPECIFIED\x10\x00\x12\x0c\n\x08VALUE_NO\x10\x01\x12\r\n\tVALUE_YES\x10\x02*\xad\r\n\rProposalError\x12\x1e\n\x1aPROPOSAL_ERROR_UNSPECIFIED\x10\x00\x12&\n"PROPOSAL_ERROR_CLOSE_TIME_TOO_SOON\x10\x01\x12&\n"PROPOSAL_ERROR_CLOSE_TIME_TOO_LATE\x10\x02\x12&\n"PROPOSAL_ERROR_ENACT_TIME_TOO_SOON\x10\x03\x12&\n"PROPOSAL_ERROR_ENACT_TIME_TOO_LATE\x10\x04\x12&\n"PROPOSAL_ERROR_INSUFFICIENT_TOKENS\x10\x05\x12.\n*PROPOSAL_ERROR_INVALID_INSTRUMENT_SECURITY\x10\x06\x12\x1d\n\x19PROPOSAL_ERROR_NO_PRODUCT\x10\x07\x12&\n"PROPOSAL_ERROR_UNSUPPORTED_PRODUCT\x10\x08\x12"\n\x1ePROPOSAL_ERROR_NO_TRADING_MODE\x10\x0b\x12+\n\'PROPOSAL_ERROR_UNSUPPORTED_TRADING_MODE\x10\x0c\x12)\n%PROPOSAL_ERROR_NODE_VALIDATION_FAILED\x10\r\x12.\n*PROPOSAL_ERROR_MISSING_BUILTIN_ASSET_FIELD\x10\x0e\x12\x31\n-PROPOSAL_ERROR_MISSING_ERC20_CONTRACT_ADDRESS\x10\x0f\x12 \n\x1cPROPOSAL_ERROR_INVALID_ASSET\x10\x10\x12*\n&PROPOSAL_ERROR_INCOMPATIBLE_TIMESTAMPS\x10\x11\x12%\n!PROPOSAL_ERROR_NO_RISK_PARAMETERS\x10\x12\x12\x30\n,PROPOSAL_ERROR_NETWORK_PARAMETER_INVALID_KEY\x10\x13\x12\x32\n.PROPOSAL_ERROR_NETWORK_PARAMETER_INVALID_VALUE\x10\x14\x12\x36\n2PROPOSAL_ERROR_NETWORK_PARAMETER_VALIDATION_FAILED\x10\x15\x12\x35\n1PROPOSAL_ERROR_OPENING_AUCTION_DURATION_TOO_SMALL\x10\x16\x12\x35\n1PROPOSAL_ERROR_OPENING_AUCTION_DURATION_TOO_LARGE\x10\x17\x12/\n+PROPOSAL_ERROR_COULD_NOT_INSTANTIATE_MARKET\x10\x19\x12)\n%PROPOSAL_ERROR_INVALID_FUTURE_PRODUCT\x10\x1a\x12)\n%PROPOSAL_ERROR_INVALID_RISK_PARAMETER\x10\x1e\x12\x31\n-PROPOSAL_ERROR_MAJORITY_THRESHOLD_NOT_REACHED\x10\x1f\x12\x36\n2PROPOSAL_ERROR_PARTICIPATION_THRESHOLD_NOT_REACHED\x10 \x12(\n$PROPOSAL_ERROR_INVALID_ASSET_DETAILS\x10!\x12\x1f\n\x1bPROPOSAL_ERROR_UNKNOWN_TYPE\x10"\x12.\n*PROPOSAL_ERROR_UNKNOWN_RISK_PARAMETER_TYPE\x10#\x12#\n\x1fPROPOSAL_ERROR_INVALID_FREEFORM\x10$\x12\x31\n-PROPOSAL_ERROR_INSUFFICIENT_EQUITY_LIKE_SHARE\x10%\x12!\n\x1dPROPOSAL_ERROR_INVALID_MARKET\x10&\x12\x31\n-PROPOSAL_ERROR_TOO_MANY_MARKET_DECIMAL_PLACES\x10\'\x12\x35\n1PROPOSAL_ERROR_TOO_MANY_PRICE_MONITORING_TRIGGERS\x10(\x12/\n+PROPOSAL_ERROR_ERC20_ADDRESS_ALREADY_IN_USE\x10)\x12-\n)PROPOSAL_ERROR_LP_PRICE_RANGE_NONPOSITIVE\x10*\x12+\n\'PROPOSAL_ERROR_LP_PRICE_RANGE_TOO_LARGE\x10+B\'Z%code.vegaprotocol.io/vega/protos/vegab\x06proto3'
+    b'\n\x15vega/governance.proto\x12\x04vega\x1a\x12vega/markets.proto\x1a\x0fvega/vega.proto\x1a\x11vega/assets.proto\x1a\x16vega/data_source.proto"\x95\x03\n\rFutureProduct\x12)\n\x10settlement_asset\x18\x01 \x01(\tR\x0fsettlementAsset\x12\x1d\n\nquote_name\x18\x02 \x01(\tR\tquoteName\x12i\n$data_source_spec_for_settlement_data\x18\x03 \x01(\x0b\x32\x1a.vega.DataSourceDefinitionR\x1f\x64\x61taSourceSpecForSettlementData\x12q\n(data_source_spec_for_trading_termination\x18\x04 \x01(\x0b\x32\x1a.vega.DataSourceDefinitionR#dataSourceSpecForTradingTermination\x12\\\n\x18\x64\x61ta_source_spec_binding\x18\x05 \x01(\x0b\x32#.vega.DataSourceSpecToFutureBindingR\x15\x64\x61taSourceSpecBinding"{\n\x17InstrumentConfiguration\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x12\n\x04\x63ode\x18\x02 \x01(\tR\x04\x63ode\x12-\n\x06\x66uture\x18\x64 \x01(\x0b\x32\x13.vega.FutureProductH\x00R\x06\x66utureB\t\n\x07product"\xb9\x05\n\x16NewMarketConfiguration\x12=\n\ninstrument\x18\x01 \x01(\x0b\x32\x1d.vega.InstrumentConfigurationR\ninstrument\x12%\n\x0e\x64\x65\x63imal_places\x18\x02 \x01(\x04R\rdecimalPlaces\x12\x1a\n\x08metadata\x18\x03 \x03(\tR\x08metadata\x12_\n\x1bprice_monitoring_parameters\x18\x04 \x01(\x0b\x32\x1f.vega.PriceMonitoringParametersR\x19priceMonitoringParameters\x12k\n\x1fliquidity_monitoring_parameters\x18\x05 \x01(\x0b\x32#.vega.LiquidityMonitoringParametersR\x1dliquidityMonitoringParameters\x12\x31\n\x06simple\x18\x64 \x01(\x0b\x32\x17.vega.SimpleModelParamsH\x00R\x06simple\x12\x39\n\nlog_normal\x18\x65 \x01(\x0b\x32\x18.vega.LogNormalRiskModelH\x00R\tlogNormal\x12\x36\n\x17position_decimal_places\x18\x06 \x01(\x03R\x15positionDecimalPlaces\x12$\n\x0elp_price_range\x18\x08 \x01(\tR\x0clpPriceRange\x12\x34\n\x16linear_slippage_factor\x18\t \x01(\tR\x14linearSlippageFactor\x12:\n\x19quadratic_slippage_factor\x18\n \x01(\tR\x17quadraticSlippageFactorB\x11\n\x0frisk_parameters"C\n\tNewMarket\x12\x36\n\x07\x63hanges\x18\x01 \x01(\x0b\x32\x1c.vega.NewMarketConfigurationR\x07\x63hanges"f\n\x0cUpdateMarket\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x39\n\x07\x63hanges\x18\x02 \x01(\x0b\x32\x1f.vega.UpdateMarketConfigurationR\x07\x63hanges"\xe3\x04\n\x19UpdateMarketConfiguration\x12\x43\n\ninstrument\x18\x01 \x01(\x0b\x32#.vega.UpdateInstrumentConfigurationR\ninstrument\x12\x1a\n\x08metadata\x18\x02 \x03(\tR\x08metadata\x12_\n\x1bprice_monitoring_parameters\x18\x03 \x01(\x0b\x32\x1f.vega.PriceMonitoringParametersR\x19priceMonitoringParameters\x12k\n\x1fliquidity_monitoring_parameters\x18\x04 \x01(\x0b\x32#.vega.LiquidityMonitoringParametersR\x1dliquidityMonitoringParameters\x12\x31\n\x06simple\x18\x64 \x01(\x0b\x32\x17.vega.SimpleModelParamsH\x00R\x06simple\x12\x39\n\nlog_normal\x18\x65 \x01(\x0b\x32\x18.vega.LogNormalRiskModelH\x00R\tlogNormal\x12$\n\x0elp_price_range\x18\x05 \x01(\tR\x0clpPriceRange\x12\x34\n\x16linear_slippage_factor\x18\x06 \x01(\tR\x14linearSlippageFactor\x12:\n\x19quadratic_slippage_factor\x18\x07 \x01(\tR\x17quadraticSlippageFactorB\x11\n\x0frisk_parameters"s\n\x1dUpdateInstrumentConfiguration\x12\x12\n\x04\x63ode\x18\x01 \x01(\tR\x04\x63ode\x12\x33\n\x06\x66uture\x18\x64 \x01(\x0b\x32\x19.vega.UpdateFutureProductH\x00R\x06\x66utureB\t\n\x07product"\xf0\x02\n\x13UpdateFutureProduct\x12\x1d\n\nquote_name\x18\x01 \x01(\tR\tquoteName\x12i\n$data_source_spec_for_settlement_data\x18\x02 \x01(\x0b\x32\x1a.vega.DataSourceDefinitionR\x1f\x64\x61taSourceSpecForSettlementData\x12q\n(data_source_spec_for_trading_termination\x18\x03 \x01(\x0b\x32\x1a.vega.DataSourceDefinitionR#dataSourceSpecForTradingTermination\x12\\\n\x18\x64\x61ta_source_spec_binding\x18\x04 \x01(\x0b\x32#.vega.DataSourceSpecToFutureBindingR\x15\x64\x61taSourceSpecBinding"J\n\x16UpdateNetworkParameter\x12\x30\n\x07\x63hanges\x18\x01 \x01(\x0b\x32\x16.vega.NetworkParameterR\x07\x63hanges"8\n\x08NewAsset\x12,\n\x07\x63hanges\x18\x01 \x01(\x0b\x32\x12.vega.AssetDetailsR\x07\x63hanges"\\\n\x0bUpdateAsset\x12\x19\n\x08\x61sset_id\x18\x01 \x01(\tR\x07\x61ssetId\x12\x32\n\x07\x63hanges\x18\x02 \x01(\x0b\x32\x18.vega.AssetDetailsUpdateR\x07\x63hanges"\r\n\x0bNewFreeform"\x90\x04\n\rProposalTerms\x12+\n\x11\x63losing_timestamp\x18\x01 \x01(\x03R\x10\x63losingTimestamp\x12/\n\x13\x65nactment_timestamp\x18\x02 \x01(\x03R\x12\x65nactmentTimestamp\x12\x31\n\x14validation_timestamp\x18\x03 \x01(\x03R\x13validationTimestamp\x12\x39\n\rupdate_market\x18\x65 \x01(\x0b\x32\x12.vega.UpdateMarketH\x00R\x0cupdateMarket\x12\x30\n\nnew_market\x18\x66 \x01(\x0b\x32\x0f.vega.NewMarketH\x00R\tnewMarket\x12X\n\x18update_network_parameter\x18g \x01(\x0b\x32\x1c.vega.UpdateNetworkParameterH\x00R\x16updateNetworkParameter\x12-\n\tnew_asset\x18h \x01(\x0b\x32\x0e.vega.NewAssetH\x00R\x08newAsset\x12\x36\n\x0cnew_freeform\x18i \x01(\x0b\x32\x11.vega.NewFreeformH\x00R\x0bnewFreeform\x12\x36\n\x0cupdate_asset\x18j \x01(\x0b\x32\x11.vega.UpdateAssetH\x00R\x0bupdateAssetB\x08\n\x06\x63hange"W\n\x11ProposalRationale\x12 \n\x0b\x64\x65scription\x18\x01 \x01(\tR\x0b\x64\x65scription\x12\x14\n\x05title\x18\x04 \x01(\tR\x05titleJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04"\x86\x03\n\x0eGovernanceData\x12*\n\x08proposal\x18\x01 \x01(\x0b\x32\x0e.vega.ProposalR\x08proposal\x12\x1c\n\x03yes\x18\x02 \x03(\x0b\x32\n.vega.VoteR\x03yes\x12\x1a\n\x02no\x18\x03 \x03(\x0b\x32\n.vega.VoteR\x02no\x12?\n\tyes_party\x18\x04 \x03(\x0b\x32".vega.GovernanceData.YesPartyEntryR\x08yesParty\x12<\n\x08no_party\x18\x05 \x03(\x0b\x32!.vega.GovernanceData.NoPartyEntryR\x07noParty\x1aG\n\rYesPartyEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12 \n\x05value\x18\x02 \x01(\x0b\x32\n.vega.VoteR\x05value:\x02\x38\x01\x1a\x46\n\x0cNoPartyEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12 \n\x05value\x18\x02 \x01(\x0b\x32\n.vega.VoteR\x05value:\x02\x38\x01"\x9a\x07\n\x08Proposal\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1c\n\treference\x18\x02 \x01(\tR\treference\x12\x19\n\x08party_id\x18\x03 \x01(\tR\x07partyId\x12*\n\x05state\x18\x04 \x01(\x0e\x32\x14.vega.Proposal.StateR\x05state\x12\x1c\n\ttimestamp\x18\x05 \x01(\x03R\ttimestamp\x12)\n\x05terms\x18\x06 \x01(\x0b\x32\x13.vega.ProposalTermsR\x05terms\x12\x30\n\x06reason\x18\x07 \x01(\x0e\x32\x13.vega.ProposalErrorH\x00R\x06reason\x88\x01\x01\x12(\n\rerror_details\x18\x08 \x01(\tH\x01R\x0c\x65rrorDetails\x88\x01\x01\x12\x35\n\trationale\x18\t \x01(\x0b\x32\x17.vega.ProposalRationaleR\trationale\x12\x35\n\x16required_participation\x18\n \x01(\tR\x15requiredParticipation\x12+\n\x11required_majority\x18\x0b \x01(\tR\x10requiredMajority\x12^\n)required_liquidity_provider_participation\x18\x0c \x01(\tH\x02R&requiredLiquidityProviderParticipation\x88\x01\x01\x12T\n$required_liquidity_provider_majority\x18\r \x01(\tH\x03R!requiredLiquidityProviderMajority\x88\x01\x01"\xae\x01\n\x05State\x12\x15\n\x11STATE_UNSPECIFIED\x10\x00\x12\x10\n\x0cSTATE_FAILED\x10\x01\x12\x0e\n\nSTATE_OPEN\x10\x02\x12\x10\n\x0cSTATE_PASSED\x10\x03\x12\x12\n\x0eSTATE_REJECTED\x10\x04\x12\x12\n\x0eSTATE_DECLINED\x10\x05\x12\x11\n\rSTATE_ENACTED\x10\x06\x12\x1f\n\x1bSTATE_WAITING_FOR_NODE_VOTE\x10\x07\x42\t\n\x07_reasonB\x10\n\x0e_error_detailsB,\n*_required_liquidity_provider_participationB\'\n%_required_liquidity_provider_majority"\x91\x03\n\x04Vote\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12&\n\x05value\x18\x02 \x01(\x0e\x32\x10.vega.Vote.ValueR\x05value\x12\x1f\n\x0bproposal_id\x18\x03 \x01(\tR\nproposalId\x12\x1c\n\ttimestamp\x18\x04 \x01(\x03R\ttimestamp\x12\x43\n\x1etotal_governance_token_balance\x18\x05 \x01(\tR\x1btotalGovernanceTokenBalance\x12\x41\n\x1dtotal_governance_token_weight\x18\x06 \x01(\tR\x1atotalGovernanceTokenWeight\x12\x42\n\x1etotal_equity_like_share_weight\x18\x07 \x01(\tR\x1atotalEquityLikeShareWeight";\n\x05Value\x12\x15\n\x11VALUE_UNSPECIFIED\x10\x00\x12\x0c\n\x08VALUE_NO\x10\x01\x12\r\n\tVALUE_YES\x10\x02*\xa0\x0e\n\rProposalError\x12\x1e\n\x1aPROPOSAL_ERROR_UNSPECIFIED\x10\x00\x12&\n"PROPOSAL_ERROR_CLOSE_TIME_TOO_SOON\x10\x01\x12&\n"PROPOSAL_ERROR_CLOSE_TIME_TOO_LATE\x10\x02\x12&\n"PROPOSAL_ERROR_ENACT_TIME_TOO_SOON\x10\x03\x12&\n"PROPOSAL_ERROR_ENACT_TIME_TOO_LATE\x10\x04\x12&\n"PROPOSAL_ERROR_INSUFFICIENT_TOKENS\x10\x05\x12.\n*PROPOSAL_ERROR_INVALID_INSTRUMENT_SECURITY\x10\x06\x12\x1d\n\x19PROPOSAL_ERROR_NO_PRODUCT\x10\x07\x12&\n"PROPOSAL_ERROR_UNSUPPORTED_PRODUCT\x10\x08\x12"\n\x1ePROPOSAL_ERROR_NO_TRADING_MODE\x10\x0b\x12+\n\'PROPOSAL_ERROR_UNSUPPORTED_TRADING_MODE\x10\x0c\x12)\n%PROPOSAL_ERROR_NODE_VALIDATION_FAILED\x10\r\x12.\n*PROPOSAL_ERROR_MISSING_BUILTIN_ASSET_FIELD\x10\x0e\x12\x31\n-PROPOSAL_ERROR_MISSING_ERC20_CONTRACT_ADDRESS\x10\x0f\x12 \n\x1cPROPOSAL_ERROR_INVALID_ASSET\x10\x10\x12*\n&PROPOSAL_ERROR_INCOMPATIBLE_TIMESTAMPS\x10\x11\x12%\n!PROPOSAL_ERROR_NO_RISK_PARAMETERS\x10\x12\x12\x30\n,PROPOSAL_ERROR_NETWORK_PARAMETER_INVALID_KEY\x10\x13\x12\x32\n.PROPOSAL_ERROR_NETWORK_PARAMETER_INVALID_VALUE\x10\x14\x12\x36\n2PROPOSAL_ERROR_NETWORK_PARAMETER_VALIDATION_FAILED\x10\x15\x12\x35\n1PROPOSAL_ERROR_OPENING_AUCTION_DURATION_TOO_SMALL\x10\x16\x12\x35\n1PROPOSAL_ERROR_OPENING_AUCTION_DURATION_TOO_LARGE\x10\x17\x12/\n+PROPOSAL_ERROR_COULD_NOT_INSTANTIATE_MARKET\x10\x19\x12)\n%PROPOSAL_ERROR_INVALID_FUTURE_PRODUCT\x10\x1a\x12)\n%PROPOSAL_ERROR_INVALID_RISK_PARAMETER\x10\x1e\x12\x31\n-PROPOSAL_ERROR_MAJORITY_THRESHOLD_NOT_REACHED\x10\x1f\x12\x36\n2PROPOSAL_ERROR_PARTICIPATION_THRESHOLD_NOT_REACHED\x10 \x12(\n$PROPOSAL_ERROR_INVALID_ASSET_DETAILS\x10!\x12\x1f\n\x1bPROPOSAL_ERROR_UNKNOWN_TYPE\x10"\x12.\n*PROPOSAL_ERROR_UNKNOWN_RISK_PARAMETER_TYPE\x10#\x12#\n\x1fPROPOSAL_ERROR_INVALID_FREEFORM\x10$\x12\x31\n-PROPOSAL_ERROR_INSUFFICIENT_EQUITY_LIKE_SHARE\x10%\x12!\n\x1dPROPOSAL_ERROR_INVALID_MARKET\x10&\x12\x31\n-PROPOSAL_ERROR_TOO_MANY_MARKET_DECIMAL_PLACES\x10\'\x12\x35\n1PROPOSAL_ERROR_TOO_MANY_PRICE_MONITORING_TRIGGERS\x10(\x12/\n+PROPOSAL_ERROR_ERC20_ADDRESS_ALREADY_IN_USE\x10)\x12-\n)PROPOSAL_ERROR_LP_PRICE_RANGE_NONPOSITIVE\x10*\x12+\n\'PROPOSAL_ERROR_LP_PRICE_RANGE_TOO_LARGE\x10+\x12\x36\n2PROPOSAL_ERROR_LINEAR_SLIPPAGE_FACTOR_OUT_OF_RANGE\x10,\x12\x39\n5PROPOSAL_ERROR_QUADRATIC_SLIPPAGE_FACTOR_OUT_OF_RANGE\x10-B\'Z%code.vegaprotocol.io/vega/protos/vegab\x06proto3'
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "vega.governance_pb2", globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b"Z%code.vegaprotocol.io/vega/protos/vega"
     _GOVERNANCEDATA_YESPARTYENTRY._options = None
     _GOVERNANCEDATA_YESPARTYENTRY._serialized_options = b"8\001"
     _GOVERNANCEDATA_NOPARTYENTRY._options = None
     _GOVERNANCEDATA_NOPARTYENTRY._serialized_options = b"8\001"
-    _PROPOSALERROR._serialized_start = 4977
-    _PROPOSALERROR._serialized_end = 6686
+    _PROPOSALERROR._serialized_start = 5205
+    _PROPOSALERROR._serialized_end = 7029
     _FUTUREPRODUCT._serialized_start = 112
     _FUTUREPRODUCT._serialized_end = 517
     _INSTRUMENTCONFIGURATION._serialized_start = 519
     _INSTRUMENTCONFIGURATION._serialized_end = 642
     _NEWMARKETCONFIGURATION._serialized_start = 645
-    _NEWMARKETCONFIGURATION._serialized_end = 1228
-    _NEWMARKET._serialized_start = 1230
-    _NEWMARKET._serialized_end = 1297
-    _UPDATEMARKET._serialized_start = 1299
-    _UPDATEMARKET._serialized_end = 1401
-    _UPDATEMARKETCONFIGURATION._serialized_start = 1404
-    _UPDATEMARKETCONFIGURATION._serialized_end = 1901
-    _UPDATEINSTRUMENTCONFIGURATION._serialized_start = 1903
-    _UPDATEINSTRUMENTCONFIGURATION._serialized_end = 2018
-    _UPDATEFUTUREPRODUCT._serialized_start = 2021
-    _UPDATEFUTUREPRODUCT._serialized_end = 2389
-    _UPDATENETWORKPARAMETER._serialized_start = 2391
-    _UPDATENETWORKPARAMETER._serialized_end = 2465
-    _NEWASSET._serialized_start = 2467
-    _NEWASSET._serialized_end = 2523
-    _UPDATEASSET._serialized_start = 2525
-    _UPDATEASSET._serialized_end = 2617
-    _NEWFREEFORM._serialized_start = 2619
-    _NEWFREEFORM._serialized_end = 2632
-    _PROPOSALTERMS._serialized_start = 2635
-    _PROPOSALTERMS._serialized_end = 3163
-    _PROPOSALRATIONALE._serialized_start = 3165
-    _PROPOSALRATIONALE._serialized_end = 3252
-    _GOVERNANCEDATA._serialized_start = 3255
-    _GOVERNANCEDATA._serialized_end = 3645
-    _GOVERNANCEDATA_YESPARTYENTRY._serialized_start = 3502
-    _GOVERNANCEDATA_YESPARTYENTRY._serialized_end = 3573
-    _GOVERNANCEDATA_NOPARTYENTRY._serialized_start = 3575
-    _GOVERNANCEDATA_NOPARTYENTRY._serialized_end = 3645
-    _PROPOSAL._serialized_start = 3648
-    _PROPOSAL._serialized_end = 4570
-    _PROPOSAL_STATE._serialized_start = 4280
-    _PROPOSAL_STATE._serialized_end = 4454
-    _VOTE._serialized_start = 4573
-    _VOTE._serialized_end = 4974
-    _VOTE_VALUE._serialized_start = 4915
-    _VOTE_VALUE._serialized_end = 4974
+    _NEWMARKETCONFIGURATION._serialized_end = 1342
+    _NEWMARKET._serialized_start = 1344
+    _NEWMARKET._serialized_end = 1411
+    _UPDATEMARKET._serialized_start = 1413
+    _UPDATEMARKET._serialized_end = 1515
+    _UPDATEMARKETCONFIGURATION._serialized_start = 1518
+    _UPDATEMARKETCONFIGURATION._serialized_end = 2129
+    _UPDATEINSTRUMENTCONFIGURATION._serialized_start = 2131
+    _UPDATEINSTRUMENTCONFIGURATION._serialized_end = 2246
+    _UPDATEFUTUREPRODUCT._serialized_start = 2249
+    _UPDATEFUTUREPRODUCT._serialized_end = 2617
+    _UPDATENETWORKPARAMETER._serialized_start = 2619
+    _UPDATENETWORKPARAMETER._serialized_end = 2693
+    _NEWASSET._serialized_start = 2695
+    _NEWASSET._serialized_end = 2751
+    _UPDATEASSET._serialized_start = 2753
+    _UPDATEASSET._serialized_end = 2845
+    _NEWFREEFORM._serialized_start = 2847
+    _NEWFREEFORM._serialized_end = 2860
+    _PROPOSALTERMS._serialized_start = 2863
+    _PROPOSALTERMS._serialized_end = 3391
+    _PROPOSALRATIONALE._serialized_start = 3393
+    _PROPOSALRATIONALE._serialized_end = 3480
+    _GOVERNANCEDATA._serialized_start = 3483
+    _GOVERNANCEDATA._serialized_end = 3873
+    _GOVERNANCEDATA_YESPARTYENTRY._serialized_start = 3730
+    _GOVERNANCEDATA_YESPARTYENTRY._serialized_end = 3801
+    _GOVERNANCEDATA_NOPARTYENTRY._serialized_start = 3803
+    _GOVERNANCEDATA_NOPARTYENTRY._serialized_end = 3873
+    _PROPOSAL._serialized_start = 3876
+    _PROPOSAL._serialized_end = 4798
+    _PROPOSAL_STATE._serialized_start = 4508
+    _PROPOSAL_STATE._serialized_end = 4682
+    _VOTE._serialized_start = 4801
+    _VOTE._serialized_end = 5202
+    _VOTE_VALUE._serialized_start = 5143
+    _VOTE_VALUE._serialized_end = 5202
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-0.67.0/vega_sim/proto/vega/markets_pb2.py` & `vega_sim-1.0.1/vega_sim/proto/vega/markets_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,21 +12,20 @@
 _sym_db = _symbol_database.Default()
 
 
 from . import data_source_pb2 as vega_dot_data__source__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x12vega/markets.proto\x12\x04vega\x1a\x16vega/data_source.proto"E\n\x0f\x41uctionDuration\x12\x1a\n\x08\x64uration\x18\x01 \x01(\x03R\x08\x64uration\x12\x16\n\x06volume\x18\x02 \x01(\x04R\x06volume"\x82\x03\n\x06\x46uture\x12)\n\x10settlement_asset\x18\x01 \x01(\tR\x0fsettlementAsset\x12\x1d\n\nquote_name\x18\x02 \x01(\tR\tquoteName\x12\x63\n$data_source_spec_for_settlement_data\x18\x03 \x01(\x0b\x32\x14.vega.DataSourceSpecR\x1f\x64\x61taSourceSpecForSettlementData\x12k\n(data_source_spec_for_trading_termination\x18\x04 \x01(\x0b\x32\x14.vega.DataSourceSpecR#dataSourceSpecForTradingTermination\x12\\\n\x18\x64\x61ta_source_spec_binding\x18\x05 \x01(\x0b\x32#.vega.DataSourceSpecToFutureBindingR\x15\x64\x61taSourceSpecBinding"\x9b\x01\n\x1d\x44\x61taSourceSpecToFutureBinding\x12\x38\n\x18settlement_data_property\x18\x01 \x01(\tR\x16settlementDataProperty\x12@\n\x1ctrading_termination_property\x18\x02 \x01(\tR\x1atradingTerminationProperty"(\n\x12InstrumentMetadata\x12\x12\n\x04tags\x18\x01 \x03(\tR\x04tags"\xad\x01\n\nInstrument\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04\x63ode\x18\x02 \x01(\tR\x04\x63ode\x12\x12\n\x04name\x18\x03 \x01(\tR\x04name\x12\x34\n\x08metadata\x18\x04 \x01(\x0b\x32\x18.vega.InstrumentMetadataR\x08metadata\x12&\n\x06\x66uture\x18\x64 \x01(\x0b\x32\x0c.vega.FutureH\x00R\x06\x66utureB\t\n\x07product"\x92\x01\n\x12LogNormalRiskModel\x12\x36\n\x17risk_aversion_parameter\x18\x01 \x01(\x01R\x15riskAversionParameter\x12\x10\n\x03tau\x18\x02 \x01(\x01R\x03tau\x12\x32\n\x06params\x18\x03 \x01(\x0b\x32\x1a.vega.LogNormalModelParamsR\x06params"J\n\x14LogNormalModelParams\x12\x0e\n\x02mu\x18\x01 \x01(\x01R\x02mu\x12\x0c\n\x01r\x18\x02 \x01(\x01R\x01r\x12\x14\n\x05sigma\x18\x03 \x01(\x01R\x05sigma"B\n\x0fSimpleRiskModel\x12/\n\x06params\x18\x01 \x01(\x0b\x32\x17.vega.SimpleModelParamsR\x06params"\xd1\x01\n\x11SimpleModelParams\x12\x1f\n\x0b\x66\x61\x63tor_long\x18\x01 \x01(\x01R\nfactorLong\x12!\n\x0c\x66\x61\x63tor_short\x18\x02 \x01(\x01R\x0b\x66\x61\x63torShort\x12\x1e\n\x0bmax_move_up\x18\x03 \x01(\x01R\tmaxMoveUp\x12"\n\rmin_move_down\x18\x04 \x01(\x01R\x0bminMoveDown\x12\x34\n\x16probability_of_trading\x18\x05 \x01(\x01R\x14probabilityOfTrading"\x89\x01\n\x0eScalingFactors\x12!\n\x0csearch_level\x18\x01 \x01(\x01R\x0bsearchLevel\x12%\n\x0einitial_margin\x18\x02 \x01(\x01R\rinitialMargin\x12-\n\x12\x63ollateral_release\x18\x03 \x01(\x01R\x11\x63ollateralRelease"Q\n\x10MarginCalculator\x12=\n\x0fscaling_factors\x18\x01 \x01(\x0b\x32\x14.vega.ScalingFactorsR\x0escalingFactors"\xad\x02\n\x12TradableInstrument\x12\x30\n\ninstrument\x18\x01 \x01(\x0b\x32\x10.vega.InstrumentR\ninstrument\x12\x43\n\x11margin_calculator\x18\x02 \x01(\x0b\x32\x16.vega.MarginCalculatorR\x10marginCalculator\x12M\n\x15log_normal_risk_model\x18\x64 \x01(\x0b\x32\x18.vega.LogNormalRiskModelH\x00R\x12logNormalRiskModel\x12\x43\n\x11simple_risk_model\x18\x65 \x01(\x0b\x32\x15.vega.SimpleRiskModelH\x00R\x0fsimpleRiskModelB\x0c\n\nrisk_model"}\n\nFeeFactors\x12\x1b\n\tmaker_fee\x18\x01 \x01(\tR\x08makerFee\x12-\n\x12infrastructure_fee\x18\x02 \x01(\tR\x11infrastructureFee\x12#\n\rliquidity_fee\x18\x03 \x01(\tR\x0cliquidityFee"2\n\x04\x46\x65\x65s\x12*\n\x07\x66\x61\x63tors\x18\x01 \x01(\x0b\x32\x10.vega.FeeFactorsR\x07\x66\x61\x63tors"\x81\x01\n\x16PriceMonitoringTrigger\x12\x18\n\x07horizon\x18\x01 \x01(\x03R\x07horizon\x12 \n\x0bprobability\x18\x02 \x01(\tR\x0bprobability\x12+\n\x11\x61uction_extension\x18\x03 \x01(\x03R\x10\x61uctionExtension"U\n\x19PriceMonitoringParameters\x12\x38\n\x08triggers\x18\x01 \x03(\x0b\x32\x1c.vega.PriceMonitoringTriggerR\x08triggers"Z\n\x17PriceMonitoringSettings\x12?\n\nparameters\x18\x01 \x01(\x0b\x32\x1f.vega.PriceMonitoringParametersR\nparameters"\xcc\x01\n\x1dLiquidityMonitoringParameters\x12S\n\x17target_stake_parameters\x18\x01 \x01(\x0b\x32\x1b.vega.TargetStakeParametersR\x15targetStakeParameters\x12)\n\x10triggering_ratio\x18\x02 \x01(\tR\x0ftriggeringRatio\x12+\n\x11\x61uction_extension\x18\x03 \x01(\x03R\x10\x61uctionExtension"_\n\x15TargetStakeParameters\x12\x1f\n\x0btime_window\x18\x01 \x01(\x03R\ntimeWindow\x12%\n\x0escaling_factor\x18\x02 \x01(\x01R\rscalingFactor"\xe6\x08\n\x06Market\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12I\n\x13tradable_instrument\x18\x02 \x01(\x0b\x32\x18.vega.TradableInstrumentR\x12tradableInstrument\x12%\n\x0e\x64\x65\x63imal_places\x18\x03 \x01(\x04R\rdecimalPlaces\x12\x1e\n\x04\x66\x65\x65s\x18\x04 \x01(\x0b\x32\n.vega.FeesR\x04\x66\x65\x65s\x12>\n\x0fopening_auction\x18\x05 \x01(\x0b\x32\x15.vega.AuctionDurationR\x0eopeningAuction\x12Y\n\x19price_monitoring_settings\x18\x06 \x01(\x0b\x32\x1d.vega.PriceMonitoringSettingsR\x17priceMonitoringSettings\x12k\n\x1fliquidity_monitoring_parameters\x18\x07 \x01(\x0b\x32#.vega.LiquidityMonitoringParametersR\x1dliquidityMonitoringParameters\x12;\n\x0ctrading_mode\x18\x08 \x01(\x0e\x32\x18.vega.Market.TradingModeR\x0btradingMode\x12(\n\x05state\x18\t \x01(\x0e\x32\x12.vega.Market.StateR\x05state\x12\x43\n\x11market_timestamps\x18\n \x01(\x0b\x32\x16.vega.MarketTimestampsR\x10marketTimestamps\x12\x36\n\x17position_decimal_places\x18\x0b \x01(\x03R\x15positionDecimalPlaces\x12$\n\x0elp_price_range\x18\x0c \x01(\tR\x0clpPriceRange"\xd8\x01\n\x05State\x12\x15\n\x11STATE_UNSPECIFIED\x10\x00\x12\x12\n\x0eSTATE_PROPOSED\x10\x01\x12\x12\n\x0eSTATE_REJECTED\x10\x02\x12\x11\n\rSTATE_PENDING\x10\x03\x12\x13\n\x0fSTATE_CANCELLED\x10\x04\x12\x10\n\x0cSTATE_ACTIVE\x10\x05\x12\x13\n\x0fSTATE_SUSPENDED\x10\x06\x12\x10\n\x0cSTATE_CLOSED\x10\x07\x12\x1c\n\x18STATE_TRADING_TERMINATED\x10\x08\x12\x11\n\rSTATE_SETTLED\x10\t"\xcc\x01\n\x0bTradingMode\x12\x1c\n\x18TRADING_MODE_UNSPECIFIED\x10\x00\x12\x1b\n\x17TRADING_MODE_CONTINUOUS\x10\x01\x12\x1e\n\x1aTRADING_MODE_BATCH_AUCTION\x10\x02\x12 \n\x1cTRADING_MODE_OPENING_AUCTION\x10\x03\x12#\n\x1fTRADING_MODE_MONITORING_AUCTION\x10\x04\x12\x1b\n\x17TRADING_MODE_NO_TRADING\x10\x05"r\n\x10MarketTimestamps\x12\x1a\n\x08proposed\x18\x01 \x01(\x03R\x08proposed\x12\x18\n\x07pending\x18\x02 \x01(\x03R\x07pending\x12\x12\n\x04open\x18\x03 \x01(\x03R\x04open\x12\x14\n\x05\x63lose\x18\x04 \x01(\x03R\x05\x63loseB\'Z%code.vegaprotocol.io/vega/protos/vegab\x06proto3'
+    b'\n\x12vega/markets.proto\x12\x04vega\x1a\x16vega/data_source.proto"E\n\x0f\x41uctionDuration\x12\x1a\n\x08\x64uration\x18\x01 \x01(\x03R\x08\x64uration\x12\x16\n\x06volume\x18\x02 \x01(\x04R\x06volume"\x82\x03\n\x06\x46uture\x12)\n\x10settlement_asset\x18\x01 \x01(\tR\x0fsettlementAsset\x12\x1d\n\nquote_name\x18\x02 \x01(\tR\tquoteName\x12\x63\n$data_source_spec_for_settlement_data\x18\x03 \x01(\x0b\x32\x14.vega.DataSourceSpecR\x1f\x64\x61taSourceSpecForSettlementData\x12k\n(data_source_spec_for_trading_termination\x18\x04 \x01(\x0b\x32\x14.vega.DataSourceSpecR#dataSourceSpecForTradingTermination\x12\\\n\x18\x64\x61ta_source_spec_binding\x18\x05 \x01(\x0b\x32#.vega.DataSourceSpecToFutureBindingR\x15\x64\x61taSourceSpecBinding"\x9b\x01\n\x1d\x44\x61taSourceSpecToFutureBinding\x12\x38\n\x18settlement_data_property\x18\x01 \x01(\tR\x16settlementDataProperty\x12@\n\x1ctrading_termination_property\x18\x02 \x01(\tR\x1atradingTerminationProperty"(\n\x12InstrumentMetadata\x12\x12\n\x04tags\x18\x01 \x03(\tR\x04tags"\xad\x01\n\nInstrument\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04\x63ode\x18\x02 \x01(\tR\x04\x63ode\x12\x12\n\x04name\x18\x03 \x01(\tR\x04name\x12\x34\n\x08metadata\x18\x04 \x01(\x0b\x32\x18.vega.InstrumentMetadataR\x08metadata\x12&\n\x06\x66uture\x18\x64 \x01(\x0b\x32\x0c.vega.FutureH\x00R\x06\x66utureB\t\n\x07product"\x92\x01\n\x12LogNormalRiskModel\x12\x36\n\x17risk_aversion_parameter\x18\x01 \x01(\x01R\x15riskAversionParameter\x12\x10\n\x03tau\x18\x02 \x01(\x01R\x03tau\x12\x32\n\x06params\x18\x03 \x01(\x0b\x32\x1a.vega.LogNormalModelParamsR\x06params"J\n\x14LogNormalModelParams\x12\x0e\n\x02mu\x18\x01 \x01(\x01R\x02mu\x12\x0c\n\x01r\x18\x02 \x01(\x01R\x01r\x12\x14\n\x05sigma\x18\x03 \x01(\x01R\x05sigma"B\n\x0fSimpleRiskModel\x12/\n\x06params\x18\x01 \x01(\x0b\x32\x17.vega.SimpleModelParamsR\x06params"\xd1\x01\n\x11SimpleModelParams\x12\x1f\n\x0b\x66\x61\x63tor_long\x18\x01 \x01(\x01R\nfactorLong\x12!\n\x0c\x66\x61\x63tor_short\x18\x02 \x01(\x01R\x0b\x66\x61\x63torShort\x12\x1e\n\x0bmax_move_up\x18\x03 \x01(\x01R\tmaxMoveUp\x12"\n\rmin_move_down\x18\x04 \x01(\x01R\x0bminMoveDown\x12\x34\n\x16probability_of_trading\x18\x05 \x01(\x01R\x14probabilityOfTrading"\x89\x01\n\x0eScalingFactors\x12!\n\x0csearch_level\x18\x01 \x01(\x01R\x0bsearchLevel\x12%\n\x0einitial_margin\x18\x02 \x01(\x01R\rinitialMargin\x12-\n\x12\x63ollateral_release\x18\x03 \x01(\x01R\x11\x63ollateralRelease"Q\n\x10MarginCalculator\x12=\n\x0fscaling_factors\x18\x01 \x01(\x0b\x32\x14.vega.ScalingFactorsR\x0escalingFactors"\xad\x02\n\x12TradableInstrument\x12\x30\n\ninstrument\x18\x01 \x01(\x0b\x32\x10.vega.InstrumentR\ninstrument\x12\x43\n\x11margin_calculator\x18\x02 \x01(\x0b\x32\x16.vega.MarginCalculatorR\x10marginCalculator\x12M\n\x15log_normal_risk_model\x18\x64 \x01(\x0b\x32\x18.vega.LogNormalRiskModelH\x00R\x12logNormalRiskModel\x12\x43\n\x11simple_risk_model\x18\x65 \x01(\x0b\x32\x15.vega.SimpleRiskModelH\x00R\x0fsimpleRiskModelB\x0c\n\nrisk_model"}\n\nFeeFactors\x12\x1b\n\tmaker_fee\x18\x01 \x01(\tR\x08makerFee\x12-\n\x12infrastructure_fee\x18\x02 \x01(\tR\x11infrastructureFee\x12#\n\rliquidity_fee\x18\x03 \x01(\tR\x0cliquidityFee"2\n\x04\x46\x65\x65s\x12*\n\x07\x66\x61\x63tors\x18\x01 \x01(\x0b\x32\x10.vega.FeeFactorsR\x07\x66\x61\x63tors"\x81\x01\n\x16PriceMonitoringTrigger\x12\x18\n\x07horizon\x18\x01 \x01(\x03R\x07horizon\x12 \n\x0bprobability\x18\x02 \x01(\tR\x0bprobability\x12+\n\x11\x61uction_extension\x18\x03 \x01(\x03R\x10\x61uctionExtension"U\n\x19PriceMonitoringParameters\x12\x38\n\x08triggers\x18\x01 \x03(\x0b\x32\x1c.vega.PriceMonitoringTriggerR\x08triggers"Z\n\x17PriceMonitoringSettings\x12?\n\nparameters\x18\x01 \x01(\x0b\x32\x1f.vega.PriceMonitoringParametersR\nparameters"\xcc\x01\n\x1dLiquidityMonitoringParameters\x12S\n\x17target_stake_parameters\x18\x01 \x01(\x0b\x32\x1b.vega.TargetStakeParametersR\x15targetStakeParameters\x12)\n\x10triggering_ratio\x18\x02 \x01(\tR\x0ftriggeringRatio\x12+\n\x11\x61uction_extension\x18\x03 \x01(\x03R\x10\x61uctionExtension"_\n\x15TargetStakeParameters\x12\x1f\n\x0btime_window\x18\x01 \x01(\x03R\ntimeWindow\x12%\n\x0escaling_factor\x18\x02 \x01(\x01R\rscalingFactor"\xd8\t\n\x06Market\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12I\n\x13tradable_instrument\x18\x02 \x01(\x0b\x32\x18.vega.TradableInstrumentR\x12tradableInstrument\x12%\n\x0e\x64\x65\x63imal_places\x18\x03 \x01(\x04R\rdecimalPlaces\x12\x1e\n\x04\x66\x65\x65s\x18\x04 \x01(\x0b\x32\n.vega.FeesR\x04\x66\x65\x65s\x12>\n\x0fopening_auction\x18\x05 \x01(\x0b\x32\x15.vega.AuctionDurationR\x0eopeningAuction\x12Y\n\x19price_monitoring_settings\x18\x06 \x01(\x0b\x32\x1d.vega.PriceMonitoringSettingsR\x17priceMonitoringSettings\x12k\n\x1fliquidity_monitoring_parameters\x18\x07 \x01(\x0b\x32#.vega.LiquidityMonitoringParametersR\x1dliquidityMonitoringParameters\x12;\n\x0ctrading_mode\x18\x08 \x01(\x0e\x32\x18.vega.Market.TradingModeR\x0btradingMode\x12(\n\x05state\x18\t \x01(\x0e\x32\x12.vega.Market.StateR\x05state\x12\x43\n\x11market_timestamps\x18\n \x01(\x0b\x32\x16.vega.MarketTimestampsR\x10marketTimestamps\x12\x36\n\x17position_decimal_places\x18\x0b \x01(\x03R\x15positionDecimalPlaces\x12$\n\x0elp_price_range\x18\x0c \x01(\tR\x0clpPriceRange\x12\x34\n\x16linear_slippage_factor\x18\r \x01(\tR\x14linearSlippageFactor\x12:\n\x19quadratic_slippage_factor\x18\x0e \x01(\tR\x17quadraticSlippageFactor"\xd8\x01\n\x05State\x12\x15\n\x11STATE_UNSPECIFIED\x10\x00\x12\x12\n\x0eSTATE_PROPOSED\x10\x01\x12\x12\n\x0eSTATE_REJECTED\x10\x02\x12\x11\n\rSTATE_PENDING\x10\x03\x12\x13\n\x0fSTATE_CANCELLED\x10\x04\x12\x10\n\x0cSTATE_ACTIVE\x10\x05\x12\x13\n\x0fSTATE_SUSPENDED\x10\x06\x12\x10\n\x0cSTATE_CLOSED\x10\x07\x12\x1c\n\x18STATE_TRADING_TERMINATED\x10\x08\x12\x11\n\rSTATE_SETTLED\x10\t"\xcc\x01\n\x0bTradingMode\x12\x1c\n\x18TRADING_MODE_UNSPECIFIED\x10\x00\x12\x1b\n\x17TRADING_MODE_CONTINUOUS\x10\x01\x12\x1e\n\x1aTRADING_MODE_BATCH_AUCTION\x10\x02\x12 \n\x1cTRADING_MODE_OPENING_AUCTION\x10\x03\x12#\n\x1fTRADING_MODE_MONITORING_AUCTION\x10\x04\x12\x1b\n\x17TRADING_MODE_NO_TRADING\x10\x05"r\n\x10MarketTimestamps\x12\x1a\n\x08proposed\x18\x01 \x01(\x03R\x08proposed\x12\x18\n\x07pending\x18\x02 \x01(\x03R\x07pending\x12\x12\n\x04open\x18\x03 \x01(\x03R\x04open\x12\x14\n\x05\x63lose\x18\x04 \x01(\x03R\x05\x63loseB\'Z%code.vegaprotocol.io/vega/protos/vegab\x06proto3'
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "vega.markets_pb2", globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b"Z%code.vegaprotocol.io/vega/protos/vega"
     _AUCTIONDURATION._serialized_start = 52
     _AUCTIONDURATION._serialized_end = 121
     _FUTURE._serialized_start = 124
     _FUTURE._serialized_end = 510
     _DATASOURCESPECTOFUTUREBINDING._serialized_start = 513
@@ -60,15 +59,15 @@
     _PRICEMONITORINGSETTINGS._serialized_start = 2318
     _PRICEMONITORINGSETTINGS._serialized_end = 2408
     _LIQUIDITYMONITORINGPARAMETERS._serialized_start = 2411
     _LIQUIDITYMONITORINGPARAMETERS._serialized_end = 2615
     _TARGETSTAKEPARAMETERS._serialized_start = 2617
     _TARGETSTAKEPARAMETERS._serialized_end = 2712
     _MARKET._serialized_start = 2715
-    _MARKET._serialized_end = 3841
-    _MARKET_STATE._serialized_start = 3418
-    _MARKET_STATE._serialized_end = 3634
-    _MARKET_TRADINGMODE._serialized_start = 3637
-    _MARKET_TRADINGMODE._serialized_end = 3841
-    _MARKETTIMESTAMPS._serialized_start = 3843
-    _MARKETTIMESTAMPS._serialized_end = 3957
+    _MARKET._serialized_end = 3955
+    _MARKET_STATE._serialized_start = 3532
+    _MARKET_STATE._serialized_end = 3748
+    _MARKET_TRADINGMODE._serialized_start = 3751
+    _MARKET_TRADINGMODE._serialized_end = 3955
+    _MARKETTIMESTAMPS._serialized_start = 3957
+    _MARKETTIMESTAMPS._serialized_end = 4071
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-0.67.0/vega_sim/proto/vega/oracle_pb2.py` & `vega_sim-1.0.1/vega_sim/proto/vega/oracle_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
     b'\n\x11vega/oracle.proto\x12\x04vega\x1a\x16vega/data_source.proto\x1a\x17vega/data/v1/data.proto"e\n\nOracleSpec\x12W\n\x19\x65xternal_data_source_spec\x18\x01 \x01(\x0b\x32\x1c.vega.ExternalDataSourceSpecR\x16\x65xternalDataSourceSpec"M\n\nOracleData\x12?\n\rexternal_data\x18\x01 \x01(\x0b\x32\x1a.vega.data.v1.ExternalDataR\x0c\x65xternalDataB\'Z%code.vegaprotocol.io/vega/protos/vegab\x06proto3'
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "vega.oracle_pb2", globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b"Z%code.vegaprotocol.io/vega/protos/vega"
     _ORACLESPEC._serialized_start = 76
     _ORACLESPEC._serialized_end = 177
     _ORACLEDATA._serialized_start = 179
     _ORACLEDATA._serialized_end = 256
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-0.67.0/vega_sim/proto/vega/snapshot/v1/snapshot_pb2.py` & `vega_sim-1.0.1/vega_sim/proto/vega/snapshot/v1/snapshot_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(
     DESCRIPTOR, "vega.snapshot.v1.snapshot_pb2", globals()
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = (
         b"Z1code.vegaprotocol.io/vega/protos/vega/snapshot/v1"
     )
     _FORMAT._serialized_start = 23178
     _FORMAT._serialized_end = 23274
     _SNAPSHOT._serialized_start = 249
```

### Comparing `vega_sim-0.67.0/vega_sim/proto/vega/vega_pb2.py` & `vega_sim-1.0.1/vega_sim/proto/vega/vega_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,47 +12,48 @@
 _sym_db = _symbol_database.Default()
 
 
 from . import markets_pb2 as vega_dot_markets__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x0fvega/vega.proto\x12\x04vega\x1a\x12vega/markets.proto"\x17\n\x05Party\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id"N\n\nRiskFactor\x12\x16\n\x06market\x18\x01 \x01(\tR\x06market\x12\x14\n\x05short\x18\x02 \x01(\tR\x05short\x12\x12\n\x04long\x18\x03 \x01(\tR\x04long"Z\n\x0bPeggedOrder\x12\x33\n\treference\x18\x01 \x01(\x0e\x32\x15.vega.PeggedReferenceR\treference\x12\x16\n\x06offset\x18\x02 \x01(\tR\x06offset"\xf2\x08\n\x05Order\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x03 \x01(\tR\x07partyId\x12\x1e\n\x04side\x18\x04 \x01(\x0e\x32\n.vega.SideR\x04side\x12\x14\n\x05price\x18\x05 \x01(\tR\x05price\x12\x12\n\x04size\x18\x06 \x01(\x04R\x04size\x12\x1c\n\tremaining\x18\x07 \x01(\x04R\tremaining\x12;\n\rtime_in_force\x18\x08 \x01(\x0e\x32\x17.vega.Order.TimeInForceR\x0btimeInForce\x12$\n\x04type\x18\t \x01(\x0e\x32\x10.vega.Order.TypeR\x04type\x12\x1d\n\ncreated_at\x18\n \x01(\x03R\tcreatedAt\x12*\n\x06status\x18\x0b \x01(\x0e\x32\x12.vega.Order.StatusR\x06status\x12\x1d\n\nexpires_at\x18\x0c \x01(\x03R\texpiresAt\x12\x1c\n\treference\x18\r \x01(\tR\treference\x12-\n\x06reason\x18\x0e \x01(\x0e\x32\x10.vega.OrderErrorH\x00R\x06reason\x88\x01\x01\x12\x1d\n\nupdated_at\x18\x0f \x01(\x03R\tupdatedAt\x12\x18\n\x07version\x18\x10 \x01(\x04R\x07version\x12\x19\n\x08\x62\x61tch_id\x18\x11 \x01(\x04R\x07\x62\x61tchId\x12\x34\n\x0cpegged_order\x18\x12 \x01(\x0b\x32\x11.vega.PeggedOrderR\x0bpeggedOrder\x12\x34\n\x16liquidity_provision_id\x18\x13 \x01(\tR\x14liquidityProvisionId"\xb6\x01\n\x0bTimeInForce\x12\x1d\n\x19TIME_IN_FORCE_UNSPECIFIED\x10\x00\x12\x15\n\x11TIME_IN_FORCE_GTC\x10\x01\x12\x15\n\x11TIME_IN_FORCE_GTT\x10\x02\x12\x15\n\x11TIME_IN_FORCE_IOC\x10\x03\x12\x15\n\x11TIME_IN_FORCE_FOK\x10\x04\x12\x15\n\x11TIME_IN_FORCE_GFA\x10\x05\x12\x15\n\x11TIME_IN_FORCE_GFN\x10\x06"O\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0e\n\nTYPE_LIMIT\x10\x01\x12\x0f\n\x0bTYPE_MARKET\x10\x02\x12\x10\n\x0cTYPE_NETWORK\x10\x03"\xc9\x01\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x11\n\rSTATUS_ACTIVE\x10\x01\x12\x12\n\x0eSTATUS_EXPIRED\x10\x02\x12\x14\n\x10STATUS_CANCELLED\x10\x03\x12\x12\n\x0eSTATUS_STOPPED\x10\x04\x12\x11\n\rSTATUS_FILLED\x10\x05\x12\x13\n\x0fSTATUS_REJECTED\x10\x06\x12\x1b\n\x17STATUS_PARTIALLY_FILLED\x10\x07\x12\x11\n\rSTATUS_PARKED\x10\x08\x42\t\n\x07_reason"B\n\x1dOrderCancellationConfirmation\x12!\n\x05order\x18\x01 \x01(\x0b\x32\x0b.vega.OrderR\x05order"\xa0\x01\n\x11OrderConfirmation\x12!\n\x05order\x18\x01 \x01(\x0b\x32\x0b.vega.OrderR\x05order\x12#\n\x06trades\x18\x02 \x03(\x0b\x32\x0b.vega.TradeR\x06trades\x12\x43\n\x17passive_orders_affected\x18\x03 \x03(\x0b\x32\x0b.vega.OrderR\x15passiveOrdersAffected"\xd3\x01\n\x16\x41uctionIndicativeState\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12)\n\x10indicative_price\x18\x02 \x01(\tR\x0findicativePrice\x12+\n\x11indicative_volume\x18\x03 \x01(\x04R\x10indicativeVolume\x12#\n\rauction_start\x18\x04 \x01(\x03R\x0c\x61uctionStart\x12\x1f\n\x0b\x61uction_end\x18\x05 \x01(\x03R\nauctionEnd"\xdb\x04\n\x05Trade\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x14\n\x05price\x18\x03 \x01(\tR\x05price\x12\x12\n\x04size\x18\x04 \x01(\x04R\x04size\x12\x14\n\x05\x62uyer\x18\x05 \x01(\tR\x05\x62uyer\x12\x16\n\x06seller\x18\x06 \x01(\tR\x06seller\x12(\n\taggressor\x18\x07 \x01(\x0e\x32\n.vega.SideR\taggressor\x12\x1b\n\tbuy_order\x18\x08 \x01(\tR\x08\x62uyOrder\x12\x1d\n\nsell_order\x18\t \x01(\tR\tsellOrder\x12\x1c\n\ttimestamp\x18\n \x01(\x03R\ttimestamp\x12$\n\x04type\x18\x0b \x01(\x0e\x32\x10.vega.Trade.TypeR\x04type\x12&\n\tbuyer_fee\x18\x0c \x01(\x0b\x32\t.vega.FeeR\x08\x62uyerFee\x12(\n\nseller_fee\x18\r \x01(\x0b\x32\t.vega.FeeR\tsellerFee\x12.\n\x13\x62uyer_auction_batch\x18\x0e \x01(\x04R\x11\x62uyerAuctionBatch\x12\x30\n\x14seller_auction_batch\x18\x0f \x01(\x04R\x12sellerAuctionBatch"o\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x10\n\x0cTYPE_DEFAULT\x10\x01\x12\x1f\n\x1bTYPE_NETWORK_CLOSE_OUT_GOOD\x10\x02\x12\x1e\n\x1aTYPE_NETWORK_CLOSE_OUT_BAD\x10\x03"v\n\x03\x46\x65\x65\x12\x1b\n\tmaker_fee\x18\x01 \x01(\tR\x08makerFee\x12-\n\x12infrastructure_fee\x18\x02 \x01(\tR\x11infrastructureFee\x12#\n\rliquidity_fee\x18\x03 \x01(\tR\x0cliquidityFee"/\n\x08TradeSet\x12#\n\x06trades\x18\x01 \x03(\x0b\x32\x0b.vega.TradeR\x06trades"\xd6\x01\n\x06\x43\x61ndle\x12\x1c\n\ttimestamp\x18\x01 \x01(\x03R\ttimestamp\x12\x1a\n\x08\x64\x61tetime\x18\x02 \x01(\tR\x08\x64\x61tetime\x12\x12\n\x04high\x18\x03 \x01(\tR\x04high\x12\x10\n\x03low\x18\x04 \x01(\tR\x03low\x12\x12\n\x04open\x18\x05 \x01(\tR\x04open\x12\x14\n\x05\x63lose\x18\x06 \x01(\tR\x05\x63lose\x12\x16\n\x06volume\x18\x07 \x01(\x04R\x06volume\x12*\n\x08interval\x18\x08 \x01(\x0e\x32\x0e.vega.IntervalR\x08interval"d\n\nPriceLevel\x12\x14\n\x05price\x18\x01 \x01(\tR\x05price\x12(\n\x10number_of_orders\x18\x02 \x01(\x04R\x0enumberOfOrders\x12\x16\n\x06volume\x18\x03 \x01(\x04R\x06volume"\x9d\x01\n\x0bMarketDepth\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12"\n\x03\x62uy\x18\x02 \x03(\x0b\x32\x10.vega.PriceLevelR\x03\x62uy\x12$\n\x04sell\x18\x03 \x03(\x0b\x32\x10.vega.PriceLevelR\x04sell\x12\'\n\x0fsequence_number\x18\x04 \x01(\x04R\x0esequenceNumber"\xdd\x01\n\x11MarketDepthUpdate\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12"\n\x03\x62uy\x18\x02 \x03(\x0b\x32\x10.vega.PriceLevelR\x03\x62uy\x12$\n\x04sell\x18\x03 \x03(\x0b\x32\x10.vega.PriceLevelR\x04sell\x12\'\n\x0fsequence_number\x18\x04 \x01(\x04R\x0esequenceNumber\x12\x38\n\x18previous_sequence_number\x18\x05 \x01(\x04R\x16previousSequenceNumber"\xfc\x01\n\x08Position\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x1f\n\x0bopen_volume\x18\x03 \x01(\x03R\nopenVolume\x12!\n\x0crealised_pnl\x18\x04 \x01(\tR\x0brealisedPnl\x12%\n\x0eunrealised_pnl\x18\x05 \x01(\tR\runrealisedPnl\x12.\n\x13\x61verage_entry_price\x18\x06 \x01(\tR\x11\x61verageEntryPrice\x12\x1d\n\nupdated_at\x18\x07 \x01(\x03R\tupdatedAt"=\n\rPositionTrade\x12\x16\n\x06volume\x18\x01 \x01(\x03R\x06volume\x12\x14\n\x05price\x18\x02 \x01(\tR\x05price"\xe4\x02\n\x07\x44\x65posit\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12,\n\x06status\x18\x02 \x01(\x0e\x32\x14.vega.Deposit.StatusR\x06status\x12\x19\n\x08party_id\x18\x03 \x01(\tR\x07partyId\x12\x14\n\x05\x61sset\x18\x04 \x01(\tR\x05\x61sset\x12\x16\n\x06\x61mount\x18\x05 \x01(\tR\x06\x61mount\x12\x17\n\x07tx_hash\x18\x06 \x01(\tR\x06txHash\x12-\n\x12\x63redited_timestamp\x18\x07 \x01(\x03R\x11\x63reditedTimestamp\x12+\n\x11\x63reated_timestamp\x18\x08 \x01(\x03R\x10\x63reatedTimestamp"]\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x0f\n\x0bSTATUS_OPEN\x10\x01\x12\x14\n\x10STATUS_CANCELLED\x10\x02\x12\x14\n\x10STATUS_FINALIZED\x10\x03"\xa8\x03\n\nWithdrawal\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x14\n\x05\x61sset\x18\x04 \x01(\tR\x05\x61sset\x12/\n\x06status\x18\x05 \x01(\x0e\x32\x17.vega.Withdrawal.StatusR\x06status\x12\x10\n\x03ref\x18\x06 \x01(\tR\x03ref\x12\x17\n\x07tx_hash\x18\x08 \x01(\tR\x06txHash\x12+\n\x11\x63reated_timestamp\x18\t \x01(\x03R\x10\x63reatedTimestamp\x12/\n\x13withdrawn_timestamp\x18\n \x01(\x03R\x12withdrawnTimestamp\x12#\n\x03\x65xt\x18\x0b \x01(\x0b\x32\x11.vega.WithdrawExtR\x03\x65xt"\\\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x0f\n\x0bSTATUS_OPEN\x10\x01\x12\x13\n\x0fSTATUS_REJECTED\x10\x02\x12\x14\n\x10STATUS_FINALIZED\x10\x03J\x04\x08\x07\x10\x08"D\n\x0bWithdrawExt\x12.\n\x05\x65rc20\x18\x01 \x01(\x0b\x32\x16.vega.Erc20WithdrawExtH\x00R\x05\x65rc20B\x05\n\x03\x65xt"=\n\x10\x45rc20WithdrawExt\x12)\n\x10receiver_address\x18\x01 \x01(\tR\x0freceiverAddress"\xa3\x01\n\x07\x41\x63\x63ount\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x14\n\x05owner\x18\x02 \x01(\tR\x05owner\x12\x18\n\x07\x62\x61lance\x18\x03 \x01(\tR\x07\x62\x61lance\x12\x14\n\x05\x61sset\x18\x04 \x01(\tR\x05\x61sset\x12\x1b\n\tmarket_id\x18\x05 \x01(\tR\x08marketId\x12%\n\x04type\x18\x06 \x01(\x0e\x32\x11.vega.AccountTypeR\x04type"?\n\x0f\x46inancialAmount\x12\x16\n\x06\x61mount\x18\x01 \x01(\tR\x06\x61mount\x12\x14\n\x05\x61sset\x18\x02 \x01(\tR\x05\x61sset"\xb3\x01\n\x08Transfer\x12\x14\n\x05owner\x18\x01 \x01(\tR\x05owner\x12-\n\x06\x61mount\x18\x02 \x01(\x0b\x32\x15.vega.FinancialAmountR\x06\x61mount\x12&\n\x04type\x18\x03 \x01(\x0e\x32\x12.vega.TransferTypeR\x04type\x12\x1d\n\nmin_amount\x18\x04 \x01(\tR\tminAmount\x12\x1b\n\tmarket_id\x18\x05 \x01(\tR\x08marketId"\x84\x01\n\x10\x44ispatchStrategy\x12(\n\x10\x61sset_for_metric\x18\x01 \x01(\tR\x0e\x61ssetForMetric\x12,\n\x06metric\x18\x02 \x01(\x0e\x32\x14.vega.DispatchMetricR\x06metric\x12\x18\n\x07markets\x18\x03 \x03(\tR\x07markets"\xe6\x01\n\x0fTransferRequest\x12\x30\n\x0c\x66rom_account\x18\x01 \x03(\x0b\x32\r.vega.AccountR\x0b\x66romAccount\x12,\n\nto_account\x18\x02 \x03(\x0b\x32\r.vega.AccountR\ttoAccount\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x1d\n\nmin_amount\x18\x04 \x01(\tR\tminAmount\x12\x14\n\x05\x61sset\x18\x05 \x01(\tR\x05\x61sset\x12&\n\x04type\x18\x07 \x01(\x0e\x32\x12.vega.TransferTypeR\x04type"\xa7\x01\n\x0e\x41\x63\x63ountDetails\x12\x19\n\x08\x61sset_id\x18\x01 \x01(\tR\x07\x61ssetId\x12%\n\x04type\x18\x02 \x01(\x0e\x32\x11.vega.AccountTypeR\x04type\x12\x19\n\x05owner\x18\x03 \x01(\tH\x00R\x05owner\x88\x01\x01\x12 \n\tmarket_id\x18\x04 \x01(\tH\x01R\x08marketId\x88\x01\x01\x42\x08\n\x06_ownerB\x0c\n\n_market_id"\xb9\x02\n\x0bLedgerEntry\x12\x37\n\x0c\x66rom_account\x18\x01 \x01(\x0b\x32\x14.vega.AccountDetailsR\x0b\x66romAccount\x12\x33\n\nto_account\x18\x02 \x01(\x0b\x32\x14.vega.AccountDetailsR\ttoAccount\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12&\n\x04type\x18\x04 \x01(\x0e\x32\x12.vega.TransferTypeR\x04type\x12\x1c\n\ttimestamp\x18\x05 \x01(\x03R\ttimestamp\x12\x30\n\x14\x66rom_account_balance\x18\x06 \x01(\tR\x12\x66romAccountBalance\x12,\n\x12to_account_balance\x18\x07 \x01(\tR\x10toAccountBalance"_\n\x13PostTransferBalance\x12.\n\x07\x61\x63\x63ount\x18\x01 \x01(\x0b\x32\x14.vega.AccountDetailsR\x07\x61\x63\x63ount\x12\x18\n\x07\x62\x61lance\x18\x02 \x01(\tR\x07\x62\x61lance"t\n\x0eLedgerMovement\x12+\n\x07\x65ntries\x18\x01 \x03(\x0b\x32\x11.vega.LedgerEntryR\x07\x65ntries\x12\x35\n\x08\x62\x61lances\x18\x02 \x03(\x0b\x32\x19.vega.PostTransferBalanceR\x08\x62\x61lances"\xad\x02\n\x0cMarginLevels\x12-\n\x12maintenance_margin\x18\x01 \x01(\tR\x11maintenanceMargin\x12!\n\x0csearch_level\x18\x02 \x01(\tR\x0bsearchLevel\x12%\n\x0einitial_margin\x18\x03 \x01(\tR\rinitialMargin\x12\x38\n\x18\x63ollateral_release_level\x18\x04 \x01(\tR\x16\x63ollateralReleaseLevel\x12\x19\n\x08party_id\x18\x05 \x01(\tR\x07partyId\x12\x1b\n\tmarket_id\x18\x06 \x01(\tR\x08marketId\x12\x14\n\x05\x61sset\x18\x07 \x01(\tR\x05\x61sset\x12\x1c\n\ttimestamp\x18\x08 \x01(\x03R\ttimestamp"\xe5\n\n\nMarketData\x12\x1d\n\nmark_price\x18\x01 \x01(\tR\tmarkPrice\x12$\n\x0e\x62\x65st_bid_price\x18\x02 \x01(\tR\x0c\x62\x65stBidPrice\x12&\n\x0f\x62\x65st_bid_volume\x18\x03 \x01(\x04R\rbestBidVolume\x12(\n\x10\x62\x65st_offer_price\x18\x04 \x01(\tR\x0e\x62\x65stOfferPrice\x12*\n\x11\x62\x65st_offer_volume\x18\x05 \x01(\x04R\x0f\x62\x65stOfferVolume\x12\x31\n\x15\x62\x65st_static_bid_price\x18\x06 \x01(\tR\x12\x62\x65stStaticBidPrice\x12\x33\n\x16\x62\x65st_static_bid_volume\x18\x07 \x01(\x04R\x13\x62\x65stStaticBidVolume\x12\x35\n\x17\x62\x65st_static_offer_price\x18\x08 \x01(\tR\x14\x62\x65stStaticOfferPrice\x12\x37\n\x18\x62\x65st_static_offer_volume\x18\t \x01(\x04R\x15\x62\x65stStaticOfferVolume\x12\x1b\n\tmid_price\x18\n \x01(\tR\x08midPrice\x12(\n\x10static_mid_price\x18\x0b \x01(\tR\x0estaticMidPrice\x12\x16\n\x06market\x18\x0c \x01(\tR\x06market\x12\x1c\n\ttimestamp\x18\r \x01(\x03R\ttimestamp\x12#\n\ropen_interest\x18\x0e \x01(\x04R\x0copenInterest\x12\x1f\n\x0b\x61uction_end\x18\x0f \x01(\x03R\nauctionEnd\x12#\n\rauction_start\x18\x10 \x01(\x03R\x0c\x61uctionStart\x12)\n\x10indicative_price\x18\x11 \x01(\tR\x0findicativePrice\x12+\n\x11indicative_volume\x18\x12 \x01(\x04R\x10indicativeVolume\x12H\n\x13market_trading_mode\x18\x13 \x01(\x0e\x32\x18.vega.Market.TradingModeR\x11marketTradingMode\x12.\n\x07trigger\x18\x14 \x01(\x0e\x32\x14.vega.AuctionTriggerR\x07trigger\x12\x41\n\x11\x65xtension_trigger\x18\x15 \x01(\x0e\x32\x14.vega.AuctionTriggerR\x10\x65xtensionTrigger\x12!\n\x0ctarget_stake\x18\x16 \x01(\tR\x0btargetStake\x12%\n\x0esupplied_stake\x18\x17 \x01(\tR\rsuppliedStake\x12S\n\x17price_monitoring_bounds\x18\x18 \x03(\x0b\x32\x1b.vega.PriceMonitoringBoundsR\x15priceMonitoringBounds\x12,\n\x12market_value_proxy\x18\x19 \x01(\tR\x10marketValueProxy\x12`\n\x1cliquidity_provider_fee_share\x18\x1a \x03(\x0b\x32\x1f.vega.LiquidityProviderFeeShareR\x19liquidityProviderFeeShare\x12\x35\n\x0cmarket_state\x18\x1b \x01(\x0e\x32\x12.vega.Market.StateR\x0bmarketState\x12-\n\x13next_mark_to_market\x18\x1c \x01(\x03R\x10nextMarkToMarket\x12*\n\x11last_traded_price\x18\x1d \x01(\tR\x0flastTradedPrice"\xba\x01\n\x19LiquidityProviderFeeShare\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12*\n\x11\x65quity_like_share\x18\x02 \x01(\tR\x0f\x65quityLikeShare\x12\x36\n\x17\x61verage_entry_valuation\x18\x03 \x01(\tR\x15\x61verageEntryValuation\x12#\n\raverage_score\x18\x04 \x01(\tR\x0c\x61verageScore"\xc8\x01\n\x15PriceMonitoringBounds\x12&\n\x0fmin_valid_price\x18\x01 \x01(\tR\rminValidPrice\x12&\n\x0fmax_valid_price\x18\x02 \x01(\tR\rmaxValidPrice\x12\x36\n\x07trigger\x18\x03 \x01(\x0b\x32\x1c.vega.PriceMonitoringTriggerR\x07trigger\x12\'\n\x0freference_price\x18\x04 \x01(\tR\x0ereferencePrice"Q\n\x0b\x45rrorDetail\x12\x12\n\x04\x63ode\x18\x01 \x01(\x05R\x04\x63ode\x12\x18\n\x07message\x18\x02 \x01(\tR\x07message\x12\x14\n\x05inner\x18\x03 \x01(\tR\x05inner":\n\x10NetworkParameter\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value"\x82\x03\n\rNetworkLimits\x12,\n\x12\x63\x61n_propose_market\x18\x01 \x01(\x08R\x10\x63\x61nProposeMarket\x12*\n\x11\x63\x61n_propose_asset\x18\x02 \x01(\x08R\x0f\x63\x61nProposeAsset\x12\x34\n\x16propose_market_enabled\x18\x04 \x01(\x08R\x14proposeMarketEnabled\x12\x32\n\x15propose_asset_enabled\x18\x05 \x01(\x08R\x13proposeAssetEnabled\x12%\n\x0egenesis_loaded\x18\x07 \x01(\x08R\rgenesisLoaded\x12=\n\x1bpropose_market_enabled_from\x18\x08 \x01(\x03R\x18proposeMarketEnabledFrom\x12;\n\x1apropose_asset_enabled_from\x18\t \x01(\x03R\x17proposeAssetEnabledFromJ\x04\x08\x03\x10\x04J\x04\x08\x06\x10\x07"}\n\x0eLiquidityOrder\x12\x33\n\treference\x18\x01 \x01(\x0e\x32\x15.vega.PeggedReferenceR\treference\x12\x1e\n\nproportion\x18\x02 \x01(\rR\nproportion\x12\x16\n\x06offset\x18\x03 \x01(\tR\x06offset"s\n\x17LiquidityOrderReference\x12\x19\n\x08order_id\x18\x01 \x01(\tR\x07orderId\x12=\n\x0fliquidity_order\x18\x02 \x01(\x0b\x32\x14.vega.LiquidityOrderR\x0eliquidityOrder"\xd2\x04\n\x12LiquidityProvision\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x1d\n\ncreated_at\x18\x03 \x01(\x03R\tcreatedAt\x12\x1d\n\nupdated_at\x18\x04 \x01(\x03R\tupdatedAt\x12\x1b\n\tmarket_id\x18\x05 \x01(\tR\x08marketId\x12+\n\x11\x63ommitment_amount\x18\x06 \x01(\tR\x10\x63ommitmentAmount\x12\x10\n\x03\x66\x65\x65\x18\x07 \x01(\tR\x03\x66\x65\x65\x12\x33\n\x05sells\x18\x08 \x03(\x0b\x32\x1d.vega.LiquidityOrderReferenceR\x05sells\x12\x31\n\x04\x62uys\x18\t \x03(\x0b\x32\x1d.vega.LiquidityOrderReferenceR\x04\x62uys\x12\x18\n\x07version\x18\n \x01(\x04R\x07version\x12\x37\n\x06status\x18\x0b \x01(\x0e\x32\x1f.vega.LiquidityProvision.StatusR\x06status\x12\x1c\n\treference\x18\x0c \x01(\tR\treference"\x9d\x01\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x11\n\rSTATUS_ACTIVE\x10\x01\x12\x12\n\x0eSTATUS_STOPPED\x10\x02\x12\x14\n\x10STATUS_CANCELLED\x10\x03\x12\x13\n\x0fSTATUS_REJECTED\x10\x04\x12\x15\n\x11STATUS_UNDEPLOYED\x10\x05\x12\x12\n\x0eSTATUS_PENDING\x10\x06"\xd0\x03\n\x0e\x45thereumConfig\x12\x1d\n\nnetwork_id\x18\x01 \x01(\tR\tnetworkId\x12\x19\n\x08\x63hain_id\x18\x02 \x01(\tR\x07\x63hainId\x12Z\n\x1a\x63ollateral_bridge_contract\x18\x03 \x01(\x0b\x32\x1c.vega.EthereumContractConfigR\x18\x63ollateralBridgeContract\x12$\n\rconfirmations\x18\x04 \x01(\rR\rconfirmations\x12T\n\x17staking_bridge_contract\x18\x05 \x01(\x0b\x32\x1c.vega.EthereumContractConfigR\x15stakingBridgeContract\x12R\n\x16token_vesting_contract\x18\x06 \x01(\x0b\x32\x1c.vega.EthereumContractConfigR\x14tokenVestingContract\x12X\n\x19multisig_control_contract\x18\x07 \x01(\x0b\x32\x1c.vega.EthereumContractConfigR\x17multisigControlContract"j\n\x16\x45thereumContractConfig\x12\x18\n\x07\x61\x64\x64ress\x18\x01 \x01(\tR\x07\x61\x64\x64ress\x12\x36\n\x17\x64\x65ployment_block_height\x18\x06 \x01(\x04R\x15\x64\x65ploymentBlockHeight"\xac\x01\n\x0f\x45pochTimestamps\x12\x1d\n\nstart_time\x18\x01 \x01(\x03R\tstartTime\x12\x1f\n\x0b\x65xpiry_time\x18\x02 \x01(\x03R\nexpiryTime\x12\x19\n\x08\x65nd_time\x18\x03 \x01(\x03R\x07\x65ndTime\x12\x1f\n\x0b\x66irst_block\x18\x04 \x01(\x04R\nfirstBlock\x12\x1d\n\nlast_block\x18\x05 \x01(\x04R\tlastBlock"\xb0\x01\n\x05\x45poch\x12\x10\n\x03seq\x18\x01 \x01(\x04R\x03seq\x12\x35\n\ntimestamps\x18\x02 \x01(\x0b\x32\x15.vega.EpochTimestampsR\ntimestamps\x12*\n\nvalidators\x18\x03 \x03(\x0b\x32\n.vega.NodeR\nvalidators\x12\x32\n\x0b\x64\x65legations\x18\x04 \x03(\x0b\x32\x10.vega.DelegationR\x0b\x64\x65legations"\x8e\x01\n\x12\x45pochParticipation\x12!\n\x05\x65poch\x18\x01 \x01(\x0b\x32\x0b.vega.EpochR\x05\x65poch\x12\x18\n\x07offline\x18\x02 \x01(\x04R\x07offline\x12\x16\n\x06online\x18\x03 \x01(\x04R\x06online\x12#\n\rtotal_rewards\x18\x04 \x01(\x01R\x0ctotalRewards"S\n\tEpochData\x12\x14\n\x05total\x18\x01 \x01(\x05R\x05total\x12\x18\n\x07offline\x18\x02 \x01(\x05R\x07offline\x12\x16\n\x06online\x18\x03 \x01(\x05R\x06online"\x9b\x02\n\x0cRankingScore\x12\x1f\n\x0bstake_score\x18\x01 \x01(\tR\nstakeScore\x12+\n\x11performance_score\x18\x02 \x01(\tR\x10performanceScore\x12\x42\n\x0fprevious_status\x18\x03 \x01(\x0e\x32\x19.vega.ValidatorNodeStatusR\x0epreviousStatus\x12\x31\n\x06status\x18\x04 \x01(\x0e\x32\x19.vega.ValidatorNodeStatusR\x06status\x12!\n\x0cvoting_power\x18\x05 \x01(\rR\x0bvotingPower\x12#\n\rranking_score\x18\x06 \x01(\tR\x0crankingScore"\xab\x02\n\x0bRewardScore\x12.\n\x13raw_validator_score\x18\x01 \x01(\tR\x11rawValidatorScore\x12+\n\x11performance_score\x18\x02 \x01(\tR\x10performanceScore\x12%\n\x0emultisig_score\x18\x03 \x01(\tR\rmultisigScore\x12\'\n\x0fvalidator_score\x18\x04 \x01(\tR\x0evalidatorScore\x12)\n\x10normalised_score\x18\x05 \x01(\tR\x0fnormalisedScore\x12\x44\n\x10validator_status\x18\x06 \x01(\x0e\x32\x19.vega.ValidatorNodeStatusR\x0fvalidatorStatus"\xb3\x05\n\x04Node\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x17\n\x07pub_key\x18\x02 \x01(\tR\x06pubKey\x12\x1c\n\ntm_pub_key\x18\x03 \x01(\tR\x08tmPubKey\x12)\n\x10\x65thereum_address\x18\x04 \x01(\tR\x0f\x65thereumAddress\x12\x19\n\x08info_url\x18\x05 \x01(\tR\x07infoUrl\x12\x1a\n\x08location\x18\x06 \x01(\tR\x08location\x12,\n\x12staked_by_operator\x18\x07 \x01(\tR\x10stakedByOperator\x12.\n\x13staked_by_delegates\x18\x08 \x01(\tR\x11stakedByDelegates\x12!\n\x0cstaked_total\x18\t \x01(\tR\x0bstakedTotal\x12,\n\x12max_intended_stake\x18\n \x01(\tR\x10maxIntendedStake\x12#\n\rpending_stake\x18\x0b \x01(\tR\x0cpendingStake\x12.\n\nepoch_data\x18\x0c \x01(\x0b\x32\x0f.vega.EpochDataR\tepochData\x12(\n\x06status\x18\r \x01(\x0e\x32\x10.vega.NodeStatusR\x06status\x12\x32\n\x0b\x64\x65legations\x18\x0e \x03(\x0b\x32\x10.vega.DelegationR\x0b\x64\x65legations\x12\x34\n\x0creward_score\x18\x0f \x01(\x0b\x32\x11.vega.RewardScoreR\x0brewardScore\x12\x37\n\rranking_score\x18\x10 \x01(\x0b\x32\x12.vega.RankingScoreR\x0crankingScore\x12\x12\n\x04name\x18\x11 \x01(\tR\x04name\x12\x1d\n\navatar_url\x18\x12 \x01(\tR\tavatarUrl"\x9c\x01\n\x07NodeSet\x12\x14\n\x05total\x18\x01 \x01(\rR\x05total\x12\x1a\n\x08inactive\x18\x02 \x01(\rR\x08inactive\x12\x1a\n\x08promoted\x18\x03 \x03(\tR\x08promoted\x12\x18\n\x07\x64\x65moted\x18\x04 \x03(\tR\x07\x64\x65moted\x12\x1d\n\x07maximum\x18\x05 \x01(\rH\x00R\x07maximum\x88\x01\x01\x42\n\n\x08_maximum"\xad\x02\n\x08NodeData\x12!\n\x0cstaked_total\x18\x01 \x01(\tR\x0bstakedTotal\x12\x1f\n\x0btotal_nodes\x18\x02 \x01(\rR\ntotalNodes\x12%\n\x0einactive_nodes\x18\x03 \x01(\rR\rinactiveNodes\x12\x38\n\x10tendermint_nodes\x18\x04 \x01(\x0b\x32\r.vega.NodeSetR\x0ftendermintNodes\x12\x30\n\x0c\x65rsatz_nodes\x18\x05 \x01(\x0b\x32\r.vega.NodeSetR\x0b\x65rsatzNodes\x12\x32\n\rpending_nodes\x18\x06 \x01(\x0b\x32\r.vega.NodeSetR\x0cpendingNodes\x12\x16\n\x06uptime\x18\x07 \x01(\x02R\x06uptime"p\n\nDelegation\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x17\n\x07node_id\x18\x02 \x01(\tR\x06nodeId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x1b\n\tepoch_seq\x18\x04 \x01(\tR\x08\x65pochSeq"\xfb\x01\n\x06Reward\x12\x19\n\x08\x61sset_id\x18\x01 \x01(\tR\x07\x61ssetId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x14\n\x05\x65poch\x18\x03 \x01(\x04R\x05\x65poch\x12\x16\n\x06\x61mount\x18\x04 \x01(\tR\x06\x61mount\x12.\n\x13percentage_of_total\x18\x05 \x01(\tR\x11percentageOfTotal\x12\x1f\n\x0breceived_at\x18\x06 \x01(\x03R\nreceivedAt\x12\x1b\n\tmarket_id\x18\x07 \x01(\tR\x08marketId\x12\x1f\n\x0breward_type\x18\x08 \x01(\tR\nrewardType"]\n\rRewardSummary\x12\x19\n\x08\x61sset_id\x18\x01 \x01(\tR\x07\x61ssetId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount"\x9b\x01\n\x12\x45pochRewardSummary\x12\x14\n\x05\x65poch\x18\x01 \x01(\x04R\x05\x65poch\x12\x19\n\x08\x61sset_id\x18\x02 \x01(\tR\x07\x61ssetId\x12\x1b\n\tmarket_id\x18\x03 \x01(\tR\x08marketId\x12\x1f\n\x0breward_type\x18\x04 \x01(\tR\nrewardType\x12\x16\n\x06\x61mount\x18\x05 \x01(\tR\x06\x61mount"y\n\x12StateValueProposal\x12 \n\x0cstate_var_id\x18\x01 \x01(\tR\nstateVarId\x12\x19\n\x08\x65vent_id\x18\x02 \x01(\tR\x07\x65ventId\x12&\n\x03kvb\x18\x03 \x03(\x0b\x32\x14.vega.KeyValueBundleR\x03kvb"k\n\x0eKeyValueBundle\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x1c\n\ttolerance\x18\x02 \x01(\tR\ttolerance\x12)\n\x05value\x18\x03 \x01(\x0b\x32\x13.vega.StateVarValueR\x05value"\xb4\x01\n\rStateVarValue\x12\x32\n\nscalar_val\x18\x01 \x01(\x0b\x32\x11.vega.ScalarValueH\x00R\tscalarVal\x12\x32\n\nvector_val\x18\x02 \x01(\x0b\x32\x11.vega.VectorValueH\x00R\tvectorVal\x12\x32\n\nmatrix_val\x18\x03 \x01(\x0b\x32\x11.vega.MatrixValueH\x00R\tmatrixValB\x07\n\x05value"#\n\x0bScalarValue\x12\x14\n\x05value\x18\x01 \x01(\tR\x05value"#\n\x0bVectorValue\x12\x14\n\x05value\x18\x01 \x03(\tR\x05value"6\n\x0bMatrixValue\x12\'\n\x05value\x18\x01 \x03(\x0b\x32\x11.vega.VectorValueR\x05value*9\n\x04Side\x12\x14\n\x10SIDE_UNSPECIFIED\x10\x00\x12\x0c\n\x08SIDE_BUY\x10\x01\x12\r\n\tSIDE_SELL\x10\x02*\x98\x01\n\x08Interval\x12\x18\n\x14INTERVAL_UNSPECIFIED\x10\x00\x12\x10\n\x0cINTERVAL_I1M\x10<\x12\x11\n\x0cINTERVAL_I5M\x10\xac\x02\x12\x12\n\rINTERVAL_I15M\x10\x84\x07\x12\x11\n\x0cINTERVAL_I1H\x10\x90\x1c\x12\x12\n\x0cINTERVAL_I6H\x10\xe0\xa8\x01\x12\x12\n\x0cINTERVAL_I1D\x10\x80\xa3\x05*\xa3\x01\n\x0e\x41uctionTrigger\x12\x1f\n\x1b\x41UCTION_TRIGGER_UNSPECIFIED\x10\x00\x12\x19\n\x15\x41UCTION_TRIGGER_BATCH\x10\x01\x12\x1b\n\x17\x41UCTION_TRIGGER_OPENING\x10\x02\x12\x19\n\x15\x41UCTION_TRIGGER_PRICE\x10\x03\x12\x1d\n\x19\x41UCTION_TRIGGER_LIQUIDITY\x10\x04*\x8b\x01\n\x0fPeggedReference\x12 \n\x1cPEGGED_REFERENCE_UNSPECIFIED\x10\x00\x12\x18\n\x14PEGGED_REFERENCE_MID\x10\x01\x12\x1d\n\x19PEGGED_REFERENCE_BEST_BID\x10\x02\x12\x1d\n\x19PEGGED_REFERENCE_BEST_ASK\x10\x03*\xdf\x0f\n\nOrderError\x12\x1b\n\x17ORDER_ERROR_UNSPECIFIED\x10\x00\x12!\n\x1dORDER_ERROR_INVALID_MARKET_ID\x10\x01\x12 \n\x1cORDER_ERROR_INVALID_ORDER_ID\x10\x02\x12\x1f\n\x1bORDER_ERROR_OUT_OF_SEQUENCE\x10\x03\x12&\n"ORDER_ERROR_INVALID_REMAINING_SIZE\x10\x04\x12\x1c\n\x18ORDER_ERROR_TIME_FAILURE\x10\x05\x12\x1f\n\x1bORDER_ERROR_REMOVAL_FAILURE\x10\x06\x12+\n\'ORDER_ERROR_INVALID_EXPIRATION_DATETIME\x10\x07\x12\'\n#ORDER_ERROR_INVALID_ORDER_REFERENCE\x10\x08\x12 \n\x1cORDER_ERROR_EDIT_NOT_ALLOWED\x10\t\x12\x1d\n\x19ORDER_ERROR_AMEND_FAILURE\x10\n\x12\x19\n\x15ORDER_ERROR_NOT_FOUND\x10\x0b\x12 \n\x1cORDER_ERROR_INVALID_PARTY_ID\x10\x0c\x12\x1d\n\x19ORDER_ERROR_MARKET_CLOSED\x10\r\x12#\n\x1fORDER_ERROR_MARGIN_CHECK_FAILED\x10\x0e\x12\'\n#ORDER_ERROR_MISSING_GENERAL_ACCOUNT\x10\x0f\x12\x1e\n\x1aORDER_ERROR_INTERNAL_ERROR\x10\x10\x12\x1c\n\x18ORDER_ERROR_INVALID_SIZE\x10\x11\x12#\n\x1fORDER_ERROR_INVALID_PERSISTENCE\x10\x12\x12\x1c\n\x18ORDER_ERROR_INVALID_TYPE\x10\x13\x12\x1c\n\x18ORDER_ERROR_SELF_TRADING\x10\x14\x12.\n*ORDER_ERROR_INSUFFICIENT_FUNDS_TO_PAY_FEES\x10\x15\x12%\n!ORDER_ERROR_INCORRECT_MARKET_TYPE\x10\x16\x12%\n!ORDER_ERROR_INVALID_TIME_IN_FORCE\x10\x17\x12\x37\n3ORDER_ERROR_CANNOT_SEND_GFN_ORDER_DURING_AN_AUCTION\x10\x18\x12?\n;ORDER_ERROR_CANNOT_SEND_GFA_ORDER_DURING_CONTINUOUS_TRADING\x10\x19\x12\x34\n0ORDER_ERROR_CANNOT_AMEND_TO_GTT_WITHOUT_EXPIRYAT\x10\x1a\x12)\n%ORDER_ERROR_EXPIRYAT_BEFORE_CREATEDAT\x10\x1b\x12,\n(ORDER_ERROR_CANNOT_HAVE_GTC_AND_EXPIRYAT\x10\x1c\x12*\n&ORDER_ERROR_CANNOT_AMEND_TO_FOK_OR_IOC\x10\x1d\x12*\n&ORDER_ERROR_CANNOT_AMEND_TO_GFA_OR_GFN\x10\x1e\x12,\n(ORDER_ERROR_CANNOT_AMEND_FROM_GFA_OR_GFN\x10\x1f\x12\x34\n0ORDER_ERROR_CANNOT_SEND_IOC_ORDER_DURING_AUCTION\x10 \x12\x34\n0ORDER_ERROR_CANNOT_SEND_FOK_ORDER_DURING_AUCTION\x10!\x12#\n\x1fORDER_ERROR_MUST_BE_LIMIT_ORDER\x10"\x12"\n\x1eORDER_ERROR_MUST_BE_GTT_OR_GTC\x10#\x12\'\n#ORDER_ERROR_WITHOUT_REFERENCE_PRICE\x10$\x12\x33\n/ORDER_ERROR_BUY_CANNOT_REFERENCE_BEST_ASK_PRICE\x10%\x12\x37\n3ORDER_ERROR_OFFSET_MUST_BE_GREATER_OR_EQUAL_TO_ZERO\x10(\x12\x34\n0ORDER_ERROR_SELL_CANNOT_REFERENCE_BEST_BID_PRICE\x10)\x12\x30\n,ORDER_ERROR_OFFSET_MUST_BE_GREATER_THAN_ZERO\x10*\x12*\n&ORDER_ERROR_INSUFFICIENT_ASSET_BALANCE\x10+\x12\x45\nAORDER_ERROR_CANNOT_AMEND_PEGGED_ORDER_DETAILS_ON_NON_PEGGED_ORDER\x10,\x12.\n*ORDER_ERROR_UNABLE_TO_REPRICE_PEGGED_ORDER\x10-\x12\x35\n1ORDER_ERROR_UNABLE_TO_AMEND_PRICE_ON_PEGGED_ORDER\x10.\x12\x38\n4ORDER_ERROR_NON_PERSISTENT_ORDER_OUT_OF_PRICE_BOUNDS\x10/\x12&\n"ORDER_ERROR_TOO_MANY_PEGGED_ORDERS\x10\x30"\x04\x08&\x10&"\x04\x08\'\x10\'*\x82\x01\n\x0b\x43hainStatus\x12\x1c\n\x18\x43HAIN_STATUS_UNSPECIFIED\x10\x00\x12\x1d\n\x19\x43HAIN_STATUS_DISCONNECTED\x10\x01\x12\x1a\n\x16\x43HAIN_STATUS_REPLAYING\x10\x02\x12\x1a\n\x16\x43HAIN_STATUS_CONNECTED\x10\x03*\xc4\x04\n\x0b\x41\x63\x63ountType\x12\x1c\n\x18\x41\x43\x43OUNT_TYPE_UNSPECIFIED\x10\x00\x12\x1a\n\x16\x41\x43\x43OUNT_TYPE_INSURANCE\x10\x01\x12\x1b\n\x17\x41\x43\x43OUNT_TYPE_SETTLEMENT\x10\x02\x12\x17\n\x13\x41\x43\x43OUNT_TYPE_MARGIN\x10\x03\x12\x18\n\x14\x41\x43\x43OUNT_TYPE_GENERAL\x10\x04\x12$\n ACCOUNT_TYPE_FEES_INFRASTRUCTURE\x10\x05\x12\x1f\n\x1b\x41\x43\x43OUNT_TYPE_FEES_LIQUIDITY\x10\x06\x12\x1b\n\x17\x41\x43\x43OUNT_TYPE_FEES_MAKER\x10\x07\x12\x15\n\x11\x41\x43\x43OUNT_TYPE_BOND\x10\t\x12\x19\n\x15\x41\x43\x43OUNT_TYPE_EXTERNAL\x10\n\x12!\n\x1d\x41\x43\x43OUNT_TYPE_GLOBAL_INSURANCE\x10\x0b\x12\x1e\n\x1a\x41\x43\x43OUNT_TYPE_GLOBAL_REWARD\x10\x0c\x12"\n\x1e\x41\x43\x43OUNT_TYPE_PENDING_TRANSFERS\x10\r\x12\'\n#ACCOUNT_TYPE_REWARD_MAKER_PAID_FEES\x10\x0e\x12+\n\'ACCOUNT_TYPE_REWARD_MAKER_RECEIVED_FEES\x10\x0f\x12(\n$ACCOUNT_TYPE_REWARD_LP_RECEIVED_FEES\x10\x10\x12(\n$ACCOUNT_TYPE_REWARD_MARKET_PROPOSERS\x10\x11"\x04\x08\x08\x10\x08*\xc9\x06\n\x0cTransferType\x12\x1d\n\x19TRANSFER_TYPE_UNSPECIFIED\x10\x00\x12\x16\n\x12TRANSFER_TYPE_LOSS\x10\x01\x12\x15\n\x11TRANSFER_TYPE_WIN\x10\x02\x12\x1a\n\x16TRANSFER_TYPE_MTM_LOSS\x10\x04\x12\x19\n\x15TRANSFER_TYPE_MTM_WIN\x10\x05\x12\x1c\n\x18TRANSFER_TYPE_MARGIN_LOW\x10\x06\x12\x1d\n\x19TRANSFER_TYPE_MARGIN_HIGH\x10\x07\x12$\n TRANSFER_TYPE_MARGIN_CONFISCATED\x10\x08\x12\x1f\n\x1bTRANSFER_TYPE_MAKER_FEE_PAY\x10\t\x12#\n\x1fTRANSFER_TYPE_MAKER_FEE_RECEIVE\x10\n\x12(\n$TRANSFER_TYPE_INFRASTRUCTURE_FEE_PAY\x10\x0b\x12/\n+TRANSFER_TYPE_INFRASTRUCTURE_FEE_DISTRIBUTE\x10\x0c\x12#\n\x1fTRANSFER_TYPE_LIQUIDITY_FEE_PAY\x10\r\x12*\n&TRANSFER_TYPE_LIQUIDITY_FEE_DISTRIBUTE\x10\x0e\x12\x1a\n\x16TRANSFER_TYPE_BOND_LOW\x10\x0f\x12\x1b\n\x17TRANSFER_TYPE_BOND_HIGH\x10\x10\x12\x1a\n\x16TRANSFER_TYPE_WITHDRAW\x10\x12\x12\x19\n\x15TRANSFER_TYPE_DEPOSIT\x10\x13\x12\x1f\n\x1bTRANSFER_TYPE_BOND_SLASHING\x10\x14\x12\x1f\n\x1bTRANSFER_TYPE_REWARD_PAYOUT\x10\x15\x12%\n!TRANSFER_TYPE_TRANSFER_FUNDS_SEND\x10\x16\x12+\n\'TRANSFER_TYPE_TRANSFER_FUNDS_DISTRIBUTE\x10\x17\x12\x1f\n\x1bTRANSFER_TYPE_CLEAR_ACCOUNT\x10\x18\x12,\n(TRANSFER_TYPE_CHECKPOINT_BALANCE_RESTORE\x10\x19"\x04\x08\x03\x10\x03"\x04\x08\x11\x10\x11*\xc7\x01\n\x0e\x44ispatchMetric\x12\x1f\n\x1b\x44ISPATCH_METRIC_UNSPECIFIED\x10\x00\x12#\n\x1f\x44ISPATCH_METRIC_MAKER_FEES_PAID\x10\x01\x12\'\n#DISPATCH_METRIC_MAKER_FEES_RECEIVED\x10\x02\x12$\n DISPATCH_METRIC_LP_FEES_RECEIVED\x10\x03\x12 \n\x1c\x44ISPATCH_METRIC_MARKET_VALUE\x10\x04*c\n\nNodeStatus\x12\x1b\n\x17NODE_STATUS_UNSPECIFIED\x10\x00\x12\x19\n\x15NODE_STATUS_VALIDATOR\x10\x01\x12\x1d\n\x19NODE_STATUS_NON_VALIDATOR\x10\x02*Y\n\x0b\x45pochAction\x12\x1c\n\x18\x45POCH_ACTION_UNSPECIFIED\x10\x00\x12\x16\n\x12\x45POCH_ACTION_START\x10\x01\x12\x14\n\x10\x45POCH_ACTION_END\x10\x02*\xa7\x01\n\x13ValidatorNodeStatus\x12%\n!VALIDATOR_NODE_STATUS_UNSPECIFIED\x10\x00\x12$\n VALIDATOR_NODE_STATUS_TENDERMINT\x10\x01\x12 \n\x1cVALIDATOR_NODE_STATUS_ERSATZ\x10\x02\x12!\n\x1dVALIDATOR_NODE_STATUS_PENDING\x10\x03\x42\'Z%code.vegaprotocol.io/vega/protos/vegab\x06proto3'
+    b'\n\x0fvega/vega.proto\x12\x04vega\x1a\x12vega/markets.proto"\x17\n\x05Party\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id"N\n\nRiskFactor\x12\x16\n\x06market\x18\x01 \x01(\tR\x06market\x12\x14\n\x05short\x18\x02 \x01(\tR\x05short\x12\x12\n\x04long\x18\x03 \x01(\tR\x04long"Z\n\x0bPeggedOrder\x12\x33\n\treference\x18\x01 \x01(\x0e\x32\x15.vega.PeggedReferenceR\treference\x12\x16\n\x06offset\x18\x02 \x01(\tR\x06offset"\xf2\x08\n\x05Order\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x03 \x01(\tR\x07partyId\x12\x1e\n\x04side\x18\x04 \x01(\x0e\x32\n.vega.SideR\x04side\x12\x14\n\x05price\x18\x05 \x01(\tR\x05price\x12\x12\n\x04size\x18\x06 \x01(\x04R\x04size\x12\x1c\n\tremaining\x18\x07 \x01(\x04R\tremaining\x12;\n\rtime_in_force\x18\x08 \x01(\x0e\x32\x17.vega.Order.TimeInForceR\x0btimeInForce\x12$\n\x04type\x18\t \x01(\x0e\x32\x10.vega.Order.TypeR\x04type\x12\x1d\n\ncreated_at\x18\n \x01(\x03R\tcreatedAt\x12*\n\x06status\x18\x0b \x01(\x0e\x32\x12.vega.Order.StatusR\x06status\x12\x1d\n\nexpires_at\x18\x0c \x01(\x03R\texpiresAt\x12\x1c\n\treference\x18\r \x01(\tR\treference\x12-\n\x06reason\x18\x0e \x01(\x0e\x32\x10.vega.OrderErrorH\x00R\x06reason\x88\x01\x01\x12\x1d\n\nupdated_at\x18\x0f \x01(\x03R\tupdatedAt\x12\x18\n\x07version\x18\x10 \x01(\x04R\x07version\x12\x19\n\x08\x62\x61tch_id\x18\x11 \x01(\x04R\x07\x62\x61tchId\x12\x34\n\x0cpegged_order\x18\x12 \x01(\x0b\x32\x11.vega.PeggedOrderR\x0bpeggedOrder\x12\x34\n\x16liquidity_provision_id\x18\x13 \x01(\tR\x14liquidityProvisionId"\xb6\x01\n\x0bTimeInForce\x12\x1d\n\x19TIME_IN_FORCE_UNSPECIFIED\x10\x00\x12\x15\n\x11TIME_IN_FORCE_GTC\x10\x01\x12\x15\n\x11TIME_IN_FORCE_GTT\x10\x02\x12\x15\n\x11TIME_IN_FORCE_IOC\x10\x03\x12\x15\n\x11TIME_IN_FORCE_FOK\x10\x04\x12\x15\n\x11TIME_IN_FORCE_GFA\x10\x05\x12\x15\n\x11TIME_IN_FORCE_GFN\x10\x06"O\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0e\n\nTYPE_LIMIT\x10\x01\x12\x0f\n\x0bTYPE_MARKET\x10\x02\x12\x10\n\x0cTYPE_NETWORK\x10\x03"\xc9\x01\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x11\n\rSTATUS_ACTIVE\x10\x01\x12\x12\n\x0eSTATUS_EXPIRED\x10\x02\x12\x14\n\x10STATUS_CANCELLED\x10\x03\x12\x12\n\x0eSTATUS_STOPPED\x10\x04\x12\x11\n\rSTATUS_FILLED\x10\x05\x12\x13\n\x0fSTATUS_REJECTED\x10\x06\x12\x1b\n\x17STATUS_PARTIALLY_FILLED\x10\x07\x12\x11\n\rSTATUS_PARKED\x10\x08\x42\t\n\x07_reason"B\n\x1dOrderCancellationConfirmation\x12!\n\x05order\x18\x01 \x01(\x0b\x32\x0b.vega.OrderR\x05order"\xa0\x01\n\x11OrderConfirmation\x12!\n\x05order\x18\x01 \x01(\x0b\x32\x0b.vega.OrderR\x05order\x12#\n\x06trades\x18\x02 \x03(\x0b\x32\x0b.vega.TradeR\x06trades\x12\x43\n\x17passive_orders_affected\x18\x03 \x03(\x0b\x32\x0b.vega.OrderR\x15passiveOrdersAffected"\xd3\x01\n\x16\x41uctionIndicativeState\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12)\n\x10indicative_price\x18\x02 \x01(\tR\x0findicativePrice\x12+\n\x11indicative_volume\x18\x03 \x01(\x04R\x10indicativeVolume\x12#\n\rauction_start\x18\x04 \x01(\x03R\x0c\x61uctionStart\x12\x1f\n\x0b\x61uction_end\x18\x05 \x01(\x03R\nauctionEnd"\xdb\x04\n\x05Trade\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x14\n\x05price\x18\x03 \x01(\tR\x05price\x12\x12\n\x04size\x18\x04 \x01(\x04R\x04size\x12\x14\n\x05\x62uyer\x18\x05 \x01(\tR\x05\x62uyer\x12\x16\n\x06seller\x18\x06 \x01(\tR\x06seller\x12(\n\taggressor\x18\x07 \x01(\x0e\x32\n.vega.SideR\taggressor\x12\x1b\n\tbuy_order\x18\x08 \x01(\tR\x08\x62uyOrder\x12\x1d\n\nsell_order\x18\t \x01(\tR\tsellOrder\x12\x1c\n\ttimestamp\x18\n \x01(\x03R\ttimestamp\x12$\n\x04type\x18\x0b \x01(\x0e\x32\x10.vega.Trade.TypeR\x04type\x12&\n\tbuyer_fee\x18\x0c \x01(\x0b\x32\t.vega.FeeR\x08\x62uyerFee\x12(\n\nseller_fee\x18\r \x01(\x0b\x32\t.vega.FeeR\tsellerFee\x12.\n\x13\x62uyer_auction_batch\x18\x0e \x01(\x04R\x11\x62uyerAuctionBatch\x12\x30\n\x14seller_auction_batch\x18\x0f \x01(\x04R\x12sellerAuctionBatch"o\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x10\n\x0cTYPE_DEFAULT\x10\x01\x12\x1f\n\x1bTYPE_NETWORK_CLOSE_OUT_GOOD\x10\x02\x12\x1e\n\x1aTYPE_NETWORK_CLOSE_OUT_BAD\x10\x03"v\n\x03\x46\x65\x65\x12\x1b\n\tmaker_fee\x18\x01 \x01(\tR\x08makerFee\x12-\n\x12infrastructure_fee\x18\x02 \x01(\tR\x11infrastructureFee\x12#\n\rliquidity_fee\x18\x03 \x01(\tR\x0cliquidityFee"/\n\x08TradeSet\x12#\n\x06trades\x18\x01 \x03(\x0b\x32\x0b.vega.TradeR\x06trades"\xd6\x01\n\x06\x43\x61ndle\x12\x1c\n\ttimestamp\x18\x01 \x01(\x03R\ttimestamp\x12\x1a\n\x08\x64\x61tetime\x18\x02 \x01(\tR\x08\x64\x61tetime\x12\x12\n\x04high\x18\x03 \x01(\tR\x04high\x12\x10\n\x03low\x18\x04 \x01(\tR\x03low\x12\x12\n\x04open\x18\x05 \x01(\tR\x04open\x12\x14\n\x05\x63lose\x18\x06 \x01(\tR\x05\x63lose\x12\x16\n\x06volume\x18\x07 \x01(\x04R\x06volume\x12*\n\x08interval\x18\x08 \x01(\x0e\x32\x0e.vega.IntervalR\x08interval"d\n\nPriceLevel\x12\x14\n\x05price\x18\x01 \x01(\tR\x05price\x12(\n\x10number_of_orders\x18\x02 \x01(\x04R\x0enumberOfOrders\x12\x16\n\x06volume\x18\x03 \x01(\x04R\x06volume"\x9d\x01\n\x0bMarketDepth\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12"\n\x03\x62uy\x18\x02 \x03(\x0b\x32\x10.vega.PriceLevelR\x03\x62uy\x12$\n\x04sell\x18\x03 \x03(\x0b\x32\x10.vega.PriceLevelR\x04sell\x12\'\n\x0fsequence_number\x18\x04 \x01(\x04R\x0esequenceNumber"\xdd\x01\n\x11MarketDepthUpdate\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12"\n\x03\x62uy\x18\x02 \x03(\x0b\x32\x10.vega.PriceLevelR\x03\x62uy\x12$\n\x04sell\x18\x03 \x03(\x0b\x32\x10.vega.PriceLevelR\x04sell\x12\'\n\x0fsequence_number\x18\x04 \x01(\x04R\x0esequenceNumber\x12\x38\n\x18previous_sequence_number\x18\x05 \x01(\x04R\x16previousSequenceNumber"\xf7\x02\n\x08Position\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x1f\n\x0bopen_volume\x18\x03 \x01(\x03R\nopenVolume\x12!\n\x0crealised_pnl\x18\x04 \x01(\tR\x0brealisedPnl\x12%\n\x0eunrealised_pnl\x18\x05 \x01(\tR\runrealisedPnl\x12.\n\x13\x61verage_entry_price\x18\x06 \x01(\tR\x11\x61verageEntryPrice\x12\x1d\n\nupdated_at\x18\x07 \x01(\x03R\tupdatedAt\x12:\n\x19loss_socialisation_amount\x18\x08 \x01(\tR\x17lossSocialisationAmount\x12=\n\x0fposition_status\x18\t \x01(\x0e\x32\x14.vega.PositionStatusR\x0epositionStatus"=\n\rPositionTrade\x12\x16\n\x06volume\x18\x01 \x01(\x03R\x06volume\x12\x14\n\x05price\x18\x02 \x01(\tR\x05price"\xe4\x02\n\x07\x44\x65posit\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12,\n\x06status\x18\x02 \x01(\x0e\x32\x14.vega.Deposit.StatusR\x06status\x12\x19\n\x08party_id\x18\x03 \x01(\tR\x07partyId\x12\x14\n\x05\x61sset\x18\x04 \x01(\tR\x05\x61sset\x12\x16\n\x06\x61mount\x18\x05 \x01(\tR\x06\x61mount\x12\x17\n\x07tx_hash\x18\x06 \x01(\tR\x06txHash\x12-\n\x12\x63redited_timestamp\x18\x07 \x01(\x03R\x11\x63reditedTimestamp\x12+\n\x11\x63reated_timestamp\x18\x08 \x01(\x03R\x10\x63reatedTimestamp"]\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x0f\n\x0bSTATUS_OPEN\x10\x01\x12\x14\n\x10STATUS_CANCELLED\x10\x02\x12\x14\n\x10STATUS_FINALIZED\x10\x03"\xa8\x03\n\nWithdrawal\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x14\n\x05\x61sset\x18\x04 \x01(\tR\x05\x61sset\x12/\n\x06status\x18\x05 \x01(\x0e\x32\x17.vega.Withdrawal.StatusR\x06status\x12\x10\n\x03ref\x18\x06 \x01(\tR\x03ref\x12\x17\n\x07tx_hash\x18\x08 \x01(\tR\x06txHash\x12+\n\x11\x63reated_timestamp\x18\t \x01(\x03R\x10\x63reatedTimestamp\x12/\n\x13withdrawn_timestamp\x18\n \x01(\x03R\x12withdrawnTimestamp\x12#\n\x03\x65xt\x18\x0b \x01(\x0b\x32\x11.vega.WithdrawExtR\x03\x65xt"\\\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x0f\n\x0bSTATUS_OPEN\x10\x01\x12\x13\n\x0fSTATUS_REJECTED\x10\x02\x12\x14\n\x10STATUS_FINALIZED\x10\x03J\x04\x08\x07\x10\x08"D\n\x0bWithdrawExt\x12.\n\x05\x65rc20\x18\x01 \x01(\x0b\x32\x16.vega.Erc20WithdrawExtH\x00R\x05\x65rc20B\x05\n\x03\x65xt"=\n\x10\x45rc20WithdrawExt\x12)\n\x10receiver_address\x18\x01 \x01(\tR\x0freceiverAddress"\xa3\x01\n\x07\x41\x63\x63ount\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x14\n\x05owner\x18\x02 \x01(\tR\x05owner\x12\x18\n\x07\x62\x61lance\x18\x03 \x01(\tR\x07\x62\x61lance\x12\x14\n\x05\x61sset\x18\x04 \x01(\tR\x05\x61sset\x12\x1b\n\tmarket_id\x18\x05 \x01(\tR\x08marketId\x12%\n\x04type\x18\x06 \x01(\x0e\x32\x11.vega.AccountTypeR\x04type"?\n\x0f\x46inancialAmount\x12\x16\n\x06\x61mount\x18\x01 \x01(\tR\x06\x61mount\x12\x14\n\x05\x61sset\x18\x02 \x01(\tR\x05\x61sset"\xb3\x01\n\x08Transfer\x12\x14\n\x05owner\x18\x01 \x01(\tR\x05owner\x12-\n\x06\x61mount\x18\x02 \x01(\x0b\x32\x15.vega.FinancialAmountR\x06\x61mount\x12&\n\x04type\x18\x03 \x01(\x0e\x32\x12.vega.TransferTypeR\x04type\x12\x1d\n\nmin_amount\x18\x04 \x01(\tR\tminAmount\x12\x1b\n\tmarket_id\x18\x05 \x01(\tR\x08marketId"\x84\x01\n\x10\x44ispatchStrategy\x12(\n\x10\x61sset_for_metric\x18\x01 \x01(\tR\x0e\x61ssetForMetric\x12,\n\x06metric\x18\x02 \x01(\x0e\x32\x14.vega.DispatchMetricR\x06metric\x12\x18\n\x07markets\x18\x03 \x03(\tR\x07markets"\xe6\x01\n\x0fTransferRequest\x12\x30\n\x0c\x66rom_account\x18\x01 \x03(\x0b\x32\r.vega.AccountR\x0b\x66romAccount\x12,\n\nto_account\x18\x02 \x03(\x0b\x32\r.vega.AccountR\ttoAccount\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x1d\n\nmin_amount\x18\x04 \x01(\tR\tminAmount\x12\x14\n\x05\x61sset\x18\x05 \x01(\tR\x05\x61sset\x12&\n\x04type\x18\x07 \x01(\x0e\x32\x12.vega.TransferTypeR\x04type"\xa7\x01\n\x0e\x41\x63\x63ountDetails\x12\x19\n\x08\x61sset_id\x18\x01 \x01(\tR\x07\x61ssetId\x12%\n\x04type\x18\x02 \x01(\x0e\x32\x11.vega.AccountTypeR\x04type\x12\x19\n\x05owner\x18\x03 \x01(\tH\x00R\x05owner\x88\x01\x01\x12 \n\tmarket_id\x18\x04 \x01(\tH\x01R\x08marketId\x88\x01\x01\x42\x08\n\x06_ownerB\x0c\n\n_market_id"\xb9\x02\n\x0bLedgerEntry\x12\x37\n\x0c\x66rom_account\x18\x01 \x01(\x0b\x32\x14.vega.AccountDetailsR\x0b\x66romAccount\x12\x33\n\nto_account\x18\x02 \x01(\x0b\x32\x14.vega.AccountDetailsR\ttoAccount\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12&\n\x04type\x18\x04 \x01(\x0e\x32\x12.vega.TransferTypeR\x04type\x12\x1c\n\ttimestamp\x18\x05 \x01(\x03R\ttimestamp\x12\x30\n\x14\x66rom_account_balance\x18\x06 \x01(\tR\x12\x66romAccountBalance\x12,\n\x12to_account_balance\x18\x07 \x01(\tR\x10toAccountBalance"_\n\x13PostTransferBalance\x12.\n\x07\x61\x63\x63ount\x18\x01 \x01(\x0b\x32\x14.vega.AccountDetailsR\x07\x61\x63\x63ount\x12\x18\n\x07\x62\x61lance\x18\x02 \x01(\tR\x07\x62\x61lance"t\n\x0eLedgerMovement\x12+\n\x07\x65ntries\x18\x01 \x03(\x0b\x32\x11.vega.LedgerEntryR\x07\x65ntries\x12\x35\n\x08\x62\x61lances\x18\x02 \x03(\x0b\x32\x19.vega.PostTransferBalanceR\x08\x62\x61lances"\xad\x02\n\x0cMarginLevels\x12-\n\x12maintenance_margin\x18\x01 \x01(\tR\x11maintenanceMargin\x12!\n\x0csearch_level\x18\x02 \x01(\tR\x0bsearchLevel\x12%\n\x0einitial_margin\x18\x03 \x01(\tR\rinitialMargin\x12\x38\n\x18\x63ollateral_release_level\x18\x04 \x01(\tR\x16\x63ollateralReleaseLevel\x12\x19\n\x08party_id\x18\x05 \x01(\tR\x07partyId\x12\x1b\n\tmarket_id\x18\x06 \x01(\tR\x08marketId\x12\x14\n\x05\x61sset\x18\x07 \x01(\tR\x05\x61sset\x12\x1c\n\ttimestamp\x18\x08 \x01(\x03R\ttimestamp"\xe5\n\n\nMarketData\x12\x1d\n\nmark_price\x18\x01 \x01(\tR\tmarkPrice\x12$\n\x0e\x62\x65st_bid_price\x18\x02 \x01(\tR\x0c\x62\x65stBidPrice\x12&\n\x0f\x62\x65st_bid_volume\x18\x03 \x01(\x04R\rbestBidVolume\x12(\n\x10\x62\x65st_offer_price\x18\x04 \x01(\tR\x0e\x62\x65stOfferPrice\x12*\n\x11\x62\x65st_offer_volume\x18\x05 \x01(\x04R\x0f\x62\x65stOfferVolume\x12\x31\n\x15\x62\x65st_static_bid_price\x18\x06 \x01(\tR\x12\x62\x65stStaticBidPrice\x12\x33\n\x16\x62\x65st_static_bid_volume\x18\x07 \x01(\x04R\x13\x62\x65stStaticBidVolume\x12\x35\n\x17\x62\x65st_static_offer_price\x18\x08 \x01(\tR\x14\x62\x65stStaticOfferPrice\x12\x37\n\x18\x62\x65st_static_offer_volume\x18\t \x01(\x04R\x15\x62\x65stStaticOfferVolume\x12\x1b\n\tmid_price\x18\n \x01(\tR\x08midPrice\x12(\n\x10static_mid_price\x18\x0b \x01(\tR\x0estaticMidPrice\x12\x16\n\x06market\x18\x0c \x01(\tR\x06market\x12\x1c\n\ttimestamp\x18\r \x01(\x03R\ttimestamp\x12#\n\ropen_interest\x18\x0e \x01(\x04R\x0copenInterest\x12\x1f\n\x0b\x61uction_end\x18\x0f \x01(\x03R\nauctionEnd\x12#\n\rauction_start\x18\x10 \x01(\x03R\x0c\x61uctionStart\x12)\n\x10indicative_price\x18\x11 \x01(\tR\x0findicativePrice\x12+\n\x11indicative_volume\x18\x12 \x01(\x04R\x10indicativeVolume\x12H\n\x13market_trading_mode\x18\x13 \x01(\x0e\x32\x18.vega.Market.TradingModeR\x11marketTradingMode\x12.\n\x07trigger\x18\x14 \x01(\x0e\x32\x14.vega.AuctionTriggerR\x07trigger\x12\x41\n\x11\x65xtension_trigger\x18\x15 \x01(\x0e\x32\x14.vega.AuctionTriggerR\x10\x65xtensionTrigger\x12!\n\x0ctarget_stake\x18\x16 \x01(\tR\x0btargetStake\x12%\n\x0esupplied_stake\x18\x17 \x01(\tR\rsuppliedStake\x12S\n\x17price_monitoring_bounds\x18\x18 \x03(\x0b\x32\x1b.vega.PriceMonitoringBoundsR\x15priceMonitoringBounds\x12,\n\x12market_value_proxy\x18\x19 \x01(\tR\x10marketValueProxy\x12`\n\x1cliquidity_provider_fee_share\x18\x1a \x03(\x0b\x32\x1f.vega.LiquidityProviderFeeShareR\x19liquidityProviderFeeShare\x12\x35\n\x0cmarket_state\x18\x1b \x01(\x0e\x32\x12.vega.Market.StateR\x0bmarketState\x12-\n\x13next_mark_to_market\x18\x1c \x01(\x03R\x10nextMarkToMarket\x12*\n\x11last_traded_price\x18\x1d \x01(\tR\x0flastTradedPrice"\xba\x01\n\x19LiquidityProviderFeeShare\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12*\n\x11\x65quity_like_share\x18\x02 \x01(\tR\x0f\x65quityLikeShare\x12\x36\n\x17\x61verage_entry_valuation\x18\x03 \x01(\tR\x15\x61verageEntryValuation\x12#\n\raverage_score\x18\x04 \x01(\tR\x0c\x61verageScore"\xc8\x01\n\x15PriceMonitoringBounds\x12&\n\x0fmin_valid_price\x18\x01 \x01(\tR\rminValidPrice\x12&\n\x0fmax_valid_price\x18\x02 \x01(\tR\rmaxValidPrice\x12\x36\n\x07trigger\x18\x03 \x01(\x0b\x32\x1c.vega.PriceMonitoringTriggerR\x07trigger\x12\'\n\x0freference_price\x18\x04 \x01(\tR\x0ereferencePrice"Q\n\x0b\x45rrorDetail\x12\x12\n\x04\x63ode\x18\x01 \x01(\x05R\x04\x63ode\x12\x18\n\x07message\x18\x02 \x01(\tR\x07message\x12\x14\n\x05inner\x18\x03 \x01(\tR\x05inner":\n\x10NetworkParameter\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value"\x82\x03\n\rNetworkLimits\x12,\n\x12\x63\x61n_propose_market\x18\x01 \x01(\x08R\x10\x63\x61nProposeMarket\x12*\n\x11\x63\x61n_propose_asset\x18\x02 \x01(\x08R\x0f\x63\x61nProposeAsset\x12\x34\n\x16propose_market_enabled\x18\x04 \x01(\x08R\x14proposeMarketEnabled\x12\x32\n\x15propose_asset_enabled\x18\x05 \x01(\x08R\x13proposeAssetEnabled\x12%\n\x0egenesis_loaded\x18\x07 \x01(\x08R\rgenesisLoaded\x12=\n\x1bpropose_market_enabled_from\x18\x08 \x01(\x03R\x18proposeMarketEnabledFrom\x12;\n\x1apropose_asset_enabled_from\x18\t \x01(\x03R\x17proposeAssetEnabledFromJ\x04\x08\x03\x10\x04J\x04\x08\x06\x10\x07"}\n\x0eLiquidityOrder\x12\x33\n\treference\x18\x01 \x01(\x0e\x32\x15.vega.PeggedReferenceR\treference\x12\x1e\n\nproportion\x18\x02 \x01(\rR\nproportion\x12\x16\n\x06offset\x18\x03 \x01(\tR\x06offset"s\n\x17LiquidityOrderReference\x12\x19\n\x08order_id\x18\x01 \x01(\tR\x07orderId\x12=\n\x0fliquidity_order\x18\x02 \x01(\x0b\x32\x14.vega.LiquidityOrderR\x0eliquidityOrder"\xd2\x04\n\x12LiquidityProvision\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x1d\n\ncreated_at\x18\x03 \x01(\x03R\tcreatedAt\x12\x1d\n\nupdated_at\x18\x04 \x01(\x03R\tupdatedAt\x12\x1b\n\tmarket_id\x18\x05 \x01(\tR\x08marketId\x12+\n\x11\x63ommitment_amount\x18\x06 \x01(\tR\x10\x63ommitmentAmount\x12\x10\n\x03\x66\x65\x65\x18\x07 \x01(\tR\x03\x66\x65\x65\x12\x33\n\x05sells\x18\x08 \x03(\x0b\x32\x1d.vega.LiquidityOrderReferenceR\x05sells\x12\x31\n\x04\x62uys\x18\t \x03(\x0b\x32\x1d.vega.LiquidityOrderReferenceR\x04\x62uys\x12\x18\n\x07version\x18\n \x01(\x04R\x07version\x12\x37\n\x06status\x18\x0b \x01(\x0e\x32\x1f.vega.LiquidityProvision.StatusR\x06status\x12\x1c\n\treference\x18\x0c \x01(\tR\treference"\x9d\x01\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x11\n\rSTATUS_ACTIVE\x10\x01\x12\x12\n\x0eSTATUS_STOPPED\x10\x02\x12\x14\n\x10STATUS_CANCELLED\x10\x03\x12\x13\n\x0fSTATUS_REJECTED\x10\x04\x12\x15\n\x11STATUS_UNDEPLOYED\x10\x05\x12\x12\n\x0eSTATUS_PENDING\x10\x06"\xd0\x03\n\x0e\x45thereumConfig\x12\x1d\n\nnetwork_id\x18\x01 \x01(\tR\tnetworkId\x12\x19\n\x08\x63hain_id\x18\x02 \x01(\tR\x07\x63hainId\x12Z\n\x1a\x63ollateral_bridge_contract\x18\x03 \x01(\x0b\x32\x1c.vega.EthereumContractConfigR\x18\x63ollateralBridgeContract\x12$\n\rconfirmations\x18\x04 \x01(\rR\rconfirmations\x12T\n\x17staking_bridge_contract\x18\x05 \x01(\x0b\x32\x1c.vega.EthereumContractConfigR\x15stakingBridgeContract\x12R\n\x16token_vesting_contract\x18\x06 \x01(\x0b\x32\x1c.vega.EthereumContractConfigR\x14tokenVestingContract\x12X\n\x19multisig_control_contract\x18\x07 \x01(\x0b\x32\x1c.vega.EthereumContractConfigR\x17multisigControlContract"j\n\x16\x45thereumContractConfig\x12\x18\n\x07\x61\x64\x64ress\x18\x01 \x01(\tR\x07\x61\x64\x64ress\x12\x36\n\x17\x64\x65ployment_block_height\x18\x06 \x01(\x04R\x15\x64\x65ploymentBlockHeight"\xac\x01\n\x0f\x45pochTimestamps\x12\x1d\n\nstart_time\x18\x01 \x01(\x03R\tstartTime\x12\x1f\n\x0b\x65xpiry_time\x18\x02 \x01(\x03R\nexpiryTime\x12\x19\n\x08\x65nd_time\x18\x03 \x01(\x03R\x07\x65ndTime\x12\x1f\n\x0b\x66irst_block\x18\x04 \x01(\x04R\nfirstBlock\x12\x1d\n\nlast_block\x18\x05 \x01(\x04R\tlastBlock"\xb0\x01\n\x05\x45poch\x12\x10\n\x03seq\x18\x01 \x01(\x04R\x03seq\x12\x35\n\ntimestamps\x18\x02 \x01(\x0b\x32\x15.vega.EpochTimestampsR\ntimestamps\x12*\n\nvalidators\x18\x03 \x03(\x0b\x32\n.vega.NodeR\nvalidators\x12\x32\n\x0b\x64\x65legations\x18\x04 \x03(\x0b\x32\x10.vega.DelegationR\x0b\x64\x65legations"\x8e\x01\n\x12\x45pochParticipation\x12!\n\x05\x65poch\x18\x01 \x01(\x0b\x32\x0b.vega.EpochR\x05\x65poch\x12\x18\n\x07offline\x18\x02 \x01(\x04R\x07offline\x12\x16\n\x06online\x18\x03 \x01(\x04R\x06online\x12#\n\rtotal_rewards\x18\x04 \x01(\x01R\x0ctotalRewards"S\n\tEpochData\x12\x14\n\x05total\x18\x01 \x01(\x05R\x05total\x12\x18\n\x07offline\x18\x02 \x01(\x05R\x07offline\x12\x16\n\x06online\x18\x03 \x01(\x05R\x06online"\x9b\x02\n\x0cRankingScore\x12\x1f\n\x0bstake_score\x18\x01 \x01(\tR\nstakeScore\x12+\n\x11performance_score\x18\x02 \x01(\tR\x10performanceScore\x12\x42\n\x0fprevious_status\x18\x03 \x01(\x0e\x32\x19.vega.ValidatorNodeStatusR\x0epreviousStatus\x12\x31\n\x06status\x18\x04 \x01(\x0e\x32\x19.vega.ValidatorNodeStatusR\x06status\x12!\n\x0cvoting_power\x18\x05 \x01(\rR\x0bvotingPower\x12#\n\rranking_score\x18\x06 \x01(\tR\x0crankingScore"\xab\x02\n\x0bRewardScore\x12.\n\x13raw_validator_score\x18\x01 \x01(\tR\x11rawValidatorScore\x12+\n\x11performance_score\x18\x02 \x01(\tR\x10performanceScore\x12%\n\x0emultisig_score\x18\x03 \x01(\tR\rmultisigScore\x12\'\n\x0fvalidator_score\x18\x04 \x01(\tR\x0evalidatorScore\x12)\n\x10normalised_score\x18\x05 \x01(\tR\x0fnormalisedScore\x12\x44\n\x10validator_status\x18\x06 \x01(\x0e\x32\x19.vega.ValidatorNodeStatusR\x0fvalidatorStatus"\xb3\x05\n\x04Node\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x17\n\x07pub_key\x18\x02 \x01(\tR\x06pubKey\x12\x1c\n\ntm_pub_key\x18\x03 \x01(\tR\x08tmPubKey\x12)\n\x10\x65thereum_address\x18\x04 \x01(\tR\x0f\x65thereumAddress\x12\x19\n\x08info_url\x18\x05 \x01(\tR\x07infoUrl\x12\x1a\n\x08location\x18\x06 \x01(\tR\x08location\x12,\n\x12staked_by_operator\x18\x07 \x01(\tR\x10stakedByOperator\x12.\n\x13staked_by_delegates\x18\x08 \x01(\tR\x11stakedByDelegates\x12!\n\x0cstaked_total\x18\t \x01(\tR\x0bstakedTotal\x12,\n\x12max_intended_stake\x18\n \x01(\tR\x10maxIntendedStake\x12#\n\rpending_stake\x18\x0b \x01(\tR\x0cpendingStake\x12.\n\nepoch_data\x18\x0c \x01(\x0b\x32\x0f.vega.EpochDataR\tepochData\x12(\n\x06status\x18\r \x01(\x0e\x32\x10.vega.NodeStatusR\x06status\x12\x32\n\x0b\x64\x65legations\x18\x0e \x03(\x0b\x32\x10.vega.DelegationR\x0b\x64\x65legations\x12\x34\n\x0creward_score\x18\x0f \x01(\x0b\x32\x11.vega.RewardScoreR\x0brewardScore\x12\x37\n\rranking_score\x18\x10 \x01(\x0b\x32\x12.vega.RankingScoreR\x0crankingScore\x12\x12\n\x04name\x18\x11 \x01(\tR\x04name\x12\x1d\n\navatar_url\x18\x12 \x01(\tR\tavatarUrl"\x9c\x01\n\x07NodeSet\x12\x14\n\x05total\x18\x01 \x01(\rR\x05total\x12\x1a\n\x08inactive\x18\x02 \x01(\rR\x08inactive\x12\x1a\n\x08promoted\x18\x03 \x03(\tR\x08promoted\x12\x18\n\x07\x64\x65moted\x18\x04 \x03(\tR\x07\x64\x65moted\x12\x1d\n\x07maximum\x18\x05 \x01(\rH\x00R\x07maximum\x88\x01\x01\x42\n\n\x08_maximum"\xad\x02\n\x08NodeData\x12!\n\x0cstaked_total\x18\x01 \x01(\tR\x0bstakedTotal\x12\x1f\n\x0btotal_nodes\x18\x02 \x01(\rR\ntotalNodes\x12%\n\x0einactive_nodes\x18\x03 \x01(\rR\rinactiveNodes\x12\x38\n\x10tendermint_nodes\x18\x04 \x01(\x0b\x32\r.vega.NodeSetR\x0ftendermintNodes\x12\x30\n\x0c\x65rsatz_nodes\x18\x05 \x01(\x0b\x32\r.vega.NodeSetR\x0b\x65rsatzNodes\x12\x32\n\rpending_nodes\x18\x06 \x01(\x0b\x32\r.vega.NodeSetR\x0cpendingNodes\x12\x16\n\x06uptime\x18\x07 \x01(\x02R\x06uptime"p\n\nDelegation\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x17\n\x07node_id\x18\x02 \x01(\tR\x06nodeId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x1b\n\tepoch_seq\x18\x04 \x01(\tR\x08\x65pochSeq"\xfb\x01\n\x06Reward\x12\x19\n\x08\x61sset_id\x18\x01 \x01(\tR\x07\x61ssetId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x14\n\x05\x65poch\x18\x03 \x01(\x04R\x05\x65poch\x12\x16\n\x06\x61mount\x18\x04 \x01(\tR\x06\x61mount\x12.\n\x13percentage_of_total\x18\x05 \x01(\tR\x11percentageOfTotal\x12\x1f\n\x0breceived_at\x18\x06 \x01(\x03R\nreceivedAt\x12\x1b\n\tmarket_id\x18\x07 \x01(\tR\x08marketId\x12\x1f\n\x0breward_type\x18\x08 \x01(\tR\nrewardType"]\n\rRewardSummary\x12\x19\n\x08\x61sset_id\x18\x01 \x01(\tR\x07\x61ssetId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount"\x9b\x01\n\x12\x45pochRewardSummary\x12\x14\n\x05\x65poch\x18\x01 \x01(\x04R\x05\x65poch\x12\x19\n\x08\x61sset_id\x18\x02 \x01(\tR\x07\x61ssetId\x12\x1b\n\tmarket_id\x18\x03 \x01(\tR\x08marketId\x12\x1f\n\x0breward_type\x18\x04 \x01(\tR\nrewardType\x12\x16\n\x06\x61mount\x18\x05 \x01(\tR\x06\x61mount"y\n\x12StateValueProposal\x12 \n\x0cstate_var_id\x18\x01 \x01(\tR\nstateVarId\x12\x19\n\x08\x65vent_id\x18\x02 \x01(\tR\x07\x65ventId\x12&\n\x03kvb\x18\x03 \x03(\x0b\x32\x14.vega.KeyValueBundleR\x03kvb"k\n\x0eKeyValueBundle\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x1c\n\ttolerance\x18\x02 \x01(\tR\ttolerance\x12)\n\x05value\x18\x03 \x01(\x0b\x32\x13.vega.StateVarValueR\x05value"\xb4\x01\n\rStateVarValue\x12\x32\n\nscalar_val\x18\x01 \x01(\x0b\x32\x11.vega.ScalarValueH\x00R\tscalarVal\x12\x32\n\nvector_val\x18\x02 \x01(\x0b\x32\x11.vega.VectorValueH\x00R\tvectorVal\x12\x32\n\nmatrix_val\x18\x03 \x01(\x0b\x32\x11.vega.MatrixValueH\x00R\tmatrixValB\x07\n\x05value"#\n\x0bScalarValue\x12\x14\n\x05value\x18\x01 \x01(\tR\x05value"#\n\x0bVectorValue\x12\x14\n\x05value\x18\x01 \x03(\tR\x05value"6\n\x0bMatrixValue\x12\'\n\x05value\x18\x01 \x03(\x0b\x32\x11.vega.VectorValueR\x05value*9\n\x04Side\x12\x14\n\x10SIDE_UNSPECIFIED\x10\x00\x12\x0c\n\x08SIDE_BUY\x10\x01\x12\r\n\tSIDE_SELL\x10\x02*\x98\x01\n\x08Interval\x12\x18\n\x14INTERVAL_UNSPECIFIED\x10\x00\x12\x10\n\x0cINTERVAL_I1M\x10<\x12\x11\n\x0cINTERVAL_I5M\x10\xac\x02\x12\x12\n\rINTERVAL_I15M\x10\x84\x07\x12\x11\n\x0cINTERVAL_I1H\x10\x90\x1c\x12\x12\n\x0cINTERVAL_I6H\x10\xe0\xa8\x01\x12\x12\n\x0cINTERVAL_I1D\x10\x80\xa3\x05*t\n\x0ePositionStatus\x12\x1f\n\x1bPOSITION_STATUS_UNSPECIFIED\x10\x00\x12!\n\x1dPOSITION_STATUS_ORDERS_CLOSED\x10\x01\x12\x1e\n\x1aPOSITION_STATUS_CLOSED_OUT\x10\x02*\xa3\x01\n\x0e\x41uctionTrigger\x12\x1f\n\x1b\x41UCTION_TRIGGER_UNSPECIFIED\x10\x00\x12\x19\n\x15\x41UCTION_TRIGGER_BATCH\x10\x01\x12\x1b\n\x17\x41UCTION_TRIGGER_OPENING\x10\x02\x12\x19\n\x15\x41UCTION_TRIGGER_PRICE\x10\x03\x12\x1d\n\x19\x41UCTION_TRIGGER_LIQUIDITY\x10\x04*\x8b\x01\n\x0fPeggedReference\x12 \n\x1cPEGGED_REFERENCE_UNSPECIFIED\x10\x00\x12\x18\n\x14PEGGED_REFERENCE_MID\x10\x01\x12\x1d\n\x19PEGGED_REFERENCE_BEST_BID\x10\x02\x12\x1d\n\x19PEGGED_REFERENCE_BEST_ASK\x10\x03*\xdf\x0f\n\nOrderError\x12\x1b\n\x17ORDER_ERROR_UNSPECIFIED\x10\x00\x12!\n\x1dORDER_ERROR_INVALID_MARKET_ID\x10\x01\x12 \n\x1cORDER_ERROR_INVALID_ORDER_ID\x10\x02\x12\x1f\n\x1bORDER_ERROR_OUT_OF_SEQUENCE\x10\x03\x12&\n"ORDER_ERROR_INVALID_REMAINING_SIZE\x10\x04\x12\x1c\n\x18ORDER_ERROR_TIME_FAILURE\x10\x05\x12\x1f\n\x1bORDER_ERROR_REMOVAL_FAILURE\x10\x06\x12+\n\'ORDER_ERROR_INVALID_EXPIRATION_DATETIME\x10\x07\x12\'\n#ORDER_ERROR_INVALID_ORDER_REFERENCE\x10\x08\x12 \n\x1cORDER_ERROR_EDIT_NOT_ALLOWED\x10\t\x12\x1d\n\x19ORDER_ERROR_AMEND_FAILURE\x10\n\x12\x19\n\x15ORDER_ERROR_NOT_FOUND\x10\x0b\x12 \n\x1cORDER_ERROR_INVALID_PARTY_ID\x10\x0c\x12\x1d\n\x19ORDER_ERROR_MARKET_CLOSED\x10\r\x12#\n\x1fORDER_ERROR_MARGIN_CHECK_FAILED\x10\x0e\x12\'\n#ORDER_ERROR_MISSING_GENERAL_ACCOUNT\x10\x0f\x12\x1e\n\x1aORDER_ERROR_INTERNAL_ERROR\x10\x10\x12\x1c\n\x18ORDER_ERROR_INVALID_SIZE\x10\x11\x12#\n\x1fORDER_ERROR_INVALID_PERSISTENCE\x10\x12\x12\x1c\n\x18ORDER_ERROR_INVALID_TYPE\x10\x13\x12\x1c\n\x18ORDER_ERROR_SELF_TRADING\x10\x14\x12.\n*ORDER_ERROR_INSUFFICIENT_FUNDS_TO_PAY_FEES\x10\x15\x12%\n!ORDER_ERROR_INCORRECT_MARKET_TYPE\x10\x16\x12%\n!ORDER_ERROR_INVALID_TIME_IN_FORCE\x10\x17\x12\x37\n3ORDER_ERROR_CANNOT_SEND_GFN_ORDER_DURING_AN_AUCTION\x10\x18\x12?\n;ORDER_ERROR_CANNOT_SEND_GFA_ORDER_DURING_CONTINUOUS_TRADING\x10\x19\x12\x34\n0ORDER_ERROR_CANNOT_AMEND_TO_GTT_WITHOUT_EXPIRYAT\x10\x1a\x12)\n%ORDER_ERROR_EXPIRYAT_BEFORE_CREATEDAT\x10\x1b\x12,\n(ORDER_ERROR_CANNOT_HAVE_GTC_AND_EXPIRYAT\x10\x1c\x12*\n&ORDER_ERROR_CANNOT_AMEND_TO_FOK_OR_IOC\x10\x1d\x12*\n&ORDER_ERROR_CANNOT_AMEND_TO_GFA_OR_GFN\x10\x1e\x12,\n(ORDER_ERROR_CANNOT_AMEND_FROM_GFA_OR_GFN\x10\x1f\x12\x34\n0ORDER_ERROR_CANNOT_SEND_IOC_ORDER_DURING_AUCTION\x10 \x12\x34\n0ORDER_ERROR_CANNOT_SEND_FOK_ORDER_DURING_AUCTION\x10!\x12#\n\x1fORDER_ERROR_MUST_BE_LIMIT_ORDER\x10"\x12"\n\x1eORDER_ERROR_MUST_BE_GTT_OR_GTC\x10#\x12\'\n#ORDER_ERROR_WITHOUT_REFERENCE_PRICE\x10$\x12\x33\n/ORDER_ERROR_BUY_CANNOT_REFERENCE_BEST_ASK_PRICE\x10%\x12\x37\n3ORDER_ERROR_OFFSET_MUST_BE_GREATER_OR_EQUAL_TO_ZERO\x10(\x12\x34\n0ORDER_ERROR_SELL_CANNOT_REFERENCE_BEST_BID_PRICE\x10)\x12\x30\n,ORDER_ERROR_OFFSET_MUST_BE_GREATER_THAN_ZERO\x10*\x12*\n&ORDER_ERROR_INSUFFICIENT_ASSET_BALANCE\x10+\x12\x45\nAORDER_ERROR_CANNOT_AMEND_PEGGED_ORDER_DETAILS_ON_NON_PEGGED_ORDER\x10,\x12.\n*ORDER_ERROR_UNABLE_TO_REPRICE_PEGGED_ORDER\x10-\x12\x35\n1ORDER_ERROR_UNABLE_TO_AMEND_PRICE_ON_PEGGED_ORDER\x10.\x12\x38\n4ORDER_ERROR_NON_PERSISTENT_ORDER_OUT_OF_PRICE_BOUNDS\x10/\x12&\n"ORDER_ERROR_TOO_MANY_PEGGED_ORDERS\x10\x30"\x04\x08&\x10&"\x04\x08\'\x10\'*\x82\x01\n\x0b\x43hainStatus\x12\x1c\n\x18\x43HAIN_STATUS_UNSPECIFIED\x10\x00\x12\x1d\n\x19\x43HAIN_STATUS_DISCONNECTED\x10\x01\x12\x1a\n\x16\x43HAIN_STATUS_REPLAYING\x10\x02\x12\x1a\n\x16\x43HAIN_STATUS_CONNECTED\x10\x03*\xc4\x04\n\x0b\x41\x63\x63ountType\x12\x1c\n\x18\x41\x43\x43OUNT_TYPE_UNSPECIFIED\x10\x00\x12\x1a\n\x16\x41\x43\x43OUNT_TYPE_INSURANCE\x10\x01\x12\x1b\n\x17\x41\x43\x43OUNT_TYPE_SETTLEMENT\x10\x02\x12\x17\n\x13\x41\x43\x43OUNT_TYPE_MARGIN\x10\x03\x12\x18\n\x14\x41\x43\x43OUNT_TYPE_GENERAL\x10\x04\x12$\n ACCOUNT_TYPE_FEES_INFRASTRUCTURE\x10\x05\x12\x1f\n\x1b\x41\x43\x43OUNT_TYPE_FEES_LIQUIDITY\x10\x06\x12\x1b\n\x17\x41\x43\x43OUNT_TYPE_FEES_MAKER\x10\x07\x12\x15\n\x11\x41\x43\x43OUNT_TYPE_BOND\x10\t\x12\x19\n\x15\x41\x43\x43OUNT_TYPE_EXTERNAL\x10\n\x12!\n\x1d\x41\x43\x43OUNT_TYPE_GLOBAL_INSURANCE\x10\x0b\x12\x1e\n\x1a\x41\x43\x43OUNT_TYPE_GLOBAL_REWARD\x10\x0c\x12"\n\x1e\x41\x43\x43OUNT_TYPE_PENDING_TRANSFERS\x10\r\x12\'\n#ACCOUNT_TYPE_REWARD_MAKER_PAID_FEES\x10\x0e\x12+\n\'ACCOUNT_TYPE_REWARD_MAKER_RECEIVED_FEES\x10\x0f\x12(\n$ACCOUNT_TYPE_REWARD_LP_RECEIVED_FEES\x10\x10\x12(\n$ACCOUNT_TYPE_REWARD_MARKET_PROPOSERS\x10\x11"\x04\x08\x08\x10\x08*\xc9\x06\n\x0cTransferType\x12\x1d\n\x19TRANSFER_TYPE_UNSPECIFIED\x10\x00\x12\x16\n\x12TRANSFER_TYPE_LOSS\x10\x01\x12\x15\n\x11TRANSFER_TYPE_WIN\x10\x02\x12\x1a\n\x16TRANSFER_TYPE_MTM_LOSS\x10\x04\x12\x19\n\x15TRANSFER_TYPE_MTM_WIN\x10\x05\x12\x1c\n\x18TRANSFER_TYPE_MARGIN_LOW\x10\x06\x12\x1d\n\x19TRANSFER_TYPE_MARGIN_HIGH\x10\x07\x12$\n TRANSFER_TYPE_MARGIN_CONFISCATED\x10\x08\x12\x1f\n\x1bTRANSFER_TYPE_MAKER_FEE_PAY\x10\t\x12#\n\x1fTRANSFER_TYPE_MAKER_FEE_RECEIVE\x10\n\x12(\n$TRANSFER_TYPE_INFRASTRUCTURE_FEE_PAY\x10\x0b\x12/\n+TRANSFER_TYPE_INFRASTRUCTURE_FEE_DISTRIBUTE\x10\x0c\x12#\n\x1fTRANSFER_TYPE_LIQUIDITY_FEE_PAY\x10\r\x12*\n&TRANSFER_TYPE_LIQUIDITY_FEE_DISTRIBUTE\x10\x0e\x12\x1a\n\x16TRANSFER_TYPE_BOND_LOW\x10\x0f\x12\x1b\n\x17TRANSFER_TYPE_BOND_HIGH\x10\x10\x12\x1a\n\x16TRANSFER_TYPE_WITHDRAW\x10\x12\x12\x19\n\x15TRANSFER_TYPE_DEPOSIT\x10\x13\x12\x1f\n\x1bTRANSFER_TYPE_BOND_SLASHING\x10\x14\x12\x1f\n\x1bTRANSFER_TYPE_REWARD_PAYOUT\x10\x15\x12%\n!TRANSFER_TYPE_TRANSFER_FUNDS_SEND\x10\x16\x12+\n\'TRANSFER_TYPE_TRANSFER_FUNDS_DISTRIBUTE\x10\x17\x12\x1f\n\x1bTRANSFER_TYPE_CLEAR_ACCOUNT\x10\x18\x12,\n(TRANSFER_TYPE_CHECKPOINT_BALANCE_RESTORE\x10\x19"\x04\x08\x03\x10\x03"\x04\x08\x11\x10\x11*\xc7\x01\n\x0e\x44ispatchMetric\x12\x1f\n\x1b\x44ISPATCH_METRIC_UNSPECIFIED\x10\x00\x12#\n\x1f\x44ISPATCH_METRIC_MAKER_FEES_PAID\x10\x01\x12\'\n#DISPATCH_METRIC_MAKER_FEES_RECEIVED\x10\x02\x12$\n DISPATCH_METRIC_LP_FEES_RECEIVED\x10\x03\x12 \n\x1c\x44ISPATCH_METRIC_MARKET_VALUE\x10\x04*c\n\nNodeStatus\x12\x1b\n\x17NODE_STATUS_UNSPECIFIED\x10\x00\x12\x19\n\x15NODE_STATUS_VALIDATOR\x10\x01\x12\x1d\n\x19NODE_STATUS_NON_VALIDATOR\x10\x02*Y\n\x0b\x45pochAction\x12\x1c\n\x18\x45POCH_ACTION_UNSPECIFIED\x10\x00\x12\x16\n\x12\x45POCH_ACTION_START\x10\x01\x12\x14\n\x10\x45POCH_ACTION_END\x10\x02*\xa7\x01\n\x13ValidatorNodeStatus\x12%\n!VALIDATOR_NODE_STATUS_UNSPECIFIED\x10\x00\x12$\n VALIDATOR_NODE_STATUS_TENDERMINT\x10\x01\x12 \n\x1cVALIDATOR_NODE_STATUS_ERSATZ\x10\x02\x12!\n\x1dVALIDATOR_NODE_STATUS_PENDING\x10\x03\x42\'Z%code.vegaprotocol.io/vega/protos/vegab\x06proto3'
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "vega.vega_pb2", globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b"Z%code.vegaprotocol.io/vega/protos/vega"
-    _SIDE._serialized_start = 13548
-    _SIDE._serialized_end = 13605
-    _INTERVAL._serialized_start = 13608
-    _INTERVAL._serialized_end = 13760
-    _AUCTIONTRIGGER._serialized_start = 13763
-    _AUCTIONTRIGGER._serialized_end = 13926
-    _PEGGEDREFERENCE._serialized_start = 13929
-    _PEGGEDREFERENCE._serialized_end = 14068
-    _ORDERERROR._serialized_start = 14071
-    _ORDERERROR._serialized_end = 16086
-    _CHAINSTATUS._serialized_start = 16089
-    _CHAINSTATUS._serialized_end = 16219
-    _ACCOUNTTYPE._serialized_start = 16222
-    _ACCOUNTTYPE._serialized_end = 16802
-    _TRANSFERTYPE._serialized_start = 16805
-    _TRANSFERTYPE._serialized_end = 17646
-    _DISPATCHMETRIC._serialized_start = 17649
-    _DISPATCHMETRIC._serialized_end = 17848
-    _NODESTATUS._serialized_start = 17850
-    _NODESTATUS._serialized_end = 17949
-    _EPOCHACTION._serialized_start = 17951
-    _EPOCHACTION._serialized_end = 18040
-    _VALIDATORNODESTATUS._serialized_start = 18043
-    _VALIDATORNODESTATUS._serialized_end = 18210
+    _SIDE._serialized_start = 13671
+    _SIDE._serialized_end = 13728
+    _INTERVAL._serialized_start = 13731
+    _INTERVAL._serialized_end = 13883
+    _POSITIONSTATUS._serialized_start = 13885
+    _POSITIONSTATUS._serialized_end = 14001
+    _AUCTIONTRIGGER._serialized_start = 14004
+    _AUCTIONTRIGGER._serialized_end = 14167
+    _PEGGEDREFERENCE._serialized_start = 14170
+    _PEGGEDREFERENCE._serialized_end = 14309
+    _ORDERERROR._serialized_start = 14312
+    _ORDERERROR._serialized_end = 16327
+    _CHAINSTATUS._serialized_start = 16330
+    _CHAINSTATUS._serialized_end = 16460
+    _ACCOUNTTYPE._serialized_start = 16463
+    _ACCOUNTTYPE._serialized_end = 17043
+    _TRANSFERTYPE._serialized_start = 17046
+    _TRANSFERTYPE._serialized_end = 17887
+    _DISPATCHMETRIC._serialized_start = 17890
+    _DISPATCHMETRIC._serialized_end = 18089
+    _NODESTATUS._serialized_start = 18091
+    _NODESTATUS._serialized_end = 18190
+    _EPOCHACTION._serialized_start = 18192
+    _EPOCHACTION._serialized_end = 18281
+    _VALIDATORNODESTATUS._serialized_start = 18284
+    _VALIDATORNODESTATUS._serialized_end = 18451
     _PARTY._serialized_start = 45
     _PARTY._serialized_end = 68
     _RISKFACTOR._serialized_start = 70
     _RISKFACTOR._serialized_end = 148
     _PEGGEDORDER._serialized_start = 150
     _PEGGEDORDER._serialized_end = 240
     _ORDER._serialized_start = 243
@@ -82,105 +83,105 @@
     _PRICELEVEL._serialized_start = 2820
     _PRICELEVEL._serialized_end = 2920
     _MARKETDEPTH._serialized_start = 2923
     _MARKETDEPTH._serialized_end = 3080
     _MARKETDEPTHUPDATE._serialized_start = 3083
     _MARKETDEPTHUPDATE._serialized_end = 3304
     _POSITION._serialized_start = 3307
-    _POSITION._serialized_end = 3559
-    _POSITIONTRADE._serialized_start = 3561
-    _POSITIONTRADE._serialized_end = 3622
-    _DEPOSIT._serialized_start = 3625
-    _DEPOSIT._serialized_end = 3981
-    _DEPOSIT_STATUS._serialized_start = 3888
-    _DEPOSIT_STATUS._serialized_end = 3981
-    _WITHDRAWAL._serialized_start = 3984
-    _WITHDRAWAL._serialized_end = 4408
-    _WITHDRAWAL_STATUS._serialized_start = 4310
-    _WITHDRAWAL_STATUS._serialized_end = 4402
-    _WITHDRAWEXT._serialized_start = 4410
-    _WITHDRAWEXT._serialized_end = 4478
-    _ERC20WITHDRAWEXT._serialized_start = 4480
-    _ERC20WITHDRAWEXT._serialized_end = 4541
-    _ACCOUNT._serialized_start = 4544
-    _ACCOUNT._serialized_end = 4707
-    _FINANCIALAMOUNT._serialized_start = 4709
-    _FINANCIALAMOUNT._serialized_end = 4772
-    _TRANSFER._serialized_start = 4775
-    _TRANSFER._serialized_end = 4954
-    _DISPATCHSTRATEGY._serialized_start = 4957
-    _DISPATCHSTRATEGY._serialized_end = 5089
-    _TRANSFERREQUEST._serialized_start = 5092
-    _TRANSFERREQUEST._serialized_end = 5322
-    _ACCOUNTDETAILS._serialized_start = 5325
-    _ACCOUNTDETAILS._serialized_end = 5492
-    _LEDGERENTRY._serialized_start = 5495
-    _LEDGERENTRY._serialized_end = 5808
-    _POSTTRANSFERBALANCE._serialized_start = 5810
-    _POSTTRANSFERBALANCE._serialized_end = 5905
-    _LEDGERMOVEMENT._serialized_start = 5907
-    _LEDGERMOVEMENT._serialized_end = 6023
-    _MARGINLEVELS._serialized_start = 6026
-    _MARGINLEVELS._serialized_end = 6327
-    _MARKETDATA._serialized_start = 6330
-    _MARKETDATA._serialized_end = 7711
-    _LIQUIDITYPROVIDERFEESHARE._serialized_start = 7714
-    _LIQUIDITYPROVIDERFEESHARE._serialized_end = 7900
-    _PRICEMONITORINGBOUNDS._serialized_start = 7903
-    _PRICEMONITORINGBOUNDS._serialized_end = 8103
-    _ERRORDETAIL._serialized_start = 8105
-    _ERRORDETAIL._serialized_end = 8186
-    _NETWORKPARAMETER._serialized_start = 8188
-    _NETWORKPARAMETER._serialized_end = 8246
-    _NETWORKLIMITS._serialized_start = 8249
-    _NETWORKLIMITS._serialized_end = 8635
-    _LIQUIDITYORDER._serialized_start = 8637
-    _LIQUIDITYORDER._serialized_end = 8762
-    _LIQUIDITYORDERREFERENCE._serialized_start = 8764
-    _LIQUIDITYORDERREFERENCE._serialized_end = 8879
-    _LIQUIDITYPROVISION._serialized_start = 8882
-    _LIQUIDITYPROVISION._serialized_end = 9476
-    _LIQUIDITYPROVISION_STATUS._serialized_start = 9319
-    _LIQUIDITYPROVISION_STATUS._serialized_end = 9476
-    _ETHEREUMCONFIG._serialized_start = 9479
-    _ETHEREUMCONFIG._serialized_end = 9943
-    _ETHEREUMCONTRACTCONFIG._serialized_start = 9945
-    _ETHEREUMCONTRACTCONFIG._serialized_end = 10051
-    _EPOCHTIMESTAMPS._serialized_start = 10054
-    _EPOCHTIMESTAMPS._serialized_end = 10226
-    _EPOCH._serialized_start = 10229
-    _EPOCH._serialized_end = 10405
-    _EPOCHPARTICIPATION._serialized_start = 10408
-    _EPOCHPARTICIPATION._serialized_end = 10550
-    _EPOCHDATA._serialized_start = 10552
-    _EPOCHDATA._serialized_end = 10635
-    _RANKINGSCORE._serialized_start = 10638
-    _RANKINGSCORE._serialized_end = 10921
-    _REWARDSCORE._serialized_start = 10924
-    _REWARDSCORE._serialized_end = 11223
-    _NODE._serialized_start = 11226
-    _NODE._serialized_end = 11917
-    _NODESET._serialized_start = 11920
-    _NODESET._serialized_end = 12076
-    _NODEDATA._serialized_start = 12079
-    _NODEDATA._serialized_end = 12380
-    _DELEGATION._serialized_start = 12382
-    _DELEGATION._serialized_end = 12494
-    _REWARD._serialized_start = 12497
-    _REWARD._serialized_end = 12748
-    _REWARDSUMMARY._serialized_start = 12750
-    _REWARDSUMMARY._serialized_end = 12843
-    _EPOCHREWARDSUMMARY._serialized_start = 12846
-    _EPOCHREWARDSUMMARY._serialized_end = 13001
-    _STATEVALUEPROPOSAL._serialized_start = 13003
-    _STATEVALUEPROPOSAL._serialized_end = 13124
-    _KEYVALUEBUNDLE._serialized_start = 13126
-    _KEYVALUEBUNDLE._serialized_end = 13233
-    _STATEVARVALUE._serialized_start = 13236
-    _STATEVARVALUE._serialized_end = 13416
-    _SCALARVALUE._serialized_start = 13418
-    _SCALARVALUE._serialized_end = 13453
-    _VECTORVALUE._serialized_start = 13455
-    _VECTORVALUE._serialized_end = 13490
-    _MATRIXVALUE._serialized_start = 13492
-    _MATRIXVALUE._serialized_end = 13546
+    _POSITION._serialized_end = 3682
+    _POSITIONTRADE._serialized_start = 3684
+    _POSITIONTRADE._serialized_end = 3745
+    _DEPOSIT._serialized_start = 3748
+    _DEPOSIT._serialized_end = 4104
+    _DEPOSIT_STATUS._serialized_start = 4011
+    _DEPOSIT_STATUS._serialized_end = 4104
+    _WITHDRAWAL._serialized_start = 4107
+    _WITHDRAWAL._serialized_end = 4531
+    _WITHDRAWAL_STATUS._serialized_start = 4433
+    _WITHDRAWAL_STATUS._serialized_end = 4525
+    _WITHDRAWEXT._serialized_start = 4533
+    _WITHDRAWEXT._serialized_end = 4601
+    _ERC20WITHDRAWEXT._serialized_start = 4603
+    _ERC20WITHDRAWEXT._serialized_end = 4664
+    _ACCOUNT._serialized_start = 4667
+    _ACCOUNT._serialized_end = 4830
+    _FINANCIALAMOUNT._serialized_start = 4832
+    _FINANCIALAMOUNT._serialized_end = 4895
+    _TRANSFER._serialized_start = 4898
+    _TRANSFER._serialized_end = 5077
+    _DISPATCHSTRATEGY._serialized_start = 5080
+    _DISPATCHSTRATEGY._serialized_end = 5212
+    _TRANSFERREQUEST._serialized_start = 5215
+    _TRANSFERREQUEST._serialized_end = 5445
+    _ACCOUNTDETAILS._serialized_start = 5448
+    _ACCOUNTDETAILS._serialized_end = 5615
+    _LEDGERENTRY._serialized_start = 5618
+    _LEDGERENTRY._serialized_end = 5931
+    _POSTTRANSFERBALANCE._serialized_start = 5933
+    _POSTTRANSFERBALANCE._serialized_end = 6028
+    _LEDGERMOVEMENT._serialized_start = 6030
+    _LEDGERMOVEMENT._serialized_end = 6146
+    _MARGINLEVELS._serialized_start = 6149
+    _MARGINLEVELS._serialized_end = 6450
+    _MARKETDATA._serialized_start = 6453
+    _MARKETDATA._serialized_end = 7834
+    _LIQUIDITYPROVIDERFEESHARE._serialized_start = 7837
+    _LIQUIDITYPROVIDERFEESHARE._serialized_end = 8023
+    _PRICEMONITORINGBOUNDS._serialized_start = 8026
+    _PRICEMONITORINGBOUNDS._serialized_end = 8226
+    _ERRORDETAIL._serialized_start = 8228
+    _ERRORDETAIL._serialized_end = 8309
+    _NETWORKPARAMETER._serialized_start = 8311
+    _NETWORKPARAMETER._serialized_end = 8369
+    _NETWORKLIMITS._serialized_start = 8372
+    _NETWORKLIMITS._serialized_end = 8758
+    _LIQUIDITYORDER._serialized_start = 8760
+    _LIQUIDITYORDER._serialized_end = 8885
+    _LIQUIDITYORDERREFERENCE._serialized_start = 8887
+    _LIQUIDITYORDERREFERENCE._serialized_end = 9002
+    _LIQUIDITYPROVISION._serialized_start = 9005
+    _LIQUIDITYPROVISION._serialized_end = 9599
+    _LIQUIDITYPROVISION_STATUS._serialized_start = 9442
+    _LIQUIDITYPROVISION_STATUS._serialized_end = 9599
+    _ETHEREUMCONFIG._serialized_start = 9602
+    _ETHEREUMCONFIG._serialized_end = 10066
+    _ETHEREUMCONTRACTCONFIG._serialized_start = 10068
+    _ETHEREUMCONTRACTCONFIG._serialized_end = 10174
+    _EPOCHTIMESTAMPS._serialized_start = 10177
+    _EPOCHTIMESTAMPS._serialized_end = 10349
+    _EPOCH._serialized_start = 10352
+    _EPOCH._serialized_end = 10528
+    _EPOCHPARTICIPATION._serialized_start = 10531
+    _EPOCHPARTICIPATION._serialized_end = 10673
+    _EPOCHDATA._serialized_start = 10675
+    _EPOCHDATA._serialized_end = 10758
+    _RANKINGSCORE._serialized_start = 10761
+    _RANKINGSCORE._serialized_end = 11044
+    _REWARDSCORE._serialized_start = 11047
+    _REWARDSCORE._serialized_end = 11346
+    _NODE._serialized_start = 11349
+    _NODE._serialized_end = 12040
+    _NODESET._serialized_start = 12043
+    _NODESET._serialized_end = 12199
+    _NODEDATA._serialized_start = 12202
+    _NODEDATA._serialized_end = 12503
+    _DELEGATION._serialized_start = 12505
+    _DELEGATION._serialized_end = 12617
+    _REWARD._serialized_start = 12620
+    _REWARD._serialized_end = 12871
+    _REWARDSUMMARY._serialized_start = 12873
+    _REWARDSUMMARY._serialized_end = 12966
+    _EPOCHREWARDSUMMARY._serialized_start = 12969
+    _EPOCHREWARDSUMMARY._serialized_end = 13124
+    _STATEVALUEPROPOSAL._serialized_start = 13126
+    _STATEVALUEPROPOSAL._serialized_end = 13247
+    _KEYVALUEBUNDLE._serialized_start = 13249
+    _KEYVALUEBUNDLE._serialized_end = 13356
+    _STATEVARVALUE._serialized_start = 13359
+    _STATEVARVALUE._serialized_end = 13539
+    _SCALARVALUE._serialized_start = 13541
+    _SCALARVALUE._serialized_end = 13576
+    _VECTORVALUE._serialized_start = 13578
+    _VECTORVALUE._serialized_end = 13613
+    _MATRIXVALUE._serialized_start = 13615
+    _MATRIXVALUE._serialized_end = 13669
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-0.67.0/vega_sim/proto/vega/wallet/v1/wallet_pb2.py` & `vega_sim-1.0.1/vega_sim/proto/vega/wallet/v1/wallet_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(
     DESCRIPTOR, "vega.wallet.v1.wallet_pb2", globals()
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = (
         b"Z/code.vegaprotocol.io/vega/protos/vega/wallet/v1"
     )
     _SUBMITTRANSACTIONREQUEST._serialized_start = 153
     _SUBMITTRANSACTIONREQUEST._serialized_end = 2512
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-0.67.0/vega_sim/quant/quant.py` & `vega_sim-1.0.1/vega_sim/quant/quant.py`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/reinforcement/agents/learning_agent.py` & `vega_sim-1.0.1/vega_sim/reinforcement/agents/learning_agent.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,23 +57,22 @@
         self,
         device: str,
         logfile_pol_imp: str,
         logfile_pol_eval: str,
         logfile_pnl: str,
         discount_factor: float,
         num_levels: int,
-        wallet_name: str,
-        wallet_pass: str,
+        key_name: str,
         market_name: str,
         initial_balance: int,
         position_decimals: int,
         asset_name: str,
         inventory_penalty: float = 0.0,
     ):
-        super().__init__(wallet_name=wallet_name, wallet_pass=wallet_pass)
+        super().__init__(key_name=key_name)
 
         self.step_num = 0
         self.latest_state = None
         self.latest_action = None
         self.device = device
         self.discount_factor = discount_factor
         self.initial_balance = initial_balance
@@ -120,15 +119,15 @@
             for m in self.vega.all_markets()
             if m.tradable_instrument.instrument.name == market_name
         ][0]
         # Get asset id
         self.tdai_id = self.vega.find_asset_id(symbol=self.asset_name)
         # Top up asset
         self.vega.mint(
-            self.wallet_name,
+            self.key_name,
             asset=self.tdai_id,
             amount=self.initial_balance,
         )
         self.vega.wait_fn(2)
 
     def _update_memory(
         self,
@@ -160,19 +159,19 @@
     def create_dataloader(self, batch_size):
         """
         creates dataset and dataloader for training.
         """
         pass
 
     def state(self, vega: VegaServiceNull) -> LAMarketState:
-        position = self.vega.positions_by_market(self.wallet_name, self.market_id)
+        position = self.vega.positions_by_market(self.key_name, self.market_id)
 
         position = position.open_volume if position else 0
         account = self.vega.party_account(
-            wallet_name=self.wallet_name,
+            key_name=self.key_name,
             asset_id=self.tdai_id,
             market_id=self.market_id,
         )
         book_state = self.vega.market_depth(
             self.market_id, num_levels=self.num_levels
         )  # make num_levels as a parameter?
 
@@ -220,15 +219,15 @@
         pass
 
     def finalise(self):
         numTries = 3
         account = None
         for i in range(0, numTries):
             account = self.vega.party_account(
-                wallet_name=self.wallet_name,
+                key_name=self.key_name,
                 asset_id=self.tdai_id,
                 market_id=self.market_id,
             )
             self.latest_state = self.state(self.vega)
             if account.margin == 0:
                 break
             self.vega.forward("1s")
```

### Comparing `vega_sim-0.67.0/vega_sim/reinforcement/agents/learning_agent_MO.py` & `vega_sim-1.0.1/vega_sim/reinforcement/agents/learning_agent_MO.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,31 +52,29 @@
         self,
         device: str,
         logfile_pol_imp: str,
         logfile_pol_eval: str,
         logfile_pnl: str,
         discount_factor: float,
         num_levels: int,
-        wallet_name: str,
-        wallet_pass: str,
+        key_name: str,
         market_name: str,
         initial_balance: int,
         position_decimals: int,
         asset_name: str,
         inventory_penalty: float = 1.0,
     ):
         super().__init__(
             device=device,
             logfile_pol_imp=logfile_pol_imp,
             logfile_pol_eval=logfile_pol_eval,
             logfile_pnl=logfile_pnl,
             discount_factor=discount_factor,
             num_levels=num_levels,
-            wallet_name=wallet_name,
-            wallet_pass=wallet_pass,
+            key_name=key_name,
             market_name=market_name,
             initial_balance=initial_balance,
             position_decimals=position_decimals,
             inventory_penalty=inventory_penalty,
             asset_name=asset_name,
         )
         self.volume = 10 ** (-self.position_decimals)
@@ -182,15 +180,15 @@
             return
         if learning_state.market_in_auction:
             return
 
         if self.latest_action.buy or self.latest_action.sell:
             try:
                 self.vega.submit_market_order(
-                    trading_wallet=self.wallet_name,
+                    trading_key=self.key_name,
                     market_id=self.market_id,
                     side="SIDE_BUY" if self.latest_action.buy else "SIDE_SELL",
                     volume=self.volume,
                     wait=False,
                     fill_or_kill=False,
                 )
             except Exception as e:
```

### Comparing `vega_sim-0.67.0/vega_sim/reinforcement/agents/learning_agent_MO_with_vol.py` & `vega_sim-1.0.1/vega_sim/reinforcement/agents/learning_agent_MO_with_vol.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,30 +75,28 @@
         self,
         device: str,
         logfile_pol_imp: str,
         logfile_pol_eval: str,
         logfile_pnl: str,
         discount_factor: float,
         num_levels: int,
-        wallet_name: str,
-        wallet_pass: str,
+        key_name: str,
         market_name: str,
         initial_balance: int,
         position_decimals: int,
         inventory_penalty: float = 0.05,
     ):
         super().__init__(
             device=device,
             logfile_pol_imp=logfile_pol_imp,
             logfile_pol_eval=logfile_pol_eval,
             logfile_pnl=logfile_pnl,
             discount_factor=discount_factor,
             num_levels=num_levels,
-            wallet_name=wallet_name,
-            wallet_pass=wallet_pass,
+            key_name=key_name,
             market_name=market_name,
             initial_balance=initial_balance,
             position_decimals=position_decimals,
             inventory_penalty=inventory_penalty,
         )
 
         # Dimensions of state and action
@@ -222,15 +220,15 @@
             return
         if learning_state.market_in_auction:
             return
 
         if self.latest_action.buy or self.latest_action.sell:
             try:
                 self.vega.submit_market_order(
-                    trading_wallet=self.wallet_name,
+                    trading_key=self.key_name,
                     market_id=self.market_id,
                     side="SIDE_BUY" if self.latest_action.buy else "SIDE_SELL",
                     volume=self.latest_action.volume,
                     wait=False,
                     fill_or_kill=False,
                 )
             except Exception as e:
```

### Comparing `vega_sim-0.67.0/vega_sim/reinforcement/agents/learning_agent_heuristic.py` & `vega_sim-1.0.1/vega_sim/reinforcement/agents/learning_agent_heuristic.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,30 +60,28 @@
         self,
         device: str,
         logfile_pol_imp: str,
         logfile_pol_eval: str,
         logfile_pnl: str,
         discount_factor: float,
         num_levels: int,
-        wallet_name: str,
-        wallet_pass: str,
+        key_name: str,
         market_name: str,
         initial_balance: int,
         position_decimals: int,
         inventory_penalty: float = 1.0,
     ):
         super().__init__(
             device=device,
             logfile_pol_imp=logfile_pol_imp,
             logfile_pol_eval=logfile_pol_eval,
             logfile_pnl=logfile_pnl,
             discount_factor=discount_factor,
             num_levels=num_levels,
-            wallet_name=wallet_name,
-            wallet_pass=wallet_pass,
+            key_name=key_name,
             market_name=market_name,
             initial_balance=initial_balance,
             position_decimals=position_decimals,
             inventory_penalty=inventory_penalty,
         )
         self.volume = 10 ** (-self.position_decimals)
 
@@ -185,15 +183,15 @@
             return
         if learning_state.market_in_auction:
             return
 
         if self.latest_action.buy or self.latest_action.sell:
             try:
                 self.vega.submit_market_order(
-                    trading_wallet=self.wallet_name,
+                    trading_key=self.key_name,
                     market_id=self.market_id,
                     side="SIDE_BUY" if self.latest_action.buy else "SIDE_SELL",
                     volume=self.volume,
                     wait=False,
                     fill_or_kill=False,
                 )
             except Exception as e:
```

### Comparing `vega_sim-0.67.0/vega_sim/reinforcement/agents/simple_agent.py` & `vega_sim-1.0.1/vega_sim/reinforcement/agents/simple_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
         self.market_name = market_name
         self.asset_name = asset_name
         self.initial_balance = initial_balance
 
     def initialise(self, vega: VegaService):
         # Initialise wallet
-        super().initialise(vega=vega, create_wallet=True)
+        super().initialise(vega=vega, create_key=True)
 
         # Get market id
         self.market_id = self.vega.find_market_id(name=self.market_name)
 
         # Get asset id
         self.asset_id = self.vega.find_asset_id(symbol=self.asset_name)
         # Top up asset
```

### Comparing `vega_sim-0.67.0/vega_sim/reinforcement/distributions.py` & `vega_sim-1.0.1/vega_sim/reinforcement/distributions.py`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/reinforcement/full_market_sim/environments.py` & `vega_sim-1.0.1/vega_sim/reinforcement/full_market_sim/environments.py`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/reinforcement/full_market_sim/utils/create_csv.py` & `vega_sim-1.0.1/vega_sim/reinforcement/full_market_sim/utils/create_csv.py`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/reinforcement/full_market_sim/utils/external_assetprice.py` & `vega_sim-1.0.1/vega_sim/reinforcement/full_market_sim/utils/external_assetprice.py`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/reinforcement/full_market_sim/utils/logdata.py` & `vega_sim-1.0.1/vega_sim/reinforcement/full_market_sim/utils/logdata.py`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/reinforcement/full_market_sim/utils/strategy.py` & `vega_sim-1.0.1/vega_sim/reinforcement/full_market_sim/utils/strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     q_upper: int,
     q_lower: int,
     kappa: int,
     lmbda: int,
     alpha: float,
     phi: float,
 ):
-
     """
     Simulate an Market Making Model and output the optimal strategy
       of posting bid/ask depth based on market parameters.
 
     Args:
         T:
             int, total simulation time
```

### Comparing `vega_sim-0.67.0/vega_sim/reinforcement/helpers.py` & `vega_sim-1.0.1/vega_sim/reinforcement/helpers.py`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/reinforcement/la_market_state.py` & `vega_sim-1.0.1/vega_sim/reinforcement/la_market_state.py`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/reinforcement/networks.py` & `vega_sim-1.0.1/vega_sim/reinforcement/networks.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,14 @@
 class FFN_Params_Normal(nn.Module):
     def __init__(
         self,
         n_in: int,
         n_distr: int,
         hidden_sizes: List[int],
     ):
-
         super().__init__()
         self.net = FFN(
             sizes=[n_in] + hidden_sizes, activation=nn.Tanh, output_activation=nn.Tanh
         )
         self.net_mu = nn.Linear(hidden_sizes[-1], n_distr)
         self.net_sigma = nn.Sequential(
             nn.Linear(hidden_sizes[-1], n_distr), nn.Softplus()
```

### Comparing `vega_sim-0.67.0/vega_sim/reinforcement/plot.py` & `vega_sim-1.0.1/vega_sim/reinforcement/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,14 @@
     ax4.plot(reward.cumsum(), label="cumulative reward")
     ax4.legend()
     fig.savefig(os.path.join(results_dir, "sim{}.pdf".format(tag)))
     plt.close()
 
 
 def plot_learning(results_dir: str, logfile_pol_imp: str, logfile_pol_eval: str):
-
     data = pd.read_csv(logfile_pol_imp)
     plt.figure()
     plt.plot(data["iteration"], data["loss"])
     plt.ylabel("KL(policy|e^Q)")
     plt.xlabel("Iteration")
     plt.title("Policy improvement")
```

### Comparing `vega_sim-0.67.0/vega_sim/reinforcement/run_rl_agent.py` & `vega_sim-1.0.1/vega_sim/reinforcement/run_rl_agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import argparse
 import logging
 import os
 from logging import getLogger
 
 import torch
+
 from vega_sim.null_service import VegaServiceNull
 from vega_sim.reinforcement.agents.learning_agent import WALLET as LEARNING_WALLET
 from vega_sim.reinforcement.agents.learning_agent import LearningAgent, state_fn
 from vega_sim.reinforcement.agents.learning_agent_heuristic import (
     LearningAgentHeuristic,
 )
 from vega_sim.reinforcement.agents.learning_agent_MO import LearningAgentFixedVol
 from vega_sim.reinforcement.agents.learning_agent_MO_with_vol import (
     LearningAgentWithVol,
 )
 from vega_sim.reinforcement.helpers import set_seed
 from vega_sim.reinforcement.plot import plot_learning, plot_pnl, plot_simulation
-from vega_sim.scenario.registry import CurveMarketMaker
 from vega_sim.scenario.common.agents import Snitch
+from vega_sim.scenario.registry import CurveMarketMaker
 
 logger = getLogger(__name__)
 
 
 def run_iteration(
     learning_agent: LearningAgent,
     step_tag: int,
@@ -54,16 +55,19 @@
         vega=vega, tag=str(step_tag), random_state=None
     )
     # add the learning agaent to the environment's list of agents
     learning_agent.set_market_tag(str(step_tag))
     learning_agent.price_process = scenario.price_process
     scenario.agents["learner"] = learning_agent
 
+    # Disabling Snitch for now to speed up training
     scenario.agents["snitch"] = Snitch(
-        agents=scenario.agents, additional_state_fn=scenario.state_extraction_fn
+        agents=scenario.agents,
+        additional_state_fn=scenario.state_extraction_fn,
+        only_extract_additional=True,
     )
 
     scenario.env = scenario.configure_environment(
         vega=vega,
         tag=str(step_tag),
     )
 
@@ -83,14 +87,15 @@
 def _run(
     max_iterations: int,
     results_dir: str = "numerical_results",
     resume_training: bool = False,
     evaluate_only: bool = False,
     plot_every_step: bool = False,
     device: str = "cpu",
+    recreate_vega_every_n_iterations: int = 100,
 ):
     # set seed for results replication
     set_seed(1)
 
     # set market name
     market_name = "ETH:USD"
     asset_name = "tDAI"
@@ -107,82 +112,95 @@
     learning_agent = LearningAgentFixedVol(
         device=device,
         logfile_pol_imp=logfile_pol_imp,
         logfile_pol_eval=logfile_pol_eval,
         logfile_pnl=logfile_pnl,
         discount_factor=0.8,
         num_levels=1,
-        wallet_name=LEARNING_WALLET.name,
-        wallet_pass=LEARNING_WALLET.passphrase,
+        key_name=LEARNING_WALLET.name,
         initial_balance=100000,
         market_name=market_name,
         position_decimals=position_decimals,
         inventory_penalty=0.1,
         asset_name=asset_name,
     )
 
-    with VegaServiceNull(
-        warn_on_raw_data_access=False,
-        run_with_console=False,
-        retain_log_files=True,
-        store_transactions=True,
-    ) as vega:
-        vega.wait_for_total_catchup()
-
-        if not evaluate_only:
-            logger.info(f"Running training for {max_iterations} iterations")
-            # TRAINING OF AGENT
-            if resume_training:
-                logger.info("Loading neural net weights from: " + results_dir)
-                learning_agent.load(results_dir)
-            else:
-                with open(logfile_pol_imp, "w") as f:
-                    f.write("iteration,loss\n")
-                with open(logfile_pol_eval, "w") as f:
-                    f.write("iteration,loss,kl_coeff_disc,kl_coeff_cont\n")
-                with open(logfile_pnl, "w") as f:
-                    f.write("iteration,pnl\n")
-
-            for it in range(max_iterations):
-                # simulation of market to get some data
-
-                learning_agent.move_to_cpu()
-                _ = run_iteration(
-                    learning_agent=learning_agent,
-                    step_tag=it,
-                    vega=vega,
-                    market_name=market_name,
-                    asset_name=asset_name,
-                    run_with_console=False,
-                    pause_at_completion=False,
-                )
-
-                # Policy evaluation + Policy improvement
-                learning_agent.move_to_device()
-                learning_agent.policy_eval(batch_size=20000, n_epochs=10)
-                learning_agent.policy_improvement(batch_size=100_000, n_epochs=10)
-
-                # save in case environment chooses to crash
-                learning_agent.save(results_dir)
-
-                if plot_every_step:
-                    plot_learning(
-                        results_dir=results_dir,
-                        logfile_pol_eval=logfile_pol_eval,
-                        logfile_pol_imp=logfile_pol_imp,
-                    )
-
+    if not evaluate_only:
+        logger.info(f"Running training for {max_iterations} iterations")
+        # TRAINING OF AGENT
+        if resume_training:
+            logger.info("Loading neural net weights from: " + results_dir)
+            learning_agent.load(results_dir)
         else:
-            # EVALUATION OF AGENT
-            logger.info("Loading neural net weights from: " + args.results_dir)
-            learning_agent.load(args.results_dir)
-            learning_agent.lerningIteration = 0
+            with open(logfile_pol_imp, "w") as f:
+                f.write("iteration,loss\n")
+            with open(logfile_pol_eval, "w") as f:
+                f.write("iteration,loss,kl_coeff_disc,kl_coeff_cont\n")
             with open(logfile_pnl, "w") as f:
                 f.write("iteration,pnl\n")
 
+        it = 0
+        while it <= max_iterations:
+            with VegaServiceNull(
+                warn_on_raw_data_access=False,
+                run_with_console=False,
+                retain_log_files=True,
+                store_transactions=True,
+            ) as vega:
+                for _ in range(recreate_vega_every_n_iterations):
+                    it += 1
+                    if it > max_iterations:
+                        break
+
+                    logger.info(f"Running iteration {it}")
+                    # simulation of market to get some data
+
+                    learning_agent.move_to_cpu()
+
+                    _ = run_iteration(
+                        learning_agent=learning_agent,
+                        step_tag=it,
+                        vega=vega,
+                        market_name=market_name,
+                        asset_name=asset_name,
+                        run_with_console=False,
+                        pause_at_completion=False,
+                    )
+
+                    # Policy evaluation + Policy improvement
+                    learning_agent.move_to_device()
+                    learning_agent.policy_eval(batch_size=20000, n_epochs=10)
+                    learning_agent.policy_improvement(batch_size=100_000, n_epochs=10)
+
+                    # save in case environment chooses to crash
+                    learning_agent.save(results_dir)
+
+                    if plot_every_step:
+                        plot_learning(
+                            results_dir=results_dir,
+                            logfile_pol_eval=logfile_pol_eval,
+                            logfile_pol_imp=logfile_pol_imp,
+                        )
+                if it >= max_iterations:
+                    logger.info("Recreating Vega instance to tidy up")
+
+    else:
+        # EVALUATION OF AGENT
+        logger.info("Loading neural net weights from: " + args.results_dir)
+        learning_agent.load(args.results_dir)
+        learning_agent.lerningIteration = 0
+        with open(logfile_pnl, "w") as f:
+            f.write("iteration,pnl\n")
+
+        with VegaServiceNull(
+            warn_on_raw_data_access=False,
+            run_with_console=False,
+            retain_log_files=True,
+            store_transactions=True,
+        ) as vega:
             for it in range(args.evaluate):
                 learning_agent.clear_memory()
                 learning_agent.exploitation = 1.0
 
                 result = run_iteration(
                     learning_agent=learning_agent,
                     step_tag=it,
@@ -257,8 +275,9 @@
     _run(
         max_iterations=args.rl_max_it,
         results_dir=args.results_dir,
         resume_training=args.resume_training,
         evaluate_only=args.evaluate,
         plot_every_step=args.plot_every_step,
         device=device,
+        recreate_vega_every_n_iterations=1000,
     )
```

### Comparing `vega_sim-0.67.0/vega_sim/reinforcement/run_simple_agent.py` & `vega_sim-1.0.1/vega_sim/reinforcement/run_simple_agent.py`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/reinforcement/theory_intro/RL.tex` & `vega_sim-1.0.1/vega_sim/reinforcement/theory_intro/RL.tex`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/reinforcement/theory_intro/images/RL.png` & `vega_sim-1.0.1/vega_sim/reinforcement/theory_intro/images/RL.png`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/reinforcement/theory_intro/images/RL_inv.png` & `vega_sim-1.0.1/vega_sim/reinforcement/theory_intro/images/RL_inv.png`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/reinforcement/theory_intro/images/logo.png` & `vega_sim-1.0.1/vega_sim/reinforcement/theory_intro/images/logo.png`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/reinforcement/theory_intro/images/logo_inv.png` & `vega_sim-1.0.1/vega_sim/reinforcement/theory_intro/images/logo_inv.png`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/replay/replay.py` & `vega_sim-1.0.1/vega_sim/replay/replay.py`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/scenario/adhoc.py` & `vega_sim-1.0.1/vega_sim/scenario/adhoc.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from vega_sim.scenario.constants import Network
 
 from vega_sim.null_service import VegaServiceNull
 from vega_sim.network_service import VegaServiceNetwork
 from vega_sim.scenario.registry import SCENARIOS
 from vega_sim.scenario.scenario import Scenario
-from vega_sim.service import VegaService
 
 
 def main():
     parser = argparse.ArgumentParser()
 
     parser.add_argument("-s", "--scenario")
     parser.add_argument("--console", action="store_true")
@@ -48,29 +47,27 @@
             transactions_per_block=(
                 scenario.transactions_per_block
                 if hasattr(scenario, "transactions_per_block")
                 else 100
             ),
             retain_log_files=True,
             use_full_vega_wallet=False,
-            start_live_feeds=True,
         ) as vega:
             scenario.run_iteration(
                 vega=vega,
                 network=Network[args.network],
                 pause_at_completion=args.pause,
                 output_data=args.output,
             )
 
     else:
         with VegaServiceNetwork(
             network=Network[args.network],
             run_with_wallet=True,
             run_with_console=True,
-            start_live_feeds=False,
         ) as vega:
             scenario.run_iteration(
                 vega=vega,
                 network=Network[args.network],
             )
```

### Comparing `vega_sim-0.67.0/vega_sim/scenario/common/agents.py` & `vega_sim-1.0.1/vega_sim/scenario/common/agents.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from __future__ import annotations
-from dataclasses import dataclass
-
 
-import logging
 import datetime
-
+import logging
+from dataclasses import dataclass
+from math import exp
 from queue import Queue
+
 import numpy as np
-from math import exp
 
 try:
     import talib
 except ImportError:
     pass  # TA-Lib not installed, but most agents don't need
 
-from enum import Enum
+import time
 from collections import namedtuple
-from typing import Callable, Iterable, List, Optional, Tuple, Union, Dict, Any
+from enum import Enum
+from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Union
+
 from numpy.typing import ArrayLike
-from vega_sim.api.data import Order, AccountData, MarketDepth, Trade
 
+import vega_sim.api.faucet as faucet
+from vega_sim.api.data import AccountData, MarketDepth, Order, Trade
+from vega_sim.api.trading import OrderRejectedError
 from vega_sim.environment import VegaState
-from vega_sim.environment.agent import StateAgentWithWallet, StateAgent, Agent
-from vega_sim.null_service import VegaServiceNull, VegaService
+from vega_sim.environment.agent import Agent, StateAgent, StateAgentWithWallet
 from vega_sim.network_service import VegaServiceNetwork
-from vega_sim.proto.vega import (
-    markets as markets_protos,
-    vega as vega_protos,
-)
+from vega_sim.null_service import VegaService, VegaServiceNull
+from vega_sim.proto.vega import markets as markets_protos
+from vega_sim.proto.vega import vega as vega_protos
 from vega_sim.scenario.common.utils.ideal_mm_models import GLFT_approx, a_s_mm_model
-from vega_sim.api.trading import OrderRejectedError
 
 WalletConfig = namedtuple("WalletConfig", ["name", "passphrase"])
 
 
 @dataclass
 class MarketHistoryData:
     at_time: datetime.datetime
@@ -82,61 +82,58 @@
 
 
 class MarketOrderTrader(StateAgentWithWallet):
     NAME_BASE = "mo_trader"
 
     def __init__(
         self,
-        wallet_name: str,
-        wallet_pass: str,
+        key_name: str,
         market_name: str,
         asset_name: str,
         initial_asset_mint: float = 1000000,
         buy_intensity: float = 1,
         sell_intensity: float = 1,
         tag: str = "",
         random_state: Optional[np.random.RandomState] = None,
         base_order_size: float = 1,
-        key_name: Optional[str] = None,
+        wallet_name: Optional[str] = None,
         step_bias: Optional[float] = 1,
     ):
-        super().__init__(
-            wallet_name=wallet_name, wallet_pass=wallet_pass, key_name=key_name, tag=tag
-        )
+        super().__init__(wallet_name=wallet_name, key_name=key_name, tag=tag)
         self.initial_asset_mint = initial_asset_mint
         self.buy_intensity = buy_intensity
         self.sell_intensity = sell_intensity
         self.market_name = market_name
         self.asset_name = asset_name
         self.random_state = (
             random_state if random_state is not None else np.random.RandomState()
         )
         self.base_order_size = base_order_size
         self.step_bias = step_bias
 
     def initialise(
         self,
         vega: Union[VegaServiceNull, VegaServiceNetwork],
-        create_wallet: bool = True,
-        mint_wallet: bool = True,
+        create_key: bool = True,
+        mint_key: bool = True,
     ):
-        # Initialise wallet
-        super().initialise(vega=vega, create_wallet=create_wallet)
+        # Initialise key
+        super().initialise(vega=vega, create_key=create_key)
         # Get market id
         self.market_id = self.vega.find_market_id(name=self.market_name)
 
         # Get asset id
         self.asset_id = self.vega.find_asset_id(symbol=self.asset_name)
-        if mint_wallet:
+        if mint_key:
             # Top up asset
             self.vega.mint(
-                self.wallet_name,
+                key_name=self.key_name,
                 asset=self.asset_id,
                 amount=self.initial_asset_mint,
-                key_name=self.key_name,
+                wallet_name=self.wallet_name,
             )
         self.vega.wait_fn(5)
         self.pdp = self.vega.market_pos_decimals.get(self.market_id, {})
         self.mdp = self.vega.market_price_decimals.get(self.market_id, {})
         self.adp = self.vega.asset_decimals.get(self.asset_id, {})
 
     def step(self, vega_state: VegaState):
@@ -174,46 +171,43 @@
                 == markets_protos.Market.TradingMode.TRADING_MODE_CONTINUOUS
             )
             and vega_state.market_state[self.market_id].state
             == markets_protos.Market.State.STATE_ACTIVE
             and volume != 0
         ):
             self.vega.submit_market_order(
-                trading_wallet=self.wallet_name,
+                trading_key=self.key_name,
                 market_id=self.market_id,
                 side=side,
                 volume=volume,
                 wait=False,
                 fill_or_kill=False,
-                key_name=self.key_name,
+                trading_wallet=self.wallet_name,
             )
 
 
 class PriceSensitiveMarketOrderTrader(StateAgentWithWallet):
     NAME_BASE = "price_sensitive_mo_trader"
 
     def __init__(
         self,
-        wallet_name: str,
-        wallet_pass: str,
+        key_name: str,
         market_name: str,
         asset_name: str,
         price_process_generator: Iterable[float],
         initial_asset_mint: float = 1000000,
         buy_intensity: float = 1,
         sell_intensity: float = 1,
         price_half_life: float = 1,
         tag: str = "",
         random_state: Optional[np.random.RandomState] = None,
         base_order_size: float = 1,
-        key_name: str = None,
+        wallet_name: str = None,
     ):
-        super().__init__(
-            wallet_name=wallet_name, wallet_pass=wallet_pass, key_name=key_name, tag=tag
-        )
+        super().__init__(wallet_name=wallet_name, key_name=key_name, tag=tag)
         self.initial_asset_mint = initial_asset_mint
         self.buy_intensity = buy_intensity
         self.sell_intensity = sell_intensity
         self.market_name = market_name
         self.asset_name = asset_name
         self.random_state = (
             random_state if random_state is not None else np.random.RandomState()
@@ -221,31 +215,31 @@
         self.base_order_size = base_order_size
         self.probability_decay = np.log(2) / price_half_life
         self.price_process_generator = price_process_generator
 
     def initialise(
         self,
         vega: Union[VegaServiceNull, VegaServiceNetwork],
-        create_wallet: bool = True,
-        mint_wallet: bool = True,
+        create_key: bool = True,
+        mint_key: bool = True,
     ):
         # Initialise wallet
-        super().initialise(vega=vega, create_wallet=create_wallet)
+        super().initialise(vega=vega, create_key=create_key)
         # Get market id
         self.market_id = self.vega.find_market_id(name=self.market_name)
 
         # Get asset id
         self.asset_id = self.vega.find_asset_id(symbol=self.asset_name)
-        if mint_wallet:
+        if mint_key:
             # Top up asset
             self.vega.mint(
-                self.wallet_name,
+                key_name=self.key_name,
                 asset=self.asset_id,
                 amount=self.initial_asset_mint,
-                key_name=self.key_name,
+                wallet_name=self.wallet_name,
             )
         self.vega.wait_fn(5)
 
     def step(self, vega_state: VegaState):
         self.curr_price = next(self.price_process_generator)
 
         buy_first = self.random_state.choice([0, 1])
@@ -290,74 +284,71 @@
                 == markets_protos.Market.TradingMode.TRADING_MODE_CONTINUOUS
             )
             and vega_state.market_state[self.market_id].state
             == markets_protos.Market.State.STATE_ACTIVE
             and volume != 0
         ):
             self.vega.submit_market_order(
-                trading_wallet=self.wallet_name,
+                trading_key=self.key_name,
                 market_id=self.market_id,
                 side=side,
                 volume=volume,
                 wait=False,
                 fill_or_kill=False,
-                key_name=self.key_name,
+                trading_wallet=self.wallet_name,
             )
 
 
 class PriceSensitiveLimitOrderTrader(StateAgentWithWallet):
     NAME_BASE = "price_sensitive_lo_trader"
 
     def __init__(
         self,
-        wallet_name: str,
-        wallet_pass: str,
+        key_name: str,
         market_name: str,
         asset_name: str,
         price_process_generator: Iterable[float],
         initial_asset_mint: float = 1000000,
         scale: float = 0.5,
         max_order_size: float = 100,
         random_state: Optional[np.random.RandomState] = None,
-        key_name: str = None,
+        wallet_name: str = None,
         tag: str = "",
     ):
-        super().__init__(
-            wallet_name=wallet_name, wallet_pass=wallet_pass, key_name=key_name, tag=tag
-        )
+        super().__init__(wallet_name=wallet_name, key_name=key_name, tag=tag)
         self.market_name = market_name
         self.asset_name = asset_name
         self.price_process_generator = price_process_generator
         self.initial_asset_mint = initial_asset_mint
         self.scale = scale
         self.max_order_size = max_order_size
         self.random_state = (
             random_state if random_state is not None else np.random.RandomState()
         )
 
     def initialise(
         self,
         vega: Union[VegaServiceNull, VegaServiceNetwork],
-        create_wallet: bool = True,
-        mint_wallet: bool = True,
+        create_key: bool = True,
+        mint_key: bool = True,
     ):
         # Initialise wallet
-        super().initialise(vega=vega, create_wallet=create_wallet)
+        super().initialise(vega=vega, create_key=create_key)
         # Get market id
         self.market_id = self.vega.find_market_id(name=self.market_name)
 
         # Get asset id
         self.asset_id = self.vega.find_asset_id(symbol=self.asset_name)
-        if mint_wallet:
+        if mint_key:
             # Top up asset
             self.vega.mint(
-                self.wallet_name,
+                key_name=self.key_name,
                 asset=self.asset_id,
                 amount=self.initial_asset_mint,
-                key_name=self.key_name,
+                wallet_name=self.wallet_name,
             )
         self.vega.wait_fn(5)
 
     def step(self, vega_state: VegaState):
         self.curr_price = next(self.price_process_generator)
 
         bid_price = self.curr_price + self.random_state.exponential(scale=self.scale)
@@ -368,16 +359,16 @@
 
     def place_order(
         self,
         side,
         price,
     ):
         self.vega.submit_order(
+            trading_key=self.key_name,
             trading_wallet=self.wallet_name,
-            key_name=self.key_name,
             market_id=self.market_id,
             order_type="TYPE_LIMIT",
             time_in_force="TIME_IN_FORCE_IOC",
             side=side,
             volume=self.max_order_size,
             price=price,
             wait=False,
@@ -385,32 +376,29 @@
 
 
 class BackgroundMarket(StateAgentWithWallet):
     NAME_BASE = "background_market"
 
     def __init__(
         self,
-        wallet_name: str,
-        wallet_pass: str,
+        key_name: str,
         market_name: str,
         asset_name: str,
         price_process: List[float],
         initial_asset_mint: float = 1000000,
         position_decimals: int = 4,
         spread: float = 0.02,
         tick_spacing: float = 0.01,
         num_levels_per_side: int = 20,
         base_volume_size: float = 0.1,
         order_distribution_kappa: float = 1,
         tag: str = "",
-        key_name: Optional[str] = None,
+        wallet_name: Optional[str] = None,
     ):
-        super().__init__(
-            wallet_name=wallet_name, wallet_pass=wallet_pass, key_name=key_name, tag=tag
-        )
+        super().__init__(wallet_name=wallet_name, key_name=key_name, tag=tag)
         self.price_process = price_process
         self.initial_asset_mint = initial_asset_mint
         self.spread = spread
         self.current_step = 0
         self.tick_spacing = tick_spacing
         self.num_levels_per_side = num_levels_per_side
         self.base_volume_size = base_volume_size
@@ -419,28 +407,28 @@
         self.asset_name = asset_name
         self.kappa = order_distribution_kappa
         self.position_decimals = position_decimals
 
     def initialise(
         self,
         vega: Union[VegaServiceNull, VegaServiceNetwork],
-        create_wallet: bool = True,
-        mint_wallet: bool = True,
+        create_key: bool = True,
+        mint_key: bool = True,
     ):
         # Initialise wallet
-        super().initialise(vega=vega, create_wallet=create_wallet)
+        super().initialise(vega=vega, create_key=create_key)
         # Get market id
         self.market_id = self.vega.find_market_id(name=self.market_name)
 
         # Get asset id
         asset_id = self.vega.find_asset_id(symbol=self.asset_name)
-        if mint_wallet:
+        if mint_key:
             # Top up asset
             self.vega.mint(
-                self.wallet_name,
+                wallet_name=self.wallet_name,
                 asset=asset_id,
                 amount=self.initial_asset_mint,
                 key_name=self.key_name,
             )
         self.vega.wait_fn(2)
 
         initial_price = self.price_process[self.current_step]
@@ -467,14 +455,15 @@
     def _submit_order(
         self, side: Union[str, vega_protos.Side], price: float, size: float
     ) -> None:
         volume = round(size, self.position_decimals)
         if volume == 0:
             return
         self.vega.submit_order(
+            trading_key=self.key_name,
             trading_wallet=self.wallet_name,
             market_id=self.market_id,
             order_type="TYPE_LIMIT",
             time_in_force="TIME_IN_FORCE_GTC",
             side=side,
             volume=volume,
             price=price,
@@ -501,15 +490,15 @@
 
         return np.c_[level_price, level_vol]
 
     def step(self, vega_state: VegaState):
         self.current_step += 1
 
         orders = self.vega.orders_for_party_from_feed(
-            self.wallet_name, self.market_id, live_only=True
+            self.key_name, self.market_id, live_only=True, wallet_name=self.wallet_name
         )
         new_price = self.price_process[self.current_step]
         new_buy_shape = self._calculate_price_volume_levels(
             new_price - self.spread / 2,
             new_price,
             side=vega_protos.SIDE_BUY,
         )
@@ -562,67 +551,63 @@
         orders: List[Order],
         new_shape: List[List[float, float]],
     ) -> None:
         for i in range(num_levels):
             if i < len(orders):
                 order_to_amend = orders[i]
                 self.vega.amend_order(
-                    trading_wallet=self.wallet_name,
+                    trading_key=self.key_name,
+                    wallet_name=self.wallet_name,
                     market_id=self.market_id,
                     order_id=order_to_amend.id,
                     price=new_shape[i][0],
                     volume_delta=new_shape[i][1] - order_to_amend.remaining,
                 )
             else:
                 self._submit_order(side, new_shape[i][0], new_shape[i][1])
 
 
 class MultiRegimeBackgroundMarket(StateAgentWithWallet):
     NAME_BASE = "multi_regime_background_market"
 
     def __init__(
         self,
-        wallet_name: str,
-        wallet_pass: str,
+        key_name: str,
         market_name: str,
         asset_name: str,
         price_process: List[float],
         market_regimes: List[MarketRegime],
         tag: str = "",
-        key_name: Optional[str] = None,
+        wallet_name: Optional[str] = None,
     ):
         """Generate a background market acting differently as time passes.
         Allows specification of varying numbers of non-overlapping regimes
         (with optional gaps in which no orders will be placed).
 
         Places an exponentially shaped Limit-Order-Book about a moving midprice.
 
         Args:
-            wallet_name:
-                str, The name of the wallet to use placing background orders
-            wallet_pass:
-                str, The password to use for the background order wallet
+            key_name:
+                str, The name of the key in the wallet to use
             market_name:
                 str, The name of the market on which the agent will trade
             asset_name:
                 str, The name of the asset to trade with
             price_process:
                 List[float], A list of prices which the market will follow.
             market_regimes:
                 List[MarketRegime], A list of specifications for market
                     regimes, allowing variation over time. Each specifies
                     a start/end date and are interpreted as a sparse set
             tag:
                 str, a tag which will be added to the wallet name
-            key_name:
-                str, optional, The name of the key in the wallet to use
+            wallet_name:
+                str, optional, The name of the wallet to use placing background orders
         """
-        super().__init__(
-            wallet_name=wallet_name, wallet_pass=wallet_pass, key_name=key_name, tag=tag
-        )
+        super().__init__(wallet_name=wallet_name, key_name=key_name, tag=tag)
         self.price_process = price_process
         self.current_step = 0
 
         self.market_name = market_name
         self.asset_name = asset_name
 
         self.market_regimes = self._market_regime_sparse_to_dense(
@@ -648,42 +633,43 @@
                     raise Exception(
                         "Overlapping regimes detected. {} starts before {} ends".format(
                             next_market_regime, market_regime
                         )
                     )
                 else:
                     market_regime = next_market_regime
-
-                regimes.append(
-                    market_regime
-                ) if market_regime.from_timepoint <= i else regimes.append(None)
+                (
+                    regimes.append(market_regime)
+                    if market_regime.from_timepoint <= i
+                    else regimes.append(None)
+                )
             else:
                 regimes.append(market_regime)
         return regimes
 
     def initialise(
         self,
         vega: Union[VegaServiceNull, VegaServiceNetwork],
-        create_wallet: bool = True,
-        mint_wallet: bool = True,
+        create_key: bool = True,
+        mint_key: bool = True,
     ):
         # Initialise wallet
-        super().initialise(vega=vega, create_wallet=create_wallet)
+        super().initialise(vega=vega, create_key=create_key)
         # Get market id
         self.market_id = self.vega.find_market_id(name=self.market_name)
 
         # Get asset id
         asset_id = self.vega.find_asset_id(symbol=self.asset_name)
-        if mint_wallet:
+        if mint_key:
             # Top up asset
             self.vega.mint(
-                self.wallet_name,
+                key_name=self.key_name,
                 asset=asset_id,
                 amount=200000,
-                key_name=self.key_name,
+                wallet_name=self.wallet_name,
             )
         self.vega.wait_fn(2)
 
         market_regime = self.market_regimes[0]
         initial_price = self.price_process[self.current_step]
 
         buy_shape = self._calculate_price_volume_levels(
@@ -711,14 +697,15 @@
             if price > 0:
                 self._submit_order(vega_protos.SIDE_SELL, price, size)
 
     def _submit_order(
         self, side: Union[str, vega_protos.Side], price: float, size: float
     ) -> None:
         self.vega.submit_order(
+            trading_key=self.key_name,
             trading_wallet=self.wallet_name,
             market_id=self.market_id,
             order_type="TYPE_LIMIT",
             time_in_force="TIME_IN_FORCE_GTC",
             side=side,
             volume=round(size, 4),
             price=price,
@@ -750,20 +737,25 @@
         return np.c_[level_price, level_vol]
 
     def step(self, vega_state: VegaState):
         self.current_step += 1
         market_regime = self.market_regimes[self.current_step]
 
         orders = self.vega.orders_for_party_from_feed(
-            self.wallet_name, self.market_id, live_only=True
+            self.key_name, self.market_id, live_only=True, wallet_name=self.wallet_name
         )
 
         if market_regime is None:
             for order in orders.values():
-                self.vega.cancel_order(self.wallet_name, self.market_id, order.id)
+                self.vega.cancel_order(
+                    self.key_name,
+                    self.market_id,
+                    order.id,
+                    wallet_name=self.wallet_name,
+                )
         else:
             new_price = self.price_process[self.current_step]
             new_buy_shape = self._calculate_price_volume_levels(
                 new_price - market_regime.spread,
                 new_price,
                 side=vega_protos.SIDE_BUY,
                 kappa=market_regime.order_distribution_buy_kappa,
@@ -822,15 +814,16 @@
         orders: List[Order],
         new_shape: List[List[float, float]],
     ) -> None:
         for i in range(num_levels):
             if i < len(orders):
                 order_to_amend = orders[i]
                 self.vega.amend_order(
-                    trading_wallet=self.wallet_name,
+                    wallet_name=self.wallet_name,
+                    trading_key=self.key_name,
                     market_id=self.market_id,
                     order_id=order_to_amend.id,
                     price=new_shape[i][0],
                     volume_delta=new_shape[i][1] - order_to_amend.remaining,
                 )
             else:
                 self._submit_order(
@@ -841,53 +834,50 @@
 
 
 class OpenAuctionPass(StateAgentWithWallet):
     NAME_BASE = "open_auction_pass"
 
     def __init__(
         self,
-        wallet_name: str,
-        wallet_pass: str,
+        key_name: str,
         side: str,
         market_name: str,
         asset_name: str,
         initial_asset_mint: float = 1000000,
         initial_price: float = 0.3,
         opening_auction_trade_amount: float = 1,
         tag: str = "",
-        key_name: str = None,
+        wallet_name: str = None,
     ):
-        super().__init__(
-            wallet_name=wallet_name, wallet_pass=wallet_pass, key_name=key_name, tag=tag
-        )
+        super().__init__(wallet_name=wallet_name, key_name=key_name, tag=tag)
         self.side = side
         self.initial_asset_mint = initial_asset_mint
         self.initial_price = initial_price
         self.market_name = market_name
         self.asset_name = asset_name
         self.opening_auction_trade_amount = opening_auction_trade_amount
 
     def initialise(
         self,
         vega: Union[VegaServiceNull, VegaServiceNetwork],
-        create_wallet: bool = True,
-        mint_wallet: bool = True,
+        create_key: bool = True,
+        mint_key: bool = True,
     ):
         # Initialise wallet
-        super().initialise(vega=vega, create_wallet=create_wallet)
+        super().initialise(vega=vega, create_key=create_key)
         # Get market id
         self.market_id = self.vega.find_market_id(name=self.market_name)
 
         self.vega.wait_for_total_catchup()
         # Get asset id
         asset_id = self.vega.find_asset_id(symbol=self.asset_name)
-        if mint_wallet:
+        if mint_key:
             # Top up asset
             self.vega.mint(
-                self.wallet_name,
+                wallet_name=self.wallet_name,
                 asset=asset_id,
                 amount=self.initial_asset_mint,
                 key_name=self.key_name,
             )
         self.vega.wait_fn(10)
         self.vega.wait_for_total_catchup()
 
@@ -896,47 +886,42 @@
             market_id=self.market_id,
             order_type="TYPE_LIMIT",
             time_in_force="TIME_IN_FORCE_GTC",
             side=self.side,
             volume=self.opening_auction_trade_amount,
             price=self.initial_price,
             wait=False,
-            key_name=self.key_name,
+            trading_key=self.key_name,
         )
 
     def step(self, vega_state: VegaState):
         pass
 
 
 class MarketManager(StateAgentWithWallet):
     NAME_BASE = "market_manager"
 
     def __init__(
         self,
-        wallet_name: str,
-        wallet_pass: str,
-        terminate_wallet_name: str,
-        terminate_wallet_pass: str,
+        key_name: str,
+        terminate_key_name: str,
         market_name: str,
         asset_name: str,
         asset_decimal: int = 5,
         market_decimal: int = 5,
         market_position_decimal: int = 2,
         initial_mint: Optional[float] = None,
         commitment_amount: Optional[float] = None,
         settlement_price: Optional[float] = None,
         tag: str = "",
-        key_name: str = None,
-        terminate_key_name: str = None,
+        wallet_name: str = None,
+        terminate_wallet_name: str = None,
     ):
-        super().__init__(
-            wallet_name=wallet_name, wallet_pass=wallet_pass, key_name=key_name, tag=tag
-        )
+        super().__init__(wallet_name=wallet_name, key_name=key_name, tag=tag)
         self.terminate_wallet_name = terminate_wallet_name
-        self.terminate_wallet_pass = terminate_wallet_pass
         self.terminate_key_name = terminate_key_name
 
         self.adp = asset_decimal
         self.mdp = market_decimal
         self.market_position_decimal = market_position_decimal
         self.commitment_amount = commitment_amount
 
@@ -953,68 +938,70 @@
         self.market_name = market_name
         self.asset_name = asset_name
         self.settlement_price = settlement_price
 
     def initialise(
         self,
         vega: Union[VegaServiceNull, VegaServiceNetwork],
-        create_wallet: bool = True,
-        mint_wallet: bool = True,
+        create_key: bool = True,
+        mint_key: bool = True,
     ):
         # Initialise wallet for LP/ Settle Party
-        super().initialise(vega=vega, create_wallet=create_wallet)
-        self.vega.create_wallet(
-            self.terminate_wallet_name,
-            self.terminate_wallet_pass,
-            self.terminate_key_name,
+        super().initialise(vega=vega, create_key=create_key)
+        self.vega.create_key(
+            wallet_name=self.terminate_wallet_name,
+            name=self.terminate_key_name,
         )
 
         # Faucet vega tokens
         self.vega.wait_for_total_catchup()
         self.vega.mint(
-            self.wallet_name, asset="VOTE", amount=1e4, key_name=self.key_name
+            wallet_name=self.wallet_name,
+            asset="VOTE",
+            amount=1e4,
+            key_name=self.key_name,
         )
         self.vega.wait_fn(5)
         self.vega.wait_for_total_catchup()
         if vega.find_asset_id(symbol=self.asset_name) is None:
             # Create asset
             self.vega.create_asset(
-                self.wallet_name,
+                wallet_name=self.wallet_name,
                 name=self.asset_name,
                 symbol=self.asset_name,
                 decimals=self.adp,
                 max_faucet_amount=5e10,
                 key_name=self.key_name,
             )
         self.vega.wait_fn(5)
         self.vega.wait_for_total_catchup()
         # Get asset id
         self.asset_id = self.vega.find_asset_id(symbol=self.asset_name)
-        if mint_wallet:
+        if mint_key:
             # Top up asset
             self.vega.mint(
-                self.wallet_name,
+                wallet_name=self.wallet_name,
                 asset=self.asset_id,
                 amount=self.initial_mint,
                 key_name=self.key_name,
             )
         self.vega.wait_fn(5)
 
         self.vega.wait_for_total_catchup()
         # Set up a future market
         self.vega.create_simple_market(
             market_name=self.market_name,
-            proposal_wallet=self.wallet_name,
+            wallet_name=self.wallet_name,
+            proposal_key=self.key_name,
             settlement_asset_id=self.asset_id,
-            termination_wallet=self.terminate_wallet_name,
             market_decimals=self.mdp,
             position_decimals=self.market_position_decimal,
             future_asset=self.asset_name,
-            key_name=self.key_name,
             termination_key=self.terminate_key_name,
+            termination_wallet_name=self.terminate_wallet_name,
         )
         self.vega.wait_for_total_catchup()
 
         # Get market id
         self.market_id = self.vega.find_market_id(name=self.market_name)
         if self.commitment_amount:
             self.vega.submit_liquidity(
@@ -1027,18 +1014,18 @@
                 is_amendment=False,
                 key_name=self.key_name,
             )
 
     def finalise(self):
         if self.settlement_price is not None:
             self.vega.settle_market(
-                self.terminate_wallet_name,
+                self.terminate_key_name,
                 self.settlement_price,
                 self.market_id,
-                self.terminate_key_name,
+                self.terminate_wallet_name,
             )
             self.vega.wait_for_total_catchup()
 
 
 class ShapedMarketMaker(StateAgentWithWallet):
     """Utilises the Ideal market maker formulation from
         Algorithmic and High-Frequency Trading by Cartea, Jaimungal and Penalva.
@@ -1050,16 +1037,15 @@
     source in the market but still to maintain an interesting full LOB.
     """
 
     NAME_BASE = "shaped_market_maker"
 
     def __init__(
         self,
-        wallet_name: str,
-        wallet_pass: str,
+        key_name: str,
         price_process_generator: Iterable[float],
         best_price_offset_fn: Callable[[float, int], Tuple[float, float]],
         shape_fn: Callable[
             [
                 float,
                 float,
             ],
@@ -1071,23 +1057,21 @@
         initial_asset_mint: float = 1000000,
         market_name: Optional[str] = None,
         asset_name: Optional[str] = None,
         commitment_amount: float = 6000,
         market_decimal_places: int = 5,
         asset_decimal_places: int = 0,
         tag: str = "",
-        key_name: str = None,
+        wallet_name: str = None,
         orders_from_stream: Optional[bool] = True,
         state_update_freq: Optional[int] = None,
         safety_factor: Optional[float] = 1.2,
         max_order_size: float = 10000,
     ):
-        super().__init__(
-            wallet_name=wallet_name, wallet_pass=wallet_pass, key_name=key_name, tag=tag
-        )
+        super().__init__(wallet_name=wallet_name, key_name=key_name, tag=tag)
         self.price_process_generator = price_process_generator
         self.commitment_amount = commitment_amount
         self.initial_asset_mint = initial_asset_mint
         self.mdp = market_decimal_places
         self.adp = asset_decimal_places
 
         self.shape_fn = shape_fn
@@ -1109,41 +1093,43 @@
 
         self.bid_depth = None
         self.ask_depth = None
 
     def initialise(
         self,
         vega: Union[VegaServiceNull, VegaServiceNetwork],
-        create_wallet: bool = True,
-        mint_wallet: bool = True,
+        create_key: bool = True,
+        mint_key: bool = True,
     ):
         # Initialise wallet for LP/ Settle Party
-        super().initialise(vega=vega, create_wallet=create_wallet)
+        super().initialise(vega=vega, create_key=create_key)
 
         # Get asset id
         self.asset_id = self.vega.find_asset_id(symbol=self.asset_name)
-        if mint_wallet:
+        if mint_key:
             # Top up asset
             self.vega.mint(
-                self.wallet_name,
+                wallet_name=self.wallet_name,
                 asset=self.asset_id,
                 amount=self.initial_asset_mint,
                 key_name=self.key_name,
             )
             self.vega.wait_for_total_catchup()
 
         # Get market id
         self.market_id = self.vega.find_market_id(name=self.market_name)
 
         self._update_state(current_step=self.current_step)
 
         if (
-            initial_liq := self.liquidity_commitment_fn(None)
-            if self.liquidity_commitment_fn is not None
-            else None
+            initial_liq := (
+                self.liquidity_commitment_fn(None)
+                if self.liquidity_commitment_fn is not None
+                else None
+            )
         ) is not None:
             self.vega.submit_liquidity(
                 wallet_name=self.wallet_name,
                 market_id=self.market_id,
                 commitment_amount=initial_liq.amount,
                 fee=initial_liq.fee,
                 buy_specs=initial_liq.buy_specs,
@@ -1178,19 +1164,26 @@
             buy_shape=new_buy_shape, sell_shape=new_sell_shape
         )
 
         curr_buy_orders, curr_sell_orders = [], []
 
         if self.orders_from_stream:
             orders = (
-                vega_state.market_state.get(self.market_id, {})
-                .orders.get(
-                    self.vega.wallet.public_key(self.wallet_name, self.key_name), {}
+                (
+                    vega_state.market_state[self.market_id]
+                    .orders.get(
+                        self.vega.wallet.public_key(
+                            wallet_name=self.wallet_name, name=self.key_name
+                        ),
+                        {},
+                    )
+                    .values()
                 )
-                .values()
+                if self.market_id in vega_state.market_state
+                else []
             )
         else:
             orders = self.vega.list_orders(
                 wallet_name=self.wallet_name,
                 key_name=self.key_name,
                 market_id=self.market_id,
                 live_only=True,
@@ -1228,17 +1221,19 @@
             self._move_side(
                 vega_protos.SIDE_BUY,
                 curr_buy_orders,
                 scaled_buy_shape,
             )
 
         if (
-            liq := self.liquidity_commitment_fn(vega_state)
-            if self.liquidity_commitment_fn is not None
-            else None
+            liq := (
+                self.liquidity_commitment_fn(vega_state)
+                if self.liquidity_commitment_fn is not None
+                else None
+            )
         ) is not None:
             self.vega.submit_liquidity(
                 wallet_name=self.wallet_name,
                 market_id=self.market_id,
                 commitment_amount=liq.amount,
                 fee=liq.fee,
                 buy_specs=liq.buy_specs,
@@ -1295,23 +1290,23 @@
 
         return provided_liquidity
 
     def _submit_order(
         self, side: Union[str, vega_protos.Side], price: float, size: float
     ) -> None:
         self.vega.submit_order(
-            trading_wallet=self.wallet_name,
+            trading_key=self.key_name,
             market_id=self.market_id,
             order_type="TYPE_LIMIT",
             time_in_force="TIME_IN_FORCE_GTC",
             side=side,
             volume=size,
             price=price,
             wait=False,
-            key_name=self.key_name,
+            trading_wallet=self.wallet_name,
         )
 
     def _move_side(
         self,
         side: vega_protos.Side,
         orders: List[Order],
         new_shape: List[MMOrder],
@@ -1396,16 +1391,15 @@
     source in the market but still to maintain an interesting full LOB.
     """
 
     NAME_BASE = "expon_shaped_market_maker"
 
     def __init__(
         self,
-        wallet_name: str,
-        wallet_pass: str,
+        key_name: str,
         num_steps: int,
         price_process_generator: Iterable[float],
         initial_asset_mint: float = 1000000,
         market_name: str = None,
         asset_name: str = None,
         commitment_amount: float = 6000,
         market_decimal_places: int = 5,
@@ -1417,22 +1411,21 @@
         inventory_lower_boundary: float = -20,
         terminal_penalty_parameter: float = 10**-4,
         running_penalty_parameter: float = 5 * 10**-6,
         market_order_arrival_rate: float = 5,
         market_kappa: float = 1,
         asset_decimal_places: int = 0,
         tag: str = "",
-        key_name: str = None,
+        wallet_name: str = None,
         orders_from_stream: Optional[bool] = True,
         state_update_freq: Optional[int] = None,
         max_order_size: float = 10000,
     ):
         super().__init__(
             wallet_name=wallet_name,
-            wallet_pass=wallet_pass,
             price_process_generator=price_process_generator,
             initial_asset_mint=initial_asset_mint,
             market_name=market_name,
             asset_name=asset_name,
             commitment_amount=commitment_amount,
             market_decimal_places=market_decimal_places,
             asset_decimal_places=asset_decimal_places,
@@ -1582,23 +1575,23 @@
 
         base_price = self.curr_price + mult_factor * price_depth
         level_price = np.arange(
             base_price,
             base_price + mult_factor * self.num_levels * self.tick_spacing,
             mult_factor * self.tick_spacing,
         )
+        level_price[level_price < 1 / 10**self.mdp] = 1 / 10**self.mdp
 
         return [MMOrder(vol, price) for vol, price in zip(level_vol, level_price)]
 
 
 class HedgedMarketMaker(ExponentialShapedMarketMaker):
     def __init__(
         self,
-        wallet_name: str,
-        wallet_pass: str,
+        key_name: str,
         num_steps: int,
         price_process_generator: Iterable[float],
         internal_key_mint: float = 1000000,
         external_key_mint: float = 1000000,
         market_name: str = None,
         external_market_name: str = None,
         asset_name: str = None,
@@ -1612,26 +1605,25 @@
         inventory_lower_boundary: float = -20,
         terminal_penalty_parameter: float = 10**-4,
         running_penalty_parameter: float = 5 * 10**-6,
         market_order_arrival_rate: float = 5,
         market_kappa: float = 1,
         asset_decimal_places: int = 0,
         tag: str = "",
-        key_name: str = None,
+        wallet_name: str = None,
         external_key_name: Optional[float] = "Hedging Key",
         orders_from_stream: Optional[bool] = True,
         state_update_freq: Optional[int] = None,
         profit_margin: Optional[float] = 0.01,
         internal_delay: int = 60 * 60,
         external_delay: int = 5 * 60,
         transfer_threshold: float = 500,
     ):
         super().__init__(
             wallet_name=wallet_name,
-            wallet_pass=wallet_pass,
             num_steps=num_steps,
             price_process_generator=price_process_generator,
             initial_asset_mint=internal_key_mint,
             market_name=market_name,
             asset_name=asset_name,
             commitment_amount=commitment_amount,
             market_decimal_places=market_decimal_places,
@@ -1663,32 +1655,32 @@
 
         self.transfer_threshold = transfer_threshold
         self.external_key_mint = external_key_mint
 
     def initialise(
         self,
         vega: Union[VegaServiceNull, VegaServiceNetwork],
-        create_wallet: bool = True,
-        mint_wallet: bool = True,
+        create_key: bool = True,
+        mint_key: bool = True,
     ):
         # Initialise the parent ExponentialShapedMarketMaker
-        super().initialise(vega, create_wallet, mint_wallet)
+        super().initialise(vega, create_key, mint_key)
 
         self.external_market_id = self.vega.find_market_id(
             name=self.external_market_name
         )
         self._update_state(current_step=self.current_step)
 
-        if vega.create_wallet:
-            vega.create_wallet(
-                name=self.wallet_name,
+        if vega.create_key:
+            vega.create_key(
+                wallet_name=self.wallet_name,
                 passphrase=self.wallet_pass,
-                key_name=self.external_key_name,
+                name=self.external_key_name,
             )
-        if mint_wallet:
+        if mint_key:
             vega.mint(
                 wallet_name=self.wallet_name,
                 asset=self.asset_id,
                 amount=self.external_key_mint,
                 key_name=self.external_key_name,
             )
 
@@ -1776,15 +1768,15 @@
         elif position_delta < 0:
             side = vega_protos.SIDE_BUY
         elif position_delta > 0:
             side = vega_protos.SIDE_SELL
 
         self.vega.submit_market_order(
             trading_wallet=self.wallet_name,
-            key_name=self.external_key_name,
+            trading_key=self.external_key_name,
             market_id=self.external_market_id,
             volume=abs(position_delta),
             side=side,
             wait=False,
             fill_or_kill=False,
         )
 
@@ -1810,27 +1802,27 @@
         # Get the balance currently locked in transfers inbound to the internal market
         transfers = self.vega.transfer_status_from_feed(live_only=True)
         internal_transfers_balance = sum(
             [
                 transfer.amount
                 for transfer in transfers.get(
                     self.vega.wallet.public_key(
-                        name=self.wallet_name, key_name=self.key_name
+                        name=self.key_name, wallet_name=self.wallet_name
                     ),
                     {},
                 ).values()
             ]
         )
         # Get the balance currently locked in transfers inbound to the external market
         external_transfers_balance = sum(
             [
                 transfer.amount
                 for transfer in transfers.get(
                     self.vega.wallet.public_key(
-                        name=self.wallet_name, key_name=self.external_key_name
+                        name=self.key_name, wallet_name=self.external_key_name
                     ),
                     {},
                 ).values()
             ]
         )
 
         # Calculate the difference between the total balance on the markets
@@ -1888,16 +1880,15 @@
     distribution where the underlying normal distribution can be adjusted.
     """
 
     NAME_BASE = "lo_trader"
 
     def __init__(
         self,
-        wallet_name: str,
-        wallet_pass: str,
+        key_name: str,
         market_name: str,
         asset_name: str,
         initial_asset_mint: float = 1000000,
         buy_volume: float = 1.0,
         sell_volume: float = 1.0,
         buy_intensity: float = 5,
         sell_intensity: float = 5,
@@ -1908,15 +1899,15 @@
         side_opts: Optional[dict] = None,
         time_in_force_opts: Optional[dict] = None,
         duration: Optional[float] = 120,
         price_process: Optional[list] = None,
         spread: Optional[float] = None,
         mean: Optional[float] = 2.0,
         sigma: Optional[float] = 1.0,
-        key_name: str = None,
+        wallet_name: str = None,
     ):
         """Init the object and class attributes.
 
         Args:
             wallet_name (str):
                 Name of the agents wallet.
             wallet_pass (str):
@@ -1951,17 +1942,15 @@
                 Spread of the agent.
             mean (float, optional):
                 Mean of the log-normal distribution.
             sigma (float, optional):
                 Standard deviation of the log-normal distribution.
         """
 
-        super().__init__(
-            wallet_name=wallet_name, wallet_pass=wallet_pass, key_name=key_name, tag=tag
-        )
+        super().__init__(wallet_name=wallet_name, key_name=key_name, tag=tag)
 
         self.current_step = 0
 
         self.market_name = market_name
         self.asset_name = asset_name
         self.initial_asset_mint = initial_asset_mint
         self.buy_intensity = buy_intensity
@@ -1991,31 +1980,31 @@
         self.spread = spread
         self.mean = mean
         self.sigma = sigma
 
     def initialise(
         self,
         vega: VegaService,
-        create_wallet: bool = True,
-        mint_wallet: bool = False,
+        create_key: bool = True,
+        mint_key: bool = False,
     ):
         """Initialise the agents wallet and mint the required market asset.
 
         Args:
             vega (VegaServiceNull):
                 Object running a locally-hosted Vega service.
         """
 
-        super().initialise(vega=vega, create_wallet=create_wallet)
+        super().initialise(vega=vega, create_key=create_key)
         self.market_id = self.vega.find_market_id(name=self.market_name)
 
         self.asset_id = self.vega.find_asset_id(symbol=self.asset_name)
-        if mint_wallet:
+        if mint_key:
             self.vega.mint(
-                self.wallet_name,
+                wallet_name=self.wallet_name,
                 asset=self.asset_id,
                 amount=self.initial_asset_mint,
                 key_name=self.key_name,
             )
         self.vega.wait_fn(2)
 
     def step(self, vega_state: VegaState):
@@ -2083,51 +2072,53 @@
             price=price,
             side=side,
             volume=volume,
             order_type=vega_protos.Order.Type.TYPE_LIMIT,
             wait=False,
             time_in_force=time_in_force,
             expires_at=expires_at,
-            key_name=self.key_name,
+            trading_key=self.key_name,
         )
 
     def _cancel_order(self, vega_state: VegaState):
         orders = vega_state.market_state.get(self.market_id, {}).orders.get(
-            self.vega.wallet.public_key(self.wallet_name, self.key_name), {}
+            self.vega.wallet.public_key(
+                wallet_name=self.wallet_name, name=self.key_name
+            ),
+            {},
         )
 
         if len(orders) > 0:
             order_key = self.random_state.choice(list(orders.keys()))
             order = orders[order_key]
 
             self.vega.cancel_order(
-                trading_wallet=self.wallet_name,
+                wallet_name=self.wallet_name,
                 market_id=self.market_id,
                 order_id=order.id,
-                key_name=self.key_name,
+                trading_key=self.key_name,
             )
 
 
 class InformedTrader(StateAgentWithWallet):
     NAME_BASE = "informed_trader"
 
     def __init__(
         self,
-        wallet_name: str,
-        wallet_pass: str,
+        key_name: str,
         price_process: List[float],
         market_name: str = None,
         asset_name: str = None,
         initial_asset_mint: float = 1e8,
         proportion_taken: float = 0.8,
         accuracy: float = 1.0,
         lookahead: int = 1,
         max_abs_position: float = 100,
         tag: str = "",
-        key_name: Optional[str] = None,
+        wallet_name: Optional[str] = None,
         random_state: Optional[np.random.RandomState] = None,
     ):
         """Agent capable of placing informed market orders.
 
         At each step, the agent is able to lookahead a specified number of steps and
         determine whether orders currently on the book are profitable to fill. The
         agent will then fill a specified proportion of those orders. This order will
@@ -2141,16 +2132,14 @@
         Additionally the accuracy arg can be used to configure the accuracy of the agent
         (1.0 being well-informed, 0.0 being ill-informed). If the agent is ill-informed
         it has a random probability of placing its orders on the wrong side.
 
         Args:
             wallet_name (str):
                 Name of the wallet.
-            wallet_pass (str):
-                Passphrase for the wallet.
             price_process (List[float]):
                 List of price history for agent to look-ahead.
             market_name (str, optional):
                 Name of the market to trade in. Defaults to None.
             asset_name (str, optional):
                 Name of the settlement asset used in the market. Defaults to None.
             initial_asset_mint (float, optional):
@@ -2166,17 +2155,15 @@
             tag (str, optional):
                 Market tag. Defaults to "".
             key_name (Optional[str], optional):
                 Name of key in wallet. Defaults to None.
             random_state (Optional[np.random.RandomState], optional):
                 RandomState object used to generate randomness. Defaults to None.
         """
-        super().__init__(
-            wallet_name=wallet_name, wallet_pass=wallet_pass, key_name=key_name, tag=tag
-        )
+        super().__init__(wallet_name=wallet_name, key_name=key_name, tag=tag)
         self.initial_asset_mint = initial_asset_mint
         self.price_process = price_process
         self.current_step = 0
         self.sim_length = len(price_process)
         self.proportion_taken = proportion_taken
         self.market_name = f"ETH:USD_{self.tag}" if market_name is None else market_name
         self.asset_name = f"tDAI_{self.tag}" if asset_name is None else asset_name
@@ -2190,29 +2177,29 @@
         self.random_state = (
             random_state if random_state is not None else np.random.RandomState()
         )
 
     def initialise(
         self,
         vega: Union[VegaServiceNull, VegaServiceNetwork],
-        create_wallet: bool = True,
-        mint_wallet: bool = True,
+        create_key: bool = True,
+        mint_key: bool = True,
     ):
         # Initialise wallet
-        super().initialise(vega=vega, create_wallet=create_wallet)
+        super().initialise(vega=vega, create_key=create_key)
 
         # Get market id
         self.market_id = self.vega.find_market_id(name=self.market_name)
 
         # Get asset id
         tDAI_id = self.vega.find_asset_id(symbol=self.asset_name)
-        if mint_wallet:
+        if mint_key:
             # Top up asset
             self.vega.mint(
-                self.wallet_name,
+                wallet_name=self.wallet_name,
                 asset=tDAI_id,
                 amount=self.initial_asset_mint,
                 key_name=self.key_name,
             )
 
         self.pdp = self.vega._market_pos_decimals.get(self.market_id, {})
         self.vega.wait_for_total_catchup()
@@ -2286,15 +2273,15 @@
             self.vega.submit_market_order(
                 trading_wallet=self.wallet_name,
                 market_id=self.market_id,
                 side=side,
                 volume=size,
                 wait=False,
                 fill_or_kill=False,
-                key_name=self.key_name,
+                trading_key=self.key_name,
             )
             return ITOrder(side=side, size=size)
 
         except OrderRejectedError:
             logger.debug("Order rejected")
             return None
 
@@ -2316,81 +2303,135 @@
             self.vega.submit_market_order(
                 trading_wallet=self.wallet_name,
                 market_id=self.market_id,
                 side=side,
                 volume=order.volume,
                 wait=True,
                 fill_or_kill=False,
-                key_name=self.key_name,
+                trading_key=self.key_name,
             )
         except OrderRejectedError:
             logger.debug("Order rejected")
 
 
-class LiquidityProvider(StateAgentWithWallet):
-    NAME_BASE = "liq_provider"
+class SimpleLiquidityProvider(StateAgentWithWallet):
+    NAME_BASE = "simple_liq_provider"
 
     def __init__(
         self,
-        wallet_name: str,
-        wallet_pass: str,
+        key_name: str,
         market_name: str,
         asset_name: str,
+        bid_inner_bound_fn: Callable,
+        bid_outer_bound_fn: Callable,
+        ask_inner_bound_fn: Callable,
+        ask_outer_bound_fn: Callable,
+        offset_proportion: int,
         initial_asset_mint: float,
         commitment_amount: float = 6000,
-        offset: float = 0.01,
         fee: float = 0.001,
         tag: str = "",
-        key_name: Optional[str] = None,
+        wallet_name: Optional[str] = None,
     ):
-        super().__init__(
-            wallet_name=wallet_name, wallet_pass=wallet_pass, key_name=key_name, tag=tag
-        )
+        super().__init__(wallet_name=wallet_name, key_name=key_name, tag=tag)
 
         self.market_name = market_name
         self.asset_name = asset_name
 
         self.initial_asset_mint = initial_asset_mint
 
-        self.offset = offset
+        self.bid_inner_bound_fn = bid_inner_bound_fn
+        self.bid_outer_bound_fn = bid_outer_bound_fn
+        self.ask_inner_bound_fn = ask_inner_bound_fn
+        self.ask_outer_bound_fn = ask_outer_bound_fn
+        self.offset_proportion = offset_proportion
 
         self.fee = fee
 
         self.commitment_amount = commitment_amount
 
     def initialise(
         self,
         vega: Union[VegaServiceNull, VegaServiceNetwork],
-        create_wallet: bool = True,
-        mint_wallet: bool = True,
+        create_key: bool = True,
+        mint_key: bool = True,
     ):
-        super().initialise(vega=vega, create_wallet=create_wallet)
+        super().initialise(vega=vega, create_key=create_key)
 
         self.market_id = self.vega.find_market_id(name=self.market_name)
         self.asset_id = self.vega.find_asset_id(symbol=self.asset_name)
-        if mint_wallet:
+        if mint_key:
             self.vega.mint(
-                self.wallet_name,
+                wallet_name=self.wallet_name,
                 asset=self.asset_id,
                 amount=self.initial_asset_mint,
                 key_name=self.key_name,
             )
             self.vega.wait_fn(2)
 
-        self.vega.wait_for_total_catchup()
+        self.vega.submit_simple_liquidity(
+            wallet_name=self.wallet_name,
+            market_id=self.market_id,
+            key_name=self.key_name,
+            commitment_amount=self.commitment_amount,
+            fee=self.fee,
+            reference_buy="PEGGED_REFERENCE_MID",
+            reference_sell="PEGGED_REFERENCE_MID",
+            delta_buy=5,
+            delta_sell=5,
+            is_amendment=False,
+        )
 
+    def step(self, vega_state: VegaState):
+        # Don't amend offset if in auction
+        if (
+            vega_state.market_state[self.market_id].trading_mode
+            != markets_protos.Market.TradingMode.TRADING_MODE_CONTINUOUS
+        ):
+            return
+
+        # Get the lower and upper bounds liquidity can be pegged between
+        bid_inner_bound = self.bid_inner_bound_fn(
+            vega_state=vega_state, market_id=self.market_id
+        )
+        bid_outer_bound = self.bid_outer_bound_fn(
+            vega_state=vega_state, market_id=self.market_id
+        )
+        ask_inner_bound = self.ask_inner_bound_fn(
+            vega_state=vega_state, market_id=self.market_id
+        )
+        ask_outer_bound = self.ask_outer_bound_fn(
+            vega_state=vega_state, market_id=self.market_id
+        )
+
+        bid_price = (
+            bid_inner_bound
+            - (bid_inner_bound - bid_outer_bound) * self.offset_proportion
+        )
+        ask_price = (
+            ask_inner_bound
+            + (ask_outer_bound - ask_inner_bound) * self.offset_proportion
+        )
+
+        # Calculate offsets for the bid and ask pegs from the mid-price
+        bid_offset = vega_state.market_state[self.market_id].midprice - bid_price
+        ask_offset = ask_price - vega_state.market_state[self.market_id].midprice
+
+        # Submit liquidity
         self.vega.submit_simple_liquidity(
             wallet_name=self.wallet_name,
+            key_name=self.key_name,
             market_id=self.market_id,
             commitment_amount=self.commitment_amount,
-            fee=0.001,
-            reference_buy="PEGGED_REFERENCE_BEST_BID",
-            reference_sell="PEGGED_REFERENCE_BEST_ASK",
-            delta_buy=self.offset,
-            delta_sell=self.offset,
+            fee=self.fee,
+            reference_buy="PEGGED_REFERENCE_MID",
+            reference_sell="PEGGED_REFERENCE_MID",
+            delta_buy=bid_offset,
+            delta_sell=ask_offset,
+            is_amendment=True,
         )
 
 
 class MomentumTrader(StateAgentWithWallet):
     """
     Trading Agent that can follow multiple momentum trading strategies.
 
@@ -2398,16 +2439,15 @@
     certain momentum indicator.
     """
 
     NAME_BASE = "mom_trader"
 
     def __init__(
         self,
-        wallet_name: str,
-        wallet_pass: str,
+        key_name: str,
         market_name: str,
         asset_name: str,
         momentum_strategy: str = "RSI",
         momentum_strategy_args: Dict[str, float] = None,
         indicator_threshold: Tuple[float, float] = (70, 30),
         initial_asset_mint: float = 1e5,
         order_intensity: float = 5,
@@ -2415,19 +2455,17 @@
         trading_proportion: float = 1,
         random_state: Optional[np.random.RandomState] = None,
         send_limit_order: bool = False,
         time_in_force_opt: Union[vega_protos.vega.Order.TimeInForce, str] = None,
         duration: Optional[float] = 120,
         offset_levels: int = 10,
         tag: str = "",
-        key_name: str = None,
+        wallet_name: str = None,
     ):
-        super().__init__(
-            wallet_name=wallet_name, wallet_pass=wallet_pass, key_name=key_name, tag=tag
-        )
+        super().__init__(wallet_name=wallet_name, key_name=key_name, tag=tag)
         self.market_name = market_name
         self.asset_name = asset_name
         self.initial_asset_mint = initial_asset_mint
         self.order_intensity = order_intensity
         self.base_order_size = base_order_size
         self.trading_proportion = trading_proportion
         self.random_state = (
@@ -2459,25 +2497,25 @@
 
         self.prices = np.array([])
         self.indicators = []
 
     def initialise(
         self,
         vega: Union[VegaServiceNull, VegaServiceNetwork],
-        create_wallet: bool = True,
-        mint_wallet: bool = True,
+        create_key: bool = True,
+        mint_key: bool = True,
     ):
-        super().initialise(vega=vega, create_wallet=create_wallet)
+        super().initialise(vega=vega, create_key=create_key)
 
         self.market_id = self.vega.find_market_id(name=self.market_name)
 
         self.asset_id = self.vega.find_asset_id(symbol=self.asset_name)
-        if mint_wallet:
+        if mint_key:
             self.vega.mint(
-                self.wallet_name,
+                wallet_name=self.wallet_name,
                 asset=self.asset_id,
                 amount=self.initial_asset_mint,
                 key_name=self.key_name,
             )
 
         self.pdp = self.vega._market_pos_decimals.get(self.market_id, {})
         self.mdp = self.vega._market_price_decimals.get(self.market_id, {})
@@ -2505,15 +2543,15 @@
                 self.vega.submit_market_order(
                     trading_wallet=self.wallet_name,
                     market_id=self.market_id,
                     side=trade_side,
                     volume=volume,
                     wait=False,
                     fill_or_kill=False,
-                    key_name=self.key_name,
+                    trading_key=self.key_name,
                 )
             else:
                 best_bid, best_ask = self.vega.best_prices(market_id=self.market_id)
                 price = (
                     best_ask + self.offset_levels / 10**self.mdp
                     if signal == TradeSignal.BUY
                     else best_bid - self.offset_levels / 10**self.mdp
@@ -2525,15 +2563,15 @@
                     order_type="TYPE_LIMIT",
                     time_in_force=self.time_in_force_opt,
                     side=trade_side,
                     volume=volume,
                     price=price,
                     expires_at=expires_at,
                     wait=False,
-                    key_name=self.key_name,
+                    trading_key=self.key_name,
                 )
 
     def _MACD(self):
         _, _, macdhist = (
             talib.MACD(self.prices)
             if self.momentum_strategy_args is None
             else talib.MACD(
@@ -2662,48 +2700,89 @@
 
     def __init__(
         self,
         agents: Optional[Dict[str, Agent]] = None,
         additional_state_fn: Optional[
             Callable[[VegaService, Dict[str, Agent]], Any]
         ] = None,
+        only_extract_additional: bool = False,
     ):
         self.tag = None
         self.states = []
         self.additional_states = []
         self.agents = agents
         self.additional_state_fn = additional_state_fn
         self.seen_trades = set()
+        self.only_extract_additional = only_extract_additional
 
     def step(self, vega_state: VegaState):
-        market_infos = {}
-        market_datas = {}
-        market_depths = {}
-        market_trades = {}
-
-        start_time = self.vega.get_blockchain_time()
-        for market in self.vega.all_markets():
-            market_infos[market.id] = self.vega.market_info(market.id)
-            market_datas[market.id] = self.vega.market_data(market.id)
-            market_depths[market.id] = self.vega.market_depth(market.id, num_levels=50)
-
-        all_trades = self.vega.get_trades_from_stream()
-        for trade in all_trades:
-            if trade.id not in self.seen_trades:
-                self.seen_trades.add(trade.id)
-                market_trades.setdefault(market.id, []).append(trade)
-
-        accounts = self.vega.list_accounts()
-        self.states.append(
-            MarketHistoryData(
-                at_time=start_time,
-                market_info=market_infos,
-                market_data=market_datas,
-                accounts=accounts,
-                market_depth=market_depths,
-                trades=market_trades,
+        if not self.only_extract_additional:
+            market_infos = {}
+            market_datas = {}
+            market_depths = {}
+            market_trades = {}
+
+            start_time = self.vega.get_blockchain_time()
+
+            all_markets = self.vega.all_markets()
+            for market in all_markets:
+                market_infos[market.id] = market
+                market_datas[market.id] = self.vega.market_data_from_feed(market.id)
+                market_depths[market.id] = self.vega.market_depth(
+                    market.id, num_levels=50
+                )
+
+            all_trades = self.vega.get_trades_from_stream(
+                exclude_trade_ids=self.seen_trades
+            )
+            for trade in all_trades:
+                if trade.id not in self.seen_trades:
+                    self.seen_trades.add(trade.id)
+                    market_trades.setdefault(market.id, []).append(trade)
+
+            accounts = self.vega.list_accounts()
+            self.states.append(
+                MarketHistoryData(
+                    at_time=start_time,
+                    market_info=market_infos,
+                    market_data=market_datas,
+                    accounts=accounts,
+                    market_depth=market_depths,
+                    trades=market_trades,
+                )
             )
-        )
         if self.additional_state_fn is not None:
             self.additional_states.append(
                 self.additional_state_fn(self.vega, self.agents)
             )
+
+
+class KeyFunder(Agent):
+    NAME_BASE = "key_funder"
+
+    def __init__(
+        self,
+        keys_to_fund: List[str],
+        asset_to_fund: str,
+        amount_to_fund: float,
+        tag: Optional[str] = None,
+    ):
+        super().__init__(tag=tag)
+        self.keys_to_fund = keys_to_fund
+        self.amount_to_fund = amount_to_fund
+        self.asset_to_fund = asset_to_fund
+
+    def initialise(
+        self,
+        vega: Union[VegaServiceNull, VegaServiceNetwork],
+        create_key: bool = True,
+        mint_key: bool = True,
+    ):
+        self.vega = vega
+        asset_id = self.vega.find_asset_id(self.asset_to_fund)
+        amount = self.amount_to_fund * 10 ** self.vega.asset_decimals[asset_id]
+        for key in self.keys_to_fund:
+            faucet.mint(key, asset_id, amount=amount, faucet_url=self.vega.faucet_url)
+        time.sleep(1)
+
+    def step(self, vega_state: VegaState):
+        pass
```

### Comparing `vega_sim-0.67.0/vega_sim/scenario/common/utils/ideal_mm_models.py` & `vega_sim-1.0.1/vega_sim/scenario/common/utils/ideal_mm_models.py`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/scenario/common/utils/price_process.py` & `vega_sim-1.0.1/vega_sim/scenario/common/utils/price_process.py`

 * *Files 18% similar despite different names*

```diff
@@ -136,29 +136,44 @@
     return res
 
 
 def get_historic_price_series(
     product_id: str,
     price_component: CoinbaseCandle = CoinbaseCandle.CLOSE,
     granularity: Optional[Granularity] = None,
+    interpolation: str = None,
     start: Optional[str] = None,
     end: Optional[str] = None,
 ) -> pd.Series:
     ohlcv = get_historic_candles(
         product_id=product_id,
         granularity=granularity,
         start=start,
         end=end,
     )
-    return pd.Series(
-        data=[o[price_component.value] for o in ohlcv],
-        index=pd.DatetimeIndex(
-            [pd.to_datetime(o[CoinbaseCandle.TIME.value], unit="s") for o in ohlcv],
-        ),
-    ).sort_index()
+    s = (
+        pd.Series(
+            data=[o[price_component.value] for o in ohlcv],
+            index=pd.DatetimeIndex(
+                [pd.to_datetime(o[CoinbaseCandle.TIME.value], unit="s") for o in ohlcv],
+            ),
+        )
+        .sort_index()
+        .drop_duplicates()
+    )
+
+    if interpolation is not None:
+        s_interpolated = pd.Series(
+            index=pd.date_range(start=s.index[0], end=s.index[-1], freq=interpolation)
+        )
+        s_interpolated.update(s)
+        s_interpolated = s_interpolated.interpolate(method="linear")
+        return s_interpolated
+    else:
+        return s
 
 
 if __name__ == "__main__":
     print(
         get_historic_price_series(
             "ETH-USD",
             granularity=Granularity.HOUR,
```

### Comparing `vega_sim-0.67.0/vega_sim/scenario/comprehensive_market/agents.py` & `vega_sim-1.0.1/vega_sim/scenario/comprehensive_market/agents.py`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/scenario/comprehensive_market/scenario.py` & `vega_sim-1.0.1/vega_sim/scenario/comprehensive_market/scenario.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     AUCTION1_WALLET,
     AUCTION2_WALLET,
     TERMINATE_WALLET,
     create_agent_wallets,
 )
 from vega_sim.scenario.common.agents import (
     MarketManager,
-    LiquidityProvider,
+    SimpleLiquidityProvider,
     MarketOrderTrader,
     LimitOrderTrader,
     MomentumTrader,
     OpenAuctionPass,
     StateAgent,
 )
 
@@ -155,63 +155,58 @@
         price_process = (
             self.price_process_fn()
             if self.price_process_fn is not None
             else self._generate_price_process(random_state=random_state)
         )
 
         mm_agent = MarketManager(
-            wallet_name=MM_WALLET.name,
-            wallet_pass=MM_WALLET.passphrase,
-            terminate_wallet_name=TERMINATE_WALLET.name,
-            terminate_wallet_pass=TERMINATE_WALLET.passphrase,
+            key_name=MM_WALLET.name,
+            terminate_key_name=TERMINATE_WALLET.name,
             asset_decimal=self.asset_decimal,
             market_decimal=self.market_decimal,
             market_position_decimal=self.market_position_decimal,
             market_name=market_name,
             asset_name=asset_name,
             commitment_amount=self.lp_commitamount,
             tag=str(tag),
             settlement_price=price_process[-1] if self.settle_at_end else None,
         )
 
         lp_agents = [
             LiquidityProvider(
-                wallet_name=self.lp_wallets[i].name,
-                wallet_pass=self.lp_wallets[i].passphrase,
+                key_name=self.lp_wallets[i].name,
                 initial_asset_mint=self.initial_asset_mint,
                 market_name=market_name,
                 asset_name=asset_name,
                 tag=f"{i}_{tag}",
                 commitment_amount=self.lp_commitamount,
                 fee=0.001,
                 offset=self.spread * (i + 1),
             )
             for i in range(len(self.lp_wallets))
         ]
 
         mo_agents = [
             MarketOrderTrader(
-                wallet_name=self.mo_wallets[i].name,
-                wallet_pass=self.mo_wallets[i].passphrase,
+                key_name=self.mo_wallets[i].name,
                 initial_asset_mint=self.initial_asset_mint,
                 market_name=market_name,
                 asset_name=asset_name,
                 tag=f"{i}_{tag}",
                 buy_intensity=self.market_order_trader_order_intensity,
                 sell_intensity=self.market_order_trader_order_intensity,
                 base_order_size=self.market_order_trader_order_size,
                 random_state=random_state,
             )
             for i in range(len(self.mo_wallets))
         ]
 
         lo_agents = [
             LimitOrderTrader(
-                wallet_name=self.lo_wallets[i].name,
-                wallet_pass=self.lo_wallets[i].passphrase,
+                key_name=self.lo_wallets[i].name,
                 initial_asset_mint=self.initial_asset_mint,
                 market_name=market_name,
                 asset_name=asset_name,
                 tag=f"{i}_{tag}",
                 spread=self.spread,
                 price_process=price_process,
                 buy_intensity=self.limit_order_trader_order_intensity,
@@ -227,16 +222,15 @@
                 random_state=random_state,
             )
             for i in range(len(self.lo_wallets))
         ]
 
         momentum_agents = [
             MomentumTrader(
-                wallet_name=self.momentum_wallets[i].name,
-                wallet_pass=self.momentum_wallets[i].passphrase,
+                key_name=self.momentum_wallets[i].name,
                 market_name=market_name,
                 asset_name=asset_name,
                 initial_asset_mint=self.initial_asset_mint,
                 order_intensity=self.momentum_trader_order_intensity,
                 base_order_size=self.momentum_trader_order_size,
                 momentum_strategy=self.momentum_trader_strategies[i],
                 momentum_strategy_args=self.momentum_trader_strategy_args[i]
@@ -247,30 +241,28 @@
                 offset_levels=20,
                 tag=f"{i}_{tag}",
             )
             for i in range(len(self.momentum_wallets))
         ]
 
         auctionpass1 = OpenAuctionPass(
-            wallet_name=AUCTION1_WALLET.name,
-            wallet_pass=AUCTION1_WALLET.passphrase,
+            key_name=AUCTION1_WALLET.name,
             side="SIDE_BUY",
             initial_asset_mint=self.initial_asset_mint,
             initial_price=self.initial_price
             if self.initial_price is not None
             else price_process[0],
             market_name=market_name,
             asset_name=asset_name,
             opening_auction_trade_amount=self.opening_auction_trade_amount,
             tag=f"1_{tag}",
         )
 
         auctionpass2 = OpenAuctionPass(
-            wallet_name=AUCTION2_WALLET.name,
-            wallet_pass=AUCTION2_WALLET.passphrase,
+            key_name=AUCTION2_WALLET.name,
             side="SIDE_SELL",
             initial_asset_mint=self.initial_asset_mint,
             initial_price=self.initial_price
             if self.initial_price is not None
             else price_process[0],
             market_name=market_name,
             asset_name=asset_name,
```

### Comparing `vega_sim-0.67.0/vega_sim/scenario/configurable_market/agents.py` & `vega_sim-1.0.1/vega_sim/scenario/configurable_market/agents.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,38 +22,34 @@
 SENSITIVE_PARTY_C = PartyConfig(WALLET_NAME, WALLET_PASS, "sensitive_party_c")
 INFORMED_PARTY = PartyConfig(WALLET_NAME, WALLET_PASS, "informed_party")
 
 
 class ConfigurableMarketManager(StateAgentWithWallet):
     def __init__(
         self,
-        proposal_wallet_name: str,
-        proposal_wallet_pass: str,
-        termination_wallet_name: str,
-        termination_wallet_pass: str,
+        proposal_key_name: str,
+        termination_key_name: str,
         market_name: str,
         market_code: str,
         asset_name: str,
         asset_dp: int,
-        proposal_key_name: Optional[str] = None,
-        termination_key_name: Optional[str] = None,
+        proposal_wallet_name: Optional[str] = None,
+        termination_wallet_name: Optional[str] = None,
         market_config: Optional[MarketConfig] = None,
         tag: Optional[str] = None,
         settlement_price: Optional[float] = None,
         initial_mint: Optional[float] = 1e9,
     ):
         super().__init__(
             wallet_name=proposal_wallet_name,
-            wallet_pass=proposal_wallet_pass,
             key_name=proposal_key_name,
             tag=tag,
         )
 
         self.termination_wallet_name = termination_wallet_name
-        self.termination_wallet_pass = termination_wallet_pass
         self.termination_key_name = termination_key_name
 
         self.market_name = market_name
         self.market_code = market_code
 
         self.asset_dp = asset_dp
         self.asset_name = asset_name
@@ -65,50 +61,52 @@
         )
 
         self.settlement_price = settlement_price
 
     def initialise(
         self,
         vega: Union[VegaServiceNull, VegaServiceNetwork],
-        create_wallet: bool = True,
-        mint_wallet: bool = True,
+        create_key: bool = True,
+        mint_key: bool = True,
     ):
-        super().initialise(vega=vega, create_wallet=create_wallet)
-        if create_wallet:
-            self.vega.create_wallet(
-                self.termination_wallet_name,
-                self.termination_wallet_pass,
-                self.termination_key_name,
+        super().initialise(vega=vega, create_key=create_key)
+        if create_key:
+            self.vega.create_key(
+                wallet_name=self.termination_wallet_name,
+                name=self.termination_key_name,
             )
 
         self.vega.wait_for_total_catchup()
-        if mint_wallet:
+        if mint_key:
             self.vega.mint(
-                self.wallet_name, asset="VOTE", amount=1e4, key_name=self.key_name
+                wallet_name=self.wallet_name,
+                asset="VOTE",
+                amount=1e4,
+                key_name=self.key_name,
             )
 
         self.vega.wait_for_total_catchup()
 
         if self.vega.find_asset_id(symbol=self.asset_name) is None:
             self.vega.create_asset(
-                self.wallet_name,
+                wallet_name=self.wallet_name,
                 name=self.asset_name,
                 symbol=self.asset_name,
                 decimals=self.asset_dp,
                 max_faucet_amount=5e10,
                 key_name=self.key_name,
             )
 
         self.vega.wait_for_total_catchup()
         self.asset_id = self.vega.find_asset_id(symbol=self.asset_name)
 
         self.vega.wait_for_total_catchup()
-        if mint_wallet:
+        if mint_key:
             self.vega.mint(
-                self.wallet_name,
+                wallet_name=self.wallet_name,
                 asset=self.asset_id,
                 amount=self.initial_mint,
                 key_name=self.key_name,
             )
 
         if self.vega.find_market_id(name=self.market_name) is None:
             # Add market information and asset information to market config
@@ -118,15 +116,16 @@
             self.market_config.set("instrument.future.quote_name", self.asset_name)
             self.market_config.set(
                 "instrument.future.number_decimal_places", self.asset_dp
             )
             self.market_config.set(
                 "instrument.future.terminating_key",
                 self.vega.wallet.public_key(
-                    self.termination_wallet_name, self.termination_key_name
+                    wallet_name=self.termination_wallet_name,
+                    name=self.termination_key_name,
                 ),
             )
 
             self.vega.wait_for_total_catchup()
             self.vega.create_market_from_config(
                 proposal_wallet_name=self.wallet_name,
                 proposal_key_name=self.key_name,
@@ -135,13 +134,13 @@
 
         self.vega.wait_for_total_catchup()
         self.market_id = self.vega.find_market_id(name=self.market_name)
 
     def finalise(self):
         if self.settlement_price is not None:
             self.vega.settle_market(
-                self.termination_wallet_name,
+                self.termination_key_name,
                 self.settlement_price,
                 self.market_id,
-                self.termination_key_name,
+                self.termination_wallet_name,
             )
             self.vega.wait_for_total_catchup()
```

### Comparing `vega_sim-0.67.0/vega_sim/scenario/configurable_market/scenario.py` & `vega_sim-1.0.1/vega_sim/scenario/configurable_market/scenario.py`

 * *Files 5% similar despite different names*

```diff
@@ -112,30 +112,27 @@
             self.price_process_fn()
             if self.price_process_fn is not None
             else self._generate_price_process(random_state=random_state)
         )
 
         market_manager = ConfigurableMarketManager(
             proposal_wallet_name=PROPOSAL_PARTY.wallet_name,
-            proposal_wallet_pass=PROPOSAL_PARTY.wallet_pass,
             proposal_key_name=PROPOSAL_PARTY.key_name,
             termination_wallet_name=TERMINATION_PARTY.wallet_name,
-            termination_wallet_pass=TERMINATION_PARTY.wallet_pass,
             termination_key_name=TERMINATION_PARTY.key_name,
             market_config=market_config,
             market_name=market_name,
             market_code=self.market_code,
             asset_dp=self.asset_decimal,
             asset_name=asset_name,
             settlement_price=price_process[-1] if self.settle_at_end else None,
         )
 
         shaped_mm = ExponentialShapedMarketMaker(
             wallet_name=MAKER_PARTY.wallet_name,
-            wallet_pass=MAKER_PARTY.wallet_pass,
             key_name=MAKER_PARTY.key_name,
             price_process_generator=iter(price_process),
             initial_asset_mint=1e9,
             commitment_amount=1e6,
             market_name=market_name,
             asset_name=asset_name,
             market_decimal_places=market_config.decimal_places,
@@ -149,86 +146,80 @@
             market_kappa=1,
             market_order_arrival_rate=10,
             state_update_freq=10,
         )
 
         sensitive_mo_trader_a = PriceSensitiveMarketOrderTrader(
             wallet_name=SENSITIVE_PARTY_A.wallet_name,
-            wallet_pass=SENSITIVE_PARTY_A.wallet_pass,
             key_name=SENSITIVE_PARTY_A.key_name,
             market_name=market_name,
             asset_name=asset_name,
             initial_asset_mint=1e10,
             buy_intensity=1,
             sell_intensity=1,
             price_half_life=10,
             price_process_generator=iter(price_process),
             base_order_size=1,
             tag="a",
         )
 
         sensitive_mo_trader_b = PriceSensitiveMarketOrderTrader(
             wallet_name=SENSITIVE_PARTY_B.wallet_name,
-            wallet_pass=SENSITIVE_PARTY_B.wallet_pass,
             key_name=SENSITIVE_PARTY_B.key_name,
             market_name=market_name,
             asset_name=asset_name,
             initial_asset_mint=1e10,
             buy_intensity=10,
             sell_intensity=10,
             price_half_life=1,
             price_process_generator=iter(price_process),
             base_order_size=1,
             tag="b",
         )
 
         sensitive_mo_trader_c = PriceSensitiveMarketOrderTrader(
             wallet_name=SENSITIVE_PARTY_C.wallet_name,
-            wallet_pass=SENSITIVE_PARTY_C.wallet_pass,
             key_name=SENSITIVE_PARTY_C.key_name,
             market_name=market_name,
             asset_name=asset_name,
             initial_asset_mint=1e10,
             buy_intensity=100,
             sell_intensity=100,
             price_half_life=0.1,
             price_process_generator=iter(price_process),
             base_order_size=1,
             tag="c",
         )
 
         auctionpass1 = OpenAuctionPass(
             wallet_name=AUCTION_PARTY_A.wallet_name,
-            wallet_pass=AUCTION_PARTY_A.wallet_pass,
             key_name=AUCTION_PARTY_A.key_name,
             side="SIDE_BUY",
             initial_asset_mint=1e9,
             initial_price=price_process[0],
             market_name=market_name,
             asset_name=asset_name,
             opening_auction_trade_amount=1,
             tag="1",
         )
 
         auctionpass2 = OpenAuctionPass(
             wallet_name=AUCTION_PARTY_B.wallet_name,
-            wallet_pass=AUCTION_PARTY_B.wallet_pass,
             key_name=AUCTION_PARTY_B.key_name,
             side="SIDE_SELL",
             initial_asset_mint=1e9,
             initial_price=price_process[0],
             market_name=market_name,
             asset_name=asset_name,
             opening_auction_trade_amount=1,
             tag="2",
         )
 
         info_trader = InformedTrader(
             wallet_name=INFORMED_PARTY.wallet_name,
-            wallet_pass=INFORMED_PARTY.wallet_pass,
             key_name=INFORMED_PARTY.key_name,
             price_process=price_process,
             market_name=market_name,
             asset_name=asset_name,
             initial_asset_mint=1e10,
             proportion_taken=0.1,
         )
```

### Comparing `vega_sim-0.67.0/vega_sim/scenario/curve_market_maker/scenario.py` & `vega_sim-1.0.1/vega_sim/scenario/curve_market_maker/scenario.py`

 * *Files 8% similar despite different names*

```diff
@@ -138,30 +138,27 @@
         )
         self.price_process = price_process
         self.initial_price = (
             self.initial_price if self.initial_price is not None else price_process[0]
         )
 
         market_manager = MarketManager(
-            wallet_name=MM_WALLET.name,
-            wallet_pass=MM_WALLET.passphrase,
-            terminate_wallet_name=TERMINATE_WALLET.name,
-            terminate_wallet_pass=TERMINATE_WALLET.passphrase,
+            key_name=MM_WALLET.name,
+            terminate_key_name=TERMINATE_WALLET.name,
             asset_decimal=self.asset_decimal,
             market_decimal=self.market_decimal,
             market_position_decimal=self.market_position_decimal,
             market_name=market_name,
             asset_name=asset_name,
             tag=str(tag) if tag is not None else None,
             settlement_price=price_process[-1] if self.settle_at_end else None,
         )
 
         shaped_mm = ExponentialShapedMarketMaker(
-            wallet_name="expon",
-            wallet_pass="expon",
+            key_name="expon",
             price_process_generator=iter(price_process),
             initial_asset_mint=self.initial_asset_mint,
             market_name=market_name,
             asset_name=asset_name,
             commitment_amount=self.lp_commitamount,
             market_decimal_places=self.market_decimal,
             asset_decimal_places=self.asset_decimal,
@@ -176,58 +173,54 @@
             running_penalty_parameter=self.phi,
             market_order_arrival_rate=self.buy_intensity,
             market_kappa=self.market_kappa,
             state_update_freq=10,
         )
 
         sensitive_mo_trader = PriceSensitiveMarketOrderTrader(
-            wallet_name=TRADER_WALLET.name,
-            wallet_pass=TRADER_WALLET.passphrase,
+            key_name=TRADER_WALLET.name,
             market_name=market_name,
             asset_name=asset_name,
             initial_asset_mint=self.initial_asset_mint,
             buy_intensity=self.buy_intensity,
             sell_intensity=self.sell_intensity,
             price_half_life=self.sensitive_price_taker_half_life,
             price_process_generator=iter(price_process),
             tag=str(tag) if tag is not None else None,
             base_order_size=self.market_order_trader_base_order_size,
         )
 
         auctionpass1 = OpenAuctionPass(
-            wallet_name=AUCTION1_WALLET.name,
-            wallet_pass=AUCTION1_WALLET.passphrase,
+            key_name=AUCTION1_WALLET.name,
             side="SIDE_BUY",
             initial_asset_mint=self.initial_asset_mint,
             initial_price=self.initial_price
             if self.initial_price is not None
             else price_process[0],
             market_name=market_name,
             asset_name=asset_name,
             opening_auction_trade_amount=self.opening_auction_trade_amount,
             tag=f"1_{tag}",
         )
 
         auctionpass2 = OpenAuctionPass(
-            wallet_name=AUCTION2_WALLET.name,
-            wallet_pass=AUCTION2_WALLET.passphrase,
+            key_name=AUCTION2_WALLET.name,
             side="SIDE_SELL",
             initial_asset_mint=self.initial_asset_mint,
             initial_price=self.initial_price
             if self.initial_price is not None
             else price_process[0],
             market_name=market_name,
             asset_name=asset_name,
             opening_auction_trade_amount=self.opening_auction_trade_amount,
             tag=f"2_{tag}",
         )
 
         info_trader = InformedTrader(
-            wallet_name=INFORMED_WALLET.name,
-            wallet_pass=INFORMED_WALLET.passphrase,
+            key_name=INFORMED_WALLET.name,
             price_process=price_process,
             market_name=market_name,
             asset_name=asset_name,
             initial_asset_mint=self.initial_asset_mint,
             proportion_taken=self.proportion_taken,
             tag=str(tag) if tag is not None else None,
         )
```

### Comparing `vega_sim-0.67.0/vega_sim/scenario/hedged_market_maker/agents.py` & `vega_sim-1.0.1/vega_sim/scenario/hedged_market_maker/agents.py`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/scenario/hedged_market_maker/scenario.py` & `vega_sim-1.0.1/vega_sim/scenario/hedged_market_maker/scenario.py`

 * *Files 5% similar despite different names*

```diff
@@ -140,15 +140,16 @@
             Defaults to 1.0.
         int_it_lookahead (int, optional):
             Number of steps for informed trader to look ahead. Defaults to 30.
         random_agent_ordering (bool, optional):
             Whether to randomly order each agents step action. Defaults to False.
         transactions_per_block (int, optional):
             Number of transactions allowed per block. Defaults to 1000.
-        state_extraction_fn (Optional[ Callable[[VegaServiceNull, List[Agent]], Any] ], optional):
+        state_extraction_fn (Optional[ Callable[[VegaServiceNull, List[Agent]], Any] ]
+            , optional):
             Defines which states to extract and record. Defaults to None.
         pause_every_n_steps (Optional[int], optional):
             Number of steps to simulate before pausing the simulation. Defaults to None.
     """
 
     def __init__(
         self,
@@ -254,47 +255,42 @@
         )
         initial_price = (
             self.initial_price if self.initial_price is not None else price_process[0]
         )
 
         int_market_manager = MarketManager(
             wallet_name=MARKET_CREATOR.wallet_name,
-            wallet_pass=MARKET_CREATOR.wallet_pass,
             key_name=MARKET_CREATOR.key_name,
             terminate_wallet_name=MARKET_SETTLER.wallet_name,
-            terminate_wallet_pass=MARKET_SETTLER.wallet_pass,
             terminate_key_name=MARKET_SETTLER.key_name,
             asset_name=self.asset_name,
             asset_decimal=self.asset_adp,
             market_decimal=self.int_mdp,
             market_position_decimal=self.int_pdp,
             market_name=self.int_name,
             settlement_price=price_process[-1],
             tag="internal",
         )
 
         ext_market_manager = MarketManager(
             wallet_name=MARKET_CREATOR.wallet_name,
-            wallet_pass=MARKET_CREATOR.wallet_pass,
             key_name=MARKET_CREATOR.key_name,
             terminate_wallet_name=MARKET_SETTLER.wallet_name,
-            terminate_wallet_pass=MARKET_SETTLER.wallet_pass,
             terminate_key_name=MARKET_SETTLER.key_name,
             asset_name=self.asset_name,
             asset_decimal=self.asset_adp,
             market_decimal=self.ext_mdp,
             market_position_decimal=self.ext_pdp,
             market_name=self.ext_name,
             settlement_price=price_process[-1],
             tag="external",
         )
 
         int_market_maker = HedgedMarketMaker(
             wallet_name=INT_MARKET_MAKER_KEY_A.wallet_name,
-            wallet_pass=INT_MARKET_MAKER_KEY_A.wallet_pass,
             key_name=INT_MARKET_MAKER_KEY_A.key_name,
             external_key_name=INT_MARKET_MAKER_KEY_B.key_name,
             price_process_generator=iter(price_process),
             internal_key_mint=self.int_mm_int_key_mint,
             external_key_mint=self.int_mm_ext_key_mint,
             commitment_amount=self.int_mm_commitment_amount,
             asset_name=self.asset_name,
@@ -315,15 +311,14 @@
             internal_delay=self.int_lock,
             external_delay=self.ext_lock,
             tag="internal",
         )
 
         ext_market_maker = ExponentialShapedMarketMaker(
             wallet_name=EXT_MARKET_MAKER.wallet_name,
-            wallet_pass=EXT_MARKET_MAKER.wallet_pass,
             key_name=EXT_MARKET_MAKER.key_name,
             price_process_generator=iter(price_process),
             initial_asset_mint=1e10,
             commitment_amount=1e6,
             asset_name=self.asset_name,
             asset_decimal_places=self.asset_adp,
             market_name=self.ext_name,
@@ -338,89 +333,82 @@
             state_update_freq=60,
             fee_amount=1e-03,
             tag="external",
         )
 
         int_auction_pass_bid = OpenAuctionPass(
             wallet_name=AUCTION_PASS_BID.wallet_name,
-            wallet_pass=AUCTION_PASS_BID.wallet_pass,
             key_name=AUCTION_PASS_BID.key_name,
             side="SIDE_BUY",
             initial_asset_mint=1e10,
             initial_price=initial_price,
             market_name=self.int_name,
             asset_name=self.asset_name,
             opening_auction_trade_amount=self.int_pdp,
             tag="internal_bid",
         )
         int_auction_pass_ask = OpenAuctionPass(
             wallet_name=AUCTION_PASS_ASK.wallet_name,
-            wallet_pass=AUCTION_PASS_ASK.wallet_pass,
             key_name=AUCTION_PASS_ASK.key_name,
             side="SIDE_SELL",
             initial_asset_mint=1e10,
             initial_price=initial_price,
             market_name=self.int_name,
             asset_name=self.asset_name,
             opening_auction_trade_amount=self.int_pdp,
             tag="internal_ask",
         )
         ext_auction_pass_bid = OpenAuctionPass(
             wallet_name=AUCTION_PASS_BID.wallet_name,
-            wallet_pass=AUCTION_PASS_BID.wallet_pass,
             key_name=AUCTION_PASS_BID.key_name,
             side="SIDE_BUY",
             initial_asset_mint=1e10,
             initial_price=initial_price,
             market_name=self.ext_name,
             asset_name=self.asset_name,
             opening_auction_trade_amount=self.ext_pdp,
             tag="external_bid",
         )
         ext_auction_pass_ask = OpenAuctionPass(
             wallet_name=AUCTION_PASS_ASK.wallet_name,
-            wallet_pass=AUCTION_PASS_ASK.wallet_pass,
             key_name=AUCTION_PASS_ASK.key_name,
             side="SIDE_SELL",
             initial_asset_mint=1e10,
             initial_price=initial_price,
             market_name=self.ext_name,
             asset_name=self.asset_name,
             opening_auction_trade_amount=self.ext_pdp,
             tag="external_bid",
         )
 
         int_random_trader = MarketOrderTrader(
             wallet_name=INT_RANDOM_TRADER.wallet_name,
-            wallet_pass=INT_RANDOM_TRADER.wallet_pass,
             key_name=INT_RANDOM_TRADER.key_name,
             market_name=self.int_name,
             asset_name=self.asset_name,
             initial_asset_mint=1e10,
             buy_intensity=1 * 10 ** (self.int_pdp),
             sell_intensity=1 * 10 ** (self.int_pdp),
             base_order_size=1 * 10 ** -(self.int_pdp),
             tag="internal",
         )
         ext_random_trader = MarketOrderTrader(
             wallet_name=EXT_RANDOM_TRADER.wallet_name,
-            wallet_pass=EXT_RANDOM_TRADER.wallet_pass,
             key_name=EXT_RANDOM_TRADER.key_name,
             market_name=self.ext_name,
             asset_name=self.asset_name,
             initial_asset_mint=1e10,
             buy_intensity=1 * 10 ** (self.ext_pdp),
             sell_intensity=1 * 10 ** (self.ext_pdp),
             base_order_size=1 * 10 ** -(self.ext_pdp),
             tag="external",
         )
 
         int_informed_trader = InformedTrader(
             wallet_name=INT_INFORMED_TRADER.wallet_name,
-            wallet_pass=INT_INFORMED_TRADER.wallet_pass,
             key_name=INT_INFORMED_TRADER.key_name,
             asset_name=self.asset_name,
             market_name=self.int_name,
             initial_asset_mint=1e10,
             proportion_taken=self.int_it_proportion,
             price_process=price_process,
             accuracy=self.int_it_accuracy,
```

### Comparing `vega_sim-0.67.0/vega_sim/scenario/ideal_market_maker/agents.py` & `vega_sim-1.0.1/vega_sim/scenario/ideal_market_maker/agents.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         self.vega.settle_market(
             self.terminate_wallet_name, self.settlement_price, self.market_id
         )
 
     def initialise(self, vega: VegaServiceNull):
         # Initialise wallet for LP/ Settle Party
         super().initialise(vega=vega)
-        self.vega.create_wallet(self.terminate_wallet_name, self.terminate_wallet_pass)
+        self.vega.create_key(self.terminate_wallet_name)
 
         # Faucet vega tokens
         self.vega.wait_for_datanode_sync()
         self.vega.mint(
             self.wallet_name,
             asset="VOTE",
             amount=1e4,
```

### Comparing `vega_sim-0.67.0/vega_sim/scenario/ideal_market_maker/environments.py` & `vega_sim-1.0.1/vega_sim/scenario/ideal_market_maker/environments.py`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/scenario/ideal_market_maker/scenario.py` & `vega_sim-1.0.1/vega_sim/scenario/ideal_market_maker/scenario.py`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/scenario/ideal_market_maker/utils/log_data.py` & `vega_sim-1.0.1/vega_sim/scenario/ideal_market_maker/utils/log_data.py`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/scenario/ideal_market_maker/utils/strategy.py` & `vega_sim-1.0.1/vega_sim/scenario/ideal_market_maker/utils/strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     q_upper: int,
     q_lower: int,
     kappa: int,
     Lambda: int,
     alpha: float,
     phi: float,
 ):
-
     """
     Simulate an Market Making Model and output the optimal strategy
       of posting bid/ask depth based on market parameters.
 
     Args:
         T:
             int, total simulation time
```

### Comparing `vega_sim-0.67.0/vega_sim/scenario/ideal_market_maker_v2/agents.py` & `vega_sim-1.0.1/vega_sim/scenario/ideal_market_maker_v2/agents.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,18 +41,16 @@
 
 
 class OptimalMarketMaker(StateAgentWithWallet):
     NAME_BASE = "optimal_mm"
 
     def __init__(
         self,
-        wallet_name: str,
-        wallet_pass: str,
-        terminate_wallet_name: str,
-        terminate_wallet_pass: str,
+        key_name: str,
+        terminate_key_name: str,
         price_process: List[float],
         initial_asset_mint: float = 1000000,
         spread: float = 0.002,
         num_steps: int = 180,
         limit_order_size: float = 10,
         market_order_arrival_rate: float = 5,
         kappa: float = 500,
@@ -65,21 +63,18 @@
         market_position_decimal: int = 2,
         market_name: str = None,
         asset_name: str = None,
         set_up_market: bool = True,
         commitment_amount: float = 6000,
         settlement_price: Optional[float] = None,
         tag: str = "",
-        key_name: Optional[str] = None,
+        wallet_name: Optional[str] = None,
     ):
-        super().__init__(
-            wallet_name=wallet_name, wallet_pass=wallet_pass, key_name=key_name, tag=tag
-        )
-        self.terminate_wallet_name = terminate_wallet_name
-        self.terminate_wallet_pass = terminate_wallet_pass
+        super().__init__(wallet_name=wallet_name, key_name=key_name, tag=tag)
+        self.terminate_key_name = terminate_key_name
 
         self.price_process = price_process
         self.spread = spread
         self.time = num_steps
         self.Lambda = market_order_arrival_rate
         self.kappa = kappa
         self.limit_order_size = limit_order_size
@@ -128,68 +123,72 @@
                 alpha=self.alpha,
                 phi=self.phi,
             )
 
     def finalise(self):
         if self.settlement_price:
             self.vega.settle_market(
-                self.terminate_wallet_name, self.settlement_price, self.market_id
+                self.terminate_key_name,
+                self.settlement_price,
+                self.market_id,
+                wallet_name=self.wallet_name,
             )
             self.current_step += 1
 
     def initialise(self, vega: VegaServiceNull):
         # Initialise wallet for LP/ Settle Party
         super().initialise(vega=vega)
-        self.vega.create_wallet(self.terminate_wallet_name, self.terminate_wallet_pass)
+        self.vega.create_key(self.terminate_key_name, self.wallet_name)
 
         # Faucet vega tokens
         self.vega.wait_fn(10)
         self.vega.wait_for_total_catchup()
         self.vega.mint(
-            self.wallet_name,
+            wallet_name=self.wallet_name,
             asset="VOTE",
             amount=1e4,
             key_name=self.key_name,
         )
         self.vega.wait_fn(10)
         self.vega.wait_for_total_catchup()
         if self.set_up_market:
             # Create asset
             self.vega.create_asset(
-                self.wallet_name,
+                wallet_name=self.wallet_name,
                 name=self.asset_name,
                 symbol=self.asset_name,
                 decimals=self.adp,
                 key_name=self.key_name,
             )
             self.vega.wait_fn(5)
             self.vega.wait_for_total_catchup()
         # Get asset id
         self.asset_id = self.vega.find_asset_id(symbol=self.asset_name)
         # Top up asset
         self.vega.mint(
-            self.wallet_name,
+            wallet_name=self.wallet_name,
             asset=self.asset_id,
             amount=self.initial_asset_mint,
             key_name=self.key_name,
         )
         self.vega.wait_fn(10)
         self.vega.wait_for_total_catchup()
 
         if self.set_up_market:
             # Set up a future market
             self.vega.create_simple_market(
                 market_name=self.market_name,
-                proposal_wallet=self.wallet_name,
+                wallet_name=self.wallet_name,
                 settlement_asset_id=self.asset_id,
-                termination_wallet=self.terminate_wallet_name,
+                termination_key=self.terminate_key_name,
+                termination_wallet_name=self.wallet_name,
                 market_decimals=self.mdp,
                 position_decimals=self.market_position_decimal,
                 future_asset=self.asset_name,
-                key_name=self.key_name,
+                proposal_key=self.key_name,
             )
             self.vega.wait_for_total_catchup()
 
         # Get market id
         self.market_id = self.vega.find_market_id(name=self.market_name)
 
         vega.submit_liquidity(
@@ -315,19 +314,19 @@
                 market_id=self.market_id,
                 pegged_order=PeggedOrder(reference=reference, offset=offset),
                 side=side,
                 volume=volume,
                 order_type=vega_protos.Order.Type.TYPE_LIMIT,
                 wait=False,
                 time_in_force=vega_protos.Order.TimeInForce.TIME_IN_FORCE_GTC,
-                key_name=self.key_name,
+                trading_key=self.key_name,
             )
         else:
             self.vega.amend_order(
                 trading_wallet=self.wallet_name,
                 market_id=self.market_id,
                 order_id=order.id,
                 pegged_reference=reference,
                 pegged_offset=offset,
                 volume_delta=volume - order.size,
-                key_name=self.key_name,
+                trading_key=self.key_name,
             )
```

### Comparing `vega_sim-0.67.0/vega_sim/scenario/ideal_market_maker_v2/scenario.py` & `vega_sim-1.0.1/vega_sim/scenario/ideal_market_maker_v2/scenario.py`

 * *Files 5% similar despite different names*

```diff
@@ -125,18 +125,16 @@
             self.price_process_fn()
             if self.price_process_fn is not None
             else self._generate_price_process(random_state=random_state)
         )
         self.price_process = price_process
 
         market_maker = OptimalMarketMaker(
-            wallet_name=MM_WALLET.name,
-            wallet_pass=MM_WALLET.passphrase,
-            terminate_wallet_name=TERMINATE_WALLET.name,
-            terminate_wallet_pass=TERMINATE_WALLET.passphrase,
+            key_name=MM_WALLET.name,
+            terminate_key_name=TERMINATE_WALLET.name,
             initial_asset_mint=self.initial_asset_mint,
             price_process=price_process,
             spread=self.spread,
             num_steps=self.num_steps,
             market_order_arrival_rate=self.buy_intensity,
             kappa=self.kappa,
             limit_order_size=self.market_marker_limit_order_size,
@@ -151,72 +149,67 @@
             asset_name=asset_name,
             commitment_amount=self.lp_commitamount,
             tag=str(tag),
             settlement_price=price_process[-1] if self.settle_at_end else None,
         )
 
         trader = MarketOrderTrader(
-            wallet_name=TRADER_WALLET.name,
-            wallet_pass=TRADER_WALLET.passphrase,
+            key_name=TRADER_WALLET.name,
             initial_asset_mint=self.initial_asset_mint,
             market_name=market_name,
             asset_name=asset_name,
             tag=str(tag),
             buy_intensity=self.buy_intensity,
             sell_intensity=self.sell_intensity,
             random_state=random_state,
             base_order_size=self.market_order_trader_base_order_size,
         )
 
         background_market = BackgroundMarket(
-            wallet_name=BACKGROUND_MARKET.name,
-            wallet_pass=BACKGROUND_MARKET.passphrase,
+            key_name=BACKGROUND_MARKET.name,
             market_name=market_name,
             asset_name=asset_name,
             initial_asset_mint=self.initial_asset_mint,
             price_process=price_process,
             spread=self.spread,
             tick_spacing=self.backgroundmarket_tick_spacing,
             order_distribution_kappa=self.kappa,
             num_levels_per_side=self.backgroundmarket_number_levels_per_side,
             tag=str(tag),
             position_decimals=self.market_position_decimal,
         )
 
         auctionpass1 = OpenAuctionPass(
-            wallet_name=AUCTION1_WALLET.name,
-            wallet_pass=AUCTION1_WALLET.passphrase,
+            key_name=AUCTION1_WALLET.name,
             side="SIDE_BUY",
             initial_asset_mint=self.initial_asset_mint,
             initial_price=self.initial_price
             if self.initial_price is not None
             else price_process[0],
             market_name=market_name,
             asset_name=asset_name,
             opening_auction_trade_amount=self.opening_auction_trade_amount,
             tag=f"1_{tag}",
         )
 
         auctionpass2 = OpenAuctionPass(
-            wallet_name=AUCTION2_WALLET.name,
-            wallet_pass=AUCTION2_WALLET.passphrase,
+            key_name=AUCTION2_WALLET.name,
             side="SIDE_SELL",
             initial_asset_mint=self.initial_asset_mint,
             initial_price=self.initial_price
             if self.initial_price is not None
             else price_process[0],
             market_name=market_name,
             asset_name=asset_name,
             opening_auction_trade_amount=self.opening_auction_trade_amount,
             tag=f"2_{tag}",
         )
 
         # info_trader = InformedTrader(
-        #     wallet_name=INFORMED_WALLET.name,
-        #     wallet_pass=INFORMED_WALLET.passphrase,
+        #     key_name=INFORMED_WALLET.name,
         #     price_process=price_process,
         #     market_name=market_name,
         #     asset_name=asset_name,
         #     initial_asset_mint=self.initial_asset_mint,
         #     proportion_taken=self.proportion_taken,
         #     tag=str(tag),
         # )
```

### Comparing `vega_sim-0.67.0/vega_sim/scenario/ideal_market_maker_v2/utils/strategy.py` & `vega_sim-1.0.1/vega_sim/scenario/ideal_market_maker_v2/utils/strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     q_upper: int,
     q_lower: int,
     kappa: int,
     Lambda: int,
     alpha: float,
     phi: float,
 ):
-
     """
     Simulate an Market Making Model and output the optimal strategy
       of posting bid/ask depth based on market parameters.
 
     Args:
         T:
             int, total simulation time
```

### Comparing `vega_sim-0.67.0/vega_sim/scenario/market_crash/price_process.py` & `vega_sim-1.0.1/vega_sim/scenario/market_crash/price_process.py`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/scenario/market_crash/scenario.py` & `vega_sim-1.0.1/vega_sim/scenario/market_crash/scenario.py`

 * *Files 10% similar despite different names*

```diff
@@ -129,18 +129,16 @@
         self.price_process = (
             self.price_process_fn()
             if self.price_process_fn is not None
             else self._generate_price_process()
         )
 
         market_maker = MarketManager(
-            wallet_name=MM_WALLET.name,
-            wallet_pass=MM_WALLET.passphrase,
-            terminate_wallet_name=TERMINATE_WALLET.name,
-            terminate_wallet_pass=TERMINATE_WALLET.passphrase,
+            key_name=MM_WALLET.name,
+            terminate_key_name=TERMINATE_WALLET.name,
             asset_decimal=self.asset_decimal,
             market_decimal=self.market_decimal,
             commitment_amount=60000,
             settlement_price=self.price_process[-1] if self.settle_at_end else None,
             market_name=self.market_name,
             asset_name=self.asset_name,
             tag=str(tag),
@@ -148,45 +146,40 @@
 
         position_traders = []
         noise_traders = []
 
         for i in range(self.num_noise_traders):
             noise_traders.append(
                 MarketOrderTrader(
-                    wallet_name=TRADER_WALLET.name,
-                    wallet_pass=TRADER_WALLET.passphrase,
                     market_name=self.market_name,
                     asset_name=self.asset_name,
                     tag=f"{tag}_noise_{i}",
                     initial_asset_mint=self.position_taker_mint,
                     buy_intensity=self.noise_buy_intensity,
                     sell_intensity=self.noise_sell_intensity,
                     random_state=random_state,
                     key_name=f"{tag}_noise_{i}",
                 )
             )
         for i in range(self.num_position_traders):
             position_traders.append(
                 MarketOrderTrader(
-                    wallet_name=TRADER_WALLET.name,
-                    wallet_pass=TRADER_WALLET.passphrase,
                     market_name=self.market_name,
                     asset_name=self.asset_name,
                     initial_asset_mint=self.position_taker_mint,
                     tag=f"{tag}_pos_{i}",
                     buy_intensity=self.position_taker_buy_intensity,
                     sell_intensity=self.position_taker_sell_intensity,
                     random_state=random_state,
                     key_name=f"{tag}_pos_{i}",
                 )
             )
 
         background_market = MultiRegimeBackgroundMarket(
-            wallet_name=BACKGROUND_MARKET.name,
-            wallet_pass=BACKGROUND_MARKET.passphrase,
+            key_name=BACKGROUND_MARKET.name,
             market_name=self.market_name,
             asset_name=self.asset_name,
             market_regimes=[
                 MarketRegime(
                     spread=self.spread,
                     tick_spacing=0.1,
                     num_levels_per_side=25,
@@ -198,27 +191,25 @@
                 )
             ],
             price_process=self.price_process,
             tag=str(tag),
         )
 
         auctionpass1 = OpenAuctionPass(
-            wallet_name=AUCTION1_WALLET.name,
-            wallet_pass=AUCTION1_WALLET.passphrase,
+            key_name=AUCTION1_WALLET.name,
             side="SIDE_BUY",
             initial_price=self.initial_price,
             market_name=self.market_name,
             asset_name=self.asset_name,
             initial_asset_mint=self.initial_asset_mint,
             tag=f"1_{tag}",
         )
 
         auctionpass2 = OpenAuctionPass(
-            wallet_name=AUCTION2_WALLET.name,
-            wallet_pass=AUCTION2_WALLET.passphrase,
+            key_name=AUCTION2_WALLET.name,
             side="SIDE_SELL",
             initial_price=self.initial_price,
             market_name=self.market_name,
             asset_name=self.asset_name,
             initial_asset_mint=self.initial_asset_mint,
             tag=f"2_{tag}",
         )
```

### Comparing `vega_sim-0.67.0/vega_sim/scenario/multi_market/agents.py` & `vega_sim-1.0.1/vega_sim/scenario/multi_market/agents.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,44 +3,44 @@
 File contains the party config tuples for each agent in the MultiMarket scenario. The
 scenario runs a network with three markets each with a configurable number of market
 order trader agents.
 
 """
 from collections import namedtuple
 
-PartyConfig = namedtuple("AgentConfig", ["wallet_name", "wallet_pass", "key_name"])
+PartyConfig = namedtuple("AgentConfig", ["wallet_name", "key_name"])
 
 # Set-up wallets and keys for MarketManager agents
 MARKET_MANAGERS = {
-    "MARKET_A_CREATOR": PartyConfig("market_managers", "pass", "Market A Creator"),
-    "MARKET_A_SETTLER": PartyConfig("market_managers", "pass", "Market A Settler"),
-    "MARKET_B_CREATOR": PartyConfig("market_managers", "pass", "Market B Creator"),
-    "MARKET_B_SETTLER": PartyConfig("market_managers", "pass", "Market B Settler"),
-    "MARKET_C_CREATOR": PartyConfig("market_managers", "pass", "Market C Creator"),
-    "MARKET_C_SETTLER": PartyConfig("market_managers", "pass", "Market C Settler"),
+    "MARKET_A_CREATOR": PartyConfig("market_managers", "Market A Creator"),
+    "MARKET_A_SETTLER": PartyConfig("market_managers", "Market A Settler"),
+    "MARKET_B_CREATOR": PartyConfig("market_managers", "Market B Creator"),
+    "MARKET_B_SETTLER": PartyConfig("market_managers", "Market B Settler"),
+    "MARKET_C_CREATOR": PartyConfig("market_managers", "Market C Creator"),
+    "MARKET_C_SETTLER": PartyConfig("market_managers", "Market C Settler"),
 }
 
 # Set-up wallets and keys for CurvedMarketMaker agents
 MARKET_MAKERS = {
-    "MARKET_A_MAKER": PartyConfig("market_makers", "pass", "Market A Maker"),
-    "MARKET_B_MAKER": PartyConfig("market_makers", "pass", "Market B Maker"),
-    "MARKET_C_MAKER": PartyConfig("market_makers", "pass", "Market C Maker"),
+    "MARKET_A_MAKER": PartyConfig("market_makers", "Market A Maker"),
+    "MARKET_B_MAKER": PartyConfig("market_makers", "Market B Maker"),
+    "MARKET_C_MAKER": PartyConfig("market_makers", "Market C Maker"),
 }
 
 # Set-up wallets and keys for AuctionPass agents
 MARKET_PASSERS = {
-    "MARKET_A_PASSER_BID": PartyConfig("market_passers", "pass", "Market A Passer Bid"),
-    "MARKET_A_PASSER_ASK": PartyConfig("market_passers", "pass", "Market A Passer Ask"),
-    "MARKET_B_PASSER_BID": PartyConfig("market_passers", "pass", "Market B Passer Bid"),
-    "MARKET_B_PASSER_ASK": PartyConfig("market_passers", "pass", "Market B Passer Ask"),
-    "MARKET_C_PASSER_BID": PartyConfig("market_passers", "pass", "Market C Passer Bid"),
-    "MARKET_C_PASSER_ASK": PartyConfig("market_passers", "pass", "Market C Passer Ask"),
+    "MARKET_A_PASSER_BID": PartyConfig("market_passers", "Market A Passer Bid"),
+    "MARKET_A_PASSER_ASK": PartyConfig("market_passers", "Market A Passer Ask"),
+    "MARKET_B_PASSER_BID": PartyConfig("market_passers", "Market B Passer Bid"),
+    "MARKET_B_PASSER_ASK": PartyConfig("market_passers", "Market B Passer Ask"),
+    "MARKET_C_PASSER_BID": PartyConfig("market_passers", "Market C Passer Bid"),
+    "MARKET_C_PASSER_ASK": PartyConfig("market_passers", "Market C Passer Ask"),
 }
 
 # Set-up wallets and keys for MarketOrderTrader agents
 MARKET_TRADERS = {
     f"MARKET_{i}_TRADER_{str(k).zfill(4)}": PartyConfig(
-        "market_traders", "pass", f"Market {i} Trader {str(k).zfill(4)}"
+        "market_traders", f"Market {i} Trader {str(k).zfill(4)}"
     )
     for i in ["A", "B", "C"]
     for k in range(1000)
 }
```

### Comparing `vega_sim-0.67.0/vega_sim/scenario/multi_market/scenario.py` & `vega_sim-1.0.1/vega_sim/scenario/multi_market/scenario.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,15 +43,14 @@
     Granularity,
     get_historic_price_series,
 )
 
 from vega_sim.scenario.scenario import Scenario
 from vega_sim.environment.environment import MarketEnvironmentWithState
 from vega_sim.null_service import VegaServiceNull
-from vega_sim.scenario.constants import Network
 from vega_sim.scenario.multi_market.agents import (
     MARKET_MANAGERS,
     MARKET_MAKERS,
     MARKET_PASSERS,
     MARKET_TRADERS,
 )
 from vega_sim.scenario.common.agents import (
@@ -95,16 +94,17 @@
     "adp": 5,
 }
 
 
 class VegaLoadTest(Scenario):
     def __init__(
         self,
-        num_steps: int = 60 * 3,
-        granularity: Granularity = Granularity.MINUTE,
+        num_steps: int = 60 * 24 * 30 * 3,
+        granularity: Granularity = Granularity.HOUR,
+        step_length_seconds: float = 60,
         transactions_per_block: int = 4096,
         block_length_seconds: float = 1,
         parties_per_market: int = 1000,
         orders_per_second: int = 100,
         trades_per_second: int = 1,
         start_date: str = None,
         market_a_args: Optional[dict] = None,
@@ -113,14 +113,20 @@
         initial_asset_mint=1e9,
         price_process_fn: Optional[Callable] = None,
     ):
         super().__init__()
 
         self.num_steps = num_steps
         self.granularity = granularity
+        self.step_length_seconds = step_length_seconds
+        self.interpolation = (
+            f"{step_length_seconds}S"
+            if step_length_seconds < granularity.value
+            else None
+        )
 
         self.block_length_seconds = block_length_seconds
         self.transactions_per_block = transactions_per_block
 
         self.start_date = start_date if start_date is not None else START_DATE
 
         self.market_a_args = (
@@ -146,212 +152,204 @@
             trades_per_second / self.num_mo_traders_per_market
         ) * self.granularity.value
 
         self.price_process_fn = price_process_fn
 
     def _generate_price_process(self, asset: str) -> list:
         start = datetime.strptime(self.start_date, "%Y-%m-%d %H:%M:%S")
-        end = start + timedelta(seconds=self.num_steps * self.granularity.value)
+        end = start + timedelta(seconds=self.num_steps * self.step_length_seconds)
 
         price_process = get_historic_price_series(
             product_id=asset,
             granularity=self.granularity,
             start=str(start),
             end=str(end),
+            interpolation=self.interpolation,
         )
 
         return list(price_process)
 
     def configure_agents(
         self,
         vega: VegaServiceNull,
         tag: str,
         random_state: Optional[np.random.RandomState],
         **kwargs,
     ) -> List[StateAgent]:
+        logging.info(f"Downloading historical data for Market A.")
         market_a_price_process = (
             self.price_process_fn()
             if self.price_process_fn is not None
             else self._generate_price_process(asset=self.market_a_args["oracle"])
         )
+        logging.info(f"Downloading historical data for Market B.")
         market_b_price_process = (
             self.price_process_fn()
             if self.price_process_fn is not None
-            else self._generate_price_process(asset=self.market_a_args["oracle"])
+            else self._generate_price_process(asset=self.market_b_args["oracle"])
         )
+        logging.info(f"Downloading historical data for Market C.")
         market_c_price_process = (
             self.price_process_fn()
             if self.price_process_fn is not None
-            else self._generate_price_process(asset=self.market_a_args["oracle"])
+            else self._generate_price_process(asset=self.market_c_args["oracle"])
         )
 
         # Create MarketManager agents
         market_a_manager = MarketManager(
             wallet_name=MARKET_MANAGERS["MARKET_A_CREATOR"].wallet_name,
-            wallet_pass=MARKET_MANAGERS["MARKET_A_CREATOR"].wallet_name,
             key_name=MARKET_MANAGERS["MARKET_A_CREATOR"].key_name,
             terminate_wallet_name=MARKET_MANAGERS["MARKET_A_SETTLER"].wallet_name,
-            terminate_wallet_pass=MARKET_MANAGERS["MARKET_A_SETTLER"].wallet_name,
             terminate_key_name=MARKET_MANAGERS["MARKET_A_SETTLER"].key_name,
             market_name=self.market_a_args["name"],
             asset_name=self.market_a_args["asset"],
             asset_decimal=self.market_a_args["adp"],
             market_decimal=self.market_a_args["mdp"],
             market_position_decimal=self.market_a_args["pdp"],
             settlement_price=market_a_price_process[-1],
             tag="a",
         )
         market_b_manager = MarketManager(
             wallet_name=MARKET_MANAGERS["MARKET_B_CREATOR"].wallet_name,
-            wallet_pass=MARKET_MANAGERS["MARKET_B_CREATOR"].wallet_name,
             key_name=MARKET_MANAGERS["MARKET_B_CREATOR"].key_name,
             terminate_wallet_name=MARKET_MANAGERS["MARKET_B_SETTLER"].wallet_name,
-            terminate_wallet_pass=MARKET_MANAGERS["MARKET_B_SETTLER"].wallet_name,
             terminate_key_name=MARKET_MANAGERS["MARKET_B_SETTLER"].key_name,
             market_name=self.market_b_args["name"],
             asset_name=self.market_b_args["asset"],
             asset_decimal=self.market_b_args["adp"],
             market_decimal=self.market_b_args["mdp"],
             market_position_decimal=self.market_b_args["pdp"],
             settlement_price=market_b_price_process[-1],
             tag="b",
         )
         market_c_manager = MarketManager(
             wallet_name=MARKET_MANAGERS["MARKET_B_CREATOR"].wallet_name,
-            wallet_pass=MARKET_MANAGERS["MARKET_B_CREATOR"].wallet_name,
             key_name=MARKET_MANAGERS["MARKET_B_CREATOR"].key_name,
             terminate_wallet_name=MARKET_MANAGERS["MARKET_C_SETTLER"].wallet_name,
-            terminate_wallet_pass=MARKET_MANAGERS["MARKET_C_SETTLER"].wallet_name,
             terminate_key_name=MARKET_MANAGERS["MARKET_C_SETTLER"].key_name,
             market_name=self.market_c_args["name"],
             asset_name=self.market_c_args["asset"],
             asset_decimal=self.market_c_args["adp"],
             market_decimal=self.market_c_args["mdp"],
             market_position_decimal=self.market_c_args["pdp"],
             settlement_price=market_c_price_process[-1],
             tag="c",
         )
 
         #  Create ExponentialShapedMarketMaker agents
         market_a_maker = ExponentialShapedMarketMaker(
             wallet_name=MARKET_MAKERS["MARKET_A_MAKER"].wallet_name,
-            wallet_pass=MARKET_MAKERS["MARKET_A_MAKER"].wallet_pass,
             key_name=MARKET_MAKERS["MARKET_A_MAKER"].key_name,
             price_process_generator=iter(market_a_price_process),
             initial_asset_mint=self.initial_asset_mint,
             market_name=self.market_a_args["name"],
             asset_name=self.market_a_args["asset"],
-            commitment_amount=1e9,
+            commitment_amount=1e6,
             market_decimal_places=self.market_a_args["mdp"],
             asset_decimal_places=self.market_a_args["adp"],
             num_steps=self.num_steps,
+            kappa=0.2,
             tick_spacing=1,
             market_kappa=10,
             state_update_freq=10,
             tag="a",
         )
         market_b_maker = ExponentialShapedMarketMaker(
             wallet_name=MARKET_MAKERS["MARKET_B_MAKER"].wallet_name,
-            wallet_pass=MARKET_MAKERS["MARKET_B_MAKER"].wallet_pass,
             key_name=MARKET_MAKERS["MARKET_B_MAKER"].key_name,
             price_process_generator=iter(market_b_price_process),
             initial_asset_mint=self.initial_asset_mint,
             market_name=self.market_b_args["name"],
             asset_name=self.market_b_args["asset"],
-            commitment_amount=1e9,
+            commitment_amount=1e6,
             market_decimal_places=self.market_b_args["mdp"],
             asset_decimal_places=self.market_b_args["adp"],
             num_steps=self.num_steps,
+            kappa=0.2,
             tick_spacing=1,
             market_kappa=10,
             state_update_freq=10,
             tag="b",
         )
         market_c_maker = ExponentialShapedMarketMaker(
             wallet_name=MARKET_MAKERS["MARKET_C_MAKER"].wallet_name,
-            wallet_pass=MARKET_MAKERS["MARKET_C_MAKER"].wallet_pass,
             key_name=MARKET_MAKERS["MARKET_C_MAKER"].key_name,
             price_process_generator=iter(market_c_price_process),
             initial_asset_mint=self.initial_asset_mint,
             market_name=self.market_c_args["name"],
             asset_name=self.market_c_args["asset"],
-            commitment_amount=1e9,
+            commitment_amount=1e6,
             market_decimal_places=self.market_c_args["mdp"],
             asset_decimal_places=self.market_c_args["adp"],
             num_steps=self.num_steps,
+            kappa=0.1,
             tick_spacing=2,
             market_kappa=5,
             state_update_freq=10,
             tag="c",
         )
 
         # Setup agents for passing auction
         market_a_passer_bid = OpenAuctionPass(
             wallet_name=MARKET_PASSERS["MARKET_A_PASSER_BID"].wallet_name,
-            wallet_pass=MARKET_PASSERS["MARKET_A_PASSER_BID"].wallet_pass,
             key_name=MARKET_PASSERS["MARKET_A_PASSER_BID"].key_name,
             side="SIDE_BUY",
             initial_asset_mint=self.initial_asset_mint,
             initial_price=market_a_price_process[0],
             market_name=self.market_a_args["name"],
             asset_name=self.market_a_args["asset"],
             opening_auction_trade_amount=1,
             tag="a_bid",
         )
         market_a_passer_ask = OpenAuctionPass(
             wallet_name=MARKET_PASSERS["MARKET_A_PASSER_ASK"].wallet_name,
-            wallet_pass=MARKET_PASSERS["MARKET_A_PASSER_ASK"].wallet_pass,
             key_name=MARKET_PASSERS["MARKET_A_PASSER_ASK"].key_name,
             side="SIDE_SELL",
             initial_asset_mint=self.initial_asset_mint,
             initial_price=market_a_price_process[0],
             market_name=self.market_a_args["name"],
             asset_name=self.market_a_args["asset"],
             opening_auction_trade_amount=1,
             tag="a_ask",
         )
         market_b_passer_bid = OpenAuctionPass(
             wallet_name=MARKET_PASSERS["MARKET_B_PASSER_BID"].wallet_name,
-            wallet_pass=MARKET_PASSERS["MARKET_B_PASSER_BID"].wallet_pass,
             key_name=MARKET_PASSERS["MARKET_B_PASSER_BID"].key_name,
             side="SIDE_BUY",
             initial_asset_mint=self.initial_asset_mint,
             initial_price=market_b_price_process[0],
             market_name=self.market_b_args["name"],
             asset_name=self.market_b_args["asset"],
             opening_auction_trade_amount=1,
             tag="b_bid",
         )
         market_b_passer_ask = OpenAuctionPass(
             wallet_name=MARKET_PASSERS["MARKET_B_PASSER_ASK"].wallet_name,
-            wallet_pass=MARKET_PASSERS["MARKET_B_PASSER_ASK"].wallet_pass,
             key_name=MARKET_PASSERS["MARKET_B_PASSER_ASK"].key_name,
             side="SIDE_SELL",
             initial_asset_mint=self.initial_asset_mint,
             initial_price=market_b_price_process[0],
             market_name=self.market_b_args["name"],
             asset_name=self.market_b_args["asset"],
             opening_auction_trade_amount=1,
             tag="b_ask",
         )
         market_c_passer_bid = OpenAuctionPass(
             wallet_name=MARKET_PASSERS["MARKET_C_PASSER_BID"].wallet_name,
-            wallet_pass=MARKET_PASSERS["MARKET_C_PASSER_BID"].wallet_pass,
             key_name=MARKET_PASSERS["MARKET_C_PASSER_BID"].key_name,
             side="SIDE_BUY",
             initial_asset_mint=self.initial_asset_mint,
             initial_price=market_c_price_process[0],
             market_name=self.market_c_args["name"],
             asset_name=self.market_c_args["asset"],
             opening_auction_trade_amount=1,
             tag="c_bid",
         )
         market_c_passer_ask = OpenAuctionPass(
             wallet_name=MARKET_PASSERS["MARKET_C_PASSER_ASK"].wallet_name,
-            wallet_pass=MARKET_PASSERS["MARKET_C_PASSER_ASK"].wallet_pass,
             key_name=MARKET_PASSERS["MARKET_C_PASSER_ASK"].key_name,
             side="SIDE_SELL",
             initial_asset_mint=self.initial_asset_mint,
             initial_price=market_c_price_process[0],
             market_name=self.market_c_args["name"],
             asset_name=self.market_c_args["asset"],
             opening_auction_trade_amount=1,
@@ -359,129 +357,111 @@
         )
 
         market_a_lo_traders = [
             LimitOrderTrader(
                 wallet_name=MARKET_TRADERS[
                     f"MARKET_A_TRADER_{str(i).zfill(4)}"
                 ].wallet_name,
-                wallet_pass=MARKET_TRADERS[
-                    f"MARKET_A_TRADER_{str(i).zfill(4)}"
-                ].wallet_pass,
                 key_name=MARKET_TRADERS[f"MARKET_A_TRADER_{str(i).zfill(4)}"].key_name,
                 market_name=self.market_a_args["name"],
                 asset_name=self.market_a_args["asset"],
                 buy_intensity=10,
                 sell_intensity=10,
                 buy_volume=1,
                 sell_volume=1,
                 submit_bias=1,
                 cancel_bias=1,
-                tag=str(i),
+                tag="market_a_" + str(i),
             )
             for i in range(self.num_lo_traders_per_market)
         ]
 
         market_b_lo_traders = [
             LimitOrderTrader(
                 wallet_name=MARKET_TRADERS[
                     f"MARKET_A_TRADER_{str(i).zfill(4)}"
                 ].wallet_name,
-                wallet_pass=MARKET_TRADERS[
-                    f"MARKET_A_TRADER_{str(i).zfill(4)}"
-                ].wallet_pass,
                 key_name=MARKET_TRADERS[f"MARKET_A_TRADER_{str(i).zfill(4)}"].key_name,
                 market_name=self.market_a_args["name"],
                 asset_name=self.market_a_args["asset"],
                 buy_intensity=10,
                 sell_intensity=10,
                 buy_volume=1,
                 sell_volume=1,
                 submit_bias=1,
                 cancel_bias=1,
-                tag=str(i),
+                tag="market_b_" + str(i),
             )
             for i in range(self.num_lo_traders_per_market)
         ]
 
         market_c_lo_traders = [
             LimitOrderTrader(
                 wallet_name=MARKET_TRADERS[
                     f"MARKET_A_TRADER_{str(i).zfill(4)}"
                 ].wallet_name,
-                wallet_pass=MARKET_TRADERS[
-                    f"MARKET_A_TRADER_{str(i).zfill(4)}"
-                ].wallet_pass,
                 key_name=MARKET_TRADERS[f"MARKET_A_TRADER_{str(i).zfill(4)}"].key_name,
                 market_name=self.market_a_args["name"],
                 asset_name=self.market_a_args["asset"],
                 buy_intensity=10,
                 sell_intensity=10,
-                buy_volume=1,
-                sell_volume=1,
+                buy_volume=0.1,
+                sell_volume=0.1,
                 submit_bias=1,
                 cancel_bias=1,
-                tag=str(i),
+                tag="market_c_" + str(i),
             )
             for i in range(self.num_lo_traders_per_market)
         ]
 
         market_a_mo_traders = [
             MarketOrderTrader(
                 wallet_name=MARKET_TRADERS[
                     f"MARKET_A_TRADER_{str(i).zfill(4)}"
                 ].wallet_name,
-                wallet_pass=MARKET_TRADERS[
-                    f"MARKET_A_TRADER_{str(i).zfill(4)}"
-                ].wallet_pass,
                 key_name=MARKET_TRADERS[f"MARKET_A_TRADER_{str(i).zfill(4)}"].key_name,
                 market_name=self.market_a_args["name"],
                 asset_name=self.market_a_args["asset"],
                 buy_intensity=10,
                 sell_intensity=10,
                 base_order_size=1,
                 step_bias=self.market_order_trader_step_bias,
-                tag=str(i),
+                tag="market_a_" + str(i),
             )
             for i in range(self.num_mo_traders_per_market)
         ]
         market_b_mo_traders = [
             MarketOrderTrader(
                 wallet_name=MARKET_TRADERS[
                     f"MARKET_B_TRADER_{str(i).zfill(4)}"
                 ].wallet_name,
-                wallet_pass=MARKET_TRADERS[
-                    f"MARKET_B_TRADER_{str(i).zfill(4)}"
-                ].wallet_pass,
                 key_name=MARKET_TRADERS[f"MARKET_B_TRADER_{str(i).zfill(4)}"].key_name,
                 market_name=self.market_b_args["name"],
                 asset_name=self.market_b_args["asset"],
                 buy_intensity=10,
                 sell_intensity=10,
                 base_order_size=1,
                 step_bias=self.market_order_trader_step_bias,
-                tag=str(i),
+                tag="market_b_" + str(i),
             )
             for i in range(self.num_mo_traders_per_market)
         ]
         market_c_mo_traders = [
             MarketOrderTrader(
                 wallet_name=MARKET_TRADERS[
                     f"MARKET_C_TRADER_{str(i).zfill(4)}"
                 ].wallet_name,
-                wallet_pass=MARKET_TRADERS[
-                    f"MARKET_C_TRADER_{str(i).zfill(4)}"
-                ].wallet_pass,
                 key_name=MARKET_TRADERS[f"MARKET_C_TRADER_{str(i).zfill(4)}"].key_name,
                 market_name=self.market_c_args["name"],
                 asset_name=self.market_c_args["asset"],
                 buy_intensity=10,
                 sell_intensity=10,
-                base_order_size=1,
+                base_order_size=0.1,
                 step_bias=self.market_order_trader_step_bias,
-                tag=str(i),
+                tag="market_c_" + str(i),
             )
             for i in range(self.num_mo_traders_per_market)
         ]
 
         agents = (
             [
                 market_a_manager,
@@ -513,36 +493,36 @@
     ) -> MarketEnvironmentWithState:
         return MarketEnvironmentWithState(
             agents=list(self.agents.values()),
             n_steps=self.num_steps,
             random_agent_ordering=False,
             transactions_per_block=self.transactions_per_block,
             vega_service=vega,
-            step_length_seconds=self.granularity.value,
+            step_length_seconds=self.step_length_seconds,
             block_length_seconds=vega.seconds_per_block,
         )
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--debug", action="store_true")
     args = parser.parse_args()
 
     logging.basicConfig(level=logging.INFO if not args.debug else logging.DEBUG)
 
     scenario = VegaLoadTest(
-        num_steps=1000,
+        num_steps=10000,
         granularity=Granularity.FIFTEEN_MINUTE,
-        block_length_seconds=60,
+        block_length_seconds=1,
         transactions_per_block=4096,
     )
 
     with VegaServiceNull(
         warn_on_raw_data_access=False,
-        run_with_console=True,
+        run_with_console=False,
         use_full_vega_wallet=False,
         retain_log_files=True,
         launch_graphql=False,
         seconds_per_block=scenario.block_length_seconds,
         transactions_per_block=scenario.transactions_per_block,
     ) as vega:
         scenario.run_iteration(
```

### Comparing `vega_sim-0.67.0/vega_sim/scenario/parameter_experiment/scenario.py` & `vega_sim-1.0.1/vega_sim/scenario/parameter_experiment/scenario.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,54 +27,62 @@
 from vega_sim.scenario.common.agents import (
     OpenAuctionPass,
     MarketOrderTrader,
     ExponentialShapedMarketMaker,
     PriceSensitiveLimitOrderTrader,
     InformedTrader,
     StateAgent,
+    SimpleLiquidityProvider,
 )
 
 from vega_sim.scenario.common.utils.price_process import (
     Granularity,
     get_historic_price_series,
 )
 
 
 class ParameterExperiment(Scenario):
     """Class simulates a scenario for use in parameter experiments.
 
-    The default values for the ParameterExperiment scenario are to simulate a daily
-    ETH:USD future with trading activity in five minute steps.
+    The default values for the ParameterExperiment scenario are to simulate an hours
+    trading activity in 10 second intervals.
 
     """
 
     def __init__(
         self,
-        num_steps: int = 360,
+        num_steps: int = 600,
+        step_length_seconds=10,
         granularity: Optional[Granularity] = Granularity.MINUTE,
         block_size: int = 100,
         block_length_seconds: int = 1,
         state_extraction_fn: Optional[
             Callable[[VegaServiceNull, Dict[str, Agent]], Any]
         ] = None,
         settle_at_end: bool = True,
         price_process_fn: Optional[Callable] = None,
         market_name: Optional[str] = "ETH:USD (6hr Future)",
         market_code: str = "ETHUSD",
         asset_name: str = "ETH",
         asset_dp: str = 18,
-        rt_mint: int = 10_000,
-        it_mint: int = 10_000,
+        rt_mint: int = 100_000,
+        it_mint: int = 100_000,
         st_mint: int = 1_000_000,
     ):
         super().__init__(state_extraction_fn=state_extraction_fn)
 
         # Simulation settings
         self.num_steps = num_steps
+        self.step_length_seconds = step_length_seconds
         self.granularity = granularity
+        self.interpolation = (
+            f"{step_length_seconds}S"
+            if step_length_seconds < granularity.value
+            else None
+        )
         self.block_size = block_size
         self.block_length_seconds = block_length_seconds
         self.settle_at_end = settle_at_end
         self.price_process_fn = price_process_fn
 
         # Asset info parameters
         self.asset_name = asset_name
@@ -89,25 +97,25 @@
         self.st_mint = st_mint
         self.it_mint = it_mint
 
     def _generate_price_process(
         self,
         random_state: np.random.RandomState,
     ) -> list:
-
         # Select a random start and end datetime
         start = datetime.strptime(
             "2022-01-01 00:00:00", "%Y-%m-%d %H:%M:%S"
         ) + timedelta(days=int(random_state.choice(range(90))))
         end = start + timedelta(seconds=(self.num_steps + 1) * self.granularity.value)
 
         # Get the historic price process between the randomly generated dates
         price_process = get_historic_price_series(
             product_id="ETH-USD",
             granularity=self.granularity,
+            interpolation=self.interpolation,
             start=str(start),
             end=str(end),
         )
 
         return list(price_process)
 
     def configure_agents(
@@ -130,81 +138,102 @@
             self.price_process_fn()
             if self.price_process_fn is not None
             else self._generate_price_process(random_state=random_state)
         )
 
         market_manager = ConfigurableMarketManager(
             proposal_wallet_name="vega",
-            proposal_wallet_pass="pass",
             proposal_key_name="market_proposer",
             termination_wallet_name="vega",
-            termination_wallet_pass="pass",
             termination_key_name="market_settler",
             market_config=market_config,
             market_name=market_name,
             market_code=self.market_code,
             asset_dp=self.asset_decimal,
             asset_name=asset_name,
             settlement_price=price_process[-1] if self.settle_at_end else None,
             tag=None,
         )
 
         market_maker = ExponentialShapedMarketMaker(
             wallet_name="vega",
-            wallet_pass="pass",
             key_name="market_maker",
             price_process_generator=iter(price_process),
-            initial_asset_mint=1e9,
-            commitment_amount=500_000,
-            fee_amount=0.0003,
+            initial_asset_mint=1e10,
+            commitment_amount=1_000_000,
+            fee_amount=0.001,
             market_name=market_name,
             asset_name=asset_name,
             market_decimal_places=market_config.decimal_places,
             asset_decimal_places=self.asset_decimal,
             num_steps=self.num_steps,
             kappa=5,
             num_levels=20,
             tick_spacing=0.01,
             inventory_upper_boundary=20,
             inventory_lower_boundary=-20,
             market_kappa=5,
             market_order_arrival_rate=0.5,
             state_update_freq=10,
             tag=None,
+            orders_from_stream=True,
         )
 
+        simple_liquidity_providers = [
+            SimpleLiquidityProvider(
+                wallet_name="vega",
+                key_name="simple_lp_c",
+                market_name=market_name,
+                asset_name=asset_name,
+                initial_asset_mint=1e10,
+                commitment_amount=100_000,
+                bid_inner_bound_fn=lambda vega_state, market_id: vega_state.market_state[
+                    market_id
+                ].midprice,
+                bid_outer_bound_fn=lambda vega_state, market_id: vega_state.market_state[
+                    market_id
+                ].min_valid_price,
+                ask_inner_bound_fn=lambda vega_state, market_id: vega_state.market_state[
+                    market_id
+                ].midprice,
+                ask_outer_bound_fn=lambda vega_state, market_id: vega_state.market_state[
+                    market_id
+                ].max_valid_price,
+                offset_proportion=0.16,
+                fee=0.001,
+            )
+            for i, offset in enumerate([0.02, 0.04, 0.06])
+        ]
+
         # Create fixed auction pass agents
         open_auction_pass_bid = OpenAuctionPass(
             wallet_name="vega",
-            wallet_pass="pass",
             key_name="auction_trader_bid",
             side="SIDE_BUY",
             initial_asset_mint=1e9,
             initial_price=price_process[0],
             market_name=market_name,
             asset_name=asset_name,
             opening_auction_trade_amount=market_config.position_decimal_places,
             tag="bid",
         )
         open_auction_pass_ask = OpenAuctionPass(
             wallet_name="vega",
-            wallet_pass="pass",
             key_name="auction_trader_ask",
             side="SIDE_SELL",
             initial_asset_mint=1e9,
             initial_price=price_process[0],
             market_name=market_name,
             asset_name=asset_name,
             opening_auction_trade_amount=market_config.position_decimal_places,
             tag="ask",
         )
 
         informed_trader = InformedTrader(
             wallet_name="vega",
-            wallet_pass="pass",
             key_name="informed_trade",
             price_process=price_process,
             market_name=market_name,
             asset_name=asset_name,
             initial_asset_mint=self.it_mint,
             proportion_taken=0.05,
             lookahead=5,
@@ -213,15 +242,14 @@
             tag=None,
             random_state=random_state,
         )
 
         random_traders = [
             MarketOrderTrader(
                 wallet_name="vega",
-                wallet_pass="pass",
                 key_name=f"random_trader_{i}",
                 market_name=market_name,
                 asset_name=asset_name,
                 initial_asset_mint=self.rt_mint,
                 base_order_size=0.1,
                 buy_intensity=buy_intensity,
                 sell_intensity=sell_intensity,
@@ -233,15 +261,14 @@
             )
         ]
 
         # Create fixed sensitive_traders
         sensitive_traders = [
             PriceSensitiveLimitOrderTrader(
                 wallet_name="vega",
-                wallet_pass="pass",
                 key_name="sensitive_trader",
                 market_name=market_name,
                 asset_name=asset_name,
                 initial_asset_mint=self.st_mint,
                 max_order_size=50,
                 scale=0.035,
                 price_process_generator=iter(price_process),
@@ -254,29 +281,29 @@
             [
                 market_manager,
                 market_maker,
                 open_auction_pass_bid,
                 open_auction_pass_ask,
                 informed_trader,
             ]
+            + simple_liquidity_providers
             + sensitive_traders
             + random_traders
         )
         return {agent.name(): agent for agent in agents}
 
     def configure_environment(
         self,
         vega: VegaServiceNull,
         random_state: Optional[np.random.RandomState] = None,
         **kwargs,
     ) -> MarketEnvironmentWithState:
-
         return MarketEnvironmentWithState(
             agents=list(self.agents.values()),
             n_steps=self.num_steps,
-            step_length_seconds=self.granularity.value,
+            step_length_seconds=self.step_length_seconds,
             random_agent_ordering=True,
             transactions_per_block=self.block_size,
             vega_service=vega,
             block_length_seconds=self.block_length_seconds,
             random_state=random_state,
         )
```

### Comparing `vega_sim-0.67.0/vega_sim/scenario/registry.py` & `vega_sim-1.0.1/vega_sim/scenario/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,19 +170,20 @@
         market_name="RESEARCH: Ethereum:USD Q3 (Daily)",
         market_code="ETH:USD",
         asset_name="tUSD",
         asset_dp=18,
         num_steps=60 * 24,
     ),
     "vega_load_test": lambda: VegaLoadTest(
-        num_steps=15 * 24 * 30,
-        granularity=Granularity.FIFTEEN_MINUTE,
-        block_length_seconds=60,
+        num_steps=60 * 24,
+        granularity=Granularity.MINUTE,
+        step_length_seconds=60,
+        block_length_seconds=5,
         transactions_per_block=4000,
-        parties_per_market=200,
+        parties_per_market=100,
         orders_per_second=100,
         trades_per_second=1,
     ),
     "hedged_market": lambda: HedgedMarket(
         num_steps=24 * 60,
         step_length_seconds=60,
         block_length_seconds=1,
```

### Comparing `vega_sim-0.67.0/vega_sim/scenario/scenario.py` & `vega_sim-1.0.1/vega_sim/scenario/scenario.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     @abc.abstractmethod
     def configure_agents(
         self,
         vega: VegaService,
         tag: str,
         random_state: Optional[np.random.RandomState],
         **kwargs,
-    ) -> List[StateAgent]:
+    ) -> Dict[str, StateAgent]:
         pass
 
     @abc.abstractmethod
     def configure_environment(
         self,
         vega: VegaService,
         tag: str,
@@ -50,15 +50,14 @@
             run_with_console=run_with_console,
         )
         return result
 
     def run_iteration(
         self,
         vega: VegaService,
-        network: Optional[Network] = None,
         pause_at_completion: bool = False,
         run_with_console: bool = False,
         random_state: Optional[np.random.RandomState] = None,
         run_with_snitch: bool = True,
         tag: Optional[str] = None,
         output_data: bool = False,
         **kwargs,
```

### Comparing `vega_sim-0.67.0/vega_sim/service.py` & `vega_sim-1.0.1/vega_sim/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 from __future__ import annotations
 
+import copy
 import datetime
 import logging
-import threading
 import time
-import copy
 from abc import ABC
 from collections import defaultdict
 from dataclasses import dataclass
 from functools import wraps
 from queue import Queue, Empty
-from typing import Dict, List, Optional, Tuple, Union, Any, Generator
 from itertools import product
+from typing import Any, Dict, Generator, List, Optional, Set, Tuple, Union
 
 import grpc
+
 import vega_sim.api.data as data
 import vega_sim.api.data_raw as data_raw
 import vega_sim.api.faucet as faucet
 import vega_sim.api.governance as gov
 import vega_sim.api.market as market
 import vega_sim.api.trading as trading
 import vega_sim.grpc.client as vac
+import vega_sim.proto.data_node.api.v2 as data_node_protos_v2
 import vega_sim.proto.vega as vega_protos
 import vega_sim.proto.vega.data_source_pb2 as data_source_protos
-import vega_sim.proto.data_node.api.v2 as data_node_protos_v2
-
 from vega_sim.api.helpers import (
     forward,
     num_to_padded_int,
     wait_for_core_catchup,
     wait_for_datanode_sync,
 )
+from vega_sim.local_data_cache import LocalDataCache
 from vega_sim.proto.vega.commands.v1.commands_pb2 import (
-    OrderCancellation,
     OrderAmendment,
+    OrderCancellation,
     OrderSubmission,
 )
 from vega_sim.proto.vega.governance_pb2 import (
     UpdateFutureProduct,
     UpdateInstrumentConfiguration,
     UpdateMarketConfiguration,
 )
@@ -62,19 +62,14 @@
     pass
 
 
 class DatanodeBehindError(Exception):
     pass
 
 
-def _queue_forwarder(source: Generator[Any], sink: Queue[Any]) -> None:
-    for elem in source:
-        sink.put(elem)
-
-
 def raw_data(fn):
     @wraps(fn)
     def wrapped_fn(self, *args, **kwargs):
         if self.warn_on_raw_data_access:
             logger.warn(
                 f"Using function with raw data from data-node {fn.__qualname__}. Be"
                 " wary if prices/positions are not converted from int form"
@@ -95,14 +90,15 @@
 
 class VegaService(ABC):
     def __init__(
         self,
         can_control_time: bool = False,
         warn_on_raw_data_access: bool = True,
         seconds_per_block: int = 1,
+        listen_for_high_volume_stream_updates: bool = False,
     ):
         """A generic service for accessing a set of Vega processes.
 
         Contains generic methods aimed at working whether the derived class
         is referencing a locally hosted Nullchain version of Vega
         or a fully-fledged remote market.
 
@@ -118,44 +114,43 @@
                     decimal places. On non-raw data functions the 'zero-padded int'
                     version of numbers will be promised to have been converted to a
                     real float version. On raw versions (generally complex objects)
                     they may well be still zero padded integers which must be
                     converted by the user.
                     (e.g. 10.1 with decimal places set to 2 would be 1010)
             seconds_per_block:
-                int, default 1, How long each block represents in seconds. For a nullchain
-                    service this can be known exactly, for anything else it will be an
-                    estimate. Used for waiting/forwarding time and determining how far
-                    forwards to place proposals starting/ending.
+                int, default 1, How long each block represents in seconds. For a
+                    nullchain service this can be known exactly, for anything
+                    else it will be an estimate. Used for waiting/forwarding time
+                    and determining how far forwards to place proposals
+                    starting/ending.
+            listen_for_high_volume_stream_updates:
+                bool, default False, Whether to listen for high volume stream updates.
+                    These are generally less necessary, but contain large numbers of
+                    updates per block, such as all ledger transactions. For a network
+                    running at ~1s/block these are likely to be fine, but can be a
+                    hindrance working at full nullchain speed.
 
         """
         self._core_client = None
         self._core_state_client = None
         self._trading_data_client_v2 = None
+        self._local_data_cache = None
         self.can_control_time = can_control_time
         self.warn_on_raw_data_access = warn_on_raw_data_access
 
         self._market_price_decimals = None
         self._market_pos_decimals = None
         self._asset_decimals = None
         self._market_to_asset = None
+        self._listen_for_high_volume_stream_updates = (
+            listen_for_high_volume_stream_updates
+        )
         self.seconds_per_block = seconds_per_block
 
-        self.orders_lock = threading.RLock()
-        self.transfers_lock = threading.RLock()
-        self.trades_lock = threading.RLock()
-        self._order_state_from_feed = {}
-        self._transfer_state_from_feed = {}
-        self._trades_from_feed: List[data.Trade] = []
-
-        self._observation_feeds: List[Queue[Any]] = []
-        self._observation_thread = None
-        self._aggregated_observation_feed: Queue[Any] = Queue()
-        self._kill_thread_sig = threading.Event()
-
     @property
     def market_price_decimals(self) -> int:
         if self._market_price_decimals is None:
             self._market_price_decimals = DecimalsCache(
                 lambda market_id: data.market_price_decimals(
                     market_id=market_id, data_client=self.trading_data_client_v2
                 )
@@ -189,14 +184,30 @@
                 lambda market_id: data_raw.market_info(
                     market_id=market_id, data_client=self.trading_data_client_v2
                 ).tradable_instrument.instrument.future.settlement_asset
             )
         return self._market_to_asset
 
     @property
+    def data_cache(self) -> LocalDataCache:
+        if self._local_data_cache is None:
+            self._local_data_cache = LocalDataCache(
+                self.trading_data_client_v2,
+                self.trading_data_client_v2,
+                self.market_pos_decimals,
+                self.market_price_decimals,
+                self.asset_decimals,
+                self.market_to_asset,
+            )
+            self._local_data_cache.start_live_feeds(
+                start_high_load_feeds=self._listen_for_high_volume_stream_updates
+            )
+        return self._local_data_cache
+
+    @property
     def data_node_rest_url(self) -> str:
         pass
 
     @property
     def faucet_url(self) -> str:
         pass
 
@@ -263,55 +274,50 @@
         wait_for_core_catchup(self.core_client)
 
     def wait_for_total_catchup(self) -> None:
         self.wait_for_core_catchup()
         self.wait_for_datanode_sync()
 
     def stop(self) -> None:
-        self._kill_thread_sig.set()
+        if self._local_data_cache is not None:
+            self._local_data_cache.stop()
 
     def login(self, name: str, passphrase: str) -> str:
         """Logs in to existing wallet in the given vega service.
 
         Args:
             name:
                 str, The name of the wallet
             passphrase:
                 str, The login passphrase used when creating the wallet
         Returns:
             str, public key associated to this waller
         """
         return self.wallet.login(name=name, passphrase=passphrase)
 
-    def create_wallet(
-        self, name: str, passphrase: str, key_name: Optional[str] = None
-    ) -> str:
-        """Logs in to existing wallet in the given vega service.
+    def create_key(self, name: str, wallet_name: Optional[str] = None) -> str:
+        """Creates a key within the default wallet.
 
         Args:
             name:
-                str, The name of the wallet
-            passphrase:
-                str, The login passphrase used when creating the wallet
-             key_name:
-                str, optional, Name of key in wallet for agent to use. Defaults
+                str, The name of the key to use
+             wallet_name:
+                str, optional, Name of wallet containing key for agent to use. Defaults
                 to value in the environment variable "VEGA_DEFAULT_KEY_NAME".
         Returns:
-            str, public key associated to this waller
+            str, public key associated to this wallet
         """
-        return self.wallet.create_wallet(
-            name=name, passphrase=passphrase, key_name=key_name
-        )
+        return self.wallet.create_key(wallet_name=wallet_name, name=name)
 
     def mint(
         self,
-        wallet_name: str,
+        key_name: Optional[str],
         asset: str,
         amount: float,
-        key_name: Optional[str] = None,
+        wallet_name: Optional[str] = None,
     ) -> None:
         """Mints a given amount of requested asset into the associated wallet
 
         Args:
             wallet_name:
                 str, The name of the wallet
             asset:
@@ -323,15 +329,15 @@
         """
         asset_decimals = self.asset_decimals[asset]
         curr_acct = self.party_account(
             wallet_name=wallet_name, asset_id=asset, market_id=None, key_name=key_name
         ).general
 
         faucet.mint(
-            self.wallet.public_key(wallet_name, key_name),
+            self.wallet.public_key(wallet_name=wallet_name, name=key_name),
             asset,
             num_to_padded_int(amount, asset_decimals),
             faucet_url=self.faucet_url,
         )
 
         self.wait_fn(1)
         self.wait_for_core_catchup()
@@ -363,21 +369,21 @@
         """
         if not self.can_control_time:
             return
         forward(time=time, vega_node_url=self.vega_node_url)
 
     def create_asset(
         self,
-        wallet_name: str,
+        key_name: str,
         name: str,
         symbol: str,
         decimals: int = 0,
         quantum: int = 1,
         max_faucet_amount: int = 10e9,
-        key_name: Optional[str] = None,
+        wallet_name: Optional[str] = None,
     ):
         """Creates a simple asset and automatically approves the proposal (assuming the
          proposing wallet has sufficient governance tokens).
 
         Args:
             wallet_name:
                 str, The name of the wallet proposing the asset
@@ -420,17 +426,17 @@
             wallet=self.wallet,
             key_name=key_name,
         )
         self.wait_fn(110)
 
     def create_market_from_config(
         self,
-        proposal_wallet_name: str,
+        proposal_key_name: str,
         market_config: market.MarketConfig,
-        proposal_key_name: Optional[str] = None,
+        proposal_wallet_name: Optional[str] = None,
     ):
         blockchain_time_seconds = gov.get_blockchain_time(self.trading_data_client_v2)
 
         proposal_id = gov.propose_market_from_config(
             wallet=self.wallet,
             data_client=self.trading_data_client_v2,
             proposal_wallet_name=proposal_wallet_name,
@@ -448,54 +454,55 @@
             key_name=proposal_key_name,
         )
         self.wait_fn(110)
 
     def create_simple_market(
         self,
         market_name: str,
-        proposal_wallet: str,
+        proposal_key: str,
         settlement_asset_id: str,
-        termination_wallet: str,
+        termination_key: str,
         future_asset: Optional[str] = None,
         position_decimals: Optional[int] = None,
         market_decimals: Optional[int] = None,
         risk_aversion: Optional[float] = 1e-6,
         tau: Optional[float] = 1.0 / 365.25 / 24,
         sigma: Optional[float] = 1.0,
         price_monitoring_parameters: Optional[
             vega_protos.markets.PriceMonitoringParameters
         ] = None,
-        key_name: Optional[str] = None,
-        termination_key: Optional[str] = None,
+        wallet_name: Optional[str] = None,
+        termination_wallet_name: Optional[str] = None,
     ) -> None:
         """Creates a simple futures market with a predefined reasonable set of parameters.
 
-        Args:
-            market_name:c
-                str, name of the market
-            proposal_wallet:
-                str, the name of the wallet to use for proposing the market
-            settlement_asset_id:
-                str, the asset id the market will use for settlement
-            termination_wallet:
-                str, the name of the wallet which will be used to send termination data
-            position_decimals:
-                int, the decimal place precision to use for positions
-                    (e.g. 2 means 2dp, so 200 => 2.00, 3 would mean 200 => 0.2)
-           market_decimals:
-                int, the decimal place precision to use for market prices
-                    (e.g. 2 means 2dp, so 200 => 2.00, 3 would mean 200 => 0.2)
-            price_monitoring_parameters:
-                PriceMonitoringParameters, A set of parameters determining when the
-                    market will drop into a price auction. If not passed defaults
-                    to a very permissive setup
-            key_name:
-                Optional[str], name of key proposing market. Defaults to None.
-            termination_key:
-                Optional[str], name of key settling market. Defaults to None.
+                Args:
+                    market_name:
+                        str, name of the market
+                    proposal_key:
+                        str, the name of the key to use for proposing the market
+                    settlement_asset_id:
+                        str, the asset id the market will use for settlement
+                    termination_key:
+                        str, the name of the key which will be used to send termination data
+                    position_decimals:
+                        int, the decimal place precision to use for positions
+                            (e.g. 2 means 2dp, so 200 => 2.00, 3 would mean 200 => 0.2)
+                   market_decimals:
+                        int, the decimal place precision to use for market prices
+                            (e.g. 2 means 2dp, so 200 => 2.00, 3 would mean 200 => 0.2)
+                    price_monitoring_parameters:
+                        PriceMonitoringParameters, A set of parameters determining when the
+                            market will drop into a price auction. If not passed defaults
+                            to a very permissive setup
+                            wallet_name: Optional[str] = None,
+        :
+                        Optional[str], name of wallet proposing market. Defaults to None.
+                    termination_wallet_name:
+                        Optional[str], name of wallet settling market. Defaults to None.
 
         """
         additional_kwargs = {}
         if future_asset is not None:
             additional_kwargs["future_asset"] = future_asset
 
         blockchain_time_seconds = gov.get_blockchain_time(self.trading_data_client_v2)
@@ -504,106 +511,106 @@
             risk_aversion_parameter=risk_aversion,
             tau=tau,
             params=vega_protos.markets.LogNormalModelParams(mu=0, r=0.0, sigma=sigma),
         )
         proposal_id = gov.propose_future_market(
             market_name=market_name,
             wallet=self.wallet,
-            wallet_name=proposal_wallet,
-            key_name=key_name,
+            wallet_name=wallet_name,
+            key_name=proposal_key,
             settlement_asset_id=settlement_asset_id,
             data_client=self.trading_data_client_v2,
             termination_pub_key=self.wallet.public_key(
-                termination_wallet, termination_key
+                wallet_name=termination_wallet_name, name=termination_key
             ),
             position_decimals=position_decimals,
             market_decimals=market_decimals,
             closing_time=blockchain_time_seconds + self.seconds_per_block * 90,
             enactment_time=blockchain_time_seconds + self.seconds_per_block * 100,
             risk_model=risk_model,
             time_forward_fn=lambda: self.wait_fn(2),
             price_monitoring_parameters=price_monitoring_parameters,
             **additional_kwargs,
         )
         gov.approve_proposal(
             proposal_id=proposal_id,
             wallet=self.wallet,
-            wallet_name=proposal_wallet,
-            key_name=key_name,
+            wallet_name=wallet_name,
+            key_name=proposal_key,
         )
         self.wait_fn(110)
 
     def submit_market_order(
         self,
-        trading_wallet: str,
+        trading_key: str,
         market_id: str,
         side: Union[vega_protos.vega.Side, str],
         volume: float,
         fill_or_kill: bool = True,
         wait: bool = True,
         order_ref: Optional[str] = None,
-        key_name: Optional[str] = None,
+        trading_wallet: Optional[str] = None,
     ) -> str:
         """Places a simple Market order, either as Fill-Or-Kill or Immediate-Or-Cancel.
 
         Args:
-            trading_wallet:
-                str, the name of the wallet to use for trading
+            trading_key:
+                str, the name of the key to use for trading
             market_name:
                 str, name of the market
             side:
                 vega.Side or str, Side of the order (BUY or SELL)
             volume:
                 float, The volume to trade.
             wait:
                 bool, whether to wait for order acceptance.
                     If true, will raise an error if order is not accepted
             order_ref:
                 optional str, reference for later identification of order
-            key_name:
-                optional str, name of key in wallet to use
+            wallet_name:
+                optional str, name of wallet to use
 
         Returns:
             str, The ID of the order
         """
 
         return self.submit_order(
             trading_wallet=trading_wallet,
             market_id=market_id,
             time_in_force="TIME_IN_FORCE_FOK" if fill_or_kill else "TIME_IN_FORCE_IOC",
             order_type="TYPE_MARKET",
             side=side,
             volume=volume,
             wait=wait,
             order_ref=order_ref,
-            key_name=key_name,
+            trading_key=trading_key,
         )
 
     def submit_order(
         self,
-        trading_wallet: str,
+        trading_key: str,
         market_id: str,
         order_type: Union[vega_protos.vega.Order.Type, str],
         time_in_force: Union[vega_protos.vega.Order.TimeInForce, str],
         side: Union[vega_protos.vega.Side, str],
         volume: float,
         price: Optional[float] = None,
         expires_at: Optional[float] = None,
         pegged_order: Optional[PeggedOrder] = None,
         wait: bool = True,
         order_ref: Optional[str] = None,
-        key_name: Optional[str] = None,
+        trading_wallet: Optional[str] = None,
     ) -> Optional[str]:
         """
         Submit orders as specified to required pre-existing market.
         Optionally wait for acceptance of order (raises on non-acceptance)
 
         Args:
-            trading_wallet:
-                str, the name of the wallet to use for trading
+            trading_key:
+                str, the name of the key to use for trading
             market_id:
                 str, the ID of the required market on vega
             order_type:
                 vega.Order.Type or str, The type of order required (market/limit etc).
                     See API documentation for full list of options
             time_in_force:
                 vega.Order.TimeInForce or str, The time in force setting for the order
@@ -669,53 +676,55 @@
             market_id=market_id,
             order_type=order_type,
             time_in_force=time_in_force,
             side=side,
             volume=submit_volume,
             price=str(submit_price) if submit_price is not None else None,
             expires_at=int(expires_at) if expires_at is not None else None,
-            pegged_order=vega_protos.vega.PeggedOrder(
-                reference=pegged_order.reference,
-                offset=str(
-                    num_to_padded_int(
-                        pegged_order.offset, self.market_price_decimals[market_id]
-                    )
-                ),
-            )
-            if pegged_order is not None
-            else None,
+            pegged_order=(
+                vega_protos.vega.PeggedOrder(
+                    reference=pegged_order.reference,
+                    offset=str(
+                        num_to_padded_int(
+                            pegged_order.offset, self.market_price_decimals[market_id]
+                        )
+                    ),
+                )
+                if pegged_order is not None
+                else None
+            ),
             wait=wait,
             time_forward_fn=lambda: self.wait_fn(2),
             order_ref=order_ref,
-            key_name=key_name,
+            key_name=trading_key,
         )
 
     def get_blockchain_time(self) -> int:
         """Returns blockchain time in seconds since the epoch"""
         return gov.get_blockchain_time(self.trading_data_client_v2)
 
     def amend_order(
         self,
-        trading_wallet: str,
+        trading_key: str,
         market_id: str,
         order_id: str,
         price: Optional[float] = None,
         expires_at: Optional[int] = None,
         pegged_offset: Optional[float] = None,
         pegged_reference: Optional[vega_protos.vega.PeggedReference] = None,
         volume_delta: float = 0,
         time_in_force: Optional[Union[vega_protos.vega.Order.TimeInForce, str]] = None,
-        key_name: Optional[str] = None,
+        wallet_name: Optional[str] = None,
     ):
         """
         Amend a Limit order by orderID in the specified market
 
         Args:
-            trading_wallet:
-                str, the name of the wallet to use for trading
+            trading_key:
+                str, the name of the key to use for trading
             market_id:
                 str, the ID of the required market on vega
             order_type:
                 vega.Order.Type or str, The type of order required (market/limit etc).
                     See API documentation for full list of options
             side:
                 vega.Side or str, Side of the order (BUY or SELL)
@@ -725,138 +734,142 @@
                 int, price of the order
             time_in_force:
                 vega.Order.TimeInForce or str, The time in force setting for the order
                     (Only valid options for market are TIME_IN_FORCE_IOC and
                         TIME_IN_FORCE_FOK)
                     See API documentation for full list of options
                     Defaults to Fill or Kill
-            key_name:
-                optional str, name of key in wallet to use
+            wallet_name:
+                optional str, name of wallet to use
         """
         trading.amend_order(
             wallet=self.wallet,
-            wallet_name=trading_wallet,
+            key_name=trading_key,
+            wallet_name=wallet_name,
             market_id=market_id,
             order_id=order_id,
-            price=str(
-                num_to_padded_int(
-                    price,
-                    self.market_price_decimals[market_id],
+            price=(
+                str(
+                    num_to_padded_int(
+                        price,
+                        self.market_price_decimals[market_id],
+                    )
                 )
-            )
-            if price is not None
-            else None,
+                if price is not None
+                else None
+            ),
             expires_at=expires_at,
-            pegged_offset=str(
-                num_to_padded_int(
-                    pegged_offset,
-                    self.market_price_decimals[market_id],
+            pegged_offset=(
+                str(
+                    num_to_padded_int(
+                        pegged_offset,
+                        self.market_price_decimals[market_id],
+                    )
                 )
-            )
-            if pegged_offset is not None
-            else None,
+                if pegged_offset is not None
+                else None
+            ),
             pegged_reference=pegged_reference,
             volume_delta=num_to_padded_int(
                 volume_delta,
                 self.market_pos_decimals[market_id],
             ),
             time_in_force=time_in_force,
-            key_name=key_name,
         )
 
     def cancel_order(
         self,
-        trading_wallet: str,
+        trading_key: str,
         market_id: str,
         order_id: str,
-        key_name: Optional[str] = None,
+        wallet_name: Optional[str] = None,
     ):
         """
         Cancel Order
 
         Args:
             trading_wallet:
                 str, the name of the wallet to use for trading
             market_id:
                 str, the ID of the required market on vega
             order_id:
                 str, Identifier of the order to cancel
         """
         trading.cancel_order(
             wallet=self.wallet,
-            wallet_name=trading_wallet,
+            wallet_name=wallet_name,
             market_id=market_id,
             order_id=order_id,
-            key_name=key_name,
+            key_name=trading_key,
         )
 
     def update_network_parameter(
-        self, proposal_wallet: str, parameter: str, new_value: str, key_name: str = None
+        self, proposal_key: str, parameter: str, new_value: str, wallet_name: str = None
     ):
         """Updates a network parameter by first proposing and then voting to approve
         the change, followed by advancing the network time period forwards.
 
         If the genesis setup of the market is such that this meets requirements then
         the proposal will be approved. Otherwise others may need to vote too.
 
         Args:
-            proposal_wallet:
-                str, the wallet proposing the change
+            proposal_key:
+                str, the key proposing the change
             parameter:
                 str, the parameter to change
             new_value:
                 str, the new value to set
-            key_name:
-                str, optional, the wallet key proposing the change
+            wallet_name:
+                str, optional, the wallet proposing the change
         Returns:
             str, the ID of the proposal
         """
         blockchain_time_seconds = gov.get_blockchain_time(self.trading_data_client_v2)
 
         proposal_id = gov.propose_network_parameter_change(
             parameter=parameter,
             value=new_value,
             wallet=self.wallet,
-            wallet_name=proposal_wallet,
+            wallet_name=wallet_name,
             data_client=self.trading_data_client_v2,
             closing_time=blockchain_time_seconds + self.seconds_per_block * 90,
             enactment_time=blockchain_time_seconds + self.seconds_per_block * 100,
             time_forward_fn=lambda: self.wait_fn(2),
-            key_name=key_name,
+            key_name=proposal_key,
         )
         gov.approve_proposal(
             proposal_id=proposal_id,
             wallet=self.wallet,
-            wallet_name=proposal_wallet,
-            key_name=key_name,
+            wallet_name=wallet_name,
+            key_name=proposal_key,
         )
         self.wait_fn(110)
 
     def update_market(
         self,
-        proposal_wallet: str,
+        proposal_key: str,
         market_id: str,
         updated_instrument: Optional[UpdateInstrumentConfiguration] = None,
         updated_metadata: Optional[str] = None,
         updated_price_monitoring_parameters: Optional[PriceMonitoringParameters] = None,
         updated_liquidity_monitoring_parameters: Optional[
             LiquidityMonitoringParameters
         ] = None,
         updated_simple_model_params: Optional[SimpleModelParams] = None,
         updated_log_normal_risk_model: Optional[LogNormalRiskModel] = None,
+        wallet_name: Optional[int] = None,
         updated_lp_price_range: Optional[float] = None,
-        key_name: Optional[int] = None,
     ):
         """Updates a market based on proposal parameters. Will attempt to propose
         and then immediately vote on the market change before forwarding time for
         the enactment to also take effect
 
         Args:
-            proposal_wallet:
-                str, the wallet proposing the change
+            proposal_key:
+                str, the key proposing the change
             market_id:
                 str, the market to change
             new_value:
                 str, the new value to set
         Returns:
             str, the ID of the proposal
         """
@@ -912,84 +925,92 @@
         if updated_log_normal_risk_model is None:
             updated_log_normal_risk_model = (
                 current_market.tradable_instrument.log_normal_risk_model
             )
 
         update_configuration = UpdateMarketConfiguration(
             instrument=updated_instrument,
-            price_monitoring_parameters=updated_price_monitoring_parameters
-            if updated_price_monitoring_parameters is not None
-            else current_market.price_monitoring_settings.parameters,
-            liquidity_monitoring_parameters=updated_liquidity_monitoring_parameters
-            if updated_liquidity_monitoring_parameters is not None
-            else current_market.liquidity_monitoring_parameters,
+            price_monitoring_parameters=(
+                updated_price_monitoring_parameters
+                if updated_price_monitoring_parameters is not None
+                else current_market.price_monitoring_settings.parameters
+            ),
+            liquidity_monitoring_parameters=(
+                updated_liquidity_monitoring_parameters
+                if updated_liquidity_monitoring_parameters is not None
+                else current_market.liquidity_monitoring_parameters
+            ),
             simple=updated_simple_model_params,
             log_normal=updated_log_normal_risk_model,
             metadata=updated_metadata,
-            lp_price_range=str(updated_lp_price_range)
-            if updated_lp_price_range is not None
-            else current_market.lp_price_range,
+            lp_price_range=(
+                str(updated_lp_price_range)
+                if updated_lp_price_range is not None
+                else current_market.lp_price_range
+            ),
         )
 
         proposal_id = gov.propose_market_update(
             market_update=update_configuration,
             market_id=market_id,
             wallet=self.wallet,
-            wallet_name=proposal_wallet,
+            key_name=proposal_key,
+            wallet_name=wallet_name,
             data_client=self.trading_data_client_v2,
             closing_time=blockchain_time_seconds + self.seconds_per_block * 90,
             enactment_time=blockchain_time_seconds + self.seconds_per_block * 100,
             time_forward_fn=lambda: self.wait_fn(2),
         )
         gov.approve_proposal(
             proposal_id=proposal_id,
             wallet=self.wallet,
-            wallet_name=proposal_wallet,
+            key_name=proposal_key,
+            wallet_name=wallet_name,
         )
         self.wait_fn(110)
 
     def settle_market(
         self,
-        settlement_wallet: str,
+        settlement_key: str,
         settlement_price: float,
         market_id: str,
-        key_name: Optional[str] = None,
+        wallet_name: Optional[str] = None,
     ):
         future_inst = data_raw.market_info(
             market_id, data_client=self.trading_data_client_v2
         ).tradable_instrument.instrument.future
 
         filter_key = future_inst.data_source_spec_for_settlement_data.data.external.oracle.filters[
             0
         ].key
         oracle_name = filter_key.name
 
         logger.info(f"Settling market at price {settlement_price} for {oracle_name}")
 
         gov.settle_oracle(
             wallet=self.wallet,
-            wallet_name=settlement_wallet,
+            wallet_name=wallet_name,
             oracle_name=oracle_name,
             settlement_price=num_to_padded_int(
                 settlement_price, decimals=filter_key.number_decimal_places
             ),
-            key_name=key_name,
+            key_name=settlement_key,
         )
 
     def party_account(
         self,
-        wallet_name: str,
+        key_name: str,
         asset_id: str,
         market_id: str,
-        key_name: Optional[str] = None,
+        wallet_name: Optional[str] = None,
     ) -> data.PartyMarketAccount:
         """Output money in general accounts/margin accounts/bond accounts (if exists)
         of a party."""
         return data.party_account(
-            self.wallet.public_key(wallet_name, key_name),
+            self.wallet.public_key(wallet_name=wallet_name, name=key_name),
             asset_id=asset_id,
             market_id=market_id,
             data_client=self.trading_data_client_v2,
         )
 
     def list_accounts(
         self,
@@ -1012,31 +1033,33 @@
 
         Returns:
             List[AccountData], cleaned account data for each account
 
         """
         return data.list_accounts(
             data_client=self.trading_data_client_v2,
-            pub_key=self.wallet.public_key(wallet_name, key_name)
-            if wallet_name is not None
-            else None,
+            pub_key=(
+                self.wallet.public_key(wallet_name=wallet_name, name=key_name)
+                if key_name is not None
+                else None
+            ),
             asset_id=asset_id,
             market_id=market_id,
             asset_decimals_map=self.asset_decimals,
         )
 
     def positions_by_market(
         self,
-        wallet_name: str,
+        key_name: str,
         market_id: Optional[str] = None,
-        key_name: Optional[str] = None,
+        wallet_name: Optional[str] = None,
     ) -> List[vega_protos.vega.Position]:
         """Output positions of a party."""
         return data.positions_by_market(
-            pub_key=self.wallet.public_key(wallet_name, key_name),
+            pub_key=self.wallet.public_key(wallet_name=wallet_name, name=key_name),
             market_id=market_id,
             data_client=self.trading_data_client_v2,
             market_price_decimals_map=self.market_price_decimals,
             market_position_decimals_map=self.market_pos_decimals,
             market_to_asset_map=self.market_to_asset,
             asset_decimals_map=self.asset_decimals,
         )
@@ -1059,18 +1082,28 @@
         Output market info.
         """
         return data_raw.market_info(
             market_id=market_id, data_client=self.trading_data_client_v2
         )
 
     @raw_data
+    def market_data_from_feed(
+        self,
+        market_id: str,
+    ) -> vega_protos.vega.MarketData:
+        """
+        Output market info.
+        """
+        return self.data_cache.market_data_from_feed(market_id)
+
+    @raw_data
     def market_data(
         self,
         market_id: str,
-    ) -> vega_protos.markets.MarketData:
+    ) -> vega_protos.vega.MarketData:
         """
         Output market info.
         """
         return data_raw.market_data(
             market_id=market_id, data_client=self.trading_data_client_v2
         )
 
@@ -1128,26 +1161,32 @@
         self,
         market_id: str,
     ) -> Tuple[int, int]:
         """
         Output the best static bid price and best static ask price in current market.
         """
         return data.best_prices(
-            market_id=market_id, data_client=self.trading_data_client_v2
+            market_id=market_id,
+            data_client=self.trading_data_client_v2,
+            market_data=self.data_cache.market_data_from_feed(market_id=market_id),
+            price_decimals=self.market_price_decimals[market_id],
         )
 
     def price_bounds(
         self,
         market_id: str,
     ) -> Tuple[Optional[float], Optional[float]]:
         """
         Output the tightest price bounds in the current market.
         """
         return data.price_bounds(
-            market_id=market_id, data_client=self.trading_data_client_v2
+            market_id=market_id,
+            data_client=self.trading_data_client_v2,
+            market_data=self.data_cache.market_data_from_feed(market_id=market_id),
+            price_decimals=self.market_price_decimals[market_id],
         )
 
     def order_book_by_market(
         self,
         market_id: str,
     ) -> data.OrderBook:
         return data.order_book_by_market(
@@ -1172,30 +1211,30 @@
             data_client=self.trading_data_client_v2,
             price_decimals=self.market_price_decimals[market_id],
             position_decimals=self.market_pos_decimals[market_id],
         )
 
     def submit_simple_liquidity(
         self,
-        wallet_name: str,
+        key_name: str,
         market_id: str,
         commitment_amount: float,
         fee: float,
         reference_buy: str,
         reference_sell: str,
         delta_buy: float,
         delta_sell: float,
         is_amendment: Optional[bool] = None,
-        key_name: Optional[str] = None,
+        wallet_name: Optional[str] = None,
     ):
         """Submit/Amend a simple liquidity commitment (LP) with a single amount on each side.
 
         Args:
-            wallet_name:
-                str, The name of the wallet which is placing the order
+            key_name:
+                str, The name of the key which is placing the order
             market_id:
                 str, The ID of the market to place the commitment on
             commitment_amount:
                 int, The amount in asset decimals of market asset to commit to
                  liquidity provision
             fee:
                 float, The fee level at which to set the LP fee
@@ -1204,14 +1243,16 @@
                 str, the reference point to use for the buy side of LP
             reference_sell:
                 str, the reference point to use for the sell side of LP
             delta_buy:
                 float, the offset from reference point for the buy side of LP
             delta_sell:
                 float, the offset from reference point for the sell side of LP
+            wallet_name:
+                str, The name of the wallet which is placing the order
         """
         asset_id = data_raw.market_info(
             market_id=market_id, data_client=self.trading_data_client_v2
         ).tradable_instrument.instrument.future.settlement_asset
 
         market_decimals = data.market_price_decimals(
             market_id=market_id, data_client=self.trading_data_client_v2
@@ -1239,42 +1280,40 @@
             wallet_name=wallet_name,
             is_amendment=is_amendment,
             key_name=key_name,
         )
 
     def has_liquidity_provision(
         self,
-        wallet_name: str,
+        key_name: str,
         market_id: str,
-        key_name: Optional[str] = None,
+        wallet_name: Optional[str] = None,
     ):
         return data.has_liquidity_provision(
             self.trading_data_client_v2,
             market_id,
-            party_id=self.wallet.public_key(wallet_name, key_name),
+            party_id=self.wallet.public_key(wallet_name=wallet_name, name=key_name),
         )
 
     def submit_liquidity(
         self,
-        wallet_name: str,
+        key_name: str,
         market_id: str,
         commitment_amount: float,
         fee: float,
         buy_specs: List[Tuple[str, float, int]],
         sell_specs: List[Tuple[str, float, int]],
         is_amendment: Optional[bool] = None,
-        key_name: Optional[str] = None,
+        wallet_name: Optional[str] = None,
     ):
         """Submit/Amend a custom liquidity profile.
 
         Args:
-            wallet_name:
-                str, the wallet name performing the action
-            wallet:
-                Wallet, wallet client
+            key_name:
+                str, the key name performing the action
             market_id:
                 str, The ID of the market to place the commitment on
             commitment_amount:
                 int, The amount in asset decimals of market asset to commit
                 to liquidity provision
             fee:
                 float, The fee level at which to set the LP fee
@@ -1283,24 +1322,22 @@
                 List[Tuple[str, int, int]], List of tuples, each containing a reference
                 point in their first position, a desired offset in their second and
                 a proportion in third
             sell_specs:
                 List[Tuple[str, int, int]], List of tuples, each containing a reference
                 point in their first position, a desired offset in their second and
                 a proportion in third
-            key_name:
-                optional, str name of key in wallet to use
+            is_amendment:
+                Optional bool, Is the submission an amendment to an existing provision
+                    If None, will query the network to check.
+            wallet_name:
+                optional, str name of wallet to use
         """
-        asset_id = data_raw.market_info(
-            market_id=market_id, data_client=self.trading_data_client_v2
-        ).tradable_instrument.instrument.future.settlement_asset
-
-        market_decimals = data.market_price_decimals(
-            market_id=market_id, data_client=self.trading_data_client_v2
-        )
+        asset_id = self.market_to_asset[market_id]
+        market_decimals = self.market_price_decimals[market_id]
 
         buy_specs = [
             (s[0], num_to_padded_int(s[1], market_decimals), s[2]) for s in buy_specs
         ]
         sell_specs = [
             (s[0], num_to_padded_int(s[1], market_decimals), s[2]) for s in sell_specs
         ]
@@ -1397,52 +1434,39 @@
         Args:
             live_only:
                 bool, default True, whether to filter out dead/cancelled deals
                     from result
 
         Returns:
             Dictionary mapping market ID -> Party ID -> Order ID -> Order detaails"""
-        with self.orders_lock:
-            order_dict = {}
-            for market_id, party_orders in self._order_state_from_feed.items():
-                for party_id, orders in party_orders.items():
-                    for order_id, order in orders.items():
-                        if not live_only or (
-                            order.status == vega_protos.vega.Order.Status.STATUS_ACTIVE
-                        ):
-                            order_dict.setdefault(market_id, {}).setdefault(
-                                party_id, {}
-                            )[order_id] = order
-        return order_dict
+        return self.data_cache.order_status_from_feed(live_only=live_only)
 
     def orders_for_party_from_feed(
         self,
-        wallet_name: str,
+        key_name: str,
         market_id: str,
         live_only: bool = True,
-        key_name: Optional[str] = None,
+        wallet_name: Optional[str] = None,
     ) -> Dict[str, data.Order]:
-        party_id = self.wallet.public_key(wallet_name, key_name)
-        return (
-            self.order_status_from_feed(live_only=live_only)
-            .get(market_id, {})
-            .get(party_id, {})
-        )
-
-    def transfer_status_from_feed(self, live_only: bool = True):
-        datetime = self.get_blockchain_time()
-
-        with self.transfers_lock:
-            transfers_dict = {}
-            for party_id, party_transfers in self._transfer_state_from_feed.items():
-                for transfer_id, transfer in party_transfers.items():
-                    deliver_on = int(transfer.one_off.deliver_on)
-                    if not live_only or (deliver_on != 0 and datetime < deliver_on):
-                        transfers_dict.setdefault(party_id, {})[transfer_id] = transfer
-        return transfers_dict
+        party_id = self.wallet.public_key(wallet_name=wallet_name, name=key_name)
+        return self.data_cache.orders_for_party_from_feed(
+            party_id=party_id, market_id=market_id, live_only=live_only
+        )
+
+    def transfer_status_from_feed(
+        self, live_only: bool = True, blockchain_time: Optional[int] = None
+    ):
+        blockchain_time = (
+            blockchain_time
+            if blockchain_time is not None or not live_only
+            else self.get_blockchain_time()
+        )
+        return self.data_cache.transfer_status_from_feed(
+            live_only=live_only, blockchain_time=blockchain_time
+        )
 
     @raw_data
     def liquidity_provisions(
         self,
         market_id: Optional[str] = None,
         party_id: Optional[str] = None,
     ) -> Optional[List[vega_protos.vega.LiquidityProvision]]:
@@ -1461,251 +1485,146 @@
         """
         return data_raw.liquidity_provisions(
             self.trading_data_client_v2, market_id=market_id, party_id=party_id
         )
 
     def party_liquidity_provisions(
         self,
-        wallet_name: str,
+        key_name: str,
         market_id: Optional[str] = None,
-        key_name: Optional[str] = None,
+        wallet_name: Optional[str] = None,
     ) -> Optional[List[vega_protos.vega.LiquidityProvision]]:
         """Loads the current liquidity provision(s) for a given market and/or party.
 
         Args:
+            key_name:
+                str, key name stored in metadata.
             market_id:
                 Optional[str], the ID of the market from which to
                     pull liquidity provisions
             party_id:
                 Optional[str], the ID of the party from which to
                     pull liquidity provisions
-            key_name:
-                Optional[str], key name stored in metadata. Defaults to None.
+            wallet_name:
+                Optional[str], Specify a different wallet name to default
 
         Returns:
             List[LiquidityProvision], list of liquidity provisions (if any exist)
         """
         return self.liquidity_provisions(
-            market_id=market_id, party_id=self.wallet.public_key(wallet_name, key_name)
-        )
-
-    def start_live_feeds(self):
-        self.start_order_monitoring()
-        self.start_transfer_monitoring()
-        self.start_trade_monitoring()
-
-        self._merge_streams()
-        self._observation_thread = threading.Thread(target=self._monitor_stream)
-        self._observation_thread.start()
-
-    def start_order_monitoring(
-        self,
-        market_ids: Optional[List[str]] = None,
-        party_ids: Optional[List[str]] = None,
-        use_core_client: bool = False,
-    ):
-        if use_core_client:
-            data_client = self.core_client
-        else:
-            data_client = self.trading_data_client_v2
-
-        order_queue = data.order_subscription(
-            data_client,
-            self.trading_data_client_v2,
-        )
-
-        base_orders = []
-        for market_party_tuple in list(
-            product(
-                (market_ids if market_ids is not None else [None]),
-                (party_ids if party_ids is not None else [None]),
-            )
-        ):
-            base_orders.extend(
-                data.list_orders(
-                    data_client=self.trading_data_client_v2,
-                    market_id=market_party_tuple[0],
-                    party_id=market_party_tuple[1],
-                    live_only=True,
-                )
-            )
-
-        with self.orders_lock:
-            for order in base_orders:
-                self._order_state_from_feed.setdefault(order.market_id, {}).setdefault(
-                    order.party_id, {}
-                )[order.id] = order
-
-        self._observation_feeds.append(order_queue)
-
-    def start_transfer_monitoring(
-        self,
-    ):
-        transfer_queue = data.transfer_subscription(
-            self.core_client,
-            self.trading_data_client_v2,
-        )
-
-        base_transfers = []
-
-        base_transfers.extend(
-            data.list_transfers(data_client=self.trading_data_client_v2)
-        )
-
-        with self.transfers_lock:
-            for t in base_transfers:
-                self._transfer_state_from_feed.setdefault(t.party_to, {})[t.id] = t
-        self._observation_feeds.append(transfer_queue)
-
-    def start_trade_monitoring(
-        self,
-    ):
-        trade_queue = data.trades_subscription(
-            self.core_client,
-            self.trading_data_client_v2,
+            market_id=market_id,
+            party_id=self.wallet.public_key(wallet_name=wallet_name, name=key_name),
         )
 
-        base_trades = []
-
-        with self.trades_lock:
-            self._trades_from_feed = base_trades
-        self._observation_feeds.append(trade_queue)
-
-    def _merge_streams(self) -> None:
-        self._merge_threads = []
-        for feed in self._observation_feeds:
-            merger = threading.Thread(
-                target=_queue_forwarder,
-                args=(feed, self._aggregated_observation_feed),
-                daemon=True,
-            )
-            self._merge_threads.append(merger)
-            merger.start()
-
-    def _monitor_stream(self) -> None:
-        while True:
-            if self._kill_thread_sig.is_set():
-                return
-            try:
-                update = self._aggregated_observation_feed.get(timeout=1)
-            except Empty:
-                continue
-            else:
-                if isinstance(update, data.Order):
-                    with self.orders_lock:
-                        if update.version >= getattr(
-                            self._order_state_from_feed.setdefault(update.market_id, {})
-                            .setdefault(update.party_id, {})
-                            .get(update.id, None),
-                            "version",
-                            0,
-                        ):
-                            self._order_state_from_feed[update.market_id][
-                                update.party_id
-                            ][update.id] = update
-
-                if isinstance(update, data.Transfer):
-                    with self.transfers_lock:
-                        self._transfer_state_from_feed.setdefault(update.party_to, {})[
-                            update.id
-                        ] = update
-
-                elif isinstance(update, data.Trade):
-                    with self.trades_lock:
-                        self._trades_from_feed.append(update)
-
     def margin_levels(
         self,
-        wallet_name: str,
+        key_name: str = None,
         market_id: Optional[str] = None,
-        key_name: Optional[str] = None,
+        wallet_name: Optional[str] = None,
     ) -> List[data.MarginLevels]:
         return data.margin_levels(
             self.trading_data_client_v2,
-            party_id=self.wallet.public_key(wallet_name, key_name),
+            party_id=self.wallet.public_key(wallet_name=wallet_name, name=key_name),
             market_id=market_id,
         )
 
     def list_orders(
         self,
-        wallet_name: str,
         key_name: str,
         market_id: str,
+        wallet_name: Optional[str] = None,
         reference: Optional[str] = None,
         live_only: Optional[bool] = True,
     ) -> List[data.Order]:
         """Return a list of orders for the specified market and party.
 
         Args:
-            wallet_name (str):
-                Name of wallet to return orders for.
             key_name (str):
                 Name of key to return orders for.
+            wallet_name (str):
+                Name of wallet to return orders for.
             market_id (str):
                 Id of market to return orders from.
             reference (Optional[str]):
                 Reference of matching orders to return.
             live_only (Optional[bool]):
                 Whether to return only live orders. Defaults to True.
 
         Returns:
             List[data.Order]:
                 List of orders for the specified market and party.
         """
         return data.list_orders(
             data_client=self.trading_data_client_v2,
             market_id=market_id,
-            party_id=self.wallet.public_key(name=wallet_name, key_name=key_name),
+            party_id=self.wallet.public_key(wallet_name=wallet_name, name=key_name),
             reference=reference,
             live_only=live_only,
         )
 
+    def get_ledger_entries_from_stream(
+        self,
+        wallet_name_from: Optional[str] = None,
+        key_name_from: Optional[str] = None,
+        wallet_name_to: Optional[str] = None,
+        key_name_to: Optional[str] = None,
+        transfer_type: Optional[str] = None,
+    ) -> List[data.LedgerEntry]:
+        return self.data_cache.get_ledger_entries_from_stream(
+            party_id_from=(
+                self.wallet.public_key(wallet_name=wallet_name_from, name=key_name_from)
+                if wallet_name_from is not None
+                else None
+            ),
+            party_id_to=(
+                self.wallet.public_key(wallet_name=wallet_name_to, name=key_name_to)
+                if wallet_name_to is not None
+                else None
+            ),
+            transfer_type=transfer_type,
+        )
+
     def get_trades_from_stream(
         self,
         market_id: Optional[str] = None,
         wallet_name: Optional[str] = None,
         key_name: Optional[str] = None,
         order_id: Optional[str] = None,
+        exclude_trade_ids: Optional[Set[str]] = None,
     ) -> List[data.Trade]:
         """Loads executed trades for a given query of party/market/specific order from
         data node. Converts values to proper decimal output.
 
         Args:
             market_id:
                 optional str, Restrict to trades on a specific market
             wallet_name:
                 optional str, Restrict to trades for a specific wallet
             key_name:
                 optional str, Select a different key to the default within a given wallet
             order_id:
                 optional str, Restrict to trades for a specific order
+            exclude_trade_ids:
+                optional set[str], Do not return trades with ID in this set
 
         Returns:
             List[Trade], list of formatted trade objects which match the required
                 restrictions.
         """
         party_id = (
-            self.wallet.public_key(wallet_name, key_name)
+            self.wallet.public_key(wallet_name=wallet_name, name=key_name)
             if key_name is not None
             else None
         )
-        with self.trades_lock:
-            results = []
-            for trade in self._trades_from_feed:
-                if party_id is not None and party_id not in (trade.buyer, trade.seller):
-                    continue
-                if market_id is not None and trade.market_id != market_id:
-                    continue
-                if order_id is not None and order_id not in (
-                    trade.buy_order,
-                    trade.sell_order,
-                ):
-                    continue
-                results.append(copy.copy(trade))
-        return results
+        return self.data_cache.get_trades_from_stream(
+            market_id=market_id,
+            party_id=party_id,
+            order_id=order_id,
+            exclude_trade_ids=exclude_trade_ids,
+        )
 
     def get_trades(
         self,
         market_id: str,
         wallet_name: Optional[str] = None,
         key_name: Optional[str] = None,
         order_id: Optional[str] = None,
@@ -1729,22 +1648,24 @@
         """
         if market_id is not None:
             self.market_pos_decimals[market_id]
             self.market_price_decimals[market_id]
             asset_dp = self.asset_decimals[self.market_to_asset[market_id]]
         return data.get_trades(
             self.trading_data_client_v2,
-            party_id=self.wallet.public_key(wallet_name, key_name)
-            if key_name is not None
-            else None,
+            party_id=(
+                self.wallet.public_key(wallet_name=wallet_name, name=key_name)
+                if key_name is not None
+                else None
+            ),
             market_id=market_id,
             order_id=order_id,
-            market_asset_decimals_map={market_id: asset_dp}
-            if market_id is not None
-            else None,
+            market_asset_decimals_map=(
+                {market_id: asset_dp} if market_id is not None else None
+            ),
             market_position_decimals_map=self.market_pos_decimals,
             market_price_decimals_map=self.market_price_decimals,
         )
 
     def create_order_amendment(
         self,
         order_id: str,
@@ -1817,17 +1738,17 @@
         return trading.order_amendment(
             order_id=order_id,
             market_id=market_id,
             price=str(price) if price is not None else price,
             size_delta=size_delta,
             expires_at=expires_at,
             time_in_force=time_in_force,
-            pegged_offset=str(pegged_offset)
-            if pegged_offset is not None
-            else pegged_offset,
+            pegged_offset=(
+                str(pegged_offset) if pegged_offset is not None else pegged_offset
+            ),
             pegged_reference=pegged_reference,
         )
 
     def create_order_cancellation(
         self,
         order_id: str,
         market_id: str,
@@ -1952,16 +1873,16 @@
             order_type=order_type,
             reference=reference,
             pegged_order=pegged_order,
         )
 
     def submit_instructions(
         self,
-        wallet_name: str,
-        key_name: Optional[str] = None,
+        key_name: str,
+        wallet_name: Optional[str] = None,
         cancellations: Optional[List[OrderCancellation]] = None,
         amendments: Optional[List[OrderAmendment]] = None,
         submissions: Optional[List[OrderSubmission]] = None,
     ):
         """Submits a batch of market instructions to be processed sequentially.
 
         Method allows lists of order cancellations, order amendments, and order
@@ -1969,18 +1890,18 @@
         order cancellations, amendments, then submissions.
 
         If the number of cancellation, amendment, and submission instructions exceed
         the network parameter spam.protection.max.batchSize, the function will submit
         the instructions in multiple batches adhering to the above rules.
 
         Args:
-            wallet_name (str):
+            key_name (str):
+                Name of key to submit transaction from.
+            wallet_name (Optional str):
                 Name of wallet to submit transaction from.
-            key_name (Optional[str], optional):
-                Name of key to submit transaction from. Defaults to None.
             cancellations (Optional[ List[OrderCancellation] ]):
                 List of OrderCancellation objects to submit. Defaults to None.
             amendments (Optional[ List[OrderAmendment] ]):
                 List of OrderAmendment objects to submit. Defaults to None.
             submissions (Optional[ List[OrderSubmission] ]):
                 List of OrderSubmission objects to submit. Defaults to None.
         """
@@ -2077,46 +1998,46 @@
         # Ping datanode then check if it is behind
         data.ping(data_client=self.trading_data_client_v2)
         if abs(self.get_blockchain_time() - time.time()) > max_time_diff:
             raise DatanodeBehindError
 
     def one_off_transfer(
         self,
-        from_wallet_name: str,
-        to_wallet_name: str,
+        from_key_name: str,
+        to_key_name: str,
         from_account_type: vega_protos.vega.AccountType,
         to_account_type: vega_protos.vega.AccountType,
         asset: str,
         amount: float,
         reference: Optional[str] = None,
-        from_key_name: Optional[str] = None,
-        to_key_name: Optional[str] = None,
+        from_wallet_name: Optional[str] = None,
+        to_wallet_name: Optional[str] = None,
         delay: Optional[int] = None,
     ):
         """Submit a one off transfer command.
 
         Args:
-            from_wallet_name (str):
-                Name of wallet to transfer from.
-            to_wallet_name (str):
-                Name of wallet to transfer to.
+            from_key_name (str):
+                Name of key in wallet to send from.
+            to_key_name (str):
+                Name of key in wallet to send to.
             from_account_type (vega_protos.vega.AccountType):
                 Type of Vega account to transfer from.
             to_account_type (vega_protos.vega.AccountType):
                 Type of Vega account to transfer to.
             asset (str):
                 Id of asset to transfer.
             amount (float):
                 Amount of asset to transfer.
             reference (Optional[str], optional):
                 Reference to assign to transfer. Defaults to None.
-            from_key_name (Optional[str], optional):
-                Name of key in wallet to send from. Defaults to None.
-            to_key_name (Optional[str], optional):
-                Name of key in wallet to send to. Defaults to None.
+            from_wallet_name (Optional[str], optional):
+                Name of wallet to transfer from.
+            to_wallet_name (Optional[str], optional):
+                Name of wallet to transfer to.
             delay (Optional[int], optional):
                 Delay in seconds to add before transfer is sent. Defaults to None.
         """
 
         adp = self.asset_decimals[asset]
 
         one_off = vega_protos.commands.v1.commands.OneOffTransfer()
@@ -2124,15 +2045,15 @@
             setattr(one_off, "deliver_on", self.get_blockchain_time() + delay)
 
         trading.transfer(
             wallet=self.wallet,
             wallet_name=from_wallet_name,
             key_name=from_key_name,
             from_account_type=from_account_type,
-            to=self.wallet.public_key(name=to_wallet_name, key_name=to_key_name),
+            to=self.wallet.public_key(wallet_name=to_wallet_name, name=to_key_name),
             to_account_type=to_account_type,
             asset=asset,
             amount=str(num_to_padded_int(amount, adp)),
             reference=reference,
             one_off=one_off,
         )
 
@@ -2154,15 +2075,15 @@
 
         Returns:
             List[Transfer]:
                 A list of processed Transfer objects for the specified party and direction.
         """
 
         party_id = (
-            self.wallet.public_key(name=wallet_name, key_name=key_name)
+            self.wallet.public_key(wallet_name=wallet_name, name=key_name)
             if wallet_name is not None
             else None
         )
 
         return data.list_transfers(
             data_client=self.trading_data_client_v2,
             party_id=party_id,
@@ -2186,18 +2107,19 @@
                 Name of specific key in wallet to get public key for. Defaults to None.
         """
 
         return data.get_liquidity_fee_shares(
             data_client=self.trading_data_client_v2,
             market_id=market_id,
             party_id=(
-                self.wallet.public_key(name=wallet_name, key_name=key_name)
+                self.wallet.public_key(wallet_name=wallet_name, name=key_name)
                 if wallet_name is not None
                 else None
             ),
+            market_data=self.market_data_from_feed(market_id=market_id),
         )
 
     def list_ledger_entries(
         self,
         close_on_account_filters: bool = False,
         asset_id: Optional[str] = None,
         from_party_ids: Optional[List[str]] = None,
```

### Comparing `vega_sim-0.67.0/vega_sim/tools/scenario_output.py` & `vega_sim-1.0.1/vega_sim/tools/scenario_output.py`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/tools/scenario_plots.py` & `vega_sim-1.0.1/vega_sim/tools/scenario_plots.py`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/vegahome/config/node/config.toml` & `vega_sim-1.0.1/vega_sim/vegahome/config/node/config.toml`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/vegahome/data/faucet/wallets/vega.1639051237294446827` & `vega_sim-1.0.1/vega_sim/vegahome/data/faucet/wallets/vega.1639051237294446827`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/vegahome/data/faucet/wallets/vega.1641976836892788243` & `vega_sim-1.0.1/vega_sim/vegahome/data/faucet/wallets/vega.1641976836892788243`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977214518086643` & `vega_sim-1.0.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977214518086643`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977270881740938` & `vega_sim-1.0.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977270881740938`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977376563008654` & `vega_sim-1.0.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977376563008654`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977471442889253` & `vega_sim-1.0.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977471442889253`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977537535784009` & `vega_sim-1.0.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977537535784009`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977956797580358` & `vega_sim-1.0.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977956797580358`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/vegahome/data/faucet/wallets/vega.1641978034856367487` & `vega_sim-1.0.1/vega_sim/vegahome/data/faucet/wallets/vega.1641978034856367487`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/vegahome/data/faucet/wallets/vega.1643100690865690276` & `vega_sim-1.0.1/vega_sim/vegahome/data/faucet/wallets/vega.1643100690865690276`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/vegahome/data/node/wallets/vega/vega.1639051228296308758` & `vega_sim-1.0.1/vega_sim/vegahome/data/node/wallets/vega/vega.1639051228296308758`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/vegahome/data/node/wallets/vega/vega.1641977668033624243` & `vega_sim-1.0.1/vega_sim/vegahome/data/node/wallets/vega/vega.1641977668033624243`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/vegahome/data/node/wallets/vega/vega.1641977838095755067` & `vega_sim-1.0.1/vega_sim/vegahome/data/node/wallets/vega/vega.1641977838095755067`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/vegahome/data/node/wallets/vega/vega.1641977916225009082` & `vega_sim-1.0.1/vega_sim/vegahome/data/node/wallets/vega/vega.1641977916225009082`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/vegahome/data/node/wallets/vega/vega.1641977947934016124` & `vega_sim-1.0.1/vega_sim/vegahome/data/node/wallets/vega/vega.1641977947934016124`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/vegahome/data/wallet-service/rsa-keys/private.pem` & `vega_sim-1.0.1/vega_sim/vegahome/data/wallet-service/rsa-keys/private.pem`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/vegahome/data/wallet-service/rsa-keys/public.pem` & `vega_sim-1.0.1/vega_sim/vegahome/data/wallet-service/rsa-keys/public.pem`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/vegahome/genesis.json` & `vega_sim-1.0.1/vega_sim/vegahome/genesis.json`

 * *Files identical despite different names*

### Comparing `vega_sim-0.67.0/vega_sim/wallet/base.py` & `vega_sim-1.0.1/vega_sim/wallet/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,60 @@
-from abc import ABC
-from typing import Any
+from abc import ABC, abstractmethod
+from typing import Any, Optional
 
 VEGA_DEFAULT_KEY_NAME = "foo"
+DEFAULT_WALLET_NAME = "MarketSim"
 
 
 class Wallet(ABC):
-    def create_wallet(
+    @abstractmethod
+    def create_key(
         self,
         name: str,
-        passphrase: str,
+        wallet_name: Optional[str] = None,
     ) -> str:
-        """Generates a new wallet from a name - passphrase pair in the given vega service.
+        """Generates a new wallet key in the given vega service.
 
         Args:
             name:
-                str, The name to use for the wallet
-            passphrase:
-                str, The passphrase to use when logging in to created wallet in future
+                str, The name to use for the wallet key
+            wallet_name:
+                str, The wallet to use if not the default
         Returns:
             str, login token to use in authenticated requests
         """
         pass
 
-    def login(self, name: str, passphrase: str) -> str:
-        """Logs in to existing wallet in the given vega service.
-
-        Args:
-            name:
-                str, The name of the wallet
-            passphrase:
-                str, The login passphrase used when creating the wallet
-        Returns:
-            str, login token to use in authenticated requests
-        """
-        pass
-
-    def submit_transaction(self, transaction: Any, name: str, transaction_type: str):
+    @abstractmethod
+    def submit_transaction(
+        self,
+        transaction: Any,
+        key_name: str,
+        transaction_type: str,
+        wallet_name: Optional[str],
+    ):
         """Submits a transaction to Vega core via wallet
 
         Args:
             transaction:
                 Any, The transaction object which will be submitted
             name:
                 str, The name to use for the wallet executing the transaction
             transaction_type:
                 str, The name, in underscore case, of the transaction
         """
         pass
 
-    def public_key(self, name: str) -> str:
-        """Return the public key associated with a given wallet name.
+    @abstractmethod
+    def public_key(
+        self,
+        name: str,
+        wallet_name: Optional[str] = None,
+    ) -> str:
+        """Return the public key associated with a given key name.
 
         Args:
             name:
                 str, The name to use for the wallet
 
         Returns:
             str, public key
```

### Comparing `vega_sim-0.67.0/vega_sim/wallet/slim_wallet.py` & `vega_sim-1.0.1/vega_sim/wallet/slim_wallet.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,47 +13,37 @@
 from vega_sim.grpc.client import VegaCoreClient
 from vega_sim.wallet.base import Wallet
 
 import vega_sim.proto.vega.api.v1.core_pb2 as core_proto
 import vega_sim.proto.vega.commands.v1.transaction_pb2 as transaction_proto
 import vega_sim.proto.vega.commands.v1.signature_pb2 as signature_proto
 from vega_sim.wallet.vega_wallet import VegaWallet
-from vega_sim.wallet.base import VEGA_DEFAULT_KEY_NAME
+from vega_sim.wallet.base import DEFAULT_WALLET_NAME
 
 logger = getLogger(__name__)
 
 
 class SlimWallet(Wallet):
     def __init__(
         self,
         core_client: VegaCoreClient,
-        height_update_frequency: int = 500,
         full_wallet: Optional[VegaWallet] = None,
-        full_wallet_default_pass: str = "passwd",
         store_transactions: bool = False,
         log_dir: Optional[str] = None,
     ):
         """Creates a wallet to running key generation internally
         and directly sending transactions to the Core node
 
         Args:
             core_client:
                 VegaCoreClient, client for vega core interaction
-            height_update_frequency:
-                int, default 500, how frequently to update the block height parameter
-                    for transactions (e.g. 500 will update every 500 calls to
-                    submit_transaction).
             full_wallet:
                 Optional[VegaWallet], optional full wallet backing. This will be used
                     for creating keypairs instead of generating them locally, making it
                     possible to connect to the Console
-            full_wallet_default_pass:
-                str, default 'passwd', If full wallet is passed, the password used
-                    when creating dummy accounts if none are passed.
-                    Use this password to log in to the Vega Console
             store_transactions:
                 bool, default False, If True will store every transaction sent into
                     a file, allowing replay of the chain without going through full
                     logic of actors etc
         """
         self.core_client = core_client
         self.keys = {}
@@ -63,30 +53,29 @@
         self.pool = ThreadPoolExecutor(max_workers=5)
 
         self.height_update_frequency = 500
         self.remaining_until_height_update = 0
         self.block_height = None
 
         self.vega_wallet = full_wallet
-        self.full_wallet_default_pass = full_wallet_default_pass
 
         self.store_transactions = store_transactions
         self.log_dir = log_dir
 
         # If it turns out that customising these is useful it's trivial to
         # make a parameter
         self.num_sigs_to_create = 1000000
         self.num_nonces_to_create = 1000000
 
         self._create_nonces()
         self._create_sigs()
 
         dotenv.load_dotenv()
-        self.vega_default_key_name = os.environ.get(
-            "VEGA_DEFAULT_KEY_NAME", VEGA_DEFAULT_KEY_NAME
+        self.vega_default_wallet_name = os.environ.get(
+            "VEGA_DEFAULT_WALLET_NAME", DEFAULT_WALLET_NAME
         )
 
     def _create_sigs(self):
         self.sigs = [os.urandom(6).hex() for _ in range(self.num_sigs_to_create)]
 
     def _create_nonces(self):
         self.nonces = np.random.randint(0, 100000, size=self.num_nonces_to_create)
@@ -101,74 +90,69 @@
     def _next_nonce(self) -> int:
         self.nonce_idx += 1
         if self.nonce_idx >= self.num_nonces_to_create:
             self.nonce_idx = 0
             self._create_nonces()
         return self.nonces[self.nonce_idx]
 
-    def create_wallet(
+    def create_key(
         self,
         name: str,
-        passphrase: Optional[str] = None,
-        key_name: Optional[str] = None,
-    ) -> None:
-        """Generates a new wallet from a name - passphrase pair in the given vega service.
+        wallet_name: Optional[str] = None,
+    ) -> str:
+        """Generates a new wallet key in the given vega service.
 
         Args:
             name:
-                str, The name to use for the wallet
+                str, The name to use for the wallet key
+            wallet_name:
+                str, The wallet to use if not the default
+        Returns:
+            str, login token to use in authenticated requests
         """
-        passphrase = (
-            passphrase if passphrase is not None else self.full_wallet_default_pass
+        wallet_name = (
+            wallet_name if wallet_name is not None else self.vega_default_wallet_name
         )
-        key_name = key_name if key_name is not None else self.vega_default_key_name
 
-        if name not in self.keys:
-            self.keys[name] = {}
-        if name not in self.pub_keys:
-            self.pub_keys[name] = {}
+        if wallet_name not in self.keys:
+            self.keys[wallet_name] = {}
+        if wallet_name not in self.pub_keys:
+            self.pub_keys[wallet_name] = {}
 
         if self.vega_wallet is None:
-            self.keys[name][key_name] = SigningKey.generate()
-            self.pub_keys[name][key_name] = (
-                self.keys[name][key_name].verify_key.encode(encoder=HexEncoder).decode()
+            self.keys[wallet_name][name] = SigningKey.generate()
+            self.pub_keys[wallet_name][name] = (
+                self.keys[wallet_name][name]
+                .verify_key.encode(encoder=HexEncoder)
+                .decode()
             )
 
         else:
-            self.vega_wallet.create_wallet(
+            self.vega_wallet.create_key(
                 name=name,
-                passphrase=passphrase,
-                key_name=key_name,
+                wallet_name=wallet_name,
+            )
+            self.pub_keys[wallet_name][name] = self.vega_wallet.public_key(
+                name, wallet_name
             )
-            self.pub_keys[name][key_name] = self.vega_wallet.public_key(name, key_name)
-
-    def login(self, name: str, **kwargs) -> None:
-        """Logs in to existing wallet in the given vega service.
-
-        Args:
-            name:
-                str, The name of the wallet
-        """
-        if name not in self.keys:
-            self.create_wallet(name=name)
 
     def submit_transaction(
         self,
-        name: str,
+        key_name: str,
         transaction: Any,
         transaction_type: str,
-        key_name: Optional[str] = None,
+        wallet_name: Optional[str] = None,
     ):
         # if self.remaining_until_height_update <= 0:
         #     self.block_height = self.core_client.LastBlockHeight(
         #         core_proto.LastBlockHeightRequest()
         #     ).height
         #     self.remaining_until_height_update = self.height_update_frequency
 
-        pub_key = self.public_key(name=name, key_name=key_name)
+        pub_key = self.public_key(name=key_name, wallet_name=wallet_name)
 
         transaction_info = {transaction_type: transaction}
         input_data = transaction_proto.InputData(
             nonce=self._next_nonce(),  # block_height=self.block_height,
             **transaction_info
         )
 
@@ -196,24 +180,24 @@
         self.pool.submit(lambda: submit_future.result())
         self.remaining_until_height_update -= 1
 
     def submit_raw_transaction(self, transaction: core_proto.SubmitTransactionRequest):
         submit_future = self.core_client.SubmitTransaction.future(transaction)
         self.pool.submit(lambda: submit_future.result())
 
-    def public_key(self, name: str, key_name: Optional[str] = None) -> str:
+    def public_key(self, name: str, wallet_name: Optional[str] = None) -> str:
         """Return a public key for the given wallet name and key name.
 
         Args:
             name (str):
-                Name of the wallet.
-            key_name (str):
-                Name of the key. Defaults to None.
+                Name of the key.
+            wallet_name (str):
+                Name of the wallet. Defaults to None.
 
         Returns:
             str, public key
         """
 
-        if key_name is None:
-            return self.pub_keys[name][self.vega_default_key_name]
+        if wallet_name is None:
+            return self.pub_keys[self.vega_default_wallet_name][name]
         else:
-            return self.pub_keys[name][key_name]
+            return self.pub_keys[wallet_name][name]
```

### Comparing `vega_sim-0.67.0/setup.py` & `vega_sim-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,30 +44,31 @@
  'vega_sim.scenario.ideal_market_maker',
  'vega_sim.scenario.ideal_market_maker.utils',
  'vega_sim.scenario.ideal_market_maker_v2',
  'vega_sim.scenario.ideal_market_maker_v2.utils',
  'vega_sim.scenario.market_crash',
  'vega_sim.scenario.multi_market',
  'vega_sim.scenario.parameter_experiment',
+ 'vega_sim.scenario.realtime_market',
  'vega_sim.tools',
  'vega_sim.wallet']
 
 package_data = \
 {'': ['*'],
  'vega_sim': ['vegahome/*',
               'vegahome/config/data-node/*',
               'vegahome/config/faucet/*',
               'vegahome/config/node/*',
+              'vegahome/config/wallet-service/*',
               'vegahome/config/wallet-service/networks/*',
               'vegahome/data/*',
               'vegahome/data/faucet/wallets/*',
               'vegahome/data/node/wallets/ethereum/*',
               'vegahome/data/node/wallets/vega/*',
-              'vegahome/data/wallet-service/rsa-keys/*',
-              'vegahome/data/wallets/*'],
+              'vegahome/data/wallet-service/rsa-keys/*'],
  'vega_sim.reinforcement': ['theory_intro/*', 'theory_intro/images/*']}
 
 install_requires = \
 ['PyNaCl>=1.5.0,<2.0.0',
  'deprecated>=1.2.13,<2.0.0',
  'grpc-gateway-protoc-gen-openapiv2>=0.1.0,<0.2.0',
  'grpcio-tools==1.48.1',
@@ -89,15 +90,15 @@
  'learning': ['torch==1.12.1',
               'tqdm>=4.64.0,<5.0.0',
               'matplotlib>=3.5.2,<4.0.0'],
  'profile': ['snakeviz>=2.1.1,<3.0.0', 'pytest-profiling>=1.7.0,<2.0.0']}
 
 setup_kwargs = {
     'name': 'vega-sim',
-    'version': '0.67.0',
+    'version': '1.0.1',
     'description': 'Simulator for running self-contained Vega chain on local PC',
     'long_description': 'None',
     'author': 'Tom McLean',
     'author_email': 'tom@vegaprotocol.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `vega_sim-0.67.0/PKG-INFO` & `vega_sim-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vega-sim
-Version: 0.67.0
+Version: 1.0.1
 Summary: Simulator for running self-contained Vega chain on local PC
 License: MIT
 Author: Tom McLean
 Author-email: tom@vegaprotocol.io
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

