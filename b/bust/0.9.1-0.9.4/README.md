# Comparing `tmp/bust-0.9.1.tar.gz` & `tmp/bust-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bust-0.9.1.tar", last modified: Thu Feb  6 13:07:17 2020, max compression
+gzip compressed data, was "dist/bust-0.9.4.tar", last modified: Mon Dec  7 10:21:10 2020, max compression
```

## Comparing `bust-0.9.1.tar` & `bust-0.9.4.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxrwxrwx   0 ogre      (1000) ogre      (1000)        0 2020-02-06 13:07:17.000000 bust-0.9.1/
-drwxrwxrwx   0 ogre      (1000) ogre      (1000)        0 2020-02-06 13:07:17.000000 bust-0.9.1/bust/
--rwxrwxrwx   0 ogre      (1000) ogre      (1000)    48166 2020-02-06 12:58:23.000000 bust-0.9.1/bust/bus.py
--rwxrwxrwx   0 ogre      (1000) ogre      (1000)     5432 2020-02-05 15:45:47.000000 bust-0.9.1/bust/documentation.py
--rwxrwxrwx   0 ogre      (1000) ogre      (1000)    15672 2020-01-30 18:49:26.000000 bust-0.9.1/bust/editor.py
--rwxrwxrwx   0 ogre      (1000) ogre      (1000)     1438 2020-02-05 15:45:47.000000 bust-0.9.1/bust/exceptions.py
--rwxrwxrwx   0 ogre      (1000) ogre      (1000)     1929 2020-02-05 15:45:47.000000 bust-0.9.1/bust/field.py
--rwxrwxrwx   0 ogre      (1000) ogre      (1000)     6181 2020-02-05 15:45:47.000000 bust-0.9.1/bust/generation.py
--rwxrwxrwx   0 ogre      (1000) ogre      (1000)     5728 2020-02-05 15:45:47.000000 bust-0.9.1/bust/header.py
--rwxrwxrwx   0 ogre      (1000) ogre      (1000)    26369 2020-02-05 15:45:47.000000 bust-0.9.1/bust/module.py
--rwxrwxrwx   0 ogre      (1000) ogre      (1000)     8161 2020-02-05 15:45:47.000000 bust-0.9.1/bust/register.py
--rwxrwxrwx   0 ogre      (1000) ogre      (1000)     3875 2020-02-04 18:29:43.000000 bust-0.9.1/bust/settings.py
--rwxrwxrwx   0 ogre      (1000) ogre      (1000)    30298 2020-02-05 15:45:47.000000 bust-0.9.1/bust/testbench.py
--rwxrwxrwx   0 ogre      (1000) ogre      (1000)     8949 2020-01-30 18:49:26.000000 bust-0.9.1/bust/utils.py
--rwxrwxrwx   0 ogre      (1000) ogre      (1000)     6403 2020-02-05 15:45:47.000000 bust-0.9.1/bust/vhdl.py
--rwxrwxrwx   0 ogre      (1000) ogre      (1000)       21 2020-02-06 12:58:23.000000 bust-0.9.1/bust/_version.py
--rwxrwxrwx   0 ogre      (1000) ogre      (1000)        0 2020-01-30 18:49:26.000000 bust-0.9.1/bust/__init__.py
--rwxrwxrwx   0 ogre      (1000) ogre      (1000)     5247 2020-02-06 10:04:19.000000 bust-0.9.1/bust/__main__.py
-drwxrwxrwx   0 ogre      (1000) ogre      (1000)        0 2020-02-06 13:07:17.000000 bust-0.9.1/bust.egg-info/
--rwxrwxrwx   0 ogre      (1000) ogre      (1000)        1 2020-02-06 13:07:14.000000 bust-0.9.1/bust.egg-info/dependency_links.txt
--rwxrwxrwx   0 ogre      (1000) ogre      (1000)       45 2020-02-06 13:07:14.000000 bust-0.9.1/bust.egg-info/entry_points.txt
--rwxrwxrwx   0 ogre      (1000) ogre      (1000)     4007 2020-02-06 13:07:14.000000 bust-0.9.1/bust.egg-info/PKG-INFO
--rwxrwxrwx   0 ogre      (1000) ogre      (1000)       30 2020-02-06 13:07:14.000000 bust-0.9.1/bust.egg-info/requires.txt
--rwxrwxrwx   0 ogre      (1000) ogre      (1000)      487 2020-02-06 13:07:15.000000 bust-0.9.1/bust.egg-info/SOURCES.txt
--rwxrwxrwx   0 ogre      (1000) ogre      (1000)       11 2020-02-06 13:07:14.000000 bust-0.9.1/bust.egg-info/top_level.txt
--rwxrwxrwx   0 ogre      (1000) ogre      (1000)     4007 2020-02-06 13:07:17.000000 bust-0.9.1/PKG-INFO
--rwxrwxrwx   0 ogre      (1000) ogre      (1000)     2898 2020-02-04 18:29:43.000000 bust-0.9.1/README.md
--rwxrwxrwx   0 ogre      (1000) ogre      (1000)       38 2020-02-06 13:07:17.000000 bust-0.9.1/setup.cfg
--rwxrwxrwx   0 ogre      (1000) ogre      (1000)     1314 2020-02-06 12:58:23.000000 bust-0.9.1/setup.py
-drwxrwxrwx   0 ogre      (1000) ogre      (1000)        0 2020-02-06 13:07:17.000000 bust-0.9.1/tests/
--rwxrwxrwx   0 ogre      (1000) ogre      (1000)     6014 2020-02-05 15:45:47.000000 bust-0.9.1/tests/test_suite.py
--rwxrwxrwx   0 ogre      (1000) ogre      (1000)        0 2020-01-30 18:49:26.000000 bust-0.9.1/tests/__init__.py
+drwxrwxr-x   0 ogre      (1000) ogre      (1000)        0 2020-12-07 10:21:10.000000 bust-0.9.4/
+drwxrwxr-x   0 ogre      (1000) ogre      (1000)        0 2020-12-07 10:21:10.000000 bust-0.9.4/bust/
+-rw-rw-r--   0 ogre      (1000) ogre      (1000)     1961 2020-12-07 10:07:19.000000 bust-0.9.4/bust/bus.py
+-rw-rw-r--   0 ogre      (1000) ogre      (1000)    46865 2020-12-07 10:07:19.000000 bust-0.9.4/bust/bus_vhdl_gen.py
+-rwxrwxrwx   0 ogre      (1000) ogre      (1000)     5432 2020-02-05 15:45:47.000000 bust-0.9.4/bust/documentation.py
+-rw-rw-rw-   0 ogre      (1000) ogre      (1000)    15672 2020-01-30 18:49:26.000000 bust-0.9.4/bust/editor.py
+-rw-rw-r--   0 ogre      (1000) ogre      (1000)     3139 2020-12-07 10:07:19.000000 bust-0.9.4/bust/exceptions.py
+-rwxrwxrwx   0 ogre      (1000) ogre      (1000)     1929 2020-02-05 15:45:47.000000 bust-0.9.4/bust/field.py
+-rwxrwxrwx   0 ogre      (1000) ogre      (1000)     6181 2020-12-07 09:59:33.000000 bust-0.9.4/bust/generation.py
+-rwxrwxrwx   0 ogre      (1000) ogre      (1000)     5728 2020-02-05 15:45:47.000000 bust-0.9.4/bust/header.py
+-rw-rw-r--   0 ogre      (1000) ogre      (1000)     8491 2020-12-07 10:07:19.000000 bust-0.9.4/bust/module.py
+-rw-rw-r--   0 ogre      (1000) ogre      (1000)    14508 2020-12-07 10:07:19.000000 bust-0.9.4/bust/module_vhdl_gen.py
+-rw-rw-r--   0 ogre      (1000) ogre      (1000)     6737 2020-12-07 10:07:19.000000 bust-0.9.4/bust/register.py
+-rwxrwxrwx   0 ogre      (1000) ogre      (1000)     3875 2020-02-04 18:29:43.000000 bust-0.9.4/bust/settings.py
+-rw-rw-r--   0 ogre      (1000) ogre      (1000)    30438 2020-12-07 10:07:55.000000 bust-0.9.4/bust/testbench.py
+-rw-rw-rw-   0 ogre      (1000) ogre      (1000)     8949 2020-01-30 18:49:26.000000 bust-0.9.4/bust/utils.py
+-rw-rw-r--   0 ogre      (1000) ogre      (1000)     6548 2020-12-07 10:07:19.000000 bust-0.9.4/bust/vhdl.py
+-rw-rw-r--   0 ogre      (1000) ogre      (1000)       21 2020-12-07 10:19:15.000000 bust-0.9.4/bust/_version.py
+-rw-rw-rw-   0 ogre      (1000) ogre      (1000)        0 2020-01-30 18:49:26.000000 bust-0.9.4/bust/__init__.py
+-rw-rw-r--   0 ogre      (1000) ogre      (1000)     5268 2020-12-07 10:07:19.000000 bust-0.9.4/bust/__main__.py
+drwxrwxr-x   0 ogre      (1000) ogre      (1000)        0 2020-12-07 10:21:10.000000 bust-0.9.4/bust.egg-info/
+-rw-rw-r--   0 ogre      (1000) ogre      (1000)        1 2020-12-07 10:21:08.000000 bust-0.9.4/bust.egg-info/dependency_links.txt
+-rw-rw-r--   0 ogre      (1000) ogre      (1000)       45 2020-12-07 10:21:08.000000 bust-0.9.4/bust.egg-info/entry_points.txt
+-rw-rw-r--   0 ogre      (1000) ogre      (1000)     4027 2020-12-07 10:21:08.000000 bust-0.9.4/bust.egg-info/PKG-INFO
+-rw-rw-r--   0 ogre      (1000) ogre      (1000)       75 2020-12-07 10:21:08.000000 bust-0.9.4/bust.egg-info/requires.txt
+-rw-rw-r--   0 ogre      (1000) ogre      (1000)      532 2020-12-07 10:21:09.000000 bust-0.9.4/bust.egg-info/SOURCES.txt
+-rw-rw-r--   0 ogre      (1000) ogre      (1000)       11 2020-12-07 10:21:08.000000 bust-0.9.4/bust.egg-info/top_level.txt
+-rw-rw-r--   0 ogre      (1000) ogre      (1000)     4027 2020-12-07 10:21:10.000000 bust-0.9.4/PKG-INFO
+-rwxrwxrwx   0 ogre      (1000) ogre      (1000)     2898 2020-02-04 18:29:43.000000 bust-0.9.4/README.md
+-rw-rw-r--   0 ogre      (1000) ogre      (1000)       38 2020-12-07 10:21:10.000000 bust-0.9.4/setup.cfg
+-rw-rw-r--   0 ogre      (1000) ogre      (1000)     1428 2020-12-07 10:19:15.000000 bust-0.9.4/setup.py
+drwxrwxr-x   0 ogre      (1000) ogre      (1000)        0 2020-12-07 10:21:10.000000 bust-0.9.4/tests/
+-rw-rw-r--   0 ogre      (1000) ogre      (1000)     6035 2020-12-07 10:07:19.000000 bust-0.9.4/tests/test_suite.py
+-rw-rw-rw-   0 ogre      (1000) ogre      (1000)        0 2020-01-30 18:49:26.000000 bust-0.9.4/tests/__init__.py
```

### Comparing `bust-0.9.1/bust/bus.py` & `bust-0.9.4/bust/bus_vhdl_gen.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,89 +1,46 @@
-from collections import OrderedDict
-
 from bust.utils import indent_string
 from bust.vhdl import async_process, sync_process, comb_process, comb_process_with_reset
-from bust.exceptions import InvalidBusType, InvalidResetMode
 
-class Bus(object):
-    """! @brief Managing bus information
 
-    """
-    supported_bus = ['axi', 'ipbus']
-    default_comp_library = "work"
-    default_comp_library_ipbus = 'ipbus'
-
-    def __init__(self, bus):
-        if bus['type'] in Bus.supported_bus:
-            self.bus_type = bus['type']
-        else:
-            raise InvalidBusType(bus['type'])
+class BusVHDLGen():
+    def __init__(self, bus_type, comp_library, data_width, addr_width, ):
+        """Code generator for the Bus module."""
+        self.bus_type = bus_type
+        self.comp_library = comp_library
+        self.clk_name = "clk"
+        self.data_width = data_width
+        self.addr_width = addr_width
 
         if self.bus_type == 'axi':
             self.short_name = 'axi'
-        elif self.bus_type == 'ipbus':
-            self.short_name = 'ipb'
-
-        self.data_width = bus['data_width']
-        self.addr_width = bus['addr_width']
-
-        if self.bus_type == 'ipbus':
-            self.comp_library = Bus.default_comp_library_ipbus
-        elif 'comp_library' in bus:
-            self.comp_library = bus['comp_library']
-        else:
-            self.comp_library = Bus.default_comp_library
-
-        # Set reset type based on bus
-        if self.bus_type == 'axi':
+            self.in_type = 't_axi_mosi'
+            self.out_type = 't_axi_miso'
             self.bus_reset = 'async'
             self.reset_active_low = True
+
         elif self.bus_type == 'ipbus':
+            self.short_name = 'ipb'
+            self.in_type = 'ipb_wbus'
+            self.out_type = 'ipb_rbus'
             self.bus_reset = 'sync'
             self.reset_active_low = False
 
-    def get_clk_name(self):
-        return "clk"
-
-    def get_reset_name(self):
-        if self.bus_reset == "async" and self.reset_active_low is True:
-            reset_name = "areset_n"
-        elif self.bus_reset == "async" and self.reset_active_low is False:
-            reset_name = "areset  "
-        elif self.bus_reset == "sync" and self.reset_active_low is False:
-            reset_name = "reset   "
+        if self.reset_active_low is True:
+            if self.bus_reset == "async":
+                self.reset_name = "areset_n"
+            else:
+                self.reset_name = "reset_n "
         else:
-            reset_name = "reset_n "
-
-        return reset_name
-
-    def get_in_type(self):
-        if self.bus_type == 'axi':
-            return 't_axi_mosi'
-        elif self.bus_type == 'ipbus':
-            return 'ipb_wbus'
-
-    def get_out_type(self):
-        if self.bus_type == 'axi':
-            return 't_axi_miso'
-        elif self.bus_type == 'ipbus':
-            return 'ipb_rbus'
-
-    def return_JSON(self):
-        json = OrderedDict()
-        json['type'] = self.bus_type
-        json['addr_width'] = self.addr_width
-        json['data_width'] = self.data_width
-        json['reset'] = self.bus_reset
-        if self.comp_library != Bus.default_comp_library:
-            json['comp_library'] = self.comp_library
-        return json
+            if self.bus_reset == "async":
+                self.reset_name = "areset  "
+            else:
+                self.reset_name = "reset   "
 
     def return_bus_pkg_VHDL(self):
-
         if self.bus_type == 'axi':
 
             s = 'library ieee;\n'
             s += 'use ieee.std_logic_1164.all;\n'
             s += '\n'
 
             s += 'package ' + self.bus_type + '_pkg is\n'
@@ -138,16 +95,16 @@
             s += '\n'
 
             s += 'end ' + self.bus_type + '_pkg;'
 
         return s
 
     def return_bus_pif_VHDL(self, mod):
-        clk_name = self.get_clk_name()
-        reset_name = self.get_reset_name()
+        clk_name = self.clk_name
+        reset_name = self.reset_name
 
         s = 'library ieee;\n'
         s += 'use ieee.std_logic_1164.all;\n'
         s += 'use ieee.numeric_std.all;\n'
         s += '\n'
         if self.comp_library != "work":
             s += "library " + self.comp_library + ";\n"
@@ -205,16 +162,16 @@
             par += 'arready        : out std_logic;\n'
             par += 'rdata          : out t_' + mod.name + '_data;\n'
             par += 'rresp          : out std_logic_vector(1 downto 0);\n'
             par += 'rvalid         : out std_logic;\n'
             par += 'rready         : in  std_logic\n'
 
         elif self.bus_type == 'ipbus':
-            par += '{}_in         : in  {};\n'.format(self.short_name, self.get_in_type())
-            par += '{}_out        : out {}\n'.format(self.short_name, self.get_out_type())
+            par += '{}_in         : in  {};\n'.format(self.short_name, self.in_type)
+            par += '{}_out        : out {}\n'.format(self.short_name, self.out_type)
 
         par += ');\n'
         s += indent_string(par, 2)
         s += 'end ' + mod.name + '_' + self.short_name + '_pif;\n\n'
 
         s += 'architecture behavior of {}_{}_pif is\n\n'.format(mod.name, self.short_name)
 
@@ -823,15 +780,15 @@
             logic_string += "elsif stall then\n"
             logic_string += indent_string("stall <= '0';\n")
             logic_string += indent_string("ack_d <= '1';\n")
             logic_string += "end if;\n"
 
             if self.bus_reset == "async":
                 s += indent_string(async_process(clk_name, reset_name, "p_stall",
-                                reset_string, logic_string, self.reset_active_low, variables))
+                                    reset_string, logic_string, self.reset_active_low, variables))
 
             elif self.bus_reset == "sync":
                 s += indent_string(sync_process(clk_name, reset_name, "p_stall",
                                     reset_string, logic_string, self.reset_active_low, variables))
             s += '\n'
 
         ####################################################################
@@ -896,16 +853,16 @@
             s = 'ipb_in              => ipb_in,\n'
             s += 'ipb_out             => ipb_out{}\n'.format(inter)
 
         return s
 
     def pulse_reg_process(self, mod, reg):
 
-        clk_name = self.get_clk_name()
-        reset_name = str.strip(self.get_reset_name())
+        clk_name = self.clk_name
+        reset_name = str.strip(self.reset_name)
         proc_name = "p_pulse_" + reg.name
         const_name = "c_" + mod.name + "_pulse_regs." + reg.name
         reg_name = self.short_name + "_pulse_regs_i." + reg.name
         reg_tmp_name = self.short_name + "_pulse_regs_cycle." + reg.name
         if reg.pulse_cycles > 1:
             variables = ["cnt : natural range 0 to " + str(reg.pulse_cycles-1) + " := 0"]
         else:
@@ -1035,30 +992,30 @@
             '                data_value,\n'
             '                msg,\n'
             '                {1}_{2},\n'
             '                {0}_if,\n'
             '                C_SCOPE,\n'
             '                shared_msg_id_panel,\n'
             '                {0}_bfm_config);\n'
-            'end;\n\n').format(ext_name, self.short_name, self.get_clk_name())
+            'end;\n\n').format(ext_name, self.short_name, self.clk_name)
 
         s += ('procedure read(\n'
               '  constant addr_value : in  unsigned;\n'
               '  variable data_value : out std_logic_vector;\n'
               '  constant msg        : in  string) is\n'
               'begin\n'
               '  {0}_read(addr_value,\n'
               '               data_value,\n'
               '               msg,\n'
               '               {1}_{2},\n'
               '               {0}_if,\n'
               '               C_SCOPE,\n'
               '               shared_msg_id_panel,\n'
               '               {0}_bfm_config);\n'
-              'end;\n').format(ext_name, self.short_name, self.get_clk_name())
+              'end;\n').format(ext_name, self.short_name, self.clk_name)
         s += 'variable dummy_data : std_logic_vector(31 downto 0);\n\n'
 
         s += ('procedure check(\n'
               '  constant addr_value : in unsigned;\n'
               '  constant data_exp   : in std_logic_vector;\n'
               '  constant msg        : in string) is\n'
               'begin\n'
@@ -1067,21 +1024,19 @@
               '                msg,\n'
               '                {1}_{2},\n'
               '                {0}_if,\n'
               '                error,\n'
               '                C_SCOPE,\n'
               '                shared_msg_id_panel,\n'
               '                {0}_bfm_config);\n'
-              'end;\n\n').format(ext_name, self.short_name, self.get_clk_name())
+              'end;\n\n').format(ext_name, self.short_name, self.clk_name)
 
         return s
 
     def uvvm_write(self, reg_addr, value, string):
         s = 'write(f_addr(g_{}_baseaddr, {}), {}, "{}");\n'.format(self.short_name, reg_addr, value, string)
         return s
 
     def uvvm_check(self, reg_addr, data_exp, string):
         s = 'check(f_addr(g_{}_baseaddr, {}), {}, "{}");\n'.format(self.short_name, reg_addr, data_exp, string)
         return s
 
-
-
```

### Comparing `bust-0.9.1/bust/documentation.py` & `bust-0.9.4/bust/documentation.py`

 * *Files identical despite different names*

### Comparing `bust-0.9.1/bust/editor.py` & `bust-0.9.4/bust/editor.py`

 * *Files identical despite different names*

### Comparing `bust-0.9.1/bust/field.py` & `bust-0.9.4/bust/field.py`

 * *Files identical despite different names*

### Comparing `bust-0.9.1/bust/generation.py` & `bust-0.9.4/bust/generation.py`

 * *Files identical despite different names*

### Comparing `bust-0.9.1/bust/header.py` & `bust-0.9.4/bust/header.py`

 * *Files identical despite different names*

### Comparing `bust-0.9.1/bust/register.py` & `bust-0.9.4/bust/register.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from bust.utils import indent_string
-from bust.utils import add_line_breaks
+from bust.exceptions import \
+    ModuleDataBitsExceeded, UndefinedRegisterType, \
+    UndefinedFieldType, InvalidRegisterFormat, \
+    InvalidFieldFormat, InvalidStallValue
 from bust.field import Field
-from bust.vhdl import is_valid_VHDL
-from bust.vhdl import is_unique
+from bust.utils import add_line_breaks, indent_string
+from bust.vhdl import is_unique, is_valid_VHDL
 
 
 class Register:
     """! @brief Managing register information
 
 
     """
@@ -191,60 +193,7 @@
             return "/STALL"
         else:
             return ""
 
     def get_stall_cycles_str(self):
         return str(self.stall_cycles-2)
 
-
-class ModuleDataBitsExceeded(Exception):
-    """! @brief Raised when the specified module data bits are exceeded
-
-    """
-
-    def __init__(self, register, reglength, mod_data_length):
-        msg = "Register length exceeded module data length by "
-        msg += str(reglength - mod_data_length)
-        msg += " in register " + register + "\n"
-        msg += 'Module length: ' + str(mod_data_length) + '\n'
-        msg += 'Register length: ' + str(reglength)
-
-        super().__init__(msg)
-
-
-class UndefinedRegisterType(RuntimeError):
-    """! @brief Raised when trying to parse a register type that is not supported
-
-    """
-
-    def __init__(self, regtype):
-        msg = "Could not parse register type: " + regtype
-        super().__init__(msg)
-
-
-class UndefinedFieldType(RuntimeError):
-    """! @brief Raised when trying to parse an field type that is not supported
-
-    """
-
-    def __init__(self, sig_type):
-        msg = "Could not parse field type: " + sig_type
-        super().__init__(msg)
-
-
-class InvalidRegisterFormat(RuntimeError):
-    """! @brief Raised when register has some unspecified format error"""
-
-    def __init__(self, msg):
-        msg = 'Invalid register format: ' + msg
-        super().__init__(msg)
-
-
-class InvalidFieldFormat(RuntimeError):
-    def __init__(self, msg):
-        msg = 'Invalid field format: ' + msg
-        super().__init__(msg)
-
-class InvalidStallValue(RuntimeError):
-    def __init__(self, val):
-        msg = 'Invalid stall value: {}. Must be between 2 and 255.'.format(val)
-        super().__init__(msg)
```

### Comparing `bust-0.9.1/bust/settings.py` & `bust-0.9.4/bust/settings.py`

 * *Files identical despite different names*

### Comparing `bust-0.9.1/bust/testbench.py` & `bust-0.9.4/bust/testbench.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,16 +128,15 @@
 
         s += ('###########################################################################\n'
               '# Simulate\n'
               '###########################################################################\n')
         s += 'vsim -quiet '
         if self.settings.coverage:
             s += '-coverage '
-        s += '{0}.{0}_{1}_pif_tb\n'.format(self.module.name, self.bus.short_name)
-        s += 'add wave -position insertpoint sim:/{}_{}_pif_tb/*\n\n'.format(self.module.name, self.bus.short_name)
+        s += '{0}.{0}_{1}_pif_tb\n\n'.format(self.module.name, self.bus.short_name)
 
         s += ('# Trick to avoid metastability warnings\n'
               'quietly set NumericStdNoWarnings 1\n'
               'run 1 ns;\n'
               'quietly set NumericStdNoWarnings 0\n'
               'run -all\n\n')
 
@@ -201,29 +200,33 @@
 
         # Initial reset value
         if self.bus.reset_active_low:
             init_reset = "'1'"
         else:
             init_reset = "'0'"
 
-        s += indent_string('-- component ports\n'
-                           'signal {0}_rw_regs    : t_{1}_rw_regs    := c_{1}_rw_regs;\n'
-                           'signal {0}_ro_regs    : t_{1}_ro_regs    := c_{1}_ro_regs;\n'
-                           'signal {0}_pulse_regs : t_{1}_pulse_regs := c_{1}_pulse_regs;\n'
-                           'signal {0}_{2}        : std_logic                   := \'1\';\n'
+        s += indent_string('-- component ports\n')
+        if self.module.count_rw_regs() > 0:
+            s += indent_string('signal {0}_rw_regs    : t_{1}_rw_regs    := c_{1}_rw_regs;\n'.format(self.bus.short_name, self.module.name))
+        if self.module.count_ro_regs() > 0:
+            s += indent_string('signal {0}_ro_regs    : t_{1}_ro_regs    := c_{1}_ro_regs;\n'.format(self.bus.short_name, self.module.name))
+        if self.module.count_pulse_regs() > 0:
+            s += indent_string('signal {0}_pulse_regs : t_{1}_pulse_regs := c_{1}_pulse_regs;\n'.format(self.bus.short_name, self.module.name))
+
+        s += indent_string('signal {0}_{2}        : std_logic                   := \'1\';\n'
                            'signal {0}_{3}   : std_logic                   := {4};\n'
                            'signal {0}_in         : {5};\n'
                            'signal {0}_out        : {6};\n'
                            '').format(self.bus.short_name,
                                       self.module.name,
-                                      self.bus.get_clk_name(),
-                                      self.bus.get_reset_name(),
+                                      self.bus.clk_name,
+                                      self.bus.reset_name,
                                       init_reset,
-                                      self.bus.get_in_type(),
-                                      self.bus.get_out_type())
+                                      self.bus.in_type,
+                                      self.bus.out_type)
         s += '\n'
 
         s += indent_string(self.bus.get_uvvm_signals())
         s += '\n'
 
         s += indent_string(self.get_addr_func())
         s += '\n'
@@ -235,15 +238,15 @@
 
         s += indent_string('-- component instantiation\n')
         s += indent_string(self.module.get_instantiation("DUT", False))
         s += '\n'
 
         s += indent_string(('-- clock generator\n'
               'clock_generator({}_{}, C_CLK_PERIOD);\n\n').format(self.bus.short_name,
-                                                                  self.bus.get_clk_name()))
+                                                                  self.bus.clk_name))
 
         s += indent_string(('-- main testbench\n'
               'p_main : process\n\n'))
 
         s += indent_string(self.get_uvvm_gen_overloads(), 2)
         s += indent_string(self.bus.get_uvvm_overloads(), 2)
 
@@ -266,15 +269,15 @@
         s += '\n'
         # Initial reset value
         if self.bus.reset_active_low:
             pulse_reset = "'0'"
         else:
             pulse_reset = "'1'"
         par = 'gen_pulse({}_{}, {}, 500 ns, BLOCKING, "Reset for 500 ns");\n'.format(self.bus.short_name,
-                                                                                    str.strip(self.bus.get_reset_name()),
+                                                                                    str.strip(self.bus.reset_name),
                                                                                     pulse_reset)
 
         s += indent_string(par, 2)
         s += '\n'
         for reg in self.module.registers:
             s += indent_string('--\n\n', 2)
```

### Comparing `bust-0.9.1/bust/utils.py` & `bust-0.9.4/bust/utils.py`

 * *Files identical despite different names*

### Comparing `bust-0.9.1/bust/vhdl.py` & `bust-0.9.4/bust/vhdl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import re
 
 from bust.utils import indent_string
 from bust.utils import is_mixed
 
+def lib_declaration():
+    s = 'library ieee;\n'
+    s += 'use ieee.std_logic_1164.all;\n'
+    s += 'use ieee.numeric_std.all;\n\n'
+    return s
 
 def sync_process(clk_name, reset_name, process_name, reset_string, logic_string, active_low=True, variables=None):
     s = process_name + " : process(" + clk_name + ")\n"
     if variables is not None:
         for var in variables:
             s += indent_string("variable " + var + ";\n")
     s += "begin\n"
```

### Comparing `bust-0.9.1/bust/__main__.py` & `bust-0.9.4/bust/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             try:
                 json_dict = json_parser(json_file)
                 settings = Settings(json_file, json_dict['settings'])
                 bus = Bus(json_dict['bus'])
                 module = Module(json_dict['module'], bus, settings)
                 header = Header(module)
                 documentation = Documentation(module)
-                testbench = Testbench(module, bus, settings)
+                testbench = Testbench(module, bus.get_VHDL_generator(), settings)
 
             except (FormatError, InvalidAddress, InvalidRegister, InvalidResetMode, InvalidBusType, NotImplementedError) as e:
                 logger.error(str(e))
                 exit(1)
 
             except Exception as e:
                 logger.error('\nERROR:\nAn unknown error has occurred...')
```

### Comparing `bust-0.9.1/bust.egg-info/PKG-INFO` & `bust-0.9.4/bust.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bust
-Version: 0.9.1
+Version: 0.9.4
 Summary: Utility for simply creating and modifying VHDL bus slave modules
 Home-page: http://github.com/olagrottvik/bust
 Author: Ola Groettvik
 Author-email: olagrottvik@gmail.com
 License: MIT
 Description: [![Build Status](https://travis-ci.com/olagrottvik/bust.svg?branch=master)](https://travis-ci.com/olagrottvik/bust)
         
@@ -101,7 +101,8 @@
         This project is licensed under the MIT license - see [LICENSE](LICENSE) for details.
         
         
 Keywords: vhdl,bus,axi
 Platform: UNKNOWN
 Requires-Python: ~=3.4
 Description-Content-Type: text/markdown
+Provides-Extra: dev
```

### Comparing `bust-0.9.1/PKG-INFO` & `bust-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bust
-Version: 0.9.1
+Version: 0.9.4
 Summary: Utility for simply creating and modifying VHDL bus slave modules
 Home-page: http://github.com/olagrottvik/bust
 Author: Ola Groettvik
 Author-email: olagrottvik@gmail.com
 License: MIT
 Description: [![Build Status](https://travis-ci.com/olagrottvik/bust.svg?branch=master)](https://travis-ci.com/olagrottvik/bust)
         
@@ -101,7 +101,8 @@
         This project is licensed under the MIT license - see [LICENSE](LICENSE) for details.
         
         
 Keywords: vhdl,bus,axi
 Platform: UNKNOWN
 Requires-Python: ~=3.4
 Description-Content-Type: text/markdown
+Provides-Extra: dev
```

### Comparing `bust-0.9.1/README.md` & `bust-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `bust-0.9.1/setup.py` & `bust-0.9.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,21 +16,26 @@
     def run(self):
         os.system("find . -name '*.pyc' -delete")
         os.system("find . -name '__pycache__' -delete")
         os.system('rm -rf ./build ./dist ./*.tgz ./*.egg-info ./.pytest_cache ./.eggs')
 
 setup(
     name='bust',
-    version='0.9.1',
+    version='0.9.4',
     packages=find_packages(),
     license='MIT',
     install_requires=[
         'docopt>=0.6.2',
         'pylatexenc>=1.2',
+        'curses-menu',
+        'PrettyTable'
       ],
+    extras_require={
+        'dev': ["pytest", "pylint"],
+        },
     python_requires='~=3.4', # For Python 3.4 and up, but not yet Python 4
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={
         'console_scripts': ['bust = bust.__main__:main'],
     },
```

### Comparing `bust-0.9.1/tests/test_suite.py` & `bust-0.9.4/tests/test_suite.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     def load_bus(bus_type):
         # Load the example JSON file
         json_file = "example/example_{}.json".format(bus_type)
         json = json_parser(json_file)
         sett = Settings(json_file, json['settings'])
         bus = Bus(json['bus'])
         mod = Module(json['module'], bus, sett)
-        tb = Testbench(mod, bus, sett)
+        tb = Testbench(mod, bus.get_VHDL_generator(), sett)
         doc = Documentation(mod)
         hdr = Header(mod)
         return sett, bus, mod, tb, doc, hdr
 
     def __repr__(self):
         return self.get_type()
```

