# Comparing `tmp/examon_pcep_package-0.2.2.tar.gz` & `tmp/examon_pcep_package-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "examon_pcep_package-0.2.2.tar", max compression
+gzip compressed data, was "examon_pcep_package-0.4.0.tar", max compression
```

## Comparing `examon_pcep_package-0.2.2.tar` & `examon_pcep_package-0.4.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       23 2023-09-02 13:03:57.173068 examon_pcep_package-0.2.2/examon_pcep_package/__init__.py
--rw-r--r--   0        0        0     9986 2023-09-16 14:01:19.963646 examon_pcep_package-0.2.2/examon_pcep_package/questions.py
--rw-r--r--   0        0        0      333 2023-10-14 13:45:40.317543 examon_pcep_package-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      344 1970-01-01 00:00:00.000000 examon_pcep_package-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       23 2023-09-02 13:03:57.173068 examon_pcep_package-0.4.0/examon_pcep_package/__init__.py
+-rw-r--r--   0        0        0     8789 2024-05-20 05:54:17.674026 examon_pcep_package-0.4.0/examon_pcep_package/questions.py
+-rw-r--r--   0        0        0      333 2024-05-20 05:32:02.077983 examon_pcep_package-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      344 1970-01-01 00:00:00.000000 examon_pcep_package-0.4.0/PKG-INFO
```

### Comparing `examon_pcep_package-0.2.2/examon_pcep_package/questions.py` & `examon_pcep_package-0.4.0/examon_pcep_package/questions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,28 @@
-from examon_core.examon_item import examon_item
+from examon_core.examon import examon
+from examon_core.global_settings import ExamonGlobalSettings
 
 REPOSITORY = 'examon_pcep_package'
+ExamonGlobalSettings.repository = REPOSITORY
 
 
-@examon_item(choices=['ace', 'ab', 'ef', 'bdf'],
-             tags=['PCEP', 'slicing', 'yield', '+'],
-             repository=REPOSITORY)
+@examon(choices=['ace', 'ab', 'ef', 'bdf'], tags=['PCEP'])
 def question01():
     def func(data):
         for d in data[::2]:
             yield d
 
     result = ''
     for x in func('abcdef'):
         result = result + x
 
     return result
 
 
-@examon_item(choices=['1', '2', '3', '4'],
-             tags=['PCEP', 'if', 'elif',
-                   'or', 'operator_precedence'],
-             repository=REPOSITORY)
+@examon(choices=['1', '2', '3', '4'], tags=['PCEP'])
 def question03():
     x = True
     y = False
     z = False
 
     print('Hi')
 
@@ -35,399 +32,398 @@
         return 2
     elif not x or y or not y and x:
         return 3
     else:
         return 4
 
 
-@examon_item(choices=['*', '**', '***', '****'], tags=['PCEP', '-=', '+', '=='],
-             repository=REPOSITORY)
+@examon(choices=['*', '**', '***', '****'], tags=['PCEP'])
 def question01():
     output = ''
     i = 4
     while i > 0:
         i -= 2
         output = output + '*'
         if i == 2:
             break
     else:
         output = output + '*'
     return len(output)
 
 
-@examon_item(choices=['3', '4', '5', '2'], tags=['PCEP', 'list_insert', 'del', 'sum'],
-             repository=REPOSITORY)
+@examon(choices=['3', '4', '5', '2'], tags=['PCEP', 'list_insert', 'del', 'sum'],
+             )
 def question01():
     x = [0, 1, 2]
     x.insert(0, 1)
     del x[1]
     return sum(x)
 
 
-@examon_item(choices=['2', '1', 'None'], tags=['PCEP', '%', '!=', 'ternary'],
-             repository=REPOSITORY)
+@examon(choices=['2', '1', 'None'], tags=['PCEP', '%', '!=', 'ternary'],
+             )
 def question01():
     def func(x):
         return 1 if x % 2 != 0 else 2
 
     return func(func(1))
 
 
-@examon_item(choices=['1,1,1', '1, 1, 1', '[1, 1, 1]'], tags=['PCEP'],
-             repository=REPOSITORY)
+@examon(choices=['1,1,1', '1, 1, 1', '[1, 1, 1]'], tags=['PCEP'],
+             )
 def question01():
     z = y = x = '1'
     return ','.join([x, y, z])
 
 
-@examon_item(choices=['**,**', '**,**,**'], tags=['PCEP', 'range', 'list.append'],
-             repository=REPOSITORY)
+@examon(choices=['**,**', '**,**,**'], tags=['PCEP', 'range', 'list.append'],
+             )
 def question01():
     l = []
     for i in range(1, 3):
         l.append(str(i) * 2)
 
     return ','.join(l)
 
 
-@examon_item(choices=['-1', '2', '0'], tags=['PCEP', '%', 'ZeroDivision'],
-             repository=REPOSITORY)
+@examon(choices=['-1', '2', '0'], tags=['PCEP', '%', 'ZeroDivision'],
+             )
 def question01():
     try:
         return 2 % 0
     except:
         return -1
 
 
-@examon_item(choices=["<class 'float'>", "<class 'decimal'>"], tags=['PCEP', '/', '__class__'],
-             repository=REPOSITORY)
+@examon(choices=["<class 'float'>", "<class 'decimal'>"], tags=['PCEP', '/', '__class__'],
+             )
 def question01():
     return (2 / 2).__class__
 
 
-@examon_item(choices=['True', 'False', 'None'], tags=['PCEP', 'not', 'in', 'list'],
-             repository=REPOSITORY)
+@examon(choices=['True', 'False', 'None'], tags=['PCEP', 'not', 'in', 'list'],
+             )
 def question01():
     return 0 not in [False, True, "2", 3, 4, 5]
 
 
-@examon_item(choices=['1', '2', '3', '4'], tags=['PCEP', 'dict', 'for'],
-             repository=REPOSITORY)
+@examon(choices=['1', '2', '3', '4'], tags=['PCEP', 'dict', 'for'],
+             )
 def question01():
     d = {}
     d['1'] = 2
     d[1] = 1
     d[1] += 1
 
     sum = 0
 
     for k in d:
         sum += d[k]
 
     return sum
 
 
-@examon_item(choices=[17.5, 8, 17, 8.5], tags=['PCEP', '/', '//', '**'],
-             repository=REPOSITORY)
+@examon(choices=[17.5, 8, 17, 8.5], tags=['PCEP', '/', '//', '**'],
+             )
 def question01():
     return 1 / 2 + 3 // 3 + 4 ** 2
 
 
-@examon_item(choices=['3011.0', '3011', '60.22', '60'], tags=['PCEP', 'exponential'],
-             repository=REPOSITORY)
+@examon(choices=['3011.0', '3011', '60.22', '60'], tags=['PCEP', 'exponential'],
+             )
 def question01():
     return 30.11E2
 
 
-@examon_item(choices=['0o213'], tags=['PCEP', 'octal'],
-             repository=REPOSITORY)
+@examon(choices=['0o213'], tags=['PCEP', 'octal'],
+             )
 def question01():
     return 0o213
 
 
-@examon_item(choices=[[0.6, 0], [0, 0.6],
+@examon(choices=[[0.6, 0], [0, 0.6],
                       [0.0, 0.6]], tags=['PCEP', '/', '//'],
-             repository=REPOSITORY)
+             )
 def question01():
     return [3 / 5, 3 // 5]
 
 
-@examon_item(choices=['14', '134', '1', '13'], tags=['PCEP', '<', '>'],
-             repository=REPOSITORY)
+@examon(choices=['14', '134', '1', '13'], tags=['PCEP', '<', '>'],
+             )
 def question01():
     x = 1
     result = []
     if x > 0 or x < 1:
         result.append("1")
     if x > 1:
         result.append("2")
     elif x >= 1:
         result.append("3")
     else:
         result.append("4")
     return ''.join(result)
 
 
-@examon_item(choices=['True', 'False'], tags=['PCEP', '__add__', 'tuple'],
-             repository=REPOSITORY)
+@examon(choices=['True', 'False'], tags=['PCEP', '__add__', 'tuple'],
+             )
 def question01():
     try:
         a = (1, 2, 3) + (2, 3, 4)
         return True
     except:
         return False
 
 
-@examon_item(choices=['[True, True, True, True]'], tags=['PCEP', 'bool', 'str'],
-             repository=REPOSITORY)
+@examon(choices=['[True, True, True, True]'], tags=['PCEP', 'bool', 'str'],
+             )
 def question01():
     w = str(bool(23))
     x = str(bool(''))
     y = str(bool(' '))
     z = str(bool([False]))
     return ','.join([w, x, y, z])
 
 
-@examon_item(choices=['404,3.02', '404,3.02,99',
+@examon(choices=['404,3.02', '404,3.02,99',
                       '1,404,3.02'], tags=['PCEP', 'slicing'],
-             repository=REPOSITORY)
+             )
 def question01():
     data = ['1', '404', '3.02', '99', '33']
     return ','.join(data[1:3])
 
 
-@examon_item(choices=[0.2, 0, 0.4, 0.0], tags=['PCEP', '//', '/', '+', 'operator_precedence'],
-             repository=REPOSITORY)
+@examon(choices=[0.2, 0, 0.4, 0.0], tags=['PCEP', '//', '/', '+', 'operator_precedence'],
+             )
 def question01():
     return 1 // 5 + 1 / 5
 
 
-@examon_item(choices=['OK', "Too bad...", "Sorry, something went wrong..."],
+@examon(choices=['OK', "Too bad...", "Sorry, something went wrong..."],
              tags=['PCEP', 'ValueError', 'ZeroDivisionError', 'except'],
-             repository=REPOSITORY)
+             )
 def question01():
     try:
         print(5 / 0)
         return 'OK'
     except (ValueError, ZeroDivisionError):
         return "Too bad..."
     except:
         return "Sorry, something went wrong..."
 
 
-@examon_item(choices=['1 42', '3 1', '3 42', '1 1'], tags=['PCEP', 'referencing'],
-             repository=REPOSITORY)
+@examon(choices=['1 42', '3 1', '3 42', '1 1'], tags=['PCEP', 'referencing'],
+             )
 def question01():
     def func(p1, p2):
         p1 = 1
         p2[0] = 42
 
     x = 3
     y = [1, 2, 3]
 
     func(x, y)
 
     return ' '.join([str(x), str(y[0])])
 
 
-@examon_item(choices=[[1, 1, 2], [2, 1, 2], [1, 2, 2]], tags=['PCEP', 'multiple_assignment'],
-             repository=REPOSITORY)
+@examon(choices=[[1, 1, 2], [2, 1, 2], [1, 2, 2]], tags=['PCEP', 'multiple_assignment'],
+             )
 def question01():
     x = 1
     y = 2
     x, y, z = x, x, y
     z, y, z = x, y, z
     return [x, y, z]
 
 
-@examon_item(choices=[''], tags=['PCEP', '+=', 'range'],
-             repository=REPOSITORY)
+@examon(choices=[''], tags=['PCEP', '+=', 'range'],
+             )
 def question01():
     def func(num):
         res = '*'
         for _ in range(num):
             res += res
         return res
 
     return func(2)
 
 
-@examon_item(choices=[[1, 1], [2, 1], [1, 2], [2, 2]],
+@examon(choices=[[1, 1], [2, 1], [1, 2], [2, 2]],
              tags=['PCEP', 'len', 'escape_characters'],
-             repository=REPOSITORY)
+             )
 def question01():
     return [len('\''), len("\"")]
 
 
-@examon_item(choices=['12', '21', '(1,2)', '(2,1)'], tags=['PCEP', 'dict', 'dict.keys'],
-             repository=REPOSITORY)
+@examon(choices=['12', '21', '(1,2)', '(2,1)'], tags=['PCEP', 'dict', 'dict.keys'],
+             )
 def question01():
     dct = {'1': (1, 2), '2': (2, 1)}
 
     result = []
     for x in dct.keys():
         result.append(dct[x][1])
     return result
 
 
-@examon_item(choices=['123', '123.0'], tags=['PCEP', '+'],
-             repository=REPOSITORY)
+@examon(choices=['123', '123.0'], tags=['PCEP', '+'],
+             )
 def question01():
     return 123 + 0.0
 
 
-@examon_item(choices=['1', '0'], tags=['PCEP', 'not', 'or', 'truthy'],
-             repository=REPOSITORY)
+@examon(choices=['1', '0'], tags=['PCEP', 'not', 'or', 'truthy'],
+             )
 def question01():
     a = 1
     b = 0
     x = a or b
     y = not (a and b)
     print(x + y)
 
 
-@examon_item(choices=['0', 'None'], tags=['PCEP', 'or', 'truthy'],
-             repository=REPOSITORY)
+@examon(choices=['0', 'None'], tags=['PCEP', 'or', 'truthy'],
+             )
 def question01():
     return 0 or 0
 
 
-@examon_item(choices=[[True, True], [False, True], [True, False], [False, False]],
+@examon(choices=[[True, True], [False, True], [True, False], [False, False]],
              tags=['PCEP', 'referencing', 'slicing', 'del'],
-             repository=REPOSITORY)
+             )
 def question01():
     nums = [1, 2, 3]
     vals = nums
     del vals[1:2]
     return [len(vals) == len(nums), vals == nums]
 
 
-@examon_item(choices=['[1, 4]', '[4, 3]', '[1, 3, 4]', '[1, 3]'],
+@examon(choices=['[1, 4]', '[4, 3]', '[1, 3, 4]', '[1, 3]'],
              tags=['PCEP', 'referencing', 'list'],
-             repository=REPOSITORY)
+             )
 def question01():
     list1 = [1, 3]
     list2 = list1
     list1[0] = 4
     return list2
 
 
-@examon_item(choices=['one', 'two', 'three'], tags=['PCEP', 'dict', 'range'],
-             repository=REPOSITORY)
+@examon(choices=['one', 'two', 'three'], tags=['PCEP', 'dict', 'range'],
+             )
 def question01():
     dictionary = {'one': 'two', 'three': 'one', 'two': 'three'}
     v = dictionary['one']
 
     for k in range(len(dictionary)):
         v = dictionary[v]
 
     return v
 
 
-@examon_item(choices=['1, 1', '1, 2', '2, 1', '2, 2'],
+@examon(choices=['1, 1', '1, 2', '2, 1', '2, 2'],
              tags=['PCEP', '-'],
-             repository=REPOSITORY)
+             )
 def question01():
     x = 1
     y = 2
     z = x
     x = y
     y = z
     return f'{x}, {y}'
 
 
-@examon_item(choices=[1, 2, 3], tags=['PCEP', 'named_parameters', ''],
-             repository=REPOSITORY)
+@examon(choices=[1, 2, 3], tags=['PCEP', 'named_parameters', ''],
+             )
 def question01():
     def test(x=1, y=2):
         x = x + y
         y += 1
         return x + y
 
     return test()
 
 
-@examon_item(choices=['True', 'False', 'None'], tags=['PCEP', 'and', 'or'],
-             repository=REPOSITORY)
+@examon(choices=['True', 'False', 'None'], tags=['PCEP', 'and', 'or'],
+             )
 def question01():
     z = 3
     y = 7
     return y < z and z > y or y > z and z < y
 
 
-@examon_item(choices=['[1, 2, 3]'], tags=['PCEP', '//', '/', '%'],
-             repository=REPOSITORY)
+@examon(choices=['[1, 2, 3]'], tags=['PCEP', '//', '/', '%'],
+             )
 def question01():
     x = 28
     y = 8
     return [x / y, x // y, x % y]
 
 
-@examon_item(choices=['1', '2', '3', '4'], tags=['PCEP', '*='],
-             repository=REPOSITORY)
+@examon(choices=['1', '2', '3', '4'], tags=['PCEP', '*='],
+             )
 def question01():
     x = 2
     y = 1
     x *= y + 1
     return x
 
 
-@examon_item(choices=[3, 4, 1], tags=['PCEP', '+', 'function'],
-             repository=REPOSITORY)
+@examon(choices=[3, 4, 1], tags=['PCEP', '+', 'function'],
+             )
 def question01():
     num2 = 1
 
     def func():
         num = num2 + 3
         return num
 
     return func()
 
 
-@examon_item(choices=[[2, 4, 6, 8]], tags=['PCEP', 'slicing'],
-             repository=REPOSITORY)
+@examon(choices=[[2, 4, 6, 8]], tags=['PCEP', 'slicing'],
+             )
 def question01():
     return [1, 2, 3, 4, 5, 6, 7, 8, 9][::2]
 
 
-@examon_item(choices=[
+@examon(choices=[
     [3, 5, 20, 5, 25, 1, 3],
     [3, 4, 5, 20, 5, 25, 3], [3, 4, 5, 20, 5, 25, 1, 3]
 ], tags=['PCEP', 'list.pop'],
-    repository=REPOSITORY)
+    )
 def question01():
     nums = [3, 4, 5, 20, 5, 25, 1, 3]
     nums.pop(1)
     return nums
 
 
-@examon_item(choices=[
+@examon(choices=[
     [4, 5, 6],
     [1, 2, 4, 5, 6],
     [1, 2, 3],
     [3, 4, 5, 6],
 ], tags=['PCEP', 'referencing', 'del'],
-    repository=REPOSITORY)
+    )
 def question01():
     def edit_list(l):
         del l[3]
 
     l = [1, 2, 3, 4, 5, 6]
     edit_list(l)
     return l
 
 
-@examon_item(choices=[['hello']], tags=['PCEP', 'list'],
-             repository=REPOSITORY)
+@examon(choices=[['hello']], tags=['PCEP', 'list'],
+             )
 def question01():
     return list('hello')
 
 
-@examon_item(choices=['1,2,3;1,2;1,2,3'], tags=['PCEP', 'named_args', 'list.join'],
-             repository=REPOSITORY)
+@examon(choices=['1,2,3;1,2;1,2,3'], tags=['PCEP', 'named_args', 'list.join'],
+             )
 def question01():
     def fun(a, b, c=0):
         return f'{a},{b},{c}'
 
     return ';'.join(
         [
             fun(1, b=2),
```

