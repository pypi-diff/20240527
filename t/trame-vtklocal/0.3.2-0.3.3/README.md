# Comparing `tmp/trame-vtklocal-0.3.2.tar.gz` & `tmp/trame-vtklocal-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-vtklocal-0.3.2.tar", last modified: Sun May  5 23:35:58 2024, max compression
+gzip compressed data, was "trame-vtklocal-0.3.3.tar", last modified: Mon May 27 21:50:08 2024, max compression
```

## Comparing `trame-vtklocal-0.3.2.tar` & `trame-vtklocal-0.3.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 23:35:58.350779 trame-vtklocal-0.3.2/
--rw-r--r--   0 root         (0) root         (0)      583 2024-05-05 23:35:35.000000 trame-vtklocal-0.3.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       34 2024-05-05 23:35:35.000000 trame-vtklocal-0.3.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2433 2024-05-05 23:35:58.350779 trame-vtklocal-0.3.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1673 2024-05-05 23:35:35.000000 trame-vtklocal-0.3.2/README.rst
--rw-r--r--   0 root         (0) root         (0)      896 2024-05-05 23:35:58.354779 trame-vtklocal-0.3.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-05 23:35:35.000000 trame-vtklocal-0.3.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 23:35:58.350779 trame-vtklocal-0.3.2/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-05 23:35:35.000000 trame-vtklocal-0.3.2/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 23:35:58.350779 trame-vtklocal-0.3.2/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-05 23:35:35.000000 trame-vtklocal-0.3.2/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       36 2024-05-05 23:35:35.000000 trame-vtklocal-0.3.2/trame/modules/vtklocal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 23:35:58.350779 trame-vtklocal-0.3.2/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-05 23:35:35.000000 trame-vtklocal-0.3.2/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      144 2024-05-05 23:35:35.000000 trame-vtklocal-0.3.2/trame/widgets/vtklocal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 23:35:58.350779 trame-vtklocal-0.3.2/trame_vtklocal/
--rw-r--r--   0 root         (0) root         (0)       96 2024-05-05 23:35:35.000000 trame-vtklocal-0.3.2/trame_vtklocal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 23:35:58.350779 trame-vtklocal-0.3.2/trame_vtklocal/module/
--rw-r--r--   0 root         (0) root         (0)      873 2024-05-05 23:35:35.000000 trame-vtklocal-0.3.2/trame_vtklocal/module/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4331 2024-05-05 23:35:35.000000 trame-vtklocal-0.3.2/trame_vtklocal/module/protocol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 23:35:58.346779 trame-vtklocal-0.3.2/trame_vtklocal/module/serve/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 23:35:58.350779 trame-vtklocal-0.3.2/trame_vtklocal/module/serve/js/
--rw-r--r--   0 root         (0) root         (0)     4135 2024-05-05 23:35:55.000000 trame-vtklocal-0.3.2/trame_vtklocal/module/serve/js/trame_vtklocal.umd.js
--rw-r--r--   0 root         (0) root         (0)     2094 2024-05-05 23:35:35.000000 trame-vtklocal-0.3.2/trame_vtklocal/module/wasm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 23:35:58.350779 trame-vtklocal-0.3.2/trame_vtklocal/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 23:35:35.000000 trame-vtklocal-0.3.2/trame_vtklocal/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4260 2024-05-05 23:35:35.000000 trame-vtklocal-0.3.2/trame_vtklocal/widgets/vtklocal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 23:35:58.350779 trame-vtklocal-0.3.2/trame_vtklocal.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2433 2024-05-05 23:35:58.000000 trame-vtklocal-0.3.2/trame_vtklocal.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      608 2024-05-05 23:35:58.000000 trame-vtklocal-0.3.2/trame_vtklocal.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 23:35:58.000000 trame-vtklocal-0.3.2/trame_vtklocal.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-05-05 23:35:58.000000 trame-vtklocal-0.3.2/trame_vtklocal.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-05 23:35:58.000000 trame-vtklocal-0.3.2/trame_vtklocal.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 21:50:08.954049 trame-vtklocal-0.3.3/
+-rw-r--r--   0 root         (0) root         (0)      583 2024-05-27 21:49:44.000000 trame-vtklocal-0.3.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       34 2024-05-27 21:49:44.000000 trame-vtklocal-0.3.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2433 2024-05-27 21:50:08.954049 trame-vtklocal-0.3.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1673 2024-05-27 21:49:44.000000 trame-vtklocal-0.3.3/README.rst
+-rw-r--r--   0 root         (0) root         (0)      896 2024-05-27 21:50:08.954049 trame-vtklocal-0.3.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-27 21:49:44.000000 trame-vtklocal-0.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 21:50:08.950049 trame-vtklocal-0.3.3/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-27 21:49:44.000000 trame-vtklocal-0.3.3/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 21:50:08.950049 trame-vtklocal-0.3.3/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-27 21:49:44.000000 trame-vtklocal-0.3.3/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       36 2024-05-27 21:49:44.000000 trame-vtklocal-0.3.3/trame/modules/vtklocal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 21:50:08.950049 trame-vtklocal-0.3.3/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-27 21:49:44.000000 trame-vtklocal-0.3.3/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      144 2024-05-27 21:49:44.000000 trame-vtklocal-0.3.3/trame/widgets/vtklocal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 21:50:08.950049 trame-vtklocal-0.3.3/trame_vtklocal/
+-rw-r--r--   0 root         (0) root         (0)       96 2024-05-27 21:49:44.000000 trame-vtklocal-0.3.3/trame_vtklocal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 21:50:08.954049 trame-vtklocal-0.3.3/trame_vtklocal/module/
+-rw-r--r--   0 root         (0) root         (0)      873 2024-05-27 21:49:44.000000 trame-vtklocal-0.3.3/trame_vtklocal/module/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4331 2024-05-27 21:49:44.000000 trame-vtklocal-0.3.3/trame_vtklocal/module/protocol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 21:50:08.950049 trame-vtklocal-0.3.3/trame_vtklocal/module/serve/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 21:50:08.954049 trame-vtklocal-0.3.3/trame_vtklocal/module/serve/js/
+-rw-r--r--   0 root         (0) root         (0)     4230 2024-05-27 21:50:05.000000 trame-vtklocal-0.3.3/trame_vtklocal/module/serve/js/trame_vtklocal.umd.js
+-rw-r--r--   0 root         (0) root         (0)     2417 2024-05-27 21:49:44.000000 trame-vtklocal-0.3.3/trame_vtklocal/module/wasm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 21:50:08.954049 trame-vtklocal-0.3.3/trame_vtklocal/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 21:49:44.000000 trame-vtklocal-0.3.3/trame_vtklocal/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4617 2024-05-27 21:49:44.000000 trame-vtklocal-0.3.3/trame_vtklocal/widgets/vtklocal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 21:50:08.950049 trame-vtklocal-0.3.3/trame_vtklocal.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2433 2024-05-27 21:50:08.000000 trame-vtklocal-0.3.3/trame_vtklocal.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      608 2024-05-27 21:50:08.000000 trame-vtklocal-0.3.3/trame_vtklocal.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 21:50:08.000000 trame-vtklocal-0.3.3/trame_vtklocal.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-27 21:50:08.000000 trame-vtklocal-0.3.3/trame_vtklocal.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-27 21:50:08.000000 trame-vtklocal-0.3.3/trame_vtklocal.egg-info/top_level.txt
```

### Comparing `trame-vtklocal-0.3.2/LICENSE` & `trame-vtklocal-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-vtklocal-0.3.2/PKG-INFO` & `trame-vtklocal-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-vtklocal
-Version: 0.3.2
+Version: 0.3.3
 Summary: VTK Local Rendering using WASM
 Author: Kitware Inc.
 License: Apache Software License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
@@ -35,15 +35,15 @@
 .. code-block:: console
 
     pip install trame-vtklocal 
 
     # We need a VTK that has its wasm counterpart
     # This is the first version available with it
     # For ParaView (not yet supported), VTK don't need to be installed
-    pip install "vtk==9.3.20240418.dev0" --extra-index-url https://wheels.vtk.org
+    pip install "vtk==9.3.20240525.dev0" --extra-index-url https://wheels.vtk.org
 
 
 Development
 ----------------------------------------
 
 Build and install the Vue components
```

### Comparing `trame-vtklocal-0.3.2/README.rst` & `trame-vtklocal-0.3.3/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 .. code-block:: console
 
     pip install trame-vtklocal 
 
     # We need a VTK that has its wasm counterpart
     # This is the first version available with it
     # For ParaView (not yet supported), VTK don't need to be installed
-    pip install "vtk==9.3.20240418.dev0" --extra-index-url https://wheels.vtk.org
+    pip install "vtk==9.3.20240525.dev0" --extra-index-url https://wheels.vtk.org
 
 
 Development
 ----------------------------------------
 
 Build and install the Vue components
```

### Comparing `trame-vtklocal-0.3.2/setup.cfg` & `trame-vtklocal-0.3.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-vtklocal
-version = 0.3.2
+version = 0.3.3
 description = VTK Local Rendering using WASM
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = Apache Software License
 classifiers = 
 	Development Status :: 4 - Beta
```

### Comparing `trame-vtklocal-0.3.2/trame_vtklocal/module/__init__.py` & `trame-vtklocal-0.3.3/trame_vtklocal/module/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-vtklocal-0.3.2/trame_vtklocal/module/protocol.py` & `trame-vtklocal-0.3.3/trame_vtklocal/module/protocol.py`

 * *Files identical despite different names*

### Comparing `trame-vtklocal-0.3.2/trame_vtklocal/module/serve/js/trame_vtklocal.umd.js` & `trame-vtklocal-0.3.3/trame_vtklocal/module/serve/js/trame_vtklocal.umd.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,28 +1,28 @@
-(function(u, s) {
-    typeof exports == "object" && typeof module < "u" ? s(exports, require("vue")) : typeof define == "function" && define.amd ? define(["exports", "vue"], s) : (u = typeof globalThis < "u" ? globalThis : u || self, s(u.trame_vtklocal = {}, u.Vue))
-})(this, function(u, s) {
+(function(u, r) {
+    typeof exports == "object" && typeof module < "u" ? r(exports, require("vue")) : typeof define == "function" && define.amd ? define(["exports", "vue"], r) : (u = typeof globalThis < "u" ? globalThis : u || self, r(u.trame_vtklocal = {}, u.Vue))
+})(this, function(u, r) {
     "use strict";
-    async function W(r, c) {
+    async function O(s, c) {
         const d = {
-                canvas: r,
+                canvas: s,
                 locateFile() {
                     return c
                 },
                 print() {
                     console.info(Array.prototype.slice.call(arguments).join(" "))
                 },
                 printErr() {
                     console.error(Array.prototype.slice.call(arguments).join(" "))
                 }
             },
             p = await window.createVTKWasmSceneManager(d);
         return p.initialize(), p
     }
-    const k = {
+    const j = {
         VtkLocal: {
             emits: ["updated", "memory-vtk", "memory-arrays"],
             props: {
                 renderWindow: {
                     type: Number
                 },
                 eagerSync: {
@@ -33,133 +33,138 @@
                     type: Number,
                     default: 1e8
                 },
                 wsClient: {
                     type: Object
                 }
             },
-            setup(r, {
+            setup(s, {
                 emit: c
             }) {
-                const d = s.inject("trame"),
+                const d = r.inject("trame"),
                     p = d.state.get("__trame_vtklocal_wasm_url"),
-                    T = s.ref(null),
-                    v = s.ref(null),
-                    y = r.wsClient || (d == null ? void 0 : d.client),
+                    T = r.ref(null),
+                    v = r.ref(null),
+                    y = s.wsClient || (d == null ? void 0 : d.client),
                     S = {},
                     g = {},
                     M = {},
-                    m = s.ref(1);
-                let o = null,
+                    m = r.ref(1);
+                let n = null,
                     w = 0,
                     b = null;
 
-                function E([e]) {
+                function R([e]) {
                     if (e.type === "state") {
                         const {
                             mtime: i,
-                            content: n,
+                            content: o,
                             id: t
                         } = e;
-                        o.unRegisterState(t), o.registerState(n), S[t] = i
+                        n.unRegisterState(t), n.registerState(o), S[t] = i
                     }
                     if (e.type === "blob") {
                         const {
                             hash: i,
-                            content: n
+                            content: o
                         } = e;
                         M[i] = new Promise(t => {
-                            n.arrayBuffer ? n.arrayBuffer().then(a => {
-                                o.registerBlob(i, new Uint8Array(a)), t()
-                            }) : (o.registerBlob(i, n), t())
+                            o.arrayBuffer ? o.arrayBuffer().then(a => {
+                                n.registerBlob(i, new Uint8Array(a)), t()
+                            }) : (n.registerBlob(i, o), t())
                         })
                     }
                 }
-                async function U() {
+                async function E() {
                     const e = y.getConnection().getSession();
-                    b = e.subscribe("vtklocal.subscriptions", E), await e.call("vtklocal.subscribe.update", [r.renderWindow, 1])
+                    b = e.subscribe("vtklocal.subscriptions", R), await e.call("vtklocal.subscribe.update", [s.renderWindow, 1])
                 }
-                async function C() {
+                async function U() {
                     const e = y.getConnection().getSession();
-                    b && (e.unsubscribe(b), b = null), await e.call("vtklocal.subscribe.update", [r.renderWindow, -1])
+                    b && (e.unsubscribe(b), b = null), await e.call("vtklocal.subscribe.update", [s.renderWindow, -1])
                 }
 
-                function O() {
+                function k() {
                     const {
                         width: e,
                         height: i
-                    } = T.value.getBoundingClientRect(), n = Math.floor(e * window.devicePixelRatio + .5), t = Math.floor(i * window.devicePixelRatio + .5), a = s.unref(v);
-                    a && o && r.renderWindow && (a.width = n, a.height = t, o.setSize(r.renderWindow, n, t), o.render(r.renderWindow))
+                    } = T.value.getBoundingClientRect(), o = Math.floor(e * window.devicePixelRatio + .5), t = Math.floor(i * window.devicePixelRatio + .5), a = r.unref(v);
+                    a && n && s.renderWindow && (a.width = o, a.height = t, n.setSize(s.renderWindow, o, t), n.render(s.renderWindow))
                 }
-                let h = new ResizeObserver(O);
+                let h = new ResizeObserver(k);
                 async function z(e) {
-                    const n = await y.getConnection().getSession().call("vtklocal.get.state", [e]);
-                    return n.length > 0 ? (S[e] = JSON.parse(n).MTime, o.unRegisterState(e), o.registerState(n)) : console.log(`Server returned empty state for ${e}`), n
+                    const o = await y.getConnection().getSession().call("vtklocal.get.state", [e]);
+                    return o.length > 0 ? (S[e] = JSON.parse(o).MTime, n.unRegisterState(e), n.registerState(o)) : console.log(`Server returned empty state for ${e}`), o
                 }
                 async function A(e) {
                     if (M[e]) {
-                        await M[e], g[e] = s.unref(m), delete M[e];
+                        await M[e], g[e] = r.unref(m), delete M[e];
                         return
                     }
-                    const n = await y.getConnection().getSession().call("vtklocal.get.hash", [e]),
-                        t = n.arrayBuffer ? new Uint8Array(await n.arrayBuffer()) : n;
-                    return o.registerBlob(e, t), g[e] = s.unref(m), t
+                    const o = await y.getConnection().getSession().call("vtklocal.get.hash", [e]),
+                        t = o.arrayBuffer ? new Uint8Array(await o.arrayBuffer()) : o;
+                    return n.registerBlob(e, t), g[e] = r.unref(m), t
                 }
 
                 function V() {
-                    const e = o.getTotalVTKDataObjectMemoryUsage(),
-                        i = o.getTotalBlobMemoryUsage(),
-                        n = Number(r.cacheSize) + e;
-                    if (i > n) {
+                    const e = n.getTotalVTKDataObjectMemoryUsage(),
+                        i = n.getTotalBlobMemoryUsage(),
+                        o = Number(s.cacheSize) + e;
+                    if (i > o) {
                         const t = {};
-                        let a = s.unref(m);
+                        let a = r.unref(m);
                         for (Object.entries(g).forEach(([f, l]) => {
                                 l < a && (a = l);
-                                const j = l.toString();
-                                t[j] ? t[j].push(f) : t[j] = [f]
-                            }); o.getTotalBlobMemoryUsage() > n;) {
+                                const W = l.toString();
+                                t[W] ? t[W].push(f) : t[W] = [f]
+                            }); n.getTotalBlobMemoryUsage() > o;) {
                             const f = t[a];
                             if (f)
-                                for (let l = 0; l < f.length; l++) o.unRegisterBlob(f[l]), delete g[f[l]];
+                                for (let l = 0; l < f.length; l++) n.unRegisterBlob(f[l]), delete g[f[l]];
                             a++
                         }
                     }
-                    c("memory-vtk", o.getTotalVTKDataObjectMemoryUsage()), c("memory-arrays", o.getTotalBlobMemoryUsage())
+                    c("memory-vtk", n.getTotalVTKDataObjectMemoryUsage()), c("memory-arrays", n.getTotalBlobMemoryUsage())
                 }
                 async function B() {
                     if (w++, w === 1) try {
-                        const i = await y.getConnection().getSession().call("vtklocal.get.status", [r.renderWindow]),
-                            n = [];
+                        const i = await y.getConnection().getSession().call("vtklocal.get.status", [s.renderWindow]),
+                            o = [];
                         i.ids.forEach(([t, a]) => {
-                            (!S[t] || S[t] < a) && n.push(z(t))
+                            (!S[t] || S[t] < a) && o.push(z(t))
                         }), i.ignore_ids.forEach(t => {
-                            o.unRegisterState(t)
+                            n.unRegisterState(t)
                         }), i.hashes.forEach(t => {
-                            g[t] || n.push(A(t)), g[t] = s.unref(m)
-                        }), await Promise.all(n), m.value++;
+                            g[t] || o.push(A(t)), g[t] = r.unref(m)
+                        }), await Promise.all(o), m.value++;
                         try {
-                            o.updateObjectsFromStates(), O()
+                            n.updateObjectsFromStates(), n.render(s.renderWindow), k()
                         } catch (t) {
                             console.error("WASM update failed"), console.log(t)
                         }
                         c("updated"), V()
                     } catch (e) {
                         console.error("Error in update", e)
                     } finally {
                         w--, w && (w = 0, await B())
                     }
                 }
-                return s.onMounted(async () => {
-                    o = await W(s.unref(v), p), r.eagerSync && U(), await B(), o.startEventLoop(r.renderWindow), h && h.observe(s.unref(T))
-                }), s.onBeforeUnmount(() => {
-                    b && C(), o.stopEventLoop(r.renderWindow), h && (h.disconnect(), h = null)
+
+                function _(e) {
+                    n.resetCamera(e), n.render(s.renderWindow)
+                }
+                return r.onMounted(async () => {
+                    n = await O(r.unref(v), p), s.eagerSync && E(), await B(), n.startEventLoop(s.renderWindow), h && h.observe(r.unref(T))
+                }), r.onBeforeUnmount(() => {
+                    b && U(), n.stopEventLoop(s.renderWindow), h && (h.disconnect(), h = null)
                 }), {
                     container: T,
                     canvas: v,
-                    update: B
+                    update: B,
+                    resetCamera: _
                 }
             },
             template: `
         <div ref="container" style="position: relative; width: 100%; height: 100%;">
           <canvas 
             id="canvas"
             ref="canvas" 
@@ -170,16 +175,16 @@
             @click="canvas.focus()"
             @mouseenter="canvas.focus()"
           />
         </div>`
         }
     };
 
-    function R(r) {
-        Object.keys(k).forEach(c => {
-            r.component(c, k[c])
+    function C(s) {
+        Object.keys(j).forEach(c => {
+            s.component(c, j[c])
         })
     }
-    u.install = R, Object.defineProperty(u, Symbol.toStringTag, {
+    u.install = C, Object.defineProperty(u, Symbol.toStringTag, {
         value: "Module"
     })
 });
```

### Comparing `trame-vtklocal-0.3.2/trame_vtklocal/widgets/vtklocal.py` & `trame-vtklocal-0.3.3/trame_vtklocal/widgets/vtklocal.py`

 * *Files 8% similar despite different names*

```diff
@@ -129,19 +129,26 @@
                     "index.json",
                     json.dumps(json_structure),
                     compress_type=ZIP_COMPRESSION,
                 )
 
             return zip_buffer.getvalue()
 
-    def reset_camera(self, **kwargs):
-        self._render_window.GetRenderers().GetFirstRenderer().ResetCamera()
-        self._render_window.Render()
-        self.object_manager.UpdateStatesFromObjects()
-        self.update()
+    def reset_camera(self, renderer_or_render_window=None, **kwargs):
+        if renderer_or_render_window is None:
+            renderer_or_render_window = self._render_window
+
+        if renderer_or_render_window.IsA("vtkRenderWindow"):
+            renderer_or_render_window = (
+                renderer_or_render_window.GetRenderers().GetFirstRenderer()
+            )
+
+        if renderer_or_render_window.IsA("vtkRenderer"):
+            id_to_reset_camera = self.get_wasm_id(renderer_or_render_window)
+            self.server.js_call(self.__ref, "resetCamera", id_to_reset_camera)
 
     @property
     def ref_name(self):
         return self.__ref
 
     def get_wasm_id(self, vtk_object):
         return self.object_manager.GetId(vtk_object)
```

### Comparing `trame-vtklocal-0.3.2/trame_vtklocal.egg-info/PKG-INFO` & `trame-vtklocal-0.3.3/trame_vtklocal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-vtklocal
-Version: 0.3.2
+Version: 0.3.3
 Summary: VTK Local Rendering using WASM
 Author: Kitware Inc.
 License: Apache Software License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
@@ -35,15 +35,15 @@
 .. code-block:: console
 
     pip install trame-vtklocal 
 
     # We need a VTK that has its wasm counterpart
     # This is the first version available with it
     # For ParaView (not yet supported), VTK don't need to be installed
-    pip install "vtk==9.3.20240418.dev0" --extra-index-url https://wheels.vtk.org
+    pip install "vtk==9.3.20240525.dev0" --extra-index-url https://wheels.vtk.org
 
 
 Development
 ----------------------------------------
 
 Build and install the Vue components
```

### Comparing `trame-vtklocal-0.3.2/trame_vtklocal.egg-info/SOURCES.txt` & `trame-vtklocal-0.3.3/trame_vtklocal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

