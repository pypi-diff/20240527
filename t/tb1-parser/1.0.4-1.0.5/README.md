# Comparing `tmp/tb1_parser-1.0.4.tar.gz` & `tmp/tb1_parser-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tb1_parser-1.0.4.tar", last modified: Fri Apr 12 16:29:56 2024, max compression
+gzip compressed data, was "tb1_parser-1.0.5.tar", last modified: Mon May 27 17:57:04 2024, max compression
```

## Comparing `tb1_parser-1.0.4.tar` & `tb1_parser-1.0.5.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 16:29:56.258595 tb1_parser-1.0.4/
--rw-rw-rw-   0        0        0      272 2024-04-12 16:29:56.257592 tb1_parser-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-07 12:17:14.000000 tb1_parser-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-12 16:29:56.259591 tb1_parser-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      393 2024-04-12 16:29:40.000000 tb1_parser-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:29:56.247561 tb1_parser-1.0.4/tb1_parser/
--rw-rw-rw-   0        0        0      269 2024-04-12 16:17:57.000000 tb1_parser-1.0.4/tb1_parser/__init__.py
--rw-rw-rw-   0        0        0     5811 2024-04-12 16:29:19.000000 tb1_parser-1.0.4/tb1_parser/_ai_sheet_parser.py
--rw-rw-rw-   0        0        0     2132 2024-04-12 16:25:47.000000 tb1_parser-1.0.4/tb1_parser/_di_sheet_parser.py
--rw-rw-rw-   0        0        0     2218 2024-04-12 16:25:58.000000 tb1_parser-1.0.4/tb1_parser/_do_sheet_parser.py
--rw-rw-rw-   0        0        0     6197 2024-04-12 16:07:03.000000 tb1_parser-1.0.4/tb1_parser/_regex_lib.py
--rw-rw-rw-   0        0        0     4459 2024-04-12 16:26:08.000000 tb1_parser-1.0.4/tb1_parser/_sheet_parser.py
--rw-rw-rw-   0        0        0     1767 2024-04-07 14:02:43.000000 tb1_parser-1.0.4/tb1_parser/_tb1_file_reader.py
--rw-rw-rw-   0        0        0       48 2024-04-07 12:17:14.000000 tb1_parser-1.0.4/tb1_parser/_tb1_readed_sheets_collection.py
--rw-rw-rw-   0        0        0     9218 2024-04-07 12:17:14.000000 tb1_parser-1.0.4/tb1_parser/_tb1_sheet_reader.py
--rw-rw-rw-   0        0        0      540 2024-04-12 16:18:19.000000 tb1_parser-1.0.4/tb1_parser/ai_signal.py
--rw-rw-rw-   0        0        0      455 2024-04-12 16:18:08.000000 tb1_parser-1.0.4/tb1_parser/di_signal.py
--rw-rw-rw-   0        0        0      353 2024-04-12 16:18:02.000000 tb1_parser-1.0.4/tb1_parser/do_signal.py
--rw-rw-rw-   0        0        0       42 2024-04-12 15:31:09.000000 tb1_parser-1.0.4/tb1_parser/parsed_tb1_collection.py
--rw-rw-rw-   0        0        0      609 2024-04-12 15:31:09.000000 tb1_parser-1.0.4/tb1_parser/signal.py
--rw-rw-rw-   0        0        0       74 2024-04-12 15:31:09.000000 tb1_parser-1.0.4/tb1_parser/signals_collection.py
--rw-rw-rw-   0        0        0     1630 2024-04-12 16:27:27.000000 tb1_parser-1.0.4/tb1_parser/tb1_parser.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:29:56.256582 tb1_parser-1.0.4/tb1_parser.egg-info/
--rw-rw-rw-   0        0        0      272 2024-04-12 16:29:56.000000 tb1_parser-1.0.4/tb1_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      693 2024-04-12 16:29:56.000000 tb1_parser-1.0.4/tb1_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 16:29:56.000000 tb1_parser-1.0.4/tb1_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-12 16:29:56.000000 tb1_parser-1.0.4/tb1_parser.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       26 2024-04-12 16:29:56.000000 tb1_parser-1.0.4/tb1_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-12 16:29:56.000000 tb1_parser-1.0.4/tb1_parser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 17:57:04.334051 tb1_parser-1.0.5/
+-rw-rw-rw-   0        0        0      272 2024-05-27 17:57:04.334051 tb1_parser-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-07 12:17:14.000000 tb1_parser-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-27 17:57:04.336050 tb1_parser-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      395 2024-05-27 17:54:49.000000 tb1_parser-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 17:57:04.326061 tb1_parser-1.0.5/tb1_parser/
+-rw-rw-rw-   0        0        0      269 2024-04-12 16:17:57.000000 tb1_parser-1.0.5/tb1_parser/__init__.py
+-rw-rw-rw-   0        0        0     5808 2024-05-18 09:53:13.000000 tb1_parser-1.0.5/tb1_parser/_ai_sheet_parser.py
+-rw-rw-rw-   0        0        0     2032 2024-05-18 09:53:13.000000 tb1_parser-1.0.5/tb1_parser/_di_sheet_parser.py
+-rw-rw-rw-   0        0        0     2098 2024-05-18 09:53:13.000000 tb1_parser-1.0.5/tb1_parser/_do_sheet_parser.py
+-rw-rw-rw-   0        0        0     6283 2024-05-18 09:53:13.000000 tb1_parser-1.0.5/tb1_parser/_regex_lib.py
+-rw-rw-rw-   0        0        0     2655 2024-05-18 19:36:19.000000 tb1_parser-1.0.5/tb1_parser/_sheet_parser.py
+-rw-rw-rw-   0        0        0     1769 2024-05-18 09:53:13.000000 tb1_parser-1.0.5/tb1_parser/_tb1_file_reader.py
+-rw-rw-rw-   0        0        0       50 2024-05-18 09:53:13.000000 tb1_parser-1.0.5/tb1_parser/_tb1_readed_sheets_collection.py
+-rw-rw-rw-   0        0        0     9149 2024-05-18 09:53:13.000000 tb1_parser-1.0.5/tb1_parser/_tb1_sheet_reader.py
+-rw-rw-rw-   0        0        0      629 2024-05-18 09:53:13.000000 tb1_parser-1.0.5/tb1_parser/ai_signal.py
+-rw-rw-rw-   0        0        0      517 2024-05-18 09:53:13.000000 tb1_parser-1.0.5/tb1_parser/di_signal.py
+-rw-rw-rw-   0        0        0      341 2024-05-18 09:53:13.000000 tb1_parser-1.0.5/tb1_parser/do_signal.py
+-rw-rw-rw-   0        0        0       44 2024-05-18 09:53:13.000000 tb1_parser-1.0.5/tb1_parser/parsed_tb1_collection.py
+-rw-rw-rw-   0        0        0      389 2024-05-18 09:53:13.000000 tb1_parser-1.0.5/tb1_parser/plc_module.py
+-rw-rw-rw-   0        0        0      838 2024-05-18 09:53:13.000000 tb1_parser-1.0.5/tb1_parser/signal.py
+-rw-rw-rw-   0        0        0       76 2024-05-18 09:53:13.000000 tb1_parser-1.0.5/tb1_parser/signals_collection.py
+-rw-rw-rw-   0        0        0     1630 2024-04-12 16:27:27.000000 tb1_parser-1.0.5/tb1_parser/tb1_parser.py
+drwxrwxrwx   0        0        0        0 2024-05-27 17:57:04.333051 tb1_parser-1.0.5/tb1_parser.egg-info/
+-rw-rw-rw-   0        0        0      272 2024-05-27 17:57:04.000000 tb1_parser-1.0.5/tb1_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      718 2024-05-27 17:57:04.000000 tb1_parser-1.0.5/tb1_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 17:57:04.000000 tb1_parser-1.0.5/tb1_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-12 16:29:56.000000 tb1_parser-1.0.5/tb1_parser.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       26 2024-05-27 17:57:04.000000 tb1_parser-1.0.5/tb1_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-27 17:57:04.000000 tb1_parser-1.0.5/tb1_parser.egg-info/top_level.txt
```

### Comparing `tb1_parser-1.0.4/tb1_parser/_ai_sheet_parser.py` & `tb1_parser-1.0.5/tb1_parser/_ai_sheet_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from pandas import DataFrame
 
 from tb1_parser import AiSignal, SignalsCollection
 
 from ._regex_lib import TB1
 from ._sheet_parser import SheetParser
 
-
 config = TB1['Ai']['regex']
 
 
 class AiSheetParser(SheetParser):
 
     def __init__(self, sheet: DataFrame) -> None:
         self._logs_owner: str = self.__class__.__name__
@@ -94,28 +93,32 @@
     def start(self) -> None:
         if not list(config['columns']['validate']['names'].keys()) == list(self._sheet):
             logging.error(f'{self._logs_owner}: передан неверный лист аналоговых сигналов')
 
         out = []
 
         for row in self._sheet.itertuples(False, 'Signal'):
+            new = AiSignal()
+            
             try:
-                new = AiSignal()
                 new.plc_module = self._parse_plc_module(row.plc_module)
                 new.plc_channel = int(row.plc_channel)
-                new.variable = self._parse_variable(row.variable, row.plc_module)
+                new.variable = self._parse_variable(row.variable)
                 new.name = self._clean_name(row.name)
-                new.formated_name = self._format_signal_name(row.name)
+                # new.formated_name = self._format_signal_name(row.name)
                 new.unit = row.unit if row.unit else self.__find_unit(row.range)
                 new.LL, new.HL = self.__parse_range(row.range)
                 new.LW, new.HW = self.__parse_range(row.warning_range)
                 new.LA, new.HA = self.__parse_range(row.alarm_range)
                 new.LE, new.HE = self.__parse_range(row.error_range)
                 # TODO Написать валидацию границ уставок
 
-                out.append(new)
                 logging.info(f'{self._logs_owner}:{row.variable}: значения успешно получены')
+
             except Exception as error:
                 logging.error(f'{self._logs_owner}:{row.variable}: ошибка парсинга - {error}')
+
+            finally:
                 out.append(new)
+        
         self._result = SignalsCollection(out)
         self._result.signals_type = 'Ai'
```

### Comparing `tb1_parser-1.0.4/tb1_parser/_di_sheet_parser.py` & `tb1_parser-1.0.5/tb1_parser/_di_sheet_parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,39 +13,42 @@
     def __init__(self, sheet: DataFrame) -> None:
         self._logs_owner: str = self.__class__.__name__
         self._sheet = sheet
 
         self._result = None
 
 
-    # REFACT Переписать метод парсинга наличия сигналов
     def __parse_signal(self, input_value: str) -> bool:
         return '+' in input_value
 
 
     def start(self) -> None:
         if not list(config['Di']['regex']['columns']['validate']['names'].keys()) == list(self._sheet):
             logging.error(f'{self._logs_owner}: передан неверный лист аналоговых сигналов')
 
         out = []
 
         for row in self._sheet.itertuples(False, 'Signal'):
+            new = DiSignal()
+
             try:
-                new = DiSignal()
                 new.plc_module = self._parse_plc_module(row.plc_module)
                 new.plc_channel = int(row.plc_channel)
-                new.variable = self._parse_variable(row.variable, row.plc_module)
+                new.variable = self._parse_variable(row.variable)
                 new.name = self._clean_name(row.name)
-                new.formated_name = self._format_signal_name(row.name)
+                # new.formated_name = self._format_signal_name(row.name)
                 new.logic_value = self._parse_logic_value(row.logic_value)
                 new.alarm_signal = self.__parse_signal(row.alarm_signal)
                 new.warning_signal = self.__parse_signal(row.warning_signal)
                 new.error_signal = self.__parse_signal(row.error_signal)
                 new.tele_signal = self.__parse_signal(row.tele_signal)
 
-                out.append(new)
                 logging.info(f'{self._logs_owner}:{row.variable}: значения успешно получены')
+
             except Exception as error:
                 logging.error(f'{self._logs_owner}:{row.variable}: ошибка парсинга - {error}')
+
+            finally:
                 out.append(new)
+                
         self._result = SignalsCollection(out)
         self._result.signals_type = 'Di'
```

### Comparing `tb1_parser-1.0.4/tb1_parser/_do_sheet_parser.py` & `tb1_parser-1.0.5/tb1_parser/_do_sheet_parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     def __init__(self, sheet: DataFrame) -> None:
         self._logs_owner: str = self.__class__.__name__
         self._sheet = sheet
 
         self._result = None
 
 
-    # REFACT Переписать и отдебажить метод парсинга логического значения
     def _parse_logic_value(self, input_value: str | int):
         input_value = str(input_value)
         try:
             out = int(input_value)
         except Exception as exception:
             if input_value != 'нет':
                 logging.error(f'{self._logs_owner}: ошибка парсинга логического значения "{input_value}" - {exception}')
@@ -33,23 +32,27 @@
     def start(self) -> None:
         if not list(config['Do']['regex']['columns']['validate']['names'].keys()) == list(self._sheet):
             logging.error(f'{self._logs_owner}: передан неверный лист аналоговых сигналов')
 
         out = []
 
         for row in self._sheet.itertuples(False, 'Signal'):
+            new = DoSignal()
+
             try:
-                new = DoSignal()
                 new.plc_module = self._parse_plc_module(row.plc_module)
                 new.plc_channel = int(row.plc_channel)
-                new.variable = self._parse_variable(row.variable, row.plc_module)
+                new.variable = self._parse_variable(row.variable)
                 new.name = self._clean_name(row.name)
-                new.formated_name = self._format_signal_name(row.name)
+                # new.formated_name = self._format_signal_name(row.name)
                 new.logic_value = self._parse_logic_value(row.logic_value)
 
-                out.append(new)
                 logging.info(f'{self._logs_owner}:{row.variable}: значения успешно получены')
+
             except Exception as error:
                 logging.error(f'{self._logs_owner}:{row.variable}: ошибка парсинга - {error}')
+            
+            finally:
                 out.append(new)
+                
         self._result = SignalsCollection(out)
         self._result.signals_type = 'Do'
```

### Comparing `tb1_parser-1.0.4/tb1_parser/_regex_lib.py` & `tb1_parser-1.0.5/tb1_parser/_regex_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,10 +133,11 @@
             'Давление': 'P',
             'Перепад давления': 'dP',
             'Ток': 'I',
             'Напряжение': 'U',
             'Уровень': 'L'
         },
         # 'find_plc_module': r'^\w{2}\-[a-z0-9-]+\,?\s+?\(?(\w(\d+).?(\d+))\)?$'
-        'find_plc_module': r'([IOAD]+.?\d+\D+\d+)\D{0,}\(?(\w\d+\-\d+)\)?'
+        # 'find_plc_module': r'([IOAD]+.?\d+\D+\d+)\D{0,}\(?(\w\d+\-\d+)\)?'
+        'find_plc_module': r'([IOAD]+).?(\d+)\w\D?(\d+)\S?\s{0,}\(?(\w\d+.\d+)\)?'
     }
 }
```

### Comparing `tb1_parser-1.0.4/tb1_parser/_sheet_parser.py` & `tb1_parser-1.0.5/tb1_parser/_sheet_parser.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,105 +3,71 @@
 
 from pandas import DataFrame
 from transliterate import translit
 
 from tb1_parser import SignalsCollection
 
 from ._regex_lib import PARSER as config
+from .plc_module import PLCModule
 
 
 class SheetParser:
 
     def __init__(self, sheet: DataFrame) -> None:
         self._logs_owner: str = self.__class__.__name__
         self._sheet = sheet
 
         self._result = None
 
 
     def _clean_name(self, input_value: str):
-        return input_value.replace('\n', '')
+        return input_value.strip().replace('\n', '')
 
 
-    # REFACT Отрефакторить метод поиска количества каналов для модуля
-    def _find_count_plc_channels(self, raw_plc_module: str):
-        try:
-            sheet: DataFrame = self._sheet
-            count: int = len(sheet[sheet['plc_module'] == raw_plc_module])
-            return count
-        except Exception as exception:
-            pass
-        finally:
-            pass
-
+    def _parse_variable(self, raw_variable: str) -> str:
+        return translit(raw_variable, 'ru', reversed=True)
 
-    # def _parse_variable(self, raw_variable: str, raw_plc_module: str) -> int | tuple[int]:
-    #     type_regex = r'^\D{2}'
-    #     clean_input = lambda x: re.sub(type_regex, '', x)
-    #     clear_variable = clean_input(raw_variable)
+    
+    # REFACT Переписать метод транслитерациии названия параметра
+    # def _format_signal_name(self, name: str) -> str:
+    #     replace_data = config['signals']['format_variable_name']
     #     try:
-    #         if 'ai' in raw_variable.lower():
-    #             out = int(clear_variable)
-    #         else:
-    #             out = nums = tuple(map(int, clear_variable.split('-')))
-
-    #     except ValueError as value_error:
-    #         logging.warning(f'{self._logs_owner}: некорректный номер переменной "{raw_variable}"')
-    #         count_plc_channels = self._find_count_plc_channels(raw_plc_module)
-    #         nums = tuple(map(int, clear_variable.split('-')))
-
-    #         if len(nums) == 2:
-    #             logging.info(f'{self._logs_owner}: вычисление порядкового номера "{raw_variable}"')
-    #             out = count_plc_channels * nums[0] + nums[1]
-    #             logging.warning(f'{self._logs_owner}: номер переменной "{raw_variable}" принудительно нормализован - "{out}"')
-    #         else:
-    #             raise ValueError('попытка вычисления порядкового номера переменной провалена')
-            
-    #     except Exception as exception:
-    #         logging.error(f'{self._logs_owner}: ошибка парсинга "{raw_variable}" переменной - {type(exception).__name__}:{exception}')
+    #         for key, value in replace_data.items():
+    #             name = re.sub(key, value, name)
+    #         name = translit(name, 'ru', reversed=True)
+    #         name = re.split(r'\s+|\-|\,', name)
+    #         name = (word for word in name if word != '')
+    #         name = '_'.join(name).replace('\'', '')
+    #         out: str = name
+    #     except Exception as error:
+    #         logging.error(f'{self._logs_owner}: ошибка транслитерации "{name}" названия параметра - {error}')
     #         out = None
-
     #     finally:
     #         return out
-
-
-    # FIXME Заглушка метода парсинга переменной сигнала
-    def _parse_variable(self, raw_variable: str, _):
-        return raw_variable
-
-    
-    # REFACT Переписать метод транслитерациии названия параметра
-    def _format_signal_name(self, name: str) -> str:
-        replace_data = config['signals']['format_variable_name']
-        try:
-            for key, value in replace_data.items():
-                name = re.sub(key, value, name)
-            name = translit(name, 'ru', reversed=True)
-            name = re.split(r'\s+|\-|\,', name)
-            name = (word for word in name if word != '')
-            name = '_'.join(name).replace('\'', '')
-            out: str = name
-        except Exception as error:
-            logging.error(f'{self._logs_owner}: ошибка транслитерации "{name}" названия параметра - {error}')
-            out = None
-        finally:
-            return out
     
 
     def _parse_plc_module(self, raw_string: str) -> str:
         try:
-            out = re.findall(config['signals']['find_plc_module'], raw_string)[0]
-            if not out:
+            raw_string = translit(raw_string, 'ru', reversed=True)
+            params = re.findall(config['signals']['find_plc_module'], raw_string)[0]
+
+            if len(params) != 4:
                 raise ValueError('ошибка сопоставления с шаблоном')
+            
+            out = PLCModule()
+            out.type, out.module = params[::3]
+            out.channels_count, out.some_num = map(int, params[1:3])
+            
         except Exception as error:
             logging.error(f'{self._logs_owner}: ошибка парсинга "{raw_string.replace('\n', '')}" модуля плк - {error}')
             out = None
+
         finally:
             return out
 
-
+ 
     def get_result(self) -> SignalsCollection | None:
         if out := self._result:
             return out
         else:
             logging.error(f'{self._logs_owner}: перед получением результатов парсинга воспользуйтесь методом start()')
-            raise IndentationError
+            raise IndentationError
```

### Comparing `tb1_parser-1.0.4/tb1_parser/_tb1_file_reader.py` & `tb1_parser-1.0.5/tb1_parser/_tb1_file_reader.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -48,8 +48,8 @@
             for sheet in sheets:
                 self.sheets[sheet] = sheet_reader.get(sheet)
         if isinstance(sheets, str):
             self.sheets[sheets] = sheet_reader.get(sheets)
 
 
     def get(self, sheet: Literal['Ai', 'Di', 'Do']):
-        return self.sheets.get(sheet)
+        return self.sheets.get(sheet)
```

### Comparing `tb1_parser-1.0.4/tb1_parser/_tb1_sheet_reader.py` & `tb1_parser-1.0.5/tb1_parser/_tb1_sheet_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                 raise ValueError(f'некорректное число совпадений с шаблоном ({matches_count})')
             
         except Exception as error:
             logging.error(f'{self.__logs_owner}:{content_type}: ошибка поиска названия листа - {error}')
             return
     
 
-    def __find_sheet_columns(self, content_type: str, dataframe_head: list[list]) -> dict[str:int]: # REFACT Переписать метод поиска столбцов
+    def __find_sheet_columns(self, content_type: str, dataframe_head: list[list]) -> dict[str:int]:
         '''
         Приватный метод для поиска индексов колонок конкреного листа ТБ1, перечисленных в либе регулярок.\n
         На входе тип содержимого листа и датафрейм из его шапки с названиями колонок.
         На выходе словарь с нормальизованными названиями колонок и их индексы.
         '''
 
         logging.info(f'{self.__logs_owner}:{content_type}: поиск столбцов для чтения..')
@@ -154,8 +154,8 @@
                 sheet[empty_col] = None
         sheet = sheet[[*columns]].copy()
 
         return sheet
 
 
     def get(self, content_type: str) -> None | DataFrame:
-        return self.__read_sheet(content_type)
+        return self.__read_sheet(content_type)
```

### Comparing `tb1_parser-1.0.4/tb1_parser/signal.py` & `tb1_parser-1.0.5/tb1_parser/ai_signal.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from dataclasses import dataclass
+from .signal import Signal
 
 
-@dataclass
-class Signal(object):
-    
+class AiSignal(Signal):
+
     def __init__(self) -> None:
         '''
-        Дата-класс. Шаблон для наследования.
+        Дата-класс для аналоговых входных сигналов, потомок 'Signal'.
         '''
-        self.variable: None | str
-        self.name: None | str
-        self.formated_name: None | str
-        self.plc_module: None | int | tuple[int]
-        self.plc_channel: None | int
-
+        super().__init__()
+        self.unit: None | str
+        self.LL: None | float
+        self.LA: None | float
+        self.LW: None | float
+        self.HW: None | float
+        self.HA: None | float
+        self.HL: None | float
+        self.LE: None | float
+        self.HE: None | float
 
-    def __repr__(self) -> str:
-        return f'{self.__class__.__name__}({str(self.__dict__)[1:-1]})'
-    
 
-    def isreserv(self) -> bool:
-        return self.name.lower() == 'резерв'
+    def isprotected(self) -> bool:
+        return (self.LA or self.HA) is not None
```

### Comparing `tb1_parser-1.0.4/tb1_parser/tb1_parser.py` & `tb1_parser-1.0.5/tb1_parser/tb1_parser.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-1.0.4/tb1_parser.egg-info/SOURCES.txt` & `tb1_parser-1.0.5/tb1_parser.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 tb1_parser/_tb1_file_reader.py
 tb1_parser/_tb1_readed_sheets_collection.py
 tb1_parser/_tb1_sheet_reader.py
 tb1_parser/ai_signal.py
 tb1_parser/di_signal.py
 tb1_parser/do_signal.py
 tb1_parser/parsed_tb1_collection.py
+tb1_parser/plc_module.py
 tb1_parser/signal.py
 tb1_parser/signals_collection.py
 tb1_parser/tb1_parser.py
 tb1_parser.egg-info/PKG-INFO
 tb1_parser.egg-info/SOURCES.txt
 tb1_parser.egg-info/dependency_links.txt
 tb1_parser.egg-info/not-zip-safe
```

