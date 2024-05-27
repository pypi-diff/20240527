# Comparing `tmp/vlttng-0.9.3.tar.gz` & `tmp/vlttng-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vlttng-0.9.3.tar", last modified: Mon Sep 24 18:29:37 2018, max compression
+gzip compressed data, was "dist/vlttng-0.9.4.tar", last modified: Sat Mar 23 22:13:36 2019, max compression
```

## Comparing `vlttng-0.9.3.tar` & `vlttng-0.9.4.tar`

### file list

```diff
@@ -1,310 +1,340 @@
-drwxr-xr-x   0 eepp      (1000) eepp      (1000)        0 2018-09-24 18:29:37.000000 vlttng-0.9.3/
-drwxr-xr-x   0 eepp      (1000) eepp      (1000)        0 2018-09-24 18:29:37.000000 vlttng-0.9.3/vlttng/
--rw-r--r--   0 eepp      (1000) eepp      (1000)     1189 2018-09-24 18:28:38.000000 vlttng-0.9.3/vlttng/__init__.py
--rw-r--r--   0 eepp      (1000) eepp      (1000)     2557 2016-10-29 23:04:11.000000 vlttng-0.9.3/vlttng/build_template.py
--rw-r--r--   0 eepp      (1000) eepp      (1000)     2563 2016-10-29 23:04:11.000000 vlttng-0.9.3/vlttng/conf_template.py
--rw-r--r--   0 eepp      (1000) eepp      (1000)    29706 2018-09-24 18:20:59.000000 vlttng-0.9.3/vlttng/venv.py
--rw-r--r--   0 eepp      (1000) eepp      (1000)     6977 2018-05-10 18:54:47.000000 vlttng-0.9.3/vlttng/vlttng_cli.py
--rw-r--r--   0 eepp      (1000) eepp      (1000)     2790 2016-10-29 23:04:11.000000 vlttng-0.9.3/vlttng/update_template.py
--rw-r--r--   0 eepp      (1000) eepp      (1000)     2565 2016-10-29 23:04:11.000000 vlttng-0.9.3/vlttng/install_template.py
-drwxr-xr-x   0 eepp      (1000) eepp      (1000)        0 2018-09-24 18:29:37.000000 vlttng-0.9.3/vlttng/profiles/
--rw-r--r--   0 eepp      (1000) eepp      (1000)       97 2016-05-19 19:00:58.000000 vlttng-0.9.3/vlttng/profiles/urcu-stable-0.8.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.6.3.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2016-11-01 02:59:55.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-stable-2.6.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      104 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-stable-2.6.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      104 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-stable-2.7.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      107 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.10.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.6.4.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2018-05-10 18:41:17.000000 vlttng-0.9.3/vlttng/profiles/glib-2.54.2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-10-18 18:03:34.000000 vlttng-0.9.3/vlttng/profiles/glib-2.50.1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      110 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.6.0-rc2.yml
--rw-rw-rw-   0 eepp      (1000) eepp      (1000)      148 2016-05-20 00:57:53.000000 vlttng-0.9.3/vlttng/profiles/libxml2-2.9.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      148 2018-05-10 18:42:44.000000 vlttng-0.9.3/vlttng/profiles/libxml2-2.9.7.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      161 2017-10-19 18:27:25.000000 vlttng-0.9.3/vlttng/profiles/tracecompass-linux-x86-64-1.2.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.6.3.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.8.7.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      107 2016-08-10 15:54:40.000000 vlttng-0.9.3/vlttng/profiles/lttng-analyses-0.5.3.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.6.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       95 2018-09-12 01:20:19.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.10.2.yml
--rw-rw-rw-   0 eepp      (1000) eepp      (1000)      107 2016-05-19 19:54:58.000000 vlttng-0.9.3/vlttng/profiles/lttng-analyses-0.4.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-10-18 18:03:34.000000 vlttng-0.9.3/vlttng/profiles/glib-2.48.2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      110 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.8.0-rc2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      111 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.10.0-rc1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.9.5.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.6.2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      161 2018-05-10 18:47:11.000000 vlttng-0.9.3/vlttng/profiles/tracecompass-linux-x86-64-3.3.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.6.1.yml
--rw-rw-rw-   0 eepp      (1000) eepp      (1000)       71 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-master.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      175 2017-10-19 18:27:25.000000 vlttng-0.9.3/vlttng/profiles/tracecompass-macos-x86-64-1.1.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.6.5.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.8.4.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2018-05-10 18:41:57.000000 vlttng-0.9.3/vlttng/profiles/glib-2.55.1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       72 2016-05-19 19:00:58.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-no-lttng-consumerd.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.7.4.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      161 2017-10-19 18:27:25.000000 vlttng-0.9.3/vlttng/profiles/tracecompass-linux-x86-64-1.2.1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.8.6.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.9.5.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2018-05-10 18:41:21.000000 vlttng-0.9.3/vlttng/profiles/glib-2.54.3.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       98 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.8.0-rc2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.6.4.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.7.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       49 2017-01-09 20:40:06.000000 vlttng-0.9.3/vlttng/profiles/debug-flags.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      280 2016-05-20 00:10:57.000000 vlttng-0.9.3/vlttng/profiles/glib-2.29.92.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.6.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.6.6.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      104 2017-10-19 18:45:54.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.6.0-rc1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      107 2017-10-19 18:27:25.000000 vlttng-0.9.3/vlttng/profiles/lttng-analyses-0.6.1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      205 2016-11-01 03:07:49.000000 vlttng-0.9.3/vlttng/profiles/lttng-master.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       68 2016-05-19 19:00:58.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-no-python.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      161 2018-05-10 18:45:49.000000 vlttng-0.9.3/vlttng/profiles/tracecompass-linux-x86-64-3.2.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:10:57.000000 vlttng-0.9.3/vlttng/profiles/glib-2.45.8.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.9.1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      280 2016-05-20 00:10:57.000000 vlttng-0.9.3/vlttng/profiles/glib-2.47.92.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       95 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.10.0.yml
--rw-rw-rw-   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:04:35.000000 vlttng-0.9.3/vlttng/profiles/glib-2.48.1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       97 2016-05-19 19:00:58.000000 vlttng-0.9.3/vlttng/profiles/urcu-stable-0.7.yml
--rw-rw-rw-   0 eepp      (1000) eepp      (1000)      148 2016-05-20 00:58:04.000000 vlttng-0.9.3/vlttng/profiles/libxml2-2.8.0.yml
--rw-rw-rw-   0 eepp      (1000) eepp      (1000)       79 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-master.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       98 2017-10-19 18:27:25.000000 vlttng-0.9.3/vlttng/profiles/urcu-stable-0.10.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       71 2016-05-19 19:00:58.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-no-lttng-sessiond.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.6.7.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      104 2017-10-19 18:45:54.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.6.0-rc2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:10:57.000000 vlttng-0.9.3/vlttng/profiles/glib-2.34.3.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      280 2016-11-01 03:07:56.000000 vlttng-0.9.3/vlttng/profiles/lttng-stable-2.6.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      107 2018-05-10 18:40:16.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.10.3.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.7.3.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2018-05-10 18:42:18.000000 vlttng-0.9.3/vlttng/profiles/glib-2.56.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      164 2017-10-19 18:27:25.000000 vlttng-0.9.3/vlttng/profiles/tracecompass-macos-x86-64-2.2.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      104 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.9.0-rc1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      110 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.9.0-rc2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:10:57.000000 vlttng-0.9.3/vlttng/profiles/glib-2.41.5.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       96 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-stable-2.7.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.7.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      105 2018-09-12 01:16:01.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-stable-2.11.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       62 2016-05-19 19:00:58.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-no-lttng.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      148 2016-11-17 21:18:07.000000 vlttng-0.9.3/vlttng/profiles/libxml2-2.9.4.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.7.6.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.9.2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.7.2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       95 2018-05-10 18:39:05.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.10.1.yml
--rw-rw-rw-   0 eepp      (1000) eepp      (1000)      112 2016-11-01 03:08:07.000000 vlttng-0.9.3/vlttng/profiles/tracecompass-master.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.8.1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      283 2018-09-12 01:17:02.000000 vlttng-0.9.3/vlttng/profiles/lttng-stable-2.11.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:10:57.000000 vlttng-0.9.3/vlttng/profiles/glib-2.36.4.yml
--rw-rw-rw-   0 eepp      (1000) eepp      (1000)      161 2016-05-19 20:38:38.000000 vlttng-0.9.3/vlttng/profiles/tracecompass-1.2.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      110 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.9.0-rc1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      105 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.10.0-rc1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       98 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.7.0-rc2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.8.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2017-10-19 18:27:25.000000 vlttng-0.9.3/vlttng/profiles/glib-2.53.2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       98 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.8.0-rc1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      283 2017-10-19 18:27:25.000000 vlttng-0.9.3/vlttng/profiles/lttng-stable-2.10.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.9.6.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       66 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-log4j-agent.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.9.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.8.2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      105 2018-09-12 01:16:01.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.11.0-rc1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       98 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.6.0-rc2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      164 2017-10-19 18:27:25.000000 vlttng-0.9.3/vlttng/profiles/tracecompass-macos-x86-64-2.3.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      164 2017-10-19 18:27:25.000000 vlttng-0.9.3/vlttng/profiles/tracecompass-macos-x86-64-1.2.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       99 2018-09-12 01:16:01.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.11.0-rc1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      107 2018-09-12 01:20:52.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.10.7.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      148 2017-10-19 19:07:38.000000 vlttng-0.9.3/vlttng/profiles/libxml2-2.9.5.yml
--rw-rw-rw-   0 eepp      (1000) eepp      (1000)      107 2016-05-19 19:54:59.000000 vlttng-0.9.3/vlttng/profiles/lttng-analyses-0.4.1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      156 2017-10-19 18:27:25.000000 vlttng-0.9.3/vlttng/profiles/elfutils-0.167.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.9.4.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.8.3.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       99 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.10.0-rc1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      280 2016-05-20 00:10:57.000000 vlttng-0.9.3/vlttng/profiles/glib-2.39.92.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.9.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      107 2017-10-19 18:27:25.000000 vlttng-0.9.3/vlttng/profiles/lttng-analyses-0.6.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       99 2016-10-18 18:03:34.000000 vlttng-0.9.3/vlttng/profiles/babeltrace-stable-1.4.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       67 2016-05-19 19:00:58.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-python.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      101 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.10.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       65 2017-10-19 18:27:25.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-embedded-help.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       98 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.6.0-rc1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      107 2016-06-01 00:29:20.000000 vlttng-0.9.3/vlttng/profiles/lttng-analyses-0.5.1.yml
--rw-rw-rw-   0 eepp      (1000) eepp      (1000)      107 2016-05-19 19:54:56.000000 vlttng-0.9.3/vlttng/profiles/lttng-analyses-0.3.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2017-10-19 18:27:25.000000 vlttng-0.9.3/vlttng/profiles/glib-2.51.5.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.9.2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.6.6.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.6.3.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       99 2016-10-18 18:03:34.000000 vlttng-0.9.3/vlttng/profiles/babeltrace-stable-1.2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      280 2016-05-20 00:12:24.000000 vlttng-0.9.3/vlttng/profiles/glib-2.27.93.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.8.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:12:16.000000 vlttng-0.9.3/vlttng/profiles/glib-2.23.6.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.8.6.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:10:57.000000 vlttng-0.9.3/vlttng/profiles/glib-2.32.4.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.7.6.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       96 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-stable-2.9.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      164 2017-10-19 19:05:47.000000 vlttng-0.9.3/vlttng/profiles/tracecompass-macos-x86-64-3.0.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       72 2016-11-01 03:08:09.000000 vlttng-0.9.3/vlttng/profiles/urcu-master.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      101 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.10.1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      104 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.6.0-rc4.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       75 2016-11-01 04:50:01.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-master.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       99 2017-01-09 20:41:55.000000 vlttng-0.9.3/vlttng/profiles/babeltrace-stable-1.5.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      148 2018-05-10 18:42:47.000000 vlttng-0.9.3/vlttng/profiles/libxml2-2.9.8.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      107 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.10.2.yml
--rw-rw-rw-   0 eepp      (1000) eepp      (1000)      148 2016-05-20 00:54:05.000000 vlttng-0.9.3/vlttng/profiles/libxml2-2.9.3.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       64 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-jul-agent.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      280 2016-05-20 00:10:57.000000 vlttng-0.9.3/vlttng/profiles/glib-2.37.93.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:10:57.000000 vlttng-0.9.3/vlttng/profiles/glib-2.38.2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.6.1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.6.2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       66 2016-05-19 19:00:58.000000 vlttng-0.9.3/vlttng/profiles/babeltrace-python.yml
--rw-rw-rw-   0 eepp      (1000) eepp      (1000)      107 2016-05-19 19:55:01.000000 vlttng-0.9.3/vlttng/profiles/lttng-analyses-0.4.2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      101 2018-05-10 18:39:39.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.10.3.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2017-10-19 18:28:37.000000 vlttng-0.9.3/vlttng/profiles/glib-2.54.1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      104 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.7.0-rc2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.9.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      172 2017-10-19 18:27:25.000000 vlttng-0.9.3/vlttng/profiles/tracecompass-linux-x86-64-1.1.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-10-18 18:03:34.000000 vlttng-0.9.3/vlttng/profiles/glib-2.49.7.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.9.3.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       99 2016-10-18 18:03:34.000000 vlttng-0.9.3/vlttng/profiles/babeltrace-stable-1.3.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      104 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-stable-2.9.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      148 2017-10-19 19:07:43.000000 vlttng-0.9.3/vlttng/profiles/libxml2-2.9.6.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2017-10-19 18:27:25.000000 vlttng-0.9.3/vlttng/profiles/glib-2.52.2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.9.3.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      104 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.7.0-rc1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.7.1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.8.5.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.7.4.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      107 2018-05-10 18:40:26.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.10.6.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.7.1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:10:57.000000 vlttng-0.9.3/vlttng/profiles/glib-2.40.2.yml
--rw-rw-rw-   0 eepp      (1000) eepp      (1000)      107 2016-05-19 19:54:50.000000 vlttng-0.9.3/vlttng/profiles/lttng-analyses-master.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:12:26.000000 vlttng-0.9.3/vlttng/profiles/glib-2.28.8.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:12:18.000000 vlttng-0.9.3/vlttng/profiles/glib-2.24.2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      164 2017-10-19 18:27:25.000000 vlttng-0.9.3/vlttng/profiles/tracecompass-macos-x86-64-2.1.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:10:57.000000 vlttng-0.9.3/vlttng/profiles/glib-2.35.9.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       62 2016-05-19 19:00:58.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-no-man-pages.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.7.2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      280 2016-11-01 02:59:55.000000 vlttng-0.9.3/vlttng/profiles/lttng-stable-2.8.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      107 2018-05-10 18:40:20.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.10.4.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2016-11-01 02:59:55.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-stable-2.8.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      104 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-stable-2.8.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      280 2016-11-01 02:59:55.000000 vlttng-0.9.3/vlttng/profiles/lttng-stable-2.7.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      104 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.6.0-rc3.yml
--rw-rw-rw-   0 eepp      (1000) eepp      (1000)       59 2016-11-01 03:03:13.000000 vlttng-0.9.3/vlttng/profiles/babeltrace-debug-info.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:10:57.000000 vlttng-0.9.3/vlttng/profiles/glib-2.42.2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      156 2017-10-19 18:27:25.000000 vlttng-0.9.3/vlttng/profiles/elfutils-0.166.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      164 2017-10-19 18:27:25.000000 vlttng-0.9.3/vlttng/profiles/tracecompass-macos-x86-64-2.0.0.yml
--rw-rw-rw-   0 eepp      (1000) eepp      (1000)      235 2016-11-01 03:07:38.000000 vlttng-0.9.3/vlttng/profiles/glib-master.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       97 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-stable-2.10.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      164 2018-05-10 18:47:49.000000 vlttng-0.9.3/vlttng/profiles/tracecompass-macos-x86-64-3.2.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.6.2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      161 2017-10-19 18:27:25.000000 vlttng-0.9.3/vlttng/profiles/tracecompass-linux-x86-64-2.2.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      164 2017-10-19 18:27:25.000000 vlttng-0.9.3/vlttng/profiles/tracecompass-macos-x86-64-2.0.1.yml
--rw-rw-rw-   0 eepp      (1000) eepp      (1000)      172 2016-05-19 20:38:33.000000 vlttng-0.9.3/vlttng/profiles/tracecompass-1.1.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      110 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.8.0-rc1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      107 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.10.1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      161 2017-10-19 18:27:25.000000 vlttng-0.9.3/vlttng/profiles/tracecompass-linux-x86-64-2.0.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2018-05-10 18:42:20.000000 vlttng-0.9.3/vlttng/profiles/glib-2.56.1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      101 2018-09-12 01:16:01.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-stable-2.11.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      164 2017-10-19 18:27:25.000000 vlttng-0.9.3/vlttng/profiles/tracecompass-macos-x86-64-1.2.1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.8.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      104 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.8.0-rc1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2018-05-10 18:41:53.000000 vlttng-0.9.3/vlttng/profiles/glib-2.55.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      197 2016-11-01 04:50:01.000000 vlttng-0.9.3/vlttng/profiles/libxml2-master.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       98 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.6.0-rc3.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      107 2016-08-10 15:54:40.000000 vlttng-0.9.3/vlttng/profiles/lttng-analyses-0.5.4.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       74 2016-11-01 03:07:31.000000 vlttng-0.9.3/vlttng/profiles/babeltrace-master.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      119 2018-05-14 15:57:57.000000 vlttng-0.9.3/vlttng/profiles/lttng-scope-0.3.0.yml
--rw-rw-rw-   0 eepp      (1000) eepp      (1000)      161 2016-05-19 20:38:41.000000 vlttng-0.9.3/vlttng/profiles/tracecompass-1.2.1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.7.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2018-05-10 18:41:59.000000 vlttng-0.9.3/vlttng/profiles/glib-2.55.2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.7.3.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      107 2016-08-10 15:54:40.000000 vlttng-0.9.3/vlttng/profiles/lttng-analyses-0.5.2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      164 2018-05-10 18:48:14.000000 vlttng-0.9.3/vlttng/profiles/tracecompass-macos-x86-64-3.3.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.7.3.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.7.5.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.9.1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:12:14.000000 vlttng-0.9.3/vlttng/profiles/glib-2.22.5.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.9.4.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       97 2018-09-12 01:16:01.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-stable-2.11.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       60 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-no-man-pages.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      101 2018-05-10 18:39:46.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.10.5.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2016-11-01 02:59:55.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-stable-2.7.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      110 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.6.0-rc1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       96 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-stable-2.6.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.8.1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.7.5.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.9.1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       99 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.10.0-rc2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.8.7.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      161 2017-10-19 18:27:25.000000 vlttng-0.9.3/vlttng/profiles/tracecompass-linux-x86-64-2.1.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       69 2016-05-19 19:00:58.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-no-lttng-relayd.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      280 2016-05-20 00:10:57.000000 vlttng-0.9.3/vlttng/profiles/glib-2.31.22.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       98 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.9.0-rc1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      111 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.10.0-rc2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.6.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-01-09 20:41:28.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-stable-2.9.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      280 2016-05-20 00:12:20.000000 vlttng-0.9.3/vlttng/profiles/glib-2.25.17.yml
--rw-rw-rw-   0 eepp      (1000) eepp      (1000)      161 2016-07-13 19:11:13.000000 vlttng-0.9.3/vlttng/profiles/tracecompass-2.0.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:12:22.000000 vlttng-0.9.3/vlttng/profiles/glib-2.26.1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      161 2017-10-19 19:06:35.000000 vlttng-0.9.3/vlttng/profiles/tracecompass-linux-x86-64-3.1.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       96 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-stable-2.8.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      280 2016-05-20 00:10:57.000000 vlttng-0.9.3/vlttng/profiles/glib-2.33.14.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.7.5.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      280 2017-01-09 20:41:28.000000 vlttng-0.9.3/vlttng/profiles/lttng-stable-2.9.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      164 2017-10-19 19:06:53.000000 vlttng-0.9.3/vlttng/profiles/tracecompass-macos-x86-64-3.1.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.7.1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      101 2018-05-10 18:39:42.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.10.4.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.8.4.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.7.4.yml
--rw-rw-rw-   0 eepp      (1000) eepp      (1000)      148 2016-05-20 00:57:35.000000 vlttng-0.9.3/vlttng/profiles/libxml2-2.9.2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      280 2016-05-20 00:10:57.000000 vlttng-0.9.3/vlttng/profiles/glib-2.43.92.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.8.3.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       68 2016-05-19 19:00:58.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-no-lttng-crash.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       98 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.7.0-rc1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      105 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-stable-2.10.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:10:57.000000 vlttng-0.9.3/vlttng/profiles/glib-2.30.3.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       46 2016-11-01 02:59:55.000000 vlttng-0.9.3/vlttng/profiles/use-ccache-gcc.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.8.2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      105 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.10.0-rc2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)     1479 2018-05-14 16:19:26.000000 vlttng-0.9.3/vlttng/profiles/all-master.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      101 2017-10-19 18:27:25.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-stable-2.10.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      156 2017-10-19 19:08:16.000000 vlttng-0.9.3/vlttng/profiles/elfutils-0.170.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.8.1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      161 2017-10-19 19:05:10.000000 vlttng-0.9.3/vlttng/profiles/tracecompass-linux-x86-64-3.0.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.6.1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      101 2018-05-10 18:39:35.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.10.2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      156 2017-10-19 18:27:25.000000 vlttng-0.9.3/vlttng/profiles/elfutils-0.169.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      110 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.7.0-rc1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      161 2017-10-19 18:27:25.000000 vlttng-0.9.3/vlttng/profiles/tracecompass-linux-x86-64-2.3.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:10:57.000000 vlttng-0.9.3/vlttng/profiles/glib-2.44.1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      156 2017-10-19 18:27:25.000000 vlttng-0.9.3/vlttng/profiles/elfutils-0.168.yml
--rw-rw-rw-   0 eepp      (1000) eepp      (1000)      148 2016-05-20 00:57:46.000000 vlttng-0.9.3/vlttng/profiles/libxml2-2.9.1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.8.4.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-2.7.2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       97 2016-05-19 19:00:58.000000 vlttng-0.9.3/vlttng/profiles/urcu-stable-0.9.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      111 2018-09-12 01:16:01.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.11.0-rc1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      107 2018-05-10 18:40:23.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.10.5.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.6.5.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.7.7.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:10:57.000000 vlttng-0.9.3/vlttng/profiles/glib-2.46.2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.8.5.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       80 2018-05-10 20:44:09.000000 vlttng-0.9.3/vlttng/profiles/lttng-scope-master.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.8.2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.8.3.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      142 2016-11-01 02:59:55.000000 vlttng-0.9.3/vlttng/profiles/popt-1.16.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)       62 2017-10-19 18:59:07.000000 vlttng-0.9.3/vlttng/profiles/lttng-ust-python-agent.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      107 2016-06-01 00:29:20.000000 vlttng-0.9.3/vlttng/profiles/lttng-analyses-0.5.0.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      110 2017-10-19 18:59:27.000000 vlttng-0.9.3/vlttng/profiles/lttng-modules-2.7.0-rc2.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.3/vlttng/profiles/lttng-tools-2.8.8.yml
--rw-rw-rw-   0 eepp      (1000) eepp      (1000)      107 2016-05-19 19:55:02.000000 vlttng-0.9.3/vlttng/profiles/lttng-analyses-0.4.3.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)      161 2017-10-19 18:27:25.000000 vlttng-0.9.3/vlttng/profiles/tracecompass-linux-x86-64-2.0.1.yml
--rw-r--r--   0 eepp      (1000) eepp      (1000)     6895 2018-05-10 20:35:58.000000 vlttng-0.9.3/vlttng/activate_template.py
--rw-r--r--   0 eepp      (1000) eepp      (1000)    18345 2018-05-10 21:09:57.000000 vlttng-0.9.3/vlttng/vlttng_quick_cli.py
--rw-r--r--   0 eepp      (1000) eepp      (1000)     8333 2018-05-10 20:42:40.000000 vlttng-0.9.3/vlttng/profile.py
--rw-r--r--   0 eepp      (1000) eepp      (1000)     1367 2016-05-19 19:00:58.000000 vlttng-0.9.3/vlttng/utils.py
--rwxr-xr-x   0 eepp      (1000) eepp      (1000)     2402 2016-10-29 22:54:05.000000 vlttng-0.9.3/setup.py
--rw-r--r--   0 eepp      (1000) eepp      (1000)      686 2018-09-24 18:29:37.000000 vlttng-0.9.3/PKG-INFO
--rw-r--r--   0 eepp      (1000) eepp      (1000)       38 2018-09-24 18:29:37.000000 vlttng-0.9.3/setup.cfg
-drwxr-xr-x   0 eepp      (1000) eepp      (1000)        0 2018-09-24 18:29:37.000000 vlttng-0.9.3/vlttng.egg-info/
--rw-r--r--   0 eepp      (1000) eepp      (1000)       93 2018-09-24 18:29:37.000000 vlttng-0.9.3/vlttng.egg-info/entry_points.txt
--rw-r--r--   0 eepp      (1000) eepp      (1000)       28 2018-09-24 18:29:37.000000 vlttng-0.9.3/vlttng.egg-info/requires.txt
--rw-r--r--   0 eepp      (1000) eepp      (1000)        1 2018-09-24 18:29:37.000000 vlttng-0.9.3/vlttng.egg-info/dependency_links.txt
--rw-r--r--   0 eepp      (1000) eepp      (1000)        7 2018-09-24 18:29:37.000000 vlttng-0.9.3/vlttng.egg-info/top_level.txt
--rw-r--r--   0 eepp      (1000) eepp      (1000)    11726 2018-09-24 18:29:37.000000 vlttng-0.9.3/vlttng.egg-info/SOURCES.txt
--rw-r--r--   0 eepp      (1000) eepp      (1000)      686 2018-09-24 18:29:37.000000 vlttng-0.9.3/vlttng.egg-info/PKG-INFO
+drwxr-xr-x   0 eepp      (1000) eepp      (1000)        0 2019-03-23 22:13:36.000000 vlttng-0.9.4/
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      686 2019-03-23 22:13:36.000000 vlttng-0.9.4/PKG-INFO
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       38 2019-03-23 22:13:36.000000 vlttng-0.9.4/setup.cfg
+-rwxr-xr-x   0 eepp      (1000) eepp      (1000)     2402 2016-10-29 22:54:05.000000 vlttng-0.9.4/setup.py
+drwxr-xr-x   0 eepp      (1000) eepp      (1000)        0 2019-03-23 22:13:36.000000 vlttng-0.9.4/vlttng/
+-rw-r--r--   0 eepp      (1000) eepp      (1000)     1189 2019-03-23 20:35:37.000000 vlttng-0.9.4/vlttng/__init__.py
+-rw-r--r--   0 eepp      (1000) eepp      (1000)     6895 2018-05-10 20:35:58.000000 vlttng-0.9.4/vlttng/activate_template.py
+-rw-r--r--   0 eepp      (1000) eepp      (1000)     2557 2016-10-29 23:04:11.000000 vlttng-0.9.4/vlttng/build_template.py
+-rw-r--r--   0 eepp      (1000) eepp      (1000)     2563 2016-10-29 23:04:11.000000 vlttng-0.9.4/vlttng/conf_template.py
+-rw-r--r--   0 eepp      (1000) eepp      (1000)     2565 2016-10-29 23:04:11.000000 vlttng-0.9.4/vlttng/install_template.py
+-rw-r--r--   0 eepp      (1000) eepp      (1000)     8333 2018-05-10 20:42:40.000000 vlttng-0.9.4/vlttng/profile.py
+drwxr-xr-x   0 eepp      (1000) eepp      (1000)        0 2019-03-23 22:13:36.000000 vlttng-0.9.4/vlttng/profiles/
+-rw-r--r--   0 eepp      (1000) eepp      (1000)     1479 2018-05-14 16:19:26.000000 vlttng-0.9.4/vlttng/profiles/all-master.yml
+-rw-rw-rw-   0 eepp      (1000) eepp      (1000)       59 2016-11-01 03:03:13.000000 vlttng-0.9.4/vlttng/profiles/babeltrace-debug-info.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       74 2016-11-01 03:07:31.000000 vlttng-0.9.4/vlttng/profiles/babeltrace-master.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       66 2016-05-19 19:00:58.000000 vlttng-0.9.4/vlttng/profiles/babeltrace-python.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       99 2016-10-18 18:03:34.000000 vlttng-0.9.4/vlttng/profiles/babeltrace-stable-1.2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       99 2016-10-18 18:03:34.000000 vlttng-0.9.4/vlttng/profiles/babeltrace-stable-1.3.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       99 2016-10-18 18:03:34.000000 vlttng-0.9.4/vlttng/profiles/babeltrace-stable-1.4.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       99 2017-01-09 20:41:55.000000 vlttng-0.9.4/vlttng/profiles/babeltrace-stable-1.5.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       49 2017-01-09 20:40:06.000000 vlttng-0.9.4/vlttng/profiles/debug-flags.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      156 2017-10-19 18:27:25.000000 vlttng-0.9.4/vlttng/profiles/elfutils-0.166.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      156 2017-10-19 18:27:25.000000 vlttng-0.9.4/vlttng/profiles/elfutils-0.167.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      156 2017-10-19 18:27:25.000000 vlttng-0.9.4/vlttng/profiles/elfutils-0.168.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      156 2017-10-19 18:27:25.000000 vlttng-0.9.4/vlttng/profiles/elfutils-0.169.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      156 2017-10-19 19:08:16.000000 vlttng-0.9.4/vlttng/profiles/elfutils-0.170.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      156 2019-03-23 20:22:03.000000 vlttng-0.9.4/vlttng/profiles/elfutils-0.171.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      156 2019-03-23 20:22:15.000000 vlttng-0.9.4/vlttng/profiles/elfutils-0.172.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      156 2019-03-23 20:22:19.000000 vlttng-0.9.4/vlttng/profiles/elfutils-0.173.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      156 2019-03-23 20:22:24.000000 vlttng-0.9.4/vlttng/profiles/elfutils-0.174.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      156 2019-03-23 20:22:30.000000 vlttng-0.9.4/vlttng/profiles/elfutils-0.175.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      156 2019-03-23 20:22:38.000000 vlttng-0.9.4/vlttng/profiles/elfutils-0.176.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:12:14.000000 vlttng-0.9.4/vlttng/profiles/glib-2.22.5.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:12:16.000000 vlttng-0.9.4/vlttng/profiles/glib-2.23.6.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:12:18.000000 vlttng-0.9.4/vlttng/profiles/glib-2.24.2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      280 2016-05-20 00:12:20.000000 vlttng-0.9.4/vlttng/profiles/glib-2.25.17.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:12:22.000000 vlttng-0.9.4/vlttng/profiles/glib-2.26.1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      280 2016-05-20 00:12:24.000000 vlttng-0.9.4/vlttng/profiles/glib-2.27.93.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:12:26.000000 vlttng-0.9.4/vlttng/profiles/glib-2.28.8.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      280 2016-05-20 00:10:57.000000 vlttng-0.9.4/vlttng/profiles/glib-2.29.92.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:10:57.000000 vlttng-0.9.4/vlttng/profiles/glib-2.30.3.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      280 2016-05-20 00:10:57.000000 vlttng-0.9.4/vlttng/profiles/glib-2.31.22.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:10:57.000000 vlttng-0.9.4/vlttng/profiles/glib-2.32.4.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      280 2016-05-20 00:10:57.000000 vlttng-0.9.4/vlttng/profiles/glib-2.33.14.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:10:57.000000 vlttng-0.9.4/vlttng/profiles/glib-2.34.3.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:10:57.000000 vlttng-0.9.4/vlttng/profiles/glib-2.35.9.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:10:57.000000 vlttng-0.9.4/vlttng/profiles/glib-2.36.4.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      280 2016-05-20 00:10:57.000000 vlttng-0.9.4/vlttng/profiles/glib-2.37.93.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:10:57.000000 vlttng-0.9.4/vlttng/profiles/glib-2.38.2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      280 2016-05-20 00:10:57.000000 vlttng-0.9.4/vlttng/profiles/glib-2.39.92.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:10:57.000000 vlttng-0.9.4/vlttng/profiles/glib-2.40.2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:10:57.000000 vlttng-0.9.4/vlttng/profiles/glib-2.41.5.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:10:57.000000 vlttng-0.9.4/vlttng/profiles/glib-2.42.2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      280 2016-05-20 00:10:57.000000 vlttng-0.9.4/vlttng/profiles/glib-2.43.92.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:10:57.000000 vlttng-0.9.4/vlttng/profiles/glib-2.44.1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:10:57.000000 vlttng-0.9.4/vlttng/profiles/glib-2.45.8.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:10:57.000000 vlttng-0.9.4/vlttng/profiles/glib-2.46.2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      280 2016-05-20 00:10:57.000000 vlttng-0.9.4/vlttng/profiles/glib-2.47.92.yml
+-rw-rw-rw-   0 eepp      (1000) eepp      (1000)      279 2016-05-20 00:04:35.000000 vlttng-0.9.4/vlttng/profiles/glib-2.48.1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-10-18 18:03:34.000000 vlttng-0.9.4/vlttng/profiles/glib-2.48.2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-10-18 18:03:34.000000 vlttng-0.9.4/vlttng/profiles/glib-2.49.7.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2016-10-18 18:03:34.000000 vlttng-0.9.4/vlttng/profiles/glib-2.50.1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2017-10-19 18:27:25.000000 vlttng-0.9.4/vlttng/profiles/glib-2.51.5.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2017-10-19 18:27:25.000000 vlttng-0.9.4/vlttng/profiles/glib-2.52.2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2017-10-19 18:27:25.000000 vlttng-0.9.4/vlttng/profiles/glib-2.53.2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2017-10-19 18:28:37.000000 vlttng-0.9.4/vlttng/profiles/glib-2.54.1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2018-05-10 18:41:17.000000 vlttng-0.9.4/vlttng/profiles/glib-2.54.2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2018-05-10 18:41:21.000000 vlttng-0.9.4/vlttng/profiles/glib-2.54.3.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2018-05-10 18:41:53.000000 vlttng-0.9.4/vlttng/profiles/glib-2.55.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2018-05-10 18:41:57.000000 vlttng-0.9.4/vlttng/profiles/glib-2.55.1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2018-05-10 18:41:59.000000 vlttng-0.9.4/vlttng/profiles/glib-2.55.2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2018-05-10 18:42:18.000000 vlttng-0.9.4/vlttng/profiles/glib-2.56.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2018-05-10 18:42:20.000000 vlttng-0.9.4/vlttng/profiles/glib-2.56.1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2019-03-23 20:23:31.000000 vlttng-0.9.4/vlttng/profiles/glib-2.56.2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2019-03-23 20:23:36.000000 vlttng-0.9.4/vlttng/profiles/glib-2.56.3.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2019-03-23 20:23:39.000000 vlttng-0.9.4/vlttng/profiles/glib-2.56.4.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2019-03-23 20:23:58.000000 vlttng-0.9.4/vlttng/profiles/glib-2.57.1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2019-03-23 20:24:06.000000 vlttng-0.9.4/vlttng/profiles/glib-2.57.2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2019-03-23 20:24:09.000000 vlttng-0.9.4/vlttng/profiles/glib-2.57.3.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2019-03-23 20:24:32.000000 vlttng-0.9.4/vlttng/profiles/glib-2.58.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2019-03-23 20:24:35.000000 vlttng-0.9.4/vlttng/profiles/glib-2.58.1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2019-03-23 20:24:38.000000 vlttng-0.9.4/vlttng/profiles/glib-2.58.2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2019-03-23 20:24:40.000000 vlttng-0.9.4/vlttng/profiles/glib-2.58.3.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2019-03-23 20:24:56.000000 vlttng-0.9.4/vlttng/profiles/glib-2.59.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2019-03-23 20:24:59.000000 vlttng-0.9.4/vlttng/profiles/glib-2.59.1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2019-03-23 20:25:01.000000 vlttng-0.9.4/vlttng/profiles/glib-2.59.2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2019-03-23 20:25:04.000000 vlttng-0.9.4/vlttng/profiles/glib-2.59.3.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      279 2019-03-23 20:25:22.000000 vlttng-0.9.4/vlttng/profiles/glib-2.60.0.yml
+-rw-rw-rw-   0 eepp      (1000) eepp      (1000)      235 2016-11-01 03:07:38.000000 vlttng-0.9.4/vlttng/profiles/glib-master.yml
+-rw-rw-rw-   0 eepp      (1000) eepp      (1000)      148 2016-05-20 00:58:04.000000 vlttng-0.9.4/vlttng/profiles/libxml2-2.8.0.yml
+-rw-rw-rw-   0 eepp      (1000) eepp      (1000)      148 2016-05-20 00:57:53.000000 vlttng-0.9.4/vlttng/profiles/libxml2-2.9.0.yml
+-rw-rw-rw-   0 eepp      (1000) eepp      (1000)      148 2016-05-20 00:57:46.000000 vlttng-0.9.4/vlttng/profiles/libxml2-2.9.1.yml
+-rw-rw-rw-   0 eepp      (1000) eepp      (1000)      148 2016-05-20 00:57:35.000000 vlttng-0.9.4/vlttng/profiles/libxml2-2.9.2.yml
+-rw-rw-rw-   0 eepp      (1000) eepp      (1000)      148 2016-05-20 00:54:05.000000 vlttng-0.9.4/vlttng/profiles/libxml2-2.9.3.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      148 2016-11-17 21:18:07.000000 vlttng-0.9.4/vlttng/profiles/libxml2-2.9.4.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      148 2017-10-19 19:07:38.000000 vlttng-0.9.4/vlttng/profiles/libxml2-2.9.5.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      148 2017-10-19 19:07:43.000000 vlttng-0.9.4/vlttng/profiles/libxml2-2.9.6.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      148 2018-05-10 18:42:44.000000 vlttng-0.9.4/vlttng/profiles/libxml2-2.9.7.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      148 2018-05-10 18:42:47.000000 vlttng-0.9.4/vlttng/profiles/libxml2-2.9.8.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      148 2019-03-23 20:26:18.000000 vlttng-0.9.4/vlttng/profiles/libxml2-2.9.9.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      197 2016-11-01 04:50:01.000000 vlttng-0.9.4/vlttng/profiles/libxml2-master.yml
+-rw-rw-rw-   0 eepp      (1000) eepp      (1000)      107 2016-05-19 19:54:56.000000 vlttng-0.9.4/vlttng/profiles/lttng-analyses-0.3.0.yml
+-rw-rw-rw-   0 eepp      (1000) eepp      (1000)      107 2016-05-19 19:54:58.000000 vlttng-0.9.4/vlttng/profiles/lttng-analyses-0.4.0.yml
+-rw-rw-rw-   0 eepp      (1000) eepp      (1000)      107 2016-05-19 19:54:59.000000 vlttng-0.9.4/vlttng/profiles/lttng-analyses-0.4.1.yml
+-rw-rw-rw-   0 eepp      (1000) eepp      (1000)      107 2016-05-19 19:55:01.000000 vlttng-0.9.4/vlttng/profiles/lttng-analyses-0.4.2.yml
+-rw-rw-rw-   0 eepp      (1000) eepp      (1000)      107 2016-05-19 19:55:02.000000 vlttng-0.9.4/vlttng/profiles/lttng-analyses-0.4.3.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      107 2016-06-01 00:29:20.000000 vlttng-0.9.4/vlttng/profiles/lttng-analyses-0.5.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      107 2016-06-01 00:29:20.000000 vlttng-0.9.4/vlttng/profiles/lttng-analyses-0.5.1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      107 2016-08-10 15:54:40.000000 vlttng-0.9.4/vlttng/profiles/lttng-analyses-0.5.2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      107 2016-08-10 15:54:40.000000 vlttng-0.9.4/vlttng/profiles/lttng-analyses-0.5.3.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      107 2016-08-10 15:54:40.000000 vlttng-0.9.4/vlttng/profiles/lttng-analyses-0.5.4.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      107 2017-10-19 18:27:25.000000 vlttng-0.9.4/vlttng/profiles/lttng-analyses-0.6.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      107 2017-10-19 18:27:25.000000 vlttng-0.9.4/vlttng/profiles/lttng-analyses-0.6.1.yml
+-rw-rw-rw-   0 eepp      (1000) eepp      (1000)      107 2016-05-19 19:54:50.000000 vlttng-0.9.4/vlttng/profiles/lttng-analyses-master.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      205 2016-11-01 03:07:49.000000 vlttng-0.9.4/vlttng/profiles/lttng-master.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      111 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.10.0-rc1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      111 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.10.0-rc2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      107 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.10.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      107 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.10.1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      107 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.10.2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      107 2018-05-10 18:40:16.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.10.3.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      107 2018-05-10 18:40:20.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.10.4.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      107 2018-05-10 18:40:23.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.10.5.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      107 2018-05-10 18:40:26.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.10.6.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      107 2018-09-12 01:20:52.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.10.7.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      107 2019-03-23 20:27:04.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.10.8.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      107 2019-03-23 20:27:12.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.10.9.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      111 2018-09-12 01:16:01.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.11.0-rc1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      111 2019-03-23 20:27:22.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.11.0-rc2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      111 2019-03-23 20:27:25.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.11.0-rc3.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      111 2019-03-23 20:27:28.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.11.0-rc4.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      110 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.6.0-rc1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      110 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.6.0-rc2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.6.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.6.1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.6.2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.6.3.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.6.4.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.6.5.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.6.6.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      110 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.7.0-rc1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      110 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.7.0-rc2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.7.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.7.1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.7.2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.7.3.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.7.4.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.7.5.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.7.6.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.7.7.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      110 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.8.0-rc1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      110 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.8.0-rc2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.8.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.8.1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.8.2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.8.3.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.8.4.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.8.5.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.8.6.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.8.7.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      110 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.9.0-rc1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      110 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.9.0-rc2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.9.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.9.1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.9.2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.9.3.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.9.4.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      106 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-2.9.5.yml
+-rw-rw-rw-   0 eepp      (1000) eepp      (1000)       79 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-master.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      105 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-stable-2.10.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      105 2018-09-12 01:16:01.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-stable-2.11.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      104 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-stable-2.6.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      104 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-stable-2.7.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      104 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-stable-2.8.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      104 2017-10-19 18:59:27.000000 vlttng-0.9.4/vlttng/profiles/lttng-modules-stable-2.9.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      119 2018-05-14 15:57:57.000000 vlttng-0.9.4/vlttng/profiles/lttng-scope-0.3.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       80 2018-05-10 20:44:09.000000 vlttng-0.9.4/vlttng/profiles/lttng-scope-master.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      283 2017-10-19 18:27:25.000000 vlttng-0.9.4/vlttng/profiles/lttng-stable-2.10.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      283 2018-09-12 01:17:02.000000 vlttng-0.9.4/vlttng/profiles/lttng-stable-2.11.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      280 2016-11-01 03:07:56.000000 vlttng-0.9.4/vlttng/profiles/lttng-stable-2.6.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      280 2016-11-01 02:59:55.000000 vlttng-0.9.4/vlttng/profiles/lttng-stable-2.7.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      280 2016-11-01 02:59:55.000000 vlttng-0.9.4/vlttng/profiles/lttng-stable-2.8.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      280 2017-01-09 20:41:28.000000 vlttng-0.9.4/vlttng/profiles/lttng-stable-2.9.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      105 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.10.0-rc1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      105 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.10.0-rc2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      101 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.10.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      101 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.10.1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      101 2018-05-10 18:39:35.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.10.2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      101 2018-05-10 18:39:39.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.10.3.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      101 2018-05-10 18:39:42.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.10.4.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      101 2018-05-10 18:39:46.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.10.5.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      101 2019-03-23 20:27:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.10.6.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      105 2018-09-12 01:16:01.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.11.0-rc1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      104 2017-10-19 18:45:54.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.6.0-rc1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      104 2017-10-19 18:45:54.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.6.0-rc2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      104 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.6.0-rc3.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      104 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.6.0-rc4.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.6.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.6.1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.6.2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.6.3.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      104 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.7.0-rc1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      104 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.7.0-rc2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.7.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.7.1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.7.2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.7.3.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.7.4.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.7.5.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.7.6.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      104 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.8.0-rc1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.8.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.8.1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.8.2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.8.3.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.8.4.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.8.5.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.8.6.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.8.7.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.8.8.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      104 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.9.0-rc1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.9.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.9.1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.9.2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.9.3.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.9.4.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.9.5.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-10-19 18:45:53.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-2.9.6.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       65 2017-10-19 18:27:25.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-embedded-help.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       75 2016-11-01 04:50:01.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-master.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       72 2016-05-19 19:00:58.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-no-lttng-consumerd.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       68 2016-05-19 19:00:58.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-no-lttng-crash.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       69 2016-05-19 19:00:58.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-no-lttng-relayd.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       71 2016-05-19 19:00:58.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-no-lttng-sessiond.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       62 2016-05-19 19:00:58.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-no-lttng.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       62 2016-05-19 19:00:58.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-no-man-pages.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       68 2016-05-19 19:00:58.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-no-python.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       67 2016-05-19 19:00:58.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-python.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      101 2017-10-19 18:27:25.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-stable-2.10.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      101 2018-09-12 01:16:01.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-stable-2.11.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2016-11-01 02:59:55.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-stable-2.6.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2016-11-01 02:59:55.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-stable-2.7.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2016-11-01 02:59:55.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-stable-2.8.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      100 2017-01-09 20:41:28.000000 vlttng-0.9.4/vlttng/profiles/lttng-tools-stable-2.9.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       99 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.10.0-rc1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       99 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.10.0-rc2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       95 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.10.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       95 2018-05-10 18:39:05.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.10.1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       95 2018-09-12 01:20:19.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.10.2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       95 2019-03-23 20:28:20.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.10.3.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       99 2018-09-12 01:16:01.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.11.0-rc1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       99 2019-03-23 20:28:33.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.11.0-rc2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       98 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.6.0-rc1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       98 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.6.0-rc2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       98 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.6.0-rc3.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.6.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.6.1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.6.2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.6.3.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.6.4.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.6.5.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.6.6.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.6.7.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       98 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.7.0-rc1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       98 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.7.0-rc2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.7.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.7.1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.7.2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.7.3.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.7.4.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.7.5.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       98 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.8.0-rc1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       98 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.8.0-rc2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.8.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.8.1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.8.2.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.8.3.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.8.4.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       98 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.9.0-rc1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.9.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       94 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-2.9.1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       64 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-jul-agent.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       66 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-log4j-agent.yml
+-rw-rw-rw-   0 eepp      (1000) eepp      (1000)       71 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-master.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       60 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-no-man-pages.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       62 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-python-agent.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       97 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-stable-2.10.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       97 2018-09-12 01:16:01.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-stable-2.11.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       96 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-stable-2.6.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       96 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-stable-2.7.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       96 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-stable-2.8.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       96 2017-10-19 18:59:07.000000 vlttng-0.9.4/vlttng/profiles/lttng-ust-stable-2.9.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      142 2016-11-01 02:59:55.000000 vlttng-0.9.4/vlttng/profiles/popt-1.16.yml
+-rw-rw-rw-   0 eepp      (1000) eepp      (1000)      172 2016-05-19 20:38:33.000000 vlttng-0.9.4/vlttng/profiles/tracecompass-1.1.0.yml
+-rw-rw-rw-   0 eepp      (1000) eepp      (1000)      161 2016-05-19 20:38:38.000000 vlttng-0.9.4/vlttng/profiles/tracecompass-1.2.0.yml
+-rw-rw-rw-   0 eepp      (1000) eepp      (1000)      161 2016-05-19 20:38:41.000000 vlttng-0.9.4/vlttng/profiles/tracecompass-1.2.1.yml
+-rw-rw-rw-   0 eepp      (1000) eepp      (1000)      161 2016-07-13 19:11:13.000000 vlttng-0.9.4/vlttng/profiles/tracecompass-2.0.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      172 2017-10-19 18:27:25.000000 vlttng-0.9.4/vlttng/profiles/tracecompass-linux-x86-64-1.1.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      161 2017-10-19 18:27:25.000000 vlttng-0.9.4/vlttng/profiles/tracecompass-linux-x86-64-1.2.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      161 2017-10-19 18:27:25.000000 vlttng-0.9.4/vlttng/profiles/tracecompass-linux-x86-64-1.2.1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      161 2017-10-19 18:27:25.000000 vlttng-0.9.4/vlttng/profiles/tracecompass-linux-x86-64-2.0.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      161 2017-10-19 18:27:25.000000 vlttng-0.9.4/vlttng/profiles/tracecompass-linux-x86-64-2.0.1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      161 2017-10-19 18:27:25.000000 vlttng-0.9.4/vlttng/profiles/tracecompass-linux-x86-64-2.1.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      161 2017-10-19 18:27:25.000000 vlttng-0.9.4/vlttng/profiles/tracecompass-linux-x86-64-2.2.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      161 2017-10-19 18:27:25.000000 vlttng-0.9.4/vlttng/profiles/tracecompass-linux-x86-64-2.3.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      161 2017-10-19 19:05:10.000000 vlttng-0.9.4/vlttng/profiles/tracecompass-linux-x86-64-3.0.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      161 2017-10-19 19:06:35.000000 vlttng-0.9.4/vlttng/profiles/tracecompass-linux-x86-64-3.1.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      161 2018-05-10 18:45:49.000000 vlttng-0.9.4/vlttng/profiles/tracecompass-linux-x86-64-3.2.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      161 2018-05-10 18:47:11.000000 vlttng-0.9.4/vlttng/profiles/tracecompass-linux-x86-64-3.3.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      175 2017-10-19 18:27:25.000000 vlttng-0.9.4/vlttng/profiles/tracecompass-macos-x86-64-1.1.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      164 2017-10-19 18:27:25.000000 vlttng-0.9.4/vlttng/profiles/tracecompass-macos-x86-64-1.2.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      164 2017-10-19 18:27:25.000000 vlttng-0.9.4/vlttng/profiles/tracecompass-macos-x86-64-1.2.1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      164 2017-10-19 18:27:25.000000 vlttng-0.9.4/vlttng/profiles/tracecompass-macos-x86-64-2.0.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      164 2017-10-19 18:27:25.000000 vlttng-0.9.4/vlttng/profiles/tracecompass-macos-x86-64-2.0.1.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      164 2017-10-19 18:27:25.000000 vlttng-0.9.4/vlttng/profiles/tracecompass-macos-x86-64-2.1.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      164 2017-10-19 18:27:25.000000 vlttng-0.9.4/vlttng/profiles/tracecompass-macos-x86-64-2.2.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      164 2017-10-19 18:27:25.000000 vlttng-0.9.4/vlttng/profiles/tracecompass-macos-x86-64-2.3.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      164 2017-10-19 19:05:47.000000 vlttng-0.9.4/vlttng/profiles/tracecompass-macos-x86-64-3.0.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      164 2017-10-19 19:06:53.000000 vlttng-0.9.4/vlttng/profiles/tracecompass-macos-x86-64-3.1.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      164 2018-05-10 18:47:49.000000 vlttng-0.9.4/vlttng/profiles/tracecompass-macos-x86-64-3.2.0.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      164 2018-05-10 18:48:14.000000 vlttng-0.9.4/vlttng/profiles/tracecompass-macos-x86-64-3.3.0.yml
+-rw-rw-rw-   0 eepp      (1000) eepp      (1000)      112 2016-11-01 03:08:07.000000 vlttng-0.9.4/vlttng/profiles/tracecompass-master.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       72 2016-11-01 03:08:09.000000 vlttng-0.9.4/vlttng/profiles/urcu-master.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       98 2017-10-19 18:27:25.000000 vlttng-0.9.4/vlttng/profiles/urcu-stable-0.10.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       97 2016-05-19 19:00:58.000000 vlttng-0.9.4/vlttng/profiles/urcu-stable-0.7.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       97 2016-05-19 19:00:58.000000 vlttng-0.9.4/vlttng/profiles/urcu-stable-0.8.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       97 2016-05-19 19:00:58.000000 vlttng-0.9.4/vlttng/profiles/urcu-stable-0.9.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       46 2016-11-01 02:59:55.000000 vlttng-0.9.4/vlttng/profiles/use-ccache-gcc.yml
+-rw-r--r--   0 eepp      (1000) eepp      (1000)     2790 2016-10-29 23:04:11.000000 vlttng-0.9.4/vlttng/update_template.py
+-rw-r--r--   0 eepp      (1000) eepp      (1000)     1367 2016-05-19 19:00:58.000000 vlttng-0.9.4/vlttng/utils.py
+-rw-r--r--   0 eepp      (1000) eepp      (1000)    29706 2018-09-24 18:20:59.000000 vlttng-0.9.4/vlttng/venv.py
+-rw-r--r--   0 eepp      (1000) eepp      (1000)     6977 2018-05-10 18:54:47.000000 vlttng-0.9.4/vlttng/vlttng_cli.py
+-rw-r--r--   0 eepp      (1000) eepp      (1000)    18345 2018-05-10 21:09:57.000000 vlttng-0.9.4/vlttng/vlttng_quick_cli.py
+drwxr-xr-x   0 eepp      (1000) eepp      (1000)        0 2019-03-23 22:13:36.000000 vlttng-0.9.4/vlttng.egg-info/
+-rw-r--r--   0 eepp      (1000) eepp      (1000)      686 2019-03-23 22:13:35.000000 vlttng-0.9.4/vlttng.egg-info/PKG-INFO
+-rw-r--r--   0 eepp      (1000) eepp      (1000)    12784 2019-03-23 22:13:36.000000 vlttng-0.9.4/vlttng.egg-info/SOURCES.txt
+-rw-r--r--   0 eepp      (1000) eepp      (1000)        1 2019-03-23 22:13:35.000000 vlttng-0.9.4/vlttng.egg-info/dependency_links.txt
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       93 2019-03-23 22:13:35.000000 vlttng-0.9.4/vlttng.egg-info/entry_points.txt
+-rw-r--r--   0 eepp      (1000) eepp      (1000)       28 2019-03-23 22:13:35.000000 vlttng-0.9.4/vlttng.egg-info/requires.txt
+-rw-r--r--   0 eepp      (1000) eepp      (1000)        7 2019-03-23 22:13:35.000000 vlttng-0.9.4/vlttng.egg-info/top_level.txt
```

### Comparing `vlttng-0.9.3/vlttng/__init__.py` & `vlttng-0.9.4/vlttng/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,9 +16,9 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
-__version__ = '0.9.3'
+__version__ = '0.9.4'
 _PROFILES_DIRNAME = 'profiles'
```

### Comparing `vlttng-0.9.3/vlttng/build_template.py` & `vlttng-0.9.4/vlttng/build_template.py`

 * *Files identical despite different names*

### Comparing `vlttng-0.9.3/vlttng/conf_template.py` & `vlttng-0.9.4/vlttng/conf_template.py`

 * *Files identical despite different names*

### Comparing `vlttng-0.9.3/vlttng/venv.py` & `vlttng-0.9.4/vlttng/venv.py`

 * *Files identical despite different names*

### Comparing `vlttng-0.9.3/vlttng/vlttng_cli.py` & `vlttng-0.9.4/vlttng/vlttng_cli.py`

 * *Files identical despite different names*

### Comparing `vlttng-0.9.3/vlttng/update_template.py` & `vlttng-0.9.4/vlttng/update_template.py`

 * *Files identical despite different names*

### Comparing `vlttng-0.9.3/vlttng/install_template.py` & `vlttng-0.9.4/vlttng/install_template.py`

 * *Files identical despite different names*

### Comparing `vlttng-0.9.3/vlttng/profiles/all-master.yml` & `vlttng-0.9.4/vlttng/profiles/all-master.yml`

 * *Files identical despite different names*

### Comparing `vlttng-0.9.3/vlttng/activate_template.py` & `vlttng-0.9.4/vlttng/activate_template.py`

 * *Files identical despite different names*

### Comparing `vlttng-0.9.3/vlttng/vlttng_quick_cli.py` & `vlttng-0.9.4/vlttng/vlttng_quick_cli.py`

 * *Files identical despite different names*

### Comparing `vlttng-0.9.3/vlttng/profile.py` & `vlttng-0.9.4/vlttng/profile.py`

 * *Files identical despite different names*

### Comparing `vlttng-0.9.3/vlttng/utils.py` & `vlttng-0.9.4/vlttng/utils.py`

 * *Files identical despite different names*

### Comparing `vlttng-0.9.3/setup.py` & `vlttng-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `vlttng-0.9.3/PKG-INFO` & `vlttng-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: vlttng
-Version: 0.9.3
+Version: 0.9.4
 Summary: Generator of LTTng virtual environment
 Home-page: https://github.com/eepp/vlttng
 Author: Philippe Proulx
 Author-email: eeppeliteloop@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `vlttng-0.9.3/vlttng.egg-info/SOURCES.txt` & `vlttng-0.9.4/vlttng.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,20 @@
 vlttng/profiles/babeltrace-stable-1.5.yml
 vlttng/profiles/debug-flags.yml
 vlttng/profiles/elfutils-0.166.yml
 vlttng/profiles/elfutils-0.167.yml
 vlttng/profiles/elfutils-0.168.yml
 vlttng/profiles/elfutils-0.169.yml
 vlttng/profiles/elfutils-0.170.yml
+vlttng/profiles/elfutils-0.171.yml
+vlttng/profiles/elfutils-0.172.yml
+vlttng/profiles/elfutils-0.173.yml
+vlttng/profiles/elfutils-0.174.yml
+vlttng/profiles/elfutils-0.175.yml
+vlttng/profiles/elfutils-0.176.yml
 vlttng/profiles/glib-2.22.5.yml
 vlttng/profiles/glib-2.23.6.yml
 vlttng/profiles/glib-2.24.2.yml
 vlttng/profiles/glib-2.25.17.yml
 vlttng/profiles/glib-2.26.1.yml
 vlttng/profiles/glib-2.27.93.yml
 vlttng/profiles/glib-2.28.8.yml
@@ -67,25 +73,41 @@
 vlttng/profiles/glib-2.54.2.yml
 vlttng/profiles/glib-2.54.3.yml
 vlttng/profiles/glib-2.55.0.yml
 vlttng/profiles/glib-2.55.1.yml
 vlttng/profiles/glib-2.55.2.yml
 vlttng/profiles/glib-2.56.0.yml
 vlttng/profiles/glib-2.56.1.yml
+vlttng/profiles/glib-2.56.2.yml
+vlttng/profiles/glib-2.56.3.yml
+vlttng/profiles/glib-2.56.4.yml
+vlttng/profiles/glib-2.57.1.yml
+vlttng/profiles/glib-2.57.2.yml
+vlttng/profiles/glib-2.57.3.yml
+vlttng/profiles/glib-2.58.0.yml
+vlttng/profiles/glib-2.58.1.yml
+vlttng/profiles/glib-2.58.2.yml
+vlttng/profiles/glib-2.58.3.yml
+vlttng/profiles/glib-2.59.0.yml
+vlttng/profiles/glib-2.59.1.yml
+vlttng/profiles/glib-2.59.2.yml
+vlttng/profiles/glib-2.59.3.yml
+vlttng/profiles/glib-2.60.0.yml
 vlttng/profiles/glib-master.yml
 vlttng/profiles/libxml2-2.8.0.yml
 vlttng/profiles/libxml2-2.9.0.yml
 vlttng/profiles/libxml2-2.9.1.yml
 vlttng/profiles/libxml2-2.9.2.yml
 vlttng/profiles/libxml2-2.9.3.yml
 vlttng/profiles/libxml2-2.9.4.yml
 vlttng/profiles/libxml2-2.9.5.yml
 vlttng/profiles/libxml2-2.9.6.yml
 vlttng/profiles/libxml2-2.9.7.yml
 vlttng/profiles/libxml2-2.9.8.yml
+vlttng/profiles/libxml2-2.9.9.yml
 vlttng/profiles/libxml2-master.yml
 vlttng/profiles/lttng-analyses-0.3.0.yml
 vlttng/profiles/lttng-analyses-0.4.0.yml
 vlttng/profiles/lttng-analyses-0.4.1.yml
 vlttng/profiles/lttng-analyses-0.4.2.yml
 vlttng/profiles/lttng-analyses-0.4.3.yml
 vlttng/profiles/lttng-analyses-0.5.0.yml
@@ -103,15 +125,20 @@
 vlttng/profiles/lttng-modules-2.10.1.yml
 vlttng/profiles/lttng-modules-2.10.2.yml
 vlttng/profiles/lttng-modules-2.10.3.yml
 vlttng/profiles/lttng-modules-2.10.4.yml
 vlttng/profiles/lttng-modules-2.10.5.yml
 vlttng/profiles/lttng-modules-2.10.6.yml
 vlttng/profiles/lttng-modules-2.10.7.yml
+vlttng/profiles/lttng-modules-2.10.8.yml
+vlttng/profiles/lttng-modules-2.10.9.yml
 vlttng/profiles/lttng-modules-2.11.0-rc1.yml
+vlttng/profiles/lttng-modules-2.11.0-rc2.yml
+vlttng/profiles/lttng-modules-2.11.0-rc3.yml
+vlttng/profiles/lttng-modules-2.11.0-rc4.yml
 vlttng/profiles/lttng-modules-2.6.0-rc1.yml
 vlttng/profiles/lttng-modules-2.6.0-rc2.yml
 vlttng/profiles/lttng-modules-2.6.0.yml
 vlttng/profiles/lttng-modules-2.6.1.yml
 vlttng/profiles/lttng-modules-2.6.2.yml
 vlttng/profiles/lttng-modules-2.6.3.yml
 vlttng/profiles/lttng-modules-2.6.4.yml
@@ -164,14 +191,15 @@
 vlttng/profiles/lttng-tools-2.10.0-rc2.yml
 vlttng/profiles/lttng-tools-2.10.0.yml
 vlttng/profiles/lttng-tools-2.10.1.yml
 vlttng/profiles/lttng-tools-2.10.2.yml
 vlttng/profiles/lttng-tools-2.10.3.yml
 vlttng/profiles/lttng-tools-2.10.4.yml
 vlttng/profiles/lttng-tools-2.10.5.yml
+vlttng/profiles/lttng-tools-2.10.6.yml
 vlttng/profiles/lttng-tools-2.11.0-rc1.yml
 vlttng/profiles/lttng-tools-2.6.0-rc1.yml
 vlttng/profiles/lttng-tools-2.6.0-rc2.yml
 vlttng/profiles/lttng-tools-2.6.0-rc3.yml
 vlttng/profiles/lttng-tools-2.6.0-rc4.yml
 vlttng/profiles/lttng-tools-2.6.0.yml
 vlttng/profiles/lttng-tools-2.6.1.yml
@@ -221,15 +249,17 @@
 vlttng/profiles/lttng-tools-stable-2.8.yml
 vlttng/profiles/lttng-tools-stable-2.9.yml
 vlttng/profiles/lttng-ust-2.10.0-rc1.yml
 vlttng/profiles/lttng-ust-2.10.0-rc2.yml
 vlttng/profiles/lttng-ust-2.10.0.yml
 vlttng/profiles/lttng-ust-2.10.1.yml
 vlttng/profiles/lttng-ust-2.10.2.yml
+vlttng/profiles/lttng-ust-2.10.3.yml
 vlttng/profiles/lttng-ust-2.11.0-rc1.yml
+vlttng/profiles/lttng-ust-2.11.0-rc2.yml
 vlttng/profiles/lttng-ust-2.6.0-rc1.yml
 vlttng/profiles/lttng-ust-2.6.0-rc2.yml
 vlttng/profiles/lttng-ust-2.6.0-rc3.yml
 vlttng/profiles/lttng-ust-2.6.0.yml
 vlttng/profiles/lttng-ust-2.6.1.yml
 vlttng/profiles/lttng-ust-2.6.2.yml
 vlttng/profiles/lttng-ust-2.6.3.yml
```

### Comparing `vlttng-0.9.3/vlttng.egg-info/PKG-INFO` & `vlttng-0.9.4/vlttng.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: vlttng
-Version: 0.9.3
+Version: 0.9.4
 Summary: Generator of LTTng virtual environment
 Home-page: https://github.com/eepp/vlttng
 Author: Philippe Proulx
 Author-email: eeppeliteloop@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

