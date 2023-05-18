# Comparing `tmp/dualopt-0.1.7.tar.gz` & `tmp/dualopt-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dualopt-0.1.7.tar", last modified: Mon May 15 05:39:56 2023, max compression
+gzip compressed data, was "dualopt-0.1.8.tar", last modified: Thu May 18 16:50:57 2023, max compression
```

## Comparing `dualopt-0.1.7.tar` & `dualopt-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 05:39:56.494077 dualopt-0.1.7/
--rw-rw-rw-   0        0        0     1091 2023-05-15 05:39:35.000000 dualopt-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     4981 2023-05-15 05:39:56.486081 dualopt-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     4296 2023-05-15 05:39:34.000000 dualopt-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 05:39:56.432122 dualopt-0.1.7/dualopt/
--rw-rw-rw-   0        0        0       96 2023-05-15 05:39:29.000000 dualopt-0.1.7/dualopt/__init__.py
--rw-rw-rw-   0        0        0     6067 2023-05-15 05:39:31.000000 dualopt-0.1.7/dualopt/classification.py
-drwxrwxrwx   0        0        0        0 2023-05-15 05:39:56.483081 dualopt-0.1.7/dualopt.egg-info/
--rw-rw-rw-   0        0        0     4981 2023-05-15 05:39:56.000000 dualopt-0.1.7/dualopt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-05-15 05:39:56.000000 dualopt-0.1.7/dualopt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 05:39:56.000000 dualopt-0.1.7/dualopt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-15 05:39:56.000000 dualopt-0.1.7/dualopt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-15 05:39:56.000000 dualopt-0.1.7/dualopt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 05:39:56.494077 dualopt-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1149 2023-05-15 05:39:32.000000 dualopt-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 16:50:57.485877 dualopt-0.1.8/
+-rw-rw-rw-   0        0        0     1091 2023-05-15 05:39:35.000000 dualopt-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0     4981 2023-05-18 16:50:57.482933 dualopt-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4296 2023-05-15 05:39:34.000000 dualopt-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 16:50:57.438025 dualopt-0.1.8/dualopt/
+-rw-rw-rw-   0        0        0       96 2023-05-15 05:39:29.000000 dualopt-0.1.8/dualopt/__init__.py
+-rw-rw-rw-   0        0        0     5920 2023-05-18 16:50:47.000000 dualopt-0.1.8/dualopt/classification.py
+drwxrwxrwx   0        0        0        0 2023-05-18 16:50:57.478881 dualopt-0.1.8/dualopt.egg-info/
+-rw-rw-rw-   0        0        0     4981 2023-05-18 16:50:57.000000 dualopt-0.1.8/dualopt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-05-18 16:50:57.000000 dualopt-0.1.8/dualopt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 16:50:57.000000 dualopt-0.1.8/dualopt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-18 16:50:57.000000 dualopt-0.1.8/dualopt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-18 16:50:57.000000 dualopt-0.1.8/dualopt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 16:50:57.485877 dualopt-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1149 2023-05-18 16:38:04.000000 dualopt-0.1.8/setup.py
```

### Comparing `dualopt-0.1.7/LICENSE` & `dualopt-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dualopt-0.1.7/PKG-INFO` & `dualopt-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dualopt
-Version: 0.1.7
+Version: 0.1.8
 Summary: Dual Optimizer Training
 Home-page: https://github.com/pranavphoenix/DualOpt
 Author: Pranav Jeevan
 Author-email: pranav13phoenix@gmail.com
 License: MIT
 Keywords: artificial intelligence,machine learning,optimizer,training,image classificationsemantic segmentation,image super-resolution
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dualopt-0.1.7/README.md` & `dualopt-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `dualopt-0.1.7/dualopt/classification.py` & `dualopt-0.1.8/dualopt/classification.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 import torch.optim as optim
 from tqdm import tqdm
 import torch.nn as nn
 from torchmetrics.classification import Accuracy
 from lion_pytorch import Lion
 
 
-def post_train(model, trainloader, testloader, device, PATH, top1, top5, traintime, testtime, num_classes, opt1 = 'adamw', pretrained = False, set_counter = 20):
+def post_train(model, trainloader, testloader, device, PATH, top1, top5, traintime, testtime, num_classes, set_counter = 20):
   optimizer = optim.SGD(model.parameters(), lr=0.001, momentum=0.9)
   print('Post-training with SGD')
 
-  top1_acc = Accuracy(task="multiclass", num_classes=10).to(device)
-  top5_acc = Accuracy(task="multiclass", num_classes=10, top_k=5).to(device)
+  top1_acc = Accuracy(task="multiclass", num_classes=num_classes).to(device)
+  top5_acc = Accuracy(task="multiclass", num_classes=num_classes, top_k=5).to(device)
 
   criterion = nn.CrossEntropyLoss()
 
   scaler = torch.cuda.amp.GradScaler()
 
   epoch = 0
   counter = 0
@@ -74,15 +74,15 @@
 
             acc = (outputs.argmax(dim=1) == labels).float().mean()
             epoch_accuracy += acc / len(trainloader)
             epoch_loss += loss / len(trainloader)
             tepoch.set_postfix_str(f" loss : {epoch_loss:.4f} - acc: {epoch_accuracy:.4f}" )
 
 
-def classification(model, trainloader, testloader, device, PATH, top1, top5, traintime, testtime, num_classes, opt1 = 'adamw', pretrained = False, set_counter = 20):
+def classification(model, trainloader, testloader, device, PATH, top1, top5, traintime, testtime, num_classes, opt1 = 'adamw', set_counter = 20):
 
   criterion = nn.CrossEntropyLoss()
 
   scaler = torch.cuda.amp.GradScaler()
 
   top1_acc = Accuracy(task="multiclass", num_classes=num_classes).to(device)
   top5_acc = Accuracy(task="multiclass", num_classes=num_classes, top_k=5).to(device)
@@ -94,18 +94,14 @@
     optimizer = Lion(model.parameters(), lr=1e-4, weight_decay=1e-2)
     print("Training with Lion")
 
   else:
     optimizer = optim.AdamW(model.parameters(), lr=0.001, betas=(0.9, 0.999), eps=1e-08, weight_decay=0.01, amsgrad=False)
     print("Training with AdamW")
 
-  # load saved model
-  if pretrained:
-    PATH = 'model.pth'
-    model.load_state_dict(torch.load(PATH))
 
   epoch = 0
   while counter < set_counter:   #Counter sets the number of epochs of non improvement before stopping
 
       t0 = time.time()
 
       train(model, trainloader, device, criterion, scaler, optimizer, epoch)
```

### Comparing `dualopt-0.1.7/dualopt.egg-info/PKG-INFO` & `dualopt-0.1.8/dualopt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dualopt
-Version: 0.1.7
+Version: 0.1.8
 Summary: Dual Optimizer Training
 Home-page: https://github.com/pranavphoenix/DualOpt
 Author: Pranav Jeevan
 Author-email: pranav13phoenix@gmail.com
 License: MIT
 Keywords: artificial intelligence,machine learning,optimizer,training,image classificationsemantic segmentation,image super-resolution
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dualopt-0.1.7/setup.py` & `dualopt-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
   name = 'dualopt',
   packages = find_packages(exclude=['examples']),
-  version = '0.1.7',
+  version = '0.1.8',
   license='MIT',
   description = 'Dual Optimizer Training',
   long_description=long_description,
   long_description_content_type = 'text/markdown',
   author = 'Pranav Jeevan',
   author_email = 'pranav13phoenix@gmail.com',
   url = 'https://github.com/pranavphoenix/DualOpt',
```

