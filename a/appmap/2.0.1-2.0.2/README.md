# Comparing `tmp/appmap-2.0.1.tar.gz` & `tmp/appmap-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appmap-2.0.1.tar", max compression
+gzip compressed data, was "appmap-2.0.2.tar", max compression
```

## Comparing `appmap-2.0.1.tar` & `appmap-2.0.2.tar`

### file list

```diff
@@ -1,163 +1,163 @@
--rw-r--r--   0        0        0     1925 2024-05-23 22:54:15.344025 appmap-2.0.1/LICENSE
--rw-r--r--   0        0        0     4534 2024-05-23 22:54:15.344025 appmap-2.0.1/README.md
--rw-r--r--   0        0        0      502 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/__init__.py
--rw-r--r--   0        0        0    15857 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/configuration.py
--rw-r--r--   0        0        0     1082 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/django.py
--rw-r--r--   0        0        0     6702 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/env.py
--rw-r--r--   0        0        0    15677 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/event.py
--rw-r--r--   0        0        0      694 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/fastapi.py
--rw-r--r--   0        0        0      822 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/flask.py
--rw-r--r--   0        0        0     3642 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/generation.py
--rw-r--r--   0        0        0    11495 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/importer.py
--rw-r--r--   0        0        0     4323 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/instrument.py
--rw-r--r--   0        0        0     1786 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/labels.py
--rw-r--r--   0        0        0     3071 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/metadata.py
--rw-r--r--   0        0        0      267 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/noappmap.py
--rw-r--r--   0        0        0      538 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/py_version_check.py
--rw-r--r--   0        0        0     5513 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/recorder.py
--rw-r--r--   0        0        0     2868 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/recording.py
--rw-r--r--   0        0        0      926 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/remote_recording.py
--rw-r--r--   0        0        0      340 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/singleton.py
--rw-r--r--   0        0        0      174 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/__init__.py
--rw-r--r--   0        0        0     3607 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/appmap_test_base.py
--rwxr-xr-x   0        0        0      121 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/bin/server_runner
--rw-r--r--   0        0        0     6048 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/conftest.py
--rw-r--r--   0        0        0      112 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/data/appmap-all-paths-malformed.yml
--rw-r--r--   0        0        0       50 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/data/appmap-broken.yml
--rw-r--r--   0        0        0       82 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/data/appmap-class.yml
--rw-r--r--   0        0        0       59 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/data/appmap-empty-path.yml
--rw-r--r--   0        0        0      126 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/data/appmap-exclude-fn.yml
--rw-r--r--   0        0        0       87 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/data/appmap-func.yml
--rw-r--r--   0        0        0       82 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/data/appmap-malformed-path.yml
--rw-r--r--   0        0        0      308 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/data/appmap-no-pyyaml.yml
--rw-r--r--   0        0        0      323 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/data/appmap.yml
--rw-r--r--   0        0        0        0 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/data/appmap_testing/__init__.py
--rw-r--r--   0        0        0      237 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/data/appmap_testing/django_simplelazyobject.py
--rw-r--r--   0        0        0        0 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/data/config/src/package/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/data/config/test/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/data/config/test/foo.py
--rw-r--r--   0        0        0       16 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/data/config-exclude/.hide/hidden_mod/__init__.py
--rw-r--r--   0        0        0       25 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/data/config-exclude/node_modules/node_mod/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/data/config-exclude/src/package/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/data/config-exclude/test/__init__.py
--rw-r--r--   0        0        0       14 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/data/config-exclude/venv/venv_mod/__init__.py
--rw-r--r--   0        0        0       20 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/data/config-up/appmap.yml
--rw-r--r--   0        0        0        0 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/data/config-up/project/p1/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/data/config-up/project/p2/sub1/__init__.py
--rw-r--r--   0        0        0       44 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/data/django/appmap.yml
--rw-r--r--   0        0        0      495 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/data/django/djangoapp/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/data/django/djangoapp/djangoapp.py
--rw-r--r--   0        0        0       39 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/data/django/djangoapp/hello_world.html
--rw-r--r--   0        0        0      154 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/data/django/djangoapp/middleware.py
--rw-r--r--   0        0        0      426 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/data/django/djangoapp/settings.py
--rw-r--r--   0        0        0      563 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/data/django/djangoapp/settings_dev.py
--rw-r--r--   0        0        0     2148 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/data/django/djangoapp/urls.py
--rw-r--r--   0        0        0       14 2024-05-23 22:54:15.344025 appmap-2.0.1/_appmap/test/data/django/init/sitecustomize.py
--rwxr-xr-x   0        0        0      665 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/django/manage.py
--rw-r--r--   0        0        0       53 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/django/pytest.ini
--rw-r--r--   0        0        0        0 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/django/test/__init__.py
--rw-r--r--   0        0        0      935 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/django/test/test_app.py
--rw-r--r--   0        0        0     2591 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/example_class.py
--rw-r--r--   0        0        0     7942 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/expected.appmap.json
--rw-r--r--   0        0        0       47 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/fastapi/appmap.yml
--rw-r--r--   0        0        0        0 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/fastapi/fastapiapp/__init__.py
--rw-r--r--   0        0        0     1647 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/fastapi/fastapiapp/main.py
--rw-r--r--   0        0        0       14 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/fastapi/init/sitecustomize.py
--rw-r--r--   0        0        0      240 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/fastapi/test_app.py
--rw-r--r--   0        0        0       38 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/flask/appmap.yml
--rw-r--r--   0        0        0     1200 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/flask/flaskapp.py
--rw-r--r--   0        0        0       14 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/flask/init/sitecustomize.py
--rw-r--r--   0        0        0        0 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/flask/templates/test.html
--rw-r--r--   0        0        0      268 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/flask/test_app.py
--rw-r--r--   0        0        0        0 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/package1/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/package1/package2/__init__.py
--rw-r--r--   0        0        0      113 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/package1/package2/__main__.py
--rw-r--r--   0        0        0       69 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/package1/package2/mod1.py
--rw-r--r--   0        0        0      653 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/params.py
--rw-r--r--   0        0        0       38 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/pytest/appmap.yml
--rw-r--r--   0        0        0     2931 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/pytest/expected/pytest.appmap.json
--rw-r--r--   0        0        0      213 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/pytest/expected/status_errored.metadata.json
--rw-r--r--   0        0        0      221 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/pytest/expected/status_failed.metadata.json
--rw-r--r--   0        0        0      221 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/pytest/expected/status_xfailed.metadata.json
--rw-r--r--   0        0        0      186 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/pytest/simple.py
--rw-r--r--   0        0        0      295 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/pytest/test_noappmap.py
--rw-r--r--   0        0        0      393 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/pytest/test_simple.py
--rw-r--r--   0        0        0     1246 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/remote.appmap.json
--rw-r--r--   0        0        0       13 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/trial/.gitignore
--rw-r--r--   0        0        0       38 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/trial/appmap.yml
--rw-r--r--   0        0        0     1897 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/trial/expected/pytest.appmap.json
--rw-r--r--   0        0        0       14 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/trial/init/sitecustomize.py
--rw-r--r--   0        0        0        0 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/trial/test/__init__.py
--rw-r--r--   0        0        0      400 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/trial/test/test_deferred.py
--rw-r--r--   0        0        0       38 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/unittest/appmap.yml
--rw-r--r--   0        0        0     4428 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/unittest/expected/pytest.appmap.json
--rw-r--r--   0        0        0      220 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/unittest/expected/status_errored.metadata.json
--rw-r--r--   0        0        0      238 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/unittest/expected/status_failed.metadata.json
--rw-r--r--   0        0        0      238 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/unittest/expected/status_xfailed.metadata.json
--rw-r--r--   0        0        0       33 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/unittest/expected/status_xsucceeded.metadata.json
--rw-r--r--   0        0        0     4430 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/unittest/expected/unittest.appmap.json
--rw-r--r--   0        0        0       14 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/unittest/init/sitecustomize.py
--rw-r--r--   0        0        0      275 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/unittest/simple/__init__.py
--rw-r--r--   0        0        0      183 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/unittest/simple/test_noappmap.py
--rw-r--r--   0        0        0     1263 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/data/unittest/simple/test_simple.py
--rw-r--r--   0        0        0      734 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/helpers.py
--rw-r--r--   0        0        0     4761 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/normalize.py
--rw-r--r--   0        0        0     4983 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/test_command.py
--rw-r--r--   0        0        0    11609 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/test_configuration.py
--rw-r--r--   0        0        0     3401 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/test_describe_value.py
--rw-r--r--   0        0        0     8341 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/test_django.py
--rw-r--r--   0        0        0      943 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/test_django_simplelazyobject.py
--rw-r--r--   0        0        0      338 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/test_env.py
--rw-r--r--   0        0        0     3198 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/test_events.py
--rw-r--r--   0        0        0     2732 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/test_fastapi.py
--rw-r--r--   0        0        0     5065 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/test_flask.py
--rw-r--r--   0        0        0     1703 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/test_generation.py
--rw-r--r--   0        0        0     1548 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/test_http.py
--rw-r--r--   0        0        0     1533 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/test_importer.py
--rw-r--r--   0        0        0     2931 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/test_labels.py
--rw-r--r--   0        0        0     1470 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/test_metadata.py
--rw-r--r--   0        0        0     9877 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/test_params.py
--rw-r--r--   0        0        0     6706 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/test_recording.py
--rw-r--r--   0        0        0     2006 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/test_runner.py
--rw-r--r--   0        0        0     3086 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/test_sqlalchemy.py
--rw-r--r--   0        0        0     7261 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/test_test_frameworks.py
--rw-r--r--   0        0        0      861 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/test_util.py
--rw-r--r--   0        0        0    15340 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/test/web_framework.py
--rw-r--r--   0        0        0     4828 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/testing_framework.py
--rw-r--r--   0        0        0      370 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/trace_logger.py
--rw-r--r--   0        0        0     2950 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/unittest.py
--rw-r--r--   0        0        0     6652 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/utils.py
--rw-r--r--   0        0        0     8622 2024-05-23 22:54:15.348025 appmap-2.0.1/_appmap/web_framework.py
--rw-r--r--   0        0        0     1832 2024-05-23 22:54:15.348025 appmap-2.0.1/appmap/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 22:54:15.348025 appmap-2.0.1/appmap/command/__init__.py
--rw-r--r--   0        0        0      420 2024-05-23 22:54:15.348025 appmap-2.0.1/appmap/command/appmap_agent_init.py
--rw-r--r--   0        0        0     3475 2024-05-23 22:54:15.348025 appmap-2.0.1/appmap/command/appmap_agent_status.py
--rw-r--r--   0        0        0     2096 2024-05-23 22:54:15.348025 appmap-2.0.1/appmap/command/appmap_agent_validate.py
--rw-r--r--   0        0        0     3916 2024-05-23 22:54:15.348025 appmap-2.0.1/appmap/command/runner.py
--rw-r--r--   0        0        0    11401 2024-05-23 22:54:15.348025 appmap-2.0.1/appmap/django.py
--rw-r--r--   0        0        0     6590 2024-05-23 22:54:15.348025 appmap-2.0.1/appmap/fastapi.py
--rw-r--r--   0        0        0     7219 2024-05-23 22:54:15.348025 appmap-2.0.1/appmap/flask.py
--rw-r--r--   0        0        0     2695 2024-05-23 22:54:15.348025 appmap-2.0.1/appmap/http.py
--rw-r--r--   0        0        0      675 2024-05-23 22:54:15.348025 appmap-2.0.1/appmap/labeling/__init__.py
--rw-r--r--   0        0        0     3387 2024-05-23 22:54:15.348025 appmap-2.0.1/appmap/labeling/crypto.yml
--rw-r--r--   0        0        0     2097 2024-05-23 22:54:15.348025 appmap-2.0.1/appmap/labeling/django.yml
--rw-r--r--   0        0        0      630 2024-05-23 22:54:15.348025 appmap-2.0.1/appmap/labeling/flask.yml
--rw-r--r--   0        0        0      831 2024-05-23 22:54:15.348025 appmap-2.0.1/appmap/labeling/formats.yml
--rw-r--r--   0        0        0       50 2024-05-23 22:54:15.348025 appmap-2.0.1/appmap/labeling/http.yml
--rw-r--r--   0        0        0      196 2024-05-23 22:54:15.348025 appmap-2.0.1/appmap/labeling/jobs.yml
--rw-r--r--   0        0        0       55 2024-05-23 22:54:15.348025 appmap-2.0.1/appmap/labeling/jwt.yml
--rw-r--r--   0        0        0      137 2024-05-23 22:54:15.348025 appmap-2.0.1/appmap/labeling/logger.yml
--rw-r--r--   0        0        0      214 2024-05-23 22:54:15.348025 appmap-2.0.1/appmap/labeling/random.yml
--rw-r--r--   0        0        0     3282 2024-05-23 22:54:15.348025 appmap-2.0.1/appmap/pytest.py
--rw-r--r--   0        0        0     2295 2024-05-23 22:54:15.348025 appmap-2.0.1/appmap/sqlalchemy.py
--rw-r--r--   0        0        0      294 2024-05-23 22:54:15.348025 appmap-2.0.1/appmap/unittest.py
--rw-r--r--   0        0        0      818 2024-05-23 22:54:15.348025 appmap-2.0.1/appmap/uvicorn.py
--rw-r--r--   0        0        0       14 2024-05-23 22:54:15.348025 appmap-2.0.1/appmap.pth
--rw-r--r--   0        0        0     3272 2024-05-23 22:57:10.092721 appmap-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     1304 2024-05-23 22:54:15.352026 appmap-2.0.1/vendor/_appmap/wrapt/LICENSE
--rw-r--r--   0        0        0     1200 2024-05-23 22:54:15.352026 appmap-2.0.1/vendor/_appmap/wrapt/__init__.py
--rw-r--r--   0        0        0     1746 2024-05-23 22:54:15.352026 appmap-2.0.1/vendor/_appmap/wrapt/arguments.py
--rw-r--r--   0        0        0    21332 2024-05-23 22:54:15.352026 appmap-2.0.1/vendor/_appmap/wrapt/decorators.py
--rw-r--r--   0        0        0    10782 2024-05-23 22:54:15.352026 appmap-2.0.1/vendor/_appmap/wrapt/importer.py
--rw-r--r--   0        0        0    38753 2024-05-23 22:54:15.352026 appmap-2.0.1/vendor/_appmap/wrapt/wrappers.py
--rw-r--r--   0        0        0     5717 1970-01-01 00:00:00.000000 appmap-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1925 2024-05-27 10:39:00.495371 appmap-2.0.2/LICENSE
+-rw-r--r--   0        0        0     4534 2024-05-27 10:39:00.495371 appmap-2.0.2/README.md
+-rw-r--r--   0        0        0      502 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/__init__.py
+-rw-r--r--   0        0        0    15857 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/configuration.py
+-rw-r--r--   0        0        0     1082 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/django.py
+-rw-r--r--   0        0        0     6702 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/env.py
+-rw-r--r--   0        0        0    15677 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/event.py
+-rw-r--r--   0        0        0      694 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/fastapi.py
+-rw-r--r--   0        0        0      822 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/flask.py
+-rw-r--r--   0        0        0     3642 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/generation.py
+-rw-r--r--   0        0        0    11495 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/importer.py
+-rw-r--r--   0        0        0     4323 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/instrument.py
+-rw-r--r--   0        0        0     1786 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/labels.py
+-rw-r--r--   0        0        0     3071 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/metadata.py
+-rw-r--r--   0        0        0      267 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/noappmap.py
+-rw-r--r--   0        0        0      538 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/py_version_check.py
+-rw-r--r--   0        0        0     5513 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/recorder.py
+-rw-r--r--   0        0        0     2868 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/recording.py
+-rw-r--r--   0        0        0      926 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/remote_recording.py
+-rw-r--r--   0        0        0      340 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/singleton.py
+-rw-r--r--   0        0        0      174 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/__init__.py
+-rw-r--r--   0        0        0     3607 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/appmap_test_base.py
+-rwxr-xr-x   0        0        0      121 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/bin/server_runner
+-rw-r--r--   0        0        0     6048 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/conftest.py
+-rw-r--r--   0        0        0      112 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/appmap-all-paths-malformed.yml
+-rw-r--r--   0        0        0       50 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/appmap-broken.yml
+-rw-r--r--   0        0        0       82 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/appmap-class.yml
+-rw-r--r--   0        0        0       59 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/appmap-empty-path.yml
+-rw-r--r--   0        0        0      126 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/appmap-exclude-fn.yml
+-rw-r--r--   0        0        0       87 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/appmap-func.yml
+-rw-r--r--   0        0        0       82 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/appmap-malformed-path.yml
+-rw-r--r--   0        0        0      308 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/appmap-no-pyyaml.yml
+-rw-r--r--   0        0        0      323 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/appmap.yml
+-rw-r--r--   0        0        0        0 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/appmap_testing/__init__.py
+-rw-r--r--   0        0        0      237 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/appmap_testing/django_simplelazyobject.py
+-rw-r--r--   0        0        0        0 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/config/src/package/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/config/test/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/config/test/foo.py
+-rw-r--r--   0        0        0       16 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/config-exclude/.hide/hidden_mod/__init__.py
+-rw-r--r--   0        0        0       25 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/config-exclude/node_modules/node_mod/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/config-exclude/src/package/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/config-exclude/test/__init__.py
+-rw-r--r--   0        0        0       14 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/config-exclude/venv/venv_mod/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/config-up/appmap.yml
+-rw-r--r--   0        0        0        0 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/config-up/project/p1/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/config-up/project/p2/sub1/__init__.py
+-rw-r--r--   0        0        0       44 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/django/appmap.yml
+-rw-r--r--   0        0        0      495 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/django/djangoapp/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/django/djangoapp/djangoapp.py
+-rw-r--r--   0        0        0       39 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/django/djangoapp/hello_world.html
+-rw-r--r--   0        0        0      154 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/django/djangoapp/middleware.py
+-rw-r--r--   0        0        0      426 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/django/djangoapp/settings.py
+-rw-r--r--   0        0        0      563 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/django/djangoapp/settings_dev.py
+-rw-r--r--   0        0        0     2148 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/django/djangoapp/urls.py
+-rw-r--r--   0        0        0       14 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/django/init/sitecustomize.py
+-rwxr-xr-x   0        0        0      665 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/django/manage.py
+-rw-r--r--   0        0        0       53 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/django/pytest.ini
+-rw-r--r--   0        0        0        0 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/django/test/__init__.py
+-rw-r--r--   0        0        0      935 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/django/test/test_app.py
+-rw-r--r--   0        0        0     2591 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/example_class.py
+-rw-r--r--   0        0        0     7942 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/expected.appmap.json
+-rw-r--r--   0        0        0       47 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/fastapi/appmap.yml
+-rw-r--r--   0        0        0        0 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/fastapi/fastapiapp/__init__.py
+-rw-r--r--   0        0        0     1647 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/fastapi/fastapiapp/main.py
+-rw-r--r--   0        0        0       14 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/fastapi/init/sitecustomize.py
+-rw-r--r--   0        0        0      240 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/fastapi/test_app.py
+-rw-r--r--   0        0        0       38 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/flask/appmap.yml
+-rw-r--r--   0        0        0     1200 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/flask/flaskapp.py
+-rw-r--r--   0        0        0       14 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/flask/init/sitecustomize.py
+-rw-r--r--   0        0        0        0 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/flask/templates/test.html
+-rw-r--r--   0        0        0      268 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/flask/test_app.py
+-rw-r--r--   0        0        0        0 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/package1/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/package1/package2/__init__.py
+-rw-r--r--   0        0        0      113 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/package1/package2/__main__.py
+-rw-r--r--   0        0        0       69 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/package1/package2/mod1.py
+-rw-r--r--   0        0        0      653 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/params.py
+-rw-r--r--   0        0        0       38 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/pytest/appmap.yml
+-rw-r--r--   0        0        0     2931 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/pytest/expected/pytest.appmap.json
+-rw-r--r--   0        0        0      213 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/pytest/expected/status_errored.metadata.json
+-rw-r--r--   0        0        0      221 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/pytest/expected/status_failed.metadata.json
+-rw-r--r--   0        0        0      221 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/pytest/expected/status_xfailed.metadata.json
+-rw-r--r--   0        0        0      186 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/pytest/simple.py
+-rw-r--r--   0        0        0      295 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/pytest/test_noappmap.py
+-rw-r--r--   0        0        0      393 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/pytest/test_simple.py
+-rw-r--r--   0        0        0     1246 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/remote.appmap.json
+-rw-r--r--   0        0        0       13 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/trial/.gitignore
+-rw-r--r--   0        0        0       38 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/trial/appmap.yml
+-rw-r--r--   0        0        0     1897 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/trial/expected/pytest.appmap.json
+-rw-r--r--   0        0        0       14 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/trial/init/sitecustomize.py
+-rw-r--r--   0        0        0        0 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/trial/test/__init__.py
+-rw-r--r--   0        0        0      400 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/trial/test/test_deferred.py
+-rw-r--r--   0        0        0       38 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/unittest/appmap.yml
+-rw-r--r--   0        0        0     4428 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/unittest/expected/pytest.appmap.json
+-rw-r--r--   0        0        0      220 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/unittest/expected/status_errored.metadata.json
+-rw-r--r--   0        0        0      238 2024-05-27 10:39:00.495371 appmap-2.0.2/_appmap/test/data/unittest/expected/status_failed.metadata.json
+-rw-r--r--   0        0        0      238 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/test/data/unittest/expected/status_xfailed.metadata.json
+-rw-r--r--   0        0        0       33 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/test/data/unittest/expected/status_xsucceeded.metadata.json
+-rw-r--r--   0        0        0     4430 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/test/data/unittest/expected/unittest.appmap.json
+-rw-r--r--   0        0        0       14 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/test/data/unittest/init/sitecustomize.py
+-rw-r--r--   0        0        0      275 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/test/data/unittest/simple/__init__.py
+-rw-r--r--   0        0        0      183 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/test/data/unittest/simple/test_noappmap.py
+-rw-r--r--   0        0        0     1263 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/test/data/unittest/simple/test_simple.py
+-rw-r--r--   0        0        0      734 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/test/helpers.py
+-rw-r--r--   0        0        0     4761 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/test/normalize.py
+-rw-r--r--   0        0        0     4983 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/test/test_command.py
+-rw-r--r--   0        0        0    11609 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/test/test_configuration.py
+-rw-r--r--   0        0        0     3401 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/test/test_describe_value.py
+-rw-r--r--   0        0        0     8341 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/test/test_django.py
+-rw-r--r--   0        0        0      943 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/test/test_django_simplelazyobject.py
+-rw-r--r--   0        0        0      338 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/test/test_env.py
+-rw-r--r--   0        0        0     3198 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/test/test_events.py
+-rw-r--r--   0        0        0     2732 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/test/test_fastapi.py
+-rw-r--r--   0        0        0     5065 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/test/test_flask.py
+-rw-r--r--   0        0        0     1703 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/test/test_generation.py
+-rw-r--r--   0        0        0     1548 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/test/test_http.py
+-rw-r--r--   0        0        0     1533 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/test/test_importer.py
+-rw-r--r--   0        0        0     2931 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/test/test_labels.py
+-rw-r--r--   0        0        0     1470 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/test/test_metadata.py
+-rw-r--r--   0        0        0     9877 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/test/test_params.py
+-rw-r--r--   0        0        0     6706 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/test/test_recording.py
+-rw-r--r--   0        0        0     2006 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/test/test_runner.py
+-rw-r--r--   0        0        0     3086 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/test/test_sqlalchemy.py
+-rw-r--r--   0        0        0     7261 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/test/test_test_frameworks.py
+-rw-r--r--   0        0        0      861 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/test/test_util.py
+-rw-r--r--   0        0        0    15340 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/test/web_framework.py
+-rw-r--r--   0        0        0     4828 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/testing_framework.py
+-rw-r--r--   0        0        0      370 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/trace_logger.py
+-rw-r--r--   0        0        0     2950 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/unittest.py
+-rw-r--r--   0        0        0     6652 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/utils.py
+-rw-r--r--   0        0        0     8622 2024-05-27 10:39:00.499371 appmap-2.0.2/_appmap/web_framework.py
+-rw-r--r--   0        0        0     1832 2024-05-27 10:39:00.499371 appmap-2.0.2/appmap/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 10:39:00.499371 appmap-2.0.2/appmap/command/__init__.py
+-rw-r--r--   0        0        0      420 2024-05-27 10:39:00.499371 appmap-2.0.2/appmap/command/appmap_agent_init.py
+-rw-r--r--   0        0        0     3475 2024-05-27 10:39:00.499371 appmap-2.0.2/appmap/command/appmap_agent_status.py
+-rw-r--r--   0        0        0     2096 2024-05-27 10:39:00.499371 appmap-2.0.2/appmap/command/appmap_agent_validate.py
+-rw-r--r--   0        0        0     3916 2024-05-27 10:39:00.499371 appmap-2.0.2/appmap/command/runner.py
+-rw-r--r--   0        0        0    11401 2024-05-27 10:39:00.499371 appmap-2.0.2/appmap/django.py
+-rw-r--r--   0        0        0     6590 2024-05-27 10:39:00.499371 appmap-2.0.2/appmap/fastapi.py
+-rw-r--r--   0        0        0     7219 2024-05-27 10:39:00.499371 appmap-2.0.2/appmap/flask.py
+-rw-r--r--   0        0        0     2695 2024-05-27 10:39:00.499371 appmap-2.0.2/appmap/http.py
+-rw-r--r--   0        0        0      675 2024-05-27 10:39:00.499371 appmap-2.0.2/appmap/labeling/__init__.py
+-rw-r--r--   0        0        0     3387 2024-05-27 10:39:00.499371 appmap-2.0.2/appmap/labeling/crypto.yml
+-rw-r--r--   0        0        0     2097 2024-05-27 10:39:00.499371 appmap-2.0.2/appmap/labeling/django.yml
+-rw-r--r--   0        0        0      630 2024-05-27 10:39:00.499371 appmap-2.0.2/appmap/labeling/flask.yml
+-rw-r--r--   0        0        0      831 2024-05-27 10:39:00.499371 appmap-2.0.2/appmap/labeling/formats.yml
+-rw-r--r--   0        0        0       50 2024-05-27 10:39:00.499371 appmap-2.0.2/appmap/labeling/http.yml
+-rw-r--r--   0        0        0      196 2024-05-27 10:39:00.499371 appmap-2.0.2/appmap/labeling/jobs.yml
+-rw-r--r--   0        0        0       55 2024-05-27 10:39:00.499371 appmap-2.0.2/appmap/labeling/jwt.yml
+-rw-r--r--   0        0        0      137 2024-05-27 10:39:00.499371 appmap-2.0.2/appmap/labeling/logger.yml
+-rw-r--r--   0        0        0      214 2024-05-27 10:39:00.499371 appmap-2.0.2/appmap/labeling/random.yml
+-rw-r--r--   0        0        0     3282 2024-05-27 10:39:00.499371 appmap-2.0.2/appmap/pytest.py
+-rw-r--r--   0        0        0     2295 2024-05-27 10:39:00.499371 appmap-2.0.2/appmap/sqlalchemy.py
+-rw-r--r--   0        0        0      294 2024-05-27 10:39:00.499371 appmap-2.0.2/appmap/unittest.py
+-rw-r--r--   0        0        0      818 2024-05-27 10:39:00.499371 appmap-2.0.2/appmap/uvicorn.py
+-rw-r--r--   0        0        0       14 2024-05-27 10:39:00.499371 appmap-2.0.2/appmap.pth
+-rw-r--r--   0        0        0     3272 2024-05-27 10:41:47.209719 appmap-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1304 2024-05-27 10:39:00.499371 appmap-2.0.2/vendor/_appmap/wrapt/LICENSE
+-rw-r--r--   0        0        0     1200 2024-05-27 10:39:00.499371 appmap-2.0.2/vendor/_appmap/wrapt/__init__.py
+-rw-r--r--   0        0        0     1746 2024-05-27 10:39:00.499371 appmap-2.0.2/vendor/_appmap/wrapt/arguments.py
+-rw-r--r--   0        0        0    21332 2024-05-27 10:39:00.499371 appmap-2.0.2/vendor/_appmap/wrapt/decorators.py
+-rw-r--r--   0        0        0    10782 2024-05-27 10:39:00.499371 appmap-2.0.2/vendor/_appmap/wrapt/importer.py
+-rw-r--r--   0        0        0    38753 2024-05-27 10:39:00.499371 appmap-2.0.2/vendor/_appmap/wrapt/wrappers.py
+-rw-r--r--   0        0        0     5717 1970-01-01 00:00:00.000000 appmap-2.0.2/PKG-INFO
```

### Comparing `appmap-2.0.1/LICENSE` & `appmap-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/README.md` & `appmap-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/configuration.py` & `appmap-2.0.2/_appmap/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -478,12 +478,11 @@
 c = Config.current
 # For various reasons, this code runs more than once on startup. Use an
 # environment variable to make sure the user only sees startup messages once.
 _startup_messages_shown = os.environ.get("_APPMAP_MESSAGES_SHOWN")
 if _startup_messages_shown is None:
     # pylint: disable=protected-access
     c._load_config(show_warnings=True)
-    logger.info("file: %s", c._file)
-    logger.info("config: %s", c._config)
+    logger.info("file: %s", c._file if c.file_present else "[no appmap.yml]")
     logger.debug("package_functions: %s", c.package_functions)
     logger.info("env: %r", os.environ)
     os.environ["_APPMAP_MESSAGES_SHOWN"] = "true"
```

### Comparing `appmap-2.0.1/_appmap/django.py` & `appmap-2.0.2/_appmap/django.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/env.py` & `appmap-2.0.2/_appmap/env.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/event.py` & `appmap-2.0.2/_appmap/event.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/fastapi.py` & `appmap-2.0.2/_appmap/fastapi.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/flask.py` & `appmap-2.0.2/_appmap/flask.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/generation.py` & `appmap-2.0.2/_appmap/generation.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/importer.py` & `appmap-2.0.2/_appmap/importer.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/instrument.py` & `appmap-2.0.2/_appmap/instrument.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/labels.py` & `appmap-2.0.2/_appmap/labels.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/metadata.py` & `appmap-2.0.2/_appmap/metadata.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/py_version_check.py` & `appmap-2.0.2/_appmap/py_version_check.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/recorder.py` & `appmap-2.0.2/_appmap/recorder.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/recording.py` & `appmap-2.0.2/_appmap/recording.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/remote_recording.py` & `appmap-2.0.2/_appmap/remote_recording.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/appmap_test_base.py` & `appmap-2.0.2/_appmap/test/appmap_test_base.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/conftest.py` & `appmap-2.0.2/_appmap/test/conftest.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/data/django/djangoapp/settings_dev.py` & `appmap-2.0.2/_appmap/test/data/django/djangoapp/settings_dev.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/data/django/djangoapp/urls.py` & `appmap-2.0.2/_appmap/test/data/django/djangoapp/urls.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/data/django/manage.py` & `appmap-2.0.2/_appmap/test/data/django/manage.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/data/django/test/test_app.py` & `appmap-2.0.2/_appmap/test/data/django/test/test_app.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/data/example_class.py` & `appmap-2.0.2/_appmap/test/data/example_class.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/data/expected.appmap.json` & `appmap-2.0.2/_appmap/test/data/expected.appmap.json`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/data/fastapi/fastapiapp/main.py` & `appmap-2.0.2/_appmap/test/data/fastapi/fastapiapp/main.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/data/flask/flaskapp.py` & `appmap-2.0.2/_appmap/test/data/flask/flaskapp.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/data/params.py` & `appmap-2.0.2/_appmap/test/data/params.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/data/pytest/expected/pytest.appmap.json` & `appmap-2.0.2/_appmap/test/data/pytest/expected/pytest.appmap.json`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/data/remote.appmap.json` & `appmap-2.0.2/_appmap/test/data/remote.appmap.json`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/data/trial/expected/pytest.appmap.json` & `appmap-2.0.2/_appmap/test/data/trial/expected/pytest.appmap.json`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/data/unittest/expected/pytest.appmap.json` & `appmap-2.0.2/_appmap/test/data/unittest/expected/pytest.appmap.json`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/data/unittest/expected/unittest.appmap.json` & `appmap-2.0.2/_appmap/test/data/unittest/expected/unittest.appmap.json`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/data/unittest/simple/test_simple.py` & `appmap-2.0.2/_appmap/test/data/unittest/simple/test_simple.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/helpers.py` & `appmap-2.0.2/_appmap/test/helpers.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/normalize.py` & `appmap-2.0.2/_appmap/test/normalize.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/test_command.py` & `appmap-2.0.2/_appmap/test/test_command.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/test_configuration.py` & `appmap-2.0.2/_appmap/test/test_configuration.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/test_describe_value.py` & `appmap-2.0.2/_appmap/test/test_describe_value.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/test_django.py` & `appmap-2.0.2/_appmap/test/test_django.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/test_django_simplelazyobject.py` & `appmap-2.0.2/_appmap/test/test_django_simplelazyobject.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/test_events.py` & `appmap-2.0.2/_appmap/test/test_events.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/test_fastapi.py` & `appmap-2.0.2/_appmap/test/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/test_flask.py` & `appmap-2.0.2/_appmap/test/test_flask.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/test_generation.py` & `appmap-2.0.2/_appmap/test/test_generation.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/test_http.py` & `appmap-2.0.2/_appmap/test/test_http.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/test_importer.py` & `appmap-2.0.2/_appmap/test/test_importer.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/test_labels.py` & `appmap-2.0.2/_appmap/test/test_labels.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/test_metadata.py` & `appmap-2.0.2/_appmap/test/test_metadata.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/test_params.py` & `appmap-2.0.2/_appmap/test/test_params.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/test_recording.py` & `appmap-2.0.2/_appmap/test/test_recording.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/test_runner.py` & `appmap-2.0.2/_appmap/test/test_runner.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/test_sqlalchemy.py` & `appmap-2.0.2/_appmap/test/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/test_test_frameworks.py` & `appmap-2.0.2/_appmap/test/test_test_frameworks.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/test_util.py` & `appmap-2.0.2/_appmap/test/test_util.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/test/web_framework.py` & `appmap-2.0.2/_appmap/test/web_framework.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/testing_framework.py` & `appmap-2.0.2/_appmap/testing_framework.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/unittest.py` & `appmap-2.0.2/_appmap/unittest.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/utils.py` & `appmap-2.0.2/_appmap/utils.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/_appmap/web_framework.py` & `appmap-2.0.2/_appmap/web_framework.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/appmap/__init__.py` & `appmap-2.0.2/appmap/__init__.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/appmap/command/appmap_agent_status.py` & `appmap-2.0.2/appmap/command/appmap_agent_status.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/appmap/command/appmap_agent_validate.py` & `appmap-2.0.2/appmap/command/appmap_agent_validate.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/appmap/command/runner.py` & `appmap-2.0.2/appmap/command/runner.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/appmap/django.py` & `appmap-2.0.2/appmap/django.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/appmap/fastapi.py` & `appmap-2.0.2/appmap/fastapi.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/appmap/flask.py` & `appmap-2.0.2/appmap/flask.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/appmap/http.py` & `appmap-2.0.2/appmap/http.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/appmap/labeling/__init__.py` & `appmap-2.0.2/appmap/labeling/__init__.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/appmap/labeling/crypto.yml` & `appmap-2.0.2/appmap/labeling/crypto.yml`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/appmap/labeling/django.yml` & `appmap-2.0.2/appmap/labeling/django.yml`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/appmap/labeling/flask.yml` & `appmap-2.0.2/appmap/labeling/flask.yml`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/appmap/labeling/formats.yml` & `appmap-2.0.2/appmap/labeling/formats.yml`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/appmap/pytest.py` & `appmap-2.0.2/appmap/pytest.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/appmap/sqlalchemy.py` & `appmap-2.0.2/appmap/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/appmap/uvicorn.py` & `appmap-2.0.2/appmap/uvicorn.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/pyproject.toml` & `appmap-2.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "appmap"
-version = "2.0.1"
+version = "2.0.2"
 description = "Create AppMap files by recording a Python application."
 readme = "README.md"
 authors = [
   "Alan Potter <alan@app.land>",
   "Viraj Kanwade <viraj.kanwade@forgeahead.io>",
   "Rafał Rzepecki <rafal@app.land>"
 ]
```

### Comparing `appmap-2.0.1/vendor/_appmap/wrapt/LICENSE` & `appmap-2.0.2/vendor/_appmap/wrapt/LICENSE`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/vendor/_appmap/wrapt/__init__.py` & `appmap-2.0.2/vendor/_appmap/wrapt/__init__.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/vendor/_appmap/wrapt/arguments.py` & `appmap-2.0.2/vendor/_appmap/wrapt/arguments.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/vendor/_appmap/wrapt/decorators.py` & `appmap-2.0.2/vendor/_appmap/wrapt/decorators.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/vendor/_appmap/wrapt/importer.py` & `appmap-2.0.2/vendor/_appmap/wrapt/importer.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/vendor/_appmap/wrapt/wrappers.py` & `appmap-2.0.2/vendor/_appmap/wrapt/wrappers.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.1/PKG-INFO` & `appmap-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appmap
-Version: 2.0.1
+Version: 2.0.2
 Summary: Create AppMap files by recording a Python application.
 Home-page: https://github.com/applandinc/appmap-python
 License: MIT
 Author: Alan Potter
 Author-email: alan@app.land
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

