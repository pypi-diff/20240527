# Comparing `tmp/qubx-0.1.83.tar.gz` & `tmp/qubx-0.1.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qubx-0.1.83.tar", max compression
+gzip compressed data, was "qubx-0.1.84.tar", max compression
```

## Comparing `qubx-0.1.83.tar` & `qubx-0.1.84.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      940 2024-04-25 07:51:17.473695 qubx-0.1.83/README.md
--rw-r--r--   0        0        0     9305 2024-04-21 10:35:06.164526 qubx-0.1.83/build.py
--rw-r--r--   0        0        0     1556 2024-05-22 11:57:18.794331 qubx-0.1.83/pyproject.toml
--rw-r--r--   0        0        0     5428 2024-04-21 10:35:06.176526 qubx-0.1.83/src/qubx/__init__.py
--rw-r--r--   0        0        0     1875 2024-05-12 17:27:41.499398 qubx-0.1.83/src/qubx/_nb_magic.py
--rw-r--r--   0        0        0        0 2024-02-29 14:43:31.739720 qubx-0.1.83/src/qubx/core/__init__.py
--rw-r--r--   0        0        0     6707 2024-04-25 07:51:17.477695 qubx-0.1.83/src/qubx/core/account.py
--rw-r--r--   0        0        0    14777 2024-05-07 13:17:10.565607 qubx-0.1.83/src/qubx/core/basics.py
--rw-r--r--   0        0        0    11559 2024-05-07 13:17:10.565607 qubx-0.1.83/src/qubx/core/helpers.py
--rw-r--r--   0        0        0    11910 2024-05-07 13:17:10.565607 qubx-0.1.83/src/qubx/core/loggers.py
--rw-r--r--   0        0        0    13688 2024-04-21 10:35:06.176526 qubx-0.1.83/src/qubx/core/lookups.py
--rw-r--r--   0        0        0     2847 2024-04-21 10:35:06.176526 qubx-0.1.83/src/qubx/core/series.pxd
--rw-r--r--   0        0        0    28108 2024-04-21 10:35:06.176526 qubx-0.1.83/src/qubx/core/series.pyx
--rw-r--r--   0        0        0    30330 2024-05-07 13:17:10.565607 qubx-0.1.83/src/qubx/core/strategy.py
--rw-r--r--   0        0        0     1368 2024-02-29 14:43:31.739720 qubx-0.1.83/src/qubx/core/utils.pyx
--rw-r--r--   0        0        0    31796 2024-05-22 11:55:16.120119 qubx-0.1.83/src/qubx/data/readers.py
--rw-r--r--   0        0        0     9150 2024-05-07 13:17:10.565607 qubx-0.1.83/src/qubx/impl/ccxt_connector.py
--rw-r--r--   0        0        0     3488 2024-05-07 13:17:10.565607 qubx-0.1.83/src/qubx/impl/ccxt_customizations.py
--rw-r--r--   0        0        0     9097 2024-05-07 13:17:10.565607 qubx-0.1.83/src/qubx/impl/ccxt_trading.py
--rw-r--r--   0        0        0     3565 2024-05-07 13:17:10.565607 qubx-0.1.83/src/qubx/impl/ccxt_utils.py
--rw-r--r--   0        0        0       33 2024-02-29 14:43:31.739720 qubx-0.1.83/src/qubx/math/__init__.py
--rw-r--r--   0        0        0     1176 2024-02-29 14:43:31.739720 qubx-0.1.83/src/qubx/math/stats.py
--rw-r--r--   0        0        0      175 2024-05-12 17:27:41.499398 qubx-0.1.83/src/qubx/pandaz/__init__.py
--rw-r--r--   0        0        0    85271 2024-05-12 17:27:41.503398 qubx-0.1.83/src/qubx/pandaz/ta.py
--rw-r--r--   0        0        0    19109 2024-05-12 17:27:41.503398 qubx-0.1.83/src/qubx/pandaz/utils.py
--rw-r--r--   0        0        0        0 2024-02-29 14:43:31.739720 qubx-0.1.83/src/qubx/ta/__init__.py
--rw-r--r--   0        0        0     7708 2024-02-29 14:43:31.739720 qubx-0.1.83/src/qubx/ta/indicators.pyx
--rw-r--r--   0        0        0       60 2024-04-21 10:35:06.176526 qubx-0.1.83/src/qubx/trackers/__init__.py
--rw-r--r--   0        0        0     5522 2024-04-21 10:35:06.176526 qubx-0.1.83/src/qubx/trackers/rebalancers.py
--rw-r--r--   0        0        0      273 2024-05-07 13:17:10.569607 qubx-0.1.83/src/qubx/utils/__init__.py
--rw-r--r--   0        0        0    12017 2024-05-14 18:44:12.292214 qubx-0.1.83/src/qubx/utils/_pyxreloader.py
--rw-r--r--   0        0        0    35158 2024-05-07 13:17:10.569607 qubx-0.1.83/src/qubx/utils/charting/mpl_helpers.py
--rw-r--r--   0        0        0    10993 2024-05-12 17:27:41.503398 qubx-0.1.83/src/qubx/utils/marketdata/binance.py
--rw-r--r--   0        0        0     9831 2024-05-12 17:27:41.503398 qubx-0.1.83/src/qubx/utils/misc.py
--rw-r--r--   0        0        0     9306 2024-05-12 17:27:41.503398 qubx-0.1.83/src/qubx/utils/runner.py
--rw-r--r--   0        0        0     4911 2024-05-14 18:44:12.292214 qubx-0.1.83/src/qubx/utils/time.py
--rw-r--r--   0        0        0     2491 1970-01-01 00:00:00.000000 qubx-0.1.83/PKG-INFO
+-rw-r--r--   0        0        0      940 2024-04-25 07:51:17.473695 qubx-0.1.84/README.md
+-rw-r--r--   0        0        0     9305 2024-04-21 10:35:06.164526 qubx-0.1.84/build.py
+-rw-r--r--   0        0        0     1556 2024-05-27 08:43:18.834739 qubx-0.1.84/pyproject.toml
+-rw-r--r--   0        0        0     6012 2024-05-27 08:42:37.963307 qubx-0.1.84/src/qubx/__init__.py
+-rw-r--r--   0        0        0     1875 2024-05-12 17:27:41.499398 qubx-0.1.84/src/qubx/_nb_magic.py
+-rw-r--r--   0        0        0        0 2024-02-29 14:43:31.739720 qubx-0.1.84/src/qubx/core/__init__.py
+-rw-r--r--   0        0        0     6707 2024-04-25 07:51:17.477695 qubx-0.1.84/src/qubx/core/account.py
+-rw-r--r--   0        0        0    14777 2024-05-07 13:17:10.565607 qubx-0.1.84/src/qubx/core/basics.py
+-rw-r--r--   0        0        0    11559 2024-05-07 13:17:10.565607 qubx-0.1.84/src/qubx/core/helpers.py
+-rw-r--r--   0        0        0    11910 2024-05-07 13:17:10.565607 qubx-0.1.84/src/qubx/core/loggers.py
+-rw-r--r--   0        0        0    13688 2024-04-21 10:35:06.176526 qubx-0.1.84/src/qubx/core/lookups.py
+-rw-r--r--   0        0        0     2847 2024-04-21 10:35:06.176526 qubx-0.1.84/src/qubx/core/series.pxd
+-rw-r--r--   0        0        0    28108 2024-04-21 10:35:06.176526 qubx-0.1.84/src/qubx/core/series.pyx
+-rw-r--r--   0        0        0    30330 2024-05-07 13:17:10.565607 qubx-0.1.84/src/qubx/core/strategy.py
+-rw-r--r--   0        0        0     1368 2024-02-29 14:43:31.739720 qubx-0.1.84/src/qubx/core/utils.pyx
+-rw-r--r--   0        0        0    32481 2024-05-27 08:42:37.963307 qubx-0.1.84/src/qubx/data/readers.py
+-rw-r--r--   0        0        0     9150 2024-05-07 13:17:10.565607 qubx-0.1.84/src/qubx/impl/ccxt_connector.py
+-rw-r--r--   0        0        0     3488 2024-05-07 13:17:10.565607 qubx-0.1.84/src/qubx/impl/ccxt_customizations.py
+-rw-r--r--   0        0        0     9097 2024-05-07 13:17:10.565607 qubx-0.1.84/src/qubx/impl/ccxt_trading.py
+-rw-r--r--   0        0        0     3565 2024-05-07 13:17:10.565607 qubx-0.1.84/src/qubx/impl/ccxt_utils.py
+-rw-r--r--   0        0        0       33 2024-02-29 14:43:31.739720 qubx-0.1.84/src/qubx/math/__init__.py
+-rw-r--r--   0        0        0     1176 2024-02-29 14:43:31.739720 qubx-0.1.84/src/qubx/math/stats.py
+-rw-r--r--   0        0        0      175 2024-05-12 17:27:41.499398 qubx-0.1.84/src/qubx/pandaz/__init__.py
+-rw-r--r--   0        0        0    85271 2024-05-12 17:27:41.503398 qubx-0.1.84/src/qubx/pandaz/ta.py
+-rw-r--r--   0        0        0    19109 2024-05-12 17:27:41.503398 qubx-0.1.84/src/qubx/pandaz/utils.py
+-rw-r--r--   0        0        0        0 2024-02-29 14:43:31.739720 qubx-0.1.84/src/qubx/ta/__init__.py
+-rw-r--r--   0        0        0     7708 2024-02-29 14:43:31.739720 qubx-0.1.84/src/qubx/ta/indicators.pyx
+-rw-r--r--   0        0        0       60 2024-04-21 10:35:06.176526 qubx-0.1.84/src/qubx/trackers/__init__.py
+-rw-r--r--   0        0        0     5522 2024-04-21 10:35:06.176526 qubx-0.1.84/src/qubx/trackers/rebalancers.py
+-rw-r--r--   0        0        0      273 2024-05-07 13:17:10.569607 qubx-0.1.84/src/qubx/utils/__init__.py
+-rw-r--r--   0        0        0    12017 2024-05-14 18:44:12.292214 qubx-0.1.84/src/qubx/utils/_pyxreloader.py
+-rw-r--r--   0        0        0    35158 2024-05-07 13:17:10.569607 qubx-0.1.84/src/qubx/utils/charting/mpl_helpers.py
+-rw-r--r--   0        0        0    10993 2024-05-12 17:27:41.503398 qubx-0.1.84/src/qubx/utils/marketdata/binance.py
+-rw-r--r--   0        0        0     9868 2024-05-27 08:42:37.963307 qubx-0.1.84/src/qubx/utils/misc.py
+-rw-r--r--   0        0        0     9306 2024-05-12 17:27:41.503398 qubx-0.1.84/src/qubx/utils/runner.py
+-rw-r--r--   0        0        0     4911 2024-05-14 18:44:12.292214 qubx-0.1.84/src/qubx/utils/time.py
+-rw-r--r--   0        0        0     2491 1970-01-01 00:00:00.000000 qubx-0.1.84/PKG-INFO
```

### Comparing `qubx-0.1.83/README.md` & `qubx-0.1.84/README.md`

 * *Files identical despite different names*

### Comparing `qubx-0.1.83/build.py` & `qubx-0.1.84/build.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.83/pyproject.toml` & `qubx-0.1.84/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Qubx"
-version = "0.1.83"
+version = "0.1.84"
 description = "Qubx - quantitative trading framework"
 authors = ["Dmitry Marienko <dmitry@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "qubx", from = "src" },
 ]
 repository = "https://github.com/dmarienko/Qubx"
```

### Comparing `qubx-0.1.83/src/qubx/__init__.py` & `qubx-0.1.84/src/qubx/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,165 +6,195 @@
 from qubx.core.lookups import FeesLookup, GlobalLookup, InstrumentsLookup
 
 
 def formatter(record):
     end = record["extra"].get("end", "\n")
     fmt = "<lvl>{message}</lvl>%s" % end
     if record["level"].name in {"WARNING", "SNAKY"}:
-        fmt = "<cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan> - %s" % fmt
-
-    prefix = "<green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green> [ <level>%s</level> ] " % record["level"].icon
+        fmt = (
+            "<cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan> - %s" % fmt
+        )
+
+    prefix = (
+        "<green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green> [ <level>%s</level> ] "
+        % record["level"].icon
+    )
 
     if record["exception"] is not None:
         # stackprinter.set_excepthook(style='darkbg2')
-        record["extra"]["stack"] = stackprinter.format(record["exception"], style="darkbg")
+        record["extra"]["stack"] = stackprinter.format(
+            record["exception"], style="darkbg"
+        )
         fmt += "\n{extra[stack]}\n"
 
     if record["level"].name in {"TEXT"}:
         prefix = ""
 
     return prefix + fmt
 
 
-config = {
-    "handlers": [ {"sink": sys.stdout, "format": "{time} - {message}"}, ],
-    "extra": {"user": "someone"},
-}
+class QubxLogConfig:
+
+    @staticmethod
+    def get_log_level():
+        return os.getenv("QUBX_LOG_LEVEL", "DEBUG")
+
+    @staticmethod
+    def set_log_level(level: str):
+        os.environ["QUBX_LOG_LEVEL"] = level
+        QubxLogConfig.setup_logger(level)
+
+    @staticmethod
+    def setup_logger(level: str | None = None):
+        global logger
+        config = {
+            "handlers": [
+                {"sink": sys.stdout, "format": "{time} - {message}"},
+            ],
+            "extra": {"user": "someone"},
+        }
+        logger.configure(**config)
+        logger.remove(None)
+        level = level or QubxLogConfig.get_log_level()
+        logger.add(sys.stdout, format=formatter, colorize=True, level=level)
+        logger = logger.opt(colors=True)
+
 
+QubxLogConfig.setup_logger()
 
-logger.configure(**config)
-logger.remove(None)
-logger.add(sys.stdout, format=formatter, colorize=True)
-logger = logger.opt(colors=True)
 
 # - global lookup helper
 lookup = GlobalLookup(InstrumentsLookup(), FeesLookup())
 
 
 # registering magic for jupyter notebook
-if runtime_env() in ['notebook', 'shell']:
-    from IPython.core.magic import (Magics, magics_class, line_magic, line_cell_magic)
+if runtime_env() in ["notebook", "shell"]:
+    from IPython.core.magic import Magics, magics_class, line_magic, line_cell_magic
     from IPython import get_ipython
 
     @magics_class
     class QubxMagics(Magics):
         # process data manager
         __manager = None
 
         @line_magic
         def qubxd(self, line: str):
-            self.qubx_setup('dark' + ' ' + line)
+            self.qubx_setup("dark" + " " + line)
 
         @line_magic
         def qubxl(self, line: str):
-            self.qubx_setup('light' + ' ' + line)
+            self.qubx_setup("light" + " " + line)
 
         @line_magic
         def qubx_setup(self, line: str):
             """
             QUBX framework initialization
             """
             import os
-            args = [x.strip() for x in line.split(' ')]
-            
+
+            args = [x.strip() for x in line.split(" ")]
+
             # setup cython dev hooks - only if 'dev' is passed as argument
-            if line and 'dev' in args: 
+            if line and "dev" in args:
                 install_pyx_recompiler_for_dev()
 
             tpl_path = os.path.join(os.path.dirname(__file__), "_nb_magic.py")
-            with open(tpl_path, 'r', encoding="utf8") as myfile:
+            with open(tpl_path, "r", encoding="utf8") as myfile:
                 s = myfile.read()
 
             exec(s, self.shell.user_ns)
 
             # setup more funcy mpl theme instead of ugly default
             if line:
-                if 'dark' in line.lower():
-                    set_mpl_theme('dark')
+                if "dark" in line.lower():
+                    set_mpl_theme("dark")
 
-                elif 'light' in line.lower():
-                    set_mpl_theme('light')
+                elif "light" in line.lower():
+                    set_mpl_theme("light")
 
             # install additional plotly helpers
             # from qube.charting.plot_helpers import install_plotly_helpers
             # install_plotly_helpers()
 
         def _get_manager(self):
             if self.__manager is None:
                 import multiprocessing as m
+
                 self.__manager = m.Manager()
             return self.__manager
 
         @line_cell_magic
         def proc(self, line, cell=None):
             """
             Run cell in separate process
 
             >>> %%proc x, y as MyProc1
             >>> x.set('Hello')
             >>> y.set([1,2,3,4])
-            
+
             """
             import multiprocessing as m
             import time, re
 
             # create ext args
             name = None
             if line:
                 # check if custom process name was provided
-                if ' as ' in line:
-                    line, name = line.split('as')
+                if " as " in line:
+                    line, name = line.split("as")
                     if not name.isspace():
                         name = name.strip()
                     else:
                         print('>>> Process name must be specified afer "as" keyword !')
                         return
 
                 ipy = get_ipython()
-                for a in [x for x in re.split('[\ ,;]', line.strip()) if x]:
+                for a in [x for x in re.split("[\ ,;]", line.strip()) if x]:
                     ipy.push({a: self._get_manager().Value(None, None)})
 
             # code to run
-            lines = '\n'.join(['    %s' % x for x in cell.split('\n')])
+            lines = "\n".join(["    %s" % x for x in cell.split("\n")])
 
             def fn():
                 result = get_ipython().run_cell(lines)
 
                 # send errors to parent
                 if result.error_before_exec:
                     raise result.error_before_exec
 
                 if result.error_in_exec:
                     raise result.error_in_exec
 
-            t_start = str(time.time()).replace('.', '_')
-            f_id = f'proc_{t_start}' if name is None else name
+            t_start = str(time.time()).replace(".", "_")
+            f_id = f"proc_{t_start}" if name is None else name
             if self._is_task_name_already_used(f_id):
                 f_id = f"{f_id}_{t_start}"
 
             task = m.Process(target=fn, name=f_id)
             task.start()
-            print(' -> Task %s is started' % f_id)
+            print(" -> Task %s is started" % f_id)
 
         def _is_task_name_already_used(self, name):
             import multiprocessing as m
+
             for p in m.active_children():
                 if p.name == name:
                     return True
             return False
 
         @line_magic
         def list_proc(self, line):
             import multiprocessing as m
+
             for p in m.active_children():
                 print(p.name)
 
         @line_magic
         def kill_proc(self, line):
             import multiprocessing as m
+
             for p in m.active_children():
                 if line and p.name.startswith(line):
                     p.terminate()
 
-
     # - registering magic here
     get_ipython().register_magics(QubxMagics)
```

### Comparing `qubx-0.1.83/src/qubx/_nb_magic.py` & `qubx-0.1.84/src/qubx/_nb_magic.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.83/src/qubx/core/account.py` & `qubx-0.1.84/src/qubx/core/account.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.83/src/qubx/core/basics.py` & `qubx-0.1.84/src/qubx/core/basics.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.83/src/qubx/core/helpers.py` & `qubx-0.1.84/src/qubx/core/helpers.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.83/src/qubx/core/loggers.py` & `qubx-0.1.84/src/qubx/core/loggers.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.83/src/qubx/core/lookups.py` & `qubx-0.1.84/src/qubx/core/lookups.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.83/src/qubx/core/series.pxd` & `qubx-0.1.84/src/qubx/core/series.pxd`

 * *Files identical despite different names*

### Comparing `qubx-0.1.83/src/qubx/core/series.pyx` & `qubx-0.1.84/src/qubx/core/series.pyx`

 * *Files identical despite different names*

### Comparing `qubx-0.1.83/src/qubx/core/strategy.py` & `qubx-0.1.84/src/qubx/core/strategy.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.83/src/qubx/core/utils.pyx` & `qubx-0.1.84/src/qubx/core/utils.pyx`

 * *Files identical despite different names*

### Comparing `qubx-0.1.83/src/qubx/data/readers.py` & `qubx-0.1.84/src/qubx/data/readers.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,23 +7,30 @@
 from pyarrow import csv
 import psycopg as pg
 from functools import wraps
 
 from qubx import logger
 from qubx.core.series import TimeSeries, OHLCV, time_as_nsec, Quote, Trade
 from qubx.utils.time import infer_series_frequency, handle_start_stop
+from psycopg.types.datetime import TimestampLoader
 
 _DT = lambda x: pd.Timedelta(x).to_numpy().item()
 D1, H1 = _DT("1D"), _DT("1h")
 
 DEFAULT_DAILY_SESSION = (_DT("00:00:00.100"), _DT("23:59:59.900"))
 STOCK_DAILY_SESSION = (_DT("9:30:00.100"), _DT("15:59:59.900"))
 CME_FUTURES_DAILY_SESSION = (_DT("8:30:00.100"), _DT("15:14:59.900"))
 
 
+class NpTimestampLoader(TimestampLoader):
+    def load(self, data) -> np.datetime64:
+        dt = super().load(data)
+        return np.datetime64(dt)
+
+
 def _recognize_t(t: Union[int, str], defaultvalue, timeunit) -> int:
     if isinstance(t, (str, pd.Timestamp)):
         try:
             return np.datetime64(t, timeunit)
         except:
             pass
     return defaultvalue
@@ -42,25 +49,31 @@
         ai = a.lower()
         if ai in xs:
             return xs.index(ai)
     raise IndexError(f"Can't find any from {args} in list: {xs}")
 
 
 _FIND_TIME_COL_IDX = lambda column_names: _find_column_index_in_list(
-    column_names, "time", "timestamp", "datetime", "date", "open_time"
+    column_names, "time", "timestamp", "datetime", "date", "open_time", "ts"
 )
 
 
 class DataTransformer:
 
     def __init__(self) -> None:
         self.buffer = []
         self._column_names = []
 
-    def start_transform(self, name: str, column_names: List[str]):
+    def start_transform(
+        self,
+        name: str,
+        column_names: List[str],
+        start: str | None = None,
+        stop: str | None = None,
+    ):
         self._column_names = column_names
         self.buffer = []
 
     def process_data(self, rows_data: Iterable) -> Any:
         if rows_data is not None:
             self.buffer.extend(rows_data)
 
@@ -177,26 +190,28 @@
         selected_table = table.slice(start_idx, length)
 
         # - in this case we want to return iterable chunks of data
         if chunksize > 0:
 
             def _iter_chunks():
                 for n in range(0, length // chunksize + 1):
-                    transform.start_transform(data_id, fieldnames)
+                    transform.start_transform(
+                        data_id, fieldnames, start=start, stop=stop
+                    )
                     raw_data = (
                         selected_table[n * chunksize : min((n + 1) * chunksize, length)]
                         .to_pandas()
                         .to_numpy()
                     )
                     transform.process_data(raw_data)
                     yield transform.collect()
 
             return _iter_chunks()
 
-        transform.start_transform(data_id, fieldnames)
+        transform.start_transform(data_id, fieldnames, start=start, stop=stop)
         raw_data = selected_table.to_pandas().to_numpy()
         transform.process_data(raw_data)
         return transform.collect()
 
     def get_names(self) -> List[str]:
         _n = []
         for s in os.listdir(self.path):
@@ -209,15 +224,15 @@
     """
     List of records to pandas dataframe transformer
     """
 
     def __init__(self, timestamp_units=None) -> None:
         self.timestamp_units = timestamp_units
 
-    def start_transform(self, name: str, column_names: List[str]):
+    def start_transform(self, name: str, column_names: List[str], **kwargs):
         self._time_idx = _FIND_TIME_COL_IDX(column_names)
         self._column_names = column_names
         self._frame = pd.DataFrame()
 
     def process_data(self, rows_data: Iterable) -> Any:
         self._frame
         p = pd.DataFrame.from_records(rows_data, columns=self._column_names)
@@ -252,15 +267,15 @@
     def __init__(self, timeframe: str | None = None, timestamp_units="ns") -> None:
         super().__init__()
         self.timeframe = timeframe
         self._series = None
         self._data_type = None
         self.timestamp_units = timestamp_units
 
-    def start_transform(self, name: str, column_names: List[str]):
+    def start_transform(self, name: str, column_names: List[str], **kwargs):
         self._time_idx = _FIND_TIME_COL_IDX(column_names)
         self._volume_idx = None
         self._b_volume_idx = None
         try:
             self._close_idx = _find_column_index_in_list(column_names, "close")
             self._open_idx = _find_column_index_in_list(column_names, "open")
             self._high_idx = _find_column_index_in_list(column_names, "high")
@@ -372,15 +387,15 @@
 
 class AsQuotes(DataTransformer):
     """
     Tries to convert incoming data to list of Quote's
     Data must have appropriate structure: bid, ask, bidsize, asksize and time
     """
 
-    def start_transform(self, name: str, column_names: List[str]):
+    def start_transform(self, name: str, column_names: List[str], **kwargs):
         self.buffer = list()
         self._time_idx = _FIND_TIME_COL_IDX(column_names)
         self._bid_idx = _find_column_index_in_list(column_names, "bid")
         self._ask_idx = _find_column_index_in_list(column_names, "ask")
         self._bidvol_idx = _find_column_index_in_list(
             column_names, "bidvol", "bid_vol", "bidsize", "bid_size"
         )
@@ -418,15 +433,15 @@
         ...
     ] ```
     """
 
     def __init__(self, timestamp_units: str | None = None) -> None:
         self.timestamp_units = timestamp_units
 
-    def start_transform(self, name: str, column_names: List[str]):
+    def start_transform(self, name: str, column_names: List[str], **kwargs):
         self.buffer = list()
         self._time_idx = _FIND_TIME_COL_IDX(column_names)
         self._column_names = column_names
 
     def process_data(self, rows_data: Iterable) -> Any:
         self.buffer.extend(rows_data)
 
@@ -461,15 +476,15 @@
         self._trades = trades
         self._bid_size = default_bid_size
         self._ask_size = default_ask_size
         self._s2 = spread / 2.0
         self._d_session_start = daily_session_start_end[0]
         self._d_session_end = daily_session_start_end[1]
 
-    def start_transform(self, name: str, column_names: List[str]):
+    def start_transform(self, name: str, column_names: List[str], **kwargs):
         self.buffer = []
         # - it will fail if receive data doesn't look as ohlcv
         self._time_idx = _FIND_TIME_COL_IDX(column_names)
         self._open_idx = _find_column_index_in_list(column_names, "open")
         self._high_idx = _find_column_index_in_list(column_names, "high")
         self._low_idx = _find_column_index_in_list(column_names, "low")
         self._close_idx = _find_column_index_in_list(column_names, "close")
@@ -602,18 +617,16 @@
     @wraps(fn)
     def wrapper(*args, **kw):
         cls = args[0]
         for x in range(cls._reconnect_tries):
             # print(x, cls._reconnect_tries)
             try:
                 return fn(*args, **kw)
-            except (pg.InterfaceError, pg.OperationalError) as e:
-                logger.warning(
-                    "Database Connection [InterfaceError or OperationalError]"
-                )
+            except (pg.InterfaceError, pg.OperationalError, AttributeError) as e:
+                logger.debug("Database Connection [InterfaceError or OperationalError]")
                 # print ("Idle for %s seconds" % (cls._reconnect_idle))
                 # time.sleep(cls._reconnect_idle)
                 cls._connect()
 
     return wrapper
 
 
@@ -696,15 +709,15 @@
 
         # - check resample format
         resample = (
             QuestDBSqlCandlesBuilder._convert_time_delta_to_qdb_resample_format(
                 resample
             )
             if resample
-            else resample
+            else "1m"  # if resample is empty let's use 1 minute timeframe
         )
         _rsmpl = f"SAMPLE by {resample}" if resample else ""
 
         table_name = self.get_table_name(data_id, data_type)
         return f"""
                 select timestamp, 
                 first(open) as open, 
@@ -745,27 +758,37 @@
         self._cursor = None
         self._host = host
         self._port = port
         self.connection_url = f"user={user} password={password} host={host} port={port}"
         self._builder = builder
         self._connect()
 
+    def __getstate__(self):
+        if self._connection:
+            self._connection.close()
+            self._connection = None
+        if self._cursor:
+            self._cursor.close()
+            self._cursor = None
+        state = self.__dict__.copy()
+        return state
+
     def _connect(self):
         self._connection = pg.connect(self.connection_url, autocommit=True)
         self._cursor = self._connection.cursor()
         logger.debug(f"Connected to QuestDB at {self._host}:{self._port}")
 
     def read(
         self,
         data_id: str,
         start: str | None = None,
         stop: str | None = None,
         transform: DataTransformer = DataTransformer(),
         chunksize=0,  # TODO: use self._cursor.fetchmany in this case !!!!
-        timeframe: str = "1m",
+        timeframe: str | None = "1m",
         data_type="candles_1m",
     ) -> Any:
         return self._read(
             data_id,
             start,
             stop,
             transform,
@@ -782,97 +805,81 @@
     def _read(
         self,
         data_id: str,
         start: str | None,
         stop: str | None,
         transform: DataTransformer,
         chunksize: int,  # TODO: use self._cursor.fetchmany in this case !!!!
-        timeframe: str,
+        timeframe: str | None,
         data_type: str,
         builder: QuestDBSqlBuilder,
     ) -> Any:
         start, end = handle_start_stop(start, stop)
         _req = builder.prepare_data_sql(data_id, start, end, timeframe, data_type)
 
         self._cursor.execute(_req)  # type: ignore
         records = self._cursor.fetchall()  # TODO: for chunksize > 0 use fetchmany etc
+        if not records:
+            return None
 
         names = [d.name for d in self._cursor.description]  # type: ignore
-        transform.start_transform(data_id, names)
+        transform.start_transform(data_id, names, start=start, stop=stop)
 
         transform.process_data(records)
         return transform.collect()
 
     @_retry
     def _get_names(self, builder: QuestDBSqlBuilder) -> List[str]:
         self._cursor.execute(builder.prepare_names_sql())  # type: ignore
         records = self._cursor.fetchall()
         return [r[0] for r in records]
 
     def __del__(self):
         for c in (self._cursor, self._connection):
             try:
-                logger.info("Closing connection")
+                logger.debug("Closing connection")
                 c.close()
             except:
                 pass
 
 
-class SnapshotsBuilder(DataTransformer):
-    """
-    Snapshots assembler from OB updates
-    """
-
-    def __init__(
-        self,
-        levels: int = -1,  # how many levels restore, 1 - TOB, -1 - all
-        as_frame=False,  # result is dataframe
-    ):
-        self.buffer = []
-        self.levels = levels
-        self.as_frame = as_frame
-
-    def start_transform(self, name: str, column_names: List[str]):
-        # initialize buffer / series etc
-        # let's keep restored snapshots into some buffer etc
-        self.buffer = []
-
-        # do additional init stuff here
-
-    def process_data(self, rows_data: List[List]) -> Any:
-        for r in rows_data:
-            # restore snapshots and put into buffer or series
-            pass
-
-    def collect(self) -> Any:
-        # - may be convert it to pandas DataFrame ?
-        if self.as_frame:
-            return pd.DataFrame.from_records(self.buffer)  # or custom transform
-
-        # - or just returns as plain list
-        return self.buffer
-
-
-class QuestDBSqlOrderBookBilder(QuestDBSqlBuilder):
+class QuestDBSqlOrderBookBuilder(QuestDBSqlCandlesBuilder):
     """
     Sql builder for snapshot data
     """
 
-    def get_table_name(self, data_id: str, sfx: str = "") -> str:
-        return ""
+    MAX_TIME_DELTA = pd.Timedelta("5h")
+    SNAPSHOT_DELTA = pd.Timedelta("1h")
+    MIN_DELTA = pd.Timedelta("1s")
 
     def prepare_data_sql(
         self,
         data_id: str,
         start: str | None,
         end: str | None,
         resample: str,
         data_type: str,
     ) -> str:
-        return ""
+        if not start or not end:
+            raise ValueError("Start and end dates must be provided for orderbook data!")
+        start_dt, end_dt = pd.Timestamp(start), pd.Timestamp(end)
+        delta = end_dt - start_dt
+        if delta > self.MAX_TIME_DELTA:
+            raise ValueError(
+                f"Time range is too big for orderbook data: {delta}, max allowed: {self.MAX_TIME_DELTA}"
+            )
+
+        raw_start_dt = start_dt.floor(self.SNAPSHOT_DELTA) - self.MIN_DELTA
+
+        table_name = self.get_table_name(data_id, data_type)
+        query = f"""
+SELECT * FROM {table_name}
+WHERE timestamp BETWEEN '{raw_start_dt}' AND '{end_dt}'
+"""
+        return query
 
 
 class TradeSql(QuestDBSqlCandlesBuilder):
 
     def prepare_data_sql(
         self,
         data_id: str,
@@ -927,23 +934,27 @@
             data_type="trade"
         )
     """
 
     _TYPE_TO_BUILDER = {
         "candles_1m": QuestDBSqlCandlesBuilder(),
         "trade": TradeSql(),
-        "orderbook": QuestDBSqlOrderBookBilder(),
+        "agg_trade": TradeSql(),
+        "orderbook": QuestDBSqlOrderBookBuilder(),
     }
 
     _TYPE_MAPPINGS = {
         "candles": "candles_1m",
         "trades": "trade",
         "ob": "orderbook",
         "trd": "trade",
         "td": "trade",
+        "aggTrade": "agg_trade",
+        "agg_trades": "agg_trade",
+        "aggTrades": "agg_trade",
     }
 
     def __init__(
         self,
         host="localhost",
         user="admin",
         password="quest",
@@ -970,17 +981,17 @@
 
     def read(
         self,
         data_id: str,
         start: str | None = None,
         stop: str | None = None,
         transform: DataTransformer = DataTransformer(),
-        chunksize=0,  # TODO: use self._cursor.fetchmany in this case !!!!
+        chunksize: int = 0,  # TODO: use self._cursor.fetchmany in this case !!!!
         timeframe: str | None = None,
-        data_type="candles",
+        data_type: str = "candles",
     ) -> Any:
         _mapped_data_type = self._TYPE_MAPPINGS.get(data_type, data_type)
         return self._read(
             data_id,
             start,
             stop,
             transform,
```

### Comparing `qubx-0.1.83/src/qubx/impl/ccxt_connector.py` & `qubx-0.1.84/src/qubx/impl/ccxt_connector.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.83/src/qubx/impl/ccxt_customizations.py` & `qubx-0.1.84/src/qubx/impl/ccxt_customizations.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.83/src/qubx/impl/ccxt_trading.py` & `qubx-0.1.84/src/qubx/impl/ccxt_trading.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.83/src/qubx/impl/ccxt_utils.py` & `qubx-0.1.84/src/qubx/impl/ccxt_utils.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.83/src/qubx/math/stats.py` & `qubx-0.1.84/src/qubx/math/stats.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.83/src/qubx/pandaz/ta.py` & `qubx-0.1.84/src/qubx/pandaz/ta.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.83/src/qubx/pandaz/utils.py` & `qubx-0.1.84/src/qubx/pandaz/utils.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.83/src/qubx/ta/indicators.pyx` & `qubx-0.1.84/src/qubx/ta/indicators.pyx`

 * *Files identical despite different names*

### Comparing `qubx-0.1.83/src/qubx/trackers/rebalancers.py` & `qubx-0.1.84/src/qubx/trackers/rebalancers.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.83/src/qubx/utils/_pyxreloader.py` & `qubx-0.1.84/src/qubx/utils/_pyxreloader.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.83/src/qubx/utils/charting/mpl_helpers.py` & `qubx-0.1.84/src/qubx/utils/charting/mpl_helpers.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.83/src/qubx/utils/marketdata/binance.py` & `qubx-0.1.84/src/qubx/utils/marketdata/binance.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.83/src/qubx/utils/misc.py` & `qubx-0.1.84/src/qubx/utils/misc.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,155 +4,159 @@
 from os.path import basename, exists, dirname, join, expanduser
 import time
 from pathlib import Path
 
 
 def version() -> str:
     # - check current version
-    version = 'Dev'
-    try: 
+    version = "Dev"
+    try:
         import importlib_metadata
-        version = importlib_metadata.version('qubx')
+
+        version = importlib_metadata.version("qubx")
     except:
         pass
 
     return version
 
 
 def install_pyx_recompiler_for_dev():
     from ._pyxreloader import pyx_install_loader
 
     # if version().lower() == 'dev':
     print(f" >  [{green('dev')}] {red('installing cython rebuilding hook')}")
-    pyx_install_loader([
-        'qubx.core', 
-        'qubx.ta', 
-        'qubx.data', 
-        'qubx.strategies'
-    ])
+    pyx_install_loader(["qubx.core", "qubx.ta", "qubx.data", "qubx.strategies"])
 
 
 def runtime_env():
     """
     Check what environment this script is being run under
     :return: environment name, possible values:
              - 'notebook' jupyter notebook
              - 'shell' any interactive shell (ipython, PyCharm's console etc)
              - 'python' standard python interpreter
              - 'unknown' can't recognize environment
     """
     try:
         from IPython.core.getipython import get_ipython
+
         shell = get_ipython().__class__.__name__
 
-        if shell == 'ZMQInteractiveShell':  # Jupyter notebook or qtconsole
-            return 'notebook'
-        elif shell.endswith('TerminalInteractiveShell'):  # Terminal running IPython
-            return 'shell'
+        if shell == "ZMQInteractiveShell":  # Jupyter notebook or qtconsole
+            return "notebook"
+        elif shell.endswith("TerminalInteractiveShell"):  # Terminal running IPython
+            return "shell"
         else:
-            return 'unknown'  # Other type (?)
+            return "unknown"  # Other type (?)
     except (NameError, ImportError):
-        return 'python'  # Probably standard Python interpreter
+        return "python"  # Probably standard Python interpreter
+
 
 _QUBX_FLDR = None
 
+
 def get_local_qubx_folder() -> str:
     global _QUBX_FLDR
 
     if _QUBX_FLDR is None:
-        _QUBX_FLDR = makedirs(os.getenv('QUBXSTORAGE', os.path.expanduser('~/.qubx')))
+        _QUBX_FLDR = makedirs(os.getenv("QUBXSTORAGE", os.path.expanduser("~/.qubx")))
 
     return _QUBX_FLDR
 
 
-def add_project_to_system_path(project_folder:str = '~/projects'):
+def add_project_to_system_path(project_folder: str = "~/projects"):
     """
     Add path to projects folder to system python path to be able importing any modules from project
     from test.Models.handy_utils import some_module
     """
     import sys
     from os.path import expanduser, relpath
     from pathlib import Path
-    
+
     # we want to track folders with these files as separate paths
-    toml = Path('pyproject.toml')
-    src = Path('src')
-    
+    toml = Path("pyproject.toml")
+    src = Path("src")
+
     try:
         prj = Path(relpath(expanduser(project_folder)))
     except ValueError as e:
         # This error can occur on Windows if user folder and python file are on different drives
         print(f"Qube> Error during get path to projects folder:\n{e}")
     else:
-        insert_path_iff = lambda p: sys.path.insert(0, p.as_posix()) if p.as_posix() not in sys.path else None
+        insert_path_iff = lambda p: (
+            sys.path.insert(0, p.as_posix()) if p.as_posix() not in sys.path else None
+        )
         if prj.exists():
             insert_path_iff(prj)
-            
+
             for di in prj.iterdir():
                 _src = di / src
                 if (di / toml).exists():
                     # when we have src/
                     if _src.exists() and _src.is_dir():
                         insert_path_iff(_src)
                     else:
                         insert_path_iff(di)
         else:
-            print(f'Qube> Cant find {project_folder} folder for adding to python path !')
+            print(
+                f"Qube> Cant find {project_folder} folder for adding to python path !"
+            )
 
 
 def is_localhost(host):
-    return host.lower() == 'localhost' or host == '127.0.0.1'
+    return host.lower() == "localhost" or host == "127.0.0.1"
 
 
 def __wrap_with_color(code):
     def inner(text, bold=False):
         c = code
         if bold:
             c = "1;%s" % c
         return "\033[%sm%s\033[0m" % (c, text)
 
     return inner
 
 
 red, green, yellow, blue, magenta, cyan, white = (
-    __wrap_with_color('31'),
-    __wrap_with_color('32'),
-    __wrap_with_color('33'),
-    __wrap_with_color('34'),
-    __wrap_with_color('35'),
-    __wrap_with_color('36'),
-    __wrap_with_color('37'),
+    __wrap_with_color("31"),
+    __wrap_with_color("32"),
+    __wrap_with_color("33"),
+    __wrap_with_color("34"),
+    __wrap_with_color("35"),
+    __wrap_with_color("36"),
+    __wrap_with_color("37"),
 )
 
 
 def logo():
     """
     Some fancy Qubx logo
     """
-    print(f"""
+    print(
+        f"""
 ⠀⠀⡰⡖⠒⠒⢒⢦⠀⠀   
 ⠀⢠⠃⠈⢆⣀⣎⣀⣱⡀  {red("QUBX")} | {cyan("Quantitative Backtesting Environment")} 
 ⠀⢳⠒⠒⡞⠚⡄⠀⡰⠁         (c) 2024, ver. {magenta(version().rstrip())}
 ⠀⠀⠱⣜⣀⣀⣈⣦⠃⠀⠀⠀ 
-        """ 
+        """
     )
 
 
 class Struct:
     """
     Dynamic structure (similar to matlab's struct it allows to add new properties dynamically)
 
     >>> a = Struct(x=1, y=2)
     >>> a.z = 'Hello'
     >>> print(a)
 
     Struct(x=1, y=2, z='Hello')
-    
+
     >>> Struct(a=234, b=Struct(c=222)).to_dict()
-    
+
     {'a': 234, 'b': {'c': 222}}
 
     >>> Struct({'a': 555}, a=123, b=Struct(c=222)).to_dict()
 
     {'a': 123, 'b': {'c': 222}}
     """
 
@@ -163,27 +167,27 @@
                 _odw = OrderedDict(Struct.dict2struct(args[0]).to_dict()) | _odw
             elif isinstance(args[0], Struct):
                 _odw = args[0].to_dict() | _odw
         self.__initialize(_odw.keys(), _odw.values())
 
     def __initialize(self, fields, values):
         self._fields = list(fields)
-        self._meta = namedtuple('Struct', ' '.join(fields))
+        self._meta = namedtuple("Struct", " ".join(fields))
         self._inst = self._meta(*values)
 
     def fields(self) -> list:
         return self._fields
 
     def __getitem__(self, idx: int):
         return getattr(self._inst, self._fields[idx])
 
     def __getattr__(self, k):
         return getattr(self._inst, k)
 
-    def __or__(self, other: Union[dict, 'Struct']):
+    def __or__(self, other: Union[dict, "Struct"]):
         if isinstance(other, dict):
             other = Struct.dict2struct(other)
         elif not isinstance(other, Struct):
             raise ValueError(f"Can't union with object of {type(other)} type ")
         for f in other.fields():
             self.__setattr__(f, other.__getattr__(f))
         return self
@@ -191,15 +195,15 @@
     def __dir__(self):
         return self._fields
 
     def __repr__(self):
         return self._inst.__repr__()
 
     def __setattr__(self, k, v):
-        if k not in ['_inst', '_meta', '_fields']:
+        if k not in ["_inst", "_meta", "_fields"]:
             new_vals = {**self._inst._asdict(), **{k: v}}
             self.__initialize(new_vals.keys(), new_vals.values())
         else:
             super().__setattr__(k, v)
 
     def __getstate__(self):
         return self._inst._asdict()
@@ -216,22 +220,22 @@
 
     def to_dict(self) -> dict:
         """
         Return this structure as dictionary
         """
         return self.__ms2d(self)
 
-    def copy(self) -> 'Struct':
+    def copy(self) -> "Struct":
         """
         Returns copy of this structure
         """
         return Struct(self.to_dict())
 
     @staticmethod
-    def dict2struct(d: dict) -> 'Struct':
+    def dict2struct(d: dict) -> "Struct":
         """
         Convert dictionary to structure
         >>> s = dict2struct({'f_1_0': 1, 'z': {'x': 1, 'y': 2}})
         >>> print(s.z.x)
         1
         """
         m = Struct()
@@ -245,89 +249,95 @@
             m.__setattr__(k, v)
         return m
 
 
 def makedirs(path: str, *args) -> str:
     path = os.path.expanduser(os.path.join(*[path, *args]))
     if not exists(path):
-        os.makedirs(path)
+        os.makedirs(path, exist_ok=True)
     return path
 
 
 class Stopwatch:
     """
-    Stopwatch timer for performance 
+    Stopwatch timer for performance
     """
-    starts: Dict[str|None, int] = {} 
-    counts: Dict[str|None, int] = defaultdict(lambda: 0)
-    latencies: Dict[str|None, int] = {} 
-    
+
+    starts: Dict[str | None, int] = {}
+    counts: Dict[str | None, int] = defaultdict(lambda: 0)
+    latencies: Dict[str | None, int] = {}
+
     def __new__(cls):
-        if not hasattr(cls, 'instance'):
+        if not hasattr(cls, "instance"):
             cls.instance = super(Stopwatch, cls).__new__(cls)
         return cls.instance
-    
+
     def start(self, scope: str | None):
         self.starts[scope] = time.perf_counter_ns()
         self.counts[scope] += 1
-        
-    def stop(self, scope: str|None=None) -> int | None:
+
+    def stop(self, scope: str | None = None) -> int | None:
         t = time.perf_counter_ns()
         s = self.starts.get(scope, None)
         lat = None
         if s:
             lat = t - s
             n = self.counts[scope]
-            self.latencies[scope] = (lat * (n - 1) + self.latencies.get(scope, lat)) // n
+            self.latencies[scope] = (
+                lat * (n - 1) + self.latencies.get(scope, lat)
+            ) // n
             del self.starts[scope]
         return lat
 
     def latency_sec(self, scope: str | None) -> float:
         return self.latencies.get(scope, 0) / 1e9
 
-    def watch(self, scope='global'):
+    def watch(self, scope="global"):
         def _decorator(func):
-            info = scope + '.' + func.__name__
+            info = scope + "." + func.__name__
+
             def wrapper(*args, **kwargs):
                 self.start(info)
                 output = func(*args, **kwargs)
                 self.stop(info)
                 return output
+
             return wrapper
+
         return _decorator
-    
+
     def reset(self):
         self.starts.clear()
         self.counts.clear()
         self.latencies.clear()
 
     def __str__(self) -> str:
         r = ""
         for l in self.latencies.keys():
             r += f"\n\t<w>{l}</w> took <r>{self.latency_sec(l):.7f}</r> secs"
         return r
 
 
-def quotify(sx: Union[str, List[str]], quote='USDT'):
+def quotify(sx: Union[str, List[str]], quote="USDT"):
     """
     Make XXX<quote> from anything if that anything doesn't end with <quote>
     """
     if isinstance(sx, str):
         return (sx if sx.endswith(quote) else sx + quote).upper()
     elif isinstance(sx, (list, set, tuple)):
         return [quotify(s, quote) for s in sx]
     raise ValueError("Can't process input data !")
 
 
-def dequotify(sx: Union[str, List[str]], quote='USDT'):
+def dequotify(sx: Union[str, List[str]], quote="USDT"):
     """
     Turns XXX<quote> to XXX (reverse of quotify)
     """
     if isinstance(sx, str):
         quote = quote.upper()
-        if (s:=sx.upper()).endswith(quote):
-            s = s.split(':')[1] if ':' in s else s # remove exch: if presented
+        if (s := sx.upper()).endswith(quote):
+            s = s.split(":")[1] if ":" in s else s  # remove exch: if presented
             return s.split(quote)[0]
     elif isinstance(sx, (list, set, tuple)):
         return [dequotify(s, quote) for s in sx]
 
-    raise ValueError("Can't process input data !")
+    raise ValueError("Can't process input data !")
```

### Comparing `qubx-0.1.83/src/qubx/utils/runner.py` & `qubx-0.1.84/src/qubx/utils/runner.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.83/src/qubx/utils/time.py` & `qubx-0.1.84/src/qubx/utils/time.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.83/PKG-INFO` & `qubx-0.1.84/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Qubx
-Version: 0.1.83
+Version: 0.1.84
 Summary: Qubx - quantitative trading framework
 Home-page: https://github.com/dmarienko/Qubx
 Author: Dmitry Marienko
 Author-email: dmitry@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

