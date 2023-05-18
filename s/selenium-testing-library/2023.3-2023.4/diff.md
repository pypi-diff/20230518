# Comparing `tmp/selenium_testing_library-2023.3.tar.gz` & `tmp/selenium_testing_library-2023.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_testing_library-2023.3.tar", max compression
+gzip compressed data, was "selenium_testing_library-2023.4.tar", max compression
```

## Comparing `selenium_testing_library-2023.3.tar` & `selenium_testing_library-2023.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2021-06-06 09:30:53.872504 selenium_testing_library-2023.3/LICENSE.md
--rw-r--r--   0        0        0     9734 2023-01-08 14:45:10.963757 selenium_testing_library-2023.3/README.md
--rw-r--r--   0        0        0     1875 2023-03-29 08:30:47.626066 selenium_testing_library-2023.3/pyproject.toml
--rw-r--r--   0        0        0       60 2023-03-29 08:30:47.627822 selenium_testing_library-2023.3/selenium_testing_library/__init__.py
--rw-r--r--   0        0        0     7525 2023-02-17 17:32:49.420064 selenium_testing_library-2023.3/selenium_testing_library/locators.py
--rw-r--r--   0        0        0   220325 2023-03-29 08:28:41.894894 selenium_testing_library-2023.3/selenium_testing_library/main.js
--rw-r--r--   0        0        0        0 2021-06-05 14:50:48.385384 selenium_testing_library-2023.3/selenium_testing_library/py.typed
--rw-r--r--   0        0        0    34005 2023-02-17 17:51:00.247649 selenium_testing_library-2023.3/selenium_testing_library/screen.py
--rw-r--r--   0        0        0    10710 1970-01-01 00:00:00.000000 selenium_testing_library-2023.3/setup.py
--rw-r--r--   0        0        0    10709 1970-01-01 00:00:00.000000 selenium_testing_library-2023.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2021-06-06 09:30:53.872504 selenium_testing_library-2023.4/LICENSE.md
+-rw-r--r--   0        0        0     9734 2023-01-08 14:45:10.963757 selenium_testing_library-2023.4/README.md
+-rw-r--r--   0        0        0     1875 2023-05-18 15:30:38.881213 selenium_testing_library-2023.4/pyproject.toml
+-rw-r--r--   0        0        0       60 2023-05-18 15:30:38.882116 selenium_testing_library-2023.4/selenium_testing_library/__init__.py
+-rw-r--r--   0        0        0     7525 2023-02-17 17:32:49.420064 selenium_testing_library-2023.4/selenium_testing_library/locators.py
+-rw-r--r--   0        0        0   220550 2023-05-18 15:28:50.991379 selenium_testing_library-2023.4/selenium_testing_library/main.js
+-rw-r--r--   0        0        0        0 2021-06-05 14:50:48.385384 selenium_testing_library-2023.4/selenium_testing_library/py.typed
+-rw-r--r--   0        0        0    34005 2023-02-17 17:51:00.247649 selenium_testing_library-2023.4/selenium_testing_library/screen.py
+-rw-r--r--   0        0        0    10710 1970-01-01 00:00:00.000000 selenium_testing_library-2023.4/setup.py
+-rw-r--r--   0        0        0    10709 1970-01-01 00:00:00.000000 selenium_testing_library-2023.4/PKG-INFO
```

### Comparing `selenium_testing_library-2023.3/LICENSE.md` & `selenium_testing_library-2023.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `selenium_testing_library-2023.3/README.md` & `selenium_testing_library-2023.4/README.md`

 * *Files identical despite different names*

### Comparing `selenium_testing_library-2023.3/pyproject.toml` & `selenium_testing_library-2023.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "selenium-testing-library"
-version = "2023.3"
+version = "2023.4"
 description = "A Python Selenium library inspired by the Testing Library"
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/anze3db/selenium-testing-library"
 authors = ["Anže Pečar <anze@pecar.me>"]
 include = [
     "selenium_testing_library/main.js"
@@ -41,15 +41,15 @@
 addopts = "--selenium-headless --cov=selenium_testing_library --cov-report html --cov-report xml --verbose --durations=10"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bumpver]
-current_version = "2023.3"
+current_version = "2023.4"
 version_pattern = "YYYY.INC1"
 commit_message = "Bump version from {old_version} to {new_version} 🚀"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `selenium_testing_library-2023.3/selenium_testing_library/locators.py` & `selenium_testing_library-2023.4/selenium_testing_library/locators.py`

 * *Files identical despite different names*

### Comparing `selenium_testing_library-2023.3/selenium_testing_library/main.js` & `selenium_testing_library-2023.4/selenium_testing_library/main.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -314,21 +314,21 @@
                         if (null === t && y(e)) {
                             var r = j(e);
                             null !== r && (t = r)
                         }
                     })), t
                 }
 
-                function R(e) {
+                function S(e) {
                     if (void 0 !== e.control) return e.control;
                     var t = e.getAttribute("for");
                     return null !== t ? e.ownerDocument.getElementById(t) : j(e)
                 }
 
-                function S(e) {
+                function R(e) {
                     var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {},
                         r = new d,
                         n = function(e) {
                             var t = (null === e.ownerDocument ? e : e.ownerDocument).defaultView;
                             if (null === t) throw new TypeError("no window available");
                             return t
                         }(e),
@@ -346,15 +346,15 @@
                         if (y(e) && u) {
                             var a = E(c(e, "::before"));
                             o = "".concat(a, " ").concat(o)
                         }
                         if ((function(e) {
                                 return y(e) && "slot" === p(e)
                             }(e) ? 0 === (n = (r = e).assignedNodes()).length ? l(r.childNodes) : n : l(e.childNodes).concat(C(e, "aria-owns"))).forEach((function(e) {
-                                var r = S(e, {
+                                var r = R(e, {
                                         isEmbeddedInLabel: t.isEmbeddedInLabel,
                                         isReferenced: !1,
                                         recursion: !0
                                     }),
                                     n = "inline" !== (y(e) ? c(e).getPropertyValue("display") : "inline") ? " " : "";
                                 o += "".concat(n).concat(r).concat(n)
                             })), y(e) && u) {
@@ -365,26 +365,26 @@
                     }
 
                     function j(e, t) {
                         var n = e.getAttributeNode(t);
                         return null === n || r.has(n) || "" === n.value.trim() ? null : (r.add(n), n.value)
                     }
 
-                    function S(e, t) {
+                    function R(e, t) {
                         if (r.has(e)) return "";
                         if (!b && function(e, t) {
                                 if (!y(e)) return !1;
                                 if (e.hasAttribute("hidden") || "true" === e.getAttribute("aria-hidden")) return !0;
                                 var r = t(e);
                                 return "none" === r.getPropertyValue("display") || "hidden" === r.getPropertyValue("visibility")
                             }(e, c) && !t.isReferenced) return r.add(e), "";
                         var n = y(e) ? e.getAttributeNode("aria-labelledby") : null,
                             o = null === n || r.has(n) ? [] : C(e, "aria-labelledby");
                         if ("name" === a && !t.isReferenced && o.length > 0) return r.add(n), o.map((function(e) {
-                            return S(e, {
+                            return R(e, {
                                 isEmbeddedInLabel: t.isEmbeddedInLabel,
                                 isReferenced: !0,
                                 recursion: !1
                             })
                         })).join(" ");
                         var i, u = t.recursion && (w(i = e, ["button", "combobox", "listbox", "textbox"]) || q(i, "range")) && "name" === a;
                         if (!u) {
@@ -397,27 +397,27 @@
                                     if (!y(e)) return null;
                                     if (function(e) {
                                             return y(e) && "fieldset" === p(e)
                                         }(e)) {
                                         r.add(e);
                                         for (var t = l(e.childNodes), n = 0; n < t.length; n += 1) {
                                             var o = t[n];
-                                            if (g(o)) return S(o, {
+                                            if (g(o)) return R(o, {
                                                 isEmbeddedInLabel: !1,
                                                 isReferenced: !1,
                                                 recursion: !1
                                             })
                                         }
                                     } else if (function(e) {
                                             return y(e) && "table" === p(e)
                                         }(e)) {
                                         r.add(e);
                                         for (var a = l(e.childNodes), i = 0; i < a.length; i += 1) {
                                             var u = a[i];
-                                            if (v(u)) return S(u, {
+                                            if (v(u)) return R(u, {
                                                 isEmbeddedInLabel: !1,
                                                 isReferenced: !1,
                                                 recursion: !1
                                             })
                                         }
                                     } else {
                                         if (function(e) {
@@ -443,37 +443,37 @@
                                     if (h(e) && ("button" === e.type || "submit" === e.type || "reset" === e.type)) {
                                         var C = j(e, "value");
                                         if (null !== C) return C;
                                         if ("submit" === e.type) return "Submit";
                                         if ("reset" === e.type) return "Reset"
                                     }
                                     var q, x, E = null === (x = (q = e).labels) ? x : void 0 !== x ? l(x) : O(q) ? l(q.ownerDocument.querySelectorAll("label")).filter((function(e) {
-                                        return R(e) === q
+                                        return S(e) === q
                                     })) : null;
                                     if (null !== E && 0 !== E.length) return r.add(e), l(E).map((function(e) {
-                                        return S(e, {
+                                        return R(e, {
                                             isEmbeddedInLabel: !0,
                                             isReferenced: !1,
                                             recursion: !0
                                         })
                                     })).filter((function(e) {
                                         return e.length > 0
                                     })).join(" ");
                                     if (h(e) && "image" === e.type) {
                                         var _ = j(e, "alt");
                                         if (null !== _) return _;
                                         var A = j(e, "title");
                                         return null !== A ? A : "Submit Query"
                                     }
                                     if (w(e, ["button"])) {
-                                        var T = m(e, {
+                                        var M = m(e, {
                                             isEmbeddedInLabel: !1,
                                             isReferenced: !1
                                         });
-                                        if ("" !== T) return T
+                                        if ("" !== M) return M
                                     }
                                     return null
                                 }(e);
                                 if (null !== d) return r.add(e), d
                             }
                         }
                         if (w(e, ["menu"])) return r.add(e), "";
@@ -481,15 +481,15 @@
                             if (w(e, ["combobox", "listbox"])) {
                                 r.add(e);
                                 var f = function(e) {
                                     return y(t = e) && "select" === p(t) ? e.selectedOptions || x(e, "[selected]") : x(e, '[aria-selected="true"]');
                                     var t
                                 }(e);
                                 return 0 === f.length ? h(e) ? e.value : "" : l(f).map((function(e) {
-                                    return S(e, {
+                                    return R(e, {
                                         isEmbeddedInLabel: t.isEmbeddedInLabel,
                                         isReferenced: !1,
                                         recursion: !0
                                     })
                                 })).join(" ")
                             }
                             if (q(e, "range")) return r.add(e), e.hasAttribute("aria-valuetext") ? e.getAttribute("aria-valuetext") : e.hasAttribute("aria-valuenow") ? e.getAttribute("aria-valuenow") : e.getAttribute("value") || "";
@@ -516,15 +516,15 @@
                             isReferenced: !1
                         });
                         var _ = function(e) {
                             return y(e) ? j(e, "title") : null
                         }(e);
                         return null !== _ ? (r.add(e), _) : (r.add(e), "")
                     }
-                    return S(e, {
+                    return R(e, {
                         isEmbeddedInLabel: !1,
                         isReferenced: "description" === a,
                         recursion: !1
                     }).trim().replace(/\s\s+/g, " ")
                 }
 
                 function _(e) {
@@ -542,27 +542,27 @@
                         t && (n = n.filter((function(t) {
                             return Object.getOwnPropertyDescriptor(e, t).enumerable
                         }))), r.push.apply(r, n)
                     }
                     return r
                 }
 
-                function T(e) {
+                function M(e) {
                     for (var t = 1; t < arguments.length; t++) {
                         var r = null != arguments[t] ? arguments[t] : {};
                         t % 2 ? A(Object(r), !0).forEach((function(t) {
-                            M(e, t, r[t])
+                            T(e, t, r[t])
                         })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(r)) : A(Object(r)).forEach((function(t) {
                             Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(r, t))
                         }))
                     }
                     return e
                 }
 
-                function M(e, t, r) {
+                function T(e, t, r) {
                     return (t = function(e) {
                         var t = function(e, t) {
                             if ("object" !== _(e) || null === e) return e;
                             var r = e[Symbol.toPrimitive];
                             if (void 0 !== r) {
                                 var n = r.call(e, "string");
                                 if ("object" !== _(n)) return n;
@@ -578,28 +578,28 @@
                         writable: !0
                     }) : e[t] = r, e
                 }
 
                 function I(e) {
                     var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {},
                         r = C(e, "aria-describedby").map((function(e) {
-                            return S(e, T(T({}, t), {}, {
+                            return R(e, M(M({}, t), {}, {
                                 compute: "description"
                             }))
                         })).join(" ");
                     if ("" === r) {
                         var n = e.getAttribute("title");
                         r = null === n ? "" : n
                     }
                     return r
                 }
 
                 function k(e) {
                     var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
-                    return w(e, ["caption", "code", "deletion", "emphasis", "generic", "insertion", "paragraph", "presentation", "strong", "subscript", "superscript"]) ? "" : S(e, t)
+                    return w(e, ["caption", "code", "deletion", "emphasis", "generic", "insertion", "paragraph", "presentation", "strong", "subscript", "superscript"]) ? "" : R(e, t)
                 }
                 var F = r(2461),
                     N = r(6961),
                     B = r.n(N);
 
                 function L(e) {
                     return e.replace(/</g, "&lt;").replace(/>/g, "&gt;")
@@ -705,15 +705,15 @@
                             var t, r;
                             e = JSON.parse(null == (t = process) || null == (r = t.env) ? void 0 : r.COLORS)
                         } catch (e) {}
                         return "boolean" == typeof e ? e : "undefined" != typeof process && void 0 !== process.versions && void 0 !== process.versions.node
                     },
                     {
                         DOMCollection: ue
-                    } = n.Gr,
+                    } = n.plugins,
                     se = 1,
                     ce = 8;
 
                 function de(e) {
                     return e.nodeType !== ce && (e.nodeType !== se || !e.matches(me().defaultIgnore))
                 }
 
@@ -870,15 +870,15 @@
                     const r = e.test(t);
                     return e.global && 0 !== e.lastIndex && (console.warn("To match all elements we had to reset the lastIndex of the RegExp because the global flag is enabled. We encourage to remove the global flag from the RegExp."), e.lastIndex = 0), r
                 }
 
                 function je(e) {
                     return e.matches("input[type=submit], input[type=button], input[type=reset]") ? e.value : Array.from(e.childNodes).filter((e => e.nodeType === re && Boolean(e.textContent))).map((e => e.textContent)).join("")
                 }
-                const Re = function(e) {
+                const Se = function(e) {
                     function t(e) {
                         let {
                             attributes: t = []
                         } = e;
                         return t.length
                     }
 
@@ -919,22 +919,22 @@
                         } = e, {
                             specificity: n
                         } = t;
                         return n - r
                     }))
                 }(F.Qv);
 
-                function Se(e) {
+                function Re(e) {
                     return !0 === e.hidden || ("true" === e.getAttribute("aria-hidden") || "none" === e.ownerDocument.defaultView.getComputedStyle(e).display)
                 }
 
                 function _e(e, t) {
                     void 0 === t && (t = {});
                     const {
-                        isSubtreeInaccessible: r = Se
+                        isSubtreeInaccessible: r = Re
                     } = t;
                     if ("hidden" === e.ownerDocument.defaultView.getComputedStyle(e).visibility) return !0;
                     let n = e;
                     for (; n;) {
                         if (r(n)) return !0;
                         n = n.parentElement
                     }
@@ -942,24 +942,24 @@
                 }
 
                 function Ae(e) {
                     for (const {
                             match: t,
                             roles: r
                         }
-                        of Re)
+                        of Se)
                         if (t(e)) return [...r];
                     return []
                 }
 
-                function Te(e, t) {
+                function Me(e, t) {
                     const r = e.getAttribute(t);
                     return "true" === r || "false" !== r && void 0
                 }
-                const Me = xe();
+                const Te = xe();
 
                 function Ie(e) {
                     return new RegExp(function(e) {
                         return e.replace(/[.*+\-?^${}()|[\]\\]/g, "\\$&")
                     }(e.toLowerCase()), "i")
                 }
 
@@ -1009,19 +1009,19 @@
                     if (Fe("LabelText", r, i)) return ke("LabelText", e, i, {
                         variant: t
                     });
                     const l = e.getAttribute("placeholder");
                     if (Fe("PlaceholderText", r, l)) return ke("PlaceholderText", e, l, {
                         variant: t
                     });
-                    const u = Me(je(e));
+                    const u = Te(je(e));
                     if (Fe("Text", r, u)) return ke("Text", e, u, {
                         variant: t
                     });
-                    if (Fe("DisplayValue", r, e.value)) return ke("DisplayValue", e, Me(e.value), {
+                    if (Fe("DisplayValue", r, e.value)) return ke("DisplayValue", e, Te(e.value), {
                         variant: t
                     });
                     const s = e.getAttribute("alt");
                     if (Fe("AltText", r, s)) return ke("AltText", e, s, {
                         variant: t
                     });
                     const c = e.getAttribute("title");
@@ -1069,22 +1069,17 @@
                                     unstable_advanceTimersWrapper: e
                                 } = me();
                                 for (g(); !f;) {
                                     if (!ne()) {
                                         const e = new Error("Changed from using fake timers to real timers while using waitFor. This is not allowed and will result in very strange behavior. Please ensure you're awaiting all async things your test is doing before changing to real timers. For more info, please go to https://github.com/testing-library/dom-testing-library/issues/830");
                                         return o || Be(e, a), void s(e)
                                     }
-                                    if (e((() => {
+                                    if (await e((async () => {
                                             jest.advanceTimersByTime(i)
-                                        })), g(), f) break;
-                                    await e((async () => {
-                                        await new Promise((e => {
-                                            setTimeout(e, 0), jest.advanceTimersByTime(0)
-                                        }))
-                                    }))
+                                        })), g(), f) break
                                 }
                             } else {
                                 try {
                                     ie(r)
                                 } catch (e) {
                                     return void s(e)
                                 }
@@ -1373,16 +1368,16 @@
                     gt = Ve(ht, ht.name, "queryAll"),
                     [Pt, Ct, wt, qt, xt] = Ge(ht, ((e, t) => "Found multiple elements with the display value: " + t + "."), ((e, t) => "Unable to find an element with the display value: " + t + ".")),
                     Et = /^(img|input|area|.+-.+)$/i,
                     Ot = function(e, t, r) {
                         return void 0 === r && (r = {}), ie(e), De("alt", e, t, r).filter((e => Et.test(e.tagName)))
                     },
                     jt = Ve(Ot, Ot.name, "queryAll"),
-                    [Rt, St, _t, At, Tt] = Ge(Ot, ((e, t) => "Found multiple elements with the alt text: " + t), ((e, t) => "Unable to find an element with the alt text: " + t)),
-                    Mt = function(e, t, r) {
+                    [St, Rt, _t, At, Mt] = Ge(Ot, ((e, t) => "Found multiple elements with the alt text: " + t), ((e, t) => "Unable to find an element with the alt text: " + t)),
+                    Tt = function(e, t, r) {
                         let {
                             exact: n = !0,
                             collapseWhitespace: o,
                             trim: a,
                             normalizer: i
                         } = void 0 === r ? {} : r;
                         ie(e);
@@ -1393,16 +1388,16 @@
                                 normalizer: i
                             });
                         return Array.from(e.querySelectorAll("[title], svg > title")).filter((e => l(e.getAttribute("title"), e, t, u) || (e => {
                             var t;
                             return "title" === e.tagName.toLowerCase() && "svg" === (null == (t = e.parentElement) ? void 0 : t.tagName.toLowerCase())
                         })(e) && l(je(e), e, t, u)))
                     },
-                    It = Ve(Mt, Mt.name, "queryAll"),
-                    [kt, Ft, Nt, Bt, Lt] = Ge(Mt, ((e, t) => "Found multiple elements with the title: " + t + "."), ((e, t) => "Unable to find an element with the title: " + t + ".")),
+                    It = Ve(Tt, Tt.name, "queryAll"),
+                    [kt, Ft, Nt, Bt, Lt] = Ge(Tt, ((e, t) => "Found multiple elements with the title: " + t + "."), ((e, t) => "Unable to find an element with the title: " + t + ".")),
                     Ut = function(e, t, r) {
                         let {
                             hidden: n = me().defaultHidden,
                             name: o,
                             description: a,
                             queryFallbacks: i = !1,
                             selected: l,
@@ -1427,18 +1422,18 @@
                         if (void 0 !== d && void 0 === (null == (w = F.uJ.get(t)) ? void 0 : w.props["aria-current"])) throw new Error('"aria-current" is not supported on role "' + t + '".');
                         if (void 0 !== p && "heading" !== t) throw new Error('Role "' + t + '" cannot have "level" property.');
                         if (void 0 !== b && void 0 === (null == (q = F.uJ.get(t)) ? void 0 : q.props["aria-valuenow"])) throw new Error('"aria-valuenow" is not supported on role "' + t + '".');
                         if (void 0 !== y && void 0 === (null == (x = F.uJ.get(t)) ? void 0 : x.props["aria-valuemax"])) throw new Error('"aria-valuemax" is not supported on role "' + t + '".');
                         if (void 0 !== m && void 0 === (null == (E = F.uJ.get(t)) ? void 0 : E.props["aria-valuemin"])) throw new Error('"aria-valuemin" is not supported on role "' + t + '".');
                         if (void 0 !== v && void 0 === (null == (O = F.uJ.get(t)) ? void 0 : O.props["aria-valuetext"])) throw new Error('"aria-valuetext" is not supported on role "' + t + '".');
                         if (void 0 !== f && void 0 === (null == (j = F.uJ.get(t)) ? void 0 : j.props["aria-expanded"])) throw new Error('"aria-expanded" is not supported on role "' + t + '".');
-                        const R = new WeakMap;
+                        const S = new WeakMap;
 
-                        function S(e) {
-                            return R.has(e) || R.set(e, Se(e)), R.get(e)
+                        function R(e) {
+                            return S.has(e) || S.set(e, Re(e)), S.get(e)
                         }
                         return Array.from(e.querySelectorAll(function(e) {
                             var t;
                             const r = '*[role~="' + e + '"]',
                                 n = null != (t = F.UN.get(e)) ? t : new Set,
                                 o = new Set(Array.from(n).map((e => {
                                     let {
@@ -1453,31 +1448,31 @@
                                 if (i) return r.split(" ").filter(Boolean).some((e => e === t));
                                 const [n] = r.split(" ");
                                 return n === t
                             }
                             return Ae(e).some((e => e === t))
                         })).filter((e => {
                             if (void 0 !== l) return l === function(e) {
-                                return "OPTION" === e.tagName ? e.selected : Te(e, "aria-selected")
+                                return "OPTION" === e.tagName ? e.selected : Me(e, "aria-selected")
                             }(e);
                             if (void 0 !== u) return u === function(e) {
                                 return "true" === e.getAttribute("aria-busy")
                             }(e);
                             if (void 0 !== s) return s === function(e) {
-                                if (!("indeterminate" in e) || !e.indeterminate) return "checked" in e ? e.checked : Te(e, "aria-checked")
+                                if (!("indeterminate" in e) || !e.indeterminate) return "checked" in e ? e.checked : Me(e, "aria-checked")
                             }(e);
                             if (void 0 !== c) return c === function(e) {
-                                return Te(e, "aria-pressed")
+                                return Me(e, "aria-pressed")
                             }(e);
                             if (void 0 !== d) return d === function(e) {
                                 var t, r;
-                                return null != (t = null != (r = Te(e, "aria-current")) ? r : e.getAttribute("aria-current")) && t
+                                return null != (t = null != (r = Me(e, "aria-current")) ? r : e.getAttribute("aria-current")) && t
                             }(e);
                             if (void 0 !== f) return f === function(e) {
-                                return Te(e, "aria-expanded")
+                                return Me(e, "aria-expanded")
                             }(e);
                             if (void 0 !== p) return p === function(e) {
                                 return e.getAttribute("aria-level") && Number(e.getAttribute("aria-level")) || {
                                     H1: 1,
                                     H2: 2,
                                     H3: 3,
                                     H4: 4,
@@ -1504,15 +1499,15 @@
                             }
                             return !0
                         })).filter((e => void 0 === o || qe(k(e, {
                             computedStyleSupportsPseudoElements: me().computedStyleSupportsPseudoElements
                         }), e, o, (e => e)))).filter((e => void 0 === a || qe(I(e, {
                             computedStyleSupportsPseudoElements: me().computedStyleSupportsPseudoElements
                         }), e, a, (e => e)))).filter((e => !1 !== n || !1 === _e(e, {
-                            isSubtreeInaccessible: S
+                            isSubtreeInaccessible: R
                         })))
                     },
                     Dt = e => {
                         let t = "";
                         return t = void 0 === e ? "" : "string" == typeof e ? ' and name "' + e + '"' : " and name `" + e + "`", t
                     },
                     Ht = Ve(Ut, Ut.name, "queryAll"),
@@ -1609,20 +1604,20 @@
                     findByText: vt,
                     queryByDisplayValue: Pt,
                     queryAllByDisplayValue: gt,
                     getByDisplayValue: wt,
                     getAllByDisplayValue: Ct,
                     findAllByDisplayValue: qt,
                     findByDisplayValue: xt,
-                    queryByAltText: Rt,
+                    queryByAltText: St,
                     queryAllByAltText: jt,
                     getByAltText: _t,
-                    getAllByAltText: St,
+                    getAllByAltText: Rt,
                     findAllByAltText: At,
-                    findByAltText: Tt,
+                    findByAltText: Mt,
                     queryByTitle: kt,
                     queryAllByTitle: It,
                     getByTitle: Nt,
                     getAllByTitle: Ft,
                     findAllByTitle: Bt,
                     findByTitle: Lt,
                     queryByRole: $t,
@@ -3824,20 +3819,20 @@
                     C = H(r(8373)),
                     w = H(r(711)),
                     q = H(r(3612)),
                     x = H(r(6909)),
                     E = H(r(6361)),
                     O = H(r(745)),
                     j = H(r(6871)),
-                    R = H(r(3035)),
-                    S = H(r(6498)),
+                    S = H(r(3035)),
+                    R = H(r(6498)),
                     _ = H(r(7364)),
                     A = H(r(6589)),
-                    T = H(r(4216)),
-                    M = H(r(386)),
+                    M = H(r(4216)),
+                    T = H(r(386)),
                     I = H(r(2554)),
                     k = H(r(5885)),
                     F = H(r(2186)),
                     N = H(r(805)),
                     B = H(r(3135)),
                     L = H(r(4174)),
                     U = H(r(5903)),
@@ -3870,20 +3865,20 @@
                     ["doc-epilogue", C.default],
                     ["doc-errata", w.default],
                     ["doc-example", q.default],
                     ["doc-footnote", x.default],
                     ["doc-foreword", E.default],
                     ["doc-glossary", O.default],
                     ["doc-glossref", j.default],
-                    ["doc-index", R.default],
-                    ["doc-introduction", S.default],
+                    ["doc-index", S.default],
+                    ["doc-introduction", R.default],
                     ["doc-noteref", _.default],
                     ["doc-notice", A.default],
-                    ["doc-pagebreak", T.default],
-                    ["doc-pagelist", M.default],
+                    ["doc-pagebreak", M.default],
+                    ["doc-pagelist", T.default],
                     ["doc-part", I.default],
                     ["doc-preface", k.default],
                     ["doc-prologue", F.default],
                     ["doc-pullquote", N.default],
                     ["doc-qna", B.default],
                     ["doc-subtitle", L.default],
                     ["doc-tip", U.default],
@@ -3938,20 +3933,20 @@
                     C = Ae(r(2686)),
                     w = Ae(r(3477)),
                     q = Ae(r(7089)),
                     x = Ae(r(949)),
                     E = Ae(r(5e3)),
                     O = Ae(r(3204)),
                     j = Ae(r(6481)),
-                    R = Ae(r(9782)),
-                    S = Ae(r(6974)),
+                    S = Ae(r(9782)),
+                    R = Ae(r(6974)),
                     _ = Ae(r(8458)),
                     A = Ae(r(2589)),
-                    T = Ae(r(4046)),
-                    M = Ae(r(8186)),
+                    M = Ae(r(4046)),
+                    T = Ae(r(8186)),
                     I = Ae(r(2339)),
                     k = Ae(r(5448)),
                     F = Ae(r(7297)),
                     N = Ae(r(2573)),
                     B = Ae(r(397)),
                     L = Ae(r(7116)),
                     U = Ae(r(6718)),
@@ -3992,24 +3987,24 @@
                     Ce = Ae(r(3193)),
                     we = Ae(r(4665)),
                     qe = Ae(r(221)),
                     xe = Ae(r(5313)),
                     Ee = Ae(r(1777)),
                     Oe = Ae(r(3316)),
                     je = Ae(r(9304)),
-                    Re = Ae(r(3538)),
-                    Se = Ae(r(5627)),
+                    Se = Ae(r(3538)),
+                    Re = Ae(r(5627)),
                     _e = Ae(r(8425));
 
                 function Ae(e) {
                     return e && e.__esModule ? e : {
                         default: e
                     }
                 }
-                var Te = [
+                var Me = [
                     ["alert", n.default],
                     ["alertdialog", o.default],
                     ["application", a.default],
                     ["article", i.default],
                     ["banner", l.default],
                     ["blockquote", u.default],
                     ["button", s.default],
@@ -4027,20 +4022,20 @@
                     ["directory", C.default],
                     ["document", w.default],
                     ["emphasis", q.default],
                     ["feed", x.default],
                     ["figure", E.default],
                     ["form", O.default],
                     ["generic", j.default],
-                    ["grid", R.default],
-                    ["gridcell", S.default],
+                    ["grid", S.default],
+                    ["gridcell", R.default],
                     ["group", _.default],
                     ["heading", A.default],
-                    ["img", T.default],
-                    ["insertion", M.default],
+                    ["img", M.default],
+                    ["insertion", T.default],
                     ["link", I.default],
                     ["list", k.default],
                     ["listbox", F.default],
                     ["listitem", N.default],
                     ["log", B.default],
                     ["main", L.default],
                     ["marquee", U.default],
@@ -4081,19 +4076,19 @@
                     ["tabpanel", Ce.default],
                     ["term", we.default],
                     ["textbox", qe.default],
                     ["time", xe.default],
                     ["timer", Ee.default],
                     ["toolbar", Oe.default],
                     ["tooltip", je.default],
-                    ["tree", Re.default],
-                    ["treegrid", Se.default],
+                    ["tree", Se.default],
+                    ["treegrid", Re.default],
                     ["treeitem", _e.default]
                 ];
-                t.default = Te
+                t.default = Me
             },
             481: (e, t) => {
                 "use strict";
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 }), t.default = void 0;
                 t.default = {
@@ -8898,14 +8893,22 @@
                                     done: !0
                                 }
                             }
                         };
                     return r
                 }
             },
+            6894: (e, t, r) => {
+                "use strict";
+                var n = r(1924)("ArrayBuffer.prototype.byteLength", !0),
+                    o = r(635);
+                e.exports = function(e) {
+                    return o(e) ? n ? n(e) : e.byteLength : NaN
+                }
+            },
             1924: (e, t, r) => {
                 "use strict";
                 var n = r(210),
                     o = r(5559),
                     a = o(n("String.prototype.indexOf"));
                 e.exports = function(e, t) {
                     var r = n(e, !!t);
@@ -8957,31 +8960,29 @@
                     f = r(8923),
                     b = r(8420),
                     m = r(2579),
                     y = r(2215),
                     v = r(3679),
                     h = r(3483),
                     g = r(6430),
-                    P = o("ArrayBuffer.prototype.byteLength", !0) || function(e) {
-                        return e.byteLength
-                    },
+                    P = r(6894),
                     C = o("SharedArrayBuffer.prototype.byteLength", !0),
                     w = o("Date.prototype.getTime"),
                     q = Object.getPrototypeOf,
                     x = o("Object.prototype.toString"),
                     E = i("%Set%", !0),
                     O = o("Map.prototype.has", !0),
                     j = o("Map.prototype.get", !0),
-                    R = o("Map.prototype.size", !0),
-                    S = o("Set.prototype.add", !0),
+                    S = o("Map.prototype.size", !0),
+                    R = o("Set.prototype.add", !0),
                     _ = o("Set.prototype.delete", !0),
                     A = o("Set.prototype.has", !0),
-                    T = o("Set.prototype.size", !0);
+                    M = o("Set.prototype.size", !0);
 
-                function M(e, t, r, n) {
+                function T(e, t, r, n) {
                     for (var o, a = l(e);
                         (o = a.next()) && !o.done;)
                         if (B(t, o.value, r, n)) return _(e, o.value), !0;
                     return !1
                 }
 
                 function I(e) {
@@ -9068,51 +9069,51 @@
                             for (K.sort(), Y.sort(), i = K.length - 1; i >= 0; i--)
                                 if (K[i] != Y[i]) return !1;
                             for (i = K.length - 1; i >= 0; i--)
                                 if (!B(e[u = K[i]], t[u], r, o)) return !1;
                             var Q = h(e),
                                 Z = h(t);
                             return Q === Z && ("Set" === Q || "Set" === Z ? function(e, t, r, n) {
-                                if (T(e) !== T(t)) return !1;
+                                if (M(e) !== M(t)) return !1;
                                 for (var o, a, i, u = l(e), s = l(t);
                                     (o = u.next()) && !o.done;)
-                                    if (o.value && "object" == typeof o.value) i || (i = new E), S(i, o.value);
+                                    if (o.value && "object" == typeof o.value) i || (i = new E), R(i, o.value);
                                     else if (!A(t, o.value)) {
                                     if (r.strict) return !1;
                                     if (!F(e, t, o.value)) return !1;
-                                    i || (i = new E), S(i, o.value)
+                                    i || (i = new E), R(i, o.value)
                                 }
                                 if (i) {
                                     for (;
                                         (a = s.next()) && !a.done;)
                                         if (a.value && "object" == typeof a.value) {
-                                            if (!M(i, a.value, r.strict, n)) return !1
-                                        } else if (!r.strict && !A(e, a.value) && !M(i, a.value, r.strict, n)) return !1;
-                                    return 0 === T(i)
+                                            if (!T(i, a.value, r.strict, n)) return !1
+                                        } else if (!r.strict && !A(e, a.value) && !T(i, a.value, r.strict, n)) return !1;
+                                    return 0 === M(i)
                                 }
                                 return !0
                             }(e, t, r, o) : "Map" !== Q || function(e, t, r, o) {
-                                if (R(e) !== R(t)) return !1;
+                                if (S(e) !== S(t)) return !1;
                                 for (var a, i, u, s, c, d, p = l(e), f = l(t);
                                     (a = p.next()) && !a.done;)
-                                    if (s = a.value[0], c = a.value[1], s && "object" == typeof s) u || (u = new E), S(u, s);
+                                    if (s = a.value[0], c = a.value[1], s && "object" == typeof s) u || (u = new E), R(u, s);
                                     else if (void 0 === (d = j(t, s)) && !O(t, s) || !B(c, d, r, o)) {
                                     if (r.strict) return !1;
                                     if (!k(e, t, s, c, r, o)) return !1;
-                                    u || (u = new E), S(u, s)
+                                    u || (u = new E), R(u, s)
                                 }
                                 if (u) {
                                     for (;
                                         (i = f.next()) && !i.done;)
                                         if (s = i.value[0], d = i.value[1], s && "object" == typeof s) {
                                             if (!N(u, e, s, d, r, o)) return !1
                                         } else if (!(r.strict || e.has(s) && B(j(e, s), d, r, o) || N(u, e, s, d, n({}, r, {
                                             strict: !1
                                         }), o))) return !1;
-                                    return 0 === T(u)
+                                    return 0 === M(u)
                                 }
                                 return !0
                             }(e, t, r, o))
                         }(e, t, i, o)
                 }
 
                 function L(e) {
@@ -9244,29 +9245,30 @@
                                 return u(arguments, "callee").get
                             } catch (e) {
                                 return s
                             }
                         }
                     }() : s,
                     d = r(1405)(),
-                    p = Object.getPrototypeOf || function(e) {
+                    p = r(8185)(),
+                    f = Object.getPrototypeOf || (p ? function(e) {
                         return e.__proto__
-                    },
-                    f = {},
-                    b = "undefined" == typeof Uint8Array ? n : p(Uint8Array),
-                    m = {
+                    } : null),
+                    b = {},
+                    m = "undefined" != typeof Uint8Array && f ? f(Uint8Array) : n,
+                    y = {
                         "%AggregateError%": "undefined" == typeof AggregateError ? n : AggregateError,
                         "%Array%": Array,
                         "%ArrayBuffer%": "undefined" == typeof ArrayBuffer ? n : ArrayBuffer,
-                        "%ArrayIteratorPrototype%": d ? p([][Symbol.iterator]()) : n,
+                        "%ArrayIteratorPrototype%": d && f ? f([][Symbol.iterator]()) : n,
                         "%AsyncFromSyncIteratorPrototype%": n,
-                        "%AsyncFunction%": f,
-                        "%AsyncGenerator%": f,
-                        "%AsyncGeneratorFunction%": f,
-                        "%AsyncIteratorPrototype%": f,
+                        "%AsyncFunction%": b,
+                        "%AsyncGenerator%": b,
+                        "%AsyncGeneratorFunction%": b,
+                        "%AsyncIteratorPrototype%": b,
                         "%Atomics%": "undefined" == typeof Atomics ? n : Atomics,
                         "%BigInt%": "undefined" == typeof BigInt ? n : BigInt,
                         "%BigInt64Array%": "undefined" == typeof BigInt64Array ? n : BigInt64Array,
                         "%BigUint64Array%": "undefined" == typeof BigUint64Array ? n : BigUint64Array,
                         "%Boolean%": Boolean,
                         "%DataView%": "undefined" == typeof DataView ? n : DataView,
                         "%Date%": Date,
@@ -9277,75 +9279,75 @@
                         "%Error%": Error,
                         "%eval%": eval,
                         "%EvalError%": EvalError,
                         "%Float32Array%": "undefined" == typeof Float32Array ? n : Float32Array,
                         "%Float64Array%": "undefined" == typeof Float64Array ? n : Float64Array,
                         "%FinalizationRegistry%": "undefined" == typeof FinalizationRegistry ? n : FinalizationRegistry,
                         "%Function%": a,
-                        "%GeneratorFunction%": f,
+                        "%GeneratorFunction%": b,
                         "%Int8Array%": "undefined" == typeof Int8Array ? n : Int8Array,
                         "%Int16Array%": "undefined" == typeof Int16Array ? n : Int16Array,
                         "%Int32Array%": "undefined" == typeof Int32Array ? n : Int32Array,
                         "%isFinite%": isFinite,
                         "%isNaN%": isNaN,
-                        "%IteratorPrototype%": d ? p(p([][Symbol.iterator]())) : n,
+                        "%IteratorPrototype%": d && f ? f(f([][Symbol.iterator]())) : n,
                         "%JSON%": "object" == typeof JSON ? JSON : n,
                         "%Map%": "undefined" == typeof Map ? n : Map,
-                        "%MapIteratorPrototype%": "undefined" != typeof Map && d ? p((new Map)[Symbol.iterator]()) : n,
+                        "%MapIteratorPrototype%": "undefined" != typeof Map && d && f ? f((new Map)[Symbol.iterator]()) : n,
                         "%Math%": Math,
                         "%Number%": Number,
                         "%Object%": Object,
                         "%parseFloat%": parseFloat,
                         "%parseInt%": parseInt,
                         "%Promise%": "undefined" == typeof Promise ? n : Promise,
                         "%Proxy%": "undefined" == typeof Proxy ? n : Proxy,
                         "%RangeError%": RangeError,
                         "%ReferenceError%": ReferenceError,
                         "%Reflect%": "undefined" == typeof Reflect ? n : Reflect,
                         "%RegExp%": RegExp,
                         "%Set%": "undefined" == typeof Set ? n : Set,
-                        "%SetIteratorPrototype%": "undefined" != typeof Set && d ? p((new Set)[Symbol.iterator]()) : n,
+                        "%SetIteratorPrototype%": "undefined" != typeof Set && d && f ? f((new Set)[Symbol.iterator]()) : n,
                         "%SharedArrayBuffer%": "undefined" == typeof SharedArrayBuffer ? n : SharedArrayBuffer,
                         "%String%": String,
-                        "%StringIteratorPrototype%": d ? p("" [Symbol.iterator]()) : n,
+                        "%StringIteratorPrototype%": d && f ? f("" [Symbol.iterator]()) : n,
                         "%Symbol%": d ? Symbol : n,
                         "%SyntaxError%": o,
                         "%ThrowTypeError%": c,
-                        "%TypedArray%": b,
+                        "%TypedArray%": m,
                         "%TypeError%": i,
                         "%Uint8Array%": "undefined" == typeof Uint8Array ? n : Uint8Array,
                         "%Uint8ClampedArray%": "undefined" == typeof Uint8ClampedArray ? n : Uint8ClampedArray,
                         "%Uint16Array%": "undefined" == typeof Uint16Array ? n : Uint16Array,
                         "%Uint32Array%": "undefined" == typeof Uint32Array ? n : Uint32Array,
                         "%URIError%": URIError,
                         "%WeakMap%": "undefined" == typeof WeakMap ? n : WeakMap,
                         "%WeakRef%": "undefined" == typeof WeakRef ? n : WeakRef,
                         "%WeakSet%": "undefined" == typeof WeakSet ? n : WeakSet
                     };
-                try {
+                if (f) try {
                     null.error
                 } catch (e) {
-                    var y = p(p(e));
-                    m["%Error.prototype%"] = y
+                    var v = f(f(e));
+                    y["%Error.prototype%"] = v
                 }
-                var v = function e(t) {
+                var h = function e(t) {
                         var r;
                         if ("%AsyncFunction%" === t) r = l("async function () {}");
                         else if ("%GeneratorFunction%" === t) r = l("function* () {}");
                         else if ("%AsyncGeneratorFunction%" === t) r = l("async function* () {}");
                         else if ("%AsyncGenerator%" === t) {
                             var n = e("%AsyncGeneratorFunction%");
                             n && (r = n.prototype)
                         } else if ("%AsyncIteratorPrototype%" === t) {
                             var o = e("%AsyncGenerator%");
-                            o && (r = p(o.prototype))
+                            o && f && (r = f(o.prototype))
                         }
-                        return m[t] = r, r
+                        return y[t] = r, r
                     },
-                    h = {
+                    g = {
                         "%ArrayBufferPrototype%": ["ArrayBuffer", "prototype"],
                         "%ArrayPrototype%": ["Array", "prototype"],
                         "%ArrayProto_entries%": ["Array", "prototype", "entries"],
                         "%ArrayProto_forEach%": ["Array", "prototype", "forEach"],
                         "%ArrayProto_keys%": ["Array", "prototype", "keys"],
                         "%ArrayProto_values%": ["Array", "prototype", "values"],
                         "%AsyncFunctionPrototype%": ["AsyncFunction", "prototype"],
@@ -9390,73 +9392,73 @@
                         "%Uint8ClampedArrayPrototype%": ["Uint8ClampedArray", "prototype"],
                         "%Uint16ArrayPrototype%": ["Uint16Array", "prototype"],
                         "%Uint32ArrayPrototype%": ["Uint32Array", "prototype"],
                         "%URIErrorPrototype%": ["URIError", "prototype"],
                         "%WeakMapPrototype%": ["WeakMap", "prototype"],
                         "%WeakSetPrototype%": ["WeakSet", "prototype"]
                     },
-                    g = r(8612),
-                    P = r(7642),
-                    C = g.call(Function.call, Array.prototype.concat),
-                    w = g.call(Function.apply, Array.prototype.splice),
-                    q = g.call(Function.call, String.prototype.replace),
-                    x = g.call(Function.call, String.prototype.slice),
-                    E = g.call(Function.call, RegExp.prototype.exec),
-                    O = /[^%.[\]]+|\[(?:(-?\d+(?:\.\d+)?)|(["'])((?:(?!\2)[^\\]|\\.)*?)\2)\]|(?=(?:\.|\[\])(?:\.|\[\]|%$))/g,
-                    j = /\\(\\)?/g,
+                    P = r(8612),
+                    C = r(7642),
+                    w = P.call(Function.call, Array.prototype.concat),
+                    q = P.call(Function.apply, Array.prototype.splice),
+                    x = P.call(Function.call, String.prototype.replace),
+                    E = P.call(Function.call, String.prototype.slice),
+                    O = P.call(Function.call, RegExp.prototype.exec),
+                    j = /[^%.[\]]+|\[(?:(-?\d+(?:\.\d+)?)|(["'])((?:(?!\2)[^\\]|\\.)*?)\2)\]|(?=(?:\.|\[\])(?:\.|\[\]|%$))/g,
+                    S = /\\(\\)?/g,
                     R = function(e, t) {
                         var r, n = e;
-                        if (P(h, n) && (n = "%" + (r = h[n])[0] + "%"), P(m, n)) {
-                            var a = m[n];
-                            if (a === f && (a = v(n)), void 0 === a && !t) throw new i("intrinsic " + e + " exists, but is not available. Please file an issue!");
+                        if (C(g, n) && (n = "%" + (r = g[n])[0] + "%"), C(y, n)) {
+                            var a = y[n];
+                            if (a === b && (a = h(n)), void 0 === a && !t) throw new i("intrinsic " + e + " exists, but is not available. Please file an issue!");
                             return {
                                 alias: r,
                                 name: n,
                                 value: a
                             }
                         }
                         throw new o("intrinsic " + e + " does not exist!")
                     };
                 e.exports = function(e, t) {
                     if ("string" != typeof e || 0 === e.length) throw new i("intrinsic name must be a non-empty string");
                     if (arguments.length > 1 && "boolean" != typeof t) throw new i('"allowMissing" argument must be a boolean');
-                    if (null === E(/^%?[^%]*%?$/, e)) throw new o("`%` may not be present anywhere but at the beginning and end of the intrinsic name");
+                    if (null === O(/^%?[^%]*%?$/, e)) throw new o("`%` may not be present anywhere but at the beginning and end of the intrinsic name");
                     var r = function(e) {
-                            var t = x(e, 0, 1),
-                                r = x(e, -1);
+                            var t = E(e, 0, 1),
+                                r = E(e, -1);
                             if ("%" === t && "%" !== r) throw new o("invalid intrinsic syntax, expected closing `%`");
                             if ("%" === r && "%" !== t) throw new o("invalid intrinsic syntax, expected opening `%`");
                             var n = [];
-                            return q(e, O, (function(e, t, r, o) {
-                                n[n.length] = r ? q(o, j, "$1") : t || e
+                            return x(e, j, (function(e, t, r, o) {
+                                n[n.length] = r ? x(o, S, "$1") : t || e
                             })), n
                         }(e),
                         n = r.length > 0 ? r[0] : "",
                         a = R("%" + n + "%", t),
                         l = a.name,
                         s = a.value,
                         c = !1,
                         d = a.alias;
-                    d && (n = d[0], w(r, C([0, 1], d)));
+                    d && (n = d[0], q(r, w([0, 1], d)));
                     for (var p = 1, f = !0; p < r.length; p += 1) {
                         var b = r[p],
-                            y = x(b, 0, 1),
-                            v = x(b, -1);
-                        if (('"' === y || "'" === y || "`" === y || '"' === v || "'" === v || "`" === v) && y !== v) throw new o("property names with quotes must have matching quotes");
-                        if ("constructor" !== b && f || (c = !0), P(m, l = "%" + (n += "." + b) + "%")) s = m[l];
+                            m = E(b, 0, 1),
+                            v = E(b, -1);
+                        if (('"' === m || "'" === m || "`" === m || '"' === v || "'" === v || "`" === v) && m !== v) throw new o("property names with quotes must have matching quotes");
+                        if ("constructor" !== b && f || (c = !0), C(y, l = "%" + (n += "." + b) + "%")) s = y[l];
                         else if (null != s) {
                             if (!(b in s)) {
                                 if (!t) throw new i("base intrinsic for " + e + " exists, but the property is not available.");
                                 return
                             }
                             if (u && p + 1 >= r.length) {
                                 var h = u(s, b);
                                 s = (f = !!h) && "get" in h && !("originalValue" in h.get) ? h.get : s[b]
-                            } else f = P(s, b), s = s[b];
-                            f && !c && (m[l] = s)
+                            } else f = C(s, b), s = s[b];
+                            f && !c && (y[l] = s)
                         }
                     }
                     return s
                 }
             },
             7296: (e, t, r) => {
                 "use strict";
@@ -9495,14 +9497,29 @@
                             value: 1
                         }).length
                     } catch (e) {
                         return !0
                     }
                 }, e.exports = o
             },
+            8185: e => {
+                "use strict";
+                var t = {
+                        foo: {}
+                    },
+                    r = Object;
+                e.exports = function() {
+                    return {
+                        __proto__: t
+                    }.foo === t.foo && !({
+                            __proto__: null
+                        }
+                        instanceof r)
+                }
+            },
             1405: (e, t, r) => {
                 "use strict";
                 var n = "undefined" != typeof Symbol && Symbol,
                     o = r(5419);
                 e.exports = function() {
                     return "function" == typeof n && "function" == typeof Symbol && "symbol" == typeof n("foo") && "symbol" == typeof Symbol("bar") && o()
                 }
@@ -10186,20 +10203,20 @@
                     C = String.prototype.toLowerCase,
                     w = RegExp.prototype.test,
                     q = Array.prototype.concat,
                     x = Array.prototype.join,
                     E = Array.prototype.slice,
                     O = Math.floor,
                     j = "function" == typeof BigInt ? BigInt.prototype.valueOf : null,
-                    R = Object.getOwnPropertySymbols,
-                    S = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? Symbol.prototype.toString : null,
+                    S = Object.getOwnPropertySymbols,
+                    R = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? Symbol.prototype.toString : null,
                     _ = "function" == typeof Symbol && "object" == typeof Symbol.iterator,
                     A = "function" == typeof Symbol && Symbol.toStringTag && (Symbol.toStringTag, 1) ? Symbol.toStringTag : null,
-                    T = Object.prototype.propertyIsEnumerable,
-                    M = ("function" == typeof Reflect ? Reflect.getPrototypeOf : Object.getPrototypeOf) || ([].__proto__ === Array.prototype ? function(e) {
+                    M = Object.prototype.propertyIsEnumerable,
+                    T = ("function" == typeof Reflect ? Reflect.getPrototypeOf : Object.getPrototypeOf) || ([].__proto__ === Array.prototype ? function(e) {
                         return e.__proto__
                     } : null);
 
                 function I(e, t) {
                     if (e === 1 / 0 || e === -1 / 0 || e != e || e && e > -1e3 && e < 1e3 || w.call(/e/, t)) return t;
                     var r = /[0-9](?=(?:[0-9]{3})+(?![0-9]))/g;
                     if ("number" == typeof e) {
@@ -10232,17 +10249,17 @@
                 function D(e) {
                     return !("[object RegExp]" !== z(e) || A && "object" == typeof e && A in e)
                 }
 
                 function H(e) {
                     if (_) return e && "object" == typeof e && e instanceof Symbol;
                     if ("symbol" == typeof e) return !0;
-                    if (!e || "object" != typeof e || !S) return !1;
+                    if (!e || "object" != typeof e || !R) return !1;
                     try {
-                        return S.call(e), !0
+                        return R.call(e), !0
                     } catch (e) {}
                     return !1
                 }
                 e.exports = function e(t, r, n, o) {
                     var l = r || {};
                     if (W(l, "quoteStyle") && "single" !== l.quoteStyle && "double" !== l.quoteStyle) throw new TypeError('option "quoteStyle" must be "single" or "double"');
                     if (W(l, "maxStringLength") && ("number" == typeof l.maxStringLength ? l.maxStringLength < 0 && l.maxStringLength !== 1 / 0 : null !== l.maxStringLength)) throw new TypeError('option "maxStringLength", if provided, must be a positive integer, Infinity, or `null`');
@@ -10262,15 +10279,15 @@
                     }
                     if ("bigint" == typeof t) {
                         var w = String(t) + "n";
                         return m ? I(t, w) : w
                     }
                     var O = void 0 === l.depth ? 5 : l.depth;
                     if (void 0 === n && (n = 0), n >= O && O > 0 && "object" == typeof t) return U(t) ? "[Array]" : "[Object]";
-                    var R, F = function(e, t) {
+                    var S, F = function(e, t) {
                         var r;
                         if ("\t" === e.indent) r = "\t";
                         else {
                             if (!("number" == typeof e.indent && e.indent > 0)) return null;
                             r = x.call(Array(e.indent + 1), " ")
                         }
                         return {
@@ -10296,18 +10313,18 @@
                                 var t = v.call(y.call(e), /^function\s*([\w$]+)/);
                                 return t ? t[1] : null
                             }(t),
                             ee = Z(t, $);
                         return "[Function" + (J ? ": " + J : " (anonymous)") + "]" + (ee.length > 0 ? " { " + x.call(ee, ", ") + " }" : "")
                     }
                     if (H(t)) {
-                        var te = _ ? g.call(String(t), /^(Symbol\(.*\))_[^)]*$/, "$1") : S.call(t);
+                        var te = _ ? g.call(String(t), /^(Symbol\(.*\))_[^)]*$/, "$1") : R.call(t);
                         return "object" != typeof t || _ ? te : X(te)
                     }
-                    if ((R = t) && "object" == typeof R && ("undefined" != typeof HTMLElement && R instanceof HTMLElement || "string" == typeof R.nodeName && "function" == typeof R.getAttribute)) {
+                    if ((S = t) && "object" == typeof S && ("undefined" != typeof HTMLElement && S instanceof HTMLElement || "string" == typeof S.nodeName && "function" == typeof S.getAttribute)) {
                         for (var re = "<" + C.call(String(t.nodeName)), ne = t.attributes || [], oe = 0; oe < ne.length; oe++) re += " " + ne[oe].name + "=" + B(L(ne[oe].value), "double", l);
                         return re += ">", t.childNodes && t.childNodes.length && (re += "..."), re + "</" + C.call(String(t.nodeName)) + ">"
                     }
                     if (U(t)) {
                         if (0 === t.length) return "[]";
                         var ae = Z(t, $);
                         return F && ! function(e) {
@@ -10316,15 +10333,15 @@
                             return !0
                         }(ae) ? "[" + Q(ae, F) + "]" : "[ " + x.call(ae, ", ") + " ]"
                     }
                     if (function(e) {
                             return !("[object Error]" !== z(e) || A && "object" == typeof e && A in e)
                         }(t)) {
                         var ie = Z(t, $);
-                        return "cause" in Error.prototype || !("cause" in t) || T.call(t, "cause") ? 0 === ie.length ? "[" + String(t) + "]" : "{ [" + String(t) + "] " + x.call(ie, ", ") + " }" : "{ [" + String(t) + "] " + x.call(q.call("[cause]: " + $(t.cause), ie), ", ") + " }"
+                        return "cause" in Error.prototype || !("cause" in t) || M.call(t, "cause") ? 0 === ie.length ? "[" + String(t) + "]" : "{ [" + String(t) + "] " + x.call(ie, ", ") + " }" : "{ [" + String(t) + "] " + x.call(q.call("[cause]: " + $(t.cause), ie), ", ") + " }"
                     }
                     if ("object" == typeof t && u) {
                         if (N && "function" == typeof t[N] && k) return k(t, {
                             depth: O - n
                         });
                         if ("symbol" !== u && "function" == typeof t.inspect) return t.inspect()
                     }
@@ -10413,15 +10430,15 @@
                     if (function(e) {
                             return !("[object String]" !== z(e) || A && "object" == typeof e && A in e)
                         }(t)) return X($(String(t)));
                     if (! function(e) {
                             return !("[object Date]" !== z(e) || A && "object" == typeof e && A in e)
                         }(t) && !D(t)) {
                         var se = Z(t, $),
-                            ce = M ? M(t) === Object.prototype : t instanceof Object || t.constructor === Object,
+                            ce = T ? T(t) === Object.prototype : t instanceof Object || t.constructor === Object,
                             de = t instanceof Object ? "" : "null prototype",
                             pe = !ce && A && Object(t) === t && A in t ? h.call(z(t), 8, -1) : de ? "Object" : "",
                             fe = (ce || "function" != typeof t.constructor ? "" : t.constructor.name ? t.constructor.name + " " : "") + (pe || de ? "[" + x.call(q.call([], pe || [], de || []), ": ") + "] " : "");
                         return 0 === se.length ? fe + "{}" : F ? fe + "{" + Q(se, F) + "}" : fe + "{ " + x.call(se, ", ") + " }"
                     }
                     return String(t)
                 };
@@ -10486,22 +10503,22 @@
                 function Z(e, t) {
                     var r = U(e),
                         n = [];
                     if (r) {
                         n.length = e.length;
                         for (var o = 0; o < e.length; o++) n[o] = W(e, o) ? t(e[o], e) : ""
                     }
-                    var a, i = "function" == typeof R ? R(e) : [];
+                    var a, i = "function" == typeof S ? S(e) : [];
                     if (_) {
                         a = {};
                         for (var l = 0; l < i.length; l++) a["$" + i[l]] = i[l]
                     }
                     for (var u in e) W(e, u) && (r && String(Number(u)) === u && u < e.length || _ && a["$" + u] instanceof Symbol || (w.call(/[^\w$]/, u) ? n.push(t(u, e) + ": " + t(e[u], e)) : n.push(u + ": " + t(e[u], e))));
-                    if ("function" == typeof R)
-                        for (var s = 0; s < i.length; s++) T.call(e, i[s]) && n.push("[" + t(i[s]) + "]: " + t(e[i[s]], e));
+                    if ("function" == typeof S)
+                        for (var s = 0; s < i.length; s++) M.call(e, i[s]) && n.push("[" + t(i[s]) + "]: " + t(e[i[s]], e));
                     return n
                 }
             },
             4244: e => {
                 "use strict";
                 var t = function(e) {
                     return e != e
@@ -10805,27 +10822,27 @@
                 }
             },
             5914: (e, t, r) => {
                 "use strict";
                 t.WU = function(e, t) {
                     if (t && (function(e) {
                             if (Object.keys(e).forEach((e => {
-                                    if (!T.hasOwnProperty(e)) throw new Error(`pretty-format: Unknown option "${e}".`)
+                                    if (!M.hasOwnProperty(e)) throw new Error(`pretty-format: Unknown option "${e}".`)
                                 })), e.min && void 0 !== e.indent && 0 !== e.indent) throw new Error('pretty-format: Options "min" and "indent" cannot be used together.');
                             if (void 0 !== e.theme) {
                                 if (null === e.theme) throw new Error('pretty-format: Option "theme" must not be null.');
                                 if ("object" != typeof e.theme) throw new Error(`pretty-format: Option "theme" must be of type "object" but instead received "${typeof e.theme}".`)
                             }
                         }(t), t.plugins)) {
-                        const r = R(t.plugins, e);
+                        const r = S(t.plugins, e);
                         if (null !== r) return j(r, e, N(t), "", 0, [])
                     }
                     const r = E(e, I(t), k(t), F(t));
                     return null !== r ? r : O(e, N(t), "", 0, [])
-                }, t.Gr = void 0;
+                }, t.plugins = void 0;
                 var n = p(r(7761)),
                     o = r(7354),
                     a = p(r(9071)),
                     i = p(r(4990)),
                     l = p(r(10)),
                     u = p(r(3195)),
                     s = p(r(4558)),
@@ -10882,102 +10899,102 @@
                 }
 
                 function O(e, t, r, n, a, i) {
                     if (-1 !== a.indexOf(e)) return "[Circular]";
                     (a = a.slice()).push(e);
                     const l = ++n > t.maxDepth,
                         u = t.min;
-                    if (t.callToJSON && !l && e.toJSON && "function" == typeof e.toJSON && !i) return S(e.toJSON(), t, r, n, a, !0);
+                    if (t.callToJSON && !l && e.toJSON && "function" == typeof e.toJSON && !i) return R(e.toJSON(), t, r, n, a, !0);
                     const s = f.call(e);
-                    return "[object Arguments]" === s ? l ? "[Arguments]" : (u ? "" : "Arguments ") + "[" + (0, o.printListItems)(e, t, r, n, a, S) + "]" : function(e) {
+                    return "[object Arguments]" === s ? l ? "[Arguments]" : (u ? "" : "Arguments ") + "[" + (0, o.printListItems)(e, t, r, n, a, R) + "]" : function(e) {
                         return "[object Array]" === e || "[object ArrayBuffer]" === e || "[object DataView]" === e || "[object Float32Array]" === e || "[object Float64Array]" === e || "[object Int8Array]" === e || "[object Int16Array]" === e || "[object Int32Array]" === e || "[object Uint8Array]" === e || "[object Uint8ClampedArray]" === e || "[object Uint16Array]" === e || "[object Uint32Array]" === e
-                    }(s) ? l ? "[" + e.constructor.name + "]" : (u ? "" : t.printBasicPrototype || "Array" !== e.constructor.name ? e.constructor.name + " " : "") + "[" + (0, o.printListItems)(e, t, r, n, a, S) + "]" : "[object Map]" === s ? l ? "[Map]" : "Map {" + (0, o.printIteratorEntries)(e.entries(), t, r, n, a, S, " => ") + "}" : "[object Set]" === s ? l ? "[Set]" : "Set {" + (0, o.printIteratorValues)(e.values(), t, r, n, a, S) + "}" : l || h(e) ? "[" + v(e) + "]" : (u ? "" : t.printBasicPrototype || "Object" !== v(e) ? v(e) + " " : "") + "{" + (0, o.printObjectProperties)(e, t, r, n, a, S) + "}"
+                    }(s) ? l ? "[" + e.constructor.name + "]" : (u ? "" : t.printBasicPrototype || "Array" !== e.constructor.name ? e.constructor.name + " " : "") + "[" + (0, o.printListItems)(e, t, r, n, a, R) + "]" : "[object Map]" === s ? l ? "[Map]" : "Map {" + (0, o.printIteratorEntries)(e.entries(), t, r, n, a, R, " => ") + "}" : "[object Set]" === s ? l ? "[Set]" : "Set {" + (0, o.printIteratorValues)(e.values(), t, r, n, a, R) + "}" : l || h(e) ? "[" + v(e) + "]" : (u ? "" : t.printBasicPrototype || "Object" !== v(e) ? v(e) + " " : "") + "{" + (0, o.printObjectProperties)(e, t, r, n, a, R) + "}"
                 }
 
                 function j(e, t, r, n, o, a) {
                     let i;
                     try {
                         i = function(e) {
                             return null != e.serialize
-                        }(e) ? e.serialize(t, r, n, o, a, S) : e.print(t, (e => S(e, r, n, o, a)), (e => {
+                        }(e) ? e.serialize(t, r, n, o, a, R) : e.print(t, (e => R(e, r, n, o, a)), (e => {
                             const t = n + r.indent;
                             return t + e.replace(P, "\n" + t)
                         }), {
                             edgeSpacing: r.spacingOuter,
                             min: r.min,
                             spacing: r.spacingInner
                         }, r.colors)
                     } catch (e) {
                         throw new C(e.message, e.stack)
                     }
                     if ("string" != typeof i) throw new Error(`pretty-format: Plugin must return type "string" but instead returned "${typeof i}".`);
                     return i
                 }
 
-                function R(e, t) {
+                function S(e, t) {
                     for (let r = 0; r < e.length; r++) try {
                         if (e[r].test(t)) return e[r]
                     } catch (e) {
                         throw new C(e.message, e.stack)
                     }
                     return null
                 }
 
-                function S(e, t, r, n, o, a) {
-                    const i = R(t.plugins, e);
+                function R(e, t, r, n, o, a) {
+                    const i = S(t.plugins, e);
                     if (null !== i) return j(i, e, t, r, n, o);
                     const l = E(e, t.printFunctionName, t.escapeRegex, t.escapeString);
                     return null !== l ? l : O(e, t, r, n, o, a)
                 }
                 const _ = {
                         comment: "gray",
                         content: "reset",
                         prop: "yellow",
                         tag: "cyan",
                         value: "green"
                     },
                     A = Object.keys(_),
-                    T = {
+                    M = {
                         callToJSON: !0,
                         compareKeys: void 0,
                         escapeRegex: !1,
                         escapeString: !0,
                         highlight: !1,
                         indent: 2,
                         maxDepth: 1 / 0,
                         min: !1,
                         plugins: [],
                         printBasicPrototype: !0,
                         printFunctionName: !0,
                         theme: _
                     },
-                    M = e => A.reduce(((t, r) => {
+                    T = e => A.reduce(((t, r) => {
                         const o = e.theme && void 0 !== e.theme[r] ? e.theme[r] : _[r],
                             a = o && n.default[o];
                         if (!a || "string" != typeof a.close || "string" != typeof a.open) throw new Error(`pretty-format: Option "theme" has a key "${r}" whose value "${o}" is undefined in ansi-styles.`);
                         return t[r] = a, t
                     }), Object.create(null)),
-                    I = e => e && void 0 !== e.printFunctionName ? e.printFunctionName : T.printFunctionName,
-                    k = e => e && void 0 !== e.escapeRegex ? e.escapeRegex : T.escapeRegex,
-                    F = e => e && void 0 !== e.escapeString ? e.escapeString : T.escapeString,
+                    I = e => e && void 0 !== e.printFunctionName ? e.printFunctionName : M.printFunctionName,
+                    k = e => e && void 0 !== e.escapeRegex ? e.escapeRegex : M.escapeRegex,
+                    F = e => e && void 0 !== e.escapeString ? e.escapeString : M.escapeString,
                     N = e => {
                         var t, r;
                         return {
-                            callToJSON: e && void 0 !== e.callToJSON ? e.callToJSON : T.callToJSON,
-                            colors: e && e.highlight ? M(e) : A.reduce(((e, t) => (e[t] = {
+                            callToJSON: e && void 0 !== e.callToJSON ? e.callToJSON : M.callToJSON,
+                            colors: e && e.highlight ? T(e) : A.reduce(((e, t) => (e[t] = {
                                 close: "",
                                 open: ""
                             }, e)), Object.create(null)),
-                            compareKeys: e && "function" == typeof e.compareKeys ? e.compareKeys : T.compareKeys,
+                            compareKeys: e && "function" == typeof e.compareKeys ? e.compareKeys : M.compareKeys,
                             escapeRegex: k(e),
                             escapeString: F(e),
-                            indent: e && e.min ? "" : (r = e && void 0 !== e.indent ? e.indent : T.indent, new Array(r + 1).join(" ")),
-                            maxDepth: e && void 0 !== e.maxDepth ? e.maxDepth : T.maxDepth,
-                            min: e && void 0 !== e.min ? e.min : T.min,
-                            plugins: e && void 0 !== e.plugins ? e.plugins : T.plugins,
+                            indent: e && e.min ? "" : (r = e && void 0 !== e.indent ? e.indent : M.indent, new Array(r + 1).join(" ")),
+                            maxDepth: e && void 0 !== e.maxDepth ? e.maxDepth : M.maxDepth,
+                            min: e && void 0 !== e.min ? e.min : M.min,
+                            plugins: e && void 0 !== e.plugins ? e.plugins : M.plugins,
                             printBasicPrototype: null === (t = null == e ? void 0 : e.printBasicPrototype) || void 0 === t || t,
                             printFunctionName: I(e),
                             spacingInner: e && e.min ? " " : "\n",
                             spacingOuter: e && e.min ? "" : "\n"
                         }
                     };
                 const B = {
@@ -10985,15 +11002,15 @@
                     ConvertAnsi: i.default,
                     DOMCollection: l.default,
                     DOMElement: u.default,
                     Immutable: s.default,
                     ReactElement: c.default,
                     ReactTestComponent: d.default
                 };
-                t.Gr = B
+                t.plugins = B
             },
             9071: (e, t, r) => {
                 "use strict";
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 }), t.test = t.serialize = t.default = void 0;
                 var n = r(7354),
@@ -11484,18 +11501,18 @@
                 var C = l,
                     w = r,
                     q = s,
                     x = o,
                     E = f,
                     O = p,
                     j = n,
-                    R = i,
-                    S = a,
+                    S = i,
+                    R = a,
                     _ = c;
-                t.ContextConsumer = u, t.ContextProvider = C, t.Element = w, t.ForwardRef = q, t.Fragment = x, t.Lazy = E, t.Memo = O, t.Portal = j, t.Profiler = R, t.StrictMode = S, t.Suspense = _, t.isAsyncMode = function() {
+                t.ContextConsumer = u, t.ContextProvider = C, t.Element = w, t.ForwardRef = q, t.Fragment = x, t.Lazy = E, t.Memo = O, t.Portal = j, t.Profiler = S, t.StrictMode = R, t.Suspense = _, t.isAsyncMode = function() {
                     return !1
                 }, t.isConcurrentMode = function() {
                     return !1
                 }, t.isContextConsumer = function(e) {
                     return P(e) === u
                 }, t.isContextProvider = function(e) {
                     return P(e) === l
@@ -11529,15 +11546,15 @@
                 "use strict";
                 var n = r(5972).functionsHaveConfigurableNames(),
                     o = Object,
                     a = TypeError;
                 e.exports = function() {
                     if (null != this && this !== o(this)) throw new a("RegExp.prototype.flags getter called on non-object");
                     var e = "";
-                    return this.hasIndices && (e += "d"), this.global && (e += "g"), this.ignoreCase && (e += "i"), this.multiline && (e += "m"), this.dotAll && (e += "s"), this.unicode && (e += "u"), this.sticky && (e += "y"), e
+                    return this.hasIndices && (e += "d"), this.global && (e += "g"), this.ignoreCase && (e += "i"), this.multiline && (e += "m"), this.dotAll && (e += "s"), this.unicode && (e += "u"), this.unicodeSets && (e += "v"), this.sticky && (e += "y"), e
                 }, n && Object.defineProperty && Object.defineProperty(e.exports, "name", {
                     value: "get flags"
                 })
             },
             2847: (e, t, r) => {
                 "use strict";
                 var n = r(4289),
```

### Comparing `selenium_testing_library-2023.3/selenium_testing_library/screen.py` & `selenium_testing_library-2023.4/selenium_testing_library/screen.py`

 * *Files identical despite different names*

### Comparing `selenium_testing_library-2023.3/setup.py` & `selenium_testing_library-2023.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['ruff>=0.0.247,<0.0.248', 'selenium>3.0.0', 'typing_extensions>=4.0.0']
 
 setup_kwargs = {
     'name': 'selenium-testing-library',
-    'version': '2023.3',
+    'version': '2023.4',
     'description': 'A Python Selenium library inspired by the Testing Library',
     'long_description': '# Selenium Testing Library\n\n[![PyPI version](https://badge.fury.io/py/selenium-testing-library.svg)](https://badge.fury.io/py/selenium-testing-library)\n[![test](https://github.com/anze3db/selenium-testing-library/actions/workflows/main.yml/badge.svg)](https://github.com/anze3db/selenium-testing-library/actions/workflows/main.yml) [![codecov](https://codecov.io/gh/anze3db/selenium-testing-library/branch/main/graph/badge.svg?token=L1M7HO3DL7)](https://codecov.io/gh/anze3db/selenium-testing-library)\n\nSelenium Testing Library (STL) is a Python library implementing [Testing-Library](https://testing-library.com/) in Selenium.\n\n## Dependencies\n\n- Python 3.7, 3.8, 3.9, 3.10, 3.11\n- [`selenium`](https://pypi.org/project/selenium/) >= 3.0.0, [`typing-extensions`](https://pypi.org/project/typing-extensions/) >= 4.0.0\n## Installation\n\n```\npip install selenium-testing-library\n```\n\n## Quick Start\n\n```python\nfrom selenium import webdriver\nfrom selenium_testing_library import Screen\n\ndriver = webdriver.Chrome()\ndriver.open(\'https://google.com/\')\n\nscreen = Screen(driver)\nsearch_input = screen.find_by_title("Search")\nsearch.send_keys("Dogs")\nsearch_button = screen.find_by_text("Google Search")\nsearch_button.click()\nscreen.wait_for_stale(search_button)\n```\n\n## Finding elements\n\nSTL implements the [Queries API](https://testing-library.com/docs/queries/about) from the Testing Library. The Testing Library queries `get_by`, `query_by`, `find_by`, and the multiple element equivalents `get_all_by`, `query_all_by`, `find_all_by` are used in places where you would normally use Selenium\'s `find_element` and `find_elements` functions.\n\n The difference between the different queries (`get_by`, `query_by`, `find_by`) is whether the query will throw an error if the element was not found (`get_by`), return `None` (`query_by`) or block, wait and retry until the element is found (`find_by`).\n\n * `get_by` returns the element matched and throws an exception if zero or more than one element matches. This is the main function that we should be using to locate elements on a page.\n * `query_by` returns the element matched or `None` if no element match. It throws an exception if more than one element matches. Mostly used for asserting that an element is **not** present: `assert not screen.query_by_text("not on page")`.\n * `find_by` behaves like `get_by`, but uses a `WebDriverWait` to wait until the element is present in the DOM.\n * `get_all_by` returns a list of elements matched. It raises an exception if no elements match.\n * `query_all_by` returns a list of elements matched. It returns an empty list when no elements match.\n * `find_all_by` behaves like `get_all_by`, but uses a `WebDriverWait` to wait until the elements are present in the DOM.\n\n When an element is found the queries return a Selenium [`WebElement`](https://selenium-python.readthedocs.io/api.html#module-selenium.webdriver.remote.webelement) or a list containing Selenium [WebElement](https://selenium-python.readthedocs.io/api.html#module-selenium.webdriver.remote.webelement)s when using `get_all_by`, `query_all_by`, `find_all_by`.\n\nThe queries accept a tuple containing the [By class identifier](https://selenium-python.readthedocs.io/api.html#locate-elements-by) and the search query, so they can be used with XPath, Css or any other native Selenium selector:\n\n```python\nfrom selenium import webdriver\nfrom selenium.webdriver.common.by import By\nfrom selenium_testing_library import Screen\n\nscreen = Screen(webdriver.Chrome())\nscreen.get_by((By.CSS, ".my_class")) # Will throw an exception if the element is not found\nscreen.query_by((By.ID, "my_id")) # you can use regular tuples as if you were using Selenium\'s find_element()\nscreen.find_by((By.XPATH, "//div"), timeout=5, poll_frequency=0.5) # locators for searching through text also work\n```\n\n## Locator Classes\n\nFor convenience Locator classes can be used instead of the tuples:\n\n```python\nfrom selenium import webdriver\nfrom selenium_testing_library import Screen, locators\n\nscreen = Screen(webdriver.Chrome())\nscreen.get_by(locators.Css(".my_class")) # Will throw an exception if the element is not found\nscreen.query_by(locators.Id("my_id")) # you can use regular tuples as if you were using Selenium\'s find_element()\nscreen.find_by(locators.XPath("//div"), timeout=5, poll_frequency=0.5) # locators for searching through text also work\n```\n\n## Testing Library Selectors\n\nBesides all the Selenium native By selectors, the queries also support Testing Library\'s selectors:\n * [Role](https://testing-library.com/docs/queries/byrole)\n * [LabelText](https://testing-library.com/docs/queries/bylabeltext)\n * [PlaceholderText](https://testing-library.com/docs/queries/byplaceholdertext)\n * [Text](https://testing-library.com/docs/queries/bytext)\n * [DisplayValue](https://testing-library.com/docs/queries/bydisplayvalue)\n * [AltText](https://testing-library.com/docs/queries/byalttext)\n * [Title](https://testing-library.com/docs/queries/bytitle)\n * [TestId](https://testing-library.com/docs/queries/bytestid)\n\n```python\nfrom selenium import webdriver\nfrom selenium_testing_library import Screen, locators\n\nscreen = Screen(webdriver.Chrome())\nscreen.get_by(locators.Text("My Text"))\nscreen.query_by(locators.Role("button", pressed=True))\nscreen.find_by(locators.TestId("my-test"), timeout=5, poll_frequency=0.5) # locators for searching through text also work\n```\n## Helper functions\n\nFor convenience helper functions on the screen class are available to avoid instantiating locator classes all over the place:\n\n[`screen.get_by_role(role_name)`](https://testing-library.com/docs/queries/byrole) Queries for elements with the given role.\n[`screen.get_by_label_text(text)`](https://testing-library.com/docs/queries/bylabeltext) Queries for label elements that match the text string and return the corresponding input element.\n[`screen.get_by_placeholder_text(text)`](https://testing-library.com/docs/queries/byplaceholdertext) Queries elements with the matching placeholder attribute.\n[`screen.get_by_text(text)`](https://testing-library.com/docs/queries/bytext) Queries elements where the content matches the provided text.\n[`screen.get_by_display_value(value)`](https://testing-library.com/docs/queries/bydisplayvalue) Queries inputs, textareas, or selects with matching display value.\n[`screen.get_by_alt_text(text)`](https://testing-library.com/docs/queries/byalttext) Queries elements with the matching alt attribute.\n`screen.get_by_title(text)` Queries elements with the matching title attribute.\n`screen.get_by_test_id(value)` Queries elements matching the `data-testid` value.\n`screen.get_by_css(css)` Queries elements matching the specified css selector.\n`screen.get_by_xpath(xpath)` Queries elements matching the specified xpath selector.\n\nThere are also `query_by_*`, `find_by_*`, `get_all_by_*`, `query_all_by_*`, `find_all_by_*`  equivalents.\n\n**Note:** The selenium project has removed the `find_element_by_*` and `find_elements_by_*` helper functions in the [Selenium 4.3.0](https://github.com/SeleniumHQ/selenium/releases/tag/selenium-4.3.0) release, so I just want to state that the `screen` helper functions will never be deprecated or removed.\n\nExamples:\n\n```python\nfrom selenium import webdriver\nfrom selenium_testing_library import Screen\n\nscreen = Screen(webdriver.Chrome())\nscreen.query_by_role("role_name")\nscreen.get_by_label_text("label text")\nscreen.find_all_by_text("my text", timeout=5, poll_frequency=0.5)\nscreen.get_all_by_alt_text("alt text")\n```\n\n## Wait functions\n\n`wait_for(condition_function)` Waits until the condition function returns a truthy value.\n`wait_for_stale(element)` Waits until the element is removed from the DOM.\n\nExamples:\n\n```python\nfrom selenium import webdriver\nfrom selenium_testing_library import Screen, locators\n\nscreen = Screen(webdriver.Chrome())\n\n# Wait for the element to be clickable:\nelement = screen.get_by_text("Submit")\nscreen.wait_for(lambda _: element.is_enabled(), timeout=5, poll_frequency=0.5)\n# Wait for the element to be removed from the page:\nscreen.wait_for_stale(element)\n```\n\n## Querying within elements\n\n`Within(element)` Used to limit the query to the children of the provided element\n\nExample:\n\n```python\nfrom selenium import webdriver\nfrom selenium_testing_library import Screen, Within\n\nscreen = Screen(webdriver.Chrome())\nparent_element = screen.get_by_css(".container")\nWithin(parent_element).get_by_title("My title inside the container")\n```\n\n# Testing Playground URLs\n\nFor debugging using [testing-playground](https://testing-playground.com/), `screen` exposes `log_testing_playground_url()` which prints end returns a URL that can be opened in the browser.\n\n```python\n# log entire document to testing-playground\nurl = screen.log_testing_playground_url()\n# log a single element\nurl = screen.log_testing_playground_url(screen.get_by_text("test"))\n```\n\n# Contributing\n\nSetting up a local development environment\n\n```shell\ngit clone https://github.com/anze3db/selenium-testing-library.git && cd selenium-testing-library\npoetry install && poetry shell\n# Make sure `chromedriver` is in your PATH, download from https://chromedriver.chromium.org/downloads\n# run tests:\npytest --selenium-headless\n# run tests and display coverage info:\npytest --selenium-headless --cov=selenium_testing_library --cov-report html\n\n# To test on multiple Python versions make sure that py37, py38, py39 are\n# installed on your system and available through python3.7, python3.8,\n# python3.9. (Use pyenv and add the pyenv shims to your path\n# `export PATH=$(pyenv root)/shims:$PATH`). Then run tox:\ntox\n```\n\n# Releasing a new version\n\n```shell\nnpm run deploy\nbumpver update  # Wait and see if the CI is green\npoetry build && poetry publish\n```\n',
     'author': 'Anže Pečar',
     'author_email': 'anze@pecar.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/anze3db/selenium-testing-library',
```

### Comparing `selenium_testing_library-2023.3/PKG-INFO` & `selenium_testing_library-2023.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-testing-library
-Version: 2023.3
+Version: 2023.4
 Summary: A Python Selenium library inspired by the Testing Library
 Home-page: https://github.com/anze3db/selenium-testing-library
 License: MIT
 Author: Anže Pečar
 Author-email: anze@pecar.me
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

