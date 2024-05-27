# Comparing `tmp/cdnmon-0.5.3.tar.gz` & `tmp/cdnmon-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdnmon-0.5.3.tar", max compression
+gzip compressed data, was "cdnmon-0.5.4.tar", max compression
```

## Comparing `cdnmon-0.5.3.tar` & `cdnmon-0.5.4.tar`

### file list

```diff
@@ -1,92 +1,92 @@
--rw-r--r--   0        0        0      636 2024-05-24 10:18:47.731824 cdnmon-0.5.3/README.md
--rw-r--r--   0        0        0      536 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/__init__.py
--rw-r--r--   0        0        0     8327 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/__init__.py
--rw-r--r--   0        0        0      401 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/advancedhosting.py
--rw-r--r--   0        0        0     1814 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/akamai.py
--rw-r--r--   0        0        0    14608 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/alibaba_cdn.py
--rw-r--r--   0        0        0     2523 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/alibaba_dcdn.py
--rw-r--r--   0        0        0     1467 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/alibaba_waf.py
--rw-r--r--   0        0        0      335 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/asia_isp.py
--rw-r--r--   0        0        0      435 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/azion.py
--rw-r--r--   0        0        0     1332 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/baidu.py
--rw-r--r--   0        0        0      919 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/baishan.py
--rw-r--r--   0        0        0      427 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/bunny.py
--rw-r--r--   0        0        0      449 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/cachefly.py
--rw-r--r--   0        0        0      335 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/cdn77.py
--rw-r--r--   0        0        0      312 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/cdnetworks.py
--rw-r--r--   0        0        0      308 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/chinacache.py
--rw-r--r--   0        0        0      365 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/chinanet.py
--rw-r--r--   0        0        0     1869 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/cloudflare.py
--rw-r--r--   0        0        0     1330 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/cloudfront.py
--rw-r--r--   0        0        0     1235 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/ctyun.py
--rw-r--r--   0        0        0      515 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/douyin.py
--rw-r--r--   0        0        0      307 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/edgecast.py
--rw-r--r--   0        0        0      277 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/edgio.py
--rw-r--r--   0        0        0     2765 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/fastly.py
--rw-r--r--   0        0        0      309 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/fastly_edge_compute.py
--rw-r--r--   0        0        0     1190 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/frontdoor.py
--rw-r--r--   0        0        0     1612 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/gcore.py
--rw-r--r--   0        0        0    12746 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/huawei.py
--rw-r--r--   0        0        0      303 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/imperva.py
--rw-r--r--   0        0        0      307 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/incapsula.py
--rw-r--r--   0        0        0     5903 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/jingdong.py
--rw-r--r--   0        0        0      395 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/keycdn.py
--rw-r--r--   0        0        0     1335 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/kingsoft.py
--rw-r--r--   0        0        0      538 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/leaseweb.py
--rw-r--r--   0        0        0      406 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/limelight.py
--rw-r--r--   0        0        0      396 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/netease.py
--rw-r--r--   0        0        0     1193 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/qihoo.py
--rw-r--r--   0        0        0     3222 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/qiniu.py
--rw-r--r--   0        0        0     2088 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/tencent.py
--rw-r--r--   0        0        0       15 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/afx.py
--rw-r--r--   0        0        0       21 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/agile.py
--rw-r--r--   0        0        0       21 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/ananke.py
--rw-r--r--   0        0        0       61 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/aodianyun.py
--rw-r--r--   0        0        0       40 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/arvancloud.py
--rw-r--r--   0        0        0       16 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/att.py
--rw-r--r--   0        0        0      299 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/beluga.py
--rw-r--r--   0        0        0       14 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/cdnify.py
--rw-r--r--   0        0        0       29 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/cdnsun.py
--rw-r--r--   0        0        0      211 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/cdnvideo.py
--rw-r--r--   0        0        0       15 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/cotendo.py
--rw-r--r--   0        0        0       16 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/cube.py
--rw-r--r--   0        0        0       16 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/digitalink.py
--rw-r--r--   0        0        0      202 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/dnion.py
--rw-r--r--   0        0        0      211 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/edgenext.py
--rw-r--r--   0        0        0       20 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/eschoolview.py
--rw-r--r--   0        0        0       20 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/gocache.py
--rw-r--r--   0        0        0     1620 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/google.py
--rw-r--r--   0        0        0       31 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/instartlogic.py
--rw-r--r--   0        0        0       20 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/internap.py
--rw-r--r--   0        0        0       24 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/invisionpower.py
--rw-r--r--   0        0        0       41 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/jiasule.py
--rw-r--r--   0        0        0       21 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/jsdelivr.py
--rw-r--r--   0        0        0      218 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/lumen.py
--rw-r--r--   0        0        0       14 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/manmanyun.py
--rw-r--r--   0        0        0     1438 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/maxcdn.py
--rw-r--r--   0        0        0       20 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/mediacloud.py
--rw-r--r--   0        0        0      272 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/medianova.py
--rw-r--r--   0        0        0       58 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/mirrorimage.py
--rw-r--r--   0        0        0       53 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/netdna.py
--rw-r--r--   0        0        0       57 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/netlify.py
--rw-r--r--   0        0        0       15 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/ngenix.py
--rw-r--r--   0        0        0       30 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/nyiftw.py
--rw-r--r--   0        0        0       38 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/onapp.py
--rw-r--r--   0        0        0       17 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/pagerain.py
--rw-r--r--   0        0        0       17 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/presscdn.py
--rw-r--r--   0        0        0       19 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/qinglanyun.py
--rw-r--r--   0        0        0      127 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/stackpath.py
--rw-r--r--   0        0        0      215 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/tata.py
--rw-r--r--   0        0        0       38 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/thunderbird.py
--rw-r--r--   0        0        0      224 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/todo/verizon.py
--rw-r--r--   0        0        0     1338 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/ucloud.py
--rw-r--r--   0        0        0     1097 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/upyun.py
--rw-r--r--   0        0        0      432 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/volc.py
--rw-r--r--   0        0        0    15868 2024-05-24 10:18:47.735824 cdnmon-0.5.3/cdnmon/model/cdn/wangsu.py
--rw-r--r--   0        0        0      327 2024-05-24 10:18:47.739824 cdnmon-0.5.3/cdnmon/model/cdn/xiaomi.py
--rw-r--r--   0        0        0      691 2024-05-24 10:18:47.739824 cdnmon-0.5.3/cdnmon/util/aws.py
--rw-r--r--   0        0        0     1051 2024-05-24 10:18:47.739824 cdnmon-0.5.3/cdnmon/util/bgpview.py
--rw-r--r--   0        0        0      389 2024-05-24 10:18:47.739824 cdnmon-0.5.3/cdnmon/util/cidr.py
--rw-r--r--   0        0        0      258 2024-05-24 10:18:47.739824 cdnmon-0.5.3/cdnmon/util/db.py
--rw-r--r--   0        0        0      531 2024-05-24 10:18:47.739824 cdnmon-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     1384 1970-01-01 00:00:00.000000 cdnmon-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0      636 2024-05-27 08:23:33.581478 cdnmon-0.5.4/README.md
+-rw-r--r--   0        0        0      536 2024-05-27 08:23:33.581478 cdnmon-0.5.4/cdnmon/__init__.py
+-rw-r--r--   0        0        0     9924 2024-05-27 08:23:33.581478 cdnmon-0.5.4/cdnmon/model/cdn/__init__.py
+-rw-r--r--   0        0        0      401 2024-05-27 08:23:33.581478 cdnmon-0.5.4/cdnmon/model/cdn/advancedhosting.py
+-rw-r--r--   0        0        0     1870 2024-05-27 08:23:33.581478 cdnmon-0.5.4/cdnmon/model/cdn/akamai.py
+-rw-r--r--   0        0        0    14636 2024-05-27 08:23:33.581478 cdnmon-0.5.4/cdnmon/model/cdn/alibaba_cdn.py
+-rw-r--r--   0        0        0     2630 2024-05-27 08:23:33.581478 cdnmon-0.5.4/cdnmon/model/cdn/alibaba_dcdn.py
+-rw-r--r--   0        0        0     1607 2024-05-27 08:23:33.581478 cdnmon-0.5.4/cdnmon/model/cdn/alibaba_waf.py
+-rw-r--r--   0        0        0      335 2024-05-27 08:23:33.581478 cdnmon-0.5.4/cdnmon/model/cdn/asia_isp.py
+-rw-r--r--   0        0        0      435 2024-05-27 08:23:33.581478 cdnmon-0.5.4/cdnmon/model/cdn/azion.py
+-rw-r--r--   0        0        0     1554 2024-05-27 08:23:33.581478 cdnmon-0.5.4/cdnmon/model/cdn/baidu.py
+-rw-r--r--   0        0        0      919 2024-05-27 08:23:33.581478 cdnmon-0.5.4/cdnmon/model/cdn/baishan.py
+-rw-r--r--   0        0        0      427 2024-05-27 08:23:33.581478 cdnmon-0.5.4/cdnmon/model/cdn/bunny.py
+-rw-r--r--   0        0        0      449 2024-05-27 08:23:33.581478 cdnmon-0.5.4/cdnmon/model/cdn/cachefly.py
+-rw-r--r--   0        0        0      335 2024-05-27 08:23:33.581478 cdnmon-0.5.4/cdnmon/model/cdn/cdn77.py
+-rw-r--r--   0        0        0      312 2024-05-27 08:23:33.581478 cdnmon-0.5.4/cdnmon/model/cdn/cdnetworks.py
+-rw-r--r--   0        0        0      308 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/chinacache.py
+-rw-r--r--   0        0        0      365 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/chinanet.py
+-rw-r--r--   0        0        0     1869 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/cloudflare.py
+-rw-r--r--   0        0        0     1330 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/cloudfront.py
+-rw-r--r--   0        0        0     1235 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/ctyun.py
+-rw-r--r--   0        0        0      515 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/douyin.py
+-rw-r--r--   0        0        0      307 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/edgecast.py
+-rw-r--r--   0        0        0      277 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/edgio.py
+-rw-r--r--   0        0        0     2765 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/fastly.py
+-rw-r--r--   0        0        0      309 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/fastly_edge_compute.py
+-rw-r--r--   0        0        0     1190 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/frontdoor.py
+-rw-r--r--   0        0        0     1627 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/gcore.py
+-rw-r--r--   0        0        0    12774 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/huawei.py
+-rw-r--r--   0        0        0      303 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/imperva.py
+-rw-r--r--   0        0        0      307 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/incapsula.py
+-rw-r--r--   0        0        0     5903 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/jingdong.py
+-rw-r--r--   0        0        0      395 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/keycdn.py
+-rw-r--r--   0        0        0     1363 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/kingsoft.py
+-rw-r--r--   0        0        0      538 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/leaseweb.py
+-rw-r--r--   0        0        0      406 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/limelight.py
+-rw-r--r--   0        0        0      396 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/netease.py
+-rw-r--r--   0        0        0     1193 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/qihoo.py
+-rw-r--r--   0        0        0     3222 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/qiniu.py
+-rw-r--r--   0        0        0     2233 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/tencent.py
+-rw-r--r--   0        0        0       15 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/afx.py
+-rw-r--r--   0        0        0       21 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/agile.py
+-rw-r--r--   0        0        0       21 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/ananke.py
+-rw-r--r--   0        0        0       61 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/aodianyun.py
+-rw-r--r--   0        0        0       40 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/arvancloud.py
+-rw-r--r--   0        0        0       16 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/att.py
+-rw-r--r--   0        0        0      299 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/beluga.py
+-rw-r--r--   0        0        0       14 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/cdnify.py
+-rw-r--r--   0        0        0       29 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/cdnsun.py
+-rw-r--r--   0        0        0      211 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/cdnvideo.py
+-rw-r--r--   0        0        0       15 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/cotendo.py
+-rw-r--r--   0        0        0       16 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/cube.py
+-rw-r--r--   0        0        0       16 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/digitalink.py
+-rw-r--r--   0        0        0      202 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/dnion.py
+-rw-r--r--   0        0        0      211 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/edgenext.py
+-rw-r--r--   0        0        0       20 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/eschoolview.py
+-rw-r--r--   0        0        0       20 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/gocache.py
+-rw-r--r--   0        0        0     1620 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/google.py
+-rw-r--r--   0        0        0       31 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/instartlogic.py
+-rw-r--r--   0        0        0       20 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/internap.py
+-rw-r--r--   0        0        0       24 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/invisionpower.py
+-rw-r--r--   0        0        0       41 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/jiasule.py
+-rw-r--r--   0        0        0       21 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/jsdelivr.py
+-rw-r--r--   0        0        0      218 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/lumen.py
+-rw-r--r--   0        0        0       14 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/manmanyun.py
+-rw-r--r--   0        0        0     1438 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/maxcdn.py
+-rw-r--r--   0        0        0       20 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/mediacloud.py
+-rw-r--r--   0        0        0      272 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/medianova.py
+-rw-r--r--   0        0        0       58 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/mirrorimage.py
+-rw-r--r--   0        0        0       53 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/netdna.py
+-rw-r--r--   0        0        0       57 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/netlify.py
+-rw-r--r--   0        0        0       15 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/ngenix.py
+-rw-r--r--   0        0        0       30 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/nyiftw.py
+-rw-r--r--   0        0        0       38 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/onapp.py
+-rw-r--r--   0        0        0       17 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/pagerain.py
+-rw-r--r--   0        0        0       17 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/presscdn.py
+-rw-r--r--   0        0        0       19 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/qinglanyun.py
+-rw-r--r--   0        0        0      127 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/stackpath.py
+-rw-r--r--   0        0        0      215 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/tata.py
+-rw-r--r--   0        0        0       38 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/thunderbird.py
+-rw-r--r--   0        0        0      224 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/todo/verizon.py
+-rw-r--r--   0        0        0     1366 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/ucloud.py
+-rw-r--r--   0        0        0     1198 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/upyun.py
+-rw-r--r--   0        0        0      432 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/volc.py
+-rw-r--r--   0        0        0    15882 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/wangsu.py
+-rw-r--r--   0        0        0      327 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/model/cdn/xiaomi.py
+-rw-r--r--   0        0        0      691 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/util/aws.py
+-rw-r--r--   0        0        0     1051 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/util/bgpview.py
+-rw-r--r--   0        0        0      389 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/util/cidr.py
+-rw-r--r--   0        0        0      258 2024-05-27 08:23:33.585478 cdnmon-0.5.4/cdnmon/util/db.py
+-rw-r--r--   0        0        0      531 2024-05-27 08:23:33.585478 cdnmon-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     1384 1970-01-01 00:00:00.000000 cdnmon-0.5.4/PKG-INFO
```

### Comparing `cdnmon-0.5.3/README.md` & `cdnmon-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.3/cdnmon/__init__.py` & `cdnmon-0.5.4/cdnmon/__init__.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.3/cdnmon/model/cdn/__init__.py` & `cdnmon-0.5.4/cdnmon/model/cdn/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -72,33 +72,82 @@
         for query_term in self.query_term_list:
             data = self.bgpview_client.search(query_term)
             for item in data["data"]["ipv6_prefixes"]:
                 ipv6_networks.append(str(ipaddress.IPv6Network(item["prefix"], strict=False)))
         return deduplicate_networks(ipv6_networks, filter_version=6)
 
 
+class CNAMEType(Enum):
+    """
+    e.g. For the following DNS result, the CNAMEType defines as follows
+
+        edgekey.net -> ROOT
+        akadns.net  -> INTERMEDIATE
+        tl88.net    -> LEAF (which means it directly points to an IP address)
+
+    $ dig www.apple.com
+
+    ; <<>> DiG 9.18.24-0ubuntu5-Ubuntu <<>> www.apple.com
+    ;; global options: +cmd
+    ;; Got answer:
+    ;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 24731
+    ;; flags: qr rd ra; QUERY: 1, ANSWER: 4, AUTHORITY: 0, ADDITIONAL: 1
+
+    ;; OPT PSEUDOSECTION:
+    ; EDNS: version: 0, flags:; udp: 65494
+    ;; QUESTION SECTION:
+    ;www.apple.com.                 IN      A
+
+    ;; ANSWER SECTION:
+    www.apple.com.          0       IN      CNAME   www.apple.com.edgekey.net.
+    www.apple.com.edgekey.net. 5050 IN      CNAME   www.apple.com.edgekey.net.globalredir.akadns.net.
+    www.apple.com.edgekey.net.globalredir.akadns.net. 0 IN CNAME e6858.e19.s.tl88.net.
+    e6858.e19.s.tl88.net.   0       IN      A       106.4.158.58
+
+    ;; Query time: 6 msec
+    ;; SERVER: 127.0.0.53#53(127.0.0.53) (UDP)
+    ;; WHEN: Mon May 27 15:48:00 CST 2024
+    ;; MSG SIZE  rcvd: 187
+    """
+
+    UNKNOWN = "unknown"
+    ROOT = "root"
+    INTERMEDIATE = "intermediate"
+    LEAF = "leaf"
+
+    def __str__(self) -> str:
+        return self.value
+
+
 @dataclass
 class CNAMEPattern:
     suffix: str = field(default_factory=str)
     pattern: str = field(default_factory=str)
     source: str = field(default_factory=str)
+    is_root: bool | None = field(default=None)
+    is_leaf: bool | None = field(default=None)
 
     def __str__(self) -> str:
         return self.suffix
 
     def __repr__(self) -> str:
         return self.suffix
 
     def marshal(self) -> dict:
-        return {
+        result = {
             "suffix": self.suffix,
             "pattern": self.pattern,
             "source": self.source,
             "subscribers": self.subscribers(),
         }
+        if self.is_root is not None:
+            result["is_root"] = self.is_root
+        if self.is_leaf is not None:
+            result["is_leaf"] = self.is_leaf
+        return result
 
     def subscribers(self) -> List[str]:
         if not os.getenv("MONGODB_URI"):
             logger.warning("MONGODB_URI is not set")
             return []
 
         suffix = self.suffix if self.suffix.endswith(".") else self.suffix + "."
```

### Comparing `cdnmon-0.5.3/cdnmon/model/cdn/akamai.py` & `cdnmon-0.5.4/cdnmon/model/cdn/akamai.py`

 * *Files 18% similar despite different names*

```diff
@@ -34,14 +34,14 @@
 CDN = CommonCDN(
     name="akamai",
     asn_patterns=["akamai"],
     cname_suffixes=[
         CNAMEPattern(suffix="-v1.akamaized.net", pattern=r"${domain}-v1.akamaized.net"),
         CNAMEPattern(suffix="-v1.edgekey.net", pattern=r"${domain}-v1.edgekey.net"),
         CNAMEPattern(suffix=".akadns.net"),
-        CNAMEPattern(suffix=".akamai.net"),
-        CNAMEPattern(suffix=".akamaiedge.net"),
-        CNAMEPattern(suffix=".edgekey.net", pattern=r"${domain}.edgekey.net"),
-        CNAMEPattern(suffix=".edgesuite.net", pattern=r"${domain}.edgesuite.net"),
+        CNAMEPattern(suffix=".akamai.net", is_leaf=True),
+        CNAMEPattern(suffix=".akamaiedge.net", is_leaf=True),
+        CNAMEPattern(suffix=".edgekey.net", pattern=r"${domain}.edgekey.net", is_root=True),
+        CNAMEPattern(suffix=".edgesuite.net", pattern=r"${domain}.edgesuite.net", is_root=True),
     ],
     cidr=AkamaiCIDR(),
 )
```

### Comparing `cdnmon-0.5.3/cdnmon/model/cdn/alibaba_cdn.py` & `cdnmon-0.5.4/cdnmon/model/cdn/alibaba_cdn.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from cdnmon.model.cdn import HTTPOwnershipVerification
 from cdnmon.model.cdn import OwnershipVerification
 
 CDN = CommonCDN(
     name="alibaba-cdn",
     asn_patterns=["alibaba", "taobao", "alicloud"],
     cname_suffixes=[
-        CNAMEPattern(suffix=".cdngslb.com", pattern=r"${domain}.cdngslb.com"),
+        CNAMEPattern(suffix=".cdngslb.com", pattern=r"${domain}.cdngslb.com", is_root=True, is_leaf=True),
         CNAMEPattern(suffix=".queniuaa.com", pattern=r"${domain}.queniuaa.com"),
         CNAMEPattern(suffix=".queniuab.com", pattern=r"${domain}.queniuab.com"),
         CNAMEPattern(suffix=".queniuai.com", pattern=r"${domain}.queniuai.com"),
         CNAMEPattern(suffix=".queniuak.com", pattern=r"${domain}.queniuak.com"),
         CNAMEPattern(suffix=".queniual.com", pattern=r"${domain}.queniual.com"),
         CNAMEPattern(suffix=".queniuam.com", pattern=r"${domain}.queniuam.com"),
         CNAMEPattern(suffix=".queniubd.com", pattern=r"${domain}.queniubd.com"),
```

### Comparing `cdnmon-0.5.3/cdnmon/model/cdn/alibaba_dcdn.py` & `cdnmon-0.5.4/cdnmon/model/cdn/alibaba_dcdn.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from cdnmon.model.cdn import HTTPOwnershipVerification
 from cdnmon.model.cdn import OwnershipVerification
 
 CDN = CommonCDN(
     name="alibaba-dcdn",
     asn_patterns=["alibaba", "taobao", "alicloud"],
     cname_suffixes=[
+        CNAMEPattern(suffix=".cdngslb.com", pattern=r"${domain}.cdngslb.com", is_root=True, is_leaf=True),
         CNAMEPattern(suffix=".m.alikunlun.com", pattern=r"${domain}.m.alikunlun.com"),
         CNAMEPattern(suffix=".m.alikunlun.net", pattern=r"${domain}.m.alikunlun.net"),
         CNAMEPattern(suffix=".w.kunlunaq.com", pattern=r"${domain}.w.kunlunaq.com"),
         CNAMEPattern(suffix=".w.kunlunar.com", pattern=r"${domain}.w.kunlunar.com"),
         CNAMEPattern(suffix=".w.kunlunca.com", pattern=r"${domain}.w.kunlunca.com"),
         CNAMEPattern(suffix=".w.kunluncan.com", pattern=r"${domain}.w.kunluncan.com"),
         CNAMEPattern(suffix=".w.kunlunea.com", pattern=r"${domain}.w.kunlunea.com"),
```

### Comparing `cdnmon-0.5.3/cdnmon/model/cdn/alibaba_waf.py` & `cdnmon-0.5.4/cdnmon/model/cdn/ctyun.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,29 +3,27 @@
 from cdnmon.model.cdn import CommonCDN
 from cdnmon.model.cdn import DomainOwnershipVerficationStatus
 from cdnmon.model.cdn import DomainOwnershipVerification
 from cdnmon.model.cdn import HTTPOwnershipVerification
 from cdnmon.model.cdn import OwnershipVerification
 
 CDN = CommonCDN(
-    name="alibaba-waf",
-    asn_patterns=["alibaba", "taobao", "alicloud"],
+    name="ctyun",
+    asn_patterns=["ctyun", "chinanet"],
     cname_suffixes=[
-        CNAMEPattern(suffix=".yundunwaf1.com", pattern=r"${random}.yundunwaf1.com"),
-        CNAMEPattern(suffix=".yundunwaf2.com", pattern=r"${random}.yundunwaf2.com"),
-        CNAMEPattern(suffix=".yundunwaf3.com", pattern=r"${random}.yundunwaf3.com"),
-        CNAMEPattern(suffix=".yundunwaf4.com", pattern=r"${random}.yundunwaf4.com"),
-        CNAMEPattern(suffix=".yundunwaf5.com", pattern=r"${random}.yundunwaf5.com"),
+        CNAMEPattern(suffix=".ctadns.cn", pattern=r"${domain}.ctadns.cn"),
+        CNAMEPattern(suffix=".ctacdn.cn", pattern=r"${domain}.ctacdn.cn"),
+        CNAMEPattern(suffix=".ctlcdn.cn", pattern=r"${domain}.ctlcdn.cn"),
     ],
-    cidr=BGPViewCIDR(["alibaba", "taobao", "alicloud"]),
+    cidr=BGPViewCIDR(["ctyun", "chinanet"]),
     frontend_ownership_verification=OwnershipVerification(
         txt=DomainOwnershipVerification(
             status=DomainOwnershipVerficationStatus.REQUIRED,
-            prefix="wafdnscheck",
-            pattern=r"[0-9]{16}-[0-9a-z]{32}",
-        )
+            prefix="dnsverify",
+            pattern=r"[0-9]{14}[0-9a-f]{50}",
+        ),
     ),
     backend_ownership_verification=OwnershipVerification(
         txt=DomainOwnershipVerification(status=DomainOwnershipVerficationStatus.NOT_REQUIRED),
         http=HTTPOwnershipVerification(status=DomainOwnershipVerficationStatus.NOT_REQUIRED),
     ),
 )
```

### Comparing `cdnmon-0.5.3/cdnmon/model/cdn/baidu.py` & `cdnmon-0.5.4/cdnmon/model/cdn/kingsoft.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,28 +3,31 @@
 from cdnmon.model.cdn import CommonCDN
 from cdnmon.model.cdn import DomainOwnershipVerficationStatus
 from cdnmon.model.cdn import DomainOwnershipVerification
 from cdnmon.model.cdn import HTTPOwnershipVerification
 from cdnmon.model.cdn import OwnershipVerification
 
 CDN = CommonCDN(
-    name="baidu",
-    asn_patterns=["baidu"],
+    name="kingsoft",
+    asn_patterns=["kingsoft", "ksyun"],
     cname_suffixes=[
-        CNAMEPattern(suffix=".a.bdydns.com", pattern=r"${domain}.a.bdydns.com"),
-        CNAMEPattern(suffix=".yjs-cdn.com", pattern=r"${domain}.yjs-cdn.com"),
-        CNAMEPattern(suffix=".yunjiasu-cdn.net", pattern=r"${domain}.yunjiasu-cdn.net"),
+        CNAMEPattern(suffix=".download.ks-cdn.com", pattern=r"${domain}.download.ks-cdn.com", is_root=True),
+        CNAMEPattern(suffix=".ksyuncdn.com", is_leaf=True),
     ],
-    cidr=BGPViewCIDR(["baidu"]),
+    cidr=BGPViewCIDR(["kingsoft", "ksyun"]),
     frontend_ownership_verification=OwnershipVerification(
         txt=DomainOwnershipVerification(
             status=DomainOwnershipVerficationStatus.REQUIRED,
-            prefix="bdy-verify",
-            pattern=r"[0-9a-f]{8}-[0-9a-f]{8}",
+            prefix="ksy-cdnauth",
+            pattern=r"[0-9a-f]{32}",
+        ),
+        http=HTTPOwnershipVerification(
+            status=DomainOwnershipVerficationStatus.REQUIRED,
+            path="/ksy-cdnauth.html",
+            pattern=r"[0-9a-f]{32}",
         ),
-        http=HTTPOwnershipVerification(status=DomainOwnershipVerficationStatus.NOT_REQUIRED),
     ),
     backend_ownership_verification=OwnershipVerification(
         txt=DomainOwnershipVerification(status=DomainOwnershipVerficationStatus.NOT_REQUIRED),
         http=HTTPOwnershipVerification(status=DomainOwnershipVerficationStatus.NOT_REQUIRED),
     ),
 )
```

### Comparing `cdnmon-0.5.3/cdnmon/model/cdn/baishan.py` & `cdnmon-0.5.4/cdnmon/model/cdn/baishan.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.3/cdnmon/model/cdn/cloudflare.py` & `cdnmon-0.5.4/cdnmon/model/cdn/cloudflare.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.3/cdnmon/model/cdn/cloudfront.py` & `cdnmon-0.5.4/cdnmon/model/cdn/cloudfront.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.3/cdnmon/model/cdn/ctyun.py` & `cdnmon-0.5.4/cdnmon/model/cdn/upyun.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,27 +3,26 @@
 from cdnmon.model.cdn import CommonCDN
 from cdnmon.model.cdn import DomainOwnershipVerficationStatus
 from cdnmon.model.cdn import DomainOwnershipVerification
 from cdnmon.model.cdn import HTTPOwnershipVerification
 from cdnmon.model.cdn import OwnershipVerification
 
 CDN = CommonCDN(
-    name="ctyun",
-    asn_patterns=["ctyun", "chinanet"],
+    name="upyun",
+    asn_patterns=["youpai", "upyun"],
     cname_suffixes=[
-        CNAMEPattern(suffix=".ctadns.cn", pattern=r"${domain}.ctadns.cn"),
-        CNAMEPattern(suffix=".ctacdn.cn", pattern=r"${domain}.ctacdn.cn"),
-        CNAMEPattern(suffix=".ctlcdn.cn", pattern=r"${domain}.ctlcdn.cn"),
+        CNAMEPattern(suffix=".b0.aicdn.com", pattern=r"[0-9a-f]{12}.b0.aicdn.com", is_root=True),
+        CNAMEPattern(suffix="nm.aicdn.com", pattern=r"nm.aicdn.com", is_leaf=True),
     ],
-    cidr=BGPViewCIDR(["ctyun", "chinanet"]),
+    cidr=BGPViewCIDR(query_term_list=["youpai", "upyun"]),
     frontend_ownership_verification=OwnershipVerification(
         txt=DomainOwnershipVerification(
             status=DomainOwnershipVerficationStatus.REQUIRED,
-            prefix="dnsverify",
-            pattern=r"[0-9]{14}[0-9a-f]{50}",
+            prefix="upyun-verify",
+            pattern=r"[0-9a-f]{32}",
         ),
     ),
     backend_ownership_verification=OwnershipVerification(
         txt=DomainOwnershipVerification(status=DomainOwnershipVerficationStatus.NOT_REQUIRED),
         http=HTTPOwnershipVerification(status=DomainOwnershipVerficationStatus.NOT_REQUIRED),
     ),
 )
```

### Comparing `cdnmon-0.5.3/cdnmon/model/cdn/douyin.py` & `cdnmon-0.5.4/cdnmon/model/cdn/douyin.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.3/cdnmon/model/cdn/fastly.py` & `cdnmon-0.5.4/cdnmon/model/cdn/fastly.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.3/cdnmon/model/cdn/frontdoor.py` & `cdnmon-0.5.4/cdnmon/model/cdn/frontdoor.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.3/cdnmon/model/cdn/gcore.py` & `cdnmon-0.5.4/cdnmon/model/cdn/gcore.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,10 +38,12 @@
             "ipv6_prefixes": deduplicate_networks(ipv6_networks, filter_version=6),
         }
 
 
 CDN = CommonCDN(
     name="gcore",
     asn_patterns=["gcore"],
-    cname_suffixes=[CNAMEPattern(suffix=".gcdn.co", source="https://www.netify.ai/resources/domains/gcdn.co")],
+    cname_suffixes=[
+        CNAMEPattern(suffix=".gcdn.co", source="https://www.netify.ai/resources/domains/gcdn.co"),
+    ],
     cidr=GCoreCIDR(),
 )
```

### Comparing `cdnmon-0.5.3/cdnmon/model/cdn/huawei.py` & `cdnmon-0.5.4/cdnmon/model/cdn/huawei.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,27 +37,27 @@
         CNAMEPattern(suffix=".cdnhwcatq08.com", pattern=r"${domain}.[0-9a-f]{8}.cdnhwcatq08.com"),
         CNAMEPattern(suffix=".cdnhwcbie120.cn", pattern=r"${domain}.[0-9a-f]{8}.cdnhwcbie120.cn"),
         CNAMEPattern(suffix=".cdnhwcbni108.com", pattern=r"${domain}.[0-9a-f]{8}.cdnhwcbni108.com"),
         CNAMEPattern(suffix=".cdnhwcbqs106.com", pattern=r"${domain}.[0-9a-f]{8}.cdnhwcbqs106.com"),
         CNAMEPattern(suffix=".cdnhwcbvo20.cn", pattern=r"${domain}.[0-9a-f]{8}.cdnhwcbvo20.cn"),
         CNAMEPattern(suffix=".cdnhwcbzj102.com", pattern=r"${domain}.[0-9a-f]{8}.cdnhwcbzj102.com"),
         CNAMEPattern(suffix=".cdnhwcchh18.com", pattern=r"${domain}.[0-9a-f]{8}.cdnhwcchh18.com"),
-        CNAMEPattern(suffix=".cdnhwccmz121.com", pattern=r"${domain}.[0-9a-f]{8}.cdnhwccmz121.com"),
+        CNAMEPattern(suffix=".cdnhwccmz121.com", pattern=r"${domain}.[0-9a-f]{8}.cdnhwccmz121.com", is_leaf=True),
         CNAMEPattern(suffix=".cdnhwccvo19.cn", pattern=r"${domain}.[0-9a-f]{8}.cdnhwccvo19.cn"),
         CNAMEPattern(suffix=".cdnhwcdkd21.cn", pattern=r"${domain}.[0-9a-f]{8}.cdnhwcdkd21.cn"),
         CNAMEPattern(suffix=".cdnhwcdvg22.cn", pattern=r"${domain}.[0-9a-f]{8}.cdnhwcdvg22.cn"),
         CNAMEPattern(suffix=".cdnhwcead111.com", pattern=r"${domain}.[0-9a-f]{8}.cdnhwcead111.com"),
         CNAMEPattern(suffix=".cdnhwcedi10.com", pattern=r"${domain}.[0-9a-f]{8}.cdnhwcedi10.com"),
         CNAMEPattern(suffix=".cdnhwcedt124.com", pattern=r"${domain}.[0-9a-f]{8}.cdnhwcedt124.com"),
         CNAMEPattern(suffix=".cdnhwceft18.cn", pattern=r"${domain}.[0-9a-f]{8}.cdnhwceft18.cn"),
         CNAMEPattern(suffix=".cdnhwceod109.cn", pattern=r"${domain}.[0-9a-f]{8}.cdnhwceod109.cn"),
         CNAMEPattern(suffix=".cdnhwcfzp15.cn", pattern=r"${domain}.[0-9a-f]{8}.cdnhwcfzp15.cn"),
         CNAMEPattern(suffix=".cdnhwcggk22.com", pattern=r"${domain}.[0-9a-f]{8}.cdnhwcggk22.com"),
         CNAMEPattern(suffix=".cdnhwcgnc118.com", pattern=r"${domain}.[0-9a-f]{8}.cdnhwcgnc118.com"),
-        CNAMEPattern(suffix=".cdnhwcgqa21.com", pattern=r"${domain}.[0-9a-f]{8}.cdnhwcgqa21.com"),
+        CNAMEPattern(suffix=".cdnhwcgqa21.com", pattern=r"${domain}.[0-9a-f]{8}.cdnhwcgqa21.com", is_root=True),
         CNAMEPattern(suffix=".cdnhwcgqs21.com", pattern=r"${domain}.[0-9a-f]{8}.cdnhwcgqs21.com"),
         CNAMEPattern(suffix=".cdnhwcgrb01.cn", pattern=r"${domain}.[0-9a-f]{8}.cdnhwcgrb01.cn"),
         CNAMEPattern(suffix=".cdnhwcgvs16.cn", pattern=r"${domain}.[0-9a-f]{8}.cdnhwcgvs16.cn"),
         CNAMEPattern(suffix=".cdnhwchcg02.com", pattern=r"${domain}.[0-9a-f]{8}.cdnhwchcg02.com"),
         CNAMEPattern(suffix=".cdnhwcibv122.com", pattern=r"${domain}.[0-9a-f]{8}.cdnhwcibv122.com"),
         CNAMEPattern(suffix=".cdnhwcick110.com", pattern=r"${domain}.[0-9a-f]{8}.cdnhwcick110.com"),
         CNAMEPattern(suffix=".cdnhwcidu117.cn", pattern=r"${domain}.[0-9a-f]{8}.cdnhwcidu117.cn"),
```

### Comparing `cdnmon-0.5.3/cdnmon/model/cdn/jingdong.py` & `cdnmon-0.5.4/cdnmon/model/cdn/jingdong.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.3/cdnmon/model/cdn/kingsoft.py` & `cdnmon-0.5.4/cdnmon/model/cdn/alibaba_waf.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,31 +3,29 @@
 from cdnmon.model.cdn import CommonCDN
 from cdnmon.model.cdn import DomainOwnershipVerficationStatus
 from cdnmon.model.cdn import DomainOwnershipVerification
 from cdnmon.model.cdn import HTTPOwnershipVerification
 from cdnmon.model.cdn import OwnershipVerification
 
 CDN = CommonCDN(
-    name="kingsoft",
-    asn_patterns=["kingsoft", "ksyun"],
+    name="alibaba-waf",
+    asn_patterns=["alibaba", "taobao", "alicloud"],
     cname_suffixes=[
-        CNAMEPattern(suffix=".download.ks-cdn.com", pattern=r"${domain}.download.ks-cdn.com"),
-        CNAMEPattern(suffix=".ksyuncdn.com"),
+        CNAMEPattern(suffix=".yundunwaf1.com", pattern=r"${random}.yundunwaf1.com", is_root=True, is_leaf=True),
+        CNAMEPattern(suffix=".yundunwaf2.com", pattern=r"${random}.yundunwaf2.com", is_root=True, is_leaf=True),
+        CNAMEPattern(suffix=".yundunwaf3.com", pattern=r"${random}.yundunwaf3.com", is_root=True, is_leaf=True),
+        CNAMEPattern(suffix=".yundunwaf4.com", pattern=r"${random}.yundunwaf4.com", is_root=True, is_leaf=True),
+        CNAMEPattern(suffix=".yundunwaf5.com", pattern=r"${random}.yundunwaf5.com", is_root=True, is_leaf=True),
     ],
-    cidr=BGPViewCIDR(["kingsoft", "ksyun"]),
+    cidr=BGPViewCIDR(["alibaba", "taobao", "alicloud"]),
     frontend_ownership_verification=OwnershipVerification(
         txt=DomainOwnershipVerification(
             status=DomainOwnershipVerficationStatus.REQUIRED,
-            prefix="ksy-cdnauth",
-            pattern=r"[0-9a-f]{32}",
-        ),
-        http=HTTPOwnershipVerification(
-            status=DomainOwnershipVerficationStatus.REQUIRED,
-            path="/ksy-cdnauth.html",
-            pattern=r"[0-9a-f]{32}",
-        ),
+            prefix="wafdnscheck",
+            pattern=r"[0-9]{16}-[0-9a-z]{32}",
+        )
     ),
     backend_ownership_verification=OwnershipVerification(
         txt=DomainOwnershipVerification(status=DomainOwnershipVerficationStatus.NOT_REQUIRED),
         http=HTTPOwnershipVerification(status=DomainOwnershipVerficationStatus.NOT_REQUIRED),
     ),
 )
```

### Comparing `cdnmon-0.5.3/cdnmon/model/cdn/leaseweb.py` & `cdnmon-0.5.4/cdnmon/model/cdn/leaseweb.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.3/cdnmon/model/cdn/qihoo.py` & `cdnmon-0.5.4/cdnmon/model/cdn/qihoo.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.3/cdnmon/model/cdn/qiniu.py` & `cdnmon-0.5.4/cdnmon/model/cdn/qiniu.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.3/cdnmon/model/cdn/tencent.py` & `cdnmon-0.5.4/cdnmon/model/cdn/tencent.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,26 +7,27 @@
 from cdnmon.model.cdn import OwnershipVerification
 
 CDN = CommonCDN(
     name="tencent",
     asn_patterns=["tencent"],
     cname_suffixes=[
         CNAMEPattern(suffix=".dsa.dnsv1.com", pattern=r"${domain}.dsa.dnsv1.com"),
-        CNAMEPattern(suffix=".dsa.dnsv1.com.cn", pattern=r"${domain}.dsa.dnsv1.com.cn"),
+        CNAMEPattern(suffix=".dsa.dnsv1.com.cn", pattern=r"${domain}.dsa.dnsv1.com.cn", is_root=True),
         CNAMEPattern(suffix=".cdn.dnsv1.com", pattern=r"${domain}.cdn.dnsv1.com"),
-        CNAMEPattern(suffix=".cdn.dnsv1.com.cn", pattern=r"${domain}.cdn.dnsv1.com.cn"),
+        CNAMEPattern(suffix=".cdn.dnsv1.com.cn", pattern=r"${domain}.cdn.dnsv1.com.cn", is_root=True),
         CNAMEPattern(suffix=".eo.dnse0.com", pattern=r"${domain}.eo.dnse0.com"),
         CNAMEPattern(suffix=".eo.dnse1.com", pattern=r"${domain}.eo.dnse1.com"),
         CNAMEPattern(suffix=".eo.dnse2.com", pattern=r"${domain}.eo.dnse2.com"),
         CNAMEPattern(suffix=".eo.dnse3.com", pattern=r"${domain}.eo.dnse3.com"),
         CNAMEPattern(suffix=".eo.dnse4.com", pattern=r"${domain}.eo.dnse4.com"),
         CNAMEPattern(suffix=".eo.dnse5.com", pattern=r"${domain}.eo.dnse5.com"),
         CNAMEPattern(suffix=".cdn.qcloudcdn.cn", pattern=r"${domain}.cdn.qcloudcdn.cn"),
         CNAMEPattern(suffix=".txlivecdn.com", pattern=r"${domain}.txlivecdn.com"),
         CNAMEPattern(suffix=".ovscdns.com", pattern=r"${domain}.ovscdns.com"),
+        CNAMEPattern(suffix=".slt-dk.sched.tdnsv8.com", pattern=r"${random}.slt-dk.sched.tdnsv8.com", is_leaf=True),
     ],
     cidr=BGPViewCIDR(query_term_list=["tencent"]),
     frontend_ownership_verification=OwnershipVerification(
         txt=DomainOwnershipVerification(
             status=DomainOwnershipVerficationStatus.REQUIRED,
             prefix="_cdnauth",
             pattern=r"[0-9]{14}[0-9a-f]{32}",
```

### Comparing `cdnmon-0.5.3/cdnmon/model/cdn/todo/google.py` & `cdnmon-0.5.4/cdnmon/model/cdn/todo/google.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.3/cdnmon/model/cdn/todo/maxcdn.py` & `cdnmon-0.5.4/cdnmon/model/cdn/todo/maxcdn.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.3/cdnmon/model/cdn/ucloud.py` & `cdnmon-0.5.4/cdnmon/model/cdn/ucloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from cdnmon.model.cdn import HTTPOwnershipVerification
 from cdnmon.model.cdn import OwnershipVerification
 
 CDN = CommonCDN(
     name="ucloud",
     asn_patterns=["ucloud"],
     cname_suffixes=[
-        CNAMEPattern(suffix=".ucloud.com.cn", pattern=r"${domain}.ucloud.com.cn"),
+        CNAMEPattern(suffix=".ucloud.com.cn", pattern=r"${domain}.ucloud.com.cn", is_root=True),
         CNAMEPattern(suffix=".ucloudnaming.cn", pattern=r"${domain}.ucloudnaming.cn"),
         CNAMEPattern(suffix=".ucloudnaming.info", pattern=r"${domain}.ucloudnaming.info"),
-        CNAMEPattern(suffix=".ugslb.net", pattern=r"${domain}.ugslb.net"),
+        CNAMEPattern(suffix=".ugslb.net", pattern=r"${domain}.ugslb.net", is_leaf=True),
     ],
     cidr=BGPViewCIDR(query_term_list=["ucloud"]),
     frontend_ownership_verification=OwnershipVerification(
         txt=DomainOwnershipVerification(status=DomainOwnershipVerficationStatus.NOT_REQUIRED),
         http=HTTPOwnershipVerification(status=DomainOwnershipVerficationStatus.NOT_REQUIRED),
     ),
     backend_ownership_verification=OwnershipVerification(
```

### Comparing `cdnmon-0.5.3/cdnmon/model/cdn/upyun.py` & `cdnmon-0.5.4/cdnmon/model/cdn/baidu.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,25 +3,30 @@
 from cdnmon.model.cdn import CommonCDN
 from cdnmon.model.cdn import DomainOwnershipVerficationStatus
 from cdnmon.model.cdn import DomainOwnershipVerification
 from cdnmon.model.cdn import HTTPOwnershipVerification
 from cdnmon.model.cdn import OwnershipVerification
 
 CDN = CommonCDN(
-    name="upyun",
-    asn_patterns=["youpai", "upyun"],
+    name="baidu",
+    asn_patterns=["baidu"],
     cname_suffixes=[
-        CNAMEPattern(suffix=".aicdn.com", pattern=r"[0-9a-f]{12}.b0.aicdn.com"),
+        CNAMEPattern(suffix=".a.bdydns.com", pattern=r"${domain}.a.bdydns.com", is_root=True),
+        CNAMEPattern(suffix=".yjs-cdn.com", pattern=r"${domain}.yjs-cdn.com"),
+        CNAMEPattern(suffix=".yunjiasu-cdn.net", pattern=r"${domain}.yunjiasu-cdn.net"),
+        CNAMEPattern(suffix="opencdnka.jomodns.com", pattern=r"opencdnka.jomodns.com", is_leaf=True),
+        CNAMEPattern(suffix="opencdnkav6.jomodns.com", pattern=r"opencdnkav6.jomodns.com", is_leaf=True),
     ],
-    cidr=BGPViewCIDR(query_term_list=["youpai", "upyun"]),
+    cidr=BGPViewCIDR(["baidu"]),
     frontend_ownership_verification=OwnershipVerification(
         txt=DomainOwnershipVerification(
             status=DomainOwnershipVerficationStatus.REQUIRED,
-            prefix="upyun-verify",
-            pattern=r"[0-9a-f]{32}",
+            prefix="bdy-verify",
+            pattern=r"[0-9a-f]{8}-[0-9a-f]{8}",
         ),
+        http=HTTPOwnershipVerification(status=DomainOwnershipVerficationStatus.NOT_REQUIRED),
     ),
     backend_ownership_verification=OwnershipVerification(
         txt=DomainOwnershipVerification(status=DomainOwnershipVerficationStatus.NOT_REQUIRED),
         http=HTTPOwnershipVerification(status=DomainOwnershipVerficationStatus.NOT_REQUIRED),
     ),
 )
```

### Comparing `cdnmon-0.5.3/cdnmon/model/cdn/wangsu.py` & `cdnmon-0.5.4/cdnmon/model/cdn/wangsu.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
         CNAMEPattern(suffix=".scdngc.net", source="https://beian.miit.gov.cn/"),
         CNAMEPattern(suffix=".sgccdn.com", source="https://beian.miit.gov.cn/"),
         CNAMEPattern(suffix=".speedcdns.com", source="https://beian.miit.gov.cn/"),
         CNAMEPattern(suffix=".speedws.com", source="https://beian.miit.gov.cn/"),
         CNAMEPattern(suffix=".srip.net.cn", source="https://beian.miit.gov.cn/"),
         CNAMEPattern(suffix=".srip88.net", source="https://beian.miit.gov.cn/"),
         CNAMEPattern(suffix=".tl53.net", source="https://beian.miit.gov.cn/"),
-        CNAMEPattern(suffix=".tl88.net", source="https://beian.miit.gov.cn/"),
+        CNAMEPattern(suffix=".tl88.net", source="https://beian.miit.gov.cn/", is_leaf=True),
         CNAMEPattern(suffix=".tl88c.net", source="https://beian.miit.gov.cn/"),
         CNAMEPattern(suffix=".vicp.cc", source="https://beian.miit.gov.cn/"),
         CNAMEPattern(suffix=".voddlb.com", source="https://beian.miit.gov.cn/"),
         CNAMEPattern(suffix=".wangsu.com", source="https://beian.miit.gov.cn/"),
         CNAMEPattern(suffix=".wangsucloud.com", source="https://beian.miit.gov.cn/"),
         CNAMEPattern(suffix=".wangsutong.com", source="https://beian.miit.gov.cn/"),
         CNAMEPattern(suffix=".waycdn.com", source="https://beian.miit.gov.cn/"),
```

### Comparing `cdnmon-0.5.3/cdnmon/util/aws.py` & `cdnmon-0.5.4/cdnmon/util/aws.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.3/cdnmon/util/bgpview.py` & `cdnmon-0.5.4/cdnmon/util/bgpview.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.3/pyproject.toml` & `cdnmon-0.5.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cdnmon"
-version = "0.5.3"
+version = "0.5.4"
 description = ""
 authors = ["Yihang Wang <wangyihanger@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.31.0"
```

### Comparing `cdnmon-0.5.3/PKG-INFO` & `cdnmon-0.5.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdnmon
-Version: 0.5.3
+Version: 0.5.4
 Summary: 
 Author: Yihang Wang
 Author-email: wangyihanger@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

