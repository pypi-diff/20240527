# Comparing `tmp/imaging_research-0.1.1.tar.gz` & `tmp/imaging_research-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imaging_research-0.1.1.tar", last modified: Wed May  1 17:08:24 2024, max compression
+gzip compressed data, was "imaging_research-0.1.2.tar", last modified: Mon May 27 13:52:39 2024, max compression
```

## Comparing `imaging_research-0.1.1.tar` & `imaging_research-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 fraser    (1000) fraser    (1000)        0 2024-05-01 17:08:24.213664 imaging_research-0.1.1/
--rw-rw-r--   0 fraser    (1000) fraser    (1000)    35149 2023-09-04 08:29:41.000000 imaging_research-0.1.1/LICENSE
--rw-r--r--   0 fraser    (1000) fraser    (1000)     5363 2024-05-01 17:08:24.213664 imaging_research-0.1.1/PKG-INFO
--rw-rw-r--   0 fraser    (1000) fraser    (1000)     4558 2024-04-30 14:45:48.000000 imaging_research-0.1.1/README.md
-drwxrwxr-x   0 fraser    (1000) fraser    (1000)        0 2024-05-01 17:08:24.213664 imaging_research-0.1.1/imaging_research.egg-info/
--rw-r--r--   0 fraser    (1000) fraser    (1000)     5363 2024-05-01 17:08:24.000000 imaging_research-0.1.1/imaging_research.egg-info/PKG-INFO
--rw-rw-r--   0 fraser    (1000) fraser    (1000)      454 2024-05-01 17:08:24.000000 imaging_research-0.1.1/imaging_research.egg-info/SOURCES.txt
--rw-rw-r--   0 fraser    (1000) fraser    (1000)        1 2024-05-01 17:08:24.000000 imaging_research-0.1.1/imaging_research.egg-info/dependency_links.txt
--rw-rw-r--   0 fraser    (1000) fraser    (1000)       63 2024-05-01 17:08:24.000000 imaging_research-0.1.1/imaging_research.egg-info/entry_points.txt
--rw-rw-r--   0 fraser    (1000) fraser    (1000)       31 2024-05-01 17:08:24.000000 imaging_research-0.1.1/imaging_research.egg-info/requires.txt
--rw-rw-r--   0 fraser    (1000) fraser    (1000)       11 2024-05-01 17:08:24.000000 imaging_research-0.1.1/imaging_research.egg-info/top_level.txt
-drwxrwxr-x   0 fraser    (1000) fraser    (1000)        0 2024-05-01 17:08:24.213664 imaging_research-0.1.1/miresearch/
--rw-rw-r--   0 fraser    (1000) fraser    (1000)        0 2023-09-04 08:29:41.000000 imaging_research-0.1.1/miresearch/__init__.py
--rw-rw-r--   0 fraser    (1000) fraser    (1000)     4002 2024-04-30 14:45:48.000000 imaging_research-0.1.1/miresearch/mi_config.py
--rw-rw-r--   0 fraser    (1000) fraser    (1000)    46035 2024-04-30 15:39:18.000000 imaging_research-0.1.1/miresearch/mi_subject.py
--rw-rw-r--   0 fraser    (1000) fraser    (1000)     7311 2024-04-02 11:54:17.000000 imaging_research-0.1.1/miresearch/mi_utils.py
--rw-rw-r--   0 fraser    (1000) fraser    (1000)      428 2024-04-30 14:45:48.000000 imaging_research-0.1.1/miresearch/miresearch.conf
--rw-rw-r--   0 fraser    (1000) fraser    (1000)     8504 2024-04-02 11:54:17.000000 imaging_research-0.1.1/miresearch/miresearch_main.py
--rw-rw-r--   0 fraser    (1000) fraser    (1000)    10833 2024-04-30 14:45:48.000000 imaging_research-0.1.1/miresearch/miresearch_watchdog.py
--rw-rw-r--   0 fraser    (1000) fraser    (1000)       38 2024-05-01 17:08:24.213664 imaging_research-0.1.1/setup.cfg
--rw-rw-r--   0 fraser    (1000) fraser    (1000)     3555 2024-05-01 17:06:00.000000 imaging_research-0.1.1/setup.py
+drwxrwxr-x   0 fraser    (1000) fraser    (1000)        0 2024-05-27 13:52:39.249580 imaging_research-0.1.2/
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)    35149 2023-07-21 12:13:15.000000 imaging_research-0.1.2/LICENSE
+-rw-r--r--   0 fraser    (1000) fraser    (1000)     5363 2024-05-27 13:52:39.249580 imaging_research-0.1.2/PKG-INFO
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)     4558 2024-04-24 15:41:49.000000 imaging_research-0.1.2/README.md
+drwxrwxr-x   0 fraser    (1000) fraser    (1000)        0 2024-05-27 13:52:39.249580 imaging_research-0.1.2/imaging_research.egg-info/
+-rw-r--r--   0 fraser    (1000) fraser    (1000)     5363 2024-05-27 13:52:39.000000 imaging_research-0.1.2/imaging_research.egg-info/PKG-INFO
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)      454 2024-05-27 13:52:39.000000 imaging_research-0.1.2/imaging_research.egg-info/SOURCES.txt
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)        1 2024-05-27 13:52:39.000000 imaging_research-0.1.2/imaging_research.egg-info/dependency_links.txt
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)       63 2024-05-27 13:52:39.000000 imaging_research-0.1.2/imaging_research.egg-info/entry_points.txt
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)       31 2024-05-27 13:52:39.000000 imaging_research-0.1.2/imaging_research.egg-info/requires.txt
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)       11 2024-05-27 13:52:39.000000 imaging_research-0.1.2/imaging_research.egg-info/top_level.txt
+drwxrwxr-x   0 fraser    (1000) fraser    (1000)        0 2024-05-27 13:52:39.249580 imaging_research-0.1.2/miresearch/
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)        0 2023-07-21 12:13:15.000000 imaging_research-0.1.2/miresearch/__init__.py
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)     4073 2024-05-21 19:12:21.000000 imaging_research-0.1.2/miresearch/mi_config.py
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)    47224 2024-05-27 13:47:16.000000 imaging_research-0.1.2/miresearch/mi_subject.py
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)     7316 2024-05-21 19:12:21.000000 imaging_research-0.1.2/miresearch/mi_utils.py
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)      428 2024-04-24 15:29:19.000000 imaging_research-0.1.2/miresearch/miresearch.conf
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)     8731 2024-05-21 19:15:04.000000 imaging_research-0.1.2/miresearch/miresearch_main.py
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)    10833 2024-04-24 15:33:57.000000 imaging_research-0.1.2/miresearch/miresearch_watchdog.py
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)       38 2024-05-27 13:52:39.249580 imaging_research-0.1.2/setup.cfg
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)     3555 2024-05-21 19:12:21.000000 imaging_research-0.1.2/setup.py
```

### Comparing `imaging_research-0.1.1/LICENSE` & `imaging_research-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `imaging_research-0.1.1/PKG-INFO` & `imaging_research-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imaging-research
-Version: 0.1.1
+Version: 0.1.2
 Summary: Medical Imaginging Research structuring and automation
 Home-page: https://github.com/fraser29/miresearch
 Author: Fraser M. Callaghan
 Author-email: callaghan.fm@gmail.com
 License: MIT
 Keywords: medical,imaging,mri,ct,dicom
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `imaging_research-0.1.1/README.md` & `imaging_research-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `imaging_research-0.1.1/imaging_research.egg-info/PKG-INFO` & `imaging_research-0.1.2/imaging_research.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imaging-research
-Version: 0.1.1
+Version: 0.1.2
 Summary: Medical Imaginging Research structuring and automation
 Home-page: https://github.com/fraser29/miresearch
 Author: Fraser M. Callaghan
 Author-email: callaghan.fm@gmail.com
 License: MIT
 Keywords: medical,imaging,mri,ct,dicom
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `imaging_research-0.1.1/miresearch/mi_config.py` & `imaging_research-0.1.2/miresearch/mi_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,32 +36,33 @@
         self._anon_level = self.config.get("app", "anon_level", fallback='NONE')
         self._data_root_dir = self.config.get("app", "data_root_dir", fallback="")
         self._subject_prefix = self.config.get("app", "subject_prefix", fallback="")
         self.stable_directory_age_sec = self.config.getint("app", "stable_directory_age_sec", fallback=60)
         self.default_pad_zeros = self.config.getint("app", "default_pad_zeros", fallback=6)
         self.directory_structure = json.loads(self.config.get("app", "directories"))
 
+        ## All parameters: 
+        self.params = {}
+        for section in self.config.sections():
+            if section.lower() == 'parameters':
+                self.params[section] = {}
+                for option in self.config.options(section):
+                    self.params[section][option] = self.config.get(section, option)
+
+        # Class objects - want to do last so have access to parameters
         self.class_obj = None
         class_path = self.config.get("app", "class_path", fallback=None)
         if class_path:
             module_name, class_name = class_path.rsplit('.', 1)
             try:
                 module = importlib.import_module(module_name)
             except ModuleNotFoundError as e:
                 raise ModuleNotFoundError(f"*** is {module_name} found in PYTHONPATH? ***") from e
             self.class_obj = getattr(module, class_name)
 
-        ## All parameters: 
-        self.params = {}
-        for section in self.config.sections():
-            if section.lower() == 'parameters':
-                self.params[section] = {}
-                for option in self.config.options(section):
-                    self.params[section][option] = self.config.get(section, option)
-
     @property
     def data_root_dir(self):
         """Function to return data root from configuration. 
 
         Returns:
             str: Path to data root - found from config
         """
```

### Comparing `imaging_research-0.1.1/miresearch/mi_subject.py` & `imaging_research-0.1.2/miresearch/mi_subject.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,44 +158,35 @@
             for j in i.childrenList:
                 os.makedirs(os.path.join(self.getTopDir(), i.name, j), exist_ok=True)
         self.logger.info(f"Directory structure correct for {self.subjID} at {self.getTopDir()}.")
 
     def getPrefix_Number(self):
         return splitSubjID(self.subjID)
 
-    ### LOADING
-    def _checkAnonName(self, anonName, name="", firstNames=""):
-        if anonName == "SOFT":
-            self.setEncodedName(NAME=name, FIRST_NAMES=firstNames)
-            return ""
-        elif anonName == "HARD":
-            return ""
-        return anonName
-
+    ### LOADING -------------------------------------------------------------------------------------------------------
     def loadDicomsToSubject(self, dicomFolderToLoad, anonName=None, HIDE_PROGRESSBAR=False):
         self.initDirectoryStructure()
-        patName = str(spydcm.getTag(dicomFolderToLoad, "PatientName")[0])
-        anonName = self._checkAnonName(anonName, patName.split("^")[0], "_".join(patName.split("^")[1:]))
         self.logger.info(f"LoadDicoms to {self.getDicomsDir()}") # Don't log source here as could be identifying
-        # self.logger.info(f"LoadDicoms ({dicomFolderToLoad} ==> {self.getDicomsDir()})")
+        self.logger.info(f"LoadDicoms ({dicomFolderToLoad} ==> {self.getDicomsDir()}) & anon={anonName}") # FIXME - debug only
         d0, dI = self.countNumberOfDicoms(), mi_utils.countFilesInDir(dicomFolderToLoad)
         study = spydcm.dcmTK.DicomStudy.setFromDirectory(dicomFolderToLoad, HIDE_PROGRESSBAR=HIDE_PROGRESSBAR)
-        res = study.writeToOrganisedFileStructure(self.getDicomsDir(), anonName=anonName)
-        self._finalLoadSteps(d0, dI)
+        res = study.writeToOrganisedFileStructure(self.getDicomsDir())
+        self._finalLoadSteps(d0, dI, anonName)
 
-    def loadSpydcmStudyToSubject(self, spydcmData, anonName=None, HIDE_PROGRESSBAR=False):
+    def loadSpydcmStudyToSubject(self, spydcmData, anonName=None):
         self.initDirectoryStructure()
-        patName = spydcmData.getTag("PatientName")
-        self._checkAnonName(anonName, patName.split("^")[0], "_".join(patName.split("^")[1:]))
         self.logger.info(f"LoadDicoms (spydcmtk data ==> {self.getDicomsDir()})")
         d0, dI = self.countNumberOfDicoms(), spydcmData.getNumberOfDicoms()
-        spydcmData.writeToOrganisedFileStructure(self.getDicomsDir(), anonName=anonName)
-        self._finalLoadSteps(d0, dI)
+        spydcmData.writeToOrganisedFileStructure(self.getDicomsDir())
+        self._finalLoadSteps(d0, dI, anonName=anonName)
     
-    def _finalLoadSteps(self, initNumDicoms, numDicomsToLoad):
+    def _finalLoadSteps(self, initNumDicoms, numDicomsToLoad, anonName=None):
+        self.buildDicomMeta()
+        if anonName is not None:
+            self.anonymise(anonName=anonName)
         finalNumDicoms = self.countNumberOfDicoms()
         self.logger.info(f"Initial number of dicoms: {initNumDicoms}, number to load: {numDicomsToLoad}, final number dicoms: {finalNumDicoms}")
         self.buildDicomMeta()
         self.buildSeriesDataMetaCSV(FORCE=True)
         self.runPostLoadPipeLine()
 
     def runPostLoadPipeLine(self, *args, **kwargs):
@@ -418,20 +409,23 @@
         dd = self.getMetaDict(metasuffix)
         dd.update(metaDict)
         spydcm.dcmTools.writeDictionaryToJSON(self.getMetaTagsFile(metasuffix), dd)
         self.logger.info('updateMetaFile')
 
     def buildDicomMeta(self):
         # this uses pydicom - so tag names are different.
+        ddFull = {'SubjectID': self.subjID, 'SubjN': self._subjN}
         dcmStudies = spydcm.dcmTK.ListOfDicomStudies.setFromDirectory(self.getDicomsDir(), HIDE_PROGRESSBAR=True)
-        ddFull = dcmStudies[0].getStudySummaryDict()
-        ddFull['SubjectID'] = self.subjID
-        ddFull['SubjN'] = self._subjN
-        for k1 in range(1, len(dcmStudies)):
-            ddFull['Series'] += dcmStudies[k1].getStudySummaryDict()['Series']
+        try:
+            dcmDict = dcmStudies[0].getStudySummaryDict()
+            ddFull.update(dcmDict)
+            for k1 in range(1, len(dcmStudies)):
+                ddFull['Series'] += dcmStudies[k1].getStudySummaryDict()['Series']
+        except IndexError:
+            pass # Found no Dicoms
         self.updateMetaFile(ddFull)
 
     def countNumberOfDicoms(self):
         return mi_utils.countFilesInDir(self.getDicomsDir())
     
     def getDicomSeriesDir_Description(self, seriesDescription):
         dd = self.getSeriesNumbersMatchingDescriptionStr(seriesDescription)
@@ -527,59 +521,73 @@
                     'StudyDate', 'StudyDescription', 'StudyInstanceUID', 'StudyID'] + extraKeys
         mm = self.getMetaDict()
         aa = '%5.2f'%(self.getAge())
         return [mm.get(i, "Unknown") for i in infoKeys]+[aa], infoKeys + ['Age']
 
     # ------------------------------------------------------------------------------------------
     def anonymise(self, anonName=None):
+        self.logger.info(f'Anonymise in place to {anonName}')
+        name, firstNames = self.getName_FirstNames()
+        anonName = self._checkAnonName(anonName, name, firstNames)
+        # anonName = self._checkAnonName(anonName, patName.split("^")[0], "_".join(patName.split("^")[1:]))
         if type(anonName) == str:
             if len(anonName) == 0:  
                 anonName = None # Still anonymise, but let program choose the new anonName
         self.logger.info('Anonymise in place')
         spydcm.anonymiseInPlace(self.getDicomsDir(), anonName=anonName)
         self.setIsAnonymised()
         self.buildDicomMeta()
 
+    def _checkAnonName(self, anonName, name="", firstNames=""):
+        self.logger.info(f'_checkAnonName args: {anonName}, name={name}, firstnames={firstNames}') # FIXME debug
+        if anonName == "SOFT":
+            self.setEncodedName(NAME=name, FIRST_NAMES=firstNames)
+            return ""
+        elif anonName == "HARD":
+            self.setEncodedName(NAME='Name-Unknown', FIRST_NAMES='FirstNames-Unknown')
+            return ""
+        return anonName
+    
     def setIsAnonymised(self):
         self.updateMetaFile({"ANONYMISED": True})
     
     def isAnonymised(self):
         return self.getTagValue("ANONYMISED", False)
 
     def setEncodedName(self, NAME, FIRST_NAMES=""):
-        """
-        funct to add name after (will encode)
-        :param NAME:
-        :param FIRST_NAMES:
-        :return:
-        """
+        self.logger.info(f"Adding encoded name {NAME} & {FIRST_NAMES} -- {mi_utils.encodeString('Name-Unknown', self.subjID)}") # FIXME THIS IS DEBUG - REMOVE ME
         dd = {'NAME': mi_utils.encodeString(NAME, self.subjID),
               'FIRST_NAMES': mi_utils.encodeString(FIRST_NAMES, self.subjID)}
         self.updateMetaFile(dd)
 
     def getName(self):
         if self.isAnonymised():
             try:
-                return mi_utils.decodeString(self.getTagValue("NAME", "UNKNOWN"), self.subjID)
+                return mi_utils.decodeString(self.getTagValue("NAME", None), self.subjID)
             except:
                 return self.getTagValue('PatientName', 'Name-Unknown')
         else:
             return self.getTagValue('PatientName', 'Name-Unknown')
 
     def getName_FirstNames(self):
         if self.isAnonymised():
-            return mi_utils.decodeString(self.getTagValue("NAME", "UNKNOWN"), self.subjID), \
-                mi_utils.decodeString(self.getTagValue("FIRST_NAMES", "UNKNOWN"), self.subjID)
-        else:
-            name = self.getName()
-            name = name.replace(" ","_")
-            name = name.replace("^","_")
-            while "__" in name:
-                name = name.replace("__","_")
-            return name
+            try:
+                return mi_utils.decodeString(self.getTagValue("NAME", None), self.subjID), \
+                    mi_utils.decodeString(self.getTagValue("FIRST_NAMES", None), self.subjID)
+            except TypeError:
+                pass
+            
+        name = self.getName()
+        self.logger.info(f"got name {name}") # FIXME THIS IS DEBUG - REMOVE ME
+        parts = name.split("^")
+        if len(parts) == 1:
+            return parts[0], ""
+        name = parts[0]
+        firstNames = "_".join(parts[1:])
+        return spydcm.dcmTools.cleanString(name), spydcm.dcmTools.cleanString(firstNames)
 
 
     # ------------------------------------------------------------------------------------------
     def getSummary_list(self):
         hh = ["SubjectID","PatientID","Gender","StudyDate","NumberOfSeries","SERIES_DECRIPTIONS"]
         parts = [self.subjID, self.getMetaTagValue('PatientID'), 
                 self.getMetaTagValue('PatientSex'), self.getMetaTagValue('StudyDate'), 
@@ -781,14 +789,15 @@
 ### ====================================================================================================================
 ###  Helper functions for subject list
 ### ====================================================================================================================
 def getAllSubjects(dataRootDir, subjectPrefix=None, SubjClass=AbstractSubject):
     if subjectPrefix is None:
         subjectPrefix = guessSubjectPrefix(dataRootDir)
     allDir = os.listdir(dataRootDir)
+    allDir = [i for i in allDir if i.startswith(subjectPrefix)]
     allDir = [i for i in allDir if os.path.isdir(os.path.join(dataRootDir, i))]
     subjObjList = []
     for i in allDir:
         try:
             subjObjList.append(SubjClass(i, dataRoot=dataRootDir))
         except ValueError:
             print(f"WARNING: {i} at {dataRootDir} not valid subject")
@@ -870,15 +879,15 @@
     allDir = [i for i in os.listdir(dataRootDir) if os.path.isdir(os.path.join(dataRootDir, i))]
     allDir_subj = {}
     for i in allDir:
         try:
             prefix_N_suffix = splitSubjID(i)
             prefix = prefix_N_suffix[0]
             N = prefix_N_suffix[1]
-        except ValueError: 
+        except (ValueError, IndexError): 
             continue # directory not correct format - could not split to integer
         allDir_subj.setdefault(prefix, []).append(N)
     options = list(allDir_subj.keys())
     if len(options) == 0:
         raise mi_utils.SubjPrefixError("Error guessing subject prefix - ambiguous - please provide")
     counts = [len(allDir_subj[i]) for i in options]
     maxCount = np.argmax(counts)
@@ -913,24 +922,30 @@
         subjectPrefix = guessSubjectPrefix(dataRootDir)
     return buildSubjectID(getNextSubjN(dataRootDir, subjectPrefix), subjectPrefix)
 
 def _createSubjectHelper(dicomDir_orData, SubjClass, subjNumber, dataRoot, subjPrefix, anonName, QUIET, FORCE_NEW_SUBJ=False):
     if FORCE_NEW_SUBJ:
         newSubj = None
     else:
+        # Check if a subject already exists with dicom data matching input
         newSubj = findSubjMatchingDicomStudyUID(dicomDir_orData, dataRoot, subjPrefix)
     if newSubj is not None:
+        # Subject exists - so check nothing conflicting from inputs
         if subjNumber is not None:
             if subjNumber != newSubj.subjN:
                 raise ValueError(f"You supplied subject number {subjNumber} but a different subject matching your input dicom study exists at {newSubj.subjN}")
         print(f"Found existing subject {newSubj.subjID} at {dataRoot} - adding to")
+    
+    # If no subject exists matching the inputs - define a new subject (increment subjN from current in root directory)
     if newSubj is None: 
         subjNumber = _subjNumberHelper(dataRoot=dataRoot, subjNumber=subjNumber, subjPrefix=subjPrefix)
         newSubj = SubjClass(subjNumber, dataRoot, subjectPrefix=subjPrefix)
     newSubj.QUIET = QUIET
+
+    # Now have a subject - either newly created or existing and matching dicom data - load dicoms to subject:
     try:
         os.path.isdir(dicomDir_orData)
         newSubj.loadDicomsToSubject(dicomDir_orData, anonName=anonName, HIDE_PROGRESSBAR=QUIET)
     except TypeError:
         newSubj.loadSpydcmStudyToSubject(dicomDir_orData, anonName=anonName)
     #
     return newSubj
```

### Comparing `imaging_research-0.1.1/miresearch/mi_utils.py` & `imaging_research-0.1.2/miresearch/mi_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         enc_c = chr((ord(strIn[i]) + ord(key_c)) % 256)
         enc.append(enc_c)
     return base64.urlsafe_b64encode("".join(enc).encode()).decode()
 
 
 def decodeString(encStr, passcode):
     dec = []
-    enc = base64.urlsafe_b64decode(encStr).decode()
+    enc = base64.urlsafe_b64decode(encStr+'==').decode()
     for i in range(len(enc)):
         key_c = passcode[i % len(passcode)]
         dec_c = chr((256 + ord(enc[i]) - ord(key_c)) % 256)
         dec.append(dec_c)
     return "".join(dec)
```

### Comparing `imaging_research-0.1.1/miresearch/miresearch_main.py` & `imaging_research-0.1.2/miresearch/miresearch_main.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,14 +42,17 @@
 groupS.add_argument('-sR', dest='subjRange', help='Subject range', nargs=2, type=int, default=[])
 groupS.add_argument('-y', dest='dataRoot', 
                     help='Path of root data directory (where subjects are stored) [default None -> may be set in config file]', 
                     type=str, default=None)
 groupS.add_argument('-sPrefix', dest='subjPrefix', 
                     help='Subject prefix [default None -> will get from config file OR dataRoot]', 
                     type=str, default=None)
+groupS.add_argument('-sSuffix', dest='subjSuffix', 
+                    help='Subject suffix [default None]', 
+                    type=str, default=None)
 groupS.add_argument('-anonName', dest='anonName', 
                     help='Set to anonymise newly loaded subject. Set to true to use for WatchDirectory. [default None]', 
                     type=str, default=None)
     
 groupA = ParentAP.add_argument_group('Actions')
 # LOADING
 groupA.add_argument('-Load', dest='loadPath', 
@@ -134,29 +137,29 @@
                                              IGNORE_UIDS=args.LoadMultiForce,
                                              QUIET=args.QUIET)
     # SUBJECT LEVEL actions
     elif len(args.subjNList) > 0:
         # --- ANONYMISE ---
         if args.anonName is not None:
             for sn in args.subjNList:
-                iSubj = args.MISubjClass(sn, args.dataRoot, args.subjPrefix)
+                iSubj = args.MISubjClass(sn, args.dataRoot, args.subjPrefix, suffix=args.subjSuffix)
                 if iSubj.exists():
                     iSubj.anonymise(args.anonName)
 
         # --- POST LOAD PIPELINE ---
         elif args.subjRunPost:
             for sn in args.subjNList:
-                iSubj = args.MISubjClass(sn, args.dataRoot, args.subjPrefix)
+                iSubj = args.MISubjClass(sn, args.dataRoot, args.subjPrefix, suffix=args.subjSuffix)
                 if iSubj.exists():
                     iSubj.runPostLoadPipeLine()
 
         # --- PRINT INFO ---
         elif args.subjInfo:
             for sn in args.subjNList:
-                iSubj = args.MISubjClass(sn, args.dataRoot, args.subjPrefix)
+                iSubj = args.MISubjClass(sn, args.dataRoot, args.subjPrefix, suffix=args.subjSuffix)
                 if iSubj.exists():
                     iSubj.info()
 
     # SUBJECT GROUP (based on dataRoot) ACTIONS
     elif args.SummaryCSV is not None:
         mi_subject.WriteSubjectStudySummary(args.dataRoot, args.SummaryCSV)
```

### Comparing `imaging_research-0.1.1/miresearch/miresearch_watchdog.py` & `imaging_research-0.1.2/miresearch/miresearch_watchdog.py`

 * *Files identical despite different names*

### Comparing `imaging_research-0.1.1/setup.py` & `imaging_research-0.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'imaging-research'
 DESCRIPTION = 'Medical Imaginging Research structuring and automation'
 URL = 'https://github.com/fraser29/miresearch'
 EMAIL = 'callaghan.fm@gmail.com'
 AUTHOR = 'Fraser M. Callaghan'
 REQUIRES_PYTHON = '>=3.9.0'
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 KEYWORDS="medical, imaging, mri, ct, dicom"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "spydcmtk", "pandas", "numpy", "watchdog"
 ]
```

