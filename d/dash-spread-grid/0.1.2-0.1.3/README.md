# Comparing `tmp/dash_spread_grid-0.1.2.tar.gz` & `tmp/dash_spread_grid-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_spread_grid-0.1.2.tar", last modified: Sat May 25 08:53:30 2024, max compression
+gzip compressed data, was "dash_spread_grid-0.1.3.tar", last modified: Mon May 27 07:25:39 2024, max compression
```

## Comparing `dash_spread_grid-0.1.2.tar` & `dash_spread_grid-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-05-25 08:53:30.932150 dash_spread_grid-0.1.2/
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-01-18 13:13:06.000000 dash_spread_grid-0.1.2/LICENSE
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      393 2024-01-18 13:13:06.000000 dash_spread_grid-0.1.2/MANIFEST.in
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      259 2024-05-25 08:53:30.932150 dash_spread_grid-0.1.2/PKG-INFO
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     3703 2024-01-20 12:13:37.000000 dash_spread_grid-0.1.2/README.md
-drwxr-xr-x   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-05-25 08:53:30.932150 dash_spread_grid-0.1.2/dash_spread_grid/
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     3288 2024-05-25 08:53:30.000000 dash_spread_grid-0.1.2/dash_spread_grid/DashSpreadGrid.py
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     2261 2024-01-18 13:13:06.000000 dash_spread_grid-0.1.2/dash_spread_grid/__init__.py
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)       78 2024-05-25 08:53:30.000000 dash_spread_grid-0.1.2/dash_spread_grid/_imports_.py
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)    54041 2024-05-25 08:53:29.000000 dash_spread_grid-0.1.2/dash_spread_grid/dash_spread_grid.min.js
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)   210227 2024-05-25 08:53:29.000000 dash_spread_grid-0.1.2/dash_spread_grid/dash_spread_grid.min.js.map
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     6046 2024-05-25 08:53:30.000000 dash_spread_grid-0.1.2/dash_spread_grid/metadata.json
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     2455 2024-05-25 08:53:30.000000 dash_spread_grid-0.1.2/dash_spread_grid/package-info.json
-drwxr-xr-x   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-05-25 08:53:30.932150 dash_spread_grid-0.1.2/dash_spread_grid.egg-info/
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      259 2024-05-25 08:53:30.000000 dash_spread_grid-0.1.2/dash_spread_grid.egg-info/PKG-INFO
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      457 2024-05-25 08:53:30.000000 dash_spread_grid-0.1.2/dash_spread_grid.egg-info/SOURCES.txt
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)        1 2024-05-25 08:53:30.000000 dash_spread_grid-0.1.2/dash_spread_grid.egg-info/dependency_links.txt
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)       17 2024-05-25 08:53:30.000000 dash_spread_grid-0.1.2/dash_spread_grid.egg-info/top_level.txt
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     2455 2024-05-25 08:53:15.000000 dash_spread_grid-0.1.2/package.json
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)       38 2024-05-25 08:53:30.932150 dash_spread_grid-0.1.2/setup.cfg
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      510 2024-01-18 13:19:42.000000 dash_spread_grid-0.1.2/setup.py
+drwxr-xr-x   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-05-27 07:25:39.587835 dash_spread_grid-0.1.3/
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-01-18 13:13:06.000000 dash_spread_grid-0.1.3/LICENSE
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      393 2024-01-18 13:13:06.000000 dash_spread_grid-0.1.3/MANIFEST.in
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      259 2024-05-27 07:25:39.587835 dash_spread_grid-0.1.3/PKG-INFO
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     3703 2024-01-20 12:13:37.000000 dash_spread_grid-0.1.3/README.md
+drwxr-xr-x   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-05-27 07:25:39.587835 dash_spread_grid-0.1.3/dash_spread_grid/
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     3288 2024-05-27 07:25:39.000000 dash_spread_grid-0.1.3/dash_spread_grid/DashSpreadGrid.py
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     2261 2024-01-18 13:13:06.000000 dash_spread_grid-0.1.3/dash_spread_grid/__init__.py
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)       78 2024-05-27 07:25:39.000000 dash_spread_grid-0.1.3/dash_spread_grid/_imports_.py
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)    55304 2024-05-27 07:25:37.000000 dash_spread_grid-0.1.3/dash_spread_grid/dash_spread_grid.min.js
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)   216183 2024-05-27 07:25:37.000000 dash_spread_grid-0.1.3/dash_spread_grid/dash_spread_grid.min.js.map
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     6046 2024-05-27 07:25:39.000000 dash_spread_grid-0.1.3/dash_spread_grid/metadata.json
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     2455 2024-05-27 07:25:38.000000 dash_spread_grid-0.1.3/dash_spread_grid/package-info.json
+drwxr-xr-x   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-05-27 07:25:39.587835 dash_spread_grid-0.1.3/dash_spread_grid.egg-info/
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      259 2024-05-27 07:25:39.000000 dash_spread_grid-0.1.3/dash_spread_grid.egg-info/PKG-INFO
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      457 2024-05-27 07:25:39.000000 dash_spread_grid-0.1.3/dash_spread_grid.egg-info/SOURCES.txt
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)        1 2024-05-27 07:25:39.000000 dash_spread_grid-0.1.3/dash_spread_grid.egg-info/dependency_links.txt
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)       17 2024-05-27 07:25:39.000000 dash_spread_grid-0.1.3/dash_spread_grid.egg-info/top_level.txt
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     2455 2024-05-27 07:25:15.000000 dash_spread_grid-0.1.3/package.json
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)       38 2024-05-27 07:25:39.587835 dash_spread_grid-0.1.3/setup.cfg
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      510 2024-01-18 13:19:42.000000 dash_spread_grid-0.1.3/setup.py
```

### Comparing `dash_spread_grid-0.1.2/README.md` & `dash_spread_grid-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `dash_spread_grid-0.1.2/dash_spread_grid/DashSpreadGrid.py` & `dash_spread_grid-0.1.3/dash_spread_grid/DashSpreadGrid.py`

 * *Files identical despite different names*

### Comparing `dash_spread_grid-0.1.2/dash_spread_grid/__init__.py` & `dash_spread_grid-0.1.3/dash_spread_grid/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_spread_grid-0.1.2/dash_spread_grid/dash_spread_grid.min.js` & `dash_spread_grid-0.1.3/dash_spread_grid/dash_spread_grid.min.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -5,15 +5,15 @@
                 __webpack_require__.d(__webpack_exports__, {
                     Z: () => __WEBPACK_DEFAULT_EXPORT__
                 });
                 var react__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(196),
                     react__WEBPACK_IMPORTED_MODULE_0___default = __webpack_require__.n(react__WEBPACK_IMPORTED_MODULE_0__),
                     prop_types__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(64),
                     prop_types__WEBPACK_IMPORTED_MODULE_1___default = __webpack_require__.n(prop_types__WEBPACK_IMPORTED_MODULE_1__),
-                    js_spread_grid__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(449);
+                    js_spread_grid__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(906);
 
                 function _typeof(e) {
                     return _typeof = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
                         return typeof e
                     } : function(e) {
                         return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
                     }, _typeof(e)
@@ -26,97 +26,97 @@
                 function _nonIterableRest() {
                     throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                 }
 
                 function _unsupportedIterableToArray(e, t) {
                     if (e) {
                         if ("string" == typeof e) return _arrayLikeToArray(e, t);
-                        var n = Object.prototype.toString.call(e).slice(8, -1);
-                        return "Object" === n && e.constructor && (n = e.constructor.name), "Map" === n || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? _arrayLikeToArray(e, t) : void 0
+                        var o = Object.prototype.toString.call(e).slice(8, -1);
+                        return "Object" === o && e.constructor && (o = e.constructor.name), "Map" === o || "Set" === o ? Array.from(e) : "Arguments" === o || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(o) ? _arrayLikeToArray(e, t) : void 0
                     }
                 }
 
                 function _arrayLikeToArray(e, t) {
                     (null == t || t > e.length) && (t = e.length);
-                    for (var n = 0, o = new Array(t); n < t; n++) o[n] = e[n];
-                    return o
+                    for (var o = 0, n = new Array(t); o < t; o++) n[o] = e[o];
+                    return n
                 }
 
                 function _iterableToArrayLimit(e, t) {
-                    var n = null == e ? null : "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
-                    if (null != n) {
-                        var o, r, i, l, s = [],
+                    var o = null == e ? null : "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
+                    if (null != o) {
+                        var n, r, i, l, s = [],
                             a = !0,
                             c = !1;
                         try {
-                            if (i = (n = n.call(e)).next, 0 === t) {
-                                if (Object(n) !== n) return;
+                            if (i = (o = o.call(e)).next, 0 === t) {
+                                if (Object(o) !== o) return;
                                 a = !1
                             } else
-                                for (; !(a = (o = i.call(n)).done) && (s.push(o.value), s.length !== t); a = !0);
+                                for (; !(a = (n = i.call(o)).done) && (s.push(n.value), s.length !== t); a = !0);
                         } catch (e) {
                             c = !0, r = e
                         } finally {
                             try {
-                                if (!a && null != n.return && (l = n.return(), Object(l) !== l)) return
+                                if (!a && null != o.return && (l = o.return(), Object(l) !== l)) return
                             } finally {
                                 if (c) throw r
                             }
                         }
                         return s
                     }
                 }
 
                 function _arrayWithHoles(e) {
                     if (Array.isArray(e)) return e
                 }
 
                 function ownKeys(e, t) {
-                    var n = Object.keys(e);
+                    var o = Object.keys(e);
                     if (Object.getOwnPropertySymbols) {
-                        var o = Object.getOwnPropertySymbols(e);
-                        t && (o = o.filter((function(t) {
+                        var n = Object.getOwnPropertySymbols(e);
+                        t && (n = n.filter((function(t) {
                             return Object.getOwnPropertyDescriptor(e, t).enumerable
-                        }))), n.push.apply(n, o)
+                        }))), o.push.apply(o, n)
                     }
-                    return n
+                    return o
                 }
 
                 function _objectSpread(e) {
                     for (var t = 1; t < arguments.length; t++) {
-                        var n = null != arguments[t] ? arguments[t] : {};
-                        t % 2 ? ownKeys(Object(n), !0).forEach((function(t) {
-                            _defineProperty(e, t, n[t])
-                        })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : ownKeys(Object(n)).forEach((function(t) {
-                            Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
+                        var o = null != arguments[t] ? arguments[t] : {};
+                        t % 2 ? ownKeys(Object(o), !0).forEach((function(t) {
+                            _defineProperty(e, t, o[t])
+                        })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(o)) : ownKeys(Object(o)).forEach((function(t) {
+                            Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(o, t))
                         }))
                     }
                     return e
                 }
 
-                function _defineProperty(e, t, n) {
+                function _defineProperty(e, t, o) {
                     return (t = _toPropertyKey(t)) in e ? Object.defineProperty(e, t, {
-                        value: n,
+                        value: o,
                         enumerable: !0,
                         configurable: !0,
                         writable: !0
-                    }) : e[t] = n, e
+                    }) : e[t] = o, e
                 }
 
                 function _toPropertyKey(e) {
                     var t = _toPrimitive(e, "string");
                     return "symbol" == _typeof(t) ? t : String(t)
                 }
 
                 function _toPrimitive(e, t) {
                     if ("object" != _typeof(e) || !e) return e;
-                    var n = e[Symbol.toPrimitive];
-                    if (void 0 !== n) {
-                        var o = n.call(e, t || "default");
-                        if ("object" != _typeof(o)) return o;
+                    var o = e[Symbol.toPrimitive];
+                    if (void 0 !== o) {
+                        var n = o.call(e, t || "default");
+                        if ("object" != _typeof(n)) return n;
                         throw new TypeError("@@toPrimitive must return a primitive value.")
                     }
                     return ("string" === t ? String : Number)(e)
                 }
 
                 function isString(e) {
                     return "string" == typeof e || e instanceof String
@@ -151,16 +151,16 @@
                     return (0, react__WEBPACK_IMPORTED_MODULE_0__.useMemo)((function() {
                         return eval("({data, row, column}) => (".concat(dataSelector, ")"))
                     }), [dataSelector])
                 }
 
                 function DashSpreadGrid(e) {
                     var t = e.setProps,
-                        n = (0, react__WEBPACK_IMPORTED_MODULE_0__.useRef)(0),
-                        o = e.data,
+                        o = (0, react__WEBPACK_IMPORTED_MODULE_0__.useRef)(0),
+                        n = e.data,
                         r = e.columns,
                         i = e.rows,
                         l = useResolvedFormatting(e.formatting),
                         s = useResolvedFiltering(e.filtering),
                         a = useResolvedDataSelector(e.data_selector),
                         c = e.pinned_top,
                         u = e.pinned_bottom,
@@ -181,26 +181,26 @@
                         }), [t]),
                         y = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
                             t({
                                 edited_cells: e
                             })
                         }), [t]),
                         w = e.clicked_cell,
-                        E = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
+                        b = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
                             t({
                                 clicked_cell: _objectSpread(_objectSpread({}, e), {}, {
-                                    n: n.current++
+                                    n: o.current++
                                 })
                             })
                         }), [t]),
-                        b = e.clicked_custom_cell,
+                        E = e.clicked_custom_cell,
                         v = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
                             t({
                                 clicked_custom_cell: _objectSpread(_objectSpread({}, e), {}, {
-                                    n: n.current++
+                                    n: o.current++
                                 })
                             })
                         }), [t]),
                         x = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
                             t({
                                 active_columns: e
                             })
@@ -210,15 +210,15 @@
                                 active_rows: e
                             })
                         }), [t]),
                         A = _slicedToArray((0, react__WEBPACK_IMPORTED_MODULE_0__.useState)(null), 2),
                         C = A[0],
                         k = A[1];
                     return C && (0, js_spread_grid__WEBPACK_IMPORTED_MODULE_2__.Z)(C, {
-                        data: o,
+                        data: n,
                         columns: r,
                         rows: i,
                         formatting: l,
                         filtering: s,
                         pinnedTop: c,
                         pinnedBottom: u,
                         pinnedLeft: d,
@@ -227,16 +227,16 @@
                         dataSelector: a,
                         editedCells: h,
                         selectedCells: _,
                         onSelectedCellsChange: m,
                         onEditedCellsChange: y,
                         onFiltersChange: g,
                         clickedCell: w,
-                        onCellClick: E,
-                        clickedCustomCell: b,
+                        onCellClick: b,
+                        clickedCustomCell: E,
                         onCustomCellClick: v,
                         onActiveColumnsChange: x,
                         onActiveRowsChange: R
                     }), react__WEBPACK_IMPORTED_MODULE_0___default().createElement("div", {
                         ref: k
                     })
                 }
@@ -303,212 +303,219 @@
             },
             64: e => {
                 e.exports = window.PropTypes
             },
             196: e => {
                 e.exports = window.React
             },
-            449: (e, t, n) => {
-                function o(e) {
-                    return null === e ? "null" : Array.isArray(e) ? `[${e.map(o).join(",")}]` : "object" == typeof e ? (t = e, `{${Object.keys(t).sort().map((e=>`${e}:${o(t[e])}`)).join(",")}}`) : JSON.stringify(e);
+            906: (e, t, o) => {
+                function n(e) {
+                    return null === e ? "null" : Array.isArray(e) ? `[${e.map(n).join(",")}]` : "object" == typeof e ? (t = e, `{${Object.keys(t).sort().map((e=>`${e}:${n(t[e])}`)).join(",")}}`) : JSON.stringify(e);
                     var t
                 }
 
                 function r(e, t) {
                     return "FILTER" === e.type ^ "FILTER" === t.type ? "FILTER" : "DATA"
                 }
 
-                function i(e, t, n, i) {
+                function i(e, t, o, i) {
                     return e.map((e => {
-                        const l = o(e.columnId),
-                            s = o(e.rowId);
-                        if (!n.has(l)) return null;
+                        const l = n(e.columnId),
+                            s = n(e.rowId);
+                        if (!o.has(l)) return null;
                         if (!i.has(s)) return null;
-                        const a = n.get(l),
+                        const a = o.get(l),
                             c = i.get(s);
                         return {
                             edit: t.resolve(c, a).edit,
                             cell: e,
                             type: r(a, c)
                         }
                     })).filter((e => e?.edit))
                 }
 
                 function l(e, t) {
                     return Math.round(e * t) / t
                 }
 
-                function s(e, t, n) {
-                    const o = e.state,
-                        r = e.canvases[`${t}-${n}`],
-                        i = o.sections[t],
-                        s = o.sections[n],
+                function s(e, t, o) {
+                    const n = e.state,
+                        r = e.canvases[`${t}-${o}`],
+                        i = n.sections[t],
+                        s = n.sections[o],
                         a = s.columns,
                         c = i.rows;
                     if (0 === c.length || 0 === a.length) return void(r.parentElement && r.parentElement.removeChild(r));
                     r.parentElement || e.element.appendChild(r);
                     const u = r.getContext("2d", {
                             alpha: !1
                         }),
-                        d = o.scrollRect,
-                        p = o.textResolver,
-                        f = o.renderFormatResolver,
-                        h = o.borderWidth,
+                        d = n.scrollRect,
+                        p = n.textResolver,
+                        f = n.renderFormatResolver,
+                        h = n.borderWidth,
                         _ = i.showTopBorder,
                         m = i.showBottomBorder,
                         g = s.showLeftBorder,
                         y = s.showRightBorder,
                         w = h / 2,
-                        E = c.length - 1 + (_ ? 1 : 0) + (m ? 1 : 0),
-                        b = a.length - 1 + (g ? 1 : 0) + (y ? 1 : 0),
+                        b = c.length - 1 + (_ ? 1 : 0) + (m ? 1 : 0),
+                        E = a.length - 1 + (g ? 1 : 0) + (y ? 1 : 0),
                         v = c.map((e => e.height)),
                         x = a.map((e => e.width)),
-                        R = x.reduce(((e, t) => e + t), 0) + b * h,
-                        A = v.reduce(((e, t) => e + t), 0) + E * h,
-                        C = "center" === n ? d.left : 0,
+                        R = x.reduce(((e, t) => e + t), 0) + E * h,
+                        A = v.reduce(((e, t) => e + t), 0) + b * h,
+                        C = "center" === o ? d.left : 0,
                         k = "middle" === t ? d.top : 0,
-                        I = "center" === n ? d.width : s.width,
+                        I = "center" === o ? d.width : s.width,
                         D = "middle" === t ? d.height : i.height,
-                        T = x.reduce(((e, t, n) => {
-                            const o = e[n] + t + h;
-                            return e.push(o), e
+                        T = x.reduce(((e, t, o) => {
+                            const n = e[o] + t + h;
+                            return e.push(n), e
                         }), [g ? h : 0]),
-                        M = v.reduce(((e, t, n) => {
-                            const o = e[n] + t + h;
-                            return e.push(o), e
+                        M = v.reduce(((e, t, o) => {
+                            const n = e[o] + t + h;
+                            return e.push(n), e
                         }), [_ ? h : 0]),
                         O = T.slice(0, -1),
-                        L = M.slice(0, -1),
-                        P = Math.max(O.findLastIndex((e => e <= C)), 0),
+                        P = M.slice(0, -1),
+                        L = Math.max(O.findLastIndex((e => e <= C)), 0),
                         B = O.findLastIndex((e => e <= C + I)),
-                        S = Math.max(L.findLastIndex((e => e <= k)), 0),
-                        K = L.findLastIndex((e => e <= k + D)),
-                        W = Math.max(P, g ? 0 : 1),
+                        S = Math.max(P.findLastIndex((e => e <= k)), 0),
+                        K = P.findLastIndex((e => e <= k + D)),
+                        W = Math.max(L, g ? 0 : 1),
                         F = B + (y ? 1 : 0),
                         z = Math.max(S, _ ? 0 : 1),
                         U = K + (m ? 1 : 0),
                         N = Array.from({
                             length: K - S + 1
                         }, ((e, t) => {
-                            const n = c[t + S];
+                            const o = c[t + S];
                             return Array.from({
-                                length: B - P + 1
+                                length: B - L + 1
                             }, ((e, t) => {
-                                const o = a[t + P];
-                                return f.resolve(n, o)
+                                const n = a[t + L];
+                                return f.resolve(o, n)
                             }))
                         })),
-                        j = (e, t) => N[e - S][t - P];
+                        H = (e, t) => N[e - S][t - L];
                     r.width = Math.round(I * devicePixelRatio), r.height = Math.round(D * devicePixelRatio), r.style.width = `${I}px`, r.style.height = `${D}px`, r.style.marginLeft = `${C}px`, r.style.marginTop = `${k}px`, r.style.marginRight = R - I - C + "px", r.style.marginBottom = A - D - k + "px", u.fillStyle = "#E9E9E9", u.fillRect(0, 0, r.width, r.height);
-                    const H = (e, t) => {
+                    const j = (e, t) => {
                             u.setTransform(devicePixelRatio, 0, 0, devicePixelRatio, (e - C) * devicePixelRatio, (t - k) * devicePixelRatio)
                         },
-                        q = (e, t, n, o) => {
-                            u.beginPath(), u.rect(e, t, n, o), u.clip()
+                        q = (e, t, o, n) => {
+                            u.beginPath(), u.rect(e, t, o, n), u.clip()
                         };
-                    for (let e = P; e <= B; e++) {
-                        u.save(), H(T[e], 0), q(0, 0, x[e], A);
+                    for (let e = L; e <= B; e++) {
+                        u.save(), j(T[e], 0), q(0, 0, x[e], A);
                         for (let t = S; t <= K; t++) {
-                            const n = j(t, e),
-                                o = n.style,
+                            const o = H(t, e),
+                                n = o.style,
                                 r = M[t],
                                 i = T[e],
                                 s = x[e],
                                 a = v[t],
-                                c = n.text,
-                                d = o.textBaseline || "middle",
-                                f = n.padding;
-                            if (H(i, r), u.fillStyle = o.background || "white", u.fillRect(0, 0, s, a), "draw" in n && n.draw(u), o.highlight && (u.fillStyle = o.highlight, u.fillRect(0, 0, s, a)), o.corner && (u.fillStyle = o.corner, u.beginPath(), u.moveTo(s - 7, a), u.lineTo(s, a), u.lineTo(s, a - 7), u.fill()), c) {
-                                u.fillStyle = o.foreground || "black", u.font = n.font;
-                                const e = p.getFontMetrics(n.font),
-                                    t = "center" == o.textAlign && p.measureWidth(c, n.font) > s - f.left - f.right ? "left" : o.textAlign || "left";
+                                c = o.text,
+                                d = n.textBaseline || "middle",
+                                f = o.padding;
+                            if (j(i, r), u.fillStyle = n.background || "white", u.fillRect(0, 0, s, a), "draw" in o && o.draw(u), n.highlight && (u.fillStyle = n.highlight, u.fillRect(0, 0, s, a)), n.corner && (u.fillStyle = n.corner, u.beginPath(), u.moveTo(s - 7, a), u.lineTo(s, a), u.lineTo(s, a - 7), u.fill()), c) {
+                                u.fillStyle = n.foreground || "black", u.font = o.font;
+                                const e = p.getFontMetrics(o.font),
+                                    t = "center" == n.textAlign && p.measureWidth(c, o.font) > s - f.left - f.right ? "left" : n.textAlign || "left";
                                 u.textAlign = t;
                                 const r = l("left" === t ? f.left : "center" === t ? s / 2 : "right" === t ? s - f.right : 0, devicePixelRatio),
                                     i = l("top" === d ? e.middle + e.topOffset + f.top : "middle" === d ? a / 2 + e.middle : "bottom" === d ? a + e.middle - e.bottomOffset - f.bottom : 0, devicePixelRatio);
                                 i - e.middle - e.topOffset >= 0 && i - e.middle + e.bottomOffset <= a ? u.fillText(c, r, i) : (u.strokeStyle = "#E9E9E9", u.lineWidth = h, u.beginPath(), u.moveTo(0, h + w), u.lineTo(s, h + w), u.moveTo(0, a - h - w), u.lineTo(s, a - h - w), u.stroke(), u.save(), q(0, 2 * h, s, a - 4 * h), u.fillText(c, r, i), u.restore())
                             }
                         }
                         u.restore()
                     }
-                    H(0, 0);
-                    const $ = (e, t, n, o, r) => {
+                    j(0, 0);
+                    const $ = (e, t, o, n, r) => {
                             if (!r) return;
                             if (0 === r.width) return;
                             const i = r.width / devicePixelRatio,
-                                l = t === o,
+                                l = t === n,
                                 s = e - (l ? i / 2 : 0),
                                 a = t - (l ? 0 : i / 2),
-                                c = n + (l ? i / 2 : 0),
-                                d = o + (l ? 0 : i / 2);
+                                c = o + (l ? i / 2 : 0),
+                                d = n + (l ? 0 : i / 2);
                             u.strokeStyle = r.color || "black", u.lineWidth = i, r.dash ? (u.setLineDash(r.dash.map((e => e / devicePixelRatio))), u.lineDashOffset = l ? s : a) : u.setLineDash([]), u.beginPath(), u.moveTo(s, a), u.lineTo(c, d), u.stroke()
                         },
                         V = (e, t) => e ? t ? e.index > t.index ? e : t : e : t;
                     for (let e = z; e <= U; e++) {
                         const t = e - 1,
-                            n = e;
-                        for (let e = P; e <= B; e++) {
-                            const o = V(t >= S ? j(t, e).style.borderBottom : null, n <= K ? j(n, e).style.borderTop : null);
-                            $(T[e] - w, M[n] - w, T[e + 1] - w, M[n] - w, o)
+                            o = e;
+                        for (let e = L; e <= B; e++) {
+                            const n = V(t >= S ? H(t, e).style.borderBottom : null, o <= K ? H(o, e).style.borderTop : null);
+                            $(T[e] - w, M[o] - w, T[e + 1] - w, M[o] - w, n)
                         }
                     }
                     for (let e = W; e <= F; e++) {
                         const t = e - 1,
-                            n = e;
+                            o = e;
                         for (let e = S; e <= K; e++) {
-                            const o = V(t >= P ? j(e, t).style.borderRight : null, n <= B ? j(e, n).style.borderLeft : null);
-                            $(T[n] - w, M[e] - w, T[n] - w, M[e + 1] - w, o)
+                            const n = V(t >= L ? H(e, t).style.borderRight : null, o <= B ? H(e, o).style.borderLeft : null);
+                            $(T[o] - w, M[e] - w, T[o] - w, M[e + 1] - w, n)
                         }
                     }
                 }
 
                 function a(e) {
                     if (!e.error) try {
                         ! function(e) {
                             s(e, "top", "left"), s(e, "top", "center"), s(e, "top", "right"), s(e, "middle", "left"), s(e, "middle", "center"), s(e, "middle", "right"), s(e, "bottom", "left"), s(e, "bottom", "center"), s(e, "bottom", "right"),
                                 function(e) {
                                     const t = e.element,
-                                        n = e.input,
-                                        o = e.state,
-                                        r = o.inputPlacement;
+                                        o = e.input,
+                                        n = e.state,
+                                        r = n.inputPlacement;
                                     if (!r) {
-                                        if (n.parentElement) {
-                                            const e = document.activeElement === n;
-                                            n.parentElement.removeChild(n), e && t.focus({
+                                        if (o.parentElement) {
+                                            const e = document.activeElement === o;
+                                            o.parentElement.removeChild(o), e && t.focus({
                                                 preventScroll: !0
                                             })
                                         }
                                         return
                                     }
                                     const i = e.canvases[r.section];
-                                    if (n.style.left = "left" in r ? `${r.left}px` : "0", n.style.top = "top" in r ? `${r.top}px` : "0", n.style.right = "right" in r ? `${r.right}px` : "0", n.style.bottom = "bottom" in r ? `${r.bottom}px` : "0", n.style.marginLeft = "marginLeft" in r ? `${r.marginLeft}px` : "0", n.style.marginTop = "marginTop" in r ? `${r.marginTop}px` : "0", n.style.width = `${r.width}px`, n.style.height = `${r.height}px`, n.style.gridArea = i.style.gridArea, n.style.zIndex = i.style.zIndex, n.style.backgroundColor = o.isTextValid ? "white" : "#eb3434", !n.parentElement) {
+                                    if (o.style.left = "left" in r ? `${r.left}px` : "0", o.style.top = "top" in r ? `${r.top}px` : "0", o.style.right = "right" in r ? `${r.right}px` : "0", o.style.bottom = "bottom" in r ? `${r.bottom}px` : "0", o.style.marginLeft = "marginLeft" in r ? `${r.marginLeft}px` : "0", o.style.marginTop = "marginTop" in r ? `${r.marginTop}px` : "0", o.style.width = `${r.width}px`, o.style.height = `${r.height}px`, o.style.gridArea = i.style.gridArea, o.style.zIndex = i.style.zIndex, o.style.backgroundColor = n.isTextValid ? "white" : "#eb3434", !o.parentElement) {
                                         const e = document.activeElement === t;
-                                        t.appendChild(n), e && n.focus({
+                                        t.appendChild(o), e && o.focus({
                                             preventScroll: !0
                                         })
                                     }
                                 }(e),
                                 function(e) {
                                     const t = e.element,
-                                        n = e.state;
-                                    n.resizableColumn && n.resizableRow ? t.style.cursor = "nwse-resize" : n.resizableColumn ? t.style.cursor = "col-resize" : n.resizableRow ? t.style.cursor = "row-resize" : t.style.cursor = "default"
+                                        o = e.state;
+                                    o.resizableColumn && o.resizableRow ? t.style.cursor = "nwse-resize" : o.resizableColumn ? t.style.cursor = "col-resize" : o.resizableRow ? t.style.cursor = "row-resize" : t.style.cursor = "default"
+                                }(e),
+                                function(e) {
+                                    const t = e.element,
+                                        o = e.tooltip,
+                                        n = e.state.tooltip,
+                                        r = e.state.tooltipPlacement;
+                                    r ? (o.innerHTML = n, o.style.left = `${r.left}px`, o.style.top = `${r.top}px`, o.parentElement || (t.appendChild(o), o.showPopover())) : o.parentElement && o.parentElement.removeChild(o)
                                 }(e)
                         }(e)
                     } catch (t) {
                         e.error = t
                     }
                     e.error && function(e) {
                         if (e.errorRendered) return;
                         e.errorRendered = !0;
                         const t = e.element,
-                            n = e.error;
-                        t.style.backgroundColor = "#9f0000", t.style.color = "white", t.style.padding = "20px", t.style.display = "flex", t.style.flexDirection = "column", t.style.userSelect = "text", t.innerHTML = `\n        <div style="font-size: 16px;">\n            An error occurred while rendering the grid, please contact the support.\n        </div>\n        <div style="font-size: 20px; font-weight: bold; padding: 20px 0;">\n            ${n.message}\n        </div>\n        <div style="font-size: 16px; white-space: pre-wrap;">${n.stack}</div>\n    `
+                            o = e.error;
+                        t.style.backgroundColor = "#9f0000", t.style.color = "white", t.style.padding = "20px", t.style.display = "flex", t.style.flexDirection = "column", t.style.userSelect = "text", t.innerHTML = `\n        <div style="font-size: 16px;">\n            An error occurred while rendering the grid, please contact the support.\n        </div>\n        <div style="font-size: 20px; font-weight: bold; padding: 20px 0;">\n            ${o.message}\n        </div>\n        <div style="font-size: 16px; white-space: pre-wrap;">${o.stack}</div>\n    `
                     }(e)
                 }
-                n.d(t, {
-                    Z: () => qe
+                o.d(t, {
+                    Z: () => Ye
                 });
                 const c = {
                     value: ({
                         newValue: e
                     }) => e || "",
                     text: ({
                         newValue: e
@@ -518,15 +525,15 @@
                         parse: ({
                             string: e
                         }) => e,
                         autoCommit: !0
                     }
                 };
 
-                function u(e, t, n) {
+                function u(e, t, o) {
                     return [{
                         column: {
                             type: "DATA"
                         },
                         row: {
                             type: "HEADER"
                         },
@@ -579,66 +586,66 @@
                         column: {
                             type: "DATA"
                         },
                         row: {
                             type: "DATA"
                         },
                         value: t
-                    }, ...e, ...n.map((({
+                    }, ...e, ...o.map((({
                         columnId: e,
                         rowId: t,
-                        direction: o
+                        direction: n
                     }, r) => ({
                         column: {
                             id: e
                         },
                         row: {
                             id: t
                         },
                         text: ({
                             value: e,
                             text: t
-                        }) => `${n.length>1?r+1:""}${"ASC"===o?"⇣":"⇡"} ${t||e}`
+                        }) => `${o.length>1?r+1:""}${"ASC"===n?"⇣":"⇡"} ${t||e}`
                     })))]
                 }
                 const d = ["column", "row", "condition"];
 
                 function p(e) {
                     return Object.keys(e).length > Object.keys(e).filter((e => d.includes(e))).length
                 }
 
                 function f(e, t) {
-                    const n = [...d, ...t];
+                    const o = [...d, ...t];
                     return e.map((e => function(e, t) {
-                        const n = {};
-                        for (const o of t) o in e && (n[o] = e[o]);
-                        return n
-                    }(e, n))).filter(p)
+                        const o = {};
+                        for (const n of t) n in e && (o[n] = e[n]);
+                        return o
+                    }(e, o))).filter(p)
                 }
 
                 function h(e) {
                     return f(e, ["value", "text", "edit"])
                 }
 
                 function _(e, t) {
                     return t ? e + "99" : e + "33"
                 }
 
-                function m(e, t, n, r, i, l, s, a, c, u) {
-                    const d = n ? o(n.columnId) : null,
-                        p = n ? o(n.rowId) : null,
+                function m(e, t, o, r, i, l, s, a, c, u) {
+                    const d = o ? n(o.columnId) : null,
+                        p = o ? n(o.rowId) : null,
                         f = null !== c,
                         h = null !== a || f,
                         m = u + 2,
                         g = u + 4,
-                        y = (e, t, n, o) => {
-                            if (n < 0 || n >= e.length) return !1;
-                            if (o < 0 || o >= t.length) return !1;
-                            const i = e[n].key,
-                                l = t[o].key;
+                        y = (e, t, o, n) => {
+                            if (o < 0 || o >= e.length) return !1;
+                            if (n < 0 || n >= t.length) return !1;
+                            const i = e[o].key,
+                                l = t[n].key;
                             return r.isKeySelected(i, l)
                         },
                         w = (e, t) => e ? [t] : [];
                     return [{
                         column: {
                             type: "DATA"
                         },
@@ -736,53 +743,53 @@
                         },
                         row: {
                             type: "ANY"
                         },
                         condition: ({
                             rows: e,
                             columns: t,
-                            row: n,
-                            column: o
-                        }) => y(e, t, n.index, o.index),
+                            row: o,
+                            column: n
+                        }) => y(e, t, o.index, n.index),
                         style: ({
                             rows: e,
                             columns: t,
-                            row: n,
-                            column: o,
+                            row: o,
+                            column: n,
                             edit: r
                         }) => ({
-                            ...y(e, t, n.index - 1, o.index) ? {} : {
+                            ...y(e, t, o.index - 1, n.index) ? {} : {
                                 borderTop: {
                                     width: m,
                                     color: "#596959",
                                     index: Number.MAX_SAFE_INTEGER
                                 }
                             },
-                            ...y(e, t, n.index + 1, o.index) ? {} : {
+                            ...y(e, t, o.index + 1, n.index) ? {} : {
                                 borderBottom: {
                                     width: m,
                                     color: "#596959",
                                     index: Number.MAX_SAFE_INTEGER
                                 }
                             },
-                            ...y(e, t, n.index, o.index - 1) ? {} : {
+                            ...y(e, t, o.index, n.index - 1) ? {} : {
                                 borderLeft: {
                                     width: m,
                                     color: "#596959",
                                     index: Number.MAX_SAFE_INTEGER
                                 }
                             },
-                            ...y(e, t, n.index, o.index + 1) ? {} : {
+                            ...y(e, t, o.index, n.index + 1) ? {} : {
                                 borderRight: {
                                     width: m,
                                     color: "#596959",
                                     index: Number.MAX_SAFE_INTEGER
                                 }
                             },
-                            highlight: _(r ? "#798d9c" : "#819481", d !== o.key || p !== n.key)
+                            highlight: _(r ? "#798d9c" : "#819481", d !== n.key || p !== o.key)
                         })
                     }, {
                         column: {
                             type: "ANY"
                         },
                         row: {
                             type: "ANY"
@@ -793,29 +800,29 @@
                         }) => i.isKeySelected(e.key, t.key),
                         style: ({
                             row: e,
                             column: t
                         }) => ({
                             highlight: _("#93a8b8", d !== t.key || p !== e.key)
                         })
-                    }, ...w(n, {
+                    }, ...w(o, {
                         column: {
-                            id: n?.columnId
+                            id: o?.columnId
                         },
                         row: {
-                            id: n?.rowId
+                            id: o?.rowId
                         },
                         style: {
                             highlight: "#ffffffaa"
                         }
                     }), ...s.map((({
                         columnId: e,
                         rowId: t,
-                        direction: n
-                    }, o) => ({
+                        direction: o
+                    }, n) => ({
                         column: {
                             id: e
                         },
                         row: {
                             id: t
                         },
                         style: {
@@ -874,43 +881,43 @@
                                 color: "cornflowerblue"
                             }
                         }
                     })]
                 }
 
                 function g(e, t) {
-                    const n = t.filter((e => "BEGIN" === e.pinned)).length,
-                        o = t.filter((e => "END" === e.pinned)).length,
-                        r = t.length - n - o,
+                    const o = t.filter((e => "BEGIN" === e.pinned)).length,
+                        n = t.filter((e => "END" === e.pinned)).length,
+                        r = t.length - o - n,
                         i = e.filter((e => "BEGIN" === e.pinned)).length,
                         l = e.filter((e => "END" === e.pinned)).length,
                         s = e.length - i - l,
-                        a = t.slice(0, n),
-                        c = t.slice(t.length - o, t.length),
-                        u = t.slice(n, t.length - o),
+                        a = t.slice(0, o),
+                        c = t.slice(t.length - n, t.length),
+                        u = t.slice(o, t.length - n),
                         d = e.slice(0, i),
                         p = e.slice(e.length - l, e.length),
                         f = e.slice(i, e.length - l),
-                        h = n > 0,
+                        h = o > 0,
                         _ = i > 0,
                         m = r > 0 || !h,
                         g = !h,
-                        y = !(o > 0),
+                        y = !(n > 0),
                         w = s > 0 || !_,
-                        E = !_,
-                        b = !(l > 0),
-                        v = (e, t, n) => {
+                        b = !_,
+                        E = !(l > 0),
+                        v = (e, t, o) => {
                             if (0 === e.length) return 0;
-                            const o = t ? e.at(0).topWithBorder : e.at(0).top;
-                            return (n ? e.at(-1).bottomWithBorder : e.at(-1).bottom) - o
+                            const n = t ? e.at(0).topWithBorder : e.at(0).top;
+                            return (o ? e.at(-1).bottomWithBorder : e.at(-1).bottom) - n
                         },
-                        x = (e, t, n) => {
+                        x = (e, t, o) => {
                             if (0 === e.length) return 0;
-                            const o = t ? e.at(0).leftWithBorder : e.at(0).left;
-                            return (n ? e.at(-1).rightWithBorder : e.at(-1).right) - o
+                            const n = t ? e.at(0).leftWithBorder : e.at(0).left;
+                            return (o ? e.at(-1).rightWithBorder : e.at(-1).right) - n
                         };
                     return {
                         top: {
                             rows: a,
                             showTopBorder: !0,
                             showBottomBorder: !0,
                             height: v(a, !0, !0)
@@ -937,150 +944,150 @@
                             columns: p,
                             showLeftBorder: w,
                             showRightBorder: !0,
                             width: x(p, w, !0)
                         },
                         center: {
                             columns: f,
-                            showLeftBorder: E,
-                            showRightBorder: b,
-                            width: x(f, E, b)
+                            showLeftBorder: b,
+                            showRightBorder: E,
+                            width: x(f, b, E)
                         }
                     }
                 }
 
                 function y(e, t) {
                     return [...e, ...t.map((e => ({
                         columnId: e.columnId,
                         rowId: e.rowId,
                         value: e.expression
                     })))]
                 }
                 class w {
                     constructor(e) {
                         this.lookup = new Map, e.forEach((e => {
-                            const t = o(e.rowId),
-                                n = o(e.columnId);
-                            this.lookup.has(t) || this.lookup.set(t, new Map), this.lookup.get(t).set(n, e.value)
+                            const t = n(e.rowId),
+                                o = n(e.columnId);
+                            this.lookup.has(t) || this.lookup.set(t, new Map), this.lookup.get(t).set(o, e.value)
                         }))
                     }
                     hasValueByKey(e, t) {
                         return this.lookup.has(e) && this.lookup.get(e).has(t)
                     }
                     getValueByKey(e, t) {
                         if (this.hasValueByKey(e, t)) return this.lookup.get(e).get(t)
                     }
                     hasValueById(e, t) {
-                        return this.hasValueByKey(o(e), o(t))
+                        return this.hasValueByKey(n(e), n(t))
                     }
                     getValueById(e, t) {
-                        return this.getValueByKey(o(e), o(t))
+                        return this.getValueByKey(n(e), n(t))
                     }
                 }
 
-                function E(e) {
+                function b(e) {
                     return new w(e)
                 }
-                class b {
+                class E {
                     constructor(e) {
                         this.lookup = new Map, e.forEach((e => {
-                            const t = o(e.rowId),
-                                n = o(e.columnId);
-                            this.lookup.has(t) || this.lookup.set(t, new Set), this.lookup.get(t).add(n)
+                            const t = n(e.rowId),
+                                o = n(e.columnId);
+                            this.lookup.has(t) || this.lookup.set(t, new Set), this.lookup.get(t).add(o)
                         }))
                     }
                     isKeySelected(e, t) {
                         return this.lookup.has(e) && this.lookup.get(e).has(t)
                     }
                     isIdSelected(e, t) {
-                        return this.isKeySelected(o(e), o(t))
+                        return this.isKeySelected(n(e), n(t))
                     }
                 }
 
                 function v(e) {
-                    return new b(e)
+                    return new E(e)
                 }
 
                 function x(e, t) {
                     return "function" == typeof e ? e(t) : e
                 }
 
-                function R(e, t, n, o) {
-                    return e < n ? "BEGIN" : e >= t - o ? "END" : void 0
+                function R(e, t, o, n) {
+                    return e < o ? "BEGIN" : e >= t - n ? "END" : void 0
                 }
 
-                function A(e, t, n) {
+                function A(e, t, o) {
                     return e.map(((r, i) => {
                         const l = "id" in r ? r.id : r.type;
                         return {
                             ...r,
                             id: l,
                             type: r.type || "DATA",
                             index: i,
-                            key: o(l),
-                            pinned: R(i, e.length, t, n),
+                            key: n(l),
+                            pinned: R(i, e.length, t, o),
                             header: "header" in r ? r.header : l,
                             labels: r.labels || []
                         }
                     }))
                 }
 
-                function C(e, t, n, r) {
+                function C(e, t, o, r) {
                     const i = new Map(r.map((({
                         columnId: e,
                         width: t
-                    }) => [o(e), t])));
-                    return A(e, t, n).map((e => ({
+                    }) => [n(e), t])));
+                    return A(e, t, o).map((e => ({
                         ...e,
                         width: i.has(e.key) ? i.get(e.key) : "width" in e ? e.width : "fit"
                     })))
                 }
 
-                function k(e, t, n, r) {
+                function k(e, t, o, r) {
                     const i = new Map(r.map((({
                         rowId: e,
                         height: t
-                    }) => [o(e), t])));
-                    return A(e, t, n).map((e => ({
+                    }) => [n(e), t])));
+                    return A(e, t, o).map((e => ({
                         ...e,
                         height: i.has(e.key) ? i.get(e.key) : "height" in e ? e.height : "fit"
                     })))
                 }
 
-                function I(e, t, n) {
-                    let o = n;
+                function I(e, t, o) {
+                    let n = o;
                     return e.map(((e, r) => {
                         const i = l("width" in e ? e.width : 100, t),
                             s = {
                                 ...e,
                                 index: r,
                                 width: i,
-                                leftWithBorder: o - n,
-                                left: o,
-                                right: o + i,
-                                rightWithBorder: o + i + n
+                                leftWithBorder: n - o,
+                                left: n,
+                                right: n + i,
+                                rightWithBorder: n + i + o
                             };
-                        return o += s.width + n, s
+                        return n += s.width + o, s
                     }))
                 }
 
-                function D(e, t, n) {
-                    let o = n;
+                function D(e, t, o) {
+                    let n = o;
                     return e.map(((e, r) => {
                         const i = l("height" in e ? e.height : 20, t),
                             s = {
                                 ...e,
                                 index: r,
                                 height: i,
-                                topWithBorder: o - n,
-                                top: o,
-                                bottom: o + i,
-                                bottomWithBorder: o + i + n
+                                topWithBorder: n - o,
+                                top: n,
+                                bottom: n + i,
+                                bottomWithBorder: n + i + o
                             };
-                        return o += s.height + n, s
+                        return n += s.height + o, s
                     }))
                 }
                 const T = "12px Calibri",
                     M = {
                         top: 2,
                         right: 5,
                         bottom: 2,
@@ -1091,221 +1098,221 @@
                         FILTER: ["FILTER"],
                         DATA: ["DATA"],
                         CUSTOM: ["CUSTOM"],
                         ANY: ["HEADER", "DATA", "FILTER", "CUSTOM"],
                         SPECIAL: ["HEADER", "FILTER", "CUSTOM"],
                         undefined: []
                     };
-                class L {
+                class P {
                     byKey = new Map;
                     byIndex = new Map;
                     byLabel = new Map;
                     byType = new Map
                 }
-                class P {
-                    lookup = new L;
+                class L {
+                    lookup = new P;
                     hasRules = !1;
-                    addRule(e, t, n) {
+                    addRule(e, t, o) {
                         if (this.hasRules = !0, Array.isArray(e))
-                            for (const o of e) this.addRule(o, t, n);
+                            for (const n of e) this.addRule(n, t, o);
                         else if (Array.isArray(t))
-                            for (const o of t) this.addRule(e, o, n);
+                            for (const n of t) this.addRule(e, n, o);
                         else {
                             e = e ? "id" in e ? {
-                                key: o(e.id)
+                                key: n(e.id)
                             } : e : {
                                 type: "DATA"
                             }, t = t ? "id" in t ? {
-                                key: o(t.id)
+                                key: n(t.id)
                             } : t : {
                                 type: "DATA"
                             }, "key" in e && i(this.lookup.byKey, e.key), "index" in e && i(this.lookup.byIndex, e.index), "label" in e && i(this.lookup.byLabel, e.label);
                             for (const t of O[e.type]) i(this.lookup.byType, t)
                         }
 
                         function r(e, t) {
-                            e.has(t) || e.set(t, []), e.get(t).push(n)
+                            e.has(t) || e.set(t, []), e.get(t).push(o)
                         }
 
-                        function i(e, n) {
-                            e.has(n) || e.set(n, new L), "key" in t && r(e.get(n).byKey, t.key), "index" in t && r(e.get(n).byIndex, t.index), "label" in t && r(e.get(n).byLabel, t.label);
-                            for (const o of O[t.type]) r(e.get(n).byType, o)
+                        function i(e, o) {
+                            e.has(o) || e.set(o, new P), "key" in t && r(e.get(o).byKey, t.key), "index" in t && r(e.get(o).byIndex, t.index), "label" in t && r(e.get(o).byLabel, t.label);
+                            for (const n of O[t.type]) r(e.get(o).byType, n)
                         }
                     }
                     getRules(e, t) {
-                        const n = [];
-                        if (!this.hasRules) return n;
+                        const o = [];
+                        if (!this.hasRules) return o;
 
-                        function o(e) {
-                            for (const t of e) n.push(t)
+                        function n(e) {
+                            for (const t of e) o.push(t)
                         }
 
                         function r(e) {
-                            e.byKey.has(t.key) && o(e.byKey.get(t.key)), e.byIndex.has(t.index) && o(e.byIndex.get(t.index)), e.byType.has(t.type) && o(e.byType.get(t.type));
-                            for (const n of t.labels) e.byLabel.has(n) && o(e.byLabel.get(n))
+                            e.byKey.has(t.key) && n(e.byKey.get(t.key)), e.byIndex.has(t.index) && n(e.byIndex.get(t.index)), e.byType.has(t.type) && n(e.byType.get(t.type));
+                            for (const o of t.labels) e.byLabel.has(o) && n(e.byLabel.get(o))
                         }
                         this.lookup.byKey.has(e.key) && r(this.lookup.byKey.get(e.key)), this.lookup.byIndex.has(e.index) && r(this.lookup.byIndex.get(e.index)), this.lookup.byType.has(e.type) && r(this.lookup.byType.get(e.type));
                         for (const t of e.labels) this.lookup.byLabel.has(t) && r(this.lookup.byLabel.get(t));
-                        return n
+                        return o
                     }
                 }
                 const B = ["borderTop", "borderRight", "borderBottom", "borderLeft"],
                     S = {
                         validate: () => !0,
                         parse: ({
                             string: e
                         }) => e
                     };
 
                 function K(e, t) {
-                    const n = {
+                    const o = {
                         ...e
                     };
-                    if ("border" in n) {
-                        for (const e of B) n[e] = n.border;
-                        delete n.border
+                    if ("border" in o) {
+                        for (const e of B) o[e] = o.border;
+                        delete o.border
                     }
-                    for (const e of B) e in n && (n[e] = {
-                        ...n[e],
+                    for (const e of B) e in o && (o[e] = {
+                        ...o[e],
                         index: t
                     });
-                    return n
+                    return o
                 }
 
                 function W(e, t) {
                     if (!1 !== e.edit) return !0 === e.edit ? "edit" in t ? t.edit : S : "edit" in t ? {
                         ...t.edit,
                         ...e.edit
                     } : {
                         ...S,
                         ...e.edit
                     }
                 }
                 class F {
                     constructor(e) {
-                        this.rulesLookup = new P;
-                        for (const [t, n] of e.entries()) {
+                        this.rulesLookup = new L;
+                        for (const [t, o] of e.entries()) {
                             const e = {
                                 index: t
                             };
-                            "condition" in n && (e.condition = n.condition), "style" in n && (e.style = "function" == typeof n.style ? n.style : () => n.style), "value" in n && (e.value = "function" == typeof n.value ? n.value : () => n.value), "text" in n && (e.text = "function" == typeof n.text ? n.text : () => n.text), "font" in n && (e.font = "function" == typeof n.font ? n.font : () => n.font), "padding" in n && (e.padding = "function" == typeof n.padding ? n.padding : () => n.padding), "edit" in n && (e.edit = n.edit), "draw" in n && (e.draw = n.draw), this.rulesLookup.addRule(n.column, n.row, e)
+                            "condition" in o && (e.condition = o.condition), "style" in o && (e.style = "function" == typeof o.style ? o.style : () => o.style), "value" in o && (e.value = "function" == typeof o.value ? o.value : () => o.value), "text" in o && (e.text = "function" == typeof o.text ? o.text : () => o.text), "font" in o && (e.font = "function" == typeof o.font ? o.font : () => o.font), "padding" in o && (e.padding = "function" == typeof o.padding ? o.padding : () => o.padding), "edit" in o && (e.edit = o.edit), "tooltip" in o && (e.tooltip = "function" == typeof o.tooltip ? o.tooltip : () => o.tooltip), "draw" in o && (e.draw = o.draw), this.rulesLookup.addRule(o.column, o.row, e)
                         }
                     }
-                    resolve(e, t, n, o, r, i) {
-                        const l = this.rulesLookup.getRules(r, o).sort(((e, t) => e.index - t.index)).filter(((e, t, n) => e.index !== n[t - 1]?.index));
-                        let s, a = {
+                    resolve(e, t, o, n, r, i) {
+                        const l = this.rulesLookup.getRules(r, n).sort(((e, t) => e.index - t.index)).filter(((e, t, o) => e.index !== o[t - 1]?.index));
+                        let s, a, c = {
                                 data: e,
                                 rows: t,
-                                columns: n,
-                                row: o,
+                                columns: o,
+                                row: n,
                                 column: r
                             },
-                            c = {},
-                            u = M,
-                            d = T;
-                        i.hasValueByKey(o.key, r.key) && (a = {
-                            ...a,
-                            newValue: i.getValueByKey(o.key, r.key)
+                            u = {},
+                            d = M,
+                            p = T;
+                        i.hasValueByKey(n.key, r.key) && (c = {
+                            ...c,
+                            newValue: i.getValueByKey(n.key, r.key)
                         });
                         for (const e of l)
-                            if ((!("condition" in e) || e.condition(a)) && ("value" in e && (a = {
-                                    ...a,
-                                    value: e.value(a)
-                                }), "style" in e && (c = {
+                            if ((!("condition" in e) || e.condition(c)) && ("value" in e && (c = {
                                     ...c,
-                                    ...K(e.style(a), e.index)
-                                }), "text" in e && (a = {
-                                    ...a,
-                                    text: e.text(a)
-                                }), "font" in e && (d = e.font(a)), "padding" in e && (u = {
+                                    value: e.value(c)
+                                }), "style" in e && (u = {
                                     ...u,
-                                    ...e.padding(a)
-                                }), "edit" in e && (a = {
-                                    ...a,
-                                    edit: W(e, a)
-                                }), "draw" in e)) {
-                                const t = a;
-                                s = n => e.draw({
+                                    ...K(e.style(c), e.index)
+                                }), "text" in e && (c = {
+                                    ...c,
+                                    text: e.text(c)
+                                }), "font" in e && (p = e.font(c)), "padding" in e && (d = {
+                                    ...d,
+                                    ...e.padding(c)
+                                }), "edit" in e && (c = {
+                                    ...c,
+                                    edit: W(e, c)
+                                }), "tooltip" in e && (a = e.tooltip(c)), "draw" in e)) {
+                                const t = c;
+                                s = o => e.draw({
                                     ...t,
-                                    ctx: n
+                                    ctx: o
                                 })
-                            } const p = function(e) {
+                            } const f = function(e) {
                                 return "text" in e ? `${e.text}` : "newValue" in e ? `${e.newValue}` : void 0 !== e.value ? `${e.value}` : ""
-                            }(a),
-                            f = {
-                                style: c,
+                            }(c),
+                            h = {
+                                style: u,
                                 visible: !0,
-                                text: p,
-                                padding: u,
-                                font: d
+                                text: f,
+                                padding: d,
+                                font: p
                             };
-                        return "value" in a && (f.value = a.value), "edit" in a && void 0 !== a.edit && (f.edit = a.edit), void 0 !== s && (f.draw = s), f
+                        return "value" in c && (h.value = c.value), "edit" in c && void 0 !== c.edit && (h.edit = c.edit), void 0 !== a && (h.tooltip = a), void 0 !== s && (h.draw = s), h
                     }
                 }
 
                 function z(e) {
                     return new F(e)
                 }
                 class U {
-                    constructor(e, t, n, o, r) {
-                        this.formattingRules = e, this.data = t, this.rows = n, this.columns = o, this.edition = r
+                    constructor(e, t, o, n, r) {
+                        this.formattingRules = e, this.data = t, this.rows = o, this.columns = n, this.edition = r
                     }
                     resolve(e, t) {
                         return this.formattingRules.resolve(this.data, this.rows, this.columns, e, t, this.edition)
                     }
                 }
 
-                function N(e, t, n, o, r) {
-                    return new U(e, t, n, o, r)
+                function N(e, t, o, n, r) {
+                    return new U(e, t, o, n, r)
                 }
 
-                function j(e, t, n) {
+                function H(e, t, o) {
                     const r = new Map;
                     for (const i of e) {
-                        const e = o(i[t]),
-                            l = o(i[n]);
+                        const e = n(i[t]),
+                            l = n(i[o]);
                         r.has(e) || r.set(e, new Map), r.get(e).set(l, i.expression)
                     }
                     return r
                 }
 
-                function H(e, t, n, o, r, i, l) {
+                function j(e, t, o, n, r, i, l) {
                     if (0 === e.length) return r;
-                    const s = j(e, "columnId", "rowId"),
+                    const s = H(e, "columnId", "rowId"),
                         a = i.filter((e => "FILTER" !== e.type && s.has(e.key)));
                     return 0 === a.length ? r : r.filter((e => {
                         for (const c of a) {
-                            const a = n.resolve(o, r, i, e, c, l),
+                            const a = o.resolve(n, r, i, e, c, l),
                                 u = s.get(c.key);
-                            if (!t.resolve(o, r, i, e, c, a.value, a.text, u)) return !1
+                            if (!t.resolve(n, r, i, e, c, a.value, a.text, u)) return !1
                         }
                         return !0
                     }))
                 }
 
-                function q(e, t, n, o, r, i, l) {
+                function q(e, t, o, n, r, i, l) {
                     if (0 === e.length) return i;
-                    const s = j(e, "rowId", "columnId"),
+                    const s = H(e, "rowId", "columnId"),
                         a = r.filter((e => "FILTER" !== e.type && s.has(e.key)));
                     return 0 === a.length ? i : i.filter((e => {
                         for (const c of a) {
-                            const a = n.resolve(o, r, i, c, e, l),
+                            const a = o.resolve(n, r, i, c, e, l),
                                 u = s.get(c.key);
-                            if (!t.resolve(o, r, i, c, e, a.value, a.text, u)) return !1
+                            if (!t.resolve(n, r, i, c, e, a.value, a.text, u)) return !1
                         }
                         return !0
                     }))
                 }
 
-                function $(e, t, n, o) {
+                function $(e, t, o, n) {
                     return {
                         top: e,
                         bottom: t,
-                        left: n,
-                        right: o
+                        left: o,
+                        right: n
                     }
                 }
 
                 function V(e, t) {
                     return {
                         width: e.length ? e.at(-1).rightWithBorder : 0,
                         height: t.length ? t.at(-1).bottomWithBorder : 0
@@ -1313,55 +1320,55 @@
                 }
                 class G {
                     constructor() {
                         this.canvas = document.createElement("canvas"), this.context = this.canvas.getContext("2d"), this.fontMetrics = new Map
                     }
                     measureWidth(e, t) {
                         if (!e) return 0;
-                        const n = this.context;
-                        return n.font = t || T, n.measureText(e).width
+                        const o = this.context;
+                        return o.font = t || T, o.measureText(e).width
                     }
                     measureHeight(e, t) {
-                        let n = 1;
-                        for (const t of e) "\n" === t && n++;
-                        return n * this.getFontMetrics(t).height
+                        let o = 1;
+                        for (const t of e) "\n" === t && o++;
+                        return o * this.getFontMetrics(t).height
                     }
                     getFontMetrics(e) {
                         const t = e;
                         if (this.fontMetrics.has(t)) return this.fontMetrics.get(t);
-                        const n = this.context;
-                        n.font = e || T;
-                        const o = n.measureText("X"),
-                            r = (o.actualBoundingBoxDescent - o.actualBoundingBoxAscent) / 2,
+                        const o = this.context;
+                        o.font = e || T;
+                        const n = o.measureText("X"),
+                            r = (n.actualBoundingBoxDescent - n.actualBoundingBoxAscent) / 2,
                             i = {
-                                topOffset: r + o.fontBoundingBoxAscent,
+                                topOffset: r + n.fontBoundingBoxAscent,
                                 middle: -r,
-                                bottomOffset: o.fontBoundingBoxDescent - r,
-                                height: o.fontBoundingBoxAscent + o.fontBoundingBoxDescent
+                                bottomOffset: n.fontBoundingBoxDescent - r,
+                                height: n.fontBoundingBoxAscent + n.fontBoundingBoxDescent
                             };
                         return this.fontMetrics.set(t, i), i
                     }
                 }
 
                 function Y() {
                     return new G
                 }
 
                 function X(e, t) {
                     return t.top >= e.top && t.left >= e.left && t.top + t.height <= e.top + e.height && t.left + t.width <= e.left + e.width
                 }
 
                 function Z(e, t) {
-                    const n = {
+                    const o = {
                         top: Math.max(e.top, t.top),
                         left: Math.max(e.left, t.left),
                         width: Math.min(e.left + e.width, t.left + t.width) - Math.max(e.left, t.left),
                         height: Math.min(e.top + e.height, t.top + t.height) - Math.max(e.top, t.top)
                     };
-                    return n.width >= 0 && n.height >= 0 ? n : {
+                    return o.width >= 0 && o.height >= 0 ? o : {
                         top: e.top,
                         left: e.left,
                         width: 0,
                         height: 0
                     }
                 }
 
@@ -1383,48 +1390,48 @@
                         top: e.top,
                         left: e.left,
                         width: Math.max(0, e.width - t.left - t.right),
                         height: Math.max(0, e.height - t.top - t.bottom)
                     }
                 }
                 const te = 200,
-                    ne = 400,
-                    oe = {
+                    oe = 400,
+                    ne = {
                         left: 0,
                         top: 0,
                         width: 0,
                         height: 0
                     };
 
-                function re(e, t, n, o) {
+                function re(e, t, o, n) {
                     const r = t.x,
                         i = t.y,
                         l = e.scrollLeft,
                         s = e.scrollTop,
                         a = e.clientWidth,
                         c = e.clientHeight;
                     return {
-                        x: r <= n.left ? r : r >= a ? r + l : r >= a - n.right ? o.width - a + r : r + l,
-                        y: i <= n.top ? i : i >= c ? i + s : i >= c - n.bottom ? o.height - c + i : i + s
+                        x: r <= o.left ? r : r >= a ? r + l : r >= a - o.right ? n.width - a + r : r + l,
+                        y: i <= o.top ? i : i >= c ? i + s : i >= c - o.bottom ? n.height - c + i : i + s
                     }
                 }
 
                 function ie(e) {
                     return e.reduce(((e, t) => e.set(t.key, t)), new Map)
                 }
 
-                function le(e, t, n, r, i, l, s, a) {
+                function le(e, t, o, r, i, l, s, a) {
                     if (!e) return [];
                     if (t) return [];
                     if (!r) return [];
-                    if (!n) return [];
-                    const c = o(n.columnId),
-                        u = o(n.rowId),
-                        d = o(r.columnId),
-                        p = o(r.rowId);
+                    if (!o) return [];
+                    const c = n(o.columnId),
+                        u = n(o.rowId),
+                        d = n(r.columnId),
+                        p = n(r.rowId);
                     if (!s.has(c)) return [];
                     if (!a.has(u)) return [];
                     if (!s.has(d)) return [];
                     if (!a.has(p)) return [];
                     const f = Math.min(s.get(c).index, s.get(d).index),
                         h = Math.max(s.get(c).index, s.get(d).index),
                         _ = Math.min(a.get(u).index, a.get(p).index),
@@ -1432,140 +1439,143 @@
                     return i.slice(f, h + 1).flatMap((e => l.slice(_, m + 1).map((t => ({
                         rowId: t.id,
                         columnId: e.id
                     })))))
                 }
 
                 function se(e, t) {
-                    const n = function(e) {
+                    const o = function(e) {
                             return "BEGIN" === e.pinned ? "top" : "END" === e.pinned ? "bottom" : "middle"
                         }(t),
-                        o = function(e) {
+                        n = function(e) {
                             return "BEGIN" === e.pinned ? "left" : "END" === e.pinned ? "right" : "center"
                         }(e);
-                    return `${n}-${o}`
+                    return `${o}-${n}`
                 }
 
-                function ae(e, t, n, r, i) {
-                    if (!t) return null;
-                    const l = o(t.columnId),
-                        s = o(t.rowId);
-                    if (!n.has(l)) return null;
-                    if (!r.has(s)) return null;
-                    const a = n.get(l),
-                        c = r.get(s);
-                    if (0 === e.length) return null;
-                    const u = {
-                        width: a.width,
-                        height: c.height,
-                        section: se(a, c)
-                    };
-                    switch (c.pinned) {
+                function ae(e, t, o, r) {
+                    if (!e) return null;
+                    const i = n(e.columnId),
+                        l = n(e.rowId);
+                    if (!t.has(i)) return null;
+                    if (!o.has(l)) return null;
+                    const s = t.get(i),
+                        a = o.get(l),
+                        c = {
+                            width: s.width,
+                            height: a.height,
+                            section: se(s, a)
+                        };
+                    switch (a.pinned) {
                         case "BEGIN":
-                            u.top = c.top;
+                            c.top = a.top;
                             break;
                         case "END":
-                            u.bottom = i.top.height + i.middle.height + i.bottom.height - c.top - c.height;
+                            c.bottom = r.top.height + r.middle.height + r.bottom.height - a.top - a.height;
                             break;
                         default:
-                            u.marginTop = c.top - i.top.height
+                            c.marginTop = a.top - r.top.height
                     }
-                    switch (a.pinned) {
+                    switch (s.pinned) {
                         case "BEGIN":
-                            u.left = a.left;
+                            c.left = s.left;
                             break;
                         case "END":
-                            u.right = i.left.width + i.center.width + i.right.width - a.left - a.width;
+                            c.right = r.left.width + r.center.width + r.right.width - s.left - s.width;
                             break;
                         default:
-                            u.marginLeft = a.left - i.left.width
+                            c.marginLeft = s.left - r.left.width
                     }
-                    return u
+                    return c
                 }
 
-                function ce(e, t) {
+                function ce(e, t, o, n, r) {
+                    return 0 === e.length ? null : ae(t, o, n, r)
+                }
+
+                function ue(e, t) {
                     return t.every((t => t.edit.validate({
                         string: e
                     })))
                 }
 
-                function ue(e) {
+                function de(e) {
                     return Array.isArray(e) ? e.map(((e, t) => t)) : Object.keys(e)
                 }
 
-                function de(e) {
-                    return ue(e)
+                function pe(e) {
+                    return de(e)
                 }
 
-                function pe(e) {
+                function fe(e) {
                     const t = new Set;
                     if (Array.isArray(e))
-                        for (const n of e)
-                            for (const e of ue(n)) t.add(e);
+                        for (const o of e)
+                            for (const e of de(o)) t.add(e);
                     else
-                        for (const n in e)
-                            for (const o of ue(e[n])) t.add(o);
+                        for (const o in e)
+                            for (const n of de(e[o])) t.add(n);
                     return [...t]
                 }
 
-                function fe(e, t) {
+                function he(e, t) {
                     if (!e.some((e => "DATA-BLOCK" === e.type))) return e;
-                    const n = [];
-                    for (const o of e)
-                        if ("DATA-BLOCK" === o.type) {
-                            const e = "selector" in o ? o.selector(t) : pe(t);
-                            for (const t of e) n.push({
-                                ...o,
+                    const o = [];
+                    for (const n of e)
+                        if ("DATA-BLOCK" === n.type) {
+                            const e = "selector" in n ? n.selector(t) : fe(t);
+                            for (const t of e) o.push({
+                                ...n,
                                 id: t,
                                 type: "DATA"
                             })
-                        } else n.push(o);
-                    return n
+                        } else o.push(n);
+                    return o
                 }
 
-                function he(e, t) {
+                function _e(e, t) {
                     if (!e.some((e => "DATA-BLOCK" === e.type))) return e;
-                    const n = [];
-                    for (const o of e)
-                        if ("DATA-BLOCK" === o.type) {
-                            const e = "selector" in o ? o.selector(t) : de(t);
-                            for (const t of e) n.push({
-                                ...o,
+                    const o = [];
+                    for (const n of e)
+                        if ("DATA-BLOCK" === n.type) {
+                            const e = "selector" in n ? n.selector(t) : pe(t);
+                            for (const t of e) o.push({
+                                ...n,
                                 id: t,
                                 type: "DATA"
                             })
-                        } else n.push(o);
-                    return n
+                        } else o.push(n);
+                    return o
                 }
-                const _e = ({
+                const me = ({
                     text: e,
                     expression: t
                 }) => e.includes(t);
-                class me {
+                class ge {
                     constructor(e) {
-                        this.rulesLookup = new P;
+                        this.rulesLookup = new L;
                         for (const t of e) {
                             const e = {
-                                by: o("by" in t ? t.by : "FILTER"),
-                                condition: t.condition || _e
+                                by: n("by" in t ? t.by : "FILTER"),
+                                condition: t.condition || me
                             };
                             this.rulesLookup.addRule(t.column, t.row, e)
                         }
                     }
-                    resolve(e, t, n, o, r, i, l, s) {
-                        const a = this.rulesLookup.getRules(r, o);
-                        if (0 === a.length) return "DATA" !== o.type || "DATA" !== r.type || !s.has('"FILTER"') || _e({
+                    resolve(e, t, o, n, r, i, l, s) {
+                        const a = this.rulesLookup.getRules(r, n);
+                        if (0 === a.length) return "DATA" !== n.type || "DATA" !== r.type || !s.has('"FILTER"') || me({
                             text: l,
                             expression: s.get('"FILTER"')
                         });
                         let c = {
                             data: e,
                             rows: t,
-                            columns: n,
-                            row: o,
+                            columns: o,
+                            row: n,
                             column: r,
                             value: i,
                             text: l
                         };
                         for (const e of a) {
                             if (!s.has(e.by)) continue;
                             const t = {
@@ -1574,501 +1584,533 @@
                             };
                             if (!e.condition(t)) return !1
                         }
                         return !0
                     }
                 }
 
-                function ge(e) {
-                    return new me(e)
+                function ye(e) {
+                    return new ge(e)
                 }
 
-                function ye(e) {
+                function we(e) {
                     return f(e, ["value", "text"])
                 }
 
-                function we(e) {
+                function be(e) {
                     return f(e, ["value", "text", "font", "padding"])
                 }
 
-                function Ee(e, t, n, o, r, i) {
+                function Ee(e, t, o, n, r, i) {
                     if (e.every((e => "number" == typeof e.width))) return e;
                     const l = e => {
                         const i = e.width;
                         if ("number" == typeof i) return i;
                         if (r.has(e.key)) {
                             const t = r.get(e.key);
                             if ("fit-once" === i && !t.dataOnly) return t.width;
                             if ("fit-data-once" === i && t.dataOnly) return t.width
                         }
                         let l = 0;
                         for (const r of t) {
                             if ("DATA" !== r.type && "fit-data-once" === i) continue;
                             if ("DATA" !== r.type && "fit-data" === i) continue;
-                            const t = o.resolve(r, e),
+                            const t = n.resolve(r, e),
                                 s = t.text,
                                 a = t.font,
                                 c = t.padding.left + t.padding.right,
-                                u = n.measureWidth(s, a) + c;
+                                u = o.measureWidth(s, a) + c;
                             l = Math.max(l, u)
                         }
                         return r.set(e.key, {
                             width: l,
                             dataOnly: "fit-data-once" === i
                         }), l
                     };
                     for (const e of r.keys()) i.has(e) || r.delete(e);
                     return e.map((e => ({
                         ...e,
                         width: l(e)
                     })))
                 }
 
-                function be(e, t, n, o, r, i) {
+                function ve(e, t, o, n, r, i) {
                     if (t.every((e => "number" == typeof e.height))) return t;
                     const l = t => {
                         const i = t.height;
                         if ("number" == typeof i) return i;
                         if (r.has(t.key)) {
                             const e = r.get(t.key);
                             if ("fit-once" === i && !e.dataOnly) return e.height;
                             if ("fit-data-once" === i && e.dataOnly) return e.height
                         }
                         let l = 0;
                         for (const r of e) {
                             if ("DATA" !== r.type && "fit-data-once" === i) continue;
                             if ("DATA" !== r.type && "fit-data" === i) continue;
-                            const e = o.resolve(t, r),
+                            const e = n.resolve(t, r),
                                 s = e.text,
                                 a = e.font,
                                 c = e.padding.top + e.padding.bottom,
-                                u = n.measureHeight(s, a) + c;
+                                u = o.measureHeight(s, a) + c;
                             l = Math.max(l, u)
                         }
                         return r.set(t.key, {
                             height: l,
                             dataOnly: "fit-data-once" === i
                         }), l
                     };
                     for (const e of r.keys()) i.has(e) || r.delete(e);
                     return t.map((e => ({
                         ...e,
                         height: l(e)
                     })))
                 }
 
-                function ve(e) {
+                function xe(e) {
                     return new Set(e.map((e => e.key)))
                 }
 
-                function xe(e) {
+                function Re(e) {
                     return f(e, ["value", "text"])
                 }
 
-                function Re(e, t) {
+                function Ae(e, t) {
                     return null != e.value && (null == t.value || e.value < t.value)
                 }
 
-                function Ae(e, t) {
+                function Ce(e, t) {
                     return null != e.value && (null == t.value || e.value > t.value)
                 }
-                class Ce {
+                class ke {
                     constructor(e) {
-                        this.rulesLookup = new P;
+                        this.rulesLookup = new L;
                         for (const t of e) {
-                            const e = t.comparator ? (e, n) => t.comparator(e, n) : (e, t) => Re(e, t),
-                                n = t.comparator ? (e, n) => !t.comparator(e, n) : (e, t) => Ae(e, t),
+                            const e = t.comparator ? (e, o) => t.comparator(e, o) : (e, t) => Ae(e, t),
+                                o = t.comparator ? (e, o) => !t.comparator(e, o) : (e, t) => Ce(e, t),
                                 r = {
-                                    by: o("by" in t ? t.by : "HEADER"),
+                                    by: n("by" in t ? t.by : "HEADER"),
                                     comparatorAsc: e,
-                                    comparatorDesc: n
+                                    comparatorDesc: o
                                 };
                             this.rulesLookup.addRule(t.column, t.row, r)
                         }
                     }
-                    resolve(e, t, n) {
-                        const o = this.rulesLookup.getRules(e, t);
-                        if (0 === o.length) return "DATA" !== t.type || "DATA" !== e.type ? null : n.has('"HEADER"') ? "ASC" === n.get('"HEADER"') ? Re : Ae : null;
-                        if (o.length > 1) throw new Error("Multiple sorting rules for the same cell");
-                        const r = o[0];
-                        return n.has(r.by) ? "ASC" === n.get(r.by) ? r.comparatorAsc : r.comparatorDesc : null
+                    resolve(e, t, o) {
+                        const n = this.rulesLookup.getRules(e, t);
+                        if (0 === n.length) return "DATA" !== t.type || "DATA" !== e.type ? null : o.has('"HEADER"') ? "ASC" === o.get('"HEADER"') ? Ae : Ce : null;
+                        if (n.length > 1) throw new Error("Multiple sorting rules for the same cell");
+                        const r = n[0];
+                        return o.has(r.by) ? "ASC" === o.get(r.by) ? r.comparatorAsc : r.comparatorDesc : null
                     }
                 }
 
-                function ke(e) {
-                    return new Ce(e)
+                function Ie(e) {
+                    return new ke(e)
                 }
 
-                function Ie(e, t, n) {
+                function De(e, t, o) {
                     const r = new Map;
                     for (const i of e) {
-                        const e = o(i[t]),
-                            l = o(i[n]);
+                        const e = n(i[t]),
+                            l = n(i[o]);
                         r.has(e) || r.set(e, new Map), r.get(e).set(l, i.direction)
                     }
                     return r
                 }
 
-                function De(e, t) {
+                function Te(e, t) {
                     e.sort(((e, t) => {
-                        const n = e.comparator(e.cell, t.cell);
-                        return "number" == typeof n ? n : n ? -1 : 1
+                        const o = e.comparator(e.cell, t.cell);
+                        return "number" == typeof o ? o : o ? -1 : 1
                     })), t.push(...e.map((e => e.entity))), e.length = 0
                 }
 
-                function Te(e, t, n, r, i, l, s) {
+                function Me(e, t, o, r, i, l, s) {
                     if (0 === e.length) return i;
-                    const a = Ie(e, "columnId", "rowId"),
+                    const a = De(e, "columnId", "rowId"),
                         c = new Map(l.map((e => [e.key, e]))),
-                        u = e.map((e => o(e.columnId))).filter((e => c.has(e))).map((e => c.get(e))).reverse();
+                        u = e.map((e => n(e.columnId))).filter((e => c.has(e))).map((e => c.get(e))).reverse();
                     if (0 === u.length) return i;
                     for (const e of u) {
-                        const o = [],
+                        const n = [],
                             c = [];
                         for (const u of i) {
                             const d = t.resolve(e, u, a.get(e.key));
                             if (!d) {
-                                De(c, o), o.push(u);
+                                Te(c, n), n.push(u);
                                 continue
                             }
                             const p = {
                                 entity: u,
                                 comparator: d,
-                                cell: n.resolve(r, i, l, u, e, s)
+                                cell: o.resolve(r, i, l, u, e, s)
                             };
-                            0 !== c.length && c[0].comparator !== d ? (De(c, o), c.push(p)) : c.push(p)
+                            0 !== c.length && c[0].comparator !== d ? (Te(c, n), c.push(p)) : c.push(p)
                         }
-                        De(c, o), i = o
+                        Te(c, n), i = n
                     }
                     return i
                 }
 
-                function Me(e, t, n, r, i, l, s) {
+                function Oe(e, t, o, r, i, l, s) {
                     if (0 === e.length) return l;
-                    const a = Ie(e, "rowId", "columnId"),
+                    const a = De(e, "rowId", "columnId"),
                         c = new Map(i.map((e => [e.key, e]))),
-                        u = e.map((e => o(e.rowId))).filter((e => c.has(e))).map((e => c.get(e))).reverse();
+                        u = e.map((e => n(e.rowId))).filter((e => c.has(e))).map((e => c.get(e))).reverse();
                     if (0 === u.length) return l;
                     for (const e of u) {
-                        const o = [],
+                        const n = [],
                             c = [];
                         for (const u of l) {
                             const d = t.resolve(u, e, a.get(e.key));
                             if (!d) {
-                                De(c, o), o.push(u);
+                                Te(c, n), n.push(u);
                                 continue
                             }
                             const p = {
                                 entity: u,
                                 comparator: d,
-                                cell: n.resolve(r, i, l, e, u, s)
+                                cell: o.resolve(r, i, l, e, u, s)
                             };
-                            0 !== c.length && c[0].comparator !== d ? (De(c, o), c.push(p)) : c.push(p)
+                            0 !== c.length && c[0].comparator !== d ? (Te(c, n), c.push(p)) : c.push(p)
                         }
-                        De(c, o), l = o
+                        Te(c, n), l = n
                     }
                     return l
                 }
-                const Oe = 5;
+                const Pe = 5;
 
-                function Le(e, t, n, r, i, l, s, a) {
+                function Le(e, t, o, r, i, l, s, a) {
                     if (!r) return null;
-                    const c = t.get(o(r.columnId));
-                    if ("HEADER" !== n.get(o(r.rowId)).type) return null;
+                    const c = t.get(n(r.columnId));
+                    if ("HEADER" !== o.get(n(r.rowId)).type) return null;
                     const u = re(i, l, s, a);
                     if (!u) return null;
                     const d = u.x;
-                    return d >= c.right - Oe && d <= c.right + Oe ? c.id : 0 === c.index || d < c.left - Oe || d > c.left + Oe ? null : e[c.index - 1].id
+                    return d >= c.right - Pe && d <= c.right + Pe ? c.id : 0 === c.index || d < c.left - Pe || d > c.left + Pe ? null : e[c.index - 1].id
                 }
 
-                function Pe(e, t, n, r, i, l, s, a) {
+                function Be(e, t, o, r, i, l, s, a) {
                     if (!r) return null;
-                    const c = t.get(o(r.columnId)),
-                        u = n.get(o(r.rowId));
+                    const c = t.get(n(r.columnId)),
+                        u = o.get(n(r.rowId));
                     if ("HEADER" !== c.type) return null;
                     const d = re(i, l, s, a);
                     if (!d) return null;
                     const p = d.y;
-                    return p >= u.bottom - Oe && p <= u.bottom + Oe ? u.id : 0 === u.index || p < u.top - Oe || p > u.top + Oe ? null : e[u.index - 1].id
+                    return p >= u.bottom - Pe && p <= u.bottom + Pe ? u.id : 0 === u.index || p < u.top - Pe || p > u.top + Pe ? null : e[u.index - 1].id
                 }
 
-                function Be(e) {
+                function Se(e) {
                     return e.map((e => ({
                         columnId: "columnId" in e ? e.columnId : "HEADER",
                         rowId: "rowId" in e ? e.rowId : "HEADER",
                         direction: e.direction
                     })))
                 }
 
-                function Se(e) {
+                function Ke(e) {
                     return e.map((e => ({
                         columnId: "columnId" in e ? e.columnId : "FILTER",
                         rowId: "rowId" in e ? e.rowId : "FILTER",
                         expression: e.expression
                     })))
                 }
 
-                function Ke(e, t) {
+                function We(e, t) {
                     return function(e, t) {
-                        const n = e.filter((e => "DATA" === e.type)).map((e => e.id));
-                        return t(n), n
+                        const o = e.filter((e => "DATA" === e.type)).map((e => e.id));
+                        return t(o), o
                     }(e, t)
                 }
 
-                function We(e) {
+                function Fe(e) {
+                    return f(e, ["value", "text", "tooltip"])
+                }
+
+                function ze(e, t, o, r) {
+                    if (!e) return null;
+                    const i = n(e.columnId),
+                        l = n(e.rowId);
+                    if (!o.has(i)) return null;
+                    if (!r.has(l)) return null;
+                    const s = r.get(l),
+                        a = o.get(i);
+                    return t.resolve(s, a).tooltip
+                }
+
+                function Ue(e, t, o, n, r) {
+                    if (!e) return null;
+                    const i = ae(t, o, n, r);
+                    return i ? {
+                        top: i.top,
+                        left: i.left
+                    } : null
+                }
+
+                function Ne(e) {
                     const t = {
                             ...e.localOptions,
                             ...e.externalOptions
                         },
-                        n = e.memory,
-                        o = e.state,
+                        o = e.memory,
+                        n = e.state,
                         r = e.element;
 
-                    function l(e, t, o) {
-                        const r = n[e] && n[e].dependencies;
-                        return r && !o.some(((e, t) => e !== r[t])) || (n[e] = {
-                            value: t(...o),
-                            dependencies: o
-                        }), n[e].value
+                    function l(e, t, n) {
+                        const r = o[e] && o[e].dependencies;
+                        return r && !n.some(((e, t) => e !== r[t])) || (o[e] = {
+                            value: t(...n),
+                            dependencies: n
+                        }), o[e].value
                     }
                     const s = window.devicePixelRatio,
                         a = t.borderWidth / s,
                         c = t.data,
                         d = e.input.value,
-                        p = l("sortBy", Be, [t.sortBy]),
-                        f = l("filters", Se, [t.filters]),
+                        p = l("sortBy", Se, [t.sortBy]),
+                        f = l("filters", Ke, [t.filters]),
                         _ = l("textResolver", Y, []),
                         w = l("dataFormatting", u, [t.formatting, t.dataSelector, p]),
-                        b = l("editedCellsAndFilters", y, [t.editedCells, f]),
-                        R = l("edition", E, [b]),
+                        E = l("editedCellsAndFilters", y, [t.editedCells, f]),
+                        R = l("edition", b, [E]),
                         A = l("invokedColumns", x, [t.columns, c]),
                         T = l("invokedRows", x, [t.rows, c]),
-                        M = l("unfoldedColumns", fe, [A, c]),
-                        O = l("unfoldedRows", he, [T, c]),
-                        L = l("unfilteredColumns", C, [M, t.pinnedLeft, t.pinnedRight, t.columnWidths]),
-                        P = l("unfilteredRows", k, [O, t.pinnedTop, t.pinnedBottom, t.rowHeights]),
-                        B = l("unfilteredColumnKeys", ve, [L]),
-                        S = l("unfilteredRowKeys", ve, [P]),
-                        K = l("filterFormatting", ye, [w]),
+                        M = l("unfoldedColumns", he, [A, c]),
+                        O = l("unfoldedRows", _e, [T, c]),
+                        P = l("unfilteredColumns", C, [M, t.pinnedLeft, t.pinnedRight, t.columnWidths]),
+                        L = l("unfilteredRows", k, [O, t.pinnedTop, t.pinnedBottom, t.rowHeights]),
+                        B = l("unfilteredColumnKeys", xe, [P]),
+                        S = l("unfilteredRowKeys", xe, [L]),
+                        K = l("filterFormatting", we, [w]),
                         W = l("filterFormattingRules", z, [K]),
-                        F = l("filteringRules", ge, [t.filtering]),
-                        U = l("filteredColumns", q, [f, F, W, c, P, L, R]),
-                        j = l("filteredRows", H, [f, F, W, c, P, L, R]),
-                        G = l("sortingFormatting", xe, [w]),
+                        F = l("filteringRules", ye, [t.filtering]),
+                        U = l("filteredColumns", q, [f, F, W, c, L, P, R]),
+                        H = l("filteredRows", j, [f, F, W, c, L, P, R]),
+                        G = l("sortingFormatting", Re, [w]),
                         se = l("sortingFormattingRules", z, [G]),
-                        ue = l("sortingRules", ke, [t.sorting]),
-                        de = l("sortedColumns", Me, [p, ue, se, c, j, U, R]),
-                        pe = l("sortedRows", Te, [p, ue, se, c, j, U, R]),
-                        _e = l("measureFormatting", we, [w]),
-                        me = l("measureFormattingRules", z, [_e]),
-                        Re = l("measureFormatResolver", N, [me, c, pe, de, R]),
+                        ae = l("sortingRules", Ie, [t.sorting]),
+                        de = l("sortedColumns", Oe, [p, ae, se, c, H, U, R]),
+                        pe = l("sortedRows", Me, [p, ae, se, c, H, U, R]),
+                        fe = l("measureFormatting", be, [w]),
+                        me = l("measureFormattingRules", z, [fe]),
+                        ge = l("measureFormatResolver", N, [me, c, pe, de, R]),
                         Ae = e.columnWidthCache,
                         Ce = e.rowHeightCache,
-                        Ie = l("measuredColumns", Ee, [de, pe, _, Re, Ae, B]),
-                        De = l("measuredRows", be, [de, pe, _, Re, Ce, S]),
-                        Oe = l("columns", I, [Ie, s, a]),
-                        We = l("rows", D, [De, s, a]),
-                        Fe = l("columnLookup", ie, [Oe]),
-                        ze = l("rowLookup", ie, [We]),
-                        Ue = t.focusedCell,
-                        Ne = l("sections", g, [Oe, We]),
-                        je = t.selectedCells,
-                        He = l("fixedSize", $, [Ne.top.height, Ne.bottom.height, Ne.left.width, Ne.right.width]),
-                        qe = l("totalSize", V, [Oe, We]),
-                        $e = function(e, t, n, o, r, i) {
+                        ke = l("measuredColumns", Ee, [de, pe, _, ge, Ae, B]),
+                        De = l("measuredRows", ve, [de, pe, _, ge, Ce, S]),
+                        Te = l("columns", I, [ke, s, a]),
+                        Pe = l("rows", D, [De, s, a]),
+                        Ne = l("columnLookup", ie, [Te]),
+                        He = l("rowLookup", ie, [Pe]),
+                        je = t.focusedCell,
+                        qe = l("sections", g, [Te, Pe]),
+                        $e = t.selectedCells,
+                        Ve = l("fixedSize", $, [qe.top.height, qe.bottom.height, qe.left.width, qe.right.width]),
+                        Ge = l("totalSize", V, [Te, Pe]),
+                        Ye = function(e, t, o, n, r, i) {
                             if (!t) return null;
                             if (t.x < 0 || t.y < 0 || t.x > i.width || t.y > i.height) return null;
                             const l = re(e, t, r, i),
                                 s = function(e, t) {
                                     if (0 === e.length) return -1;
                                     if (t < e[0].topWithBorder) return -1;
                                     if (t > e[e.length - 1].bottomWithBorder) return -1;
-                                    let n = 0,
-                                        o = e.length - 1;
-                                    for (; n <= o;) {
-                                        const r = Math.floor((n + o) / 2);
-                                        if (t < e[r].topWithBorder) o = r - 1;
+                                    let o = 0,
+                                        n = e.length - 1;
+                                    for (; o <= n;) {
+                                        const r = Math.floor((o + n) / 2);
+                                        if (t < e[r].topWithBorder) n = r - 1;
                                         else {
                                             if (!(t > e[r].bottomWithBorder)) return r;
-                                            n = r + 1
+                                            o = r + 1
                                         }
                                     }
                                     return -1
-                                }(n, l.y),
+                                }(o, l.y),
                                 a = function(e, t) {
                                     if (0 === e.length) return -1;
                                     if (t < e[0].leftWithBorder) return -1;
                                     if (t > e[e.length - 1].rightWithBorder) return -1;
-                                    let n = 0,
-                                        o = e.length - 1;
-                                    for (; n <= o;) {
-                                        const r = Math.floor((n + o) / 2);
-                                        if (t < e[r].leftWithBorder) o = r - 1;
+                                    let o = 0,
+                                        n = e.length - 1;
+                                    for (; o <= n;) {
+                                        const r = Math.floor((o + n) / 2);
+                                        if (t < e[r].leftWithBorder) n = r - 1;
                                         else {
                                             if (!(t > e[r].rightWithBorder)) return r;
-                                            n = r + 1
+                                            o = r + 1
                                         }
                                     }
                                     return -1
-                                }(o, l.x);
+                                }(n, l.x);
                             return -1 === s || -1 === a ? null : {
-                                rowId: n[s].id,
-                                columnId: o[a].id
+                                rowId: o[s].id,
+                                columnId: n[a].id
                             }
-                        }(r, e.mousePosition, We, Oe, He, qe),
-                        Ve = e.resizingColumn || l("resizableColumn", Le, [Oe, Fe, ze, $e, r, e.mousePosition, He, qe]),
-                        Ge = e.resizingRow || l("resizableRow", Pe, [We, Fe, ze, $e, r, e.mousePosition, He, qe]),
-                        Ye = l("highlightedCells", le, [e.isMouseDown, !!Ve || !!Ge, Ue, $e, Oe, We, Fe, ze]),
-                        Xe = l("selection", v, [je]),
-                        Ze = l("highlight", v, [Ye]),
-                        Je = l("renderFormatting", m, [w, $e, Ue, Xe, Ze, R, p, Ve, Ge, t.borderWidth]),
-                        Qe = l("renderFormattingRules", z, [Je]),
-                        et = l("renderFormatResolver", N, [Qe, c, We, Oe, R]),
-                        tt = l("inputFormatting", h, [w]),
-                        nt = l("inputFormattingRules", z, [tt]),
-                        ot = l("inputFormatResolver", N, [nt, c, We, Oe, R]),
-                        rt = l("editableCells", i, [je, ot, Fe, ze]),
-                        it = l("inputPlacement", ae, [rt, Ue, Fe, ze, Ne]),
-                        lt = l("isTextValid", ce, [d, rt]),
-                        st = function(e, t, n, o) {
+                        }(r, e.mousePosition, Pe, Te, Ve, Ge),
+                        Xe = e.resizingColumn || l("resizableColumn", Le, [Te, Ne, He, Ye, r, e.mousePosition, Ve, Ge]),
+                        Ze = e.resizingRow || l("resizableRow", Be, [Pe, Ne, He, Ye, r, e.mousePosition, Ve, Ge]),
+                        Je = l("highlightedCells", le, [e.isMouseDown, !!Xe || !!Ze, je, Ye, Te, Pe, Ne, He]),
+                        Qe = l("selection", v, [$e]),
+                        et = l("highlight", v, [Je]),
+                        tt = l("renderFormatting", m, [w, Ye, je, Qe, et, R, p, Xe, Ze, t.borderWidth]),
+                        ot = l("renderFormattingRules", z, [tt]),
+                        nt = l("renderFormatResolver", N, [ot, c, Pe, Te, R]),
+                        rt = l("inputFormatting", h, [w]),
+                        it = l("inputFormattingRules", z, [rt]),
+                        lt = l("inputFormatResolver", N, [it, c, Pe, Te, R]),
+                        st = l("editableCells", i, [$e, lt, Ne, He]),
+                        at = l("inputPlacement", ce, [st, je, Ne, He, qe]),
+                        ct = l("isTextValid", ue, [d, st]),
+                        ut = l("contextFormatting", Fe, [w]),
+                        dt = l("contextFormattingRules", z, [ut]),
+                        pt = l("contextFormatResolver", N, [dt, c, Pe, Te, R]),
+                        ft = l("tooltip", ze, [Ye, pt, Ne, He]),
+                        ht = l("tooltipPlacement", Ue, [ft, Ye, Ne, He, qe]),
+                        _t = function(e, t, o, n) {
                             const r = {
-                                    width: o.getBoundingClientRect().width,
-                                    height: o.getBoundingClientRect().height
+                                    width: n.getBoundingClientRect().width,
+                                    height: n.getBoundingClientRect().height
                                 },
                                 i = {
-                                    left: o.scrollLeft,
-                                    top: o.scrollTop
+                                    left: n.scrollLeft,
+                                    top: n.scrollTop
                                 },
-                                l = e || oe,
+                                l = e || ne,
                                 s = ee({
                                     left: 0,
                                     top: 0,
                                     ...t
-                                }, n),
+                                }, o),
                                 a = ee({
                                     ...i,
                                     ...r
-                                }, n),
+                                }, o),
                                 c = Z(s, J(a, te)),
-                                u = Z(s, J(a, ne));
+                                u = Z(s, J(a, oe));
                             return X(s, l) && X(l, c) ? Q(l) > 2 * Q(u) ? u : l : u
-                        }(o?.scrollRect, qe, He, r);
-                    l("activeColumns", Ke, [Oe, t.onActiveColumnsChange]), l("activeRows", Ke, [We, t.onActiveRowsChange]), e.state = {
+                        }(n?.scrollRect, Ge, Ve, r);
+                    l("activeColumns", We, [Te, t.onActiveColumnsChange]), l("activeRows", We, [Pe, t.onActiveRowsChange]), e.state = {
                         options: t,
                         devicePixelRatio: s,
                         borderWidth: a,
                         data: c,
-                        dataFormatting: w,
                         edition: R,
                         filteredColumns: U,
-                        filteredRows: j,
-                        columns: Oe,
-                        rows: We,
-                        sections: Ne,
-                        selectedCells: je,
-                        selection: Xe,
-                        highlight: Ze,
-                        hoveredCell: $e,
-                        focusedCell: Ue,
-                        renderFormatting: Je,
-                        renderFormatResolver: et,
-                        inputFormatting: tt,
-                        inputFormatResolver: ot,
-                        fixedSize: He,
-                        totalSize: qe,
+                        filteredRows: H,
+                        columns: Te,
+                        rows: Pe,
+                        sections: qe,
+                        selectedCells: $e,
+                        selection: Qe,
+                        highlight: et,
+                        hoveredCell: Ye,
+                        focusedCell: je,
+                        renderFormatting: tt,
+                        renderFormatResolver: nt,
+                        inputFormatting: rt,
+                        inputFormatResolver: lt,
+                        fixedSize: Ve,
+                        totalSize: Ge,
                         textResolver: _,
-                        scrollRect: st,
-                        highlightedCells: Ye,
-                        inputPlacement: it,
-                        columnLookup: Fe,
-                        rowLookup: ze,
+                        scrollRect: _t,
+                        highlightedCells: Je,
+                        inputPlacement: at,
+                        columnLookup: Ne,
+                        rowLookup: He,
                         text: d,
-                        isTextValid: lt,
-                        resizableColumn: Ve,
-                        resizableRow: Ge
+                        isTextValid: ct,
+                        resizableColumn: Xe,
+                        resizableRow: Ze,
+                        tooltip: ft,
+                        tooltipPlacement: ht
                     }
                 }
 
-                function Fe(e) {
+                function He(e) {
                     if (!e.error) try {
-                        We(e)
+                        Ne(e)
                     } catch (t) {
                         e.error = t
                     }
                 }
 
-                function ze(e, t) {
-                    const n = new b(t);
-                    return [...t, ...e.filter((e => !n.isIdSelected(e.rowId, e.columnId)))]
+                function je(e, t) {
+                    const o = new E(t);
+                    return [...t, ...e.filter((e => !o.isIdSelected(e.rowId, e.columnId)))]
                 }
 
-                function Ue(e, t) {
-                    const n = new b(t);
-                    return e.filter((e => !n.isIdSelected(e.rowId, e.columnId)))
+                function qe(e, t) {
+                    const o = new E(t);
+                    return e.filter((e => !o.isIdSelected(e.rowId, e.columnId)))
                 }
 
-                function Ne(e) {
+                function $e(e) {
                     const t = e.currentTarget.getBoundingClientRect();
                     return {
                         x: e.clientX - t.left,
                         y: e.clientY - t.top
                     }
                 }
 
-                function je(e, t) {
+                function Ve(e, t) {
                     return e.map((e => ({
                         ...e,
                         columnId: "id" in e ? e.id : t,
                         rowId: "id" in e ? e.id : t
                     })))
                 }
 
-                function He(e) {
+                function Ge(e) {
                     if ("spread-grid-context" in e) return;
                     const t = {
                             "top-left": document.createElement("canvas"),
                             "top-center": document.createElement("canvas"),
                             "top-right": document.createElement("canvas"),
                             "middle-left": document.createElement("canvas"),
                             "middle-center": document.createElement("canvas"),
                             "middle-right": document.createElement("canvas"),
                             "bottom-left": document.createElement("canvas"),
                             "bottom-center": document.createElement("canvas"),
                             "bottom-right": document.createElement("canvas")
                         },
-                        n = document.createElement("input");
-                    e.setAttribute("tabindex", "0"), e.setAttribute("style", "max-width: 100vw; max-height: 100vh; overflow: auto; display: grid; position: relative; grid-template-columns: fit-content(0) fit-content(0) fit-content(0); grid-template-rows: fit-content(0) fit-content(0) fit-content(0); outline: none; user-select: none;"), e.classList.add("spread-grid"), t["top-left"].setAttribute("style", "position: sticky; left: 0; top: 0; z-index: 2; grid-row: 1; grid-column: 1;"), t["top-center"].setAttribute("style", "position: sticky; top: 0; z-index: 1; grid-row: 1; grid-column: 2;"), t["top-right"].setAttribute("style", "position: sticky; right: 0; top: 0; z-index: 2; grid-row: 1; grid-column: 3;"), t["middle-left"].setAttribute("style", "position: sticky; left: 0; z-index: 1; grid-row: 2; grid-column: 1;"), t["middle-center"].setAttribute("style", "grid-row: 2; grid-column: 2; z-index: 0;"), t["middle-right"].setAttribute("style", "position: sticky; right: 0; z-index: 1; grid-row: 2; grid-column: 3;"), t["bottom-left"].setAttribute("style", "position: sticky; left: 0; bottom: 0; z-index: 2; grid-row: 3; grid-column: 1;"), t["bottom-center"].setAttribute("style", "position: sticky; bottom: 0; z-index: 1; grid-row: 3; grid-column: 2;"), t["bottom-right"].setAttribute("style", "position: sticky; right: 0; bottom: 0; z-index: 2; grid-row: 3; grid-column: 3;"), n.setAttribute("style", "position: sticky; z-index: 3; outline: none; border: none; box-shadow: none; padding: 0 5px; font-size: 12px; font-family: Calibri; background-color: white; box-sizing: border-box; opacity: 0; pointer-events: none;");
-                    const l = {
+                        o = document.createElement("input"),
+                        l = document.createElement("div");
+                    e.setAttribute("tabindex", "0"), e.setAttribute("style", "max-width: 100vw; max-height: 100vh; overflow: auto; display: grid; position: relative; grid-template-columns: fit-content(0) fit-content(0) fit-content(0); grid-template-rows: fit-content(0) fit-content(0) fit-content(0); outline: none; user-select: none;"), e.classList.add("spread-grid"), t["top-left"].setAttribute("style", "position: sticky; left: 0; top: 0; z-index: 2; grid-row: 1; grid-column: 1;"), t["top-center"].setAttribute("style", "position: sticky; top: 0; z-index: 1; grid-row: 1; grid-column: 2;"), t["top-right"].setAttribute("style", "position: sticky; right: 0; top: 0; z-index: 2; grid-row: 1; grid-column: 3;"), t["middle-left"].setAttribute("style", "position: sticky; left: 0; z-index: 1; grid-row: 2; grid-column: 1;"), t["middle-center"].setAttribute("style", "grid-row: 2; grid-column: 2; z-index: 0;"), t["middle-right"].setAttribute("style", "position: sticky; right: 0; z-index: 1; grid-row: 2; grid-column: 3;"), t["bottom-left"].setAttribute("style", "position: sticky; left: 0; bottom: 0; z-index: 2; grid-row: 3; grid-column: 1;"), t["bottom-center"].setAttribute("style", "position: sticky; bottom: 0; z-index: 1; grid-row: 3; grid-column: 2;"), t["bottom-right"].setAttribute("style", "position: sticky; right: 0; bottom: 0; z-index: 2; grid-row: 3; grid-column: 3;"), o.setAttribute("style", "position: sticky; z-index: 3; outline: none; border: none; box-shadow: none; padding: 0 5px; font-size: 12px; font-family: Calibri; background-color: white; box-sizing: border-box; opacity: 0; pointer-events: none;"), l.setAttribute("style", "pointer-events: none; background-color: white; color: black; border: 1px solid black; padding: 5px;"), l.setAttribute("popover", "");
+                    const s = {
                         externalOptions: {},
                         state: null,
                         memory: {},
                         element: e,
                         canvases: t,
-                        input: n,
+                        input: o,
+                        tooltip: l,
                         renderRequested: !1,
                         mousePosition: null,
                         isMouseDown: !1,
                         columnWidthCache: new Map,
                         rowHeightCache: new Map,
                         requestNewRender: () => {
-                            l.renderRequested || (l.renderRequested = !0, requestAnimationFrame((() => {
-                                l.renderRequested = !1, Fe(l), a(l)
+                            s.renderRequested || (s.renderRequested = !0, requestAnimationFrame((() => {
+                                s.renderRequested = !1, He(s), a(s)
                             })))
                         },
-                        addEventListener: (e, t, n) => {
+                        addEventListener: (e, t, o) => {
                             e.addEventListener(t, (e => {
                                 try {
-                                    n(e)
+                                    o(e)
                                 } catch (e) {
-                                    e.message = `[${t} event]: ${e.message}`, l.error = e, l.requestNewRender()
+                                    e.message = `[${t} event]: ${e.message}`, s.error = e, s.requestNewRender()
                                 }
                             }))
                         }
                     };
-                    l.localOptions = {
+                    s.localOptions = {
                         data: [],
                         columns: [{
                             type: "DATA-BLOCK"
                         }],
                         rows: [{
                             type: "HEADER"
                         }, {
@@ -2076,319 +2118,331 @@
                         }],
                         formatting: [],
                         filtering: [],
                         sorting: [],
                         dataSelector: ({
                             data: e,
                             row: t,
-                            column: n
-                        }) => e?.[t.id]?.[n.id],
+                            column: o
+                        }) => e?.[t.id]?.[o.id],
                         pinnedTop: 0,
                         pinnedBottom: 0,
                         pinnedLeft: 0,
                         pinnedRight: 0,
                         borderWidth: 1,
                         focusedCell: null,
                         onFocusedCellChange: e => {
-                            l.localOptions.focusedCell = e, l.requestNewRender()
+                            s.localOptions.focusedCell = e, s.requestNewRender()
                         },
                         selectedCells: [],
                         onSelectedCellsChange: e => {
-                            l.localOptions.selectedCells = e, l.requestNewRender()
+                            s.localOptions.selectedCells = e, s.requestNewRender()
                         },
                         highlightedCells: [],
                         editedCells: [],
                         onEditedCellsChange: e => {
-                            l.localOptions.editedCells = e, l.requestNewRender()
+                            s.localOptions.editedCells = e, s.requestNewRender()
                         },
                         filters: [],
                         onFiltersChange: e => {
-                            l.localOptions.filters = e, l.requestNewRender()
+                            s.localOptions.filters = e, s.requestNewRender()
                         },
                         sortBy: [],
                         onSortByChange: e => {
-                            l.localOptions.sortBy = e, l.requestNewRender()
+                            s.localOptions.sortBy = e, s.requestNewRender()
                         },
                         onCellClick: () => {},
                         onCustomCellClick: () => {},
                         columnWidths: [],
                         onColumnWidthsChange: e => {
-                            l.localOptions.columnWidths = e, l.requestNewRender()
+                            s.localOptions.columnWidths = e, s.requestNewRender()
                         },
                         rowHeights: [],
                         onRowHeightsChange: e => {
-                            l.localOptions.rowHeights = e, l.requestNewRender()
+                            s.localOptions.rowHeights = e, s.requestNewRender()
                         },
                         onActiveColumnsChange: () => {},
                         onActiveRowsChange: () => {}
-                    }, e["spread-grid-context"] = l;
-                    const s = e => {
-                            n.value = e, n.dispatchEvent(new Event("input"))
-                        },
-                        c = e => {
-                            const t = l.state.options.selectedCells,
-                                n = l.state.inputFormatResolver,
-                                o = l.state.columnLookup,
-                                r = l.state.rowLookup,
-                                a = l.state.text,
-                                c = l.state.isTextValid,
-                                u = l.state.options.onEditedCellsChange,
-                                d = l.state.options.onFiltersChange,
-                                p = i(t, n, o, r);
-                            if ("" === a) return;
-                            if (!c) return;
+                    }, e["spread-grid-context"] = s;
+                    const c = e => {
+                            o.value = e, o.dispatchEvent(new Event("input"))
+                        },
+                        u = e => {
+                            const t = s.state.options.selectedCells,
+                                o = s.state.inputFormatResolver,
+                                n = s.state.columnLookup,
+                                r = s.state.rowLookup,
+                                l = s.state.text,
+                                a = s.state.isTextValid,
+                                u = s.state.options.onEditedCellsChange,
+                                d = s.state.options.onFiltersChange,
+                                p = i(t, o, n, r);
+                            if ("" === l) return;
+                            if (!a) return;
                             if (e && !p.every((e => e.edit.autoCommit))) return;
                             const f = p.filter((e => "DATA" === e.type)),
                                 h = p.filter((e => "FILTER" === e.type));
                             var _;
                             _ = f.map((e => ({
                                 ...e.cell,
                                 value: e.edit.parse({
-                                    string: a
+                                    string: l
                                 })
-                            }))), u(ze(l.state.options.editedCells, _)), (e => {
-                                d(ze(je(l.state.options.filters, "FILTER"), e))
+                            }))), u(je(s.state.options.editedCells, _)), (e => {
+                                d(je(Ve(s.state.options.filters, "FILTER"), e))
                             })(h.map((e => ({
                                 ...e.cell,
                                 expression: e.edit.parse({
-                                    string: a
+                                    string: l
                                 })
-                            })))), e || s("")
+                            })))), e || c("")
                         },
-                        u = e => {
-                            const t = l.state.options.selectedCells,
-                                n = l.state.options.onEditedCellsChange,
-                                o = l.state.options.onFiltersChange,
-                                r = i(t, l.state.inputFormatResolver, l.state.columnLookup, l.state.rowLookup);
-                            var s;
-                            e && !r.every((e => e.edit.autoCommit)) || (s = t, n(Ue(l.state.options.editedCells, s)), (e => {
-                                o(Ue(je(l.state.options.filters, "FILTER"), e))
+                        d = e => {
+                            const t = s.state.options.selectedCells,
+                                o = s.state.options.onEditedCellsChange,
+                                n = s.state.options.onFiltersChange,
+                                r = i(t, s.state.inputFormatResolver, s.state.columnLookup, s.state.rowLookup);
+                            var l;
+                            e && !r.every((e => e.edit.autoCommit)) || (l = t, o(qe(s.state.options.editedCells, l)), (e => {
+                                n(qe(Ve(s.state.options.filters, "FILTER"), e))
                             })(t))
                         };
-                    l.addEventListener(e, "scroll", (e => {
-                        l.requestNewRender()
-                    })), l.addEventListener(e, "mouseenter", (e => {
-                        l.mousePosition = Ne(e), l.requestNewRender()
-                    })), l.addEventListener(e, "mousemove", (t => {
-                        if (l.mousePosition = Ne(t), l.resizingColumn) {
-                            const t = l.state.columnLookup.get(o(l.resizingColumn)),
-                                n = t.width,
+                    s.addEventListener(e, "scroll", (e => {
+                        s.requestNewRender()
+                    })), s.addEventListener(e, "mouseenter", (e => {
+                        s.mousePosition = $e(e), s.requestNewRender()
+                    })), s.addEventListener(e, "mousemove", (t => {
+                        if (s.mousePosition = $e(t), s.resizingColumn) {
+                            const t = s.state.columnLookup.get(n(s.resizingColumn)),
+                                o = t.width,
                                 r = t.right,
-                                i = re(e, l.mousePosition, l.state.fixedSize, l.state.totalSize),
-                                s = Math.max(10, i.x - r + n),
-                                a = l.state.options.columnWidths.filter((e => o(e.columnId) !== t.key)).concat([{
+                                i = re(e, s.mousePosition, s.state.fixedSize, s.state.totalSize),
+                                l = Math.max(10, i.x - r + o),
+                                a = s.state.options.columnWidths.filter((e => n(e.columnId) !== t.key)).concat([{
                                     columnId: t.id,
-                                    width: s
+                                    width: l
                                 }]);
-                            l.state.options.onColumnWidthsChange(a)
+                            s.state.options.onColumnWidthsChange(a)
                         }
-                        if (l.resizingRow) {
-                            const t = l.state.rowLookup.get(o(l.resizingRow)),
-                                n = t.height,
+                        if (s.resizingRow) {
+                            const t = s.state.rowLookup.get(n(s.resizingRow)),
+                                o = t.height,
                                 r = t.bottom,
-                                i = re(e, l.mousePosition, l.state.fixedSize, l.state.totalSize),
-                                s = Math.max(10, i.y - r + n),
-                                a = l.state.options.rowHeights.filter((e => o(e.rowId) !== t.key)).concat([{
+                                i = re(e, s.mousePosition, s.state.fixedSize, s.state.totalSize),
+                                l = Math.max(10, i.y - r + o),
+                                a = s.state.options.rowHeights.filter((e => n(e.rowId) !== t.key)).concat([{
                                     rowId: t.id,
-                                    height: s
+                                    height: l
                                 }]);
-                            l.state.options.onRowHeightsChange(a)
+                            s.state.options.onRowHeightsChange(a)
                         }
-                        l.requestNewRender()
-                    })), l.addEventListener(e, "mouseleave", (() => {
-                        l.mousePosition = null, l.requestNewRender()
-                    })), l.addEventListener(e, "mousedown", (e => {
-                        Fe(l), s(""), l.isMouseDown = !0, l.mouseDownPosition = l.mousePosition, l.mouseDownCell = l.state.hoveredCell, l.state.resizableColumn && (l.resizingColumn = l.state.resizableColumn), l.state.resizableRow && (l.resizingRow = l.state.resizableRow), l.state.resizableColumn || l.state.resizableRow || l.state.options.onFocusedCellChange(l.state.hoveredCell), e.ctrlKey || l.state.options.onSelectedCellsChange([]), l.requestNewRender()
-                    })), l.addEventListener(e, "mouseup", (e => {
-                        Fe(l), l.isMouseDown = !1, l.resizingColumn = null, l.resizingRow = null, l.state.options.onSelectedCellsChange(ze(l.state.options.selectedCells, l.state.highlightedCells)), l.requestNewRender()
-                    })), l.addEventListener(e, "pointerdown", (e => {
-                        l.element.setPointerCapture(e.pointerId)
-                    })), l.addEventListener(e, "pointerup", (e => {
-                        l.element.releasePointerCapture(e.pointerId)
-                    })), l.addEventListener(e, "click", (e => {
-                        Fe(l);
-                        const t = l.state.hoveredCell,
-                            n = l.mouseDownCell;
-                        if (l.state.resizableColumn || l.state.resizableRow) return;
+                        s.requestNewRender()
+                    })), s.addEventListener(e, "mouseleave", (() => {
+                        s.mousePosition = null, s.requestNewRender()
+                    })), s.addEventListener(e, "mousedown", (e => {
+                        He(s), c(""), s.isMouseDown = !0, s.mouseDownPosition = s.mousePosition, s.mouseDownCell = s.state.hoveredCell, s.state.resizableColumn && (s.resizingColumn = s.state.resizableColumn), s.state.resizableRow && (s.resizingRow = s.state.resizableRow), s.state.resizableColumn || s.state.resizableRow || s.state.options.onFocusedCellChange(s.state.hoveredCell), e.ctrlKey || s.state.options.onSelectedCellsChange([]), s.requestNewRender()
+                    })), s.addEventListener(e, "mouseup", (e => {
+                        He(s), s.isMouseDown = !1, s.resizingColumn = null, s.resizingRow = null, s.state.options.onSelectedCellsChange(je(s.state.options.selectedCells, s.state.highlightedCells)), s.requestNewRender()
+                    })), s.addEventListener(e, "pointerdown", (e => {
+                        s.element.setPointerCapture(e.pointerId)
+                    })), s.addEventListener(e, "pointerup", (e => {
+                        s.element.releasePointerCapture(e.pointerId)
+                    })), s.addEventListener(e, "click", (e => {
+                        He(s);
+                        const t = s.state.hoveredCell,
+                            o = s.mouseDownCell;
+                        if (s.state.resizableColumn || s.state.resizableRow) return;
                         if (null === t) return;
-                        if (o(t.columnId) !== o(n.columnId)) return;
-                        if (o(t.rowId) !== o(n.rowId)) return;
-                        const i = l.state.columnLookup.get(o(t.columnId)),
-                            s = l.state.rowLookup.get(o(t.rowId)),
-                            a = l.state.options.sortBy,
-                            c = l.state.inputFormatResolver.resolve(s, i);
+                        if (n(t.columnId) !== n(o.columnId)) return;
+                        if (n(t.rowId) !== n(o.rowId)) return;
+                        const i = s.state.columnLookup.get(n(t.columnId)),
+                            l = s.state.rowLookup.get(n(t.rowId)),
+                            a = s.state.options.sortBy,
+                            c = s.state.inputFormatResolver.resolve(l, i),
+                            u = {
+                                ctrlKey: e.ctrlKey,
+                                shiftKey: e.shiftKey,
+                                button: e.button,
+                                buttons: e.buttons
+                            };
                         if (c.edit?.toggle) {
-                            const e = function(e, t, n, o) {
-                                    const r = o.hasValueByKey(n.key, t.key) ? o.getValueByKey(n.key, t.key) : e.value,
+                            const e = function(e, t, o, n) {
+                                    const r = n.hasValueByKey(o.key, t.key) ? n.getValueByKey(o.key, t.key) : e.value,
                                         i = e.edit.toggle;
                                     return "function" == typeof i ? i({
                                         value: r
                                     }) : i[(i.indexOf(r) + 1) % i.length]
-                                }(c, i, s, l.state.edition),
-                                n = r(i, s);
-                            "DATA" === n && l.state.options.onEditedCellsChange(ze(l.state.options.editedCells, [{
+                                }(c, i, l, s.state.edition),
+                                o = r(i, l);
+                            "DATA" === o && s.state.options.onEditedCellsChange(je(s.state.options.editedCells, [{
                                 ...t,
                                 value: e
-                            }])), "FILTER" === n && l.state.options.onFiltersChange(ze(l.state.options.filters, [{
+                            }])), "FILTER" === o && s.state.options.onFiltersChange(je(s.state.options.filters, [{
                                 ...t,
                                 expression: e
                             }]))
-                        } else if ("DATA" === i.type && "DATA" === s.type) l.state.options.onCellClick(l.state.hoveredCell);
-                        else if ("CUSTOM" === i.type || "CUSTOM" === s.type) l.state.options.onCustomCellClick(l.state.hoveredCell);
-                        else if ("HEADER" === i.type || "HEADER" === s.type) {
-                            const t = function(e, t, n, r) {
+                        } else if ("DATA" === i.type && "DATA" === l.type) s.state.options.onCellClick({
+                            ...s.state.hoveredCell,
+                            ...u
+                        });
+                        else if ("CUSTOM" === i.type || "CUSTOM" === l.type) s.state.options.onCustomCellClick({
+                            ...s.state.hoveredCell,
+                            ...u
+                        });
+                        else if ("HEADER" === i.type || "HEADER" === l.type) {
+                            const t = function(e, t, o, r) {
                                 function i(e) {
                                     const r = "columnId" in e ? e.columnId : "HEADER",
                                         i = "rowId" in e ? e.rowId : "HEADER";
-                                    return t.key === o(r) && n.key === o(i)
+                                    return t.key === n(r) && o.key === n(i)
                                 }
                                 const l = ["ASC", "DESC", void 0],
                                     s = e.find(i),
                                     a = l.indexOf(s?.direction),
                                     c = l[(a + 1) % l.length],
                                     u = e.indexOf(s) === e.length - 1;
                                 return [...!r || !u && s ? e.filter((e => ! function(e) {
                                     const r = "columnId" in e ? e.columnId : "HEADER",
                                         i = "rowId" in e ? e.rowId : "HEADER";
-                                    return "HEADER" === t.type && t.key === o(r) || "HEADER" === n.type && n.key === o(i)
+                                    return "HEADER" === t.type && t.key === n(r) || "HEADER" === o.type && o.key === n(i)
                                 }(e))) : e.filter((e => !i(e))), ...c ? [{
                                     columnId: t.id,
-                                    rowId: n.id,
+                                    rowId: o.id,
                                     direction: c
                                 }] : []]
-                            }(a, i, s, e.ctrlKey);
-                            l.state.options.onSortByChange(t), l.state.options.onSelectedCellsChange([])
+                            }(a, i, l, e.ctrlKey);
+                            s.state.options.onSortByChange(t), s.state.options.onSelectedCellsChange([])
                         }
-                    })), l.addEventListener(e, "dblclick", (e => {
-                        if (Fe(l), l.state.resizableColumn) {
-                            const e = o(l.state.resizableColumn),
-                                t = l.state.options.columnWidths.filter((t => o(t.columnId) !== e));
-                            l.state.options.onColumnWidthsChange(t), l.columnWidthCache.delete(e)
-                        }
-                        if (l.state.resizableRow) {
-                            const e = o(l.state.resizableRow),
-                                t = l.state.options.rowHeights.filter((t => o(t.rowId) !== e));
-                            l.state.options.onRowHeightsChange(t), l.rowHeightCache.delete(e)
+                    })), s.addEventListener(e, "dblclick", (e => {
+                        if (He(s), s.state.resizableColumn) {
+                            const e = n(s.state.resizableColumn),
+                                t = s.state.options.columnWidths.filter((t => n(t.columnId) !== e));
+                            s.state.options.onColumnWidthsChange(t), s.columnWidthCache.delete(e)
+                        }
+                        if (s.state.resizableRow) {
+                            const e = n(s.state.resizableRow),
+                                t = s.state.options.rowHeights.filter((t => n(t.rowId) !== e));
+                            s.state.options.onRowHeightsChange(t), s.rowHeightCache.delete(e)
                         }
-                        const t = l.state.focusedCell;
+                        const t = s.state.focusedCell;
                         if (null === t) return;
-                        const r = o(t.columnId),
-                            i = o(t.rowId),
-                            a = l.state.columnLookup,
-                            c = l.state.rowLookup,
-                            u = l.state.inputFormatResolver;
-                        if (!a.has(r)) return;
-                        if (!c.has(i)) return;
-                        const d = a.get(r),
-                            p = c.get(i),
+                        const r = n(t.columnId),
+                            i = n(t.rowId),
+                            l = s.state.columnLookup,
+                            a = s.state.rowLookup,
+                            u = s.state.inputFormatResolver;
+                        if (!l.has(r)) return;
+                        if (!a.has(i)) return;
+                        const d = l.get(r),
+                            p = a.get(i),
                             f = u.resolve(p, d),
                             h = f.text;
-                        f.edit && (f.edit.toggle || (s(h), n?.select()))
-                    })), l.addEventListener(e, "focus", (() => {
-                        n.parentElement && n.focus({
+                        f.edit && (f.edit.toggle || (c(h), o?.select()))
+                    })), s.addEventListener(e, "focus", (() => {
+                        o.parentElement && o.focus({
                             preventScroll: !0
                         })
-                    })), l.addEventListener(e, "keydown", (e => {
-                        Fe(l);
-                        const t = l.state.focusedCell,
-                            n = l.state.columnLookup,
-                            r = l.state.rowLookup,
-                            i = l.state.options.selectedCells,
-                            a = l.state.options.onSelectedCellsChange,
-                            d = l.state.options.onFocusedCellChange,
-                            p = l.state.options.editedCells,
-                            f = l.state.options.onEditedCellsChange,
-                            h = l.state.columns,
-                            _ = l.state.rows,
-                            m = l.state.text,
-                            g = l.state.inputFormatResolver,
+                    })), s.addEventListener(e, "keydown", (e => {
+                        He(s);
+                        const t = s.state.focusedCell,
+                            o = s.state.columnLookup,
+                            r = s.state.rowLookup,
+                            i = s.state.options.selectedCells,
+                            l = s.state.options.onSelectedCellsChange,
+                            a = s.state.options.onFocusedCellChange,
+                            p = s.state.options.editedCells,
+                            f = s.state.options.onEditedCellsChange,
+                            h = s.state.columns,
+                            _ = s.state.rows,
+                            m = s.state.text,
+                            g = s.state.inputFormatResolver,
                             y = (e, t) => {
-                                d(e), t.shiftKey ? a(ze(i, [e])) : a([e])
+                                a(e), t.shiftKey ? l(je(i, [e])) : l([e])
                             },
                             w = (e, r) => {
                                 if (!t) return;
-                                const i = o(t.columnId);
-                                if (!n.has(i)) return;
-                                const l = n.get(i).index,
+                                const i = n(t.columnId);
+                                if (!o.has(i)) return;
+                                const l = o.get(i).index,
                                     s = Math.max(0, Math.min(h.length - 1, l + e));
                                 if (s === l) return;
                                 const a = {
                                     rowId: t.rowId,
                                     columnId: h[s].id
                                 };
                                 y(a, r)
                             },
-                            E = (e, n) => {
+                            b = (e, o) => {
                                 if (!t) return;
-                                const i = o(t.rowId);
+                                const i = n(t.rowId);
                                 if (!r.has(i)) return;
                                 const l = r.get(i).index,
                                     s = Math.max(0, Math.min(_.length - 1, l + e));
                                 if (s === l) return;
                                 const a = {
                                     rowId: _[s].id,
                                     columnId: t.columnId
                                 };
-                                y(a, n)
+                                y(a, o)
                             },
                             v = () => {
                                 e.preventDefault(), e.stopPropagation()
                             };
                         switch (e.key) {
                             case "Escape":
-                                "" !== m ? s("") : i.length > 1 ? a([t]) : p.length > 0 ? f([]) : (d(null), a([]));
+                                "" !== m ? c("") : i.length > 1 ? l([t]) : p.length > 0 ? f([]) : (a(null), l([]));
                                 break;
                             case "Enter":
-                                c();
+                                u();
                                 break;
                             case "ArrowUp":
-                                v(), E(e.ctrlKey ? -_.length : -1, e);
+                                v(), b(e.ctrlKey ? -_.length : -1, e);
                                 break;
                             case "ArrowDown":
-                                v(), E(e.ctrlKey ? _.length : 1, e);
+                                v(), b(e.ctrlKey ? _.length : 1, e);
                                 break;
                             case "ArrowLeft":
                                 v(), w(e.ctrlKey ? -h.length : -1, e);
                                 break;
                             case "ArrowRight":
                                 v(), w(e.ctrlKey ? h.length : 1, e);
                                 break;
                             case "Delete":
                             case "Backspace":
-                                u();
+                                d();
                                 break;
                             case "c":
                                 (e => {
                                     if (!e.ctrlKey) return;
-                                    const t = function(e, t, n, r) {
+                                    const t = function(e, t, o, r) {
                                         const i = new Map(t.map((e => [e.key, e]))),
-                                            l = new Map(n.map((e => [e.key, e]))),
+                                            l = new Map(o.map((e => [e.key, e]))),
                                             s = e.map((e => ({
-                                                columnKey: o(e.columnId),
-                                                rowKey: o(e.rowId)
+                                                columnKey: n(e.columnId),
+                                                rowKey: n(e.rowId)
                                             }))).filter((e => i.has(e.columnKey) && l.has(e.rowKey))),
                                             a = new Set(s.map((e => e.columnKey))),
                                             c = new Set(s.map((e => e.rowKey)));
                                         if (0 === s.length) return "";
-                                        const u = new b(e),
+                                        const u = new E(e),
                                             d = Math.min(...s.map((e => i.get(e.columnKey).index))),
                                             p = Math.max(...s.map((e => i.get(e.columnKey).index))),
                                             f = Math.min(...s.map((e => l.get(e.rowKey).index))),
                                             h = Math.max(...s.map((e => l.get(e.rowKey).index))),
                                             _ = [];
                                         for (let e = f; e <= h; e++) {
-                                            const o = n[e],
-                                                i = o.key;
+                                            const n = o[e],
+                                                i = n.key;
                                             if (c.has(i)) {
                                                 for (let e = d; e <= p; e++) {
-                                                    const n = t[e],
-                                                        l = n.key;
+                                                    const o = t[e],
+                                                        l = o.key;
                                                     if (a.has(l)) {
                                                         if (u.isKeySelected(i, l)) {
-                                                            const e = r.resolve(o, n).text;
+                                                            const e = r.resolve(n, o).text;
                                                             _.push(e)
                                                         }
                                                         e < p && _.push("\t")
                                                     }
                                                 }
                                                 e < h && _.push("\n")
                                             }
@@ -2399,81 +2453,81 @@
                                     else {
                                         const e = document.createElement("textarea");
                                         e.value = t, document.body.appendChild(e), e.select(), document.execCommand("copy"), document.body.removeChild(e)
                                     }
                                 })(e)
                         }
                     })), new ResizeObserver((() => {
-                        l.requestNewRender()
-                    })).observe(e), l.addEventListener(n, "input", (e => {
-                        Fe(l), e.target.value ? (c(!0), n.style.opacity = 1, n.style.pointerEvents = "auto") : (e.isTrusted && u(!0), n.style.opacity = 0, n.style.pointerEvents = "none")
-                    })), l.addEventListener(n, "click", (e => {
+                        s.requestNewRender()
+                    })).observe(e), s.addEventListener(o, "input", (e => {
+                        He(s), e.target.value ? (u(!0), o.style.opacity = 1, o.style.pointerEvents = "auto") : (e.isTrusted && d(!0), o.style.opacity = 0, o.style.pointerEvents = "none")
+                    })), s.addEventListener(o, "click", (e => {
                         e.stopPropagation()
-                    })), l.addEventListener(n, "dblclick", (e => {
+                    })), s.addEventListener(o, "dblclick", (e => {
                         e.stopPropagation()
-                    })), l.addEventListener(n, "mousedown", (e => {
+                    })), s.addEventListener(o, "mousedown", (e => {
                         e.stopPropagation()
-                    })), l.addEventListener(n, "keydown", (e => {
+                    })), s.addEventListener(o, "keydown", (e => {
                         switch (e.key) {
                             case "Enter":
                             case "Escape":
                                 break;
                             case "Delete":
                             case "Backspace":
                             case "ArrowUp":
                             case "ArrowDown":
                             case "ArrowLeft":
                             case "ArrowRight":
-                                "" !== n.value && (e.stopPropagation(), l.requestNewRender());
+                                "" !== o.value && (e.stopPropagation(), s.requestNewRender());
                                 break;
                             default:
-                                e.stopPropagation(), l.requestNewRender()
+                                e.stopPropagation(), s.requestNewRender()
                         }
                     }))
                 }
 
-                function qe(e, t) {
-                    He(e);
-                    const n = e["spread-grid-context"];
-                    n.externalOptions = t, null === n.state ? (Fe(n), a(n)) : n.requestNewRender()
+                function Ye(e, t) {
+                    Ge(e);
+                    const o = e["spread-grid-context"];
+                    o.externalOptions = t, null === o.state ? (He(o), a(o)) : o.requestNewRender()
                 }
             }
         },
         __webpack_module_cache__ = {};
 
     function __webpack_require__(e) {
         var t = __webpack_module_cache__[e];
         if (void 0 !== t) return t.exports;
-        var n = __webpack_module_cache__[e] = {
+        var o = __webpack_module_cache__[e] = {
             exports: {}
         };
-        return __webpack_modules__[e](n, n.exports, __webpack_require__), n.exports
+        return __webpack_modules__[e](o, o.exports, __webpack_require__), o.exports
     }
     __webpack_require__.n = e => {
         var t = e && e.__esModule ? () => e.default : () => e;
         return __webpack_require__.d(t, {
             a: t
         }), t
     }, __webpack_require__.d = (e, t) => {
-        for (var n in t) __webpack_require__.o(t, n) && !__webpack_require__.o(e, n) && Object.defineProperty(e, n, {
+        for (var o in t) __webpack_require__.o(t, o) && !__webpack_require__.o(e, o) && Object.defineProperty(e, o, {
             enumerable: !0,
-            get: t[n]
+            get: t[o]
         })
     }, __webpack_require__.o = (e, t) => Object.prototype.hasOwnProperty.call(e, t), __webpack_require__.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     };
     var getCurrentScript = function() {
             var e = document.currentScript;
             if (!e) {
-                for (var t = document.getElementsByTagName("script"), n = [], o = 0; o < t.length; o++) n.push(t[o]);
-                e = (n = n.filter((function(e) {
+                for (var t = document.getElementsByTagName("script"), o = [], n = 0; n < t.length; n++) o.push(t[n]);
+                e = (o = o.filter((function(e) {
                     return !e.async && !e.text && !e.textContent
                 }))).slice(-1)[0]
             }
             return e
         },
         isLocalScript = function(e) {
             return /\/_dash-component-suites\//.test(e.src)
@@ -2483,20 +2537,20 @@
             get: (url = getCurrentScript().src.split("/").slice(0, -1).join("/") + "/", function() {
                 return url
             })
         }), "undefined" != typeof jsonpScriptSrc) {
         var __jsonpScriptSrc__ = jsonpScriptSrc;
         jsonpScriptSrc = function(e) {
             var t = getCurrentScript(),
-                n = isLocalScript(t),
-                o = __jsonpScriptSrc__(e);
-            if (!n) return o;
-            var r = o.split("/"),
+                o = isLocalScript(t),
+                n = __jsonpScriptSrc__(e);
+            if (!o) return n;
+            var r = n.split("/"),
                 i = r.slice(-1)[0].split(".");
-            return i.splice(1, 0, "v0_1_2m1716627209"), r.splice(-1, 1, i.join(".")), r.join("/")
+            return i.splice(1, 0, "v0_1_3m1716794736"), r.splice(-1, 1, i.join(".")), r.join("/")
         }
     }
     var __webpack_exports__ = {};
     (() => {
         __webpack_require__.r(__webpack_exports__), __webpack_require__.d(__webpack_exports__, {
             DashSpreadGrid: () => e.Z
         });
```

### Comparing `dash_spread_grid-0.1.2/dash_spread_grid/dash_spread_grid.min.js.map` & `dash_spread_grid-0.1.3/dash_spread_grid/dash_spread_grid.min.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9062375898152667%*

 * *Differences: {"'mappings'": "'2rGAMA,SAASA,SAASC,GACd,MAAwB,iBAAVA,GAAsBA,aAAiBC,MACzD,CAEA,SAASC,sBAAsBC,YAC3B,OAAOC,EAAAA,mCAAAA,UAAQ,WACX,IAAMC,QAAU,yEAEhB,OAAOF,WAAWG,KAAI,SAAAC,MAClB,IAAMC,WAAa,CAAC,EAkBpB,GAhBI,WAAYD,OACZC,WAAWC,OAASF,KAAKE,QACzB,QAASF,OACTC,WAAWE,IAAMH,KAAKG,KACtB,cAAeH,OACfC,WAAWG,UAAYC,KAAK,IAADC,OAAKR,QAAO,UAAAQ,OAASN,KAAKI,UAAS,OAC9D,UAAWJ,OACXC,WAAWR,MAAQY,KAAK,IAADC,OAAKR,QAAO,SAAAQ,OAAQN,KAAKP,MAAK,OACrD,SAAUO,OACVC,WAAWM,KAAOF,KAAK,IAADC,OAAKR,QAAO,UAAAQ,OAASN,KAAKO,KAAI,OACpD,UAAWP,OACXC […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "dash_spread_grid.min.js",
-    "mappings": "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",
+    "mappings": "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",
     "names": [
         "isString",
         "value",
         "String",
         "useResolvedFormatting",
         "formatting",
         "useMemo",
@@ -272,20 +272,26 @@
         "backgroundColor",
         "isTextValid",
         "renderInput",
         "resizableColumn",
         "resizableRow",
         "cursor",
         "renderCursor",
+        "tooltip",
+        "content",
+        "placement",
+        "tooltipPlacement",
+        "innerHTML",
+        "showPopover",
+        "renderTooltip",
         "renderInternal",
         "errorRendered",
         "display",
         "flexDirection",
         "userSelect",
-        "innerHTML",
         "message",
         "stack",
         "renderError",
         "filterRule",
         "newValue",
         "string",
         "getDataFormatting",
@@ -420,15 +426,14 @@
         "entry",
         "array",
         "currentContext",
         "getText",
         "result",
         "visible",
         "getFormattingRules",
-        "dataFormatting",
         "FormatResolver",
         "formattingRules",
         "getFormatResolver",
         "getFilterLookup",
         "primaryKey",
         "secondaryKey",
         "filterLookup",
@@ -549,25 +554,30 @@
         "internalPosition",
         "getResizableRow",
         "getResolvedSortBy",
         "getResolvedFilters",
         "getActiveColumns",
         "callback",
         "getActive",
+        "getContextFormatting",
+        "getTooltip",
+        "getTooltipPlacement",
+        "cellPlacement",
         "updateStateInternal",
         "options",
         "localOptions",
         "externalOptions",
         "memory",
         "previousState",
         "cache",
         "func",
         "dependencies",
         "previousDependencies",
         "dependency",
+        "dataFormatting",
         "invokedColumns",
         "invokedRows",
         "unfilteredColumns",
         "unfilteredRows",
         "unfilteredColumnKeys",
         "unfilteredRowKeys",
         "filterFormatting",
@@ -595,14 +605,17 @@
         "resizingColumn",
         "resizingRow",
         "renderFormatting",
         "renderFormattingRules",
         "inputFormatting",
         "inputFormattingRules",
         "inputFormatResolver",
+        "contextFormatting",
+        "contextFormattingRules",
+        "contextFormatResolver",
         "previous",
         "size",
         "getBoundingClientRect",
         "prevScrollRect",
         "requiredScrollRect",
         "preloadedScrollRect",
         "getScrollRect",
@@ -653,14 +666,18 @@
         "mouseDownPosition",
         "mouseDownCell",
         "ctrlKey",
         "setPointerCapture",
         "pointerId",
         "releasePointerCapture",
         "cellData",
+        "eventProperties",
+        "shiftKey",
+        "button",
+        "buttons",
         "indexOf",
         "getToggledValue",
         "cellType",
         "newSortBy",
         "isCurrentRule",
         "directionLoop",
         "currentRule",
@@ -672,15 +689,14 @@
         "getNewSortBy",
         "resizableColumnKey",
         "resizableRowKey",
         "select",
         "setSelectedCells",
         "setFocusedCell",
         "arrowTo",
-        "shiftKey",
         "arrowHorizontally",
         "focusedColumnIndex",
         "newColumnIndex",
         "newFocusedCell",
         "arrowVertically",
         "focusedRowIndex",
         "newRowIndex",
@@ -784,14 +800,15 @@
         "webpack:///../lib/src/state-utils/getTextResolver.js",
         "webpack:///../lib/src/core-utils/rect.js",
         "webpack:///../lib/src/state-utils/getScrollRect.js",
         "webpack:///../lib/src/state-utils/getInternalPosition.js",
         "webpack:///../lib/src/state-utils/getLookup.js",
         "webpack:///../lib/src/state-utils/getHighlightedCells.js",
         "webpack:///../lib/src/state-utils/getCellSection.js",
+        "webpack:///../lib/src/state-utils/getCellPlacement.js",
         "webpack:///../lib/src/state-utils/getInputPlacement.js",
         "webpack:///../lib/src/state-utils/getIsTextValid.js",
         "webpack:///../lib/src/state-utils/getUnfolded.js",
         "webpack:///../lib/src/types/FilteringRules.js",
         "webpack:///../lib/src/state-utils/getFilteringRules.js",
         "webpack:///../lib/src/state-utils/getFilterFormatting.js",
         "webpack:///../lib/src/state-utils/getMeasureFormatting.js",
@@ -801,14 +818,17 @@
         "webpack:///../lib/src/types/SortingRules.js",
         "webpack:///../lib/src/state-utils/getSortingRules.js",
         "webpack:///../lib/src/state-utils/getSorted.js",
         "webpack:///../lib/src/state-utils/getResizable.js",
         "webpack:///../lib/src/state-utils/getResolvedSortBy.js",
         "webpack:///../lib/src/state-utils/getResolvedFilters.js",
         "webpack:///../lib/src/state-utils/getActive.js",
+        "webpack:///../lib/src/state-utils/getContextFormatting.js",
+        "webpack:///../lib/src/state-utils/getTooltip.js",
+        "webpack:///../lib/src/state-utils/getTooltipPlacement.js",
         "webpack:///../lib/src/core/state.js",
         "webpack:///../lib/src/state-utils/getHoveredCell.js",
         "webpack:///../lib/src/state-utils/getRowIndex.js",
         "webpack:///../lib/src/state-utils/getColumnIndex.js",
         "webpack:///../lib/src/state-utils/getCombinedCells.js",
         "webpack:///../lib/src/state-utils/getReducedCells.js",
         "webpack:///../lib/src/state-utils/getMousePosition.js",
@@ -828,47 +848,48 @@
         "/* eslint-disable import/prefer-default-export */\n\nimport React, { useCallback, useMemo, useRef, useState } from 'react';\nimport PropTypes from 'prop-types';\nimport createGrid from 'js-spread-grid';\n\nfunction isString(value) {\n    return typeof value === 'string' || value instanceof String;\n}\n\nfunction useResolvedFormatting(formatting) {\n    return useMemo(() => {\n        const context = '{data, rows, columns, row, column, value, newValue, text, string, ctx}';\n\n        return formatting.map(rule => {\n            const mappedRule = {};\n\n            if ('column' in rule)\n                mappedRule.column = rule.column;\n            if ('row' in rule)\n                mappedRule.row = rule.row;\n            if ('condition' in rule)\n                mappedRule.condition = eval(`(${context}) => (${rule.condition})`);\n            if ('value' in rule)\n                mappedRule.value = eval(`(${context})=> (${rule.value})`);\n            if ('text' in rule)\n                mappedRule.text = eval(`(${context}) => (${rule.text})`);\n            if ('style' in rule)\n                mappedRule.style = isString(rule.style) ? eval(`(${context}) => (${rule.style})`) : rule.style;\n            if ('padding' in rule)\n                mappedRule.padding = isString(rule.padding) ? eval(`(${context}) => (${rule.padding})`) : rule.padding;\n            if ('draw' in rule)\n                mappedRule.draw = eval(`(${context}) => {${rule.draw}}`);\n            if ('edit' in rule)\n                if (rule.edit) {\n                    const mappedEdit = {};\n                    if ('validate' in rule.edit)\n                        mappedEdit.validate = eval(`({string}) => (${rule.edit.validate})`);\n                    if ('parse' in rule.edit)\n                        mappedEdit.parse = eval(`(${context}) => (${rule.edit.parse})`);\n                    if ('auto_commit' in rule.edit)\n                        mappedEdit.autoCommit = rule.edit.auto_commit;\n                    if ('toggle' in rule.edit)\n                        mappedEdit.toggle = rule.edit.toggle;\n                    mappedRule.edit = mappedEdit;\n                }\n                else {\n                    mappedRule.edit = rule.edit;\n                }\n\n            return mappedRule;\n        });\n    }, [formatting]);\n}\n\nfunction useResolvedFiltering(filtering) {\n    return useMemo(() => {\n        const context = '{data, rows, columns, row, column, value, text, expression}';\n\n        return filtering.map(rule => {\n            const mappedRule = {};\n\n            if ('column' in rule)\n                mappedRule.column = rule.column;\n            if ('row' in rule)\n                mappedRule.row = rule.row;\n            if ('condition' in rule)\n                mappedRule.condition = eval(`(${context}) => (${rule.condition})`);\n\n            return mappedRule;\n        });\n    }, [filtering]);\n}\n\nfunction useResolvedDataSelector(dataSelector) {\n    return useMemo(() => {\n        return eval(`({data, row, column}) => (${dataSelector})`);\n    }, [dataSelector]);\n}\n\n// TODO: Write description\n// TODO: Rename to DashSpreadGrid\nfunction DashSpreadGrid(props) {\n    // console.count('render DashSpreadGrid');\n\n    const setProps = props.setProps;\n    const counter = useRef(0);\n\n    const data = props.data;\n    const columns = props.columns;\n    const rows = props.rows;\n    const formatting = useResolvedFormatting(props.formatting);\n    const filtering = useResolvedFiltering(props.filtering);\n    const dataSelector = useResolvedDataSelector(props.data_selector);\n    const pinnedTop = props.pinned_top;\n    const pinnedBottom = props.pinned_bottom;\n    const pinnedLeft = props.pinned_left;\n    const pinnedRight = props.pinned_right;\n    const filters = props.filters;\n    const editedCells = props.edited_cells;\n    const selectedCells = props.selected_cells;\n    const onSelectedCellsChange = useCallback((selectedCells) => {\n        setProps({ selected_cells: selectedCells });\n    }, [setProps]);\n    const onFiltersChange = useCallback((filters) => {\n        setProps({ filters });\n    }, [setProps]);\n    const onEditedCellsChange = useCallback((editedCells) => {\n        setProps({ edited_cells: editedCells });\n    }, [setProps]);\n    const clickedCell = props.clicked_cell;\n    const onCellClick = useCallback((cell) => {\n        setProps({ clicked_cell: { ...cell, n: counter.current++ } });\n    }, [setProps]);\n    const clickedCustomCell = props.clicked_custom_cell;\n    const onCustomCellClick = useCallback((cell) => {\n        setProps({ clicked_custom_cell: { ...cell, n: counter.current++ } });\n    }, [setProps]);\n    const onActiveColumnsChange = useCallback((activeColumns) => {\n        setProps({ active_columns: activeColumns });\n    }, [setProps]);\n    const onActiveRowsChange = useCallback((activeRows) => {\n        setProps({ active_rows: activeRows });\n    }, [setProps]);\n\n    const [element, setElement] = useState(null);\n\n    if (element)\n        createGrid(element, {\n            data,\n            columns,\n            rows,\n            formatting,\n            filtering,\n            pinnedTop,\n            pinnedBottom,\n            pinnedLeft,\n            pinnedRight,\n            filters,\n            dataSelector,\n            editedCells,\n            selectedCells,\n            onSelectedCellsChange,\n            onEditedCellsChange,\n            onFiltersChange,\n            clickedCell,\n            onCellClick,\n            clickedCustomCell,\n            onCustomCellClick,\n            onActiveColumnsChange,\n            onActiveRowsChange\n        });\n\n    return React.createElement(\"div\", { ref: setElement });\n};\n\n// TODO: add descriptions\n// TODO: Fix types\nDashSpreadGrid.propTypes = {\n    // _\n    setProps: PropTypes.func,\n    // _\n    id: PropTypes.string,\n    // _\n    data: PropTypes.any,\n    // _\n    columns: PropTypes.array,\n    // _\n    rows: PropTypes.array,\n    // _\n    formatting: PropTypes.array,\n    // _\n    filtering: PropTypes.array,\n    // _\n    sorting: PropTypes.array,\n    // _\n    data_selector: PropTypes.string,\n    // _\n    pinned_top: PropTypes.number,\n    // _\n    pinned_bottom: PropTypes.number,\n    // _\n    pinned_left: PropTypes.number,\n    // _\n    pinned_right: PropTypes.number,\n    // _\n    borderWidth: PropTypes.number,\n    // _\n    focusedCell: PropTypes.object,\n    // _\n    selected_cells: PropTypes.array,\n    // _\n    highlightedCells: PropTypes.array,\n    // _\n    edited_cells: PropTypes.array,\n    // _\n    filters: PropTypes.array,\n    // _\n    sort_by: PropTypes.array,\n    // _\n    columnWidths: PropTypes.array,\n    // _\n    rowHeights: PropTypes.array,\n    // _\n    clicked_cell: PropTypes.object,\n    // _\n    clicked_custom_cell: PropTypes.object,\n    // _\n    active_columns: PropTypes.array,\n    // _\n    active_rows: PropTypes.array\n};\n\nDashSpreadGrid.defaultProps = {\n    data: [],\n    columns: [{ \"type\": \"DATA-BLOCK\" }],\n    rows: [{ \"type\": \"HEADER\" }, { \"type\": \"DATA-BLOCK\" }],\n    formatting: [],\n    filtering: [],\n    sorting: [],\n    data_selector: \"data[row.id][column.id]\",\n    pinned_top: 0,\n    pinned_bottom: 0,\n    pinned_left: 0,\n    pinned_right: 0,\n    borderWidth: 1,\n    focusedCell: null,\n    selected_cells: [],\n    highlightedCells: [],\n    edited_cells: [],\n    filters: [],\n    sort_by: [],\n    columnWidths: [],\n    rowHeights: [],\n    clicked_cell: null,\n    clicked_custom_cell: null,\n    active_columns: [],\n    active_rows: []\n};\n\nexport default DashSpreadGrid;\n",
         "module.exports = window[\"PropTypes\"];",
         "module.exports = window[\"React\"];",
         "function stringifyObject(object) {\n    const keys = Object.keys(object).sort();\n    const stringified = keys.map(key => {\n        return `${key}:${stringifyId(object[key])}`\n    });\n\n    return `{${stringified.join(',')}}`;\n}\n\nfunction stringifyArray(array) {\n    const stringified = array.map(stringifyId);\n\n    return `[${stringified.join(',')}]`;\n}\n\nexport default function stringifyId(key) {\n    if (key === null)\n        return 'null'\n\n    if (Array.isArray(key))\n        return stringifyArray(key)\n\n    if (typeof key === 'object')\n        return stringifyObject(key)\n\n    return JSON.stringify(key)\n}",
         "export default function getCellEditType(column, row) {\n    if (column.type === 'FILTER' ^ row.type === 'FILTER')\n        return 'FILTER';\n    return 'DATA';\n}",
         "import stringifyId from \"../core-utils/stringifyId.js\";\nimport getCellEditType from \"./getCellEditType.js\";\n\nexport default function getEditableCells(selectedCells, formatResolver, columnLookup, rowLookup) {\n    return selectedCells.map(cell => {\n        const columnKey = stringifyId(cell.columnId);\n        const rowKey = stringifyId(cell.rowId);\n\n        if (!columnLookup.has(columnKey))\n            return null;\n        if (!rowLookup.has(rowKey))\n            return null;\n\n        const column = columnLookup.get(columnKey);\n        const row = rowLookup.get(rowKey);\n\n        return {\n            edit: formatResolver.resolve(row, column).edit,\n            cell: cell,\n            type: getCellEditType(column, row)\n        }\n    }).filter(cell => cell?.edit);\n}",
         "export default function roundToPixels(value, devicePixelRatio) {\n    return Math.round(value * devicePixelRatio) / devicePixelRatio;\n}",
-        "import roundToPixels from \"../core-utils/roundToPixels.js\";\n\nfunction renderSection(context, vertical, horizontal) {\n    const state = context.state;\n    const canvas = context.canvases[`${vertical}-${horizontal}`];\n    const verticalSection = state.sections[vertical];\n    const horizontalSection = state.sections[horizontal];\n    const columns = horizontalSection.columns;\n    const rows = verticalSection.rows;\n\n    if (rows.length === 0 || columns.length === 0) {\n        if (canvas.parentElement)\n            canvas.parentElement.removeChild(canvas);\n        return;\n    }\n\n    if (!canvas.parentElement)\n        context.element.appendChild(canvas);\n\n    // Checking how often this is called\n    // console.log('draw');\n\n    // TODO: Borders are still blurry after scrolling at high zoom-out levels\n\n    const ctx = canvas.getContext(\"2d\", { alpha: false });\n    // TODO: Make that \"1\" configurable as cell spacing\n    const scrollRect = state.scrollRect;\n    const textResolver = state.textResolver;\n    // TODO: Make sure those formatters are split based on the rule areas\n    const formatResolver = state.renderFormatResolver;\n    const borderWidth = state.borderWidth;\n    const sectionBorders = {\n        top: verticalSection.showTopBorder,\n        bottom: verticalSection.showBottomBorder,\n        left: horizontalSection.showLeftBorder,\n        right: horizontalSection.showRightBorder\n    };\n    const borderOffset = borderWidth / 2;\n    const rowCount = rows.length;\n    const columnCount = columns.length;\n    const horizontalBorderCount = rowCount - 1 + (sectionBorders.top ? 1 : 0) + (sectionBorders.bottom ? 1 : 0);\n    const verticalBorderCount = columnCount - 1 + (sectionBorders.left ? 1 : 0) + (sectionBorders.right ? 1 : 0);\n    const rowHeights = rows.map(row => row.height);\n    const columnWidths = columns.map(column => column.width);\n    const totalWidth = columnWidths.reduce((a, b) => a + b, 0) + verticalBorderCount * borderWidth;\n    const totalHeight = rowHeights.reduce((a, b) => a + b, 0) + horizontalBorderCount * borderWidth;\n\n    const left = horizontal === 'center'\n        ? scrollRect.left\n        : 0;\n    const top = vertical === 'middle'\n        ? scrollRect.top\n        : 0;\n    const width = horizontal === 'center'\n        ? scrollRect.width\n        : horizontalSection.width;\n    const height = vertical === 'middle'\n        ? scrollRect.height\n        : verticalSection.height;\n\n    // TODO: Move somewhere else\n    const horizontalOffsets = columnWidths.reduce((acc, width, index) => {\n        const prevOffset = acc[index];\n        const offset = prevOffset + width + borderWidth;\n        acc.push(offset);\n        return acc;\n    }, [sectionBorders.left ? borderWidth : 0]);\n    const verticalOffsets = rowHeights.reduce((acc, height, index) => {\n        const prevOffset = acc[index];\n        const offset = prevOffset + height + borderWidth;\n        acc.push(offset);\n        return acc;\n    }, [sectionBorders.top ? borderWidth : 0]);\n\n    const columnOffsets = horizontalOffsets.slice(0, -1);\n    const rowOffsets = verticalOffsets.slice(0, -1);\n\n    const minVisibleColumnIndex = Math.max(columnOffsets.findLastIndex(offset => offset <= left), 0);\n    const maxVisibleColumnIndex = columnOffsets.findLastIndex(offset => offset <= left + width);\n    const minVisibleRowIndex = Math.max(rowOffsets.findLastIndex(offset => offset <= top), 0);\n    const maxVisibleRowIndex = rowOffsets.findLastIndex(offset => offset <= top + height);\n\n    const minVisibleVerticalBorderIndex = Math.max(minVisibleColumnIndex, sectionBorders.left ? 0 : 1);\n    const maxVisibleVerticalBorderIndex = maxVisibleColumnIndex + (sectionBorders.right ? 1 : 0);\n    const minVisibleHorizontalBorderIndex = Math.max(minVisibleRowIndex, sectionBorders.top ? 0 : 1);\n    const maxVisibleHorizontalBorderIndex = maxVisibleRowIndex + (sectionBorders.bottom ? 1 : 0);\n\n    const cells = Array.from({ length: maxVisibleRowIndex - minVisibleRowIndex + 1 }, (_, rowIndex) => {\n        const row = rows[rowIndex + minVisibleRowIndex];\n        return Array.from({ length: maxVisibleColumnIndex - minVisibleColumnIndex + 1 }, (_, columnIndex) => {\n            const column = columns[columnIndex + minVisibleColumnIndex];\n            return formatResolver.resolve(row, column);\n        });\n    });\n    const getCell = (rowIndex, columnIndex) => cells[rowIndex - minVisibleRowIndex][columnIndex - minVisibleColumnIndex];\n\n    canvas.width = Math.round(width * devicePixelRatio);\n    canvas.height = Math.round(height * devicePixelRatio);\n    canvas.style.width = `${width}px`;\n    canvas.style.height = `${height}px`;\n    canvas.style.marginLeft = `${left}px`;\n    canvas.style.marginTop = `${top}px`;\n    canvas.style.marginRight = `${totalWidth - width - left}px`;\n    canvas.style.marginBottom = `${totalHeight - height - top}px`;;\n\n    ctx.fillStyle = \"#E9E9E9\";\n    ctx.fillRect(0, 0, canvas.width, canvas.height);\n\n    const setTransform = (x, y) => {\n        ctx.setTransform(devicePixelRatio, 0, 0, devicePixelRatio, (x - left) * devicePixelRatio, (y - top) * devicePixelRatio);\n    };\n    const setClip = (x, y, width, height) => {\n        ctx.beginPath();\n        ctx.rect(x, y, width, height);\n        ctx.clip();\n    };\n\n    // Draw cells\n    for (let columnIndex = minVisibleColumnIndex; columnIndex <= maxVisibleColumnIndex; columnIndex++) {\n        ctx.save();\n        setTransform(horizontalOffsets[columnIndex], 0);\n        setClip(0, 0, columnWidths[columnIndex], totalHeight);\n\n        for (let rowIndex = minVisibleRowIndex; rowIndex <= maxVisibleRowIndex; rowIndex++) {\n            const cell = getCell(rowIndex, columnIndex);\n            const style = cell.style;\n            const cellTop = verticalOffsets[rowIndex];\n            const cellLeft = horizontalOffsets[columnIndex];\n            const cellWidth = columnWidths[columnIndex];\n            const cellHeight = rowHeights[rowIndex];\n            const text = cell.text;\n            const textBaseline = style.textBaseline || 'middle';\n            const padding = cell.padding;\n\n            setTransform(cellLeft, cellTop);\n\n            ctx.fillStyle = style.background || 'white';\n            ctx.fillRect(0, 0, cellWidth, cellHeight);\n\n            if ('draw' in cell)\n                cell.draw(ctx);\n\n            if (style.highlight) {\n                ctx.fillStyle = style.highlight;\n                ctx.fillRect(0, 0, cellWidth, cellHeight);\n            }\n\n            if (style.corner) {\n                ctx.fillStyle = style.corner;\n                ctx.beginPath();\n                ctx.moveTo(cellWidth - 7, cellHeight);\n                ctx.lineTo(cellWidth, cellHeight);\n                ctx.lineTo(cellWidth, cellHeight - 7);\n                ctx.fill();\n            }\n\n            if (text) {\n                ctx.fillStyle = style.foreground || 'black';\n                ctx.font = cell.font;\n\n                const fontMetrics = textResolver.getFontMetrics(cell.font);\n\n                const textAlign = (style.textAlign == 'center' && textResolver.measureWidth(text, cell.font) > cellWidth - padding.left - padding.right)\n                    ? 'left'\n                    : style.textAlign || 'left';\n                ctx.textAlign = textAlign;\n\n                // TODO: Make sure that values are rounded using devicePixelRatio\n                const textX = roundToPixels(\n                    textAlign === 'left' ? padding.left :\n                        textAlign === 'center' ? cellWidth / 2 :\n                            textAlign === 'right' ? cellWidth - padding.right :\n                                0,\n                    devicePixelRatio\n                );\n\n                const textY = roundToPixels(\n                    textBaseline === 'top' ? fontMetrics.middle + fontMetrics.topOffset + padding.top :\n                        textBaseline === 'middle' ? cellHeight / 2 + fontMetrics.middle :\n                            textBaseline === 'bottom' ? cellHeight + fontMetrics.middle - fontMetrics.bottomOffset - padding.bottom :\n                                0,\n                    devicePixelRatio\n                );\n\n                const fitsVertically = textY - fontMetrics.middle - fontMetrics.topOffset >= 0 && textY - fontMetrics.middle + fontMetrics.bottomOffset <= cellHeight;\n\n                if (fitsVertically) {\n                    ctx.fillText(text, textX, textY);\n                }\n                else {\n                    // TODO: Clip if the text is too high (and draw some indicator if you do)\n                    ctx.strokeStyle = '#E9E9E9';\n                    ctx.lineWidth = borderWidth;\n\n                    ctx.beginPath();\n                    ctx.moveTo(0, borderWidth + borderOffset);\n                    ctx.lineTo(cellWidth, borderWidth + borderOffset);\n                    ctx.moveTo(0, cellHeight - borderWidth - borderOffset);\n                    ctx.lineTo(cellWidth, cellHeight - borderWidth - borderOffset);\n                    ctx.stroke();\n\n                    ctx.save();\n                    setClip(0, 2 * borderWidth, cellWidth, cellHeight - 4 * borderWidth);\n\n                    ctx.fillText(text, textX, textY);\n\n                    ctx.restore();\n                }\n            }\n        }\n\n        ctx.restore();\n    }\n\n    setTransform(0, 0);\n\n    // Draw borders\n\n    // TODO: clip drawing area to the middle of neighboring columns/rows (might be useful for redrawing only the changed cells)\n    // TODO: move somewhere (?)\n    const drawBorder = (x1, y1, x2, y2, style) => {\n        if (!style)\n            return;\n        if (style.width === 0)\n            return;\n\n        const width = style.width / devicePixelRatio\n\n        const isHorizontal = y1 === y2;\n\n        // TODO: Don't add offset if the border is not continued\n        const xa = x1 - (isHorizontal ? width / 2 : 0);\n        const ya = y1 - (!isHorizontal ? width / 2 : 0);\n        const xb = x2 + (isHorizontal ? width / 2 : 0);\n        const yb = y2 + (!isHorizontal ? width / 2 : 0);\n\n        ctx.strokeStyle = style.color || 'black'; // TODO: resolve this color earlier\n        ctx.lineWidth = width;\n\n        if (style.dash) {\n            ctx.setLineDash(style.dash.map(value => value / devicePixelRatio));\n            ctx.lineDashOffset = (isHorizontal ? xa : ya);\n        }\n        else {\n            ctx.setLineDash([]);\n        }\n\n        ctx.beginPath();\n        ctx.moveTo(xa, ya);\n        ctx.lineTo(xb, yb);\n        ctx.stroke();\n    }\n\n    const selectBorder = (borderStyleA, borderStyleB) => {\n        if (!borderStyleA)\n            return borderStyleB;\n\n        if (!borderStyleB)\n            return borderStyleA;\n\n        if (borderStyleA.index > borderStyleB.index)\n            return borderStyleA;\n\n        return borderStyleB;\n    }\n\n    // TODO: Move somewhere else (?)\n    for (let horizontalBorderIndex = minVisibleHorizontalBorderIndex; horizontalBorderIndex <= maxVisibleHorizontalBorderIndex; horizontalBorderIndex++) {\n        const topRowIndex = horizontalBorderIndex - 1;\n        const bottomRowIndex = horizontalBorderIndex;\n\n        for (let columnIndex = minVisibleColumnIndex; columnIndex <= maxVisibleColumnIndex; columnIndex++) {\n            const topBorderStyle = topRowIndex >= minVisibleRowIndex ? getCell(topRowIndex, columnIndex).style.borderBottom : null;\n            const bottomBorderStyle = bottomRowIndex <= maxVisibleRowIndex ? getCell(bottomRowIndex, columnIndex).style.borderTop : null;\n\n            const borderStyle = selectBorder(topBorderStyle, bottomBorderStyle);\n\n            drawBorder(\n                horizontalOffsets[columnIndex] - borderOffset,\n                verticalOffsets[bottomRowIndex] - borderOffset,\n                horizontalOffsets[columnIndex + 1] - borderOffset,\n                verticalOffsets[bottomRowIndex] - borderOffset,\n                borderStyle);\n        }\n    }\n\n    for (let verticalBorderIndex = minVisibleVerticalBorderIndex; verticalBorderIndex <= maxVisibleVerticalBorderIndex; verticalBorderIndex++) {\n        const leftColumnIndex = verticalBorderIndex - 1;\n        const rightColumnIndex = verticalBorderIndex;\n\n        for (let rowIndex = minVisibleRowIndex; rowIndex <= maxVisibleRowIndex; rowIndex++) {\n            const leftBorderStyle = leftColumnIndex >= minVisibleColumnIndex ? getCell(rowIndex, leftColumnIndex).style.borderRight : null;\n            const rightBorderStyle = rightColumnIndex <= maxVisibleColumnIndex ? getCell(rowIndex, rightColumnIndex).style.borderLeft : null;\n\n            const borderStyle = selectBorder(leftBorderStyle, rightBorderStyle);\n\n            drawBorder(\n                horizontalOffsets[rightColumnIndex] - borderOffset,\n                verticalOffsets[rowIndex] - borderOffset,\n                horizontalOffsets[rightColumnIndex] - borderOffset,\n                verticalOffsets[rowIndex + 1] - borderOffset,\n                borderStyle);\n        }\n    }\n}\n\nfunction renderInput(context) {\n    const element = context.element;\n    const input = context.input;\n    const state = context.state;\n    const inputPlacement = state.inputPlacement;\n\n    if (!inputPlacement) {\n        if (input.parentElement) {\n            const hasFocus = document.activeElement === input;\n            input.parentElement.removeChild(input);\n            if (hasFocus)\n                element.focus({ preventScroll: true });\n        }\n        return;\n    }\n\n    const canvas = context.canvases[inputPlacement.section];\n\n    input.style.left = 'left' in inputPlacement ? `${inputPlacement.left}px` : '0';\n    input.style.top = 'top' in inputPlacement ? `${inputPlacement.top}px` : '0';\n    input.style.right = 'right' in inputPlacement ? `${inputPlacement.right}px` : '0';\n    input.style.bottom = 'bottom' in inputPlacement ? `${inputPlacement.bottom}px` : '0';\n    input.style.marginLeft = 'marginLeft' in inputPlacement ? `${inputPlacement.marginLeft}px` : '0';\n    input.style.marginTop = 'marginTop' in inputPlacement ? `${inputPlacement.marginTop}px` : '0';\n    input.style.width = `${inputPlacement.width}px`;\n    input.style.height = `${inputPlacement.height}px`;\n    input.style.gridArea = canvas.style.gridArea;\n    input.style.zIndex = canvas.style.zIndex;\n    input.style.backgroundColor = state.isTextValid ? 'white' : '#eb3434';\n\n    if (!input.parentElement) {\n        const hasFocus = document.activeElement === element;\n        element.appendChild(input);\n        if (hasFocus)\n            input.focus({ preventScroll: true });\n    }\n}\n\nfunction renderCursor(context) {\n    const element = context.element;\n    const state = context.state;\n\n    if (state.resizableColumn && state.resizableRow)\n        element.style.cursor = 'nwse-resize';\n    else if (state.resizableColumn)\n        element.style.cursor = 'col-resize';\n    else if (state.resizableRow)\n        element.style.cursor = 'row-resize';\n    else\n        element.style.cursor = 'default';\n}\n\nfunction renderInternal(context) {\n    renderSection(context, 'top', 'left');\n    renderSection(context, 'top', 'center');\n    renderSection(context, 'top', 'right');\n    renderSection(context, 'middle', 'left');\n    renderSection(context, 'middle', 'center');\n    renderSection(context, 'middle', 'right');\n    renderSection(context, 'bottom', 'left');\n    renderSection(context, 'bottom', 'center');\n    renderSection(context, 'bottom', 'right');\n\n    renderInput(context);\n    renderCursor(context);\n}\n\nfunction renderError(context) {\n    if (context.errorRendered)\n        return;\n\n    context.errorRendered = true;\n\n    const element = context.element;\n    const error = context.error;\n\n    element.style.backgroundColor = '#9f0000';\n    element.style.color = 'white';\n    element.style.padding = '20px';\n    element.style.display = 'flex';\n    element.style.flexDirection = 'column';\n    element.style.userSelect = 'text';\n    element.innerHTML = `\n        <div style=\"font-size: 16px;\">\n            An error occurred while rendering the grid, please contact the support.\n        </div>\n        <div style=\"font-size: 20px; font-weight: bold; padding: 20px 0;\">\n            ${error.message}\n        </div>\n        <div style=\"font-size: 16px; white-space: pre-wrap;\">${error.stack}</div>\n    `;\n}\n\nexport default function render(context) {\n    if (!context.error) {\n        try {\n            renderInternal(context);\n        }\n        catch (error) {\n            context.error = error;\n        }\n    }\n\n    if (context.error)\n        renderError(context);\n}",
+        "import roundToPixels from \"../core-utils/roundToPixels.js\";\n\nfunction renderSection(context, vertical, horizontal) {\n    const state = context.state;\n    const canvas = context.canvases[`${vertical}-${horizontal}`];\n    const verticalSection = state.sections[vertical];\n    const horizontalSection = state.sections[horizontal];\n    const columns = horizontalSection.columns;\n    const rows = verticalSection.rows;\n\n    if (rows.length === 0 || columns.length === 0) {\n        if (canvas.parentElement)\n            canvas.parentElement.removeChild(canvas);\n        return;\n    }\n\n    if (!canvas.parentElement)\n        context.element.appendChild(canvas);\n\n    // Checking how often this is called\n    // console.log('draw');\n\n    // TODO: Borders are still blurry after scrolling at high zoom-out levels\n\n    const ctx = canvas.getContext(\"2d\", { alpha: false });\n    // TODO: Make that \"1\" configurable as cell spacing\n    const scrollRect = state.scrollRect;\n    const textResolver = state.textResolver;\n    // TODO: Make sure those formatters are split based on the rule areas\n    const formatResolver = state.renderFormatResolver;\n    const borderWidth = state.borderWidth;\n    const sectionBorders = {\n        top: verticalSection.showTopBorder,\n        bottom: verticalSection.showBottomBorder,\n        left: horizontalSection.showLeftBorder,\n        right: horizontalSection.showRightBorder\n    };\n    const borderOffset = borderWidth / 2;\n    const rowCount = rows.length;\n    const columnCount = columns.length;\n    const horizontalBorderCount = rowCount - 1 + (sectionBorders.top ? 1 : 0) + (sectionBorders.bottom ? 1 : 0);\n    const verticalBorderCount = columnCount - 1 + (sectionBorders.left ? 1 : 0) + (sectionBorders.right ? 1 : 0);\n    const rowHeights = rows.map(row => row.height);\n    const columnWidths = columns.map(column => column.width);\n    const totalWidth = columnWidths.reduce((a, b) => a + b, 0) + verticalBorderCount * borderWidth;\n    const totalHeight = rowHeights.reduce((a, b) => a + b, 0) + horizontalBorderCount * borderWidth;\n\n    const left = horizontal === 'center'\n        ? scrollRect.left\n        : 0;\n    const top = vertical === 'middle'\n        ? scrollRect.top\n        : 0;\n    const width = horizontal === 'center'\n        ? scrollRect.width\n        : horizontalSection.width;\n    const height = vertical === 'middle'\n        ? scrollRect.height\n        : verticalSection.height;\n\n    // TODO: Move somewhere else\n    const horizontalOffsets = columnWidths.reduce((acc, width, index) => {\n        const prevOffset = acc[index];\n        const offset = prevOffset + width + borderWidth;\n        acc.push(offset);\n        return acc;\n    }, [sectionBorders.left ? borderWidth : 0]);\n    const verticalOffsets = rowHeights.reduce((acc, height, index) => {\n        const prevOffset = acc[index];\n        const offset = prevOffset + height + borderWidth;\n        acc.push(offset);\n        return acc;\n    }, [sectionBorders.top ? borderWidth : 0]);\n\n    const columnOffsets = horizontalOffsets.slice(0, -1);\n    const rowOffsets = verticalOffsets.slice(0, -1);\n\n    const minVisibleColumnIndex = Math.max(columnOffsets.findLastIndex(offset => offset <= left), 0);\n    const maxVisibleColumnIndex = columnOffsets.findLastIndex(offset => offset <= left + width);\n    const minVisibleRowIndex = Math.max(rowOffsets.findLastIndex(offset => offset <= top), 0);\n    const maxVisibleRowIndex = rowOffsets.findLastIndex(offset => offset <= top + height);\n\n    const minVisibleVerticalBorderIndex = Math.max(minVisibleColumnIndex, sectionBorders.left ? 0 : 1);\n    const maxVisibleVerticalBorderIndex = maxVisibleColumnIndex + (sectionBorders.right ? 1 : 0);\n    const minVisibleHorizontalBorderIndex = Math.max(minVisibleRowIndex, sectionBorders.top ? 0 : 1);\n    const maxVisibleHorizontalBorderIndex = maxVisibleRowIndex + (sectionBorders.bottom ? 1 : 0);\n\n    const cells = Array.from({ length: maxVisibleRowIndex - minVisibleRowIndex + 1 }, (_, rowIndex) => {\n        const row = rows[rowIndex + minVisibleRowIndex];\n        return Array.from({ length: maxVisibleColumnIndex - minVisibleColumnIndex + 1 }, (_, columnIndex) => {\n            const column = columns[columnIndex + minVisibleColumnIndex];\n            return formatResolver.resolve(row, column);\n        });\n    });\n    const getCell = (rowIndex, columnIndex) => cells[rowIndex - minVisibleRowIndex][columnIndex - minVisibleColumnIndex];\n\n    canvas.width = Math.round(width * devicePixelRatio);\n    canvas.height = Math.round(height * devicePixelRatio);\n    canvas.style.width = `${width}px`;\n    canvas.style.height = `${height}px`;\n    canvas.style.marginLeft = `${left}px`;\n    canvas.style.marginTop = `${top}px`;\n    canvas.style.marginRight = `${totalWidth - width - left}px`;\n    canvas.style.marginBottom = `${totalHeight - height - top}px`;;\n\n    ctx.fillStyle = \"#E9E9E9\";\n    ctx.fillRect(0, 0, canvas.width, canvas.height);\n\n    const setTransform = (x, y) => {\n        ctx.setTransform(devicePixelRatio, 0, 0, devicePixelRatio, (x - left) * devicePixelRatio, (y - top) * devicePixelRatio);\n    };\n    const setClip = (x, y, width, height) => {\n        ctx.beginPath();\n        ctx.rect(x, y, width, height);\n        ctx.clip();\n    };\n\n    // Draw cells\n    for (let columnIndex = minVisibleColumnIndex; columnIndex <= maxVisibleColumnIndex; columnIndex++) {\n        ctx.save();\n        setTransform(horizontalOffsets[columnIndex], 0);\n        setClip(0, 0, columnWidths[columnIndex], totalHeight);\n\n        for (let rowIndex = minVisibleRowIndex; rowIndex <= maxVisibleRowIndex; rowIndex++) {\n            const cell = getCell(rowIndex, columnIndex);\n            const style = cell.style;\n            const cellTop = verticalOffsets[rowIndex];\n            const cellLeft = horizontalOffsets[columnIndex];\n            const cellWidth = columnWidths[columnIndex];\n            const cellHeight = rowHeights[rowIndex];\n            const text = cell.text;\n            const textBaseline = style.textBaseline || 'middle';\n            const padding = cell.padding;\n\n            setTransform(cellLeft, cellTop);\n\n            ctx.fillStyle = style.background || 'white';\n            ctx.fillRect(0, 0, cellWidth, cellHeight);\n\n            if ('draw' in cell)\n                cell.draw(ctx);\n\n            if (style.highlight) {\n                ctx.fillStyle = style.highlight;\n                ctx.fillRect(0, 0, cellWidth, cellHeight);\n            }\n\n            if (style.corner) {\n                ctx.fillStyle = style.corner;\n                ctx.beginPath();\n                ctx.moveTo(cellWidth - 7, cellHeight);\n                ctx.lineTo(cellWidth, cellHeight);\n                ctx.lineTo(cellWidth, cellHeight - 7);\n                ctx.fill();\n            }\n\n            if (text) {\n                ctx.fillStyle = style.foreground || 'black';\n                ctx.font = cell.font;\n\n                const fontMetrics = textResolver.getFontMetrics(cell.font);\n\n                const textAlign = (style.textAlign == 'center' && textResolver.measureWidth(text, cell.font) > cellWidth - padding.left - padding.right)\n                    ? 'left'\n                    : style.textAlign || 'left';\n                ctx.textAlign = textAlign;\n\n                // TODO: Make sure that values are rounded using devicePixelRatio\n                const textX = roundToPixels(\n                    textAlign === 'left' ? padding.left :\n                        textAlign === 'center' ? cellWidth / 2 :\n                            textAlign === 'right' ? cellWidth - padding.right :\n                                0,\n                    devicePixelRatio\n                );\n\n                const textY = roundToPixels(\n                    textBaseline === 'top' ? fontMetrics.middle + fontMetrics.topOffset + padding.top :\n                        textBaseline === 'middle' ? cellHeight / 2 + fontMetrics.middle :\n                            textBaseline === 'bottom' ? cellHeight + fontMetrics.middle - fontMetrics.bottomOffset - padding.bottom :\n                                0,\n                    devicePixelRatio\n                );\n\n                const fitsVertically = textY - fontMetrics.middle - fontMetrics.topOffset >= 0 && textY - fontMetrics.middle + fontMetrics.bottomOffset <= cellHeight;\n\n                if (fitsVertically) {\n                    ctx.fillText(text, textX, textY);\n                }\n                else {\n                    // TODO: Clip if the text is too high (and draw some indicator if you do)\n                    ctx.strokeStyle = '#E9E9E9';\n                    ctx.lineWidth = borderWidth;\n\n                    ctx.beginPath();\n                    ctx.moveTo(0, borderWidth + borderOffset);\n                    ctx.lineTo(cellWidth, borderWidth + borderOffset);\n                    ctx.moveTo(0, cellHeight - borderWidth - borderOffset);\n                    ctx.lineTo(cellWidth, cellHeight - borderWidth - borderOffset);\n                    ctx.stroke();\n\n                    ctx.save();\n                    setClip(0, 2 * borderWidth, cellWidth, cellHeight - 4 * borderWidth);\n\n                    ctx.fillText(text, textX, textY);\n\n                    ctx.restore();\n                }\n            }\n        }\n\n        ctx.restore();\n    }\n\n    setTransform(0, 0);\n\n    // Draw borders\n\n    // TODO: clip drawing area to the middle of neighboring columns/rows (might be useful for redrawing only the changed cells)\n    // TODO: move somewhere (?)\n    const drawBorder = (x1, y1, x2, y2, style) => {\n        if (!style)\n            return;\n        if (style.width === 0)\n            return;\n\n        const width = style.width / devicePixelRatio\n\n        const isHorizontal = y1 === y2;\n\n        // TODO: Don't add offset if the border is not continued\n        const xa = x1 - (isHorizontal ? width / 2 : 0);\n        const ya = y1 - (!isHorizontal ? width / 2 : 0);\n        const xb = x2 + (isHorizontal ? width / 2 : 0);\n        const yb = y2 + (!isHorizontal ? width / 2 : 0);\n\n        ctx.strokeStyle = style.color || 'black'; // TODO: resolve this color earlier\n        ctx.lineWidth = width;\n\n        if (style.dash) {\n            ctx.setLineDash(style.dash.map(value => value / devicePixelRatio));\n            ctx.lineDashOffset = (isHorizontal ? xa : ya);\n        }\n        else {\n            ctx.setLineDash([]);\n        }\n\n        ctx.beginPath();\n        ctx.moveTo(xa, ya);\n        ctx.lineTo(xb, yb);\n        ctx.stroke();\n    }\n\n    const selectBorder = (borderStyleA, borderStyleB) => {\n        if (!borderStyleA)\n            return borderStyleB;\n\n        if (!borderStyleB)\n            return borderStyleA;\n\n        if (borderStyleA.index > borderStyleB.index)\n            return borderStyleA;\n\n        return borderStyleB;\n    }\n\n    // TODO: Move somewhere else (?)\n    for (let horizontalBorderIndex = minVisibleHorizontalBorderIndex; horizontalBorderIndex <= maxVisibleHorizontalBorderIndex; horizontalBorderIndex++) {\n        const topRowIndex = horizontalBorderIndex - 1;\n        const bottomRowIndex = horizontalBorderIndex;\n\n        for (let columnIndex = minVisibleColumnIndex; columnIndex <= maxVisibleColumnIndex; columnIndex++) {\n            const topBorderStyle = topRowIndex >= minVisibleRowIndex ? getCell(topRowIndex, columnIndex).style.borderBottom : null;\n            const bottomBorderStyle = bottomRowIndex <= maxVisibleRowIndex ? getCell(bottomRowIndex, columnIndex).style.borderTop : null;\n\n            const borderStyle = selectBorder(topBorderStyle, bottomBorderStyle);\n\n            drawBorder(\n                horizontalOffsets[columnIndex] - borderOffset,\n                verticalOffsets[bottomRowIndex] - borderOffset,\n                horizontalOffsets[columnIndex + 1] - borderOffset,\n                verticalOffsets[bottomRowIndex] - borderOffset,\n                borderStyle);\n        }\n    }\n\n    for (let verticalBorderIndex = minVisibleVerticalBorderIndex; verticalBorderIndex <= maxVisibleVerticalBorderIndex; verticalBorderIndex++) {\n        const leftColumnIndex = verticalBorderIndex - 1;\n        const rightColumnIndex = verticalBorderIndex;\n\n        for (let rowIndex = minVisibleRowIndex; rowIndex <= maxVisibleRowIndex; rowIndex++) {\n            const leftBorderStyle = leftColumnIndex >= minVisibleColumnIndex ? getCell(rowIndex, leftColumnIndex).style.borderRight : null;\n            const rightBorderStyle = rightColumnIndex <= maxVisibleColumnIndex ? getCell(rowIndex, rightColumnIndex).style.borderLeft : null;\n\n            const borderStyle = selectBorder(leftBorderStyle, rightBorderStyle);\n\n            drawBorder(\n                horizontalOffsets[rightColumnIndex] - borderOffset,\n                verticalOffsets[rowIndex] - borderOffset,\n                horizontalOffsets[rightColumnIndex] - borderOffset,\n                verticalOffsets[rowIndex + 1] - borderOffset,\n                borderStyle);\n        }\n    }\n}\n\nfunction renderInput(context) {\n    const element = context.element;\n    const input = context.input;\n    const state = context.state;\n    const inputPlacement = state.inputPlacement;\n\n    if (!inputPlacement) {\n        if (input.parentElement) {\n            const hasFocus = document.activeElement === input;\n            input.parentElement.removeChild(input);\n            if (hasFocus)\n                element.focus({ preventScroll: true });\n        }\n        return;\n    }\n\n    const canvas = context.canvases[inputPlacement.section];\n\n    input.style.left = 'left' in inputPlacement ? `${inputPlacement.left}px` : '0';\n    input.style.top = 'top' in inputPlacement ? `${inputPlacement.top}px` : '0';\n    input.style.right = 'right' in inputPlacement ? `${inputPlacement.right}px` : '0';\n    input.style.bottom = 'bottom' in inputPlacement ? `${inputPlacement.bottom}px` : '0';\n    input.style.marginLeft = 'marginLeft' in inputPlacement ? `${inputPlacement.marginLeft}px` : '0';\n    input.style.marginTop = 'marginTop' in inputPlacement ? `${inputPlacement.marginTop}px` : '0';\n    input.style.width = `${inputPlacement.width}px`;\n    input.style.height = `${inputPlacement.height}px`;\n    input.style.gridArea = canvas.style.gridArea;\n    input.style.zIndex = canvas.style.zIndex;\n    input.style.backgroundColor = state.isTextValid ? 'white' : '#eb3434';\n\n    if (!input.parentElement) {\n        const hasFocus = document.activeElement === element;\n        element.appendChild(input);\n        if (hasFocus)\n            input.focus({ preventScroll: true });\n    }\n}\n\nfunction renderCursor(context) {\n    const element = context.element;\n    const state = context.state;\n\n    if (state.resizableColumn && state.resizableRow)\n        element.style.cursor = 'nwse-resize';\n    else if (state.resizableColumn)\n        element.style.cursor = 'col-resize';\n    else if (state.resizableRow)\n        element.style.cursor = 'row-resize';\n    else\n        element.style.cursor = 'default';\n}\n\nfunction renderTooltip(context) {\n    const element = context.element;\n    const tooltip = context.tooltip;\n    const content = context.state.tooltip;\n    const placement = context.state.tooltipPlacement;\n\n    if (!placement) {\n        if (tooltip.parentElement)\n            tooltip.parentElement.removeChild(tooltip);\n        return;\n    }\n\n    tooltip.innerHTML = content;\n    tooltip.style.left = `${placement.left}px`;\n    tooltip.style.top = `${placement.top}px`;\n\n    if (!tooltip.parentElement) {\n        element.appendChild(tooltip);\n        tooltip.showPopover();\n    }\n}\n\nfunction renderInternal(context) {\n    renderSection(context, 'top', 'left');\n    renderSection(context, 'top', 'center');\n    renderSection(context, 'top', 'right');\n    renderSection(context, 'middle', 'left');\n    renderSection(context, 'middle', 'center');\n    renderSection(context, 'middle', 'right');\n    renderSection(context, 'bottom', 'left');\n    renderSection(context, 'bottom', 'center');\n    renderSection(context, 'bottom', 'right');\n\n    renderInput(context);\n    renderCursor(context);\n    renderTooltip(context);\n}\n\nfunction renderError(context) {\n    if (context.errorRendered)\n        return;\n\n    context.errorRendered = true;\n\n    const element = context.element;\n    const error = context.error;\n\n    element.style.backgroundColor = '#9f0000';\n    element.style.color = 'white';\n    element.style.padding = '20px';\n    element.style.display = 'flex';\n    element.style.flexDirection = 'column';\n    element.style.userSelect = 'text';\n    element.innerHTML = `\n        <div style=\"font-size: 16px;\">\n            An error occurred while rendering the grid, please contact the support.\n        </div>\n        <div style=\"font-size: 20px; font-weight: bold; padding: 20px 0;\">\n            ${error.message}\n        </div>\n        <div style=\"font-size: 16px; white-space: pre-wrap;\">${error.stack}</div>\n    `;\n}\n\nexport default function render(context) {\n    if (!context.error) {\n        try {\n            renderInternal(context);\n        }\n        catch (error) {\n            context.error = error;\n        }\n    }\n\n    if (context.error)\n        renderError(context);\n}",
         "const filterRule = {\n    value: ({ newValue }) => newValue || '',\n    text: ({ newValue }) => newValue || 'Search...', // TODO: Move to render formatting?\n    edit: {\n        validate: () => true,\n        parse: ({ string }) => string,\n        autoCommit: true\n    }\n};\n\nexport default function getDataFormatting(formatting, dataSelector, sortBy) {\n    return [\n        {\n            column: { type: 'DATA' },\n            row: { type: 'HEADER' },\n            value: ({ column }) => column.header === undefined ? column.id : column.header\n        },\n        {\n            column: { type: 'HEADER' },\n            row: { type: 'DATA' },\n            value: ({ row }) => row.header === undefined ? row.id : row.header\n        },\n        {\n            column: { type: 'HEADER' },\n            row: { type: 'SPECIAL' },\n            value: ''\n        },\n        {\n            column: { type: 'SPECIAL' },\n            row: { type: 'HEADER' },\n            value: ''\n        },\n        {\n            column: { type: 'DATA' },\n            row: { type: 'FILTER' },\n            ...filterRule\n        },\n        {\n            column: { type: 'FILTER' },\n            row: { type: 'DATA' },\n            ...filterRule\n        },\n        {\n            column: { type: 'DATA' },\n            row: { type: 'DATA' },\n            value: dataSelector\n        },\n        ...formatting,\n        // TODO: Fix headers of sorted rows\n        ...sortBy.map(({ columnId, rowId, direction }, index) => ({\n            column: { id: columnId },\n            row: { id: rowId },\n            text: ({ value, text }) => `${sortBy.length > 1 ? index + 1 : ''}${direction === 'ASC' ? '\u21e3' : '\u21e1'} ${text || value}`\n        })),\n    ];\n}",
-        "const commonFields = ['column', 'row', 'condition'];\n\nfunction reduce(rule, fields) {\n  const reducedRule = {};\n  for (const field of fields) {\n    if (field in rule)\n      reducedRule[field] = rule[field];\n  }\n  return reducedRule;\n}\n\nfunction hasImpact(rule) {\n  const allKeys = Object.keys(rule).length;\n  const commonKeys = Object.keys(rule).filter(key => commonFields.includes(key)).length;\n\n  return allKeys > commonKeys;\n}\n\nexport default function getReducedFormatting(formatting, fields) {\n  const acceptedFields = [...commonFields, ...fields];\n\n  return formatting.map(rule => reduce(rule, acceptedFields)).filter(hasImpact);\n}",
+        "const commonFields = ['column', 'row', 'condition'];\n\nfunction reduce(rule, fields) {\n    const reducedRule = {};\n    for (const field of fields) {\n        if (field in rule)\n            reducedRule[field] = rule[field];\n    }\n    return reducedRule;\n}\n\nfunction hasImpact(rule) {\n    const allKeys = Object.keys(rule).length;\n    const commonKeys = Object.keys(rule).filter(key => commonFields.includes(key)).length;\n\n    return allKeys > commonKeys;\n}\n\nexport default function getReducedFormatting(formatting, fields) {\n    const acceptedFields = [...commonFields, ...fields];\n\n    return formatting.map(rule => reduce(rule, acceptedFields)).filter(hasImpact);\n}",
         "import getReducedFormatting from \"./getReducedFormatting.js\";\n\nexport default function getInputFormatting(formatting) {\n    return getReducedFormatting(formatting, ['value', 'text', 'edit']);\n}",
         "import stringifyId from '../core-utils/stringifyId.js';\n\nfunction getHighlightColor(baseColor, isStrong) {\n    if (isStrong)\n        return baseColor + '99';\n    else\n        return baseColor + '33';\n}\n\nexport default function getRenderFormatting(formatting, hoveredCell, focusedCell, selection, highlight, edition, sortBy, resizableColumn, resizableRow, borderWidth) {\n    const focusedColumnKey = focusedCell ? stringifyId(focusedCell.columnId) : null;\n    const focusedRowKey = focusedCell ? stringifyId(focusedCell.rowId) : null;\n    const isResizingColumn = resizableColumn !== null;\n    const isResizingRow = resizableRow !== null;\n    const isResizing = isResizingColumn || isResizingRow;\n    const selectionBorderWidth = borderWidth + 2;\n    const resizableBorderWidth = borderWidth + 4;\n\n    const isSelected = (rows, columns, rowIndex, columnIndex) => {\n        if (rowIndex < 0 || rowIndex >= rows.length)\n            return false;\n        if (columnIndex < 0 || columnIndex >= columns.length)\n            return false;\n\n        const rowKey = rows[rowIndex].key;\n        const columnKey = columns[columnIndex].key;\n\n        return selection.isKeySelected(rowKey, columnKey);\n    };\n\n    const optional = (condition, style) => {\n        if (condition)\n            return [style];\n        else\n            return [];\n    }\n\n    return [\n        {\n            column: { type: 'DATA' },\n            row: { type: 'FILTER' },\n            style: ({ newValue }) => ({ background: '#FBFBFB', foreground: newValue ? 'black' : '#cccccc', border: { width: 1, color: 'gray' } })\n        },\n        {\n            column: { type: 'FILTER' },\n            row: { type: 'DATA' },\n            style: ({ newValue }) => ({ background: '#FBFBFB', foreground: newValue ? 'black' : '#cccccc', border: { width: 1, color: 'gray' } })\n        },\n        {\n            column: { type: 'ANY' },\n            row: { type: 'HEADER' },\n            style: { background: '#F5F5F5', border: { width: borderWidth, color: 'gray' } }\n        },\n        {\n            column: { type: 'HEADER' },\n            row: { type: 'ANY' },\n            style: { background: '#F5F5F5', border: { width: borderWidth, color: 'gray' } }\n        },\n        {\n            column: { type: 'HEADER' },\n            row: { type: 'HEADER' },\n            style: { background: '#E0E0E0' }\n        },\n        ...formatting,\n        // TODO: optionally re-enable\n        // ...optional(hoveredCell && !isResizingColumn, {\n        //     column: { id: hoveredCell?.columnId },\n        //     row: { type: 'ANY' },\n        //     style: { highlight: '#81948133' },\n        // }),\n        ...optional(hoveredCell && !isResizingRow, {\n            column: { type: 'ANY' },\n            row: { id: hoveredCell?.rowId },\n            style: { highlight: '#81948133' },\n        }),\n        ...optional(hoveredCell && !isResizing, {\n            column: { id: hoveredCell?.columnId },\n            row: { id: hoveredCell?.rowId },\n            style: { highlight: '#81948188' },\n        }),\n        {\n            column: { type: 'ANY' },\n            row: { type: 'ANY' },\n            condition: ({ rows, columns, row, column }) => isSelected(rows, columns, row.index, column.index),\n            style: ({ rows, columns, row, column, edit }) => ({\n                ...(!isSelected(rows, columns, row.index - 1, column.index) ? { borderTop: { width: selectionBorderWidth, color: '#596959', index: Number.MAX_SAFE_INTEGER } } : {}),\n                ...(!isSelected(rows, columns, row.index + 1, column.index) ? { borderBottom: { width: selectionBorderWidth, color: '#596959', index: Number.MAX_SAFE_INTEGER } } : {}),\n                ...(!isSelected(rows, columns, row.index, column.index - 1) ? { borderLeft: { width: selectionBorderWidth, color: '#596959', index: Number.MAX_SAFE_INTEGER } } : {}),\n                ...(!isSelected(rows, columns, row.index, column.index + 1) ? { borderRight: { width: selectionBorderWidth, color: '#596959', index: Number.MAX_SAFE_INTEGER } } : {}),\n                highlight: getHighlightColor(edit ? '#798d9c' : '#819481', focusedColumnKey !== column.key || focusedRowKey !== row.key)\n            }),\n        },\n        {\n            column: { type: 'ANY' },\n            row: { type: 'ANY' },\n            condition: ({ row, column }) => highlight.isKeySelected(row.key, column.key),\n            style: ({ row, column }) => ({\n                highlight: getHighlightColor('#93a8b8', focusedColumnKey !== column.key || focusedRowKey !== row.key)\n            })\n        },\n        ...optional(focusedCell, {\n            column: { id: focusedCell?.columnId },\n            row: { id: focusedCell?.rowId },\n            style: { highlight: '#ffffffaa' }\n        }),\n        ...sortBy.map(({ columnId, rowId, direction }, index) => ({\n            column: { id: columnId },\n            row: { id: rowId },\n            style: { highlight: '#0377fc44' }\n        })),\n        {\n            column: { type: 'ANY' },\n            row: { type: 'ANY' },\n            condition: ({ edit }) => edit,\n            style: { corner: '#77777720' },\n        },\n        {\n            column: { type: 'ANY' },\n            row: { type: 'ANY' },\n            condition: ({ row, column }) => edition.hasValueByKey(row.key, column.key),\n            style: { corner: 'darkgreen' },\n        },\n        ...optional(resizableColumn, {\n            column: { id: resizableColumn },\n            row: { type: 'HEADER' },\n            style: { borderRight: { width: resizableBorderWidth, color: 'cornflowerblue' } }\n        }),\n        ...optional(resizableRow, {\n            column: { type: 'HEADER' },\n            row: { id: resizableRow },\n            style: { borderBottom: { width: resizableBorderWidth, color: 'cornflowerblue' } }\n        }),\n    ];\n}",
         "export default function getSections(columns, rows) {\n    const topLength = rows.filter(row => row.pinned === 'BEGIN').length; // TODO: optimize\n    const bottomLength = rows.filter(row => row.pinned === 'END').length;\n    const middleLength = rows.length - topLength - bottomLength;\n    const leftLength = columns.filter(column => column.pinned === 'BEGIN').length;\n    const rightLength = columns.filter(column => column.pinned === 'END').length;\n    const centerLength = columns.length - leftLength - rightLength;\n\n    const topRows = rows.slice(0, topLength);\n    const bottomRows = rows.slice(rows.length - bottomLength, rows.length);\n    const middleRows = rows.slice(topLength, rows.length - bottomLength);\n    const leftColumns = columns.slice(0, leftLength);\n    const rightColumns = columns.slice(columns.length - rightLength, columns.length);\n    const centerColumns = columns.slice(leftLength, columns.length - rightLength);\n\n    const hasTopRows = topLength > 0;\n    const hasBottomRows = bottomLength > 0;\n    const hasMiddleRows = middleLength > 0;\n    const hasLeftColumns = leftLength > 0;\n    const hasRightColumns = rightLength > 0;\n    const hasCenterColumns = centerLength > 0;\n\n    const topShowTopBorder = true;\n    const topShowBottomBorder = true;\n    const bottomShowTopBorder = hasMiddleRows || !hasTopRows;\n    const bottomShowBottomBorder = true;\n    const middleShowTopBorder = !hasTopRows;\n    const middleShowBottomBorder = !hasBottomRows;\n    const leftShowLeftBorder = true;\n    const leftShowRightBorder = true;\n    const rightShowLeftBorder = hasCenterColumns || !hasLeftColumns;\n    const rightShowRightBorder = true;\n    const centerShowLeftBorder = !hasLeftColumns;\n    const centerShowRightBorder = !hasRightColumns;\n\n    const getHeight = (rows, showTopBorder, showBottomBorder) => {\n        if (rows.length === 0)\n            return 0;\n\n        const top = showTopBorder ? rows.at(0).topWithBorder : rows.at(0).top;\n        const bottom = showBottomBorder ? rows.at(-1).bottomWithBorder : rows.at(-1).bottom;\n\n        return bottom - top;\n    }\n\n    const getWidth = (columns, showLeftBorder, showRightBorder) => {\n        if (columns.length === 0)\n            return 0;\n\n        const left = showLeftBorder ? columns.at(0).leftWithBorder : columns.at(0).left;\n        const right = showRightBorder ? columns.at(-1).rightWithBorder : columns.at(-1).right;\n\n        return right - left;\n    }\n\n    const topHeight = getHeight(topRows, topShowTopBorder, topShowBottomBorder);\n    const bottomHeight = getHeight(bottomRows, bottomShowTopBorder, bottomShowBottomBorder);\n    const middleHeight = getHeight(middleRows, middleShowTopBorder, middleShowBottomBorder);\n    const leftWidth = getWidth(leftColumns, leftShowLeftBorder, leftShowRightBorder);\n    const rightWidth = getWidth(rightColumns, rightShowLeftBorder, rightShowRightBorder);\n    const centerWidth = getWidth(centerColumns, centerShowLeftBorder, centerShowRightBorder);\n\n    return {\n        top: {\n            rows: topRows,\n            showTopBorder: topShowTopBorder,\n            showBottomBorder: topShowBottomBorder,\n            height: topHeight\n        },\n        bottom: {\n            rows: bottomRows,\n            showTopBorder: bottomShowTopBorder,\n            showBottomBorder: bottomShowBottomBorder,\n            height: bottomHeight\n        },\n        middle: {\n            rows: middleRows,\n            showTopBorder: middleShowTopBorder,\n            showBottomBorder: middleShowBottomBorder,\n            height: middleHeight\n        },\n        left: {\n            columns: leftColumns,\n            showLeftBorder: leftShowLeftBorder,\n            showRightBorder: leftShowRightBorder,\n            width: leftWidth\n        },\n        right: {\n            columns: rightColumns,\n            showLeftBorder: rightShowLeftBorder,\n            showRightBorder: rightShowRightBorder,\n            width: rightWidth\n        },\n        center: {\n            columns: centerColumns,\n            showLeftBorder: centerShowLeftBorder,\n            showRightBorder: centerShowRightBorder,\n            width: centerWidth\n        }\n    };\n}",
         "// TODO: Move\nexport default function getEditedCellsAndFilters(editedCells, filters) {\n    return [...editedCells, ...filters.map(filter => ({ columnId: filter.columnId, rowId: filter.rowId, value: filter.expression }))];\n}\n",
         "import stringifyId from \"../core-utils/stringifyId.js\";\n\n// TODO: write unit tests\nexport default class Edition {\n    constructor(editedCells) {\n        this.lookup = new Map();\n\n        editedCells.forEach(cell => {\n            const rowKey = stringifyId(cell.rowId);\n            const columnKey = stringifyId(cell.columnId);\n\n            if (!this.lookup.has(rowKey))\n                this.lookup.set(rowKey, new Map());\n\n            this.lookup.get(rowKey).set(columnKey, cell.value);\n        });\n    }\n\n    hasValueByKey(rowKey, columnKey) {\n        return this.lookup.has(rowKey) && this.lookup.get(rowKey).has(columnKey);\n    }\n\n    getValueByKey(rowKey, columnKey) {\n        if (!this.hasValueByKey(rowKey, columnKey))\n            return undefined;\n\n        return this.lookup.get(rowKey).get(columnKey);\n    }\n\n    hasValueById(rowId, columnId) {\n        return this.hasValueByKey(stringifyId(rowId), stringifyId(columnId));\n    }\n\n    getValueById(rowId, columnId) {\n        return this.getValueByKey(stringifyId(rowId), stringifyId(columnId));\n    }\n}",
         "import Edition from \"../types/Edition.js\";\n\n// TODO: Move\nexport default function getEdition(editedCellsAndFilters) {\n    return new Edition(editedCellsAndFilters);\n}\n",
         "import stringifyId from \"../core-utils/stringifyId.js\";\n\nexport default class Selection {\n    constructor(selectedCells) {\n        this.lookup = new Map();\n\n        selectedCells.forEach(cell => {\n            const rowKey = stringifyId(cell.rowId);\n            const columnKey = stringifyId(cell.columnId);\n\n            if (!this.lookup.has(rowKey))\n                this.lookup.set(rowKey, new Set());\n\n            this.lookup.get(rowKey).add(columnKey);\n        });\n    }\n\n    isKeySelected(rowKey, columnKey) {\n        return this.lookup.has(rowKey) && this.lookup.get(rowKey).has(columnKey);\n    }\n\n    isIdSelected(rowId, columnId) {\n        return this.isKeySelected(stringifyId(rowId), stringifyId(columnId));\n    }\n}",
         "import Selection from \"../types/Selection.js\";\n\nexport default function getSelection(selectedCells) {\n    return new Selection(selectedCells);\n}\n",
         "export default function getInvoked(columnsOrRows, data) {\n    return typeof columnsOrRows === 'function'\n        ? columnsOrRows(data)\n        : columnsOrRows;\n}\n",
         "// TODO: Move\nexport default function getPinned(index, length, pinnedBegin, pinnedEnd) {\n    if (index < pinnedBegin)\n        return \"BEGIN\";\n    if (index >= length - pinnedEnd)\n        return \"END\";\n    return undefined;\n}\n",
         "import stringifyId from \"../core-utils/stringifyId.js\";\nimport getPinned from \"./getPinned.js\";\n\nfunction getResolved(elements, pinnedBegin, pinnedEnd) {\n    return elements.map((element, index) => {\n        const id = 'id' in element ? element.id : element.type;\n        return {\n            ...element,\n            id: id,\n            type: element.type || \"DATA\",\n            index: index,\n            key: stringifyId(id),\n            pinned: getPinned(index, elements.length, pinnedBegin, pinnedEnd),\n            header: 'header' in element ? element.header : id,\n            labels: element.labels || []\n        };\n    });\n}\n\nexport function getResolvedColumns(columns, pinnedBegin, pinnedEnd, columnWidths) {\n    const widthsLookup = new Map(columnWidths.map(({ columnId, width }) => [stringifyId(columnId), width]));\n    const resolvedColumns = getResolved(columns, pinnedBegin, pinnedEnd);\n\n    return resolvedColumns.map(column => ({\n        ...column,\n        width: widthsLookup.has(column.key)\n            ? widthsLookup.get(column.key)\n            : 'width' in column\n                ? column.width\n                : 'fit'\n    }));\n}\n\nexport function getResolvedRows(rows, pinnedBegin, pinnedEnd, rowHeights) {\n    const heightsLookup = new Map(rowHeights.map(({ rowId, height }) => [stringifyId(rowId), height]));\n    const resolvedRows = getResolved(rows, pinnedBegin, pinnedEnd);\n\n    return resolvedRows.map(row => ({\n        ...row,\n        height: heightsLookup.has(row.key)\n            ? heightsLookup.get(row.key)\n            : 'height' in row\n                ? row.height\n                : 'fit'\n    }));\n}\n",
         "import roundToPixels from \"../core-utils/roundToPixels.js\";\n\nexport function getPlacedColumns(columns, devicePixelRatio, borderWidth) {\n    let left = borderWidth;\n\n    return columns.map((column, index) => {\n        const assignedWidth = 'width' in column ? column.width : 100;\n        const width = roundToPixels(assignedWidth, devicePixelRatio);\n        const newColumn = {\n            ...column,\n            index: index,\n            width: width,\n            leftWithBorder: left - borderWidth,\n            left: left,\n            right: left + width,\n            rightWithBorder: left + width + borderWidth\n        };\n\n        left += newColumn.width + borderWidth;\n\n        return newColumn;\n    });\n}\n\nexport function getPlacedRows(rows, devicePixelRatio, borderWidth) {\n    let top = borderWidth;\n\n    return rows.map((row, index) => {\n        const assignedHeight = 'height' in row ? row.height : 20;\n        const height = roundToPixels(assignedHeight, devicePixelRatio);\n        const newRow = {\n            ...row,\n            index: index,\n            height: height,\n            topWithBorder: top - borderWidth,\n            top: top,\n            bottom: top + height,\n            bottomWithBorder: top + height + borderWidth\n        };\n\n        top += newRow.height + borderWidth;\n\n        return newRow;\n    });\n}\n",
         "const defaultFont = '12px Calibri';\nconst defaultPadding = { top: 2, right: 5, bottom: 2, left: 5 };\n\nexport { defaultFont, defaultPadding };",
         "import stringifyId from \"../core-utils/stringifyId.js\";\n\nconst typeMapping = {\n    'HEADER': ['HEADER'],\n    'FILTER': ['FILTER'],\n    'DATA': ['DATA'],\n    'CUSTOM': ['CUSTOM'],\n    'ANY': ['HEADER', 'DATA', 'FILTER', 'CUSTOM'],\n    'SPECIAL': ['HEADER', 'FILTER', 'CUSTOM'],\n    undefined: []\n};\n\nclass Lookup {\n    byKey = new Map();\n    byIndex = new Map(); // TODO: Should this be removed?\n    byLabel = new Map();\n    byType = new Map();\n}\n\nexport default class RulesLookup {\n    lookup = new Lookup();\n    hasRules = false;\n\n    addRule(column, row, rule) {\n        this.hasRules = true;\n\n        if (Array.isArray(column)) {\n            for (const c of column)\n                this.addRule(c, row, rule);\n            return;\n        }\n\n        if (Array.isArray(row)) {\n            for (const r of row)\n                this.addRule(column, r, rule);\n            return;\n        }\n\n        column = column\n            ? 'id' in column\n                ? { key: stringifyId(column.id) }\n                : column\n            : { type: 'DATA' };\n        row = row\n            ? 'id' in row\n                ? { key: stringifyId(row.id) }\n                : row\n            : { type: 'DATA' };\n\n        function addRowRule(lookup, key) {\n            if (!lookup.has(key))\n                lookup.set(key, []);\n\n            lookup.get(key).push(rule);\n        }\n\n        function addColumnRule(lookup, key) {\n            if (!lookup.has(key))\n                lookup.set(key, new Lookup());\n\n            if ('key' in row)\n                addRowRule(lookup.get(key).byKey, row.key);\n            if ('index' in row)\n                addRowRule(lookup.get(key).byIndex, row.index);\n            if ('label' in row)\n                addRowRule(lookup.get(key).byLabel, row.label);\n            for (const type of typeMapping[row.type])\n                addRowRule(lookup.get(key).byType, type);\n        }\n\n        if ('key' in column)\n            addColumnRule(this.lookup.byKey, column.key);\n        if ('index' in column)\n            addColumnRule(this.lookup.byIndex, column.index);\n        if ('label' in column)\n            addColumnRule(this.lookup.byLabel, column.label);\n        for (const type of typeMapping[column.type])\n            addColumnRule(this.lookup.byType, type);\n    }\n\n    getRules(column, row) {\n        const rules = [];\n\n        if (!this.hasRules)\n            return rules;\n\n        function gatherRules(newRules) {\n            for (const rule of newRules)\n                rules.push(rule);\n        }\n\n        function gatherRowRules(lookup) {\n            if (lookup.byKey.has(row.key))\n                gatherRules(lookup.byKey.get(row.key));\n            if (lookup.byIndex.has(row.index))\n                gatherRules(lookup.byIndex.get(row.index));\n            if (lookup.byType.has(row.type))\n                gatherRules(lookup.byType.get(row.type));\n            for (const label of row.labels) {\n                if (lookup.byLabel.has(label))\n                    gatherRules(lookup.byLabel.get(label));\n            }\n        }\n\n        if (this.lookup.byKey.has(column.key))\n            gatherRowRules(this.lookup.byKey.get(column.key));\n        if (this.lookup.byIndex.has(column.index))\n            gatherRowRules(this.lookup.byIndex.get(column.index));\n        if (this.lookup.byType.has(column.type))\n            gatherRowRules(this.lookup.byType.get(column.type));\n        for (const label of column.labels) {\n            if (this.lookup.byLabel.has(label))\n                gatherRowRules(this.lookup.byLabel.get(label));\n        }\n\n        return rules;\n    }\n};",
-        "import { defaultFont, defaultPadding } from \"../core-utils/defaults.js\";\nimport RulesLookup from \"./RulesLookup.js\";\n\nconst borderTypes = ['borderTop', 'borderRight', 'borderBottom', 'borderLeft'];\n// TODO: better handle default validate for toggle edit\nconst defaultEdit = { validate: () => true, parse: ({ string }) => string };\n\n// TODO: Don't recreate styles if they haven't changed\nfunction indexBorders(style, index) {\n    const newStyle = { ...style };\n\n    if ('border' in newStyle) {\n        for (const borderType of borderTypes)\n            newStyle[borderType] = newStyle.border;\n        delete newStyle.border;\n    }\n\n    for (const borderType of borderTypes)\n        if (borderType in newStyle)\n            newStyle[borderType] = { ...newStyle[borderType], index };\n\n    return newStyle;\n}\n\nfunction getText(context) {\n    if ('text' in context)\n        return `${context.text}`;\n    if ('newValue' in context)\n        return `${context.newValue}`;\n    if (context.value !== undefined)\n        return `${context.value}`;\n    return '';\n}\n\nfunction getEdit(rule, context) {\n    if (rule.edit === false)\n        return undefined;\n    if (rule.edit === true)\n        return 'edit' in context ? context.edit : defaultEdit;\n    if ('edit' in context)\n        return { ...context.edit, ...rule.edit };\n    return { ...defaultEdit, ...rule.edit };\n}\n\n// TODO: Rename to FormatResolver\n// TODO: Optimize by not searching using keys that don't have correlated type rules\n// TODO: Accept both a function and an object as a style (where the object is a resolved style)\n// TODO: Consider removing index from the lookup\nexport default class FormattingRules {\n    constructor(rules) {\n        this.rulesLookup = new RulesLookup();\n\n        for (const [index, rule] of rules.entries()) {\n            const entry = { index };\n\n            if ('condition' in rule)\n                entry.condition = rule.condition;\n            if ('style' in rule)\n                entry.style = typeof rule.style === 'function' ? rule.style : () => rule.style;\n            if ('value' in rule)\n                entry.value = typeof rule.value === 'function' ? rule.value : () => rule.value;\n            if ('text' in rule)\n                entry.text = typeof rule.text === 'function' ? rule.text : () => rule.text;\n            if ('font' in rule)\n                entry.font = typeof rule.font === 'function' ? rule.font : () => rule.font;\n            if ('padding' in rule)\n                entry.padding = typeof rule.padding === 'function' ? rule.padding : () => rule.padding;\n            if ('edit' in rule)\n                entry.edit = rule.edit;\n            if ('draw' in rule)\n                entry.draw = rule.draw;\n\n            this.rulesLookup.addRule(rule.column, rule.row, entry);\n        }\n    }\n\n    resolve(data, rows, columns, row, column, edition) {\n        const rules = this.rulesLookup\n            .getRules(column, row)\n            .sort((a, b) => a.index - b.index)\n            .filter((value, index, array) => value.index !== array[index - 1]?.index);\n\n        let context = { data, rows, columns, row, column };\n        let style = {};\n        let draw = undefined;\n        let visible = true;\n        let padding = defaultPadding;\n        let font = defaultFont;\n\n        if (edition.hasValueByKey(row.key, column.key))\n            context = { ...context, newValue: edition.getValueByKey(row.key, column.key) };\n\n        for (const rule of rules) {\n            if ('condition' in rule && !rule.condition(context))\n                continue;\n\n            // TODO: Don't actually add things like `edit` to the context\n            if ('value' in rule)\n                context = { ...context, value: rule.value(context) };\n            if ('style' in rule)\n                style = { ...style, ...indexBorders(rule.style(context), rule.index) };\n            if ('text' in rule)\n                context = { ...context, text: rule.text(context) };\n            if ('font' in rule)\n                font = rule.font(context);\n            if ('padding' in rule)\n                padding = { ...padding, ...rule.padding(context) };\n            if ('edit' in rule)\n                context = { ...context, edit: getEdit(rule, context) };\n            if ('draw' in rule) {\n                const currentContext = context;\n                draw = (ctx) => rule.draw({ ...currentContext, ctx });\n            }\n\n            // TODO: Add StopPropagation\n        }\n\n        const text = getText(context);\n        const result = {\n            style,\n            visible,\n            text,\n            padding,\n            font\n        };\n\n        if ('value' in context)\n            result.value = context.value;\n        if ('edit' in context && context.edit !== undefined)\n            result.edit = context.edit;\n        if (draw !== undefined)\n            result.draw = draw;\n\n        return result;\n    }\n}",
-        "import FormattingRules from \"../types/FormattingRules.js\";\n\nexport default function getFormattingRules(dataFormatting) {\n    return new FormattingRules(dataFormatting);\n}\n",
+        "import { defaultFont, defaultPadding } from \"../core-utils/defaults.js\";\nimport RulesLookup from \"./RulesLookup.js\";\n\nconst borderTypes = ['borderTop', 'borderRight', 'borderBottom', 'borderLeft'];\n// TODO: better handle default validate for toggle edit\nconst defaultEdit = { validate: () => true, parse: ({ string }) => string };\n\n// TODO: Don't recreate styles if they haven't changed\nfunction indexBorders(style, index) {\n    const newStyle = { ...style };\n\n    if ('border' in newStyle) {\n        for (const borderType of borderTypes)\n            newStyle[borderType] = newStyle.border;\n        delete newStyle.border;\n    }\n\n    for (const borderType of borderTypes)\n        if (borderType in newStyle)\n            newStyle[borderType] = { ...newStyle[borderType], index };\n\n    return newStyle;\n}\n\nfunction getText(context) {\n    if ('text' in context)\n        return `${context.text}`;\n    if ('newValue' in context)\n        return `${context.newValue}`;\n    if (context.value !== undefined)\n        return `${context.value}`;\n    return '';\n}\n\nfunction getEdit(rule, context) {\n    if (rule.edit === false)\n        return undefined;\n    if (rule.edit === true)\n        return 'edit' in context ? context.edit : defaultEdit;\n    if ('edit' in context)\n        return { ...context.edit, ...rule.edit };\n    return { ...defaultEdit, ...rule.edit };\n}\n\n// TODO: Rename to FormatResolver\n// TODO: Optimize by not searching using keys that don't have correlated type rules\n// TODO: Accept both a function and an object as a style (where the object is a resolved style)\n// TODO: Consider removing index from the lookup\nexport default class FormattingRules {\n    constructor(rules) {\n        this.rulesLookup = new RulesLookup();\n\n        for (const [index, rule] of rules.entries()) {\n            const entry = { index };\n\n            // TODO: Mark which rules are actually present and only check those in resolve\n            if ('condition' in rule)\n                entry.condition = rule.condition;\n            if ('style' in rule)\n                entry.style = typeof rule.style === 'function' ? rule.style : () => rule.style;\n            if ('value' in rule)\n                entry.value = typeof rule.value === 'function' ? rule.value : () => rule.value;\n            if ('text' in rule)\n                entry.text = typeof rule.text === 'function' ? rule.text : () => rule.text;\n            if ('font' in rule)\n                entry.font = typeof rule.font === 'function' ? rule.font : () => rule.font;\n            if ('padding' in rule)\n                entry.padding = typeof rule.padding === 'function' ? rule.padding : () => rule.padding;\n            if ('edit' in rule)\n                entry.edit = rule.edit;\n            if ('tooltip' in rule)\n                entry.tooltip = typeof rule.tooltip === 'function' ? rule.tooltip : () => rule.tooltip;\n            if ('draw' in rule)\n                entry.draw = rule.draw;\n\n            this.rulesLookup.addRule(rule.column, rule.row, entry);\n        }\n    }\n\n    resolve(data, rows, columns, row, column, edition) {\n        const rules = this.rulesLookup\n            .getRules(column, row)\n            .sort((a, b) => a.index - b.index)\n            .filter((value, index, array) => value.index !== array[index - 1]?.index);\n\n        let context = { data, rows, columns, row, column };\n        let style = {};\n        let draw = undefined;\n        let visible = true;\n        let padding = defaultPadding;\n        let font = defaultFont;\n        let tooltip = undefined;\n\n        if (edition.hasValueByKey(row.key, column.key))\n            context = { ...context, newValue: edition.getValueByKey(row.key, column.key) };\n\n        for (const rule of rules) {\n            if ('condition' in rule && !rule.condition(context))\n                continue;\n\n            // TODO: Don't actually add things like `edit` to the context\n            if ('value' in rule)\n                context = { ...context, value: rule.value(context) };\n            if ('style' in rule)\n                style = { ...style, ...indexBorders(rule.style(context), rule.index) };\n            if ('text' in rule)\n                context = { ...context, text: rule.text(context) };\n            if ('font' in rule)\n                font = rule.font(context);\n            if ('padding' in rule)\n                padding = { ...padding, ...rule.padding(context) };\n            if ('edit' in rule)\n                context = { ...context, edit: getEdit(rule, context) };\n            if ('tooltip' in rule)\n                tooltip = rule.tooltip(context);\n            if ('draw' in rule) {\n                const currentContext = context;\n                draw = (ctx) => rule.draw({ ...currentContext, ctx });\n            }\n\n            // TODO: Add StopPropagation\n        }\n\n        const text = getText(context);\n        const result = {\n            style,\n            visible,\n            text,\n            padding,\n            font\n        };\n\n        if ('value' in context)\n            result.value = context.value;\n        if ('edit' in context && context.edit !== undefined)\n            result.edit = context.edit;\n        if (tooltip !== undefined)\n            result.tooltip = tooltip;\n        if (draw !== undefined)\n            result.draw = draw;\n\n        return result;\n    }\n}",
+        "import FormattingRules from \"../types/FormattingRules.js\";\n\nexport default function getFormattingRules(formatting) {\n    return new FormattingRules(formatting);\n}\n",
         "export default class FormatResolver {\n    constructor(formattingRules, data, rows, columns, edition) {\n        this.formattingRules = formattingRules;\n        this.data = data;\n        this.rows = rows;\n        this.columns = columns;\n        this.edition = edition;\n    }\n\n    resolve(row, column) {\n        return this.formattingRules.resolve(\n            this.data,\n            this.rows,\n            this.columns,\n            row,\n            column,\n            this.edition);\n    }\n}",
         "import FormatResolver from \"../types/FormatResolver.js\";\n\nexport default function getFormatResolver(formattingRules, data, rows, columns, edition) {\n    return new FormatResolver(formattingRules, data, rows, columns, edition);\n}\n",
         "import stringifyId from \"../core-utils/stringifyId.js\";\n\nfunction getFilterLookup(filters, primaryKey, secondaryKey) {\n    const filterLookup = new Map();\n    for (const cell of filters) {\n        const primary = stringifyId(cell[primaryKey]);\n        const secondary = stringifyId(cell[secondaryKey]);\n\n        if (!filterLookup.has(primary))\n            filterLookup.set(primary, new Map());\n\n        filterLookup.get(primary).set(secondary, cell.expression);\n    }\n    return filterLookup;\n}\n\nexport function getFilteredRows(filters, filteringRules, formattingRules, data, rows, columns, edition) {\n    if (filters.length === 0)\n        return rows;\n\n    const filterLookup = getFilterLookup(filters, 'columnId', 'rowId');\n    const filteredColumns = columns.filter(column => column.type !== 'FILTER' && filterLookup.has(column.key));\n\n    if (filteredColumns.length === 0)\n        return rows;\n\n    return rows.filter(row => {\n        for (const column of filteredColumns) {\n            const cell = formattingRules.resolve(data, rows, columns, row, column, edition);\n            const columnFilters = filterLookup.get(column.key);\n            const visible = filteringRules.resolve(data, rows, columns, row, column, cell.value, cell.text, columnFilters);\n\n            if (!visible)\n                return false;\n        }\n        return true;\n    });\n}\n\nexport function getFilteredColumns(filters, filteringRules, formattingRules, data, rows, columns, edition) {\n    if (filters.length === 0)\n        return columns;\n\n    const filterLookup = getFilterLookup(filters, 'rowId', 'columnId');\n    const filteredRows = rows.filter(row => row.type !== 'FILTER' && filterLookup.has(row.key));\n\n    if (filteredRows.length === 0)\n        return columns;\n\n    return columns.filter(column => {\n        for (const row of filteredRows) {\n            const cell = formattingRules.resolve(data, rows, columns, row, column, edition);\n            const rowFilters = filterLookup.get(row.key);\n            const visible = filteringRules.resolve(data, rows, columns, row, column, cell.value, cell.text, rowFilters);\n\n            if (!visible)\n                return false;\n        }\n        return true;\n    });\n}",
         "export default function getFixedSize(top, bottom, left, right) {\n    return {\n        top: top,\n        bottom: bottom,\n        left: left,\n        right: right\n    };\n}\n",
         "export default function getTotalSize(columns, rows) {\n    return {\n        width: columns.length ? columns.at(-1).rightWithBorder : 0,\n        height: rows.length ? rows.at(-1).bottomWithBorder : 0\n    };\n}\n",
         "import { defaultFont } from \"../core-utils/defaults.js\";\n\nexport default class TextResolver {\n    constructor() {\n        this.canvas = document.createElement('canvas');\n        this.context = this.canvas.getContext('2d');\n        this.fontMetrics = new Map();\n    }\n\n    measureWidth(text, font) {\n        if (!text)\n            return 0;\n\n        const ctx = this.context;\n        ctx.font = font || defaultFont;\n        const textMetrics = ctx.measureText(text);\n\n        return textMetrics.width;\n    }\n\n    measureHeight(text, font) {\n        let lines = 1;\n        for (const char of text) {\n            if (char === '\\n')\n                lines++;\n        }\n\n        return lines * this.getFontMetrics(font).height;\n    }\n\n    getFontMetrics(font) {\n        const key = font;\n\n        if (this.fontMetrics.has(key))\n            return this.fontMetrics.get(key);\n\n        const ctx = this.context;\n\n        // TODO: Set other font properties\n        ctx.font = font || defaultFont;\n\n        const textMetrics = ctx.measureText('X');\n\n        const middle = (textMetrics.actualBoundingBoxDescent - textMetrics.actualBoundingBoxAscent) / 2;\n        const topOffset = middle + textMetrics.fontBoundingBoxAscent;\n        const bottomOffset = textMetrics.fontBoundingBoxDescent - middle;\n        const height = textMetrics.fontBoundingBoxAscent + textMetrics.fontBoundingBoxDescent;\n\n        const fontMetrics = {\n            topOffset: topOffset,\n            middle: -middle,\n            bottomOffset: bottomOffset,\n            height: height\n        };\n\n        this.fontMetrics.set(key, fontMetrics);\n\n        return fontMetrics;\n    }\n}",
         "import TextResolver from \"../types/TextResolver.js\";\n\nexport default function getTextResolver() {\n    return new TextResolver();\n}\n",
         "export function contains(bounds, rect) {\n    return (\n        rect.top >= bounds.top &&\n        rect.left >= bounds.left &&\n        rect.top + rect.height <= bounds.top + bounds.height &&\n        rect.left + rect.width <= bounds.left + bounds.width\n    );\n}\n\nexport function clip(bounds, rect) {\n    const newRect = {\n        top: Math.max(bounds.top, rect.top),\n        left: Math.max(bounds.left, rect.left),\n        width: Math.min(bounds.left + bounds.width, rect.left + rect.width) - Math.max(bounds.left, rect.left),\n        height: Math.min(bounds.top + bounds.height, rect.top + rect.height) - Math.max(bounds.top, rect.top)\n    };\n\n    if (newRect.width >= 0 && newRect.height >= 0)\n        return newRect;\n\n    return {\n        top: bounds.top,\n        left: bounds.left,\n        width: 0,\n        height: 0\n    }\n}\n\nexport function expand(rect, margin) {\n    return {\n        top: rect.top - margin,\n        left: rect.left - margin,\n        width: rect.width + margin * 2,\n        height: rect.height + margin * 2\n    };\n}\n\nexport function area(rect) {\n    return rect.width * rect.height;\n}\n\nexport function subtract(rect, margin) {\n    return {\n        top: rect.top,\n        left: rect.left,\n        width: Math.max(0, rect.width - margin.left - margin.right),\n        height: Math.max(0, rect.height - margin.top - margin.bottom)\n    };\n}",
         "import { area, clip, contains, expand, subtract } from \"../core-utils/rect.js\";\n\nconst requiredMargin = 200;\nconst preloadedMargin = 400;\nconst emptyRect = {\n    left: 0,\n    top: 0,\n    width: 0,\n    height: 0\n};\n\nexport default function getScrollRect(previous, totalSize, fixedSize, element) {\n    // TODO: Is it optimal to use getBoundingClientRect()?\n    const size = {\n        width: element.getBoundingClientRect().width,\n        height: element.getBoundingClientRect().height\n    };\n    const scrollOffset = {\n        left: element.scrollLeft,\n        top: element.scrollTop\n    };\n\n    const prevScrollRect = previous || emptyRect;\n\n    const totalRect = { left: 0, top: 0, ...totalSize };\n    const bounds = subtract(totalRect, fixedSize);\n    const scrollRect = subtract({ ...scrollOffset, ...size }, fixedSize);\n    const requiredScrollRect = clip(bounds, expand(scrollRect, requiredMargin));\n    const preloadedScrollRect = clip(bounds, expand(scrollRect, preloadedMargin));\n\n    if (!contains(bounds, prevScrollRect))\n        return preloadedScrollRect;\n\n    if (!contains(prevScrollRect, requiredScrollRect))\n        return preloadedScrollRect;\n\n    if (area(prevScrollRect) > 2 * area(preloadedScrollRect))\n        return preloadedScrollRect;\n\n    return prevScrollRect;\n}\n",
         "export default function getInternalPosition(element, position, fixedSize, totalSize) {\n  // TODO: sometimes mousePosition is outside of bounds and it crashes the click events\n  const x = position.x;\n  const y = position.y;\n\n  const scrollOffset = {\n    left: element.scrollLeft,\n    top: element.scrollTop\n  };\n\n  const clientSize = {\n    width: element.clientWidth,\n    height: element.clientHeight\n  };\n\n  return {\n    x: x <= fixedSize.left\n      ? x\n      : x >= clientSize.width // TODO: This will not work for resizing columns pinned to the right\n        ? x + scrollOffset.left\n        : x >= clientSize.width - fixedSize.right\n          ? totalSize.width - clientSize.width + x\n          : x + scrollOffset.left,\n    y: y <= fixedSize.top\n      ? y\n      : y >= clientSize.height // TODO: This will not work for resizing rows pinned to the bottom\n        ? y + scrollOffset.top\n        : y >= clientSize.height - fixedSize.bottom\n          ? totalSize.height - clientSize.height + y\n          : y + scrollOffset.top\n  };\n}",
         "export default function getLookup(elements) {\n    return elements.reduce((lookup, element) => lookup.set(element.key, element), new Map());\n}\n",
         "import stringifyId from \"../core-utils/stringifyId.js\";\n\nexport default function getHighlightedCells(isMouseDown, isResizing, focusedCell, hoveredCell, columns, rows, columnLookup, rowLookup) {\n    if (!isMouseDown)\n        return [];\n    if (isResizing)\n        return [];\n    if (!hoveredCell)\n        return [];\n    if (!focusedCell)\n        return [];\n\n    const focusedColumnKey = stringifyId(focusedCell.columnId);\n    const focusedRowKey = stringifyId(focusedCell.rowId);\n    const hoveredColumnKey = stringifyId(hoveredCell.columnId);\n    const hoveredRowKey = stringifyId(hoveredCell.rowId);\n\n    if (!columnLookup.has(focusedColumnKey))\n        return [];\n    if (!rowLookup.has(focusedRowKey))\n        return [];\n    if (!columnLookup.has(hoveredColumnKey))\n        return [];\n    if (!rowLookup.has(hoveredRowKey))\n        return [];\n\n    const minColumnIndex = Math.min(columnLookup.get(focusedColumnKey).index, columnLookup.get(hoveredColumnKey).index);\n    const maxColumnIndex = Math.max(columnLookup.get(focusedColumnKey).index, columnLookup.get(hoveredColumnKey).index);\n    const minRowIndex = Math.min(rowLookup.get(focusedRowKey).index, rowLookup.get(hoveredRowKey).index);\n    const maxRowIndex = Math.max(rowLookup.get(focusedRowKey).index, rowLookup.get(hoveredRowKey).index);\n\n    return columns.slice(minColumnIndex, maxColumnIndex + 1).flatMap(column => {\n        return rows.slice(minRowIndex, maxRowIndex + 1).map(row => {\n            return {\n                rowId: row.id,\n                columnId: column.id\n            };\n        });\n    });\n}\n",
         "function getVerticalSection(row) {\n    if (row.pinned === \"BEGIN\")\n        return \"top\";\n    if (row.pinned === \"END\")\n        return \"bottom\";\n    return \"middle\";\n}\n\nfunction getHorizontalSection(column) {\n    if (column.pinned === \"BEGIN\")\n        return \"left\";\n    if (column.pinned === \"END\")\n        return \"right\";\n    return \"center\";\n}\n\nexport default function getCellSection(column, row) {\n    const verticalSection = getVerticalSection(row);\n    const horizontalSection = getHorizontalSection(column);\n\n    return `${verticalSection}-${horizontalSection}`;\n}",
-        "import stringifyId from \"../core-utils/stringifyId.js\";\nimport getCellSection from \"./getCellSection.js\";\n\nexport default function getInputPlacement(editableCells, focusedCell, columnLookup, rowLookup, sections) {\n    if (!focusedCell)\n        return null;\n\n    const focusedColumnKey = stringifyId(focusedCell.columnId);\n    const focusedRowKey = stringifyId(focusedCell.rowId);\n\n    if (!columnLookup.has(focusedColumnKey))\n        return null;\n    if (!rowLookup.has(focusedRowKey))\n        return null;\n\n    const column = columnLookup.get(focusedColumnKey);\n    const row = rowLookup.get(focusedRowKey);\n\n    if (editableCells.length === 0)\n        return null;\n\n    const position = {\n        width: column.width,\n        height: row.height,\n        section: getCellSection(column, row)\n    };\n\n    switch (row.pinned) {\n        case \"BEGIN\":\n            position.top = row.top;\n            break;\n        case \"END\":\n            position.bottom = sections.top.height + sections.middle.height + sections.bottom.height - row.top - row.height;\n            break;\n        default:\n            position.marginTop = row.top - sections.top.height;\n    }\n\n    switch (column.pinned) {\n        case \"BEGIN\":\n            position.left = column.left;\n            break;\n        case \"END\":\n            position.right = sections.left.width + sections.center.width + sections.right.width - column.left - column.width;\n            break;\n        default:\n            position.marginLeft = column.left - sections.left.width;\n    }\n\n    return position;\n}\n",
+        "import stringifyId from \"../core-utils/stringifyId.js\";\nimport getCellSection from \"./getCellSection.js\";\n\nexport default function getInputPlacement(cell, columnLookup, rowLookup, sections) {\n    if (!cell)\n        return null;\n\n    const columnKey = stringifyId(cell.columnId);\n    const rowKey = stringifyId(cell.rowId);\n\n    if (!columnLookup.has(columnKey))\n        return null;\n    if (!rowLookup.has(rowKey))\n        return null;\n\n    const column = columnLookup.get(columnKey);\n    const row = rowLookup.get(rowKey);\n\n    const position = {\n        width: column.width,\n        height: row.height,\n        section: getCellSection(column, row)\n    };\n\n    switch (row.pinned) {\n        case \"BEGIN\":\n            position.top = row.top;\n            break;\n        case \"END\":\n            position.bottom = sections.top.height + sections.middle.height + sections.bottom.height - row.top - row.height;\n            break;\n        default:\n            position.marginTop = row.top - sections.top.height;\n    }\n\n    switch (column.pinned) {\n        case \"BEGIN\":\n            position.left = column.left;\n            break;\n        case \"END\":\n            position.right = sections.left.width + sections.center.width + sections.right.width - column.left - column.width;\n            break;\n        default:\n            position.marginLeft = column.left - sections.left.width;\n    }\n\n    return position;\n}\n",
+        "import getCellPlacement from \"./getCellPlacement.js\";\n\nexport default function getInputPlacement(editableCells, focusedCell, columnLookup, rowLookup, sections) {\n    if (editableCells.length === 0)\n        return null;\n\n    return getCellPlacement(focusedCell, columnLookup, rowLookup, sections);\n}\n",
         "export default function getIsTextValid(text, editableCells) {\n    return editableCells.every(cell => cell.edit.validate({ string: text }));\n}\n",
         "function getDefaultIds(elements) {\n    if (!Array.isArray(elements))\n        return Object.keys(elements);\n\n    return elements.map((_, index) => index);\n}\n\nfunction getDefaultRowIds(data) {\n    return getDefaultIds(data);\n}\n\nfunction getDefaultColumnIds(data) {\n    const keys = new Set();\n\n    if (Array.isArray(data)) {\n        for (const element of data) {\n            for (const id of getDefaultIds(element))\n                keys.add(id);\n        }\n    } else {\n        for (const key in data) {\n            for (const id of getDefaultIds(data[key]))\n                keys.add(id);\n        }\n    }\n\n    return [...keys];\n}\n\nexport function getUnfoldedColumns(columns, data) {\n    const hasDataBlocks = columns.some(column => column.type === 'DATA-BLOCK');\n\n    if (!hasDataBlocks)\n        return columns;\n\n    const unfoldedColumns = [];\n\n    for (const column of columns) {\n        if (column.type === 'DATA-BLOCK') {\n            const ids = 'selector' in column\n                ? column.selector(data)\n                : getDefaultColumnIds(data);\n\n            for (const id of ids) {\n                unfoldedColumns.push({\n                    ...column,\n                    id,\n                    type: 'DATA'\n                });\n            }\n        } else {\n            unfoldedColumns.push(column);\n        }\n    }\n\n    return unfoldedColumns;\n}\n\nexport function getUnfoldedRows(rows, data) {\n    const hasDataBlocks = rows.some(row => row.type === 'DATA-BLOCK');\n\n    if (!hasDataBlocks)\n        return rows;\n\n    const unfoldedRows = [];\n\n    for (const row of rows) {\n        if (row.type === 'DATA-BLOCK') {\n            const ids = 'selector' in row\n                ? row.selector(data)\n                : getDefaultRowIds(data);\n\n            for (const id of ids) {\n                unfoldedRows.push({\n                    ...row,\n                    id,\n                    type: 'DATA'\n                });\n            }\n        } else {\n            unfoldedRows.push(row);\n        }\n    }\n\n    return unfoldedRows;\n}",
         "import stringifyId from \"../core-utils/stringifyId.js\";\nimport RulesLookup from \"./RulesLookup.js\";\n\nconst defaultCondition = ({ text, expression }) => text.includes(expression);\n\nexport default class FilteringRules {\n    constructor(rules) {\n        this.rulesLookup = new RulesLookup();\n\n        for (const rule of rules) {\n            const entry = {\n                by: stringifyId('by' in rule ? rule.by : 'FILTER'),\n                condition: rule.condition || defaultCondition\n            };\n\n            this.rulesLookup.addRule(rule.column, rule.row, entry);\n        }\n    }\n\n    resolve(data, rows, columns, row, column, value, text, filterLookup) {\n        const rules = this.rulesLookup.getRules(column, row);\n\n        if (rules.length === 0) {\n            if (row.type !== 'DATA')\n                return true;\n            if (column.type !== 'DATA')\n                return true;\n            if (!filterLookup.has('\"FILTER\"'))\n                return true;\n\n            return defaultCondition({ text, expression: filterLookup.get('\"FILTER\"') });\n        }\n\n        let context = { data, rows, columns, row, column, value, text };\n\n        for (const rule of rules) {\n            if (!filterLookup.has(rule.by))\n                continue;\n\n            const filterContext = { ...context, expression: filterLookup.get(rule.by) };\n\n            if (!rule.condition(filterContext))\n                return false;\n        }\n\n        return true;\n    }\n}",
         "import FilteringRules from \"../types/FilteringRules.js\";\n\nexport default function getFilteringRules(filtering) {\n    return new FilteringRules(filtering);\n}",
         "import getReducedFormatting from \"./getReducedFormatting.js\";\n\nexport default function getFilterFormatting(formatting) {\n    return getReducedFormatting(formatting, ['value', 'text']);\n}",
         "import getReducedFormatting from \"./getReducedFormatting.js\";\n\nexport default function getMeasureFormatting(formatting) {\n    return getReducedFormatting(formatting, ['value', 'text', 'font', 'padding']);\n}",
         "import { defaultPadding } from \"../core-utils/defaults.js\";\n\n// TODO: add expand and expand-data\n\nexport function getMeasuredColumns(columns, rows, textResolver, formatResolver, measuringCache, presentKeys) {\n    if (columns.every(column => typeof column.width === 'number'))\n        return columns;\n\n    const measureColumn = column => {\n        const requestedWidth = column.width;\n\n        if (typeof requestedWidth === 'number')\n            return requestedWidth;\n\n        if (measuringCache.has(column.key)) {\n            const cached = measuringCache.get(column.key);\n\n            if (requestedWidth === 'fit-once' && !cached.dataOnly)\n                return cached.width;\n            if (requestedWidth === 'fit-data-once' && cached.dataOnly)\n                return cached.width;\n        }\n\n        let width = 0;\n        for (const row of rows) {\n            if (row.type !== 'DATA' && requestedWidth === 'fit-data-once')\n                continue;\n            if (row.type !== 'DATA' && requestedWidth === 'fit-data')\n                continue;\n\n            const cell = formatResolver.resolve(row, column);\n            const text = cell.text;\n            const font = cell.font;\n            const padding = cell.padding.left + cell.padding.right;\n\n            const cellWidth = textResolver.measureWidth(text, font) + padding;\n\n            width = Math.max(width, cellWidth);\n        }\n\n        measuringCache.set(column.key, {\n            width,\n            dataOnly: requestedWidth === 'fit-data-once'\n        });\n\n        return width;\n    }\n\n    for (const key of measuringCache.keys()) {\n        if (!presentKeys.has(key))\n            measuringCache.delete(key);\n    }\n\n    return columns.map(column => ({\n        ...column,\n        width: measureColumn(column)\n    }));\n}\n\nexport function getMeasuredRows(columns, rows, textResolver, formatResolver, measuringCache, presentKeys) {\n    if (rows.every(row => typeof row.height === 'number'))\n        return rows;\n\n    const measureRow = row => {\n        const requestedHeight = row.height;\n\n        if (typeof requestedHeight === 'number')\n            return requestedHeight;\n\n        if (measuringCache.has(row.key)) {\n            const cached = measuringCache.get(row.key);\n\n            if (requestedHeight === 'fit-once' && !cached.dataOnly)\n                return cached.height;\n            if (requestedHeight === 'fit-data-once' && cached.dataOnly)\n                return cached.height;\n        }\n\n        let height = 0;\n        for (const column of columns) {\n            if (column.type !== 'DATA' && requestedHeight === 'fit-data-once')\n                continue;\n            if (column.type !== 'DATA' && requestedHeight === 'fit-data')\n                continue;\n\n            const cell = formatResolver.resolve(row, column);\n            const text = cell.text;\n            const font = cell.font;\n            const padding = cell.padding.top + cell.padding.bottom;\n\n            const cellHeight = textResolver.measureHeight(text, font) + padding;\n\n            height = Math.max(height, cellHeight);\n        }\n\n        measuringCache.set(row.key, {\n            height,\n            dataOnly: requestedHeight === 'fit-data-once'\n        });\n\n        return height;\n    }\n\n    for (const key of measuringCache.keys()) {\n        if (!presentKeys.has(key))\n            measuringCache.delete(key);\n    }\n\n    return rows.map(row => ({\n        ...row,\n        height: measureRow(row)\n    }));\n}",
@@ -877,28 +898,31 @@
         "import RulesLookup from \"./RulesLookup.js\";\nimport stringifyId from \"../core-utils/stringifyId.js\";\n\nfunction defaultComparatorAsc(lhs, rhs) {\n    if (lhs.value == undefined)\n        return false;\n    if (rhs.value == undefined)\n        return true;\n    return lhs.value < rhs.value;\n}\n\nfunction defaultComparatorDesc(lhs, rhs) {\n    if (lhs.value == undefined)\n        return false;\n    if (rhs.value == undefined)\n        return true;\n    return lhs.value > rhs.value;\n}\n\nexport default class SortingRules {\n    constructor(rules) {\n        this.rulesLookup = new RulesLookup();\n\n        for (const rule of rules) {\n            const comparatorAsc = rule.comparator\n                ? (lhs, rhs) => rule.comparator(lhs, rhs)\n                : (lhs, rhs) => defaultComparatorAsc(lhs, rhs);\n            const comparatorDesc = rule.comparator\n                ? (lhs, rhs) => !rule.comparator(lhs, rhs)\n                : (lhs, rhs) => defaultComparatorDesc(lhs, rhs);\n\n            const entry = {\n                by: stringifyId('by' in rule ? rule.by : 'HEADER'),\n                comparatorAsc: comparatorAsc,\n                comparatorDesc: comparatorDesc\n            };\n\n            this.rulesLookup.addRule(rule.column, rule.row, entry);\n        }\n    }\n\n    resolve(column, row, sortByLookup) {\n        const rules = this.rulesLookup.getRules(column, row);\n\n        if (rules.length === 0) {\n            if (row.type !== 'DATA')\n                return null;\n            if (column.type !== 'DATA')\n                return null;\n            if (!sortByLookup.has('\"HEADER\"'))\n                return null;\n\n            return sortByLookup.get('\"HEADER\"') === 'ASC'\n                ? defaultComparatorAsc\n                : defaultComparatorDesc;\n        }\n\n        if (rules.length > 1)\n            throw new Error('Multiple sorting rules for the same cell'); // TODO: add more context\n\n        const rule = rules[0];\n\n        if (!sortByLookup.has(rule.by))\n            return null;\n\n        return sortByLookup.get(rule.by) === 'ASC'\n            ? rule.comparatorAsc\n            : rule.comparatorDesc;\n    }\n}",
         "import SortingRules from \"../types/SortingRules.js\";\n\nexport default function getSortingRules(sorting) {\n    return new SortingRules(sorting);\n}",
         "import stringifyId from \"../core-utils/stringifyId.js\";\n\nfunction getSortByLookup(sortBy, primaryKey, secondaryKey) {\n    const sortByLookup = new Map();\n    for (const cell of sortBy) {\n        const primary = stringifyId(cell[primaryKey]);\n        const secondary = stringifyId(cell[secondaryKey]);\n\n        if (!sortByLookup.has(primary))\n            sortByLookup.set(primary, new Map());\n\n        sortByLookup.get(primary).set(secondary, cell.direction);\n    }\n    return sortByLookup;\n}\n\nfunction flush(temp, result) {\n    temp.sort((lhs, rhs) => {\n        const result = lhs.comparator(lhs.cell, rhs.cell);\n        if (typeof result === 'number')\n            return result;\n        return result ? -1 : 1;\n    });\n    result.push(...temp.map(entry => entry.entity));\n    temp.length = 0;\n}\n\nexport function getSortedRows(sortBy, sortingRules, formattingRules, data, rows, columns, edition) {\n    if (sortBy.length === 0)\n        return rows;\n\n    const sortByLookup = getSortByLookup(sortBy, 'columnId', 'rowId');\n    const columnLookup = new Map(columns.map(column => [column.key, column]));\n    const sortedColumns = sortBy\n        .map(cell => stringifyId(cell.columnId))\n        .filter(key => columnLookup.has(key))\n        .map(key => columnLookup.get(key))\n        .reverse();\n\n    if (sortedColumns.length === 0)\n        return rows;\n\n    for (const column of sortedColumns) {\n        const result = [];\n        const temp = [];\n\n        for (const row of rows) {\n            const comparator = sortingRules.resolve(column, row, sortByLookup.get(column.key));\n\n            if (!comparator) {\n                flush(temp, result);\n                result.push(row);\n                continue;\n            }\n\n            const cell = formattingRules.resolve(data, rows, columns, row, column, edition);\n            const entry = { entity: row, comparator, cell };\n\n            if (temp.length === 0) {\n                temp.push(entry);\n                continue;\n            }\n\n            if (temp[0].comparator === comparator) {\n                temp.push(entry);\n                continue;\n            }\n\n            flush(temp, result);\n            temp.push(entry);\n        }\n\n        flush(temp, result);\n        rows = result;\n    }\n\n    return rows;\n}\n\nexport function getSortedColumns(sortBy, sortingRules, formattingRules, data, rows, columns, edition) {\n    if (sortBy.length === 0)\n        return columns;\n\n    const sortByLookup = getSortByLookup(sortBy, 'rowId', 'columnId');\n    const rowLookup = new Map(rows.map(row => [row.key, row]));\n    const sortedRows = sortBy\n        .map(cell => stringifyId(cell.rowId))\n        .filter(key => rowLookup.has(key))\n        .map(key => rowLookup.get(key))\n        .reverse();\n\n    if (sortedRows.length === 0)\n        return columns;\n\n    for (const row of sortedRows) {\n        const result = [];\n        const temp = [];\n\n        for (const column of columns) {\n            const comparator = sortingRules.resolve(column, row, sortByLookup.get(row.key));\n\n            if (!comparator) {\n                flush(temp, result);\n                result.push(column);\n                continue;\n            }\n\n            const cell = formattingRules.resolve(data, rows, columns, row, column, edition);\n            const entry = { entity: column, comparator, cell };\n\n            if (temp.length === 0) {\n                temp.push(entry);\n                continue;\n            }\n\n            if (temp[0].comparator === comparator) {\n                temp.push(entry);\n                continue;\n            }\n\n            flush(temp, result);\n            temp.push(entry);\n        }\n\n        flush(temp, result);\n        columns = result;\n    }\n\n    return columns;\n}",
         "import stringifyId from \"../core-utils/stringifyId.js\";\nimport getInternalPosition from \"./getInternalPosition.js\";\n\nconst grabOffset = 5;\n\n// TODO: not working when scrolled\n\nexport function getResizableColumn(columns, columnLookup, rowLookup, hoveredCell, element, mousePosition, fixedSize, totalSize) {\n    if (!hoveredCell)\n        return null;\n\n    const column = columnLookup.get(stringifyId(hoveredCell.columnId));\n    const row = rowLookup.get(stringifyId(hoveredCell.rowId));\n\n    if (row.type !== 'HEADER')\n        return null;\n\n    const internalPosition = getInternalPosition(element, mousePosition, fixedSize, totalSize);\n    if (!internalPosition)\n        return null;\n    const x = internalPosition.x;\n\n    if (x >= column.right - grabOffset && x <= column.right + grabOffset)\n        return column.id;\n\n    if (column.index === 0)\n        return null;\n    if (x < column.left - grabOffset || x > column.left + grabOffset)\n        return null;\n\n    return columns[column.index - 1].id;\n}\n\nexport function getResizableRow(rows, columnLookup, rowLookup, hoveredCell, element, mousePosition, fixedSize, totalSize) {\n    if (!hoveredCell)\n        return null;\n\n    const column = columnLookup.get(stringifyId(hoveredCell.columnId));\n    const row = rowLookup.get(stringifyId(hoveredCell.rowId));\n\n    if (column.type !== 'HEADER')\n        return null;\n\n    const internalPosition = getInternalPosition(element, mousePosition, fixedSize, totalSize);\n    if (!internalPosition)\n        return null;\n    const y = internalPosition.y;\n\n    if (y >= row.bottom - grabOffset && y <= row.bottom + grabOffset)\n        return row.id;\n\n    if (row.index === 0)\n        return null;\n    if (y < row.top - grabOffset || y > row.top + grabOffset)\n        return null;\n\n    return rows[row.index - 1].id;\n}",
         "export default function getResolvedSortBy(sortBy) {\n    return sortBy.map(sort => ({\n        columnId: 'columnId' in sort ? sort.columnId : 'HEADER',\n        rowId: 'rowId' in sort ? sort.rowId : 'HEADER',\n        direction: sort.direction\n    }));\n}",
         "export default function getResolvedFilters(filters) {\n    return filters.map(filter => ({\n        columnId: 'columnId' in filter ? filter.columnId : 'FILTER',\n        rowId: 'rowId' in filter ? filter.rowId : 'FILTER',\n        expression: filter.expression\n    }));\n}",
         "function getActive(entries, callback) {\n    const ids = entries\n        .filter(entry => entry.type === 'DATA')\n        .map(entry => entry.id);\n\n    callback(ids);\n\n    return ids;\n}\n\nexport function getActiveColumns(columns, callback) {\n    return getActive(columns, callback);\n}\n\nexport function getActiveRows(rows, callback) {\n    return getActive(rows, callback);\n}",
-        "import getEditableCells from \"../state-utils/getEditableCells.js\";\nimport getDataFormatting from \"../state-utils/getDataFormatting.js\";\nimport getInputFormatting from \"../state-utils/getInputFormatting.js\";\nimport getRenderFormatting from \"../state-utils/getRenderFormatting.js\";\nimport getSections from \"../state-utils/getSections.js\";\nimport getEditedCellsAndFilters from \"../state-utils/getEditedCellsAndFilters.js\";\nimport getEdition from \"../state-utils/getEdition.js\";\nimport getSelection from \"../state-utils/getSelection.js\";\nimport getInvoked from \"../state-utils/getInvoked.js\";\nimport { getResolvedColumns, getResolvedRows } from \"../state-utils/getResolved.js\";\nimport { getPlacedColumns, getPlacedRows } from \"../state-utils/getPlaced.js\";\nimport getFormattingRules from \"../state-utils/getFormattingRules.js\";\nimport getFormatResolver from \"../state-utils/getFormatResolver.js\";\nimport { getFilteredColumns as getFilteredColumns, getFilteredRows as getFilteredRows } from \"../state-utils/getFiltered.js\";\nimport getFixedSize from \"../state-utils/getFixedSize.js\";\nimport getTotalSize from \"../state-utils/getTotalSize.js\";\nimport getTextResolver from \"../state-utils/getTextResolver.js\";\nimport getScrollRect from \"../state-utils/getScrollRect.js\";\nimport getHoveredCell from \"../state-utils/getHoveredCell.js\";\nimport getLookup from \"../state-utils/getLookup.js\";\nimport getHighlightedCells from \"../state-utils/getHighlightedCells.js\";\nimport getInputPlacement from \"../state-utils/getInputPlacement.js\";\nimport getIsTextValid from \"../state-utils/getIsTextValid.js\";\nimport { getUnfoldedColumns, getUnfoldedRows } from \"../state-utils/getUnfolded.js\";\nimport getFilteringRules from \"../state-utils/getFilteringRules.js\";\nimport getFilterFormatting from \"../state-utils/getFilterFormatting.js\";\nimport getMeasureFormatting from \"../state-utils/getMeasureFormatting.js\";\nimport { getMeasuredColumns, getMeasuredRows } from \"../state-utils/getMeasured.js\";\nimport getKeys from \"../state-utils/getKeys.js\";\nimport getSortingFormatting from \"../state-utils/getSortingFormatting.js\";\nimport getSortingRules from \"../state-utils/getSortingRules.js\";\nimport { getSortedColumns, getSortedRows } from \"../state-utils/getSorted.js\";\nimport { getResizableColumn, getResizableRow } from \"../state-utils/getResizable.js\";\nimport getResolvedSortBy from \"../state-utils/getResolvedSortBy.js\";\nimport getResolvedFilters from \"../state-utils/getResolvedFilters.js\";\nimport { getActiveColumns } from \"../state-utils/getActive.js\";\n\n// TODO: write some test to check if the cache is working properly\nfunction updateStateInternal(context) {\n    // console.count('updateState');\n\n    const options = { ...context.localOptions, ...context.externalOptions };\n    const memory = context.memory;\n    const previousState = context.state;\n    const element = context.element;\n\n    // TODO: Move to utils\n    function cache(key, func, dependencies) {\n        const previousDependencies = memory[key] && memory[key].dependencies;\n        if (!previousDependencies || dependencies.some((dependency, index) => dependency !== previousDependencies[index]))\n            memory[key] = { value: func(...dependencies), dependencies };\n        return memory[key].value;\n    }\n\n    const devicePixelRatio = window.devicePixelRatio; // TODO: Trigger update on devicePixelRatio change\n    const borderWidth = options.borderWidth / devicePixelRatio;\n    const data = options.data;\n    const text = context.input.value;\n    const sortBy = cache('sortBy', getResolvedSortBy, [options.sortBy]);\n    const filters = cache('filters', getResolvedFilters, [options.filters]);\n    const textResolver = cache('textResolver', getTextResolver, []);\n    const dataFormatting = cache('dataFormatting', getDataFormatting, [options.formatting, options.dataSelector, sortBy]);\n    const editedCellsAndFilters = cache('editedCellsAndFilters', getEditedCellsAndFilters, [options.editedCells, filters]);\n    const edition = cache('edition', getEdition, [editedCellsAndFilters]);\n    const invokedColumns = cache('invokedColumns', getInvoked, [options.columns, data]);\n    const invokedRows = cache('invokedRows', getInvoked, [options.rows, data]);\n    // TODO: throw on duplicate ids\n    // TODO: throw on duplicate row/column filter ids\n    const unfoldedColumns = cache('unfoldedColumns', getUnfoldedColumns, [invokedColumns, data]);\n    const unfoldedRows = cache('unfoldedRows', getUnfoldedRows, [invokedRows, data]);\n    const unfilteredColumns = cache('unfilteredColumns', getResolvedColumns, [unfoldedColumns, options.pinnedLeft, options.pinnedRight, options.columnWidths]);\n    const unfilteredRows = cache('unfilteredRows', getResolvedRows, [unfoldedRows, options.pinnedTop, options.pinnedBottom, options.rowHeights]);\n    const unfilteredColumnKeys = cache('unfilteredColumnKeys', getKeys, [unfilteredColumns]);\n    const unfilteredRowKeys = cache('unfilteredRowKeys', getKeys, [unfilteredRows]);\n\n    // Filtering\n    const filterFormatting = cache('filterFormatting', getFilterFormatting, [dataFormatting]);\n    const filterFormattingRules = cache('filterFormattingRules', getFormattingRules, [filterFormatting]);\n    const filteringRules = cache('filteringRules', getFilteringRules, [options.filtering]);\n    const filteredColumns = cache('filteredColumns', getFilteredColumns, [filters, filteringRules, filterFormattingRules, data, unfilteredRows, unfilteredColumns, edition]);\n    const filteredRows = cache('filteredRows', getFilteredRows, [filters, filteringRules, filterFormattingRules, data, unfilteredRows, unfilteredColumns, edition]);\n\n    // Sorting\n    const sortingFormatting = cache('sortingFormatting', getSortingFormatting, [dataFormatting]);\n    const sortingFormattingRules = cache('sortingFormattingRules', getFormattingRules, [sortingFormatting]);\n    const sortingRules = cache('sortingRules', getSortingRules, [options.sorting]);\n    const sortedColumns = cache('sortedColumns', getSortedColumns, [sortBy, sortingRules, sortingFormattingRules, data, filteredRows, filteredColumns, edition]);\n    const sortedRows = cache('sortedRows', getSortedRows, [sortBy, sortingRules, sortingFormattingRules, data, filteredRows, filteredColumns, edition]);\n\n    // Shaping\n    const shapedColumns = sortedColumns;\n    const shapedRows = sortedRows;\n\n    // Measuring\n    const measureFormatting = cache('measureFormatting', getMeasureFormatting, [dataFormatting]);\n    const measureFormattingRules = cache('measureFormattingRules', getFormattingRules, [measureFormatting]);\n    const measureFormatResolver = cache('measureFormatResolver', getFormatResolver, [measureFormattingRules, data, shapedRows, shapedColumns, edition]);\n    const columnWidthCache = context.columnWidthCache;\n    const rowHeightCache = context.rowHeightCache;\n    const measuredColumns = cache('measuredColumns', getMeasuredColumns, [shapedColumns, shapedRows, textResolver, measureFormatResolver, columnWidthCache, unfilteredColumnKeys]);\n    const measuredRows = cache('measuredRows', getMeasuredRows, [shapedColumns, shapedRows, textResolver, measureFormatResolver, rowHeightCache, unfilteredRowKeys]);\n\n    // Placement\n    const columns = cache('columns', getPlacedColumns, [measuredColumns, devicePixelRatio, borderWidth]);\n    const rows = cache('rows', getPlacedRows, [measuredRows, devicePixelRatio, borderWidth]);\n    const columnLookup = cache('columnLookup', getLookup, [columns]);\n    const rowLookup = cache('rowLookup', getLookup, [rows]);\n    const focusedCell = options.focusedCell;\n    const sections = cache('sections', getSections, [columns, rows]);\n    const selectedCells = options.selectedCells;\n    const fixedSize = cache('fixedSize', getFixedSize, [sections.top.height, sections.bottom.height, sections.left.width, sections.right.width]);\n    const totalSize = cache('totalSize', getTotalSize, [columns, rows]);\n    // TODO: do some proper caching, so that if value is not changed, the old value is returned (currently not working because of scrolling)\n    const hoveredCell = getHoveredCell(element, context.mousePosition, rows, columns, fixedSize, totalSize);\n    const resizableColumn = context.resizingColumn || cache('resizableColumn', getResizableColumn, [columns, columnLookup, rowLookup, hoveredCell, element, context.mousePosition, fixedSize, totalSize]);\n    const resizableRow = context.resizingRow || cache('resizableRow', getResizableRow, [rows, columnLookup, rowLookup, hoveredCell, element, context.mousePosition, fixedSize, totalSize]);\n    const isMouseDown = context.isMouseDown;\n    const isResizing = !!resizableColumn || !!resizableRow;\n    const highlightedCells = cache('highlightedCells', getHighlightedCells, [isMouseDown, isResizing, focusedCell, hoveredCell, columns, rows, columnLookup, rowLookup]);\n    const selection = cache('selection', getSelection, [selectedCells]);\n    const highlight = cache('highlight', getSelection, [highlightedCells]);\n    // TODO: addDataFormattingRules and addRenderFormattingRules should remove unnecessary rules\n    const renderFormatting = cache('renderFormatting', getRenderFormatting, [dataFormatting, hoveredCell, focusedCell, selection, highlight, edition, sortBy, resizableColumn, resizableRow, options.borderWidth]);\n    const renderFormattingRules = cache('renderFormattingRules', getFormattingRules, [renderFormatting]);\n    const renderFormatResolver = cache('renderFormatResolver', getFormatResolver, [renderFormattingRules, data, rows, columns, edition]);\n    const inputFormatting = cache('inputFormatting', getInputFormatting, [dataFormatting]);\n    const inputFormattingRules = cache('inputFormattingRules', getFormattingRules, [inputFormatting]);\n    const inputFormatResolver = cache('inputFormatResolver', getFormatResolver, [inputFormattingRules, data, rows, columns, edition]);\n    const editableCells = cache('editableCells', getEditableCells, [selectedCells, inputFormatResolver, columnLookup, rowLookup]);\n    const inputPlacement = cache('inputPlacement', getInputPlacement, [editableCells, focusedCell, columnLookup, rowLookup, sections]);\n    const isTextValid = cache('isTextValid', getIsTextValid, [text, editableCells]);\n\n    // cache result, but not call\n    const scrollRect = getScrollRect(previousState?.scrollRect, totalSize, fixedSize, element);\n\n    // callbacks\n    cache('activeColumns', getActiveColumns, [columns, options.onActiveColumnsChange]);\n    cache('activeRows', getActiveColumns, [rows, options.onActiveRowsChange]);\n\n    context.state = {\n        options,\n        devicePixelRatio,\n        borderWidth,\n        data,\n        dataFormatting,\n        edition,\n        filteredColumns,\n        filteredRows,\n        columns,\n        rows,\n        sections,\n        selectedCells,\n        selection,\n        highlight,\n        hoveredCell,\n        focusedCell,\n        renderFormatting,\n        renderFormatResolver,\n        inputFormatting,\n        inputFormatResolver,\n        fixedSize,\n        totalSize,\n        textResolver,\n        scrollRect,\n        highlightedCells,\n        inputPlacement,\n        columnLookup,\n        rowLookup,\n        text,\n        isTextValid,\n        resizableColumn,\n        resizableRow,\n    };\n}\n\nexport default function updateState(context) {\n    if (!context.error) {\n        try {\n            updateStateInternal(context);\n        } catch (error) {\n            context.error = error;\n        }\n    }\n}",
+        "import getReducedFormatting from \"./getReducedFormatting.js\";\n\nexport default function getContextFormatting(formatting) {\n    return getReducedFormatting(formatting, ['value', 'text', 'tooltip']);\n}",
+        "import stringifyId from \"../core-utils/stringifyId.js\";\n\nexport default function getTooltip(hoveredCell, formatResolver, columnLookup, rowLookup) {\n    if (!hoveredCell)\n        return null;\n\n    const columnKey = stringifyId(hoveredCell.columnId);\n    const rowKey = stringifyId(hoveredCell.rowId);\n\n    if (!columnLookup.has(columnKey))\n        return null;\n    if (!rowLookup.has(rowKey))\n        return null;\n\n    const row = rowLookup.get(rowKey);\n    const column = columnLookup.get(columnKey);\n\n    return formatResolver.resolve(row, column).tooltip;\n}",
+        "import getCellPlacement from \"./getCellPlacement.js\";\n\nexport default function getTooltipPlacement(tooltip, focusedCell, columnLookup, rowLookup, sections) {\n    if (!tooltip)\n        return null;\n\n    const cellPlacement = getCellPlacement(focusedCell, columnLookup, rowLookup, sections);\n\n    if (!cellPlacement)\n        return null;\n\n    return {\n        top: cellPlacement.top,\n        left: cellPlacement.left\n    };\n}",
+        "import getEditableCells from \"../state-utils/getEditableCells.js\";\nimport getDataFormatting from \"../state-utils/getDataFormatting.js\";\nimport getInputFormatting from \"../state-utils/getInputFormatting.js\";\nimport getRenderFormatting from \"../state-utils/getRenderFormatting.js\";\nimport getSections from \"../state-utils/getSections.js\";\nimport getEditedCellsAndFilters from \"../state-utils/getEditedCellsAndFilters.js\";\nimport getEdition from \"../state-utils/getEdition.js\";\nimport getSelection from \"../state-utils/getSelection.js\";\nimport getInvoked from \"../state-utils/getInvoked.js\";\nimport { getResolvedColumns, getResolvedRows } from \"../state-utils/getResolved.js\";\nimport { getPlacedColumns, getPlacedRows } from \"../state-utils/getPlaced.js\";\nimport getFormattingRules from \"../state-utils/getFormattingRules.js\";\nimport getFormatResolver from \"../state-utils/getFormatResolver.js\";\nimport { getFilteredColumns as getFilteredColumns, getFilteredRows as getFilteredRows } from \"../state-utils/getFiltered.js\";\nimport getFixedSize from \"../state-utils/getFixedSize.js\";\nimport getTotalSize from \"../state-utils/getTotalSize.js\";\nimport getTextResolver from \"../state-utils/getTextResolver.js\";\nimport getScrollRect from \"../state-utils/getScrollRect.js\";\nimport getHoveredCell from \"../state-utils/getHoveredCell.js\";\nimport getLookup from \"../state-utils/getLookup.js\";\nimport getHighlightedCells from \"../state-utils/getHighlightedCells.js\";\nimport getInputPlacement from \"../state-utils/getInputPlacement.js\";\nimport getIsTextValid from \"../state-utils/getIsTextValid.js\";\nimport { getUnfoldedColumns, getUnfoldedRows } from \"../state-utils/getUnfolded.js\";\nimport getFilteringRules from \"../state-utils/getFilteringRules.js\";\nimport getFilterFormatting from \"../state-utils/getFilterFormatting.js\";\nimport getMeasureFormatting from \"../state-utils/getMeasureFormatting.js\";\nimport { getMeasuredColumns, getMeasuredRows } from \"../state-utils/getMeasured.js\";\nimport getKeys from \"../state-utils/getKeys.js\";\nimport getSortingFormatting from \"../state-utils/getSortingFormatting.js\";\nimport getSortingRules from \"../state-utils/getSortingRules.js\";\nimport { getSortedColumns, getSortedRows } from \"../state-utils/getSorted.js\";\nimport { getResizableColumn, getResizableRow } from \"../state-utils/getResizable.js\";\nimport getResolvedSortBy from \"../state-utils/getResolvedSortBy.js\";\nimport getResolvedFilters from \"../state-utils/getResolvedFilters.js\";\nimport { getActiveColumns } from \"../state-utils/getActive.js\";\nimport getContextFormatting from \"../state-utils/getContextFormatting.js\";\nimport getTooltip from \"../state-utils/getTooltip.js\";\nimport getTooltipPlacement from \"../state-utils/getTooltipPlacement.js\";\n\n// TODO: write some test to check if the cache is working properly\nfunction updateStateInternal(context) {\n    // console.count('updateState');\n\n    const options = { ...context.localOptions, ...context.externalOptions };\n    const memory = context.memory;\n    const previousState = context.state;\n    const element = context.element;\n\n    // TODO: Move to utils\n    function cache(key, func, dependencies) {\n        const previousDependencies = memory[key] && memory[key].dependencies;\n        if (!previousDependencies || dependencies.some((dependency, index) => dependency !== previousDependencies[index]))\n            memory[key] = { value: func(...dependencies), dependencies };\n        return memory[key].value;\n    }\n\n    const devicePixelRatio = window.devicePixelRatio; // TODO: Trigger update on devicePixelRatio change\n    const borderWidth = options.borderWidth / devicePixelRatio;\n    const data = options.data;\n    const text = context.input.value;\n    const sortBy = cache('sortBy', getResolvedSortBy, [options.sortBy]);\n    const filters = cache('filters', getResolvedFilters, [options.filters]);\n    const textResolver = cache('textResolver', getTextResolver, []);\n    const dataFormatting = cache('dataFormatting', getDataFormatting, [options.formatting, options.dataSelector, sortBy]);\n    const editedCellsAndFilters = cache('editedCellsAndFilters', getEditedCellsAndFilters, [options.editedCells, filters]);\n    const edition = cache('edition', getEdition, [editedCellsAndFilters]);\n    const invokedColumns = cache('invokedColumns', getInvoked, [options.columns, data]);\n    const invokedRows = cache('invokedRows', getInvoked, [options.rows, data]);\n    // TODO: throw on duplicate ids\n    // TODO: throw on duplicate row/column filter ids\n    const unfoldedColumns = cache('unfoldedColumns', getUnfoldedColumns, [invokedColumns, data]);\n    const unfoldedRows = cache('unfoldedRows', getUnfoldedRows, [invokedRows, data]);\n    const unfilteredColumns = cache('unfilteredColumns', getResolvedColumns, [unfoldedColumns, options.pinnedLeft, options.pinnedRight, options.columnWidths]);\n    const unfilteredRows = cache('unfilteredRows', getResolvedRows, [unfoldedRows, options.pinnedTop, options.pinnedBottom, options.rowHeights]);\n    const unfilteredColumnKeys = cache('unfilteredColumnKeys', getKeys, [unfilteredColumns]);\n    const unfilteredRowKeys = cache('unfilteredRowKeys', getKeys, [unfilteredRows]);\n\n    // Filtering\n    const filterFormatting = cache('filterFormatting', getFilterFormatting, [dataFormatting]);\n    const filterFormattingRules = cache('filterFormattingRules', getFormattingRules, [filterFormatting]);\n    const filteringRules = cache('filteringRules', getFilteringRules, [options.filtering]);\n    const filteredColumns = cache('filteredColumns', getFilteredColumns, [filters, filteringRules, filterFormattingRules, data, unfilteredRows, unfilteredColumns, edition]);\n    const filteredRows = cache('filteredRows', getFilteredRows, [filters, filteringRules, filterFormattingRules, data, unfilteredRows, unfilteredColumns, edition]);\n\n    // Sorting\n    const sortingFormatting = cache('sortingFormatting', getSortingFormatting, [dataFormatting]);\n    const sortingFormattingRules = cache('sortingFormattingRules', getFormattingRules, [sortingFormatting]);\n    const sortingRules = cache('sortingRules', getSortingRules, [options.sorting]);\n    const sortedColumns = cache('sortedColumns', getSortedColumns, [sortBy, sortingRules, sortingFormattingRules, data, filteredRows, filteredColumns, edition]);\n    const sortedRows = cache('sortedRows', getSortedRows, [sortBy, sortingRules, sortingFormattingRules, data, filteredRows, filteredColumns, edition]);\n\n    // Shaping\n    const shapedColumns = sortedColumns;\n    const shapedRows = sortedRows;\n\n    // Measuring\n    const measureFormatting = cache('measureFormatting', getMeasureFormatting, [dataFormatting]);\n    const measureFormattingRules = cache('measureFormattingRules', getFormattingRules, [measureFormatting]);\n    const measureFormatResolver = cache('measureFormatResolver', getFormatResolver, [measureFormattingRules, data, shapedRows, shapedColumns, edition]);\n    const columnWidthCache = context.columnWidthCache;\n    const rowHeightCache = context.rowHeightCache;\n    const measuredColumns = cache('measuredColumns', getMeasuredColumns, [shapedColumns, shapedRows, textResolver, measureFormatResolver, columnWidthCache, unfilteredColumnKeys]);\n    const measuredRows = cache('measuredRows', getMeasuredRows, [shapedColumns, shapedRows, textResolver, measureFormatResolver, rowHeightCache, unfilteredRowKeys]);\n\n    // Placement\n    const columns = cache('columns', getPlacedColumns, [measuredColumns, devicePixelRatio, borderWidth]);\n    const rows = cache('rows', getPlacedRows, [measuredRows, devicePixelRatio, borderWidth]);\n    const columnLookup = cache('columnLookup', getLookup, [columns]);\n    const rowLookup = cache('rowLookup', getLookup, [rows]);\n    const focusedCell = options.focusedCell;\n    const sections = cache('sections', getSections, [columns, rows]);\n    const selectedCells = options.selectedCells;\n    const fixedSize = cache('fixedSize', getFixedSize, [sections.top.height, sections.bottom.height, sections.left.width, sections.right.width]);\n    const totalSize = cache('totalSize', getTotalSize, [columns, rows]);\n    // TODO: do some proper caching, so that if value is not changed, the old value is returned (currently not working because of scrolling)\n    const hoveredCell = getHoveredCell(element, context.mousePosition, rows, columns, fixedSize, totalSize);\n    const resizableColumn = context.resizingColumn || cache('resizableColumn', getResizableColumn, [columns, columnLookup, rowLookup, hoveredCell, element, context.mousePosition, fixedSize, totalSize]);\n    const resizableRow = context.resizingRow || cache('resizableRow', getResizableRow, [rows, columnLookup, rowLookup, hoveredCell, element, context.mousePosition, fixedSize, totalSize]);\n    const isMouseDown = context.isMouseDown;\n    const isResizing = !!resizableColumn || !!resizableRow;\n    const highlightedCells = cache('highlightedCells', getHighlightedCells, [isMouseDown, isResizing, focusedCell, hoveredCell, columns, rows, columnLookup, rowLookup]);\n    const selection = cache('selection', getSelection, [selectedCells]);\n    const highlight = cache('highlight', getSelection, [highlightedCells]);\n    // TODO: addDataFormattingRules and addRenderFormattingRules should remove unnecessary rules\n    const renderFormatting = cache('renderFormatting', getRenderFormatting, [dataFormatting, hoveredCell, focusedCell, selection, highlight, edition, sortBy, resizableColumn, resizableRow, options.borderWidth]);\n    const renderFormattingRules = cache('renderFormattingRules', getFormattingRules, [renderFormatting]);\n    const renderFormatResolver = cache('renderFormatResolver', getFormatResolver, [renderFormattingRules, data, rows, columns, edition]);\n    const inputFormatting = cache('inputFormatting', getInputFormatting, [dataFormatting]);\n    const inputFormattingRules = cache('inputFormattingRules', getFormattingRules, [inputFormatting]);\n    const inputFormatResolver = cache('inputFormatResolver', getFormatResolver, [inputFormattingRules, data, rows, columns, edition]);\n    const editableCells = cache('editableCells', getEditableCells, [selectedCells, inputFormatResolver, columnLookup, rowLookup]);\n    const inputPlacement = cache('inputPlacement', getInputPlacement, [editableCells, focusedCell, columnLookup, rowLookup, sections]);\n    const isTextValid = cache('isTextValid', getIsTextValid, [text, editableCells]);\n    const contextFormatting = cache('contextFormatting', getContextFormatting, [dataFormatting]);\n    const contextFormattingRules = cache('contextFormattingRules', getFormattingRules, [contextFormatting]);\n    const contextFormatResolver = cache('contextFormatResolver', getFormatResolver, [contextFormattingRules, data, rows, columns, edition]);\n    const tooltip = cache('tooltip', getTooltip, [hoveredCell, contextFormatResolver, columnLookup, rowLookup]);\n    const tooltipPlacement = cache('tooltipPlacement', getTooltipPlacement, [tooltip, hoveredCell, columnLookup, rowLookup, sections]);\n\n    // cache result, but not call\n    const scrollRect = getScrollRect(previousState?.scrollRect, totalSize, fixedSize, element);\n\n    // callbacks\n    cache('activeColumns', getActiveColumns, [columns, options.onActiveColumnsChange]);\n    cache('activeRows', getActiveColumns, [rows, options.onActiveRowsChange]);\n\n    context.state = {\n        options,\n        devicePixelRatio,\n        borderWidth,\n        data,\n        edition,\n        filteredColumns,\n        filteredRows,\n        columns,\n        rows,\n        sections,\n        selectedCells,\n        selection,\n        highlight,\n        hoveredCell,\n        focusedCell,\n        renderFormatting,\n        renderFormatResolver,\n        inputFormatting,\n        inputFormatResolver,\n        fixedSize,\n        totalSize,\n        textResolver,\n        scrollRect,\n        highlightedCells,\n        inputPlacement,\n        columnLookup,\n        rowLookup,\n        text,\n        isTextValid,\n        resizableColumn,\n        resizableRow,\n        tooltip,\n        tooltipPlacement,\n    };\n}\n\nexport default function updateState(context) {\n    if (!context.error) {\n        try {\n            updateStateInternal(context);\n        } catch (error) {\n            context.error = error;\n        }\n    }\n}",
         "import getColumnIndex from \"./getColumnIndex.js\";\nimport getInternalPosition from \"./getInternalPosition.js\";\nimport getRowIndex from \"./getRowIndex.js\";\n\nexport default function getHoveredCell(element, mousePosition, rows, columns, fixedSize, totalSize) {\n    if (!mousePosition)\n        return null;\n    if (mousePosition.x < 0 || mousePosition.y < 0 || mousePosition.x > totalSize.width || mousePosition.y > totalSize.height)\n        return null;\n\n    const internalPosition = getInternalPosition(element, mousePosition, fixedSize, totalSize);\n    const hoverRowIndex = getRowIndex(rows, internalPosition.y);\n    const hoverColumnIndex = getColumnIndex(columns, internalPosition.x);\n\n    if (hoverRowIndex === -1 || hoverColumnIndex === -1)\n        return null;\n\n    return {\n        rowId: rows[hoverRowIndex].id,\n        columnId: columns[hoverColumnIndex].id\n    };\n}\n",
         "export default function getRowIndex(rows, y) {\n    if (rows.length === 0)\n        return -1;\n    if (y < rows[0].topWithBorder)\n        return -1;\n    if (y > rows[rows.length - 1].bottomWithBorder)\n        return -1;\n\n    let iterA = 0;\n    let iterC = rows.length - 1;\n\n    while (iterA <= iterC) {\n        const iterB = Math.floor((iterA + iterC) / 2);\n\n        if (y < rows[iterB].topWithBorder)\n            iterC = iterB - 1;\n        else if (y > rows[iterB].bottomWithBorder)\n            iterA = iterB + 1;\n\n        else\n            return iterB;\n    }\n\n    return -1;\n}\n",
         "export default function getColumnIndex(columns, x) {\n    if (columns.length === 0)\n        return -1;\n    if (x < columns[0].leftWithBorder)\n        return -1;\n    if (x > columns[columns.length - 1].rightWithBorder)\n        return -1;\n\n    let iterA = 0;\n    let iterC = columns.length - 1;\n\n    while (iterA <= iterC) {\n        const iterB = Math.floor((iterA + iterC) / 2);\n\n        if (x < columns[iterB].leftWithBorder)\n            iterC = iterB - 1;\n        else if (x > columns[iterB].rightWithBorder)\n            iterA = iterB + 1;\n\n        else\n            return iterB;\n    }\n\n    return -1;\n}\n",
         "import Selection from \"../types/Selection.js\";\n\nexport default function getCombinedCells(previousCells, newCells) {\n    const selection = new Selection(newCells);\n    return [...newCells, ...previousCells.filter(cell => !selection.isIdSelected(cell.rowId, cell.columnId))];\n}\n",
         "import Selection from \"../types/Selection.js\";\n\nexport default function getReducedCells(previousCells, cellsToRemove) {\n    const selection = new Selection(cellsToRemove);\n    return previousCells.filter(cell => !selection.isIdSelected(cell.rowId, cell.columnId));\n}\n",
         "export default function getMousePosition(event) {\n    const element = event.currentTarget;\n    const rect = element.getBoundingClientRect();\n    return {\n        x: event.clientX - rect.left,\n        y: event.clientY - rect.top\n    };\n}",
         "export function getWithAssumedId(cells, defaultId) {\n    return cells.map(cell => ({\n        ...cell,\n        columnId: 'id' in cell ? cell.id : defaultId,\n        rowId: 'id' in cell ? cell.id : defaultId\n    }));\n}",
-        "import getEditableCells from \"./state-utils/getEditableCells.js\";\nimport stringifyId from \"./core-utils/stringifyId.js\";\nimport render from \"./core/render.js\";\nimport updateState from \"./core/state.js\";\nimport getCombinedCells from \"./state-utils/getCombinedCells.js\";\nimport getReducedCells from \"./state-utils/getReducedCells.js\";\nimport getMousePosition from \"./state-utils/getMousePosition.js\";\nimport getNewSortBy from \"./state-utils/getNewSortBy.js\";\nimport getClipboardData from \"./state-utils/getClipboardData.js\";\nimport getToggledValue from \"./state-utils/getToggledValue.js\";\nimport getCellEditType from \"./state-utils/getCellEditType.js\";\nimport getInternalPosition from \"./state-utils/getInternalPosition.js\";\nimport { getWithAssumedId } from \"./state-utils/getWithAssumedId.js\";\n\nfunction initialize(element) {\n    if ('spread-grid-context' in element) return;\n\n    // console.log('initialize');\n\n    const canvases = {\n        'top-left': document.createElement('canvas'),\n        'top-center': document.createElement('canvas'),\n        'top-right': document.createElement('canvas'),\n        'middle-left': document.createElement('canvas'),\n        'middle-center': document.createElement('canvas'),\n        'middle-right': document.createElement('canvas'),\n        'bottom-left': document.createElement('canvas'),\n        'bottom-center': document.createElement('canvas'),\n        'bottom-right': document.createElement('canvas')\n    };\n    const input = document.createElement('input');\n\n    element.setAttribute('tabindex', '0');\n    element.setAttribute('style', 'max-width: 100vw; max-height: 100vh; overflow: auto; display: grid; position: relative; grid-template-columns: fit-content(0) fit-content(0) fit-content(0); grid-template-rows: fit-content(0) fit-content(0) fit-content(0); outline: none; user-select: none;');\n    element.classList.add('spread-grid');\n    canvases['top-left'].setAttribute('style', 'position: sticky; left: 0; top: 0; z-index: 2; grid-row: 1; grid-column: 1;');\n    canvases['top-center'].setAttribute('style', 'position: sticky; top: 0; z-index: 1; grid-row: 1; grid-column: 2;');\n    canvases['top-right'].setAttribute('style', 'position: sticky; right: 0; top: 0; z-index: 2; grid-row: 1; grid-column: 3;');\n    canvases['middle-left'].setAttribute('style', 'position: sticky; left: 0; z-index: 1; grid-row: 2; grid-column: 1;');\n    canvases['middle-center'].setAttribute('style', 'grid-row: 2; grid-column: 2; z-index: 0;');\n    canvases['middle-right'].setAttribute('style', 'position: sticky; right: 0; z-index: 1; grid-row: 2; grid-column: 3;');\n    canvases['bottom-left'].setAttribute('style', 'position: sticky; left: 0; bottom: 0; z-index: 2; grid-row: 3; grid-column: 1;');\n    canvases['bottom-center'].setAttribute('style', 'position: sticky; bottom: 0; z-index: 1; grid-row: 3; grid-column: 2;');\n    canvases['bottom-right'].setAttribute('style', 'position: sticky; right: 0; bottom: 0; z-index: 2; grid-row: 3; grid-column: 3;');\n    input.setAttribute('style', 'position: sticky; z-index: 3; outline: none; border: none; box-shadow: none; padding: 0 5px; font-size: 12px; font-family: Calibri; background-color: white; box-sizing: border-box; opacity: 0; pointer-events: none;');\n\n    const context = {\n        externalOptions: {},\n        state: null,\n        memory: {},\n        element: element,\n        canvases: canvases,\n        input: input,\n        renderRequested: false,\n        mousePosition: null,\n        isMouseDown: false,\n        columnWidthCache: new Map(),\n        rowHeightCache: new Map(),\n    };\n\n    context.requestNewRender = () => {\n        if (context.renderRequested) return;\n        context.renderRequested = true;\n        requestAnimationFrame(() => {\n            context.renderRequested = false;\n            updateState(context);\n            render(context);\n        });\n    };\n\n    context.addEventListener = (element, type, listener) => {\n        element.addEventListener(type, (event) => {\n            try {\n                listener(event);\n            }\n            catch (error) {\n                error.message = `[${type} event]: ${error.message}`;\n                context.error = error;\n                context.requestNewRender();\n            }\n        });\n    }\n\n    context.localOptions = {\n        data: [],\n        columns: [{ type: 'DATA-BLOCK' }],\n        rows: [{ type: 'HEADER' }, { type: 'DATA-BLOCK' }],\n        formatting: [],\n        filtering: [],\n        sorting: [],\n        dataSelector: ({ data, row, column }) => data?.[row.id]?.[column.id],\n        pinnedTop: 0,\n        pinnedBottom: 0,\n        pinnedLeft: 0,\n        pinnedRight: 0,\n        borderWidth: 1,\n        focusedCell: null,\n        onFocusedCellChange: (focusedCell) => {\n            context.localOptions.focusedCell = focusedCell;\n            context.requestNewRender();\n        },\n        selectedCells: [],\n        onSelectedCellsChange: (selectedCells) => {\n            context.localOptions.selectedCells = selectedCells;\n            context.requestNewRender();\n        },\n        highlightedCells: [],\n        editedCells: [],\n        onEditedCellsChange: (editedCells) => {\n            // TODO: optimize by coalescing\n            context.localOptions.editedCells = editedCells;\n            context.requestNewRender();\n        },\n        filters: [],\n        onFiltersChange: (filters) => {\n            context.localOptions.filters = filters;\n            context.requestNewRender();\n        },\n        sortBy: [],\n        onSortByChange: (sortBy) => {\n            context.localOptions.sortBy = sortBy;\n            context.requestNewRender();\n        },\n        onCellClick: () => { },\n        onCustomCellClick: () => { },\n        columnWidths: [],\n        onColumnWidthsChange: (columnWidths) => {\n            context.localOptions.columnWidths = columnWidths;\n            context.requestNewRender();\n        },\n        rowHeights: [],\n        onRowHeightsChange: (rowHeights) => {\n            context.localOptions.rowHeights = rowHeights;\n            context.requestNewRender();\n        },\n        onActiveColumnsChange: () => { },\n        onActiveRowsChange: () => { },\n    };\n\n    element['spread-grid-context'] = context;\n\n    const setText = (text) => {\n        input.value = text;\n        input.dispatchEvent(new Event('input'));\n    }\n\n    const accept = (autoCommit) => {\n        const selectedCells = context.state.options.selectedCells;\n        const formatResolver = context.state.inputFormatResolver;\n        const columnLookup = context.state.columnLookup;\n        const rowLookup = context.state.rowLookup;\n        const text = context.state.text;\n        const isTextValid = context.state.isTextValid;\n        const setEditedCells = context.state.options.onEditedCellsChange;\n        const setFilters = context.state.options.onFiltersChange;\n        const addEditedCells = (cells) => setEditedCells(getCombinedCells(context.state.options.editedCells, cells));\n        const addFilters = (cells) => setFilters(getCombinedCells(getWithAssumedId(context.state.options.filters, 'FILTER'), cells));\n        const editableCells = getEditableCells(selectedCells, formatResolver, columnLookup, rowLookup);\n\n        if (text === '')\n            return;\n        if (!isTextValid)\n            return;\n        if (autoCommit && !editableCells.every(cell => cell.edit.autoCommit))\n            return;\n\n        const dataCells = editableCells.filter(cell => cell.type === 'DATA');\n        const filterCells = editableCells.filter(cell => cell.type === 'FILTER');\n\n        addEditedCells(dataCells.map(cell => ({ ...cell.cell, value: cell.edit.parse({ string: text }) })));\n        addFilters(filterCells.map(cell => ({ ...cell.cell, expression: cell.edit.parse({ string: text }) })));\n\n        if (!autoCommit)\n            setText('');\n    };\n\n    const clear = (autoCommit) => {\n        const selectedCells = context.state.options.selectedCells;\n        const setEditedCells = context.state.options.onEditedCellsChange;\n        const setFilters = context.state.options.onFiltersChange;\n        const removeEditedCells = (cells) => setEditedCells(getReducedCells(context.state.options.editedCells, cells));\n        const removeFilters = (cells) => setFilters(getReducedCells(getWithAssumedId(context.state.options.filters, 'FILTER'), cells));\n        const formatResolver = context.state.inputFormatResolver;\n        const columnLookup = context.state.columnLookup;\n        const rowLookup = context.state.rowLookup;\n        const editableCells = getEditableCells(selectedCells, formatResolver, columnLookup, rowLookup);\n\n        if (autoCommit && !editableCells.every(cell => cell.edit.autoCommit))\n            return;\n\n        removeEditedCells(selectedCells);\n        removeFilters(selectedCells);\n    }\n\n    // TODO: Move other input functions here as well\n\n    context.addEventListener(element, 'scroll', (event) => {\n        // TODO: only request new render if scroll position changed outside of the scope\n        // TODO: how to: calculate the new scrollRect here and compare it to the one in the state\n        // TODO: Also don't forget to check if the highlighted cell did change\n        // TODO: Consider forcing a new render when visible scrollRect changes (without waiting for the next render frame)\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'mouseenter', (event) => {\n        context.mousePosition = getMousePosition(event);\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'mousemove', (event) => {\n        context.mousePosition = getMousePosition(event);\n\n        if (context.resizingColumn) {\n            const column = context.state.columnLookup.get(stringifyId(context.resizingColumn));\n            const columnWidth = column.width;\n            const columnRight = column.right;\n            const internalPosition = getInternalPosition(element, context.mousePosition, context.state.fixedSize, context.state.totalSize);\n            const newColumnWidth = Math.max(10, internalPosition.x - columnRight + columnWidth);\n            const previousColumnWidths = context.state.options.columnWidths;\n            const newColumnWidths = previousColumnWidths\n                .filter(columnWidth => stringifyId(columnWidth.columnId) !== column.key)\n                .concat([{ columnId: column.id, width: newColumnWidth }]);\n            context.state.options.onColumnWidthsChange(newColumnWidths);\n        }\n        if (context.resizingRow) {\n            const row = context.state.rowLookup.get(stringifyId(context.resizingRow));\n            const rowHeight = row.height;\n            const rowBottom = row.bottom;\n            const internalPosition = getInternalPosition(element, context.mousePosition, context.state.fixedSize, context.state.totalSize);\n            const newRowHeight = Math.max(10, internalPosition.y - rowBottom + rowHeight);\n            const previousRowHeights = context.state.options.rowHeights;\n            const newRowHeights = previousRowHeights\n                .filter(rowHeight => stringifyId(rowHeight.rowId) !== row.key)\n                .concat([{ rowId: row.id, height: newRowHeight }]);\n            context.state.options.onRowHeightsChange(newRowHeights);\n        }\n\n        // TODO: only request new render if hovered cell changed\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'mouseleave', () => {\n        context.mousePosition = null;\n        context.requestNewRender();\n    });\n\n    // TODO: update mouse position on resize\n\n    context.addEventListener(element, 'mousedown', (event) => {\n        updateState(context);\n        setText('');\n\n        context.isMouseDown = true;\n        context.mouseDownPosition = context.mousePosition;\n        context.mouseDownCell = context.state.hoveredCell;\n\n        if (context.state.resizableColumn) {\n            context.resizingColumn = context.state.resizableColumn;\n        }\n        if (context.state.resizableRow) {\n            context.resizingRow = context.state.resizableRow;\n        }\n        if (!context.state.resizableColumn && !context.state.resizableRow) {\n            context.state.options.onFocusedCellChange(context.state.hoveredCell);\n        }\n\n        if (!event.ctrlKey)\n            context.state.options.onSelectedCellsChange([]);\n\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'mouseup', (event) => {\n        updateState(context);\n\n        context.isMouseDown = false;\n        context.resizingColumn = null;\n        context.resizingRow = null;\n\n        context.state.options.onSelectedCellsChange(getCombinedCells(context.state.options.selectedCells, context.state.highlightedCells));\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'pointerdown', (event) => {\n        context.element.setPointerCapture(event.pointerId);\n    });\n\n    context.addEventListener(element, 'pointerup', (event) => {\n        context.element.releasePointerCapture(event.pointerId);\n    });\n\n    context.addEventListener(element, 'click', (event) => {\n        updateState(context);\n\n        const cell = context.state.hoveredCell;\n        const mouseDownCell = context.mouseDownCell;\n\n        if (context.state.resizableColumn || context.state.resizableRow)\n            return;\n        if (cell === null)\n            return;\n        if (stringifyId(cell.columnId) !== stringifyId(mouseDownCell.columnId))\n            return;\n        if (stringifyId(cell.rowId) !== stringifyId(mouseDownCell.rowId))\n            return;\n\n        const column = context.state.columnLookup.get(stringifyId(cell.columnId));\n        const row = context.state.rowLookup.get(stringifyId(cell.rowId));\n        const sortBy = context.state.options.sortBy;\n        const formatResolver = context.state.inputFormatResolver;\n        const cellData = formatResolver.resolve(row, column);\n\n        if (cellData.edit?.toggle) {\n            const edition = context.state.edition;\n            const newValue = getToggledValue(cellData, column, row, edition);\n            const cellType = getCellEditType(column, row);\n            if (cellType === 'DATA')\n                context.state.options.onEditedCellsChange(getCombinedCells(context.state.options.editedCells, [{ ...cell, value: newValue }]));\n            if (cellType === 'FILTER')\n                context.state.options.onFiltersChange(getCombinedCells(context.state.options.filters, [{ ...cell, expression: newValue }]));\n        } else if (column.type === 'DATA' && row.type === 'DATA') {\n            context.state.options.onCellClick(context.state.hoveredCell);\n        } else if (column.type === 'CUSTOM' || row.type === 'CUSTOM') {\n            context.state.options.onCustomCellClick(context.state.hoveredCell);\n        } else if (column.type === 'HEADER' || row.type === 'HEADER') {\n            const newSortBy = getNewSortBy(sortBy, column, row, event.ctrlKey);\n            context.state.options.onSortByChange(newSortBy);\n            context.state.options.onSelectedCellsChange([]);\n        }\n    });\n\n    context.addEventListener(element, 'dblclick', (event) => {\n        updateState(context);\n\n        if (context.state.resizableColumn) {\n            const resizableColumnKey = stringifyId(context.state.resizableColumn);\n            const newColumnWidths = context.state.options.columnWidths.filter(columnWidth => stringifyId(columnWidth.columnId) !== resizableColumnKey);\n            context.state.options.onColumnWidthsChange(newColumnWidths);\n            context.columnWidthCache.delete(resizableColumnKey);\n        }\n        if (context.state.resizableRow) {\n            const resizableRowKey = stringifyId(context.state.resizableRow);\n            const newRowHeights = context.state.options.rowHeights.filter(rowHeight => stringifyId(rowHeight.rowId) !== resizableRowKey);\n            context.state.options.onRowHeightsChange(newRowHeights);\n            context.rowHeightCache.delete(resizableRowKey);\n        }\n\n        const focusedCell = context.state.focusedCell;\n        if (focusedCell === null)\n            return;\n\n        const focusedColumnKey = stringifyId(focusedCell.columnId);\n        const focusedRowKey = stringifyId(focusedCell.rowId);\n        const columnLookup = context.state.columnLookup;\n        const rowLookup = context.state.rowLookup;\n        const formatResolver = context.state.inputFormatResolver;\n\n        if (!columnLookup.has(focusedColumnKey))\n            return;\n        if (!rowLookup.has(focusedRowKey))\n            return;\n\n        const column = columnLookup.get(focusedColumnKey);\n        const row = rowLookup.get(focusedRowKey);\n        const cell = formatResolver.resolve(row, column);\n        const text = cell.text; // TODO: Make it configurable\n\n        if (!cell.edit)\n            return;\n        if (cell.edit.toggle)\n            return;\n\n        setText(text);\n        input?.select();\n    });\n\n    context.addEventListener(element, 'focus', () => {\n        if (input.parentElement)\n            input.focus({ preventScroll: true });\n    });\n\n    context.addEventListener(element, 'keydown', (event) => {\n        // TODO: make sure it's not invoked on keydown of the input\n        updateState(context);\n\n        const focusedCell = context.state.focusedCell;\n        const columnLookup = context.state.columnLookup;\n        const rowLookup = context.state.rowLookup;\n        const selectedCells = context.state.options.selectedCells;\n        const setSelectedCells = context.state.options.onSelectedCellsChange;\n        const addSelectedCells = (cells) => setSelectedCells(getCombinedCells(selectedCells, cells));\n        const setFocusedCell = context.state.options.onFocusedCellChange;\n        const editedCells = context.state.options.editedCells;\n        const setEditedCells = context.state.options.onEditedCellsChange;\n        const columns = context.state.columns;\n        const rows = context.state.rows;\n        const text = context.state.text;\n        const inputFormatResolver = context.state.inputFormatResolver;\n\n        const arrowTo = (cell, event) => {\n            setFocusedCell(cell);\n\n            if (event.shiftKey)\n                addSelectedCells([cell]);\n            else\n                setSelectedCells([cell]);\n        };\n\n        const arrowHorizontally = (offset, event) => {\n            if (!focusedCell)\n                return;\n\n            const focusedColumnKey = stringifyId(focusedCell.columnId);\n            if (!columnLookup.has(focusedColumnKey))\n                return;\n\n            const focusedColumnIndex = columnLookup.get(focusedColumnKey).index;\n            const newColumnIndex = Math.max(0, Math.min(columns.length - 1, focusedColumnIndex + offset));\n            if (newColumnIndex === focusedColumnIndex)\n                return;\n\n            const newFocusedCell = { rowId: focusedCell.rowId, columnId: columns[newColumnIndex].id };\n\n            arrowTo(newFocusedCell, event);\n        }\n\n        const arrowVertically = (offset, event) => {\n            if (!focusedCell)\n                return;\n\n            const focusedRowKey = stringifyId(focusedCell.rowId);\n            if (!rowLookup.has(focusedRowKey))\n                return;\n\n            const focusedRowIndex = rowLookup.get(focusedRowKey).index;\n            const newRowIndex = Math.max(0, Math.min(rows.length - 1, focusedRowIndex + offset));\n            if (newRowIndex === focusedRowIndex)\n                return;\n\n            const newFocusedCell = { rowId: rows[newRowIndex].id, columnId: focusedCell.columnId };\n\n            arrowTo(newFocusedCell, event);\n        }\n\n        const preventDefault = () => {\n            event.preventDefault();\n            event.stopPropagation();\n        };\n\n        const cancel = () => {\n            if (text !== '') {\n                setText('');\n            }\n            else if (selectedCells.length > 1) {\n                setSelectedCells([focusedCell]);\n            }\n            else if (editedCells.length > 0) {\n                setEditedCells([]);\n            }\n            else {\n                setFocusedCell(null);\n                setSelectedCells([]);\n            }\n        };\n\n        const copyToClipboard = (event) => {\n            if (!event.ctrlKey)\n                return;\n\n            const clipboardData = getClipboardData(selectedCells, columns, rows, inputFormatResolver);\n\n            if (navigator.clipboard) {\n                navigator.clipboard.writeText(clipboardData);\n            } else {\n                const textArea = document.createElement('textarea');\n                textArea.value = clipboardData;\n                document.body.appendChild(textArea);\n                textArea.select();\n                document.execCommand('copy');\n                document.body.removeChild(textArea);\n            }\n        }\n\n        switch (event.key) {\n            case 'Escape':\n                cancel();\n                break;\n            case 'Enter':\n                accept();\n                break;\n            case 'ArrowUp':\n                // TODO: When ctrl and shift are pressed together, select all cells between the focused cell and the new cell\n                // TODO: When shift is pressed, expand the current rect selection instead of moving the focused cell\n                preventDefault();\n                arrowVertically(event.ctrlKey ? -rows.length : -1, event);\n                break;\n            case 'ArrowDown':\n                preventDefault();\n                arrowVertically(event.ctrlKey ? rows.length : 1, event);\n                break;\n            case 'ArrowLeft':\n                preventDefault();\n                arrowHorizontally(event.ctrlKey ? -columns.length : -1, event);\n                break;\n            case 'ArrowRight':\n                preventDefault();\n                arrowHorizontally(event.ctrlKey ? columns.length : 1, event);\n                break;\n            case 'Delete':\n            case 'Backspace':\n                clear();\n                break;\n            case 'c':\n                copyToClipboard(event);\n                break;\n            default:\n                break;\n        }\n    });\n\n    new ResizeObserver(() => {\n        context.requestNewRender();\n    }).observe(element);\n\n    context.addEventListener(input, 'input', (event) => {\n        // TODO: check performance of this (if it's ok to update the state on every input event)\n        updateState(context);\n\n        if (event.target.value) {\n            accept(true);\n\n            input.style.opacity = 1;\n            input.style.pointerEvents = 'auto';\n        }\n        else {\n            if (event.isTrusted)\n                clear(true);\n\n            input.style.opacity = 0;\n            input.style.pointerEvents = 'none';\n        }\n    });\n\n    context.addEventListener(input, 'click', (event) => {\n        event.stopPropagation();\n    });\n\n    context.addEventListener(input, 'dblclick', (event) => {\n        event.stopPropagation();\n    });\n\n    context.addEventListener(input, 'mousedown', (event) => {\n        event.stopPropagation();\n    });\n\n    context.addEventListener(input, 'keydown', (event) => {\n        switch (event.key) {\n            case 'Enter':\n            case 'Escape':\n                break;\n            case 'Delete':\n            case 'Backspace':\n            case 'ArrowUp':\n            case 'ArrowDown':\n            case 'ArrowLeft':\n            case 'ArrowRight':\n                if (input.value !== '') {\n                    event.stopPropagation();\n                    context.requestNewRender();\n                }\n                break;\n            default:\n                event.stopPropagation();\n                // TODO: maybe only check if the new text is valid\n                context.requestNewRender();\n                break;\n        }\n    });\n}\n\nexport default function createGrid(element, options) {\n    // console.log('createGrid');\n\n    initialize(element);\n\n    const context = element['spread-grid-context'];\n    context.externalOptions = options;\n\n    if (context.state === null) {\n        updateState(context);\n        // TODO: only render if the state has sufficiently changed\n        render(context);\n    }\n    else {\n        context.requestNewRender();\n    }\n}",
+        "import getEditableCells from \"./state-utils/getEditableCells.js\";\nimport stringifyId from \"./core-utils/stringifyId.js\";\nimport render from \"./core/render.js\";\nimport updateState from \"./core/state.js\";\nimport getCombinedCells from \"./state-utils/getCombinedCells.js\";\nimport getReducedCells from \"./state-utils/getReducedCells.js\";\nimport getMousePosition from \"./state-utils/getMousePosition.js\";\nimport getNewSortBy from \"./state-utils/getNewSortBy.js\";\nimport getClipboardData from \"./state-utils/getClipboardData.js\";\nimport getToggledValue from \"./state-utils/getToggledValue.js\";\nimport getCellEditType from \"./state-utils/getCellEditType.js\";\nimport getInternalPosition from \"./state-utils/getInternalPosition.js\";\nimport { getWithAssumedId } from \"./state-utils/getWithAssumedId.js\";\n\nfunction initialize(element) {\n    if ('spread-grid-context' in element) return;\n\n    // console.log('initialize');\n\n    const canvases = {\n        'top-left': document.createElement('canvas'),\n        'top-center': document.createElement('canvas'),\n        'top-right': document.createElement('canvas'),\n        'middle-left': document.createElement('canvas'),\n        'middle-center': document.createElement('canvas'),\n        'middle-right': document.createElement('canvas'),\n        'bottom-left': document.createElement('canvas'),\n        'bottom-center': document.createElement('canvas'),\n        'bottom-right': document.createElement('canvas')\n    };\n    const input = document.createElement('input');\n    const tooltip = document.createElement('div');\n\n    element.setAttribute('tabindex', '0');\n    element.setAttribute('style', 'max-width: 100vw; max-height: 100vh; overflow: auto; display: grid; position: relative; grid-template-columns: fit-content(0) fit-content(0) fit-content(0); grid-template-rows: fit-content(0) fit-content(0) fit-content(0); outline: none; user-select: none;');\n    element.classList.add('spread-grid');\n    canvases['top-left'].setAttribute('style', 'position: sticky; left: 0; top: 0; z-index: 2; grid-row: 1; grid-column: 1;');\n    canvases['top-center'].setAttribute('style', 'position: sticky; top: 0; z-index: 1; grid-row: 1; grid-column: 2;');\n    canvases['top-right'].setAttribute('style', 'position: sticky; right: 0; top: 0; z-index: 2; grid-row: 1; grid-column: 3;');\n    canvases['middle-left'].setAttribute('style', 'position: sticky; left: 0; z-index: 1; grid-row: 2; grid-column: 1;');\n    canvases['middle-center'].setAttribute('style', 'grid-row: 2; grid-column: 2; z-index: 0;');\n    canvases['middle-right'].setAttribute('style', 'position: sticky; right: 0; z-index: 1; grid-row: 2; grid-column: 3;');\n    canvases['bottom-left'].setAttribute('style', 'position: sticky; left: 0; bottom: 0; z-index: 2; grid-row: 3; grid-column: 1;');\n    canvases['bottom-center'].setAttribute('style', 'position: sticky; bottom: 0; z-index: 1; grid-row: 3; grid-column: 2;');\n    canvases['bottom-right'].setAttribute('style', 'position: sticky; right: 0; bottom: 0; z-index: 2; grid-row: 3; grid-column: 3;');\n    input.setAttribute('style', 'position: sticky; z-index: 3; outline: none; border: none; box-shadow: none; padding: 0 5px; font-size: 12px; font-family: Calibri; background-color: white; box-sizing: border-box; opacity: 0; pointer-events: none;');\n    tooltip.setAttribute('style', 'pointer-events: none; background-color: white; color: black; border: 1px solid black; padding: 5px;');\n    tooltip.setAttribute('popover', '');\n\n    const context = {\n        externalOptions: {},\n        state: null,\n        memory: {},\n        element: element,\n        canvases: canvases,\n        input: input,\n        tooltip: tooltip,\n        renderRequested: false,\n        mousePosition: null,\n        isMouseDown: false,\n        columnWidthCache: new Map(),\n        rowHeightCache: new Map(),\n    };\n\n    context.requestNewRender = () => {\n        if (context.renderRequested) return;\n        context.renderRequested = true;\n        requestAnimationFrame(() => {\n            context.renderRequested = false;\n            updateState(context);\n            render(context);\n        });\n    };\n\n    context.addEventListener = (element, type, listener) => {\n        element.addEventListener(type, (event) => {\n            try {\n                listener(event);\n            }\n            catch (error) {\n                error.message = `[${type} event]: ${error.message}`;\n                context.error = error;\n                context.requestNewRender();\n            }\n        });\n    }\n\n    context.localOptions = {\n        data: [],\n        columns: [{ type: 'DATA-BLOCK' }],\n        rows: [{ type: 'HEADER' }, { type: 'DATA-BLOCK' }],\n        formatting: [],\n        filtering: [],\n        sorting: [],\n        dataSelector: ({ data, row, column }) => data?.[row.id]?.[column.id],\n        pinnedTop: 0,\n        pinnedBottom: 0,\n        pinnedLeft: 0,\n        pinnedRight: 0,\n        borderWidth: 1,\n        focusedCell: null,\n        onFocusedCellChange: (focusedCell) => {\n            context.localOptions.focusedCell = focusedCell;\n            context.requestNewRender();\n        },\n        selectedCells: [],\n        onSelectedCellsChange: (selectedCells) => {\n            context.localOptions.selectedCells = selectedCells;\n            context.requestNewRender();\n        },\n        highlightedCells: [],\n        editedCells: [],\n        onEditedCellsChange: (editedCells) => {\n            // TODO: optimize by coalescing\n            context.localOptions.editedCells = editedCells;\n            context.requestNewRender();\n        },\n        filters: [],\n        onFiltersChange: (filters) => {\n            context.localOptions.filters = filters;\n            context.requestNewRender();\n        },\n        sortBy: [],\n        onSortByChange: (sortBy) => {\n            context.localOptions.sortBy = sortBy;\n            context.requestNewRender();\n        },\n        onCellClick: () => { },\n        onCustomCellClick: () => { },\n        columnWidths: [],\n        onColumnWidthsChange: (columnWidths) => {\n            context.localOptions.columnWidths = columnWidths;\n            context.requestNewRender();\n        },\n        rowHeights: [],\n        onRowHeightsChange: (rowHeights) => {\n            context.localOptions.rowHeights = rowHeights;\n            context.requestNewRender();\n        },\n        onActiveColumnsChange: () => { },\n        onActiveRowsChange: () => { },\n    };\n\n    element['spread-grid-context'] = context;\n\n    const setText = (text) => {\n        input.value = text;\n        input.dispatchEvent(new Event('input'));\n    }\n\n    const accept = (autoCommit) => {\n        const selectedCells = context.state.options.selectedCells;\n        const formatResolver = context.state.inputFormatResolver;\n        const columnLookup = context.state.columnLookup;\n        const rowLookup = context.state.rowLookup;\n        const text = context.state.text;\n        const isTextValid = context.state.isTextValid;\n        const setEditedCells = context.state.options.onEditedCellsChange;\n        const setFilters = context.state.options.onFiltersChange;\n        const addEditedCells = (cells) => setEditedCells(getCombinedCells(context.state.options.editedCells, cells));\n        const addFilters = (cells) => setFilters(getCombinedCells(getWithAssumedId(context.state.options.filters, 'FILTER'), cells));\n        const editableCells = getEditableCells(selectedCells, formatResolver, columnLookup, rowLookup);\n\n        if (text === '')\n            return;\n        if (!isTextValid)\n            return;\n        if (autoCommit && !editableCells.every(cell => cell.edit.autoCommit))\n            return;\n\n        const dataCells = editableCells.filter(cell => cell.type === 'DATA');\n        const filterCells = editableCells.filter(cell => cell.type === 'FILTER');\n\n        addEditedCells(dataCells.map(cell => ({ ...cell.cell, value: cell.edit.parse({ string: text }) })));\n        addFilters(filterCells.map(cell => ({ ...cell.cell, expression: cell.edit.parse({ string: text }) })));\n\n        if (!autoCommit)\n            setText('');\n    };\n\n    const clear = (autoCommit) => {\n        const selectedCells = context.state.options.selectedCells;\n        const setEditedCells = context.state.options.onEditedCellsChange;\n        const setFilters = context.state.options.onFiltersChange;\n        const removeEditedCells = (cells) => setEditedCells(getReducedCells(context.state.options.editedCells, cells));\n        const removeFilters = (cells) => setFilters(getReducedCells(getWithAssumedId(context.state.options.filters, 'FILTER'), cells));\n        const formatResolver = context.state.inputFormatResolver;\n        const columnLookup = context.state.columnLookup;\n        const rowLookup = context.state.rowLookup;\n        const editableCells = getEditableCells(selectedCells, formatResolver, columnLookup, rowLookup);\n\n        if (autoCommit && !editableCells.every(cell => cell.edit.autoCommit))\n            return;\n\n        removeEditedCells(selectedCells);\n        removeFilters(selectedCells);\n    }\n\n    // TODO: Move other input functions here as well\n\n    context.addEventListener(element, 'scroll', (event) => {\n        // TODO: only request new render if scroll position changed outside of the scope\n        // TODO: how to: calculate the new scrollRect here and compare it to the one in the state\n        // TODO: Also don't forget to check if the highlighted cell did change\n        // TODO: Consider forcing a new render when visible scrollRect changes (without waiting for the next render frame)\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'mouseenter', (event) => {\n        context.mousePosition = getMousePosition(event);\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'mousemove', (event) => {\n        context.mousePosition = getMousePosition(event);\n\n        if (context.resizingColumn) {\n            const column = context.state.columnLookup.get(stringifyId(context.resizingColumn));\n            const columnWidth = column.width;\n            const columnRight = column.right;\n            const internalPosition = getInternalPosition(element, context.mousePosition, context.state.fixedSize, context.state.totalSize);\n            const newColumnWidth = Math.max(10, internalPosition.x - columnRight + columnWidth);\n            const previousColumnWidths = context.state.options.columnWidths;\n            const newColumnWidths = previousColumnWidths\n                .filter(columnWidth => stringifyId(columnWidth.columnId) !== column.key)\n                .concat([{ columnId: column.id, width: newColumnWidth }]);\n            context.state.options.onColumnWidthsChange(newColumnWidths);\n        }\n        if (context.resizingRow) {\n            const row = context.state.rowLookup.get(stringifyId(context.resizingRow));\n            const rowHeight = row.height;\n            const rowBottom = row.bottom;\n            const internalPosition = getInternalPosition(element, context.mousePosition, context.state.fixedSize, context.state.totalSize);\n            const newRowHeight = Math.max(10, internalPosition.y - rowBottom + rowHeight);\n            const previousRowHeights = context.state.options.rowHeights;\n            const newRowHeights = previousRowHeights\n                .filter(rowHeight => stringifyId(rowHeight.rowId) !== row.key)\n                .concat([{ rowId: row.id, height: newRowHeight }]);\n            context.state.options.onRowHeightsChange(newRowHeights);\n        }\n\n        // TODO: only request new render if hovered cell changed\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'mouseleave', () => {\n        context.mousePosition = null;\n        context.requestNewRender();\n    });\n\n    // TODO: update mouse position on resize\n\n    context.addEventListener(element, 'mousedown', (event) => {\n        updateState(context);\n        setText('');\n\n        context.isMouseDown = true;\n        context.mouseDownPosition = context.mousePosition;\n        context.mouseDownCell = context.state.hoveredCell;\n\n        if (context.state.resizableColumn) {\n            context.resizingColumn = context.state.resizableColumn;\n        }\n        if (context.state.resizableRow) {\n            context.resizingRow = context.state.resizableRow;\n        }\n        if (!context.state.resizableColumn && !context.state.resizableRow) {\n            context.state.options.onFocusedCellChange(context.state.hoveredCell);\n        }\n\n        if (!event.ctrlKey)\n            context.state.options.onSelectedCellsChange([]);\n\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'mouseup', (event) => {\n        updateState(context);\n\n        context.isMouseDown = false;\n        context.resizingColumn = null;\n        context.resizingRow = null;\n\n        context.state.options.onSelectedCellsChange(getCombinedCells(context.state.options.selectedCells, context.state.highlightedCells));\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'pointerdown', (event) => {\n        context.element.setPointerCapture(event.pointerId);\n    });\n\n    context.addEventListener(element, 'pointerup', (event) => {\n        context.element.releasePointerCapture(event.pointerId);\n    });\n\n    context.addEventListener(element, 'click', (event) => {\n        updateState(context);\n\n        const cell = context.state.hoveredCell;\n        const mouseDownCell = context.mouseDownCell;\n\n        if (context.state.resizableColumn || context.state.resizableRow)\n            return;\n        if (cell === null)\n            return;\n        if (stringifyId(cell.columnId) !== stringifyId(mouseDownCell.columnId))\n            return;\n        if (stringifyId(cell.rowId) !== stringifyId(mouseDownCell.rowId))\n            return;\n\n        const column = context.state.columnLookup.get(stringifyId(cell.columnId));\n        const row = context.state.rowLookup.get(stringifyId(cell.rowId));\n        const sortBy = context.state.options.sortBy;\n        const formatResolver = context.state.inputFormatResolver;\n        const cellData = formatResolver.resolve(row, column);\n        const eventProperties = {\n            ctrlKey: event.ctrlKey,\n            shiftKey: event.shiftKey,\n            button: event.button,\n            buttons: event.buttons\n        };\n\n        if (cellData.edit?.toggle) {\n            const edition = context.state.edition;\n            const newValue = getToggledValue(cellData, column, row, edition);\n            const cellType = getCellEditType(column, row);\n            if (cellType === 'DATA')\n                context.state.options.onEditedCellsChange(getCombinedCells(context.state.options.editedCells, [{ ...cell, value: newValue }]));\n            if (cellType === 'FILTER')\n                context.state.options.onFiltersChange(getCombinedCells(context.state.options.filters, [{ ...cell, expression: newValue }]));\n        } else if (column.type === 'DATA' && row.type === 'DATA') {\n            context.state.options.onCellClick({ ...context.state.hoveredCell, ...eventProperties });\n        } else if (column.type === 'CUSTOM' || row.type === 'CUSTOM') {\n            context.state.options.onCustomCellClick({ ...context.state.hoveredCell, ...eventProperties });\n        } else if (column.type === 'HEADER' || row.type === 'HEADER') {\n            const newSortBy = getNewSortBy(sortBy, column, row, event.ctrlKey);\n            context.state.options.onSortByChange(newSortBy);\n            context.state.options.onSelectedCellsChange([]);\n        }\n    });\n\n    context.addEventListener(element, 'dblclick', (event) => {\n        updateState(context);\n\n        if (context.state.resizableColumn) {\n            const resizableColumnKey = stringifyId(context.state.resizableColumn);\n            const newColumnWidths = context.state.options.columnWidths.filter(columnWidth => stringifyId(columnWidth.columnId) !== resizableColumnKey);\n            context.state.options.onColumnWidthsChange(newColumnWidths);\n            context.columnWidthCache.delete(resizableColumnKey);\n        }\n        if (context.state.resizableRow) {\n            const resizableRowKey = stringifyId(context.state.resizableRow);\n            const newRowHeights = context.state.options.rowHeights.filter(rowHeight => stringifyId(rowHeight.rowId) !== resizableRowKey);\n            context.state.options.onRowHeightsChange(newRowHeights);\n            context.rowHeightCache.delete(resizableRowKey);\n        }\n\n        const focusedCell = context.state.focusedCell;\n        if (focusedCell === null)\n            return;\n\n        const focusedColumnKey = stringifyId(focusedCell.columnId);\n        const focusedRowKey = stringifyId(focusedCell.rowId);\n        const columnLookup = context.state.columnLookup;\n        const rowLookup = context.state.rowLookup;\n        const formatResolver = context.state.inputFormatResolver;\n\n        if (!columnLookup.has(focusedColumnKey))\n            return;\n        if (!rowLookup.has(focusedRowKey))\n            return;\n\n        const column = columnLookup.get(focusedColumnKey);\n        const row = rowLookup.get(focusedRowKey);\n        const cell = formatResolver.resolve(row, column);\n        const text = cell.text; // TODO: Make it configurable\n\n        if (!cell.edit)\n            return;\n        if (cell.edit.toggle)\n            return;\n\n        setText(text);\n        input?.select();\n    });\n\n    context.addEventListener(element, 'focus', () => {\n        if (input.parentElement)\n            input.focus({ preventScroll: true });\n    });\n\n    context.addEventListener(element, 'keydown', (event) => {\n        // TODO: make sure it's not invoked on keydown of the input\n        updateState(context);\n\n        const focusedCell = context.state.focusedCell;\n        const columnLookup = context.state.columnLookup;\n        const rowLookup = context.state.rowLookup;\n        const selectedCells = context.state.options.selectedCells;\n        const setSelectedCells = context.state.options.onSelectedCellsChange;\n        const addSelectedCells = (cells) => setSelectedCells(getCombinedCells(selectedCells, cells));\n        const setFocusedCell = context.state.options.onFocusedCellChange;\n        const editedCells = context.state.options.editedCells;\n        const setEditedCells = context.state.options.onEditedCellsChange;\n        const columns = context.state.columns;\n        const rows = context.state.rows;\n        const text = context.state.text;\n        const inputFormatResolver = context.state.inputFormatResolver;\n\n        const arrowTo = (cell, event) => {\n            setFocusedCell(cell);\n\n            if (event.shiftKey)\n                addSelectedCells([cell]);\n            else\n                setSelectedCells([cell]);\n        };\n\n        const arrowHorizontally = (offset, event) => {\n            if (!focusedCell)\n                return;\n\n            const focusedColumnKey = stringifyId(focusedCell.columnId);\n            if (!columnLookup.has(focusedColumnKey))\n                return;\n\n            const focusedColumnIndex = columnLookup.get(focusedColumnKey).index;\n            const newColumnIndex = Math.max(0, Math.min(columns.length - 1, focusedColumnIndex + offset));\n            if (newColumnIndex === focusedColumnIndex)\n                return;\n\n            const newFocusedCell = { rowId: focusedCell.rowId, columnId: columns[newColumnIndex].id };\n\n            arrowTo(newFocusedCell, event);\n        }\n\n        const arrowVertically = (offset, event) => {\n            if (!focusedCell)\n                return;\n\n            const focusedRowKey = stringifyId(focusedCell.rowId);\n            if (!rowLookup.has(focusedRowKey))\n                return;\n\n            const focusedRowIndex = rowLookup.get(focusedRowKey).index;\n            const newRowIndex = Math.max(0, Math.min(rows.length - 1, focusedRowIndex + offset));\n            if (newRowIndex === focusedRowIndex)\n                return;\n\n            const newFocusedCell = { rowId: rows[newRowIndex].id, columnId: focusedCell.columnId };\n\n            arrowTo(newFocusedCell, event);\n        }\n\n        const preventDefault = () => {\n            event.preventDefault();\n            event.stopPropagation();\n        };\n\n        const cancel = () => {\n            if (text !== '') {\n                setText('');\n            }\n            else if (selectedCells.length > 1) {\n                setSelectedCells([focusedCell]);\n            }\n            else if (editedCells.length > 0) {\n                setEditedCells([]);\n            }\n            else {\n                setFocusedCell(null);\n                setSelectedCells([]);\n            }\n        };\n\n        const copyToClipboard = (event) => {\n            if (!event.ctrlKey)\n                return;\n\n            const clipboardData = getClipboardData(selectedCells, columns, rows, inputFormatResolver);\n\n            if (navigator.clipboard) {\n                navigator.clipboard.writeText(clipboardData);\n            } else {\n                const textArea = document.createElement('textarea');\n                textArea.value = clipboardData;\n                document.body.appendChild(textArea);\n                textArea.select();\n                document.execCommand('copy');\n                document.body.removeChild(textArea);\n            }\n        }\n\n        switch (event.key) {\n            case 'Escape':\n                cancel();\n                break;\n            case 'Enter':\n                accept();\n                break;\n            case 'ArrowUp':\n                // TODO: When ctrl and shift are pressed together, select all cells between the focused cell and the new cell\n                // TODO: When shift is pressed, expand the current rect selection instead of moving the focused cell\n                preventDefault();\n                arrowVertically(event.ctrlKey ? -rows.length : -1, event);\n                break;\n            case 'ArrowDown':\n                preventDefault();\n                arrowVertically(event.ctrlKey ? rows.length : 1, event);\n                break;\n            case 'ArrowLeft':\n                preventDefault();\n                arrowHorizontally(event.ctrlKey ? -columns.length : -1, event);\n                break;\n            case 'ArrowRight':\n                preventDefault();\n                arrowHorizontally(event.ctrlKey ? columns.length : 1, event);\n                break;\n            case 'Delete':\n            case 'Backspace':\n                clear();\n                break;\n            case 'c':\n                copyToClipboard(event);\n                break;\n            default:\n                break;\n        }\n    });\n\n    new ResizeObserver(() => {\n        context.requestNewRender();\n    }).observe(element);\n\n    context.addEventListener(input, 'input', (event) => {\n        // TODO: check performance of this (if it's ok to update the state on every input event)\n        updateState(context);\n\n        if (event.target.value) {\n            accept(true);\n\n            input.style.opacity = 1;\n            input.style.pointerEvents = 'auto';\n        }\n        else {\n            if (event.isTrusted)\n                clear(true);\n\n            input.style.opacity = 0;\n            input.style.pointerEvents = 'none';\n        }\n    });\n\n    context.addEventListener(input, 'click', (event) => {\n        event.stopPropagation();\n    });\n\n    context.addEventListener(input, 'dblclick', (event) => {\n        event.stopPropagation();\n    });\n\n    context.addEventListener(input, 'mousedown', (event) => {\n        event.stopPropagation();\n    });\n\n    context.addEventListener(input, 'keydown', (event) => {\n        switch (event.key) {\n            case 'Enter':\n            case 'Escape':\n                break;\n            case 'Delete':\n            case 'Backspace':\n            case 'ArrowUp':\n            case 'ArrowDown':\n            case 'ArrowLeft':\n            case 'ArrowRight':\n                if (input.value !== '') {\n                    event.stopPropagation();\n                    context.requestNewRender();\n                }\n                break;\n            default:\n                event.stopPropagation();\n                // TODO: maybe only check if the new text is valid\n                context.requestNewRender();\n                break;\n        }\n    });\n}\n\nexport default function createGrid(element, options) {\n    // console.log('createGrid');\n\n    initialize(element);\n\n    const context = element['spread-grid-context'];\n    context.externalOptions = options;\n\n    if (context.state === null) {\n        updateState(context);\n        // TODO: only render if the state has sufficiently changed\n        render(context);\n    }\n    else {\n        context.requestNewRender();\n    }\n}",
         "export default function getToggledValue(cell, column, row, edition) {\n    const value = edition.hasValueByKey(row.key, column.key)\n        ? edition.getValueByKey(row.key, column.key)\n        : cell.value;\n    const toggle = cell.edit.toggle;\n\n    if (typeof toggle === 'function')\n        return toggle({value}); // TODO: expand by context\n\n    return toggle[(toggle.indexOf(value) + 1) % toggle.length];\n}",
         "import stringifyId from '../core-utils/stringifyId.js';\n\nexport default function getNewSortBy(sortBy, column, row, ctrlKey) {\n    // TODO: better support for multi-row sorting\n\n    function isCurrentRule(rule) {\n        const columnId = 'columnId' in rule ? rule.columnId : 'HEADER';\n        const rowId = 'rowId' in rule ? rule.rowId : 'HEADER';\n\n        return column.key === stringifyId(columnId) && row.key === stringifyId(rowId);\n    }\n\n    function isConflictingWithCurrentRule(rule) {\n        const columnId = 'columnId' in rule ? rule.columnId : 'HEADER';\n        const rowId = 'rowId' in rule ? rule.rowId : 'HEADER';\n\n        return column.type === 'HEADER' && column.key === stringifyId(columnId)\n            || row.type === 'HEADER' && row.key === stringifyId(rowId);\n    }\n\n    const directionLoop = ['ASC', 'DESC', undefined];\n    const currentRule = sortBy.find(isCurrentRule);\n    const directionIndex = directionLoop.indexOf(currentRule?.direction);\n    const newDirection = directionLoop[(directionIndex + 1) % directionLoop.length];\n    const isLastRule = sortBy.indexOf(currentRule) === sortBy.length - 1;\n    const shouldKeepOld = ctrlKey && (isLastRule || !currentRule);\n    const rulesToKeep = shouldKeepOld\n        ? sortBy.filter(rule => !isCurrentRule(rule))\n        : sortBy.filter(rule => !isConflictingWithCurrentRule(rule));\n    const newRules = newDirection ? [{ columnId: column.id, rowId: row.id, direction: newDirection }] : [];\n\n    return [...rulesToKeep, ...newRules];\n}",
         "import stringifyId from \"../core-utils/stringifyId.js\";\nimport Selection from \"../types/Selection.js\";\n\nexport default function getClipboardData(selectedCells, columns, rows, formatResolver) {\n    const columnLookup = new Map(columns.map(column => [column.key, column]));\n    const rowLookup = new Map(rows.map(row => [row.key, row]));\n    const selectedCellKeys = selectedCells.map(cell => ({\n        columnKey: stringifyId(cell.columnId),\n        rowKey: stringifyId(cell.rowId)\n    })).filter(cell => columnLookup.has(cell.columnKey) && rowLookup.has(cell.rowKey));\n    const selectedColumns = new Set(selectedCellKeys.map(cell => cell.columnKey));\n    const selectedRows = new Set(selectedCellKeys.map(cell => cell.rowKey));\n\n    if (selectedCellKeys.length === 0)\n        return '';\n\n    const selection = new Selection(selectedCells);\n    const minColumnIndex = Math.min(...selectedCellKeys.map(cell => columnLookup.get(cell.columnKey).index));\n    const maxColumnIndex = Math.max(...selectedCellKeys.map(cell => columnLookup.get(cell.columnKey).index));\n    const minRowIndex = Math.min(...selectedCellKeys.map(cell => rowLookup.get(cell.rowKey).index));\n    const maxRowIndex = Math.max(...selectedCellKeys.map(cell => rowLookup.get(cell.rowKey).index));\n\n    const stringBuilder = [];\n\n    for (let rowIndex = minRowIndex; rowIndex <= maxRowIndex; rowIndex++) {\n        const row = rows[rowIndex];\n        const rowKey = row.key;\n\n        if (!selectedRows.has(rowKey))\n            continue;\n\n        for (let columnIndex = minColumnIndex; columnIndex <= maxColumnIndex; columnIndex++) {\n            const column = columns[columnIndex];\n            const columnKey = column.key;\n\n            if (!selectedColumns.has(columnKey))\n                continue;\n\n            if (selection.isKeySelected(rowKey, columnKey)) {\n                const cellData = formatResolver.resolve(row, column).text;\n                stringBuilder.push(cellData);\n            }\n\n            if (columnIndex < maxColumnIndex)\n                stringBuilder.push('\\t');\n        }\n\n        if (rowIndex < maxRowIndex)\n            stringBuilder.push('\\n');\n    }\n\n    return stringBuilder.join('');\n}",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\t// no module.id needed\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId](module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_1_2m1716627209\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n"
+        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_1_3m1716794736\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n"
     ],
     "version": 3
 }
```

### Comparing `dash_spread_grid-0.1.2/dash_spread_grid/metadata.json` & `dash_spread_grid-0.1.3/dash_spread_grid/metadata.json`

 * *Files identical despite different names*

### Comparing `dash_spread_grid-0.1.2/dash_spread_grid/package-info.json` & `dash_spread_grid-0.1.3/dash_spread_grid/package-info.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'version'": "'0.1.3'"}*

```diff
@@ -53,15 +53,15 @@
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:backends)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py",
         "watch": "npm-watch"
     },
-    "version": "0.1.2",
+    "version": "0.1.3",
     "watch": {
         "build": {
             "patterns": [
                 "../lib/**/*",
                 "./src/lib/**/*"
             ]
         }
```

### Comparing `dash_spread_grid-0.1.2/package.json` & `dash_spread_grid-0.1.3/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'version'": "'0.1.3'"}*

```diff
@@ -53,15 +53,15 @@
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:backends)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py",
         "watch": "npm-watch"
     },
-    "version": "0.1.2",
+    "version": "0.1.3",
     "watch": {
         "build": {
             "patterns": [
                 "../lib/**/*",
                 "./src/lib/**/*"
             ]
         }
```

