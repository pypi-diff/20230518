# Comparing `tmp/diploma-1.0.1.tar.gz` & `tmp/diploma-1.0.2.tar.gz`

## Comparing `diploma-1.0.1.tar` & `diploma-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 diploma-1.0.1/.prettierignore
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 diploma-1.0.1/CHANGELOG.md
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 diploma-1.0.1/RELEASE.md
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 diploma-1.0.1/Untitled.ipynb
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 diploma-1.0.1/install.json
--rw-r--r--   0        0        0   309970 2020-02-02 00:00:00.000000 diploma-1.0.1/package-lock.json
--rw-r--r--   0        0        0     5742 2020-02-02 00:00:00.000000 diploma-1.0.1/package.json
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 diploma-1.0.1/setup.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 diploma-1.0.1/tsconfig.json
--rw-r--r--   0        0        0   189319 2020-02-02 00:00:00.000000 diploma-1.0.1/yarn.lock
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 diploma-1.0.1/diploma/__init__.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 diploma-1.0.1/diploma/_version.py
--rw-r--r--   0        0        0     4964 2020-02-02 00:00:00.000000 diploma-1.0.1/diploma/labextension/package.json
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 diploma-1.0.1/diploma/labextension/static/568.962882a5bb99fc8a6963.js
--rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 diploma-1.0.1/diploma/labextension/static/747.5502c25ad31c15dc26c8.js
--rw-r--r--   0        0        0     6383 2020-02-02 00:00:00.000000 diploma-1.0.1/diploma/labextension/static/remoteEntry.d22adb3c9e43be6bb93e.js
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 diploma-1.0.1/diploma/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 diploma-1.0.1/diploma/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 diploma-1.0.1/src/index.ts
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 diploma-1.0.1/style/base.css
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 diploma-1.0.1/style/index.css
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 diploma-1.0.1/style/index.js
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 diploma-1.0.1/.gitignore
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 diploma-1.0.1/LICENSE
--rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 diploma-1.0.1/README.md
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 diploma-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 diploma-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 diploma-1.0.2/.prettierignore
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 diploma-1.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 diploma-1.0.2/RELEASE.md
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 diploma-1.0.2/Untitled.ipynb
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 diploma-1.0.2/install.json
+-rw-r--r--   0        0        0   309970 2020-02-02 00:00:00.000000 diploma-1.0.2/package-lock.json
+-rw-r--r--   0        0        0     5742 2020-02-02 00:00:00.000000 diploma-1.0.2/package.json
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 diploma-1.0.2/setup.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 diploma-1.0.2/tsconfig.json
+-rw-r--r--   0        0        0   189319 2020-02-02 00:00:00.000000 diploma-1.0.2/yarn.lock
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 diploma-1.0.2/diploma/__init__.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 diploma-1.0.2/diploma/_version.py
+-rw-r--r--   0        0        0     4964 2020-02-02 00:00:00.000000 diploma-1.0.2/diploma/labextension/package.json
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 diploma-1.0.2/diploma/labextension/static/568.e923939cfca8f87d41ed.js
+-rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 diploma-1.0.2/diploma/labextension/static/747.5502c25ad31c15dc26c8.js
+-rw-r--r--   0        0        0     6383 2020-02-02 00:00:00.000000 diploma-1.0.2/diploma/labextension/static/remoteEntry.a1f3889159c32ac462bd.js
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 diploma-1.0.2/diploma/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 diploma-1.0.2/diploma/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 diploma-1.0.2/src/index.ts
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 diploma-1.0.2/style/base.css
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 diploma-1.0.2/style/index.css
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 diploma-1.0.2/style/index.js
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 diploma-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 diploma-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 diploma-1.0.2/README.md
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 diploma-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 diploma-1.0.2/PKG-INFO
```

### Comparing `diploma-1.0.1/RELEASE.md` & `diploma-1.0.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `diploma-1.0.1/package-lock.json` & `diploma-1.0.2/package-lock.json`

 * *Files identical despite different names*

### Comparing `diploma-1.0.1/package.json` & `diploma-1.0.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'1.0.2'"}*

```diff
@@ -159,9 +159,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.1"
+    "version": "1.0.2"
 }
```

### Comparing `diploma-1.0.1/tsconfig.json` & `diploma-1.0.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `diploma-1.0.1/yarn.lock` & `diploma-1.0.2/yarn.lock`

 * *Files identical despite different names*

### Comparing `diploma-1.0.1/diploma/labextension/package.json` & `diploma-1.0.2/diploma/labextension/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9785879629629629%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static\\\\remoteEntry.a1f3889159c32ac462bd.js'}}",*

 * * "'version'": "'1.0.2'"}*

```diff
@@ -92,15 +92,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/FMyb/diplomaext",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static\\remoteEntry.d22adb3c9e43be6bb93e.js",
+            "load": "static\\remoteEntry.a1f3889159c32ac462bd.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "diploma/labextension"
     },
     "keywords": [
         "jupyter",
@@ -164,9 +164,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.1"
+    "version": "1.0.2"
 }
```

### Comparing `diploma-1.0.1/diploma/labextension/static/568.962882a5bb99fc8a6963.js` & `diploma-1.0.2/diploma/labextension/static/568.e923939cfca8f87d41ed.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -38,26 +38,24 @@
                             let t;
                             return t = null != o ? o.data.map((t => t.name)) : ["current vm"], n.InputDialog.getItem({
                                 title: "Switch to vm",
                                 items: t
                             }).then((async t => {
                                 if (t.button.accept && null != o) {
                                     let e = o.data.find((e => e.name === t.value));
-                                    const a = t => new Promise((e => setTimeout(e, t)));
                                     if (null != e) {
-                                        await a(1e4);
                                         const t = await fetch(`${i}/api/switch_vm`, {
                                             method: "POST",
                                             headers: {
                                                 "Content-Type": "application/json"
                                             },
                                             body: JSON.stringify(e)
                                         });
                                         if (!t.ok) throw new Error("failed to switch vm");
-                                        null == t.body ? window.location.href = document.location.href : window.location.href = await t.text()
+                                        null == t.body ? location.href = document.location.href : location.href = await t.text()
                                     }
                                 }
                             }))
                         },
                         tooltip: "Move state"
                     });
                     return t.toolbar.insertItem(10, "moveState", s), new a.DisposableDelegate((() => {
```

### Comparing `diploma-1.0.1/diploma/labextension/static/747.5502c25ad31c15dc26c8.js` & `diploma-1.0.2/diploma/labextension/static/747.5502c25ad31c15dc26c8.js`

 * *Files identical despite different names*

### Comparing `diploma-1.0.1/diploma/labextension/static/remoteEntry.d22adb3c9e43be6bb93e.js` & `diploma-1.0.2/diploma/labextension/static/remoteEntry.a1f3889159c32ac462bd.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, s, f, d, p, c, h, v, b = {
+    var e, r, t, n, o, a, i, u, l, f, s, d, p, c, h, v, m = {
             460: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(568).then((() => () => t(568))),
                         "./extension": () => t.e(568).then((() => () => t(568))),
                         "./style": () => t.e(747).then((() => () => t(747)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -21,57 +21,57 @@
                     };
                 t.d(r, {
                     get: () => o,
                     init: () => a
                 })
             }
         },
-        m = {};
+        b = {};
 
     function g(e) {
-        var r = m[e];
+        var r = b[e];
         if (void 0 !== r) return r.exports;
-        var t = m[e] = {
+        var t = b[e] = {
             id: e,
             exports: {}
         };
-        return b[e](t, t.exports, g), t.exports
+        return m[e](t, t.exports, g), t.exports
     }
-    g.m = b, g.c = m, g.n = e => {
+    g.m = m, g.c = b, g.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
         return g.d(r, {
             a: r
         }), r
     }, g.d = (e, r) => {
         for (var t in r) g.o(r, t) && !g.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, g.f = {}, g.e = e => Promise.all(Object.keys(g.f).reduce(((r, t) => (g.f[t](e, r), r)), [])), g.u = e => e + "." + {
-        568: "962882a5bb99fc8a6963",
+        568: "e923939cfca8f87d41ed",
         747: "5502c25ad31c15dc26c8"
     } [e] + ".js?v=" + {
-        568: "962882a5bb99fc8a6963",
+        568: "e923939cfca8f87d41ed",
         747: "5502c25ad31c15dc26c8"
     } [e], g.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), g.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "diploma:", g.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== o)
-                for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
-                    var f = l[s];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
-                        i = f;
+                for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
+                    var s = l[f];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
+                        i = s;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, g.nc && i.setAttribute("nonce", g.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
             var d = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(p);
                     var o = e[t];
@@ -106,15 +106,15 @@
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => g.e(568).then((() => () => g(568))),
                         from: i,
                         eager: !1
                     })
-                })("diploma", "1.0.1"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("diploma", "1.0.2"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         g.g.importScripts && (e = g.g.location + "");
         var r = g.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -164,31 +164,31 @@
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var s, f, d = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
-                if ("u" == f) {
+                var f, s, d = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
+                if ("u" == s) {
                     if (!l || "u" != d) return !1
                 } else if (l)
-                    if (d == f)
+                    if (d == s)
                         if (u <= n) {
-                            if (s != e[u]) return !1
+                            if (f != e[u]) return !1
                         } else {
-                            if (o ? s > e[u] : s < e[u]) return !1;
-                            s != e[u] && (l = !1)
+                            if (o ? f > e[u] : f < e[u]) return !1;
+                            f != e[u] && (l = !1)
                         }
                 else if ("s" != d && "n" != d) {
                     if (o || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || f < d != o) return !1;
+                    if (u <= n || s < d != o) return !1;
                     l = !1
                 } else "s" != d && "n" != d && (l = !1, u--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
@@ -199,23 +199,23 @@
     }, i = (e, r) => {
         var t = g.S[e];
         if (!t || !g.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
+    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
         var o = u(e, t);
-        return a(n, o) || f(l(e, t, o, n)), d(e[t][o])
-    }, f = e => {
+        return a(n, o) || s(l(e, t, o, n)), d(e[t][o])
+    }, s = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, d = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, o) {
         var a = g.I(r);
         return a && a.then ? a.then(e.bind(e, r, g.S[r], t, n, o)) : e(r, g.S[r], t, n)
-    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), c = {}, h = {
+    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), c = {}, h = {
         33: () => p("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
         923: () => p("default", "@lumino/disposable", [1, 1, 10, 0])
     }, v = {
         568: [33, 923]
     }, g.f.consumes = (e, r) => {
         g.o(v, e) && v[e].forEach((e => {
             if (g.o(c, e)) return r.push(c[e]);
```

### Comparing `diploma-1.0.1/diploma/labextension/static/third-party-licenses.json` & `diploma-1.0.2/diploma/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `diploma-1.0.1/src/index.ts` & `diploma-1.0.2/src/index.ts`

 * *Files 2% similar despite different names*

```diff
@@ -64,31 +64,29 @@
             }
             return InputDialog.getItem({
                 title: 'Switch to vm',
                 items: items
             }).then(async result => {
                 if (result.button.accept && availableVm != undefined) {
                     let vm = availableVm.data.find(it => it.name === result.value);
-                    const sleep = (ms : number) => new Promise(r => setTimeout(r, ms));
                     if (vm != undefined) {
-                        await sleep(10000);
                         const response =  await fetch(`${currentAddress}/api/switch_vm`, {
                             method: 'POST',
                             headers: {
                                 'Content-Type': 'application/json'
                             },
                             body: JSON.stringify(vm)
                         });
                         if (!response.ok) {
                             throw new Error('failed to switch vm');
                         }
                         if (response.body == null) {
-                            window.location.href = document.location.href
+                            location.href = document.location.href
                         } else {
-                            window.location.href = await response.text()
+                            location.href = await response.text()
                         }
                     }
                 }
             })
         };
 
         const button = new ToolbarButton({
```

### Comparing `diploma-1.0.1/.gitignore` & `diploma-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `diploma-1.0.1/LICENSE` & `diploma-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `diploma-1.0.1/README.md` & `diploma-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `diploma-1.0.1/pyproject.toml` & `diploma-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `diploma-1.0.1/PKG-INFO` & `diploma-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diploma
-Version: 1.0.1
+Version: 1.0.2
 Summary: A JupyterLab extension.
 Project-URL: Homepage, https://github.com/FMyb/diplomaext
 Project-URL: Bug Tracker, https://github.com/FMyb/diplomaext/issues
 Project-URL: Repository, https://github.com/FMyb/diplomaext.git
 Author-email: FMyb <neznayu.ucoz.org@gmail.com>
 License: BSD 3-Clause License
```

