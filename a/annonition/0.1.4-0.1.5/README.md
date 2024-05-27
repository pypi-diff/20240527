# Comparing `tmp/annonition-0.1.4.tar.gz` & `tmp/annonition-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annonition-0.1.4.tar", last modified: Mon May 27 01:47:13 2024, max compression
+gzip compressed data, was "annonition-0.1.5.tar", last modified: Mon May 27 03:49:01 2024, max compression
```

## Comparing `annonition-0.1.4.tar` & `annonition-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 01:47:13.360000 annonition-0.1.4/
--rw-rw-rw-   0        0        0     1089 2024-05-26 00:32:06.000000 annonition-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     5049 2024-05-27 01:47:14.000000 annonition-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     4639 2024-05-27 01:43:46.000000 annonition-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 01:47:13.380000 annonition-0.1.4/annonition/
--rw-rw-rw-   0        0        0       93 2024-05-26 00:15:56.000000 annonition-0.1.4/annonition/__init__.py
--rw-rw-rw-   0        0        0    11150 2024-05-27 01:46:46.000000 annonition-0.1.4/annonition/logger.py
--rw-rw-rw-   0        0        0      113 2024-05-26 00:15:48.000000 annonition-0.1.4/annonition/main.py
-drwxrwxrwx   0        0        0        0 2024-05-27 01:47:13.400000 annonition-0.1.4/annonition.egg-info/
--rw-rw-rw-   0        0        0     5049 2024-05-27 01:47:14.000000 annonition-0.1.4/annonition.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-05-27 01:47:14.000000 annonition-0.1.4/annonition.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 01:47:14.000000 annonition-0.1.4/annonition.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-27 01:47:14.000000 annonition-0.1.4/annonition.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-27 01:47:14.000000 annonition-0.1.4/annonition.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 01:47:14.000000 annonition-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      750 2024-05-27 01:47:04.000000 annonition-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 03:48:58.140000 annonition-0.1.5/
+-rw-rw-rw-   0        0        0     1089 2024-05-26 00:32:06.000000 annonition-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     5049 2024-05-27 03:49:02.000000 annonition-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4639 2024-05-27 01:43:46.000000 annonition-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 03:48:58.790000 annonition-0.1.5/annonition/
+-rw-rw-rw-   0        0        0       93 2024-05-26 00:15:56.000000 annonition-0.1.5/annonition/__init__.py
+-rw-rw-rw-   0        0        0    11124 2024-05-27 03:48:04.000000 annonition-0.1.5/annonition/logger.py
+-rw-rw-rw-   0        0        0      113 2024-05-26 00:15:48.000000 annonition-0.1.5/annonition/main.py
+drwxrwxrwx   0        0        0        0 2024-05-27 03:48:59.400000 annonition-0.1.5/annonition.egg-info/
+-rw-rw-rw-   0        0        0     5049 2024-05-27 03:48:58.000000 annonition-0.1.5/annonition.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-05-27 03:49:00.000000 annonition-0.1.5/annonition.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 03:48:58.000000 annonition-0.1.5/annonition.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-27 03:48:58.000000 annonition-0.1.5/annonition.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-27 03:48:58.000000 annonition-0.1.5/annonition.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 03:49:02.000000 annonition-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      750 2024-05-27 03:48:42.000000 annonition-0.1.5/setup.py
```

### Comparing `annonition-0.1.4/LICENSE` & `annonition-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `annonition-0.1.4/PKG-INFO` & `annonition-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annonition
-Version: 0.1.4
+Version: 0.1.5
 Summary: Log everything in style.
 Author: Abtin Turing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `annonition-0.1.4/README.md` & `annonition-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `annonition-0.1.4/annonition/logger.py` & `annonition-0.1.5/annonition/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -578,120 +578,119 @@
 00002410: 656e 645f 7469 6d65 203d 204e 6f6e 650d  end_time = None.
 00002420: 0a0d 0a20 2020 2020 2020 2064 6566 205f  ...        def _
 00002430: 5f65 6e74 6572 5f5f 2873 656c 6629 3a0d  _enter__(self):.
 00002440: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
 00002450: 662e 7374 6172 745f 7469 6d65 203d 2074  f.start_time = t
 00002460: 696d 652e 7065 7266 5f63 6f75 6e74 6572  ime.perf_counter
 00002470: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00002480: 7072 696e 7428 2248 4579 2229 0d0a 2020  print("HEy")..  
-00002490: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000024a0: 2073 656c 660d 0a0d 0a20 2020 2020 2020   self....       
-000024b0: 2064 6566 205f 5f65 7869 745f 5f28 7365   def __exit__(se
-000024c0: 6c66 2c20 6578 635f 7479 7065 2c20 6578  lf, exc_type, ex
-000024d0: 635f 7661 6c2c 2065 7863 5f74 6229 3a0d  c_val, exc_tb):.
-000024e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000024f0: 662e 656e 645f 7469 6d65 203d 2074 696d  f.end_time = tim
-00002500: 652e 7065 7266 5f63 6f75 6e74 6572 2829  e.perf_counter()
-00002510: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-00002520: 6170 7365 645f 7469 6d65 203d 2073 656c  apsed_time = sel
-00002530: 662e 656e 645f 7469 6d65 202d 2073 656c  f.end_time - sel
-00002540: 662e 7374 6172 745f 7469 6d65 0d0a 2020  f.start_time..  
-00002550: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00002560: 6c6f 675f 7469 6d65 2865 6c61 7073 6564  log_time(elapsed
-00002570: 5f74 696d 6529 0d0a 0d0a 2020 2020 2020  _time)....      
-00002580: 2020 6465 6620 6765 745f 7469 6d65 2873    def get_time(s
-00002590: 656c 6629 3a0d 0a20 2020 2020 2020 2020  elf):..         
-000025a0: 2020 2069 6620 7365 6c66 2e73 7461 7274     if self.start
-000025b0: 5f74 696d 6520 6973 204e 6f6e 653a 0d0a  _time is None:..
-000025c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025d0: 7265 7475 726e 2030 2e30 0d0a 2020 2020  return 0.0..    
-000025e0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000025f0: 656e 645f 7469 6d65 2069 7320 6e6f 7420  end_time is not 
-00002600: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00002610: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00002620: 6c66 2e65 6e64 5f74 696d 6520 2d20 7365  lf.end_time - se
-00002630: 6c66 2e73 7461 7274 5f74 696d 650d 0a20  lf.start_time.. 
-00002640: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00002650: 6e20 7469 6d65 2e70 6572 665f 636f 756e  n time.perf_coun
-00002660: 7465 7228 2920 2d20 7365 6c66 2e73 7461  ter() - self.sta
-00002670: 7274 5f74 696d 650d 0a0d 0a20 2020 2020  rt_time....     
-00002680: 2020 2064 6566 205f 6c6f 675f 7469 6d65     def _log_time
-00002690: 2873 656c 662c 2065 6c61 7073 6564 5f74  (self, elapsed_t
-000026a0: 696d 6529 3a0d 0a20 2020 2020 2020 2020  ime):..         
-000026b0: 2020 206d 6573 7361 6765 203d 2066 227b     message = f"{
-000026c0: 7365 6c66 2e74 6173 6b5f 6e61 6d65 7d3a  self.task_name}:
-000026d0: 207b 656c 6170 7365 645f 7469 6d65 3a2e   {elapsed_time:.
-000026e0: 3466 7d73 220d 0a20 2020 2020 2020 2020  4f}s"..         
-000026f0: 2020 2069 6620 7365 6c66 2e6c 6f67 5f74     if self.log_t
-00002700: 7970 6520 3d3d 2022 7072 696e 7422 3a0d  ype == "print":.
-00002710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002720: 2070 7269 6e74 286d 6573 7361 6765 290d   print(message).
-00002730: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-00002740: 6620 7365 6c66 2e6c 6f67 5f74 7970 6520  f self.log_type 
-00002750: 3d3d 2022 6465 6275 6722 3a0d 0a20 2020  == "debug":..   
-00002760: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00002770: 662e 6c6f 6767 6572 2e64 6562 7567 286d  f.logger.debug(m
-00002780: 6573 7361 6765 290d 0a20 2020 2020 2020  essage)..       
-00002790: 2020 2020 2065 6c69 6620 7365 6c66 2e6c       elif self.l
-000027a0: 6f67 5f74 7970 6520 3d3d 2022 696e 666f  og_type == "info
-000027b0: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
-000027c0: 2020 2020 7365 6c66 2e6c 6f67 6765 722e      self.logger.
-000027d0: 696e 666f 286d 6573 7361 6765 290d 0a20  info(message).. 
-000027e0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-000027f0: 7365 6c66 2e6c 6f67 5f74 7970 6520 3d3d  self.log_type ==
-00002800: 2022 7761 726e 696e 6722 3a0d 0a20 2020   "warning":..   
-00002810: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00002820: 662e 6c6f 6767 6572 2e77 6172 6e69 6e67  f.logger.warning
-00002830: 286d 6573 7361 6765 290d 0a20 2020 2020  (message)..     
-00002840: 2020 2020 2020 2065 6c69 6620 7365 6c66         elif self
-00002850: 2e6c 6f67 5f74 7970 6520 3d3d 2022 6572  .log_type == "er
-00002860: 726f 7222 3a0d 0a20 2020 2020 2020 2020  ror":..         
-00002870: 2020 2020 2020 2073 656c 662e 6c6f 6767         self.logg
-00002880: 6572 2e65 7272 6f72 286d 6573 7361 6765  er.error(message
-00002890: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
-000028a0: 6c69 6620 7365 6c66 2e6c 6f67 5f74 7970  lif self.log_typ
-000028b0: 6520 3d3d 2022 6372 6974 6963 616c 223a  e == "critical":
-000028c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000028d0: 2020 7365 6c66 2e6c 6f67 6765 722e 6372    self.logger.cr
-000028e0: 6974 6963 616c 286d 6573 7361 6765 290d  itical(message).
-000028f0: 0a0d 0a20 2020 2040 636f 6e74 6578 746d  ...    @contextm
-00002900: 616e 6167 6572 0d0a 2020 2020 6465 6620  anager..    def 
-00002910: 7469 6d65 7228 7365 6c66 2c20 7461 736b  timer(self, task
-00002920: 5f6e 616d 653a 2073 7472 2c20 7479 7065  _name: str, type
-00002930: 3a20 4f70 7469 6f6e 616c 5b54 696d 6572  : Optional[Timer
-00002940: 5479 7065 5d20 3d22 696e 666f 2229 3a0d  Type] ="info"):.
-00002950: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00002960: 2020 2020 2020 5265 7475 726e 7320 6120        Returns a 
-00002970: 636f 6e74 6578 7420 6d61 6e61 6765 7220  context manager 
-00002980: 666f 7220 7469 6d69 6e67 2061 2062 6c6f  for timing a blo
-00002990: 636b 206f 6620 636f 6465 2e0d 0a0d 0a20  ck of code..... 
-000029a0: 2020 2020 2020 2055 7361 6765 3a0d 0a20         Usage:.. 
-000029b0: 2020 2020 2020 2060 6060 7079 7468 6f6e         ```python
-000029c0: 0d0a 2020 2020 2020 2020 7769 7468 206c  ..        with l
-000029d0: 6f67 6765 722e 7469 6d65 7228 2244 6f69  ogger.timer("Doi
-000029e0: 6e67 2073 6f6d 6574 6869 6e67 2e2e 2e22  ng something..."
-000029f0: 2920 6173 2074 696d 6572 5f63 6f6e 7465  ) as timer_conte
-00002a00: 7874 3a0d 0a20 2020 2020 2020 2020 2020  xt:..           
-00002a10: 2074 696d 652e 736c 6565 7028 3529 0d0a   time.sleep(5)..
-00002a20: 2020 2020 2020 2020 2020 2020 656c 6170              elap
-00002a30: 7365 6420 3d20 7469 6d65 725f 636f 6e74  sed = timer_cont
-00002a40: 6578 742e 6765 745f 7469 6d65 2829 0d0a  ext.get_time()..
-00002a50: 2020 2020 2020 2020 6060 600d 0a20 2020          ```..   
-00002a60: 2020 2020 204c 6f67 733a 0d0a 2020 2020       Logs:..    
-00002a70: 2020 2020 6044 6f69 6e67 2073 6f6d 6574      `Doing somet
-00002a80: 6869 6e67 2e2e 2e3a 2035 2e30 3032 3673  hing...: 5.0026s
-00002a90: 600d 0a20 2020 2020 2020 2022 2222 0d0a  `..        """..
-00002aa0: 2020 2020 2020 2020 7469 6d65 725f 636f          timer_co
-00002ab0: 6e74 6578 7420 3d20 7365 6c66 2e54 696d  ntext = self.Tim
-00002ac0: 6572 436f 6e74 6578 7428 7461 736b 5f6e  erContext(task_n
-00002ad0: 616d 652c 2073 656c 662e 6164 6170 7465  ame, self.adapte
-00002ae0: 722c 2074 7970 6529 0d0a 2020 2020 2020  r, type)..      
-00002af0: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
-00002b00: 2020 2020 7469 6d65 725f 636f 6e74 6578      timer_contex
-00002b10: 742e 5f5f 656e 7465 725f 5f28 290d 0a20  t.__enter__().. 
-00002b20: 2020 2020 2020 2020 2020 2079 6965 6c64             yield
-00002b30: 2074 696d 6572 5f63 6f6e 7465 7874 0d0a   timer_context..
-00002b40: 2020 2020 2020 2020 6669 6e61 6c6c 793a          finally:
-00002b50: 0d0a 2020 2020 2020 2020 2020 2020 7469  ..            ti
-00002b60: 6d65 725f 636f 6e74 6578 742e 5f5f 6578  mer_context.__ex
-00002b70: 6974 5f5f 284e 6f6e 652c 204e 6f6e 652c  it__(None, None,
-00002b80: 204e 6f6e 6529 0d0a 2020 2020 0d0a        None)..    ..
+00002480: 7265 7475 726e 2073 656c 660d 0a0d 0a20  return self.... 
+00002490: 2020 2020 2020 2064 6566 205f 5f65 7869         def __exi
+000024a0: 745f 5f28 7365 6c66 2c20 6578 635f 7479  t__(self, exc_ty
+000024b0: 7065 2c20 6578 635f 7661 6c2c 2065 7863  pe, exc_val, exc
+000024c0: 5f74 6229 3a0d 0a20 2020 2020 2020 2020  _tb):..         
+000024d0: 2020 2073 656c 662e 656e 645f 7469 6d65     self.end_time
+000024e0: 203d 2074 696d 652e 7065 7266 5f63 6f75   = time.perf_cou
+000024f0: 6e74 6572 2829 0d0a 2020 2020 2020 2020  nter()..        
+00002500: 2020 2020 656c 6170 7365 645f 7469 6d65      elapsed_time
+00002510: 203d 2073 656c 662e 656e 645f 7469 6d65   = self.end_time
+00002520: 202d 2073 656c 662e 7374 6172 745f 7469   - self.start_ti
+00002530: 6d65 0d0a 2020 2020 2020 2020 2020 2020  me..            
+00002540: 7365 6c66 2e5f 6c6f 675f 7469 6d65 2865  self._log_time(e
+00002550: 6c61 7073 6564 5f74 696d 6529 0d0a 0d0a  lapsed_time)....
+00002560: 2020 2020 2020 2020 6465 6620 6765 745f          def get_
+00002570: 7469 6d65 2873 656c 6629 3a0d 0a20 2020  time(self):..   
+00002580: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00002590: 2e73 7461 7274 5f74 696d 6520 6973 204e  .start_time is N
+000025a0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+000025b0: 2020 2020 2020 7265 7475 726e 2030 2e30        return 0.0
+000025c0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+000025d0: 2073 656c 662e 656e 645f 7469 6d65 2069   self.end_time i
+000025e0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+000025f0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00002600: 7572 6e20 7365 6c66 2e65 6e64 5f74 696d  urn self.end_tim
+00002610: 6520 2d20 7365 6c66 2e73 7461 7274 5f74  e - self.start_t
+00002620: 696d 650d 0a20 2020 2020 2020 2020 2020  ime..           
+00002630: 2072 6574 7572 6e20 7469 6d65 2e70 6572   return time.per
+00002640: 665f 636f 756e 7465 7228 2920 2d20 7365  f_counter() - se
+00002650: 6c66 2e73 7461 7274 5f74 696d 650d 0a0d  lf.start_time...
+00002660: 0a20 2020 2020 2020 2064 6566 205f 6c6f  .        def _lo
+00002670: 675f 7469 6d65 2873 656c 662c 2065 6c61  g_time(self, ela
+00002680: 7073 6564 5f74 696d 6529 3a0d 0a20 2020  psed_time):..   
+00002690: 2020 2020 2020 2020 206d 6573 7361 6765           message
+000026a0: 203d 2066 227b 7365 6c66 2e74 6173 6b5f   = f"{self.task_
+000026b0: 6e61 6d65 7d3a 207b 656c 6170 7365 645f  name}: {elapsed_
+000026c0: 7469 6d65 3a2e 3466 7d73 220d 0a20 2020  time:.4f}s"..   
+000026d0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+000026e0: 2e6c 6f67 5f74 7970 6520 3d3d 2022 7072  .log_type == "pr
+000026f0: 696e 7422 3a0d 0a20 2020 2020 2020 2020  int":..         
+00002700: 2020 2020 2020 2070 7269 6e74 286d 6573         print(mes
+00002710: 7361 6765 290d 0a20 2020 2020 2020 2020  sage)..         
+00002720: 2020 2065 6c69 6620 7365 6c66 2e6c 6f67     elif self.log
+00002730: 5f74 7970 6520 3d3d 2022 6465 6275 6722  _type == "debug"
+00002740: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00002750: 2020 2073 656c 662e 6c6f 6767 6572 2e64     self.logger.d
+00002760: 6562 7567 286d 6573 7361 6765 290d 0a20  ebug(message).. 
+00002770: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00002780: 7365 6c66 2e6c 6f67 5f74 7970 6520 3d3d  self.log_type ==
+00002790: 2022 696e 666f 223a 0d0a 2020 2020 2020   "info":..      
+000027a0: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
+000027b0: 6f67 6765 722e 696e 666f 286d 6573 7361  ogger.info(messa
+000027c0: 6765 290d 0a20 2020 2020 2020 2020 2020  ge)..           
+000027d0: 2065 6c69 6620 7365 6c66 2e6c 6f67 5f74   elif self.log_t
+000027e0: 7970 6520 3d3d 2022 7761 726e 696e 6722  ype == "warning"
+000027f0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00002800: 2020 2073 656c 662e 6c6f 6767 6572 2e77     self.logger.w
+00002810: 6172 6e69 6e67 286d 6573 7361 6765 290d  arning(message).
+00002820: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+00002830: 6620 7365 6c66 2e6c 6f67 5f74 7970 6520  f self.log_type 
+00002840: 3d3d 2022 6572 726f 7222 3a0d 0a20 2020  == "error":..   
+00002850: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00002860: 662e 6c6f 6767 6572 2e65 7272 6f72 286d  f.logger.error(m
+00002870: 6573 7361 6765 290d 0a20 2020 2020 2020  essage)..       
+00002880: 2020 2020 2065 6c69 6620 7365 6c66 2e6c       elif self.l
+00002890: 6f67 5f74 7970 6520 3d3d 2022 6372 6974  og_type == "crit
+000028a0: 6963 616c 223a 0d0a 2020 2020 2020 2020  ical":..        
+000028b0: 2020 2020 2020 2020 7365 6c66 2e6c 6f67          self.log
+000028c0: 6765 722e 6372 6974 6963 616c 286d 6573  ger.critical(mes
+000028d0: 7361 6765 290d 0a0d 0a20 2020 2040 636f  sage)....    @co
+000028e0: 6e74 6578 746d 616e 6167 6572 0d0a 2020  ntextmanager..  
+000028f0: 2020 6465 6620 7469 6d65 7228 7365 6c66    def timer(self
+00002900: 2c20 7461 736b 5f6e 616d 653a 2073 7472  , task_name: str
+00002910: 2c20 7479 7065 3a20 4f70 7469 6f6e 616c  , type: Optional
+00002920: 5b54 696d 6572 5479 7065 5d20 3d22 696e  [TimerType] ="in
+00002930: 666f 2229 3a0d 0a20 2020 2020 2020 2022  fo"):..        "
+00002940: 2222 0d0a 2020 2020 2020 2020 5265 7475  ""..        Retu
+00002950: 726e 7320 6120 636f 6e74 6578 7420 6d61  rns a context ma
+00002960: 6e61 6765 7220 666f 7220 7469 6d69 6e67  nager for timing
+00002970: 2061 2062 6c6f 636b 206f 6620 636f 6465   a block of code
+00002980: 2e0d 0a0d 0a20 2020 2020 2020 2055 7361  .....        Usa
+00002990: 6765 3a0d 0a20 2020 2020 2020 2060 6060  ge:..        ```
+000029a0: 7079 7468 6f6e 0d0a 2020 2020 2020 2020  python..        
+000029b0: 7769 7468 206c 6f67 6765 722e 7469 6d65  with logger.time
+000029c0: 7228 2244 6f69 6e67 2073 6f6d 6574 6869  r("Doing somethi
+000029d0: 6e67 2e2e 2e22 2920 6173 2074 696d 6572  ng...") as timer
+000029e0: 5f63 6f6e 7465 7874 3a0d 0a20 2020 2020  _context:..     
+000029f0: 2020 2020 2020 2074 696d 652e 736c 6565         time.slee
+00002a00: 7028 3529 0d0a 2020 2020 2020 2020 2020  p(5)..          
+00002a10: 2020 656c 6170 7365 6420 3d20 7469 6d65    elapsed = time
+00002a20: 725f 636f 6e74 6578 742e 6765 745f 7469  r_context.get_ti
+00002a30: 6d65 2829 0d0a 2020 2020 2020 2020 6060  me()..        ``
+00002a40: 600d 0a20 2020 2020 2020 204c 6f67 733a  `..        Logs:
+00002a50: 0d0a 2020 2020 2020 2020 6044 6f69 6e67  ..        `Doing
+00002a60: 2073 6f6d 6574 6869 6e67 2e2e 2e3a 2035   something...: 5
+00002a70: 2e30 3032 3673 600d 0a20 2020 2020 2020  .0026s`..       
+00002a80: 2022 2222 0d0a 2020 2020 2020 2020 7469   """..        ti
+00002a90: 6d65 725f 636f 6e74 6578 7420 3d20 7365  mer_context = se
+00002aa0: 6c66 2e54 696d 6572 436f 6e74 6578 7428  lf.TimerContext(
+00002ab0: 7461 736b 5f6e 616d 652c 2073 656c 662e  task_name, self.
+00002ac0: 6164 6170 7465 722c 2074 7970 6529 0d0a  adapter, type)..
+00002ad0: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
+00002ae0: 2020 2020 2020 2020 2020 7469 6d65 725f            timer_
+00002af0: 636f 6e74 6578 742e 5f5f 656e 7465 725f  context.__enter_
+00002b00: 5f28 290d 0a20 2020 2020 2020 2020 2020  _()..           
+00002b10: 2079 6965 6c64 2074 696d 6572 5f63 6f6e   yield timer_con
+00002b20: 7465 7874 0d0a 2020 2020 2020 2020 6669  text..        fi
+00002b30: 6e61 6c6c 793a 0d0a 2020 2020 2020 2020  nally:..        
+00002b40: 2020 2020 7469 6d65 725f 636f 6e74 6578      timer_contex
+00002b50: 742e 5f5f 6578 6974 5f5f 284e 6f6e 652c  t.__exit__(None,
+00002b60: 204e 6f6e 652c 204e 6f6e 6529 0d0a 2020   None, None)..  
+00002b70: 2020 0d0a                                  ..
```

### Comparing `annonition-0.1.4/annonition.egg-info/PKG-INFO` & `annonition-0.1.5/annonition.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annonition
-Version: 0.1.4
+Version: 0.1.5
 Summary: Log everything in style.
 Author: Abtin Turing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `annonition-0.1.4/setup.py` & `annonition-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open(path.join(working_dir, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="annonition",
-    version="0.1.4",
+    version="0.1.5",
     author="Abtin Turing",
     description="Log everything in style.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

