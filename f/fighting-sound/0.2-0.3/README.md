# Comparing `tmp/fighting_sound-0.2.tar.gz` & `tmp/fighting_sound-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fighting_sound-0.2.tar", last modified: Sat May 18 14:32:34 2024, max compression
+gzip compressed data, was "fighting_sound-0.3.tar", last modified: Mon May 27 07:58:25 2024, max compression
```

## Comparing `fighting_sound-0.2.tar` & `fighting_sound-0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 14:32:34.022709 fighting_sound-0.2/
--rw-rw-rw-   0        0        0      924 2024-05-18 14:32:34.020332 fighting_sound-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      392 2024-05-17 21:28:52.000000 fighting_sound-0.2/README.md
--rw-rw-rw-   0        0        0      547 2024-05-18 14:31:37.000000 fighting_sound-0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-18 14:32:34.022709 fighting_sound-0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-18 14:32:33.989080 fighting_sound-0.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-18 14:32:34.020332 fighting_sound-0.2/src/fighting_sound.egg-info/
--rw-rw-rw-   0        0        0      924 2024-05-18 14:32:33.000000 fighting_sound-0.2/src/fighting_sound.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      633 2024-05-18 14:32:33.000000 fighting_sound-0.2/src/fighting_sound.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 14:32:33.000000 fighting_sound-0.2/src/fighting_sound.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-18 14:32:33.000000 fighting_sound-0.2/src/fighting_sound.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-18 14:32:33.000000 fighting_sound-0.2/src/fighting_sound.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-18 14:32:34.004706 fighting_sound-0.2/src/pyftg_sound/
-drwxrwxrwx   0        0        0        0 2024-05-18 14:32:34.004706 fighting_sound-0.2/src/pyftg_sound/models/
--rw-rw-rw-   0        0        0      771 2024-05-17 21:28:52.000000 fighting_sound-0.2/src/pyftg_sound/models/audio_buffer.py
--rw-rw-rw-   0        0        0      618 2024-05-17 21:28:52.000000 fighting_sound-0.2/src/pyftg_sound/models/audio_source.py
--rw-rw-rw-   0        0        0     4896 2024-05-17 21:28:52.000000 fighting_sound-0.2/src/pyftg_sound/models/sound_renderer.py
-drwxrwxrwx   0        0        0        0 2024-05-18 14:32:34.004706 fighting_sound-0.2/src/pyftg_sound/openal/
--rw-rw-rw-   0        0        0     3326 2024-05-17 21:28:52.000000 fighting_sound-0.2/src/pyftg_sound/openal/__init__.py
--rw-rw-rw-   0        0        0    11580 2024-05-17 21:28:52.000000 fighting_sound-0.2/src/pyftg_sound/openal/al.py
--rw-rw-rw-   0        0        0     6354 2024-05-17 21:28:52.000000 fighting_sound-0.2/src/pyftg_sound/openal/alc.py
--rw-rw-rw-   0        0        0       54 2024-05-17 21:28:52.000000 fighting_sound-0.2/src/pyftg_sound/openal/log.py
--rw-rw-rw-   0        0        0     1471 2024-05-17 21:28:52.000000 fighting_sound-0.2/src/pyftg_sound/openal/soft.py
--rw-rw-rw-   0        0        0     6657 2024-05-17 21:33:25.000000 fighting_sound-0.2/src/pyftg_sound/sound_manager.py
-drwxrwxrwx   0        0        0        0 2024-05-18 14:32:34.004706 fighting_sound-0.2/src/pyftg_sound/utils/
--rw-rw-rw-   0        0        0      296 2024-05-17 21:28:52.000000 fighting_sound-0.2/src/pyftg_sound/utils/dtype.py
--rw-rw-rw-   0        0        0     1269 2024-05-17 21:28:52.000000 fighting_sound-0.2/src/pyftg_sound/utils/openal.py
--rw-rw-rw-   0        0        0      662 2024-05-17 21:28:52.000000 fighting_sound-0.2/src/pyftg_sound/utils/wave.py
+drwxrwxr-x   0 lin       (1000) lin       (1000)        0 2024-05-27 07:58:25.386014 fighting_sound-0.3/
+-rw-r--r--   0 lin       (1000) lin       (1000)      872 2024-05-27 07:58:25.386014 fighting_sound-0.3/PKG-INFO
+-rw-rw-r--   0 lin       (1000) lin       (1000)      374 2024-05-26 20:47:01.000000 fighting_sound-0.3/README.md
+-rw-rw-r--   0 lin       (1000) lin       (1000)      506 2024-05-27 07:44:28.000000 fighting_sound-0.3/pyproject.toml
+-rw-rw-r--   0 lin       (1000) lin       (1000)       38 2024-05-27 07:58:25.386014 fighting_sound-0.3/setup.cfg
+drwxrwxr-x   0 lin       (1000) lin       (1000)        0 2024-05-27 07:58:25.382014 fighting_sound-0.3/src/
+drwxrwxr-x   0 lin       (1000) lin       (1000)        0 2024-05-27 07:58:25.386014 fighting_sound-0.3/src/fighting_sound.egg-info/
+-rw-r--r--   0 lin       (1000) lin       (1000)      872 2024-05-27 07:58:25.000000 fighting_sound-0.3/src/fighting_sound.egg-info/PKG-INFO
+-rw-rw-r--   0 lin       (1000) lin       (1000)      633 2024-05-27 07:58:25.000000 fighting_sound-0.3/src/fighting_sound.egg-info/SOURCES.txt
+-rw-rw-r--   0 lin       (1000) lin       (1000)        1 2024-05-27 07:58:25.000000 fighting_sound-0.3/src/fighting_sound.egg-info/dependency_links.txt
+-rw-rw-r--   0 lin       (1000) lin       (1000)       14 2024-05-27 07:58:25.000000 fighting_sound-0.3/src/fighting_sound.egg-info/requires.txt
+-rw-rw-r--   0 lin       (1000) lin       (1000)       12 2024-05-27 07:58:25.000000 fighting_sound-0.3/src/fighting_sound.egg-info/top_level.txt
+drwxrwxr-x   0 lin       (1000) lin       (1000)        0 2024-05-27 07:58:25.382014 fighting_sound-0.3/src/pyftg_sound/
+drwxrwxr-x   0 lin       (1000) lin       (1000)        0 2024-05-27 07:58:25.382014 fighting_sound-0.3/src/pyftg_sound/models/
+-rw-rw-r--   0 lin       (1000) lin       (1000)      748 2024-05-26 20:47:01.000000 fighting_sound-0.3/src/pyftg_sound/models/audio_buffer.py
+-rw-rw-r--   0 lin       (1000) lin       (1000)      598 2024-05-26 20:47:01.000000 fighting_sound-0.3/src/pyftg_sound/models/audio_source.py
+-rw-rw-r--   0 lin       (1000) lin       (1000)     4767 2024-05-26 20:47:01.000000 fighting_sound-0.3/src/pyftg_sound/models/sound_renderer.py
+drwxrwxr-x   0 lin       (1000) lin       (1000)        0 2024-05-27 07:58:25.382014 fighting_sound-0.3/src/pyftg_sound/openal/
+-rw-rw-r--   0 lin       (1000) lin       (1000)     3225 2024-05-26 20:47:01.000000 fighting_sound-0.3/src/pyftg_sound/openal/__init__.py
+-rw-rw-r--   0 lin       (1000) lin       (1000)    11332 2024-05-26 20:47:01.000000 fighting_sound-0.3/src/pyftg_sound/openal/al.py
+-rw-rw-r--   0 lin       (1000) lin       (1000)     6202 2024-05-26 20:47:01.000000 fighting_sound-0.3/src/pyftg_sound/openal/alc.py
+-rw-rw-r--   0 lin       (1000) lin       (1000)       51 2024-05-26 20:47:01.000000 fighting_sound-0.3/src/pyftg_sound/openal/log.py
+-rw-rw-r--   0 lin       (1000) lin       (1000)     1431 2024-05-26 20:47:01.000000 fighting_sound-0.3/src/pyftg_sound/openal/soft.py
+-rw-rw-r--   0 lin       (1000) lin       (1000)     7190 2024-05-27 07:30:19.000000 fighting_sound-0.3/src/pyftg_sound/sound_manager.py
+drwxrwxr-x   0 lin       (1000) lin       (1000)        0 2024-05-27 07:58:25.386014 fighting_sound-0.3/src/pyftg_sound/utils/
+-rw-rw-r--   0 lin       (1000) lin       (1000)      282 2024-05-26 20:47:01.000000 fighting_sound-0.3/src/pyftg_sound/utils/dtype.py
+-rw-rw-r--   0 lin       (1000) lin       (1000)     1239 2024-05-26 20:47:01.000000 fighting_sound-0.3/src/pyftg_sound/utils/openal.py
+-rw-rw-r--   0 lin       (1000) lin       (1000)      640 2024-05-26 20:47:01.000000 fighting_sound-0.3/src/pyftg_sound/utils/wave.py
```

### Comparing `fighting_sound-0.2/src/fighting_sound.egg-info/SOURCES.txt` & `fighting_sound-0.3/src/fighting_sound.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fighting_sound-0.2/src/pyftg_sound/models/audio_buffer.py` & `fighting_sound-0.3/src/pyftg_sound/models/audio_buffer.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from pathlib import Path
-from typing import List
-
-from pyftg_sound.openal import al, alc
-from pyftg_sound.utils.wave import load_sound
-
-
-class AudioBuffer:
-    contexts: List[alc.ALCcontext]
-    buffers: List[int]
-
-    def __init__(self, contexts: List[alc.ALCcontext], buffers: List[int]) -> None:
-        self.contexts = contexts
-        self.buffers = buffers
-
-    def get_buffers(self) -> List[int]:
-        return self.buffers
-    
-    def register_sound(self, file_path: Path) -> None:
-        for i, buffer_id in enumerate(self.buffers):
-            alc.alcMakeContextCurrent(self.contexts[i])
-            alformat, wavbuf, samplerate = load_sound(file_path)
-            al.alBufferData(buffer_id, alformat, wavbuf, len(wavbuf), samplerate)
+from pathlib import Path
+from typing import List
+
+from pyftg_sound.openal import al, alc
+from pyftg_sound.utils.wave import load_sound
+
+
+class AudioBuffer:
+    contexts: List[alc.ALCcontext]
+    buffers: List[int]
+
+    def __init__(self, contexts: List[alc.ALCcontext], buffers: List[int]) -> None:
+        self.contexts = contexts
+        self.buffers = buffers
+
+    def get_buffers(self) -> List[int]:
+        return self.buffers
+    
+    def register_sound(self, file_path: Path) -> None:
+        for i, buffer_id in enumerate(self.buffers):
+            alc.alcMakeContextCurrent(self.contexts[i])
+            alformat, wavbuf, samplerate = load_sound(file_path)
+            al.alBufferData(buffer_id, alformat, wavbuf, len(wavbuf), samplerate)
```

### Comparing `fighting_sound-0.2/src/pyftg_sound/models/sound_renderer.py` & `fighting_sound-0.3/src/pyftg_sound/models/sound_renderer.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-import ctypes
-from typing import List
-
-import numpy as np
-
-from pyftg_sound.openal import al, alc, soft
-from pyftg_sound.utils.dtype import dtype_map
-from pyftg_sound.utils.openal import set_source_attribute
-
-
-class SoundRenderer:
-    device = None
-    context = None
-
-    def __init__(self, device, context) -> None:
-        self.device = device
-        self.context = context
-
-    @staticmethod
-    def create_default_renderer():
-        device = alc.alcOpenDevice(None)
-        context = alc.alcCreateContext(device, None)
-        return SoundRenderer(device, context)
-
-    @staticmethod
-    def create_virtual_renderer(format: int = soft.ALC_FLOAT_SOFT, channel: int = soft.ALC_STEREO_SOFT, sample_rate: int = 48000):
-        device = soft.alcLoopbackOpenDeviceSOFT(None)
-        attrs = [
-            soft.ALC_FORMAT_TYPE_SOFT, format, soft.ALC_FORMAT_CHANNELS_SOFT,
-            channel, alc.ALC_FREQUENCY, sample_rate, 0
-        ]
-        attrs_c = (al.ALint * len(attrs))(*attrs)
-        context = alc.alcCreateContext(device, attrs_c)
-        return SoundRenderer(device, context)
-
-    def set(self) -> None:
-        alc.alcMakeContextCurrent(self.context)
-
-    def create_source(self, attrs: dict) -> int:
-        self.set()
-        source = al.ALuint(0)
-        al.alGenSources(1, source)
-        for attr, value in attrs.items():
-            set_source_attribute(source, attr, value)
-        return source.value
-        
-    def create_buffer(self) -> int:
-        self.set()
-        buffer = al.ALuint(0)
-        al.alGenBuffers(1, buffer)
-        return buffer.value
-
-    def al_listener_fv(self, param: int, values: List[float]) -> None:
-        self.set()
-        values_arr = (al.ALfloat * len(values))(*values)
-        al.alListenerfv(param, values_arr)
-
-    def play(self, source_id: int) -> None:
-        self.set()
-        al.alSourcePlay(source_id)
-
-    def is_playing(self, source_id: int) -> bool:
-        self.set()
-        state = al.ALint(0)
-        al.alGetSourcei(source_id, al.AL_SOURCE_STATE, state)
-        return state.value == al.AL_PLAYING
-
-    def stop(self, source_id: int) -> None:
-        self.set()
-        if self.is_playing(source_id):
-            al.alSourceStop(source_id)
-
-    def play2(self, source_id: int, buffer_id: int, x: float, y: float, z: float, loop: bool) -> None:
-        self.set()
-        if self.is_playing(source_id):
-            self.stop(source_id)
-        set_source_attribute(source_id, al.AL_BUFFER, buffer_id)
-        set_source_attribute(source_id, al.AL_POSITION, [x, y, z])
-        set_source_attribute(source_id, al.AL_LOOPING, al.AL_TRUE if loop else al.AL_FALSE)
-        self.play(source_id)
-
-    def delete_source(self, source_id: int) -> None:
-        self.set()
-        al.alDeleteSources(1, al.ALuint(source_id))
-
-    def delete_buffer(self, buffer_id: int) -> None:
-        self.set()
-        al.alDeleteBuffers(1, al.ALuint(buffer_id))
-
-    def close(self) -> None:
-        self.set()
-        alc.alcDestroyContext(self.context)
-        alc.alcCloseDevice(self.device)
-
-    def sample_audio(self, dtype: type, render_size: int, nchannels: int) -> np.ndarray:
-        self.set()
-        audio_sample_type = dtype * render_size * nchannels
-        audio_sample_ptr = ctypes.cast(audio_sample_type(), ctypes.c_void_p)
-        soft.alcRenderSamplesSOFT(self.device, audio_sample_ptr, al.ALsizei(render_size))
-        separated_channel_audio = np.zeros((nchannels, render_size), dtype=dtype_map[dtype])
-        separated_channel_audio[:, :] = ctypes.cast(audio_sample_ptr, ctypes.POINTER(audio_sample_type)).contents
-        return separated_channel_audio
-    
-    def get_processed_buffers(self, source_id: int) -> int:
-        self.set()
-        processed_buffers = al.ALint(0)
-        al.alGetSourcei(source_id, al.AL_BUFFERS_PROCESSED, processed_buffers)
-        return processed_buffers.value
-    
-    def playback(self, source_id: int, format: int, audio_sample: bytes, sample_rate: int) -> None:
-        self.set()
-        buffer = al.ALuint(0)
-        if self.get_processed_buffers(source_id) > 0:
-            al.alSourceUnqueueBuffers(source_id, 1, buffer)
-        else:
-            al.alGenBuffers(1, buffer)
-        al.alBufferData(buffer, format, audio_sample, len(audio_sample), sample_rate)
-        al.alSourceQueueBuffers(source_id, 1, buffer)
-        if not self.is_playing(source_id):
-            self.play(source_id)
-
-    def stop_playback(self, source_id: int) -> None:
-        self.set()
-        buffer = al.ALuint(0)
-        for _ in range(self.get_processed_buffers(source_id)):
-            al.alSourceUnqueueBuffers(source_id, 1, buffer)
-            al.alDeleteBuffers(1, buffer)
-        self.stop(source_id)
-        self.al_source_i(source_id, al.AL_BUFFER, al.AL_NONE)
+import ctypes
+from typing import List
+
+import numpy as np
+
+from pyftg_sound.openal import al, alc, soft
+from pyftg_sound.utils.dtype import dtype_map
+from pyftg_sound.utils.openal import set_source_attribute
+
+
+class SoundRenderer:
+    device = None
+    context = None
+
+    def __init__(self, device, context) -> None:
+        self.device = device
+        self.context = context
+
+    @staticmethod
+    def create_default_renderer():
+        device = alc.alcOpenDevice(None)
+        context = alc.alcCreateContext(device, None)
+        return SoundRenderer(device, context)
+
+    @staticmethod
+    def create_virtual_renderer(format: int = soft.ALC_FLOAT_SOFT, channel: int = soft.ALC_STEREO_SOFT, sample_rate: int = 48000):
+        device = soft.alcLoopbackOpenDeviceSOFT(None)
+        attrs = [
+            soft.ALC_FORMAT_TYPE_SOFT, format, soft.ALC_FORMAT_CHANNELS_SOFT,
+            channel, alc.ALC_FREQUENCY, sample_rate, 0
+        ]
+        attrs_c = (al.ALint * len(attrs))(*attrs)
+        context = alc.alcCreateContext(device, attrs_c)
+        return SoundRenderer(device, context)
+
+    def set(self) -> None:
+        alc.alcMakeContextCurrent(self.context)
+
+    def create_source(self, attrs: dict) -> int:
+        self.set()
+        source = al.ALuint(0)
+        al.alGenSources(1, source)
+        for attr, value in attrs.items():
+            set_source_attribute(source, attr, value)
+        return source.value
+        
+    def create_buffer(self) -> int:
+        self.set()
+        buffer = al.ALuint(0)
+        al.alGenBuffers(1, buffer)
+        return buffer.value
+
+    def al_listener_fv(self, param: int, values: List[float]) -> None:
+        self.set()
+        values_arr = (al.ALfloat * len(values))(*values)
+        al.alListenerfv(param, values_arr)
+
+    def play(self, source_id: int) -> None:
+        self.set()
+        al.alSourcePlay(source_id)
+
+    def is_playing(self, source_id: int) -> bool:
+        self.set()
+        state = al.ALint(0)
+        al.alGetSourcei(source_id, al.AL_SOURCE_STATE, state)
+        return state.value == al.AL_PLAYING
+
+    def stop(self, source_id: int) -> None:
+        self.set()
+        if self.is_playing(source_id):
+            al.alSourceStop(source_id)
+
+    def play2(self, source_id: int, buffer_id: int, x: float, y: float, z: float, loop: bool) -> None:
+        self.set()
+        if self.is_playing(source_id):
+            self.stop(source_id)
+        set_source_attribute(source_id, al.AL_BUFFER, buffer_id)
+        set_source_attribute(source_id, al.AL_POSITION, [x, y, z])
+        set_source_attribute(source_id, al.AL_LOOPING, al.AL_TRUE if loop else al.AL_FALSE)
+        self.play(source_id)
+
+    def delete_source(self, source_id: int) -> None:
+        self.set()
+        al.alDeleteSources(1, al.ALuint(source_id))
+
+    def delete_buffer(self, buffer_id: int) -> None:
+        self.set()
+        al.alDeleteBuffers(1, al.ALuint(buffer_id))
+
+    def close(self) -> None:
+        self.set()
+        alc.alcDestroyContext(self.context)
+        alc.alcCloseDevice(self.device)
+
+    def sample_audio(self, dtype: type, render_size: int, nchannels: int) -> np.ndarray:
+        self.set()
+        audio_sample_type = dtype * render_size * nchannels
+        audio_sample_ptr = ctypes.cast(audio_sample_type(), ctypes.c_void_p)
+        soft.alcRenderSamplesSOFT(self.device, audio_sample_ptr, al.ALsizei(render_size))
+        separated_channel_audio = np.zeros((nchannels, render_size), dtype=dtype_map[dtype])
+        separated_channel_audio[:, :] = ctypes.cast(audio_sample_ptr, ctypes.POINTER(audio_sample_type)).contents
+        return separated_channel_audio
+    
+    def get_processed_buffers(self, source_id: int) -> int:
+        self.set()
+        processed_buffers = al.ALint(0)
+        al.alGetSourcei(source_id, al.AL_BUFFERS_PROCESSED, processed_buffers)
+        return processed_buffers.value
+    
+    def playback(self, source_id: int, format: int, audio_sample: bytes, sample_rate: int) -> None:
+        self.set()
+        buffer = al.ALuint(0)
+        if self.get_processed_buffers(source_id) > 0:
+            al.alSourceUnqueueBuffers(source_id, 1, buffer)
+        else:
+            al.alGenBuffers(1, buffer)
+        al.alBufferData(buffer, format, audio_sample, len(audio_sample), sample_rate)
+        al.alSourceQueueBuffers(source_id, 1, buffer)
+        if not self.is_playing(source_id):
+            self.play(source_id)
+
+    def stop_playback(self, source_id: int) -> None:
+        self.set()
+        buffer = al.ALuint(0)
+        for _ in range(self.get_processed_buffers(source_id)):
+            al.alSourceUnqueueBuffers(source_id, 1, buffer)
+            al.alDeleteBuffers(1, buffer)
+        self.stop(source_id)
+        self.al_source_i(source_id, al.AL_BUFFER, al.AL_NONE)
```

### Comparing `fighting_sound-0.2/src/pyftg_sound/openal/al.py` & `fighting_sound-0.3/src/pyftg_sound/openal/al.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,248 +1,248 @@
-import ctypes
-
-from . import dll
-
-__all__ = ["AL_INVALID", "AL_NONE", "AL_TRUE", "AL_FALSE",
-           "AL_SOURCE_RELATIVE", "AL_CONE_INNER_ANGLE", "AL_CONE_OUTER_ANGLE",
-           "AL_PITCH", "AL_POSITION", "AL_DIRECTION", "AL_VELOCITY",
-           "AL_LOOPING", "AL_BUFFER", "AL_GAIN", "AL_MIN_GAIN", "AL_MAX_GAIN",
-           "AL_ORIENTATION", "AL_CHANNEL_MASK", "AL_SOURCE_STATE",
-           "AL_INITIAL", "AL_PLAYING", "AL_PAUSED", "AL_STOPPED",
-           "AL_BUFFERS_QUEUED", "AL_BUFFERS_PROCESSED", "AL_SEC_OFFSET",
-           "AL_SAMPLE_OFFSET", "AL_BYTE_OFFSET", "AL_SOURCE_TYPE",
-           "AL_STATIC", "AL_STREAMING", "AL_UNDETERMINED", "AL_FORMAT_MONO8",
-           "AL_FORMAT_MONO16", "AL_FORMAT_STEREO8", "AL_FORMAT_STEREO16",
-           "AL_REFERENCE_DISTANCE", "AL_ROLLOFF_FACTOR", "AL_CONE_OUTER_GAIN",
-           "AL_MAX_DISTANCE", "AL_FREQUENCY", "AL_BITS", "AL_CHANNELS",
-           "AL_SIZE", "AL_UNUSED", "AL_PENDING", "AL_PROCESSED", "AL_NO_ERROR",
-           "AL_INVALID_NAME", "AL_ILLEGAL_ENUM", "AL_INVALID_ENUM",
-           "AL_INVALID_VALUE", "AL_ILLEGAL_COMMAND", "AL_INVALID_OPERATION",
-           "AL_OUT_OF_MEMORY", "AL_VENDOR", "AL_VERSION", "AL_RENDERER",
-           "AL_EXTENSIONS", "AL_DOPPLER_FACTOR", "AL_DOPPLER_VELOCITY",
-           "AL_SPEED_OF_SOUND", "AL_DISTANCE_MODEL", "AL_INVERSE_DISTANCE",
-           "AL_INVERSE_DISTANCE_CLAMPED", "AL_LINEAR_DISTANCE",
-           "AL_LINEAR_DISTANCE_CLAMPED", "AL_EXPONENT_DISTANCE",
-           "AL_EXPONENT_DISTANCE_CLAMPED", "ALboolean", "ALchar", "ALbyte",
-           "ALubyte", "ALshort", "ALushort", "ALint", "ALuint", "ALsizei",
-           "ALenum", "ALfloat", "ALdouble", "ALvoid",
-           "alEnable", "alDisable", "alIsEnabled", "alGetString",
-           "alGetBooleanv", "alGetIntegerv", "alGetFloatv", "alGetDoublev",
-           "alGetBoolean", "alGetInteger", "alGetFloat", "alGetDouble",
-           "alGetError", "alIsExtensionPresent", "alGetProcAddress",
-           "alGetEnumValue", "alListenerf", "alListener3f", "alListenerfv",
-           "alListeneri", "alListener3i", "alListeneriv", "alGetListenerf",
-           "alGetListener3f", "alGetListenerfv", "alGetListeneri",
-           "alGetListener3i", "alGetListeneriv", "alGenSources",
-           "alDeleteSources", "alIsSource", "alSourcef", "alSource3f",
-           "alSourcefv", "alSourcei", "alSource3i", "alSourceiv",
-           "alGetSourcef", "alGetSource3f", "alGetSourcefv", "alGetSourcei",
-           "alGetSource3i", "alGetSourceiv", "alSourcePlayv", "alSourcePlay",
-           "alSourceStopv", "alSourceStop", "alSourceRewindv",
-           "alSourceRewind", "alSourcePausev", "alSourcePause",
-           "alSourceQueueBuffers", "alSourceUnqueueBuffers", "alGenBuffers",
-           "alIsBuffer", "alBufferData", "alBufferf", "alBuffer3f",
-           "alBufferfv", "alBufferi", "alBuffer3i", "alBufferiv",
-           "alGetBufferf", "alGetBuffer3f", "alGetBufferfv", "alGetBufferi",
-           "alGetBuffer3i", "alGetBufferiv", "alDopplerFactor",
-           "alDopplerVelocity", "alSpeedOfSound", "alDistanceModel",
-           ]
-
-_bind = dll.bind_function
-
-AL_INVALID = -1
-AL_NONE = 0
-
-AL_FALSE = 0
-AL_TRUE = 1
-
-AL_SOURCE_RELATIVE = 0x202
-
-AL_CONE_INNER_ANGLE = 0x1001
-AL_CONE_OUTER_ANGLE = 0x1002
-AL_PITCH = 0x1003
-AL_POSITION = 0x1004
-AL_DIRECTION = 0x1005
-AL_VELOCITY = 0x1006
-AL_LOOPING = 0x1007
-AL_BUFFER = 0x1009
-AL_GAIN = 0x100A
-AL_MIN_GAIN = 0x100D
-AL_MAX_GAIN = 0x100E
-AL_ORIENTATION = 0x100F
-
-AL_CHANNEL_MASK = 0x3000
-
-AL_SOURCE_STATE = 0x1010
-AL_INITIAL = 0x1011
-AL_PLAYING = 0x1012
-AL_PAUSED = 0x1013
-AL_STOPPED = 0x1014
-AL_BUFFERS_QUEUED = 0x1015
-AL_BUFFERS_PROCESSED = 0x1016
-
-AL_SEC_OFFSET = 0x1024
-AL_SAMPLE_OFFSET = 0x1025
-AL_BYTE_OFFSET = 0x1026
-AL_SOURCE_TYPE = 0x1027
-AL_STATIC = 0x1028
-AL_STREAMING = 0x1029
-AL_UNDETERMINED = 0x1030
-
-AL_FORMAT_MONO8 = 0x1100
-AL_FORMAT_MONO16 = 0x1101
-AL_FORMAT_STEREO8 = 0x1102
-AL_FORMAT_STEREO16 = 0x1103
-
-AL_REFERENCE_DISTANCE = 0x1020
-AL_ROLLOFF_FACTOR = 0x1021
-AL_CONE_OUTER_GAIN = 0x1022
-AL_MAX_DISTANCE = 0x1023
-
-AL_FREQUENCY = 0x2001
-AL_BITS = 0x2002
-AL_CHANNELS = 0x2003
-AL_SIZE = 0x2004
-
-AL_UNUSED = 0x2010
-AL_PENDING = 0x2011
-AL_PROCESSED = 0x2012
-
-AL_NO_ERROR = AL_FALSE
-AL_INVALID_NAME = 0xA001
-AL_ILLEGAL_ENUM = 0xA002
-AL_INVALID_ENUM = 0xA002
-AL_INVALID_VALUE = 0xA003
-AL_ILLEGAL_COMMAND = 0xA004
-AL_INVALID_OPERATION = 0xA004
-AL_OUT_OF_MEMORY = 0xA005
-
-AL_VENDOR = 0xB001
-AL_VERSION = 0xB002
-AL_RENDERER = 0xB003
-AL_EXTENSIONS = 0xB004
-
-AL_DOPPLER_FACTOR = 0xC000
-AL_DOPPLER_VELOCITY = 0xC001
-AL_SPEED_OF_SOUND = 0xC003
-
-AL_DISTANCE_MODEL = 0xD000
-AL_INVERSE_DISTANCE = 0xD001
-AL_INVERSE_DISTANCE_CLAMPED = 0xD002
-AL_LINEAR_DISTANCE = 0xD003
-AL_LINEAR_DISTANCE_CLAMPED = 0xD004
-AL_EXPONENT_DISTANCE = 0xD005
-AL_EXPONENT_DISTANCE_CLAMPED = 0xD006
-
-ALboolean = ctypes.c_char
-ALchar = ctypes.c_char
-ALbyte = ctypes.c_char
-ALubyte = ctypes.c_ubyte
-ALshort = ctypes.c_short
-ALushort = ctypes.c_ushort
-ALint = ctypes.c_int
-ALuint = ctypes.c_uint
-ALsizei = ctypes.c_int
-ALenum = ctypes.c_int
-ALfloat = ctypes.c_float
-ALdouble = ctypes.c_double
-ALvoid = None
-
-class ALCCapabilities(ctypes.Structure):
-    pass
-
-_bind = dll.bind_function
-
-alEnable = _bind("alEnable", [ALenum])
-alDisable = _bind("alDisable", [ALenum])
-alIsEnabled = _bind("alIsEnabled", [ALenum], ALboolean)
-alGetString = _bind("alGetString", [ALenum], ctypes.POINTER(ALchar))
-alGetBooleanv = _bind("alGetBooleanv", [ALenum, ctypes.POINTER(ALboolean)])
-alGetIntegerv = _bind("alGetIntegerv", [ALenum, ctypes.POINTER(ALint)])
-alGetFloatv = _bind("alGetFloatv", [ALenum, ctypes.POINTER(ALfloat)])
-alGetDoublev = _bind("alGetDoublev", [ALenum, ctypes.POINTER(ALdouble)])
-alGetBoolean = _bind("alGetBoolean", [ALenum], ALboolean)
-alGetInteger = _bind("alGetInteger", [ALenum], ALint)
-alGetFloat = _bind("alGetFloat", [ALenum], ALfloat)
-alGetDouble = _bind("alGetDouble", [ALenum], ALdouble)
-alGetError = _bind("alGetError", None, ALenum)
-alIsExtensionPresent = _bind("alIsExtensionPresent",
-                             [ctypes.POINTER(ALchar)], ALboolean)
-alGetProcAddress = _bind("alGetProcAddress",
-                         [ctypes.POINTER(ALchar)], ctypes.c_void_p)
-alGetEnumValue = _bind("alGetEnumValue", [ctypes.POINTER(ALchar)], ALenum)
-alListenerf = _bind("alListenerf", [ALenum, ALfloat])
-alListener3f = _bind("alListener3f", [ALenum, ALfloat, ALfloat, ALfloat])
-alListenerfv = _bind("alListenerfv", [ALenum, ctypes.POINTER(ALfloat)])
-alListeneri = _bind("alListeneri", [ALenum, ALint])
-alListener3i = _bind("alListener3i", [ALenum, ALint, ALint, ALint])
-alListeneriv = _bind("alListeneriv", [ALenum, ctypes.POINTER(ALint)])
-alGetListenerf = _bind("alGetListenerf", [ALenum, ctypes.POINTER(ALfloat)])
-alGetListener3f = _bind("alGetListener3f", [ALenum, ctypes.POINTER(ALfloat),
-                                            ctypes.POINTER(ALfloat),
-                                            ctypes.POINTER(ALfloat)])
-alGetListenerfv = _bind("alGetListenerfv", [ALenum, ctypes.POINTER(ALfloat)])
-alGetListeneri = _bind("alGetListeneri", [ALenum, ctypes.POINTER(ALint)])
-alGetListener3i = _bind("alGetListener3i", [ALenum, ctypes.POINTER(ALint),
-                                            ctypes.POINTER(ALint),
-                                            ctypes.POINTER(ALint)])
-alGetListeneriv = _bind("alGetListeneriv", [ALenum, ctypes.POINTER(ALint)])
-alGenSources = _bind("alGenSources", [ALsizei, ctypes.POINTER(ALuint)])
-alDeleteSources = _bind("alDeleteSources", [ALsizei, ctypes.POINTER(ALuint)])
-alIsSource = _bind("alIsSource", [ALuint], ALboolean)
-alSourcef = _bind("alSourcef", [ALuint, ALenum, ALfloat])
-alSource3f = _bind("alSource3f", [ALuint, ALenum, ALfloat, ALfloat, ALfloat])
-alSourcefv = _bind("alSourcefv", [ALuint, ALenum, ctypes.POINTER(ALfloat)])
-alSourcei = _bind("alSourcei", [ALuint, ALenum, ALint])
-alSource3i = _bind("alSource3i", [ALuint, ALenum, ALint, ALint, ALint])
-alSourceiv = _bind("alSourceiv", [ALuint, ALenum, ctypes.POINTER(ALint)])
-alGetSourcef = _bind("alGetSourcef", [ALuint, ALenum, ctypes.POINTER(ALfloat)])
-alGetSource3f = _bind("alGetSource3f", [ALuint, ALenum, ctypes.POINTER(ALfloat),
-                                        ctypes.POINTER(ALfloat),
-                                        ctypes.POINTER(ALfloat)])
-alGetSourcefv = _bind("alGetSourcefv", [ALuint, ALenum,
-                                        ctypes.POINTER(ALfloat)])
-alGetSourcei = _bind("alGetSourcei", [ALuint, ALenum, ctypes.POINTER(ALint)])
-alGetSource3i = _bind("alGetSource3i", [ALuint, ALenum, ctypes.POINTER(ALint),
-                                        ctypes.POINTER(ALint),
-                                        ctypes.POINTER(ALint)])
-alGetSourceiv = _bind("alGetSourceiv", [ALuint, ALenum, ctypes.POINTER(ALint)])
-alSourcePlayv = _bind("alSourcePlayv", [ALsizei, ctypes.POINTER(ALuint)])
-alSourceStopv = _bind("alSourceStopv", [ALsizei, ctypes.POINTER(ALuint)])
-alSourceRewindv = _bind("alSourceRewindv", [ALsizei, ctypes.POINTER(ALuint)])
-alSourcePausev = _bind("alSourcePausev", [ALsizei, ctypes.POINTER(ALuint)])
-alSourcePlay = _bind("alSourcePlay", [ALuint])
-alSourceStop = _bind("alSourceStop", [ALuint])
-alSourceRewind = _bind("alSourceRewind", [ALuint])
-alSourcePause = _bind("alSourcePause", [ALuint])
-alSourceQueueBuffers = _bind("alSourceQueueBuffers",
-                             [ALuint, ALsizei, ctypes.POINTER(ALuint)])
-alSourceUnqueueBuffers = _bind("alSourceUnqueueBuffers",
-                               [ALuint, ALsizei, ctypes.POINTER(ALuint)])
-alGenBuffers = _bind("alGenBuffers", [ALsizei, ctypes.POINTER(ALuint)])
-alDeleteBuffers = _bind("alDeleteBuffers", [ALsizei, ctypes.POINTER(ALuint)])
-alIsBuffer = _bind("alIsBuffer", [ALuint], ALboolean)
-alBufferData = _bind("alBufferData", [ALuint, ALenum, ctypes.POINTER(ALvoid),
-                                      ALsizei, ALsizei])
-alBufferf = _bind("alBufferf", [ALuint, ALenum, ALfloat])
-alBuffer3f = _bind("alBuffer3f", [ALuint, ALenum, ALfloat, ALfloat, ALfloat])
-alBufferfv = _bind("alBufferfv", [ALuint, ALenum, ctypes.POINTER(ALfloat)])
-alBufferi = _bind("alBufferi", [ALuint, ALenum, ALint])
-alBuffer3i = _bind("alBuffer3i", [ALuint, ALenum, ALint, ALint, ALint])
-alBufferiv = _bind("alBufferiv", [ALuint, ALenum, ctypes.POINTER(ALint)])
-alGetBufferf = _bind("alGetBufferf", [ALuint, ALenum, ctypes.POINTER(ALfloat)])
-alGetBuffer3f = _bind("alGetBuffer3f", [ALuint, ALenum,
-                                        ctypes.POINTER(ALfloat),
-                                        ctypes.POINTER(ALfloat),
-                                        ctypes.POINTER(ALfloat)])
-alGetBufferfv = _bind("alGetBufferfv", [ALuint, ALenum,
-                                        ctypes.POINTER(ALfloat)])
-alGetBufferi = _bind("alGetBufferi", [ALuint, ALenum, ctypes.POINTER(ALint)])
-alGetBuffer3i = _bind("alGetBuffer3i", [ALuint, ALenum,
-                                        ctypes.POINTER(ALint),
-                                        ctypes.POINTER(ALint),
-                                        ctypes.POINTER(ALint)])
-alGetBufferiv = _bind("alGetBufferiv", [ALuint, ALenum, ctypes.POINTER(ALint)])
-alDopplerFactor = _bind("alDopplerFactor", [ALfloat])
-alDopplerVelocity = _bind("alDopplerVelocity", [ALfloat])
-alSpeedOfSound = _bind("alSpeedOfSound", [ALfloat])
-alDistanceModel = _bind("alDistanceModel", [ALenum])
+import ctypes
+
+from . import dll
+
+__all__ = ["AL_INVALID", "AL_NONE", "AL_TRUE", "AL_FALSE",
+           "AL_SOURCE_RELATIVE", "AL_CONE_INNER_ANGLE", "AL_CONE_OUTER_ANGLE",
+           "AL_PITCH", "AL_POSITION", "AL_DIRECTION", "AL_VELOCITY",
+           "AL_LOOPING", "AL_BUFFER", "AL_GAIN", "AL_MIN_GAIN", "AL_MAX_GAIN",
+           "AL_ORIENTATION", "AL_CHANNEL_MASK", "AL_SOURCE_STATE",
+           "AL_INITIAL", "AL_PLAYING", "AL_PAUSED", "AL_STOPPED",
+           "AL_BUFFERS_QUEUED", "AL_BUFFERS_PROCESSED", "AL_SEC_OFFSET",
+           "AL_SAMPLE_OFFSET", "AL_BYTE_OFFSET", "AL_SOURCE_TYPE",
+           "AL_STATIC", "AL_STREAMING", "AL_UNDETERMINED", "AL_FORMAT_MONO8",
+           "AL_FORMAT_MONO16", "AL_FORMAT_STEREO8", "AL_FORMAT_STEREO16",
+           "AL_REFERENCE_DISTANCE", "AL_ROLLOFF_FACTOR", "AL_CONE_OUTER_GAIN",
+           "AL_MAX_DISTANCE", "AL_FREQUENCY", "AL_BITS", "AL_CHANNELS",
+           "AL_SIZE", "AL_UNUSED", "AL_PENDING", "AL_PROCESSED", "AL_NO_ERROR",
+           "AL_INVALID_NAME", "AL_ILLEGAL_ENUM", "AL_INVALID_ENUM",
+           "AL_INVALID_VALUE", "AL_ILLEGAL_COMMAND", "AL_INVALID_OPERATION",
+           "AL_OUT_OF_MEMORY", "AL_VENDOR", "AL_VERSION", "AL_RENDERER",
+           "AL_EXTENSIONS", "AL_DOPPLER_FACTOR", "AL_DOPPLER_VELOCITY",
+           "AL_SPEED_OF_SOUND", "AL_DISTANCE_MODEL", "AL_INVERSE_DISTANCE",
+           "AL_INVERSE_DISTANCE_CLAMPED", "AL_LINEAR_DISTANCE",
+           "AL_LINEAR_DISTANCE_CLAMPED", "AL_EXPONENT_DISTANCE",
+           "AL_EXPONENT_DISTANCE_CLAMPED", "ALboolean", "ALchar", "ALbyte",
+           "ALubyte", "ALshort", "ALushort", "ALint", "ALuint", "ALsizei",
+           "ALenum", "ALfloat", "ALdouble", "ALvoid",
+           "alEnable", "alDisable", "alIsEnabled", "alGetString",
+           "alGetBooleanv", "alGetIntegerv", "alGetFloatv", "alGetDoublev",
+           "alGetBoolean", "alGetInteger", "alGetFloat", "alGetDouble",
+           "alGetError", "alIsExtensionPresent", "alGetProcAddress",
+           "alGetEnumValue", "alListenerf", "alListener3f", "alListenerfv",
+           "alListeneri", "alListener3i", "alListeneriv", "alGetListenerf",
+           "alGetListener3f", "alGetListenerfv", "alGetListeneri",
+           "alGetListener3i", "alGetListeneriv", "alGenSources",
+           "alDeleteSources", "alIsSource", "alSourcef", "alSource3f",
+           "alSourcefv", "alSourcei", "alSource3i", "alSourceiv",
+           "alGetSourcef", "alGetSource3f", "alGetSourcefv", "alGetSourcei",
+           "alGetSource3i", "alGetSourceiv", "alSourcePlayv", "alSourcePlay",
+           "alSourceStopv", "alSourceStop", "alSourceRewindv",
+           "alSourceRewind", "alSourcePausev", "alSourcePause",
+           "alSourceQueueBuffers", "alSourceUnqueueBuffers", "alGenBuffers",
+           "alIsBuffer", "alBufferData", "alBufferf", "alBuffer3f",
+           "alBufferfv", "alBufferi", "alBuffer3i", "alBufferiv",
+           "alGetBufferf", "alGetBuffer3f", "alGetBufferfv", "alGetBufferi",
+           "alGetBuffer3i", "alGetBufferiv", "alDopplerFactor",
+           "alDopplerVelocity", "alSpeedOfSound", "alDistanceModel",
+           ]
+
+_bind = dll.bind_function
+
+AL_INVALID = -1
+AL_NONE = 0
+
+AL_FALSE = 0
+AL_TRUE = 1
+
+AL_SOURCE_RELATIVE = 0x202
+
+AL_CONE_INNER_ANGLE = 0x1001
+AL_CONE_OUTER_ANGLE = 0x1002
+AL_PITCH = 0x1003
+AL_POSITION = 0x1004
+AL_DIRECTION = 0x1005
+AL_VELOCITY = 0x1006
+AL_LOOPING = 0x1007
+AL_BUFFER = 0x1009
+AL_GAIN = 0x100A
+AL_MIN_GAIN = 0x100D
+AL_MAX_GAIN = 0x100E
+AL_ORIENTATION = 0x100F
+
+AL_CHANNEL_MASK = 0x3000
+
+AL_SOURCE_STATE = 0x1010
+AL_INITIAL = 0x1011
+AL_PLAYING = 0x1012
+AL_PAUSED = 0x1013
+AL_STOPPED = 0x1014
+AL_BUFFERS_QUEUED = 0x1015
+AL_BUFFERS_PROCESSED = 0x1016
+
+AL_SEC_OFFSET = 0x1024
+AL_SAMPLE_OFFSET = 0x1025
+AL_BYTE_OFFSET = 0x1026
+AL_SOURCE_TYPE = 0x1027
+AL_STATIC = 0x1028
+AL_STREAMING = 0x1029
+AL_UNDETERMINED = 0x1030
+
+AL_FORMAT_MONO8 = 0x1100
+AL_FORMAT_MONO16 = 0x1101
+AL_FORMAT_STEREO8 = 0x1102
+AL_FORMAT_STEREO16 = 0x1103
+
+AL_REFERENCE_DISTANCE = 0x1020
+AL_ROLLOFF_FACTOR = 0x1021
+AL_CONE_OUTER_GAIN = 0x1022
+AL_MAX_DISTANCE = 0x1023
+
+AL_FREQUENCY = 0x2001
+AL_BITS = 0x2002
+AL_CHANNELS = 0x2003
+AL_SIZE = 0x2004
+
+AL_UNUSED = 0x2010
+AL_PENDING = 0x2011
+AL_PROCESSED = 0x2012
+
+AL_NO_ERROR = AL_FALSE
+AL_INVALID_NAME = 0xA001
+AL_ILLEGAL_ENUM = 0xA002
+AL_INVALID_ENUM = 0xA002
+AL_INVALID_VALUE = 0xA003
+AL_ILLEGAL_COMMAND = 0xA004
+AL_INVALID_OPERATION = 0xA004
+AL_OUT_OF_MEMORY = 0xA005
+
+AL_VENDOR = 0xB001
+AL_VERSION = 0xB002
+AL_RENDERER = 0xB003
+AL_EXTENSIONS = 0xB004
+
+AL_DOPPLER_FACTOR = 0xC000
+AL_DOPPLER_VELOCITY = 0xC001
+AL_SPEED_OF_SOUND = 0xC003
+
+AL_DISTANCE_MODEL = 0xD000
+AL_INVERSE_DISTANCE = 0xD001
+AL_INVERSE_DISTANCE_CLAMPED = 0xD002
+AL_LINEAR_DISTANCE = 0xD003
+AL_LINEAR_DISTANCE_CLAMPED = 0xD004
+AL_EXPONENT_DISTANCE = 0xD005
+AL_EXPONENT_DISTANCE_CLAMPED = 0xD006
+
+ALboolean = ctypes.c_char
+ALchar = ctypes.c_char
+ALbyte = ctypes.c_char
+ALubyte = ctypes.c_ubyte
+ALshort = ctypes.c_short
+ALushort = ctypes.c_ushort
+ALint = ctypes.c_int
+ALuint = ctypes.c_uint
+ALsizei = ctypes.c_int
+ALenum = ctypes.c_int
+ALfloat = ctypes.c_float
+ALdouble = ctypes.c_double
+ALvoid = None
+
+class ALCCapabilities(ctypes.Structure):
+    pass
+
+_bind = dll.bind_function
+
+alEnable = _bind("alEnable", [ALenum])
+alDisable = _bind("alDisable", [ALenum])
+alIsEnabled = _bind("alIsEnabled", [ALenum], ALboolean)
+alGetString = _bind("alGetString", [ALenum], ctypes.POINTER(ALchar))
+alGetBooleanv = _bind("alGetBooleanv", [ALenum, ctypes.POINTER(ALboolean)])
+alGetIntegerv = _bind("alGetIntegerv", [ALenum, ctypes.POINTER(ALint)])
+alGetFloatv = _bind("alGetFloatv", [ALenum, ctypes.POINTER(ALfloat)])
+alGetDoublev = _bind("alGetDoublev", [ALenum, ctypes.POINTER(ALdouble)])
+alGetBoolean = _bind("alGetBoolean", [ALenum], ALboolean)
+alGetInteger = _bind("alGetInteger", [ALenum], ALint)
+alGetFloat = _bind("alGetFloat", [ALenum], ALfloat)
+alGetDouble = _bind("alGetDouble", [ALenum], ALdouble)
+alGetError = _bind("alGetError", None, ALenum)
+alIsExtensionPresent = _bind("alIsExtensionPresent",
+                             [ctypes.POINTER(ALchar)], ALboolean)
+alGetProcAddress = _bind("alGetProcAddress",
+                         [ctypes.POINTER(ALchar)], ctypes.c_void_p)
+alGetEnumValue = _bind("alGetEnumValue", [ctypes.POINTER(ALchar)], ALenum)
+alListenerf = _bind("alListenerf", [ALenum, ALfloat])
+alListener3f = _bind("alListener3f", [ALenum, ALfloat, ALfloat, ALfloat])
+alListenerfv = _bind("alListenerfv", [ALenum, ctypes.POINTER(ALfloat)])
+alListeneri = _bind("alListeneri", [ALenum, ALint])
+alListener3i = _bind("alListener3i", [ALenum, ALint, ALint, ALint])
+alListeneriv = _bind("alListeneriv", [ALenum, ctypes.POINTER(ALint)])
+alGetListenerf = _bind("alGetListenerf", [ALenum, ctypes.POINTER(ALfloat)])
+alGetListener3f = _bind("alGetListener3f", [ALenum, ctypes.POINTER(ALfloat),
+                                            ctypes.POINTER(ALfloat),
+                                            ctypes.POINTER(ALfloat)])
+alGetListenerfv = _bind("alGetListenerfv", [ALenum, ctypes.POINTER(ALfloat)])
+alGetListeneri = _bind("alGetListeneri", [ALenum, ctypes.POINTER(ALint)])
+alGetListener3i = _bind("alGetListener3i", [ALenum, ctypes.POINTER(ALint),
+                                            ctypes.POINTER(ALint),
+                                            ctypes.POINTER(ALint)])
+alGetListeneriv = _bind("alGetListeneriv", [ALenum, ctypes.POINTER(ALint)])
+alGenSources = _bind("alGenSources", [ALsizei, ctypes.POINTER(ALuint)])
+alDeleteSources = _bind("alDeleteSources", [ALsizei, ctypes.POINTER(ALuint)])
+alIsSource = _bind("alIsSource", [ALuint], ALboolean)
+alSourcef = _bind("alSourcef", [ALuint, ALenum, ALfloat])
+alSource3f = _bind("alSource3f", [ALuint, ALenum, ALfloat, ALfloat, ALfloat])
+alSourcefv = _bind("alSourcefv", [ALuint, ALenum, ctypes.POINTER(ALfloat)])
+alSourcei = _bind("alSourcei", [ALuint, ALenum, ALint])
+alSource3i = _bind("alSource3i", [ALuint, ALenum, ALint, ALint, ALint])
+alSourceiv = _bind("alSourceiv", [ALuint, ALenum, ctypes.POINTER(ALint)])
+alGetSourcef = _bind("alGetSourcef", [ALuint, ALenum, ctypes.POINTER(ALfloat)])
+alGetSource3f = _bind("alGetSource3f", [ALuint, ALenum, ctypes.POINTER(ALfloat),
+                                        ctypes.POINTER(ALfloat),
+                                        ctypes.POINTER(ALfloat)])
+alGetSourcefv = _bind("alGetSourcefv", [ALuint, ALenum,
+                                        ctypes.POINTER(ALfloat)])
+alGetSourcei = _bind("alGetSourcei", [ALuint, ALenum, ctypes.POINTER(ALint)])
+alGetSource3i = _bind("alGetSource3i", [ALuint, ALenum, ctypes.POINTER(ALint),
+                                        ctypes.POINTER(ALint),
+                                        ctypes.POINTER(ALint)])
+alGetSourceiv = _bind("alGetSourceiv", [ALuint, ALenum, ctypes.POINTER(ALint)])
+alSourcePlayv = _bind("alSourcePlayv", [ALsizei, ctypes.POINTER(ALuint)])
+alSourceStopv = _bind("alSourceStopv", [ALsizei, ctypes.POINTER(ALuint)])
+alSourceRewindv = _bind("alSourceRewindv", [ALsizei, ctypes.POINTER(ALuint)])
+alSourcePausev = _bind("alSourcePausev", [ALsizei, ctypes.POINTER(ALuint)])
+alSourcePlay = _bind("alSourcePlay", [ALuint])
+alSourceStop = _bind("alSourceStop", [ALuint])
+alSourceRewind = _bind("alSourceRewind", [ALuint])
+alSourcePause = _bind("alSourcePause", [ALuint])
+alSourceQueueBuffers = _bind("alSourceQueueBuffers",
+                             [ALuint, ALsizei, ctypes.POINTER(ALuint)])
+alSourceUnqueueBuffers = _bind("alSourceUnqueueBuffers",
+                               [ALuint, ALsizei, ctypes.POINTER(ALuint)])
+alGenBuffers = _bind("alGenBuffers", [ALsizei, ctypes.POINTER(ALuint)])
+alDeleteBuffers = _bind("alDeleteBuffers", [ALsizei, ctypes.POINTER(ALuint)])
+alIsBuffer = _bind("alIsBuffer", [ALuint], ALboolean)
+alBufferData = _bind("alBufferData", [ALuint, ALenum, ctypes.POINTER(ALvoid),
+                                      ALsizei, ALsizei])
+alBufferf = _bind("alBufferf", [ALuint, ALenum, ALfloat])
+alBuffer3f = _bind("alBuffer3f", [ALuint, ALenum, ALfloat, ALfloat, ALfloat])
+alBufferfv = _bind("alBufferfv", [ALuint, ALenum, ctypes.POINTER(ALfloat)])
+alBufferi = _bind("alBufferi", [ALuint, ALenum, ALint])
+alBuffer3i = _bind("alBuffer3i", [ALuint, ALenum, ALint, ALint, ALint])
+alBufferiv = _bind("alBufferiv", [ALuint, ALenum, ctypes.POINTER(ALint)])
+alGetBufferf = _bind("alGetBufferf", [ALuint, ALenum, ctypes.POINTER(ALfloat)])
+alGetBuffer3f = _bind("alGetBuffer3f", [ALuint, ALenum,
+                                        ctypes.POINTER(ALfloat),
+                                        ctypes.POINTER(ALfloat),
+                                        ctypes.POINTER(ALfloat)])
+alGetBufferfv = _bind("alGetBufferfv", [ALuint, ALenum,
+                                        ctypes.POINTER(ALfloat)])
+alGetBufferi = _bind("alGetBufferi", [ALuint, ALenum, ctypes.POINTER(ALint)])
+alGetBuffer3i = _bind("alGetBuffer3i", [ALuint, ALenum,
+                                        ctypes.POINTER(ALint),
+                                        ctypes.POINTER(ALint),
+                                        ctypes.POINTER(ALint)])
+alGetBufferiv = _bind("alGetBufferiv", [ALuint, ALenum, ctypes.POINTER(ALint)])
+alDopplerFactor = _bind("alDopplerFactor", [ALfloat])
+alDopplerVelocity = _bind("alDopplerVelocity", [ALfloat])
+alSpeedOfSound = _bind("alSpeedOfSound", [ALfloat])
+alDistanceModel = _bind("alDistanceModel", [ALenum])
```

### Comparing `fighting_sound-0.2/src/pyftg_sound/openal/alc.py` & `fighting_sound-0.3/src/pyftg_sound/openal/alc.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,152 +1,152 @@
-import ctypes
-
-from . import dll
-
-__all__ = ["ALC_FALSE", "ALC_TRUE", "ALC_INVALID", "ALC_FREQUENCY",
-           "ALC_REFRESH", "ALC_SYNC", "ALC_MONO_SOURCES", "ALC_STEREO_SOURCES",
-           "ALC_NO_ERROR", "ALC_INVALID_DEVICE", "ALC_INVALID_CONTEXT",
-           "ALC_INVALID_ENUM", "ALC_INVALID_VALUE", "ALC_OUT_OF_MEMORY",
-           "ALC_DEFAULT_DEVICE_SPECIFIER", "ALC_DEVICE_SPECIFIER",
-           "ALC_EXTENSIONS", "ALC_MAJOR_VERSION", "ALC_MINOR_VERSION",
-           "ALC_ATTRIBUTES_SIZE", "ALC_ALL_ATTRIBUTES",
-           "ALC_DEFAULT_ALL_DEVICES_SPECIFIER", "ALC_ALL_DEVICES_SPECIFIER",
-           "ALC_CAPTURE_DEVICE_SPECIFIER",
-           "ALC_CAPTURE_DEFAULT_DEVICE_SPECIFIER", "ALC_CAPTURE_SAMPLES",
-           "ALC_HRTF_SOFT", "ALC_HRTF_ID_SOFT", "ALC_DONT_CARE_SOFT",
-           "ALC_HRTF_STATUS_SOFT", "ALC_NUM_HRTF_SPECIFIERS_SOFT",
-           "ALC_HRTF_SPECIFIER_SOFT", "ALC_HRTF_DISABLED_SOFT",
-           "ALC_HRTF_ENABLED_SOFT", "ALC_HRTF_DENIED_SOFT",
-           "ALC_HRTF_REQUIRED_SOFT", "ALC_HRTF_HEADPHONES_DETECTED_SOFT",
-           "ALC_HRTF_UNSUPPORTED_FORMAT_SOFT",
-           "ALCboolean", "ALCchar", "ALCbyte", "ALCubyte", "ALCshort",
-           "ALCushort", "ALCint", "ALCuint", "ALCsizei", "ALCenum", "ALCfloat",
-           "ALCdouble", "ALCvoid", "ALCdevice", "ALCcontext",
-           "alcCreateContext", "alcMakeContextCurrent", "alcProcessContext",
-           "alcSuspendContext", "alcDestroyContext", "alcGetCurrentContext",
-           "alcGetContextsDevice", "alcOpenDevice", "alcCloseDevice",
-           "alcGetError", "alcIsExtensionPresent", "alcGetProcAddress",
-           "alcGetEnumValue", "alcGetString", "alcGetIntegerv",
-           "alcCaptureOpenDevice", "alcCaptureCloseDevice", "alcCaptureStart",
-           "alcCaptureStop", "alcCaptureSamples",
-           ]
-
-_bind = dll.bind_function
-
-ALC_INVALID = 0
-ALC_FALSE = 0
-ALC_TRUE = 1
-
-ALC_FREQUENCY = 0x1007
-ALC_REFRESH = 0x1008
-ALC_SYNC = 0x1009
-
-ALC_MONO_SOURCES = 0x1010
-ALC_STEREO_SOURCES = 0x1011
-
-ALC_NO_ERROR = ALC_FALSE
-ALC_INVALID_DEVICE = 0xA001
-ALC_INVALID_CONTEXT = 0xA002
-ALC_INVALID_ENUM = 0xA003
-ALC_INVALID_VALUE = 0xA004
-ALC_OUT_OF_MEMORY = 0xA005
-
-ALC_DEFAULT_DEVICE_SPECIFIER = 0x1004
-ALC_DEVICE_SPECIFIER = 0x1005
-ALC_EXTENSIONS = 0x1006
-
-ALC_MAJOR_VERSION = 0x1000
-ALC_MINOR_VERSION = 0x1001
-
-ALC_ATTRIBUTES_SIZE = 0x1002
-ALC_ALL_ATTRIBUTES = 0x1003
-
-ALC_DEFAULT_ALL_DEVICES_SPECIFIER = 0x1012
-ALC_ALL_DEVICES_SPECIFIER = 0x1013
-
-ALC_CAPTURE_DEVICE_SPECIFIER = 0x310
-ALC_CAPTURE_DEFAULT_DEVICE_SPECIFIER = 0x311
-ALC_CAPTURE_SAMPLES = 0x312
-
-ALC_HRTF_SOFT = 0x1992
-ALC_HRTF_ID_SOFT = 0x1996
-ALC_DONT_CARE_SOFT = 0x002
-ALC_HRTF_STATUS_SOFT = 0x1993
-ALC_NUM_HRTF_SPECIFIERS_SOFT = 0x1994
-ALC_HRTF_SPECIFIER_SOFT = 0x1995
-ALC_HRTF_DISABLED_SOFT = 0x0000
-ALC_HRTF_ENABLED_SOFT = 0x0001
-ALC_HRTF_DENIED_SOFT = 0x0002
-ALC_HRTF_REQUIRED_SOFT = 0x0003
-ALC_HRTF_HEADPHONES_DETECTED_SOFT = 0x0004
-ALC_HRTF_UNSUPPORTED_FORMAT_SOFT = 0x0005
-
-ALCboolean = ctypes.c_char
-ALCchar = ctypes.c_char
-ALCbyte = ctypes.c_char
-ALCubyte = ctypes.c_ubyte
-ALCshort = ctypes.c_short
-ALCushort = ctypes.c_ushort
-ALCint = ctypes.c_int
-ALCuint = ctypes.c_uint
-ALCsizei = ctypes.c_int
-ALCenum = ctypes.c_int
-ALCfloat = ctypes.c_float
-ALCdouble = ctypes.c_double
-ALCfloatArray = ctypes.c_float * 100000
-ALCLong = ctypes.c_long
-ALCvoid = None
-
-
-class ALCdevice(ctypes.Structure):
-    """A OpenAL device used for audio operations."""
-    pass
-
-
-class ALCcontext(ctypes.Structure):
-    """An execution context on a OpenAL device."""
-    pass
-
-class ALCCapabilities(ctypes.Structure):
-    pass
-
-alcCreateContext = _bind("alcCreateContext", [ctypes.POINTER(ALCdevice),
-                                              ctypes.POINTER(ALCint * 7)],
-                         ctypes.POINTER(ALCcontext))
-alcMakeContextCurrent = _bind("alcMakeContextCurrent",
-                              [ctypes.POINTER(ALCcontext)], ALCboolean)
-alcProcessContext = _bind("alcProcessContext", [ctypes.POINTER(ALCcontext)])
-alcSuspendContext = _bind("alcSuspendContext", [ctypes.POINTER(ALCcontext)])
-alcDestroyContext = _bind("alcDestroyContext", [ctypes.POINTER(ALCcontext)])
-alcGetCurrentContext = _bind("alcGetCurrentContext", None,
-                             ctypes.POINTER(ALCcontext))
-alcGetContextsDevice = _bind("alcGetContextsDevice",
-                             [ctypes.POINTER(ALCcontext)],
-                             ctypes.POINTER(ALCdevice))
-alcOpenDevice = _bind("alcOpenDevice", [ctypes.POINTER(ALCchar)],
-                      ctypes.POINTER(ALCdevice))
-alcCloseDevice = _bind("alcCloseDevice", [ctypes.POINTER(ALCdevice)],
-                       ALCboolean)
-alcGetError = _bind("alcGetError", [ctypes.POINTER(ALCdevice)], ALCenum)
-alcIsExtensionPresent = _bind("alcIsExtensionPresent",
-                              [ctypes.POINTER(ALCdevice),
-                               ctypes.POINTER(ALCchar)])
-alcGetProcAddress = _bind("alcGetProcAddress", [ctypes.POINTER(ALCdevice),
-                                                ctypes.POINTER(ALCchar)],
-                          ctypes.c_void_p)
-alcGetEnumValue = _bind("alcGetEnumValue", [ctypes.POINTER(ALCdevice),
-                                            ctypes.POINTER(ALCchar)], ALCenum)
-alcGetString = _bind("alcGetString", [ctypes.POINTER(ALCdevice), ALCenum],
-                     ctypes.POINTER(ALCchar))
-alcGetIntegerv = _bind("alcGetIntegerv", [ctypes.POINTER(ALCdevice),
-                                          ALCenum, ALCsizei,
-                                          ctypes.POINTER(ALCint)])
-alcCaptureOpenDevice = _bind("alcCaptureOpenDevice",
-                             [ctypes.POINTER(ALCchar), ALCuint, ALCenum,
-                              ALCsizei], ctypes.POINTER(ALCdevice))
-alcCaptureCloseDevice = _bind("alcCaptureCloseDevice",
-                              [ctypes.POINTER(ALCdevice)])
-alcCaptureStart = _bind("alcCaptureStart", [ctypes.POINTER(ALCdevice)])
-alcCaptureStop = _bind("alcCaptureStop", [ctypes.POINTER(ALCdevice)])
-alcCaptureSamples = _bind("alcCaptureSamples", [ctypes.POINTER(ALCdevice),
-                                                ctypes.POINTER(ALCvoid),
-                                                ALCsizei])
+import ctypes
+
+from . import dll
+
+__all__ = ["ALC_FALSE", "ALC_TRUE", "ALC_INVALID", "ALC_FREQUENCY",
+           "ALC_REFRESH", "ALC_SYNC", "ALC_MONO_SOURCES", "ALC_STEREO_SOURCES",
+           "ALC_NO_ERROR", "ALC_INVALID_DEVICE", "ALC_INVALID_CONTEXT",
+           "ALC_INVALID_ENUM", "ALC_INVALID_VALUE", "ALC_OUT_OF_MEMORY",
+           "ALC_DEFAULT_DEVICE_SPECIFIER", "ALC_DEVICE_SPECIFIER",
+           "ALC_EXTENSIONS", "ALC_MAJOR_VERSION", "ALC_MINOR_VERSION",
+           "ALC_ATTRIBUTES_SIZE", "ALC_ALL_ATTRIBUTES",
+           "ALC_DEFAULT_ALL_DEVICES_SPECIFIER", "ALC_ALL_DEVICES_SPECIFIER",
+           "ALC_CAPTURE_DEVICE_SPECIFIER",
+           "ALC_CAPTURE_DEFAULT_DEVICE_SPECIFIER", "ALC_CAPTURE_SAMPLES",
+           "ALC_HRTF_SOFT", "ALC_HRTF_ID_SOFT", "ALC_DONT_CARE_SOFT",
+           "ALC_HRTF_STATUS_SOFT", "ALC_NUM_HRTF_SPECIFIERS_SOFT",
+           "ALC_HRTF_SPECIFIER_SOFT", "ALC_HRTF_DISABLED_SOFT",
+           "ALC_HRTF_ENABLED_SOFT", "ALC_HRTF_DENIED_SOFT",
+           "ALC_HRTF_REQUIRED_SOFT", "ALC_HRTF_HEADPHONES_DETECTED_SOFT",
+           "ALC_HRTF_UNSUPPORTED_FORMAT_SOFT",
+           "ALCboolean", "ALCchar", "ALCbyte", "ALCubyte", "ALCshort",
+           "ALCushort", "ALCint", "ALCuint", "ALCsizei", "ALCenum", "ALCfloat",
+           "ALCdouble", "ALCvoid", "ALCdevice", "ALCcontext",
+           "alcCreateContext", "alcMakeContextCurrent", "alcProcessContext",
+           "alcSuspendContext", "alcDestroyContext", "alcGetCurrentContext",
+           "alcGetContextsDevice", "alcOpenDevice", "alcCloseDevice",
+           "alcGetError", "alcIsExtensionPresent", "alcGetProcAddress",
+           "alcGetEnumValue", "alcGetString", "alcGetIntegerv",
+           "alcCaptureOpenDevice", "alcCaptureCloseDevice", "alcCaptureStart",
+           "alcCaptureStop", "alcCaptureSamples",
+           ]
+
+_bind = dll.bind_function
+
+ALC_INVALID = 0
+ALC_FALSE = 0
+ALC_TRUE = 1
+
+ALC_FREQUENCY = 0x1007
+ALC_REFRESH = 0x1008
+ALC_SYNC = 0x1009
+
+ALC_MONO_SOURCES = 0x1010
+ALC_STEREO_SOURCES = 0x1011
+
+ALC_NO_ERROR = ALC_FALSE
+ALC_INVALID_DEVICE = 0xA001
+ALC_INVALID_CONTEXT = 0xA002
+ALC_INVALID_ENUM = 0xA003
+ALC_INVALID_VALUE = 0xA004
+ALC_OUT_OF_MEMORY = 0xA005
+
+ALC_DEFAULT_DEVICE_SPECIFIER = 0x1004
+ALC_DEVICE_SPECIFIER = 0x1005
+ALC_EXTENSIONS = 0x1006
+
+ALC_MAJOR_VERSION = 0x1000
+ALC_MINOR_VERSION = 0x1001
+
+ALC_ATTRIBUTES_SIZE = 0x1002
+ALC_ALL_ATTRIBUTES = 0x1003
+
+ALC_DEFAULT_ALL_DEVICES_SPECIFIER = 0x1012
+ALC_ALL_DEVICES_SPECIFIER = 0x1013
+
+ALC_CAPTURE_DEVICE_SPECIFIER = 0x310
+ALC_CAPTURE_DEFAULT_DEVICE_SPECIFIER = 0x311
+ALC_CAPTURE_SAMPLES = 0x312
+
+ALC_HRTF_SOFT = 0x1992
+ALC_HRTF_ID_SOFT = 0x1996
+ALC_DONT_CARE_SOFT = 0x002
+ALC_HRTF_STATUS_SOFT = 0x1993
+ALC_NUM_HRTF_SPECIFIERS_SOFT = 0x1994
+ALC_HRTF_SPECIFIER_SOFT = 0x1995
+ALC_HRTF_DISABLED_SOFT = 0x0000
+ALC_HRTF_ENABLED_SOFT = 0x0001
+ALC_HRTF_DENIED_SOFT = 0x0002
+ALC_HRTF_REQUIRED_SOFT = 0x0003
+ALC_HRTF_HEADPHONES_DETECTED_SOFT = 0x0004
+ALC_HRTF_UNSUPPORTED_FORMAT_SOFT = 0x0005
+
+ALCboolean = ctypes.c_char
+ALCchar = ctypes.c_char
+ALCbyte = ctypes.c_char
+ALCubyte = ctypes.c_ubyte
+ALCshort = ctypes.c_short
+ALCushort = ctypes.c_ushort
+ALCint = ctypes.c_int
+ALCuint = ctypes.c_uint
+ALCsizei = ctypes.c_int
+ALCenum = ctypes.c_int
+ALCfloat = ctypes.c_float
+ALCdouble = ctypes.c_double
+ALCfloatArray = ctypes.c_float * 100000
+ALCLong = ctypes.c_long
+ALCvoid = None
+
+
+class ALCdevice(ctypes.Structure):
+    """A OpenAL device used for audio operations."""
+    pass
+
+
+class ALCcontext(ctypes.Structure):
+    """An execution context on a OpenAL device."""
+    pass
+
+class ALCCapabilities(ctypes.Structure):
+    pass
+
+alcCreateContext = _bind("alcCreateContext", [ctypes.POINTER(ALCdevice),
+                                              ctypes.POINTER(ALCint * 7)],
+                         ctypes.POINTER(ALCcontext))
+alcMakeContextCurrent = _bind("alcMakeContextCurrent",
+                              [ctypes.POINTER(ALCcontext)], ALCboolean)
+alcProcessContext = _bind("alcProcessContext", [ctypes.POINTER(ALCcontext)])
+alcSuspendContext = _bind("alcSuspendContext", [ctypes.POINTER(ALCcontext)])
+alcDestroyContext = _bind("alcDestroyContext", [ctypes.POINTER(ALCcontext)])
+alcGetCurrentContext = _bind("alcGetCurrentContext", None,
+                             ctypes.POINTER(ALCcontext))
+alcGetContextsDevice = _bind("alcGetContextsDevice",
+                             [ctypes.POINTER(ALCcontext)],
+                             ctypes.POINTER(ALCdevice))
+alcOpenDevice = _bind("alcOpenDevice", [ctypes.POINTER(ALCchar)],
+                      ctypes.POINTER(ALCdevice))
+alcCloseDevice = _bind("alcCloseDevice", [ctypes.POINTER(ALCdevice)],
+                       ALCboolean)
+alcGetError = _bind("alcGetError", [ctypes.POINTER(ALCdevice)], ALCenum)
+alcIsExtensionPresent = _bind("alcIsExtensionPresent",
+                              [ctypes.POINTER(ALCdevice),
+                               ctypes.POINTER(ALCchar)])
+alcGetProcAddress = _bind("alcGetProcAddress", [ctypes.POINTER(ALCdevice),
+                                                ctypes.POINTER(ALCchar)],
+                          ctypes.c_void_p)
+alcGetEnumValue = _bind("alcGetEnumValue", [ctypes.POINTER(ALCdevice),
+                                            ctypes.POINTER(ALCchar)], ALCenum)
+alcGetString = _bind("alcGetString", [ctypes.POINTER(ALCdevice), ALCenum],
+                     ctypes.POINTER(ALCchar))
+alcGetIntegerv = _bind("alcGetIntegerv", [ctypes.POINTER(ALCdevice),
+                                          ALCenum, ALCsizei,
+                                          ctypes.POINTER(ALCint)])
+alcCaptureOpenDevice = _bind("alcCaptureOpenDevice",
+                             [ctypes.POINTER(ALCchar), ALCuint, ALCenum,
+                              ALCsizei], ctypes.POINTER(ALCdevice))
+alcCaptureCloseDevice = _bind("alcCaptureCloseDevice",
+                              [ctypes.POINTER(ALCdevice)])
+alcCaptureStart = _bind("alcCaptureStart", [ctypes.POINTER(ALCdevice)])
+alcCaptureStop = _bind("alcCaptureStop", [ctypes.POINTER(ALCdevice)])
+alcCaptureSamples = _bind("alcCaptureSamples", [ctypes.POINTER(ALCdevice),
+                                                ctypes.POINTER(ALCvoid),
+                                                ALCsizei])
```

### Comparing `fighting_sound-0.2/src/pyftg_sound/sound_manager.py` & `fighting_sound-0.3/src/pyftg_sound/sound_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,139 +1,153 @@
-from pathlib import Path
-from typing import Dict, List
-
-import numpy as np
-
-from pyftg_sound.models.audio_buffer import AudioBuffer
-from pyftg_sound.models.audio_source import AudioSource
-from pyftg_sound.models.sound_renderer import SoundRenderer
-from pyftg_sound.openal import al
-from pyftg_sound.utils.openal import set_source_attribute
-
-
-class SoundManager:
-    sound_renderers: List[SoundRenderer] = []
-    audio_sources: List[AudioSource] = []
-    audio_buffers: List[AudioBuffer] = []
-    sound_buffers: Dict[str, AudioBuffer] = {}
-    virtual_renderer: SoundRenderer = None
-
-    def __init__(self) -> None:
-        pass
-
-    def set_default_renderer(self, sound_renderer: SoundRenderer) -> None:
-        self.sound_renderers.append(sound_renderer)
-
-    def set_virtual_renderer(self, virtual_renderer: SoundRenderer) -> None:
-        self.virtual_renderer = virtual_renderer
-        self.sound_renderers.append(virtual_renderer)
-
-    def set_listener_position(self, x: float, y: float, z: float) -> None:
-        listener_pos = [x, y, z]
-        for sound_renderer in self.sound_renderers:
-            sound_renderer.al_listener_fv(al.AL_POSITION, listener_pos)
-
-    def set_listener_velocity(self, x: float, y: float, z: float) -> None:
-        listener_vel = [x, y, z]
-        for sound_renderer in self.sound_renderers:
-            sound_renderer.al_listener_fv(al.AL_VELOCITY, listener_vel)
-
-    def set_listener_orientation(self, x: float, y: float, z: float, x_up: float, y_up: float, z_up: float) -> None:
-        listener_ori = [x, y, z, x_up, y_up, z_up]
-        for sound_renderer in self.sound_renderers:
-            sound_renderer.al_listener_fv(al.AL_ORIENTATION, listener_ori)
-    
-    def create_audio_source(self, attrs: dict = {}) -> AudioSource:
-        contexts = [sound_renderer.context for sound_renderer in self.sound_renderers]
-        source_ids = [0] * len(self.sound_renderers)
-        for i, sound_renderer in enumerate(self.sound_renderers):
-            source_ids[i] = sound_renderer.create_source(attrs)
-        audio_source = AudioSource(contexts, source_ids)
-        self.audio_sources.append(audio_source)
-        return audio_source
-
-    def create_audio_buffer(self, file_path: Path = None) -> AudioBuffer:
-        contexts = [sound_renderer.context for sound_renderer in self.sound_renderers]
-        buffer_ids = [0] * len(self.sound_renderers)
-        for i, sound_renderer in enumerate(self.sound_renderers):
-            buffer_ids[i] = sound_renderer.create_buffer()
-        audio_buffer = AudioBuffer(contexts, buffer_ids)
-        if file_path is not None:
-            audio_buffer.register_sound(file_path)
-            self.sound_buffers[file_path.name] = audio_buffer
-        self.audio_buffers.append(audio_buffer)
-        return audio_buffer
-
-    def is_playing(self, source: AudioSource) -> bool:
-        ans = False
-        for i, sound_renderer in enumerate(self.sound_renderers):
-            source_id = source.get_source_ids()[i]
-            ans = ans or sound_renderer.is_playing(source_id)
-        return ans
-    
-    def play(self, source: AudioSource, buffer: AudioBuffer, x: float, y: float, loop: bool) -> None:
-        self.play3d(source, buffer, x, 0, y, loop)
-
-    def play3d(self, source: AudioSource, buffer: AudioBuffer, x: float, y: float, z: float, loop: bool) -> None:
-        for i, sound_renderer in enumerate(self.sound_renderers):
-            source_id = source.get_source_ids()[i]
-            buffer_id = buffer.get_buffers()[i]
-            sound_renderer.play2(source_id, buffer_id, x, y, z, loop)
-
-    def stop(self, source: AudioSource) -> None:
-        for i, sound_renderer in enumerate(self.sound_renderers):
-            source_id = source.get_source_ids()[i]
-            sound_renderer.stop(source_id)
-
-    def set_source_pos(self, source: AudioSource, x: float, y: float) -> None:
-        self.set_source_pos3d(source, x, 0, y)
-
-    def set_source_pos3d(self, source: AudioSource, x: float, y: float, z: float) -> None:
-        for i, sound_renderer in enumerate(self.sound_renderers):
-            source_id = source.get_source_ids()[i]
-            set_source_attribute(source_id, al.AL_POSITION, [x, y, z], context=sound_renderer.context)
-
-    def set_source_gain(self, source: AudioSource, gain: float) -> None:
-        for i, sound_renderer in enumerate(self.sound_renderers):
-            source_id = source.get_source_ids()[i]
-            set_source_attribute(source_id, al.AL_GAIN, gain, context=sound_renderer.context)
-
-    def set_source_pitch(self, source: AudioSource, pitch: float) -> None:
-        for i, sound_renderer in enumerate(self.sound_renderers):
-            source_id = source.get_source_ids()[i]
-            set_source_attribute(source_id, al.AL_PITCH, pitch, context=sound_renderer.context)
-
-    def get_sound_buffer(self, sound_name: str) -> AudioBuffer:
-        return self.sound_buffers.get(sound_name)
-
-    def sample_audio(self, dtype: type = al.ALfloat, render_size: int = 800, nchannels: int = 2) -> np.ndarray:
-        if not self.virtual_renderer:
-            raise ValueError("Virtual renderer not set")
-        return self.virtual_renderer.sample_audio(dtype, render_size, nchannels)
-    
-    def remove_source(self, source: AudioSource) -> None:
-        for i, sound_renderer in enumerate(self.sound_renderers):
-            source_id = source.get_source_ids()[i]
-            sound_renderer.delete_source(source_id)
-        self.audio_sources.remove(source)
-
-    def playback(self, source: AudioSource, format: int, audio_sample: bytes, sample_rate: int) -> None:
-        for i, sound_renderer in enumerate(self.sound_renderers):
-            source_id = source.get_source_ids()[i]
-            sound_renderer.playback(source_id, format, audio_sample, sample_rate)
-
-    def stop_playback(self, source: AudioSource) -> None:
-        for i, sound_renderer in enumerate(self.sound_renderers):
-            source_id = source.get_source_ids()[i]
-            sound_renderer.stop_playback(source_id)
-
-    def stop_all(self) -> None:
-        for audio_source in self.audio_sources:
-            self.stop(audio_source)
-
-    def close(self) -> None:
-        for i, sound_renderer in enumerate(self.sound_renderers):
-            for audio_buffer in self.audio_buffers:
-                sound_renderer.delete_buffer(audio_buffer.get_buffers()[i])
-            for audio_source in self.audio_sources:
-                sound_renderer.delete_source(audio_source.get_source_ids()[i])
-            sound_renderer.close()
+from pathlib import Path
+from typing import Dict, List
+
+import numpy as np
+
+from pyftg_sound.models.audio_buffer import AudioBuffer
+from pyftg_sound.models.audio_source import AudioSource
+from pyftg_sound.models.sound_renderer import SoundRenderer
+from pyftg_sound.openal import al
+from pyftg_sound.utils.openal import set_source_attribute
+
+
+class SoundManager:
+    sound_renderers: List[SoundRenderer] = []
+    audio_sources: List[AudioSource] = []
+    audio_buffers: List[AudioBuffer] = []
+    sound_buffers: Dict[str, AudioBuffer] = {}
+    virtual_renderer: SoundRenderer = None
+    default_renderer: SoundRenderer = None
+    virtual_renderer_index:int
+    default_renderer_index:int
+
+    def __init__(self) -> None:
+        pass
+
+    def set_default_renderer(self, sound_renderer: SoundRenderer) -> None:
+        self.default_renderer = sound_renderer
+        self.default_renderer_index = len(self.sound_renderers)
+        self.sound_renderers.append(sound_renderer)
+
+    def set_virtual_renderer(self, virtual_renderer: SoundRenderer) -> None:
+        self.virtual_renderer = virtual_renderer
+        self.virtual_renderer_index = len(self.sound_renderers)
+        self.sound_renderers.append(virtual_renderer)
+
+    def set_listener_position(self, x: float, y: float, z: float) -> None:
+        listener_pos = [x, y, z]
+        for sound_renderer in self.sound_renderers:
+            sound_renderer.al_listener_fv(al.AL_POSITION, listener_pos)
+
+    def set_listener_velocity(self, x: float, y: float, z: float) -> None:
+        listener_vel = [x, y, z]
+        for sound_renderer in self.sound_renderers:
+            sound_renderer.al_listener_fv(al.AL_VELOCITY, listener_vel)
+
+    def set_listener_orientation(self, x: float, y: float, z: float, x_up: float, y_up: float, z_up: float) -> None:
+        listener_ori = [x, y, z, x_up, y_up, z_up]
+        for sound_renderer in self.sound_renderers:
+            sound_renderer.al_listener_fv(al.AL_ORIENTATION, listener_ori)
+    
+    def create_audio_source(self, attrs: dict = {}) -> AudioSource:
+        contexts = [sound_renderer.context for sound_renderer in self.sound_renderers]
+        source_ids = [0] * len(self.sound_renderers)
+        for i, sound_renderer in enumerate(self.sound_renderers):
+            source_ids[i] = sound_renderer.create_source(attrs)
+        audio_source = AudioSource(contexts, source_ids)
+        self.audio_sources.append(audio_source)
+        return audio_source
+
+    def create_audio_buffer(self, file_path: Path = None) -> AudioBuffer:
+        contexts = [sound_renderer.context for sound_renderer in self.sound_renderers]
+        buffer_ids = [0] * len(self.sound_renderers)
+        for i, sound_renderer in enumerate(self.sound_renderers):
+            buffer_ids[i] = sound_renderer.create_buffer()
+        audio_buffer = AudioBuffer(contexts, buffer_ids)
+        if file_path is not None:
+            audio_buffer.register_sound(file_path)
+            self.sound_buffers[file_path.name] = audio_buffer
+        self.audio_buffers.append(audio_buffer)
+        return audio_buffer
+
+    def is_playing(self, source: AudioSource) -> bool:
+        ans = False
+        for i, sound_renderer in enumerate(self.sound_renderers):
+            source_id = source.get_source_ids()[i]
+            ans = ans or sound_renderer.is_playing(source_id)
+        return ans
+    
+    def play(self, source: AudioSource, buffer: AudioBuffer, x: float, y: float, loop: bool) -> None:
+        self.play3d(source, buffer, x, 0, y, loop)
+
+    def play_default_render(self, source: AudioSource, buffer: AudioBuffer, x: float, y: float, loop: bool) -> None:
+        if self.default_renderer:
+            i = self.default_renderer_index
+            source_id = source.get_source_ids()[i]
+            buffer_id = buffer.get_buffers()[i]
+            # fixme
+            self.default_renderer.play2(source_id, buffer_id, x, 0, y, loop)
+
+    def play3d(self, source: AudioSource, buffer: AudioBuffer, x: float, y: float, z: float, loop: bool) -> None:
+        for i, sound_renderer in enumerate(self.sound_renderers):
+            source_id = source.get_source_ids()[i]
+            buffer_id = buffer.get_buffers()[i]
+            sound_renderer.play2(source_id, buffer_id, x, y, z, loop)
+
+    def stop(self, source: AudioSource) -> None:
+        for i, sound_renderer in enumerate(self.sound_renderers):
+            source_id = source.get_source_ids()[i]
+            sound_renderer.stop(source_id)
+
+    def set_source_pos(self, source: AudioSource, x: float, y: float) -> None:
+        self.set_source_pos3d(source, x, 0, y)
+
+    def set_source_pos3d(self, source: AudioSource, x: float, y: float, z: float) -> None:
+        for i, sound_renderer in enumerate(self.sound_renderers):
+            source_id = source.get_source_ids()[i]
+            set_source_attribute(source_id, al.AL_POSITION, [x, y, z], context=sound_renderer.context)
+
+    def set_source_gain(self, source: AudioSource, gain: float) -> None:
+        for i, sound_renderer in enumerate(self.sound_renderers):
+            source_id = source.get_source_ids()[i]
+            set_source_attribute(source_id, al.AL_GAIN, gain, context=sound_renderer.context)
+
+    def set_source_pitch(self, source: AudioSource, pitch: float) -> None:
+        for i, sound_renderer in enumerate(self.sound_renderers):
+            source_id = source.get_source_ids()[i]
+            set_source_attribute(source_id, al.AL_PITCH, pitch, context=sound_renderer.context)
+
+    def get_sound_buffer(self, sound_name: str) -> AudioBuffer:
+        return self.sound_buffers.get(sound_name)
+
+    def sample_audio(self, dtype: type = al.ALfloat, render_size: int = 800, nchannels: int = 2) -> np.ndarray:
+        if not self.virtual_renderer:
+            raise ValueError("Virtual renderer not set")
+        return self.virtual_renderer.sample_audio(dtype, render_size, nchannels)
+    
+    def remove_source(self, source: AudioSource) -> None:
+        for i, sound_renderer in enumerate(self.sound_renderers):
+            source_id = source.get_source_ids()[i]
+            sound_renderer.delete_source(source_id)
+        self.audio_sources.remove(source)
+
+    def playback(self, source: AudioSource, format: int, audio_sample: bytes, sample_rate: int) -> None:
+        for i, sound_renderer in enumerate(self.sound_renderers):
+            source_id = source.get_source_ids()[i]
+            sound_renderer.playback(source_id, format, audio_sample, sample_rate)
+
+    def stop_playback(self, source: AudioSource) -> None:
+        for i, sound_renderer in enumerate(self.sound_renderers):
+            source_id = source.get_source_ids()[i]
+            sound_renderer.stop_playback(source_id)
+
+    def stop_all(self) -> None:
+        for audio_source in self.audio_sources:
+            self.stop(audio_source)
+
+    def close(self) -> None:
+        for i, sound_renderer in enumerate(self.sound_renderers):
+            for audio_buffer in self.audio_buffers:
+                sound_renderer.delete_buffer(audio_buffer.get_buffers()[i])
+            for audio_source in self.audio_sources:
+                sound_renderer.delete_source(audio_source.get_source_ids()[i])
+            sound_renderer.close()
```

### Comparing `fighting_sound-0.2/src/pyftg_sound/utils/openal.py` & `fighting_sound-0.3/src/pyftg_sound/utils/openal.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from typing import Any, List
-
-from pyftg_sound.openal import al, alc
-
-
-def set_source_list_attribute(source_id: int, attr: int, values: List):
-    if all(isinstance(item, int) for item in values):
-        func = al.alSource3i if len(values) == 3 else al.alSourceiv
-        value_arr = (al.ALint * len(values))(*values)
-        func(source_id, attr, *value_arr if len(values) == 3 else value_arr)
-    elif all(isinstance(item, float) for item in values):
-        func = al.alSource3f if len(values) == 3 else al.alSourcefv
-        value_arr = (al.ALfloat * len(values))(*values)
-        func(source_id, attr, *value_arr if len(values) == 3 else value_arr)
-    else:
-        raise ValueError("List should contain either all integers or all floats")
-
-
-def set_source_attribute(source_id: int, attr: int, value: Any, context: alc.ALCcontext = None) -> None:
-    if context:
-        alc.alcMakeContextCurrent(context)
-    
-    if isinstance(value, int):
-        al.alSourcei(source_id, attr, value)
-    elif isinstance(value, float):
-        al.alSourcef(source_id, attr, value)
-    elif isinstance(value, list):
-        set_source_list_attribute(source_id, attr, value)
-    else:
-        raise ValueError(f"Invalid value type: {type(value)}")
+from typing import Any, List
+
+from pyftg_sound.openal import al, alc
+
+
+def set_source_list_attribute(source_id: int, attr: int, values: List):
+    if all(isinstance(item, int) for item in values):
+        func = al.alSource3i if len(values) == 3 else al.alSourceiv
+        value_arr = (al.ALint * len(values))(*values)
+        func(source_id, attr, *value_arr if len(values) == 3 else value_arr)
+    elif all(isinstance(item, float) for item in values):
+        func = al.alSource3f if len(values) == 3 else al.alSourcefv
+        value_arr = (al.ALfloat * len(values))(*values)
+        func(source_id, attr, *value_arr if len(values) == 3 else value_arr)
+    else:
+        raise ValueError("List should contain either all integers or all floats")
+
+
+def set_source_attribute(source_id: int, attr: int, value: Any, context: alc.ALCcontext = None) -> None:
+    if context:
+        alc.alcMakeContextCurrent(context)
+    
+    if isinstance(value, int):
+        al.alSourcei(source_id, attr, value)
+    elif isinstance(value, float):
+        al.alSourcef(source_id, attr, value)
+    elif isinstance(value, list):
+        set_source_list_attribute(source_id, attr, value)
+    else:
+        raise ValueError(f"Invalid value type: {type(value)}")
```

### Comparing `fighting_sound-0.2/src/pyftg_sound/utils/wave.py` & `fighting_sound-0.3/src/pyftg_sound/utils/wave.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import wave
-from pathlib import Path
-from typing import Tuple
-
-from pyftg_sound.openal import al
-
-formatmap = {
-    (1, 8) : al.AL_FORMAT_MONO8,
-    (2, 8) : al.AL_FORMAT_STEREO8,
-    (1, 16): al.AL_FORMAT_MONO16,
-    (2, 16) : al.AL_FORMAT_STEREO16,
-}
-
-
-def load_sound(file_path: Path) -> Tuple[int, bytes, int]:
-    with wave.open(str(file_path), 'rb') as wavefp:
-        channels = wavefp.getnchannels()
-        bitrate = wavefp.getsampwidth() * 8
-        samplerate = wavefp.getframerate()
-        wavbuf = wavefp.readframes(wavefp.getnframes())
-        alformat = formatmap[(channels, bitrate)]
-    return alformat, wavbuf, samplerate
+import wave
+from pathlib import Path
+from typing import Tuple
+
+from pyftg_sound.openal import al
+
+formatmap = {
+    (1, 8) : al.AL_FORMAT_MONO8,
+    (2, 8) : al.AL_FORMAT_STEREO8,
+    (1, 16): al.AL_FORMAT_MONO16,
+    (2, 16) : al.AL_FORMAT_STEREO16,
+}
+
+
+def load_sound(file_path: Path) -> Tuple[int, bytes, int]:
+    with wave.open(str(file_path), 'rb') as wavefp:
+        channels = wavefp.getnchannels()
+        bitrate = wavefp.getsampwidth() * 8
+        samplerate = wavefp.getframerate()
+        wavbuf = wavefp.readframes(wavefp.getnframes())
+        alformat = formatmap[(channels, bitrate)]
+    return alformat, wavbuf, samplerate
```

