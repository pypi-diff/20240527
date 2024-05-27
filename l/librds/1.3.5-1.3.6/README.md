# Comparing `tmp/librds-1.3.5.tar.gz` & `tmp/librds-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librds-1.3.5.tar", last modified: Sun May 26 15:36:51 2024, max compression
+gzip compressed data, was "librds-1.3.6.tar", last modified: Sun May 26 17:04:17 2024, max compression
```

## Comparing `librds-1.3.5.tar` & `librds-1.3.6.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 kuba      (1000) kuba      (1000)        0 2024-05-26 15:36:51.325839 librds-1.3.5/
--rw-rw-r--   0 kuba      (1000) kuba      (1000)    35187 2024-05-26 15:33:12.000000 librds-1.3.5/LICENCE
--rw-r--r--   0 kuba      (1000) kuba      (1000)      545 2024-05-26 15:36:51.325839 librds-1.3.5/PKG-INFO
-drwxrwxr-x   0 kuba      (1000) kuba      (1000)        0 2024-05-26 15:36:51.321839 librds-1.3.5/librds/
--rw-rw-r--   0 kuba      (1000) kuba      (1000)      255 2024-05-26 15:11:14.000000 librds-1.3.5/librds/__init__.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     3275 2024-05-26 11:06:06.000000 librds-1.3.5/librds/af.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)    17372 2024-05-26 14:56:10.000000 librds-1.3.5/librds/charset.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     1011 2024-05-25 10:25:25.000000 librds-1.3.5/librds/comfort.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     4771 2024-05-26 15:12:19.000000 librds-1.3.5/librds/decoder.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     5764 2024-05-26 10:32:08.000000 librds-1.3.5/librds/generator.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)      601 2024-05-26 09:47:47.000000 librds-1.3.5/librds/group.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     1178 2024-05-26 11:07:23.000000 librds-1.3.5/librds/interface.py
-drwxrwxr-x   0 kuba      (1000) kuba      (1000)        0 2024-05-26 15:36:51.321839 librds-1.3.5/librds.egg-info/
--rw-r--r--   0 kuba      (1000) kuba      (1000)      545 2024-05-26 15:36:51.000000 librds-1.3.5/librds.egg-info/PKG-INFO
--rw-rw-r--   0 kuba      (1000) kuba      (1000)      278 2024-05-26 15:36:51.000000 librds-1.3.5/librds.egg-info/SOURCES.txt
--rw-rw-r--   0 kuba      (1000) kuba      (1000)        1 2024-05-26 15:36:51.000000 librds-1.3.5/librds.egg-info/dependency_links.txt
--rw-rw-r--   0 kuba      (1000) kuba      (1000)        7 2024-05-26 15:36:51.000000 librds-1.3.5/librds.egg-info/top_level.txt
--rw-rw-r--   0 kuba      (1000) kuba      (1000)       38 2024-05-26 15:36:51.325839 librds-1.3.5/setup.cfg
--rw-rw-r--   0 kuba      (1000) kuba      (1000)      854 2024-05-26 15:36:26.000000 librds-1.3.5/setup.py
+drwxrwxr-x   0 kuba      (1000) kuba      (1000)        0 2024-05-26 17:04:17.705911 librds-1.3.6/
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)    35187 2024-05-26 15:33:12.000000 librds-1.3.6/LICENCE
+-rw-r--r--   0 kuba      (1000) kuba      (1000)     1619 2024-05-26 17:04:17.705911 librds-1.3.6/PKG-INFO
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)     1078 2024-05-26 16:55:12.000000 librds-1.3.6/README.md
+drwxrwxr-x   0 kuba      (1000) kuba      (1000)        0 2024-05-26 17:04:17.705911 librds-1.3.6/librds/
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)      255 2024-05-26 17:03:39.000000 librds-1.3.6/librds/__init__.py
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)     3275 2024-05-26 16:50:31.000000 librds-1.3.6/librds/af.py
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)    17372 2024-05-26 16:47:04.000000 librds-1.3.6/librds/charset.py
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)     1011 2024-05-25 10:25:25.000000 librds-1.3.6/librds/comfort.py
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)     4713 2024-05-26 16:49:35.000000 librds-1.3.6/librds/decoder.py
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)     5811 2024-05-26 16:56:09.000000 librds-1.3.6/librds/generator.py
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)      601 2024-05-26 16:49:45.000000 librds-1.3.6/librds/group.py
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)     1178 2024-05-26 11:07:23.000000 librds-1.3.6/librds/interface.py
+drwxrwxr-x   0 kuba      (1000) kuba      (1000)        0 2024-05-26 17:04:17.705911 librds-1.3.6/librds.egg-info/
+-rw-r--r--   0 kuba      (1000) kuba      (1000)     1619 2024-05-26 17:04:17.000000 librds-1.3.6/librds.egg-info/PKG-INFO
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)      288 2024-05-26 17:04:17.000000 librds-1.3.6/librds.egg-info/SOURCES.txt
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)        1 2024-05-26 17:04:17.000000 librds-1.3.6/librds.egg-info/dependency_links.txt
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)        7 2024-05-26 17:04:17.000000 librds-1.3.6/librds.egg-info/top_level.txt
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)       38 2024-05-26 17:04:17.705911 librds-1.3.6/setup.cfg
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)      851 2024-05-26 17:04:09.000000 librds-1.3.6/setup.py
```

### Comparing `librds-1.3.5/LICENCE` & `librds-1.3.6/LICENCE`

 * *Files identical despite different names*

### Comparing `librds-1.3.5/librds/af.py` & `librds-1.3.6/librds/af.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             case AF_Bands.MF:
                 self.af_freq = int(int(frequency - 531.0)/9+16)
             case AF_Bands.MF_RBDS:
                 self.af_freq = int(int(frequency - 540.0)/10+17)
     def __len__(self):
         return self.lenght
     def __repr__(self) -> str:
-        return f"<AFEntry FREQ:{self.freq} BAND:{self.band.name} AF_FREQ:{self.af_freq} LEN:{self.lenght} LFMF:{self.lfmf}>"
+        return f"<AFEntry freq={self.freq} band={self.band.name} af_freq={self.af_freq} len={self.lenght} lfmf={self.lfmf}>"
 class AlternativeFrequency:
     """This is a working Alterntive Frequency implementation that was tested on FM, LF, MF, RBDS MF
     however the rbds MF does have a problem, on rds mf 540 and 549 work but 550 doesnt, this is expected as 550 is not divisible by 9 as in europe am has a 9 khz step
     in the us however am has a 10 khz step 540 works as expected but 549 round to 540, as expected but 550 does the same?
     but im doing rbds out of generosity, not need or want"""
     def __init__(self, af:list[AlternativeFrequencyEntry]=[]) -> None:
         self.af = af
```

### Comparing `librds-1.3.5/librds/charset.py` & `librds-1.3.6/librds/charset.py`

 * *Files identical despite different names*

### Comparing `librds-1.3.5/librds/comfort.py` & `librds-1.3.6/librds/comfort.py`

 * *Files identical despite different names*

### Comparing `librds-1.3.5/librds/decoder.py` & `librds-1.3.6/librds/decoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from enum import IntEnum
 from .charset import RDSCharsetDecode
 from .group import Group, dataclass
 
 @dataclass
 class Details:
     details=True
-
 @dataclass
 class PSDetails(Details):
     segment: int
     di: int
     ms: bool
     ta: bool
     text: str
@@ -19,68 +18,65 @@
     ab: int
     text: str
 @dataclass
 class PTYNDetails(Details):
     segment: int
     ab: int
     text: str
-    
 @dataclass
 class ECCLICDetails(Details):
     data:int
     is_lic:bool
-
 @dataclass
 class DecodedGroup:
     raw_group:Group
     pi: int
     tp: bool
     pty: int
     group: IntEnum
     details:Details
-
 class GroupDecoder:
     def _decode_0(self, group: Group, dgroup: DecodedGroup):
         segment = group.b & 3
         ta = (group.b >> 4) & 1
         ms = (group.b >> 3) & 1
         if segment == 3:
             di = (group.b >> 2) & 9
         else:
             di = 0
         details = PSDetails(segment,di,bool(ms),bool(ta),"")
-        
+
         char_1 = (group.d >> 8) & 0xFF
         char_2 = group.d & 0xFF
         details.text += RDSCharsetDecode.translate(char_1)
         details.text += RDSCharsetDecode.translate(char_2)
-        
+
         dgroup.details = details
         return group, dgroup
     def _decode_2(self, group: Group, dgroup: DecodedGroup):
         dgroup.group = 2
         segment = group.b & 15
         ab = (group.b >> 4) & 1
         details = RTDetails(segment,ab,"")
-        
+
         if not group.is_version_b:
             char_1 = (group.c >> 8) & 0xFF
             char_2 = group.c & 0xFF
             char_3 = (group.d >> 8) & 0xFF
             char_4 = group.d & 0xFF
             details.text += RDSCharsetDecode.translate(char_1)
             details.text += RDSCharsetDecode.translate(char_2)
             details.text += RDSCharsetDecode.translate(char_3)
             details.text += RDSCharsetDecode.translate(char_4)
         else:
             char_1 = (group.d >> 8) & 0xFF
             char_2 = group.d & 0xFF
             details.text += RDSCharsetDecode.translate(char_1)
             details.text += RDSCharsetDecode.translate(char_2)
-        
+
         dgroup.details = details
         return group, dgroup
     def _decode_1(self, group:Group, dgroup:DecodedGroup):
         dgroup.group = 1
         tmp = (group.c & 0xFF)
         details = ECCLICDetails(0,False)
         if tmp < 0x46:
@@ -99,16 +95,14 @@
         char_4 = group.d & 0xFF
         details.text += RDSCharsetDecode.translate(char_1)
         details.text += RDSCharsetDecode.translate(char_2)
         details.text += RDSCharsetDecode.translate(char_3)
         details.text += RDSCharsetDecode.translate(char_4)
         dgroup.details = details
         return group, dgroup
-        
-        
     def decode(self, group: Group):
         out = DecodedGroup(group,group.a,False,0,0,None)
         out.pty = ((group.b >> 5) & 31)
         out.tp = bool((group.b >> 10) & 1)
         gr = (group.b >> 12) & ((1 << 12) - 1)
         if group.is_version_b and gr != 0: gr -= 1
         match gr:
```

### Comparing `librds-1.3.5/librds/generator.py` & `librds-1.3.6/librds/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .group import Group
 from .comfort import get_from_list
 from .af import AlternativeFrequency
 from .charset import *
 
 class GroupGenerator:
     def basic(pi:int, tp: bool=False, pty: int=0):
-        """This function will generate a basic block structure which includes the PI, TP and PTY"""
+        """This function will generate a basic block structure which includes the PI, TP and PTY, this shouldn't be sent by itself to a decoder"""
         return Group(
             pi & 0xFFFF, #A
             (int(tp) << 10 | pty << 5) & 0xFFFF, #B
             0,0, #C
             None #is_b
         )
     def ps(blocks:Group,ps_text:str,segment:int,ms:bool=True,ta:bool=False,di:int=1,block2:int=0):
```

### Comparing `librds-1.3.5/librds/group.py` & `librds-1.3.6/librds/group.py`

 * *Files identical despite different names*

### Comparing `librds-1.3.5/librds/interface.py` & `librds-1.3.6/librds/interface.py`

 * *Files identical despite different names*

