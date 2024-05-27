# Comparing `tmp/pytest-lambda-2.2.0.tar.gz` & `tmp/pytest_lambda-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-lambda-2.2.0.tar", max compression
+gzip compressed data, was "pytest_lambda-2.2.1.tar", max compression
```

## Comparing `pytest-lambda-2.2.0.tar` & `pytest_lambda-2.2.1.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1069 2022-03-24 20:04:57.896391 pytest-lambda-2.2.0/LICENSE
--rw-r--r--   0        0        0     8824 2022-07-17 06:19:35.739630 pytest-lambda-2.2.0/README.md
--rw-r--r--   0        0        0     1120 2022-08-20 08:30:10.751438 pytest-lambda-2.2.0/pyproject.toml
--rw-r--r--   0        0        0      120 2022-08-20 08:30:11.291451 pytest-lambda-2.2.0/pytest_lambda/__init__.py
--rw-r--r--   0        0        0      387 2022-08-20 08:20:13.525898 pytest-lambda-2.2.0/pytest_lambda/compat.py
--rw-r--r--   0        0        0      420 2022-03-24 20:04:57.896391 pytest-lambda-2.2.0/pytest_lambda/exceptions.py
--rw-r--r--   0        0        0     5508 2022-08-20 08:15:52.768907 pytest-lambda-2.2.0/pytest_lambda/fixtures.py
--rw-r--r--   0        0        0    11739 2022-08-20 08:27:51.432084 pytest-lambda-2.2.0/pytest_lambda/impl.py
--rw-r--r--   0        0        0     2874 2022-08-20 08:10:38.718898 pytest-lambda-2.2.0/pytest_lambda/plugin.py
--rw-r--r--   0        0        0        0 2022-08-20 07:50:38.279980 pytest-lambda-2.2.0/pytest_lambda/py.typed
--rw-r--r--   0        0        0      414 2022-08-20 08:20:54.426681 pytest-lambda-2.2.0/pytest_lambda/types.py
--rw-r--r--   0        0        0     4641 2022-08-20 08:23:30.061660 pytest-lambda-2.2.0/pytest_lambda/util.py
--rw-r--r--   0        0        0    10080 2022-08-20 08:31:08.686293 pytest-lambda-2.2.0/setup.py
--rw-r--r--   0        0        0     9848 2022-08-20 08:31:08.686868 pytest-lambda-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-03-24 20:04:57.896391 pytest_lambda-2.2.1/LICENSE
+-rw-r--r--   0        0        0     8959 2024-05-27 07:54:25.549198 pytest_lambda-2.2.1/README.md
+-rw-r--r--   0        0        0      934 2024-05-27 07:55:27.782508 pytest_lambda-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0      120 2024-05-27 07:55:28.310520 pytest_lambda-2.2.1/pytest_lambda/__init__.py
+-rw-r--r--   0        0        0      387 2022-08-20 08:20:13.525898 pytest_lambda-2.2.1/pytest_lambda/compat.py
+-rw-r--r--   0        0        0      420 2022-03-24 20:04:57.896391 pytest_lambda-2.2.1/pytest_lambda/exceptions.py
+-rw-r--r--   0        0        0     5682 2022-08-20 18:46:12.265587 pytest_lambda-2.2.1/pytest_lambda/fixtures.py
+-rw-r--r--   0        0        0    11739 2022-08-20 08:27:51.432084 pytest_lambda-2.2.1/pytest_lambda/impl.py
+-rw-r--r--   0        0        0     2874 2022-08-20 08:10:38.718898 pytest_lambda-2.2.1/pytest_lambda/plugin.py
+-rw-r--r--   0        0        0        0 2022-08-20 07:50:38.279980 pytest_lambda-2.2.1/pytest_lambda/py.typed
+-rw-r--r--   0        0        0      414 2022-08-20 08:20:54.426681 pytest_lambda-2.2.1/pytest_lambda/types.py
+-rw-r--r--   0        0        0     4641 2022-08-20 08:23:30.061660 pytest_lambda-2.2.1/pytest_lambda/util.py
+-rw-r--r--   0        0        0     9972 1970-01-01 00:00:00.000000 pytest_lambda-2.2.1/PKG-INFO
```

### Comparing `pytest-lambda-2.2.0/LICENSE` & `pytest_lambda-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-lambda-2.2.0/README.md` & `pytest_lambda-2.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # pytest-lambda
 
+[![PyPI version](https://badge.fury.io/py/pytest-lambda.svg)](https://badge.fury.io/py/pytest-lambda)
+
 Define pytest fixtures with lambda functions.
 
 
 # Quickstart
 
 ```bash
 pip install pytest-lambda
@@ -313,8 +315,8 @@
 # Development
 
 How can I build and test the thing locally?
 
 1. Create a virtualenv, however you prefer. Or don't, if you prefer.
 2. `pip install poetry`
 3. `poetry install` to install setuptools entrypoint, so pytest automatically loads the plugin (otherwise, you'll have to run `py.test -p pytest_lambda.plugin`)
-4. Run `py.test`. The tests will be collected from the README.md (thanks to [pytest-markdown](https://github.com/Jc2k/pytest-markdown)).
+4. Run `py.test --markdown-docs`. The tests will be collected from the README.md (thanks to [pytest-markdown-docs](https://github.com/modal-labs/pytest-markdown-docs)).
```

### Comparing `pytest-lambda-2.2.0/pyproject.toml` & `pytest_lambda-2.2.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 [tool.poetry]
 name = 'pytest-lambda'
-version = "2.2.0"
+version = "2.2.1"
 description = 'Define pytest fixtures with lambda functions.'
 license = 'MIT'
 
 authors = [
     'Zach "theY4Kman" Kanzler <they4kman@gmail.com>'
 ]
 
 readme = 'README.md'
 
 repository = 'https://github.com/theY4Kman/pytest-lambda'
 homepage = 'https://github.com/theY4Kman/pytest-lambda'
 
 keywords = ['pytest']
 classifiers=[
-    'Development Status :: 3 - Alpha',
+    'Development Status :: 5 - Production/Stable',
     'Programming Language :: Python',
     'Framework :: Pytest',
     'License :: OSI Approved :: MIT License',
     'Topic :: Software Development :: Testing',
 ]
 
 
 [tool.poetry.dependencies]
-# Typing annotations are used
-# XXX: for whatever reason, poetry doesn't like `>=3.7` — the additional pin allows locking to work
-python = '^3.7.0, >= 3.7.0'
+python = '^3.8.0'
 
-pytest = '>=3.6, <8'
-typing-extensions = { version = '^4.2.0', python = '<=3.7' }
+pytest = '>=3.6, <9'
 wrapt = '^1.11.0'
 
 
 [tool.poetry.dev-dependencies]
 mypy = "^0.971"
 pytest-asyncio = "*"
-pytest-markdown = "*"
+pytest-markdown-docs = "*"
 tox = "^3.12"
 
 
 [tool.poetry.plugins."pytest11"]
 lambda = "pytest_lambda.plugin"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pytest-lambda-2.2.0/pytest_lambda/fixtures.py` & `pytest_lambda-2.2.1/pytest_lambda/fixtures.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,24 +32,27 @@
     Usage:
 
         class DescribeMyTests:
             url = lambda_fixture('list_url')
             updated_name = lambda_fixture(lambda vendor: vendor.name + ' updated')
 
 
-    :param fixture_name_or_lambda: Either the name of another fixture, or a
-        lambda function, which can request other fixtures with its params. If
-        None, this defaults to the name of the attribute containing the lambda_fixture.
-
-    :param bind: Set this to true to pass self to your fixture. It must be the
-        first parameter in your fixture. This cannot be true if using a fixture
-        name.
-
-    :param async_: If True, the lambda will be wrapped in an async function; if the
-        lambda evaluates to an awaitable value, it will be awaited.
+    :param fixture_name_or_lambda:
+        Either the name of another fixture, or a lambda function, which can request other fixtures
+        with its params. If None, this defaults to the name of the attribute containing the
+        lambda_fixture.
+
+    :param bind:
+        Set this to True to pass self to your fixture. It must be the first parameter in your
+        fixture. This cannot be True if using a fixture name.
+
+    :param async_:
+        If True, the lambda will be wrapped in an async function; if the lambda evaluates to an
+        awaitable value, it will be awaited. If False, the lambda's return value will be returned
+        verbatim, regardless of whether it's awaitable.
 
     :param scope:
     :param params:
     :param autouse:
     :param ids:
     :param name:
         Options to pass to pytest.fixture()
@@ -91,16 +94,17 @@
 
     Usage:
 
         class DescribeMyTests:
             url = error_fixture(lambda request: Exception(
                 f'Please override the {request.fixturename} fixture!'))
 
-    :param error_fn: fixture method which returns an exception to raise. It may
-        request pytest fixtures in its arguments
+    :param error_fn:
+        Fixture method which returns an exception to raise. It may request pytest fixtures
+        in its arguments.
 
     """
     proto = tuple(inspect.signature(error_fn).parameters)
     args = ', '.join(proto)
     kwargs = ', '.join(f'{arg}={arg}' for arg in proto)
 
     source = RAISE_EXCEPTION_FIXTURE_FUNCTION_FORMAT.format(
@@ -108,15 +112,15 @@
         kwargs=kwargs,
     )
 
     ctx = {'error_fn': error_fn}
     exec(source, ctx)
 
     raise_exception = ctx['raise_exception']
-    raise_exception.__module__ = error_fn.__module__
+    raise_exception.__module__ = getattr(error_fn, '__module__', raise_exception.__module__)
     return lambda_fixture(raise_exception, **fixture_kwargs)
 
 
 def disabled_fixture(**fixture_kwargs) -> LambdaFixture[NoReturn]:
     """Mark a fixture as disabled – using the fixture will raise an error
 
     This is useful when you know any usage of a fixture would be in error. When
```

### Comparing `pytest-lambda-2.2.0/pytest_lambda/impl.py` & `pytest_lambda-2.2.1/pytest_lambda/impl.py`

 * *Files identical despite different names*

### Comparing `pytest-lambda-2.2.0/pytest_lambda/plugin.py` & `pytest_lambda-2.2.1/pytest_lambda/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-lambda-2.2.0/pytest_lambda/util.py` & `pytest_lambda-2.2.1/pytest_lambda/util.py`

 * *Files identical despite different names*

### Comparing `pytest-lambda-2.2.0/setup.py` & `pytest_lambda-2.2.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,349 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pytest-lambda
+Version: 2.2.1
+Summary: Define pytest fixtures with lambda functions.
+Home-page: https://github.com/theY4Kman/pytest-lambda
+License: MIT
+Keywords: pytest
+Author: Zach "theY4Kman" Kanzler
+Author-email: they4kman@gmail.com
+Requires-Python: >=3.8.0,<4.0.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: Pytest
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Testing
+Requires-Dist: pytest (>=3.6,<9)
+Requires-Dist: wrapt (>=1.11.0,<2.0.0)
+Project-URL: Repository, https://github.com/theY4Kman/pytest-lambda
+Description-Content-Type: text/markdown
 
-packages = \
-['pytest_lambda']
+# pytest-lambda
 
-package_data = \
-{'': ['*']}
+[![PyPI version](https://badge.fury.io/py/pytest-lambda.svg)](https://badge.fury.io/py/pytest-lambda)
 
-install_requires = \
-['pytest>=3.6,<8', 'wrapt>=1.11.0,<2.0.0']
-
-extras_require = \
-{':python_version <= "3.7"': ['typing-extensions>=4.2.0,<5.0.0']}
-
-entry_points = \
-{'pytest11': ['lambda = pytest_lambda.plugin']}
-
-setup_kwargs = {
-    'name': 'pytest-lambda',
-    'version': '2.2.0',
-    'description': 'Define pytest fixtures with lambda functions.',
-    'long_description': "# pytest-lambda\n\nDefine pytest fixtures with lambda functions.\n\n\n# Quickstart\n\n```bash\npip install pytest-lambda\n```\n\n```python\n# test_the_namerator.py\n\nfrom pytest_lambda import lambda_fixture, static_fixture\n\nfirst = static_fixture('John')\nmiddle = static_fixture('Jacob')\nlast = static_fixture('Jingleheimer-Schmidt')\n\n\nfull_name = lambda_fixture(lambda first, middle, last: f'{first} {middle} {last}')\n\n\ndef test_the_namerator(full_name):\n    assert full_name == 'John Jacob Jingleheimer-Schmidt'\n```\n\n\n# Cheatsheet\n\n ```python\nimport asyncio\nimport pytest\nfrom pytest_lambda import (\n    disabled_fixture,\n    error_fixture,\n    lambda_fixture,\n    not_implemented_fixture,\n    static_fixture,\n)\n\n# Basic usage\nfixture_name = lambda_fixture(lambda other_fixture: 'expression', scope='session', autouse=True)\n\n# Async fixtures (awaitables automatically awaited) — requires an async plugin, like pytest-asyncio\nfixture_name = lambda_fixture(lambda: asyncio.sleep(0, 'expression'), async_=True)\n\n# Request fixtures by name\nfixture_name = lambda_fixture('other_fixture')\nfixture_name = lambda_fixture('other_fixture', 'another_fixture', 'cant_believe_its_not_fixture')\nren, ame, it = lambda_fixture('other_fixture', 'another_fixture', 'cant_believe_its_not_fixture')\n\n# Reference `self` inside a class\nclass TestContext:\n    fixture_name = lambda_fixture(lambda self: self.__class__.__name__, bind=True)\n\n# Parametrize\nfixture_name = lambda_fixture(params=['a', 'b'])\nfixture_name = lambda_fixture(params=['a', 'b'], ids=['A!', 'B!'])\nfixture_name = lambda_fixture(params=[pytest.param('a', id='A!'),\n                                      pytest.param('b', id='B!')])\nalpha, omega = lambda_fixture(params=[pytest.param('start', 'end', id='uno'),\n                                      pytest.param('born', 'dead', id='dos')])\n\n# Use literal value (not lazily evaluated)\nfixture_name = static_fixture(42)\nfixture_name = static_fixture('just six sevens', autouse=True, scope='module')\n\n# Raise an exception if fixture is requested\nfixture_name = error_fixture(lambda: ValueError('my life has no intrinsic value'))\n\n# Or maybe don't raise the exception\nfixture_name = error_fixture(lambda other_fixture: TypeError('nope') if other_fixture else None)\n\n# Create an abstract fixture (to be overridden by the user)\nfixture_name = not_implemented_fixture()\nfixture_name = not_implemented_fixture(autouse=True, scope='session')\n\n# Disable usage of a fixture (fail early to save future head scratching)\nfixture_name = disabled_fixture()\n```\n\n\n# What else is possible?\n\nOf course, you can use lambda fixtures inside test classes:\n```python\n# test_staying_classy.py\n\nfrom pytest_lambda import lambda_fixture\n\nclass TestClassiness:\n    classiness = lambda_fixture(lambda: 9000 + 1)\n\n    def test_how_classy_we_is(self, classiness):\n        assert classiness == 9001\n```\n\n\n### Aliasing other fixtures\n\nYou can also pass the name of another fixture, instead of a lambda:\n```python\n# test_the_bourne_identity.py\n\nfrom pytest_lambda import lambda_fixture, static_fixture\n\nagent = static_fixture('Bourne')\nwho_i_am = lambda_fixture('agent')\n\ndef test_my_identity(who_i_am):\n    assert who_i_am == 'Bourne'\n```\n\n\nEven multiple fixture names can be used:\n```python\n# test_the_bourne_identity.py\n\nfrom pytest_lambda import lambda_fixture, static_fixture\n\nagent_first = static_fixture('Jason')\nagent_last = static_fixture('Bourne')\nwho_i_am = lambda_fixture('agent_first', 'agent_last')\n\ndef test_my_identity(who_i_am):\n    assert who_i_am == ('Jason', 'Bourne')\n```\n\nDestructuring assignment is also supported, allowing multiple fixtures to be renamed in one statement:\n```python\n# test_the_bourne_identity.py\n\nfrom pytest_lambda import lambda_fixture, static_fixture\n\nagent_first = static_fixture('Jason')\nagent_last = static_fixture('Bourne')\nfirst, last = lambda_fixture('agent_first', 'agent_last')\n\ndef test_my_identity(first, last):\n    assert first == 'Jason'\n    assert last == 'Bourne'\n```\n\n\n#### Annotating aliased fixtures\n\nYou can force the loading of fixtures without trying to remember the name of `pytest.mark.usefixtures`\n```python\n# test_garage.py\n\nfrom pytest_lambda import lambda_fixture, static_fixture\n\ncar = static_fixture({\n    'type': 'Sweet-ass Cadillac',\n    'is_started': False,\n})\nturn_the_key = lambda_fixture(lambda car: car.update(is_started=True))\n\npreconditions = lambda_fixture('turn_the_key', autouse=True)\n\ndef test_my_caddy(car):\n    assert car['is_started']\n```\n\n\n### Parametrizing\n\nTests can be parametrized with `lambda_fixture`'s `params` kwarg\n```python\n# test_number_5.py\n\nfrom pytest_lambda import lambda_fixture\n\nlady = lambda_fixture(params=[\n    'Monica', 'Erica', 'Rita', 'Tina', 'Sandra', 'Mary', 'Jessica'\n])\n\ndef test_your_man(lady):\n    assert lady[:0] in 'my life'\n```\n\nDestructuring assignment of a parametrized lambda fixture is also supported\n```python\n# test_number_5.py\n\nimport pytest\nfrom pytest_lambda import lambda_fixture\n\nlady, where = lambda_fixture(params=[\n    pytest.param('Monica', 'in my life'),\n    pytest.param('Erica', 'by my side'),\n    pytest.param('Rita', 'is all I need'),\n    pytest.param('Tina', 'is what I see'),\n    pytest.param('Sandra', 'in the sun'),\n    pytest.param('Mary', 'all night long'),\n    pytest.param('Jessica', 'here I am'),\n])\n\ndef test_your_man(lady, where):\n    assert lady[:0] in where\n```\n\n\n### Declaring abstract things\n\n`not_implemented_fixture` is perfect for labeling abstract parameter fixtures of test mixins\n```python\n# test_mixinalot.py\n\nimport pytest\nfrom pytest_lambda import static_fixture, not_implemented_fixture\n\nclass Dials1900MixinALot:\n    butt_shape = not_implemented_fixture()\n    desires = not_implemented_fixture()\n\n    def it_kicks_them_nasty_thoughts(self, butt_shape, desires):\n        assert butt_shape == 'round' and 'triple X throw down' in desires\n\n\n@pytest.mark.xfail\nclass DescribeMissThing(Dials1900MixinALot):\n    butt_shape = static_fixture('flat')\n    desires = static_fixture(['playin workout tapes by Fonda'])\n\n\nclass DescribeSistaICantResista(Dials1900MixinALot):\n    butt_shape = static_fixture('round')\n    desires = static_fixture(['gettin in yo Benz', 'triple X throw down'])\n```\n\n\nUse `disabled_fixture` to mark a fixture as disabled. Go figure.\n```python\n# test_ada.py\n\nimport pytest\nfrom pytest_lambda import disabled_fixture\n\nwheelchair = disabled_fixture()\n\n@pytest.mark.xfail(strict=True)\ndef test_stairs(wheelchair):\n    assert wheelchair + 'floats'\n```\n\n\n### Raising exceptions\n\nYou can also raise an arbitrary exception when a fixture is requested, using `error_fixture`\n```python\n# test_bikeshed.py\n\nimport pytest\nfrom pytest_lambda import error_fixture, not_implemented_fixture, static_fixture\n\nbicycle = static_fixture('a sledgehammer')\n\ndef it_does_sweet_jumps(bicycle):\n    assert bicycle + 'jump' >= '3 feet'\n\n\nclass ContextOcean:\n    depth = not_implemented_fixture()\n    bicycle = error_fixture(lambda bicycle, depth: (\n        RuntimeError(f'Now is not the time to use that! ({bicycle})') if depth > '1 league' else None))\n\n\n    class ContextDeep:\n        depth = static_fixture('20,000 leagues')\n\n        @pytest.mark.xfail(strict=True, raises=RuntimeError)\n        def it_doesnt_flip_and_shit(self, bicycle):\n            assert bicycle + 'floats'\n\n\n    class ContextBeach:\n        depth = static_fixture('1 inch')\n\n        def it_gets_you_all_wet_but_otherwise_rides_like_a_champ(self, bicycle):\n            assert 'im wet'\n```\n\n\n### Async fixtures\n\nBy passing `async_=True` to `lambda_fixture`, the fixture will be defined as an async function, and if the returned value is awaitable, it will be automatically awaited before exposing it to pytest. This allows the usage of async things while only being slightly salty that Python, TO THIS DAY, still does not support `await` expressions within lambdas! Yes, only slightly salty!\n\nNOTE: an asyncio pytest plugin is required to use async fixtures, such as [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio)\n\n```python\n# test_a_sink.py\n\nimport asyncio\nimport pytest\nfrom pytest_lambda import lambda_fixture\n\nasync def hows_the_sink():\n    await asyncio.sleep(1)\n    return 'leaky'\n\na_sink = lambda_fixture(lambda: hows_the_sink(), async_=True)\n\nclass DescribeASink:\n    @pytest.mark.asyncio\n    async def it_is_leaky(self, a_sink):\n        assert a_sink is 'leaky'\n```\n\n\n# Development\n\nHow can I build and test the thing locally?\n\n1. Create a virtualenv, however you prefer. Or don't, if you prefer.\n2. `pip install poetry`\n3. `poetry install` to install setuptools entrypoint, so pytest automatically loads the plugin (otherwise, you'll have to run `py.test -p pytest_lambda.plugin`)\n4. Run `py.test`. The tests will be collected from the README.md (thanks to [pytest-markdown](https://github.com/Jc2k/pytest-markdown)).\n",
-    'author': 'Zach "theY4Kman" Kanzler',
-    'author_email': 'they4kman@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/theY4Kman/pytest-lambda',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.0,<4.0.0',
-}
+Define pytest fixtures with lambda functions.
 
 
-setup(**setup_kwargs)
+# Quickstart
+
+```bash
+pip install pytest-lambda
+```
+
+```python
+# test_the_namerator.py
+
+from pytest_lambda import lambda_fixture, static_fixture
+
+first = static_fixture('John')
+middle = static_fixture('Jacob')
+last = static_fixture('Jingleheimer-Schmidt')
+
+
+full_name = lambda_fixture(lambda first, middle, last: f'{first} {middle} {last}')
+
+
+def test_the_namerator(full_name):
+    assert full_name == 'John Jacob Jingleheimer-Schmidt'
+```
+
+
+# Cheatsheet
+
+ ```python
+import asyncio
+import pytest
+from pytest_lambda import (
+    disabled_fixture,
+    error_fixture,
+    lambda_fixture,
+    not_implemented_fixture,
+    static_fixture,
+)
+
+# Basic usage
+fixture_name = lambda_fixture(lambda other_fixture: 'expression', scope='session', autouse=True)
+
+# Async fixtures (awaitables automatically awaited) — requires an async plugin, like pytest-asyncio
+fixture_name = lambda_fixture(lambda: asyncio.sleep(0, 'expression'), async_=True)
+
+# Request fixtures by name
+fixture_name = lambda_fixture('other_fixture')
+fixture_name = lambda_fixture('other_fixture', 'another_fixture', 'cant_believe_its_not_fixture')
+ren, ame, it = lambda_fixture('other_fixture', 'another_fixture', 'cant_believe_its_not_fixture')
+
+# Reference `self` inside a class
+class TestContext:
+    fixture_name = lambda_fixture(lambda self: self.__class__.__name__, bind=True)
+
+# Parametrize
+fixture_name = lambda_fixture(params=['a', 'b'])
+fixture_name = lambda_fixture(params=['a', 'b'], ids=['A!', 'B!'])
+fixture_name = lambda_fixture(params=[pytest.param('a', id='A!'),
+                                      pytest.param('b', id='B!')])
+alpha, omega = lambda_fixture(params=[pytest.param('start', 'end', id='uno'),
+                                      pytest.param('born', 'dead', id='dos')])
+
+# Use literal value (not lazily evaluated)
+fixture_name = static_fixture(42)
+fixture_name = static_fixture('just six sevens', autouse=True, scope='module')
+
+# Raise an exception if fixture is requested
+fixture_name = error_fixture(lambda: ValueError('my life has no intrinsic value'))
+
+# Or maybe don't raise the exception
+fixture_name = error_fixture(lambda other_fixture: TypeError('nope') if other_fixture else None)
+
+# Create an abstract fixture (to be overridden by the user)
+fixture_name = not_implemented_fixture()
+fixture_name = not_implemented_fixture(autouse=True, scope='session')
+
+# Disable usage of a fixture (fail early to save future head scratching)
+fixture_name = disabled_fixture()
+```
+
+
+# What else is possible?
+
+Of course, you can use lambda fixtures inside test classes:
+```python
+# test_staying_classy.py
+
+from pytest_lambda import lambda_fixture
+
+class TestClassiness:
+    classiness = lambda_fixture(lambda: 9000 + 1)
+
+    def test_how_classy_we_is(self, classiness):
+        assert classiness == 9001
+```
+
+
+### Aliasing other fixtures
+
+You can also pass the name of another fixture, instead of a lambda:
+```python
+# test_the_bourne_identity.py
+
+from pytest_lambda import lambda_fixture, static_fixture
+
+agent = static_fixture('Bourne')
+who_i_am = lambda_fixture('agent')
+
+def test_my_identity(who_i_am):
+    assert who_i_am == 'Bourne'
+```
+
+
+Even multiple fixture names can be used:
+```python
+# test_the_bourne_identity.py
+
+from pytest_lambda import lambda_fixture, static_fixture
+
+agent_first = static_fixture('Jason')
+agent_last = static_fixture('Bourne')
+who_i_am = lambda_fixture('agent_first', 'agent_last')
+
+def test_my_identity(who_i_am):
+    assert who_i_am == ('Jason', 'Bourne')
+```
+
+Destructuring assignment is also supported, allowing multiple fixtures to be renamed in one statement:
+```python
+# test_the_bourne_identity.py
+
+from pytest_lambda import lambda_fixture, static_fixture
+
+agent_first = static_fixture('Jason')
+agent_last = static_fixture('Bourne')
+first, last = lambda_fixture('agent_first', 'agent_last')
+
+def test_my_identity(first, last):
+    assert first == 'Jason'
+    assert last == 'Bourne'
+```
+
+
+#### Annotating aliased fixtures
+
+You can force the loading of fixtures without trying to remember the name of `pytest.mark.usefixtures`
+```python
+# test_garage.py
+
+from pytest_lambda import lambda_fixture, static_fixture
+
+car = static_fixture({
+    'type': 'Sweet-ass Cadillac',
+    'is_started': False,
+})
+turn_the_key = lambda_fixture(lambda car: car.update(is_started=True))
+
+preconditions = lambda_fixture('turn_the_key', autouse=True)
+
+def test_my_caddy(car):
+    assert car['is_started']
+```
+
+
+### Parametrizing
+
+Tests can be parametrized with `lambda_fixture`'s `params` kwarg
+```python
+# test_number_5.py
+
+from pytest_lambda import lambda_fixture
+
+lady = lambda_fixture(params=[
+    'Monica', 'Erica', 'Rita', 'Tina', 'Sandra', 'Mary', 'Jessica'
+])
+
+def test_your_man(lady):
+    assert lady[:0] in 'my life'
+```
+
+Destructuring assignment of a parametrized lambda fixture is also supported
+```python
+# test_number_5.py
+
+import pytest
+from pytest_lambda import lambda_fixture
+
+lady, where = lambda_fixture(params=[
+    pytest.param('Monica', 'in my life'),
+    pytest.param('Erica', 'by my side'),
+    pytest.param('Rita', 'is all I need'),
+    pytest.param('Tina', 'is what I see'),
+    pytest.param('Sandra', 'in the sun'),
+    pytest.param('Mary', 'all night long'),
+    pytest.param('Jessica', 'here I am'),
+])
+
+def test_your_man(lady, where):
+    assert lady[:0] in where
+```
+
+
+### Declaring abstract things
+
+`not_implemented_fixture` is perfect for labeling abstract parameter fixtures of test mixins
+```python
+# test_mixinalot.py
+
+import pytest
+from pytest_lambda import static_fixture, not_implemented_fixture
+
+class Dials1900MixinALot:
+    butt_shape = not_implemented_fixture()
+    desires = not_implemented_fixture()
+
+    def it_kicks_them_nasty_thoughts(self, butt_shape, desires):
+        assert butt_shape == 'round' and 'triple X throw down' in desires
+
+
+@pytest.mark.xfail
+class DescribeMissThing(Dials1900MixinALot):
+    butt_shape = static_fixture('flat')
+    desires = static_fixture(['playin workout tapes by Fonda'])
+
+
+class DescribeSistaICantResista(Dials1900MixinALot):
+    butt_shape = static_fixture('round')
+    desires = static_fixture(['gettin in yo Benz', 'triple X throw down'])
+```
+
+
+Use `disabled_fixture` to mark a fixture as disabled. Go figure.
+```python
+# test_ada.py
+
+import pytest
+from pytest_lambda import disabled_fixture
+
+wheelchair = disabled_fixture()
+
+@pytest.mark.xfail(strict=True)
+def test_stairs(wheelchair):
+    assert wheelchair + 'floats'
+```
+
+
+### Raising exceptions
+
+You can also raise an arbitrary exception when a fixture is requested, using `error_fixture`
+```python
+# test_bikeshed.py
+
+import pytest
+from pytest_lambda import error_fixture, not_implemented_fixture, static_fixture
+
+bicycle = static_fixture('a sledgehammer')
+
+def it_does_sweet_jumps(bicycle):
+    assert bicycle + 'jump' >= '3 feet'
+
+
+class ContextOcean:
+    depth = not_implemented_fixture()
+    bicycle = error_fixture(lambda bicycle, depth: (
+        RuntimeError(f'Now is not the time to use that! ({bicycle})') if depth > '1 league' else None))
+
+
+    class ContextDeep:
+        depth = static_fixture('20,000 leagues')
+
+        @pytest.mark.xfail(strict=True, raises=RuntimeError)
+        def it_doesnt_flip_and_shit(self, bicycle):
+            assert bicycle + 'floats'
+
+
+    class ContextBeach:
+        depth = static_fixture('1 inch')
+
+        def it_gets_you_all_wet_but_otherwise_rides_like_a_champ(self, bicycle):
+            assert 'im wet'
+```
+
+
+### Async fixtures
+
+By passing `async_=True` to `lambda_fixture`, the fixture will be defined as an async function, and if the returned value is awaitable, it will be automatically awaited before exposing it to pytest. This allows the usage of async things while only being slightly salty that Python, TO THIS DAY, still does not support `await` expressions within lambdas! Yes, only slightly salty!
+
+NOTE: an asyncio pytest plugin is required to use async fixtures, such as [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio)
+
+```python
+# test_a_sink.py
+
+import asyncio
+import pytest
+from pytest_lambda import lambda_fixture
+
+async def hows_the_sink():
+    await asyncio.sleep(1)
+    return 'leaky'
+
+a_sink = lambda_fixture(lambda: hows_the_sink(), async_=True)
+
+class DescribeASink:
+    @pytest.mark.asyncio
+    async def it_is_leaky(self, a_sink):
+        assert a_sink is 'leaky'
+```
+
+
+# Development
+
+How can I build and test the thing locally?
+
+1. Create a virtualenv, however you prefer. Or don't, if you prefer.
+2. `pip install poetry`
+3. `poetry install` to install setuptools entrypoint, so pytest automatically loads the plugin (otherwise, you'll have to run `py.test -p pytest_lambda.plugin`)
+4. Run `py.test --markdown-docs`. The tests will be collected from the README.md (thanks to [pytest-markdown-docs](https://github.com/modal-labs/pytest-markdown-docs)).
+
```

