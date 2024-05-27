# Comparing `tmp/quantylf-0.0.9.tar.gz` & `tmp/quantylf-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantylf-0.0.9.tar", last modified: Tue May  7 19:26:01 2024, max compression
+gzip compressed data, was "quantylf-0.1.0.tar", last modified: Mon May 27 16:55:13 2024, max compression
```

## Comparing `quantylf-0.0.9.tar` & `quantylf-0.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:26:01.980629 quantylf-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-07 19:25:57.000000 quantylf-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-07 19:25:57.000000 quantylf-0.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-07 19:26:01.980629 quantylf-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-07 19:25:57.000000 quantylf-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-07 19:25:57.000000 quantylf-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-07 19:26:01.984629 quantylf-0.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:26:01.976629 quantylf-0.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:26:01.980629 quantylf-0.0.9/src/QuantyLF/
--rw-r--r--   0 runner    (1001) docker     (127)    18703 2024-05-07 19:25:57.000000 quantylf-0.0.9/src/QuantyLF/QuantyLF.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:25:57.000000 quantylf-0.0.9/src/QuantyLF/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:26:01.980629 quantylf-0.0.9/src/QuantyLF/cases/
--rw-r--r--   0 runner    (1001) docker     (127)    20672 2024-05-07 19:25:57.000000 quantylf-0.0.9/src/QuantyLF/cases/D3h_3d.lua
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-07 19:25:57.000000 quantylf-0.0.9/src/QuantyLF/cases/D3h_3d.txt
--rw-r--r--   0 runner    (1001) docker     (127)    19016 2024-05-07 19:25:57.000000 quantylf-0.0.9/src/QuantyLF/cases/Oh_3d.lua
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-07 19:25:57.000000 quantylf-0.0.9/src/QuantyLF/cases/Oh_3d.txt
--rw-r--r--   0 runner    (1001) docker     (127)    19083 2024-05-07 19:25:57.000000 quantylf-0.0.9/src/QuantyLF/cases/Td_3d.lua
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-07 19:25:57.000000 quantylf-0.0.9/src/QuantyLF/cases/Td_3d.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:26:01.980629 quantylf-0.0.9/src/QuantyLF/cases/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-07 19:25:57.000000 quantylf-0.0.9/src/QuantyLF/cases/utils/slater_integrals.lua
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:26:01.980629 quantylf-0.0.9/src/QuantyLF.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-07 19:26:01.000000 quantylf-0.0.9/src/QuantyLF.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-07 19:26:01.000000 quantylf-0.0.9/src/QuantyLF.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 19:26:01.000000 quantylf-0.0.9/src/QuantyLF.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-07 19:26:01.000000 quantylf-0.0.9/src/QuantyLF.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 19:26:01.000000 quantylf-0.0.9/src/QuantyLF.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:55:13.040406 quantylf-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-27 16:55:08.000000 quantylf-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-27 16:55:08.000000 quantylf-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-05-27 16:55:13.040406 quantylf-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-05-27 16:55:08.000000 quantylf-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-27 16:55:08.000000 quantylf-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-27 16:55:13.040406 quantylf-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:55:13.036406 quantylf-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:55:13.036406 quantylf-0.1.0/src/QuantyLF/
+-rw-r--r--   0 runner    (1001) docker     (127)    19561 2024-05-27 16:55:08.000000 quantylf-0.1.0/src/QuantyLF/QuantyLF.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:55:08.000000 quantylf-0.1.0/src/QuantyLF/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:55:13.040406 quantylf-0.1.0/src/QuantyLF/cases/
+-rw-r--r--   0 runner    (1001) docker     (127)    20734 2024-05-27 16:55:08.000000 quantylf-0.1.0/src/QuantyLF/cases/D3h_3d.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-27 16:55:08.000000 quantylf-0.1.0/src/QuantyLF/cases/D3h_3d.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19016 2024-05-27 16:55:08.000000 quantylf-0.1.0/src/QuantyLF/cases/Oh_3d.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-27 16:55:08.000000 quantylf-0.1.0/src/QuantyLF/cases/Oh_3d.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19083 2024-05-27 16:55:08.000000 quantylf-0.1.0/src/QuantyLF/cases/Td_3d.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-27 16:55:08.000000 quantylf-0.1.0/src/QuantyLF/cases/Td_3d.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:55:13.040406 quantylf-0.1.0/src/QuantyLF/cases/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-27 16:55:08.000000 quantylf-0.1.0/src/QuantyLF/cases/utils/slater_integrals.lua
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:55:13.040406 quantylf-0.1.0/src/QuantyLF.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-05-27 16:55:13.000000 quantylf-0.1.0/src/QuantyLF.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-27 16:55:13.000000 quantylf-0.1.0/src/QuantyLF.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:55:13.000000 quantylf-0.1.0/src/QuantyLF.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-27 16:55:13.000000 quantylf-0.1.0/src/QuantyLF.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-27 16:55:13.000000 quantylf-0.1.0/src/QuantyLF.egg-info/top_level.txt
```

### Comparing `quantylf-0.0.9/LICENSE` & `quantylf-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quantylf-0.0.9/setup.cfg` & `quantylf-0.1.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = QuantyLF
-version = 0.0.9
+version = 0.1.0
 author = Carl Magnus Meier
 author_email = magnus.meier@outook.de
 description = QuantyLF is a libary to help manage Liegand Field simulations in Quanty.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CMM02/XPlotLib
 classifiers = 
@@ -16,14 +16,15 @@
 package_dir = 
 	= src
 include_package_data = True
 packages = find:
 python_requires = >=3.10
 install_requires = 
 	numpy
+	matplotlib
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 dev = 
 	pytest
```

### Comparing `quantylf-0.0.9/src/QuantyLF/QuantyLF.py` & `quantylf-0.1.0/src/QuantyLF/QuantyLF.py`

 * *Files 8% similar despite different names*

```diff
@@ -212,16 +212,16 @@
             
             #fit scaling of the RIXS spectra to get best agreement
             #with experiment (linear least squares fit, single scaling for all)
             #to do this, concatenate all the RIXS spectra
             calcRIXS2 = np.copy(self.expRIXS)
             for i in range(len(calcRIXS2[0,:])-1):
                 calcRIXS2[:,i+1] = np.interp(self.expRIXS[:,0],calcRIXS[:,0],calcRIXS[:,i+1])
-                calcRIXSCat = np.copy(calcRIXS2[:,1])
-                expRIXSCat = np.copy(self.expRIXS[:,1])
+            calcRIXSCat = np.copy(calcRIXS2[:,1])
+            expRIXSCat = np.copy(self.expRIXS[:,1])
             for i in range(len(calcRIXS[0,:])-2):
                 calcRIXSCat = np.hstack((calcRIXSCat,calcRIXS2[:,i+2]))
                 expRIXSCat = np.hstack((expRIXSCat,self.expRIXS[:,i+2]))
             
             #do the linear least squares fit
             amp,res = nnls(np.array(calcRIXSCat[:,None]),expRIXSCat)
 
@@ -292,19 +292,24 @@
         print(res.params)
 
 
 
     """
     Configure the edge jump for the XAS calculation. The edge jump is modelled as a arctan function.
 
-    Parameters:
-    edge_jumps: List of edge jumps. Each element in the list is a list of 3 elements: [position, jump, slope]
-    x_range: The range of x values to model the edge jump over
-    y_offset: The y offset of the edge jump
-    display: If True, the edge jump will be displayed along with the experimental XASs
+    Parameters
+    ----------
+    edge_jumps: list of 3-element lists
+        List of edge jumps. Each element in the list is a list of 3 elements: [position, jump, slope]
+    x_range: list of floats
+        The range of x values to model the edge jump over
+    y_offset: float, optional
+        The y offset of the edge jump
+    display: bool, optional
+        If True, the edge jump will be displayed along with the experimental XASs
     """
     def config_edge_jump(self, edge_jumps, x_range, y_offset=0, display=False):
         x_range = np.linspace(x_range[0], x_range[1], math.ceil((max(x_range)-min(x_range))/0.1))
         edge_jump_y = [y_offset] * len(x_range)
         for i in range(len(edge_jumps)):
             cur_jump = edge_jumps[i]
             edge_jump_y += self.__edge_jump__(x_range, cur_jump[0], cur_jump[1], cur_jump[2])
@@ -319,35 +324,37 @@
                 plt.plot(self.expXAS[:,0], self.expXAS[:,1])
             plt.plot(x_range, edge_jump_y)
             plt.show()
 
     """
     Return the available cases for which the Quanty calculations are available
 
-    ----------------
-    Returns:
+    Returns
+    -------
     List of available cases
     """
     def available_cases(self):
         base_path = impresources.files(cases)
         available_cases = []
         for file in base_path.iterdir():
             if file.suffix == '.lua':
                 available_cases.append(file.stem)
 
         return available_cases
     
 
     """
-    Load a Quanty case)
+    Load a Quanty case
 
-    ----------------
-    Parameters:
-    case: Name of the case to load (pattern: {point_group}_{orbitals})
-    manual: If True, the manual for the case is displayed (list of parameters available for fitting)
+    Parameters
+    ----------
+    case: str
+        Name of the case to load (pattern: {point_group}_{orbitals})
+    manual: bool, optional
+        If True, the manual for the case is displayed (list of parameters available for fitting)
     """    
     def load_case(self, case, manual=False):
         base_path = impresources.files(cases)
         case_path = base_path / f"{case}.lua"
         if not case_path.exists():
             raise ValueError(f"Case {case} not found")
         self.quanty_file = case_path
@@ -363,34 +370,39 @@
                 print(f"Case {case} loaded, but no manual available")
             
 
 
     """
     Load a custom Quanty case from a file
 
-    ----------------
-    Parameters:
-    case_file: Path to the Quanty case file
+    Parameters
+    ----------
+    case_file: str
+        Path to the Quanty case file
     """
     def load_custom_case(self, case_file):
         if not isfile(case_file):
             raise ValueError(f"File {case_file} not found")
         self.quanty_file = case_file
 
 
 
     """
     Add a parameter to the model
 
-    ----------------
-    Parameters:
-    name: Name of the parameter
-    init_val: Initial value of the parameter
-    interv: List of two values, lower and upper bounds of the parameter
-    from_file: If True (default True), the parameter is read from a file (file value overrides init_val)
+    Parameters
+    ----------
+    name: str
+        Name of the parameter
+    init_val: float
+        Initial value of the parameter
+    interv: list of 2 floats, optional
+        List of two values, lower and upper bounds of the parameter
+    from_file: bool, optional
+        If True (default True), the parameter is read from a file (file value overrides init_val)
     """
     def add_par(self, name, init_val, interv = None, from_file = True):
         if interv and (interv[1] - interv[0]) < 0:
             raise ValueError("Upper bound of parameter should be greater than lower bound")
         if interv and (init_val < interv[0] or init_val > interv[1]):
             raise ValueError("Initial value of parameter should be within the bounds")
 
@@ -406,89 +418,106 @@
                 init_val = self.file_par_dict[name] if from_file else init_val
         self.par_list.append([name, init_val, low, high, 1 if interv else 0])
 
 
     """
     Add broadening to the XAS or RIXS data
 
-    ----------------
-    Parameters:
-    type: "XAS" or "RIXS"
-    gamma: Guassian broadening parameter
-    lorenzians: List of lorenzian broadening parameters (center, width)
+    Parameters
+    ----------
+    type: str
+        "XAS" or "RIXS"
+    lorenzians: list of 2-element lists
+        List of lorenzian broadening parameters (center, width)
+    gamma: float, optional
+        Guassian broadening parameter
     """
     def add_broadening(self, type, lorenzians, gamma=0):
         self.add_par(type + "_Gamma", gamma)
         for lorenzian in lorenzians:
             val = f'{lorenzian[0]} {lorenzian[1]}'
             self.add_par(type + "_Broad", val, from_file=False)
 
     """
     Fit the parameters of the model to the experimental data
 
-    ----------------
-    Parameters:
-    mode: "XAS" or "RIXS". If "XAS", only the XAS data is fitted. If "RIXS", both XAS and RIXS data is fitted
+    Parameters
+    ----------
+    mode: str
+        "XAS" or "RIXS". If "XAS", only the XAS data is fitted. If "RIXS", both XAS and RIXS data is fitted
     """
     def fit(self, type):        
         self.__fit_pars__(type)
 
     """
     Load the experimental XAS data from a file (no header, two columns: energy, intensity)
 
-    ----------------
-    Parameters:
-    path: Path to the file containing the experimental XAS data
+    Parameters
+    ----------
+    path: str
+        Path to the file containing the experimental XAS data
     """
     def load_exp_xas(self, path):
         self.expXAS = np.loadtxt(path)
 
 
     """
     Load the experimental RIXS data from a file (no header, first row: resonance energies, rest of the rows: energy, intensity)
 
-    ----------------
-    Parameters:
-    path: Path to the file containing the experimental RIXS data
-    RIXS_energies: List of resonance energies for which the RIXS data is available
+    Parameters
+    ----------
+    path: str   
+        Path to the file containing the experimental RIXS data
+    RIXS_energies: list of floats
+        List of resonance energies for which the RIXS data is available
     """
     def load_exp_rixs(self, path, RIXS_energies):        
-        for RIXS_energy in RIXS_energies:
-            self.add_par("RIXS",RIXS_energy,from_file=False)
-        
         #load exp RIXS. For experimental, the first row are the resonance energies
         expRIXS = np.loadtxt(path)
+        energies = expRIXS[0,:]
+        if energies[0] != 0:
+            raise ValueError("First value of the first row should be 0, as it is the energy axis for the RIXS data")
+        for i in range(len(RIXS_energies)):
+            if RIXS_energies[i] != energies[i+1]:
+                raise ValueError(f"Resonant energy {RIXS_energies[i]} not found in the experimental RIXS data. First row should contain the resonance energies")
+
+        for RIXS_energy in RIXS_energies:
+            self.add_par("RIXS",RIXS_energy,from_file=False)
         
         #trim the exp RIXS just to have the columns with resonant energies we are calculating
         indices = [0] #0th column is energy, which we will keep
         for i in range(len(RIXS_energies)):
             for j in range(len(expRIXS[0,:])):
                 if(abs(RIXS_energies[i]-expRIXS[0,j]) < 0.1):
                     indices.append(j)
             
         self.expRIXS = expRIXS[1:,indices] #this removes the first row as well, which had the energy values (which we no longer need)
 
 
     """
-    Set the path to the Quanty executable
+    Set the path to the Quanty executable (default is 'Quanty' added to path)
 
-    ----------------
-    Parameters:
-    command: Path to the Quanty executable
-    platform: Platform for which the path is being set, if not set the current platform is used
+    Parameters
+    ----------
+    command: str
+        Path to the Quanty executable
+    platform: str, optional
+        Platform for which the path is being set (if not set the current platform is used)
     """
     def set_quanty_command(self, command, for_platform=None):
         if for_platform is None:
             for_platform = platform.system()
         self.quanty_command[for_platform] = command
 
 
     """
     Set custom path to the parameter file (default: ParVals.txt)
+    !Warning: Should not be changed for default cases!
 
-    ----------------
-    Parameters:
-    par_file: Path to the parameter file
+    Parameters
+    ----------
+    par_file: str
+        Path to the parameter file
     """
     def set_par_file(self, par_file):
         self.par_file = par_file
```

### Comparing `quantylf-0.0.9/src/QuantyLF/cases/D3h_3d.lua` & `quantylf-0.1.0/src/QuantyLF/cases/D3h_3d.lua`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 -- large enough clusters in a full many-body calculation to capture dispersion....
 
 -- We here take a route where we define an effective low energy operator that only allows
 -- to make magnetic excitations, but has the same resonant energy and polarisation dependence
 -- as the RIXS scattering. We then can use this effective operator to calculate the dispersive
 -- magnons using linear spin-wave theory. (Or any other level of theory you want)
 -- The local moment is alligned in the cluster due to an exchange field
-Hex = 0 -- 6*0.084
 HexDir = {1, 1, 1}
 
 -- We calculate the resonant energy dependence in the following window.
 Emin1 = -10
 Emax1 = 20
 NE1 = 120
 Gamma1 = 1.0
@@ -101,14 +100,15 @@
 -- Setup the hybridization
 Vb1g = 0
 Va1g = 0
 Vb2g = 0
 Veg = 0
 
 -- setup initial parameters for fitting values to initialize variables
+Hex = 0
 tenDq = 1
 tenDqFs = 0
 Ds = 0
 Dt = 0
 DsFs = 0
 DtFs = 0
 VfScale = 1
@@ -126,22 +126,25 @@
     end
     if (pars[i].name == "DtF") then
         DtFs = pars[i].val
     end
     if (pars[i].name == "VfScale") then
         VfScale = pars[i].val
     end
+    if (pars[i].name == "Hex") then
+        Hex = pars[i].val
+    end
 end
 
 tenDqF = tenDqFs * tenDq
 DsF = DsFs * Ds
 DtF = DtFs * Dt
 
-Va1g = -2 * Ds - 6 * Dt
-Ve1g = 2 * Ds - Dt
+Va1g = 2 * Ds - 6 * Dt
+Ve1g = -2 * Ds - Dt
 Ve2g = -1 * Ds + 4 * Dt
 
 Va1gF = Va1g * VfScale
 Ve1gF = Ve1g * VfScale
 Ve2gF = Ve2g * VfScale
 
 OppSx_3d = NewOperator("Sx", NF, IndexUp_3d, IndexDn_3d);
```

### Comparing `quantylf-0.0.9/src/QuantyLF/cases/Oh_3d.lua` & `quantylf-0.1.0/src/QuantyLF/cases/Oh_3d.lua`

 * *Files identical despite different names*

### Comparing `quantylf-0.0.9/src/QuantyLF/cases/Td_3d.lua` & `quantylf-0.1.0/src/QuantyLF/cases/Td_3d.lua`

 * *Files identical despite different names*

### Comparing `quantylf-0.0.9/src/QuantyLF/cases/utils/slater_integrals.lua` & `quantylf-0.1.0/src/QuantyLF/cases/utils/slater_integrals.lua`

 * *Files identical despite different names*

