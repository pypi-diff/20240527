# Comparing `tmp/ytmusicapi-1.7.2.tar.gz` & `tmp/ytmusicapi-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytmusicapi-1.7.2.tar", last modified: Mon May 20 19:57:38 2024, max compression
+gzip compressed data, was "ytmusicapi-1.7.3.tar", last modified: Mon May 27 19:20:07 2024, max compression
```

## Comparing `ytmusicapi-1.7.2.tar` & `ytmusicapi-1.7.3.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.735709 ytmusicapi-1.7.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.711708 ytmusicapi-1.7.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.711708 ytmusicapi-1.7.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.711708 ytmusicapi-1.7.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/.github/workflows/docsbuild.yml
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/.github/workflows/pdm.yml
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-20 19:57:38.735709 ytmusicapi-1.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.711708 ytmusicapi-1.7.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.715708 ytmusicapi-1.7.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/docs/source/reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/docs/source/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.715708 ytmusicapi-1.7.2/docs/source/setup/
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/docs/source/setup/browser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/docs/source/setup/headers_auth.json.example
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/docs/source/setup/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/docs/source/setup/oauth.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)    61554 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/pdm.lock
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 19:57:38.735709 ytmusicapi-1.7.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.715708 ytmusicapi-1.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/tests/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.715708 ytmusicapi-1.7.2/tests/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/tests/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/tests/auth/test_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/tests/auth/test_oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.719708 ytmusicapi-1.7.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)   226650 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/tests/data/2024_03_get_album.json
--rw-r--r--   0 runner    (1001) docker     (127)  1039226 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/tests/data/2024_03_get_playlist.json
--rw-r--r--   0 runner    (1001) docker     (127)  1004367 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/tests/data/2024_03_get_playlist_public.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.723708 ytmusicapi-1.7.2/tests/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/tests/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/tests/mixins/test_browsing.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/tests/mixins/test_explore.py
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/tests/mixins/test_library.py
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/tests/mixins/test_playlists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/tests/mixins/test_podcasts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/tests/mixins/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/tests/mixins/test_uploads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/tests/mixins/test_watch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.723708 ytmusicapi-1.7.2/tests/setup/
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/tests/setup/setup_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/tests/test.example.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/tests/test_ytmusic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.723708 ytmusicapi-1.7.2/ytmusicapi/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.723708 ytmusicapi-1.7.2/ytmusicapi/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/auth/browser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.727708 ytmusicapi-1.7.2/ytmusicapi/auth/oauth/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/auth/oauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/auth/oauth/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/auth/oauth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/auth/oauth/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/auth/oauth/token.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/auth/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/continuations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.727708 ytmusicapi-1.7.2/ytmusicapi/locales/
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.707708 ytmusicapi-1.7.2/ytmusicapi/locales/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.727708 ytmusicapi-1.7.2/ytmusicapi/locales/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/ar/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/ar/LC_MESSAGES/base.po
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/base.pot
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.707708 ytmusicapi-1.7.2/ytmusicapi/locales/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.727708 ytmusicapi-1.7.2/ytmusicapi/locales/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/de/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/de/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.707708 ytmusicapi-1.7.2/ytmusicapi/locales/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.727708 ytmusicapi-1.7.2/ytmusicapi/locales/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/en/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/en/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.707708 ytmusicapi-1.7.2/ytmusicapi/locales/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.727708 ytmusicapi-1.7.2/ytmusicapi/locales/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/es/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/es/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.707708 ytmusicapi-1.7.2/ytmusicapi/locales/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.727708 ytmusicapi-1.7.2/ytmusicapi/locales/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/fr/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/fr/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.707708 ytmusicapi-1.7.2/ytmusicapi/locales/hi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.727708 ytmusicapi-1.7.2/ytmusicapi/locales/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/hi/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/hi/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.707708 ytmusicapi-1.7.2/ytmusicapi/locales/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.727708 ytmusicapi-1.7.2/ytmusicapi/locales/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/it/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/it/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.707708 ytmusicapi-1.7.2/ytmusicapi/locales/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.727708 ytmusicapi-1.7.2/ytmusicapi/locales/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/ja/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/ja/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.707708 ytmusicapi-1.7.2/ytmusicapi/locales/ko/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.731708 ytmusicapi-1.7.2/ytmusicapi/locales/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/ko/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/ko/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.707708 ytmusicapi-1.7.2/ytmusicapi/locales/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.731708 ytmusicapi-1.7.2/ytmusicapi/locales/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/nl/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/nl/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.707708 ytmusicapi-1.7.2/ytmusicapi/locales/pt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.731708 ytmusicapi-1.7.2/ytmusicapi/locales/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/pt/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/pt/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.707708 ytmusicapi-1.7.2/ytmusicapi/locales/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.731708 ytmusicapi-1.7.2/ytmusicapi/locales/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/ru/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/ru/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.707708 ytmusicapi-1.7.2/ytmusicapi/locales/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.731708 ytmusicapi-1.7.2/ytmusicapi/locales/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/tr/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/tr/LC_MESSAGES/base.po
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/update_mo.sh
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/update_po.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.707708 ytmusicapi-1.7.2/ytmusicapi/locales/ur/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.731708 ytmusicapi-1.7.2/ytmusicapi/locales/ur/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/ur/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/ur/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.707708 ytmusicapi-1.7.2/ytmusicapi/locales/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.731708 ytmusicapi-1.7.2/ytmusicapi/locales/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.711708 ytmusicapi-1.7.2/ytmusicapi/locales/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.731708 ytmusicapi-1.7.2/ytmusicapi/locales/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.735709 ytmusicapi-1.7.2/ytmusicapi/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/mixins/_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/mixins/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    39178 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/mixins/browsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/mixins/explore.py
--rw-r--r--   0 runner    (1001) docker     (127)    17492 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/mixins/library.py
--rw-r--r--   0 runner    (1001) docker     (127)    20529 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/mixins/playlists.py
--rw-r--r--   0 runner    (1001) docker     (127)     9836 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/mixins/podcasts.py
--rw-r--r--   0 runner    (1001) docker     (127)    12370 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/mixins/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    10742 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/mixins/uploads.py
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/mixins/watch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.735709 ytmusicapi-1.7.2/ytmusicapi/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/parsers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/parsers/albums.py
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/parsers/browsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/parsers/explore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/parsers/i18n.py
--rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/parsers/library.py
--rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/parsers/playlists.py
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/parsers/podcasts.py
--rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/parsers/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/parsers/songs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/parsers/uploads.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/parsers/watch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    11518 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/ytmusic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.735709 ytmusicapi-1.7.2/ytmusicapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-20 19:57:38.000000 ytmusicapi-1.7.2/ytmusicapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-05-20 19:57:38.000000 ytmusicapi-1.7.2/ytmusicapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 19:57:38.000000 ytmusicapi-1.7.2/ytmusicapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-20 19:57:38.000000 ytmusicapi-1.7.2/ytmusicapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-20 19:57:38.000000 ytmusicapi-1.7.2/ytmusicapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-20 19:57:38.000000 ytmusicapi-1.7.2/ytmusicapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.690034 ytmusicapi-1.7.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.666033 ytmusicapi-1.7.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.666033 ytmusicapi-1.7.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.670033 ytmusicapi-1.7.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/.github/workflows/docsbuild.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/.github/workflows/pdm.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-27 19:20:07.690034 ytmusicapi-1.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.670033 ytmusicapi-1.7.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.670033 ytmusicapi-1.7.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/docs/source/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/docs/source/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.670033 ytmusicapi-1.7.3/docs/source/setup/
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/docs/source/setup/browser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/docs/source/setup/headers_auth.json.example
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/docs/source/setup/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/docs/source/setup/oauth.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    61554 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/pdm.lock
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 19:20:07.690034 ytmusicapi-1.7.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.670033 ytmusicapi-1.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/tests/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.670033 ytmusicapi-1.7.3/tests/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/tests/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/tests/auth/test_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/tests/auth/test_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.674033 ytmusicapi-1.7.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   226650 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/tests/data/2024_03_get_album.json
+-rw-r--r--   0 runner    (1001) docker     (127)  1039226 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/tests/data/2024_03_get_playlist.json
+-rw-r--r--   0 runner    (1001) docker     (127)  1004367 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/tests/data/2024_03_get_playlist_public.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.678033 ytmusicapi-1.7.3/tests/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/tests/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/tests/mixins/test_browsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/tests/mixins/test_explore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/tests/mixins/test_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/tests/mixins/test_playlists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/tests/mixins/test_podcasts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/tests/mixins/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/tests/mixins/test_uploads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/tests/mixins/test_watch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.678033 ytmusicapi-1.7.3/tests/setup/
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/tests/setup/setup_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/tests/test.example.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/tests/test_ytmusic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.678033 ytmusicapi-1.7.3/ytmusicapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.678033 ytmusicapi-1.7.3/ytmusicapi/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/auth/browser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.682034 ytmusicapi-1.7.3/ytmusicapi/auth/oauth/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/auth/oauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/auth/oauth/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/auth/oauth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/auth/oauth/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/auth/oauth/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/auth/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/continuations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.682034 ytmusicapi-1.7.3/ytmusicapi/locales/
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.662033 ytmusicapi-1.7.3/ytmusicapi/locales/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.682034 ytmusicapi-1.7.3/ytmusicapi/locales/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/ar/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/ar/LC_MESSAGES/base.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/base.pot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.662033 ytmusicapi-1.7.3/ytmusicapi/locales/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.682034 ytmusicapi-1.7.3/ytmusicapi/locales/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/de/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/de/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.662033 ytmusicapi-1.7.3/ytmusicapi/locales/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.682034 ytmusicapi-1.7.3/ytmusicapi/locales/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/en/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/en/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.662033 ytmusicapi-1.7.3/ytmusicapi/locales/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.682034 ytmusicapi-1.7.3/ytmusicapi/locales/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/es/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/es/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.662033 ytmusicapi-1.7.3/ytmusicapi/locales/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.682034 ytmusicapi-1.7.3/ytmusicapi/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/fr/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/fr/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.662033 ytmusicapi-1.7.3/ytmusicapi/locales/hi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.682034 ytmusicapi-1.7.3/ytmusicapi/locales/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/hi/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/hi/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.662033 ytmusicapi-1.7.3/ytmusicapi/locales/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.682034 ytmusicapi-1.7.3/ytmusicapi/locales/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/it/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/it/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.662033 ytmusicapi-1.7.3/ytmusicapi/locales/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.682034 ytmusicapi-1.7.3/ytmusicapi/locales/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/ja/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/ja/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.662033 ytmusicapi-1.7.3/ytmusicapi/locales/ko/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.686034 ytmusicapi-1.7.3/ytmusicapi/locales/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/ko/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/ko/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.662033 ytmusicapi-1.7.3/ytmusicapi/locales/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.686034 ytmusicapi-1.7.3/ytmusicapi/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/nl/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/nl/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.662033 ytmusicapi-1.7.3/ytmusicapi/locales/pt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.686034 ytmusicapi-1.7.3/ytmusicapi/locales/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/pt/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/pt/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.662033 ytmusicapi-1.7.3/ytmusicapi/locales/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.686034 ytmusicapi-1.7.3/ytmusicapi/locales/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/ru/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/ru/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.662033 ytmusicapi-1.7.3/ytmusicapi/locales/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.686034 ytmusicapi-1.7.3/ytmusicapi/locales/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/tr/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/tr/LC_MESSAGES/base.po
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/update_mo.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/update_po.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.666033 ytmusicapi-1.7.3/ytmusicapi/locales/ur/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.686034 ytmusicapi-1.7.3/ytmusicapi/locales/ur/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/ur/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/ur/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.666033 ytmusicapi-1.7.3/ytmusicapi/locales/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.686034 ytmusicapi-1.7.3/ytmusicapi/locales/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.666033 ytmusicapi-1.7.3/ytmusicapi/locales/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.686034 ytmusicapi-1.7.3/ytmusicapi/locales/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.690034 ytmusicapi-1.7.3/ytmusicapi/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/mixins/_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/mixins/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39126 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/mixins/browsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/mixins/explore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17492 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/mixins/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20529 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/mixins/playlists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9836 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/mixins/podcasts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12432 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/mixins/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10742 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/mixins/uploads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/mixins/watch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.690034 ytmusicapi-1.7.3/ytmusicapi/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/parsers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/parsers/albums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/parsers/browsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/parsers/explore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/parsers/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/parsers/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/parsers/playlists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/parsers/podcasts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10927 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/parsers/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/parsers/songs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/parsers/uploads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/parsers/watch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11518 2024-05-27 19:20:02.000000 ytmusicapi-1.7.3/ytmusicapi/ytmusic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:07.690034 ytmusicapi-1.7.3/ytmusicapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-27 19:20:07.000000 ytmusicapi-1.7.3/ytmusicapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-05-27 19:20:07.000000 ytmusicapi-1.7.3/ytmusicapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 19:20:07.000000 ytmusicapi-1.7.3/ytmusicapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-27 19:20:07.000000 ytmusicapi-1.7.3/ytmusicapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-27 19:20:07.000000 ytmusicapi-1.7.3/ytmusicapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 19:20:07.000000 ytmusicapi-1.7.3/ytmusicapi.egg-info/top_level.txt
```

### Comparing `ytmusicapi-1.7.2/.github/ISSUE_TEMPLATE/bug_report.md` & `ytmusicapi-1.7.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/.github/ISSUE_TEMPLATE/feature_request.md` & `ytmusicapi-1.7.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/.github/dependabot.yml` & `ytmusicapi-1.7.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/.github/workflows/coverage.yml` & `ytmusicapi-1.7.3/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/.github/workflows/docsbuild.yml` & `ytmusicapi-1.7.3/.github/workflows/docsbuild.yml`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/.github/workflows/lint.yml` & `ytmusicapi-1.7.3/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/.github/workflows/pythonpublish.yml` & `ytmusicapi-1.7.3/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/CONTRIBUTING.rst` & `ytmusicapi-1.7.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/LICENSE` & `ytmusicapi-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/PKG-INFO` & `ytmusicapi-1.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytmusicapi
-Version: 1.7.2
+Version: 1.7.3
 Summary: Unofficial API for YouTube Music
 Author-email: sigma67 <ytmusicapi@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 sigma67
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ytmusicapi-1.7.2/README.rst` & `ytmusicapi-1.7.3/README.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/docs/Makefile` & `ytmusicapi-1.7.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/docs/make.bat` & `ytmusicapi-1.7.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/docs/source/conf.py` & `ytmusicapi-1.7.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/docs/source/faq.rst` & `ytmusicapi-1.7.3/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/docs/source/index.rst` & `ytmusicapi-1.7.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/docs/source/reference.rst` & `ytmusicapi-1.7.3/docs/source/reference.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/docs/source/setup/browser.rst` & `ytmusicapi-1.7.3/docs/source/setup/browser.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/docs/source/usage.rst` & `ytmusicapi-1.7.3/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/pdm.lock` & `ytmusicapi-1.7.3/pdm.lock`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/pyproject.toml` & `ytmusicapi-1.7.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/tests/README.rst` & `ytmusicapi-1.7.3/tests/README.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/tests/auth/test_browser.py` & `ytmusicapi-1.7.3/tests/auth/test_browser.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/tests/auth/test_oauth.py` & `ytmusicapi-1.7.3/tests/auth/test_oauth.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/tests/conftest.py` & `ytmusicapi-1.7.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/tests/data/2024_03_get_album.json` & `ytmusicapi-1.7.3/tests/data/2024_03_get_album.json`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/tests/data/2024_03_get_playlist.json` & `ytmusicapi-1.7.3/tests/data/2024_03_get_playlist.json`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/tests/data/2024_03_get_playlist_public.json` & `ytmusicapi-1.7.3/tests/data/2024_03_get_playlist_public.json`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/tests/mixins/test_browsing.py` & `ytmusicapi-1.7.3/tests/mixins/test_browsing.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/tests/mixins/test_explore.py` & `ytmusicapi-1.7.3/tests/mixins/test_explore.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/tests/mixins/test_library.py` & `ytmusicapi-1.7.3/tests/mixins/test_library.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/tests/mixins/test_playlists.py` & `ytmusicapi-1.7.3/tests/mixins/test_playlists.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/tests/mixins/test_podcasts.py` & `ytmusicapi-1.7.3/tests/mixins/test_podcasts.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/tests/mixins/test_search.py` & `ytmusicapi-1.7.3/tests/mixins/test_search.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/tests/mixins/test_uploads.py` & `ytmusicapi-1.7.3/tests/mixins/test_uploads.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/tests/mixins/test_watch.py` & `ytmusicapi-1.7.3/tests/mixins/test_watch.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/tests/setup/setup_account.py` & `ytmusicapi-1.7.3/tests/setup/setup_account.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/tests/test.example.cfg` & `ytmusicapi-1.7.3/tests/test.example.cfg`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/auth/browser.py` & `ytmusicapi-1.7.3/ytmusicapi/auth/browser.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/auth/oauth/credentials.py` & `ytmusicapi-1.7.3/ytmusicapi/auth/oauth/credentials.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/auth/oauth/models.py` & `ytmusicapi-1.7.3/ytmusicapi/auth/oauth/models.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/auth/oauth/token.py` & `ytmusicapi-1.7.3/ytmusicapi/auth/oauth/token.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/auth/types.py` & `ytmusicapi-1.7.3/ytmusicapi/auth/types.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/constants.py` & `ytmusicapi-1.7.3/ytmusicapi/constants.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/continuations.py` & `ytmusicapi-1.7.3/ytmusicapi/continuations.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/helpers.py` & `ytmusicapi-1.7.3/ytmusicapi/helpers.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/locales/README.rst` & `ytmusicapi-1.7.3/ytmusicapi/locales/README.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/locales/ar/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.3/ytmusicapi/locales/ar/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/locales/ar/LC_MESSAGES/base.po` & `ytmusicapi-1.7.3/ytmusicapi/locales/ar/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/locales/base.pot` & `ytmusicapi-1.7.3/ytmusicapi/locales/base.pot`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/locales/de/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.3/ytmusicapi/locales/de/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/locales/de/LC_MESSAGES/base.po` & `ytmusicapi-1.7.3/ytmusicapi/locales/de/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/locales/en/LC_MESSAGES/base.po` & `ytmusicapi-1.7.3/ytmusicapi/locales/en/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/locales/es/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.3/ytmusicapi/locales/es/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/locales/es/LC_MESSAGES/base.po` & `ytmusicapi-1.7.3/ytmusicapi/locales/es/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/locales/fr/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.3/ytmusicapi/locales/fr/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/locales/fr/LC_MESSAGES/base.po` & `ytmusicapi-1.7.3/ytmusicapi/locales/fr/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/locales/hi/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.3/ytmusicapi/locales/hi/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/locales/hi/LC_MESSAGES/base.po` & `ytmusicapi-1.7.3/ytmusicapi/locales/hi/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/locales/it/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.3/ytmusicapi/locales/it/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/locales/it/LC_MESSAGES/base.po` & `ytmusicapi-1.7.3/ytmusicapi/locales/it/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/locales/ja/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.3/ytmusicapi/locales/ja/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/locales/ja/LC_MESSAGES/base.po` & `ytmusicapi-1.7.3/ytmusicapi/locales/ja/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/locales/ko/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.3/ytmusicapi/locales/ko/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/locales/ko/LC_MESSAGES/base.po` & `ytmusicapi-1.7.3/ytmusicapi/locales/ko/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/locales/nl/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.3/ytmusicapi/locales/nl/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/locales/nl/LC_MESSAGES/base.po` & `ytmusicapi-1.7.3/ytmusicapi/locales/nl/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/locales/pt/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.3/ytmusicapi/locales/pt/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/locales/pt/LC_MESSAGES/base.po` & `ytmusicapi-1.7.3/ytmusicapi/locales/pt/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/locales/ru/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.3/ytmusicapi/locales/ru/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/locales/ru/LC_MESSAGES/base.po` & `ytmusicapi-1.7.3/ytmusicapi/locales/ru/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/locales/tr/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.3/ytmusicapi/locales/tr/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/locales/tr/LC_MESSAGES/base.po` & `ytmusicapi-1.7.3/ytmusicapi/locales/tr/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/locales/ur/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.3/ytmusicapi/locales/ur/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/locales/ur/LC_MESSAGES/base.po` & `ytmusicapi-1.7.3/ytmusicapi/locales/ur/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.3/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.po` & `ytmusicapi-1.7.3/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.3/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.po` & `ytmusicapi-1.7.3/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/mixins/_protocol.py` & `ytmusicapi-1.7.3/ytmusicapi/mixins/_protocol.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/mixins/_utils.py` & `ytmusicapi-1.7.3/ytmusicapi/mixins/_utils.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/mixins/browsing.py` & `ytmusicapi-1.7.3/ytmusicapi/mixins/browsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 
             [
                 {
                     "title": "Your morning music",
                     "contents": [
                         { //album result
                             "title": "Sentiment",
-                            "year": "Said The Sky",
                             "browseId": "MPREb_QtqXtd2xZMR",
                             "thumbnails": [...]
                         },
                         { //playlist result
                             "title": "r/EDM top submissions 01/28/2022",
                             "playlistId": "PLz7-xrYmULdSLRZGk-6GKUtaBZcgQNwel",
                             "thumbnails": [...],
```

### Comparing `ytmusicapi-1.7.2/ytmusicapi/mixins/explore.py` & `ytmusicapi-1.7.3/ytmusicapi/mixins/explore.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/mixins/library.py` & `ytmusicapi-1.7.3/ytmusicapi/mixins/library.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/mixins/playlists.py` & `ytmusicapi-1.7.3/ytmusicapi/mixins/playlists.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/mixins/podcasts.py` & `ytmusicapi-1.7.3/ytmusicapi/mixins/podcasts.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/mixins/search.py` & `ytmusicapi-1.7.3/ytmusicapi/mixins/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,16 +79,17 @@
                   "add": null,
                   "remove": null
                 }
               },
               {
                 "category": "Albums",
                 "resultType": "album",
-                "browseId": "MPREb_9nqEki4ZDpp",
-                "title": "(What's The Story) Morning Glory? (Remastered)",
+                "browseId": "MPREb_IInSY5QXXrW",
+                "playlistId": "OLAK5uy_kunInnOpcKECWIBQGB0Qj6ZjquxDvfckg",
+                "title": "(What's The Story) Morning Glory?",
                 "type": "Album",
                 "artist": "Oasis",
                 "year": "1995",
                 "isExplicit": false
               },
               {
                 "category": "Community playlists",
```

### Comparing `ytmusicapi-1.7.2/ytmusicapi/mixins/uploads.py` & `ytmusicapi-1.7.3/ytmusicapi/mixins/uploads.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/mixins/watch.py` & `ytmusicapi-1.7.3/ytmusicapi/mixins/watch.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/navigation.py` & `ytmusicapi-1.7.3/ytmusicapi/navigation.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/parsers/_utils.py` & `ytmusicapi-1.7.3/ytmusicapi/parsers/_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from functools import wraps
 
 from ytmusicapi.navigation import *
 
 
 def parse_menu_playlists(data, result):
-    watch_menu = find_objects_by_key(nav(data, MENU_ITEMS), MNIR)
+    menu_items = nav(data, MENU_ITEMS, True)
+    if menu_items is None:
+        return
+    watch_menu = find_objects_by_key(menu_items, MNIR)
     for item in [_x[MNIR] for _x in watch_menu]:
         icon = nav(item, ICON_TYPE)
         if icon == "MUSIC_SHUFFLE":
             watch_key = "shuffleId"
         elif icon == "MIX":
             watch_key = "radioId"
         else:
```

### Comparing `ytmusicapi-1.7.2/ytmusicapi/parsers/albums.py` & `ytmusicapi-1.7.3/ytmusicapi/parsers/albums.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/parsers/browsing.py` & `ytmusicapi-1.7.3/ytmusicapi/parsers/browsing.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from .podcasts import parse_episode, parse_podcast
 from .songs import *
 
 
 def parse_mixed_content(rows):
     items = []
     for row in rows:
         if DESCRIPTION_SHELF[0] in row:
@@ -26,19 +27,22 @@
                             content = parse_song(data)
                     elif page_type == "MUSIC_PAGE_TYPE_ALBUM":
                         content = parse_album(data)
                     elif page_type == "MUSIC_PAGE_TYPE_ARTIST":
                         content = parse_related_artist(data)
                     elif page_type == "MUSIC_PAGE_TYPE_PLAYLIST":
                         content = parse_playlist(data)
-                else:
-                    data = nav(result, [MRLIR], True)
-                    if not data:
-                        continue
+                    elif page_type == "MUSIC_PAGE_TYPE_PODCAST_SHOW_DETAIL_PAGE":
+                        content = parse_podcast(data)
+                elif data := nav(result, [MRLIR], True):
                     content = parse_song_flat(data)
+                elif data := nav(result, [MMRIR], True):
+                    content = parse_episode(data)
+                else:
+                    continue
 
                 contents.append(content)
 
         items.append({"title": title, "contents": contents})
     return items
 
 
@@ -47,25 +51,29 @@
     for result in results:
         contents.append(parse_func(result[key]))
 
     return contents
 
 
 def parse_album(result):
-    return {
+    album = {
         "title": nav(result, TITLE_TEXT),
         "type": nav(result, SUBTITLE),
-        "year": nav(result, SUBTITLE2, True),
         "artists": [parse_id_name(x) for x in nav(result, ["subtitle", "runs"]) if "navigationEndpoint" in x],
         "browseId": nav(result, TITLE + NAVIGATION_BROWSE_ID),
         "audioPlaylistId": nav(result, THUMBNAIL_OVERLAY, True),
         "thumbnails": nav(result, THUMBNAIL_RENDERER),
         "isExplicit": nav(result, SUBTITLE_BADGE_LABEL, True) is not None,
     }
 
+    if (year := nav(result, SUBTITLE2, True)) and year.isnumeric():
+        album["year"] = year
+
+    return album
+
 
 def parse_single(result):
     return {
         "title": nav(result, TITLE_TEXT),
         "year": nav(result, SUBTITLE, True),
         "browseId": nav(result, TITLE + NAVIGATION_BROWSE_ID),
         "thumbnails": nav(result, THUMBNAIL_RENDERER),
```

### Comparing `ytmusicapi-1.7.2/ytmusicapi/parsers/explore.py` & `ytmusicapi-1.7.3/ytmusicapi/parsers/explore.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/parsers/i18n.py` & `ytmusicapi-1.7.3/ytmusicapi/parsers/i18n.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/parsers/library.py` & `ytmusicapi-1.7.3/ytmusicapi/parsers/library.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/parsers/playlists.py` & `ytmusicapi-1.7.3/ytmusicapi/parsers/playlists.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/parsers/podcasts.py` & `ytmusicapi-1.7.3/ytmusicapi/parsers/podcasts.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,12 +125,12 @@
     }
 
 
 def parse_podcast(data):
     """Parses a single podcast under "Podcasts" on a channel page"""
     return {
         "title": nav(data, TITLE_TEXT),
-        "channel": parse_id_name(nav(data, [*SUBTITLE_RUNS, 0])),
+        "channel": parse_id_name(nav(data, [*SUBTITLE_RUNS, 0], True)),
         "browseId": nav(data, TITLE + NAVIGATION_BROWSE_ID),
         "podcastId": nav(data, THUMBNAIL_OVERLAY, True),
         "thumbnails": nav(data, THUMBNAIL_RENDERER),
     }
```

### Comparing `ytmusicapi-1.7.2/ytmusicapi/parsers/search.py` & `ytmusicapi-1.7.3/ytmusicapi/parsers/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from ..helpers import to_int
 from ._utils import *
 from .songs import *
 
 UNIQUE_RESULT_TYPES = ["artist", "playlist", "song", "video", "station", "profile", "podcast", "episode"]
 ALL_RESULT_TYPES = ["album", *UNIQUE_RESULT_TYPES]
 
 
@@ -42,14 +43,15 @@
         search_result["title"] = nav(data, TITLE_TEXT)
         runs = nav(data, ["subtitle", "runs"])
         song_info = parse_song_runs(runs[2:])
         search_result.update(song_info)
 
     if result_type in ["album"]:
         search_result["browseId"] = nav(data, TITLE + NAVIGATION_BROWSE_ID, True)
+        search_result["playlistId"] = nav(data, ["buttons", 0, "buttonRenderer", "command", *WATCH_PID], True)
 
     if result_type in ["playlist"]:
         search_result["playlistId"] = nav(data, MENU_PLAYLIST_ID)
         search_result["title"] = nav(data, TITLE_TEXT)
         search_result["author"] = parse_song_artists_runs(nav(data, ["subtitle", "runs"])[2:])
 
     search_result["thumbnails"] = nav(data, THUMBNAILS, True)
@@ -93,14 +95,16 @@
     elif result_type == "album":
         search_result["type"] = get_item_text(data, 1)
 
     elif result_type == "playlist":
         flex_item = get_flex_column_item(data, 1)["text"]["runs"]
         has_author = len(flex_item) == default_offset + 3
         search_result["itemCount"] = get_item_text(data, 1, default_offset + has_author * 2).split(" ")[0]
+        if search_result["itemCount"] and search_result["itemCount"].isnumeric():
+            search_result["itemCount"] = to_int(search_result["itemCount"])
         search_result["author"] = None if not has_author else get_item_text(data, 1, default_offset)
 
     elif result_type == "station":
         search_result["videoId"] = nav(data, NAVIGATION_VIDEO_ID)
         search_result["playlistId"] = nav(data, NAVIGATION_PLAYLIST_ID)
 
     elif result_type == "profile":
@@ -155,14 +159,21 @@
 
     if result_type in ["artist", "album", "playlist", "profile", "podcast"]:
         search_result["browseId"] = nav(data, NAVIGATION_BROWSE_ID, True)
 
     if result_type in ["song", "album"]:
         search_result["isExplicit"] = nav(data, BADGE_LABEL, True) is not None
 
+    if result_type in ["album"]:
+        search_result["playlistId"] = nav(
+            data,
+            [*PLAY_BUTTON, "playNavigationEndpoint", "watchEndpoint", "playlistId"],
+            True,
+        )
+
     if result_type in ["episode"]:
         flex_item = get_flex_column_item(data, 1)
         has_date = int(len(nav(flex_item, TEXT_RUNS)) > 1)
         search_result["live"] = bool(nav(data, ["badges", 0, "liveBadgeRenderer"], True))
         if has_date:
             search_result["date"] = nav(flex_item, TEXT_RUN_TEXT)
```

### Comparing `ytmusicapi-1.7.2/ytmusicapi/parsers/songs.py` & `ytmusicapi-1.7.3/ytmusicapi/parsers/songs.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/parsers/uploads.py` & `ytmusicapi-1.7.3/ytmusicapi/parsers/uploads.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/parsers/watch.py` & `ytmusicapi-1.7.3/ytmusicapi/parsers/watch.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/setup.py` & `ytmusicapi-1.7.3/ytmusicapi/setup.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi/ytmusic.py` & `ytmusicapi-1.7.3/ytmusicapi/ytmusic.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.2/ytmusicapi.egg-info/PKG-INFO` & `ytmusicapi-1.7.3/ytmusicapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytmusicapi
-Version: 1.7.2
+Version: 1.7.3
 Summary: Unofficial API for YouTube Music
 Author-email: sigma67 <ytmusicapi@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 sigma67
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ytmusicapi-1.7.2/ytmusicapi.egg-info/SOURCES.txt` & `ytmusicapi-1.7.3/ytmusicapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

