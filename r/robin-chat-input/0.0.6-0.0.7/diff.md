# Comparing `tmp/robin-chat-input-0.0.6.tar.gz` & `tmp/robin-chat-input-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robin-chat-input-0.0.6.tar", last modified: Wed May 17 15:57:17 2023, max compression
+gzip compressed data, was "robin-chat-input-0.0.7.tar", last modified: Thu May 18 10:49:35 2023, max compression
```

## Comparing `robin-chat-input-0.0.6.tar` & `robin-chat-input-0.0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:57:17.000902 robin-chat-input-0.0.6/
--rw-r--r--   0 chris      (501) staff       (20)     1063 2023-05-17 11:31:38.000000 robin-chat-input-0.0.6/LICENSE
--rw-r--r--   0 chris      (501) staff       (20)       52 2023-05-17 15:07:24.000000 robin-chat-input-0.0.6/MANIFEST.in
--rw-r--r--   0 chris      (501) staff       (20)      208 2023-05-17 15:57:17.000737 robin-chat-input-0.0.6/PKG-INFO
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:57:16.994705 robin-chat-input-0.0.6/robin_chat_input/
--rw-r--r--   0 chris      (501) staff       (20)     3489 2023-05-17 15:57:06.000000 robin-chat-input-0.0.6/robin_chat_input/__init__.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:57:16.993838 robin-chat-input-0.0.6/robin_chat_input/frontend/
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:57:16.996568 robin-chat-input-0.0.6/robin_chat_input/frontend/build/
--rw-r--r--   0 chris      (501) staff       (20)      691 2023-05-17 15:07:42.000000 robin-chat-input-0.0.6/robin_chat_input/frontend/build/asset-manifest.json
--rw-r--r--   0 chris      (501) staff       (20)   197459 2023-05-17 15:07:39.000000 robin-chat-input-0.0.6/robin_chat_input/frontend/build/bootstrap.min.css
--rw-r--r--   0 chris      (501) staff       (20)     2101 2023-05-17 15:07:42.000000 robin-chat-input-0.0.6/robin_chat_input/frontend/build/index.html
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:57:16.993974 robin-chat-input-0.0.6/robin_chat_input/frontend/build/static/
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:57:17.000388 robin-chat-input-0.0.6/robin_chat_input/frontend/build/static/js/
--rw-r--r--   0 chris      (501) staff       (20)   464246 2023-05-17 15:07:42.000000 robin-chat-input-0.0.6/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js
--rw-r--r--   0 chris      (501) staff       (20)     2059 2023-05-17 15:07:42.000000 robin-chat-input-0.0.6/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js.LICENSE.txt
--rw-r--r--   0 chris      (501) staff       (20)  1710225 2023-05-17 15:07:42.000000 robin-chat-input-0.0.6/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js.map
--rw-r--r--   0 chris      (501) staff       (20)     1620 2023-05-17 15:07:42.000000 robin-chat-input-0.0.6/robin_chat_input/frontend/build/static/js/main.63e3d358.chunk.js
--rw-r--r--   0 chris      (501) staff       (20)     4657 2023-05-17 15:07:42.000000 robin-chat-input-0.0.6/robin_chat_input/frontend/build/static/js/main.63e3d358.chunk.js.map
--rw-r--r--   0 chris      (501) staff       (20)     1598 2023-05-17 15:07:42.000000 robin-chat-input-0.0.6/robin_chat_input/frontend/build/static/js/runtime-main.e6b0ae4c.js
--rw-r--r--   0 chris      (501) staff       (20)     8383 2023-05-17 15:07:42.000000 robin-chat-input-0.0.6/robin_chat_input/frontend/build/static/js/runtime-main.e6b0ae4c.js.map
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:57:16.995336 robin-chat-input-0.0.6/robin_chat_input.egg-info/
--rw-r--r--   0 chris      (501) staff       (20)      208 2023-05-17 15:57:16.000000 robin-chat-input-0.0.6/robin_chat_input.egg-info/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)      875 2023-05-17 15:57:16.000000 robin-chat-input-0.0.6/robin_chat_input.egg-info/SOURCES.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2023-05-17 15:57:16.000000 robin-chat-input-0.0.6/robin_chat_input.egg-info/dependency_links.txt
--rw-r--r--   0 chris      (501) staff       (20)       16 2023-05-17 15:57:16.000000 robin-chat-input-0.0.6/robin_chat_input.egg-info/requires.txt
--rw-r--r--   0 chris      (501) staff       (20)       17 2023-05-17 15:57:16.000000 robin-chat-input-0.0.6/robin_chat_input.egg-info/top_level.txt
--rw-r--r--   0 chris      (501) staff       (20)       38 2023-05-17 15:57:17.000947 robin-chat-input-0.0.6/setup.cfg
--rw-r--r--   0 chris      (501) staff       (20)      440 2023-05-17 15:57:12.000000 robin-chat-input-0.0.6/setup.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-18 10:49:35.380084 robin-chat-input-0.0.7/
+-rw-r--r--   0 chris      (501) staff       (20)     1063 2023-05-17 11:31:38.000000 robin-chat-input-0.0.7/LICENSE
+-rw-r--r--   0 chris      (501) staff       (20)       52 2023-05-17 15:07:24.000000 robin-chat-input-0.0.7/MANIFEST.in
+-rw-r--r--   0 chris      (501) staff       (20)      208 2023-05-18 10:49:35.379935 robin-chat-input-0.0.7/PKG-INFO
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-18 10:49:35.376282 robin-chat-input-0.0.7/robin_chat_input/
+-rw-r--r--   0 chris      (501) staff       (20)     3490 2023-05-18 10:46:46.000000 robin-chat-input-0.0.7/robin_chat_input/__init__.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-18 10:49:35.375251 robin-chat-input-0.0.7/robin_chat_input/frontend/
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-18 10:49:35.377776 robin-chat-input-0.0.7/robin_chat_input/frontend/build/
+-rw-r--r--   0 chris      (501) staff       (20)      691 2023-05-18 10:48:05.000000 robin-chat-input-0.0.7/robin_chat_input/frontend/build/asset-manifest.json
+-rw-r--r--   0 chris      (501) staff       (20)   197459 2023-05-18 10:48:02.000000 robin-chat-input-0.0.7/robin_chat_input/frontend/build/bootstrap.min.css
+-rw-r--r--   0 chris      (501) staff       (20)     2101 2023-05-18 10:48:05.000000 robin-chat-input-0.0.7/robin_chat_input/frontend/build/index.html
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-18 10:49:35.375382 robin-chat-input-0.0.7/robin_chat_input/frontend/build/static/
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-18 10:49:35.379743 robin-chat-input-0.0.7/robin_chat_input/frontend/build/static/js/
+-rw-r--r--   0 chris      (501) staff       (20)   464246 2023-05-18 10:48:05.000000 robin-chat-input-0.0.7/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js
+-rw-r--r--   0 chris      (501) staff       (20)     2059 2023-05-18 10:48:05.000000 robin-chat-input-0.0.7/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js.LICENSE.txt
+-rw-r--r--   0 chris      (501) staff       (20)  1710225 2023-05-18 10:48:05.000000 robin-chat-input-0.0.7/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js.map
+-rw-r--r--   0 chris      (501) staff       (20)     1630 2023-05-18 10:48:05.000000 robin-chat-input-0.0.7/robin_chat_input/frontend/build/static/js/main.f16661d0.chunk.js
+-rw-r--r--   0 chris      (501) staff       (20)     4815 2023-05-18 10:48:05.000000 robin-chat-input-0.0.7/robin_chat_input/frontend/build/static/js/main.f16661d0.chunk.js.map
+-rw-r--r--   0 chris      (501) staff       (20)     1598 2023-05-18 10:48:05.000000 robin-chat-input-0.0.7/robin_chat_input/frontend/build/static/js/runtime-main.e6b0ae4c.js
+-rw-r--r--   0 chris      (501) staff       (20)     8383 2023-05-18 10:48:05.000000 robin-chat-input-0.0.7/robin_chat_input/frontend/build/static/js/runtime-main.e6b0ae4c.js.map
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-18 10:49:35.377104 robin-chat-input-0.0.7/robin_chat_input.egg-info/
+-rw-r--r--   0 chris      (501) staff       (20)      208 2023-05-18 10:49:35.000000 robin-chat-input-0.0.7/robin_chat_input.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)      875 2023-05-18 10:49:35.000000 robin-chat-input-0.0.7/robin_chat_input.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (501) staff       (20)        1 2023-05-18 10:49:35.000000 robin-chat-input-0.0.7/robin_chat_input.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (501) staff       (20)       16 2023-05-18 10:49:35.000000 robin-chat-input-0.0.7/robin_chat_input.egg-info/requires.txt
+-rw-r--r--   0 chris      (501) staff       (20)       17 2023-05-18 10:49:35.000000 robin-chat-input-0.0.7/robin_chat_input.egg-info/top_level.txt
+-rw-r--r--   0 chris      (501) staff       (20)       38 2023-05-18 10:49:35.380120 robin-chat-input-0.0.7/setup.cfg
+-rw-r--r--   0 chris      (501) staff       (20)      440 2023-05-18 10:48:20.000000 robin-chat-input-0.0.7/setup.py
```

### Comparing `robin-chat-input-0.0.6/LICENSE` & `robin-chat-input-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `robin-chat-input-0.0.6/robin_chat_input/__init__.py` & `robin-chat-input-0.0.7/robin_chat_input/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import streamlit.components.v1 as components
 
 # Create a _RELEASE constant. We'll set this to False while we're developing
 # the component, and True when we're ready to package and distribute it.
 # (This is, of course, optional - there are innumerable ways to manage your
 # release process.)
-_RELEASE = True 
+_RELEASE = False 
 
 # Declare a Streamlit component. `declare_component` returns a function
 # that is used to create instances of the component. We're naming this
 # function "_component_func", with an underscore prefix, because we don't want
 # to expose it directly to users. Instead, we will create a custom wrapper
 # function, below, that will serve as our component's public API.
```

### Comparing `robin-chat-input-0.0.6/robin_chat_input/frontend/build/asset-manifest.json` & `robin-chat-input-0.0.7/robin_chat_input/frontend/build/asset-manifest.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.84375%*

 * *Differences: {"'entrypoints'": "{insert: [(2, 'static/js/main.f16661d0.chunk.js')], delete: [2]}",*

 * * "'files'": "{'main.js': './static/js/main.f16661d0.chunk.js', 'main.js.map': "*

 * *            "'./static/js/main.f16661d0.chunk.js.map'}"}*

```diff
@@ -1,17 +1,17 @@
 {
     "entrypoints": [
         "static/js/runtime-main.e6b0ae4c.js",
         "static/js/2.08b0a941.chunk.js",
-        "static/js/main.63e3d358.chunk.js"
+        "static/js/main.f16661d0.chunk.js"
     ],
     "files": {
         "index.html": "./index.html",
-        "main.js": "./static/js/main.63e3d358.chunk.js",
-        "main.js.map": "./static/js/main.63e3d358.chunk.js.map",
+        "main.js": "./static/js/main.f16661d0.chunk.js",
+        "main.js.map": "./static/js/main.f16661d0.chunk.js.map",
         "runtime-main.js": "./static/js/runtime-main.e6b0ae4c.js",
         "runtime-main.js.map": "./static/js/runtime-main.e6b0ae4c.js.map",
         "static/js/2.08b0a941.chunk.js": "./static/js/2.08b0a941.chunk.js",
         "static/js/2.08b0a941.chunk.js.LICENSE.txt": "./static/js/2.08b0a941.chunk.js.LICENSE.txt",
         "static/js/2.08b0a941.chunk.js.map": "./static/js/2.08b0a941.chunk.js.map"
     }
 }
```

### Comparing `robin-chat-input-0.0.6/robin_chat_input/frontend/build/bootstrap.min.css` & `robin-chat-input-0.0.7/robin_chat_input/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `robin-chat-input-0.0.6/robin_chat_input/frontend/build/index.html` & `robin-chat-input-0.0.7/robin_chat_input/frontend/build/index.html`

 * *Files 15% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.08b0a941.chunk.js"></script><script src="./static/js/main.63e3d358.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.08b0a941.chunk.js"></script><script src="./static/js/main.f16661d0.chunk.js"></script></body></html>
```

### Comparing `robin-chat-input-0.0.6/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js` & `robin-chat-input-0.0.7/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js`

 * *Files identical despite different names*

### Comparing `robin-chat-input-0.0.6/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js.LICENSE.txt` & `robin-chat-input-0.0.7/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robin-chat-input-0.0.6/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js.map` & `robin-chat-input-0.0.7/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js.map`

 * *Files identical despite different names*

### Comparing `robin-chat-input-0.0.6/robin_chat_input/frontend/build/static/js/main.63e3d358.chunk.js` & `robin-chat-input-0.0.7/robin_chat_input/frontend/build/static/js/main.f16661d0.chunk.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -28,14 +28,15 @@
                                 style: {
                                     padding: 20
                                 },
                                 children: Object(p.jsxs)("div", {
                                     style: {
                                         border: "solid",
                                         borderBlockColor: "#2A344F",
+                                        borderWidth: 1,
                                         padding: 15,
                                         borderRadius: 5,
                                         display: "flex",
                                         alignItems: "center"
                                     },
                                     children: [Object(p.jsx)("input", {
                                         type: "text",
@@ -48,15 +49,15 @@
                                             flex: 1
                                         }
                                     }), Object(p.jsx)("div", {
                                         style: {
                                             position: "relative"
                                         },
                                         children: Object(p.jsx)("img", {
-                                            src: "https://i.ibb.co/6X1cVqb/button-upscaled.png",
+                                            src: "https://i.ibb.co/TT47TC6/Blue-Button.png",
                                             style: {
                                                 height: 40,
                                                 marginLeft: 10,
                                                 transition: "transform 0.5s"
                                             },
                                             onMouseOver: function(t) {
                                                 return t.target.style.transform = "rotate(180deg)"
@@ -88,8 +89,8 @@
             }), document.getElementById("root"))
         }
     },
     [
         [24, 1, 2]
     ]
 ]);
-//# sourceMappingURL=main.63e3d358.chunk.js.map
+//# sourceMappingURL=main.f16661d0.chunk.js.map
```

### Comparing `robin-chat-input-0.0.6/robin_chat_input/frontend/build/static/js/main.63e3d358.chunk.js.map` & `robin-chat-input-0.0.7/robin_chat_input/frontend/build/static/js/main.f16661d0.chunk.js.map`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8083717357910907%*

 * *Differences: {"'file'": "'static/js/main.f16661d0.chunk.js'",*

 * * "'mappings'": "'oOAgBMA,EAAc,SAAAC,GAAAC,YAAAF,EAAAC,GAAA,IAAAE,EAAAC,YAAAJ,GAAA,SAAAA,IAAA,IAAAK,EAAAC,YAAA,KAAAN,GAAA,QAAAO,EAAAC,UAAAC,OAAAC,EAAA,IAAAC,MAAAJ,GAAAK,EAAA,EAAAA,EAAAL,EAAAK,IAAAF,EAAAE,GAAAJ,UAAAI,GAwDjB,OAxDiBP,EAAAF,EAAAU,KAAAC,MAAAX,EAAA,OAAAY,OAAAL,KACXM,MAAQ,CAAEC,WAAY,IAAIZ,EAE1Ba,OAAS,WACd,OACEC,cAAA,OAAKC,MAAO,CAAEC,QAAS,IAAKC,SAC1BC,eAAA,OACEH,MAAO,CACLI,OAAQ,QACRC,iBAAkB,UAClBC,YAAa,EACbL,QAAS,GACTM,aAAc,EACdC,QAAS,OACTC,WAAY,UACZP […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.63e3d358.chunk.js",
-    "mappings": "oOAgBMA,EAAc,SAAAC,GAAAC,YAAAF,EAAAC,GAAA,IAAAE,EAAAC,YAAAJ,GAAA,SAAAA,IAAA,IAAAK,EAAAC,YAAA,KAAAN,GAAA,QAAAO,EAAAC,UAAAC,OAAAC,EAAA,IAAAC,MAAAJ,GAAAK,EAAA,EAAAA,EAAAL,EAAAK,IAAAF,EAAAE,GAAAJ,UAAAI,GAiDjB,OAjDiBP,EAAAF,EAAAU,KAAAC,MAAAX,EAAA,OAAAY,OAAAL,KACXM,MAAQ,CAAEC,WAAY,IAAIZ,EAE1Ba,OAAS,WACd,OACEC,cAAA,OAAKC,MAAO,CAACC,QAAS,IAAIC,SACxBC,eAAA,OACEH,MAAO,CACLI,OAAQ,QACRC,iBAAkB,UAClBJ,QAAS,GACTK,aAAc,EACdC,QAAS,OACTC,WAAY,UACZN,SAAA,CAEFH,cAAA,SACEU,KAAK,OACLC,MAAOzB,EAAKW,MAAMC,WAClBc,SAAU1B,EAAK2B,kBACfC,YAAY,2BACZb,MAAO,CAAEI,OAAQ,OAAQU,QAAS,OAAQC,KAAM,KAElDhB,cAAA,OAAKC,MAAO,CAAEgB,SAAU,YAAad,SACnCH,cAAA,OACEkB,IAAI,+CACJjB,MAAO,CAAEkB,OAAQ,GAAIC,WAAY,GAAIC,WAAY,kBACjDC,YAAa,SAACC,GAAC,OACXA,EAAEC,OAA4BvB,MAAMwB,UAAY,gBAAgB,EAEpEC,WAAY,SAACH,GAAC,OACVA,EAAEC,OAA4BvB,MAAMwB,UAAY,cAAc,EAElEE,QAASzC,EAAK0C,0BAM1B,EAAC1C,EAEO0C,kBAAoB,WAC1BC,IAAUC,kBAAkB5C,EAAKW,MAAMC,YACvCZ,EAAK6C,SAAS,CAAEjC,WAAY,IAC9B,EAACZ,EAEO2B,kBAAoB,SAACmB,GAC3B,IAAMC,EAAYD,EAAMR,OAAOb,MAC/BzB,EAAK6C,SAAS,CAAEjC,WAAYmC,GAC9B,EAAC/C,CAAA,QAAAgD,YAAArD,EAAA,CAjDiB,CAASsD,KAyDdC,cAAwBvD,GCrEvCwD,IAAStC,OACPC,cAACsC,IAAMC,WAAU,CAAApC,SACfH,cAACnB,EAAc,MAEjB2D,SAASC,eAAe,Q",
+    "file": "static/js/main.f16661d0.chunk.js",
+    "mappings": "oOAgBMA,EAAc,SAAAC,GAAAC,YAAAF,EAAAC,GAAA,IAAAE,EAAAC,YAAAJ,GAAA,SAAAA,IAAA,IAAAK,EAAAC,YAAA,KAAAN,GAAA,QAAAO,EAAAC,UAAAC,OAAAC,EAAA,IAAAC,MAAAJ,GAAAK,EAAA,EAAAA,EAAAL,EAAAK,IAAAF,EAAAE,GAAAJ,UAAAI,GAwDjB,OAxDiBP,EAAAF,EAAAU,KAAAC,MAAAX,EAAA,OAAAY,OAAAL,KACXM,MAAQ,CAAEC,WAAY,IAAIZ,EAE1Ba,OAAS,WACd,OACEC,cAAA,OAAKC,MAAO,CAAEC,QAAS,IAAKC,SAC1BC,eAAA,OACEH,MAAO,CACLI,OAAQ,QACRC,iBAAkB,UAClBC,YAAa,EACbL,QAAS,GACTM,aAAc,EACdC,QAAS,OACTC,WAAY,UACZP,SAAA,CAEFH,cAAA,SACEW,KAAK,OACLC,MAAO1B,EAAKW,MAAMC,WAClBe,SAAU3B,EAAK4B,kBACfC,YAAY,2BACZd,MAAO,CAAEI,OAAQ,OAAQW,QAAS,OAAQC,KAAM,KAElDjB,cAAA,OAAKC,MAAO,CAAEiB,SAAU,YAAaf,SACnCH,cAAA,OACEmB,IAAI,2CACJlB,MAAO,CACLmB,OAAQ,GACRC,WAAY,GACZC,WAAY,kBAEdC,YAAa,SAACC,GAAC,OACXA,EAAEC,OAA4BxB,MAAMyB,UACpC,gBAAgB,EAEpBC,WAAY,SAACH,GAAC,OACVA,EAAEC,OAA4BxB,MAAMyB,UACpC,cAAc,EAElBE,QAAS1C,EAAK2C,0BAM1B,EAAC3C,EAEO2C,kBAAoB,WAC1BC,IAAUC,kBAAkB7C,EAAKW,MAAMC,YACvCZ,EAAK8C,SAAS,CAAElC,WAAY,IAC9B,EAACZ,EAEO4B,kBAAoB,SAACmB,GAC3B,IAAMC,EAAYD,EAAMR,OAAOb,MAC/B1B,EAAK8C,SAAS,CAAElC,WAAYoC,GAC9B,EAAChD,CAAA,QAAAiD,YAAAtD,EAAA,CAxDiB,CAASuD,KAgEdC,cAAwBxD,GC5EvCyD,IAASvC,OACPC,cAACuC,IAAMC,WAAU,CAAArC,SACfH,cAACnB,EAAc,MAEjB4D,SAASC,eAAe,Q",
     "names": [
         "RobinChatInput",
         "_StreamlitComponentBa",
         "_inherits",
         "_super",
         "_createSuper",
         "_this",
@@ -24,14 +24,15 @@
         "_jsx",
         "style",
         "padding",
         "children",
         "_jsxs",
         "border",
         "borderBlockColor",
+        "borderWidth",
         "borderRadius",
         "display",
         "alignItems",
         "type",
         "value",
         "onChange",
         "handleInputChange",
@@ -66,12 +67,12 @@
     ],
     "sourceRoot": "",
     "sources": [
         "RobinChatInput.tsx",
         "index.tsx"
     ],
     "sourcesContent": [
-        "import {\n  Streamlit,\n  StreamlitComponentBase,\n  withStreamlitConnection,\n} from \"streamlit-component-lib\"\nimport React, { ReactNode } from \"react\"\n\n\ninterface State {\n  inputValue: string\n}\n\n/**\n * This is a React-based component template. The `render()` function is called\n * automatically when your component should be re-rendered.\n */\nclass RobinChatInput extends StreamlitComponentBase<State> {\n  public state = { inputValue: \"\" }\n\n  public render = (): ReactNode => {\n    return (\n      <div style={{padding: 20}}>\n        <div\n          style={{\n            border: \"solid\",\n            borderBlockColor: \"#2A344F\",\n            padding: 15,\n            borderRadius: 5,\n            display: \"flex\",\n            alignItems: \"center\",\n          }}\n        >\n          <input\n            type=\"text\"\n            value={this.state.inputValue}\n            onChange={this.handleInputChange}\n            placeholder=\"Enter your question here\"\n            style={{ border: \"none\", outline: \"none\", flex: 1 }}\n          />\n          <div style={{ position: \"relative\" }}>\n            <img\n              src=\"https://i.ibb.co/6X1cVqb/button-upscaled.png\"\n              style={{ height: 40, marginLeft: 10, transition: \"transform 0.5s\" }}\n              onMouseOver={(e) =>\n                ((e.target as HTMLImageElement).style.transform = \"rotate(180deg)\")\n              }\n              onMouseOut={(e) =>\n                ((e.target as HTMLImageElement).style.transform = \"rotate(0deg)\")\n              }\n              onClick={this.handleInputSubmit}\n            />\n          </div>\n        </div>\n      </div>\n    )\n  }\n\n  private handleInputSubmit = (): void => {\n    Streamlit.setComponentValue(this.state.inputValue)\n    this.setState({ inputValue: \"\" })\n  }\n\n  private handleInputChange = (event: React.ChangeEvent<HTMLInputElement>) => {\n    const userInput = event.target.value\n    this.setState({ inputValue: userInput })\n  }\n}\n\n// \"withStreamlitConnection\" is a wrapper function. It bootstraps the\n// connection between your component and the Streamlit app, and handles\n// passing arguments from Python -> Component.\n//\n// You don't need to edit withStreamlitConnection (but you're welcome to!).\nexport default withStreamlitConnection(RobinChatInput)\n",
+        "import {\n  Streamlit,\n  StreamlitComponentBase,\n  withStreamlitConnection,\n} from \"streamlit-component-lib\"\nimport React, { ReactNode } from \"react\"\n\n\ninterface State {\n  inputValue: string\n}\n\n/**\n * This is a React-based component template. The `render()` function is called\n * automatically when your component should be re-rendered.\n */\nclass RobinChatInput extends StreamlitComponentBase<State> {\n  public state = { inputValue: \"\" }\n\n  public render = (): ReactNode => {\n    return (\n      <div style={{ padding: 20 }}>\n        <div\n          style={{\n            border: \"solid\",\n            borderBlockColor: \"#2A344F\",\n            borderWidth: 1,\n            padding: 15,\n            borderRadius: 5,\n            display: \"flex\",\n            alignItems: \"center\",\n          }}\n        >\n          <input\n            type=\"text\"\n            value={this.state.inputValue}\n            onChange={this.handleInputChange}\n            placeholder=\"Enter your question here\"\n            style={{ border: \"none\", outline: \"none\", flex: 1 }}\n          />\n          <div style={{ position: \"relative\" }}>\n            <img\n              src=\"https://i.ibb.co/TT47TC6/Blue-Button.png\"\n              style={{\n                height: 40,\n                marginLeft: 10,\n                transition: \"transform 0.5s\",\n              }}\n              onMouseOver={(e) =>\n                ((e.target as HTMLImageElement).style.transform =\n                  \"rotate(180deg)\")\n              }\n              onMouseOut={(e) =>\n                ((e.target as HTMLImageElement).style.transform =\n                  \"rotate(0deg)\")\n              }\n              onClick={this.handleInputSubmit}\n            />\n          </div>\n        </div>\n      </div>\n    )\n  }\n\n  private handleInputSubmit = (): void => {\n    Streamlit.setComponentValue(this.state.inputValue)\n    this.setState({ inputValue: \"\" })\n  }\n\n  private handleInputChange = (event: React.ChangeEvent<HTMLInputElement>) => {\n    const userInput = event.target.value\n    this.setState({ inputValue: userInput })\n  }\n}\n\n// \"withStreamlitConnection\" is a wrapper function. It bootstraps the\n// connection between your component and the Streamlit app, and handles\n// passing arguments from Python -> Component.\n//\n// You don't need to edit withStreamlitConnection (but you're welcome to!).\nexport default withStreamlitConnection(RobinChatInput)\n",
         "import React from \"react\"\nimport ReactDOM from \"react-dom\"\nimport RobinChatInput from \"./RobinChatInput\"\n\nReactDOM.render(\n  <React.StrictMode>\n    <RobinChatInput />\n  </React.StrictMode>,\n  document.getElementById(\"root\")\n)\n"
     ],
     "version": 3
 }
```

### Comparing `robin-chat-input-0.0.6/robin_chat_input/frontend/build/static/js/runtime-main.e6b0ae4c.js` & `robin-chat-input-0.0.7/robin_chat_input/frontend/build/static/js/runtime-main.e6b0ae4c.js`

 * *Files identical despite different names*

### Comparing `robin-chat-input-0.0.6/robin_chat_input/frontend/build/static/js/runtime-main.e6b0ae4c.js.map` & `robin-chat-input-0.0.7/robin_chat_input/frontend/build/static/js/runtime-main.e6b0ae4c.js.map`

 * *Files identical despite different names*

### Comparing `robin-chat-input-0.0.6/robin_chat_input.egg-info/SOURCES.txt` & `robin-chat-input-0.0.7/robin_chat_input.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 robin_chat_input.egg-info/top_level.txt
 robin_chat_input/frontend/build/asset-manifest.json
 robin_chat_input/frontend/build/bootstrap.min.css
 robin_chat_input/frontend/build/index.html
 robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js
 robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js.LICENSE.txt
 robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js.map
-robin_chat_input/frontend/build/static/js/main.63e3d358.chunk.js
-robin_chat_input/frontend/build/static/js/main.63e3d358.chunk.js.map
+robin_chat_input/frontend/build/static/js/main.f16661d0.chunk.js
+robin_chat_input/frontend/build/static/js/main.f16661d0.chunk.js.map
 robin_chat_input/frontend/build/static/js/runtime-main.e6b0ae4c.js
 robin_chat_input/frontend/build/static/js/runtime-main.e6b0ae4c.js.map
```

