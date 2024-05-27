# Comparing `tmp/quizengine4trivia_tirsvadcli-0.0.5.tar.gz` & `tmp/quizengine4trivia_tirsvadcli-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quizengine4trivia_tirsvadcli-0.0.5.tar", last modified: Sun May 26 03:28:30 2024, max compression
+gzip compressed data, was "quizengine4trivia_tirsvadcli-0.0.6.tar", last modified: Mon May 27 11:55:37 2024, max compression
```

## Comparing `quizengine4trivia_tirsvadcli-0.0.5.tar` & `quizengine4trivia_tirsvadcli-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 03:28:30.870794 quizengine4trivia_tirsvadcli-0.0.5/
--rw-rw-rw-   0        0        0    35823 2024-05-20 12:50:09.000000 quizengine4trivia_tirsvadcli-0.0.5/LICENSE
--rw-rw-rw-   0        0        0       62 2024-05-21 10:57:47.000000 quizengine4trivia_tirsvadcli-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0    46992 2024-05-26 03:28:30.855168 quizengine4trivia_tirsvadcli-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     4999 2024-05-26 03:24:55.000000 quizengine4trivia_tirsvadcli-0.0.5/README.md
--rw-rw-rw-   0        0        0     1771 2024-05-25 16:30:27.000000 quizengine4trivia_tirsvadcli-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       17 2024-05-22 15:43:49.000000 quizengine4trivia_tirsvadcli-0.0.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 03:28:30.870794 quizengine4trivia_tirsvadcli-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-26 03:28:30.823926 quizengine4trivia_tirsvadcli-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-05-26 03:28:30.823926 quizengine4trivia_tirsvadcli-0.0.5/src/QuizEngine4Trivia/
--rw-rw-rw-   0        0        0     2011 2024-05-25 15:22:04.000000 quizengine4trivia_tirsvadcli-0.0.5/src/QuizEngine4Trivia/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 03:28:30.823926 quizengine4trivia_tirsvadcli-0.0.5/src/QuizEngine4Trivia/models/
--rw-rw-rw-   0        0        0     3401 2024-05-25 15:37:25.000000 quizengine4trivia_tirsvadcli-0.0.5/src/QuizEngine4Trivia/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 03:28:30.855168 quizengine4trivia_tirsvadcli-0.0.5/src/QuizEngine4Trivia_TirsvadCLI.egg-info/
--rw-rw-rw-   0        0        0    46992 2024-05-26 03:28:30.000000 quizengine4trivia_tirsvadcli-0.0.5/src/QuizEngine4Trivia_TirsvadCLI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      441 2024-05-26 03:28:30.000000 quizengine4trivia_tirsvadcli-0.0.5/src/QuizEngine4Trivia_TirsvadCLI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 03:28:30.000000 quizengine4trivia_tirsvadcli-0.0.5/src/QuizEngine4Trivia_TirsvadCLI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-26 03:28:30.000000 quizengine4trivia_tirsvadcli-0.0.5/src/QuizEngine4Trivia_TirsvadCLI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-26 03:28:30.000000 quizengine4trivia_tirsvadcli-0.0.5/src/QuizEngine4Trivia_TirsvadCLI.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-26 03:28:30.855168 quizengine4trivia_tirsvadcli-0.0.5/tests/
--rw-rw-rw-   0        0        0     2698 2024-05-26 02:30:55.000000 quizengine4trivia_tirsvadcli-0.0.5/tests/test_quiz_engine.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:55:37.372909 quizengine4trivia_tirsvadcli-0.0.6/
+-rw-rw-rw-   0        0        0    35823 2024-05-20 12:50:09.000000 quizengine4trivia_tirsvadcli-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0       62 2024-05-21 10:57:47.000000 quizengine4trivia_tirsvadcli-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    47457 2024-05-27 11:55:37.372909 quizengine4trivia_tirsvadcli-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5464 2024-05-27 03:10:41.000000 quizengine4trivia_tirsvadcli-0.0.6/README.md
+-rw-rw-rw-   0        0        0     1771 2024-05-27 03:10:41.000000 quizengine4trivia_tirsvadcli-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       17 2024-05-22 15:43:49.000000 quizengine4trivia_tirsvadcli-0.0.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 11:55:37.372909 quizengine4trivia_tirsvadcli-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-27 11:55:37.326043 quizengine4trivia_tirsvadcli-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2024-05-27 11:55:37.341666 quizengine4trivia_tirsvadcli-0.0.6/src/QuizEngine4Trivia/
+-rw-rw-rw-   0        0        0     3017 2024-05-27 10:47:45.000000 quizengine4trivia_tirsvadcli-0.0.6/src/QuizEngine4Trivia/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:55:37.341666 quizengine4trivia_tirsvadcli-0.0.6/src/QuizEngine4Trivia/models/
+-rw-rw-rw-   0        0        0     3437 2024-05-27 10:37:55.000000 quizengine4trivia_tirsvadcli-0.0.6/src/QuizEngine4Trivia/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:55:37.372909 quizengine4trivia_tirsvadcli-0.0.6/src/QuizEngine4Trivia_TirsvadCLI.egg-info/
+-rw-rw-rw-   0        0        0    47457 2024-05-27 11:55:37.000000 quizengine4trivia_tirsvadcli-0.0.6/src/QuizEngine4Trivia_TirsvadCLI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      441 2024-05-27 11:55:37.000000 quizengine4trivia_tirsvadcli-0.0.6/src/QuizEngine4Trivia_TirsvadCLI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 11:55:37.000000 quizengine4trivia_tirsvadcli-0.0.6/src/QuizEngine4Trivia_TirsvadCLI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-27 11:55:37.000000 quizengine4trivia_tirsvadcli-0.0.6/src/QuizEngine4Trivia_TirsvadCLI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-27 11:55:37.000000 quizengine4trivia_tirsvadcli-0.0.6/src/QuizEngine4Trivia_TirsvadCLI.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 11:55:37.372909 quizengine4trivia_tirsvadcli-0.0.6/tests/
+-rw-rw-rw-   0        0        0     3287 2024-05-27 11:02:04.000000 quizengine4trivia_tirsvadcli-0.0.6/tests/test_quiz_engine.py
```

### Comparing `quizengine4trivia_tirsvadcli-0.0.5/LICENSE` & `quizengine4trivia_tirsvadcli-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `quizengine4trivia_tirsvadcli-0.0.5/PKG-INFO` & `quizengine4trivia_tirsvadcli-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuizEngine4Trivia-TirsvadCLI
-Version: 0.0.5
+Version: 0.0.6
 Summary: Question Engine for Trivia Queston DB
 Author: Jens Tirsvad Nielsen
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -758,32 +758,44 @@
 ```python
 from QuizEngine4Trivia import QuizEngine
 import html
 
 quiz = QuizEngine()
 
 while quiz.still_has_questions():
-    print(f"Your score : {quiz.score}\n\n")
+
     current = quiz.next_question()
-    print({html.unescape(current.question)})
 
+    user_answer: int = -1
     count = 0
-    for possible_answer in current.possible_answers:
-        print(f"{count}: {html.unescape(possible_answer)}")
-        count += 1
-
-    user_answer = int(input("Answer .:"))
-    if 0 <= user_answer <= count:
-        if quiz.check_answer(current.possible_answers[user_answer]):
-            print("You are right")
-        else:
-            print("You are wrong")
+    while not 0 <= user_answer <= count:
+        count = 0
+        print(f"Your score : {quiz.score}\n\n")
+        print(f"{html.unescape(current.category)}")
+        print(f"{html.unescape(current.question)}\n")
+
+        for possible_answer in current.possible_answers:
+            print(f"{count}: {html.unescape(possible_answer)}")
+            count += 1
+        count -= 1 # roll back last increment
+        user_answer = int(input("Answer .:"))
+
+    if quiz.check_answer(current.possible_answers[user_answer]):
+        print("You are right")
+    else:
+        print("You are wrong")
 
 print("You've completed the quiz")
 print(f"Your final score was: {quiz.score}/{quiz.question_number}")
+
+# show the right correct answer for those we didn't know the answers on
+for result in quiz.get_result():
+    if not result[0]:
+        print(html.unescape(result[1]))
+        print(html.unescape(result[2]))
 ```
 
 ## Contributing
 
 Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any
 contributions you make are greatly appreciated.
 
@@ -807,32 +819,32 @@
 git commit -m 'Add my feature enhance to project'
 git push origin feature
 ```
 
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
 
-[contributors-shield]: https://img.shields.io/github/contributors/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
+[contributors-shield]: https://img.shields.io/github/contributors/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-badge
 [contributors-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/graphs/contributors
 
-[forks-shield]: https://img.shields.io/github/forks/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
+[forks-shield]: https://img.shields.io/github/forks/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-badge
 [forks-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/network/members
 
-[stars-shield]: https://img.shields.io/github/stars/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
+[stars-shield]: https://img.shields.io/github/stars/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-badge
 [stars-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/stargazers
 
-[issues-shield]: https://img.shields.io/github/issues/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
+[issues-shield]: https://img.shields.io/github/issues/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-badge
 [issues-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/issues
 
-[license-shield]: https://img.shields.io/github/license/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
+[license-shield]: https://img.shields.io/github/license/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-badge
 [license-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/blob/master/LICENSE
 
-[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat&logo=linkedin&colorB=555
+[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
 [linkedin-url]: https://www.linkedin.com/in/jens-tirsvad-nielsen-13b795b9/
 
-[coveralls-shield]: https://img.shields.io/coverallsCoverage/github/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
+[coveralls-shield]: https://img.shields.io/coverallsCoverage/github/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-badge
 [coverall-url]: https://coveralls.io/github/TirsvadCLI/Python.QuizEngine4Trivia
 
-[pypi-shield]: https://img.shields.io/pypi/v/QuizEngine4Trivia-TirsvadCLI?style=flat
+[pypi-shield]: https://img.shields.io/pypi/v/QuizEngine4Trivia-TirsvadCLI?style=for-the-badge
 [pypi-url]: https://pypi.org/project/QuizEngine4Trivia-TirsvadCLI/
 
-[pypipyver-shield]: https://img.shields.io/pypi/pyversions/QuizEngine4Trivia-TirsvadCLI?style=flat
+[pypipyver-shield]: https://img.shields.io/pypi/pyversions/QuizEngine4Trivia-TirsvadCLI?style=for-the-badge
```

### Comparing `quizengine4trivia_tirsvadcli-0.0.5/README.md` & `quizengine4trivia_tirsvadcli-0.0.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -64,32 +64,44 @@
 ```python
 from QuizEngine4Trivia import QuizEngine
 import html
 
 quiz = QuizEngine()
 
 while quiz.still_has_questions():
-    print(f"Your score : {quiz.score}\n\n")
+
     current = quiz.next_question()
-    print({html.unescape(current.question)})
 
+    user_answer: int = -1
     count = 0
-    for possible_answer in current.possible_answers:
-        print(f"{count}: {html.unescape(possible_answer)}")
-        count += 1
-
-    user_answer = int(input("Answer .:"))
-    if 0 <= user_answer <= count:
-        if quiz.check_answer(current.possible_answers[user_answer]):
-            print("You are right")
-        else:
-            print("You are wrong")
+    while not 0 <= user_answer <= count:
+        count = 0
+        print(f"Your score : {quiz.score}\n\n")
+        print(f"{html.unescape(current.category)}")
+        print(f"{html.unescape(current.question)}\n")
+
+        for possible_answer in current.possible_answers:
+            print(f"{count}: {html.unescape(possible_answer)}")
+            count += 1
+        count -= 1 # roll back last increment
+        user_answer = int(input("Answer .:"))
+
+    if quiz.check_answer(current.possible_answers[user_answer]):
+        print("You are right")
+    else:
+        print("You are wrong")
 
 print("You've completed the quiz")
 print(f"Your final score was: {quiz.score}/{quiz.question_number}")
+
+# show the right correct answer for those we didn't know the answers on
+for result in quiz.get_result():
+    if not result[0]:
+        print(html.unescape(result[1]))
+        print(html.unescape(result[2]))
 ```
 
 ## Contributing
 
 Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any
 contributions you make are greatly appreciated.
 
@@ -113,32 +125,32 @@
 git commit -m 'Add my feature enhance to project'
 git push origin feature
 ```
 
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
 
-[contributors-shield]: https://img.shields.io/github/contributors/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
+[contributors-shield]: https://img.shields.io/github/contributors/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-badge
 [contributors-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/graphs/contributors
 
-[forks-shield]: https://img.shields.io/github/forks/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
+[forks-shield]: https://img.shields.io/github/forks/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-badge
 [forks-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/network/members
 
-[stars-shield]: https://img.shields.io/github/stars/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
+[stars-shield]: https://img.shields.io/github/stars/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-badge
 [stars-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/stargazers
 
-[issues-shield]: https://img.shields.io/github/issues/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
+[issues-shield]: https://img.shields.io/github/issues/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-badge
 [issues-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/issues
 
-[license-shield]: https://img.shields.io/github/license/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
+[license-shield]: https://img.shields.io/github/license/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-badge
 [license-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/blob/master/LICENSE
 
-[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat&logo=linkedin&colorB=555
+[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
 [linkedin-url]: https://www.linkedin.com/in/jens-tirsvad-nielsen-13b795b9/
 
-[coveralls-shield]: https://img.shields.io/coverallsCoverage/github/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
+[coveralls-shield]: https://img.shields.io/coverallsCoverage/github/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-badge
 [coverall-url]: https://coveralls.io/github/TirsvadCLI/Python.QuizEngine4Trivia
 
-[pypi-shield]: https://img.shields.io/pypi/v/QuizEngine4Trivia-TirsvadCLI?style=flat
+[pypi-shield]: https://img.shields.io/pypi/v/QuizEngine4Trivia-TirsvadCLI?style=for-the-badge
 [pypi-url]: https://pypi.org/project/QuizEngine4Trivia-TirsvadCLI/
 
-[pypipyver-shield]: https://img.shields.io/pypi/pyversions/QuizEngine4Trivia-TirsvadCLI?style=flat
+[pypipyver-shield]: https://img.shields.io/pypi/pyversions/QuizEngine4Trivia-TirsvadCLI?style=for-the-badge
```

#### html2text {}

```diff
@@ -13,49 +13,54 @@
 
                          _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 # Quiz Engine for Trivia # Getting Started Quiz Engine for Trivia module Easy
 to create a quiz game by using this module. ## Prerequisites You have python 3
 installed. ## Use In a terminal do following ```commandline pip install
 tirsvadCLI-quiz_engine_4_trivia ``` ```python from QuizEngine4Trivia import
 QuizEngine import html quiz = QuizEngine() while quiz.still_has_questions():
-print(f"Your score : {quiz.score}\n\n") current = quiz.next_question() print(
-{html.unescape(current.question)}) count = 0 for possible_answer in
-current.possible_answers: print(f"{count}: {html.unescape(possible_answer)}")
-count += 1 user_answer = int(input("Answer .:")) if 0 <= user_answer <= count:
-if quiz.check_answer(current.possible_answers[user_answer]): print("You are
-right") else: print("You are wrong") print("You've completed the quiz") print
-(f"Your final score was: {quiz.score}/{quiz.question_number}") ``` ##
-Contributing Contributions are what make the open source community such an
+current = quiz.next_question() user_answer: int = -1 count = 0 while not 0 <=
+user_answer <= count: count = 0 print(f"Your score : {quiz.score}\n\n") print
+(f"{html.unescape(current.category)}") print(f"{html.unescape
+(current.question)}\n") for possible_answer in current.possible_answers: print
+(f"{count}: {html.unescape(possible_answer)}") count += 1 count -= 1 # roll
+back last increment user_answer = int(input("Answer .:")) if quiz.check_answer
+(current.possible_answers[user_answer]): print("You are right") else: print
+("You are wrong") print("You've completed the quiz") print(f"Your final score
+was: {quiz.score}/{quiz.question_number}") # show the right correct answer for
+those we didn't know the answers on for result in quiz.get_result(): if not
+result[0]: print(html.unescape(result[1])) print(html.unescape(result[2])) ```
+## Contributing Contributions are what make the open source community such an
 amazing place to learn, inspire, and create. Any contributions you make are
 greatly appreciated. If you have a suggestion that would make this better,
 please fork the repo and create a pull request. You can also simply open an
 issue with the tag "enhancement". Don't forget to give the project a star!
 Thanks again! Fork the Project
    1. Fork the Project
    2. Create your Feature Branch
    3. Commit your Changes
    4. Push to the Branch
    5. Open a Pull Request
 Example ```commandline git checkout -b feature git commit -m 'Add my feature
 enhance to project' git push origin feature ``` [contributors-shield]: https://
 img.shields.io/github/contributors/TirsvadCLI/
-Python.QuizEngine4Trivia?style=flat [contributors-url]: https://github.com/
-TirsvadCLI/Python.QuizEngine4Trivia/graphs/contributors [forks-shield]: https:/
-/img.shields.io/github/forks/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
-[forks-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/network/
-members [stars-shield]: https://img.shields.io/github/stars/TirsvadCLI/
-Python.QuizEngine4Trivia?style=flat [stars-url]: https://github.com/TirsvadCLI/
-Python.QuizEngine4Trivia/stargazers [issues-shield]: https://img.shields.io/
-github/issues/TirsvadCLI/Python.QuizEngine4Trivia?style=flat [issues-url]:
-https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/issues [license-shield]:
-https://img.shields.io/github/license/TirsvadCLI/
-Python.QuizEngine4Trivia?style=flat [license-url]: https://github.com/
-TirsvadCLI/Python.QuizEngine4Trivia/blob/master/LICENSE [linkedin-shield]:
-https://img.shields.io/badge/-LinkedIn-
-black.svg?style=flat&logo=linkedin&colorB=555 [linkedin-url]: https://
-www.linkedin.com/in/jens-tirsvad-nielsen-13b795b9/ [coveralls-shield]: https://
-img.shields.io/coverallsCoverage/github/TirsvadCLI/
-Python.QuizEngine4Trivia?style=flat [coverall-url]: https://coveralls.io/
-github/TirsvadCLI/Python.QuizEngine4Trivia [pypi-shield]: https://
-img.shields.io/pypi/v/QuizEngine4Trivia-TirsvadCLI?style=flat [pypi-url]:
-https://pypi.org/project/QuizEngine4Trivia-TirsvadCLI/ [pypipyver-shield]:
-https://img.shields.io/pypi/pyversions/QuizEngine4Trivia-TirsvadCLI?style=flat
+Python.QuizEngine4Trivia?style=for-the-badge [contributors-url]: https://
+github.com/TirsvadCLI/Python.QuizEngine4Trivia/graphs/contributors [forks-
+shield]: https://img.shields.io/github/forks/TirsvadCLI/
+Python.QuizEngine4Trivia?style=for-the-badge [forks-url]: https://github.com/
+TirsvadCLI/Python.QuizEngine4Trivia/network/members [stars-shield]: https://
+img.shields.io/github/stars/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-
+badge [stars-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/
+stargazers [issues-shield]: https://img.shields.io/github/issues/TirsvadCLI/
+Python.QuizEngine4Trivia?style=for-the-badge [issues-url]: https://github.com/
+TirsvadCLI/Python.QuizEngine4Trivia/issues [license-shield]: https://
+img.shields.io/github/license/TirsvadCLI/Python.QuizEngine4Trivia?style=for-
+the-badge [license-url]: https://github.com/TirsvadCLI/
+Python.QuizEngine4Trivia/blob/master/LICENSE [linkedin-shield]: https://
+img.shields.io/badge/-LinkedIn-black.svg?style=for-the-
+badge&logo=linkedin&colorB=555 [linkedin-url]: https://www.linkedin.com/in/
+jens-tirsvad-nielsen-13b795b9/ [coveralls-shield]: https://img.shields.io/
+coverallsCoverage/github/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-
+badge [coverall-url]: https://coveralls.io/github/TirsvadCLI/
+Python.QuizEngine4Trivia [pypi-shield]: https://img.shields.io/pypi/v/
+QuizEngine4Trivia-TirsvadCLI?style=for-the-badge [pypi-url]: https://pypi.org/
+project/QuizEngine4Trivia-TirsvadCLI/ [pypipyver-shield]: https://
+img.shields.io/pypi/pyversions/QuizEngine4Trivia-TirsvadCLI?style=for-the-badge
```

### Comparing `quizengine4trivia_tirsvadcli-0.0.5/pyproject.toml` & `quizengine4trivia_tirsvadcli-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b70 726f 6a65 6374 5d0d 0a6e 616d 653d  [project]..name=
 00000010: 2751 7569 7a45 6e67 696e 6534 5472 6976  'QuizEngine4Triv
 00000020: 6961 2d54 6972 7376 6164 434c 4927 0d0a  ia-TirsvadCLI'..
-00000030: 7665 7273 696f 6e20 3d20 2230 2e30 2e35  version = "0.0.5
+00000030: 7665 7273 696f 6e20 3d20 2230 2e30 2e36  version = "0.0.6
 00000040: 220d 0a64 6573 6372 6970 7469 6f6e 203d  "..description =
 00000050: 2022 5175 6573 7469 6f6e 2045 6e67 696e   "Question Engin
 00000060: 6520 666f 7220 5472 6976 6961 2051 7565  e for Trivia Que
 00000070: 7374 6f6e 2044 4222 0d0a 7265 6164 6d65  ston DB"..readme
 00000080: 203d 2022 5245 4144 4d45 2e6d 6422 0d0a   = "README.md"..
 00000090: 6175 7468 6f72 7320 3d20 5b0d 0a20 2020  authors = [..   
 000000a0: 207b 6e61 6d65 203d 2022 4a65 6e73 2054   {name = "Jens T
```

### Comparing `quizengine4trivia_tirsvadcli-0.0.5/src/QuizEngine4Trivia/__init__.py` & `quizengine4trivia_tirsvadcli-0.0.6/src/QuizEngine4Trivia/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,14 +7,16 @@
     api: TriviaApiModel
     trivia_data: TriviaDataModel
 
     question_number: int = 0
     score: int = 0
     current_question: TriviaQuestionModel
 
+    track_answer: dict = {}
+
     def __init__(self) -> None:
         """
         QuestionEngine fetch question from trivia api
         """
         self.api = TriviaApiModel()
         self.trivia_data = TriviaDataModel()
         response = requests.get(url=self.api.url, params=self.api.url_params)
@@ -22,36 +24,59 @@
         self.trivia_data.from_json(response.json()['results'])
 
     def still_has_questions(self):
         """
         Is there still more question in the deck
         :return boolean:
         """
-        return self.question_number < len(self.trivia_data.data)
+        return self.question_number < len(self.trivia_data.questions)
 
     def next_question(self) -> CurrentQuestionModel:
         """
         Return the next question from deck
         :return str: question
         """
-        self.current_question = self.trivia_data.data[self.question_number]
+        self.current_question = self.trivia_data.questions[self.question_number]
         self.question_number += 1
         question = CurrentQuestionModel()
+        question.category = self.current_question.category
         question.question = f"Q.{self.question_number}: {self.current_question.question}:"
-        question.possible_answers = self.current_question.incorrect_answers
+        question.possible_answers = list(self.current_question.incorrect_answers)
         question.possible_answers.append(self.current_question.correct_answer)
         shuffle(question.possible_answers)
         return question
 
     def check_answer(self, user_answer: str) -> bool:
         """
         Checking user answer. Increase score if answer is correct
 
         :param user_answer: str
         :return boolean: Return True if answer is correct
         """
-        correct_answer = self.current_question.correct_answer
-        if user_answer.lower() == correct_answer.lower():
+
+        if user_answer.lower() == self.current_question.correct_answer.lower():
             self.score += 1
+            self.track_answer.update({self.question_number - 1: [True, user_answer]})
             return True
         else:
+            self.track_answer.update({self.question_number - 1: [False, user_answer]})
             return False
+
+    def get_result(self) -> list[tuple[bool, str, str]]:
+        """
+        Get the result of your answers
+
+        :return list[tuple[bool, str, str]]:
+        """
+        result = []
+        for k, v in self.track_answer.items():
+            if v[0]:
+                result.append((
+                    True,
+                    f"Q.{k} answer was correct : {self.trivia_data.questions[int(k)].question}",
+                    f"{v[1]}"))
+            else:
+                result.append((
+                    False,
+                    f"Q.{k} answer was wrong : {self.trivia_data.questions[k].question}",
+                    f"your answer {v[1]}\ncorrect answer {self.trivia_data.questions[int(k)].correct_answer}"))
+        return result
```

### Comparing `quizengine4trivia_tirsvadcli-0.0.5/src/QuizEngine4Trivia/models/__init__.py` & `quizengine4trivia_tirsvadcli-0.0.6/src/QuizEngine4Trivia/models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,17 +90,19 @@
         key: str
         for key, value in locals_vars.items():
             if value is not None:
                 self.url_params.update({key.split('_')[1]: value})
 
 
 class TriviaDataModel:
-    data: list[TriviaQuestionModel] = []
+    questions: list[TriviaQuestionModel] = []
 
     def from_json(self, question_list):
         for question in question_list:
-            self.data.append(TriviaQuestionModel(**question))
+            self.questions.append(TriviaQuestionModel(**question))
+
 
 
 class CurrentQuestionModel:
+    category: str = ""
     question: str = ""
     possible_answers: list = []
```

### Comparing `quizengine4trivia_tirsvadcli-0.0.5/src/QuizEngine4Trivia_TirsvadCLI.egg-info/PKG-INFO` & `quizengine4trivia_tirsvadcli-0.0.6/src/QuizEngine4Trivia_TirsvadCLI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuizEngine4Trivia-TirsvadCLI
-Version: 0.0.5
+Version: 0.0.6
 Summary: Question Engine for Trivia Queston DB
 Author: Jens Tirsvad Nielsen
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -758,32 +758,44 @@
 ```python
 from QuizEngine4Trivia import QuizEngine
 import html
 
 quiz = QuizEngine()
 
 while quiz.still_has_questions():
-    print(f"Your score : {quiz.score}\n\n")
+
     current = quiz.next_question()
-    print({html.unescape(current.question)})
 
+    user_answer: int = -1
     count = 0
-    for possible_answer in current.possible_answers:
-        print(f"{count}: {html.unescape(possible_answer)}")
-        count += 1
-
-    user_answer = int(input("Answer .:"))
-    if 0 <= user_answer <= count:
-        if quiz.check_answer(current.possible_answers[user_answer]):
-            print("You are right")
-        else:
-            print("You are wrong")
+    while not 0 <= user_answer <= count:
+        count = 0
+        print(f"Your score : {quiz.score}\n\n")
+        print(f"{html.unescape(current.category)}")
+        print(f"{html.unescape(current.question)}\n")
+
+        for possible_answer in current.possible_answers:
+            print(f"{count}: {html.unescape(possible_answer)}")
+            count += 1
+        count -= 1 # roll back last increment
+        user_answer = int(input("Answer .:"))
+
+    if quiz.check_answer(current.possible_answers[user_answer]):
+        print("You are right")
+    else:
+        print("You are wrong")
 
 print("You've completed the quiz")
 print(f"Your final score was: {quiz.score}/{quiz.question_number}")
+
+# show the right correct answer for those we didn't know the answers on
+for result in quiz.get_result():
+    if not result[0]:
+        print(html.unescape(result[1]))
+        print(html.unescape(result[2]))
 ```
 
 ## Contributing
 
 Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any
 contributions you make are greatly appreciated.
 
@@ -807,32 +819,32 @@
 git commit -m 'Add my feature enhance to project'
 git push origin feature
 ```
 
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
 
-[contributors-shield]: https://img.shields.io/github/contributors/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
+[contributors-shield]: https://img.shields.io/github/contributors/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-badge
 [contributors-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/graphs/contributors
 
-[forks-shield]: https://img.shields.io/github/forks/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
+[forks-shield]: https://img.shields.io/github/forks/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-badge
 [forks-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/network/members
 
-[stars-shield]: https://img.shields.io/github/stars/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
+[stars-shield]: https://img.shields.io/github/stars/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-badge
 [stars-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/stargazers
 
-[issues-shield]: https://img.shields.io/github/issues/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
+[issues-shield]: https://img.shields.io/github/issues/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-badge
 [issues-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/issues
 
-[license-shield]: https://img.shields.io/github/license/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
+[license-shield]: https://img.shields.io/github/license/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-badge
 [license-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/blob/master/LICENSE
 
-[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat&logo=linkedin&colorB=555
+[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
 [linkedin-url]: https://www.linkedin.com/in/jens-tirsvad-nielsen-13b795b9/
 
-[coveralls-shield]: https://img.shields.io/coverallsCoverage/github/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
+[coveralls-shield]: https://img.shields.io/coverallsCoverage/github/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-badge
 [coverall-url]: https://coveralls.io/github/TirsvadCLI/Python.QuizEngine4Trivia
 
-[pypi-shield]: https://img.shields.io/pypi/v/QuizEngine4Trivia-TirsvadCLI?style=flat
+[pypi-shield]: https://img.shields.io/pypi/v/QuizEngine4Trivia-TirsvadCLI?style=for-the-badge
 [pypi-url]: https://pypi.org/project/QuizEngine4Trivia-TirsvadCLI/
 
-[pypipyver-shield]: https://img.shields.io/pypi/pyversions/QuizEngine4Trivia-TirsvadCLI?style=flat
+[pypipyver-shield]: https://img.shields.io/pypi/pyversions/QuizEngine4Trivia-TirsvadCLI?style=for-the-badge
```

### Comparing `quizengine4trivia_tirsvadcli-0.0.5/tests/test_quiz_engine.py` & `quizengine4trivia_tirsvadcli-0.0.6/tests/test_quiz_engine.py`

 * *Files 14% similar despite different names*

```diff
@@ -52,15 +52,28 @@
 
     def test_answer_question_true(self):
         self.app.question_number = 0
         self.question = self.app.next_question()
         self.assertTrue(self.app.check_answer(self.app.current_question.correct_answer))
 
     def test_still_has_questions_true(self):
-        length = len(self.app.trivia_data.data)
+        length = len(self.app.trivia_data.questions)
         self.app.question_number = 0
         self.assertTrue(self.app.still_has_questions())
 
     def test_still_has_questions_false(self):
-        length = len(self.app.trivia_data.data)
+        length = len(self.app.trivia_data.questions)
         self.app.question_number = length
         self.assertFalse(self.app.still_has_questions())
+
+    def test_get_result_return_type(self):
+        self.app.question_number = 0
+        self.app.next_question()
+        self.app.check_answer(self.app.current_question.incorrect_answers[0])
+        self.app.next_question()
+        self.app.check_answer(self.app.current_question.correct_answer)
+        result = self.app.get_result()
+        self.assertIs(type(result), list)
+        self.assertIs(type(result[0]), tuple)
+        self.assertIs(type(result[0][0]), bool)
+        self.assertIs(type(result[0][1]), str)
+        self.assertIs(type(result[0][2]), str)
```

