# Comparing `tmp/haniwers-0.14.4.tar.gz` & `tmp/haniwers-0.15.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haniwers-0.14.4.tar", max compression
+gzip compressed data, was "haniwers-0.15.0.tar", max compression
```

## Comparing `haniwers-0.14.4.tar` & `haniwers-0.15.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1072 2023-05-17 08:20:30.907111 haniwers-0.14.4/LICENSE
--rw-r--r--   0        0        0     6183 2024-05-22 14:20:19.674777 haniwers-0.14.4/README.md
--rw-r--r--   0        0        0       23 2024-05-25 10:40:59.348636 haniwers-0.14.4/haniwers/__init__.py
--rw-r--r--   0        0        0    11788 2024-05-22 14:20:19.753181 haniwers-0.14.4/haniwers/cli.py
--rw-r--r--   0        0        0    16312 2024-05-22 14:19:28.812153 haniwers-0.14.4/haniwers/config.py
--rw-r--r--   0        0        0    17847 2024-05-25 10:40:42.556454 haniwers-0.14.4/haniwers/daq.py
--rw-r--r--   0        0        0     9267 2024-05-24 13:38:55.352520 haniwers-0.14.4/haniwers/dataset.py
--rw-r--r--   0        0        0     3443 2024-05-23 11:03:00.878115 haniwers-0.14.4/haniwers/mimic.py
--rw-r--r--   0        0        0      774 2024-05-22 14:19:28.812968 haniwers-0.14.4/haniwers/postprocess.py
--rw-r--r--   0        0        0    12810 2024-05-23 11:22:23.101251 haniwers-0.14.4/haniwers/preprocess.py
--rw-r--r--   0        0        0     7655 2024-05-25 10:40:42.557102 haniwers-0.14.4/haniwers/threshold.py
--rw-r--r--   0        0        0     1450 2024-05-25 10:40:59.359954 haniwers-0.14.4/pyproject.toml
--rw-r--r--   0        0        0     7639 1970-01-01 00:00:00.000000 haniwers-0.14.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-17 08:20:30.907111 haniwers-0.15.0/LICENSE
+-rw-r--r--   0        0        0     6942 2024-05-26 12:45:22.524830 haniwers-0.15.0/README.md
+-rw-r--r--   0        0        0       23 2024-05-27 02:58:58.835360 haniwers-0.15.0/haniwers/__init__.py
+-rw-r--r--   0        0        0    11782 2024-05-27 02:58:41.796262 haniwers-0.15.0/haniwers/cli.py
+-rw-r--r--   0        0        0    16792 2024-05-27 02:58:41.796496 haniwers-0.15.0/haniwers/config.py
+-rw-r--r--   0        0        0    22913 2024-05-27 02:58:41.796982 haniwers-0.15.0/haniwers/daq.py
+-rw-r--r--   0        0        0     9820 2024-05-27 02:58:41.797488 haniwers-0.15.0/haniwers/dataset.py
+-rw-r--r--   0        0        0     2618 2024-05-27 02:58:41.797813 haniwers-0.15.0/haniwers/mimic.py
+-rw-r--r--   0        0        0      774 2024-05-22 14:19:28.812968 haniwers-0.15.0/haniwers/postprocess.py
+-rw-r--r--   0        0        0    12810 2024-05-23 11:22:23.101251 haniwers-0.15.0/haniwers/preprocess.py
+-rw-r--r--   0        0        0     8512 2024-05-27 02:58:41.798249 haniwers-0.15.0/haniwers/threshold.py
+-rw-r--r--   0        0        0     1482 2024-05-27 02:58:58.846023 haniwers-0.15.0/pyproject.toml
+-rw-r--r--   0        0        0     8398 1970-01-01 00:00:00.000000 haniwers-0.15.0/PKG-INFO
```

### Comparing `haniwers-0.14.4/LICENSE` & `haniwers-0.15.0/LICENSE`

 * *Files identical despite different names*

### Comparing `haniwers-0.14.4/README.md` & `haniwers-0.15.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+
+
+![GitLab Tag](https://img.shields.io/gitlab/v/tag/qumasan%2Fhaniwers?sort=semver&style=for-the-badge) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/haniwers?style=for-the-badge) ![GitLab License](https://img.shields.io/gitlab/license/qumasan%2Fhaniwers?style=for-the-badge)
+![PyPI - Downloads](https://img.shields.io/pypi/dd/haniwers?style=for-the-badge) ![PyPI -Downloads](https://img.shields.io/pypi/dw/haniwers?style=for-the-badge) ![PyPI - Downloads](https://img.shields.io/pypi/dm/haniwers?style=for-the-badge)
+![Gitlab Pipeline Status](https://img.shields.io/gitlab/pipeline-status/qumasan%2Fhaniwers?style=for-the-badge) ![GitLab Last Commit](https://img.shields.io/gitlab/last-commit/qumasan%2Fhaniwers?style=for-the-badge)
+
+---
+
+
 # Haniwers : ハニワーズ
 
 墳Qの解析コード（個人用）
 
 ![w:300](../docs/_static/haniwer.png)
 
 # インストール
```

### Comparing `haniwers-0.14.4/haniwers/cli.py` & `haniwers-0.15.0/haniwers/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,17 +168,15 @@
 
     for port in ports:
         if "UART" in port.description:
             logger.info(f"Please use '{port.device}' as your device path")
 
 
 @app.command()
-def vth(
-    ch: int = 0, vth: int = 0, max_retry: int = 3, load_from: str = "daq.toml"
-) -> None:
+def vth(ch: int = 0, vth: int = 0, max_retry: int = 3, load_from: str = "daq.toml") -> None:
     """Set threshold to each channel. 1step = 4mV.
 
     OSECHIの各チャンネルにスレッショルドを設定します。
     カレントディレクトリにある ``thresholds_latest.csv`` を参考に、
     スレッショルド値の最良推定値を設定します。
     1step = 4mVに相当します。
```

### Comparing `haniwers-0.14.4/haniwers/config.py` & `haniwers-0.15.0/haniwers/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from dataclasses import dataclass
 from icecream import ic
 from loguru import logger
 from pathlib import Path
-from typing import Optional
+from typing import Optional, Any
 import pandas as pd
 import sys
-import tomli
-import tomllib
+import tomli  # Python3.9対応のためtomliを使う
+
+# import tomllib  # TODO: いずれtomllibに置き換える
+from pydantic import BaseModel
 
 ic.configureOutput(prefix=f"{__name__}: ")
 
 
 @dataclass
 class RunData:
     """
@@ -276,16 +278,15 @@
         self.device = _config.get("device", "/dev/ttyUSB0")
         self.baudrate = _config.get("baudrate", 115200)
         self.timeout = _config.get("timeout", 1000)
         self.fname_logs = _config.get("fname_logs", "threshold_logs.csv")
         self.fname_scan = _config.get("fname_scan", "threshold_scan.csv")
 
 
-@dataclass
-class UserSettings:
+class UserSettings(BaseModel):
     """ユーザー設定用のクラス
 
     ``read_from`` に指定したファイルからユーザー設定を読み込みます。
     設定ファイルはTOML形式で作成してください。
     その他の形式に対応する予定はいまのところありません。
     また、読み込み時のファイル形式のチェックもしていません。
 
@@ -311,54 +312,74 @@
     dict_keys(
         ['default', 'device', 'daq', 'scan', 'threshold', 'loguru']
     )
     ```
 
     """
 
-    read_from: str | Path
+    load_from: str
+    settings: dict = {}
+    sections: list = []
 
-    def __post_init__(self):
-        settings = self.load_toml(self.read_from)
+    def model_post_init(self, __context: Any) -> None:
+        settings = self.load_toml(self.load_from)
         self.settings = settings
-        self.sections = settings.keys()
+        self.sections = list(settings.keys())
+        return super().model_post_init(__context)
 
-    def load_toml(self, read_from: str) -> dict:
+    def load_toml(self, load_from: str) -> dict:
         """設定をTOMLファイルから読み込んで、辞書型に変換する
 
         UserSettingsクラスのオブジェクトを生成するときに ``__post_init__``の中で実行している。
         プロダクション環境では、このメソッドをわざわざ実行する必要はありません。
 
         新しい設定ファイルを作成した場合の内容確認のために使えると思います。
 
         :Args:
-        - read_from(str): ファイル名
+        - load_from(str): ファイル名
 
         :Returns:
         - settings(dict): ユーザー設定
 
         ```
 
         """
-        p = Path(read_from)
+        p = Path(load_from)
         with p.open("rb") as f:
-            settings = tomllib.load(f)
+            settings = tomli.load(f)
+        return settings
+
+    def _get_settings(self, keys: list) -> dict:
+        """設定を取得する
+
+        :Example:
+        >>> us = UserSettings(load_from="../sandbox/hnw.toml")
+        >>> keys = ["default", "device", "scan", "threshold"]
+        >>> settings = s._get_settings(keys)
+        """
+        settings = {}
+        for key in keys:
+            d = self.settings.get(key)
+            if d is None:
+                pass
+            else:
+                settings.update(d)
         return settings
 
     def get_daq_settings(self) -> dict:
         """DAQに必要な設定を取得する
 
         :Returns:
         - settings(dict): DAQの設定に必要な項目
 
         :Example:
 
         ```python
-        >>> s = UserSettings("../sandbox/hnw.toml")
-        >>> settings = s.get_daq_settings()
+        >>> us = UserSettings(load_from="../sandbox/hnw.toml")
+        >>> settings = us.get_daq_settings()
         >>> settings
         {
             'saved': '',
             'suffix': '.csv',
             'skip': 10,
             'max_rows': 1000,
             'port': '/dev/ttyUSB0',
@@ -367,34 +388,28 @@
             'prefix': 'osechi_data',
             'max_files': 1000
         }
         ```
 
         """
         keys = ["default", "device", "daq"]
-        settings = {}
-        for key in keys:
-            d = self.settings.get(key)
-            if d is None:
-                pass
-            else:
-                settings.update(d)
+        settings = self._get_settings(keys)
         return settings
 
     def get_scan_settings(self) -> dict:
         """スレッショルド測定に必要は設定を取得する
 
         :Returns:
         - settings(dict): スレッショルド測定に必要な項目
 
         :Example:
 
         ```python
-        >>> s = UserSettings("../sandbox/hnw.toml")
-        >>> settings = s.get_scan_settings()
+        >>> us = UserSettings(load_from="../sandbox/hnw.toml")
+        >>> settings = us.get_scan_settings()
         >>> settings
         {
             'saved': '',
             'suffix': '.csv',
             'skip': 10,
             'max_rows': 1000,
             'port': '/dev/ttyUSB0',
@@ -407,21 +422,15 @@
             'fit': {'fname': 'threshold_fit.csv', 'names': ['time', 'ch', '0sigma', '1sigma', '3sigma', '5sigma']}
         }
         ```
 
         """
 
         keys = ["default", "device", "scan", "threshold"]
-        settings = {}
-        for key in keys:
-            d = self.settings.get(key)
-            if d is None:
-                pass
-            else:
-                settings.update(d)
+        settings = self._get_settings(keys)
         return settings
 
     def get_loguru(self, level: str = "DEBUG") -> logger:
         """ロガーを初期化する
 
         loguruパッケージを使ったロガーを初期化します。
         ``level`` オプションで指定したログレベルで、標準エラー出力（``sys.stderr``）のハンドラーを作成します。
```

### Comparing `haniwers-0.14.4/haniwers/daq.py` & `haniwers-0.15.0/haniwers/daq.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,18 +11,23 @@
 from pydantic import BaseModel
 from tqdm import tqdm
 
 from .config import Daq
 
 
 class RealEvent(BaseModel):
-    """実イベント"""
+    """実イベント
+
+    OSECHIに接続したUSBポートから、シリアル通信で受け取った値を格納するためのデータクラス。
+    ファイルに書き出したり、`pandas.DataFrame`に変換できるように自作メソッドを追加。
+
+    """
 
     timestamp: datetime = pendulum.now()
-    """測定時刻。宇宙線イベントが通過した日時"""
+    """測定時刻。宇宙線イベントが通過した日時。タイムゾーン付きの日付オブジェクト"""
     top: int = 0
     """topレイヤーのヒット。0 - 10の値"""
     mid: int = 0
     """midレイヤーのヒット。0 - 10の値"""
     btm: int = 0
     """btmレイヤーのヒット。0 - 10の値"""
     adc: int = 0
@@ -30,14 +35,81 @@
     tmp: float = 0.0
     """BME280で測定した気温。[degC]"""
     atm: float = 0.0
     """BME280で測定した気圧。[Pa]"""
     hmd: float = 0.0
     """BME280で測定した湿度。[%]"""
 
+    def to_list_string(self) -> list[str]:
+        """List
+
+        メンバー変数を文字列にしたリストに変換します。
+
+        ```python
+        >>> real_data = RealEvent()
+        >>> read_data.to_list_string()
+        ['2024-05-21 08:44:20.389786+09:00', '0', '0', '0', '0', '0', '0', '0']
+        ```
+
+        """
+        data = self.model_dump()
+        values = [str(v) for v in data.values()]
+        return values
+
+    def to_csv_string(self) -> str:
+        """Comma Separated Values
+
+        メンバー変数をCSV形式（カンマ区切り）の文字列に変換します。
+        OSECHIから受け取ったデータを、ファイルに保存する際に使うことを想定したメソッドです。
+
+        ```python
+        >>> real_data = RealEvent()
+        >>> real_data.to_csv_string()
+        '2024-05-21 08:44:20.389786+09:00,0,0,0,0,0,0,0'
+        ```
+
+        """
+        data = self.model_dump().values()
+        values = [str(v) for v in data]
+        csv_string = (",").join(values)
+        return csv_string
+
+    def to_tsv_string(self) -> str:
+        """Tab Separated Values
+
+        メンバー変数をTSV形式（タブ区切り）の文字列に変換します。
+
+        ```python
+        >>> real_data = RealEvent()
+        >>> real_data.to_tsv_string()
+        '2024-05-21 08:44:20.389786+09:00\t0\t0\t0\t0\t0\t0\t0'
+        ```
+
+        """
+        data = self.model_dump().values()
+        values = [str(v) for v in data]
+        tsv_string = ("\t").join(values)
+        return tsv_string
+
+    def to_ltsv_string(self) -> str:
+        """Labeled Tab-Separated Values
+
+        メンバー変数をLTSV形式（ラベルありのタブ区切り）の文字列に変換します。
+
+        ```python
+        >>> real_data = RealEvent()
+        >>> real_data.to_ltsv_string()
+        'timestamp:2024-05-21 08:44:20.389786+09:00\ttop:0\tmid:0\tbtm:0\tadc:0\ttmp:0\tatm:0\thmd:0'
+        ```
+        """
+        data = self.model_dump().items()
+        values = [f"{k}:{v}" for k, v in data]
+        ltsv_string = ("\t").join(values)
+        return ltsv_string
+
 
 def init_saved(daq: Daq) -> None:
     """Initialize destination directory to save data files
 
     保存先のディレクトリを初期化します。
     ディレクトリが存在しない場合は、作成します。
     ディレクトリが存在する場合は、``FileExistsError``を発行し、終了（``sys.exit``）します。
@@ -280,15 +352,15 @@
         logger.error(e)
         msg = """Could not open the port. Device name might be wrong.
         Run 'arduino-cli board list' and check the device name.
         Edit 'daq.toml' if you needed.
         """
         logger.warning(msg)
         sys.exit()
-    except Exception as e:
+    except Exception as e:  # noqa
         logger.error(e)
         msg = """
         Unaware error occurred.
         Please think if you need to handle this error.
         """
         sys.exit()
 
@@ -313,49 +385,131 @@
             return True
         msg = f"Retry: {i} / {max_retry} times."
         logger.warning(msg)
 
     return False
 
 
-def read_serial_data(port: serial.Serial) -> list:
-    """Read serial data from port.
+@deprecated(
+    version="0.15.0",
+    reason="Will be deprecated. Use _read_serial_data_as_event with validation.",
+)
+def _read_serial_data_as_list(port: serial.Serial) -> list:
+    """(Will be deprecated) Read serial data from port.
 
     OSECHIが接続されているポートからデータを読み出します。
-    引数にしていするポートは、あらかじめ開いたものを渡してください。
+    引数に指定するポートは、あらかじめ開いたものを渡してください。
     ``run_daq``や``time_daq``でデータを取得するために使います。
 
     :Args:
     - port (serial.Serial): Serialオブジェクト
 
     :Returns:
     - row (list): 読み出した時刻を追加したデータのリスト
 
     :Examples:
     ```python
     >>> with open_serial_connection() as port:
-    >>>     row = read_serialc_data(port)
+    >>>     row = read_serial_data(port)
     >>>     row
     [日付, top, mid, btm, adc, tmp, atm, hmd]
     ```
 
-    :TODO:
-    - list -> RealEventオブジェクトに変換する
-    - タイムアウトしたときの処理を整理する
-
     """
+    msg = "Will be deprecated."
+    logger.warning(msg)
     now = pendulum.now().to_iso8601_string()
     data = port.readline().decode("UTF-8").strip()
     if len(data) == 0:
         msg = f"No data to readout. Timed-out: {port.timeout}"
         logger.warning(msg)
     row = f"{now} {data}".split()
     return row
 
 
+def _read_serial_data_as_event(port: serial.Serial) -> RealEvent:
+    """Read serial data from port.
+
+    OSECHIが接続されているポートからデータを読み出します。
+    引数に指定するポートは、あらかじめ開いたものを渡してください。
+    ``run_daq``や``time_daq``でデータを取得するために使います。
+
+    :Args:
+    - port (serial.Serial): Serialオブジェクト
+
+    :Returns:
+    - row (list): 読み出した時刻を追加したデータのリスト
+
+    :Examples:
+    ```python
+    >>> with open_serial_connection() as port:
+    >>>     row = read_serialc_data(port)
+    >>>     row
+    [日付, top, mid, btm, adc, tmp, atm, hmd]
+    ```
+
+    """
+    data = port.readline().decode("UTF-8").strip().split()
+    if len(data) == 0:
+        msg = f"No data to readout. Timed-out: {port.timeout}"
+        logger.warning(msg)
+    event = RealEvent()
+    event.timestamp = pendulum.now()
+    event.top = int(data[0])
+    event.mid = int(data[1])
+    event.btm = int(data[2])
+    event.adc = int(data[3])
+    event.tmp = float(data[4])
+    event.atm = float(data[5])
+    event.hmd = float(data[6])
+    return event
+
+
+def read_serial_data(port: serial.Serial) -> list:
+    # data = _read_serial_data_as_list(port)
+    data = _read_serial_data_as_event(port)
+    return data.to_list_string()
+
+
+def _loop_events(port: serial.Serial, rows: list) -> RealEvent:
+    """イベント取得ループ
+
+    :Args:
+    - `port (serial.Serial)`: 接続済みのSerialオブジェクト
+    - `rows (list)`: ループする回数
+
+    :Yield:
+    - event (RealEvent): OSECHIの測定データ
+
+    """
+    for _ in tqdm(rows, leave=False, desc="loops"):
+        event = _read_serial_data_as_event(port)
+        yield event
+
+
+def loop_and_save_events(f, daq: Daq, port: serial.Serial) -> list[RealEvent]:
+    rows = range(daq.max_rows)
+    events = []
+    for event in _loop_events(port, rows):
+        events.append(event.model_dump_json())
+        row = event.to_list_string()
+        if daq.suffix in [".csv"]:
+            row = event.to_csv_string()
+            f.write(row + "\n")
+        elif daq.suffix in [".dat", ".tsv"]:
+            row = event.to_tsv_string()
+            f.write(row + "\n")
+        elif daq.suffix in [".json", ".jsonl"]:
+            row = event.model_dump_json()
+            f.write(row + "\n")
+        f.flush()
+    return events
+
+
+@deprecated(version="0.15.0", reason="Will be deprecated. Use loop_and_save_events instead.")
 def save_serial_data(f, daq: Daq, port: serial.Serial) -> list:
     """
     :Args:
     - f: ファイルポインタ
     - daq (Daq): Daqオブジェクト
     - port (serial.Serial): Serialオブジェクト
 
@@ -364,15 +518,15 @@
 
     :TODO:
     - Daqオブジェクトに依存しない関数にしたい（ジェネレーターにするのがいいのかな？）
     - pd.DataFrameを返した方がいいかもしれない？
     """
     max_rows = daq.max_rows
     rows = []
-    for nrow in tqdm(range(max_rows), leave=False, desc="rows"):
+    for _ in tqdm(range(max_rows), leave=False, desc="rows"):
         row = read_serial_data(port)
         rows.append(row)
         if daq.suffix == ".csv":
             writer = csv.writer(f)
             writer.writerow(row)
         else:
             writer = csv.writer(f, delimiter=" ")
@@ -398,15 +552,16 @@
         for nfile in tqdm(range(daq.max_files), desc="files"):
             savef = get_savef_with_timestamp(daq, nfile)
             msg = f"Saving data to: {savef}."
             logger.info(msg)
             logger.info("Press Ctrl-c to stop.")
 
             with savef.open("a") as f:
-                save_serial_data(f, daq, port)
+                # save_serial_data(f, daq, port)
+                loop_and_save_events(f, daq, port)
 
             msg = f"Saved data to: {savef}."
             logger.success(msg)
 
 
 def run(args: Daq):
     """メインのDAQ
@@ -427,15 +582,15 @@
         logger.warning(msg)
         sys.exit()
     except KeyboardInterrupt as e:
         logger.warning(e)
         msg = """Quit."""
         logger.info(msg)
         sys.exit()
-    except Exception as e:
+    except Exception as e:  # noqa
         logger.error(e)
         msg = """Exit.
         Unaware error occurred.
         Please think if you need to handle this error.
         """
         logger.error(msg)
         sys.exit()
@@ -463,15 +618,15 @@
 
         logger.debug(f"- DAQ Started: {daq_start}")
         logger.debug(f"- DAQ Stop   : {daq_stop}")
 
         while pendulum.now() < daq_stop:
             row = read_serial_data(port)
             event = RealEvent()
-            event.timestamp = pendulum.parse(row[0])
+            event.timestamp = pendulum.now()
             event.top = int(row[1])
             event.mid = int(row[2])
             event.btm = int(row[3])
             event.adc = int(row[4])
             event.tmp = float(row[5])
             event.atm = float(row[6])
             event.hmd = float(row[7])
@@ -542,17 +697,15 @@
     return data
 
 
 @deprecated(
     version="0.14.0",
     reason="Will be deprecated. Use threshold.scan_thresholds instead.",
 )
-def scan_ch_thresholds(
-    daq: Daq, duration: int, ch: int, thresholds: list[int]
-) -> list[list]:
+def scan_ch_thresholds(daq: Daq, duration: int, ch: int, thresholds: list[int]) -> list[list]:
     """
     Run threshold scan.
 
     :Args:
     - daq (Daq): Daqオブジェクト
     - duration (int): 測定時間（秒）
     - ch (int): チャンネル番号
```

### Comparing `haniwers-0.14.4/haniwers/dataset.py` & `haniwers-0.15.0/haniwers/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,20 @@
 
     def _ondotori_raw_data(self) -> list[Path]:
         """（プライベート関数）おんどとりのデータを取得する"""
         p = self.raw_data_path() / self._stem()
         fnames = sorted(p.glob("TR41_*.csv"))
         return fnames
 
+    def _threshlod_logs_data(self) -> list[Path]:
+        """（プライベート関数）スレッショルド設定のログを取得する"""
+        p = self.raw_data_path() / self._stem()
+        fnames = sorted(p.glob("threshold_logs.csv"))
+        return fnames
+
     def _to_dataframe(self, fnames, **kwargs) -> pd.DataFrame:
         """（プライベート関数）すべてのファイルをデータフレームに変換する
 
         :Args:
         - `fnames (list[Path])`: ファイル名のリスト
         - `**kwargs`: pd.DataFrameのオプション
 
@@ -145,16 +151,22 @@
         fnames = self._osechi_resampled_data()
         data = self._to_dataframe(fnames, parse_dates=["time"])
         return data
 
     def ondotori_data(self) -> pd.DataFrame:
         """おんどとりのデータフレーム"""
         fnames = self._ondotori_raw_data()
+        data = self._to_dataframe(fnames, skiprows=4, names=["time", "tmpC"], parse_dates=["time"])
+        return data
+
+    def threshold_logs(self) -> pd.DataFrame:
+        """スレッショルド設定のデータフレーム"""
+        fnames = self._threshlod_logs_data()
         data = self._to_dataframe(
-            fnames, skiprows=4, names=["time", "tmpC"], parse_dates=["time"]
+            fnames, names=["time", "ch", "vth", "success"], parse_dates=["time"]
         )
         return data
 
     def __str__(self):
         return self.name
```

### Comparing `haniwers-0.14.4/haniwers/mimic.py` & `haniwers-0.15.0/haniwers/mimic.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,41 +11,26 @@
 
 
 # 擬似イベントのデータフレームを取得する例
 fake_data = mimic.fake_events(100)
 ```
 """
 
-from pydantic import BaseModel
-import pendulum
 import random
-import pandas as pd
 import time
-from datetime import datetime
+
+import pandas as pd
+import pendulum
+
+from .daq import RealEvent
 
 
-class FakeEvent(BaseModel):
+class FakeEvent(RealEvent):
     """擬似イベント用のクラス"""
 
-    timestamp: datetime = pendulum.now()
-    """タイムスタンプ。擬似イベントを生成した日時"""
-    top: int = 0
-    """topレイヤーの擬似ヒット。0 - 10のランダム値"""
-    mid: int = 0
-    """midレイヤーの擬似ヒット。0 - 10のランダム値"""
-    btm: int = 0
-    """btmレイヤーの擬似ヒット。0 - 10のランダム値"""
-    adc: int = 0
-    """topレイヤーにヒットがあったときのADC値。0 - 1023のランダム値"""
-    tmp: float = 0.0
-    """擬似イベントの気温。25度くらいのランダム値"""
-    atm: float = 0.0
-    """擬似イベントの気圧。1気圧（101800 Pa）くらいのランダム値"""
-    hmd: float = 0.0
-    """擬似イベントの湿度。50%くらいのランダム値"""
     seed: int | None = None
     """乱数シード。デフォルト値は`None`"""
     is_fake: bool = True
     """データ種類のフラグ。FakeEventオブジェクトは常に``True``に設定"""
 
     def model_post_init(self, __context) -> None:
         """メンバー変数を初期化する"""
@@ -58,17 +43,15 @@
         self.atm = random.gauss(mu=101000, sigma=1000) + random.gauss()
         self.hmd = random.gauss(mu=50, sigma=15) + random.gauss()
 
         if self.top > 0:
             self.adc = random.randint(1, 1024)
 
 
-def fake_events_generator(
-    n: int, seed: int | None = None, interval: str | int = "random"
-):
+def fake_events_generator(n: int, seed: int | None = None, interval: str | int = "random"):
     """指定した回数のFakeEventを任意の間隔で生成する
 
     :Args:
         - n (int): 生成するFakeEventの数
         - seed (int | None) : 乱数シード。デフォルトは `None`
         - interval (int | str) : 生成する間隔。デフォルトは "random"
```

### Comparing `haniwers-0.14.4/haniwers/postprocess.py` & `haniwers-0.15.0/haniwers/postprocess.py`

 * *Files identical despite different names*

### Comparing `haniwers-0.14.4/haniwers/preprocess.py` & `haniwers-0.15.0/haniwers/preprocess.py`

 * *Files identical despite different names*

### Comparing `haniwers-0.14.4/haniwers/threshold.py` & `haniwers-0.15.0/haniwers/threshold.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import numpy as np
 import pandas as pd
 import pendulum
 from loguru import logger
 from scipy.optimize import curve_fit
 from scipy.special import erfc
+from pydantic import BaseModel
 
 from .config import Daq
 from .daq import get_savef_with_timestamp, set_vth_retry, time_daq
 
 
 def scan_threshold_by_channel(daq: Daq, duration: int, ch: int, vth: int) -> list:
     """
@@ -68,29 +69,22 @@
 
 def scan_thresholds_in_serial(
     daq: Daq, duration: int, ch: int, thresholds: list[int]
 ) -> list[list]:
     """
     Run threshold scan for all channels by default.
 
-    Parameters
-    ----------
-    daq : Daq
-        Daqクラスのオブジェクトを指定します。
-    duration : int
-        測定時間を秒で指定します。
-    ch : int
-        測定するチャンネル番号を指定します。
-    thresholds : list[int]
-        測定するスレッショルド値をリストで指定します。
-
-    Returns
-    -------
-    list[list]
-        [測定時刻、チャンネル番号、スレッショルド値、イベント数]のリストです。
+    :Args:
+    - daq (Daq): Daqオブジェクト
+    - duration (int): 測定時間（秒）
+    - ch (int): チャンネル番号（1 - 3)
+    - thresholds (list[int])： 測定するスレッショルド値のリスト
+
+    :Returns:
+    - rows (list[list]):  [測定時刻、チャンネル番号、スレッショルド値、イベント数]のリスト
     """
 
     # Estimated time for scan
     msg = f"Number of points: {len(thresholds)}"
     logger.info(msg)
     estimated_time = len(thresholds) * duration
     msg = f"Estimated time: {estimated_time} sec."
@@ -109,23 +103,47 @@
         row = scan_threshold_by_channel(daq, duration, ch, vth)
         if row:
             rows.append(row)
 
     return rows
 
 
-def scan_thresholds_in_parallel(
-    daq: Daq, duration: int, ch: int, thresholds: list[int]
-):
-    pass
+def scan_thresholds_in_parallel(daq: Daq, duration: int, thresholds: list[int]):
+    # Estimated time for scan
+    msg = f"Number of points: {len(thresholds)}"
+    logger.info(msg)
+    estimated_time = len(thresholds) * duration
+    msg = f"Estimated time: {estimated_time} sec."
+    logger.info(msg)
+
+    n = len(thresholds)
+    for i, vth in enumerate(thresholds):
+        msg = "-" * 40 + f"[{i+1:2d}/{n:2d}: {vth}]"
+        logger.info(msg)
+        # すべてのチャンネルの閾値を設定
+        set_vth_retry(daq, 1, vth, 5)
+        set_vth_retry(daq, 2, vth, 5)
+        set_vth_retry(daq, 3, vth, 5)
+
+        try:
+            rows = time_daq(daq, duration)
+            counts = len(rows)
+            tmp = rows["tmp"].mean()
+            atm = rows["atm"].mean()
+            hmd = rows["hmd"].mean()
+            fname = get_savef_with_timestamp(daq, ch)
+            rows.to_csv(fname, index=False)
+            msg = f"Saved data to: {fname}"
+            logger.info(msg)
+        except Exception as e:
+            pass
+        # それっぽいものを作ってる途中
 
 
-def scan_thresholds(
-    daq: Daq, duration: int, ch: int, thresholds: list[int]
-) -> list[list]:
+def scan_thresholds(daq: Daq, duration: int, ch: int, thresholds: list[int]) -> list[list]:
     return scan_thresholds_in_serial(daq, duration, ch, thresholds)
 
 
 def erfc_function(x, a, b, c, d):
     """
     誤差補正関数（Error function complement）。
```

### Comparing `haniwers-0.14.4/pyproject.toml` & `haniwers-0.15.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool]
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.14.4"
+version = "0.15.0"
 tag_format = "$version"
 version_files = [
     "pyproject.toml:version",
     "haniwers/__init__.py:__version__",
 ]
 
 [tool.poetry]
 name = "haniwers"
-version = "0.14.4"
+version = "0.15.0"
 description = "Analysis tool for TanQ/FunQ project"
 authors = ["Shota Takahashi (KMI) <shotakaha@kmi.nagoya-u.ac.jp>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://qumasan.gitlab.io/haniwers/docs/"
 repository = "https://gitlab.com/qumasan/haniwers/"
 keywords = ["muon"]
@@ -53,13 +53,17 @@
 nodeenv = "^1.8.0"
 sphinx-autobuild = "^2024.2.4"
 sphinx-autodoc2 = "^0.5.0"
 
 [tool.poetry.group.dev.dependencies]
 commitizen = "^3.12.0"
 ruff = "^0.3.4"
-pytest = "^8.1.1"
+pytest = "^8.2.1"
 ipykernel = "^6.29.4"
 
+[tool.ruff]
+line-length = 100
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
```

### Comparing `haniwers-0.14.4/PKG-INFO` & `haniwers-0.15.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haniwers
-Version: 0.14.4
+Version: 0.15.0
 Summary: Analysis tool for TanQ/FunQ project
 Home-page: https://qumasan.gitlab.io/haniwers/docs/
 License: MIT
 Keywords: muon
 Author: Shota Takahashi (KMI)
 Author-email: shotakaha@kmi.nagoya-u.ac.jp
 Requires-Python: >=3.9,<3.13
@@ -32,14 +32,23 @@
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: typer (>=0.12.0,<0.13.0)
 Requires-Dist: vl-convert-python (>=1.1.0,<2.0.0)
 Project-URL: Repository, https://gitlab.com/qumasan/haniwers/
 Description-Content-Type: text/markdown
 
+
+
+![GitLab Tag](https://img.shields.io/gitlab/v/tag/qumasan%2Fhaniwers?sort=semver&style=for-the-badge) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/haniwers?style=for-the-badge) ![GitLab License](https://img.shields.io/gitlab/license/qumasan%2Fhaniwers?style=for-the-badge)
+![PyPI - Downloads](https://img.shields.io/pypi/dd/haniwers?style=for-the-badge) ![PyPI -Downloads](https://img.shields.io/pypi/dw/haniwers?style=for-the-badge) ![PyPI - Downloads](https://img.shields.io/pypi/dm/haniwers?style=for-the-badge)
+![Gitlab Pipeline Status](https://img.shields.io/gitlab/pipeline-status/qumasan%2Fhaniwers?style=for-the-badge) ![GitLab Last Commit](https://img.shields.io/gitlab/last-commit/qumasan%2Fhaniwers?style=for-the-badge)
+
+---
+
+
 # Haniwers : ハニワーズ
 
 墳Qの解析コード（個人用）
 
 ![w:300](../docs/_static/haniwer.png)
 
 # インストール
```

