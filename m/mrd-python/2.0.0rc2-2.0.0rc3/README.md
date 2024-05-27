# Comparing `tmp/mrd_python-2.0.0rc2.tar.gz` & `tmp/mrd_python-2.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrd_python-2.0.0rc2.tar", last modified: Wed May 22 18:12:30 2024, max compression
+gzip compressed data, was "mrd_python-2.0.0rc3.tar", last modified: Mon May 27 15:59:49 2024, max compression
```

## Comparing `mrd_python-2.0.0rc2.tar` & `mrd_python-2.0.0rc3.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-22 18:12:30.363811 mrd_python-2.0.0rc2/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      828 2024-05-22 18:12:30.363811 mrd_python-2.0.0rc2/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)       76 2024-05-22 18:06:12.000000 mrd_python-2.0.0rc2/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-22 18:12:30.353811 mrd_python-2.0.0rc2/mrd/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2275 2024-04-22 16:37:24.000000 mrd_python-2.0.0rc2/mrd/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    46614 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc2/mrd/_binary.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3390 2024-04-22 16:37:24.000000 mrd_python-2.0.0rc2/mrd/_dtypes.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    39791 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc2/mrd/_ndjson.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    53801 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc2/mrd/binary.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)   169451 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc2/mrd/ndjson.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    23566 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc2/mrd/protocols.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-22 18:12:30.353811 mrd_python-2.0.0rc2/mrd/tools/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1372 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc2/mrd/tools/export_png_images.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5866 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc2/mrd/tools/phantom.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6220 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc2/mrd/tools/simulation.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8396 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc2/mrd/tools/stream_recon.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1337 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc2/mrd/tools/transform.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    93782 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc2/mrd/types.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9563 2024-04-22 16:37:24.000000 mrd_python-2.0.0rc2/mrd/yardl_types.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-22 18:12:30.363811 mrd_python-2.0.0rc2/mrd_python.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      828 2024-05-22 18:12:30.000000 mrd_python-2.0.0rc2/mrd_python.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      465 2024-05-22 18:12:30.000000 mrd_python-2.0.0rc2/mrd_python.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-05-22 18:12:30.000000 mrd_python-2.0.0rc2/mrd_python.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2024-05-22 18:12:30.000000 mrd_python-2.0.0rc2/mrd_python.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        4 2024-05-22 18:12:30.000000 mrd_python-2.0.0rc2/mrd_python.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      849 2024-05-22 18:07:54.000000 mrd_python-2.0.0rc2/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2024-05-22 18:12:30.363811 mrd_python-2.0.0rc2/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)      157 2024-05-21 17:46:22.000000 mrd_python-2.0.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:59:49.455181 mrd_python-2.0.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-27 15:59:49.455181 mrd_python-2.0.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:59:49.451182 mrd_python-2.0.0rc3/mrd/
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/mrd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46614 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/mrd/_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/mrd/_dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39791 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/mrd/_ndjson.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53801 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/mrd/binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)   169451 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/mrd/ndjson.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23566 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/mrd/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:59:49.451182 mrd_python-2.0.0rc3/mrd/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/mrd/tools/export_png_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/mrd/tools/minimal_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/mrd/tools/phantom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/mrd/tools/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8396 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/mrd/tools/stream_recon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/mrd/tools/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    97266 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/mrd/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9563 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/mrd/yardl_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:59:49.455181 mrd_python-2.0.0rc3/mrd_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-27 15:59:49.000000 mrd_python-2.0.0rc3/mrd_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-27 15:59:49.000000 mrd_python-2.0.0rc3/mrd_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 15:59:49.000000 mrd_python-2.0.0rc3/mrd_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-27 15:59:49.000000 mrd_python-2.0.0rc3/mrd_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-27 15:59:49.000000 mrd_python-2.0.0rc3/mrd_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 15:59:49.455181 mrd_python-2.0.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/setup.py
```

### Comparing `mrd_python-2.0.0rc2/PKG-INFO` & `mrd_python-2.0.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrd-python
-Version: 2.0.0rc2
+Version: 2.0.0rc3
 Summary: Library and tools for working with data in the ISMRM Raw Data (MRD) format.
 Project-URL: Homepage, https://ismrmrd.github.io/mrd
 Project-URL: Documentation, https://ismrmrd.github.io/mrd
 Project-URL: Repository, https://github.com/ismrmrd/mrd
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mrd_python-2.0.0rc2/mrd/__init__.py` & `mrd_python-2.0.0rc3/mrd/__init__.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc2/mrd/_binary.py` & `mrd_python-2.0.0rc3/mrd/_binary.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc2/mrd/_dtypes.py` & `mrd_python-2.0.0rc3/mrd/_dtypes.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc2/mrd/_ndjson.py` & `mrd_python-2.0.0rc3/mrd/_ndjson.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc2/mrd/binary.py` & `mrd_python-2.0.0rc3/mrd/binary.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc2/mrd/ndjson.py` & `mrd_python-2.0.0rc3/mrd/ndjson.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc2/mrd/protocols.py` & `mrd_python-2.0.0rc3/mrd/protocols.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc2/mrd/tools/export_png_images.py` & `mrd_python-2.0.0rc3/mrd/tools/export_png_images.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc2/mrd/tools/phantom.py` & `mrd_python-2.0.0rc3/mrd/tools/phantom.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc2/mrd/tools/simulation.py` & `mrd_python-2.0.0rc3/mrd/tools/simulation.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc2/mrd/tools/stream_recon.py` & `mrd_python-2.0.0rc3/mrd/tools/stream_recon.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc2/mrd/tools/transform.py` & `mrd_python-2.0.0rc3/mrd/tools/transform.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc2/mrd/types.py` & `mrd_python-2.0.0rc3/mrd/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,23 +62,43 @@
     def __hash__(self) -> int:
         return hash(self.value)
 
     __str__ = enum.Flag.__str__ # type: ignore
 
 class EncodingCounters:
     kspace_encode_step_1: typing.Optional[yardl.UInt32]
+    """Phase encoding line"""
+
     kspace_encode_step_2: typing.Optional[yardl.UInt32]
+    """Partition encoding"""
+
     average: typing.Optional[yardl.UInt32]
+    """Signal average"""
+
     slice: typing.Optional[yardl.UInt32]
+    """Slice number (multi-slice 2D)"""
+
     contrast: typing.Optional[yardl.UInt32]
+    """Echo number in multi-echo"""
+
     phase: typing.Optional[yardl.UInt32]
+    """Cardiac phase"""
+
     repetition: typing.Optional[yardl.UInt32]
+    """Counter in repeated/dynamic acquisitions"""
+
     set: typing.Optional[yardl.UInt32]
+    """Sets of different preparation, e.g. flow encoding, diffusion weighting"""
+
     segment: typing.Optional[yardl.UInt32]
+    """Counter for segmented acquisitions"""
+
     user: list[yardl.UInt32]
+    """User-defined counters"""
+
 
     def __init__(self, *,
         kspace_encode_step_1: typing.Optional[yardl.UInt32] = None,
         kspace_encode_step_2: typing.Optional[yardl.UInt32] = None,
         average: typing.Optional[yardl.UInt32] = None,
         slice: typing.Optional[yardl.UInt32] = None,
         contrast: typing.Optional[yardl.UInt32] = None,
@@ -123,34 +143,80 @@
 
 AcquisitionData = npt.NDArray[np.complex64]
 
 TrajectoryData = npt.NDArray[np.float32]
 
 class Acquisition:
     flags: AcquisitionFlags
+    """A bit mask of common attributes applicable to individual acquisition"""
+
     idx: EncodingCounters
+    """Encoding loop counters"""
+
     measurement_uid: yardl.UInt32
+    """Unique ID corresponding to the readout"""
+
     scan_counter: typing.Optional[yardl.UInt32]
+    """Zero-indexed incrementing counter for readouts"""
+
     acquisition_time_stamp: typing.Optional[yardl.UInt32]
+    """Clock time stamp (e.g. milliseconds since midnight)"""
+
     physiology_time_stamp: list[yardl.UInt32]
+    """Time stamps relative to physiological triggering"""
+
     channel_order: list[yardl.UInt32]
+    """Channel numbers"""
+
     discard_pre: typing.Optional[yardl.UInt32]
+    """Number of readout samples to be discarded at the beginning
+      (e.g. if the ADC is active during gradient events)
+    """
+
     discard_post: typing.Optional[yardl.UInt32]
+    """Number of readout samples to be discarded at the end
+      (e.g. if the ADC is active during gradient events)
+    """
+
     center_sample: typing.Optional[yardl.UInt32]
+    """Index of the readout sample corresponing to k-space center (zero indexed)"""
+
     encoding_space_ref: typing.Optional[yardl.UInt32]
+    """Indexed reference to the encoding spaces enumerated in the MRD Header"""
+
     sample_time_us: typing.Optional[yardl.Float32]
+    """Readout bandwidth, as time between samples in microseconds"""
+
     position: npt.NDArray[np.float32]
+    """Center of the excited volume, in LPS coordinates relative to isocenter in millimeters"""
+
     read_dir: npt.NDArray[np.float32]
+    """Directional cosine of readout/frequency encoding"""
+
     phase_dir: npt.NDArray[np.float32]
+    """Directional cosine of phase encoding (2D)"""
+
     slice_dir: npt.NDArray[np.float32]
+    """Directional cosine of slice normal, i.e. cross-product of read_dir and phase_dir"""
+
     patient_table_position: npt.NDArray[np.float32]
+    """Offset position of the patient table, in LPS coordinates"""
+
     user_int: list[yardl.Int32]
+    """User-defined integer parameters"""
+
     user_float: list[yardl.Float32]
+    """User-defined float parameters"""
+
     data: AcquisitionData
+    """Raw k-space samples array"""
+
     trajectory: TrajectoryData
+    """Trajectory array"""
+
 
     def __init__(self, *,
         flags: AcquisitionFlags = AcquisitionFlags(0),
         idx: typing.Optional[EncodingCounters] = None,
         measurement_uid: yardl.UInt32 = 0,
         scan_counter: typing.Optional[yardl.UInt32] = None,
         acquisition_time_stamp: typing.Optional[yardl.UInt32] = None,
@@ -1424,36 +1490,82 @@
 
     def __repr__(self) -> str:
         return f"ImageMetaData(name={repr(self.name)}, value={repr(self.value)})"
 
 
 class Image(typing.Generic[T_NP]):
     flags: ImageFlags
+    """A bit mask of common attributes applicable to individual images"""
+
     measurement_uid: yardl.UInt32
+    """Unique ID corresponding to the image"""
+
     field_of_view: npt.NDArray[np.float32]
+    """Physical size (in mm) in each of the 3 dimensions in the image"""
+
     position: npt.NDArray[np.float32]
+    """Center of the excited volume, in LPS coordinates relative to isocenter in millimeters"""
+
     col_dir: npt.NDArray[np.float32]
+    """Directional cosine of readout/frequency encoding"""
+
     line_dir: npt.NDArray[np.float32]
+    """Directional cosine of phase encoding (2D)"""
+
     slice_dir: npt.NDArray[np.float32]
+    """Directional cosine of 3D phase encoding direction"""
+
     patient_table_position: npt.NDArray[np.float32]
+    """Offset position of the patient table, in LPS coordinates"""
+
     average: typing.Optional[yardl.UInt32]
+    """Signal average"""
+
     slice: typing.Optional[yardl.UInt32]
+    """Slice number (multi-slice 2D)"""
+
     contrast: typing.Optional[yardl.UInt32]
+    """Echo number in multi-echo"""
+
     phase: typing.Optional[yardl.UInt32]
+    """Cardiac phase"""
+
     repetition: typing.Optional[yardl.UInt32]
+    """Counter in repeated/dynamic acquisitions"""
+
     set: typing.Optional[yardl.UInt32]
+    """Sets of different preparation, e.g. flow encoding, diffusion weighting"""
+
     acquisition_time_stamp: typing.Optional[yardl.UInt32]
+    """Clock time stamp (e.g. milliseconds since midnight)"""
+
     physiology_time_stamp: list[yardl.UInt32]
+    """Time stamps relative to physiological triggering, e.g. ECG, pulse oximetry, respiratory"""
+
     image_type: ImageType
+    """Interpretation type of the image"""
+
     image_index: typing.Optional[yardl.UInt32]
+    """Image index number within a series of images, corresponding to DICOM InstanceNumber (0020,0013)"""
+
     image_series_index: typing.Optional[yardl.UInt32]
+    """Series index, used to separate images into different series, corresponding to DICOM SeriesNumber (0020,0011)"""
+
     user_int: list[yardl.Int32]
+    """User-defined int parameters"""
+
     user_float: list[yardl.Float32]
+    """User-defined float parameters"""
+
     data: ImageData[T_NP]
+    """Image data array"""
+
     meta: dict[str, list[str]]
+    """Meta attributes"""
+
 
     def __init__(self, *,
         flags: ImageFlags = ImageFlags(0),
         measurement_uid: yardl.UInt32 = 0,
         field_of_view: typing.Optional[npt.NDArray[np.float32]] = None,
         position: typing.Optional[npt.NDArray[np.float32]] = None,
         col_dir: typing.Optional[npt.NDArray[np.float32]] = None,
@@ -1547,20 +1659,34 @@
         return f"Image(flags={repr(self.flags)}, measurementUid={repr(self.measurement_uid)}, fieldOfView={repr(self.field_of_view)}, position={repr(self.position)}, colDir={repr(self.col_dir)}, lineDir={repr(self.line_dir)}, sliceDir={repr(self.slice_dir)}, patientTablePosition={repr(self.patient_table_position)}, average={repr(self.average)}, slice={repr(self.slice)}, contrast={repr(self.contrast)}, phase={repr(self.phase)}, repetition={repr(self.repetition)}, set={repr(self.set)}, acquisitionTimeStamp={repr(self.acquisition_time_stamp)}, physiologyTimeStamp={repr(self.physiology_time_stamp)}, imageType={repr(self.image_type)}, imageIndex={repr(self.image_index)}, imageSeriesIndex={repr(self.image_series_index)}, userInt={repr(self.user_int)}, userFloat={repr(self.user_float)}, data={repr(self.data)}, meta={repr(self.meta)})"
 
 
 WaveformSamples = npt.NDArray[T_NP]
 
 class Waveform(typing.Generic[T_NP]):
     flags: yardl.UInt64
+    """Bit field of flags. Currently unused"""
+
     measurement_uid: yardl.UInt32
+    """Unique ID for this measurement"""
+
     scan_counter: yardl.UInt32
+    """Number of the acquisition after this waveform"""
+
     time_stamp: yardl.UInt32
+    """Starting timestamp of this waveform"""
+
     sample_time_us: yardl.Float32
+    """Time between samples in microseconds"""
+
     waveform_id: yardl.UInt32
+    """ID matching the waveform in the MRD header"""
+
     data: WaveformSamples[T_NP]
+    """Waveform sample array"""
+
 
     def __init__(self, *,
         flags: yardl.UInt64 = 0,
         measurement_uid: yardl.UInt32 = 0,
         scan_counter: yardl.UInt32 = 0,
         time_stamp: yardl.UInt32 = 0,
         sample_time_us: yardl.Float32 = 0.0,
```

### Comparing `mrd_python-2.0.0rc2/mrd/yardl_types.py` & `mrd_python-2.0.0rc3/mrd/yardl_types.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc2/mrd_python.egg-info/PKG-INFO` & `mrd_python-2.0.0rc3/mrd_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrd-python
-Version: 2.0.0rc2
+Version: 2.0.0rc3
 Summary: Library and tools for working with data in the ISMRM Raw Data (MRD) format.
 Project-URL: Homepage, https://ismrmrd.github.io/mrd
 Project-URL: Documentation, https://ismrmrd.github.io/mrd
 Project-URL: Repository, https://github.com/ismrmrd/mrd
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mrd_python-2.0.0rc2/pyproject.toml` & `mrd_python-2.0.0rc3/pyproject.toml`

 * *Files identical despite different names*

