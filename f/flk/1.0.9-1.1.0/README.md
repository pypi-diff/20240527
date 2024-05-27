# Comparing `tmp/flk-1.0.9.tar.gz` & `tmp/flk-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flk-1.0.9.tar", last modified: Fri May 24 10:54:19 2024, max compression
+gzip compressed data, was "flk-1.1.0.tar", last modified: Mon May 27 10:47:13 2024, max compression
```

## Comparing `flk-1.0.9.tar` & `flk-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 10:54:19.525843 flk-1.0.9/
--rw-rw-rw-   0        0        0    11558 2024-05-20 16:14:53.000000 flk-1.0.9/LICENSE
--rw-rw-rw-   0        0        0      306 2024-05-24 10:54:19.523333 flk-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     3429 2024-05-22 19:23:10.000000 flk-1.0.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 10:54:19.496611 flk-1.0.9/flk/
--rw-rw-rw-   0        0        0       31 2024-05-21 08:15:15.000000 flk-1.0.9/flk/__init__.py
--rw-rw-rw-   0        0        0     1199 2024-05-21 08:11:02.000000 flk-1.0.9/flk/__main__.py
--rw-rw-rw-   0        0        0    12339 2024-05-24 10:24:25.000000 flk-1.0.9/flk/parser.py
--rw-rw-rw-   0        0        0     1919 2024-05-24 10:32:33.000000 flk-1.0.9/flk/variable.py
-drwxrwxrwx   0        0        0        0 2024-05-24 10:54:19.522215 flk-1.0.9/flk.egg-info/
--rw-rw-rw-   0        0        0      306 2024-05-24 10:54:19.000000 flk-1.0.9/flk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2024-05-24 10:54:19.000000 flk-1.0.9/flk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 10:54:19.000000 flk-1.0.9/flk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-05-24 10:54:19.000000 flk-1.0.9/flk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 10:54:19.525843 flk-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0      383 2024-05-24 10:35:54.000000 flk-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:47:13.907931 flk-1.1.0/
+-rw-rw-rw-   0        0        0    11558 2024-05-20 16:14:53.000000 flk-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      306 2024-05-27 10:47:13.905934 flk-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4190 2024-05-27 10:42:22.000000 flk-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 10:47:13.896961 flk-1.1.0/flk/
+-rw-rw-rw-   0        0        0       31 2024-05-21 08:15:15.000000 flk-1.1.0/flk/__init__.py
+-rw-rw-rw-   0        0        0     1199 2024-05-21 08:11:02.000000 flk-1.1.0/flk/__main__.py
+-rw-rw-rw-   0        0        0    14924 2024-05-27 10:38:33.000000 flk-1.1.0/flk/parser.py
+-rw-rw-rw-   0        0        0     1919 2024-05-24 10:32:33.000000 flk-1.1.0/flk/variable.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:47:13.904935 flk-1.1.0/flk.egg-info/
+-rw-rw-rw-   0        0        0      306 2024-05-27 10:47:13.000000 flk-1.1.0/flk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2024-05-27 10:47:13.000000 flk-1.1.0/flk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 10:47:13.000000 flk-1.1.0/flk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2024-05-27 10:47:13.000000 flk-1.1.0/flk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 10:47:13.907931 flk-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      383 2024-05-27 10:45:22.000000 flk-1.1.0/setup.py
```

### Comparing `flk-1.0.9/LICENSE` & `flk-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flk-1.0.9/README.md` & `flk-1.1.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -23,26 +23,39 @@
 ```
 
 ## Быстрый старт
 
 ### Импорт и использование парсера
 
 ```python
+# Импортируем класс Parser из модуля flk
 from flk import Parser
 
+# Создаем экземпляр парсера
 parser = Parser()
 
+# Задаем имя переменной, значение которой мы хотим изменить
+variable_name = "num_1"
+
+# Парсим файл "example.fl" и анализируем его содержимое
 parser.parse_file("example.fl")
 
-variable_name = "my_int"
+# Изменяем значение переменной с именем, указанным в variable_name, на 3
+parser.edit_var_value(variable_name, 3)
+
+# Получаем объект переменной с именем, указанным в variable_name
 my_var = parser.get_var(variable_name)
 
+# Получаем тип переменной
 var_type = my_var.get_type()
+
+# Получаем значение переменной
 var_value = my_var.get_value()
 
+# Выводим информацию о переменной
 print(f"Тип переменной '{variable_name}': {var_type}")
 print(f"Значение переменной '{variable_name}': {var_value}")
 ```
 
 ### Командная строка
 
 Используйте FLK из командной строки:
```

### Comparing `flk-1.0.9/flk/__main__.py` & `flk-1.1.0/flk/__main__.py`

 * *Files identical despite different names*

### Comparing `flk-1.0.9/flk/parser.py` & `flk-1.1.0/flk/parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -187,14 +187,70 @@
                 raise ValueError(f"Неправильный формат строки: {line}")
 
         if name in self.data:
             self.data[name].set_value(parsed_value)
         else:
             self.data[name] = Variable(var_type, parsed_value)
 
+    def edit_var_value(self, var_name: str, new_var_value: str):
+        """
+        Изменяет значение переменной во всех файлах, включая импортированные.
+
+        Параметры:
+            var_name: Имя переменной.
+            new_var_value: Новое значение переменной.
+        """
+
+        if var_name in self.data:
+            var_type = self.data[var_name].get_type()
+            parsed_value = self.parse_value(var_type, new_var_value)
+            self.data[var_name].set_value(parsed_value)
+        else:
+            raise ValueError(f"Переменная {var_name} не найдена.")
+
+        self.update_file_var_value(self.current_file, var_name, new_var_value)
+
+    def update_file_var_value(self, file_path: str, var_name: str, new_var_value: str):
+        """
+        Изменяет значение переменной в указанном файле и его импортированных файлах.
+
+        Параметры:
+            file_path: Путь к файлу.
+            var_name: Имя переменной.
+            new_var_value: Новое значение переменной.
+        """
+
+        with open(file_path, 'r', encoding='utf-8') as file:
+            lines = file.readlines()
+
+        new_lines = []
+        var_assignment_pattern = re.compile(rf'(\b{var_name}\b)\((\w+)\) = (.+)')
+
+        for line in lines:
+            match = var_assignment_pattern.match(line.strip())
+            if match:
+                name, var_type, value = match.groups()
+                if name == var_name:
+                    new_line = f"{var_name}({var_type}) = {new_var_value}\n"
+                    new_lines.append(new_line)
+                    continue
+            new_lines.append(line)
+
+        with open(file_path, 'w', encoding='utf-8') as file:
+            file.writelines(new_lines)
+
+        with open(file_path, 'r', encoding='utf-8') as file:
+            for line in file:
+                if line.startswith('(import)'):
+                    import_path = line.strip().split(' ')[1].strip('()')
+                    import_file_path = f"{import_path.replace('.', '/')}.fl"
+                    full_import_file_path = os.path.join(os.path.dirname(file_path), import_file_path)
+                    self.update_file_var_value(full_import_file_path, var_name, new_var_value)
+
+
     def parse_logical_expression(self, expression: str) -> bool:
         """
         Парсит логическое выражение.
 
         Параметры:
             expression (str): Строка с логическим выражением.
 
@@ -224,15 +280,17 @@
             line (str): Строка, содержащая директиву импорта.
         """
         parts = line.strip().split(' ')
         if len(parts) > 1:
             import_path = parts[1].strip('()')
             path = f"{import_path.replace('.', '/')}.fl"
             full_path = os.path.join(os.path.dirname(self.current_file), path)
+            original_file = self.current_file
             self.parse_file(full_path)
+            self.current_file = original_file
         else:
             raise ValueError("Неправильный формат директивы импорта: " + line)
 
     def get_var(self, name: str) -> Variable:
         """
         Возвращает объект переменной по имени.
```

### Comparing `flk-1.0.9/flk/variable.py` & `flk-1.1.0/flk/variable.py`

 * *Files identical despite different names*

