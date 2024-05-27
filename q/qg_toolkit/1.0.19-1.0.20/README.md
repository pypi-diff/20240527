# Comparing `tmp/qg_toolkit-1.0.19.tar.gz` & `tmp/qg_toolkit-1.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qg_toolkit-1.0.19.tar", max compression
+gzip compressed data, was "qg_toolkit-1.0.20.tar", max compression
```

## Comparing `qg_toolkit-1.0.19.tar` & `qg_toolkit-1.0.20.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0      854 2024-05-02 09:58:36.462299 qg_toolkit-1.0.19/pyproject.toml
--rw-r--r--   0        0        0       94 2024-04-27 10:53:56.731750 qg_toolkit-1.0.19/qg_toolkit/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 18:53:34.039466 qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/__init__.py
--rw-r--r--   0        0        0       94 2024-04-27 10:54:32.432326 qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_fullpage/__init__.py
--rw-r--r--   0        0        0     5190 2024-04-24 18:53:34.040467 qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_fullpage/geetest_v4.py
--rw-r--r--   0        0        0     5433 2024-04-24 18:53:34.040467 qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_fullpage/jiyan.js
--rw-r--r--   0        0        0     2288 2024-04-27 11:00:05.704720 qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_fullpage/mian.py
--rw-r--r--   0        0        0       94 2024-04-27 10:54:37.081886 qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/__init__.py
--rw-r--r--   0        0        0     2723 2024-04-24 18:53:34.042468 qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/gap.py
--rw-r--r--   0        0        0    37946 2024-04-29 17:00:55.850149 qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/geetest_slide_v4.py
--rw-r--r--   0        0        0    51280 2024-04-24 18:53:34.044476 qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/img/bg.png
--rw-r--r--   0        0        0     4818 2024-04-24 18:53:34.045475 qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/img/show_image.png
--rw-r--r--   0        0        0     9121 2024-04-24 18:53:34.045475 qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/img/slide.png
--rw-r--r--   0        0        0  1793853 2024-04-24 18:53:34.058465 qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/img/tracks.json
--rw-r--r--   0        0        0     2362 2024-04-24 18:53:34.059468 qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/jiyan.js
--rw-r--r--   0        0        0     2349 2024-04-27 11:14:05.254088 qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/mian.py
--rw-r--r--   0        0        0     1043 2024-04-24 18:53:34.060469 qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/trace.py
--rw-r--r--   0        0        0   101372 2024-04-29 17:00:55.853150 qg_toolkit-1.0.19/qg_toolkit/qgalxe/galxe.py
--rw-r--r--   0        0        0     5383 2024-05-02 09:57:56.938543 qg_toolkit-1.0.19/qg_toolkit/qgalxe/GeetestFullPageV4.py
--rw-r--r--   0        0        0     3795 2024-04-29 17:00:55.851150 qg_toolkit-1.0.19/qg_toolkit/qgalxe/GeetestSlideV4.py
--rw-r--r--   0        0        0       96 2024-04-27 10:54:21.799092 qg_toolkit-1.0.19/qg_toolkit/qtweepy/__init__.py
--rw-r--r--   0        0        0      103 2024-04-27 10:52:23.199431 qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/__init__.py
--rw-r--r--   0        0        0     4912 2024-04-29 17:00:55.853150 qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/account_checker.py
--rw-r--r--   0        0        0     2251 2024-04-27 10:52:23.208431 qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/follow_each_other.py
--rw-r--r--   0        0        0        0 2024-04-27 05:31:12.415935 qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/input-output/BAD_TOKEN.txt
--rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/input-output/CONSENT_LOCKED.txt
--rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/input-output/GOOD.txt
--rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/input-output/LOCKED.txt
--rw-r--r--   0        0        0       44 2024-04-29 17:00:55.854150 qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/input-output/PROXIES.txt
--rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/input-output/SUSPENDED.txt
--rw-r--r--   0        0        0       40 2024-04-27 05:31:12.415935 qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/input-output/UNKNOWN.txt
--rw-r--r--   0        0        0     3622 2024-04-27 10:52:23.284728 qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/mavia.py
--rw-r--r--   0        0        0     2373 2024-04-27 10:52:23.217431 qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/set_2fa.py
--rw-r--r--   0        0        0     3081 2024-04-27 10:52:23.184432 qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/set_avatars_and_banners.py
--rw-r--r--   0        0        0      697 2024-04-27 10:52:23.174431 qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/uploading_images.py
--rw-r--r--   0        0        0     2253 2024-04-27 10:52:23.159432 qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/voter.py
--rw-r--r--   0        0        0     3120 2024-04-27 10:52:23.191432 qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/xai.py
--rw-r--r--   0        0        0      687 2024-04-20 19:57:03.446998 qg_toolkit-1.0.19/qg_toolkit/qtweepy/pyproject.toml
--rw-r--r--   0        0        0     8720 2024-04-20 19:48:15.063903 qg_toolkit-1.0.19/qg_toolkit/qtweepy/README.md
--rw-r--r--   0        0        0      132 2024-04-24 18:22:26.184000 qg_toolkit-1.0.19/qg_toolkit/qtweepy/tea.yaml
--rw-r--r--   0        0        0      732 2024-04-20 19:48:15.068902 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/__init__.py
--rw-r--r--   0        0        0        0 2024-04-20 19:48:15.069903 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/_capsolver/__init__.py
--rw-r--r--   0        0        0        0 2024-04-20 19:48:15.069903 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/_capsolver/core/__init__.py
--rw-r--r--   0        0        0     8883 2024-04-20 19:48:15.070903 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/_capsolver/core/base.py
--rw-r--r--   0        0        0     1054 2024-04-20 19:48:15.070903 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/_capsolver/core/config.py
--rw-r--r--   0        0        0     1741 2024-04-20 19:48:15.071903 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/_capsolver/core/enum.py
--rw-r--r--   0        0        0     2602 2024-04-20 19:48:15.071903 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/_capsolver/core/serializer.py
--rw-r--r--   0        0        0    10974 2024-04-20 19:48:15.072903 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/_capsolver/fun_captcha.py
--rw-r--r--   0        0        0     3248 2024-04-20 19:48:15.072903 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/account.py
--rw-r--r--   0        0        0      141 2024-04-20 19:48:15.072903 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/base/__init__.py
--rw-r--r--   0        0        0      500 2024-04-20 19:48:15.074292 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/base/client.py
--rw-r--r--   0        0        0     2175 2024-04-27 10:52:23.255728 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/base/session.py
--rw-r--r--   0        0        0    70738 2024-04-20 19:48:15.075686 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/client.py
--rw-r--r--   0        0        0      267 2024-04-20 19:48:15.076283 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/enums.py
--rw-r--r--   0        0        0     5322 2024-04-20 19:48:15.076811 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/errors.py
--rw-r--r--   0        0        0     4695 2024-04-20 19:48:15.076811 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/models.py
--rw-r--r--   0        0        0      665 2024-04-20 19:48:15.077920 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/utils/__init__.py
--rw-r--r--   0        0        0     1152 2024-04-20 19:48:15.077920 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/utils/file.py
--rw-r--r--   0        0        0     2140 2024-04-20 19:48:15.078463 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/utils/html.py
--rw-r--r--   0        0        0     1061 2024-04-20 19:48:15.078992 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/utils/other.py
--rw-r--r--   0        0        0      279 2024-04-29 17:00:55.855149 qg_toolkit-1.0.19/qg_toolkit/test/demo.yaml
--rw-r--r--   0        0        0        0 2024-04-27 11:06:09.049630 qg_toolkit-1.0.19/qg_toolkit/test/test.py
--rw-r--r--   0        0        0       96 2024-04-27 10:54:04.685704 qg_toolkit-1.0.19/qg_toolkit/tools/__init__.py
--rw-r--r--   0        0        0     5391 2024-04-29 17:18:03.385731 qg_toolkit-1.0.19/qg_toolkit/tools/cui_qiu_client.py
--rw-r--r--   0        0        0     1245 2024-04-29 17:00:55.856150 qg_toolkit-1.0.19/qg_toolkit/tools/date_util.py
--rw-r--r--   0        0        0    12289 2024-04-29 17:00:55.857149 qg_toolkit-1.0.19/qg_toolkit/tools/discord.py
--rw-r--r--   0        0        0     5905 2024-04-29 05:37:22.967370 qg_toolkit-1.0.19/qg_toolkit/tools/qg_airdrop.py
--rw-r--r--   0        0        0      985 2024-04-20 20:27:34.147592 qg_toolkit-1.0.19/qg_toolkit/tools/qg_crypto.py
--rw-r--r--   0        0        0    36155 2024-04-29 17:00:55.858150 qg_toolkit-1.0.19/qg_toolkit/tools/qg_eth.py
--rw-r--r--   0        0        0     3710 2024-05-02 09:57:56.939543 qg_toolkit-1.0.19/qg_toolkit/tools/qg_file.py
--rw-r--r--   0        0        0      300 2024-04-24 18:53:34.062471 qg_toolkit-1.0.19/qg_toolkit/tools/qg_models.py
--rw-r--r--   0        0        0      741 2024-04-20 20:24:22.248041 qg_toolkit-1.0.19/qg_toolkit/tools/qg_random.py
--rw-r--r--   0        0        0     6168 2024-04-29 05:55:33.712699 qg_toolkit-1.0.19/qg_toolkit/tools/qg_solana.py
--rw-r--r--   0        0        0     2764 2024-04-24 18:21:31.477405 qg_toolkit-1.0.19/qg_toolkit/tools/qg_starknet.py
--rw-r--r--   0        0        0     3241 2024-04-20 19:48:15.080086 qg_toolkit-1.0.19/qg_toolkit/tools/qproxy.py
--rw-r--r--   0        0        0     1239 2024-04-29 17:00:55.858150 qg_toolkit-1.0.19/qg_toolkit/tools/random_tool.py
--rw-r--r--   0        0        0     6113 2024-05-02 06:59:59.061718 qg_toolkit-1.0.19/qg_toolkit/tools/rpc.py
--rw-r--r--   0        0        0    72567 2024-04-29 17:16:01.332559 qg_toolkit-1.0.19/qg_toolkit/tools/twitter.py
--rw-r--r--   0        0        0     4182 2024-04-29 17:16:29.644862 qg_toolkit-1.0.19/qg_toolkit/tools/yescaptcha.py
--rw-r--r--   0        0        0       38 2024-04-20 19:50:56.436133 qg_toolkit-1.0.19/README.md
--rw-r--r--   0        0        0      133 2024-05-02 09:59:11.389046 qg_toolkit-1.0.19/tea.yaml
--rw-r--r--   0        0        0     1370 1970-01-01 00:00:00.000000 qg_toolkit-1.0.19/PKG-INFO
+-rw-r--r--   0        0        0      854 2024-05-27 09:39:43.313119 qg_toolkit-1.0.20/pyproject.toml
+-rw-r--r--   0        0        0       94 2024-04-28 01:55:09.875818 qg_toolkit-1.0.20/qg_toolkit/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 01:55:09.876818 qg_toolkit-1.0.20/qg_toolkit/geetest_captcha/__init__.py
+-rw-r--r--   0        0        0       94 2024-04-28 01:55:09.876818 qg_toolkit-1.0.20/qg_toolkit/geetest_captcha/geetest4_fullpage/__init__.py
+-rw-r--r--   0        0        0     5190 2024-04-28 01:55:09.877828 qg_toolkit-1.0.20/qg_toolkit/geetest_captcha/geetest4_fullpage/geetest_v4.py
+-rw-r--r--   0        0        0     5433 2024-04-28 01:55:09.877828 qg_toolkit-1.0.20/qg_toolkit/geetest_captcha/geetest4_fullpage/jiyan.js
+-rw-r--r--   0        0        0     2288 2024-04-28 01:55:09.877828 qg_toolkit-1.0.20/qg_toolkit/geetest_captcha/geetest4_fullpage/mian.py
+-rw-r--r--   0        0        0       94 2024-04-28 01:55:09.878819 qg_toolkit-1.0.20/qg_toolkit/geetest_captcha/geetest4_slide/__init__.py
+-rw-r--r--   0        0        0     2723 2024-04-28 01:55:09.878819 qg_toolkit-1.0.20/qg_toolkit/geetest_captcha/geetest4_slide/gap.py
+-rw-r--r--   0        0        0    37946 2024-04-29 11:35:41.976417 qg_toolkit-1.0.20/qg_toolkit/geetest_captcha/geetest4_slide/geetest_slide_v4.py
+-rw-r--r--   0        0        0    51280 2024-04-28 01:55:09.880829 qg_toolkit-1.0.20/qg_toolkit/geetest_captcha/geetest4_slide/img/bg.png
+-rw-r--r--   0        0        0     4818 2024-04-28 01:55:09.880829 qg_toolkit-1.0.20/qg_toolkit/geetest_captcha/geetest4_slide/img/show_image.png
+-rw-r--r--   0        0        0     9121 2024-04-28 01:55:09.881818 qg_toolkit-1.0.20/qg_toolkit/geetest_captcha/geetest4_slide/img/slide.png
+-rw-r--r--   0        0        0  1793853 2024-04-28 01:55:09.890818 qg_toolkit-1.0.20/qg_toolkit/geetest_captcha/geetest4_slide/img/tracks.json
+-rw-r--r--   0        0        0     2362 2024-04-28 01:55:09.890818 qg_toolkit-1.0.20/qg_toolkit/geetest_captcha/geetest4_slide/jiyan.js
+-rw-r--r--   0        0        0     2349 2024-04-28 01:55:09.891818 qg_toolkit-1.0.20/qg_toolkit/geetest_captcha/geetest4_slide/mian.py
+-rw-r--r--   0        0        0     1043 2024-04-28 01:55:09.891818 qg_toolkit-1.0.20/qg_toolkit/geetest_captcha/geetest4_slide/trace.py
+-rw-r--r--   0        0        0   101372 2024-04-29 10:29:45.977586 qg_toolkit-1.0.20/qg_toolkit/qgalxe/galxe.py
+-rw-r--r--   0        0        0     5383 2024-05-23 09:29:16.359221 qg_toolkit-1.0.20/qg_toolkit/qgalxe/GeetestFullPageV4.py
+-rw-r--r--   0        0        0     3795 2024-04-29 11:32:19.680739 qg_toolkit-1.0.20/qg_toolkit/qgalxe/GeetestSlideV4.py
+-rw-r--r--   0        0        0       96 2024-04-28 01:55:09.892818 qg_toolkit-1.0.20/qg_toolkit/qtweepy/__init__.py
+-rw-r--r--   0        0        0      103 2024-04-28 01:55:09.892818 qg_toolkit-1.0.20/qg_toolkit/qtweepy/examples/__init__.py
+-rw-r--r--   0        0        0     4912 2024-04-28 06:26:10.954966 qg_toolkit-1.0.20/qg_toolkit/qtweepy/examples/account_checker.py
+-rw-r--r--   0        0        0     2251 2024-04-28 01:55:09.893817 qg_toolkit-1.0.20/qg_toolkit/qtweepy/examples/follow_each_other.py
+-rw-r--r--   0        0        0        0 2024-04-28 06:38:00.187702 qg_toolkit-1.0.20/qg_toolkit/qtweepy/examples/input-output/BAD_TOKEN.txt
+-rw-r--r--   0        0        0        0 2024-04-28 06:38:00.188701 qg_toolkit-1.0.20/qg_toolkit/qtweepy/examples/input-output/CONSENT_LOCKED.txt
+-rw-r--r--   0        0        0        0 2024-04-28 06:38:00.188701 qg_toolkit-1.0.20/qg_toolkit/qtweepy/examples/input-output/GOOD.txt
+-rw-r--r--   0        0        0        0 2024-04-28 06:38:00.188701 qg_toolkit-1.0.20/qg_toolkit/qtweepy/examples/input-output/LOCKED.txt
+-rw-r--r--   0        0        0       44 2024-04-28 06:37:01.438691 qg_toolkit-1.0.20/qg_toolkit/qtweepy/examples/input-output/PROXIES.txt
+-rw-r--r--   0        0        0        0 2024-04-28 06:38:00.187702 qg_toolkit-1.0.20/qg_toolkit/qtweepy/examples/input-output/SUSPENDED.txt
+-rw-r--r--   0        0        0       40 2024-04-28 06:38:00.187702 qg_toolkit-1.0.20/qg_toolkit/qtweepy/examples/input-output/UNKNOWN.txt
+-rw-r--r--   0        0        0     3622 2024-04-28 01:55:09.894817 qg_toolkit-1.0.20/qg_toolkit/qtweepy/examples/mavia.py
+-rw-r--r--   0        0        0     2373 2024-04-28 01:55:09.895818 qg_toolkit-1.0.20/qg_toolkit/qtweepy/examples/set_2fa.py
+-rw-r--r--   0        0        0     3081 2024-04-28 01:55:09.895818 qg_toolkit-1.0.20/qg_toolkit/qtweepy/examples/set_avatars_and_banners.py
+-rw-r--r--   0        0        0      697 2024-04-28 01:55:09.895818 qg_toolkit-1.0.20/qg_toolkit/qtweepy/examples/uploading_images.py
+-rw-r--r--   0        0        0     2253 2024-04-28 01:55:09.896820 qg_toolkit-1.0.20/qg_toolkit/qtweepy/examples/voter.py
+-rw-r--r--   0        0        0     3120 2024-04-28 01:55:09.896820 qg_toolkit-1.0.20/qg_toolkit/qtweepy/examples/xai.py
+-rw-r--r--   0        0        0      687 2024-04-28 01:55:09.896820 qg_toolkit-1.0.20/qg_toolkit/qtweepy/pyproject.toml
+-rw-r--r--   0        0        0     8720 2024-04-28 01:55:09.892818 qg_toolkit-1.0.20/qg_toolkit/qtweepy/README.md
+-rw-r--r--   0        0        0      132 2024-04-28 01:55:09.897831 qg_toolkit-1.0.20/qg_toolkit/qtweepy/tea.yaml
+-rw-r--r--   0        0        0      732 2024-04-28 01:55:09.897831 qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 01:55:09.897831 qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/_capsolver/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 01:55:09.897831 qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/_capsolver/core/__init__.py
+-rw-r--r--   0        0        0     8883 2024-04-28 01:55:09.898831 qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/_capsolver/core/base.py
+-rw-r--r--   0        0        0     1054 2024-04-28 01:55:09.898831 qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/_capsolver/core/config.py
+-rw-r--r--   0        0        0     1741 2024-04-28 01:55:09.899826 qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/_capsolver/core/enum.py
+-rw-r--r--   0        0        0     2602 2024-04-28 01:55:09.899826 qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/_capsolver/core/serializer.py
+-rw-r--r--   0        0        0    10974 2024-04-28 01:55:09.900819 qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/_capsolver/fun_captcha.py
+-rw-r--r--   0        0        0     3248 2024-04-28 01:55:09.900819 qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/account.py
+-rw-r--r--   0        0        0      141 2024-04-28 01:55:09.900819 qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/base/__init__.py
+-rw-r--r--   0        0        0      500 2024-04-28 01:55:09.901826 qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/base/client.py
+-rw-r--r--   0        0        0     2175 2024-04-28 01:55:09.901826 qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/base/session.py
+-rw-r--r--   0        0        0    70738 2024-04-28 01:55:09.902820 qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/client.py
+-rw-r--r--   0        0        0      267 2024-04-28 01:55:09.902820 qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/enums.py
+-rw-r--r--   0        0        0     5322 2024-04-28 01:55:09.903823 qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/errors.py
+-rw-r--r--   0        0        0     4695 2024-04-28 01:55:09.903823 qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/models.py
+-rw-r--r--   0        0        0      665 2024-04-28 01:55:09.903823 qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/utils/__init__.py
+-rw-r--r--   0        0        0     1152 2024-04-28 01:55:09.904830 qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/utils/file.py
+-rw-r--r--   0        0        0     2140 2024-04-28 01:55:09.904830 qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/utils/html.py
+-rw-r--r--   0        0        0     1061 2024-04-28 01:55:09.904830 qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/utils/other.py
+-rw-r--r--   0        0        0      279 2024-04-28 01:55:09.905829 qg_toolkit-1.0.20/qg_toolkit/test/demo.yaml
+-rw-r--r--   0        0        0        0 2024-04-28 01:55:09.905829 qg_toolkit-1.0.20/qg_toolkit/test/test.py
+-rw-r--r--   0        0        0       96 2024-04-28 01:55:09.905829 qg_toolkit-1.0.20/qg_toolkit/tools/__init__.py
+-rw-r--r--   0        0        0     5391 2024-04-30 01:04:07.615542 qg_toolkit-1.0.20/qg_toolkit/tools/cui_qiu_client.py
+-rw-r--r--   0        0        0     1245 2024-04-29 09:52:12.132611 qg_toolkit-1.0.20/qg_toolkit/tools/date_util.py
+-rw-r--r--   0        0        0    12289 2024-04-29 09:59:28.288628 qg_toolkit-1.0.20/qg_toolkit/tools/discord.py
+-rw-r--r--   0        0        0     5905 2024-04-29 06:52:45.801970 qg_toolkit-1.0.20/qg_toolkit/tools/qg_airdrop.py
+-rw-r--r--   0        0        0      985 2024-04-28 01:55:09.906829 qg_toolkit-1.0.20/qg_toolkit/tools/qg_crypto.py
+-rw-r--r--   0        0        0    36155 2024-04-29 07:53:05.424108 qg_toolkit-1.0.20/qg_toolkit/tools/qg_eth.py
+-rw-r--r--   0        0        0     3710 2024-04-30 08:41:06.280335 qg_toolkit-1.0.20/qg_toolkit/tools/qg_file.py
+-rw-r--r--   0        0        0      300 2024-04-28 01:55:09.908828 qg_toolkit-1.0.20/qg_toolkit/tools/qg_models.py
+-rw-r--r--   0        0        0      741 2024-04-28 01:55:09.908828 qg_toolkit-1.0.20/qg_toolkit/tools/qg_random.py
+-rw-r--r--   0        0        0     6168 2024-04-29 06:52:45.802969 qg_toolkit-1.0.20/qg_toolkit/tools/qg_solana.py
+-rw-r--r--   0        0        0     2764 2024-04-28 01:55:09.908828 qg_toolkit-1.0.20/qg_toolkit/tools/qg_starknet.py
+-rw-r--r--   0        0        0     3241 2024-04-28 01:55:09.909829 qg_toolkit-1.0.20/qg_toolkit/tools/qproxy.py
+-rw-r--r--   0        0        0     1239 2024-04-29 10:01:18.869266 qg_toolkit-1.0.20/qg_toolkit/tools/random_tool.py
+-rw-r--r--   0        0        0     6068 2024-04-28 01:55:09.909829 qg_toolkit-1.0.20/qg_toolkit/tools/rpc.py
+-rw-r--r--   0        0        0    72707 2024-05-27 09:37:09.168351 qg_toolkit-1.0.20/qg_toolkit/tools/twitter.py
+-rw-r--r--   0        0        0     4182 2024-04-30 01:04:07.617541 qg_toolkit-1.0.20/qg_toolkit/tools/yescaptcha.py
+-rw-r--r--   0        0        0       70 2024-05-27 09:43:22.269934 qg_toolkit-1.0.20/README.md
+-rw-r--r--   0        0        0      133 2024-05-27 09:39:43.317110 qg_toolkit-1.0.20/tea.yaml
+-rw-r--r--   0        0        0     1401 1970-01-01 00:00:00.000000 qg_toolkit-1.0.20/PKG-INFO
```

### Comparing `qg_toolkit-1.0.19/pyproject.toml` & `qg_toolkit-1.0.20/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qg_toolkit"
-version = "1.0.19"
+version = "1.0.20"
 description = "qg_toolkit for Python!"
 authors = ["qg <qg@gmail.com>"]
 readme = "README.md"
 packages = [{include = "qg_toolkit"}]
 include = [{path = "tea.yaml"}]
```

### Comparing `qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_fullpage/geetest_v4.py` & `qg_toolkit-1.0.20/qg_toolkit/geetest_captcha/geetest4_fullpage/geetest_v4.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_fullpage/jiyan.js` & `qg_toolkit-1.0.20/qg_toolkit/geetest_captcha/geetest4_fullpage/jiyan.js`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_fullpage/mian.py` & `qg_toolkit-1.0.20/qg_toolkit/geetest_captcha/geetest4_fullpage/mian.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/gap.py` & `qg_toolkit-1.0.20/qg_toolkit/geetest_captcha/geetest4_slide/gap.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/geetest_slide_v4.py` & `qg_toolkit-1.0.20/qg_toolkit/geetest_captcha/geetest4_slide/geetest_slide_v4.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/img/bg.png` & `qg_toolkit-1.0.20/qg_toolkit/geetest_captcha/geetest4_slide/img/bg.png`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/img/show_image.png` & `qg_toolkit-1.0.20/qg_toolkit/geetest_captcha/geetest4_slide/img/show_image.png`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/img/slide.png` & `qg_toolkit-1.0.20/qg_toolkit/geetest_captcha/geetest4_slide/img/slide.png`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/img/tracks.json` & `qg_toolkit-1.0.20/qg_toolkit/geetest_captcha/geetest4_slide/img/tracks.json`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/jiyan.js` & `qg_toolkit-1.0.20/qg_toolkit/geetest_captcha/geetest4_slide/jiyan.js`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/mian.py` & `qg_toolkit-1.0.20/qg_toolkit/geetest_captcha/geetest4_slide/mian.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/trace.py` & `qg_toolkit-1.0.20/qg_toolkit/geetest_captcha/geetest4_slide/trace.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/qgalxe/galxe.py` & `qg_toolkit-1.0.20/qg_toolkit/qgalxe/galxe.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/qgalxe/GeetestFullPageV4.py` & `qg_toolkit-1.0.20/qg_toolkit/qgalxe/GeetestFullPageV4.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/qgalxe/GeetestSlideV4.py` & `qg_toolkit-1.0.20/qg_toolkit/qgalxe/GeetestSlideV4.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/account_checker.py` & `qg_toolkit-1.0.20/qg_toolkit/qtweepy/examples/account_checker.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/follow_each_other.py` & `qg_toolkit-1.0.20/qg_toolkit/qtweepy/examples/follow_each_other.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/mavia.py` & `qg_toolkit-1.0.20/qg_toolkit/qtweepy/examples/mavia.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/set_2fa.py` & `qg_toolkit-1.0.20/qg_toolkit/qtweepy/examples/set_2fa.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/set_avatars_and_banners.py` & `qg_toolkit-1.0.20/qg_toolkit/qtweepy/examples/set_avatars_and_banners.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/uploading_images.py` & `qg_toolkit-1.0.20/qg_toolkit/qtweepy/examples/uploading_images.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/voter.py` & `qg_toolkit-1.0.20/qg_toolkit/qtweepy/examples/voter.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/xai.py` & `qg_toolkit-1.0.20/qg_toolkit/qtweepy/examples/xai.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/qtweepy/pyproject.toml` & `qg_toolkit-1.0.20/qg_toolkit/qtweepy/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/qtweepy/README.md` & `qg_toolkit-1.0.20/qg_toolkit/qtweepy/README.md`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/__init__.py` & `qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/__init__.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/_capsolver/core/base.py` & `qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/_capsolver/core/base.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/_capsolver/core/config.py` & `qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/_capsolver/core/config.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/_capsolver/core/enum.py` & `qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/_capsolver/core/enum.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/_capsolver/core/serializer.py` & `qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/_capsolver/core/serializer.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/_capsolver/fun_captcha.py` & `qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/_capsolver/fun_captcha.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/account.py` & `qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/account.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/base/session.py` & `qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/base/session.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/client.py` & `qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/client.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/errors.py` & `qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/errors.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/models.py` & `qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/models.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/utils/__init__.py` & `qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/utils/file.py` & `qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/utils/file.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/utils/html.py` & `qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/utils/html.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/utils/other.py` & `qg_toolkit-1.0.20/qg_toolkit/qtweepy/twitter/utils/other.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/tools/cui_qiu_client.py` & `qg_toolkit-1.0.20/qg_toolkit/tools/cui_qiu_client.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/tools/date_util.py` & `qg_toolkit-1.0.20/qg_toolkit/tools/date_util.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/tools/discord.py` & `qg_toolkit-1.0.20/qg_toolkit/tools/discord.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/tools/qg_airdrop.py` & `qg_toolkit-1.0.20/qg_toolkit/tools/qg_airdrop.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/tools/qg_crypto.py` & `qg_toolkit-1.0.20/qg_toolkit/tools/qg_crypto.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/tools/qg_eth.py` & `qg_toolkit-1.0.20/qg_toolkit/tools/qg_eth.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/tools/qg_file.py` & `qg_toolkit-1.0.20/qg_toolkit/tools/qg_file.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/tools/qg_random.py` & `qg_toolkit-1.0.20/qg_toolkit/tools/qg_random.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/tools/qg_solana.py` & `qg_toolkit-1.0.20/qg_toolkit/tools/qg_solana.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/tools/qg_starknet.py` & `qg_toolkit-1.0.20/qg_toolkit/tools/qg_starknet.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/tools/qproxy.py` & `qg_toolkit-1.0.20/qg_toolkit/tools/qproxy.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/tools/random_tool.py` & `qg_toolkit-1.0.20/qg_toolkit/tools/random_tool.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/qg_toolkit/tools/rpc.py` & `qg_toolkit-1.0.20/qg_toolkit/tools/rpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,16 +71,15 @@
     # "avav": "https://rpc.ankr.com/avalanche",
     "avav": "https://avalanche.drpc.org",
     # "avav": "https://avax-pokt.nodies.app/ext/bc/C/rpc",
     "berachain": "https://artio.rpc.berachain.com",
     "kly": "https://public-en-cypress.klaytn.net",
     "blast": "https://sepolia.blast.io",
     "holesky": "https://ethereum-holesky.publicnode.com",
-    "katla": "https://rpc.katla.taiko.xyz",
-    "hekla": "https://rpc.hekla.taiko.xyz"
+    "katla": "https://rpc.katla.taiko.xyz"
 }
 # api接口
 bases = {
     "goerli": "https://api-goerli.etherscan.io/api",
     # "goerli": "https://eth-goerli.blockscout.com/api",
     "sepolia": "https://api-sepolia.etherscan.io/api",
     # "linea": "https://explorer.goerli.linea.build/api",
```

### Comparing `qg_toolkit-1.0.19/qg_toolkit/tools/twitter.py` & `qg_toolkit-1.0.20/qg_toolkit/tools/twitter.py`

 * *Files 0% similar despite different names*

```diff
@@ -770,54 +770,53 @@
         json_data = {
             'variables': {
                 'tweet_text': f'{content}',
                 'reply': {
                     'in_reply_to_tweet_id': f'{tweet_id}',
                     'exclude_reply_user_ids': [],
                 },
-                'batch_compose': 'BatchSubsequent',
                 'dark_request': False,
                 'media': {
                     'media_entities': [],
                     'possibly_sensitive': False,
                 },
                 'semantic_annotation_ids': [],
             },
             'features': {
+                'communities_web_enable_tweet_community_results_fetch': True,
+                'c9s_tweet_anatomy_moderator_badge_enabled': True,
                 'tweetypie_unmention_optimization_enabled': True,
                 'responsive_web_edit_tweet_api_enabled': True,
                 'graphql_is_translatable_rweb_tweet_is_translatable_enabled': True,
                 'view_counts_everywhere_api_enabled': True,
                 'longform_notetweets_consumption_enabled': True,
-                'responsive_web_twitter_article_tweet_consumption_enabled': False,
+                'responsive_web_twitter_article_tweet_consumption_enabled': True,
                 'tweet_awards_web_tipping_enabled': False,
+                'creator_subscriptions_quote_tweet_preview_enabled': False,
                 'longform_notetweets_rich_text_read_enabled': True,
                 'longform_notetweets_inline_media_enabled': True,
+                'articles_preview_enabled': True,
+                'rweb_video_timestamps_enabled': True,
+                'rweb_tipjar_consumption_enabled': True,
                 'responsive_web_graphql_exclude_directive_enabled': True,
                 'verified_phone_label_enabled': False,
                 'freedom_of_speech_not_reach_fetch_enabled': True,
                 'standardized_nudges_misinfo': True,
                 'tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled': True,
-                'responsive_web_media_download_video_enabled': False,
                 'responsive_web_graphql_skip_user_profile_image_extensions_enabled': False,
                 'responsive_web_graphql_timeline_navigation_enabled': True,
                 'responsive_web_enhance_cards_enabled': False,
             },
-            'fieldToggles': {
-                'withArticleRichContentState': False,
-                'withAuxiliaryUserLabels': False,
-            },
-            'queryId': 'SoVnbfCycZ7fERGCwpZkYA',
+            'queryId': '31-6kYrWwW7ZqHmLu2mm9w',
         }
-
         response = self.session.post(
-            'https://twitter.com/i/api/graphql/SoVnbfCycZ7fERGCwpZkYA/CreateTweet',
+            'https://x.com/i/api/graphql/31-6kYrWwW7ZqHmLu2mm9w/CreateTweet',
             json=json_data,
         )
-        if response.status_code == 200:
+        if response.status_code == 200 and "duplicate" not in response.text:
             logger.info(f'【{self.username}】【{self.index}】回复推特成功,报文:{response.text}')
             return f'https://twitter.com/{self.username}/status/{response.json()["data"]["create_tweet"]["tweet_results"]["result"]["rest_id"]}'
         else:
             logger.info(f'【{self.username}】【{self.index}】回复推特失败,报文:{response.text}')
             return None
 
     def retweet(self, tweet_id, tw_info=None):
```

### Comparing `qg_toolkit-1.0.19/qg_toolkit/tools/yescaptcha.py` & `qg_toolkit-1.0.20/qg_toolkit/tools/yescaptcha.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.19/PKG-INFO` & `qg_toolkit-1.0.20/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qg_toolkit
-Version: 1.0.19
+Version: 1.0.20
 Summary: qg_toolkit for Python!
 Author: qg
 Author-email: qg@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -33,10 +33,11 @@
 Requires-Dist: tenacity (>=8,<9)
 Requires-Dist: web3 (>=6.17.2,<7.0.0)
 Requires-Dist: websockets (==11.0.3)
 Requires-Dist: yarl (>=1,<2)
 Description-Content-Type: text/markdown
 
 # QG_TOOLKIT
-
+> poetry build
+> poetry publish
 some tool in Python.
```

