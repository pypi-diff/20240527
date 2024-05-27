# Comparing `tmp/d3vis_ipynb-0.2.2.tar.gz` & `tmp/d3vis_ipynb-0.2.3.tar.gz`

## Comparing `d3vis_ipynb-0.2.2.tar` & `d3vis_ipynb-0.2.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/D3vis_ipynb.json
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/MANIFEST.in
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/RELEASE.md
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/install.json
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/setup.cfg
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/setup.py
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/d3vis_ipynb/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/d3vis_ipynb/_version.py
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/d3vis_ipynb/custom.py
--rw-r--r--   0        0        0     4921 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/d3vis_ipynb/embedding.py
--rw-r--r--   0        0        0     6868 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/d3vis_ipynb/widgets.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/d3vis_ipynb/labextension/package.json
--rw-r--r--   0        0        0    32478 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/d3vis_ipynb/labextension/static/112.a36093df8a8075509d10.js
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/d3vis_ipynb/labextension/static/493.9def85d738cd0e72c5f5.js
--rw-r--r--   0        0        0   282230 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/d3vis_ipynb/labextension/static/693.c8409ce8329f6703470f.js
--rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/d3vis_ipynb/labextension/static/remoteEntry.6f9edec5dc6ff6501b02.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/d3vis_ipynb/labextension/static/style.js
--rw-r--r--   0        0        0    35163 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/d3vis_ipynb/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0    98223 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/d3vis_ipynb/nbextension/index.js
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/README.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/amd-public-path.js
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/package.json
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/webpack.config.js
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/webpack.exports.config.js
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/css/widget.css
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/lib/extension.js
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/lib/index.js
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/lib/labplugin.js
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/lib/web-dev.js
--rw-r--r--   0        0        0    15340 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/lib/widgets.js
--rw-r--r--   0        0        0     9163 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/lib/graphs/barplot.js
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/lib/graphs/histogramplot.js
--rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/lib/graphs/linearhistplot.js
--rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/lib/graphs/linearplot.js
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/lib/graphs/rangeslider.js
--rw-r--r--   0        0        0     4410 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/lib/graphs/scatterplot.js
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/lib/tools/group_data.js
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/lib/tools/lasso.js
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/.gitignore
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/LICENSE.txt
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/README.md
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/D3vis_ipynb.json
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/MANIFEST.in
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/RELEASE.md
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/install.json
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/setup.cfg
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/setup.py
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/d3vis_ipynb/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/d3vis_ipynb/_version.py
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/d3vis_ipynb/custom.py
+-rw-r--r--   0        0        0     4921 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/d3vis_ipynb/embedding.py
+-rw-r--r--   0        0        0     6868 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/d3vis_ipynb/widgets.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/d3vis_ipynb/labextension/package.json
+-rw-r--r--   0        0        0    32688 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/d3vis_ipynb/labextension/static/112.3054f9386990c9655128.js
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/d3vis_ipynb/labextension/static/493.9def85d738cd0e72c5f5.js
+-rw-r--r--   0        0        0   282230 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/d3vis_ipynb/labextension/static/693.c8409ce8329f6703470f.js
+-rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/d3vis_ipynb/labextension/static/remoteEntry.113ae5fdcfdb6db5a7b5.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/d3vis_ipynb/labextension/static/style.js
+-rw-r--r--   0        0        0    35163 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/d3vis_ipynb/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    98433 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/d3vis_ipynb/nbextension/index.js
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/js/README.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/js/amd-public-path.js
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/js/package.json
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/js/webpack.config.js
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/js/webpack.exports.config.js
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/js/css/widget.css
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/js/lib/extension.js
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/js/lib/index.js
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/js/lib/labplugin.js
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/js/lib/web-dev.js
+-rw-r--r--   0        0        0    15730 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/js/lib/widgets.js
+-rw-r--r--   0        0        0     9163 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/js/lib/graphs/barplot.js
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/js/lib/graphs/histogramplot.js
+-rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/js/lib/graphs/linearhistplot.js
+-rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/js/lib/graphs/linearplot.js
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/js/lib/graphs/rangeslider.js
+-rw-r--r--   0        0        0     4410 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/js/lib/graphs/scatterplot.js
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/js/lib/tools/group_data.js
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/js/lib/tools/lasso.js
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/LICENSE.txt
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/README.md
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.3/PKG-INFO
```

### Comparing `d3vis_ipynb-0.2.2/RELEASE.md` & `d3vis_ipynb-0.2.3/RELEASE.md`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.2/setup.cfg` & `d3vis_ipynb-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.2/d3vis_ipynb/__init__.py` & `d3vis_ipynb-0.2.3/d3vis_ipynb/__init__.py`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.2/d3vis_ipynb/custom.py` & `d3vis_ipynb-0.2.3/d3vis_ipynb/custom.py`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.2/d3vis_ipynb/embedding.py` & `d3vis_ipynb-0.2.3/d3vis_ipynb/embedding.py`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.2/d3vis_ipynb/widgets.py` & `d3vis_ipynb-0.2.3/d3vis_ipynb/widgets.py`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.2/d3vis_ipynb/labextension/package.json` & `d3vis_ipynb-0.2.3/d3vis_ipynb/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9603365384615384%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.113ae5fdcfdb6db5a7b5.js'}}",*

 * * "'version'": "'0.2.3'"}*

```diff
@@ -16,15 +16,15 @@
         "lib/**/*.js",
         "dist/*.js",
         "css/*.css"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.6f9edec5dc6ff6501b02.js"
+            "load": "static/remoteEntry.113ae5fdcfdb6db5a7b5.js"
         },
         "extension": "lib/labplugin",
         "outputDir": "../d3vis_ipynb/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -52,9 +52,9 @@
         "build:prod": "webpack --mode=production && yarn run build:labextension",
         "clean": "rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension",
         "prepublish": "yarn run clean && yarn run build:prod",
         "start": "webpack serve --open --config webpack.exports.config.js",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch --mode=development"
     },
-    "version": "0.2.2"
+    "version": "0.2.3"
 }
```

### Comparing `d3vis_ipynb-0.2.2/d3vis_ipynb/labextension/static/112.a36093df8a8075509d10.js` & `d3vis_ipynb-0.2.3/d3vis_ipynb/labextension/static/112.3054f9386990c9655128.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,23 +1,23 @@
 "use strict";
 (self.webpackChunkd3vis_ipynb = self.webpackChunkd3vis_ipynb || []).push([
     [112], {
         112: (e, t, n) => {
             n.r(t), n.d(t, {
                 BarPlotModel: () => j,
                 BarPlotView: () => C,
-                EmbeddingModel: () => B,
-                EmbeddingView: () => W,
+                EmbeddingModel: () => P,
+                EmbeddingView: () => B,
                 HistogramPlotModel: () => R,
                 HistogramPlotView: () => I,
                 LinearHistPlotModel: () => E,
                 LinearHistPlotView: () => S,
                 LinearPlotModel: () => D,
                 LinearPlotView: () => O,
-                RangeSliderModel: () => P,
+                RangeSliderModel: () => W,
                 RangeSliderView: () => H,
                 ScatterPlotModel: () => V,
                 ScatterPlotView: () => A,
                 author: () => T.author,
                 dependencies: () => T.dependencies,
                 description: () => T.description,
                 devDependencies: () => T.devDependencies,
@@ -35,46 +35,46 @@
                 i = n(72),
                 o = n.n(i),
                 s = n(825),
                 r = n.n(s),
                 l = n(659),
                 d = n.n(l),
                 c = n(56),
-                m = n.n(c),
-                u = n(540),
-                p = n.n(u),
+                u = n.n(c),
+                m = n(540),
+                p = n.n(m),
                 h = n(113),
-                g = n.n(h),
-                f = n(930),
+                f = n.n(h),
+                g = n(930),
                 v = {};
-            v.styleTagTransform = g(), v.setAttributes = m(), v.insert = d().bind(null, "head"), v.domAPI = r(), v.insertStyleElement = p(), o()(f.A, v), f.A && f.A.locals && f.A.locals;
+            v.styleTagTransform = f(), v.setAttributes = u(), v.insert = d().bind(null, "head"), v.domAPI = r(), v.insertStyleElement = p(), o()(g.A, v), g.A && g.A.locals && g.A.locals;
             var _ = n(840);
 
             function x(e) {
                 const t = e.reduce(((e, t) => e + t), 0) / e.length,
                     n = 1.96 * function(e, t) {
                         let n = 0;
                         return e.forEach((e => n += (e - t) ** 2)), n = Math.sqrt(n) / e.length, n
                     }(e, t);
                 return [t - n, t + n]
             }
 
             function y(e, t, n, a, i, o, s, r, l, d) {
                 let c = [];
-                const m = _.line(),
-                    u = _.select(e).selectAll(".dot"),
+                const u = _.line(),
+                    m = _.select(e).selectAll(".dot"),
                     p = _.drag().on("start", (function() {
                         c = [], r(), _.select(e).select("svg").append("path").attr("id", "lasso" + d)
                     })).on("drag", (function(e) {
                         let t = e.sourceEvent.offsetX,
                             n = e.sourceEvent.offsetY;
-                        c.push([t, n]), _.select("#lasso" + d).style("stroke", "blue").style("stroke-width", 2).style("fill", "#00008854").attr("d", m(c))
+                        c.push([t, n]), _.select("#lasso" + d).style("stroke", "blue").style("stroke-width", 2).style("fill", "#00008854").attr("d", u(c))
                     })).on("end", (function() {
                         let e = [];
-                        u.each(((r, l) => {
+                        m.each(((r, l) => {
                             (function(e, t) {
                                 for (var n = e[0], a = e[1], i = !1, o = 0, s = t.length - 1; o < t.length; s = o++) {
                                     var r = t[o][0],
                                         l = t[o][1],
                                         d = t[s][0],
                                         c = t[s][1];
                                     l > a != c > a && n < (d - r) * (a - l) / (c - l) + r && (i = !i)
@@ -136,43 +136,44 @@
                 timeout;
                 render() {
                     L(this), this.model.on("change:linearData_x", (() => L(this)), this), this.model.on("change:linearData_y", (() => L(this)), this), this.model.on("change:histogramData", (() => L(this)), this), window.addEventListener("resize", (() => L(this)))
                 }
                 plot() {
                     const e = this.model.get("linearData_x"),
                         t = this.model.get("linearData_y"),
-                        n = this.model.get("histogramData"),
-                        a = this.model.get("elementId");
+                        n = this.model.get("histogramData");
+                    let a = this.model.get("elementId");
+                    "function" == typeof a && (a = a());
                     let i = k,
                         o = this.el;
                     a && (o = document.getElementById(a), i = o.clientHeight);
                     let s = o.clientWidth;
                     const r = M;
                     ! function(e, t, n, a, i, o, s, r) {
                         const l = o - r.left - r.right,
                             d = s - r.top - r.bottom,
                             c = d / 4;
                         _.select(a).selectAll("*").remove();
-                        const m = Math.min(_.min(e), _.min(n)),
-                            u = Math.max(_.max(e), _.max(n)),
+                        const u = Math.min(_.min(e), _.min(n)),
+                            m = Math.max(_.max(e), _.max(n)),
                             p = _.scaleLinear().range([0, l]),
                             h = _.scaleLinear().range([d, 0]),
-                            g = _.scaleLinear().range([c, 0]),
-                            f = _.axisBottom(p),
+                            f = _.scaleLinear().range([c, 0]),
+                            g = _.axisBottom(p),
                             v = _.axisLeft(h),
                             x = _.bin().thresholds(20).value((e => Math.round(10 * e) / 10))(n),
                             y = _.select(a).append("svg").attr("width", o).attr("height", s).append("g").attr("transform", "translate(" + r.left + "," + r.top + ")");
-                        p.domain([m, u]), h.domain(_.extent(t)), g.domain([0, _.max(x, (e => e.length))]);
+                        p.domain([u, m]), h.domain(_.extent(t)), f.domain([0, _.max(x, (e => e.length))]);
                         const b = y.append("g").append("rect").style("fill", "none").attr("width", 160).attr("height", 40).attr("stroke", "#69b3a2").attr("stroke-width", 4).style("opacity", 0),
                             w = y.append("g").append("text").style("opacity", 0).attr("text-anchor", "left").attr("alignment-baseline", "middle");
-                        y.append("g").attr("transform", "translate(0," + d + ")").call(f).append("text").attr("x", l).attr("y", -6).style("text-anchor", "end"), y.append("g").call(v).append("text").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end");
+                        y.append("g").attr("transform", "translate(0," + d + ")").call(g).append("text").attr("x", l).attr("y", -6).style("text-anchor", "end"), y.append("g").call(v).append("text").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end");
                         const k = [];
                         k.x0 = x[0].x0 - 2.5, k.x1 = x[0].x1 - 2.5, x.unshift(k);
                         const M = [];
-                        M.x0 = x[x.length - 1].x0 + 2.5, M.x1 = x[x.length - 1].x1 + 2.5, y.append("path").datum(x).attr("fill", "paleturquoise").attr("stroke", "steelblue").attr("stroke-width", 1).attr("d", _.line().x((e => p((e.x1 + e.x0) / 2))).y((e => g(e.length) + d - c)).curve(_.curveCatmullRom));
+                        M.x0 = x[x.length - 1].x0 + 2.5, M.x1 = x[x.length - 1].x1 + 2.5, y.append("path").datum(x).attr("fill", "paleturquoise").attr("stroke", "steelblue").attr("stroke-width", 1).attr("d", _.line().x((e => p((e.x1 + e.x0) / 2))).y((e => f(e.length) + d - c)).curve(_.curveCatmullRom));
                         const L = e.map(((e, n) => [e, t[n]])).map((([e, t]) => ({
                             x: e,
                             y: t
                         })));
                         y.append("path").datum(L).attr("fill", "none").attr("stroke", "steelblue").attr("stroke-width", 1.5).attr("d", _.line().x((e => p(e.x))).y((e => h(e.y)))), y.selectAll("myCircles").data(L).enter().append("circle").attr("fill", "red").attr("stroke", "none").attr("cx", (e => p(e.x))).attr("cy", (e => h(e.y))).attr("r", 3).on("mouseover", (function(e, t) {
                             b.style("opacity", 1), w.style("opacity", 1), b.attr("x", e.offsetX - 30).attr("y", e.offsetY - 40), w.html("x:" + Math.round(10 * t.x) / 10 + "  -  y:" + Math.round(10 * t.y) / 10).attr("x", e.offsetX - 15).attr("y", e.offsetY - 20)
                         })).on("mouseout", (function() {
@@ -220,63 +221,64 @@
                 render() {
                     L(this), this.model.on("change:dataRecords", (() => L(this)), this), this.model.on("change:x", (() => L(this)), this), this.model.on("change:y", (() => L(this)), this), this.model.on("change:hue", (() => L(this)), this), window.addEventListener("resize", (() => L(this)))
                 }
                 plot() {
                     const e = this.model.get("dataRecords"),
                         t = this.model.get("x"),
                         n = this.model.get("y"),
-                        a = this.model.get("hue"),
-                        i = this.model.get("elementId");
+                        a = this.model.get("hue");
+                    let i = this.model.get("elementId");
+                    "function" == typeof i && (i = i());
                     let o = k,
                         s = this.el;
                     i && (s = document.getElementById(i), o = s.clientHeight);
                     let r = s.clientWidth;
                     const l = M;
                     ! function(e, t, n, a, i, o, s, r, l, d) {
                         const c = r - d.left - d.right,
-                            m = l - d.top - d.bottom;
+                            u = l - d.top - d.bottom;
                         for (let t = 0; t < e.length; t++) e[t].id = t;
-                        const u = Math.floor(Math.random() * Date.now() * 1e4).toString(36);
+                        const m = Math.floor(Math.random() * Date.now() * 1e4).toString(36);
                         _.select(i).selectAll("*").remove();
                         const p = _.scaleLinear().range([0, c]),
-                            h = _.scaleLinear().range([m, 0]),
-                            g = _.scaleOrdinal(_.schemeCategory10),
-                            f = _.axisBottom(p),
+                            h = _.scaleLinear().range([u, 0]),
+                            f = _.scaleOrdinal(_.schemeCategory10),
+                            g = _.axisBottom(p),
                             v = _.axisLeft(h),
                             x = _.select(i).append("svg").attr("width", r).attr("height", l).append("g").attr("transform", "translate(" + d.left + "," + d.top + ")");
                         if (p.domain(_.extent(e, (function(e) {
                                 return e[t]
                             }))).nice(), h.domain(_.extent(e, (function(e) {
                                 return e[n]
-                            }))).nice(), x.append("g").attr("class", "x axis").attr("transform", "translate(0," + m + ")").call(f).append("text").attr("class", "label").attr("x", c).attr("y", -6).style("text-anchor", "end"), x.append("g").attr("class", "y axis").call(v).append("text").attr("class", "label").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), x.selectAll(".dot").data(e).enter().append("circle").attr("id", (function(e, t) {
-                                return "dot-" + u + e.id
+                            }))).nice(), x.append("g").attr("class", "x axis").attr("transform", "translate(0," + u + ")").call(g).append("text").attr("class", "label").attr("x", c).attr("y", -6).style("text-anchor", "end"), x.append("g").attr("class", "y axis").call(v).append("text").attr("class", "label").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), x.selectAll(".dot").data(e).enter().append("circle").attr("id", (function(e, t) {
+                                return "dot-" + m + e.id
                             })).attr("class", "dot").attr("r", 3.5).attr("cx", (function(e) {
                                 return p(e[t])
                             })).attr("cy", (function(e) {
                                 return h(e[n])
                             })).style("fill", (function(e) {
-                                return g(e[a])
+                                return f(e[a])
                             })).on("mouseover", (function(e, a) {
                                 b.style("opacity", 1), w.style("opacity", 1), b.attr("x", e.offsetX - 30).attr("y", e.offsetY - 40), w.html("x: " + Math.round(10 * a[t]) / 10 + "&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;y: " + Math.round(10 * a[n]) / 10).attr("x", e.offsetX - 15).attr("y", e.offsetY - 20)
                             })).on("mouseout", (function() {
                                 b.style("opacity", 0), w.style("opacity", 0)
                             })).on("click", (function(e, a) {
                                 const i = "x:" + Math.round(10 * a[t]) / 10 + "    y:" + Math.round(10 * a[n]) / 10;
                                 void 0 !== o && o(i)
                             })), y(i, p, h, t, n, d.left, d.top, (function() {
                                 x.selectAll(".dot").data(e).attr("r", 3.5).style("fill", (function(e) {
-                                    return g(e[a])
+                                    return f(e[a])
                                 }))
                             }), (function(e) {
                                 void 0 !== s && s(e)
-                            }), u), a) {
-                            const e = x.selectAll(".legend").data(g.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(e, t) {
+                            }), m), a) {
+                            const e = x.selectAll(".legend").data(f.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(e, t) {
                                 return "translate(0," + 20 * t + ")"
                             }));
-                            e.append("rect").attr("x", c - 18).attr("width", 18).attr("height", 18).style("fill", g), e.append("text").attr("x", c - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(e) {
+                            e.append("rect").attr("x", c - 18).attr("width", 18).attr("height", 18).style("fill", f), e.append("text").attr("x", c - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(e) {
                                 return e
                             }))
                         }
                         const b = x.append("g").append("rect").style("fill", "none").attr("width", 160).attr("height", 40).attr("stroke", "#69b3a2").attr("stroke-width", 4).style("opacity", 0),
                             w = x.append("g").append("text").style("opacity", 0).attr("text-anchor", "left").attr("alignment-baseline", "middle")
                     }(e, t, n, a, s, this.setValue.bind(this), this.setSelectedValues.bind(this), r, o, l)
                 }
@@ -322,24 +324,25 @@
                 render() {
                     L(this), this.model.on("change:dataRecords", (() => L(this)), this), this.model.on("change:x", (() => L(this)), this), this.model.on("change:y", (() => L(this)), this), this.model.on("change:hue", (() => L(this)), this), window.addEventListener("resize", (() => L(this)))
                 }
                 plot() {
                     const e = this.model.get("dataRecords"),
                         t = this.model.get("x"),
                         n = this.model.get("y"),
-                        a = this.model.get("hue"),
-                        i = this.model.get("elementId");
+                        a = this.model.get("hue");
+                    let i = this.model.get("elementId");
+                    "function" == typeof i && (i = i());
                     let o = k,
                         s = this.el;
                     i && (s = document.getElementById(i), o = s.clientHeight);
                     let r = s.clientWidth;
                     const l = M;
                     ! function(e, t, n, a, i, o, s, r, l, d) {
                         const c = r - d.left - d.right,
-                            m = l - d.top - d.bottom;
+                            u = l - d.top - d.bottom;
                         e = function(e, t, n, a) {
                             function i(e) {
                                 const i = e.reduce((function(e, i) {
                                         if (!e[i[t]]) {
                                             const o = {};
                                             return o[t] = i[t], o[n] = i[n], a && (o[a] = i[a]), o.count = 1, e[i[t]] = o, e
                                         }
@@ -363,62 +366,62 @@
                                 s = [];
                             return Object.values(o).forEach((function(e, t) {
                                 const n = i(e);
                                 s = s.concat(n)
                             })), s
                         }(e, t, [n], a);
                         for (let t = 0; t < e.length; t++) e[t].id = t;
-                        const u = Math.floor(Math.random() * Date.now() * 1e4).toString(36);
+                        const m = Math.floor(Math.random() * Date.now() * 1e4).toString(36);
                         _.select(i).selectAll("*").remove();
                         const p = _.scaleLinear().range([0, c]),
-                            h = _.scaleLinear().range([m, 0]),
-                            g = _.scaleOrdinal(_.schemeCategory10),
-                            f = _.axisBottom(p),
+                            h = _.scaleLinear().range([u, 0]),
+                            f = _.scaleOrdinal(_.schemeCategory10),
+                            g = _.axisBottom(p),
                             v = _.axisLeft(h),
                             x = _.select(i).append("svg").attr("width", r).attr("height", l).append("g").attr("transform", "translate(" + d.left + "," + d.top + ")");
 
                         function w(e, a) {
-                            x.append("path").datum(e).attr("fill", "none").attr("stroke", g(a)).attr("stroke-width", 2).attr("d", _.line().x((e => p(e[t]))).y((e => h(e[n]))))
+                            x.append("path").datum(e).attr("fill", "none").attr("stroke", f(a)).attr("stroke-width", 2).attr("d", _.line().x((e => p(e[t]))).y((e => h(e[n]))))
                         }
                         if (p.domain(_.extent(e, (function(e) {
                                 return e[t]
                             }))).nice(), h.domain(_.extent(e, (function(e) {
                                 return e[n]
-                            }))).nice(), x.append("g").attr("class", "x axis").attr("transform", "translate(0," + m + ")").call(f).append("text").attr("class", "label").attr("x", c).attr("y", -6).style("text-anchor", "end"), x.append("g").attr("class", "y axis").call(v).append("text").attr("class", "label").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), a) {
+                            }))).nice(), x.append("g").attr("class", "x axis").attr("transform", "translate(0," + u + ")").call(g).append("text").attr("class", "label").attr("x", c).attr("y", -6).style("text-anchor", "end"), x.append("g").attr("class", "y axis").call(v).append("text").attr("class", "label").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), a) {
                             const t = b(e, a);
                             Object.keys(t).forEach((function(e, n) {
                                 w(t[e], e)
                             }))
                         } else w(e);
                         if (x.selectAll(".dot").data(e).enter().append("circle").attr("id", (function(e, t) {
-                                return "dot-" + u + e.id
+                                return "dot-" + m + e.id
                             })).attr("class", "dot").attr("r", 3.5).attr("cx", (function(e) {
                                 return p(e[t])
                             })).attr("cy", (function(e) {
                                 return h(e[n])
                             })).style("fill", (function(e) {
-                                return g(e[a])
+                                return f(e[a])
                             })).on("mouseover", (function(e, a) {
                                 k.style("opacity", 1), M.style("opacity", 1), k.attr("x", e.offsetX - 30).attr("y", e.offsetY - 40), M.html("x: " + Math.round(10 * a[t]) / 10 + "&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;y: " + Math.round(10 * a[n]) / 10).attr("x", e.offsetX - 15).attr("y", e.offsetY - 20)
                             })).on("mouseout", (function() {
                                 k.style("opacity", 0), M.style("opacity", 0)
                             })).on("click", (function(e, a) {
                                 const i = "x:" + Math.round(10 * a[t]) / 10 + "    y:" + Math.round(10 * a[n]) / 10;
                                 void 0 !== o && o(i)
                             })), y(i, p, h, t, n, d.left, d.top, (function() {
                                 x.selectAll(".dot").data(e).attr("r", 3.5).style("fill", (function(e) {
-                                    return g(e[a])
+                                    return f(e[a])
                                 }))
                             }), (function(e) {
                                 void 0 !== s && s(e)
-                            }), u), a) {
-                            const e = x.selectAll(".legend").data(g.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(e, t) {
+                            }), m), a) {
+                            const e = x.selectAll(".legend").data(f.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(e, t) {
                                 return "translate(0," + 20 * t + ")"
                             }));
-                            e.append("rect").attr("x", c - 18).attr("width", 18).attr("height", 18).style("fill", g), e.append("text").attr("x", c - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(e) {
+                            e.append("rect").attr("x", c - 18).attr("width", 18).attr("height", 18).style("fill", f), e.append("text").attr("x", c - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(e) {
                                 return e
                             }))
                         }
                         const k = x.append("g").append("rect").style("fill", "none").attr("width", 160).attr("height", 40).attr("stroke", "#69b3a2").attr("stroke-width", 4).style("opacity", 0),
                             M = x.append("g").append("text").style("opacity", 0).attr("text-anchor", "left").attr("alignment-baseline", "middle")
                     }(e, t, n, a, s, this.setValue.bind(this), this.setSelectedValues.bind(this), r, o, l)
                 }
@@ -446,188 +449,189 @@
                         dataRecords: [],
                         x: String,
                         y: String,
                         hue: String,
                         elementId: String
                     }
                 }
-                static model_name = "BarplotModel";
+                static model_name = "BarPlotModel";
                 static model_module = w.name;
                 static model_module_version = w.version;
-                static view_name = "BarplotView";
+                static view_name = "BarPlotView";
                 static view_module = w.name;
                 static view_module_version = w.version
             }
             class C extends a.DOMWidgetView {
                 timeout;
                 render() {
                     L(this), this.model.on("change:dataRecords", (() => L(this)), this), this.model.on("change:x", (() => L(this)), this), this.model.on("change:y", (() => L(this)), this), this.model.on("change:hue", (() => L(this)), this), window.addEventListener("resize", (() => L(this)))
                 }
                 plot() {
                     const e = this.model.get("dataRecords"),
                         t = this.model.get("x"),
                         n = this.model.get("y"),
-                        a = this.model.get("hue"),
-                        i = this.model.get("elementId");
+                        a = this.model.get("hue");
+                    let i = this.model.get("elementId");
+                    "function" == typeof i && (i = i());
                     let o = k,
                         s = this.el;
                     i && (s = document.getElementById(i), o = s.clientHeight),
                         function(e, t, n, a, i, o, s, r) {
                             const l = o - r.left - r.right,
                                 d = s - r.top - r.bottom;
                             _.select(i).selectAll("*").remove();
                             const c = _.select(i).append("svg").attr("width", o).attr("height", s).append("g").attr("transform", "translate(" + r.left + "," + r.top + ")");
                             a || (a = t);
-                            const m = e.reduce(((e, t) => (e && -1 === e.indexOf(t[a]) && e.push(t[a]), e)), []),
-                                u = {},
+                            const u = e.reduce(((e, t) => (e && -1 === e.indexOf(t[a]) && e.push(t[a]), e)), []),
+                                m = {},
                                 p = _.scaleOrdinal(_.schemeCategory10);
                             a == t ? function() {
                                 let a = e.reduce(((e, a) => {
                                     const i = a[t],
                                         o = a[n];
-                                    if (i in e) e[i] += o, u[i].qt += 1, u[i][n].push(o);
+                                    if (i in e) e[i] += o, m[i].qt += 1, m[i][n].push(o);
                                     else {
                                         const t = {
                                             qt: 1
                                         };
-                                        t[n] = [], t[n].push(o), u[i] = t, e[i] = o
+                                        t[n] = [], t[n].push(o), m[i] = t, e[i] = o
                                     }
                                     return e
                                 }), {});
                                 a = Object.keys(a).map((e => {
                                     const i = {};
-                                    return i[t] = e, i[n] = a[e], 0 != u[e].qt && (i[n] = i[n] / u[e].qt), i
-                                })), Object.keys(u).forEach((e => {
-                                    const t = u[e][n],
+                                    return i[t] = e, i[n] = a[e], 0 != m[e].qt && (i[n] = i[n] / m[e].qt), i
+                                })), Object.keys(m).forEach((e => {
+                                    const t = m[e][n],
                                         [a, i] = x(t);
-                                    u[e].min = a, u[e].max = i
+                                    m[e].min = a, m[e].max = i
                                 }));
                                 const i = a.map((e => e[t])),
                                     o = [],
-                                    s = Object.keys(u).map((e => u[e]));
+                                    s = Object.keys(m).map((e => m[e]));
                                 o.push(_.min(s, (e => e.min))), o.push(_.max(s, (e => e.max))), o[0] > 0 && o[1] > 0 ? o[0] = 0 : o[0] < 0 && o[1] < 0 && (o[1] = 0);
                                 const r = _.scaleLinear().domain(o).range([d, 0]);
                                 c.append("g").call(_.axisLeft(r));
                                 const h = _.scaleBand().domain(i).range([0, l]).padding([.2]);
                                 c.append("g").selectAll("g").data(a).enter().append("rect").attr("x", (function(e) {
                                     return h(e[t])
                                 })).attr("y", (function(e) {
                                     return r(e[n]) < r(0) ? r(e[n]) : r(0)
                                 })).attr("width", h.bandwidth()).attr("height", (function(e) {
                                     return Math.abs(r(0) - r(e[n]))
-                                })).data(m).attr("fill", (function(e) {
+                                })).data(u).attr("fill", (function(e) {
                                     return p(e)
                                 }));
-                                const g = Object.keys(u).map((e => {
+                                const f = Object.keys(m).map((e => {
                                     const n = {};
-                                    return n[t] = e, n.min = u[e].min, n.max = u[e].max, n
+                                    return n[t] = e, n.min = m[e].min, n.max = m[e].max, n
                                 }));
-                                c.append("g").selectAll("g").data(g).enter().append("rect").attr("x", (function(e) {
+                                c.append("g").selectAll("g").data(f).enter().append("rect").attr("x", (function(e) {
                                     return h(e[t]) + h.bandwidth() / 2 - 1
                                 })).attr("y", (function(e) {
                                     return r(e.max)
                                 })).attr("width", 2).attr("height", (function(e) {
                                     return r(e.min) - r(e.max)
                                 })), c.append("g").style("font", "18px times").attr("transform", "translate(0," + r(0) + ")").call(_.axisBottom(h).tickSize(0))
                             }() : function() {
                                 let i = e.reduce(((e, i) => {
                                     const o = i[t],
                                         s = i[n],
                                         r = i[a];
                                     if (o in e) {
-                                        u[o].qt[n + "-" + r] += 1, u[o][r][n].push(s);
-                                        for (const t of m) r == t && (e[o][n + "-" + t] += s)
+                                        m[o].qt[n + "-" + r] += 1, m[o][r][n].push(s);
+                                        for (const t of u) r == t && (e[o][n + "-" + t] += s)
                                     } else {
                                         const t = {};
-                                        m.forEach((e => {
+                                        u.forEach((e => {
                                             t[e] = {}, t[e][n] = []
                                         }));
                                         const a = {};
-                                        for (const e of m) a[n + "-" + e] = 0;
-                                        a[n + "-" + r] = 1, t.qt = a, t[r][n].push(s), u[o] = t;
+                                        for (const e of u) a[n + "-" + e] = 0;
+                                        a[n + "-" + r] = 1, t.qt = a, t[r][n].push(s), m[o] = t;
                                         const i = {};
-                                        for (const e of m) i[n + "-" + e] = r == e ? s : 0;
+                                        for (const e of u) i[n + "-" + e] = r == e ? s : 0;
                                         e[o] = i
                                     }
                                     return e
                                 }), {});
                                 i = Object.keys(i).map((e => {
                                     let n = {};
                                     n[t] = e;
-                                    for (const t of Object.keys(i[e])) 0 != u[e].qt[t] && (i[e][t] = i[e][t] / u[e].qt[t]);
+                                    for (const t of Object.keys(i[e])) 0 != m[e].qt[t] && (i[e][t] = i[e][t] / m[e].qt[t]);
                                     return n = {
                                         ...n,
                                         ...i[e]
                                     }, n
-                                })), Object.keys(u).forEach((e => {
-                                    m.forEach((t => {
-                                        const a = u[e][t][n],
+                                })), Object.keys(m).forEach((e => {
+                                    u.forEach((t => {
+                                        const a = m[e][t][n],
                                             [i, o] = x(a);
-                                        u[e][t].min = i, u[e][t].max = o
+                                        m[e][t].min = i, m[e][t].max = o
                                     }))
                                 }));
-                                const o = m.map((e => n + "-" + e)),
+                                const o = u.map((e => n + "-" + e)),
                                     s = i.map((e => e[t])),
                                     r = [];
-                                Object.keys(u).map((e => {
-                                    m.forEach((t => r.push(u[e][t])))
+                                Object.keys(m).map((e => {
+                                    u.forEach((t => r.push(m[e][t])))
                                 }));
                                 const h = [];
                                 h.push(_.min(r, (e => e.min))), h.push(_.max(r, (e => e.max))), h[0] > 0 && h[1] > 0 ? h[0] = 0 : h[0] < 0 && h[1] < 0 && (h[1] = 0);
-                                const g = _.scaleLinear().domain(h).range([d, 0]);
-                                c.append("g").call(_.axisLeft(g));
-                                const f = _.scaleBand().domain(s).range([0, l]).padding([.2]),
-                                    v = _.scaleBand().domain(o).range([0, f.bandwidth()]).padding([.05]);
+                                const f = _.scaleLinear().domain(h).range([d, 0]);
+                                c.append("g").call(_.axisLeft(f));
+                                const g = _.scaleBand().domain(s).range([0, l]).padding([.2]),
+                                    v = _.scaleBand().domain(o).range([0, g.bandwidth()]).padding([.05]);
                                 c.append("g").selectAll("g").data(i).enter().append("g").attr("transform", (function(e) {
-                                    return "translate(" + f(e[t]) + ",0)"
+                                    return "translate(" + g(e[t]) + ",0)"
                                 })).selectAll("rect").data((function(e) {
                                     return o.map((function(t) {
                                         return {
                                             key: t,
                                             value: e[t]
                                         }
                                     }))
                                 })).enter().append("rect").attr("x", (function(e) {
                                     return v(e.key)
                                 })).attr("y", (function(e) {
-                                    return g(e.value) < g(0) ? g(e.value) : g(0)
+                                    return f(e.value) < f(0) ? f(e.value) : f(0)
                                 })).attr("width", v.bandwidth()).attr("height", (function(e) {
-                                    return Math.abs(g(0) - g(e.value))
-                                })).data(m).attr("fill", (function(e) {
+                                    return Math.abs(f(0) - f(e.value))
+                                })).data(u).attr("fill", (function(e) {
                                     return p(e)
                                 }));
-                                const y = Object.keys(u).map((e => {
+                                const y = Object.keys(m).map((e => {
                                     let n = {};
                                     return n[t] = e, n = {
                                         ...n,
-                                        ...u[e]
+                                        ...m[e]
                                     }, n
                                 }));
                                 c.append("g").selectAll("g").data(y).enter().append("g").attr("transform", (function(e) {
-                                    return "translate(" + f(e[t]) + ",0)"
+                                    return "translate(" + g(e[t]) + ",0)"
                                 })).selectAll("rect").data((function(e) {
-                                    return m.map((function(t) {
+                                    return u.map((function(t) {
                                         return {
                                             key: n + "-" + t,
                                             value: e[t]
                                         }
                                     }))
                                 })).enter().append("rect").attr("x", (function(e) {
                                     return v(e.key) + v.bandwidth() / 2 - 1
                                 })).attr("y", (function(e) {
-                                    return e.value.max ? g(e.value.max) : 0
+                                    return e.value.max ? f(e.value.max) : 0
                                 })).attr("width", 2).attr("height", (function(e) {
-                                    return e.value.min && e.value.max ? g(e.value.min) - g(e.value.max) : 0
+                                    return e.value.min && e.value.max ? f(e.value.min) - f(e.value.max) : 0
                                 }));
                                 const b = c.selectAll(".legend").data(p.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(e, t) {
                                     return "translate(0," + 20 * t + ")"
                                 }));
                                 b.append("rect").attr("x", l - 18).attr("width", 18).attr("height", 18).style("fill", p), b.append("text").attr("x", l - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(e) {
                                     return e
-                                })), c.append("g").style("font", "18px times").attr("transform", "translate(0," + g(0) + ")").call(_.axisBottom(f).tickSize(0))
+                                })), c.append("g").style("font", "18px times").attr("transform", "translate(0," + f(0) + ")").call(_.axisBottom(g).tickSize(0))
                             }()
                         }(e, t, n, a, s, s.clientWidth, o, M)
                 }
             }
             class R extends a.DOMWidgetModel {
                 defaults() {
                     return {
@@ -641,77 +645,78 @@
                         dataRecords: [],
                         x: String,
                         start: Number,
                         end: Number,
                         elementId: String
                     }
                 }
-                static model_name = "HistogramplotModel";
+                static model_name = "HistogramPlotModel";
                 static model_module = w.name;
                 static model_module_version = w.version;
-                static view_name = "HistogramplotView";
+                static view_name = "HistogramPlotView";
                 static view_module = w.name;
                 static view_module_version = w.version
             }
             class I extends a.DOMWidgetView {
                 timeout;
                 render() {
                     L(this), this.model.on("change:dataRecords", (() => L(this)), this), this.model.on("change:x", (() => L(this)), this), this.model.on("change:start", (() => L(this)), this), this.model.on("change:end", (() => L(this)), this), window.addEventListener("resize", (() => L(this)))
                 }
                 plot() {
                     const e = this.model.get("dataRecords"),
                         t = this.model.get("x"),
                         n = this.model.get("start"),
-                        a = this.model.get("end"),
-                        i = this.model.get("elementId");
+                        a = this.model.get("end");
+                    let i = this.model.get("elementId");
+                    "function" == typeof i && (i = i());
                     let o = k,
                         s = this.el;
                     i && (s = document.getElementById(i), o = s.clientHeight),
                         function(e, t, n, a, i, o, s, r) {
                             const l = o - r.left - r.right,
                                 d = s - r.top - r.bottom;
                             _.select(i).selectAll("*").remove();
                             let c = n;
                             n || (c = _.min(e, (e => e[t])));
-                            let m = a;
-                            a || (m = _.max(e, (e => e[t])));
-                            const u = _.scaleLinear().range([0, l]),
+                            let u = a;
+                            a || (u = _.max(e, (e => e[t])));
+                            const m = _.scaleLinear().range([0, l]),
                                 p = _.scaleLinear().range([d, 0]),
-                                h = _.axisBottom(u),
-                                g = _.axisLeft(p),
-                                f = _.bin().thresholds(40).value((e => Math.round(10 * e[t]) / 10))(e),
+                                h = _.axisBottom(m),
+                                f = _.axisLeft(p),
+                                g = _.bin().thresholds(40).value((e => Math.round(10 * e[t]) / 10))(e),
                                 v = _.select(i).append("svg").attr("width", o).attr("height", s).append("g").attr("transform", "translate(" + r.left + "," + r.top + ")");
-                            u.domain([c, m]), p.domain([0, _.max(f, (e => e.length))]), v.append("g").attr("transform", "translate(0," + d + ")").call(h).append("text").attr("x", l).attr("y", -6).style("text-anchor", "end"), v.append("g").call(g).append("text").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), v.append("g").attr("fill", "steelblue").selectAll().data(f).join("rect").attr("x", (e => u(e.x0) + 1)).attr("width", (e => u(e.x1) - u(e.x0) - 1)).attr("y", (e => p(e.length))).attr("height", (e => p(0) - p(e.length)))
+                            m.domain([c, u]), p.domain([0, _.max(g, (e => e.length))]), v.append("g").attr("transform", "translate(0," + d + ")").call(h).append("text").attr("x", l).attr("y", -6).style("text-anchor", "end"), v.append("g").call(f).append("text").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), v.append("g").attr("fill", "steelblue").selectAll().data(g).join("rect").attr("x", (e => m(e.x0) + 1)).attr("width", (e => m(e.x1) - m(e.x0) - 1)).attr("y", (e => p(e.length))).attr("height", (e => p(0) - p(e.length)))
                         }(e, t, n, a, s, s.clientWidth, o, M)
                 }
             }
-            class B extends a.DOMWidgetModel {
+            class P extends a.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
-                        _model_name: B.model_name,
-                        _view_name: B.view_name,
-                        _model_module: B.model_module,
-                        _view_module: B.view_module,
-                        _model_module_version: B.model_module_version,
-                        _view_module_version: B.view_module_version,
+                        _model_name: P.model_name,
+                        _view_name: P.view_name,
+                        _model_module: P.model_module,
+                        _view_module: P.view_module,
+                        _model_module_version: P.model_module_version,
+                        _view_module_version: P.view_module_version,
                         matrix: [],
                         grid_areas: [],
                         grid_template_areas: String,
                         style: String
                     }
                 }
                 static model_name = "EmbeddingModel";
                 static model_module = w.name;
                 static model_module_version = w.version;
                 static view_name = "EmbeddingView";
                 static view_module = w.name;
                 static view_module_version = w.version
             }
-            class W extends a.DOMWidgetView {
+            class B extends a.DOMWidgetView {
                 render() {
                     this.value_changed()
                 }
                 value_changed() {
                     const e = this.model.get("matrix"),
                         t = this.model.get("grid_areas"),
                         n = this.model.get("grid_template_areas");
@@ -720,24 +725,24 @@
                     const i = document.createElement("div");
                     i.classList.add(a), i.style.display = "grid", i.style.gridTemplateAreas = n, i.style.gridTemplateRows = "repeat(" + e.length + ", 180px)", i.style.gridTemplateColumns = "repeat(" + e[0].length + ", 1fr)", i.style.width = "100%", t.forEach((e => {
                         const t = document.createElement("div");
                         t.setAttribute("id", e), t.style.gridArea = e, t.classList.add("dashboard-div"), i.appendChild(t)
                     })), this.el.appendChild(i)
                 }
             }
-            class P extends a.DOMWidgetModel {
+            class W extends a.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
-                        _model_name: P.model_name,
-                        _view_name: P.view_name,
-                        _model_module: P.model_module,
-                        _view_module: P.view_module,
-                        _model_module_version: P.model_module_version,
-                        _view_module_version: P.view_module_version,
+                        _model_name: W.model_name,
+                        _view_name: W.view_name,
+                        _model_module: W.model_module,
+                        _view_module: W.view_module,
+                        _model_module_version: W.model_module_version,
+                        _view_module_version: W.view_module_version,
                         dataRecords: [],
                         variable: String,
                         step: Number,
                         description: String,
                         minValue: Number,
                         maxValue: Number,
                         elementId: String
@@ -754,54 +759,55 @@
                 render() {
                     L(this), this.model.on("change:dataRecords", (() => L(this)), this), this.model.on("change:variable", (() => L(this)), this), this.model.on("change:step", (() => L(this)), this), this.model.on("change:description", (() => L(this)), this), window.addEventListener("resize", (() => L(this)))
                 }
                 plot() {
                     const e = this.model.get("dataRecords"),
                         t = this.model.get("variable"),
                         n = this.model.get("step"),
-                        a = this.model.get("description"),
-                        i = this.model.get("elementId"),
-                        o = this.model.get("minValue"),
+                        a = this.model.get("description");
+                    let i = this.model.get("elementId");
+                    const o = this.model.get("minValue"),
                         s = this.model.get("maxValue");
+                    "function" == typeof i && (i = i());
                     let r = this.el;
                     i && (r = document.getElementById(i));
                     const l = M;
                     ! function(e, t, n, a, i, o, s, r, l) {
                         const d = document.createElement("div");
                         d.classList.add("range_outside_container"), d.style.margin = l.top + "px " + l.right + "px " + l.bottom + "px " + l.left + "px";
                         const c = document.createElement("span");
                         c.classList.add("range_description"), c.textContent = a, d.appendChild(c);
-                        const m = document.createElement("div");
-                        m.classList.add("range_inside_container"), d.appendChild(m);
-                        const u = document.createElement("span");
-                        u.classList.add("range_value"), d.appendChild(u);
+                        const u = document.createElement("div");
+                        u.classList.add("range_inside_container"), d.appendChild(u);
+                        const m = document.createElement("span");
+                        m.classList.add("range_value"), d.appendChild(m);
                         const p = document.createElement("div");
-                        p.classList.add("sliders_control"), m.appendChild(p);
+                        p.classList.add("sliders_control"), u.appendChild(p);
                         const h = document.createElement("input");
                         h.classList.add("top_slider"), h.setAttribute("step", n), h.setAttribute("type", "range"), p.appendChild(h);
-                        const g = document.createElement("input");
+                        const f = document.createElement("input");
 
-                        function f(e, t) {
-                            u.textContent = e + " - " + t, s(e, t)
+                        function g(e, t) {
+                            m.textContent = e + " - " + t, s(e, t)
                         }
-                        g.setAttribute("step", n), g.setAttribute("type", "range"), p.appendChild(g);
+                        f.setAttribute("step", n), f.setAttribute("type", "range"), p.appendChild(f);
                         const v = _.min(e, (e => e[t])),
                             x = _.max(e, (e => e[t]));
-                        h.setAttribute("min", v), h.setAttribute("max", x), g.setAttribute("min", v), g.setAttribute("max", x), i && o ? (h.value = i, g.value = o) : (h.value = v, g.value = x), f(parseFloat(h.value), parseFloat(g.value)), h.addEventListener("input", (() => {
+                        h.setAttribute("min", v), h.setAttribute("max", x), f.setAttribute("min", v), f.setAttribute("max", x), i && o ? (h.value = i, f.value = o) : (h.value = v, f.value = x), g(parseFloat(h.value), parseFloat(f.value)), h.addEventListener("input", (() => {
                             const e = parseFloat(h.value),
-                                t = parseFloat(g.value);
-                            e > t && (h.value = g.value), f(e, t)
-                        })), g.addEventListener("input", (() => {
+                                t = parseFloat(f.value);
+                            e > t && (h.value = f.value), g(e, t)
+                        })), f.addEventListener("input", (() => {
                             const e = parseFloat(h.value),
-                                t = parseFloat(g.value);
-                            t < e && (g.value = h.value), f(e, t)
+                                t = parseFloat(f.value);
+                            t < e && (f.value = h.value), g(e, t)
                         })), h.addEventListener("click", (() => {
-                            h.classList.add("top_slider"), g.classList.remove("top_slider")
-                        })), g.addEventListener("click", (() => {
-                            g.classList.add("top_slider"), h.classList.remove("top_slider")
+                            h.classList.add("top_slider"), f.classList.remove("top_slider")
+                        })), f.addEventListener("click", (() => {
+                            f.classList.add("top_slider"), h.classList.remove("top_slider")
                         })), r.innerHTML = "", r.appendChild(d)
                     }(e, t, n, a, o, s, this.setValues.bind(this), r, l)
                 }
                 setValues(e, t) {
                     this.model.set({
                         minValue: e
                     }), this.model.set({
@@ -865,34 +871,34 @@
             }
 
             function a(e, a) {
                 for (var o = {}, s = [], r = 0; r < e.length; r++) {
                     var l = e[r],
                         d = a.base ? l[0] + a.base : l[0],
                         c = o[d] || 0,
-                        m = "".concat(d, " ").concat(c);
+                        u = "".concat(d, " ").concat(c);
                     o[d] = c + 1;
-                    var u = n(m),
+                    var m = n(u),
                         p = {
                             css: l[1],
                             media: l[2],
                             sourceMap: l[3],
                             supports: l[4],
                             layer: l[5]
                         };
-                    if (-1 !== u) t[u].references++, t[u].updater(p);
+                    if (-1 !== m) t[m].references++, t[m].updater(p);
                     else {
                         var h = i(p, a);
                         a.byIndex = r, t.splice(r, 0, {
-                            identifier: m,
+                            identifier: u,
                             updater: h,
                             references: 1
                         })
                     }
-                    s.push(m)
+                    s.push(u)
                 }
                 return s
             }
 
             function i(e, t) {
                 var n = t.domAPI(t);
                 return n.update(e),
@@ -983,11 +989,11 @@
                 else {
                     for (; t.firstChild;) t.removeChild(t.firstChild);
                     t.appendChild(document.createTextNode(e))
                 }
             }
         },
         330: e => {
-            e.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.2.2","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.2.3","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `d3vis_ipynb-0.2.2/d3vis_ipynb/labextension/static/493.9def85d738cd0e72c5f5.js` & `d3vis_ipynb-0.2.3/d3vis_ipynb/labextension/static/493.9def85d738cd0e72c5f5.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.2/d3vis_ipynb/labextension/static/693.c8409ce8329f6703470f.js` & `d3vis_ipynb-0.2.3/d3vis_ipynb/labextension/static/693.c8409ce8329f6703470f.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.2/d3vis_ipynb/labextension/static/remoteEntry.6f9edec5dc6ff6501b02.js` & `d3vis_ipynb-0.2.3/d3vis_ipynb/labextension/static/remoteEntry.113ae5fdcfdb6db5a7b5.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,30 +1,30 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, s, l, d, f, p, c, h, v, g, b, m, y, w = {
+    var e, r, t, n, o, i, a, u, s, l, f, d, c, p, h, v, b, g, m, y, w = {
             772: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(112).then((() => () => t(112))),
                         "./extension": () => Promise.all([t.e(112), t.e(493)]).then((() => () => t(493)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    a = (e, r) => {
+                    i = (e, r) => {
                         if (t.S) {
                             var n = "default",
                                 o = t.S[n];
                             if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
                     get: () => o,
-                    init: () => a
+                    init: () => i
                 })
             }
         },
         S = {};
 
     function E(e) {
         var r = S[e];
@@ -42,51 +42,51 @@
         }), r
     }, E.d = (e, r) => {
         for (var t in r) E.o(r, t) && !E.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, E.f = {}, E.e = e => Promise.all(Object.keys(E.f).reduce(((r, t) => (E.f[t](e, r), r)), [])), E.u = e => e + "." + {
-        112: "a36093df8a8075509d10",
+        112: "3054f9386990c9655128",
         493: "9def85d738cd0e72c5f5",
         693: "c8409ce8329f6703470f"
     } [e] + ".js?v=" + {
-        112: "a36093df8a8075509d10",
+        112: "3054f9386990c9655128",
         493: "9def85d738cd0e72c5f5",
         693: "c8409ce8329f6703470f"
     } [e], E.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), E.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "d3vis_ipynb:", E.l = (t, n, o, a) => {
+    }(), E.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "d3vis_ipynb:", E.l = (t, n, o, i) => {
         if (e[t]) e[t].push(n);
         else {
-            var i, u;
+            var a, u;
             if (void 0 !== o)
                 for (var s = document.getElementsByTagName("script"), l = 0; l < s.length; l++) {
-                    var d = s[l];
-                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + o) {
-                        i = d;
+                    var f = s[l];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
+                        a = f;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, E.nc && i.setAttribute("nonce", E.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
-            var f = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(p);
+            a || (u = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, E.nc && a.setAttribute("nonce", E.nc), a.setAttribute("data-webpack", r + o), a.src = t), e[t] = [n];
+            var d = (r, n) => {
+                    a.onerror = a.onload = null, clearTimeout(c);
                     var o = e[t];
-                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
+                    if (delete e[t], a.parentNode && a.parentNode.removeChild(a), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(f.bind(null, void 0, {
+                c = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
-                    target: i
+                    target: a
                 }), 12e4);
-            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
+            a.onerror = d.bind(null, a.onerror), a.onload = d.bind(null, a.onload), u && document.head.appendChild(a)
         }
     }, E.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -96,27 +96,27 @@
             r = {};
         E.I = (t, n) => {
             n || (n = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
                 if (n.push(o), e[t]) return e[t];
                 E.o(E.S, t) || (E.S[t] = {});
-                var a = E.S[t],
-                    i = "d3vis_ipynb",
+                var i = E.S[t],
+                    a = "d3vis_ipynb",
                     u = (e, r, t, n) => {
-                        var o = a[e] = a[e] || {},
+                        var o = i[e] = i[e] || {},
                             u = o[r];
-                        (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (o[r] = {
+                        (!u || !u.loaded && (!n != !u.eager ? n : a > u.from)) && (o[r] = {
                             get: t,
-                            from: i,
+                            from: a,
                             eager: !!n
                         })
                     },
                     s = [];
-                return "default" === t && (u("d3", "7.9.0", (() => E.e(693).then((() => () => E(693))))), u("d3vis_ipynb", "0.2.2", (() => E.e(112).then((() => () => E(112)))))), e[t] = s.length ? Promise.all(s).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("d3", "7.9.0", (() => E.e(693).then((() => () => E(693))))), u("d3vis_ipynb", "0.2.3", (() => E.e(112).then((() => () => E(112)))))), e[t] = s.length ? Promise.all(s).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         E.g.importScripts && (e = E.g.location + "");
         var r = E.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -132,125 +132,125 @@
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
             var o = e[n],
-                a = (typeof o)[0];
-            if (n >= r.length) return "u" == a;
-            var i = r[n],
-                u = (typeof i)[0];
-            if (a != u) return "o" == a && "n" == u || "s" == u || "u" == a;
-            if ("o" != a && "u" != a && o != i) return o < i;
+                i = (typeof o)[0];
+            if (n >= r.length) return "u" == i;
+            var a = r[n],
+                u = (typeof a)[0];
+            if (i != u) return "o" == i && "n" == u || "s" == u || "u" == i;
+            if ("o" != i && "u" != i && o != a) return o < a;
             n++
         }
     }, o = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(u = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
+            for (var n = 1, i = 1; i < e.length; i++) n--, t += "u" == (typeof(u = e[i]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
             return t
         }
-        var i = [];
-        for (a = 1; a < e.length; a++) {
-            var u = e[a];
-            i.push(0 === u ? "not(" + s() + ")" : 1 === u ? "(" + s() + " || " + s() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
+        var a = [];
+        for (i = 1; i < e.length; i++) {
+            var u = e[i];
+            a.push(0 === u ? "not(" + s() + ")" : 1 === u ? "(" + s() + " || " + s() + ")" : 2 === u ? a.pop() + " " + a.pop() : o(u))
         }
         return s();
 
         function s() {
-            return i.pop().replace(/^\((.+)\)$/, "$1")
+            return a.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, a = (e, r) => {
+    }, i = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
-            for (var i = 0, u = 1, s = !0;; u++, i++) {
-                var l, d, f = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (d = (typeof(l = r[i]))[0])) return !s || ("u" == f ? u > n && !o : "" == f != o);
-                if ("u" == d) {
-                    if (!s || "u" != f) return !1
+            for (var a = 0, u = 1, s = !0;; u++, a++) {
+                var l, f, d = u < e.length ? (typeof e[u])[0] : "";
+                if (a >= r.length || "o" == (f = (typeof(l = r[a]))[0])) return !s || ("u" == d ? u > n && !o : "" == d != o);
+                if ("u" == f) {
+                    if (!s || "u" != d) return !1
                 } else if (s)
-                    if (f == d)
+                    if (d == f)
                         if (u <= n) {
                             if (l != e[u]) return !1
                         } else {
                             if (o ? l > e[u] : l < e[u]) return !1;
                             l != e[u] && (s = !1)
                         }
-                else if ("s" != f && "n" != f) {
+                else if ("s" != d && "n" != d) {
                     if (o || u <= n) return !1;
                     s = !1, u--
                 } else {
-                    if (u <= n || d < f != o) return !1;
+                    if (u <= n || f < d != o) return !1;
                     s = !1
-                } else "s" != f && "n" != f && (s = !1, u--)
+                } else "s" != d && "n" != d && (s = !1, u--)
             }
         }
-        var p = [],
-            c = p.pop.bind(p);
-        for (i = 1; i < e.length; i++) {
-            var h = e[i];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
+        var c = [],
+            p = c.pop.bind(c);
+        for (a = 1; a < e.length; a++) {
+            var h = e[a];
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? i(h, r) : !p())
         }
-        return !!c()
-    }, i = (e, r) => {
+        return !!p()
+    }, a = (e, r) => {
         var t = E.S[e];
         if (!t || !E.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, s = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", l = (e, r, t, n) => {
         var o = u(e, t);
-        return a(n, o) || f(s(e, t, o, n)), p(e[t][o])
-    }, d = (e, r, t) => {
+        return i(n, o) || d(s(e, t, o, n)), c(e[t][o])
+    }, f = (e, r, t) => {
         var o = e[r];
-        return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
-    }, f = e => {
+        return (r = Object.keys(o).reduce(((e, r) => !i(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
+    }, d = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, p = e => (e.loaded = 1, e.get()), h = (c = e => function(r, t, n, o) {
-        var a = E.I(r);
-        return a && a.then ? a.then(e.bind(e, r, E.S[r], t, n, o)) : e(r, E.S[r], t, n, o)
-    })(((e, r, t, n) => (i(e, t), l(r, 0, t, n)))), v = c(((e, r, t, n, o) => {
-        var a = r && E.o(r, t) && d(r, t, n);
-        return a ? p(a) : o()
-    })), g = {}, b = {
+    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, o) {
+        var i = E.I(r);
+        return i && i.then ? i.then(e.bind(e, r, E.S[r], t, n, o)) : e(r, E.S[r], t, n, o)
+    })(((e, r, t, n) => (a(e, t), l(r, 0, t, n)))), v = p(((e, r, t, n, o) => {
+        var i = r && E.o(r, t) && f(r, t, n);
+        return i ? c(i) : o()
+    })), b = {}, g = {
         801: () => h("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 4],
             [1, 3],
             [1, 2],
             [1, 1, 1], 1, 1, 1, 1
         ]),
         840: () => v("default", "d3", [1, 7, 9, 0], (() => E.e(693).then((() => () => E(693)))))
     }, m = {
         112: [801, 840]
     }, y = {}, E.f.consumes = (e, r) => {
         E.o(m, e) && m[e].forEach((e => {
-            if (E.o(g, e)) return r.push(g[e]);
+            if (E.o(b, e)) return r.push(b[e]);
             if (!y[e]) {
                 var t = r => {
-                    g[e] = 0, E.m[e] = t => {
+                    b[e] = 0, E.m[e] = t => {
                         delete E.c[e], t.exports = r()
                     }
                 };
                 y[e] = !0;
                 var n = r => {
-                    delete g[e], E.m[e] = t => {
+                    delete b[e], E.m[e] = t => {
                         throw delete E.c[e], r
                     }
                 };
                 try {
-                    var o = b[e]();
-                    o.then ? r.push(g[e] = o.then(t).catch(n)) : t(o)
+                    var o = g[e]();
+                    o.then ? r.push(b[e] = o.then(t).catch(n)) : t(o)
                 } catch (e) {
                     n(e)
                 }
             }
         }))
     }, (() => {
         var e = {
@@ -259,33 +259,33 @@
         E.f.j = (r, t) => {
             var n = E.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
                     var o = new Promise(((t, o) => n = e[r] = [t, o]));
                     t.push(n[2] = o);
-                    var a = E.p + E.u(r),
-                        i = new Error;
-                    E.l(a, (t => {
+                    var i = E.p + E.u(r),
+                        a = new Error;
+                    E.l(i, (t => {
                         if (E.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
                             var o = t && ("load" === t.type ? "missing" : t.type),
-                                a = t && t.target && t.target.src;
-                            i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
+                                i = t && t.target && t.target.src;
+                            a.message = "Loading chunk " + r + " failed.\n(" + o + ": " + i + ")", a.name = "ChunkLoadError", a.type = o, a.request = i, n[1](a)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
-                var n, o, [a, i, u] = t,
+                var n, o, [i, a, u] = t,
                     s = 0;
-                if (a.some((r => 0 !== e[r]))) {
-                    for (n in i) E.o(i, n) && (E.m[n] = i[n]);
+                if (i.some((r => 0 !== e[r]))) {
+                    for (n in a) E.o(a, n) && (E.m[n] = a[n]);
                     u && u(E)
                 }
-                for (r && r(t); s < a.length; s++) o = a[s], E.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); s < i.length; s++) o = i[s], E.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkd3vis_ipynb = self.webpackChunkd3vis_ipynb || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), E.nc = void 0;
     var P = E(772);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).d3vis_ipynb = P
 })();
```

### Comparing `d3vis_ipynb-0.2.2/d3vis_ipynb/labextension/static/third-party-licenses.json` & `d3vis_ipynb-0.2.3/d3vis_ipynb/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.2/d3vis_ipynb/nbextension/index.js` & `d3vis_ipynb-0.2.3/d3vis_ipynb/nbextension/index.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -179,15 +179,15 @@
             55: t => {
                 t.exports = e
             },
             308: e => {
                 e.exports = t
             },
             330: t => {
-                t.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.2.2","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+                t.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.2.3","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
             }
         },
         r = {};
 
     function i(t) {
         var e = r[t];
         if (void 0 !== e) return e.exports;
@@ -223,21 +223,21 @@
         i.r(o), i.d(o, {
             BarPlotModel: () => Ri,
             BarPlotView: () => Ii,
             EmbeddingModel: () => zi,
             EmbeddingView: () => Xi,
             HistogramPlotModel: () => qi,
             HistogramPlotView: () => Hi,
-            LinearHistPlotModel: () => Ci,
-            LinearHistPlotView: () => Ti,
+            LinearHistPlotModel: () => ji,
+            LinearHistPlotView: () => Ci,
             LinearPlotModel: () => Li,
             LinearPlotView: () => Di,
             RangeSliderModel: () => Yi,
             RangeSliderView: () => Bi,
-            ScatterPlotModel: () => Pi,
+            ScatterPlotModel: () => Ti,
             ScatterPlotView: () => Oi,
             author: () => Fi.author,
             dependencies: () => Fi.dependencies,
             description: () => Fi.description,
             devDependencies: () => Fi.devDependencies,
             files: () => Fi.files,
             jupyterlab: () => Fi.jupyterlab,
@@ -334,30 +334,30 @@
         }
 
         function N(t) {
             return t
         }
         const $ = Math.sqrt(50),
             V = Math.sqrt(10),
-            j = Math.sqrt(2);
+            P = Math.sqrt(2);
 
-        function C(t, e, n) {
+        function j(t, e, n) {
             const r = (e - t) / Math.max(0, n),
                 i = Math.floor(Math.log10(r)),
                 o = r / Math.pow(10, i),
-                a = o >= $ ? 10 : o >= V ? 5 : o >= j ? 2 : 1;
+                a = o >= $ ? 10 : o >= V ? 5 : o >= P ? 2 : 1;
             let s, l, u;
-            return i < 0 ? (u = Math.pow(10, -i) / a, s = Math.round(t * u), l = Math.round(e * u), s / u < t && ++s, l / u > e && --l, u = -u) : (u = Math.pow(10, i) * a, s = Math.round(t / u), l = Math.round(e / u), s * u < t && ++s, l * u > e && --l), l < s && .5 <= n && n < 2 ? C(t, e, 2 * n) : [s, l, u]
+            return i < 0 ? (u = Math.pow(10, -i) / a, s = Math.round(t * u), l = Math.round(e * u), s / u < t && ++s, l / u > e && --l, u = -u) : (u = Math.pow(10, i) * a, s = Math.round(t / u), l = Math.round(e / u), s * u < t && ++s, l * u > e && --l), l < s && .5 <= n && n < 2 ? j(t, e, 2 * n) : [s, l, u]
         }
 
-        function T(t, e, n) {
+        function C(t, e, n) {
             if (!((n = +n) > 0)) return [];
             if ((t = +t) == (e = +e)) return [t];
             const r = e < t,
-                [i, o, a] = r ? C(e, t, n) : C(t, e, n);
+                [i, o, a] = r ? j(e, t, n) : j(t, e, n);
             if (!(o >= i)) return [];
             const s = o - i + 1,
                 l = new Array(s);
             if (r)
                 if (a < 0)
                     for (let t = 0; t < s; ++t) l[t] = (o - t) / -a;
                 else
@@ -365,16 +365,16 @@
             else if (a < 0)
                 for (let t = 0; t < s; ++t) l[t] = (i + t) / -a;
             else
                 for (let t = 0; t < s; ++t) l[t] = (i + t) * a;
             return l
         }
 
-        function P(t, e, n) {
-            return C(t = +t, e = +e, n = +n)[2]
+        function T(t, e, n) {
+            return j(t = +t, e = +e, n = +n)[2]
         }
 
         function O(t) {
             return Math.max(1, Math.ceil(Math.log(function(t, e) {
                 let n = 0;
                 for (let e of t) null != e && (e = +e) >= e && ++n;
                 return n
@@ -397,21 +397,21 @@
                     d = n(l, c, h);
                 if (!Array.isArray(d)) {
                     const t = h,
                         n = +d;
                     if (e === g && ([c, h] = function(t, e, n) {
                             let r;
                             for (;;) {
-                                const i = P(t, e, n);
+                                const i = T(t, e, n);
                                 if (i === r || 0 === i || !isFinite(i)) return [t, e];
                                 i > 0 ? (t = Math.floor(t / i) * i, e = Math.ceil(e / i) * i) : i < 0 && (t = Math.ceil(t * i) / i, e = Math.floor(e * i) / i), r = i
                             }
-                        }(c, h, n)), (d = T(c, h, n))[0] <= c && (a = P(c, h, n)), d[d.length - 1] >= h)
+                        }(c, h, n)), (d = C(c, h, n))[0] <= c && (a = T(c, h, n)), d[d.length - 1] >= h)
                         if (t >= h && e === g) {
-                            const t = P(c, h, n);
+                            const t = T(c, h, n);
                             isFinite(t) && (t > 0 ? h = (Math.floor(h / t) + 1) * t : t < 0 && (h = (Math.ceil(h * -t) + 1) / -t))
                         } else d.pop()
                 }
                 for (var f = d.length, p = 0, m = f; d[p] <= c;) ++p;
                 for (; d[m - 1] > h;) --m;
                 (p || m < f) && (d = d.slice(p, m), f = m - p);
                 var _, v = new Array(f + 1);
@@ -732,45 +732,45 @@
 
         function Vt(t) {
             return function() {
                 delete this[t]
             }
         }
 
-        function jt(t, e) {
+        function Pt(t, e) {
             return function() {
                 this[t] = e
             }
         }
 
-        function Ct(t, e) {
+        function jt(t, e) {
             return function() {
                 var n = e.apply(this, arguments);
                 null == n ? delete this[t] : this[t] = n
             }
         }
 
-        function Tt(t) {
+        function Ct(t) {
             return t.trim().split(/^|\s+/)
         }
 
-        function Pt(t) {
+        function Tt(t) {
             return t.classList || new Ot(t)
         }
 
         function Ot(t) {
-            this._node = t, this._names = Tt(t.getAttribute("class") || "")
+            this._node = t, this._names = Ct(t.getAttribute("class") || "")
         }
 
         function Lt(t, e) {
-            for (var n = Pt(t), r = -1, i = e.length; ++r < i;) n.add(e[r])
+            for (var n = Tt(t), r = -1, i = e.length; ++r < i;) n.add(e[r])
         }
 
         function Dt(t, e) {
-            for (var n = Pt(t), r = -1, i = e.length; ++r < i;) n.remove(e[r])
+            for (var n = Tt(t), r = -1, i = e.length; ++r < i;) n.remove(e[r])
         }
 
         function Rt(t) {
             return function() {
                 Lt(this, t)
             }
         }
@@ -1077,20 +1077,20 @@
                 }
                 return this.each((null == e ? n.local ? wt : yt : "function" == typeof e ? n.local ? kt : Mt : n.local ? bt : xt)(n, e))
             },
             style: function(t, e, n) {
                 return arguments.length > 1 ? this.each((null == e ? Et : "function" == typeof e ? Nt : St)(t, e, null == n ? "" : n)) : $t(this.node(), t)
             },
             property: function(t, e) {
-                return arguments.length > 1 ? this.each((null == e ? Vt : "function" == typeof e ? Ct : jt)(t, e)) : this.node()[t]
+                return arguments.length > 1 ? this.each((null == e ? Vt : "function" == typeof e ? jt : Pt)(t, e)) : this.node()[t]
             },
             classed: function(t, e) {
-                var n = Tt(t + "");
+                var n = Ct(t + "");
                 if (arguments.length < 2) {
-                    for (var r = Pt(this.node()), i = -1, o = n.length; ++i < o;)
+                    for (var r = Tt(this.node()), i = -1, o = n.length; ++i < o;)
                         if (!r.contains(n[i])) return !1;
                     return !0
                 }
                 return this.each(("function" == typeof e ? qt : e ? Rt : It)(n, e))
             },
             text: function(t) {
                 return arguments.length ? this.each(null == t ? Ht : ("function" == typeof t ? Xt : zt)(t)) : this.node().textContent
@@ -1252,60 +1252,60 @@
             ke = 0
         }
 
         function Ve() {
             this._call = this._time = this._next = null
         }
 
-        function je(t, e, n) {
+        function Pe(t, e, n) {
             var r = new Ve;
             return r.restart(t, e, n), r
         }
 
-        function Ce() {
+        function je() {
             ke = (Me = Ee.now()) + Ae, ye = we = 0;
             try {
                 ! function() {
                     Ne(), ++ye;
                     for (var t, e = ge; e;)(t = ke - e._time) >= 0 && e._call.call(void 0, t), e = e._next;
                     --ye
                 }()
             } finally {
                 ye = 0,
                     function() {
                         for (var t, e, n = ge, r = 1 / 0; n;) n._call ? (r > n._time && (r = n._time), t = n, n = n._next) : (e = n._next, n._next = null, n = t ? t._next = e : ge = e);
-                        ve = t, Pe(r)
+                        ve = t, Te(r)
                     }(), ke = 0
             }
         }
 
-        function Te() {
+        function Ce() {
             var t = Ee.now(),
                 e = t - Me;
             e > be && (Ae -= e, Me = t)
         }
 
-        function Pe(t) {
-            ye || (we && (we = clearTimeout(we)), t - ke > 24 ? (t < 1 / 0 && (we = setTimeout(Ce, t - Ee.now() - Ae)), xe && (xe = clearInterval(xe))) : (xe || (Me = Ee.now(), xe = setInterval(Te, be)), ye = 1, Se(Ce)))
+        function Te(t) {
+            ye || (we && (we = clearTimeout(we)), t - ke > 24 ? (t < 1 / 0 && (we = setTimeout(je, t - Ee.now() - Ae)), xe && (xe = clearInterval(xe))) : (xe || (Me = Ee.now(), xe = setInterval(Ce, be)), ye = 1, Se(je)))
         }
 
         function Oe(t, e, n) {
             var r = new Ve;
             return e = null == e ? 0 : +e, r.restart((n => {
                 r.stop(), t(n + e)
             }), e, n), r
         }
-        Ve.prototype = je.prototype = {
+        Ve.prototype = Pe.prototype = {
             constructor: Ve,
             restart: function(t, e, n) {
                 if ("function" != typeof t) throw new TypeError("callback is not a function");
-                n = (null == n ? Ne() : +n) + (null == e ? 0 : +e), this._next || ve === this || (ve ? ve._next = this : ge = this, ve = this), this._call = t, this._time = n, Pe()
+                n = (null == n ? Ne() : +n) + (null == e ? 0 : +e), this._next || ve === this || (ve ? ve._next = this : ge = this, ve = this), this._call = t, this._time = n, Te()
             },
             stop: function() {
-                this._call && (this._call = null, this._time = 1 / 0, Pe())
+                this._call && (this._call = null, this._time = 1 / 0, Te())
             }
         };
         var Le = _e("start", "end", "cancel", "interrupt"),
             De = [],
             Re = 0,
             Ie = 3;
 
@@ -1337,15 +1337,15 @@
                     5 === n.state && (n.on.call("end", t, t.__data__, n.index, n.group), s())
                 }
 
                 function s() {
                     for (var r in n.state = 6, n.timer.stop(), delete i[e], i) return;
                     delete t.__transition
                 }
-                i[e] = n, n.timer = je((function(t) {
+                i[e] = n, n.timer = Pe((function(t) {
                     n.state = 1, n.timer.restart(o, n.delay, n.time), n.delay <= t && o(t - n.delay)
                 }), 0, n.time)
             }(t, n, {
                 name: e,
                 index: r,
                 group: i,
                 on: Le,
@@ -1731,41 +1731,41 @@
         }
 
         function $n(t) {
             return ((t = Nn(t)) < 16 ? "0" : "") + t.toString(16)
         }
 
         function Vn(t, e, n, r) {
-            return r <= 0 ? t = e = n = NaN : n <= 0 || n >= 1 ? t = e = NaN : e <= 0 && (t = NaN), new Cn(t, e, n, r)
+            return r <= 0 ? t = e = n = NaN : n <= 0 || n >= 1 ? t = e = NaN : e <= 0 && (t = NaN), new jn(t, e, n, r)
         }
 
-        function jn(t) {
-            if (t instanceof Cn) return new Cn(t.h, t.s, t.l, t.opacity);
-            if (t instanceof rn || (t = wn(t)), !t) return new Cn;
-            if (t instanceof Cn) return t;
+        function Pn(t) {
+            if (t instanceof jn) return new jn(t.h, t.s, t.l, t.opacity);
+            if (t instanceof rn || (t = wn(t)), !t) return new jn;
+            if (t instanceof jn) return t;
             var e = (t = t.rgb()).r / 255,
                 n = t.g / 255,
                 r = t.b / 255,
                 i = Math.min(e, n, r),
                 o = Math.max(e, n, r),
                 a = NaN,
                 s = o - i,
                 l = (o + i) / 2;
-            return s ? (a = e === o ? (n - r) / s + 6 * (n < r) : n === o ? (r - e) / s + 2 : (e - n) / s + 4, s /= l < .5 ? o + i : 2 - o - i, a *= 60) : s = l > 0 && l < 1 ? 0 : a, new Cn(a, s, l, t.opacity)
+            return s ? (a = e === o ? (n - r) / s + 6 * (n < r) : n === o ? (r - e) / s + 2 : (e - n) / s + 4, s /= l < .5 ? o + i : 2 - o - i, a *= 60) : s = l > 0 && l < 1 ? 0 : a, new jn(a, s, l, t.opacity)
         }
 
-        function Cn(t, e, n, r) {
+        function jn(t, e, n, r) {
             this.h = +t, this.s = +e, this.l = +n, this.opacity = +r
         }
 
-        function Tn(t) {
+        function Cn(t) {
             return (t = (t || 0) % 360) < 0 ? t + 360 : t
         }
 
-        function Pn(t) {
+        function Tn(t) {
             return Math.max(0, Math.min(1, t || 0))
         }
 
         function On(t, e, n) {
             return 255 * (t < 60 ? e + (n - e) * t / 60 : t < 180 ? n : t < 240 ? e + (n - e) * (240 - t) / 60 : e)
         }
 
@@ -1783,15 +1783,15 @@
             },
             hex: vn,
             formatHex: vn,
             formatHex8: function() {
                 return this.rgb().formatHex8()
             },
             formatHsl: function() {
-                return jn(this).formatHsl()
+                return Pn(this).formatHsl()
             },
             formatRgb: yn,
             toString: yn
         }), en(kn, Mn, nn(rn, {
             brighter(t) {
                 return t = null == t ? an : Math.pow(an, t), new kn(this.r * t, this.g * t, this.b * t, this.opacity)
             },
@@ -1810,40 +1810,40 @@
             hex: An,
             formatHex: An,
             formatHex8: function() {
                 return `#${$n(this.r)}${$n(this.g)}${$n(this.b)}${$n(255*(isNaN(this.opacity)?1:this.opacity))}`
             },
             formatRgb: En,
             toString: En
-        })), en(Cn, (function(t, e, n, r) {
-            return 1 === arguments.length ? jn(t) : new Cn(t, e, n, null == r ? 1 : r)
+        })), en(jn, (function(t, e, n, r) {
+            return 1 === arguments.length ? Pn(t) : new jn(t, e, n, null == r ? 1 : r)
         }), nn(rn, {
             brighter(t) {
-                return t = null == t ? an : Math.pow(an, t), new Cn(this.h, this.s, this.l * t, this.opacity)
+                return t = null == t ? an : Math.pow(an, t), new jn(this.h, this.s, this.l * t, this.opacity)
             },
             darker(t) {
-                return t = null == t ? on : Math.pow(on, t), new Cn(this.h, this.s, this.l * t, this.opacity)
+                return t = null == t ? on : Math.pow(on, t), new jn(this.h, this.s, this.l * t, this.opacity)
             },
             rgb() {
                 var t = this.h % 360 + 360 * (this.h < 0),
                     e = isNaN(t) || isNaN(this.s) ? 0 : this.s,
                     n = this.l,
                     r = n + (n < .5 ? n : 1 - n) * e,
                     i = 2 * n - r;
                 return new kn(On(t >= 240 ? t - 240 : t + 120, i, r), On(t, i, r), On(t < 120 ? t + 240 : t - 120, i, r), this.opacity)
             },
             clamp() {
-                return new Cn(Tn(this.h), Pn(this.s), Pn(this.l), Sn(this.opacity))
+                return new jn(Cn(this.h), Tn(this.s), Tn(this.l), Sn(this.opacity))
             },
             displayable() {
                 return (0 <= this.s && this.s <= 1 || isNaN(this.s)) && 0 <= this.l && this.l <= 1 && 0 <= this.opacity && this.opacity <= 1
             },
             formatHsl() {
                 const t = Sn(this.opacity);
-                return `${1===t?"hsl(":"hsla("}${Tn(this.h)}, ${100*Pn(this.s)}%, ${100*Pn(this.l)}%${1===t?")":`, ${t})`}`
+                return `${1===t?"hsl(":"hsla("}${Cn(this.h)}, ${100*Tn(this.s)}%, ${100*Tn(this.l)}%${1===t?")":`, ${t})`}`
             }
         }));
         const Dn = t => () => t;
 
         function Rn(t, e) {
             var n = e - t;
             return n ? function(t, e) {
@@ -2536,46 +2536,46 @@
             return t.has(r) ? t.get(r) : n
         }
 
         function Vr(t) {
             return null !== t && "object" == typeof t ? t.valueOf() : t
         }
         Set;
-        const jr = Symbol("implicit");
+        const Pr = Symbol("implicit");
 
-        function Cr() {
+        function jr() {
             var t = new Nr,
                 e = [],
                 n = [],
-                r = jr;
+                r = Pr;
 
             function i(i) {
                 let o = t.get(i);
                 if (void 0 === o) {
-                    if (r !== jr) return r;
+                    if (r !== Pr) return r;
                     t.set(i, o = e.push(i) - 1)
                 }
                 return n[o % n.length]
             }
             return i.domain = function(n) {
                 if (!arguments.length) return e.slice();
                 e = [], t = new Nr;
                 for (const r of n) t.has(r) || t.set(r, e.push(r) - 1);
                 return i
             }, i.range = function(t) {
                 return arguments.length ? (n = Array.from(t), i) : n.slice()
             }, i.unknown = function(t) {
                 return arguments.length ? (r = t, i) : r
             }, i.copy = function() {
-                return Cr(e, n).unknown(r)
+                return jr(e, n).unknown(r)
             }, Sr.apply(i, arguments), i
         }
 
-        function Tr() {
-            var t, e, n = Cr().unknown(void 0),
+        function Cr() {
+            var t, e, n = jr().unknown(void 0),
                 r = n.domain,
                 i = n.range,
                 o = 0,
                 a = 1,
                 s = !1,
                 l = 0,
                 u = 0,
@@ -2613,19 +2613,19 @@
             }, n.paddingInner = function(t) {
                 return arguments.length ? (l = Math.min(1, t), h()) : l
             }, n.paddingOuter = function(t) {
                 return arguments.length ? (u = +t, h()) : u
             }, n.align = function(t) {
                 return arguments.length ? (c = Math.max(0, Math.min(1, t)), h()) : c
             }, n.copy = function() {
-                return Tr(r(), [o, a]).round(s).paddingInner(l).paddingOuter(u).align(c)
+                return Cr(r(), [o, a]).round(s).paddingInner(l).paddingOuter(u).align(c)
             }, Sr.apply(h(), arguments)
         }
 
-        function Pr(t, e) {
+        function Tr(t, e) {
             var n, r = e ? e.length : 0,
                 i = t ? Math.min(r, t.length) : 0,
                 o = new Array(i),
                 a = new Array(r);
             for (n = 0; n < i; ++n) o[n] = Rr(t[n], e[n]);
             for (; n < r; ++n) a[n] = e[n];
             return function(t) {
@@ -2660,15 +2660,15 @@
                 for (n = 0; n < r; ++n) i[n] = t[n] * (1 - o) + e[n] * o;
                 return i
             }
         }
 
         function Rr(t, e) {
             var n, r, i = typeof e;
-            return null == e || "boolean" === i ? Dn(e) : ("number" === i ? Ye : "string" === i ? (n = wn(e)) ? (e = n, In) : Xn : e instanceof wn ? In : e instanceof Date ? Or : (r = e, !ArrayBuffer.isView(r) || r instanceof DataView ? Array.isArray(e) ? Pr : "function" != typeof e.valueOf && "function" != typeof e.toString || isNaN(e) ? Lr : Ye : Dr))(t, e)
+            return null == e || "boolean" === i ? Dn(e) : ("number" === i ? Ye : "string" === i ? (n = wn(e)) ? (e = n, In) : Xn : e instanceof wn ? In : e instanceof Date ? Or : (r = e, !ArrayBuffer.isView(r) || r instanceof DataView ? Array.isArray(e) ? Tr : "function" != typeof e.valueOf && "function" != typeof e.toString || isNaN(e) ? Lr : Ye : Dr))(t, e)
         }
 
         function Ir(t, e) {
             return t = +t, e = +e,
                 function(n) {
                     return Math.round(t * (1 - n) + e * n)
                 }
@@ -2829,22 +2829,22 @@
                     return e = t, ai().domain(e.domain()).range(e.range()).interpolate(e.interpolate()).clamp(e.clamp()).unknown(e.unknown());
                     var e
                 }, Sr.apply(t, arguments),
                 function(t) {
                     var e = t.domain;
                     return t.ticks = function(t) {
                         var n = e();
-                        return T(n[0], n[n.length - 1], null == t ? 10 : t)
+                        return C(n[0], n[n.length - 1], null == t ? 10 : t)
                     }, t.tickFormat = function(t, n) {
                         var r = e();
                         return function(t, e, n, r) {
                             var i, o = function(t, e, n) {
                                 n = +n;
                                 const r = (e = +e) < (t = +t),
-                                    i = r ? P(e, t, n) : P(t, e, n);
+                                    i = r ? T(e, t, n) : T(t, e, n);
                                 return (r ? -1 : 1) * (i < 0 ? 1 / -i : i)
                             }(t, e, n);
                             switch ((r = Ur(null == r ? ",f" : r)).type) {
                                 case "s":
                                     var a = Math.max(Math.abs(t), Math.abs(e));
                                     return null != r.precision || isNaN(i = function(t, e) {
                                         return Math.max(0, 3 * Math.max(-8, Math.min(8, Math.floor(Zr(e) / 3))) - Zr(Math.abs(t)))
@@ -2871,15 +2871,15 @@
                         var r, i, o = e(),
                             a = 0,
                             s = o.length - 1,
                             l = o[a],
                             u = o[s],
                             c = 10;
                         for (u < l && (i = l, l = u, u = i, i = a, a = s, s = i); c-- > 0;) {
-                            if ((i = P(l, u, n)) === r) return o[a] = l, o[s] = u, e(o);
+                            if ((i = T(l, u, n)) === r) return o[a] = l, o[s] = u, e(o);
                             if (i > 0) l = Math.floor(l / i) * i, u = Math.ceil(u / i) * i;
                             else {
                                 if (!(i < 0)) break;
                                 l = Math.ceil(l * i) / i, u = Math.floor(u * i) / i
                             }
                             r = i
                         }
@@ -3487,53 +3487,54 @@
             Vi = {
                 top: 20,
                 right: 20,
                 bottom: 30,
                 left: 40
             };
 
-        function ji(t) {
+        function Pi(t) {
             t.timeout && clearTimeout(t.timeout), t.timeout = setTimeout((() => {
                 t.plot()
             }), 100)
         }
-        class Ci extends t.DOMWidgetModel {
+        class ji extends t.DOMWidgetModel {
             defaults() {
                 return {
                     ...super.defaults(),
-                    _model_name: Ci.model_name,
-                    _view_name: Ci.view_name,
-                    _model_module: Ci.model_module,
-                    _view_module: Ci.view_module,
-                    _model_module_version: Ci.model_module_version,
-                    _view_module_version: Ci.view_module_version,
+                    _model_name: ji.model_name,
+                    _view_name: ji.view_name,
+                    _model_module: ji.model_module,
+                    _view_module: ji.view_module,
+                    _model_module_version: ji.model_module_version,
+                    _view_module_version: ji.view_module_version,
                     linearData_x: [],
                     linearData_y: [],
                     histogramData: [],
                     elementId: String,
                     clickedValue: String
                 }
             }
             static model_name = "LinearHistPlotModel";
             static model_module = Ni.name;
             static model_module_version = Ni.version;
             static view_name = "LinearHistPlotView";
             static view_module = Ni.name;
             static view_module_version = Ni.version
         }
-        class Ti extends t.DOMWidgetView {
+        class Ci extends t.DOMWidgetView {
             timeout;
             render() {
-                ji(this), this.model.on("change:linearData_x", (() => ji(this)), this), this.model.on("change:linearData_y", (() => ji(this)), this), this.model.on("change:histogramData", (() => ji(this)), this), window.addEventListener("resize", (() => ji(this)))
+                Pi(this), this.model.on("change:linearData_x", (() => Pi(this)), this), this.model.on("change:linearData_y", (() => Pi(this)), this), this.model.on("change:histogramData", (() => Pi(this)), this), window.addEventListener("resize", (() => Pi(this)))
             }
             plot() {
                 const t = this.model.get("linearData_x"),
                     e = this.model.get("linearData_y"),
-                    n = this.model.get("histogramData"),
-                    r = this.model.get("elementId");
+                    n = this.model.get("histogramData");
+                let r = this.model.get("elementId");
+                "function" == typeof r && (r = r());
                 let i = $i,
                     o = this.el;
                 r && (o = document.getElementById(r), i = o.clientHeight);
                 let a = o.clientWidth;
                 const s = Vi;
                 ! function(t, e, n, r, i, o, a, s) {
                     const l = o - s.left - s.right,
@@ -3573,24 +3574,24 @@
             }
             setValue(t) {
                 this.model.set({
                     clickedValue: t
                 }), this.model.save_changes()
             }
         }
-        class Pi extends t.DOMWidgetModel {
+        class Ti extends t.DOMWidgetModel {
             defaults() {
                 return {
                     ...super.defaults(),
-                    _model_name: Pi.model_name,
-                    _view_name: Pi.view_name,
-                    _model_module: Pi.model_module,
-                    _view_module: Pi.view_module,
-                    _model_module_version: Pi.model_module_version,
-                    _view_module_version: Pi.view_module_version,
+                    _model_name: Ti.model_name,
+                    _view_name: Ti.view_name,
+                    _model_module: Ti.model_module,
+                    _view_module: Ti.view_module,
+                    _model_module_version: Ti.model_module_version,
+                    _view_module_version: Ti.view_module_version,
                     dataRecords: [],
                     x: String,
                     y: String,
                     hue: String,
                     elementId: String,
                     clickedValue: String,
                     selectedValuesRecords: []
@@ -3602,36 +3603,37 @@
             static view_name = "ScatterPlotView";
             static view_module = Ni.name;
             static view_module_version = Ni.version
         }
         class Oi extends t.DOMWidgetView {
             timeout;
             render() {
-                ji(this), this.model.on("change:dataRecords", (() => ji(this)), this), this.model.on("change:x", (() => ji(this)), this), this.model.on("change:y", (() => ji(this)), this), this.model.on("change:hue", (() => ji(this)), this), window.addEventListener("resize", (() => ji(this)))
+                Pi(this), this.model.on("change:dataRecords", (() => Pi(this)), this), this.model.on("change:x", (() => Pi(this)), this), this.model.on("change:y", (() => Pi(this)), this), this.model.on("change:hue", (() => Pi(this)), this), window.addEventListener("resize", (() => Pi(this)))
             }
             plot() {
                 const t = this.model.get("dataRecords"),
                     e = this.model.get("x"),
                     n = this.model.get("y"),
-                    r = this.model.get("hue"),
-                    i = this.model.get("elementId");
+                    r = this.model.get("hue");
+                let i = this.model.get("elementId");
+                "function" == typeof i && (i = i());
                 let o = $i,
                     a = this.el;
                 i && (a = document.getElementById(i), o = a.clientHeight);
                 let s = a.clientWidth;
                 const l = Vi;
                 ! function(t, e, n, r, i, o, a, s, l, u) {
                     const c = s - u.left - u.right,
                         h = l - u.top - u.bottom;
                     for (let e = 0; e < t.length; e++) t[e].id = e;
                     const d = Math.floor(Math.random() * Date.now() * 1e4).toString(36);
                     mr(i).selectAll("*").remove();
                     const f = ai().range([0, c]),
                         p = ai().range([h, 0]),
-                        m = Cr(si),
+                        m = jr(si),
                         _ = Z(f),
                         v = K(p),
                         y = mr(i).append("svg").attr("width", s).attr("height", l).append("g").attr("transform", "translate(" + u.left + "," + u.top + ")");
                     if (f.domain(g(t, (function(t) {
                             return t[e]
                         }))).nice(), p.domain(g(t, (function(t) {
                             return t[n]
@@ -3704,22 +3706,23 @@
             static view_name = "LinearPlotView";
             static view_module = Ni.name;
             static view_module_version = Ni.version
         }
         class Di extends t.DOMWidgetView {
             timeout;
             render() {
-                ji(this), this.model.on("change:dataRecords", (() => ji(this)), this), this.model.on("change:x", (() => ji(this)), this), this.model.on("change:y", (() => ji(this)), this), this.model.on("change:hue", (() => ji(this)), this), window.addEventListener("resize", (() => ji(this)))
+                Pi(this), this.model.on("change:dataRecords", (() => Pi(this)), this), this.model.on("change:x", (() => Pi(this)), this), this.model.on("change:y", (() => Pi(this)), this), this.model.on("change:hue", (() => Pi(this)), this), window.addEventListener("resize", (() => Pi(this)))
             }
             plot() {
                 const t = this.model.get("dataRecords"),
                     e = this.model.get("x"),
                     n = this.model.get("y"),
-                    r = this.model.get("hue"),
-                    i = this.model.get("elementId");
+                    r = this.model.get("hue");
+                let i = this.model.get("elementId");
+                "function" == typeof i && (i = i());
                 let o = $i,
                     a = this.el;
                 i && (a = document.getElementById(i), o = a.clientHeight);
                 let s = a.clientWidth;
                 const l = Vi;
                 ! function(t, e, n, r, i, o, a, s, l, u) {
                     const c = s - u.left - u.right,
@@ -3755,15 +3758,15 @@
                         })), a
                     }(t, e, [n], r);
                     for (let e = 0; e < t.length; e++) t[e].id = e;
                     const d = Math.floor(Math.random() * Date.now() * 1e4).toString(36);
                     mr(i).selectAll("*").remove();
                     const f = ai().range([0, c]),
                         p = ai().range([h, 0]),
-                        m = Cr(si),
+                        m = jr(si),
                         _ = Z(f),
                         v = K(p),
                         y = mr(i).append("svg").attr("width", s).attr("height", l).append("g").attr("transform", "translate(" + u.left + "," + u.top + ")");
 
                     function w(t, r) {
                         y.append("path").datum(t).attr("fill", "none").attr("stroke", m(r)).attr("stroke-width", 2).attr("d", yi().x((t => f(t[e]))).y((t => p(t[n]))))
                     }
@@ -3834,44 +3837,45 @@
                     dataRecords: [],
                     x: String,
                     y: String,
                     hue: String,
                     elementId: String
                 }
             }
-            static model_name = "BarplotModel";
+            static model_name = "BarPlotModel";
             static model_module = Ni.name;
             static model_module_version = Ni.version;
-            static view_name = "BarplotView";
+            static view_name = "BarPlotView";
             static view_module = Ni.name;
             static view_module_version = Ni.version
         }
         class Ii extends t.DOMWidgetView {
             timeout;
             render() {
-                ji(this), this.model.on("change:dataRecords", (() => ji(this)), this), this.model.on("change:x", (() => ji(this)), this), this.model.on("change:y", (() => ji(this)), this), this.model.on("change:hue", (() => ji(this)), this), window.addEventListener("resize", (() => ji(this)))
+                Pi(this), this.model.on("change:dataRecords", (() => Pi(this)), this), this.model.on("change:x", (() => Pi(this)), this), this.model.on("change:y", (() => Pi(this)), this), this.model.on("change:hue", (() => Pi(this)), this), window.addEventListener("resize", (() => Pi(this)))
             }
             plot() {
                 const t = this.model.get("dataRecords"),
                     e = this.model.get("x"),
                     n = this.model.get("y"),
-                    r = this.model.get("hue"),
-                    i = this.model.get("elementId");
+                    r = this.model.get("hue");
+                let i = this.model.get("elementId");
+                "function" == typeof i && (i = i());
                 let o = $i,
                     a = this.el;
                 i && (a = document.getElementById(i), o = a.clientHeight),
                     function(t, e, n, r, i, o, a, s) {
                         const l = o - s.left - s.right,
                             u = a - s.top - s.bottom;
                         mr(i).selectAll("*").remove();
                         const c = mr(i).append("svg").attr("width", o).attr("height", a).append("g").attr("transform", "translate(" + s.left + "," + s.top + ")");
                         r || (r = e);
                         const h = t.reduce(((t, e) => (t && -1 === t.indexOf(e[r]) && t.push(e[r]), t)), []),
                             d = {},
-                            f = Cr(si);
+                            f = jr(si);
                         r == e ? function() {
                             let r = t.reduce(((t, r) => {
                                 const i = r[e],
                                     o = r[n];
                                 if (i in t) t[i] += o, d[i].qt += 1, d[i][n].push(o);
                                 else {
                                     const e = {
@@ -3891,15 +3895,15 @@
                             }));
                             const i = r.map((t => t[e])),
                                 o = [],
                                 a = Object.keys(d).map((t => d[t]));
                             o.push(R(a, (t => t.min))), o.push(D(a, (t => t.max))), o[0] > 0 && o[1] > 0 ? o[0] = 0 : o[0] < 0 && o[1] < 0 && (o[1] = 0);
                             const s = ai().domain(o).range([u, 0]);
                             c.append("g").call(K(s));
-                            const p = Tr().domain(i).range([0, l]).padding([.2]);
+                            const p = Cr().domain(i).range([0, l]).padding([.2]);
                             c.append("g").selectAll("g").data(r).enter().append("rect").attr("x", (function(t) {
                                 return p(t[e])
                             })).attr("y", (function(t) {
                                 return s(t[n]) < s(0) ? s(t[n]) : s(0)
                             })).attr("width", p.bandwidth()).attr("height", (function(t) {
                                 return Math.abs(s(0) - s(t[n]))
                             })).data(h).attr("fill", (function(t) {
@@ -3959,16 +3963,16 @@
                             Object.keys(d).map((t => {
                                 h.forEach((e => s.push(d[t][e])))
                             }));
                             const p = [];
                             p.push(R(s, (t => t.min))), p.push(D(s, (t => t.max))), p[0] > 0 && p[1] > 0 ? p[0] = 0 : p[0] < 0 && p[1] < 0 && (p[1] = 0);
                             const m = ai().domain(p).range([u, 0]);
                             c.append("g").call(K(m));
-                            const _ = Tr().domain(a).range([0, l]).padding([.2]),
-                                g = Tr().domain(o).range([0, _.bandwidth()]).padding([.05]);
+                            const _ = Cr().domain(a).range([0, l]).padding([.2]),
+                                g = Cr().domain(o).range([0, _.bandwidth()]).padding([.05]);
                             c.append("g").selectAll("g").data(i).enter().append("g").attr("transform", (function(t) {
                                 return "translate(" + _(t[e]) + ",0)"
                             })).selectAll("rect").data((function(t) {
                                 return o.map((function(e) {
                                     return {
                                         key: e,
                                         value: t[e]
@@ -4029,32 +4033,33 @@
                     dataRecords: [],
                     x: String,
                     start: Number,
                     end: Number,
                     elementId: String
                 }
             }
-            static model_name = "HistogramplotModel";
+            static model_name = "HistogramPlotModel";
             static model_module = Ni.name;
             static model_module_version = Ni.version;
-            static view_name = "HistogramplotView";
+            static view_name = "HistogramPlotView";
             static view_module = Ni.name;
             static view_module_version = Ni.version
         }
         class Hi extends t.DOMWidgetView {
             timeout;
             render() {
-                ji(this), this.model.on("change:dataRecords", (() => ji(this)), this), this.model.on("change:x", (() => ji(this)), this), this.model.on("change:start", (() => ji(this)), this), this.model.on("change:end", (() => ji(this)), this), window.addEventListener("resize", (() => ji(this)))
+                Pi(this), this.model.on("change:dataRecords", (() => Pi(this)), this), this.model.on("change:x", (() => Pi(this)), this), this.model.on("change:start", (() => Pi(this)), this), this.model.on("change:end", (() => Pi(this)), this), window.addEventListener("resize", (() => Pi(this)))
             }
             plot() {
                 const t = this.model.get("dataRecords"),
                     e = this.model.get("x"),
                     n = this.model.get("start"),
-                    r = this.model.get("end"),
-                    i = this.model.get("elementId");
+                    r = this.model.get("end");
+                let i = this.model.get("elementId");
+                "function" == typeof i && (i = i());
                 let o = $i,
                     a = this.el;
                 i && (a = document.getElementById(i), o = a.clientHeight),
                     function(t, e, n, r, i, o, a, s) {
                         const l = o - s.left - s.right,
                             u = a - s.top - s.bottom;
                         mr(i).selectAll("*").remove();
@@ -4136,24 +4141,25 @@
             static model_module_version = Ni.version;
             static view_name = "RangeSliderView";
             static view_module = Ni.name;
             static view_module_version = Ni.version
         }
         class Bi extends t.DOMWidgetView {
             render() {
-                ji(this), this.model.on("change:dataRecords", (() => ji(this)), this), this.model.on("change:variable", (() => ji(this)), this), this.model.on("change:step", (() => ji(this)), this), this.model.on("change:description", (() => ji(this)), this), window.addEventListener("resize", (() => ji(this)))
+                Pi(this), this.model.on("change:dataRecords", (() => Pi(this)), this), this.model.on("change:variable", (() => Pi(this)), this), this.model.on("change:step", (() => Pi(this)), this), this.model.on("change:description", (() => Pi(this)), this), window.addEventListener("resize", (() => Pi(this)))
             }
             plot() {
                 const t = this.model.get("dataRecords"),
                     e = this.model.get("variable"),
                     n = this.model.get("step"),
-                    r = this.model.get("description"),
-                    i = this.model.get("elementId"),
-                    o = this.model.get("minValue"),
+                    r = this.model.get("description");
+                let i = this.model.get("elementId");
+                const o = this.model.get("minValue"),
                     a = this.model.get("maxValue");
+                "function" == typeof i && (i = i());
                 let s = this.el;
                 i && (s = document.getElementById(i));
                 const l = Vi;
                 ! function(t, e, n, r, i, o, a, s, l) {
                     const u = document.createElement("div");
                     u.classList.add("range_outside_container"), u.style.margin = l.top + "px " + l.right + "px " + l.bottom + "px " + l.left + "px";
                     const c = document.createElement("span");
```

### Comparing `d3vis_ipynb-0.2.2/js/amd-public-path.js` & `d3vis_ipynb-0.2.3/js/amd-public-path.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.2/js/package.json` & `d3vis_ipynb-0.2.3/js/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.2.3'"}*

```diff
@@ -48,9 +48,9 @@
         "build:prod": "webpack --mode=production && yarn run build:labextension",
         "clean": "rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension",
         "prepublish": "yarn run clean && yarn run build:prod",
         "start": "webpack serve --open --config webpack.exports.config.js",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch --mode=development"
     },
-    "version": "0.2.2"
+    "version": "0.2.3"
 }
```

### Comparing `d3vis_ipynb-0.2.2/js/webpack.config.js` & `d3vis_ipynb-0.2.3/js/webpack.config.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.2/js/webpack.exports.config.js` & `d3vis_ipynb-0.2.3/js/webpack.exports.config.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.2/js/css/widget.css` & `d3vis_ipynb-0.2.3/js/css/widget.css`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.2/js/lib/labplugin.js` & `d3vis_ipynb-0.2.3/js/lib/labplugin.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.2/js/lib/web-dev.js` & `d3vis_ipynb-0.2.3/js/lib/web-dev.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.2/js/lib/widgets.js` & `d3vis_ipynb-0.2.3/js/lib/widgets.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -80,15 +80,17 @@
         window.addEventListener("resize", () => plotAfterInterval(this));
     }
 
     plot() {
         const linearData_x = this.model.get("linearData_x");
         const linearData_y = this.model.get("linearData_y");
         const histogramData = this.model.get("histogramData");
-        const elementId = this.model.get("elementId");
+        let elementId = this.model.get("elementId");
+
+        if (typeof elementId === "function") elementId = elementId();
 
         let height = WIDGET_HEIGHT;
         let element = this.el;
         if (elementId) {
             element = document.getElementById(elementId);
             height = element.clientHeight;
         }
@@ -158,15 +160,17 @@
     }
 
     plot() {
         const data = this.model.get("dataRecords");
         const x = this.model.get("x");
         const y = this.model.get("y");
         const hue = this.model.get("hue");
-        const elementId = this.model.get("elementId");
+        let elementId = this.model.get("elementId");
+
+        if (typeof elementId === "function") elementId = elementId();
 
         let height = WIDGET_HEIGHT;
         let element = this.el;
         if (elementId) {
             element = document.getElementById(elementId);
             height = element.clientHeight;
         }
@@ -245,15 +249,17 @@
     }
 
     plot() {
         const data = this.model.get("dataRecords");
         const x = this.model.get("x");
         const y = this.model.get("y");
         const hue = this.model.get("hue");
-        const elementId = this.model.get("elementId");
+        let elementId = this.model.get("elementId");
+
+        if (typeof elementId === "function") elementId = elementId();
 
         let height = WIDGET_HEIGHT;
         let element = this.el;
         if (elementId) {
             element = document.getElementById(elementId);
             height = element.clientHeight;
         }
@@ -304,18 +310,18 @@
             x: String,
             y: String,
             hue: String,
             elementId: String,
         };
     }
 
-    static model_name = "BarplotModel";
+    static model_name = "BarPlotModel";
     static model_module = packageData.name;
     static model_module_version = packageData.version;
-    static view_name = "BarplotView"; // Set to null if no view
+    static view_name = "BarPlotView"; // Set to null if no view
     static view_module = packageData.name; // Set to null if no view
     static view_module_version = packageData.version;
 }
 
 export class BarPlotView extends DOMWidgetView {
     timeout;
 
@@ -330,15 +336,17 @@
     }
 
     plot() {
         const data = this.model.get("dataRecords");
         const x = this.model.get("x");
         const y = this.model.get("y");
         const hue = this.model.get("hue");
-        const elementId = this.model.get("elementId");
+        let elementId = this.model.get("elementId");
+
+        if (typeof elementId === "function") elementId = elementId();
 
         let height = WIDGET_HEIGHT;
         let element = this.el;
         if (elementId) {
             element = document.getElementById(elementId);
             height = element.clientHeight;
         }
@@ -364,18 +372,18 @@
             x: String,
             start: Number,
             end: Number,
             elementId: String,
         };
     }
 
-    static model_name = "HistogramplotModel";
+    static model_name = "HistogramPlotModel";
     static model_module = packageData.name;
     static model_module_version = packageData.version;
-    static view_name = "HistogramplotView"; // Set to null if no view
+    static view_name = "HistogramPlotView"; // Set to null if no view
     static view_module = packageData.name; // Set to null if no view
     static view_module_version = packageData.version;
 }
 
 export class HistogramPlotView extends DOMWidgetView {
     timeout;
 
@@ -390,15 +398,17 @@
     }
 
     plot() {
         const data = this.model.get("dataRecords");
         const x = this.model.get("x");
         const start = this.model.get("start");
         const end = this.model.get("end");
-        const elementId = this.model.get("elementId");
+        let elementId = this.model.get("elementId");
+
+        if (typeof elementId === "function") elementId = elementId();
 
         let height = WIDGET_HEIGHT;
         let element = this.el;
         if (elementId) {
             element = document.getElementById(elementId);
             height = element.clientHeight;
         }
@@ -512,18 +522,20 @@
     }
 
     plot() {
         const data = this.model.get("dataRecords");
         const variable = this.model.get("variable");
         const step = this.model.get("step");
         const description = this.model.get("description");
-        const elementId = this.model.get("elementId");
+        let elementId = this.model.get("elementId");
         const minValue = this.model.get("minValue");
         const maxValue = this.model.get("maxValue");
 
+        if (typeof elementId === "function") elementId = elementId();
+
         let element = this.el;
         if (elementId) {
             element = document.getElementById(elementId);
         }
         const margin = WIDGET_MARGIN;
 
         rangeslider(
```

### Comparing `d3vis_ipynb-0.2.2/js/lib/graphs/barplot.js` & `d3vis_ipynb-0.2.3/js/lib/graphs/barplot.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.2/js/lib/graphs/histogramplot.js` & `d3vis_ipynb-0.2.3/js/lib/graphs/histogramplot.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.2/js/lib/graphs/linearhistplot.js` & `d3vis_ipynb-0.2.3/js/lib/graphs/linearhistplot.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.2/js/lib/graphs/linearplot.js` & `d3vis_ipynb-0.2.3/js/lib/graphs/linearplot.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.2/js/lib/graphs/rangeslider.js` & `d3vis_ipynb-0.2.3/js/lib/graphs/rangeslider.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.2/js/lib/graphs/scatterplot.js` & `d3vis_ipynb-0.2.3/js/lib/graphs/scatterplot.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.2/js/lib/tools/group_data.js` & `d3vis_ipynb-0.2.3/js/lib/tools/group_data.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.2/js/lib/tools/lasso.js` & `d3vis_ipynb-0.2.3/js/lib/tools/lasso.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.2/LICENSE.txt` & `d3vis_ipynb-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.2/README.md` & `d3vis_ipynb-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.2/pyproject.toml` & `d3vis_ipynb-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "ipywidgets==7.7.1",
     "simplejson >=3.19.0",
     "anywidget >= 0.9.6"
 ]
-version = "0.2.2"
+version = "0.2.3"
 
 [project.optional-dependencies]
 docs = [
     "jupyter_sphinx",
     "nbsphinx",
     "nbsphinx-link",
     "pypandoc",
```

### Comparing `d3vis_ipynb-0.2.2/PKG-INFO` & `d3vis_ipynb-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: d3vis_ipynb
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Custom Jupyter Widget Library with visualizations created with D3.js.
 Project-URL: Homepage, https://github.com/H-IAAC/d3vis_ipynb
 Author-email: Daniel Adam Miranda <daniel.miranda@eldorado.org.br>
 License: Copyright (c) 2024 Daniel Adam Miranda
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

