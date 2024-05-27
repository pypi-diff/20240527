# Comparing `tmp/FastHPOCR-0.1.1.tar.gz` & `tmp/FastHPOCR-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FastHPOCR-0.1.1.tar", last modified: Mon May 20 10:59:05 2024, max compression
+gzip compressed data, was "FastHPOCR-0.1.2.tar", last modified: Mon May 27 04:21:23 2024, max compression
```

## Comparing `FastHPOCR-0.1.1.tar` & `FastHPOCR-0.1.2.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-20 10:59:05.212227 FastHPOCR-0.1.1/
-drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-20 10:59:05.204017 FastHPOCR-0.1.1/FastHPOCR/
--rw-r--r--   0 tudor      (501) staff       (20)     1295 2024-05-15 11:08:04.000000 FastHPOCR-0.1.1/FastHPOCR/HPOAnnotator.py
--rw-r--r--   0 tudor      (501) staff       (20)     5044 2024-05-20 10:46:20.000000 FastHPOCR-0.1.1/FastHPOCR/IndexHPO.py
--rw-r--r--   0 tudor      (501) staff       (20)     3491 2024-05-15 11:09:02.000000 FastHPOCR-0.1.1/FastHPOCR/IndexORPHANET.py
--rw-r--r--   0 tudor      (501) staff       (20)     4492 2024-05-15 11:09:14.000000 FastHPOCR-0.1.1/FastHPOCR/IndexSNOMED.py
--rw-r--r--   0 tudor      (501) staff       (20)     3507 2024-05-06 04:11:34.000000 FastHPOCR-0.1.1/FastHPOCR/README.md
--rw-r--r--   0 tudor      (501) staff       (20)        0 2024-03-18 01:56:25.000000 FastHPOCR-0.1.1/FastHPOCR/__init__.py
-drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-20 10:59:05.205680 FastHPOCR-0.1.1/FastHPOCR/cr/
--rw-r--r--   0 tudor      (501) staff       (20)     3621 2024-05-15 11:06:19.000000 FastHPOCR-0.1.1/FastHPOCR/cr/CRIndexKB.py
--rw-r--r--   0 tudor      (501) staff       (20)     1051 2024-02-21 03:39:40.000000 FastHPOCR-0.1.1/FastHPOCR/cr/CandidateMatcher.py
--rw-r--r--   0 tudor      (501) staff       (20)     3642 2024-05-15 11:08:04.000000 FastHPOCR-0.1.1/FastHPOCR/cr/FormatResults.py
--rw-r--r--   0 tudor      (501) staff       (20)     1734 2024-03-02 08:55:02.000000 FastHPOCR-0.1.1/FastHPOCR/cr/SequenceCache.py
--rw-r--r--   0 tudor      (501) staff       (20)     3675 2024-05-15 11:08:04.000000 FastHPOCR-0.1.1/FastHPOCR/cr/TextProcessor.py
--rw-r--r--   0 tudor      (501) staff       (20)     3875 2024-05-15 11:06:36.000000 FastHPOCR-0.1.1/FastHPOCR/cr/TextSplitter.py
--rw-r--r--   0 tudor      (501) staff       (20)        0 2024-02-23 02:34:40.000000 FastHPOCR-0.1.1/FastHPOCR/cr/__init__.py
-drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-20 10:59:05.207309 FastHPOCR-0.1.1/FastHPOCR/index/
--rw-r--r--   0 tudor      (501) staff       (20)     1858 2024-05-20 10:46:20.000000 FastHPOCR-0.1.1/FastHPOCR/index/HPOLabelCollector.py
--rw-r--r--   0 tudor      (501) staff       (20)     2323 2024-05-15 11:06:42.000000 FastHPOCR-0.1.1/FastHPOCR/index/IndexTerms.py
--rw-r--r--   0 tudor      (501) staff       (20)     3564 2024-05-15 13:22:03.000000 FastHPOCR-0.1.1/FastHPOCR/index/LabelProcessor.py
--rw-r--r--   0 tudor      (501) staff       (20)     1062 2024-05-15 11:08:04.000000 FastHPOCR-0.1.1/FastHPOCR/index/ORPHALabelCollector.py
--rw-r--r--   0 tudor      (501) staff       (20)     2668 2024-05-20 10:46:20.000000 FastHPOCR-0.1.1/FastHPOCR/index/PreprocessHPOTerms.py
--rw-r--r--   0 tudor      (501) staff       (20)     2157 2024-05-15 11:08:04.000000 FastHPOCR-0.1.1/FastHPOCR/index/PreprocessORPHATerms.py
--rw-r--r--   0 tudor      (501) staff       (20)     2135 2024-05-15 11:08:04.000000 FastHPOCR-0.1.1/FastHPOCR/index/PreprocessSNOMEDTerms.py
--rw-r--r--   0 tudor      (501) staff       (20)     1703 2024-05-15 11:08:04.000000 FastHPOCR-0.1.1/FastHPOCR/index/SNOMEDLabelCollector.py
--rw-r--r--   0 tudor      (501) staff       (20)     3036 2024-05-02 09:49:49.000000 FastHPOCR-0.1.1/FastHPOCR/index/SNOMEDParser.py
--rw-r--r--   0 tudor      (501) staff       (20)     2556 2024-02-28 12:38:42.000000 FastHPOCR-0.1.1/FastHPOCR/index/SynonymExpader.py
--rw-r--r--   0 tudor      (501) staff       (20)        0 2024-02-23 02:34:32.000000 FastHPOCR-0.1.1/FastHPOCR/index/__init__.py
--rw-r--r--   0 tudor      (501) staff       (20)     1058 2024-03-18 01:51:44.000000 FastHPOCR-0.1.1/FastHPOCR/license.txt
-drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-20 10:59:05.207583 FastHPOCR-0.1.1/FastHPOCR/resources/
--rw-r--r--   0 tudor      (501) staff       (20)     1385 2024-05-13 14:33:20.000000 FastHPOCR-0.1.1/FastHPOCR/resources/base-synonyms
--rw-r--r--   0 tudor      (501) staff       (20)  6300038 2024-05-14 04:27:52.000000 FastHPOCR-0.1.1/FastHPOCR/resources/vocab.clusters.list
-drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-20 10:59:05.211912 FastHPOCR-0.1.1/FastHPOCR/util/
--rw-r--r--   0 tudor      (501) staff       (20)      828 2024-02-20 02:33:16.000000 FastHPOCR-0.1.1/FastHPOCR/util/AnnotationObject.py
--rw-r--r--   0 tudor      (501) staff       (20)     1123 2024-05-15 11:07:20.000000 FastHPOCR-0.1.1/FastHPOCR/util/AnnotationToken.py
--rw-r--r--   0 tudor      (501) staff       (20)     1511 2024-05-02 10:33:44.000000 FastHPOCR-0.1.1/FastHPOCR/util/CRConstants.py
--rw-r--r--   0 tudor      (501) staff       (20)     1196 2024-05-14 04:26:12.000000 FastHPOCR-0.1.1/FastHPOCR/util/ContentUtil.py
--rw-r--r--   0 tudor      (501) staff       (20)     4740 2024-05-15 11:07:31.000000 FastHPOCR-0.1.1/FastHPOCR/util/OntoReader.py
--rw-r--r--   0 tudor      (501) staff       (20)    42275 2024-03-02 08:55:57.000000 FastHPOCR-0.1.1/FastHPOCR/util/SequenceData.py
--rw-r--r--   0 tudor      (501) staff       (20)        0 2024-02-23 02:36:52.000000 FastHPOCR-0.1.1/FastHPOCR/util/__init__.py
-drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-20 10:59:05.204618 FastHPOCR-0.1.1/FastHPOCR.egg-info/
--rw-r--r--   0 tudor      (501) staff       (20)      206 2024-05-20 10:59:05.000000 FastHPOCR-0.1.1/FastHPOCR.egg-info/PKG-INFO
--rw-r--r--   0 tudor      (501) staff       (20)     1190 2024-05-20 10:59:05.000000 FastHPOCR-0.1.1/FastHPOCR.egg-info/SOURCES.txt
--rw-r--r--   0 tudor      (501) staff       (20)        1 2024-05-20 10:59:05.000000 FastHPOCR-0.1.1/FastHPOCR.egg-info/dependency_links.txt
--rw-r--r--   0 tudor      (501) staff       (20)       10 2024-05-20 10:59:05.000000 FastHPOCR-0.1.1/FastHPOCR.egg-info/top_level.txt
--rw-r--r--   0 tudor      (501) staff       (20)      206 2024-05-20 10:59:05.212085 FastHPOCR-0.1.1/PKG-INFO
--rw-r--r--   0 tudor      (501) staff       (20)       38 2024-05-20 10:59:05.212288 FastHPOCR-0.1.1/setup.cfg
--rw-r--r--   0 tudor      (501) staff       (20)      447 2024-05-20 10:58:13.000000 FastHPOCR-0.1.1/setup.py
+drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-27 04:21:23.396238 FastHPOCR-0.1.2/
+drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-27 04:21:23.388494 FastHPOCR-0.1.2/FastHPOCR/
+-rw-r--r--   0 tudor      (501) staff       (20)     1934 2024-05-24 14:17:49.000000 FastHPOCR-0.1.2/FastHPOCR/HPOAnnotator.py
+-rw-r--r--   0 tudor      (501) staff       (20)     5162 2024-05-24 14:18:38.000000 FastHPOCR-0.1.2/FastHPOCR/IndexHPO.py
+-rw-r--r--   0 tudor      (501) staff       (20)     5109 2024-05-24 14:19:15.000000 FastHPOCR-0.1.2/FastHPOCR/IndexORPHANET.py
+-rw-r--r--   0 tudor      (501) staff       (20)     6736 2024-05-24 14:19:44.000000 FastHPOCR-0.1.2/FastHPOCR/IndexSNOMED.py
+-rw-r--r--   0 tudor      (501) staff       (20)     5385 2024-05-27 04:17:46.000000 FastHPOCR-0.1.2/FastHPOCR/README.md
+-rw-r--r--   0 tudor      (501) staff       (20)        0 2024-03-18 01:56:25.000000 FastHPOCR-0.1.2/FastHPOCR/__init__.py
+drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-27 04:21:23.390036 FastHPOCR-0.1.2/FastHPOCR/cr/
+-rw-r--r--   0 tudor      (501) staff       (20)     4627 2024-05-24 14:15:10.000000 FastHPOCR-0.1.2/FastHPOCR/cr/CRIndexKB.py
+-rw-r--r--   0 tudor      (501) staff       (20)     1051 2024-02-21 03:39:40.000000 FastHPOCR-0.1.2/FastHPOCR/cr/CandidateMatcher.py
+-rw-r--r--   0 tudor      (501) staff       (20)     3738 2024-05-24 14:15:10.000000 FastHPOCR-0.1.2/FastHPOCR/cr/FormatResults.py
+-rw-r--r--   0 tudor      (501) staff       (20)     1734 2024-03-02 08:55:02.000000 FastHPOCR-0.1.2/FastHPOCR/cr/SequenceCache.py
+-rw-r--r--   0 tudor      (501) staff       (20)     3675 2024-05-24 14:14:48.000000 FastHPOCR-0.1.2/FastHPOCR/cr/TextProcessor.py
+-rw-r--r--   0 tudor      (501) staff       (20)     3875 2024-05-24 14:14:51.000000 FastHPOCR-0.1.2/FastHPOCR/cr/TextSplitter.py
+-rw-r--r--   0 tudor      (501) staff       (20)        0 2024-02-23 02:34:40.000000 FastHPOCR-0.1.2/FastHPOCR/cr/__init__.py
+drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-27 04:21:23.391765 FastHPOCR-0.1.2/FastHPOCR/index/
+-rw-r--r--   0 tudor      (501) staff       (20)     2864 2024-05-24 14:17:49.000000 FastHPOCR-0.1.2/FastHPOCR/index/HPOLabelCollector.py
+-rw-r--r--   0 tudor      (501) staff       (20)     2535 2024-05-24 14:17:49.000000 FastHPOCR-0.1.2/FastHPOCR/index/IndexTerms.py
+-rw-r--r--   0 tudor      (501) staff       (20)     4635 2024-05-24 14:17:49.000000 FastHPOCR-0.1.2/FastHPOCR/index/LabelProcessor.py
+-rw-r--r--   0 tudor      (501) staff       (20)     1659 2024-05-24 14:17:49.000000 FastHPOCR-0.1.2/FastHPOCR/index/ORPHALabelCollector.py
+-rw-r--r--   0 tudor      (501) staff       (20)     3339 2024-05-24 14:17:49.000000 FastHPOCR-0.1.2/FastHPOCR/index/PreprocessHPOTerms.py
+-rw-r--r--   0 tudor      (501) staff       (20)     2439 2024-05-24 14:17:49.000000 FastHPOCR-0.1.2/FastHPOCR/index/PreprocessORPHATerms.py
+-rw-r--r--   0 tudor      (501) staff       (20)     2699 2024-05-24 14:17:49.000000 FastHPOCR-0.1.2/FastHPOCR/index/PreprocessSNOMEDTerms.py
+-rw-r--r--   0 tudor      (501) staff       (20)     2476 2024-05-24 14:17:49.000000 FastHPOCR-0.1.2/FastHPOCR/index/SNOMEDLabelCollector.py
+-rw-r--r--   0 tudor      (501) staff       (20)     4804 2024-05-24 14:17:49.000000 FastHPOCR-0.1.2/FastHPOCR/index/SNOMEDParser.py
+-rw-r--r--   0 tudor      (501) staff       (20)     2853 2024-05-24 01:59:14.000000 FastHPOCR-0.1.2/FastHPOCR/index/SynonymExpader.py
+-rw-r--r--   0 tudor      (501) staff       (20)        0 2024-02-23 02:34:32.000000 FastHPOCR-0.1.2/FastHPOCR/index/__init__.py
+-rw-r--r--   0 tudor      (501) staff       (20)     1058 2024-03-18 01:51:44.000000 FastHPOCR-0.1.2/FastHPOCR/license.txt
+drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-27 04:21:23.392014 FastHPOCR-0.1.2/FastHPOCR/resources/
+-rw-r--r--   0 tudor      (501) staff       (20)     1385 2024-05-13 14:33:20.000000 FastHPOCR-0.1.2/FastHPOCR/resources/base-synonyms
+-rw-r--r--   0 tudor      (501) staff       (20)  6300038 2024-05-14 04:27:52.000000 FastHPOCR-0.1.2/FastHPOCR/resources/vocab.clusters.list
+drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-27 04:21:23.395979 FastHPOCR-0.1.2/FastHPOCR/util/
+-rw-r--r--   0 tudor      (501) staff       (20)     1596 2024-05-24 02:31:08.000000 FastHPOCR-0.1.2/FastHPOCR/util/AnnotationObject.py
+-rw-r--r--   0 tudor      (501) staff       (20)     1123 2024-05-24 14:15:02.000000 FastHPOCR-0.1.2/FastHPOCR/util/AnnotationToken.py
+-rw-r--r--   0 tudor      (501) staff       (20)     1511 2024-05-02 10:33:44.000000 FastHPOCR-0.1.2/FastHPOCR/util/CRConstants.py
+-rw-r--r--   0 tudor      (501) staff       (20)      220 2024-05-24 01:30:25.000000 FastHPOCR-0.1.2/FastHPOCR/util/ConfigConstants.py
+-rw-r--r--   0 tudor      (501) staff       (20)     1196 2024-05-14 04:26:12.000000 FastHPOCR-0.1.2/FastHPOCR/util/ContentUtil.py
+-rw-r--r--   0 tudor      (501) staff       (20)     4740 2024-05-24 14:15:17.000000 FastHPOCR-0.1.2/FastHPOCR/util/OntoReader.py
+-rw-r--r--   0 tudor      (501) staff       (20)    42275 2024-03-02 08:55:57.000000 FastHPOCR-0.1.2/FastHPOCR/util/SequenceData.py
+-rw-r--r--   0 tudor      (501) staff       (20)        0 2024-02-23 02:36:52.000000 FastHPOCR-0.1.2/FastHPOCR/util/__init__.py
+drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-27 04:21:23.388957 FastHPOCR-0.1.2/FastHPOCR.egg-info/
+-rw-r--r--   0 tudor      (501) staff       (20)      206 2024-05-27 04:21:23.000000 FastHPOCR-0.1.2/FastHPOCR.egg-info/PKG-INFO
+-rw-r--r--   0 tudor      (501) staff       (20)     1224 2024-05-27 04:21:23.000000 FastHPOCR-0.1.2/FastHPOCR.egg-info/SOURCES.txt
+-rw-r--r--   0 tudor      (501) staff       (20)        1 2024-05-27 04:21:23.000000 FastHPOCR-0.1.2/FastHPOCR.egg-info/dependency_links.txt
+-rw-r--r--   0 tudor      (501) staff       (20)       10 2024-05-27 04:21:23.000000 FastHPOCR-0.1.2/FastHPOCR.egg-info/top_level.txt
+-rw-r--r--   0 tudor      (501) staff       (20)      206 2024-05-27 04:21:23.396118 FastHPOCR-0.1.2/PKG-INFO
+-rw-r--r--   0 tudor      (501) staff       (20)       38 2024-05-27 04:21:23.396280 FastHPOCR-0.1.2/setup.cfg
+-rw-r--r--   0 tudor      (501) staff       (20)      447 2024-05-27 04:20:53.000000 FastHPOCR-0.1.2/setup.py
```

### Comparing `FastHPOCR-0.1.1/FastHPOCR/HPOAnnotator.py` & `FastHPOCR-0.1.2/FastHPOCR/HPOAnnotator.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,29 +8,47 @@
 class HPOAnnotator:
     crIndexKB = None
 
     def __init__(self, crDataFile):
         self.crIndexKB = CRIndexKB()
         self.crIndexKB.load(crDataFile)
 
-    def annotate(self, text: str, longestMatch = False) -> [AnnotationObject]:
+    def annotate(self, text: str, longestMatch=False) -> [AnnotationObject]:
         textProcessor = TextProcessor(self.crIndexKB)
         textProcessor.process(text)
 
         candidateMatcher = CandidateMatcher(self.crIndexKB)
         candidateMatcher.matchCandidates(textProcessor.getCandidates())
 
         result = FormatResults(text, self.crIndexKB, candidateMatcher.getMatches(), longestMatch).getResult()
         return result
 
-    def printResults(self, annotationList):
+    def printResults(self, annotationList, includeCategoriesIfPresent=False):
         lines = []
         for annotationObject in annotationList:
-            lines.append(annotationObject.toString())
+            if includeCategoriesIfPresent:
+                lines.append(annotationObject.toStringWithCategories())
+            else:
+                lines.append(annotationObject.toString())
         print('\n'.join(lines))
 
-    def serialize(self, annotationList, fileOut):
+    def serialize(self, annotationList, fileOut, includeCategoriesIfPresent=False):
         lines = []
         for annotationObject in annotationList:
-            lines.append(annotationObject.toString())
+            if includeCategoriesIfPresent:
+                lines.append(annotationObject.toStringWithCategories())
+            else:
+                lines.append(annotationObject.toString())
         with open(fileOut, 'w') as fh:
             fh.write('\n'.join(lines))
+
+
+def main():
+    hpoAnnotator = HPOAnnotator('/Users/tudor/Desktop/FFF/Test/hp.index')
+
+    text = 'cancer'
+    result = hpoAnnotator.annotate(text)
+    hpoAnnotator.serialize(result, '/Users/tudor/Desktop/FFF/Test/res.txt', includeCategoriesIfPresent=True)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `FastHPOCR-0.1.1/FastHPOCR/IndexHPO.py` & `FastHPOCR-0.1.2/FastHPOCR/IndexHPO.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,66 +3,64 @@
 import time
 from os.path import join
 
 from FastHPOCR.cr.CRIndexKB import CRIndexKB
 from FastHPOCR.index.IndexTerms import IndexTerms
 from FastHPOCR.index.PreprocessHPOTerms import PreprocessHPOTerms
 from FastHPOCR.index.SynonymExpader import SynonymExpader
+from FastHPOCR.util import ConfigConstants
 from FastHPOCR.util.CRConstants import HP_INDEX_FILE, BASE_CLUSTERS, BASE_SYNONYMS
 
 
 class IndexHPO:
     resFolder = None
     hpoLocation = None
     outputFolder = None
-    externalSynFile = None
+    indexConfig = {}
     valid = False
-    allow3LetterAcronyms = False
-    rootConcepts = []
 
     clusters = {}
     synClusters = {}
     externalSynonyms = {}
     crIndexKB = None
 
-    def __init__(self, hpoLocation: str, outputFolder: str, rootConcepts=[], externalSynFile=None, allow3LetterAcronyms=False):
+    def __init__(self, hpoLocation: str, outputFolder: str, indexConfig={}):
         self.resFolder = 'resources'
         self.hpoLocation = hpoLocation
         self.outputFolder = outputFolder
-        self.externalSynFile = externalSynFile
-        self.rootConcepts = rootConcepts
+        self.indexConfig = indexConfig
         self.valid = False
-        self.allow3LetterAcronyms = allow3LetterAcronyms
         self.crIndexKB = CRIndexKB()
         self.externalSynonyms = {}
 
     def index(self):
         start = time.time()
         self.checkPrerequisites()
         if not self.valid:
             return
 
         self.loadPrerequisites()
         print(' - Preprocessing HPO terms ...')
         preprocessHPOTerms = PreprocessHPOTerms(self.hpoLocation,
-                                                rootConcepts=self.rootConcepts,
                                                 externalSynonyms=self.externalSynonyms,
-                                                allow3LetterAcronyms=self.allow3LetterAcronyms)
+                                                indexConfig=self.indexConfig)
         processedTerms = preprocessHPOTerms.getProcessedTerms()
+        catDictionary = preprocessHPOTerms.getCategoriesDictionary()
 
         print(' - Indexing HPO terms ...')
         indexTerms = IndexTerms(processedTerms, self.clusters, self.crIndexKB)
         termsToIndex = indexTerms.getTermsToIndex()
         voidTokens = indexTerms.getVoidTokens()
 
         synonymExpader = SynonymExpader(termsToIndex, voidTokens, self.synClusters)
         termsToIndex = synonymExpader.getTermsToIndex()
 
         print(' - Serializing index ...')
         self.crIndexKB.setHPOIndex(termsToIndex)
+        self.crIndexKB.setCatDictionary(catDictionary)
         self.crIndexKB.serialize(join(self.outputFolder, HP_INDEX_FILE), self.clusters)
         end = time.time()
         print(' - HPO index created in {}s'.format(round(end - start, 2)))
 
     def loadPrerequisites(self):
         self.loadClusterData()
         self.loadSynClusters()
@@ -94,17 +92,22 @@
                     token = token.strip()
                     clusterSet.append(self.clusters[token])
                 for token in tokens:
                     token = token.strip()
                     self.synClusters[self.clusters[token]] = clusterSet
 
     def loadExternalSynonyms(self):
-        if not self.externalSynFile:
+        if not self.indexConfig:
             return
-        with open(self.externalSynFile, 'r') as fh:
+
+        if self.indexConfig:
+            if not ConfigConstants.VAR_EXTENAL_SYNS in self.indexConfig:
+                return
+
+        with open(self.indexConfig[ConfigConstants.VAR_EXTENAL_SYNS], 'r') as fh:
             lines = fh.readlines()
 
         for line in lines:
             line = line.strip()
             if not line:
                 continue
             segs = line.split('=')
@@ -126,13 +129,14 @@
             self.valid = False
             return
         if not os.path.isdir(self.outputFolder):
             print('ERROR: Output folder provided [{}] does not exist!'.format(self.outputFolder))
             self.valid = False
             return
 
-        if self.externalSynFile:
-            if not os.path.isfile(self.externalSynFile):
-                print('WARNING: External synonyms file provided [{}] does not exist!'.format(self.externalSynFile))
-                self.externalSynFile = None
+        if self.indexConfig:
+            if ConfigConstants.VAR_EXTENAL_SYNS in self.indexConfig:
+                if not os.path.isfile(self.indexConfig[ConfigConstants.VAR_EXTENAL_SYNS]):
+                    print('WARNING: External synonyms file provided [{}] does not exist!'.format(
+                        self.indexConfig[ConfigConstants.VAR_EXTENAL_SYNS]))
 
         self.valid = True
```

### Comparing `FastHPOCR-0.1.1/FastHPOCR/cr/CRIndexKB.py` & `FastHPOCR-0.1.2/FastHPOCR/cr/CRIndexKB.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,19 +6,23 @@
 
 class CRIndexKB:
     clusters = {}
     invertedClusters = {}
     hpoIndex = {}
 
     uriBasedIndex = {}
+    uriCategories = {}
     clusterSetBasedIndex = {}
+    catDictionary = {}
 
     def __init__(self):
         self.clusters = {}
         self.invertedClusters = {}
+        self.catDictionary = {}
+        self.uriCategories = {}
 
         self.hpoIndex = []
         self.uriBasedIndex = {}
         self.clusterSetBasedIndex = {}
 
     def addToInvertedClusters(self, token, clusterId):
         self.invertedClusters[token] = clusterId
@@ -40,29 +44,37 @@
         for token in baseClusters:
             if baseClusters[token] == clusterId:
                 tokenList.append(token)
         return tokenList
 
     def setHPOIndex(self, termsToIndex):
         for uri in termsToIndex:
-            self.hpoIndex.append({
+            entry = {
                 'uri': uri,
-                'labels': termsToIndex[uri]
-            })
+                'labels': termsToIndex[uri]['labels']
+            }
+            if 'categories' in termsToIndex[uri]:
+                entry['categories'] = termsToIndex[uri]['categories']
+            self.hpoIndex.append(entry)
+
+    def setCatDictionary(self, catDictionary):
+        self.catDictionary = catDictionary
 
     def load(self, crIndexKBFile):
         with open(crIndexKBFile, 'r') as fh:
             crData = json.load(fh)
 
         self.clusters = crData['clusters']
         for clusterId in self.clusters:
             for entry in self.clusters[clusterId]:
                 self.invertedClusters[entry] = clusterId
 
         self.hpoIndex = crData['termData']
+        if 'catDictionary' in crData:
+            self.catDictionary = crData['catDictionary']
         self.restructureHPOIndex()
 
     def restructureHPOIndex(self):
         for term in self.hpoIndex:
             uri = term['uri']
             labels = term['labels']
 
@@ -85,30 +97,49 @@
 
                 lst = []
                 if clusterSig in clusterData:
                     lst = clusterData[clusterSig]
                 lst.append(label)
                 clusterData[clusterSig] = lst
             self.uriBasedIndex[uri] = clusterData
+            if 'categories' in term:
+                self.uriCategories[uri] = term['categories']
 
     def getClusterBasedTerms(self, clusterSig):
         if clusterSig in self.clusterSetBasedIndex:
             return self.clusterSetBasedIndex[clusterSig]
         return None
 
     def getLabelsForUri(self, uri, clusterSig):
         return self.uriBasedIndex[uri][clusterSig]
 
+    def getCategoriesForUri(self, uri):
+        if not self.catDictionary:
+            return []
+
+        if not uri in self.uriCategories:
+            return []
+
+        result = []
+        for cat in self.uriCategories[uri]:
+            result.append({
+                'uri': cat,
+                'label': self.catDictionary[cat]
+            })
+        return result
+
     def serialize(self, fileOut, baseClusters):
         self.prepareClustersToSerialise(baseClusters)
 
         data = {
             'termData': self.hpoIndex,
             'clusters': self.clusters
         }
+        if self.catDictionary:
+            data['catDictionary'] = self.catDictionary
 
         with open(fileOut, 'w') as fh:
             json.dump(data, fh, sort_keys=True, indent=4)
 
     def getClusterId(self, token):
         if token in self.invertedClusters:
             return self.invertedClusters[token]
```

### Comparing `FastHPOCR-0.1.1/FastHPOCR/cr/CandidateMatcher.py` & `FastHPOCR-0.1.2/FastHPOCR/cr/CandidateMatcher.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.1/FastHPOCR/cr/FormatResults.py` & `FastHPOCR-0.1.2/FastHPOCR/cr/FormatResults.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,20 +59,21 @@
                             continue
                         else:
                             if label['native']:
                                 finalLabel = label
                                 finalUri = uri
                                 break
 
+            categoryInfo = self.crIndexKB.getCategoriesForUri(finalUri)
             tempResults[position] = AnnotationObject(compressedCandidate['textSpan'],
                                                      finalUri,
                                                      finalLabel['originalLabel'],
                                                      compressedCandidate['startOffset'],
-                                                     compressedCandidate['endOffset']
-                                                     )
+                                                     compressedCandidate['endOffset'],
+                                                     categories=categoryInfo)
 
         for entry in tempResults:
             self.result.append(tempResults[entry])
 
     def compressCandidate(self, candidate):
         min = 10000
         max = 0
```

### Comparing `FastHPOCR-0.1.1/FastHPOCR/cr/SequenceCache.py` & `FastHPOCR-0.1.2/FastHPOCR/cr/SequenceCache.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.1/FastHPOCR/cr/TextProcessor.py` & `FastHPOCR-0.1.2/FastHPOCR/cr/TextProcessor.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.1/FastHPOCR/cr/TextSplitter.py` & `FastHPOCR-0.1.2/FastHPOCR/cr/TextSplitter.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.1/FastHPOCR/index/IndexTerms.py` & `FastHPOCR-0.1.2/FastHPOCR/index/IndexTerms.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,20 +23,26 @@
         self.termsToIndex = {}
         self.newClusterData = {}
 
         self.indexTerms()
 
     def indexTerms(self):
         for uri in self.processedTerms:
-            labelSet = self.processedTerms[uri]
+            labelSet = self.processedTerms[uri]['terms']
 
             readyLabels = []
             for label in labelSet:
                 readyLabels.append(self.prepareLabel(label))
-            self.termsToIndex[uri] = readyLabels
+
+            entry = {
+                'labels': readyLabels
+            }
+            if 'categories' in self.processedTerms[uri]:
+                entry['categories'] = self.processedTerms[uri]['categories']
+            self.termsToIndex[uri] = entry
 
     def prepareLabel(self, label):
         clusterIds = []
 
         for el in label['tokens']:
             if el['token'] in self.baseClusters:
                 clusterId = self.baseClusters[el['token']]
```

### Comparing `FastHPOCR-0.1.1/FastHPOCR/index/LabelProcessor.py` & `FastHPOCR-0.1.2/FastHPOCR/index/LabelProcessor.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,42 @@
+from FastHPOCR.util import ConfigConstants
+
+
 class LabelProcessor:
     terms = {}
     labels = {}
     dupLabels = {}
     allow3LetterAcronyms = False
+    allowDuplicateEntries = False
 
-    def __init__(self, terms, allow3LetterAcronyms=False):
+    def __init__(self, terms, indexConfig={}):
         self.terms = terms
-        self.allow3LetterAcronyms = allow3LetterAcronyms
         self.labels = {}
         self.dupLabels = {}
+        self.processConfig(indexConfig)
 
         print(' - Processing labels ...')
         self.processBracketsInLabels()
         print(' - Collected {} terms.'.format(len(self.terms)))
         print(' - Found {} duplicated labels.'.format(len(self.dupLabels)))
         for label in self.dupLabels:
             print(' -- {} -> {}'.format(label, self.dupLabels[label]))
-        self.processDuplicates()
+        if not self.allowDuplicateEntries:
+            self.processDuplicates()
+
+    def processConfig(self, indexConfig):
+        if not indexConfig:
+            self.allow3LetterAcronyms = False
+            self.allowDuplicateEntries = False
+            return
+
+        if ConfigConstants.VAR_3LETTER_ACRONYMS in indexConfig:
+            self.allow3LetterAcronyms = indexConfig[ConfigConstants.VAR_3LETTER_ACRONYMS]
+        if ConfigConstants.VAR_ALLOW_DUPLICATE_ENTRIES in indexConfig:
+            self.allowDuplicateEntries = indexConfig[ConfigConstants.VAR_ALLOW_DUPLICATE_ENTRIES]
 
     def processBracketsInLabels(self):
         for uri in self.terms:
             label = self.terms[uri]['label']
             syns = self.terms[uri]['syns']
 
             newSyns = []
@@ -29,22 +45,25 @@
             for syn in syns:
                 procced = self.processBrackets(syn, isSyn=True)
                 if procced:
                     size = 4
                     if self.allow3LetterAcronyms:
                         size = 3
 
-                    if len(syn) < size:
+                    if len(syn) < size and syn.isupper():
                         continue
                     newSyns.append(syn)
 
-            self.terms[uri] = {
+            entry = {
                 'label': label,
                 'syns': newSyns
             }
+            if 'categories' in self.terms[uri]:
+                entry['categories'] = self.terms[uri]['categories']
+            self.terms[uri] = entry
 
             if not label in self.labels:
                 self.labels[label] = uri
             else:
                 existUri = self.labels[label]
                 self.labels.pop(label)
 
@@ -80,33 +99,38 @@
             label = self.terms[uri]['label']
             syns = self.terms[uri]['syns']
 
             newSyns = []
             for syn in syns:
                 if not syn in self.labels:
                     newSyns.append(syn)
-
-            self.terms[uri] = {
+            entry = {
                 'label': label,
                 'syns': newSyns
             }
+            if 'categories' in self.terms[uri]:
+                entry['categories'] = self.terms[uri]['categories']
+            self.terms[uri] = entry
 
         for label in self.dupLabels:
             uris = self.dupLabels[label]
             toRemove = []
             for uri in uris:
                 syns = self.terms[uri]['syns']
                 if syns:
                     newSyns = syns.copy()
                     newLabel = syns[0]
                     newSyns.remove(newLabel)
-                    self.terms[uri] = {
+                    entry = {
                         'label': newLabel,
                         'syns': newSyns
                     }
+                    if 'categories' in self.terms[uri]:
+                        entry['categories'] = self.terms[uri]['categories']
+                    self.terms[uri] = entry
                 else:
                     toRemove.append(uri)
             for uri in toRemove:
                 self.terms.pop(uri)
 
     def getProcessedTerms(self):
         return self.terms
```

### Comparing `FastHPOCR-0.1.1/FastHPOCR/index/PreprocessHPOTerms.py` & `FastHPOCR-0.1.2/FastHPOCR/index/PreprocessORPHATerms.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-from FastHPOCR.index.HPOLabelCollector import HPOLabelCollector
 from FastHPOCR.index.LabelProcessor import LabelProcessor
+from FastHPOCR.index.ORPHALabelCollector import ORPHALabelCollector
 from FastHPOCR.util import ContentUtil
 from FastHPOCR.util.CRConstants import VB_BLACKLIST, POS_LIST
-from FastHPOCR.util.OntoReader import OntoReader
 
 
-class PreprocessHPOTerms:
+class PreprocessORPHATerms:
     processedTerms = {}
     terms = {}
 
-    def __init__(self, ontologyFile, rootConcepts=[], externalSynonyms={}, allow3LetterAcronyms=False):
-        ontoReader = OntoReader(ontologyFile)
+    def __init__(self, orphaDataFile, externalSynonyms={}, indexConfig={}):
         self.processedTerms = {}
 
-        labelProcessor = LabelProcessor(HPOLabelCollector(ontoReader,
-                                                          rootConcepts=rootConcepts,
-                                                          externalSynonyms=externalSynonyms,
-                                                          allow3LetterAcronyms=allow3LetterAcronyms).getTerms(),
-                                        allow3LetterAcronyms=allow3LetterAcronyms)
+        labelProcessor = LabelProcessor(ORPHALabelCollector(orphaDataFile,
+                                                            externalSynonyms=externalSynonyms,
+                                                            indexConfig=indexConfig).getTerms(),
+                                        indexConfig=indexConfig)
         self.terms = labelProcessor.getProcessedTerms()
 
         self.filterTerms()
 
     def filterTerms(self):
         for uri in self.terms:
             label = self.terms[uri]['label']
```

### Comparing `FastHPOCR-0.1.1/FastHPOCR/index/PreprocessORPHATerms.py` & `FastHPOCR-0.1.2/FastHPOCR/index/PreprocessSNOMEDTerms.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 from FastHPOCR.index.LabelProcessor import LabelProcessor
-from FastHPOCR.index.ORPHALabelCollector import ORPHALabelCollector
+from FastHPOCR.index.SNOMEDLabelCollector import SNOMEDLabelCollector
 from FastHPOCR.util import ContentUtil
 from FastHPOCR.util.CRConstants import VB_BLACKLIST, POS_LIST
 
 
-class PreprocessORPHATerms:
+class PreprocessSNOMEDTerms:
     processedTerms = {}
-    terms = {}
 
-    def __init__(self, orphaDataFile):
+    def __init__(self, jsonData, externalSynonyms={}, indexConfig={}):
         self.processedTerms = {}
-
-        labelProcessor = LabelProcessor(ORPHALabelCollector(orphaDataFile).getTerms())
+        labelProcessor = LabelProcessor(SNOMEDLabelCollector(jsonData,
+                                                             externalSynonyms=externalSynonyms,
+                                                             indexConfig=indexConfig).getTerms(),
+                                        indexConfig=indexConfig)
         self.terms = labelProcessor.getProcessedTerms()
 
         self.filterTerms()
 
     def filterTerms(self):
         for uri in self.terms:
             label = self.terms[uri]['label']
             syns = self.terms[uri]['syns']
+            categories = []
+            if 'categories' in self.terms[uri]:
+                categories = self.terms[uri]['categories']
+
             termLst = []
 
             tokenSet = self.processTerm(self.processLabel(label))
             filteredTokenSet = self.filter(tokenSet)
             termLst.append({
                 'originalLabel': label,
                 'preferredLabel': True,
@@ -34,15 +39,21 @@
                 tokenSet = self.processTerm(self.processLabel(syn))
                 filteredTokenSet = self.filter(tokenSet)
                 termLst.append({
                     'originalLabel': syn,
                     'preferredLabel': False,
                     'tokens': filteredTokenSet
                 })
-            self.processedTerms[uri] = termLst
+
+            entry = {
+                'terms': termLst
+            }
+            if categories:
+                entry['categories'] = categories
+            self.processedTerms[uri] = entry
 
     def processLabel(self, label) -> str:
         label = label.lower()
         label = ContentUtil.spaceReplace(label)
         label = ContentUtil.cleanToken(label)
         label = label.replace('  ', ' ')
         return label.strip()
```

### Comparing `FastHPOCR-0.1.1/FastHPOCR/index/PreprocessSNOMEDTerms.py` & `FastHPOCR-0.1.2/FastHPOCR/index/PreprocessHPOTerms.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,40 @@
+from FastHPOCR.index.HPOLabelCollector import HPOLabelCollector
 from FastHPOCR.index.LabelProcessor import LabelProcessor
-from FastHPOCR.index.SNOMEDLabelCollector import SNOMEDLabelCollector
-from FastHPOCR.util import ContentUtil
+from FastHPOCR.util import ContentUtil, ConfigConstants
 from FastHPOCR.util.CRConstants import VB_BLACKLIST, POS_LIST
+from FastHPOCR.util.OntoReader import OntoReader
 
 
-class PreprocessSNOMEDTerms:
+class PreprocessHPOTerms:
     processedTerms = {}
+    terms = {}
+    catDictionary = {}
 
-    def __init__(self, jsonData):
+    def __init__(self, ontologyFile, externalSynonyms={}, indexConfig={}):
+        ontoReader = OntoReader(ontologyFile)
         self.processedTerms = {}
-        labelProcessor = LabelProcessor(SNOMEDLabelCollector(jsonData).getTerms())
+
+        labelProcessor = LabelProcessor(HPOLabelCollector(ontoReader,
+                                                          externalSynonyms=externalSynonyms,
+                                                          indexConfig=indexConfig).getTerms(),
+                                        indexConfig=indexConfig)
         self.terms = labelProcessor.getProcessedTerms()
 
         self.filterTerms()
+        self.buildCategoriesDictionary(indexConfig, ontoReader)
 
     def filterTerms(self):
         for uri in self.terms:
             label = self.terms[uri]['label']
             syns = self.terms[uri]['syns']
+            categories = []
+            if 'categories' in self.terms[uri]:
+                categories = self.terms[uri]['categories']
+
             termLst = []
 
             tokenSet = self.processTerm(self.processLabel(label))
             filteredTokenSet = self.filter(tokenSet)
             termLst.append({
                 'originalLabel': label,
                 'preferredLabel': True,
@@ -32,15 +45,20 @@
                 tokenSet = self.processTerm(self.processLabel(syn))
                 filteredTokenSet = self.filter(tokenSet)
                 termLst.append({
                     'originalLabel': syn,
                     'preferredLabel': False,
                     'tokens': filteredTokenSet
                 })
-            self.processedTerms[uri] = termLst
+            entry = {
+                'terms': termLst
+            }
+            if categories:
+                entry['categories'] = categories
+            self.processedTerms[uri] = entry
 
     def processLabel(self, label) -> str:
         label = label.lower()
         label = ContentUtil.spaceReplace(label)
         label = ContentUtil.cleanToken(label)
         label = label.replace('  ', ' ')
         return label.strip()
@@ -58,9 +76,21 @@
         result = []
         for token in tokenSet:
             if token['token'] in VB_BLACKLIST or token['token'] in POS_LIST:
                 continue
             result.append(token)
         return result
 
+    def buildCategoriesDictionary(self, indexConfig, ontoReader):
+        if not indexConfig:
+            return
+
+        if ConfigConstants.VAR_INCLUDE_CATEGORY in indexConfig:
+            if indexConfig[ConfigConstants.VAR_INCLUDE_CATEGORY]:
+                for uri in ontoReader.abn_classes:
+                    self.catDictionary[uri] = ontoReader.terms[uri]
+
     def getProcessedTerms(self):
         return self.processedTerms
+
+    def getCategoriesDictionary(self):
+        return self.catDictionary
```

### Comparing `FastHPOCR-0.1.1/FastHPOCR/index/SynonymExpader.py` & `FastHPOCR-0.1.2/FastHPOCR/index/SynonymExpader.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,19 @@
     synClusters = None
 
     def __init__(self, termsToIndex, voidTokens, synClusters):
         self.expandedTerms = {}
         self.synClusters = synClusters
 
         for uri in termsToIndex:
-            newLabelList = self.augment(termsToIndex[uri], voidTokens)
-            self.expand(uri, newLabelList)
+            newLabelList = self.augment(termsToIndex[uri]['labels'], voidTokens)
+            categories = []
+            if 'categories' in termsToIndex[uri]:
+                categories = termsToIndex[uri]['categories']
+            self.expand(uri, newLabelList, categories)
 
     def augment(self, labelList, voidTokens):
         newList = []
         for label in labelList:
             newList.append(label)
             clusterSet = label['tokenSet']
             for clusterId in clusterSet:
@@ -27,24 +30,29 @@
                         'tokens': clusterIdsCopy,
                         'tokenSet': clusterSet,
                         'native': False
                     })
 
         return newList
 
-    def expand(self, uri, labelList):
+    def expand(self, uri, labelList, categories):
         newLabelList = []
         for label in labelList:
             newLabelList.append(label)
             clusterSet = label['tokenSet']
             for clusterId in clusterSet:
                 if clusterId in self.synClusters:
                     newLabels = self.generate(label, clusterId, self.synClusters[clusterId])
                     newLabelList.extend(newLabels)
-        self.expandedTerms[uri] = newLabelList
+        entry = {
+            'labels': newLabelList
+        }
+        if categories:
+            entry['categories'] = categories
+        self.expandedTerms[uri] = entry
 
     def generate(self, label, clusterId, synClusterSet):
         labelSet = []
 
         for syn in synClusterSet:
             if syn == clusterId:
                 continue
```

### Comparing `FastHPOCR-0.1.1/FastHPOCR/license.txt` & `FastHPOCR-0.1.2/FastHPOCR/license.txt`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.1/FastHPOCR/resources/base-synonyms` & `FastHPOCR-0.1.2/FastHPOCR/resources/base-synonyms`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.1/FastHPOCR/resources/vocab.clusters.list` & `FastHPOCR-0.1.2/FastHPOCR/resources/vocab.clusters.list`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.1/FastHPOCR/util/AnnotationToken.py` & `FastHPOCR-0.1.2/FastHPOCR/util/AnnotationToken.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.1/FastHPOCR/util/CRConstants.py` & `FastHPOCR-0.1.2/FastHPOCR/util/CRConstants.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.1/FastHPOCR/util/ContentUtil.py` & `FastHPOCR-0.1.2/FastHPOCR/util/ContentUtil.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.1/FastHPOCR/util/OntoReader.py` & `FastHPOCR-0.1.2/FastHPOCR/util/OntoReader.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.1/FastHPOCR/util/SequenceData.py` & `FastHPOCR-0.1.2/FastHPOCR/util/SequenceData.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.1/FastHPOCR.egg-info/SOURCES.txt` & `FastHPOCR-0.1.2/FastHPOCR.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -29,11 +29,12 @@
 FastHPOCR/index/SynonymExpader.py
 FastHPOCR/index/__init__.py
 FastHPOCR/resources/base-synonyms
 FastHPOCR/resources/vocab.clusters.list
 FastHPOCR/util/AnnotationObject.py
 FastHPOCR/util/AnnotationToken.py
 FastHPOCR/util/CRConstants.py
+FastHPOCR/util/ConfigConstants.py
 FastHPOCR/util/ContentUtil.py
 FastHPOCR/util/OntoReader.py
 FastHPOCR/util/SequenceData.py
 FastHPOCR/util/__init__.py
```

