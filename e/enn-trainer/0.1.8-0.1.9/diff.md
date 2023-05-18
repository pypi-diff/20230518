# Comparing `tmp/enn-trainer-0.1.8.tar.gz` & `tmp/enn-trainer-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enn-trainer-0.1.8.tar", max compression
+gzip compressed data, was "enn-trainer-0.1.9.tar", max compression
```

## Comparing `enn-trainer-0.1.8.tar` & `enn-trainer-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     9693 2022-07-15 03:25:18.253790 enn-trainer-0.1.8/LICENSE-APACHE
--rw-r--r--   0        0        0     1088 2022-07-15 03:25:18.257790 enn-trainer-0.1.8/LICENSE-MIT
--rw-r--r--   0        0        0      666 2022-07-15 03:25:18.257790 enn-trainer-0.1.8/enn_trainer/__init__.py
--rw-r--r--   0        0        0     2570 2022-07-15 03:25:18.257790 enn-trainer-0.1.8/enn_trainer/agent.py
--rw-r--r--   0        0        0     8923 2022-07-15 03:25:18.257790 enn-trainer-0.1.8/enn_trainer/config.py
--rw-r--r--   0        0        0     5136 2022-07-15 03:25:18.257790 enn-trainer-0.1.8/enn_trainer/eval.py
--rw-r--r--   0        0        0     2131 2022-07-15 03:25:18.257790 enn-trainer-0.1.8/enn_trainer/gae.py
--rw-r--r--   0        0        0    20155 2022-07-15 03:25:18.257790 enn-trainer-0.1.8/enn_trainer/hypertuna.py
--rw-r--r--   0        0        0      824 2022-07-15 03:25:18.257790 enn-trainer-0.1.8/enn_trainer/load_checkpoint.py
--rw-r--r--   0        0        0     4067 2022-07-15 03:25:18.257790 enn-trainer-0.1.8/enn_trainer/ppo.py
--rw-r--r--   0        0        0        0 2022-07-15 03:25:18.257790 enn-trainer-0.1.8/enn_trainer/py.typed
--rw-r--r--   0        0        0     8241 2022-07-15 03:25:18.257790 enn-trainer-0.1.8/enn_trainer/rollout.py
--rw-r--r--   0        0        0    13023 2022-07-15 03:25:18.257790 enn-trainer-0.1.8/enn_trainer/supervised.py
--rw-r--r--   0        0        0      905 2022-07-15 03:25:18.257790 enn-trainer-0.1.8/enn_trainer/tests/test_configs.py
--rw-r--r--   0        0        0     5719 2022-07-15 03:25:18.257790 enn-trainer-0.1.8/enn_trainer/tests/test_training.py
--rw-r--r--   0        0        0    27240 2022-07-15 03:25:18.261790 enn-trainer-0.1.8/enn_trainer/train.py
--rw-r--r--   0        0        0      768 2022-07-15 03:25:18.261790 enn-trainer-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1014 2022-07-15 03:26:01.778650 enn-trainer-0.1.8/setup.py
--rw-r--r--   0        0        0      905 2022-07-15 03:26:01.778976 enn-trainer-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     9693 2022-07-28 15:39:18.851989 enn-trainer-0.1.9/LICENSE-APACHE
+-rw-r--r--   0        0        0     1088 2022-07-28 15:39:18.851989 enn-trainer-0.1.9/LICENSE-MIT
+-rw-r--r--   0        0        0      666 2022-07-28 15:39:18.855989 enn-trainer-0.1.9/enn_trainer/__init__.py
+-rw-r--r--   0        0        0     2570 2022-07-28 15:39:18.855989 enn-trainer-0.1.9/enn_trainer/agent.py
+-rw-r--r--   0        0        0     8923 2022-07-28 15:39:18.855989 enn-trainer-0.1.9/enn_trainer/config.py
+-rw-r--r--   0        0        0     5136 2022-07-28 15:39:18.855989 enn-trainer-0.1.9/enn_trainer/eval.py
+-rw-r--r--   0        0        0     2131 2022-07-28 15:39:18.855989 enn-trainer-0.1.9/enn_trainer/gae.py
+-rw-r--r--   0        0        0    20202 2022-07-28 15:39:18.855989 enn-trainer-0.1.9/enn_trainer/hypertuna.py
+-rw-r--r--   0        0        0      824 2022-07-28 15:39:18.855989 enn-trainer-0.1.9/enn_trainer/load_checkpoint.py
+-rw-r--r--   0        0        0     4067 2022-07-28 15:39:18.855989 enn-trainer-0.1.9/enn_trainer/ppo.py
+-rw-r--r--   0        0        0        0 2022-07-28 15:39:18.855989 enn-trainer-0.1.9/enn_trainer/py.typed
+-rw-r--r--   0        0        0     8241 2022-07-28 15:39:18.855989 enn-trainer-0.1.9/enn_trainer/rollout.py
+-rw-r--r--   0        0        0    13023 2022-07-28 15:39:18.855989 enn-trainer-0.1.9/enn_trainer/supervised.py
+-rw-r--r--   0        0        0      905 2022-07-28 15:39:18.855989 enn-trainer-0.1.9/enn_trainer/tests/test_configs.py
+-rw-r--r--   0        0        0     5719 2022-07-28 15:39:18.855989 enn-trainer-0.1.9/enn_trainer/tests/test_training.py
+-rw-r--r--   0        0        0    27487 2022-07-28 15:39:18.855989 enn-trainer-0.1.9/enn_trainer/train.py
+-rw-r--r--   0        0        0      768 2022-07-28 15:39:18.855989 enn-trainer-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1014 2022-07-28 15:40:07.010604 enn-trainer-0.1.9/setup.py
+-rw-r--r--   0        0        0      905 2022-07-28 15:40:07.011028 enn-trainer-0.1.9/PKG-INFO
```

### Comparing `enn-trainer-0.1.8/LICENSE-APACHE` & `enn-trainer-0.1.9/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `enn-trainer-0.1.8/LICENSE-MIT` & `enn-trainer-0.1.9/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `enn-trainer-0.1.8/enn_trainer/__init__.py` & `enn-trainer-0.1.9/enn_trainer/__init__.py`

 * *Files identical despite different names*

### Comparing `enn-trainer-0.1.8/enn_trainer/agent.py` & `enn-trainer-0.1.9/enn_trainer/agent.py`

 * *Files identical despite different names*

### Comparing `enn-trainer-0.1.8/enn_trainer/config.py` & `enn-trainer-0.1.9/enn_trainer/config.py`

 * *Files identical despite different names*

### Comparing `enn-trainer-0.1.8/enn_trainer/eval.py` & `enn-trainer-0.1.9/enn_trainer/eval.py`

 * *Files identical despite different names*

### Comparing `enn-trainer-0.1.8/enn_trainer/gae.py` & `enn-trainer-0.1.9/enn_trainer/gae.py`

 * *Files identical despite different names*

### Comparing `enn-trainer-0.1.8/enn_trainer/hypertuna.py` & `enn-trainer-0.1.9/enn_trainer/hypertuna.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,19 @@
 from distutils.util import strtobool
 from enum import Enum
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
 import numpy as np
 import optuna
 import wandb
-import xprun  # type: ignore
+
+try:
+    import xprun  # type: ignore
+except ImportError:
+    xprun = None
 
 logger = logging.getLogger(__name__)
 
 
 class SamplingStrategy(Enum):
     OMINUS = 0
     POWER_OF_TWO = 1
```

### Comparing `enn-trainer-0.1.8/enn_trainer/load_checkpoint.py` & `enn-trainer-0.1.9/enn_trainer/load_checkpoint.py`

 * *Files identical despite different names*

### Comparing `enn-trainer-0.1.8/enn_trainer/ppo.py` & `enn-trainer-0.1.9/enn_trainer/ppo.py`

 * *Files identical despite different names*

### Comparing `enn-trainer-0.1.8/enn_trainer/rollout.py` & `enn-trainer-0.1.9/enn_trainer/rollout.py`

 * *Files identical despite different names*

### Comparing `enn-trainer-0.1.8/enn_trainer/supervised.py` & `enn-trainer-0.1.9/enn_trainer/supervised.py`

 * *Files identical despite different names*

### Comparing `enn-trainer-0.1.8/enn_trainer/tests/test_configs.py` & `enn-trainer-0.1.9/enn_trainer/tests/test_configs.py`

 * *Files identical despite different names*

### Comparing `enn-trainer-0.1.8/enn_trainer/tests/test_training.py` & `enn-trainer-0.1.9/enn_trainer/tests/test_training.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,13 +191,13 @@
         env=EnvConfig(id="RockPaperScissors"),
         rollout=RolloutConfig(steps=1, num_envs=256),
         optim=OptimizerConfig(bs=64, lr=0.01),
         ppo=PPOConfig(ent_coef=0.1),
     )
     meanrew = _train(cfg)
     print(f"Final mean reward: {meanrew}")
-    assert 0.8 <= meanrew <= 1.1
+    assert 0.8 <= meanrew <= 1.2
 
     cfg.env.kwargs = '{"cheat": true}'
     meanrew = _train(cfg)
     print(f"Final mean reward: {meanrew}")
     assert meanrew > 1.9
```

### Comparing `enn-trainer-0.1.8/enn_trainer/train.py` & `enn-trainer-0.1.9/enn_trainer/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,21 +101,23 @@
         return RogueNet(
             RogueNetConfig(),
             obs_space,
             dict(action_space),
             regression_heads={"value": 1},
         ).to(device)
     else:
-        return StateManager(
+        agent = StateManager(
             TrainConfig,
             State,
             init_train_state,
             init_path=path,
             ignore_extra_fields=True,
-        ).state.agent.to(device)
+        ).state.agent
+        agent.set_obs_filter(obs_space)
+        return agent.to(device)
 
 
 @dataclass
 class State(hyperstate.Lazy):
     """
     Mutable state of training run.
 
@@ -337,14 +339,15 @@
 
     start_time = time.time()
     num_updates = cfg.total_timesteps // (cfg.rollout.num_envs * cfg.rollout.steps)
     initial_step = state.step
     for update in range(
         1 + initial_step // (cfg.rollout.num_envs * cfg.rollout.steps), num_updates + 1
     ):
+        update_start_time = time.time()
         if (
             cfg.eval is not None
             and state.next_eval_step is not None
             and rollout.global_step * parallelism >= state.next_eval_step
         ):
             state.next_eval_step += cfg.eval.interval
             _run_eval()
@@ -598,15 +601,19 @@
                         for i, label in enumerate(space.index_to_label):
                             writer.add_scalar(
                                 f"actions/{action_name}/{label}",
                                 np.sum(_actions == i).item() / len(_actions),
                                 global_step,
                             )
 
-            fps = (global_step - initial_step) / (time.time() - start_time)
+            fps = (
+                cfg.rollout.num_envs
+                * cfg.rollout.steps
+                / (time.time() - update_start_time)
+            )
             digits = int(np.ceil(np.log10(cfg.total_timesteps)))
             episodic_reward = metrics["episodic_reward"].mean
             episode_length = metrics["episode_length"].mean
             episode_count = metrics["episode_length"].count
             mean_reward = metrics["reward"].mean
 
             def green(s: str) -> str:
@@ -637,14 +644,15 @@
             )
             # fmt: on
             writer.add_scalar(
                 "charts/SPS",
                 int((global_step - initial_step) / (time.time() - start_time)),
                 global_step,
             )
+            writer.add_scalar("throughput", fps, global_step)
         tracer.end("metrics")
         tracer.end("update")
         traces = tracer.finish()
         if rank == 0:
             for callstack, timing in traces.items():
                 writer.add_scalar(f"trace/{callstack}", timing, global_step)
```

### Comparing `enn-trainer-0.1.8/pyproject.toml` & `enn-trainer-0.1.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "enn-trainer"
-version = "0.1.8"
+version = "0.1.9"
 description = "PPO and supervised training loops compatible with entity-gym"
 authors = ["Clemens Winter <clemenswinter1@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.7.1,<3.10"
 numpy = "^1.21.4"
 tensorboard = "^2.7.0"
 msgpack = "^1.0.3"
 msgpack-numpy = "^0.4.7"
 tqdm = "^4.62.3"
-ragged-buffer = "^0.3.9"
+ragged-buffer = "^0.4.3"
 wandb = "^0.12.7"
 optuna = "^2.10.0"
 moviepy = "^1.0.3"
 click = "^8.0.4"
 hyperstate = "^0.4.1"
-entity-gym = "^0.1.4"
-rogue-net = "^0.1.5"
+entity-gym = "^0.1.6"
+rogue-net = "^0.1.6"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "^2.19.0"
 pytest = "^7.1.2"
 black = "^22.3.0"
 mypy = "^0.950"
 Sphinx = "^4.5.0"
```

### Comparing `enn-trainer-0.1.8/setup.py` & `enn-trainer-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 ['enn_trainer', 'enn_trainer.tests']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['click>=8.0.4,<9.0.0',
- 'entity-gym>=0.1.4,<0.2.0',
+ 'entity-gym>=0.1.6,<0.2.0',
  'hyperstate>=0.4.1,<0.5.0',
  'moviepy>=1.0.3,<2.0.0',
  'msgpack-numpy>=0.4.7,<0.5.0',
  'msgpack>=1.0.3,<2.0.0',
  'numpy>=1.21.4,<2.0.0',
  'optuna>=2.10.0,<3.0.0',
- 'ragged-buffer>=0.3.9,<0.4.0',
- 'rogue-net>=0.1.5,<0.2.0',
+ 'ragged-buffer>=0.4.3,<0.5.0',
+ 'rogue-net>=0.1.6,<0.2.0',
  'tensorboard>=2.7.0,<3.0.0',
  'tqdm>=4.62.3,<5.0.0',
  'wandb>=0.12.7,<0.13.0']
 
 setup_kwargs = {
     'name': 'enn-trainer',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'PPO and supervised training loops compatible with entity-gym',
     'long_description': None,
     'author': 'Clemens Winter',
     'author_email': 'clemenswinter1@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `enn-trainer-0.1.8/PKG-INFO` & `enn-trainer-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: enn-trainer
-Version: 0.1.8
+Version: 0.1.9
 Summary: PPO and supervised training loops compatible with entity-gym
 Author: Clemens Winter
 Author-email: clemenswinter1@gmail.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: click (>=8.0.4,<9.0.0)
-Requires-Dist: entity-gym (>=0.1.4,<0.2.0)
+Requires-Dist: entity-gym (>=0.1.6,<0.2.0)
 Requires-Dist: hyperstate (>=0.4.1,<0.5.0)
 Requires-Dist: moviepy (>=1.0.3,<2.0.0)
 Requires-Dist: msgpack (>=1.0.3,<2.0.0)
 Requires-Dist: msgpack-numpy (>=0.4.7,<0.5.0)
 Requires-Dist: numpy (>=1.21.4,<2.0.0)
 Requires-Dist: optuna (>=2.10.0,<3.0.0)
-Requires-Dist: ragged-buffer (>=0.3.9,<0.4.0)
-Requires-Dist: rogue-net (>=0.1.5,<0.2.0)
+Requires-Dist: ragged-buffer (>=0.4.3,<0.5.0)
+Requires-Dist: rogue-net (>=0.1.6,<0.2.0)
 Requires-Dist: tensorboard (>=2.7.0,<3.0.0)
 Requires-Dist: tqdm (>=4.62.3,<5.0.0)
 Requires-Dist: wandb (>=0.12.7,<0.13.0)
```

