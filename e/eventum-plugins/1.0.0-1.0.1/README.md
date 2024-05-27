# Comparing `tmp/eventum_plugins-1.0.0.tar.gz` & `tmp/eventum_plugins-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventum_plugins-1.0.0.tar", max compression
+gzip compressed data, was "eventum_plugins-1.0.1.tar", max compression
```

## Comparing `eventum_plugins-1.0.0.tar` & `eventum_plugins-1.0.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0    11357 2024-05-21 17:41:05.247172 eventum_plugins-1.0.0/LICENSE
--rw-r--r--   0        0        0       37 2024-05-21 17:41:05.247172 eventum_plugins-1.0.0/README.md
--rw-r--r--   0        0        0        0 2024-05-21 17:54:41.546979 eventum_plugins-1.0.0/eventum_plugins/__init__.py
--rw-r--r--   0        0        0        0 2024-05-25 11:40:55.321933 eventum_plugins-1.0.0/eventum_plugins/event/__init__.py
--rw-r--r--   0        0        0      722 2024-05-25 13:00:17.860819 eventum_plugins-1.0.0/eventum_plugins/event/base.py
--rw-r--r--   0        0        0    11216 2024-05-26 11:50:22.309370 eventum_plugins-1.0.0/eventum_plugins/event/jinja.py
--rw-r--r--   0        0        0        0 2024-05-25 13:52:48.830090 eventum_plugins-1.0.0/eventum_plugins/event/jinja_modules/__init__.py
--rw-r--r--   0        0        0     5656 2024-05-25 11:40:55.301933 eventum_plugins-1.0.0/eventum_plugins/event/jinja_modules/rand.py
--rw-r--r--   0        0        0       29 2024-05-26 11:41:50.809487 eventum_plugins-1.0.0/eventum_plugins/event/tests/static/sample.csv
--rw-r--r--   0        0        0     3316 2024-05-26 11:50:22.309370 eventum_plugins-1.0.0/eventum_plugins/event/tests/test_jinja.py
--rw-r--r--   0        0        0        0 2024-05-25 11:40:23.651940 eventum_plugins-1.0.0/eventum_plugins/input/__init__.py
--rw-r--r--   0        0        0     2095 2024-05-25 15:37:58.068606 eventum_plugins-1.0.0/eventum_plugins/input/base.py
--rw-r--r--   0        0        0     1552 2024-05-25 15:26:31.658758 eventum_plugins-1.0.0/eventum_plugins/input/cron.py
--rw-r--r--   0        0        0     1680 2024-05-24 18:11:30.781755 eventum_plugins-1.0.0/eventum_plugins/input/linspace.py
--rw-r--r--   0        0        0     1127 2024-05-24 18:11:30.781755 eventum_plugins-1.0.0/eventum_plugins/input/sample.py
--rw-r--r--   0        0        0      116 2024-05-26 07:54:34.102677 eventum_plugins-1.0.0/eventum_plugins/input/tests/static/time_pattern_invalid.yml
--rw-r--r--   0        0        0      227 2024-05-26 11:27:33.109687 eventum_plugins-1.0.0/eventum_plugins/input/tests/static/time_pattern_valid.yml
--rw-r--r--   0        0        0     1383 2024-05-26 09:03:08.741710 eventum_plugins-1.0.0/eventum_plugins/input/tests/test_cron.py
--rw-r--r--   0        0        0     2062 2024-05-25 16:56:57.927494 eventum_plugins-1.0.0/eventum_plugins/input/tests/test_linspace.py
--rw-r--r--   0        0        0      814 2024-05-25 17:03:09.517408 eventum_plugins-1.0.0/eventum_plugins/input/tests/test_sample.py
--rw-r--r--   0        0        0     1902 2024-05-26 11:29:21.659661 eventum_plugins-1.0.0/eventum_plugins/input/tests/test_time_patterns.py
--rw-r--r--   0        0        0      843 2024-05-26 07:18:51.813193 eventum_plugins-1.0.0/eventum_plugins/input/tests/test_timer.py
--rw-r--r--   0        0        0     2039 2024-05-26 09:37:42.431227 eventum_plugins-1.0.0/eventum_plugins/input/tests/test_timestamps.py
--rw-r--r--   0        0        0    18406 2024-05-26 08:11:16.792437 eventum_plugins-1.0.0/eventum_plugins/input/time_patterns.py
--rw-r--r--   0        0        0     1400 2024-05-26 07:14:57.043229 eventum_plugins-1.0.0/eventum_plugins/input/timer.py
--rw-r--r--   0        0        0     1860 2024-05-26 09:36:53.081239 eventum_plugins-1.0.0/eventum_plugins/input/timestamps.py
--rw-r--r--   0        0        0        0 2024-05-22 17:54:51.017205 eventum_plugins-1.0.0/eventum_plugins/output/__init__.py
--rw-r--r--   0        0        0     3679 2024-05-26 14:50:30.446840 eventum_plugins-1.0.0/eventum_plugins/output/base.py
--rw-r--r--   0        0        0     2618 2024-05-26 14:33:17.597076 eventum_plugins-1.0.0/eventum_plugins/output/file.py
--rw-r--r--   0        0        0     4930 2024-05-26 14:51:09.566830 eventum_plugins-1.0.0/eventum_plugins/output/opensearch.py
--rw-r--r--   0        0        0     1489 2024-05-26 14:50:57.506833 eventum_plugins-1.0.0/eventum_plugins/output/stdout.py
--rw-r--r--   0        0        0     1036 2024-05-26 13:27:44.227998 eventum_plugins-1.0.0/eventum_plugins/output/tests/test_file.py
--rw-r--r--   0        0        0     3971 2024-05-26 14:49:45.596850 eventum_plugins-1.0.0/eventum_plugins/output/tests/test_opensearch.py
--rw-r--r--   0        0        0        0 2024-05-24 16:48:46.953250 eventum_plugins-1.0.0/eventum_plugins/py.typed
--rw-r--r--   0        0        0        0 2024-05-25 11:40:43.771936 eventum_plugins-1.0.0/eventum_plugins/utils/__init__.py
--rw-r--r--   0        0        0      298 2024-05-25 14:02:03.079955 eventum_plugins-1.0.0/eventum_plugins/utils/modules.py
--rw-r--r--   0        0        0      467 2024-05-26 08:55:31.731840 eventum_plugins-1.0.0/eventum_plugins/utils/numpy_time.py
--rw-r--r--   0        0        0     1411 2024-05-24 18:11:28.351759 eventum_plugins-1.0.0/eventum_plugins/utils/relative_time.py
--rw-r--r--   0        0        0     1311 2024-05-22 17:28:13.897819 eventum_plugins-1.0.0/eventum_plugins/utils/tests/test_relative_time.py
--rw-r--r--   0        0        0      715 2024-05-26 09:36:13.411247 eventum_plugins-1.0.0/eventum_plugins/utils/tests/test_timeseries.py
--rw-r--r--   0        0        0      634 2024-05-26 09:35:32.351257 eventum_plugins-1.0.0/eventum_plugins/utils/timeseries.py
--rw-r--r--   0        0        0     1368 2024-05-26 13:10:36.008241 eventum_plugins-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1309 1970-01-01 00:00:00.000000 eventum_plugins-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-21 17:41:05.247172 eventum_plugins-1.0.1/LICENSE
+-rw-r--r--   0        0        0       37 2024-05-21 17:41:05.247172 eventum_plugins-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-21 17:54:41.546979 eventum_plugins-1.0.1/eventum_plugins/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-25 11:40:55.321933 eventum_plugins-1.0.1/eventum_plugins/event/__init__.py
+-rw-r--r--   0        0        0      722 2024-05-25 13:00:17.860819 eventum_plugins-1.0.1/eventum_plugins/event/base.py
+-rw-r--r--   0        0        0    11216 2024-05-26 11:50:22.309370 eventum_plugins-1.0.1/eventum_plugins/event/jinja.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:52:48.830090 eventum_plugins-1.0.1/eventum_plugins/event/jinja_modules/__init__.py
+-rw-r--r--   0        0        0     5656 2024-05-25 11:40:55.301933 eventum_plugins-1.0.1/eventum_plugins/event/jinja_modules/rand.py
+-rw-r--r--   0        0        0       29 2024-05-26 11:41:50.809487 eventum_plugins-1.0.1/eventum_plugins/event/tests/static/sample.csv
+-rw-r--r--   0        0        0     3316 2024-05-26 11:50:22.309370 eventum_plugins-1.0.1/eventum_plugins/event/tests/test_jinja.py
+-rw-r--r--   0        0        0        0 2024-05-25 11:40:23.651940 eventum_plugins-1.0.1/eventum_plugins/input/__init__.py
+-rw-r--r--   0        0        0     2173 2024-05-27 17:37:19.844745 eventum_plugins-1.0.1/eventum_plugins/input/base.py
+-rw-r--r--   0        0        0     1554 2024-05-27 17:28:58.074867 eventum_plugins-1.0.1/eventum_plugins/input/cron.py
+-rw-r--r--   0        0        0     1682 2024-05-27 17:29:08.314866 eventum_plugins-1.0.1/eventum_plugins/input/linspace.py
+-rw-r--r--   0        0        0     1129 2024-05-27 17:29:14.294865 eventum_plugins-1.0.1/eventum_plugins/input/sample.py
+-rw-r--r--   0        0        0      116 2024-05-26 07:54:34.102677 eventum_plugins-1.0.1/eventum_plugins/input/tests/static/time_pattern_invalid.yml
+-rw-r--r--   0        0        0      227 2024-05-26 11:27:33.109687 eventum_plugins-1.0.1/eventum_plugins/input/tests/static/time_pattern_valid.yml
+-rw-r--r--   0        0        0     1383 2024-05-26 09:03:08.741710 eventum_plugins-1.0.1/eventum_plugins/input/tests/test_cron.py
+-rw-r--r--   0        0        0     2062 2024-05-25 16:56:57.927494 eventum_plugins-1.0.1/eventum_plugins/input/tests/test_linspace.py
+-rw-r--r--   0        0        0      814 2024-05-25 17:03:09.517408 eventum_plugins-1.0.1/eventum_plugins/input/tests/test_sample.py
+-rw-r--r--   0        0        0     1902 2024-05-26 11:29:21.659661 eventum_plugins-1.0.1/eventum_plugins/input/tests/test_time_patterns.py
+-rw-r--r--   0        0        0      843 2024-05-26 07:18:51.813193 eventum_plugins-1.0.1/eventum_plugins/input/tests/test_timer.py
+-rw-r--r--   0        0        0     2039 2024-05-26 09:37:42.431227 eventum_plugins-1.0.1/eventum_plugins/input/tests/test_timestamps.py
+-rw-r--r--   0        0        0    18439 2024-05-27 17:30:13.454853 eventum_plugins-1.0.1/eventum_plugins/input/time_patterns.py
+-rw-r--r--   0        0        0     1402 2024-05-27 17:29:40.814860 eventum_plugins-1.0.1/eventum_plugins/input/timer.py
+-rw-r--r--   0        0        0     1862 2024-05-27 17:29:46.244859 eventum_plugins-1.0.1/eventum_plugins/input/timestamps.py
+-rw-r--r--   0        0        0        0 2024-05-22 17:54:51.017205 eventum_plugins-1.0.1/eventum_plugins/output/__init__.py
+-rw-r--r--   0        0        0     3915 2024-05-27 18:07:02.584332 eventum_plugins-1.0.1/eventum_plugins/output/base.py
+-rw-r--r--   0        0        0     2662 2024-05-27 18:10:13.024289 eventum_plugins-1.0.1/eventum_plugins/output/file.py
+-rw-r--r--   0        0        0     4966 2024-05-27 18:09:35.024298 eventum_plugins-1.0.1/eventum_plugins/output/opensearch.py
+-rw-r--r--   0        0        0     1525 2024-05-27 18:10:04.304291 eventum_plugins-1.0.1/eventum_plugins/output/stdout.py
+-rw-r--r--   0        0        0     1036 2024-05-26 15:11:30.906539 eventum_plugins-1.0.1/eventum_plugins/output/tests/test_file.py
+-rw-r--r--   0        0        0     3971 2024-05-26 14:49:45.596850 eventum_plugins-1.0.1/eventum_plugins/output/tests/test_opensearch.py
+-rw-r--r--   0        0        0        0 2024-05-24 16:48:46.953250 eventum_plugins-1.0.1/eventum_plugins/py.typed
+-rw-r--r--   0        0        0        0 2024-05-25 11:40:43.771936 eventum_plugins-1.0.1/eventum_plugins/utils/__init__.py
+-rw-r--r--   0        0        0      298 2024-05-25 14:02:03.079955 eventum_plugins-1.0.1/eventum_plugins/utils/modules.py
+-rw-r--r--   0        0        0      469 2024-05-27 17:29:51.864858 eventum_plugins-1.0.1/eventum_plugins/utils/numpy_time.py
+-rw-r--r--   0        0        0     1411 2024-05-24 18:11:28.351759 eventum_plugins-1.0.1/eventum_plugins/utils/relative_time.py
+-rw-r--r--   0        0        0     1311 2024-05-22 17:28:13.897819 eventum_plugins-1.0.1/eventum_plugins/utils/tests/test_relative_time.py
+-rw-r--r--   0        0        0      715 2024-05-26 09:36:13.411247 eventum_plugins-1.0.1/eventum_plugins/utils/tests/test_timeseries.py
+-rw-r--r--   0        0        0      634 2024-05-26 09:35:32.351257 eventum_plugins-1.0.1/eventum_plugins/utils/timeseries.py
+-rw-r--r--   0        0        0     1386 2024-05-27 18:10:53.894280 eventum_plugins-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1309 1970-01-01 00:00:00.000000 eventum_plugins-1.0.1/PKG-INFO
```

### Comparing `eventum_plugins-1.0.0/LICENSE` & `eventum_plugins-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.0/eventum_plugins/event/base.py` & `eventum_plugins-1.0.1/eventum_plugins/event/base.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.0/eventum_plugins/event/jinja.py` & `eventum_plugins-1.0.1/eventum_plugins/event/jinja.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.0/eventum_plugins/event/jinja_modules/rand.py` & `eventum_plugins-1.0.1/eventum_plugins/event/jinja_modules/rand.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.0/eventum_plugins/event/tests/test_jinja.py` & `eventum_plugins-1.0.1/eventum_plugins/event/tests/test_jinja.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.0/eventum_plugins/input/base.py` & `eventum_plugins-1.0.1/eventum_plugins/input/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABC, abstractmethod
-from typing import Any, Callable
+from typing import Any, Callable, TypeAlias
 
 from numpy import datetime64
 from pydantic import BaseModel
-from pytz.tzinfo import DstTzInfo
+from pytz.tzinfo import BaseTzInfo
 
 
 class InputPluginError(Exception):
     """Base exception for all input plugin errors."""
 
 
 class InputPluginConfigurationError(InputPluginError):
@@ -28,15 +28,15 @@
     """Base config model for input plugins"""
 
 
 class BaseInputPlugin(ABC):
     """Base class for all input plugins."""
 
     @abstractmethod
-    def __init__(self, config: Any, tz: DstTzInfo) -> None:
+    def __init__(self, config: Any, tz: BaseTzInfo) -> None:
         ...
 
 
 class LiveInputPlugin(BaseInputPlugin):
     """Base class for input plugins that can be used in live mode."""
 
     @abstractmethod
@@ -60,7 +60,10 @@
         current timestamp as a single parameter. The process execution
         is not tied to real time and there is no any delay between
         `on_event` calls. Therefore distribution is expected to have
         specific start and end time to generate finite sample of
         timestamps.
         """
         ...
+
+
+InputPlugin: TypeAlias = (SampleInputPlugin | LiveInputPlugin)
```

### Comparing `eventum_plugins-1.0.0/eventum_plugins/input/cron.py` & `eventum_plugins-1.0.1/eventum_plugins/input/cron.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import time
 from datetime import datetime
 from typing import Any, Callable
 
 from croniter import croniter
 from numpy import datetime64
 from pydantic import Field, field_validator
-from pytz.tzinfo import DstTzInfo
+from pytz.tzinfo import BaseTzInfo
 
 from eventum_plugins.input.base import InputPluginBaseConfig, LiveInputPlugin
 
 
 class CronInputConfig(InputPluginBaseConfig, frozen=True):
     expression: str
     count: int = Field(..., gt=0)
@@ -22,15 +22,15 @@
 
 
 class CronInputPlugin(LiveInputPlugin):
     """Input plugin for generating events at moments defined by cron
     expression.
     """
 
-    def __init__(self, config: CronInputConfig, tz: DstTzInfo) -> None:
+    def __init__(self, config: CronInputConfig, tz: BaseTzInfo) -> None:
         self._expression = config.expression
         self._count = config.count
         self._tz = tz
 
     def live(self, on_event: Callable[[datetime64], Any]) -> None:
         cron = croniter(
             expr_format=self._expression,
```

### Comparing `eventum_plugins-1.0.0/eventum_plugins/input/linspace.py` & `eventum_plugins-1.0.1/eventum_plugins/input/linspace.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime
 from typing import Any, Callable
 
 from numpy import datetime64, linspace, timedelta64
 from pydantic import Field, model_validator
-from pytz.tzinfo import DstTzInfo
+from pytz.tzinfo import BaseTzInfo
 
 from eventum_plugins.input.base import InputPluginBaseConfig, SampleInputPlugin
 
 
 class LinspaceInputConfig(InputPluginBaseConfig, frozen=True):
     start: datetime
     end: datetime
@@ -22,15 +22,15 @@
 
 
 class LinspaceInputPlugin(SampleInputPlugin):
     """Input plugin for generating specified count of events linearly
     spaced in time.
     """
 
-    def __init__(self, config: LinspaceInputConfig, tz: DstTzInfo) -> None:
+    def __init__(self, config: LinspaceInputConfig, tz: BaseTzInfo) -> None:
         self._start = config.start
         self._end = config.end
         self._count = config.count
         self._endpoint = config.endpoint
         self._tz = tz
 
     def sample(self, on_event: Callable[[datetime64], Any]) -> None:
```

### Comparing `eventum_plugins-1.0.0/eventum_plugins/input/sample.py` & `eventum_plugins-1.0.1/eventum_plugins/input/sample.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, Callable
 
 from numpy import datetime64
 from pydantic import Field
-from pytz.tzinfo import DstTzInfo
+from pytz.tzinfo import BaseTzInfo
 
 from eventum_plugins.input.base import InputPluginBaseConfig
 from eventum_plugins.input.base import \
     SampleInputPlugin as BaseSampleInputPlugin
 from eventum_plugins.utils.numpy_time import get_now
 
 
@@ -17,15 +17,15 @@
 class SampleInputPlugin(BaseSampleInputPlugin):
     """Input plugin for generating specified count of events. Use it
     when you only need to produce event facts and timestamps aren't
     important. For all events timestamps are the same and have a value
     of time when sample generating process was started.
     """
 
-    def __init__(self, config: SampleInputConfig, tz: DstTzInfo) -> None:
+    def __init__(self, config: SampleInputConfig, tz: BaseTzInfo) -> None:
         self._count = config.count
         self._tz = tz
 
     def sample(self, on_event: Callable[[datetime64], Any]) -> None:
         timestamp = get_now(tz=self._tz)
 
         for _ in range(self._count):
```

### Comparing `eventum_plugins-1.0.0/eventum_plugins/input/tests/test_cron.py` & `eventum_plugins-1.0.1/eventum_plugins/input/tests/test_cron.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.0/eventum_plugins/input/tests/test_linspace.py` & `eventum_plugins-1.0.1/eventum_plugins/input/tests/test_linspace.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.0/eventum_plugins/input/tests/test_sample.py` & `eventum_plugins-1.0.1/eventum_plugins/input/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.0/eventum_plugins/input/tests/test_time_patterns.py` & `eventum_plugins-1.0.1/eventum_plugins/input/tests/test_time_patterns.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.0/eventum_plugins/input/tests/test_timer.py` & `eventum_plugins-1.0.1/eventum_plugins/input/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.0/eventum_plugins/input/tests/test_timestamps.py` & `eventum_plugins-1.0.1/eventum_plugins/input/tests/test_timestamps.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.0/eventum_plugins/input/time_patterns.py` & `eventum_plugins-1.0.1/eventum_plugins/input/time_patterns.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import Annotated, Any, Callable, TypeAlias, assert_never
 
 import numpy as np
 from eventum_content_manager.manage import (ContentManagementError,
                                             load_time_pattern)
 from numpy.typing import NDArray
 from pydantic import AfterValidator, Field, ValidationError, model_validator
-from pytz.tzinfo import DstTzInfo
+from pytz.tzinfo import BaseTzInfo
 
 from eventum_plugins.input.base import (InputPluginBaseConfig,
                                         InputPluginConfigurationError,
                                         InputPluginRuntimeError,
                                         LiveInputPlugin, PerformanceError,
                                         SampleInputPlugin)
 from eventum_plugins.utils.numpy_time import get_now, timedelta_to_seconds
@@ -163,15 +163,15 @@
         end of live interval is reached.
         """
 
     _PERFORMANCE_TEST_SAMPLE_SIZE = 100000
     _REQUIRED_EPS_RESERVE_RATIO = 1.15
     PUBLISH_PRECISION_SECONDS = 0.01
 
-    def __init__(self, config: TimePatternConfig, tz: DstTzInfo) -> None:
+    def __init__(self, config: TimePatternConfig, tz: BaseTzInfo) -> None:
         self._config = config
         self._tz = tz
         self._randomizer_factors = self._generate_randomizer_factors()
 
     def _generate_randomizer_factors(
         self,
         size: int = 1000
@@ -459,15 +459,19 @@
 
 
 class TimePatternPoolInputPlugin(LiveInputPlugin, SampleInputPlugin):
     """Input plugin for combining multiple `TimePatternInputPlugin`
     plugins.
     """
 
-    def __init__(self, config: TimePatternsInputConfig, tz: DstTzInfo) -> None:
+    def __init__(
+        self,
+        config: TimePatternsInputConfig,
+        tz: BaseTzInfo
+    ) -> None:
         self._tz = tz
         time_patterns: list[TimePatternInputPlugin] = []
 
         for config_path in config.configs:
             try:
                 time_pattern_obj = load_time_pattern(path=config_path)
                 time_pattern = TimePatternConfig.model_validate(
```

### Comparing `eventum_plugins-1.0.0/eventum_plugins/input/timer.py` & `eventum_plugins-1.0.1/eventum_plugins/input/timer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import time
 from typing import Any, Callable
 
 from numpy import datetime64, timedelta64
 from pydantic import Field
-from pytz.tzinfo import DstTzInfo
+from pytz.tzinfo import BaseTzInfo
 
 from eventum_plugins.input.base import InputPluginBaseConfig, LiveInputPlugin
 from eventum_plugins.utils.numpy_time import get_now, timedelta_to_seconds
 
 
 class TimerInputConfig(InputPluginBaseConfig, frozen=True):
     seconds: float = Field(..., ge=0.1)
@@ -16,15 +16,15 @@
 
 
 class TimerInputPlugin(LiveInputPlugin):
     """Input plugin for generating events after specified number of
     seconds.
     """
 
-    def __init__(self, config: TimerInputConfig, tz: DstTzInfo) -> None:
+    def __init__(self, config: TimerInputConfig, tz: BaseTzInfo) -> None:
         self._seconds = config.seconds
         self._count = config.count
         self._repeat = config.repeat
         self._tz = tz
 
     def live(self, on_event: Callable[[datetime64], Any]) -> None:
         timeout = timedelta64(int(self._seconds * 1000), 'ms')
```

### Comparing `eventum_plugins-1.0.0/eventum_plugins/input/timestamps.py` & `eventum_plugins-1.0.1/eventum_plugins/input/timestamps.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import time
 from datetime import datetime
 from typing import Any, Callable
 
 from numpy import array, datetime64
 from numpy.typing import NDArray
 from pydantic import Field
-from pytz.tzinfo import DstTzInfo
+from pytz.tzinfo import BaseTzInfo
 
 from eventum_plugins.input.base import (InputPluginBaseConfig, LiveInputPlugin,
                                         SampleInputPlugin)
 from eventum_plugins.utils.numpy_time import get_now, timedelta_to_seconds
 from eventum_plugins.utils.timeseries import get_future_slice
 
 
 class TimestampsInputConfig(InputPluginBaseConfig, frozen=True):
     source: tuple[datetime, ...] = Field(..., min_length=1)
 
 
 class TimestampsInputPlugin(LiveInputPlugin, SampleInputPlugin):
     """Input plugin for generating events in specified timestamps."""
 
-    def __init__(self, config: TimestampsInputConfig, tz: DstTzInfo) -> None:
+    def __init__(self, config: TimestampsInputConfig, tz: BaseTzInfo) -> None:
         self._timestamps: NDArray[datetime64] = array(
             [
                 ts.astimezone(tz=tz).replace(tzinfo=None)
                 if ts.tzinfo else ts.replace(tzinfo=None)
                 for ts in config.source
             ],
             dtype='datetime64'
```

### Comparing `eventum_plugins-1.0.0/eventum_plugins/output/base.py` & `eventum_plugins-1.0.1/eventum_plugins/output/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,17 +33,23 @@
 class OutputFormat(StrEnum):
     ORIGINAL = 'original'
     JSON_LINES = 'json-lines'
 
 
 class BaseOutputPlugin(ABC):
     """Base class for all output plugins."""
-    def __init__(self, format: OutputFormat | None = None) -> None:
-        self._format = format
+    def __init__(self, config: Any) -> None:
         self._is_opened = False
+        self._format: OutputFormat | None = None
+
+    def _set_formatter(self, format: OutputFormat | None) -> None:
+        """Set the format to which events will be converted before
+        they are passed to `_write` and `_write_many` methods.
+        """
+        self._format = format
 
     async def __aenter__(self) -> Self:
         await self.open()
         return self
 
     async def __aexit__(
         self,
```

### Comparing `eventum_plugins-1.0.0/eventum_plugins/output/file.py` & `eventum_plugins-1.0.1/eventum_plugins/output/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,17 @@
             return v
         raise ValueError('Path must be absolute')
 
 
 class FileOutputPlugin(BaseOutputPlugin):
     """Output plugin for writing events to file."""
     def __init__(self, config: FileOutputConfig) -> None:
-        super().__init__(config.format)
+        super().__init__(config)
+        self._set_formatter(format=config.format)
+
         self._filepath = config.path
         self._flush = config.flush
 
         self._check_file_access()
 
         self._file: AsyncTextIOWrapper
```

### Comparing `eventum_plugins-1.0.0/eventum_plugins/output/opensearch.py` & `eventum_plugins-1.0.1/eventum_plugins/output/opensearch.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,16 @@
 
 class OpensearchOutputPlugin(BaseOutputPlugin):
     """Output plugin for sending events to opensearch."""
 
     def __init__(self, config: OpensearchOutputConfig) -> None:
         # Format is JSON_LINES here because we need to validate that
         # string is a valid json document that OpenSearch can index
-        super().__init__(format=OutputFormat.JSON_LINES)
+        super().__init__(config)
+        self._set_formatter(format=OutputFormat.JSON_LINES)
 
         self._hosts = config.hosts
         self._user = config.user
         self._password = config.password
         self._index = config.index
 
         self._ssl_context = ssl.create_default_context()
```

### Comparing `eventum_plugins-1.0.0/eventum_plugins/output/stdout.py` & `eventum_plugins-1.0.1/eventum_plugins/output/stdout.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,16 @@
     format: OutputFormat = OutputFormat.ORIGINAL
 
 
 class StdoutOutputPlugin(BaseOutputPlugin):
     """Output plugin for writing events to stdout."""
 
     def __init__(self, config: StdOutOutputConfig) -> None:
-        super().__init__(format=config.format)
+        super().__init__(config)
+        self._set_formatter(format=config.format)
 
         self._writer: asyncio.StreamWriter
 
     async def _open(self) -> None:
         loop = asyncio.get_event_loop()
         w_transport, w_protocol = await loop.connect_write_pipe(
             protocol_factory=asyncio.streams.FlowControlMixin,
```

### Comparing `eventum_plugins-1.0.0/eventum_plugins/output/tests/test_file.py` & `eventum_plugins-1.0.1/eventum_plugins/output/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.0/eventum_plugins/output/tests/test_opensearch.py` & `eventum_plugins-1.0.1/eventum_plugins/output/tests/test_opensearch.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.0/eventum_plugins/utils/relative_time.py` & `eventum_plugins-1.0.1/eventum_plugins/utils/relative_time.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.0/eventum_plugins/utils/tests/test_relative_time.py` & `eventum_plugins-1.0.1/eventum_plugins/utils/tests/test_relative_time.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.0/eventum_plugins/utils/tests/test_timeseries.py` & `eventum_plugins-1.0.1/eventum_plugins/utils/tests/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.0/eventum_plugins/utils/timeseries.py` & `eventum_plugins-1.0.1/eventum_plugins/utils/timeseries.py`

 * *Files identical despite different names*

### Comparing `eventum_plugins-1.0.0/pyproject.toml` & `eventum_plugins-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eventum-plugins"
-version = "1.0.0"
+version = "1.0.1"
 description = "Plugins for Eventum"
 license = "Apache-2.0"
 authors = ["Nikita Reznikov <nikita.reznikov.public@mail.ru>"]
 readme = "README.md"
 repository = "https://github.com/Eventum-Generatives/EventumPlugins"
 documentation = "https://eventum-generatives.github.io/Website/"
 keywords = ["plugin", "generator", "template", "scheduling", "time"]
@@ -38,11 +38,12 @@
 mypy = "^1.9.0"
 types-aiofiles = "^23.2.0.20240403"
 types-croniter = "^2.0.0.20240423"
 types-pytz = "^2024.1.0.20240417"
 freezegun = "^1.5.1"
 pytest-asyncio = "^0.23.7"
 aioresponses = "^0.7.6"
+flake8 = "^7.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `eventum_plugins-1.0.0/PKG-INFO` & `eventum_plugins-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventum-plugins
-Version: 1.0.0
+Version: 1.0.1
 Summary: Plugins for Eventum
 Home-page: https://github.com/Eventum-Generatives/EventumPlugins
 License: Apache-2.0
 Keywords: plugin,generator,template,scheduling,time
 Author: Nikita Reznikov
 Author-email: nikita.reznikov.public@mail.ru
 Requires-Python: >=3.11,<4.0
```

