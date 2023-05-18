# Comparing `tmp/cdx_tf-0.1.2.tar.gz` & `tmp/cdx_tf-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdx_tf-0.1.2.tar", last modified: Sat May 13 09:50:10 2023, max compression
+gzip compressed data, was "cdx_tf-0.1.3.tar", last modified: Thu May 18 07:58:06 2023, max compression
```

## Comparing `cdx_tf-0.1.2.tar` & `cdx_tf-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 09:50:10.063374 cdx_tf-0.1.2/
--rw-rw-rw-   0        0        0     1090 2023-03-09 01:49:43.000000 cdx_tf-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     2716 2023-05-13 09:50:10.061373 cdx_tf-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2286 2023-03-20 22:12:29.000000 cdx_tf-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-13 09:50:10.026377 cdx_tf-0.1.2/cdx_tf/
--rw-rw-rw-   0        0        0      126 2023-05-13 09:50:07.000000 cdx_tf-0.1.2/cdx_tf/__init__.py
--rw-rw-rw-   0        0        0     5461 2023-05-13 09:28:16.000000 cdx_tf-0.1.2/cdx_tf/clip.py
--rw-rw-rw-   0        0        0    72406 2023-05-13 09:31:45.000000 cdx_tf-0.1.2/cdx_tf/gym.py
--rw-rw-rw-   0        0        0    42122 2023-05-13 09:31:14.000000 cdx_tf-0.1.2/cdx_tf/models.py
--rw-rw-rw-   0        0        0    19005 2023-05-13 09:29:54.000000 cdx_tf-0.1.2/cdx_tf/monetary_utility.py
--rw-rw-rw-   0        0        0     2323 2023-05-13 09:29:54.000000 cdx_tf-0.1.2/cdx_tf/optimizer.py
--rw-rw-rw-   0        0        0    10962 2023-04-15 17:30:23.000000 cdx_tf-0.1.2/cdx_tf/util.py
-drwxrwxrwx   0        0        0        0 2023-05-13 09:50:10.059372 cdx_tf-0.1.2/cdx_tf.egg-info/
--rw-rw-rw-   0        0        0     2716 2023-05-13 09:50:09.000000 cdx_tf-0.1.2/cdx_tf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-05-13 09:50:09.000000 cdx_tf-0.1.2/cdx_tf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 09:50:09.000000 cdx_tf-0.1.2/cdx_tf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2023-05-13 09:50:09.000000 cdx_tf-0.1.2/cdx_tf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-13 09:50:09.000000 cdx_tf-0.1.2/cdx_tf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-13 09:50:10.063374 cdx_tf-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      908 2023-05-13 09:50:07.000000 cdx_tf-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 07:58:06.138254 cdx_tf-0.1.3/
+-rw-rw-rw-   0        0        0     1090 2023-03-09 01:49:43.000000 cdx_tf-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     4075 2023-05-18 07:58:06.137251 cdx_tf-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3645 2023-05-13 10:14:58.000000 cdx_tf-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 07:58:06.097249 cdx_tf-0.1.3/cdx_tf/
+-rw-rw-rw-   0        0        0      126 2023-05-18 07:58:03.000000 cdx_tf-0.1.3/cdx_tf/__init__.py
+-rw-rw-rw-   0        0        0     5461 2023-05-13 09:28:16.000000 cdx_tf-0.1.3/cdx_tf/clip.py
+-rw-rw-rw-   0        0        0    70704 2023-05-18 07:54:03.000000 cdx_tf-0.1.3/cdx_tf/gym.py
+-rw-rw-rw-   0        0        0    42857 2023-05-18 07:26:32.000000 cdx_tf-0.1.3/cdx_tf/models.py
+-rw-rw-rw-   0        0        0    19005 2023-05-13 09:29:54.000000 cdx_tf-0.1.3/cdx_tf/monetary_utility.py
+-rw-rw-rw-   0        0        0     2323 2023-05-13 09:29:54.000000 cdx_tf-0.1.3/cdx_tf/optimizer.py
+-rw-rw-rw-   0        0        0    10962 2023-04-15 17:30:23.000000 cdx_tf-0.1.3/cdx_tf/util.py
+drwxrwxrwx   0        0        0        0 2023-05-18 07:58:06.134261 cdx_tf-0.1.3/cdx_tf.egg-info/
+-rw-rw-rw-   0        0        0     4075 2023-05-18 07:58:05.000000 cdx_tf-0.1.3/cdx_tf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-05-18 07:58:05.000000 cdx_tf-0.1.3/cdx_tf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 07:58:05.000000 cdx_tf-0.1.3/cdx_tf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2023-05-18 07:58:05.000000 cdx_tf-0.1.3/cdx_tf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-18 07:58:05.000000 cdx_tf-0.1.3/cdx_tf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 07:58:06.138254 cdx_tf-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      908 2023-05-18 07:58:03.000000 cdx_tf-0.1.3/setup.py
```

### Comparing `cdx_tf-0.1.2/LICENSE` & `cdx_tf-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cdx_tf-0.1.2/PKG-INFO` & `cdx_tf-0.1.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: cdx_tf
-Version: 0.1.2
+Version: 0.1.3
 Summary: Basic Python tools
 Home-page: https://github.com/hansbuehler/cdx_tf
 Author: Hans Buehler
 Author-email: github@buehler.london
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# cdx_tf (do not use yet)
+# cdx_tf (do not use this yet)
 Basic utilities for TensorFlow, following the Deep Hedging usage pattern.
 
 **This library is not ready for public use yet**
 
 The main component is a new keras model base class, `Gym`, whose implementation pattern eases:
 * Automated caching during training, including state of the optimizer.
   The motivation for introducing this class is that the standard tf/keras caching schemes such as `tf.keras.callbacks.ModelCheckpoint` or `tf.keras.callbacks.BackupAndRestore` do not work well with custom models. Neither does `model_save`.
   
 * Standardized ML pattern
   Fully driven by `cdxbasics.Config` configurations with self-documenting configuration handling. Self-declarative `layers.Agent` and `layers.RecurrentAgent`.
 
 * Monitoring training progress 
-  Seggregation of tracking training progress from visualizing it. As a result, the pattern allows multi-processing with `ray`.
+  Seggregation of tracking training progress from visualizing it.<br>
+  As a result, the pattern allows multi-processing with `ray`.
 
     
 ### Installation
 
 Install by
 
     conda install cdx_tf -c hansbuehler
@@ -39,17 +40,24 @@
     pip install cdx_tf
 
 # Basic usage pattern
 
 The main presumption of the pattern is that there are two kinds of "models" involved in training the desired agents.
 1) The agents themselves
 
-   Such agents are networks which map input features to actions. Such agents will usually be implemented using `layers.RecurrentAgent` which provides a default implementation pattern for recurrent agents which make self-declarative use of features, and which can have standard configuration patterns for users.
+   Such agents are networks which map input features to actions. Such agents will usually be implemented using `models.DenseAgent` or `models.RecurrentAgent` which provides a default implementation pattern for recurrent agents which make self-declarative use of features, and which can have standard configuration patterns for users.
+
+   The `models` module also contains simpler models, encapsulated in `dense_model` which transparently covers, well, dense simple models and variables in the case where the model has no input features. 
 
 2) The `gym`
 
    This is the model which executes the main business logic around the agents. In case of Deep Hedging, this is the core Monte Carlo loop for hedging derivatives. Gyms are derived from `gym.Gym`, and trained with `gym.train`. 
 
-   During training we will typically collect data about the progress of training such as the history of losses, current agent performance etc. This is implemented by deriving from `gym.ProgressData`. The main idea of `ProgressData` is that it abstracts data collection from the actual visualization of the data. This seggregation allows to send the `ProgressData` during training through an asynchronous queue - this way training can be parallelized including across machines. We show an example using `ray`.
+   **Training**: during training we will typically collect data about the progress of training such as the history of losses,  current agent performance etc. This is implemented by deriving from `gym.ProgressData`. The main idea of `ProgressData` is that it abstracts data collection from the actual visualization of the data. This seggregation allows to send `ProgressData` during training through an asynchronous queue - this way training can be parallelized including across machines. We show an example using `ray`.
    
+   The core training loop `gym.train` by default caches progress of training, which means that it can be interrupted and picked up again at any time. `train` also handles training and validation sets more robustly than tensorflow does if the sample weights are not uniform.
+
+   The default implementation provides a simple text summaries, but graphical updates as used in Deep Hedging can be implemented using `cdxbasics.dynaplot`.
 
+   **Serialization**: the integrated caching methdology means that a model can easily be restored from a saved file. _Restoration in this package is different than native TensorFlow model serialization_: our serialization will essentially restore all weights of a model reconstructed using Python code correctly - including in the compiled optimizer. The common TensorFlow serialization attempts to serialze the traced ("complied") model. 
 
+   The latter results a faster compiled model, while out method ensures that you have a valid Python object you can work with. It is also our preferred choice during active model development, as it is more robust vs code changes.
```

### Comparing `cdx_tf-0.1.2/README.md` & `cdx_tf-0.1.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-# cdx_tf (do not use yet)
+# cdx_tf (do not use this yet)
 Basic utilities for TensorFlow, following the Deep Hedging usage pattern.
 
 **This library is not ready for public use yet**
 
 The main component is a new keras model base class, `Gym`, whose implementation pattern eases:
 * Automated caching during training, including state of the optimizer.
   The motivation for introducing this class is that the standard tf/keras caching schemes such as `tf.keras.callbacks.ModelCheckpoint` or `tf.keras.callbacks.BackupAndRestore` do not work well with custom models. Neither does `model_save`.
   
 * Standardized ML pattern
   Fully driven by `cdxbasics.Config` configurations with self-documenting configuration handling. Self-declarative `layers.Agent` and `layers.RecurrentAgent`.
 
 * Monitoring training progress 
-  Seggregation of tracking training progress from visualizing it. As a result, the pattern allows multi-processing with `ray`.
+  Seggregation of tracking training progress from visualizing it.<br>
+  As a result, the pattern allows multi-processing with `ray`.
 
     
 ### Installation
 
 Install by
 
     conda install cdx_tf -c hansbuehler
@@ -25,17 +26,24 @@
     pip install cdx_tf
 
 # Basic usage pattern
 
 The main presumption of the pattern is that there are two kinds of "models" involved in training the desired agents.
 1) The agents themselves
 
-   Such agents are networks which map input features to actions. Such agents will usually be implemented using `layers.RecurrentAgent` which provides a default implementation pattern for recurrent agents which make self-declarative use of features, and which can have standard configuration patterns for users.
+   Such agents are networks which map input features to actions. Such agents will usually be implemented using `models.DenseAgent` or `models.RecurrentAgent` which provides a default implementation pattern for recurrent agents which make self-declarative use of features, and which can have standard configuration patterns for users.
+
+   The `models` module also contains simpler models, encapsulated in `dense_model` which transparently covers, well, dense simple models and variables in the case where the model has no input features. 
 
 2) The `gym`
 
    This is the model which executes the main business logic around the agents. In case of Deep Hedging, this is the core Monte Carlo loop for hedging derivatives. Gyms are derived from `gym.Gym`, and trained with `gym.train`. 
 
-   During training we will typically collect data about the progress of training such as the history of losses, current agent performance etc. This is implemented by deriving from `gym.ProgressData`. The main idea of `ProgressData` is that it abstracts data collection from the actual visualization of the data. This seggregation allows to send the `ProgressData` during training through an asynchronous queue - this way training can be parallelized including across machines. We show an example using `ray`.
+   **Training**: during training we will typically collect data about the progress of training such as the history of losses,  current agent performance etc. This is implemented by deriving from `gym.ProgressData`. The main idea of `ProgressData` is that it abstracts data collection from the actual visualization of the data. This seggregation allows to send `ProgressData` during training through an asynchronous queue - this way training can be parallelized including across machines. We show an example using `ray`.
    
+   The core training loop `gym.train` by default caches progress of training, which means that it can be interrupted and picked up again at any time. `train` also handles training and validation sets more robustly than tensorflow does if the sample weights are not uniform.
+
+   The default implementation provides a simple text summaries, but graphical updates as used in Deep Hedging can be implemented using `cdxbasics.dynaplot`.
 
+   **Serialization**: the integrated caching methdology means that a model can easily be restored from a saved file. _Restoration in this package is different than native TensorFlow model serialization_: our serialization will essentially restore all weights of a model reconstructed using Python code correctly - including in the compiled optimizer. The common TensorFlow serialization attempts to serialze the traced ("complied") model. 
 
+   The latter results a faster compiled model, while out method ensures that you have a valid Python object you can work with. It is also our preferred choice during active model development, as it is more robust vs code changes.
```

### Comparing `cdx_tf-0.1.2/cdx_tf/clip.py` & `cdx_tf-0.1.3/cdx_tf/clip.py`

 * *Files identical despite different names*

### Comparing `cdx_tf-0.1.2/cdx_tf/gym.py` & `cdx_tf-0.1.3/cdx_tf/gym.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,59 +170,17 @@
     def cache_uid( self ):
         """ Return the unique ID for this gym. """
         return self._cache_unique_id
 
     @property
     def cache_def_directory_name( self ):
         """ Returns a descriptive name for this class which can be used as directory for the caches. No trailing '/' """
-        name = str( self.__class__.__name__ )
-        return name if self.CACHE_VERSION is None else ( name + "/" + str(self.CACHE_VERSION) )
-
-    # -------------------
-    # Keras serialization
-    # -------------------
-
-    @staticmethod
-    def from_config( tf_config : dict ):
-        """
-        You will have to implement this for all derived classes.
-        Default pattern is written below
-        """
-        raise NotImplementedError("Please implement Gym.from_config")
-
-    @staticmethod
-    def from_config_default( Class : type, tf_config : dict ):
-        """
-        Default 'from_config' code.
-        Meant to be used as
-
-        class MyGyum(Gym):
-
-            @staticmethod
-            def from_config( tf_config : dict ):
-                return Gym.from_config_default( MyGym, tf_config )
-        """
-        _log.verify( tf_config['cache_version'] == Class.CACHE_VERSION, "Error reading configuration from cache for '%s'': version mismatch. Found version %s, but current code is version %s", Class.__name__, tf_config['cache_version'], Class.CACHE_VERSION )
-        return Class( config        = tf_config['config'],
-                      name          = tf_config['name'],
-                      dtype         = tf_config['dtype'],
-                      trainable     = tf_config['trainable'],
-                      cache_uid     = tf_config['cache_uid']
-                )
-
-    def get_config( self ):
-        """ You will need to overwrite this if your __init__ signature changes """
-        return dict(
-            config        = self._cache_config,
-            cache_uid     = self._cache_unique_id,
-            name          = self.name,
-            dtype         = self.dtype,
-            trainable     = self.trainable,
-            cache_version = self.CACHE_VERSION
-            )
+        name  = str( self.__class__.__name__ )
+        fname = self.name
+        return (name + "/" + fname ) if not fname is None and fname != name else name
 
 # ==========================================================================
 # TrainingInfo
 # Information on the current training run
 # ==========================================================================
 
 class TrainingInfo(object):
@@ -580,15 +538,15 @@
             self.process            = PrettyDict()
             self.process.memory_rss = [ p.memory_info().rss / (1024.*1024.) ]
             self.process.memory_vms = [ p.memory_info().vms / (1024.*1024.) ]
 
     # --------------------
     # Status information
     # --------------------
-    
+
     @property
     def current_epoch(self) -> int:
         """ Returns the current epoch. Returns -1 if no epoch was yet recorded """
         return len(self.times_per_epoch)-1
 
     @property
     def remaining_epochs(self) -> int:
@@ -662,15 +620,15 @@
                                  predicted_data : PrettyDict,   # current predicted training and validation data; current loss.
                                  training_info  : TrainingInfo, # number of epochs to be computed etc
                                  logs           : dict          # logs c.f. keras Callback
                           ) -> Status:
         """
         Callback at the end of an epoch.
         Intended to update all calculation for this ProgressData object.
-        
+
         All native data such as current_epoch, timing, results etc are updated at this point, except information on caching because
         this  unction is called before a decision to cache the current object is made.
         Therefore any data computed in a derived on_epoch_end_prep() and stored in 'self' will be cached, too.
 
         Use on_epoch_end_update() to update the user after caching (e.g. self.last_cached_epoch is correct)
         Note that on_epoch_end_update() is not called if this function returns a stopping reason other than Status.CONTINUE.
         Instead, on_done() is called.
@@ -975,20 +933,20 @@
             assert self.cache_last_epoch == self.progress_data.current_epoch, "Interal error: %ld > %ld ?" % (self.cache_last_epoch, self.progress_data.current_epoch)
             return
         assert self.progress_data.current_epoch >= 0, "Internal error: current epoch is -1"
 
         t0     = time.time()
         gym    = self.environment.gym
         opt_w  = gym.optimizer.get_weights() if TF_VERSION <= 210 else [ w.value() for w in gym.optimizer.variables() ]
-        cache  = dict( name        = gym.__class__.__name__,
-                       version     = str(gym.CACHE_VERSION),
-                       progress    = self.progress_data,
-                       gym_weights = gym.get_weights(),
-                       opt_config  = tf.keras.optimizers.serialize(gym.optimizer),
-                       opt_weights = opt_w
+        cache  = dict( name         = gym.__class__.__name__,
+                       version      = str(gym.CACHE_VERSION),
+                       progress     = self.progress_data,
+                       gym_weights  = gym.get_weights(),
+                       opt_config   = tf.keras.optimizers.serialize(gym.optimizer),
+                       opt_weights  = opt_w
                       )
 
         self.cache_dir.write( self.cache_file, cache )
         self.cache_last_epoch = self.progress_data.current_epoch
 
         self.progress_data._on_cache_written( environment       = self.environment,
                                               training_info     = self.training_info,
@@ -1272,15 +1230,15 @@
         environment   = Environment(gym=gym, **create_environment )
     else:
         _log.verify( len(create_environment) == 0,  "If 'environment' is specified, then you cannot specify additional keywords. Found %s", fmt_list( list(create_environment.keys())))
 
     config.gym.mark_done()
     gym                      = environment.gym
     optimizer_uid            = config.train.optimizer.unique_id()
-    train_uid                = uniqueFileName48( [ gym.cache_uid, optimizer_uid, gym.CACHE_VERSION ] )
+    train_uid                = uniqueFileName48( [ gym.cache_uid, optimizer_uid ] )
     display_name             = display_name if not display_name is None else gym.display_name
     display_name             = config.train("display_name", display_name, str, "Display name for this training run" )
     verbose.report(0,"Initializing training for %(display_name)s", display_name = display_name )
 
     # caching
     def_directory_name       = gym.cache_def_directory_name + "/batch_" + (str(batch_size) if not batch_size is None else "default")
     cache_config             = PrettyDict()
@@ -1328,15 +1286,15 @@
         environment.set_gym( gym, cached=False )
 
         predicted_data0  = environment.predict()
         progress_data    = create_progress( environment=environment,
                                             predicted_data0=predicted_data0,
                                             training_info=training_info,
                                             config=config.progress )
-        verbose.report(1, "%s: model generated. Preparing training for %ld epochs. Model has %ld trainable weights.", display_name, progress_data.remaining_epochs, gym.num_trainable_weights)
+        verbose.report(1, "%s: model generated. Preparing training for %ld epochs. Model has %s trainable weights.", display_name, progress_data.remaining_epochs, fmt_big_number( gym.num_trainable_weights) )
 
     config.done()
 
     description = gym.description
     if not description is None:
         verbose.report(2, description)
```

### Comparing `cdx_tf-0.1.2/cdx_tf/models.py` & `cdx_tf-0.1.3/cdx_tf/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,14 +138,15 @@
                         nOutput    : int,
                         width      : int = 50,
                         depth      : int = 3,
                         activation : str = "relu",
                         final_act  : str = "linear",
                         zero_model : bool = False,
                         regression : bool = False,
+                        norm_batch : bool = False,
                         dtype      : tf.DType = def_dtype,
                         name       : str = None,
                         trainable  : bool = True
                     ):
         """
         Represents a dense network with a given 'depth', 'width', 'activation' function and a final layer with activation function 'final_act' (typicall linear).
         The layer maps a tensors of dimension nInput into tensors of dimension nOutput.
@@ -163,14 +164,15 @@
                 activation   : activation function in core network
                 final_activation : activation function to compress last 'width' to nOutput. Usually linear.
                 zero_model   : whether the model is initialzed to zero initial value (but not zero gradients)
                                Practically, the model constructs both the original model F and a non-trainable
                                model F', then sets the weights of F' to the initial weights of F, and defines
                                the full model as M=F-F'. If 'trainable' is False then this function returnbs a network
                                with zero initial value.
+                norm_batch   : add batch normalization
                 regression   : hard set the network to a pure regression model.
                                This is equivalent to setting depth = 0, width = nInput, and final_activation = 'linear'.
             dtype, name, trainable :
                 see tf.keras.Model()
         """
         tf.keras.Model.__init__(self, name=name, dtype=dtype, trainable=trainable )
 
@@ -183,14 +185,15 @@
                                  nOutput    = self._nOutput,
                                  width      = width,
                                  depth      = depth,
                                  activation = activation,
                                  final_act  = final_act,
                                  zero_model = zero_model,
                                  regression = regression,
+                                 norm_batch = norm_batch,
                                  dtype      = dtype,
                                  name       = name,
                                  trainable = trainable)
 
         if regression:
             depth      = 0
             width      = nInput
@@ -210,14 +213,18 @@
                                        use_bias=True, dtype=dtype,
                                        trainable=False )
             x1 = d1(x1)
             x2 = d2(x2)
             return x1, x2
 
         inp       = tf.keras.layers.Input( shape=(nInput,), dtype=dtype )
+        
+        if norm_batch:
+            inp = tf.keras.layers.BatchNormalization(synchronized=True)(inp)
+        
         x1, x2    = ( inp, inp if zero_model else None )
         for d in range(depth):
             x1, x2    = dense( width, activation, x1, x2 )
         x1, x2 = dense( nOutput, final_act, x1, x2 )
         x  = tf.keras.layers.Subtract()([x1, x2]) if not x2 is None else x1
         m  = tf.keras.Model( inputs=inp, outputs=x, name=name )
         if zero_model:
@@ -239,15 +246,14 @@
         """
         Returns the number of weights. The gym must have been call()ed once
         Agent needs to have been called at least once
         """
         weights = self.trainable_weights
         return np.sum( [ np.prod( w.get_shape() ) for w in weights ] ) if not weights is None else 0.
 
-
 def dense_model( nInput     : int,
                  nOutput    : int,
                  config     : Config = None,
                  kwargs_cfg : dict = None,
                  **kwargs
                  ) -> tf.keras.Model:
     """
@@ -307,49 +313,53 @@
 
     width           = kwargs('width', None, (None, Int>0))
     depth           = kwargs('depth', None, (None, Int>=0))
     activation      = kwargs('activation', None, (None, str))
     final_act       = kwargs('final_act', None, (None,str))
     zero_model      = kwargs('zero_model', None, (None, bool))
     regression      = kwargs('regression', None, (None, bool))
+    norm_batch      = kwargs('normalize_batch', None, (None, bool))
 
     dtype           = kwargs('dtype', def_dtype )
     name            = kwargs('name', None, (str, None))
     trainable       = kwargs('trainable', True, bool)
 
     def_width       = kwargs("def_width", 50, Int>0 )
     def_depth       = kwargs("def_depth", 3, Int>=0 )
     def_activation  = kwargs("def_activation", 'relu', str)
     def_final_act   = kwargs("def_final_act", "linear", str)
     def_zero_model  = kwargs("def_zero_model", True, bool)
     def_regression  = kwargs("def_regression", False, bool)
+    def_norm_batch  = kwargs("def_normalize_batch", False, bool)
 
     kwargs.done() # catch developer typos
 
     config          = config if not config is None else Config()
     width           = config("width", def_width, Int>0, "Width") if width is None else width
     depth           = config("depth", def_depth, Int>=0, "Depth") if depth is None else depth
     activation      = config("activation", def_activation, str, "Activation function") if activation is None else activation
     final_act       = config("final_activation",def_final_act, str, "Final activation function") if final_act is None else final_act
     zero_model      = config("zero_model", def_zero_model, bool, "Whether to initialze values (but not derivatives) of the model with zero") if zero_model is None else zero_model
     regression      = config("simple_regression", def_regression, bool, "Learn simple regression model only") if regression is None else regression
+    norm_batch      = config("normalize_batch", def_norm_batch, bool, "Apply batch normalization") if norm_batch is None else norm_batch
 
     config.done() # catch user errors
 
     if nInput == 0:
         return VariableModel( int(nOutput), name=name, dtype=dtype, trainable=trainable )
 
     return DenseModel( nInput  = nInput,
                        nOutput = nOutput,
                        width   = width,
                        depth   = depth,
                        activation = activation,
                        final_act  = final_act,
                        zero_model = zero_model,
                        regression = regression,
+                       norm_batch = norm_batch,
                        dtype = dtype,
                        name = name,
                        trainable = trainable)
 
 # =====================================================================================
 # Agents
 # Agents extract named features from the 'data' given to __call__
@@ -359,15 +369,15 @@
     """
     Standardized generic agent which will use named features as inputs, and will extract those from the 'data' dictionary provided.
     All features are flattened before passed on to the agent.
 
     If no features are selected, then this model becomes a VariableModel, e.g. it is a variable of size nOutput.
     """
 
-    def __init__(self, nOutput : int, state_size : int = 0, config : Config = None, *, kwargs_cfg : dict = None, **kwargs ):
+    def __init__(self, nOutput : int, nRawInput : int = 0, config : Config = None, *, kwargs_cfg : dict = None, **kwargs ):
         """
         Create standard Agent.
 
         The model implements a dense network of 'depth' and 'width' with activation function 'activation'.
         The final layer then condenses the last 'width' nodes to 'nOutput' nodes, usually with a linear 'final_act'.
         The model will extract the user-requested features from the 'data' dictionary provided to __call__.
         The user specifies the desired features with the 'features' config keyword. The model can be made to always
@@ -379,15 +389,15 @@
 
         If the model is created without features it will represent a VariableModel.
 
         Parameters
         ----------
             nOutput :
                 number of output states
-            state_size :
+            nRawInput :
                 If non-zero, this specifies the second dimension of an additional state vector which is to be passed
                 to the agent when calling() it.
                 This allows the calling user to add a fixed state to the otherwise dynamic features extracted during
                 runtime
 
             kwargs_cfg, **kwargs:
                 Only one of these can be non-empty.
@@ -413,43 +423,43 @@
                                    with zero initial value.
                     regression   : hard set the network to a pure regression model. This is a debugging option with default False.
                                    This is equivalent to setting depth = 0, width = nInput, and final_activation = 'linear'.
 
                 A more complex example is that of selecting features for the underlying agent.
                 Those are specified by name. The agent will then drive extraction of the relevant data from the data universe automatically.
 
-                    def_features     : just as in the above example, these are the default features for the agent.
+                    def_features     : these are the default features for the agent.
                     required_features: features which the agent always needs to use
-                    allow_no_features: whether or not to allow an empty list fo features. This is set to False if required_features
+                    allow_no_features: whether or not to allow an empty list fo features.
 
                     features         : if specified by the developer, then these features are always used.
-                                       Note that if required_features are defined, then the two lists are merged.
-
+                                       Note that if required_features are defined, then the two lists are merged for convenience.
+                                       The presence of 'features' will no longer allow the user to specify their own features.
                     config('features') : if 'features' is not specified, then the user may choose her own features.
 
                 Finally, both kwargs_cfg and kwargs may also contain standard keyword parameters for tf.keras.Model() such as dtype, name, trainable.
         """
         assert kwargs_cfg is None or len(kwargs) == 0, "Cannot specify 'kwargs_cfg' and **kwargs"
 
         kwargs                   = to_config(kwargs_cfg if not kwargs_cfg is None else kwargs, config_name="kwargs_DenseAgent")
         nOutput                  = int(nOutput)
-        state_size               = int(state_size)
+        nRawInput                = int(nRawInput)
         _log.verify( nOutput > 0, "'nOutput' must be positive. Found %ld", nOutput )
-        _log.verify( state_size >= 0, "'state_size' must not be negative. Found %ld", state_size )
+        _log.verify( nRawInput >= 0, "'nRawInput' must not be negative. Found %ld", nRawInput )
 
         dtype                    = kwargs('dtype', def_dtype )
         name                     = kwargs('name', None, (str, None))
         trainable                = kwargs('trainable', True, bool)
         tf.keras.Model.__init__(self, name=name, dtype=dtype, trainable=trainable )
 
         self._model              = None
         self._available_features = None
         self._size_features      = None
         self._nOutput            = nOutput
-        self._state_size         = state_size
+        self._nRawInput          = nRawInput
 
         self._features           = kwargs('features', None, (None, list))
         def_features             = kwargs("def_features", [], list)
         req_features             = kwargs("required_features", [], list)
         allow_no_features        = kwargs("allow_no_features", True, bool) if len(req_features)==0 else False
         self._kwargs             = kwargs.detach() # store kwargs for a subsequent call to dense_model()
 
@@ -462,101 +472,100 @@
         config.done() # catch user errors
         kwargs.done() # catch dev errors
 
     # ----------------------------
     # keras build/call
     # ----------------------------
 
-    def build(self, shapes_data_and_state : dict ):
+    def build(self, shapes_data_and_inputs : dict ):
         """ Extract the requested features from the shapes provided """
         assert self._model is None, "'build' called twice?"
 
-        state_shape = shapes_data_and_state.get('state', None)
-        shapes      = shapes_data_and_state['data']
+        shapes = shapes_data_and_inputs['data']
 
         self._available_features = list(shapes.keys())
         self._available_features.sort()
 
         self._size_features = 0
         missing         = []
         for f in self._features:
             fs = shapes.get(f,None)
             if fs is None:
                 missing.append(f)
                 continue
             # we will flatten all features
             if len(fs) > 2:
-                fs = [ fs[0], np.product( fs.as_list()[1:] ) ]
-            self._size_features += fs[1] if len(fs) > 0 else 1
-
+                self._size_features += np.product( fs.as_list()[1:] )
+            elif len(fs) == 2:
+                self._size_features += fs[1]
+            else:
+                self._size_features += 1
+                
         if len(missing) > 0:
             missing   = fmt_list(missing)
             available = fmt_list(self._available_features, "(none)")
             _log.throw("Could not extract the following features: %s. Available features are: %s", missing, available)
 
         self._model = dense_model(
-                nInput      = self._size_features + self._state_size,
+                nInput      = self._size_features + self._nRawInput,
                 nOutput     = self._nOutput,
                 config      = self._config,
                 kwargs_cfg  = self._kwargs
                 )
 
-    def call(self, data_with_state : dict, training : bool = False) ->  tf.Tensor:
+    def call(self, data_and_inputs : dict, training : bool = False) ->  tf.Tensor:
         """
-        Return action based on data provied
+        Return action based on data provided
         This construction here is a bit convoluted. Would prefer to just use __call__ TODO
         """
         assert not self._model is None, "build() was not called...?"
-        data     = data_with_state['data']
-        state    = data_with_state['state'] if self._state_size > 0 else None
+        data     = data_and_inputs['data']
+        inputs   = data_and_inputs.get('inputs', None)
         features = None
         if len(self._features) > 0:
             features  = [ data[f] for f in self._features ]
             features  = [ tf_make_dim( f, target_dim=2 ) for f in features ]
             features  = tf.concat( features, axis=1 ) if len(features) > 1 else features[0]
             assert features.shape[1] == self._size_features, "Internal error: %ld != %ld" % ( features.shape[1], self._size_features)
 
-        if self._state_size > 0:
-            _log.verify( not state is None, "Error calling '%s': state_size was set to %ld, hence you need to provide a state. Found 'None'")
-            _log.verify( len(state.shape) == 2 and int(state.shape[1]) == self._state_size, "Error calling '%s': state_size was set to %ld, hence you need to provide a state of shape [None, %ld]. Found tensor of shape %s", self._state_size, self._state_size, state.shape.as_list())
-            features = tf.concat( [features, state], axis=1) if not features is None else state
+        if self._nRawInput > 0:
+            _log.verify( not inputs is None, "Error calling '%s': nRawInput was set to %ld, hence you need to provide 'inputs'. Found 'None'", name(self), self._nRawInput)
+            _log.verify( len(inputs.shape) == 2 and int(inputs.shape[1]) == self._nRawInput, "Error calling '%s': nRawInput was set to %ld, hence you need to provide 'inputs' of shape [None, %ld]. Found tensor of shape %s", self._nRawInput, self._nRawInput, inputs.shape.as_list())
+            features = tf.concat( [features, inputs], axis=1) if not features is None else inputs
         else:
-            _log.verify( state is None, "Error calling '%s': model is not recurrent, but a state was provided. Set state to 'None'.", name(self) )
+            _log.verify( inputs is None, "Error calling '%s': model has no raw inputs, but 'inputs' were provided. Set 'inputs' to 'None'.", name(self) )
 
         assert features is None or isinstance( features, tf.Tensor ), "'features' must be a tensor, not %s" % type(features).__name__
         return self._model( features if not features is None else data, training=training )
 
-    def __call__(self, data : dict, state : tf.Tensor = None, **kwargs ):
+    def __call__(self, data : dict, inputs : tf.Tensor = None, **kwargs ):
         """
         Compute agent result.
 
 
         Parameters
         ----------
             data : dict
                 Dictionary containing the models' named features for this model. Does not include 'state'
-            state : tf.Tensor or None
-                If the model has a state, then 'state' must be set to a matrix tensor with second dimension equal to self.size_recurrent_state.
-                For the first call, this is the initial state. For subsequent calls, provide the 'new_state' of the previous __call__()
-                If the model does not have a state, then 'state' must be None
+            inputs : tf.Tensor or None
+                If the model has a raw inputs (e.g. nRawInputs > 0 in __init__), then 'inputs' must be set to a matrix tensor with second dimension equal to self._nRawInput.
+                If the model does not have a raw inputs, then 'inputs' must be None
             **kwargs:
                 see tf.keras.Model.__call__()
 
         Returns
         -------
-            A tuple (result, new_state)
-            If the model has a state, then 'new_state' is the state to be passed to the next function call.
-            If the model does not have a state, then 'state' is None
+            A tensor of shape [None, nOutput] where 'nOutput' was specified in __init__.
         """
         assert isinstance( data, Mapping ), "'data' must be dictionary or similar, not '%s'" % type(data).__name__
-        if self._state_size > 0:
-            _log.verify( isinstance( state, tf.Tensor ), "'state' must be tensor of shape [None, %ld], not a type '%s'", self._state_size, type(state).__name__ )
+        if self._nRawInput > 0:
+            _log.verify( isinstance( inputs, tf.Tensor ), "'inputs' must be tensor of shape [None, %ld], not a type '%s'", self._nRawInput, type(inputs).__name__ )
         else:
-            _log.verify( state is None, "'state' must be None, not '%s'", type(state).__name__  )
-        return tf.keras.Model.__call__(self, dict( data=data, state=state ) if not state is None else dict(data=data), **kwargs )
+            _log.verify( inputs is None, "'inputs' must be None, not '%s'", type(inputs).__name__  )
+        return tf.keras.Model.__call__(self, dict( data=data, inputs=inputs ) if not inputs is None else dict(data=data), **kwargs )
 
     # ----------------------------
     # data access
     # ----------------------------
 
     @property
     def features(self) -> list:
@@ -581,14 +590,21 @@
     def available_features(self) -> list:
         """
         Returns the sorted list of available features for this agent.
         Agent needs to have been called at least once
         """
         assert not self._model is None, "agent model needs to be called at least once before calling this function"
         return self._available_features
+    
+    @property
+    def unused_features(self) -> list:
+        """ 
+        Returns the sorted list of any available features which were not used
+        """
+        return sorted( set(self.available_features)-set(self.features) )
 
     @property
     def num_output(self) -> int:
         """ Returns the dimnension of the action output tensor """
         return self._nOutput
 
     @property
@@ -600,20 +616,20 @@
         assert not self._model is None, "agent model needs to be called at least once before calling this function"
         weights = self.trainable_weights
         return np.sum( [ np.prod( w.get_shape() ) for w in weights ] ) if not weights is None else 0.
 
     @property
     def has_state(self):
         """ Whether this agent is recurrent """
-        return self._state_size > 0
+        return self._nRawInput > 0
 
     @property
     def state_size(self):
         """ Returns the size of the recurrent state """
-        return self._state_size
+        return self._nRawInput
 
     @property
     def dim_all_features(self) -> int:
         """
         Returns the size of the total features vector after flattening
         Agent needs to have been called at least once
         """
```

### Comparing `cdx_tf-0.1.2/cdx_tf/monetary_utility.py` & `cdx_tf-0.1.3/cdx_tf/monetary_utility.py`

 * *Files identical despite different names*

### Comparing `cdx_tf-0.1.2/cdx_tf/optimizer.py` & `cdx_tf-0.1.3/cdx_tf/optimizer.py`

 * *Files identical despite different names*

### Comparing `cdx_tf-0.1.2/cdx_tf/util.py` & `cdx_tf-0.1.3/cdx_tf/util.py`

 * *Files identical despite different names*

### Comparing `cdx_tf-0.1.2/cdx_tf.egg-info/PKG-INFO` & `cdx_tf-0.1.3/cdx_tf.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: cdx-tf
-Version: 0.1.2
+Version: 0.1.3
 Summary: Basic Python tools
 Home-page: https://github.com/hansbuehler/cdx_tf
 Author: Hans Buehler
 Author-email: github@buehler.london
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# cdx_tf (do not use yet)
+# cdx_tf (do not use this yet)
 Basic utilities for TensorFlow, following the Deep Hedging usage pattern.
 
 **This library is not ready for public use yet**
 
 The main component is a new keras model base class, `Gym`, whose implementation pattern eases:
 * Automated caching during training, including state of the optimizer.
   The motivation for introducing this class is that the standard tf/keras caching schemes such as `tf.keras.callbacks.ModelCheckpoint` or `tf.keras.callbacks.BackupAndRestore` do not work well with custom models. Neither does `model_save`.
   
 * Standardized ML pattern
   Fully driven by `cdxbasics.Config` configurations with self-documenting configuration handling. Self-declarative `layers.Agent` and `layers.RecurrentAgent`.
 
 * Monitoring training progress 
-  Seggregation of tracking training progress from visualizing it. As a result, the pattern allows multi-processing with `ray`.
+  Seggregation of tracking training progress from visualizing it.<br>
+  As a result, the pattern allows multi-processing with `ray`.
 
     
 ### Installation
 
 Install by
 
     conda install cdx_tf -c hansbuehler
@@ -39,17 +40,24 @@
     pip install cdx_tf
 
 # Basic usage pattern
 
 The main presumption of the pattern is that there are two kinds of "models" involved in training the desired agents.
 1) The agents themselves
 
-   Such agents are networks which map input features to actions. Such agents will usually be implemented using `layers.RecurrentAgent` which provides a default implementation pattern for recurrent agents which make self-declarative use of features, and which can have standard configuration patterns for users.
+   Such agents are networks which map input features to actions. Such agents will usually be implemented using `models.DenseAgent` or `models.RecurrentAgent` which provides a default implementation pattern for recurrent agents which make self-declarative use of features, and which can have standard configuration patterns for users.
+
+   The `models` module also contains simpler models, encapsulated in `dense_model` which transparently covers, well, dense simple models and variables in the case where the model has no input features. 
 
 2) The `gym`
 
    This is the model which executes the main business logic around the agents. In case of Deep Hedging, this is the core Monte Carlo loop for hedging derivatives. Gyms are derived from `gym.Gym`, and trained with `gym.train`. 
 
-   During training we will typically collect data about the progress of training such as the history of losses, current agent performance etc. This is implemented by deriving from `gym.ProgressData`. The main idea of `ProgressData` is that it abstracts data collection from the actual visualization of the data. This seggregation allows to send the `ProgressData` during training through an asynchronous queue - this way training can be parallelized including across machines. We show an example using `ray`.
+   **Training**: during training we will typically collect data about the progress of training such as the history of losses,  current agent performance etc. This is implemented by deriving from `gym.ProgressData`. The main idea of `ProgressData` is that it abstracts data collection from the actual visualization of the data. This seggregation allows to send `ProgressData` during training through an asynchronous queue - this way training can be parallelized including across machines. We show an example using `ray`.
    
+   The core training loop `gym.train` by default caches progress of training, which means that it can be interrupted and picked up again at any time. `train` also handles training and validation sets more robustly than tensorflow does if the sample weights are not uniform.
+
+   The default implementation provides a simple text summaries, but graphical updates as used in Deep Hedging can be implemented using `cdxbasics.dynaplot`.
 
+   **Serialization**: the integrated caching methdology means that a model can easily be restored from a saved file. _Restoration in this package is different than native TensorFlow model serialization_: our serialization will essentially restore all weights of a model reconstructed using Python code correctly - including in the compiled optimizer. The common TensorFlow serialization attempts to serialze the traced ("complied") model. 
 
+   The latter results a faster compiled model, while out method ensures that you have a valid Python object you can work with. It is also our preferred choice during active model development, as it is more robust vs code changes.
```

### Comparing `cdx_tf-0.1.2/setup.py` & `cdx_tf-0.1.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cdx_tf", 
-    version="0.1.2",  # will auto-update via pip_modify_setup.py
+    version="0.1.3",  # will auto-update via pip_modify_setup.py
     author="Hans Buehler",
     author_email="github@buehler.london",
     description="Basic Python tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hansbuehler/cdx_tf",
     packages=setuptools.find_packages(),
```

