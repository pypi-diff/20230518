# Comparing `tmp/qufit-1.1.6.tar.gz` & `tmp/qufit-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qufit-1.1.6.tar", last modified: Tue Apr 25 15:02:08 2023, max compression
+gzip compressed data, was "qufit-1.1.7.tar", last modified: Thu May 18 10:36:38 2023, max compression
```

## Comparing `qufit-1.1.6.tar` & `qufit-1.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 15:02:08.703328 qufit-1.1.6/
--rw-rw-rw-   0        0        0      820 2023-04-25 15:02:08.702331 qufit-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      331 2022-11-06 13:08:56.000000 qufit-1.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 15:02:08.684380 qufit-1.1.6/qufit/
--rw-rw-rw-   0        0        0       16 2022-11-06 12:49:07.000000 qufit-1.1.6/qufit/__init__.py
--rw-rw-rw-   0        0        0    26246 2023-04-25 15:01:15.000000 qufit-1.1.6/qufit/dataTools.py
--rw-rw-rw-   0        0        0     3907 2022-09-21 03:02:11.000000 qufit-1.1.6/qufit/opt.py
--rw-rw-rw-   0        0        0    59941 2023-04-24 07:03:24.000000 qufit-1.1.6/qufit/optimize.py
-drwxrwxrwx   0        0        0        0 2023-04-25 15:02:08.701338 qufit-1.1.6/qufit.egg-info/
--rw-rw-rw-   0        0        0      820 2023-04-25 15:02:08.000000 qufit-1.1.6/qufit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-04-25 15:02:08.000000 qufit-1.1.6/qufit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 15:02:08.000000 qufit-1.1.6/qufit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-25 15:02:08.000000 qufit-1.1.6/qufit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 15:02:08.703328 qufit-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0      707 2023-04-25 15:01:52.000000 qufit-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 10:36:38.192907 qufit-1.1.7/
+-rw-rw-rw-   0        0        0      820 2023-05-18 10:36:38.191910 qufit-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2022-11-06 13:08:56.000000 qufit-1.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 10:36:38.161988 qufit-1.1.7/qufit/
+-rw-rw-rw-   0        0        0       16 2022-11-06 12:49:07.000000 qufit-1.1.7/qufit/__init__.py
+-rw-rw-rw-   0        0        0    27120 2023-05-18 10:36:05.000000 qufit-1.1.7/qufit/dataTools.py
+-rw-rw-rw-   0        0        0     3907 2022-09-21 03:02:11.000000 qufit-1.1.7/qufit/opt.py
+-rw-rw-rw-   0        0        0    59941 2023-04-24 07:03:24.000000 qufit-1.1.7/qufit/optimize.py
+drwxrwxrwx   0        0        0        0 2023-05-18 10:36:38.189915 qufit-1.1.7/qufit.egg-info/
+-rw-rw-rw-   0        0        0      820 2023-05-18 10:36:37.000000 qufit-1.1.7/qufit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-05-18 10:36:38.000000 qufit-1.1.7/qufit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 10:36:37.000000 qufit-1.1.7/qufit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-18 10:36:37.000000 qufit-1.1.7/qufit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 10:36:38.192907 qufit-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      707 2023-05-18 10:35:53.000000 qufit-1.1.7/setup.py
```

### Comparing `qufit-1.1.6/PKG-INFO` & `qufit-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qufit
-Version: 1.1.6
+Version: 1.1.7
 Summary: 本模块包括了超导量子计算实验中常用模型的拟合函数于数据处理方法。
 Home-page: https://pypi.org/
 Author: 赵寿宽(sk zhao)
 Author-email: 2396776980@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qufit-1.1.6/qufit/dataTools.py` & `qufit-1.1.7/qufit/dataTools.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,93 +323,110 @@
         num1 = np.count_nonzero(s1_cut)
         print(num0)
         num0 /= (num0+num1)
         num1 /= (num0+num1)
 
         return num0, num1
 
-def find_circle(s_st,target=0,stdnum=1,n_clusters=2):
+def find_circle(s_st,target=0,stdnum=1,n_clusters=2,figsize=(9,14)):
     from collections.abc import Iterable
     dim = np.shape(s_st)[-1]
     target = target if isinstance(target,Iterable) else [target]
     fig, axes = plt.subplots(ncols=2,nrows=dim,figsize=(9,14))
     cLst_m, num0Lst, num1Lst = [], [], []
     cLst, pLst = [], []
     for i,qi in enumerate(range(dim)):
         ax0 = axes[i][0] if dim>1 else axes[0]
         ax1 = axes[i][1] if dim>1 else axes[1]
- 
-        x,z, predict,center,color,p=Classify_fit(s_st,qnum=i,nstate=n_clusters)
-        pLst.append(p)
-        center = np.array([center[i][0]+1j*center[i][1] for i in range(n_clusters)])
-        center0, center1 = center[:2]
-        if n_clusters < 3:
+        if qi not in target:
             s_off, s_on = s_st[0,:,qi], s_st[1,:,qi]
             sdiff = complex((center1-center0))
             s0 = s_off / (sdiff/np.abs(sdiff))
             s1 = s_on / (sdiff/np.abs(sdiff))
             s0 = np.real(s0)
             s1 = np.real(s1)
             bins = 120
-            mu = complex(center1)/ (sdiff/np.abs(sdiff))
-            x0 = np.linspace(min(s0),max(s0),bins)
-            x1_old = np.linspace(min(s1),max(s1),bins)
-            lower, high = np.real(mu)-2*np.std(s1), np.real(mu)+2*np.std(s1)
-            x1 = x1_old[x1_old>lower]
 
             bin0 = ax1.hist(s0,bins=bins)
             bin1 = ax1.hist(s1,bins=bins)
-            para0, func0 = op.Gaussian_Fit().fitGaussian(x0,bin0[0],fine=False)
-            ax1.plot(x0,func0(x0,para0.x))
-            b1 = bin1[0][x1_old>lower]
-            b1 = b1[x1<high]
-            x1 = x1[x1<high]
-            para1, func1 = op.Gaussian_Fit().fitGaussian(x1,b1,fine=False)
-            ax1.plot(x1,func1(x1,para1.x))
-        #     axes[0].set_title(f'center={center0,center1}')
-
-            offstd, onstd = stdnum*np.abs(para0.x[2]), stdnum*np.abs(para1.x[2])
-            theta = np.arange(0, 2*np.pi, 0.01)
-            roff = center0.real + offstd * np.cos(theta)
-            ioff = center0.imag + offstd * np.sin(theta)
-            ron = center1.real + onstd * np.cos(theta)
-            ion = center1.imag + onstd * np.sin(theta)
+         
             ax0.plot(np.real(s_off),np.imag(s_off),'.')
-            # ax0.plot(np.real(s_on2),np.imag(s_on2),'.',alpha=0.4)
             ax0.plot(np.real(s_on),np.imag(s_on),'.')
-            ax0.plot(center1.real,center1.imag,'bo')
-            ax0.plot(center0.real,center0.imag,'ro')
-            ax0.plot(roff,ioff)
-            ax0.plot(ron,ion)
             ax0.axis('equal')
-            cLst_m.append([(center0,offstd),(center1,onstd)])
-            # cLst.append([c0Lst,c1Lst])
-            num0, _ = cutCircle((center0,offstd),(center1,onstd),s_off)
-            _, num1 = cutCircle((center0,offstd),(center1,onstd),s_on)
-            num0Lst.append(num0)
-            num1Lst.append(num1)
             plt.tight_layout()
         else:
             
-            cLst_m = [(center[i],stdnum*np.std(s_st[i,:,qi])) for i in range(n_clusters)]
-            num0Lst, num1Lst = p[:2]
-            for n_state in range(n_clusters):
-                s = s_st[n_state,:,qi]
-                ax0.plot(np.real(s),np.imag(s),'.')
-            color = ['ko','wo','bo']
-            for n_state in range(n_clusters):
-                s = s_st[n_state,:,qi]
+            x,z, predict,center,color,p=Classify_fit(s_st,qnum=i,nstate=n_clusters)
+            pLst.append(p)
+            center = np.array([center[i][0]+1j*center[i][1] for i in range(n_clusters)])
+            center0, center1 = center[:2]
+            if n_clusters < 3:
+                s_off, s_on = s_st[0,:,qi], s_st[1,:,qi]
+                sdiff = complex((center1-center0))
+                s0 = s_off / (sdiff/np.abs(sdiff))
+                s1 = s_on / (sdiff/np.abs(sdiff))
+                s0 = np.real(s0)
+                s1 = np.real(s1)
+                bins = 120
+                mu = complex(center1)/ (sdiff/np.abs(sdiff))
+                x0 = np.linspace(min(s0),max(s0),bins)
+                x1_old = np.linspace(min(s1),max(s1),bins)
+                lower, high = np.real(mu)-2*np.std(s1), np.real(mu)+2*np.std(s1)
+                x1 = x1_old[x1_old>lower]
+
+                bin0 = ax1.hist(s0,bins=bins)
+                bin1 = ax1.hist(s1,bins=bins)
+                para0, func0 = op.Gaussian_Fit().fitGaussian(x0,bin0[0],fine=False)
+                ax1.plot(x0,func0(x0,para0.x))
+                b1 = bin1[0][x1_old>lower]
+                b1 = b1[x1<high]
+                x1 = x1[x1<high]
+                para1, func1 = op.Gaussian_Fit().fitGaussian(x1,b1,fine=False)
+                ax1.plot(x1,func1(x1,para1.x))
+            #     axes[0].set_title(f'center={center0,center1}')
+
+                offstd, onstd = stdnum*np.abs(para0.x[2]), stdnum*np.abs(para1.x[2])
                 theta = np.arange(0, 2*np.pi, 0.01)
-                roff = np.real(center[n_state]) + stdnum*np.std(s) * np.cos(theta)
-                ioff = np.imag(center[n_state]) + stdnum*np.std(s) * np.sin(theta)
-                ax0.plot(np.real(center[n_state]),np.imag(center[n_state]),color[n_state],label=str(n_state))
+                roff = center0.real + offstd * np.cos(theta)
+                ioff = center0.imag + offstd * np.sin(theta)
+                ron = center1.real + onstd * np.cos(theta)
+                ion = center1.imag + onstd * np.sin(theta)
+                ax0.plot(np.real(s_off),np.imag(s_off),'.')
+                # ax0.plot(np.real(s_on2),np.imag(s_on2),'.',alpha=0.4)
+                ax0.plot(np.real(s_on),np.imag(s_on),'.')
+                ax0.plot(center1.real,center1.imag,'bo')
+                ax0.plot(center0.real,center0.imag,'ro')
                 ax0.plot(roff,ioff)
+                ax0.plot(ron,ion)
                 ax0.axis('equal')
-            ax0.legend()
-        cLst.append(cLst_m)
+                cLst_m.append([(center0,offstd),(center1,onstd)])
+                # cLst.append([c0Lst,c1Lst])
+                num0, _ = cutCircle((center0,offstd),(center1,onstd),s_off)
+                _, num1 = cutCircle((center0,offstd),(center1,onstd),s_on)
+                num0Lst.append(num0)
+                num1Lst.append(num1)
+                plt.tight_layout()
+            else:
+
+                cLst_m = [(center[i],stdnum*np.std(s_st[i,:,qi])) for i in range(n_clusters)]
+                num0Lst, num1Lst = p[:2]
+                for n_state in range(n_clusters):
+                    s = s_st[n_state,:,qi]
+                    ax0.plot(np.real(s),np.imag(s),'.')
+                color = ['ko','wo','bo']
+                for n_state in range(n_clusters):
+                    s = s_st[n_state,:,qi]
+                    theta = np.arange(0, 2*np.pi, 0.01)
+                    roff = np.real(center[n_state]) + stdnum*np.std(s) * np.cos(theta)
+                    ioff = np.imag(center[n_state]) + stdnum*np.std(s) * np.sin(theta)
+                    ax0.plot(np.real(center[n_state]),np.imag(center[n_state]),color[n_state],label=str(n_state))
+                    ax0.plot(roff,ioff)
+                    ax0.axis('equal')
+                ax0.legend()
+            cLst.append(cLst_m)
     return cLst, num0Lst, num1Lst, fig, axes, pLst
     
 
 def post_selection(measure,s,sigma_num=2):
     center0,center1 = [], []
     radius0, radius1 = [], []
     for i in measure.postSle:
```

### Comparing `qufit-1.1.6/qufit/opt.py` & `qufit-1.1.7/qufit/opt.py`

 * *Files identical despite different names*

### Comparing `qufit-1.1.6/qufit/optimize.py` & `qufit-1.1.7/qufit/optimize.py`

 * *Files identical despite different names*

### Comparing `qufit-1.1.6/qufit.egg-info/PKG-INFO` & `qufit-1.1.7/qufit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qufit
-Version: 1.1.6
+Version: 1.1.7
 Summary: 本模块包括了超导量子计算实验中常用模型的拟合函数于数据处理方法。
 Home-page: https://pypi.org/
 Author: 赵寿宽(sk zhao)
 Author-email: 2396776980@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qufit-1.1.6/setup.py` & `qufit-1.1.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="qufit",
-    version="1.1.6",
+    version="1.1.7",
     author="赵寿宽(sk zhao)",
     author_email="2396776980@qq.com",
     description="本模块包括了超导量子计算实验中常用模型的拟合函数于数据处理方法。",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://pypi.org/",
     packages=setuptools.find_packages(),
```

