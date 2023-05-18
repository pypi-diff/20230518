# Comparing `tmp/patas-2.0.5.tar.gz` & `tmp/patas-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patas-2.0.5.tar", last modified: Sun May 14 13:59:41 2023, max compression
+gzip compressed data, was "patas-2.0.6.tar", last modified: Thu May 18 18:52:21 2023, max compression
```

## Comparing `patas-2.0.5.tar` & `patas-2.0.6.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-14 13:59:41.173720 patas-2.0.5/
--rw-rw-r--   0 diego     (1000) diego     (1000)    13930 2023-05-14 13:59:41.173720 patas-2.0.5/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)    13512 2023-05-13 20:44:01.000000 patas-2.0.5/README.md
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-14 13:59:41.173720 patas-2.0.5/patas/
--rw-rw-r--   0 diego     (1000) diego     (1000)       19 2023-05-08 20:38:56.000000 patas-2.0.5/patas/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)    32279 2023-05-13 20:39:28.000000 patas-2.0.5/patas/argparsers.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      205 2023-05-14 13:59:35.000000 patas-2.0.5/patas/consts.py
--rw-rw-r--   0 diego     (1000) diego     (1000)    16391 2023-05-13 20:39:28.000000 patas-2.0.5/patas/graphics.py
--rw-rw-r--   0 diego     (1000) diego     (1000)    26220 2023-05-11 14:18:45.000000 patas-2.0.5/patas/grid_explorer.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      330 2023-05-06 20:57:54.000000 patas-2.0.5/patas/log.py
--rwxrwxr-x   0 diego     (1000) diego     (1000)     9837 2023-05-13 20:39:28.000000 patas-2.0.5/patas/main.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     7619 2023-05-11 22:04:38.000000 patas-2.0.5/patas/parse.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     1021 2023-05-14 13:58:00.000000 patas-2.0.5/patas/query_engine.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     6117 2023-05-11 20:10:23.000000 patas-2.0.5/patas/schemas.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     9283 2023-05-10 13:33:56.000000 patas-2.0.5/patas/utils.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-14 13:59:41.173720 patas-2.0.5/patas.egg-info/
--rw-rw-r--   0 diego     (1000) diego     (1000)    13930 2023-05-14 13:59:41.000000 patas-2.0.5/patas.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)      425 2023-05-14 13:59:41.000000 patas-2.0.5/patas.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        1 2023-05-14 13:59:41.000000 patas-2.0.5/patas.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       42 2023-05-14 13:59:41.000000 patas-2.0.5/patas.egg-info/entry_points.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       26 2023-05-14 13:59:41.000000 patas-2.0.5/patas.egg-info/requires.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       12 2023-05-14 13:59:41.000000 patas-2.0.5/patas.egg-info/top_level.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       38 2023-05-14 13:59:41.173720 patas-2.0.5/setup.cfg
--rw-rw-r--   0 diego     (1000) diego     (1000)      852 2023-05-10 22:45:33.000000 patas-2.0.5/setup.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-14 13:59:41.173720 patas-2.0.5/tests/
--rw-rw-r--   0 diego     (1000) diego     (1000)       18 2023-05-07 16:31:37.000000 patas-2.0.5/tests/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     1420 2023-05-07 16:54:01.000000 patas-2.0.5/tests/test_schemas.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-18 18:52:21.739164 patas-2.0.6/
+-rw-rw-r--   0 diego     (1000) diego     (1000)    15443 2023-05-18 18:52:21.739164 patas-2.0.6/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)    15025 2023-05-18 18:52:10.000000 patas-2.0.6/README.md
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-18 18:52:21.735164 patas-2.0.6/patas/
+-rw-rw-r--   0 diego     (1000) diego     (1000)       19 2023-05-08 20:38:56.000000 patas-2.0.6/patas/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)    28362 2023-05-18 18:52:10.000000 patas-2.0.6/patas/argparsers.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      205 2023-05-18 18:52:10.000000 patas-2.0.6/patas/consts.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)    16391 2023-05-13 20:39:28.000000 patas-2.0.6/patas/graphics.old.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     5360 2023-05-18 18:52:10.000000 patas-2.0.6/patas/graphics.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      330 2023-05-06 20:57:54.000000 patas-2.0.6/patas/log.py
+-rwxrwxr-x   0 diego     (1000) diego     (1000)    11029 2023-05-18 18:52:10.000000 patas-2.0.6/patas/main.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     8262 2023-05-18 18:52:10.000000 patas-2.0.6/patas/parse.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1154 2023-05-18 18:52:10.000000 patas-2.0.6/patas/query.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)    22505 2023-05-18 18:52:10.000000 patas-2.0.6/patas/scheduler.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)    16215 2023-05-18 18:52:10.000000 patas-2.0.6/patas/schemas.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     9715 2023-05-18 18:52:10.000000 patas-2.0.6/patas/utils.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-18 18:52:21.739164 patas-2.0.6/patas.egg-info/
+-rw-rw-r--   0 diego     (1000) diego     (1000)    15443 2023-05-18 18:52:21.000000 patas-2.0.6/patas.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)      436 2023-05-18 18:52:21.000000 patas-2.0.6/patas.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        1 2023-05-18 18:52:21.000000 patas-2.0.6/patas.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       42 2023-05-18 18:52:21.000000 patas-2.0.6/patas.egg-info/entry_points.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       23 2023-05-18 18:52:21.000000 patas-2.0.6/patas.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       12 2023-05-18 18:52:21.000000 patas-2.0.6/patas.egg-info/top_level.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       38 2023-05-18 18:52:21.739164 patas-2.0.6/setup.cfg
+-rw-rw-r--   0 diego     (1000) diego     (1000)      849 2023-05-18 18:52:10.000000 patas-2.0.6/setup.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-18 18:52:21.739164 patas-2.0.6/tests/
+-rw-rw-r--   0 diego     (1000) diego     (1000)       18 2023-05-07 16:31:37.000000 patas-2.0.6/tests/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1420 2023-05-07 16:54:01.000000 patas-2.0.6/tests/test_schemas.py
```

### Comparing `patas-2.0.5/PKG-INFO` & `patas-2.0.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,18 @@
-Metadata-Version: 2.1
-Name: patas
-Version: 2.0.5
-Summary: Hyperparameter search with a single command
-Home-page: https://github.com/diegofps/patas
-Author: Diego Souza
-Author-email: diegofpsouza+patas@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Provides-Extra: full
-
 # Patas 🐾
 
 Patas is a command line utility designed to execute any program in parallel and collect its output, varying its input parameters and starting the programs automatically. The script may be parallelized on your local machine or in a cluster. The only requirement to run it on a cluster is an SSH connection between the machines. Assuming the programs are located on each worker machine, patas can start and manage the parallel programs with one command. Parsing the outputs is done in a second command. Its name means PArser and TAsk Scheduler. You can install it using pip with the following command.
 
 ```shell
 pip install patas
 ```
 
 # Basic usage 🐣
 
-Considering the use case that we need to find the optimal configuration for a neural network. In this case we are interested in variating the number of hidden neurons and the activation function in the hidden layer. We want to execute our prgoram multiple times, combining the values of these two parameters, and collect metrics of interest, like train and test accuracies. We then want to analyse this output and select the best configuration. The following subsections will describe how to achieve this.
+Considering the use case that we need to find the optimal configuration for a neural network. In this case we are interested in variating the number of hidden neurons, the activation function, and the complexity of preprocessing we do. We want to execute our prgoram multiple times, combining the values of these two parameters, and collect metrics of interest, like train and test accuracies. We then want to analyse this output and select the best configuration. The following subsections will describe how to achieve this.
 
 ## The program
 
 We will use a mockup code present in `examples/basic_usage`. This is a script that pretends to run a neural network, receiving the two variables of interest and printing the desired metrics to stdout. This could easily be replaced by a real program training a neural network, but we use a mockup to speed up the process. To access this program you just need to access the folder.
 
 ```shell
 # Enter the program folder
@@ -33,54 +20,65 @@
 
 # Example of program execution
 ./main.py 100 relu
 ```
 
 ## patas explore
 
-Assuming we want to vary the number of hidden neurons from `1` to `51` with steps of `2` and the activation function in `['relu' 'leaky_relu' 'sigmoid' 'tanh']`, we can generate all combinationsand parallelize the script above using `patas explore grid`. This will also collect its entire stdout and save them in the folder `patasout/grid`. Each combination will be executed `10` times, as we want to measure the average accuracies later.
+Assuming we want to vary the number of hidden neurons from `1` to `51` with steps of `2` and the activation function in `['relu' 'leaky_relu' 'sigmoid' 'tanh']`, we can generate all combinationsand parallelize the script above using `patas explore grid`. This will also collect its entire stdout and save them in the folder `pataslab/grid`. Each combination will be executed `10` times, as we want to measure the average accuracies later.
 
 ```shell
-patas explore grid \
-    --cmd './main.py {neurons} {activation}' \
+patas explore --type grid \
+    --cmd './main.py {neurons} {activation} {preprocessing}' \
     --va neurons 1 51 2 \
+    --vl preprocessing fast medium intense \
     --vl activation relu leaky_relu sigmoid tanh \
+    --node localhost \
     --repeat 10
 ```
 
-The parameter `--cmd` define the command that must be executed. If we define more than one `--cmd` they will all be executed, one after the other. The parameter `--vl` defines a variable of type list, it receives the variable name and the list of values it can receive. Next, the parameter `--repeat` defines the number of times the program will be called using a given variable combination. In this example, the parameter neurons define `26` values and the paramter activation define `4` values. This will generate `104 combinations`. Considering the repeat parameter has the value `10`, the program will be excuted `1040` times. That is, patas will have `1040 tasks` to do. You can define as many variable as you want, but the more you have the longer it will take to execute, growing exponentially.
+Here is a short description of the parameters above:
+
+`--cmd` - defines the command that must be executed. If we define more than one `--cmd` they will all be executed, one after the other. 
+`--va` - defines a variable of type arithmetic, it receives the variable name, an initial value, a maximum value and a step value. It will generate a list similar to the Python's method `range`. 
+`--vl` - defines a variable of type list, it receives the variable name and the list of values it can receive. 
+`--node` - defines a node to execute the program. This may be any machine accessible via SSH that won't ask for a password. This command accepts an optional argument to indicate the number of workers in the machine. If non is provided, it will default to the number of cores in the machine. You may want to check the program `ssh-copy-id` to learn how to install a public key on a remote machine and log in without a password. 
+`--repeat` defines the number of times the program will be called using a given variable combination. In this example, the parameter neurons define `25` values, parameter preprocessing defines `3` values and the paramter activation define `4` values. This will generate `300 combinations`. Considering the repeat parameter has the value `10`, the program will be excuted `3000` timesm. That is, we asked patas to do `3000 tasks`. You can define as many variables as you want, but the more you have the longer it will take to execute.
 
 ## patas parse
 
 When the experiment is done executing, we can parse its outputs and collect the desired values using `patas parse`.
 
 ```shell
 patas parse \
-    -e 'patasout/grid/' \
-    -p train_acc  'Train accuracy:     (@float@)' \
-    -p test_acc   'Test accuracy:      (@float@)'
+    -e 'pataslab/grid/' \
+    -p train_time  'Time to train \(ms\): (@float@)' \
+    -p test_time   'Time to test \(ms\):  (@float@)' \
+    -p train_acc   'Train accuracy:     (@float@)' \
+    -p test_acc    'Test accuracy:      (@float@)' \
+    -p loss        'Final Loss:         (@float@)'
 ```
 
-The parameter `-e` define the experiment folder, containing the prgoram outputs and a few extra info. The parameter `-p` define a pattern patas is going to look for. It receives a name and a regular expression string. The output file will be saved in `patasout/grid/grid.csv`. This contains a table with the input variables, collected results, and extra variables associated to the experiment. 
+The parameter `-e` define the experiment folder, containing the prgoram outputs and a few extra info. The parameter `-p` define a pattern patas is going to look for. It receives a name and a regular expression string. The output file will be saved in `pataslab/grid/grid.csv`. This contains a table with the input variables, collected results, and extra variables associated to the experiment. 
 
 ## patas query
 
 We use `patas query` to inspect the contents of the csv file generated above. This command works with any csv file and recognizes the experiment names as table names.
 
 ```shell
 patas query 'select * from grid limit 2' -m
 ```
 
 The parameter `-m` asks patas to print the output in markdown format.
 The output for the command above should have a similar structure to the content bellow. The values may vary as the script is non-determininstic.
 
-| in_activation | in_neurons | out_train_acc | out_test_acc | break_id | task_id | repeat_id | combination_id | experiment_id | experiment_name | duration |          started_at |            ended_at | tries | max_tries | cluster_id | cluster_name | node_id | node_name | worker_id | output_dir                                                       | work_dir                                       |
-| ------------- | ---------- | ------------- | ------------ | -------- | ------- | --------- | -------------- | ------------- | --------------- | -------- | ------------------- | ------------------- | ----- | --------- | ---------- | ------------ | ------- | --------- | --------- | ---------------------------------------------------------------- | ---------------------------------------------- |
-| leaky_relu    |         25 |         0,487 |        0,452 |    False |     386 |         6 |             38 |         False | grid            |   0,048… | 2023-05-11 14:13:34 | 2023-05-11 14:13:34 |  True |         3 |      False | cluster      |   False | localhost |         7 | /home/ubuntu/Sources/patas/examples/basic_usage/patasout/grid/386 | /home/ubuntu/Sources/patas/examples/basic_usage |
-| sigmoid       |         27 |         0,841 |        0,820 |    False |     652 |         2 |             65 |         False | grid            |   0,055… | 2023-05-11 14:13:34 | 2023-05-11 14:13:34 |  True |         3 |      False | cluster      |   False | localhost |        57 | /home/ubuntu/Sources/patas/examples/basic_usage/patasout/grid/652 | /home/ubuntu/Sources/patas/examples/basic_usage |
+| in_activation | in_neurons | in_preprocessing | out_train_time | out_test_time | out_train_acc | out_test_acc | out_loss | break_id | task_id | repeat_id | combination_id | experiment_id | experiment_name | tries | max_tries | duration | started_at                 | ended_at                   | cluster_name | node_name | cluster_in_lab | node_in_lab | node_in_cluster | worker_in_lab | worker_in_cluster | worker_in_node | output_dir                                                        | work_dir                                 |
+| ------------- | ---------- | ---------------- | -------------- | ------------- | ------------- | ------------ | -------- | -------- | ------- | --------- | -------------- | ------------- | --------------- | ----- | --------- | -------- | -------------------------- | -------------------------- | ------------ | --------- | -------------- | ----------- | --------------- | ------------- | ----------------- | -------------- | ----------------------------------------------------------------- | ---------------------------------------- |
+| relu          | 33         | medium           | 175.812        | 4.880         | 0.423         | 0.411        | 0.338    | 0        | 1160    | 0         | 116            | 0             | grid            | 1     | 3         | 0.224591 | 2023-05-17 19:14:55.472312 | 2023-05-17 19:14:55.696903 | cluster      | node0     | 0              | 0           | 0               | 14            | 14                | 14             | /home/diego/Sources/patas/examples/basic_usage/pataslab/grid/1160 | $HOME/Sources/patas/examples/basic_usage |
+| leaky_relu    | 27         | fast             | 190.677        | 6.904         | 0.286         | 0.270        | 0.288    | 0        | 386     | 6         | 38             | 0             | grid            | 1     | 3         | 0.225969 | 2023-05-17 19:14:58.327345 | 2023-05-17 19:14:58.553314 | cluster      | node0     | 0              | 0           | 0               | 47            | 47                | 47             | /home/diego/Sources/patas/examples/basic_usage/pataslab/grid/386  | $HOME/Sources/patas/examples/basic_usage |
 
 We must remember that for every combination, patas will execute the program `--repeat` times, passing the same input parameters and collecting multiple output variables. This is useful when the algorithm we are evaluating is non-deterministic and we wish to collect reliable metrics, like our script. To aggregate these values we can calculate the average value using the `AVG` function with the `GROUP BY` statement.
 
 ```shell
 patas query '
     SELECT in_activation, 
            in_neurons, 
@@ -110,135 +108,115 @@
 
 | in_activation | in_neurons | train_acc | test_acc |
 | ------------- | ---------- | --------- | -------- |
 | relu          |          5 |    0,995… |   0,946… |
 
 ## patas draw
 
-Patas will also help you quickly create basic graphics based on the data in the csv file. This might help you inspect the data and get some quick insights. As of now, patas supports three graphic types, `heatmap`, `bars`, and `lines`.
+Patas can also help you quickly create basic graphics based on the data in the csv file. It provides a wrapper for a few seaborn functions to quickly generate graphics, without needing to create a python script for this. If you need complex charts, though, we recommend you use the advanced graphics library of your preference. As of now, patas provides three drawing functions: `heatmap`, `categorical`, and `lines`.
 
 ### Heatmap
 
 ```shell
 patas draw heatmap \
-    --input patasout/grid/grid.csv \
+    --input pataslab/grid/grid.csv \
     --x-column in_neurons \
     --y-column in_activation \
     --z-column out_test_acc \
-    --size 10 2
+    --fig-size 15 3
 ```
 
 ![Basic heatmap example](https://github.com/diegofps/patas/blob/main/docs/images/heatmap1.png?raw=true)
 
 ```shell
 patas draw heatmap \
-    --input 'patasout/grid/grid.csv' \
-    --title 'Grid Search Results' \
+    --input pataslab/grid/grid.csv \
+    --output heatmap.png \
+    --title 'Average test accuracy' \
     --x-column in_neurons \
-    --x-change 'int(X[i])*2' \
-    --x-label Neurons \
+    --x-label 'Number of Neurons' \
+    --x-change 'X[i]' \
     --y-column in_activation \
+    --y-label 'Activation function' \
     --y-change 'Y[i][:3]' \
-    --y-label 'Activation Function' \
     --z-column out_test_acc \
-    --z-change 'Z[i]*100' \
-    --r-function min \
-    --r-format 'int(R[y,x])' \
-    --r-label Accuracy \
-    --size 10 2 \
-    --colormap AAAAAA 000011
+    --z-label 'Accuracy' \
+    --z-change 'int(Z[i]*100)' \
+    --fig-size 15 3 \
+    --annot \
+    --aggfunc mean \
+    --fmt '.0f'
 ```
 
 ![Extended heatmap example](https://github.com/diegofps/patas/blob/main/docs/images/heatmap2.png?raw=true)
 
-### Bars
-
-```shell
-patas query 'select * from grid where in_activation="relu"' > test.csv
-```
+### Categorical
 
 ```shell
-patas draw bars \
-    --input test.csv \
-    --x-column in_neurons \
+patas draw categories \
+    --input pataslab/grid/grid.csv \
+    --x-column in_activation \
     --y-column out_test_acc \
-    --size 10 2
+    --fig-size 10 7 \
+    --x-label 'Activation function' \
+    --y-label 'Test Accuracy' \
+    --title 'Test performance by activation function'
 ```
 
-![Bars example](https://github.com/diegofps/patas/blob/main/docs/images/bars1.png?raw=true)
+![Categorical example](https://github.com/diegofps/patas/blob/main/docs/images/categorical1.png?raw=true)
 
 ```shell
-patas draw bars \
-    --input test.csv \
-    --title 'Performance using the function relu' \
-    --x-column in_neurons \
-    --x-change 'int(float(X[i]))' \
-    --x-label 'Neurons' \
+patas draw categories \
+    --input pataslab/grid/grid.csv \
+    --x-column in_activation \
+    --hue-column in_preprocessing \
     --y-column out_test_acc \
-    --y-change 'round(Y[i]*100)/100' \
-    --r-function mean \
-    --r-format 'R[i]:.2f' \
-    --r-label 'Accuracy' \
-    --size 10 2 \
-    --bar-size 0.8 \
-    --bar-color B00020 \
-    --show-grid \
-    --show-error \
-    --ticks 5 \
-    --ticks-format 'T[i]:.2f' \
-    --border none
+    --fig-size 10 4 \
+    --x-label 'Activation function' \
+    --y-label 'Test Accuracy' \
+    --legend-label 'Preprocessing' \
+    --errorbar 'sd' \
+    --title 'Test performance by activation function and preprocessing'
 ```
 
-![Bars example](https://github.com/diegofps/patas/blob/main/docs/images/bars2.png?raw=true)
+![Categorical example](https://github.com/diegofps/patas/blob/main/docs/images/categorical2.png?raw=true)
 
 ### Lines
 
 ```shell
 patas draw lines \
-    --input patasout/grid/grid.csv \
-    --size 10 2 \
-    --new-line \
-    --x-column in_neurons \
-    --y-column out_test_acc \
-    \
-    --new-line \
-    --x-column in_neurons \
-    --y-column out_train_acc
+    --input 'pataslab/grid/grid.csv' \
+    --fig-size 10 4 \
+    --x-column 'in_neurons' \
+    --x-label 'Neurons' \
+    --y-column 'out_test_acc' \
+    --y-label 'Accuracy' \
+    --title 'Average test accuracy' \
+    --err-style 'bars' \
+    --errorbar 'sd'
 ```
 
 ![Lines example](https://github.com/diegofps/patas/blob/main/docs/images/lines1.png?raw=true)
 
 ```shell
 patas draw lines \
-    --input patasout/grid/grid.csv \
-    --title "Testing Title" \
-    --x-label "x axis" \
-    --r-label "y axis" \
-    --size 10 2 \
-    --show-grid \
-    --border none \
-    --ticks 5 \
-    --ticks-format 'T[i]:.2f' \
-    \
-    --new-line \
-    --label 'Test accuracy' \
-    --x-column in_neurons \
-    --y-column out_test_acc \
-    --style dash \
-    --marker diamond \
-    \
-    --new-line \
-    --label 'Train accuracy' \
-    --x-column in_neurons \
-    --y-column out_train_acc \
-    --style dot \
-    --marker circle
+    --input 'pataslab/grid/grid.csv' \
+    --fig-size 10 4 \
+    --x-column 'in_neurons' \
+    --x-label 'Neurons' \
+    --y-column 'out_test_acc' \
+    --y-label 'Accuracy' \
+    --hue-column 'in_activation' \
+    --title 'Average test accuracy' \
+    --legend-label 'Act. Function' \
+    --err-style 'band' \
+    --errorbar 'sd'
 ```
 
-![Extended lines example](https://github.com/diegofps/patas/blob/main/docs/images/lines2.png?raw=true)
+![Lines example](https://github.com/diegofps/patas/blob/main/docs/images/lines2.png?raw=true)
 
 # Documentation 📚
 
 ## When should I use Patas? ⭐
 
 Use this program if you want to evaluate your model against multiple parameters and measure your own performance metrics. It is a quick way to parallelize an experiment over various machines. It is also handy when you don't want to, or can't, change the original program.
```

### Comparing `patas-2.0.5/README.md` & `patas-2.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,31 @@
+Metadata-Version: 2.1
+Name: patas
+Version: 2.0.6
+Summary: Hyperparameter search with a single command
+Home-page: https://github.com/diegofps/patas
+Author: Diego Souza
+Author-email: diegofpsouza+patas@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+Provides-Extra: full
+
 # Patas 🐾
 
 Patas is a command line utility designed to execute any program in parallel and collect its output, varying its input parameters and starting the programs automatically. The script may be parallelized on your local machine or in a cluster. The only requirement to run it on a cluster is an SSH connection between the machines. Assuming the programs are located on each worker machine, patas can start and manage the parallel programs with one command. Parsing the outputs is done in a second command. Its name means PArser and TAsk Scheduler. You can install it using pip with the following command.
 
 ```shell
 pip install patas
 ```
 
 # Basic usage 🐣
 
-Considering the use case that we need to find the optimal configuration for a neural network. In this case we are interested in variating the number of hidden neurons and the activation function in the hidden layer. We want to execute our prgoram multiple times, combining the values of these two parameters, and collect metrics of interest, like train and test accuracies. We then want to analyse this output and select the best configuration. The following subsections will describe how to achieve this.
+Considering the use case that we need to find the optimal configuration for a neural network. In this case we are interested in variating the number of hidden neurons, the activation function, and the complexity of preprocessing we do. We want to execute our prgoram multiple times, combining the values of these two parameters, and collect metrics of interest, like train and test accuracies. We then want to analyse this output and select the best configuration. The following subsections will describe how to achieve this.
 
 ## The program
 
 We will use a mockup code present in `examples/basic_usage`. This is a script that pretends to run a neural network, receiving the two variables of interest and printing the desired metrics to stdout. This could easily be replaced by a real program training a neural network, but we use a mockup to speed up the process. To access this program you just need to access the folder.
 
 ```shell
 # Enter the program folder
@@ -20,54 +33,65 @@
 
 # Example of program execution
 ./main.py 100 relu
 ```
 
 ## patas explore
 
-Assuming we want to vary the number of hidden neurons from `1` to `51` with steps of `2` and the activation function in `['relu' 'leaky_relu' 'sigmoid' 'tanh']`, we can generate all combinationsand parallelize the script above using `patas explore grid`. This will also collect its entire stdout and save them in the folder `patasout/grid`. Each combination will be executed `10` times, as we want to measure the average accuracies later.
+Assuming we want to vary the number of hidden neurons from `1` to `51` with steps of `2` and the activation function in `['relu' 'leaky_relu' 'sigmoid' 'tanh']`, we can generate all combinationsand parallelize the script above using `patas explore grid`. This will also collect its entire stdout and save them in the folder `pataslab/grid`. Each combination will be executed `10` times, as we want to measure the average accuracies later.
 
 ```shell
-patas explore grid \
-    --cmd './main.py {neurons} {activation}' \
+patas explore --type grid \
+    --cmd './main.py {neurons} {activation} {preprocessing}' \
     --va neurons 1 51 2 \
+    --vl preprocessing fast medium intense \
     --vl activation relu leaky_relu sigmoid tanh \
+    --node localhost \
     --repeat 10
 ```
 
-The parameter `--cmd` define the command that must be executed. If we define more than one `--cmd` they will all be executed, one after the other. The parameter `--vl` defines a variable of type list, it receives the variable name and the list of values it can receive. Next, the parameter `--repeat` defines the number of times the program will be called using a given variable combination. In this example, the parameter neurons define `26` values and the paramter activation define `4` values. This will generate `104 combinations`. Considering the repeat parameter has the value `10`, the program will be excuted `1040` times. That is, patas will have `1040 tasks` to do. You can define as many variable as you want, but the more you have the longer it will take to execute, growing exponentially.
+Here is a short description of the parameters above:
+
+`--cmd` - defines the command that must be executed. If we define more than one `--cmd` they will all be executed, one after the other. 
+`--va` - defines a variable of type arithmetic, it receives the variable name, an initial value, a maximum value and a step value. It will generate a list similar to the Python's method `range`. 
+`--vl` - defines a variable of type list, it receives the variable name and the list of values it can receive. 
+`--node` - defines a node to execute the program. This may be any machine accessible via SSH that won't ask for a password. This command accepts an optional argument to indicate the number of workers in the machine. If non is provided, it will default to the number of cores in the machine. You may want to check the program `ssh-copy-id` to learn how to install a public key on a remote machine and log in without a password. 
+`--repeat` defines the number of times the program will be called using a given variable combination. In this example, the parameter neurons define `25` values, parameter preprocessing defines `3` values and the paramter activation define `4` values. This will generate `300 combinations`. Considering the repeat parameter has the value `10`, the program will be excuted `3000` timesm. That is, we asked patas to do `3000 tasks`. You can define as many variables as you want, but the more you have the longer it will take to execute.
 
 ## patas parse
 
 When the experiment is done executing, we can parse its outputs and collect the desired values using `patas parse`.
 
 ```shell
 patas parse \
-    -e 'patasout/grid/' \
-    -p train_acc  'Train accuracy:     (@float@)' \
-    -p test_acc   'Test accuracy:      (@float@)'
+    -e 'pataslab/grid/' \
+    -p train_time  'Time to train \(ms\): (@float@)' \
+    -p test_time   'Time to test \(ms\):  (@float@)' \
+    -p train_acc   'Train accuracy:     (@float@)' \
+    -p test_acc    'Test accuracy:      (@float@)' \
+    -p loss        'Final Loss:         (@float@)'
 ```
 
-The parameter `-e` define the experiment folder, containing the prgoram outputs and a few extra info. The parameter `-p` define a pattern patas is going to look for. It receives a name and a regular expression string. The output file will be saved in `patasout/grid/grid.csv`. This contains a table with the input variables, collected results, and extra variables associated to the experiment. 
+The parameter `-e` define the experiment folder, containing the prgoram outputs and a few extra info. The parameter `-p` define a pattern patas is going to look for. It receives a name and a regular expression string. The output file will be saved in `pataslab/grid/grid.csv`. This contains a table with the input variables, collected results, and extra variables associated to the experiment. 
 
 ## patas query
 
 We use `patas query` to inspect the contents of the csv file generated above. This command works with any csv file and recognizes the experiment names as table names.
 
 ```shell
 patas query 'select * from grid limit 2' -m
 ```
 
 The parameter `-m` asks patas to print the output in markdown format.
 The output for the command above should have a similar structure to the content bellow. The values may vary as the script is non-determininstic.
 
-| in_activation | in_neurons | out_train_acc | out_test_acc | break_id | task_id | repeat_id | combination_id | experiment_id | experiment_name | duration |          started_at |            ended_at | tries | max_tries | cluster_id | cluster_name | node_id | node_name | worker_id | output_dir                                                       | work_dir                                       |
-| ------------- | ---------- | ------------- | ------------ | -------- | ------- | --------- | -------------- | ------------- | --------------- | -------- | ------------------- | ------------------- | ----- | --------- | ---------- | ------------ | ------- | --------- | --------- | ---------------------------------------------------------------- | ---------------------------------------------- |
-| leaky_relu    |         25 |         0,487 |        0,452 |    False |     386 |         6 |             38 |         False | grid            |   0,048… | 2023-05-11 14:13:34 | 2023-05-11 14:13:34 |  True |         3 |      False | cluster      |   False | localhost |         7 | /home/ubuntu/Sources/patas/examples/basic_usage/patasout/grid/386 | /home/ubuntu/Sources/patas/examples/basic_usage |
-| sigmoid       |         27 |         0,841 |        0,820 |    False |     652 |         2 |             65 |         False | grid            |   0,055… | 2023-05-11 14:13:34 | 2023-05-11 14:13:34 |  True |         3 |      False | cluster      |   False | localhost |        57 | /home/ubuntu/Sources/patas/examples/basic_usage/patasout/grid/652 | /home/ubuntu/Sources/patas/examples/basic_usage |
+| in_activation | in_neurons | in_preprocessing | out_train_time | out_test_time | out_train_acc | out_test_acc | out_loss | break_id | task_id | repeat_id | combination_id | experiment_id | experiment_name | tries | max_tries | duration | started_at                 | ended_at                   | cluster_name | node_name | cluster_in_lab | node_in_lab | node_in_cluster | worker_in_lab | worker_in_cluster | worker_in_node | output_dir                                                        | work_dir                                 |
+| ------------- | ---------- | ---------------- | -------------- | ------------- | ------------- | ------------ | -------- | -------- | ------- | --------- | -------------- | ------------- | --------------- | ----- | --------- | -------- | -------------------------- | -------------------------- | ------------ | --------- | -------------- | ----------- | --------------- | ------------- | ----------------- | -------------- | ----------------------------------------------------------------- | ---------------------------------------- |
+| relu          | 33         | medium           | 175.812        | 4.880         | 0.423         | 0.411        | 0.338    | 0        | 1160    | 0         | 116            | 0             | grid            | 1     | 3         | 0.224591 | 2023-05-17 19:14:55.472312 | 2023-05-17 19:14:55.696903 | cluster      | node0     | 0              | 0           | 0               | 14            | 14                | 14             | /home/diego/Sources/patas/examples/basic_usage/pataslab/grid/1160 | $HOME/Sources/patas/examples/basic_usage |
+| leaky_relu    | 27         | fast             | 190.677        | 6.904         | 0.286         | 0.270        | 0.288    | 0        | 386     | 6         | 38             | 0             | grid            | 1     | 3         | 0.225969 | 2023-05-17 19:14:58.327345 | 2023-05-17 19:14:58.553314 | cluster      | node0     | 0              | 0           | 0               | 47            | 47                | 47             | /home/diego/Sources/patas/examples/basic_usage/pataslab/grid/386  | $HOME/Sources/patas/examples/basic_usage |
 
 We must remember that for every combination, patas will execute the program `--repeat` times, passing the same input parameters and collecting multiple output variables. This is useful when the algorithm we are evaluating is non-deterministic and we wish to collect reliable metrics, like our script. To aggregate these values we can calculate the average value using the `AVG` function with the `GROUP BY` statement.
 
 ```shell
 patas query '
     SELECT in_activation, 
            in_neurons, 
@@ -97,135 +121,115 @@
 
 | in_activation | in_neurons | train_acc | test_acc |
 | ------------- | ---------- | --------- | -------- |
 | relu          |          5 |    0,995… |   0,946… |
 
 ## patas draw
 
-Patas will also help you quickly create basic graphics based on the data in the csv file. This might help you inspect the data and get some quick insights. As of now, patas supports three graphic types, `heatmap`, `bars`, and `lines`.
+Patas can also help you quickly create basic graphics based on the data in the csv file. It provides a wrapper for a few seaborn functions to quickly generate graphics, without needing to create a python script for this. If you need complex charts, though, we recommend you use the advanced graphics library of your preference. As of now, patas provides three drawing functions: `heatmap`, `categorical`, and `lines`.
 
 ### Heatmap
 
 ```shell
 patas draw heatmap \
-    --input patasout/grid/grid.csv \
+    --input pataslab/grid/grid.csv \
     --x-column in_neurons \
     --y-column in_activation \
     --z-column out_test_acc \
-    --size 10 2
+    --fig-size 15 3
 ```
 
 ![Basic heatmap example](https://github.com/diegofps/patas/blob/main/docs/images/heatmap1.png?raw=true)
 
 ```shell
 patas draw heatmap \
-    --input 'patasout/grid/grid.csv' \
-    --title 'Grid Search Results' \
+    --input pataslab/grid/grid.csv \
+    --output heatmap.png \
+    --title 'Average test accuracy' \
     --x-column in_neurons \
-    --x-change 'int(X[i])*2' \
-    --x-label Neurons \
+    --x-label 'Number of Neurons' \
+    --x-change 'X[i]' \
     --y-column in_activation \
+    --y-label 'Activation function' \
     --y-change 'Y[i][:3]' \
-    --y-label 'Activation Function' \
     --z-column out_test_acc \
-    --z-change 'Z[i]*100' \
-    --r-function min \
-    --r-format 'int(R[y,x])' \
-    --r-label Accuracy \
-    --size 10 2 \
-    --colormap AAAAAA 000011
+    --z-label 'Accuracy' \
+    --z-change 'int(Z[i]*100)' \
+    --fig-size 15 3 \
+    --annot \
+    --aggfunc mean \
+    --fmt '.0f'
 ```
 
 ![Extended heatmap example](https://github.com/diegofps/patas/blob/main/docs/images/heatmap2.png?raw=true)
 
-### Bars
-
-```shell
-patas query 'select * from grid where in_activation="relu"' > test.csv
-```
+### Categorical
 
 ```shell
-patas draw bars \
-    --input test.csv \
-    --x-column in_neurons \
+patas draw categories \
+    --input pataslab/grid/grid.csv \
+    --x-column in_activation \
     --y-column out_test_acc \
-    --size 10 2
+    --fig-size 10 7 \
+    --x-label 'Activation function' \
+    --y-label 'Test Accuracy' \
+    --title 'Test performance by activation function'
 ```
 
-![Bars example](https://github.com/diegofps/patas/blob/main/docs/images/bars1.png?raw=true)
+![Categorical example](https://github.com/diegofps/patas/blob/main/docs/images/categorical1.png?raw=true)
 
 ```shell
-patas draw bars \
-    --input test.csv \
-    --title 'Performance using the function relu' \
-    --x-column in_neurons \
-    --x-change 'int(float(X[i]))' \
-    --x-label 'Neurons' \
+patas draw categories \
+    --input pataslab/grid/grid.csv \
+    --x-column in_activation \
+    --hue-column in_preprocessing \
     --y-column out_test_acc \
-    --y-change 'round(Y[i]*100)/100' \
-    --r-function mean \
-    --r-format 'R[i]:.2f' \
-    --r-label 'Accuracy' \
-    --size 10 2 \
-    --bar-size 0.8 \
-    --bar-color B00020 \
-    --show-grid \
-    --show-error \
-    --ticks 5 \
-    --ticks-format 'T[i]:.2f' \
-    --border none
+    --fig-size 10 4 \
+    --x-label 'Activation function' \
+    --y-label 'Test Accuracy' \
+    --legend-label 'Preprocessing' \
+    --errorbar 'sd' \
+    --title 'Test performance by activation function and preprocessing'
 ```
 
-![Bars example](https://github.com/diegofps/patas/blob/main/docs/images/bars2.png?raw=true)
+![Categorical example](https://github.com/diegofps/patas/blob/main/docs/images/categorical2.png?raw=true)
 
 ### Lines
 
 ```shell
 patas draw lines \
-    --input patasout/grid/grid.csv \
-    --size 10 2 \
-    --new-line \
-    --x-column in_neurons \
-    --y-column out_test_acc \
-    \
-    --new-line \
-    --x-column in_neurons \
-    --y-column out_train_acc
+    --input 'pataslab/grid/grid.csv' \
+    --fig-size 10 4 \
+    --x-column 'in_neurons' \
+    --x-label 'Neurons' \
+    --y-column 'out_test_acc' \
+    --y-label 'Accuracy' \
+    --title 'Average test accuracy' \
+    --err-style 'bars' \
+    --errorbar 'sd'
 ```
 
 ![Lines example](https://github.com/diegofps/patas/blob/main/docs/images/lines1.png?raw=true)
 
 ```shell
 patas draw lines \
-    --input patasout/grid/grid.csv \
-    --title "Testing Title" \
-    --x-label "x axis" \
-    --r-label "y axis" \
-    --size 10 2 \
-    --show-grid \
-    --border none \
-    --ticks 5 \
-    --ticks-format 'T[i]:.2f' \
-    \
-    --new-line \
-    --label 'Test accuracy' \
-    --x-column in_neurons \
-    --y-column out_test_acc \
-    --style dash \
-    --marker diamond \
-    \
-    --new-line \
-    --label 'Train accuracy' \
-    --x-column in_neurons \
-    --y-column out_train_acc \
-    --style dot \
-    --marker circle
+    --input 'pataslab/grid/grid.csv' \
+    --fig-size 10 4 \
+    --x-column 'in_neurons' \
+    --x-label 'Neurons' \
+    --y-column 'out_test_acc' \
+    --y-label 'Accuracy' \
+    --hue-column 'in_activation' \
+    --title 'Average test accuracy' \
+    --legend-label 'Act. Function' \
+    --err-style 'band' \
+    --errorbar 'sd'
 ```
 
-![Extended lines example](https://github.com/diegofps/patas/blob/main/docs/images/lines2.png?raw=true)
+![Lines example](https://github.com/diegofps/patas/blob/main/docs/images/lines2.png?raw=true)
 
 # Documentation 📚
 
 ## When should I use Patas? ⭐
 
 Use this program if you want to evaluate your model against multiple parameters and measure your own performance metrics. It is a quick way to parallelize an experiment over various machines. It is also handy when you don't want to, or can't, change the original program.
```

### Comparing `patas-2.0.5/patas/argparsers.py` & `patas-2.0.6/patas/argparsers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import argparse
-from argparse import ArgumentParser, Namespace
-from collections.abc import Sequence
-from typing import Any
 
-DEFAULT_PATAS_OUTPUT_DIR = './patasout'
 
+DEFAULT_PATAS_OUTPUT_DIR = './pataslab'
+DEFAULT_FIG_SIZE = (10, 7)
 
-def parse_patas_explore_grid(argv):
+
+def parse_patas_explore(argv):
 
     # argparse for 'patas explore grid'
 
     parser = argparse.ArgumentParser(
-                        prog='patas explore grid',
-                        description='Execute a program permutating its input parameters.',
+                        prog='patas explore',
+                        description='Start a hyperparameter search.',
                         epilog="Check the README.md to learn more tips on how to use this feature: https://github.com/diegofps/patas/blob/main/README.md",
                         formatter_class=argparse.RawDescriptionHelpFormatter)
 
     # General parameters
 
     parser.add_argument('--cluster',
                         type=str,
@@ -28,98 +27,105 @@
     parser.add_argument('--experiment',
                         type=str,
                         metavar='FILEPATH',
                         dest='experiment',
                         help="path to an experiment file",
                         action='append')
 
-    parser.add_argument('--redo',
-                        dest='redo_tasks',
-                        help="forces patas to redo all tasks when an experiment is executed again",
-                        action='store_true')
-
-    parser.add_argument('--recreate',
-                        dest='recreate',
-                        help="recreate the entire output folder if it contains a different experiment configuration",
-                        action='store_true')
-
-    parser.add_argument('--filter-tasks',
-                        type=str,
-                        default=[],
-                        nargs='*',
-                        metavar='A:B',
-                        dest='task_filters',
-                        help="restricts the tasks that will be executed [A:B, A:, :B, :]",
-                        action='append')
-
-    parser.add_argument('--filter-nodes',
-                        type=str,
-                        default=[],
-                        metavar='TAG',
-                        nargs='*',
-                        dest='node_filters',
-                        help="filter nodes that match these tags (AND)",
-                        action='store')
-
     parser.add_argument('--node',
                         type=str,
                         nargs='*',
                         metavar='NAME USER@HOST:PORT WORKERS TAG1 ...',
                         dest='node',
                         help="adds a machine with the given number of workers to the cluster",
                         action='append')
 
     parser.add_argument('-y',
                         dest='confirmed',
                         help="skip confirmation before starting the tasks",
                         action='store_true')
 
+    parser.add_argument('-q',
+                        dest='quiet',
+                        help="only display critical events",
+                        action='store_true')
+
     parser.add_argument('-o',
                         type=str,
                         default=DEFAULT_PATAS_OUTPUT_DIR,
                         metavar='FOLDER',
                         dest='output_folder',
                         help="folder to store the program outputs",
                         action='store')
 
     # Quick Experiment parameters
 
+    parser.add_argument('--type',
+                        default='grid',
+                        metavar='NAME',
+                        choices=('grid', 'cdeepso'),
+                        help='type of experiment to execute',
+                        action='store')
+
+    parser.add_argument('--redo',
+                        dest='redo_tasks',
+                        help="forces patas to redo all tasks when an experiment is executed again",
+                        action='store_true')
+
+    parser.add_argument('--filter-tasks',
+                        type=str,
+                        default=[],
+                        nargs='*',
+                        metavar='A:B',
+                        dest='task_filters',
+                        help="restricts the tasks that will be executed [A:B, A:, :B, :]",
+                        action='append')
+
+    parser.add_argument('--filter-nodes',
+                        type=str,
+                        default=[],
+                        metavar='TAG',
+                        nargs='*',
+                        dest='node_filters',
+                        help="filter nodes that match these tags (AND)",
+                        action='store')
+
     parser.add_argument('--name',
                         type=str,
                         default='grid',
                         metavar='NAME',
                         dest='name',
                         help="changes the name of the experiment folder, default is grid",
                         action='store')
 
     parser.add_argument('--vl',
                         type=str,
                         nargs='*',
                         default=[],
                         metavar='VAL',
                         dest='var_list',
-                        help="defines an input variable that can assume a fixed number of values",
+                        help="defines an input variable that can assume a fixed number of values, used only in grid search",
                         action='append')
 
     parser.add_argument('--va',
                         type=str,
                         nargs=4,
                         default=[],
                         metavar=('NAME', 'MIN', 'MAX', 'FACTOR'),
                         dest='var_arithmetic',
-                        help="defines an input variable that grows according to an arithmetic progression",
+                        help="defines an input variable that grows according to an arithmetic progression, used only in grid search",
                         action='append')
 
     parser.add_argument('--vg',
                         type=str,
                         nargs=4,
                         default=[],
                         metavar=('NAME', 'MIN', 'MAX', 'FACTOR'),
                         dest='var_geometric',
-                        help="defines an input variable that grows according to a geometric progression",
+                        help="defines an input variable that grows according to a geometric progression, used only in grid search",
                         action='append')
 
     parser.add_argument('--repeat',
                         type=int,
                         metavar='R',
                         default='1',
                         dest='repeat',
@@ -144,14 +150,21 @@
                         type=str,
                         metavar='CMD',
                         required=True,
                         dest='cmd',
                         help="command to be executed. Use {VAR_NAME} to replace its parameters with a named variable",
                         action='append')
 
+    parser.add_argument('--score-pattern',
+                        type=str,
+                        metavar='REGEX',
+                        dest='score_pattern',
+                        help="Pattern used to capture the fitness of the particle, used only with CDEEPSO search",
+                        action='store')
+
     return parser.parse_args(args=argv)
 
 
 def parse_patas_parse(argv):
 
     # argparse for 'patas parse'
 
@@ -310,420 +323,313 @@
     parser.add_argument('--y-label', 
                         type=str, 
                         dest='y_label',
                         metavar='L',
                         help='label for the y axis',
                         action='store')
 
-    parser.add_argument('--r-label', 
+    parser.add_argument('--z-label', 
                         type=str, 
-                        dest='r_label',
+                        dest='z_label',
                         metavar='L',
-                        help='label for the reduced data',
+                        help='label for the colorbar',
                         action='store')
 
     parser.add_argument('--output', 
                         type=str, 
+                        default=None,
                         metavar='FILEPATH',
                         dest='output_file',
                         help='filepath of output file to save the image. If not present, the result will be displayed',
                         action='store')
 
-    parser.add_argument('--r-function', 
+    parser.add_argument('--aggfunc', 
                         type=str, 
-                        choices=('sum', 'mean', 'std', 'product', 'min', 'max'),
+                        choices=('sum', 'mean', 'std', 'product', 'min', 'max', 'count'),
                         default='mean',
-                        dest='r_function',
+                        dest='aggfunc',
                         metavar='NAME',
-                        help='each y,x pair will usualy map to multiple values, this function defines how to reduce them.',
+                        help='aggregation function to use when x,y coordinates map to multiple values.',
                         action='store')
 
-    parser.add_argument('--r-format', 
+    parser.add_argument('--fmt', 
                         type=str,  
                         metavar='CODE',
-                        dest='r_format',
-                        help='formats the reduced values for display. Example: --r-format \'int(R[y,x]*100)\'',
+                        dest='fmt',
+                        default='.2f',
+                        help='string used to format annotations',
                         action='store')
 
-    parser.add_argument('--size', 
+    parser.add_argument('--fig-size', 
                         type=float, 
                         nargs=2, 
-                        dest='size',
+                        dest='fig_size',
                         metavar='W H',
+                        default=DEFAULT_FIG_SIZE,
                         help='size of output image',
                         action='store')
 
-    parser.add_argument('--verbose', 
-                        help='print extra info during execution',
+    parser.add_argument('--annot', 
+                        help='Enable cell annotation',
+                        default=False,
                         action='store_true')
 
-    parser.add_argument('--colormap', 
-                        type=str, 
-                        dest='colormap',
-                        nargs='*',
-                        metavar=('NAME|C1', 'C2...'),
-                        help='list of HTML colors without # or name of colormap from https://matplotlib.org/stable/tutorials/colors/colormaps.html',
-                        action='store')
-
     return parser.parse_args(args=argv)
 
 
-def parse_patas_draw_bars(argv):
+def parse_patas_draw_categories(argv):
 
     parser = argparse.ArgumentParser(
-                        prog='patas draw bars',
+                        prog='patas draw categories',
                         description='Draws bars from a csv file',
                         epilog="Check the README.md to learn more tips on how to use this feature: https://github.com/diegofps/patas/blob/main/README.md",
                         formatter_class=argparse.RawDescriptionHelpFormatter)
 
     # INITIAL PARAMETERS
 
     parser.add_argument('--input', 
                         type=str, 
                         required=True, 
                         metavar='FILEPATH',
                         dest='input_file',
                         help='filepath to the csv file containing the data',
                         action='store')
 
+    parser.add_argument('--output', 
+                        type=str, 
+                        metavar='FILEPATH',
+                        dest='output_file',
+                        help='filepath of output file to save the image. If not present, the result will be displayed',
+                        action='store')
+
     parser.add_argument('--x-column', 
                         type=str, 
                         required=True, 
-                        metavar='X_COLUMN',
+                        metavar='NAME',
                         dest='x_column',
                         help='name of the x column in the data source',
                         action='store')
 
     parser.add_argument('--y-column', 
                         type=str, 
                         required=True, 
-                        metavar='Y_COLUMN',
+                        metavar='NAME',
                         dest='y_column',
                         help='name of the y column in the data source',
                         action='store')
 
+    parser.add_argument('--hue-column', 
+                        type=str, 
+                        metavar='NAME',
+                        dest='hue_column',
+                        help='name of the hue column in the data source, if necessary',
+                        action='store')
+
     parser.add_argument('--title', 
                         type=str, 
                         dest='title',
                         metavar='FILEPATH',
                         help='title of the graphic',
                         action='store')
 
     parser.add_argument('--x-label', 
                         type=str, 
                         metavar='L',
                         dest='x_label',
                         help='label for the x axis',
                         action='store')
 
-    parser.add_argument('--r-label', 
+    parser.add_argument('--y-label', 
                         type=str, 
-                        dest='r_label',
+                        dest='y_label',
                         metavar='L',
-                        help='label for the reduced values',
+                        help='label for the y axis',
                         action='store')
 
-    parser.add_argument('--output', 
+    parser.add_argument('--legend-label', 
                         type=str, 
-                        metavar='FILEPATH',
-                        dest='output_file',
-                        help='filepath of output file to save the image. If not present, the result will be displayed',
+                        dest='legend_label',
+                        metavar='L',
+                        help='label for the legend',
                         action='store')
 
     parser.add_argument('--x-change', 
                         type=str, 
                         metavar='CODE',
                         dest='x_change',
-                        help='transforms the x column using the variables X, Y, Z, math, and i. For example: --x-change "math.log2(X[i])"',
+                        help='transforms the x column. For example: --x-change "math.log2(X[i])"',
                         action='store')
 
     parser.add_argument('--y-change', 
                         type=str, 
                         metavar='CODE',
                         dest='y_change',
-                        help='transforms the y column using the variables X, Y, Z, math, and i. For example: --y-change "math.log2(Y[i])"',
+                        help='transforms the y column. For example: --y-change "math.log2(Y[i])"',
                         action='store')
 
-    parser.add_argument('--r-function', 
+    parser.add_argument('--hue-change', 
                         type=str, 
-                        choices=('sum', 'mean', 'std', 'product', 'min', 'max'),
-                        default='mean',
-                        dest='r_function',
-                        metavar='NAME',
-                        help='each x value will usualy map to multiple values, this function defines how to reduce them.',
-                        action='store')
-
-    parser.add_argument('--r-format', 
-                        type=str,  
                         metavar='CODE',
-                        dest='r_format',
-                        help='formats reduced values for display. Example: --r-format \'int(D[x]*100)\'',
+                        dest='hue_change',
+                        help='transforms the hue column. For example: --hue-change "math.log2(H[i])"',
                         action='store')
 
-    parser.add_argument('--size', 
+    parser.add_argument('--fig-size', 
                         type=float, 
                         nargs=2, 
-                        dest='size',
+                        dest='fig_size',
                         metavar='W H',
-                        help='size of output image',
+                        help='size of the output image',
                         action='store')
 
-    parser.add_argument('--verbose', 
-                        help='print extra info during execution',
-                        action='store_true')
-
-    parser.add_argument('--bar-color', 
-                        type=str, 
-                        dest='bar_color',
-                        metavar='COLOR',
-                        help='an HTML color without #',
-                        action='store')
-
-    parser.add_argument('--bar-size', 
-                        type=float, 
-                        dest='bar_size',
-                        metavar='W',
-                        help='size of each bar, a value from 0.0 to 1.0',
-                        action='store')
-
-    parser.add_argument('--border', 
-                        type=str,
-                        choices=('all', 'ticks', 'lines', 'none'),
-                        dest='border',
-                        metavar='MODE',
-                        help='style of the border, default is all',
-                        action='store')
-
-    parser.add_argument('--ticks', 
-                        type=int, 
-                        dest='ticks',
-                        metavar='T',
-                        help='number of values to appear in the axis',
-                        action='store')
-
-    parser.add_argument('--ticks-format', 
-                        type=str,  
-                        metavar='CODE',
-                        dest='ticks_format',
-                        help='formats tick display value using its current value t. Example: --ticks-format \'t:02f\'',
+    parser.add_argument('--errorbar',  
+                        dest='errorbar',
+                        choices=("sd", "se", "pi", "ci"),
+                        default=None,
+                        help='show error: standard deviation, standard error, percentile interval or confidence interval',
                         action='store')
 
-    parser.add_argument('--horizontal',  
-                        dest='horizontal',
-                        help='set this flag if you want horizontal bars',
-                        action='store_true')
-
-    parser.add_argument('--show-grid',  
-                        dest='show_grid',
-                        help='set this flag if you want gridlines displayed',
-                        action='store_true')
-
-    parser.add_argument('--show-error',  
-                        dest='show_error',
-                        help='set this flag if you want the standard deviation to be shown',
-                        action='store_true')
-
     return parser.parse_args(args=argv)
 
+
 def parse_patas_draw_lines(argv):
 
-    parser = ArgumentParser2(
+    parser = argparse.ArgumentParser(
                         prog='patas draw lines',
                         description='Draws lines from a csv file',
                         epilog="Check the README.md to learn more tips on how to use this feature: https://github.com/diegofps/patas/blob/main/README.md",
                         formatter_class=argparse.RawDescriptionHelpFormatter)
 
-
     # GENERAL PARAMETERS
 
     parser.add_argument('--input', 
                         type=str, 
                         required=True, 
                         metavar='FILEPATH',
                         dest='input_file',
                         help='filepath to the csv file containing the data',
                         action='store')
 
+    parser.add_argument('--output', 
+                        type=str, 
+                        metavar='FILEPATH',
+                        dest='output_file',
+                        help='filepath of output file to save the image. If not present, the result will be displayed',
+                        action='store')
+
     parser.add_argument('--title', 
                         type=str, 
                         dest='title',
                         metavar='FILEPATH',
                         help='title of the graphic',
                         action='store')
 
     parser.add_argument('--x-label', 
                         type=str, 
                         metavar='L',
                         dest='x_label',
                         help='label for the x axis',
                         action='store')
 
-    parser.add_argument('--r-label', 
+    parser.add_argument('--y-label', 
                         type=str, 
-                        dest='r_label',
+                        dest='y_label',
                         metavar='L',
-                        help='label for the reduced values',
-                        action='store')
-
-    parser.add_argument('--output', 
-                        type=str, 
-                        metavar='FILEPATH',
-                        dest='output_file',
-                        help='filepath of output file to save the image. If not present, the result will be displayed',
-                        action='store')
-
-    parser.add_argument('--size', 
-                        type=float, 
-                        nargs=2, 
-                        dest='size',
-                        metavar='W H',
-                        help='size of output image',
-                        action='store')
-
-    parser.add_argument('--verbose', 
-                        help='print extra info during execution',
-                        action='store_true')
-
-    parser.add_argument('--border', 
-                        type=str,
-                        choices=('all', 'ticks', 'lines', 'none'),
-                        dest='border',
-                        metavar='MODE',
-                        help='style of the border, default is all',
-                        action='store')
-
-    parser.add_argument('--ticks', 
-                        type=int, 
-                        dest='ticks',
-                        metavar='T',
-                        help='number of values to appear in the axis',
-                        action='store')
-
-    parser.add_argument('--ticks-format', 
-                        type=str,  
-                        metavar='CODE',
-                        dest='ticks_format',
-                        help='formats tick display value using its current value t. Example: --ticks-format \'t:02f\'',
+                        help='label for the y axis',
                         action='store')
 
-    parser.add_argument('--legend-location', 
+    parser.add_argument('--legend-label', 
                         type=str, 
-                        choices=('tr', 'tl', 'bl', 'br', 'cr', 'cl', 'tc', 'bc', 'cc', 'c'),
-                        default=None,
-                        dest='legend_location',
-                        metavar='YX',
-                        help='Position of the legend (t=top, b=bottom, c=center, r=right, l=left)',
+                        dest='legend_label',
+                        metavar='L',
+                        help='label for the legend',
                         action='store')
 
-    parser.add_argument('--show-grid', 
-                        dest='show_grid', 
-                        help='set this flag if you want gridlines displayed', 
-                        action='store_true')
-
-    parser.add_argument('--show-error',  
-                        dest='show_error',
-                        help='set this flag if you want the standard deviation to be shown',
-                        action='store_true')
-
-
-    # LINE PARAMETERS
-
-    parser.add_argument_group('Line parameters')
-
-    lines = parser.add_argument('--new-line', 
-                                dest='lines',
-                                help='begin definition of a new line',
-                                action='create_context')
-
     parser.add_argument('--x-column', 
                         type=str, 
+                        required=True, 
+                        metavar='NAME',
                         dest='x_column',
-                        metavar='X_COLUMN',
                         help='name of the x column in the data source',
-                        action='store',
-                        context=lines)
+                        action='store')
 
     parser.add_argument('--y-column', 
                         type=str, 
-                        metavar='Y_COLUMN',
+                        required=True, 
+                        metavar='NAME',
                         dest='y_column',
                         help='name of the y column in the data source',
-                        action='store',
-                        context=lines)
+                        action='store')
+
+    parser.add_argument('--hue-column', 
+                        type=str, 
+                        metavar='NAME',
+                        dest='hue_column',
+                        help='name of the hue column in the data source, if necessary',
+                        action='store')
+
+    parser.add_argument('--style-column', 
+                        type=str, 
+                        metavar='NAME',
+                        dest='style_column',
+                        help='name of the style column in the data source, if necessary',
+                        action='store')
 
     parser.add_argument('--x-change', 
                         type=str, 
                         metavar='CODE',
                         dest='x_change',
-                        default=None,
                         help='transforms the x column. For example: --x-change "math.log2(X[i])"',
-                        action='store',
-                        context=lines)
+                        action='store')
 
     parser.add_argument('--y-change', 
                         type=str, 
                         metavar='CODE',
                         dest='y_change',
                         help='transforms the y column. For example: --y-change "math.log2(Y[i])"',
-                        action='store',
-                        context=lines)
-
-    parser.add_argument('--r-function', 
-                        type=str, 
-                        choices=('sum', 'mean', 'std', 'product', 'min', 'max'),
-                        default='mean',
-                        dest='r_function',
-                        metavar='NAME',
-                        help='each x value will usualy map to multiple values, this function defines how to reduce them.',
-                        action='store',
-                        context=lines)
-
-    parser.add_argument('--label', 
-                        type=str, 
-                        dest='label',
-                        metavar='NAME',
-                        help='label representing this line in the legend',
-                        action='store',
-                        context=lines)
+                        action='store')
 
-    parser.add_argument('--style', 
+    parser.add_argument('--hue-change', 
                         type=str, 
-                        choices=('solid', 'dash', 'dashdot', 'dot'),
-                        default=None,
-                        dest='style',
-                        metavar='NAME',
-                        help='style used to draw the line',
-                        action='store',
-                        context=lines)
+                        metavar='CODE',
+                        dest='hue_change',
+                        help='transforms the hue column. For example: --hue-change "math.log2(H[i])"',
+                        action='store')
 
-    parser.add_argument('--marker', 
+    parser.add_argument('--style-change', 
                         type=str, 
-                        choices=('point', 'circle', 'x', 'diamond', 'hexagon', 'square', 'plus'),
-                        default=None,
-                        dest='marker',
-                        metavar='NAME',
-                        help='marker used to highlight the points in the line',
-                        action='store',
-                        context=lines)
+                        metavar='CODE',
+                        dest='style_change',
+                        help='transforms the style column. For example: --style-change "math.log2(S[i])"',
+                        action='store')
 
-    parser.add_argument('--marker-size', 
+    parser.add_argument('--fig-size', 
                         type=float, 
-                        default=5,
-                        dest='marker_size',
-                        metavar='FLOAT',
-                        help='size of the marker',
-                        action='store',
-                        context=lines)
+                        nargs=2, 
+                        dest='fig_size',
+                        metavar='W H',
+                        help='size of output image',
+                        action='store')
 
+    parser.add_argument('--errorbar',  
+                        dest='errorbar',
+                        choices=("sd", "se", "pi", "ci"),
+                        default=None,
+                        help='show error: standard deviation, standard error, percentile interval or confidence interval',
+                        action='store')
 
+    parser.add_argument('--err-style',  
+                        dest='err_style',
+                        default='band',
+                        choices=('band', 'bars'),
+                        help='set the err_style to render: band or bars',
+                        action='store')
 
     args = parser.parse_args(args=argv)
 
-    print(args)
-    
     return args
 
 
 class ArgumentParser2(argparse.ArgumentParser):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
```

### Comparing `patas-2.0.5/patas/graphics.py` & `patas-2.0.6/patas/graphics.old.py`

 * *Files identical despite different names*

### Comparing `patas-2.0.5/patas/grid_explorer.py` & `patas-2.0.6/patas/scheduler.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-from .utils import expand_path, error, warn, info, debug, critical, abort, readlines, clean_folder, estimate, human_time, quote, colors
-from .schemas import Experiment, Cluster, Node, format_as_dict
+from .utils import expand_path, error, warn, info, debug, critical, abort, readlines, estimate, human_time, quote, colors, confirm
+from .schemas import ClusterSchema, NodeSchema, Task
 
 from multiprocessing import Process, Queue
-from subprocess import Popen, PIPE
+from subprocess import Popen, PIPE, STDOUT
 from datetime import datetime
 
-import hashlib
-import base64
 import select
 import shlex
 import copy
 import time
-import yaml
 import pty
 import sys
 import os
 
 
 KEY_SSH_ON  = b'74ffc7c4-a6ad-4315-94cb-59d045a230c0'
 KEY_SSH_OFF = b'93dfc971-fa64-4beb-a24e-d8874738b9ca'
@@ -26,32 +23,14 @@
 
 ECHO_SSH_ON  = build_echo_cmd(KEY_SSH_ON)
 ECHO_SSH_OFF = build_echo_cmd(KEY_SSH_OFF)
 ECHO_CMD_ON  = build_echo_cmd(KEY_CMD_ON)
 ECHO_CMD_OFF = b" echo -en \"\n $? %s\"" % KEY_CMD_OFF.replace(b"-", b"-\b-")
 
 
-def combine_variables(variables, combination={}):
-
-    if len(variables) == len(combination):
-        yield copy.copy(combination)
-    
-    else:
-        var = variables[len(combination)]
-        name = var.name
-        
-        for value in var.values:
-            combination[name] = value
-            
-            for tmp in combine_variables(variables, combination):
-                yield tmp
-            
-        del combination[name]
-
-
 class WorkerMessage(dict):
 
     def __init__(self, action, source=-1):
         self.action = action
         self.source = source
         self.data = {}
     
@@ -64,83 +43,53 @@
     def __getattr__(self, key):
         return self[key]
     
     def __setattr__(self, key, value):
         self[key] = value
 
 
-class Task:
-
-    def __init__(self, 
-            experiment_name, task_output_dir, work_dir, experiment_idd, combination_idd, 
-            repeat_idd, task_idd, combination, cmdlines, max_tries):
-
-        self.experiment_name = experiment_name
-        self.combination_idd = combination_idd
-        self.experiment_idd  = experiment_idd
-        self.output_dir      = task_output_dir
-        self.combination     = combination
-        self.repeat_idd      = repeat_idd
-        self.max_tries       = max_tries
-        self.work_dir        = work_dir
-        self.task_idd        = task_idd
-        self.commands        = cmdlines
-        self.assigned_to     = None
-        self.started_at      = None
-        self.ended_at        = None
-        self.duration        = None
-        self.success         = None
-        self.output          = None
-        self.status          = None
-        self.tries           = 0
-    
-    
-    def __repr__(self):
-
-        combination = ";".join(f"{k}={v}" for k, v in self.combination.items())
-        return f"{self.experiment_idd} {self.combination_idd} {self.repeat_idd} {self.task_idd} {combination} {self.commands}"
-
-
 class ExecutorBuilder:
 
     def __init__(self, executor_type, node):
         self.executor_type = executor_type
         self.node = node
 
-
     def __call__(self):
         return self.executor_type(self.node)
 
 
 class BashExecutor:
     
     def __init__(self, node):
 
         self.is_alive = True
         self.node = node
     
-
     def execute(self, initrc, cmds):
 
         if type(cmds) is not list:
             cmds = [cmds]
 
-        cmds = [x + b' 2>&1 ' for x in cmds]
-
         p1 = b" ; ".join(initrc)
         p3 = b" ; ".join(cmds)
 
         cmd_str = b" %s ; %s " % (p1, p3)
-        cmd_str = "bash -c " + quote(cmd_str.decode('utf-8'))
-        
-        ps = Popen(shlex.split(cmd_str), stdout=PIPE)
+        cmd_str = cmd_str.decode('utf-8')
+        cmd_str = " bash -c " + quote(cmd_str)
+        # print(cmd_str)
+        
+        ps = Popen(shlex.split(cmd_str), stdout=PIPE, stderr=STDOUT)
+        stdout, _ = ps.communicate()
+        status = ps.returncode
+        # print(status)
 
-        status = ps.wait()
-        stdout = ps.stdout
+        # status = ps.wait()
+        # stdout = ps.stdout.read()
 
+        # print("after wait")
         return (status == 0), stdout, status
 
 
 class SSHExecutor:
 
     def __init__(self, node):
 
@@ -151,15 +100,14 @@
         self.master, self.slave = pty.openpty()
         self._start_bash()
         
         self.conn_string = self._build_connnection_string(self.node)
 
         self._connect()
     
-
     def _build_connnection_string(self, node):
 
         tokens = [b' ssh']
 
         if node.private_key:
             tokens.append(b' -i ')
             tokens.append(node.private_key.encode())
@@ -175,28 +123,26 @@
         tokens.append(ECHO_SSH_ON)
         tokens.append(b" ; bash' ; ")
         tokens.append(ECHO_SSH_OFF)
         tokens.append(b'\n')
         
         return b"".join(tokens)
 
-
     def _start_bash(self):
 
         debug("Starting bash")
 
         self.popen = Popen(
                 shlex.shlex("bash"),
                 preexec_fn=os.setsid,
                 stdin=self.slave,
                 stdout=self.slave,
                 stderr=self.slave,
                 universal_newlines=True)
 
-
     def _connect(self):
 
         conn_try = 1
 
         while True:
             debug("Connection attempt:", conn_try)
 
@@ -234,15 +180,14 @@
                     warn("SSH connection against %s has failed, trying again" % self.node.name)
                     break
 
             warn("Sleeping before next try...")
             time.sleep(1)
             conn_try += 1
 
-
     def execute(self, initrc, cmds):
 
         if type(cmds) is not list:
             cmds = [cmds]
 
         lines = []
         output_start = 0
@@ -284,485 +229,368 @@
                     #debug("Found KEY_CMD_OFF")
                     output_end = i
             
             if output_end is not None:
                 status = lines[output_end].strip().split()[0].decode("utf-8") if output_end < len(lines) else "255"
                 break
 
-        return (status == "0"), lines[output_start:output_end], status
+        return (status == "0"), b'\n'.join(lines[output_start:output_end]), status
 
 
 class WorkerProcess:
 
-    def __init__(self, worker_idd, executor_builder, env_variables):
+    def __init__(self, worker_idd_in_lab, worker_idd_in_cluster, worker_idd_in_node, executor_builder, env_variables):
 
+        self.worker_idd_in_lab = worker_idd_in_lab
+        self.worker_idd_in_cluster = worker_idd_in_cluster
+        self.worker_idd_in_node = worker_idd_in_node
         self.executor_builder = executor_builder
         self.env_variables = env_variables
-        self.worker_idd = worker_idd
         self.process = None
         self.queue = None
 
-
     def start(self, queue_master):
 
-        self.queue = Queue()
+        self.queue   = Queue()
         self.process = Process(target=self.run, args=(self.queue, queue_master))
         self.process.start()
 
-
     def run(self, queue_in, queue_master):
 
         try:
             executor = self.executor_builder()
 
-            msg_out = WorkerMessage("ready", self.worker_idd)
+            msg_out = WorkerMessage("ready", self.worker_idd_in_lab)
             queue_master.put(msg_out)
             
             while True:
                 msg_in = queue_in.get()
 
                 if msg_in.action == "execute":
-                    success = self.execute(msg_in, executor)
 
-                    msg_out = WorkerMessage("finished", self.worker_idd)
-                    msg_out.success = success
+                    msg_out = WorkerMessage("finished", self.worker_idd_in_lab)
+                    msg_out.task = self.execute(msg_in, executor)
                     queue_master.put(msg_out)
 
                     if not executor.is_alive:
                         executor = self.executor_builder()
 
-                    msg_out = WorkerMessage("ready", self.worker_idd)
+                    msg_out = WorkerMessage("ready", self.worker_idd_in_lab)
                     queue_master.put(msg_out)
                 
                 elif msg_in.action == "terminate":
                     break
                 
                 else:
-                    warn("Unknown action:", msg_in.action)
+                    warn(f"Unknown action: {msg_in.action}")
             
-            msg_out = WorkerMessage("ended", self.worker_idd)
+            msg_out = WorkerMessage("ended", self.worker_idd_in_lab)
             queue_master.put(msg_out)
+            
         except KeyboardInterrupt:
             pass
 
-
     def execute(self, msg_in, executor):
 
         task:Task = msg_in.task
 
         # Prepare the initrc
 
         env_variables = copy.copy(self.env_variables)
         env_variables["PATAS_WORK_DIR"] = task.work_dir
+        env_variables["PATAS_ATTEMPT"] = str(task.tries + 1)
 
         for k,v in task.combination.items():
             env_variables["PATAS_VAR_" + k] = str(v)
 
         initrc = [b"export %s=\"%s\"" % (a.encode(), b.encode()) for a, b in env_variables.items()]
-        initrc.insert(0, b"cd \"%s\"" % task.work_dir.encode())
+
+        if task.work_dir:
+            initrc.insert(0, b"cd \"%s\"" % task.work_dir.encode())
+
+        initrc.insert(0, b'set -e')
 
         # Prepare the command line we will execute
 
         cmdline = " ; ".join(task.commands).encode()
 
         # Execute this task
 
-        task.started_at = datetime.now()
-        task.success, task.output, task.status = executor.execute(initrc, cmdline)
-        task.ended_at = datetime.now()
-        task.duration = (task.ended_at - task.started_at).total_seconds()
-
-        # Create the task folder and clean any old .done file
-
-        done_filepath = os.path.join(task.output_dir, ".done")
-        os.makedirs(task.output_dir, exist_ok=True)
-        if os.path.exists(done_filepath):
-            os.remove(done_filepath)
-
-        # Dump task info
-        
-        info = {
-            "task_id": task.task_idd,
-            "repeat_id": task.repeat_idd,
-            "experiment_id": task.experiment_idd,
-            "experiment_name": task.experiment_name,
-            "combination_id": task.combination_idd,
-            "combination": task.combination,
-            "started_at": task.started_at,
-            "ended_at": task.ended_at,
-            "duration": task.duration,
-            "env_variables": env_variables,
-            "max_tries": task.max_tries,
-            "tries": task.tries + 1,
-            "output_dir": task.output_dir,
-            "work_dir": task.work_dir,
-            "commands": task.commands,
-            "assigned_to": task.assigned_to,
+        started_at = datetime.now()
+        task.success, stdout, status = executor.execute(initrc, cmdline)
+        ended_at = datetime.now()
+        duration = (ended_at - started_at).total_seconds()
+
+        # Add result to the task results
+
+        result = {
+            'env_variables': env_variables,
+            'started_at': started_at,
+            'ended_at': ended_at,
+            'duration': duration,
+            'stdout': stdout,
+            'status': status,
         }
 
-        filepath = os.path.join(task.output_dir, "info.yml")
-        with open(filepath, "w") as fout:
-            yaml.dump(info, fout, default_flow_style=False)
+        task.attempts.append(result)
         
-        # Dump task output
-
-        filepath = os.path.join(task.output_dir, "stdout")
-        with open(filepath, "wb") as fout:
-            fout.writelines(task.output)
-
-        # Create .done file if the task succeded
-
-        if task.success:
-            with open(done_filepath, 'a'):
-                os.utime(done_filepath, None)
-
-        # Write output to stdout if the task failed
-
-        else:
-            warn("--- TASK %d FAILED WITH EXIT CODE %s ---" % (task.task_idd, task.status))
-            for line in task.output:
-                os.write(sys.stdout.fileno(), line)
-            warn("--- END OF FAILED OUTPUT ---")
+        # Return True if the task succeeded
 
-        return task.success
+        return task
 
 
-class GridExplorer():
+class Scheduler():
 
-    def __init__(self, task_filters, node_filters, 
-            output_dir, redo_tasks, recreate, confirmed,
-            experiments, clusters):
+    def __init__(self, node_filters, output_dir, redo_tasks, confirmed, experiments, clusters, quiet):
 
-        self.output_folder = expand_path  (output_dir)
-        self.task_filters  = task_filters
+        self.output_folder = expand_path(output_dir)
         self.node_filters  = node_filters
         self.experiments   = experiments
         self.redo_tasks    = redo_tasks
         self.confirmed     = confirmed
-        self.recreate      = recreate
         self.clusters      = clusters
+        self.quiet         = quiet
+        self.todo          = []
 
         self.workers:list[WorkerProcess] = None
-        self.tasks  :list[Task         ] = None
-
 
     def start(self):
 
         os.makedirs(self.output_folder, exist_ok=True)
 
-        self._show_summary(self.experiments, self.clusters, self.confirmed)
-        self._write_signature()
-        self.tasks   = self._create_tasks(self.experiments, self.output_folder, self.redo_tasks, self.task_filters)
+        self.show_summary(self.experiments, self.clusters, self.confirmed)
         self.workers = self._create_workers(self.clusters, self.node_filters)
         self._exec()
 
+    def push_todo(self, task):
+        self.todo.append(task)
+
+    def push_done(self, task):
+        self.done.append(task)
+
+    def push_filtered(self, task):
+        self.filtered.append(task)
 
-    def _show_summary(self, experiments, clusters, confirmed):
+    def show_summary(self, experiments, clusters, confirmed):
 
         # Display experiments
 
         print(colors.white("\n --- Experiments --- \n"))
 
-        experiment: Experiment = None
         total_tasks = 0
-
         for experiment in experiments:
-            variables = experiment.vars
-            current = 1
-
-            for var in variables:
-                current *= len(var.values)
-            
-            current *= experiment.repeat
-            total_tasks += current
-
-            print(f"'{experiment.name}' has {len(variables)} variable(s) and produces {current} task(s):")
-            for var in variables:
-                print(f"    {var.name} = {str(var.values)}, len = {len(var.values)}")
+            experiment.show_summary()
+            total_tasks += experiment.number_of_tasks()
         
         # Display clusters
 
         print(colors.white("\n --- Clusters --- \n"))
 
-        total_nodes = 0
+        total_nodes   = 0
         total_workers = 0
-        node:Node = None
-        cluster:Cluster = None
-
         for cluster in clusters:
-            total_nodes += len(cluster.nodes)
-            print(f"'{cluster.name}' has {len(cluster.nodes)} node(s):")
-
-            for node in cluster.nodes:
-                total_workers += node.workers
-                print(f"    '{node.name}' has {node.workers} worker(s)")
-        
+            cluster.show_summary()
+            total_nodes   += cluster.number_of_nodes()
+            total_workers += cluster.number_of_workers()
+            
         # Display total numbers and estimations
 
         print(colors.white("\n --- Overview --- \n"))
 
         print(f"Redo:          {self.redo_tasks}")
-        print(f"Task filters:  {self.task_filters}")
         print(f"Node filters:  {self.node_filters}")
         print(f"Output folder: {self.output_folder}")
-        print(f"Recreate:      {self.recreate}")
 
         print()
 
-        print(f"Total number of clusters: {len(clusters)}")
-        print(f"Total number of nodes:    {total_nodes}")
-        print(f"Total number of workers:  {total_workers}")
-        print(f"Total number of tasks:    {total_tasks}")
+        print(f"Number of experiments: {len(experiments)}")
+        print(f"Number of clusters:    {len(clusters)}")
+        print(f"Number of nodes:       {total_nodes}")
+        print(f"Number of workers:     {total_workers}")
+        print(f"Number of tasks:       {total_tasks}")
 
         print()
 
-        print('Estimated time to complete if each task takes:')
-        print(f"    One second: { estimate(total_tasks, total_workers,        1) }")
-        print(f"    One minute: { estimate(total_tasks, total_workers,       60) }")
-        print(f"    One hour:   { estimate(total_tasks, total_workers,    60*60) }")
-        print(f"    One day:    { estimate(total_tasks, total_workers, 60*60*24) }")
+        # Check experiment signatures
 
-        print()
+        issues = [x for x in experiments if not x.check_signature(self.output_folder)]
+
+        if issues:
+            names = ', '.join([x.name for x in issues])
+            warn(f"The following experiments have changed their configuration, proceeding will restart all their tasks: {names}")
 
         # Confirm
 
         if not confirmed:
-            try:
-                while True:
-                    option = input('Do you want to continue? [Y/n] ').strip()
-                    if option in ['Y', 'y', '']:
-                        break
-                    elif option in ['N', 'n']:
-                        sys.exit(0)
-                    else:
-                        print('Invalid option')
-            except KeyboardInterrupt:
-                sys.exit(0)
-
-    def _write_signature(self):
-
-        # Calculate the signature for the received configuration
-
-        key = hashlib.md5()
-
-        key.update(str(format_as_dict(self.experiments)).encode())
-
-        signature = base64.b64encode(key.digest()).decode("utf-8")
-
-        # Data to be saved into the signature file
-
-        info = {
-            "output_folder": self.output_folder,
-            "task_filters": self.task_filters,
-            "node_filters": self.node_filters,
-            "experiments": format_as_dict(self.experiments),
-            "redo_tasks": self.redo_tasks,
-            "recreate": self.recreate,
-            "clusters": format_as_dict(self.clusters),
-            "signature": signature
-        }
-
-        # Load the previous signature file, if it exists
-
-        info_filepath = os.path.join(self.output_folder, "info.yml")
-
-        try:
-            with open(info_filepath, "r") as fin:
-                other = yaml.load(fin, Loader=yaml.FullLoader)
-        except:
-            other = None
-
-        # If the previous file was loaded and it has a signature, compare it to the current signature
-
-        if other and "signature" in other and other["signature"] != signature:
-            if self.recreate:
-                print("Recreating output folder...")
-                clean_folder(self.output_folder)
-            else:
-                abort("The output folder contains a different output configuration. Provide an empty folder or add the parameter --recreate to overwrite this one")
-
-        # Write the new signature file
-            
-        with open(info_filepath, "w") as fout:
-            yaml.dump(info, fout, default_flow_style=False)
-
-
-    def _create_tasks(self, experiments, output_folder, redo_tasks, task_filters):
-
-        print("Creating tasks...")
-
-        e:Experiment = None
-        combination_idd = -1
-        experiment_idd = -1
-        task_idd = -1
-        tasks = []
-
-        for e in experiments:
-
-            experiment_idd += 1
-
-            experiment_filepath = os.path.join(output_folder, e.name)
-            info_filepath = os.path.join(experiment_filepath, "info.yml")
-            os.makedirs(experiment_filepath, exist_ok=True)
-
-            info = {
-                "experiment_name": e.name,
-                "workdir": e.workdir,
-                "commands": e.cmd,
-                "repeat": e.repeat,
-                "max_tries": e.max_tries,
-                "variables": {v.name:v.values for v in e.vars}
-            }
-
-            with open(info_filepath, "w") as fout:
-                yaml.dump(info, fout, default_flow_style=False)
-
-            for combination in combine_variables(e.vars):
-                combination_idd += 1
-
-                for repeat_idd in range(e.repeat):
-                    task_idd += 1
-
-                    if task_filters and not any(a <= task_idd < b for a, b in task_filters):
-                        continue
-
-                    task_output_folder = os.path.join(experiment_filepath, str(task_idd))
-
-                    if not redo_tasks and os.path.exists(os.path.join(task_output_folder, ".done")):
-                        continue
-
-                    cmds = [x.format(**combination) for x in e.cmd]
+            confirm()
+        
+        # Clean diverging experiments
 
-                    task = Task(e.name, task_output_folder, e.workdir, experiment_idd, combination_idd, repeat_idd, task_idd, combination, cmds, e.max_tries)
-                    tasks.append(task)
+        if issues:
+            warn("Cleaning diverging experiments...")
+            for experiment in issues:
+                experiment.clean_output()
 
-        if not tasks:
-            abort("No tasks to do.")
-        
-        return tasks
+        # Write signature files
 
+        for experiment in experiments:
+            experiment.write_info()
 
     def _create_workers(self, clusters, node_filters):
 
         print("Creating workers...")
 
+        worker_idd_in_lab = -1
+        node_idd_in_lab = -1
         cluster_idd = -1
-        worker_idd = -1
-        node_idd = -1
 
         workers = []
 
-        cluster:Cluster = None
-        node:Node = None
+        cluster:ClusterSchema = None
+        node:NodeSchema = None
 
         for cluster in clusters:
+
+            worker_idd_in_cluster = -1
+            node_idd_in_cluster = -1
             cluster_idd += 1
 
             for node in cluster.nodes:
-                node_idd += 1
+
+                worker_idd_in_node = -1
+                node_idd_in_cluster += 1
+                node_idd_in_lab += 1
+
+                node.cluster_idd = node_idd_in_cluster
+                node.global_idd = node_idd_in_lab
 
                 for _ in range(node.workers):
-                    worker_idd += 1
+
+                    worker_idd_in_cluster += 1
+                    worker_idd_in_lab += 1
+                    worker_idd_in_node += 1
 
                     if node_filters and not any(all(tag in node.tags for tag in filter) for filter in node_filters):
                         continue
 
                     if node.hostname in ['localhost', '127.0.0.1']:
-                        builder = ExecutorBuilder(BashExecutor, node)    
+                        builder = ExecutorBuilder(BashExecutor, node)
+
                     else:
                         builder = ExecutorBuilder(SSHExecutor, node)
 
                     env_variables = {
                         "PATAS_CLUSTER_NAME": cluster.name,
-                        "PATAS_NODE_NAME": node.name,
+                        "PATAS_NODE_NAME":    node.name,
 
-                        "PATAS_CLUSTER_ID": str(cluster_idd),
-                        "PATAS_NODE_ID": str(node_idd),
-                        "PATAS_WORKER_ID": str(worker_idd)
+                        "PATAS_CLUSTER_IN_LAB":    str(cluster_idd),
+                        "PATAS_NODE_IN_LAB":       str(node_idd_in_lab),
+                        "PATAS_NODE_IN_CLUSTER":   str(node_idd_in_cluster),
+                        "PATAS_WORKER_IN_LAB":     str(worker_idd_in_lab),
+                        "PATAS_WORKER_IN_CLUSTER": str(worker_idd_in_cluster),
+                        "PATAS_WORKER_IN_NODE":    str(worker_idd_in_node),
                     }
 
-                    worker = WorkerProcess(worker_idd, builder, env_variables)
+                    worker = WorkerProcess(worker_idd_in_lab, worker_idd_in_cluster, worker_idd_in_node, builder, env_variables)
                     workers.append(worker)
         
         if not workers:
             abort("No workers to work.")
         
         return workers
 
-
     def _exec(self):
 
         self.queue    = Queue()
 
-        self.todo     = copy.copy(self.tasks)
+        self.todo     = []
         self.doing    = []
         self.done     = []
         self.given_up = []
+        self.filtered = []
 
         self.idle     = []
         self.ended    = []
 
-        len_todo      = len(str(len(self.todo)))
-        len_workers   = len(str(len(self.workers)))
+        chars_todo    = 10
+        chars_work    = 10
         
         # Start workers
 
         print()
-        info("Starting %d worker(s)" % len(self.workers))
+        info(f"Starting {len(self.workers)} worker(s)")
 
         for worker in self.workers:
             worker.start(self.queue)
         
         info("Worker(s) started")
 
+        # Start experiments
+
+        print()
+        info(f"Starting {len(self.experiments)} experiment(s)")
+        
+        for experiment in self.experiments:
+            experiment.on_start(self)
+        
+        info("Experiment(s) started")
+
         # Main loop
 
         main_loop_started_at = datetime.now()
 
         try:
 
             print()
-            info("Starting main loop")
+            info("Starting main loop...")
 
             while self.todo or self.doing:
 
                 msg_in = self.queue.get()
 
-                l1 = str(len(self.todo    ))
-                l2 = str(len(self.doing   ))
-                l3 = str(len(self.done    ))
-                l4 = str(len(self.given_up))
-
-                d  = colors.gray("|%s|" % str(datetime.now()))
-                l1 = colors.white(" " * (len_todo    - len(l1)) + l1 + " |")
-                l2 = colors.white(" " * (len_workers - len(l2)) + l2 + " |")
-                l3 = colors.green(" " * (len_todo    - len(l3)) + l3 + " |")
-                l4 = colors.red  (" " * (len_todo    - len(l4)) + l4 + " |")
+                if not self.quiet:
+                    l1 = str(len(self.todo    ))
+                    l2 = str(len(self.doing   ))
+                    l3 = str(len(self.done    ))
+                    l4 = str(len(self.given_up))
+                    l5 = str(len(self.filtered))
+
+                    d  = colors.gray  ("|%s|" % str(datetime.now()))
+                    l1 = colors.white ('|TODO:'     + " " * (chars_todo - len(l1)) + l1 + "|")
+                    l2 = colors.green ('|DOING:'    + " " * (chars_work - len(l2)) + l2 + "|")
+                    l3 = colors.blue  ('|DONE:'     + " " * (chars_todo - len(l3)) + l3 + "|")
+                    l4 = colors.red   ('|GIVEN_UP:' + " " * (chars_todo - len(l4)) + l4 + "|")
+                    l5 = colors.purple('|FILTERED:' + " " * (chars_todo - len(l5)) + l5 + "|")
 
-                print(f"{d} {l1} {l2} {l3} {l4}")
+                    print(f"{d} {l1} {l2} {l3} {l4} {l5}")
 
                 if msg_in.action == "ready":
-                    self._ready(msg_in)
+                    self._on_worker_is_ready(msg_in)
                 
                 elif msg_in.action == "finished":
-                    self._finished(msg_in)
+                    self._on_task_finished(msg_in)
                 
                 else:
                     warn("Unknown action:", msg_in.action)
             
             info("Main loop completed")
 
         except KeyboardInterrupt:
 
             print("Operation interrupted")
             return
 
         main_loop_ended_at = datetime.now()
         main_loop_duration = (main_loop_ended_at - main_loop_started_at).total_seconds()
         
+        # Send on_finish to all experiments
+
+        for experiment in self.experiments:
+            experiment.on_finish()
+
         # Terminate workers
 
         terminate_loop_started_at = datetime.now()
 
         try:
             print()
             info("Releasing workers...")
@@ -776,27 +604,16 @@
             # Waiting for ENDED signal
 
             while len(self.workers) != len(self.ended):
 
                 msg = self.queue.get()
 
                 if msg.action == "ended":
-
                     self.ended.append(msg.source)
 
-                    d = colors.gray("|%s|" % str(datetime.now()))
-
-                    l1 = str(len(self.ended))
-                    l2 = str(len(self.workers))
-
-                    l1 = " " * (len_workers - len(l1)) + l1
-                    l2 = " " * (len_workers - len(l2)) + l2
-
-                    print("%s %sEnded %s / %s%s" % (d, colors.WHITE, l1, l2, colors.RESET))
-                
                 else:
                     #debug("Ignoring action %s from %s, execution is ending" % (msg.source, msg.action))
                     pass
 
             info("All workers are resting.")
             
         except KeyboardInterrupt:
@@ -806,62 +623,122 @@
 
         terminate_loop_ended_at = datetime.now()
         terminate_loop_duration = (terminate_loop_ended_at - terminate_loop_started_at).total_seconds()
         
         # Display execution summary
 
         print(colors.white("\n --- Execution Summary --- \n"))
-        print(f"    Time to execute tasks: {human_time(main_loop_duration)}")
-        print(f"    Time to terminate workers: {human_time(terminate_loop_duration)}")
-        print(f"    Tasks requested: {len(self.tasks)}")
+
+        print(f"    Time to execute experiments: {human_time(main_loop_duration)}")
+        print(f"    Time to terminate workers:   {human_time(terminate_loop_duration)}")
+        print(f"    Tasks requested: {len(self.done) + len(self.given_up)}")
         print(f"    Tasks completed: {len(self.done)}")
-        print(f"    Tasks given up: {len(self.given_up)}")
+        print(f"    Tasks given up:  {len(self.given_up)}")
         print()
 
-    def _ready(self, msg_in):
+        # if self.given_up:
+        #     print("Gave up on:", [t.task_idd for t in self.given_up])
+        
+        # if self.done:
+        #     print("Done:", [t.task_idd for t in self.done])
+
+    def _on_worker_is_ready(self, msg_in):
+
+        # If there is a task to be done, send it back to the worker
 
         if self.todo:
             msg_out = WorkerMessage("execute")
             msg_out.task = self.todo.pop()
             msg_out.task.assigned_to = msg_in.source
 
             self.doing.append(msg_out.task)
             self.workers[msg_in.source].queue.put(msg_out)
+
+            # if not self.quiet:
+            #     print(f"Sending task {msg_out.task.task_idd} to worker {msg_in.source}")
         
+        # Otherwise, move the worker to the like of idle workers
+
         else:
             self.idle.append(msg_in.source)
 
+            # if not self.quiet:
+            #     print(f"Moving worker {msg_in.source} to idle")
+
+    def _on_task_finished(self, msg_in):
 
-    def _finished(self, msg_in):
+        # Find the position of the task we just received in the message
 
         for i, x in enumerate(self.doing):
             if x.assigned_to == msg_in.source:
                 break
-        
-        if i == len(self.doing):
-            warn("Received finished msg but the task was not found inside the doing list")
+        else:
+            critical(f"Received finished event for task {msg_in.task.task_idd}, which was not found inside the doing list")
             return
         
-        task:Task = self.doing[i]
-        del self.doing[i]
+        # Retrieve the task we sent the worker
+
+        task_sent:Task = self.doing[i]
+
+        # Retrieve the task we received back
+
+        task:Task = msg_in.task
+
+        # Check if they are the same, otherwise something weird is happening
+
+        if not task.task_idd == task_sent.task_idd:
+            critical("Received finished event for a task that was not the task we found in the doing list")
+            return
+    
+        # This is a valid task, proceed
+
+        experiment = self.experiments[task.experiment_idd]
         task.tries += 1
+        del self.doing[i]
+
+        # Print stdout if the task has failed
+
+        if not task.success and task.attempts:
+            result = task.attempts[-1]
+            warn(f"--- TASK {task.task_idd} FAILED WITH EXIT CODE {result['status']} {task.tries}/{task.max_tries} ---")
+            os.write(sys.stdout.fileno(), result['stdout'])
+            warn("--- END OF FAILED OUTPUT ---")
 
-        if msg_in.success:
+        # If the task finished successfully, notify its experiment and move it to done
+
+        if task.success:
             self.done.append(task)
-            return
+            experiment.on_task_completed(self, task)
 
-        if task.tries >= task.max_tries:
-            critical(f"Giving up on task {task.task_idd}, max_tries reached.")
+            # if not self.quiet:
+            #     print(f"Moving task {task.task_idd} to done")
+
+        # If max_tries has been reached, notify the experiment and move it to given_up
+
+        elif task.tries >= task.max_tries:
             self.given_up.append(task)
-            return
+            experiment.on_task_completed(self, task)
+            critical(f"Giving up on task {task.task_idd}, max_tries reached.")
         
-        if not self.idle:
-            self.todo.append(task)
-            return
+        # If a worker is available, ask it to execute the task again
+
+        elif self.idle:
+            worker_idd = self.idle.pop()
+
+            task.assigned_to = worker_idd
+            self.doing.append(task)
+
+            msg_out = WorkerMessage("execute")
+            msg_out.task = task
 
-        target = self.idle.pop()
+            self.workers[worker_idd].queue.put(msg_out)
 
-        msg_out = WorkerMessage("execute")
-        msg_out.task = task
-        msg_out.task.assigned_to = target
+            # if not self.quiet:
+            #     print(f"Reassigning task {task.task_idd} to new worker {worker_idd} after fail")
+
+        # Otherwise, move the task back to todo, we will schedule it again in the future
+
+        else:
+            self.todo.append(task)
 
-        self.workers[target].queue.put(msg_out)
+            # if not self.quiet:
+            #     print(f"No worker available to retry task {task.task_idd}, moving it back to todo")
```

### Comparing `patas-2.0.5/patas/main.py` & `patas-2.0.6/patas/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,92 +1,135 @@
 #!/usr/bin/env python3
 
 try:
     from . import consts as c
 except:
     from patas import consts as c
 
-from patas.utils import error, node_cpu_count, abort
+from patas.utils import error, node_cpu_count, abort, warn
+from collections import defaultdict
 from patas import argparsers
+from patas import schemas
 
 import sys
 
-BASIC_OPTIONS   = ['explore', 'parse', 'query', 'draw', 'doctor']
-DRAW_OPTIONS    = ['heatmap', 'lines', 'lines_3d', 'bars', 'bars_3d', 'boxplot', 'violin', 'scatter', 'scatter_3d', 'surface', 'pie']
-EXPLORE_OPTIONS = ['grid', 'cdeepso']
 
+BASIC_OPTIONS   = ['explore', 'parse', 'query', 'draw', 'doctor']
+DRAW_OPTIONS    = ['heatmap', 'categories', 'lines', 'bars']
 
-def create_experiments(args):
 
-    from patas.schemas import Experiment, ListVariable, ArithmeticVariable, GeometricVariable, load_experiment
-
-    experiments = []
-    
-    # If experiment parameters are provided, create an experiment for them
-
-    experiment = Experiment()
+def parse_base_experiment(args, experiment:schemas.BaseExperimentSchema):
 
     if args.name:
         experiment.name = args.name
 
     if args.repeat:
         experiment.repeat = args.repeat
     
     if args.workdir:
         experiment.workdir = args.workdir
     else:
         from os import environ
-        experiment.workdir = environ['PWD']
+        pwd  = environ.get('PWD', None)
+        home = environ.get('HOME', None)
+
+        if home and pwd.startswith(home):
+            experiment.workdir = '$HOME' + pwd[len(home):]
+        else:
+            experiment.workdir = pwd
     
     if args.cmd:
         experiment.cmd = args.cmd
 
     if args.max_tries:
         experiment.max_tries = args.max_tries
 
+    if args.redo_tasks:
+        experiment.redo_tasks = args.redo_tasks
+
+def append_grid_experiment(args, experiments):
+
+    experiment = schemas.GridExperimentSchema()
+
+    parse_base_experiment(args, experiment)
+    
     for values in args.var_list:
-        var = ListVariable()
-        var.name = values[0]
+        var        = schemas.ListVariableSchema()
+        var.name   = values[0]
         var.values = values[1:]
         experiment.vars.append(var)
 
     for name, min, max, step in args.var_arithmetic:
-        var      = ArithmeticVariable()
+        var      = schemas.ArithmeticVariableSchema()
         var.name = name
         var.min  = float(min)  if '.' in min  else int(min)
         var.max  = float(max)  if '.' in max  else int(max)
         var.step = float(step) if '.' in step else int(step)
         var.update()
         experiment.vars.append(var)
 
     for name, min, max, step in args.var_geometric:
-        var        = GeometricVariable()
+        var        = schemas.GeometricVariableSchema()
         var.name   = name
         var.min    = float(min)  if '.' in min  else int(min)
         var.max    = float(max)  if '.' in max  else int(max)
         var.factor = float(step) if '.' in step else int(step)
         var.update()
         experiment.vars.append(var)
 
-    if experiment.cmd or experiment.vars:
+    if args.score_pattern:
+        warn("GridExperiment is not compatible with parameter --score-pattern")
+
+    if experiment.cmd and experiment.vars:
+        experiments.append(experiment)
+    
+    return experiments
+
+
+def append_cdeepso_experiment(args, experiments:list):
+    
+    experiment = schemas.CDEEPSOExperimentSchema()
+
+    parse_base_experiment(args, experiment)
+    
+    if args.score_pattern:
+        experiment.score_pattern = args.score_pattern
+    
+    if args.var_list:
+        warn("CDEEPSOExperiment is not compatible with parameter --vl")
+
+    if args.var_arithmetic:
+        warn("CDEEPSOExperiment is not compatible with parameter --va")
+
+    if args.var_geometric:
+        warn("CDEEPSOExperiment is not compatible with parameter --vg")
+
+    if experiment.cmd and experiment.vars:
         experiments.append(experiment)
+    
+    return experiments
+
+
+def load_experiments_from_files(args):
 
+    experiments = []
+    
     # If experiment files are provided, load all of them
 
     if args.experiment:
         for filepath in args.experiment:
-            experiment = load_experiment(filepath)
+            experiment = schemas.load_experiment(filepath)
             experiments.append(experiment)
     
     return experiments
 
 
 def create_clusters(args):
 
-    from patas.schemas import Cluster, Node, load_cluster
+    from patas.schemas import ClusterSchema, NodeSchema, load_cluster
 
     clusters = []
 
     # If cluster files are provided, we will use them
 
     if args.cluster:
         for filepath in args.cluster:
@@ -94,21 +137,21 @@
             cluster = load_cluster(filepath)
             clusters.append(cluster)
     
     # If nodes are provided, we will add them to the QuickCluster
 
     if args.node:
         
-        cluster = Cluster()
+        cluster = ClusterSchema()
         cluster.name = 'cluster'
         clusters.append(cluster)
 
         for i, node_params in enumerate(args.node):
 
-            node = Node()
+            node = NodeSchema()
             node.name = f'node{i}'
 
             address      = node_params[0]
             node.workers = int(node_params[1]) if len(node_params) > 1 else None
             node.tags    = node_params[2:] if len(node_params) > 2 else []
 
             if ':' in address:
@@ -128,52 +171,60 @@
 
     # If no cluster or node is provided, we will create a simple one based on the local machine
 
     if not clusters:
 
         from multiprocessing import cpu_count
 
-        node          = Node()
+        node          = NodeSchema()
         node.name     = 'localhost'
         node.hostname = 'localhost'
         node.workers  = cpu_count()
 
-        cluster       = Cluster()
+        cluster       = ClusterSchema()
         cluster.name  = 'cluster'
 
         cluster.nodes.append(node)
         clusters.append(cluster)
     
     return clusters
 
 
 def create_task_filters(args):
 
-    task_filters = []
+    task_filters = defaultdict(list)
 
     for filters in args.task_filters:
-        for task in filters:
+        for slice in filters:
             try:
 
-                cells = task.split(':')
+                cells = slice.split(':')
 
-                if len(cells) == 2:
+                if len(cells) == 3:
+                    xp =     cells[0]  if cells[0] else args.type
+                    i1 = int(cells[1]) if cells[1] else 0
+                    i2 = int(cells[2]) if cells[2] else float('inf')
+                
+                elif len(cells) == 2:
+                    xp = args.type
                     i1 = int(cells[0]) if cells[0] else 0
                     i2 = int(cells[1]) if cells[1] else float('inf')
-                    task_filters.append((i1, i2))
 
                 elif len(cells) == 1:
+                    xp = args.type
                     i1 = int(cells[0]) if cells[0] else 0
-                    task_filters.append((i1, i1+1))
+                    i2 = i1+1
 
                 else:
-                    error(f'Invalid attribute for --task-filter: {task}')
+                    error(f'Invalid attribute for --task-filter: {slice}')
+                
+                task_filters[xp].append((i1, i2))
 
             except ValueError:
-                error(f'Invalid attribute for --task-filter: {task}')
+                error(f'Invalid attribute for --task-filter: {slice}')
 
     return task_filters
 
 
 def create_node_filters(args):
 
     return [ x for filters in args.node_filters for x in filters ]
@@ -189,30 +240,42 @@
 def create_linebreakers(args):
 
     from patas.parse import Pattern
 
     return [Pattern(None, pattern) for pattern in args.linebreakers]
 
 
-def do_explore_grid(argv):
+def do_explore(argv):
 
-    from patas.grid_explorer import GridExplorer
+    from patas.scheduler import Scheduler
 
-    args         = argparsers.parse_patas_explore_grid(argv)
-    experiments  = create_experiments(args)
+    args         = argparsers.parse_patas_explore(argv)
     clusters     = create_clusters(args)
     task_filters = create_task_filters(args)
     node_filters = create_node_filters(args)
-    gridexec     = GridExplorer(task_filters, node_filters, args.output_folder, args.redo_tasks, args.recreate, args.confirmed, experiments, clusters)
+    experiments  = load_experiments_from_files(args)
 
-    gridexec.start()
+    if args.type == 'grid':
+        append_grid_experiment(args, experiments)
+
+    elif args.type == 'cdeepso':
+        append_cdeepso_experiment(args, experiments)
+
+    for x in experiments:
+        x.task_filters = task_filters.pop(x.name, [])
+    
+    for idd, x in enumerate(experiments):
+        x.experiment_idd = idd
 
+    if task_filters:
+        names = ', '.join([x for x in task_filters])
+        warn(f"Ignoring task-filters for the following experiments: {names}")
 
-def do_explore_cdeepso(argv):
-    abort("CDEEPSO is not implemented yet.")
+    scheduler = Scheduler(node_filters, args.output_folder, args.redo_tasks, args.confirmed, experiments, clusters, args.quiet)
+    scheduler.start()
 
 
 def do_parse(argv):
 
     from patas.parse import ExperimentParser
 
     args         = argparsers.parse_patas_parse(argv)
@@ -221,72 +284,63 @@
     parser       = ExperimentParser(patterns, linebreakers, True)
 
     parser.start(args.experiment_folder, args.output_file)
 
 
 def do_query(argv):
 
-    from patas.query_engine import QueryEngine
+    from patas.query import QueryEngine
     
     args   = argparsers.parse_patas_query(argv)
     engine = QueryEngine(args.patas_folder)
     engine.query(args.query, args.pretty_print)
 
 
 def do_draw_heatmap(argv):
 
     from patas import graphics
 
     args = argparsers.parse_patas_draw_heatmap(argv)
 
     graphics.render_heatmap(args.x_column, args.y_column, args.z_column,
-                            args.title, args.x_label, args.y_label, args.r_label,
-                            args.x_change, args.y_change, args.z_change, args.r_format, 
+                            args.title, args.x_label, args.y_label, args.z_label,
+                            args.x_change, args.y_change, args.z_change, args.annot, args.fmt, 
                             args.input_file, args.output_file, 
-                            args.size, args.r_function, args.colormap, 
-                            args.verbose)
+                            args.fig_size, args.aggfunc)
 
 
+def do_draw_categories(argv):
+    
+    from patas import graphics
+
+    args = argparsers.parse_patas_draw_categories(argv)
+
+    graphics.render_categories(args.x_column, args.y_column, args.hue_column, 
+                         args.title, args.x_label, args.y_label, args.legend_label, 
+                         args.x_change, args.y_change, args.hue_change, 
+                         args.input_file, args.output_file, 
+                         args.fig_size, args.errorbar)
+
 def do_draw_lines(argv):
     
     from patas import graphics
 
     args = argparsers.parse_patas_draw_lines(argv)
 
-    lines = [
-        (line.x_column, line.y_column, line.x_change, line.y_change, line.r_function, line.label, line.style, line.marker, line.marker_size) 
-        for line in args.lines
-    ]
-
-    graphics.render_lines(lines, args.title, args.size, 
-                          args.x_label, args.r_label, 
+    graphics.render_lines(args.title, args.x_label, args.y_label, args.legend_label, 
+                          args.x_column, args.y_column, args.hue_column, args.style_column,
+                          args.x_change, args.y_change, args.hue_change,  args.style_change,
                           args.input_file, args.output_file, 
-                          args.show_grid, args.border, args.show_error, 
-                          args.ticks, args.ticks_format, args.legend_location,
-                          args.verbose)
+                          args.fig_size, args.err_style, args.errorbar)
+    
 
 def do_draw_lines_3d(argv):
     abort("Draw lines_3d is not implemented yet.")
 
 
-def do_draw_bars(argv):
-    
-    from patas import graphics
-
-    args = argparsers.parse_patas_draw_bars(argv)
-
-    graphics.render_bars(args.x_column, args.y_column, 
-                         args.title, args.x_label, args.r_label, 
-                         args.x_change, args.y_change, args.r_format, 
-                         args.input_file, args.output_file, 
-                         args.size, args.r_function, args.bar_color, args.bar_size, args.horizontal, args.show_grid, 
-                         args.ticks, args.ticks_format, args.border, args.show_error,
-                         args.verbose)
-
-
 def do_draw_bars_3d(args):
     abort("Draw bars_3d is not implemented yet.")
 
 
 def do_draw_boxplot(args):
     abort("Draw boxplot is not implemented yet.")
 
@@ -316,37 +370,26 @@
 
 
 def help_main_syntax():
     print(f"Patas {c.version}")
     print(f"Syntax: patas [{','.join(BASIC_OPTIONS)}] ...")
 
 
-def help_explore_syntax():
-    print(f"Syntax: patas explore [{','.join(EXPLORE_OPTIONS)}] ...")
-
-
 def help_draw_syntax():
     print(f"Syntax: patas draw [{','.join(DRAW_OPTIONS)}] ...")
 
 
 def main(*params):
 
     # parser.add_subparsers()
 
     args = sys.argv[1:]
 
     if len(args) == 0 or not args[0] in BASIC_OPTIONS:
         help_main_syntax()
-    
-    if args[0] == 'explore':
-
-        if len(args) == 1 or not args[1] in EXPLORE_OPTIONS:
-            help_explore_syntax()
-        
-        globals()['do_explore_' + args[1]](args[2:])
         
     elif args[0] == 'draw':
 
         if len(args) == 1 or not args[1] in DRAW_OPTIONS:
             help_draw_syntax()
         
         globals()['do_draw_' + args[1]](args[2:])
```

### Comparing `patas-2.0.5/patas/parse.py` & `patas-2.0.6/patas/parse.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,16 +74,17 @@
         for pattern in patterns:
             self._add_column(pattern.name)
 
         # Add columns with extra info
         
         if verbose:
             for var_name in ["break_id", "task_id", "repeat_id", "combination_id", "experiment_id", "experiment_name", 
-                            "duration", "started_at", "ended_at", "tries", "max_tries", 
-                            "cluster_id", "cluster_name", "node_id", "node_name", "worker_id", "output_dir", "work_dir"]:
+                            "tries", "max_tries", "duration", "started_at", "ended_at", 
+                            "cluster_name", "node_name", "cluster_in_lab", "node_in_lab", "node_in_cluster",
+                            "worker_in_lab", "worker_in_cluster", "worker_in_node", "output_dir", "work_dir"]:
 
                 self._add_column(var_name)
 
         self.row_values = [None for _ in range(len(self.header_map))]
 
 
     def _add_column(self, name):
@@ -96,26 +97,27 @@
 
 
     def digest(self, task_folderpath, writer):
 
         # Filepaths for each task files
 
         info_filepath   = os.path.join(task_folderpath, "info.yml")
-        output_filepath = os.path.join(task_folderpath, "stdout")
-        done_filepath   = os.path.join(task_folderpath, ".done")
+        output_filepath = os.path.join(task_folderpath, "success.stdout")
+        done_filepath   = os.path.join(task_folderpath, ".success")
 
         # We clean the output row, as we will populate it with the data from the task
 
         for i in range(len(self.row_values)):
             self.row_values[i] = None
 
-        # If the done file does not exist, it means the task wasnot completed, this is likely a user mistake
+        # If the done file does not exist, it means the task was not completed, this is likely a user mistake
 
         if not os.path.exists(done_filepath):
             warn("Task not completed:", task_folderpath)
+            return
         
         # Load the task info
 
         with open(info_filepath, "r") as fin:
             data = yaml.load(fin, Loader=yaml.FullLoader)
         
         # Load the variable values
@@ -132,27 +134,37 @@
 
             self.row_values[self.header_map["break_id"        ]] = str(break_idd)
             self.row_values[self.header_map["task_id"         ]] = data["task_id"         ]
             self.row_values[self.header_map["repeat_id"       ]] = data["repeat_id"       ]
             self.row_values[self.header_map["combination_id"  ]] = data["combination_id"  ]
             self.row_values[self.header_map["experiment_id"   ]] = data["experiment_id"   ]
             self.row_values[self.header_map["experiment_name" ]] = data["experiment_name" ]
-            self.row_values[self.header_map["duration"        ]] = data["duration"        ]
-            self.row_values[self.header_map["started_at"      ]] = data["started_at"      ]
-            self.row_values[self.header_map["ended_at"        ]] = data["ended_at"        ]
-            self.row_values[self.header_map["tries"           ]] = data["tries"           ]
             self.row_values[self.header_map["max_tries"       ]] = data["max_tries"       ]
             self.row_values[self.header_map["output_dir"      ]] = data["output_dir"      ]
             self.row_values[self.header_map["work_dir"        ]] = data["work_dir"        ]
+            
+            if data['results']:
+
+                result = data['results'][-1]
+
+                self.row_values[self.header_map["tries"]] = len(data["results"])
+
+                self.row_values[self.header_map["duration"  ]] = result["duration"  ]
+                self.row_values[self.header_map["started_at"]] = result["started_at"]
+                self.row_values[self.header_map["ended_at"  ]] = result["ended_at"  ]
+
+                self.row_values[self.header_map["cluster_name"     ]] = result["env_variables"]["PATAS_CLUSTER_NAME"     ]
+                self.row_values[self.header_map["node_name"        ]] = result["env_variables"]["PATAS_NODE_NAME"        ]
+                self.row_values[self.header_map["cluster_in_lab"   ]] = result["env_variables"]["PATAS_CLUSTER_IN_LAB"   ]
+                self.row_values[self.header_map["node_in_lab"      ]] = result["env_variables"]["PATAS_NODE_IN_LAB"      ]
+                self.row_values[self.header_map["node_in_cluster"  ]] = result["env_variables"]["PATAS_NODE_IN_CLUSTER"  ]
+                self.row_values[self.header_map["worker_in_lab"    ]] = result["env_variables"]["PATAS_WORKER_IN_LAB"    ]
+                self.row_values[self.header_map["worker_in_cluster"]] = result["env_variables"]["PATAS_WORKER_IN_CLUSTER"]
+                self.row_values[self.header_map["worker_in_node"   ]] = result["env_variables"]["PATAS_WORKER_IN_NODE"   ]
 
-            self.row_values[self.header_map["cluster_id"  ]] = data["env_variables"]["PATAS_CLUSTER_ID"  ]
-            self.row_values[self.header_map["cluster_name"]] = data["env_variables"]["PATAS_CLUSTER_NAME"]
-            self.row_values[self.header_map["node_id"     ]] = data["env_variables"]["PATAS_NODE_ID"     ]
-            self.row_values[self.header_map["node_name"   ]] = data["env_variables"]["PATAS_NODE_NAME"   ]
-            self.row_values[self.header_map["worker_id"   ]] = data["env_variables"]["PATAS_WORKER_ID"   ]
 
         # Parse the patterns and write to output
 
         pattern:Pattern = None
 
         with open(output_filepath, "r") as fin:
             for line in fin:
```

### Comparing `patas-2.0.5/patas/utils.py` & `patas-2.0.6/patas/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from subprocess import Popen, PIPE
 
+import pathlib
 import shutil
 import shlex
-import glob
 import sys
 import re
 import os
 
 
 
 class colors:
@@ -301,20 +301,21 @@
 
 
 class PatasError(Exception):
     def __init__(self, message=None):
         self.message = message
 
 
-def clean_folder(folderpath):
+def clean_folder(folderpath, quiet=False):
     
     if os.path.exists(folderpath):
         if os.path.isdir(folderpath):
-            for filepath in glob.glob(os.path.join(folderpath, '*')):
-                debug("  Removing:", filepath)
+            for filepath in pathlib.Path(folderpath).glob('*'):
+                if not quiet:
+                    debug("  Removing:", filepath)
                 if os.path.isdir(filepath):
                     shutil.rmtree(filepath)
                 else:
                     os.remove(filepath)
         else:
             os.remove(folderpath)
     else:
@@ -322,42 +323,42 @@
 
 
 def human_time(seconds):
 
     v = seconds
 
     if v < 60:
-        return f"{v} seconds"
+        return f"{v:.2f} seconds"
     v /= 60
 
     if v < 60:
-        return f"{v} minutes"
+        return f"{v:.2f} minutes"
     v /= 60
 
     if v < 24:
-        return f"{v} hours"
+        return f"{v:.2f} hours"
     v /= 24
 
     if v < 7:
-        return f"{v} days"
+        return f"{v:.2f} days"
     v /= 7
 
     if v < 52:
-        return f"{v} weeks ~ {v / 4.0} months"
+        return f"{v:.2f} weeks ~ {v/4.0:.2f} months"
     v /= 52
 
     if v < 100:
-        return f"{v} years"
+        return f"{v:.2f} years"
     v /= 100
 
     if v < 10:
-        return f"{v} centuries"
+        return f"{v:.2f} centuries"
     v /= 10
 
-    return f"{v} milleniums"
+    return f"{v:.2f} milleniums"
 
 
 def estimate(tasks, workers, seconds):
     
     return human_time(tasks / workers * seconds)
 
 
@@ -386,8 +387,21 @@
     if status != 0:
         return default
 
     try:
         return int(output[0])
     except ValueError:
         return default
-                
+                
+def confirm():
+
+    try:
+        while True:
+            option = input('Do you want to continue? [Y/n] ').strip()
+            if option in ['Y', 'y', '']:
+                break
+            elif option in ['N', 'n']:
+                sys.exit(0)
+            else:
+                print('Invalid option')
+    except KeyboardInterrupt:
+        sys.exit(0)
```

### Comparing `patas-2.0.5/patas.egg-info/PKG-INFO` & `patas-2.0.6/patas.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patas
-Version: 2.0.5
+Version: 2.0.6
 Summary: Hyperparameter search with a single command
 Home-page: https://github.com/diegofps/patas
 Author: Diego Souza
 Author-email: diegofpsouza+patas@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 
 ```shell
 pip install patas
 ```
 
 # Basic usage 🐣
 
-Considering the use case that we need to find the optimal configuration for a neural network. In this case we are interested in variating the number of hidden neurons and the activation function in the hidden layer. We want to execute our prgoram multiple times, combining the values of these two parameters, and collect metrics of interest, like train and test accuracies. We then want to analyse this output and select the best configuration. The following subsections will describe how to achieve this.
+Considering the use case that we need to find the optimal configuration for a neural network. In this case we are interested in variating the number of hidden neurons, the activation function, and the complexity of preprocessing we do. We want to execute our prgoram multiple times, combining the values of these two parameters, and collect metrics of interest, like train and test accuracies. We then want to analyse this output and select the best configuration. The following subsections will describe how to achieve this.
 
 ## The program
 
 We will use a mockup code present in `examples/basic_usage`. This is a script that pretends to run a neural network, receiving the two variables of interest and printing the desired metrics to stdout. This could easily be replaced by a real program training a neural network, but we use a mockup to speed up the process. To access this program you just need to access the folder.
 
 ```shell
 # Enter the program folder
@@ -33,54 +33,65 @@
 
 # Example of program execution
 ./main.py 100 relu
 ```
 
 ## patas explore
 
-Assuming we want to vary the number of hidden neurons from `1` to `51` with steps of `2` and the activation function in `['relu' 'leaky_relu' 'sigmoid' 'tanh']`, we can generate all combinationsand parallelize the script above using `patas explore grid`. This will also collect its entire stdout and save them in the folder `patasout/grid`. Each combination will be executed `10` times, as we want to measure the average accuracies later.
+Assuming we want to vary the number of hidden neurons from `1` to `51` with steps of `2` and the activation function in `['relu' 'leaky_relu' 'sigmoid' 'tanh']`, we can generate all combinationsand parallelize the script above using `patas explore grid`. This will also collect its entire stdout and save them in the folder `pataslab/grid`. Each combination will be executed `10` times, as we want to measure the average accuracies later.
 
 ```shell
-patas explore grid \
-    --cmd './main.py {neurons} {activation}' \
+patas explore --type grid \
+    --cmd './main.py {neurons} {activation} {preprocessing}' \
     --va neurons 1 51 2 \
+    --vl preprocessing fast medium intense \
     --vl activation relu leaky_relu sigmoid tanh \
+    --node localhost \
     --repeat 10
 ```
 
-The parameter `--cmd` define the command that must be executed. If we define more than one `--cmd` they will all be executed, one after the other. The parameter `--vl` defines a variable of type list, it receives the variable name and the list of values it can receive. Next, the parameter `--repeat` defines the number of times the program will be called using a given variable combination. In this example, the parameter neurons define `26` values and the paramter activation define `4` values. This will generate `104 combinations`. Considering the repeat parameter has the value `10`, the program will be excuted `1040` times. That is, patas will have `1040 tasks` to do. You can define as many variable as you want, but the more you have the longer it will take to execute, growing exponentially.
+Here is a short description of the parameters above:
+
+`--cmd` - defines the command that must be executed. If we define more than one `--cmd` they will all be executed, one after the other. 
+`--va` - defines a variable of type arithmetic, it receives the variable name, an initial value, a maximum value and a step value. It will generate a list similar to the Python's method `range`. 
+`--vl` - defines a variable of type list, it receives the variable name and the list of values it can receive. 
+`--node` - defines a node to execute the program. This may be any machine accessible via SSH that won't ask for a password. This command accepts an optional argument to indicate the number of workers in the machine. If non is provided, it will default to the number of cores in the machine. You may want to check the program `ssh-copy-id` to learn how to install a public key on a remote machine and log in without a password. 
+`--repeat` defines the number of times the program will be called using a given variable combination. In this example, the parameter neurons define `25` values, parameter preprocessing defines `3` values and the paramter activation define `4` values. This will generate `300 combinations`. Considering the repeat parameter has the value `10`, the program will be excuted `3000` timesm. That is, we asked patas to do `3000 tasks`. You can define as many variables as you want, but the more you have the longer it will take to execute.
 
 ## patas parse
 
 When the experiment is done executing, we can parse its outputs and collect the desired values using `patas parse`.
 
 ```shell
 patas parse \
-    -e 'patasout/grid/' \
-    -p train_acc  'Train accuracy:     (@float@)' \
-    -p test_acc   'Test accuracy:      (@float@)'
+    -e 'pataslab/grid/' \
+    -p train_time  'Time to train \(ms\): (@float@)' \
+    -p test_time   'Time to test \(ms\):  (@float@)' \
+    -p train_acc   'Train accuracy:     (@float@)' \
+    -p test_acc    'Test accuracy:      (@float@)' \
+    -p loss        'Final Loss:         (@float@)'
 ```
 
-The parameter `-e` define the experiment folder, containing the prgoram outputs and a few extra info. The parameter `-p` define a pattern patas is going to look for. It receives a name and a regular expression string. The output file will be saved in `patasout/grid/grid.csv`. This contains a table with the input variables, collected results, and extra variables associated to the experiment. 
+The parameter `-e` define the experiment folder, containing the prgoram outputs and a few extra info. The parameter `-p` define a pattern patas is going to look for. It receives a name and a regular expression string. The output file will be saved in `pataslab/grid/grid.csv`. This contains a table with the input variables, collected results, and extra variables associated to the experiment. 
 
 ## patas query
 
 We use `patas query` to inspect the contents of the csv file generated above. This command works with any csv file and recognizes the experiment names as table names.
 
 ```shell
 patas query 'select * from grid limit 2' -m
 ```
 
 The parameter `-m` asks patas to print the output in markdown format.
 The output for the command above should have a similar structure to the content bellow. The values may vary as the script is non-determininstic.
 
-| in_activation | in_neurons | out_train_acc | out_test_acc | break_id | task_id | repeat_id | combination_id | experiment_id | experiment_name | duration |          started_at |            ended_at | tries | max_tries | cluster_id | cluster_name | node_id | node_name | worker_id | output_dir                                                       | work_dir                                       |
-| ------------- | ---------- | ------------- | ------------ | -------- | ------- | --------- | -------------- | ------------- | --------------- | -------- | ------------------- | ------------------- | ----- | --------- | ---------- | ------------ | ------- | --------- | --------- | ---------------------------------------------------------------- | ---------------------------------------------- |
-| leaky_relu    |         25 |         0,487 |        0,452 |    False |     386 |         6 |             38 |         False | grid            |   0,048… | 2023-05-11 14:13:34 | 2023-05-11 14:13:34 |  True |         3 |      False | cluster      |   False | localhost |         7 | /home/ubuntu/Sources/patas/examples/basic_usage/patasout/grid/386 | /home/ubuntu/Sources/patas/examples/basic_usage |
-| sigmoid       |         27 |         0,841 |        0,820 |    False |     652 |         2 |             65 |         False | grid            |   0,055… | 2023-05-11 14:13:34 | 2023-05-11 14:13:34 |  True |         3 |      False | cluster      |   False | localhost |        57 | /home/ubuntu/Sources/patas/examples/basic_usage/patasout/grid/652 | /home/ubuntu/Sources/patas/examples/basic_usage |
+| in_activation | in_neurons | in_preprocessing | out_train_time | out_test_time | out_train_acc | out_test_acc | out_loss | break_id | task_id | repeat_id | combination_id | experiment_id | experiment_name | tries | max_tries | duration | started_at                 | ended_at                   | cluster_name | node_name | cluster_in_lab | node_in_lab | node_in_cluster | worker_in_lab | worker_in_cluster | worker_in_node | output_dir                                                        | work_dir                                 |
+| ------------- | ---------- | ---------------- | -------------- | ------------- | ------------- | ------------ | -------- | -------- | ------- | --------- | -------------- | ------------- | --------------- | ----- | --------- | -------- | -------------------------- | -------------------------- | ------------ | --------- | -------------- | ----------- | --------------- | ------------- | ----------------- | -------------- | ----------------------------------------------------------------- | ---------------------------------------- |
+| relu          | 33         | medium           | 175.812        | 4.880         | 0.423         | 0.411        | 0.338    | 0        | 1160    | 0         | 116            | 0             | grid            | 1     | 3         | 0.224591 | 2023-05-17 19:14:55.472312 | 2023-05-17 19:14:55.696903 | cluster      | node0     | 0              | 0           | 0               | 14            | 14                | 14             | /home/diego/Sources/patas/examples/basic_usage/pataslab/grid/1160 | $HOME/Sources/patas/examples/basic_usage |
+| leaky_relu    | 27         | fast             | 190.677        | 6.904         | 0.286         | 0.270        | 0.288    | 0        | 386     | 6         | 38             | 0             | grid            | 1     | 3         | 0.225969 | 2023-05-17 19:14:58.327345 | 2023-05-17 19:14:58.553314 | cluster      | node0     | 0              | 0           | 0               | 47            | 47                | 47             | /home/diego/Sources/patas/examples/basic_usage/pataslab/grid/386  | $HOME/Sources/patas/examples/basic_usage |
 
 We must remember that for every combination, patas will execute the program `--repeat` times, passing the same input parameters and collecting multiple output variables. This is useful when the algorithm we are evaluating is non-deterministic and we wish to collect reliable metrics, like our script. To aggregate these values we can calculate the average value using the `AVG` function with the `GROUP BY` statement.
 
 ```shell
 patas query '
     SELECT in_activation, 
            in_neurons, 
@@ -110,135 +121,115 @@
 
 | in_activation | in_neurons | train_acc | test_acc |
 | ------------- | ---------- | --------- | -------- |
 | relu          |          5 |    0,995… |   0,946… |
 
 ## patas draw
 
-Patas will also help you quickly create basic graphics based on the data in the csv file. This might help you inspect the data and get some quick insights. As of now, patas supports three graphic types, `heatmap`, `bars`, and `lines`.
+Patas can also help you quickly create basic graphics based on the data in the csv file. It provides a wrapper for a few seaborn functions to quickly generate graphics, without needing to create a python script for this. If you need complex charts, though, we recommend you use the advanced graphics library of your preference. As of now, patas provides three drawing functions: `heatmap`, `categorical`, and `lines`.
 
 ### Heatmap
 
 ```shell
 patas draw heatmap \
-    --input patasout/grid/grid.csv \
+    --input pataslab/grid/grid.csv \
     --x-column in_neurons \
     --y-column in_activation \
     --z-column out_test_acc \
-    --size 10 2
+    --fig-size 15 3
 ```
 
 ![Basic heatmap example](https://github.com/diegofps/patas/blob/main/docs/images/heatmap1.png?raw=true)
 
 ```shell
 patas draw heatmap \
-    --input 'patasout/grid/grid.csv' \
-    --title 'Grid Search Results' \
+    --input pataslab/grid/grid.csv \
+    --output heatmap.png \
+    --title 'Average test accuracy' \
     --x-column in_neurons \
-    --x-change 'int(X[i])*2' \
-    --x-label Neurons \
+    --x-label 'Number of Neurons' \
+    --x-change 'X[i]' \
     --y-column in_activation \
+    --y-label 'Activation function' \
     --y-change 'Y[i][:3]' \
-    --y-label 'Activation Function' \
     --z-column out_test_acc \
-    --z-change 'Z[i]*100' \
-    --r-function min \
-    --r-format 'int(R[y,x])' \
-    --r-label Accuracy \
-    --size 10 2 \
-    --colormap AAAAAA 000011
+    --z-label 'Accuracy' \
+    --z-change 'int(Z[i]*100)' \
+    --fig-size 15 3 \
+    --annot \
+    --aggfunc mean \
+    --fmt '.0f'
 ```
 
 ![Extended heatmap example](https://github.com/diegofps/patas/blob/main/docs/images/heatmap2.png?raw=true)
 
-### Bars
-
-```shell
-patas query 'select * from grid where in_activation="relu"' > test.csv
-```
+### Categorical
 
 ```shell
-patas draw bars \
-    --input test.csv \
-    --x-column in_neurons \
+patas draw categories \
+    --input pataslab/grid/grid.csv \
+    --x-column in_activation \
     --y-column out_test_acc \
-    --size 10 2
+    --fig-size 10 7 \
+    --x-label 'Activation function' \
+    --y-label 'Test Accuracy' \
+    --title 'Test performance by activation function'
 ```
 
-![Bars example](https://github.com/diegofps/patas/blob/main/docs/images/bars1.png?raw=true)
+![Categorical example](https://github.com/diegofps/patas/blob/main/docs/images/categorical1.png?raw=true)
 
 ```shell
-patas draw bars \
-    --input test.csv \
-    --title 'Performance using the function relu' \
-    --x-column in_neurons \
-    --x-change 'int(float(X[i]))' \
-    --x-label 'Neurons' \
+patas draw categories \
+    --input pataslab/grid/grid.csv \
+    --x-column in_activation \
+    --hue-column in_preprocessing \
     --y-column out_test_acc \
-    --y-change 'round(Y[i]*100)/100' \
-    --r-function mean \
-    --r-format 'R[i]:.2f' \
-    --r-label 'Accuracy' \
-    --size 10 2 \
-    --bar-size 0.8 \
-    --bar-color B00020 \
-    --show-grid \
-    --show-error \
-    --ticks 5 \
-    --ticks-format 'T[i]:.2f' \
-    --border none
+    --fig-size 10 4 \
+    --x-label 'Activation function' \
+    --y-label 'Test Accuracy' \
+    --legend-label 'Preprocessing' \
+    --errorbar 'sd' \
+    --title 'Test performance by activation function and preprocessing'
 ```
 
-![Bars example](https://github.com/diegofps/patas/blob/main/docs/images/bars2.png?raw=true)
+![Categorical example](https://github.com/diegofps/patas/blob/main/docs/images/categorical2.png?raw=true)
 
 ### Lines
 
 ```shell
 patas draw lines \
-    --input patasout/grid/grid.csv \
-    --size 10 2 \
-    --new-line \
-    --x-column in_neurons \
-    --y-column out_test_acc \
-    \
-    --new-line \
-    --x-column in_neurons \
-    --y-column out_train_acc
+    --input 'pataslab/grid/grid.csv' \
+    --fig-size 10 4 \
+    --x-column 'in_neurons' \
+    --x-label 'Neurons' \
+    --y-column 'out_test_acc' \
+    --y-label 'Accuracy' \
+    --title 'Average test accuracy' \
+    --err-style 'bars' \
+    --errorbar 'sd'
 ```
 
 ![Lines example](https://github.com/diegofps/patas/blob/main/docs/images/lines1.png?raw=true)
 
 ```shell
 patas draw lines \
-    --input patasout/grid/grid.csv \
-    --title "Testing Title" \
-    --x-label "x axis" \
-    --r-label "y axis" \
-    --size 10 2 \
-    --show-grid \
-    --border none \
-    --ticks 5 \
-    --ticks-format 'T[i]:.2f' \
-    \
-    --new-line \
-    --label 'Test accuracy' \
-    --x-column in_neurons \
-    --y-column out_test_acc \
-    --style dash \
-    --marker diamond \
-    \
-    --new-line \
-    --label 'Train accuracy' \
-    --x-column in_neurons \
-    --y-column out_train_acc \
-    --style dot \
-    --marker circle
+    --input 'pataslab/grid/grid.csv' \
+    --fig-size 10 4 \
+    --x-column 'in_neurons' \
+    --x-label 'Neurons' \
+    --y-column 'out_test_acc' \
+    --y-label 'Accuracy' \
+    --hue-column 'in_activation' \
+    --title 'Average test accuracy' \
+    --legend-label 'Act. Function' \
+    --err-style 'band' \
+    --errorbar 'sd'
 ```
 
-![Extended lines example](https://github.com/diegofps/patas/blob/main/docs/images/lines2.png?raw=true)
+![Lines example](https://github.com/diegofps/patas/blob/main/docs/images/lines2.png?raw=true)
 
 # Documentation 📚
 
 ## When should I use Patas? ⭐
 
 Use this program if you want to evaluate your model against multiple parameters and measure your own performance metrics. It is a quick way to parallelize an experiment over various machines. It is also handy when you don't want to, or can't, change the original program.
```

### Comparing `patas-2.0.5/setup.py` & `patas-2.0.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,14 @@
     ],
     entry_points = {
         'console_scripts': [
             'patas = patas.main:main'
         ],
     },
     install_requires=[
-        'csvkit', 'matplotlib'
+        'csvkit', 'seaborn'
     ],
     extras_require={
         "full": []
     }
 )
```

### Comparing `patas-2.0.5/tests/test_schemas.py` & `patas-2.0.6/tests/test_schemas.py`

 * *Files identical despite different names*

