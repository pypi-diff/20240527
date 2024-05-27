# Comparing `tmp/thermolib-0.3.0.tar.gz` & `tmp/thermolib-0.3.1.tar.gz`

## Comparing `thermolib-0.3.0.tar` & `thermolib-0.3.1.tar`

### file list

```diff
@@ -1,39 +1,45 @@
--rw-r--r--   0        0        0      655 1970-01-01 00:00:00.000000 thermolib-0.3.0/Cargo.toml
--rw-r--r--   0        0        0       22 2024-03-13 13:32:17.000000 thermolib-0.3.0/.gitignore
--rw-r--r--   0        0        0   121546 2024-05-22 09:42:05.000000 thermolib-0.3.0/Cargo.lock
--rw-r--r--   0        0        0     1082 2024-02-20 03:32:56.000000 thermolib-0.3.0/LICENSE
--rw-r--r--   0        0        0      167 2024-02-20 03:32:56.000000 thermolib-0.3.0/README.md
--rw-r--r--   0        0        0       76 2024-05-22 09:31:41.000000 thermolib-0.3.0/build.rs
--rw-r--r--   0        0        0     6177 2024-04-10 07:36:35.000000 thermolib-0.3.0/res/SO2.json
--rw-r--r--   0        0        0       88 2024-05-22 09:31:41.000000 thermolib-0.3.0/src/bin/thermo.rs
--rw-r--r--   0        0        0      142 2024-05-22 09:31:41.000000 thermolib-0.3.0/src/bin/thermo.slint
--rw-r--r--   0        0        0     5451 2024-05-22 09:31:41.000000 thermolib-0.3.0/src/core/core_traits.rs
--rw-r--r--   0        0        0    18046 2024-05-22 09:31:41.000000 thermolib-0.3.0/src/core/generic_a.rs
--rw-r--r--   0        0        0      711 2024-05-21 12:58:03.000000 thermolib-0.3.0/src/core/ideal_cv.rs
--rw-r--r--   0        0        0     5682 2024-05-22 09:31:41.000000 thermolib-0.3.0/src/core/readme.md
--rw-r--r--   0        0        0      894 2024-05-21 12:58:36.000000 thermolib-0.3.0/src/core/tlerr.rs
--rw-r--r--   0        0        0      250 2024-04-20 06:32:36.000000 thermolib-0.3.0/src/core.rs
--rw-r--r--   0        0        0     7673 2024-05-22 09:31:41.000000 thermolib-0.3.0/src/helmholtz/alpha.rs
--rw-r--r--   0        0        0     4787 2024-05-22 09:31:41.000000 thermolib-0.3.0/src/helmholtz/alpha_i.rs
--rw-r--r--   0        0        0     8014 2024-05-22 09:31:41.000000 thermolib-0.3.0/src/helmholtz/alpha_r.rs
--rw-r--r--   0        0        0     2931 2024-05-22 04:13:04.000000 thermolib-0.3.0/src/helmholtz/anc_equ.rs
--rw-r--r--   0        0        0      250 2024-04-03 11:57:39.000000 thermolib-0.3.0/src/helmholtz.rs
--rw-r--r--   0        0        0      471 2024-05-22 09:31:41.000000 thermolib-0.3.0/src/lib.rs
--rw-r--r--   0        0        0     2969 2024-05-22 09:31:41.000000 thermolib-0.3.0/src/pc_saft/alpha.rs
--rw-r--r--   0        0        0     7483 2024-05-22 09:31:41.000000 thermolib-0.3.0/src/pc_saft/alpha_r.rs
--rw-r--r--   0        0        0    31349 2024-05-22 07:41:05.000000 thermolib-0.3.0/src/pc_saft/disp.rs
--rw-r--r--   0        0        0    20476 2024-05-22 07:43:46.000000 thermolib-0.3.0/src/pc_saft/hc.rs
--rw-r--r--   0        0        0      248 2024-05-22 09:31:41.000000 thermolib-0.3.0/src/pc_saft.rs
--rw-r--r--   0        0        0     1939 2024-05-22 07:46:25.000000 thermolib-0.3.0/src/pr/density_pr.rs
--rw-r--r--   0        0        0     9569 2024-05-22 09:31:41.000000 thermolib-0.3.0/src/pr/pr_pure.rs
--rw-r--r--   0        0        0      155 2024-05-22 09:31:41.000000 thermolib-0.3.0/src/pr.rs
--rw-r--r--   0        0        0     9805 2024-05-22 09:31:41.000000 thermolib-0.3.0/src/python.rs
--rw-r--r--   0        0        0     1316 2024-05-22 08:33:49.000000 thermolib-0.3.0/tests/internals/mod.rs
--rw-r--r--   0        0        0      406 2024-05-22 08:33:46.000000 thermolib-0.3.0/tests/main.cpp
--rw-r--r--   0        0        0      744 2024-05-22 09:31:41.000000 thermolib-0.3.0/tests/main.py
--rw-r--r--   0        0        0   118429 2024-05-22 08:34:33.000000 thermolib-0.3.0/tests/pcsaft.cpp
--rw-r--r--   0        0        0     5416 2024-05-21 11:39:49.000000 thermolib-0.3.0/tests/pcsaft.h
--rw-r--r--   0        0        0      550 2024-05-22 08:33:57.000000 thermolib-0.3.0/tests/test_json.rs
--rw-r--r--   0        0        0     1091 2024-05-22 08:34:00.000000 thermolib-0.3.0/tests/test_so2.rs
--rw-r--r--   0        0        0      406 2024-03-27 02:49:30.000000 thermolib-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      669 1970-01-01 00:00:00.000000 thermolib-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      655 1970-01-01 00:00:00.000000 thermolib-0.3.1/Cargo.toml
+-rw-r--r--   0        0        0       22 2024-03-13 13:32:17.000000 thermolib-0.3.1/.gitignore
+-rw-r--r--   0        0        0   121546 2024-05-27 08:23:40.000000 thermolib-0.3.1/Cargo.lock
+-rw-r--r--   0        0        0     1082 2024-02-20 03:32:56.000000 thermolib-0.3.1/LICENSE
+-rw-r--r--   0        0        0      167 2024-02-20 03:32:56.000000 thermolib-0.3.1/README.md
+-rw-r--r--   0        0        0       76 2024-05-22 09:31:41.000000 thermolib-0.3.1/build.rs
+-rw-r--r--   0        0        0     6045 2024-05-27 08:19:27.000000 thermolib-0.3.1/res/22DimethylButane.json
+-rw-r--r--   0        0        0     5756 2024-05-27 08:19:27.000000 thermolib-0.3.1/res/23DimethylButane.json
+-rw-r--r--   0        0        0     6154 2024-05-27 08:19:27.000000 thermolib-0.3.1/res/3MethylPentane.json
+-rw-r--r--   0        0        0     5573 2024-05-27 08:19:27.000000 thermolib-0.3.1/res/C4F10.json
+-rw-r--r--   0        0        0     5584 2024-05-27 08:19:27.000000 thermolib-0.3.1/res/C5F12.json
+-rw-r--r--   0        0        0     5594 2024-05-27 08:19:27.000000 thermolib-0.3.1/res/C6F14.json
+-rw-r--r--   0        0        0     6177 2024-04-10 07:36:35.000000 thermolib-0.3.1/res/SO2.json
+-rw-r--r--   0        0        0       85 2024-05-27 08:19:27.000000 thermolib-0.3.1/src/bin/thermo.rs
+-rw-r--r--   0        0        0      138 2024-05-27 08:19:27.000000 thermolib-0.3.1/src/bin/thermo.slint
+-rw-r--r--   0        0        0     6284 2024-05-27 08:19:27.000000 thermolib-0.3.1/src/core/core_traits.rs
+-rw-r--r--   0        0        0    27734 2024-05-27 08:19:27.000000 thermolib-0.3.1/src/core/generic_a.rs
+-rw-r--r--   0        0        0      729 2024-05-27 08:19:27.000000 thermolib-0.3.1/src/core/ideal_cv.rs
+-rw-r--r--   0        0        0     6171 2024-05-27 08:19:27.000000 thermolib-0.3.1/src/core/readme.md
+-rw-r--r--   0        0        0      894 2024-05-21 12:58:36.000000 thermolib-0.3.1/src/core/tlerr.rs
+-rw-r--r--   0        0        0      259 2024-05-27 08:19:27.000000 thermolib-0.3.1/src/core.rs
+-rw-r--r--   0        0        0     7673 2024-05-24 13:17:30.000000 thermolib-0.3.1/src/helmholtz/alpha.rs
+-rw-r--r--   0        0        0     4854 2024-05-27 08:19:27.000000 thermolib-0.3.1/src/helmholtz/alpha_i.rs
+-rw-r--r--   0        0        0     8049 2024-05-27 08:19:27.000000 thermolib-0.3.1/src/helmholtz/alpha_r.rs
+-rw-r--r--   0        0        0     2959 2024-05-27 08:19:27.000000 thermolib-0.3.1/src/helmholtz/anc_equ.rs
+-rw-r--r--   0        0        0      250 2024-04-03 11:57:39.000000 thermolib-0.3.1/src/helmholtz.rs
+-rw-r--r--   0        0        0      471 2024-05-22 09:31:41.000000 thermolib-0.3.1/src/lib.rs
+-rw-r--r--   0        0        0     1425 2024-05-27 08:19:27.000000 thermolib-0.3.1/src/pc_saft/alpha.rs
+-rw-r--r--   0        0        0     7501 2024-05-27 08:19:27.000000 thermolib-0.3.1/src/pc_saft/alpha_r.rs
+-rw-r--r--   0        0        0    31367 2024-05-27 08:19:27.000000 thermolib-0.3.1/src/pc_saft/disp.rs
+-rw-r--r--   0        0        0    20494 2024-05-27 08:19:27.000000 thermolib-0.3.1/src/pc_saft/hc.rs
+-rw-r--r--   0        0        0      248 2024-05-22 09:31:41.000000 thermolib-0.3.1/src/pc_saft.rs
+-rw-r--r--   0        0        0     1939 2024-05-22 07:46:25.000000 thermolib-0.3.1/src/pr/density_pr.rs
+-rw-r--r--   0        0        0     9587 2024-05-27 08:19:27.000000 thermolib-0.3.1/src/pr/pr_pure.rs
+-rw-r--r--   0        0        0      155 2024-05-22 09:31:41.000000 thermolib-0.3.1/src/pr.rs
+-rw-r--r--   0        0        0    10013 2024-05-27 08:19:27.000000 thermolib-0.3.1/src/python.rs
+-rw-r--r--   0        0        0      550 2024-05-27 08:19:27.000000 thermolib-0.3.1/tests/find_json.rs
+-rw-r--r--   0        0        0     2020 2024-05-27 08:19:27.000000 thermolib-0.3.1/tests/internals/mod.rs
+-rw-r--r--   0        0        0      406 2024-05-22 08:33:46.000000 thermolib-0.3.1/tests/main.cpp
+-rw-r--r--   0        0        0      747 2024-05-27 08:19:27.000000 thermolib-0.3.1/tests/main.py
+-rw-r--r--   0        0        0   118429 2024-05-22 08:34:33.000000 thermolib-0.3.1/tests/pcsaft.cpp
+-rw-r--r--   0        0        0     5416 2024-05-21 11:39:49.000000 thermolib-0.3.1/tests/pcsaft.h
+-rw-r--r--   0        0        0     8006 2024-05-27 08:19:27.000000 thermolib-0.3.1/tests/test_fluid.rs
+-rw-r--r--   0        0        0      406 2024-03-27 02:49:30.000000 thermolib-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      669 1970-01-01 00:00:00.000000 thermolib-0.3.1/PKG-INFO
```

### Comparing `thermolib-0.3.0/Cargo.toml` & `thermolib-0.3.1/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "thermolib"
 build = "build.rs"
-version = "0.3.0"
+version = "0.3.1"
 edition = "2021"
 license = "MIT"
 repository = "https://github.com/shaw-yu2020/thermolib"
 description = "An open-source library for the calculation of fluid properties"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `thermolib-0.3.0/Cargo.lock` & `thermolib-0.3.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -3620,15 +3620,15 @@
 name = "text-size"
 version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f18aa187839b2bdb1ad2fa35ead8c4c2976b64e4363c386d45ac0f7ee85c9233"
 
 [[package]]
 name = "thermolib"
-version = "0.3.0"
+version = "0.3.1"
 dependencies = [
  "anyhow",
  "pyo3",
  "serde",
  "serde_json",
  "slint",
  "slint-build",
```

### Comparing `thermolib-0.3.0/LICENSE` & `thermolib-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `thermolib-0.3.0/res/SO2.json` & `thermolib-0.3.1/res/SO2.json`

 * *Files identical despite different names*

### Comparing `thermolib-0.3.0/src/core/core_traits.rs` & `thermolib-0.3.1/src/core/core_traits.rs`

 * *Files 14% similar despite different names*

```diff
@@ -64,17 +64,25 @@
     /// > fn rT2D0(&self, _T: f64, _D: f64) -> f64; Equal to =  
     /// > $$T^2\left(\frac{\partial^2a^r}{\partial T^2}\right)_D$$  
     fn rT2D0(&self, _T: f64, _D: f64) -> f64 {
         println!("no implementation for CalcAr::rT2D0(), return 0.0");
         0.0
     }
 }
+/// Settings for fundumental helmholtz equation of state.
+#[allow(non_snake_case)]
+pub trait Setting {
+    fn set_mass_unit(&mut self);
+    fn set_molar_unit(&mut self);
+}
 /// Flash calculation of fundumental helmholtz equation of state.
 #[allow(non_snake_case)]
 pub trait Flash {
+    /// Temperature and Density UNCHECKED
+    fn td_unchecked(&mut self, _T: f64, _D: f64) -> anyhow::Result<()>;
     /// Critical point
     fn c_flash(&mut self) -> anyhow::Result<()>;
     /// Temperature of saturated state
     fn t_flash(&mut self, _Ts: f64) -> anyhow::Result<()>;
     /// Temperature and Density
     fn td_flash(&mut self, _T: f64, _D: f64) -> anyhow::Result<()>;
     /// Temperature and Pressure
@@ -84,50 +92,60 @@
 #[allow(non_snake_case)]
 pub trait Prop {
     /// Temperature
     fn T(&self) -> anyhow::Result<f64>;
     /// Density
     fn D(&self) -> anyhow::Result<f64>;
     /// pressure
-    fn p(&self) -> anyhow::Result<f64>;
-    fn Dp_DT_D(&self) -> anyhow::Result<f64>;
-    fn Dp_DD_T(&self) -> anyhow::Result<f64>;
+    fn p(&mut self) -> anyhow::Result<f64>;
+    fn Dp_DT_D(&mut self) -> anyhow::Result<f64>;
+    fn Dp_DD_T(&mut self) -> anyhow::Result<f64>;
     /// isochoric heat capacity
-    fn cv(&self) -> anyhow::Result<f64>;
+    fn cv(&mut self) -> anyhow::Result<f64>;
     /// isobaric heat capacity
-    fn cp(&self) -> anyhow::Result<f64>;
+    fn cp(&mut self) -> anyhow::Result<f64>;
     /// sound speed
-    fn w(&self) -> anyhow::Result<f64>;
+    fn w(&mut self) -> anyhow::Result<f64>;
     /// entropy
-    fn s(&self) -> anyhow::Result<f64>;
-    fn Ds_DT_D(&self) -> anyhow::Result<f64>;
-    fn Ds_DD_T(&self) -> anyhow::Result<f64>;
-    fn s_res(&self) -> anyhow::Result<f64>;
+    fn s(&mut self) -> anyhow::Result<f64>;
+    fn Ds_DT_D(&mut self) -> anyhow::Result<f64>;
+    fn Ds_DD_T(&mut self) -> anyhow::Result<f64>;
+    fn s_res(&mut self) -> anyhow::Result<f64>;
     /// internal energy
-    fn u(&self) -> anyhow::Result<f64>;
-    fn u_res(&self) -> anyhow::Result<f64>;
+    fn u(&mut self) -> anyhow::Result<f64>;
+    fn u_res(&mut self) -> anyhow::Result<f64>;
     /// enthalpy
-    fn h(&self) -> anyhow::Result<f64>;
-    fn Dh_DT_D(&self) -> anyhow::Result<f64>;
-    fn Dh_DD_T(&self) -> anyhow::Result<f64>;
-    fn h_res(&self) -> anyhow::Result<f64>;
+    fn h(&mut self) -> anyhow::Result<f64>;
+    fn Dh_DT_D(&mut self) -> anyhow::Result<f64>;
+    fn Dh_DD_T(&mut self) -> anyhow::Result<f64>;
+    fn h_res(&mut self) -> anyhow::Result<f64>;
     /// helmholtz energy
-    fn a(&self) -> anyhow::Result<f64>;
-    fn a_res(&self) -> anyhow::Result<f64>;
+    fn a(&mut self) -> anyhow::Result<f64>;
+    fn a_res(&mut self) -> anyhow::Result<f64>;
     /// gibbs energy
-    fn g(&self) -> anyhow::Result<f64>;
-    fn Dg_DT_D(&self) -> anyhow::Result<f64>;
-    fn Dg_DD_T(&self) -> anyhow::Result<f64>;
-    fn g_res(&self) -> anyhow::Result<f64>;
+    fn g(&mut self) -> anyhow::Result<f64>;
+    fn Dg_DT_D(&mut self) -> anyhow::Result<f64>;
+    fn Dg_DD_T(&mut self) -> anyhow::Result<f64>;
+    fn g_res(&mut self) -> anyhow::Result<f64>;
     /// compressibility factor
-    fn Z(&self) -> anyhow::Result<f64>;
+    fn Z(&mut self) -> anyhow::Result<f64>;
     /// second virial coefficient
-    fn B(&self) -> anyhow::Result<f64>;
+    fn B(&mut self) -> anyhow::Result<f64>;
     /// third virial coefficient
-    fn C(&self) -> anyhow::Result<f64>;
+    fn C(&mut self) -> anyhow::Result<f64>;
+    /// isothermal expansion coefficient
+    fn k_T(&mut self) -> anyhow::Result<f64>;
+    /// isentropic expansion coefficient
+    fn k_s(&mut self) -> anyhow::Result<f64>;
+    /// isothermal compressibility
+    fn kappa_T(&mut self) -> anyhow::Result<f64>;
+    /// isentropic compressibility
+    fn kappa_s(&mut self) -> anyhow::Result<f64>;
     /// vapor pressure
-    fn ps(&self) -> anyhow::Result<f64>;
+    fn ps(&mut self) -> anyhow::Result<f64>;
     /// saturated gas density
     fn Dgs(&self) -> anyhow::Result<f64>;
     /// saturated liquid density
     fn Dls(&self) -> anyhow::Result<f64>;
+    /// enthalpy of evaporation
+    fn h_evap(&mut self) -> anyhow::Result<f64>;
 }
```

### Comparing `thermolib-0.3.0/src/core/ideal_cv.rs` & `thermolib-0.3.1/src/core/ideal_cv.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 use super::CalcAi;
 /// isochoric heat capacity of ideal gas
 /// used to calculate ideal helmholtz energy
+#[derive(Clone)]
 pub struct IdealCv {}
 #[allow(non_snake_case)]
 impl CalcAi for IdealCv {
     /// > fn iT0(&self, _T: f64) -> f64; Equal to =  
     /// > $$a^i\left(T,D\right)-RT\ln D$$  
     fn iT0(&self, _T: f64) -> f64 {
         0.0
```

### Comparing `thermolib-0.3.0/src/core/readme.md` & `thermolib-0.3.1/src/core/readme.md`

 * *Files 12% similar despite different names*

```diff
@@ -168,7 +168,24 @@
 > +D\left(\frac{\partial a^r}{\partial D}\right)_T$$
 
 > $$B
 > =\frac{1}{RT}\left(\frac{\partial a^r}{\partial D}\right)_T$$
 
 > $$C
 > =\frac{1}{RT}\left(\frac{\partial^2a^r}{\partial D^2}\right)_T$$
+
+> $$k_T
+> =-\frac{v}{p}\left(\frac{\partial p}{\partial v}\right)_T
+> =\frac{\rho}{p}\left(\frac{\partial p}{\partial\rho}\right)_T$$
+
+> $$k_s
+> =-\frac{v}{p}\left(\frac{\partial p}{\partial v}\right)_s
+> =\frac{\rho w^2}{p}$$
+
+> $$\kappa_T
+> =-\frac{1}{v}\left(\frac{\partial v}{\partial p}\right)_T
+> =\frac{1}{\rho}\left(\frac{\partial p}{\partial\rho}\right)_T^{-1}$$
+
+> $$\kappa_s
+> =-\frac{1}{v}\left(\frac{\partial v}{\partial p}\right)_s
+> =\frac{1}{\rho w^2}$$
+
```

### Comparing `thermolib-0.3.0/src/core/tlerr.rs` & `thermolib-0.3.1/src/core/tlerr.rs`

 * *Files identical despite different names*

### Comparing `thermolib-0.3.0/src/helmholtz/alpha.rs` & `thermolib-0.3.1/src/helmholtz/alpha.rs`

 * *Files identical despite different names*

### Comparing `thermolib-0.3.0/src/helmholtz/alpha_i.rs` & `thermolib-0.3.1/src/helmholtz/alpha_i.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 use crate::core::CalcAi;
 use serde::{Deserialize, Serialize};
 /// Partial derivatives of ideal polynomial term
-#[derive(Serialize, Deserialize, Debug)]
+#[derive(Serialize, Deserialize, Debug, Clone)]
 struct PolynomialTerm {
     is_alpha: bool,
     a: f64,
     t: f64,
 }
 #[allow(non_snake_case)]
 impl PolynomialTerm {
@@ -34,15 +34,15 @@
             -self.a * self.t * (self.t + 1.0) / (Tr / T).powf(self.t)
         } else {
             -self.a * T.powf(self.t)
         }
     }
 }
 /// Partial derivatives of ideal plank einstein term
-#[derive(Serialize, Deserialize, Debug)]
+#[derive(Serialize, Deserialize, Debug, Clone)]
 struct PlankEinsteinTerm {
     is_alpha: bool,
     v: f64,
     b: f64,
 }
 #[allow(non_snake_case)]
 impl PlankEinsteinTerm {
@@ -66,20 +66,22 @@
         let bitau = if self.is_alpha { self.b } else { self.b / Tr } * Tr / T;
         let exp_bitau = (-bitau).exp();
         -self.v * exp_bitau * (bitau / (1.0 - exp_bitau)).powi(2)
     }
 }
 /// Partial derivatives of ideal helmholtz equation of state
 #[allow(non_snake_case)]
-#[derive(Serialize, Deserialize, Debug)]
+#[derive(Serialize, Deserialize, Debug, Clone)]
 pub struct AlphaI {
     a_1: f64,
     a_tau: f64,
     a_lntau: f64,
+    #[serde(default)]
     poly_terms: Vec<PolynomialTerm>,
+    #[serde(default)]
     pe_terms: Vec<PlankEinsteinTerm>,
     Tc: f64,
     Dc: f64,
     R: f64,
 }
 #[allow(non_snake_case)]
 impl AlphaI {
```

### Comparing `thermolib-0.3.0/src/helmholtz/alpha_r.rs` & `thermolib-0.3.1/src/helmholtz/alpha_r.rs`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 use serde::{Deserialize, Serialize};
 /// No implemention for derivatives
 fn no_implementation(flag: &str, d: i32) -> f64 {
     println!("no implementation for {}{}", flag, d);
     0.0
 }
 /// Partial derivatives of residual polynomial term
-#[derive(Serialize, Deserialize, Debug)]
+#[derive(Serialize, Deserialize, Debug, Clone)]
 struct PolynomialTerm {
     n: f64,
     d: f64,
     t: f64,
 }
 impl PolynomialTerm {
     /// Equal to tau^(dtau) * delta(ddelta) * AlpharDtauDdelta
@@ -28,15 +28,15 @@
             _ => no_implementation("AlpharPT::Ddelta", ddelta),
         }) * self.n
             * delta.powf(self.d)
             * tau.powf(self.t)
     }
 }
 /// Partial derivatives of residual exponential term
-#[derive(Serialize, Deserialize, Debug)]
+#[derive(Serialize, Deserialize, Debug, Clone)]
 struct ExponentialTerm {
     n: f64,
     d: f64,
     t: f64,
     l: f64,
 }
 impl ExponentialTerm {
@@ -59,15 +59,15 @@
         }) * self.n
             * delta.powf(self.d)
             * tau.powf(self.t)
             * (-delta.powf(self.l)).exp()
     }
 }
 /// Partial derivatives of residual gaussian term
-#[derive(Serialize, Deserialize, Debug)]
+#[derive(Serialize, Deserialize, Debug, Clone)]
 struct GaussianTerm {
     n: f64,
     d: f64,
     t: f64,
     eta: f64,
     epsilon: f64,
     beta: f64,
@@ -100,15 +100,15 @@
             * delta.powf(self.d)
             * tau.powf(self.t)
             * (-self.eta * (delta - self.epsilon).powi(2) - self.beta * (tau - self.gamma).powi(2))
                 .exp()
     }
 }
 #[allow(non_snake_case)]
-#[derive(Serialize, Deserialize, Debug)]
+#[derive(Serialize, Deserialize, Debug, Clone)]
 pub struct ResidualTerms {
     poly_terms: Vec<PolynomialTerm>,
     exp_terms: Vec<ExponentialTerm>,
     gauss_terms: Vec<GaussianTerm>,
 }
 impl ResidualTerms {
     /// calculate tau^(dT) * delta^(dD) * alphar_dtau_delta
@@ -127,15 +127,15 @@
                 .iter()
                 .map(|term| term.calc_dtau_ddelta((dtau, ddelta), tau, delta))
                 .sum::<f64>()
     }
 }
 /// Partial derivatives of residual helmholtz equation of state
 #[allow(non_snake_case)]
-#[derive(Serialize, Deserialize, Debug)]
+#[derive(Serialize, Deserialize, Debug, Clone)]
 pub struct AlphaR {
     alphar: ResidualTerms,
     ps: PsEqu,
     rhogs: DgsEqu,
     rhols: DlsEqu,
     omega: f64,
     Tc: f64,
```

### Comparing `thermolib-0.3.0/src/helmholtz/anc_equ.rs` & `thermolib-0.3.1/src/helmholtz/anc_equ.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 use serde::{Deserialize, Serialize};
 /// Ancillary Equations
 /// + Vapor Pressure Equation
 /// + Saturated Gas Density Equation
 /// + Saturated Liquid Density Equation
-#[derive(Serialize, Deserialize, Debug)]
+#[derive(Serialize, Deserialize, Debug, Clone)]
 struct AncEquTerm {
     n: f64, // coefficients
     t: f64, // exponents
 }
 impl AncEquTerm {
     fn calc(&self, theta: f64) -> f64 {
         self.n * theta.powf(self.t)
     }
 }
-#[derive(Serialize, Deserialize, Debug)]
+#[derive(Serialize, Deserialize, Debug, Clone)]
 pub struct PsEqu {
     flag: i32,
     terms: Vec<AncEquTerm>,
 }
 impl PsEqu {
     #[allow(non_snake_case)]
     pub fn calc(&self, T: f64, Tr: f64, Pr: f64) -> f64 {
@@ -33,15 +33,15 @@
             _ => {
                 println!("no flag={} in vapor_pressure_equation", self.flag);
                 1.0
             }
         })
     }
 }
-#[derive(Serialize, Deserialize, Debug)]
+#[derive(Serialize, Deserialize, Debug, Clone)]
 pub struct DgsEqu {
     flag: i32,
     terms: Vec<AncEquTerm>,
 }
 impl DgsEqu {
     #[allow(non_snake_case)]
     pub fn calc(&self, T: f64, Tr: f64, Dr: f64) -> f64 {
@@ -63,15 +63,15 @@
             _ => {
                 println!("no flag={} in saturated_gas_density_equation", self.flag);
                 1.0
             }
         })
     }
 }
-#[derive(Serialize, Deserialize, Debug)]
+#[derive(Serialize, Deserialize, Debug, Clone)]
 pub struct DlsEqu {
     flag: i32,
     terms: Vec<AncEquTerm>,
 }
 impl DlsEqu {
     #[allow(non_snake_case)]
     pub fn calc(&self, T: f64, Tr: f64, Dr: f64) -> f64 {
```

### Comparing `thermolib-0.3.0/src/pc_saft/alpha_r.rs` & `thermolib-0.3.1/src/pc_saft/alpha_r.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 use super::{AlphaDisp, AlphaHC, NA};
 use crate::core::CalcAr;
+#[derive(Clone)]
 #[allow(non_snake_case)]
 pub struct AlphaR {
     disp: AlphaDisp,
     hc: AlphaHC,
     R: f64,
     M: f64,
 }
```

### Comparing `thermolib-0.3.0/src/pc_saft/disp.rs` & `thermolib-0.3.1/src/pc_saft/disp.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 use std::f64::consts::PI;
+#[derive(Clone)]
 pub struct AlphaDisp {
     m: f64,
     sigma: f64,
     epsilon: f64,
 }
 #[allow(non_snake_case)]
 impl AlphaDisp {
```

### Comparing `thermolib-0.3.0/src/pc_saft/hc.rs` & `thermolib-0.3.1/src/pc_saft/hc.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 use std::f64::consts::PI;
+#[derive(Clone)]
 pub struct AlphaHC {
     m: f64,
     sigma: f64,
     epsilon: f64,
 }
 #[allow(non_snake_case)]
 impl AlphaHC {
```

### Comparing `thermolib-0.3.0/src/pr/density_pr.rs` & `thermolib-0.3.1/src/pr/density_pr.rs`

 * *Files identical despite different names*

### Comparing `thermolib-0.3.0/src/pr/pr_pure.rs` & `thermolib-0.3.1/src/pr/pr_pure.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 use crate::core::{CalcAr, GenericA, IdealCv, Phase, TlErr};
 use anyhow::anyhow;
 /// residual fundumental helmholtz equation of state
 /// transformed from pr equation of state
+#[derive(Clone)]
 #[allow(non_snake_case)]
 pub struct PrAr {
     R: f64,
     Tc: f64,
     ac: f64,
     bc: f64, // b=bc
     kappa: f64,
```

### Comparing `thermolib-0.3.0/src/python.rs` & `thermolib-0.3.1/src/python.rs`

 * *Files 8% similar despite different names*

```diff
@@ -77,191 +77,191 @@
     fn D(&self) -> anyhow::Result<f64> {
         match &self.model {
             Models::Helmholtz(model) => model.D(),
             Models::PcSaft(model) => model.D(),
             Models::Pr(model) => model.D(),
         }
     }
-    fn p(&self) -> anyhow::Result<f64> {
-        match &self.model {
+    fn p(&mut self) -> anyhow::Result<f64> {
+        match &mut self.model {
             Models::Helmholtz(model) => model.p(),
             Models::PcSaft(model) => model.p(),
             Models::Pr(model) => model.p(),
         }
     }
-    fn Dp_DT_D(&self) -> anyhow::Result<f64> {
-        match &self.model {
+    fn Dp_DT_D(&mut self) -> anyhow::Result<f64> {
+        match &mut self.model {
             Models::Helmholtz(model) => model.Dp_DT_D(),
             Models::PcSaft(model) => model.Dp_DT_D(),
             Models::Pr(model) => model.Dp_DT_D(),
         }
     }
-    fn Dp_DD_T(&self) -> anyhow::Result<f64> {
-        match &self.model {
+    fn Dp_DD_T(&mut self) -> anyhow::Result<f64> {
+        match &mut self.model {
             Models::Helmholtz(model) => model.Dp_DD_T(),
             Models::PcSaft(model) => model.Dp_DD_T(),
             Models::Pr(model) => model.Dp_DD_T(),
         }
     }
-    fn cv(&self) -> anyhow::Result<f64> {
-        match &self.model {
+    fn cv(&mut self) -> anyhow::Result<f64> {
+        match &mut self.model {
             Models::Helmholtz(model) => model.cv(),
             Models::PcSaft(model) => model.cv(),
             Models::Pr(model) => model.cv(),
         }
     }
-    fn cp(&self) -> anyhow::Result<f64> {
-        match &self.model {
+    fn cp(&mut self) -> anyhow::Result<f64> {
+        match &mut self.model {
             Models::Helmholtz(model) => model.cp(),
             Models::PcSaft(model) => model.cp(),
             Models::Pr(model) => model.cp(),
         }
     }
-    fn w(&self) -> anyhow::Result<f64> {
-        match &self.model {
+    fn w(&mut self) -> anyhow::Result<f64> {
+        match &mut self.model {
             Models::Helmholtz(model) => model.w(),
             Models::PcSaft(model) => model.w(),
             Models::Pr(model) => model.w(),
         }
     }
-    fn s(&self) -> anyhow::Result<f64> {
-        match &self.model {
+    fn s(&mut self) -> anyhow::Result<f64> {
+        match &mut self.model {
             Models::Helmholtz(model) => model.s(),
             Models::PcSaft(model) => model.s(),
             Models::Pr(model) => model.s(),
         }
     }
-    fn Ds_DT_D(&self) -> anyhow::Result<f64> {
-        match &self.model {
+    fn Ds_DT_D(&mut self) -> anyhow::Result<f64> {
+        match &mut self.model {
             Models::Helmholtz(model) => model.Ds_DT_D(),
             Models::PcSaft(model) => model.Ds_DT_D(),
             Models::Pr(model) => model.Ds_DT_D(),
         }
     }
-    fn Ds_DD_T(&self) -> anyhow::Result<f64> {
-        match &self.model {
+    fn Ds_DD_T(&mut self) -> anyhow::Result<f64> {
+        match &mut self.model {
             Models::Helmholtz(model) => model.Ds_DD_T(),
             Models::PcSaft(model) => model.Ds_DD_T(),
             Models::Pr(model) => model.Ds_DD_T(),
         }
     }
-    fn s_res(&self) -> anyhow::Result<f64> {
-        match &self.model {
+    fn s_res(&mut self) -> anyhow::Result<f64> {
+        match &mut self.model {
             Models::Helmholtz(model) => model.s_res(),
             Models::PcSaft(model) => model.s_res(),
             Models::Pr(model) => model.s_res(),
         }
     }
-    fn u(&self) -> anyhow::Result<f64> {
-        match &self.model {
+    fn u(&mut self) -> anyhow::Result<f64> {
+        match &mut self.model {
             Models::Helmholtz(model) => model.u(),
             Models::PcSaft(model) => model.u(),
             Models::Pr(model) => model.u(),
         }
     }
-    fn u_res(&self) -> anyhow::Result<f64> {
-        match &self.model {
+    fn u_res(&mut self) -> anyhow::Result<f64> {
+        match &mut self.model {
             Models::Helmholtz(model) => model.u_res(),
             Models::PcSaft(model) => model.u_res(),
             Models::Pr(model) => model.u_res(),
         }
     }
-    fn h(&self) -> anyhow::Result<f64> {
-        match &self.model {
+    fn h(&mut self) -> anyhow::Result<f64> {
+        match &mut self.model {
             Models::Helmholtz(model) => model.h(),
             Models::PcSaft(model) => model.h(),
             Models::Pr(model) => model.h(),
         }
     }
-    fn Dh_DT_D(&self) -> anyhow::Result<f64> {
-        match &self.model {
+    fn Dh_DT_D(&mut self) -> anyhow::Result<f64> {
+        match &mut self.model {
             Models::Helmholtz(model) => model.Dh_DT_D(),
             Models::PcSaft(model) => model.Dh_DT_D(),
             Models::Pr(model) => model.Dh_DT_D(),
         }
     }
-    fn Dh_DD_T(&self) -> anyhow::Result<f64> {
-        match &self.model {
+    fn Dh_DD_T(&mut self) -> anyhow::Result<f64> {
+        match &mut self.model {
             Models::Helmholtz(model) => model.Dh_DD_T(),
             Models::PcSaft(model) => model.Dh_DD_T(),
             Models::Pr(model) => model.Dh_DD_T(),
         }
     }
-    fn h_res(&self) -> anyhow::Result<f64> {
-        match &self.model {
+    fn h_res(&mut self) -> anyhow::Result<f64> {
+        match &mut self.model {
             Models::Helmholtz(model) => model.h_res(),
             Models::PcSaft(model) => model.h_res(),
             Models::Pr(model) => model.h_res(),
         }
     }
-    fn a(&self) -> anyhow::Result<f64> {
-        match &self.model {
+    fn a(&mut self) -> anyhow::Result<f64> {
+        match &mut self.model {
             Models::Helmholtz(model) => model.a(),
             Models::PcSaft(model) => model.a(),
             Models::Pr(model) => model.a(),
         }
     }
-    fn a_res(&self) -> anyhow::Result<f64> {
-        match &self.model {
+    fn a_res(&mut self) -> anyhow::Result<f64> {
+        match &mut self.model {
             Models::Helmholtz(model) => model.a_res(),
             Models::PcSaft(model) => model.a_res(),
             Models::Pr(model) => model.a_res(),
         }
     }
-    fn g(&self) -> anyhow::Result<f64> {
-        match &self.model {
+    fn g(&mut self) -> anyhow::Result<f64> {
+        match &mut self.model {
             Models::Helmholtz(model) => model.g(),
             Models::PcSaft(model) => model.g(),
             Models::Pr(model) => model.g(),
         }
     }
-    fn Dg_DT_D(&self) -> anyhow::Result<f64> {
-        match &self.model {
+    fn Dg_DT_D(&mut self) -> anyhow::Result<f64> {
+        match &mut self.model {
             Models::Helmholtz(model) => model.Dg_DT_D(),
             Models::PcSaft(model) => model.Dg_DT_D(),
             Models::Pr(model) => model.Dg_DT_D(),
         }
     }
-    fn Dg_DD_T(&self) -> anyhow::Result<f64> {
-        match &self.model {
+    fn Dg_DD_T(&mut self) -> anyhow::Result<f64> {
+        match &mut self.model {
             Models::Helmholtz(model) => model.Dg_DD_T(),
             Models::PcSaft(model) => model.Dg_DD_T(),
             Models::Pr(model) => model.Dg_DD_T(),
         }
     }
-    fn g_res(&self) -> anyhow::Result<f64> {
-        match &self.model {
+    fn g_res(&mut self) -> anyhow::Result<f64> {
+        match &mut self.model {
             Models::Helmholtz(model) => model.g_res(),
             Models::PcSaft(model) => model.g_res(),
             Models::Pr(model) => model.g_res(),
         }
     }
-    fn Z(&self) -> anyhow::Result<f64> {
-        match &self.model {
+    fn Z(&mut self) -> anyhow::Result<f64> {
+        match &mut self.model {
             Models::Helmholtz(model) => model.Z(),
             Models::PcSaft(model) => model.Z(),
             Models::Pr(model) => model.Z(),
         }
     }
-    fn B(&self) -> anyhow::Result<f64> {
-        match &self.model {
+    fn B(&mut self) -> anyhow::Result<f64> {
+        match &mut self.model {
             Models::Helmholtz(model) => model.B(),
             Models::PcSaft(model) => model.B(),
             Models::Pr(model) => model.B(),
         }
     }
-    fn C(&self) -> anyhow::Result<f64> {
-        match &self.model {
+    fn C(&mut self) -> anyhow::Result<f64> {
+        match &mut self.model {
             Models::Helmholtz(model) => model.C(),
             Models::PcSaft(model) => model.C(),
             Models::Pr(model) => model.C(),
         }
     }
-    fn ps(&self) -> anyhow::Result<f64> {
-        match &self.model {
+    fn ps(&mut self) -> anyhow::Result<f64> {
+        match &mut self.model {
             Models::Helmholtz(model) => model.ps(),
             Models::PcSaft(model) => model.ps(),
             Models::Pr(model) => model.ps(),
         }
     }
     fn Dgs(&self) -> anyhow::Result<f64> {
         match &self.model {
```

### Comparing `thermolib-0.3.0/tests/main.py` & `thermolib-0.3.1/tests/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,13 +16,13 @@
 pyargs = {"m": m, "s": s, "e": e}
 
 t = 300  # K
 den = 6.02214076e-4
 den = den / (6.02214076e23) * 1e30
 
 ps = flashTQ(t, 0.5, x, pyargs)
-print("ps of ethane at {} K : {} Pa".format(t, ps))
+print("ps of ethane at {} K : {} Pa".format(t, ps[0]))
 
 ares = pcsaft_ares(t, den, x, pyargs)
 print("ares of ethane at {} K {} mol/m3 : {} J/mol".format(t, den, ares))
 p = pcsaft_p(t, den, x, pyargs)
 print("p of ethane at {} K {} mol/m3 : {} Pa".format(t, den, p))
```

### Comparing `thermolib-0.3.0/tests/pcsaft.cpp` & `thermolib-0.3.1/tests/pcsaft.cpp`

 * *Files identical despite different names*

### Comparing `thermolib-0.3.0/tests/pcsaft.h` & `thermolib-0.3.1/tests/pcsaft.h`

 * *Files identical despite different names*

### Comparing `thermolib-0.3.0/tests/test_json.rs` & `thermolib-0.3.1/tests/find_json.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 /// Test all fluid.json
 use std::fs;
 use std::path::Path;
 #[test]
-fn test_json() {
+fn find_json() {
     let res_path = Path::new(env!("CARGO_MANIFEST_DIR")).join("res");
     let res_dir = fs::read_dir(res_path);
     let mut vec_file: Vec<String> = vec![];
     for entry in res_dir.expect("no res") {
         if let Ok(entry) = entry {
             if entry.file_name().to_string_lossy().contains(".json") {
                 vec_file.push(entry.file_name().to_string_lossy().to_string());
```

### Comparing `thermolib-0.3.0/PKG-INFO` & `thermolib-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: thermolib
-Version: 0.3.0
+Version: 0.3.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: An open-source library for the calculation of fluid properties
 License: MIT
 Requires-Python: >=3.8
```

