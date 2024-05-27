# Comparing `tmp/netbox-routing-0.1.1.tar.gz` & `tmp/netbox-routing-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/netbox-routing-0.1.1.tar", last modified: Tue May  7 17:49:42 2024, max compression
+gzip compressed data, was "dist/netbox-routing-0.1.2.tar", last modified: Mon May 27 19:21:33 2024, max compression
```

## Comparing `netbox-routing-0.1.1.tar` & `netbox-routing-0.1.2.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/api/nested_serializers/
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/nested_serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/nested_serializers/bgp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/nested_serializers/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/nested_serializers/ospf.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/nested_serializers/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/api/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/serializers/bgp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/serializers/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/serializers/ospf.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/serializers/static.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/api/views/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/views/bgp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/views/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/views/ospf.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/api/views/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/choices/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/choices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/choices/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/choices/bgp.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/choices/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/constants/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/constants/bgp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/fields/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/fields/ip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/filtersets/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/filtersets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/filtersets/bgp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/filtersets/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/filtersets/ospf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/filtersets/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/forms/
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/forms/bgp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/forms/bulk_edit/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/forms/bulk_edit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/forms/bulk_edit/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/forms/bulk_edit/ospf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/forms/bulk_import/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/forms/bulk_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/forms/bulk_import/ospf.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/forms/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/forms/filtersets/
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/forms/filtersets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/forms/filtersets/bgp.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/forms/filtersets/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/forms/filtersets/ospf.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/forms/filtersets/static.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/forms/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/forms/ospf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/forms/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/migrations/0002_netboxmodel_updates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/migrations/0003_model_ordering_and_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/migrations/0004_alter_prefixlistentry_ge_alter_prefixlistentry_le.py
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/migrations/0005_ospf.py
--rw-r--r--   0 runner    (1001) docker     (127)    13099 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/migrations/0006_bgp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/migrations/0007_bgpsessiontemplate_asn_bgpsessiontemplate_bfd_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/models/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/models/bgp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/models/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/models/ospf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/models/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/navigation/
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/navigation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/navigation/bgp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/navigation/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/navigation/ospf.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/navigation/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/tables/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/tables/bgp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/tables/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/tables/ospf.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/tables/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/bgpaddressfamily.html
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/bgprouter.html
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/bgpscope.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/inc/
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/inc/settings.html
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/object_children.html
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/objecttable.html
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/ospfarea.html
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/ospfinstance.html
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/ospfinterface.html
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/prefixlist.html
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/prefixlistentry.html
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/routemap.html
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/routemapentry.html
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/staticroute.html
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/staticroute_devices.html
--rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing/views/
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/views/bgp.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/views/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/views/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     5269 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/views/ospf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/netbox_routing/views/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/netbox_routing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 17:49:42.000000 netbox-routing-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-07 17:49:38.000000 netbox-routing-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:33.000000 netbox-routing-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-27 19:21:33.000000 netbox-routing-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:33.000000 netbox-routing-0.1.2/netbox_routing/
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:33.000000 netbox-routing-0.1.2/netbox_routing/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:33.000000 netbox-routing-0.1.2/netbox_routing/api/nested_serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/api/nested_serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/api/nested_serializers/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/api/nested_serializers/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/api/nested_serializers/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/api/nested_serializers/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:33.000000 netbox-routing-0.1.2/netbox_routing/api/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/api/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/api/serializers/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/api/serializers/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/api/serializers/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/api/serializers/static.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:33.000000 netbox-routing-0.1.2/netbox_routing/api/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/api/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/api/views/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/api/views/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/api/views/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/api/views/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:33.000000 netbox-routing-0.1.2/netbox_routing/choices/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/choices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/choices/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/choices/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/choices/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:33.000000 netbox-routing-0.1.2/netbox_routing/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/constants/bgp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:33.000000 netbox-routing-0.1.2/netbox_routing/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/fields/ip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:33.000000 netbox-routing-0.1.2/netbox_routing/filtersets/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/filtersets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/filtersets/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/filtersets/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/filtersets/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/filtersets/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:33.000000 netbox-routing-0.1.2/netbox_routing/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/forms/bgp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:33.000000 netbox-routing-0.1.2/netbox_routing/forms/bulk_edit/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/forms/bulk_edit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/forms/bulk_edit/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/forms/bulk_edit/ospf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:33.000000 netbox-routing-0.1.2/netbox_routing/forms/bulk_import/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/forms/bulk_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/forms/bulk_import/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/forms/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:33.000000 netbox-routing-0.1.2/netbox_routing/forms/filtersets/
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/forms/filtersets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/forms/filtersets/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/forms/filtersets/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/forms/filtersets/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/forms/filtersets/static.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/forms/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/forms/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/forms/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:33.000000 netbox-routing-0.1.2/netbox_routing/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:33.000000 netbox-routing-0.1.2/netbox_routing/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/migrations/0002_netboxmodel_updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/migrations/0003_model_ordering_and_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/migrations/0004_alter_prefixlistentry_ge_alter_prefixlistentry_le.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/migrations/0005_ospf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13099 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/migrations/0006_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/migrations/0007_bgpsessiontemplate_asn_bgpsessiontemplate_bfd_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:33.000000 netbox-routing-0.1.2/netbox_routing/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/models/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/models/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/models/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/models/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:33.000000 netbox-routing-0.1.2/netbox_routing/navigation/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/navigation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/navigation/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/navigation/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/navigation/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/navigation/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:33.000000 netbox-routing-0.1.2/netbox_routing/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/tables/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/tables/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/tables/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/tables/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:33.000000 netbox-routing-0.1.2/netbox_routing/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:33.000000 netbox-routing-0.1.2/netbox_routing/templates/netbox_routing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/templates/netbox_routing/bgpaddressfamily.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/templates/netbox_routing/bgprouter.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/templates/netbox_routing/bgpscope.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:33.000000 netbox-routing-0.1.2/netbox_routing/templates/netbox_routing/inc/
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/templates/netbox_routing/inc/settings.html
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/templates/netbox_routing/object_children.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/templates/netbox_routing/objecttable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/templates/netbox_routing/ospfarea.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/templates/netbox_routing/ospfinstance.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/templates/netbox_routing/ospfinterface.html
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/templates/netbox_routing/prefixlist.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/templates/netbox_routing/prefixlistentry.html
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/templates/netbox_routing/routemap.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/templates/netbox_routing/routemapentry.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/templates/netbox_routing/staticroute.html
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/templates/netbox_routing/staticroute_devices.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:33.000000 netbox-routing-0.1.2/netbox_routing/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/views/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/views/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6238 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/views/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/views/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/netbox_routing/views/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:33.000000 netbox-routing-0.1.2/netbox_routing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-27 19:21:33.000000 netbox-routing-0.1.2/netbox_routing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-27 19:21:33.000000 netbox-routing-0.1.2/netbox_routing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 19:21:33.000000 netbox-routing-0.1.2/netbox_routing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 19:21:33.000000 netbox-routing-0.1.2/netbox_routing.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-27 19:21:33.000000 netbox-routing-0.1.2/netbox_routing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-27 19:21:33.000000 netbox-routing-0.1.2/netbox_routing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 19:21:33.000000 netbox-routing-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-27 19:21:25.000000 netbox-routing-0.1.2/setup.py
```

### Comparing `netbox-routing-0.1.1/LICENSE` & `netbox-routing-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/PKG-INFO` & `netbox-routing-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-routing
-Version: 0.1.1
+Version: 0.1.2
 Summary: NetBox Routing
 Home-page: https://github.com/dansheps/netbox-routing/
 Download-URL: https://pypi.org/project/netbox-routing/
 Author: Daniel Sheppard
 Author-email: dans@dansheps.com
 Maintainer: Daniel Sheppard
 Maintainer-email: dans@dansheps.com
```

### Comparing `netbox-routing-0.1.1/README.md` & `netbox-routing-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/__init__.py` & `netbox-routing-0.1.2/netbox_routing/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/api/nested_serializers/__init__.py` & `netbox-routing-0.1.2/netbox_routing/api/nested_serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/api/nested_serializers/bgp.py` & `netbox-routing-0.1.2/netbox_routing/api/nested_serializers/bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/api/nested_serializers/objects.py` & `netbox-routing-0.1.2/netbox_routing/api/nested_serializers/objects.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/api/nested_serializers/ospf.py` & `netbox-routing-0.1.2/netbox_routing/api/nested_serializers/ospf.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/api/serializers/__init__.py` & `netbox-routing-0.1.2/netbox_routing/api/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/api/serializers/bgp.py` & `netbox-routing-0.1.2/netbox_routing/api/serializers/bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/api/serializers/objects.py` & `netbox-routing-0.1.2/netbox_routing/api/serializers/objects.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/api/serializers/ospf.py` & `netbox-routing-0.1.2/netbox_routing/api/serializers/ospf.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/api/serializers/static.py` & `netbox-routing-0.1.2/netbox_routing/api/serializers/static.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/api/urls.py` & `netbox-routing-0.1.2/netbox_routing/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/api/views/__init__.py` & `netbox-routing-0.1.2/netbox_routing/api/views/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/api/views/bgp.py` & `netbox-routing-0.1.2/netbox_routing/api/views/bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/api/views/objects.py` & `netbox-routing-0.1.2/netbox_routing/api/views/objects.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/api/views/ospf.py` & `netbox-routing-0.1.2/netbox_routing/api/views/ospf.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/choices/bgp.py` & `netbox-routing-0.1.2/netbox_routing/choices/bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/constants/bgp.py` & `netbox-routing-0.1.2/netbox_routing/constants/bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/fields/ip.py` & `netbox-routing-0.1.2/netbox_routing/fields/ip.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/filtersets/bgp.py` & `netbox-routing-0.1.2/netbox_routing/filtersets/bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/filtersets/objects.py` & `netbox-routing-0.1.2/netbox_routing/filtersets/objects.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/filtersets/ospf.py` & `netbox-routing-0.1.2/netbox_routing/filtersets/ospf.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/filtersets/static.py` & `netbox-routing-0.1.2/netbox_routing/filtersets/static.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/forms/__init__.py` & `netbox-routing-0.1.2/netbox_routing/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/forms/bgp.py` & `netbox-routing-0.1.2/netbox_routing/forms/bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/forms/bulk_edit/objects.py` & `netbox-routing-0.1.2/netbox_routing/forms/bulk_edit/objects.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/forms/bulk_edit/ospf.py` & `netbox-routing-0.1.2/netbox_routing/forms/bulk_edit/ospf.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/forms/bulk_import/ospf.py` & `netbox-routing-0.1.2/netbox_routing/forms/bulk_import/ospf.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/forms/filtersets/__init__.py` & `netbox-routing-0.1.2/netbox_routing/forms/filtersets/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/forms/filtersets/bgp.py` & `netbox-routing-0.1.2/netbox_routing/forms/filtersets/bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/forms/filtersets/ospf.py` & `netbox-routing-0.1.2/netbox_routing/forms/filtersets/ospf.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/forms/filtersets/static.py` & `netbox-routing-0.1.2/netbox_routing/forms/filtersets/static.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/forms/objects.py` & `netbox-routing-0.1.2/netbox_routing/forms/objects.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/forms/ospf.py` & `netbox-routing-0.1.2/netbox_routing/forms/ospf.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/forms/static.py` & `netbox-routing-0.1.2/netbox_routing/forms/static.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/migrations/0001_initial.py` & `netbox-routing-0.1.2/netbox_routing/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/migrations/0002_netboxmodel_updates.py` & `netbox-routing-0.1.2/netbox_routing/migrations/0002_netboxmodel_updates.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/migrations/0003_model_ordering_and_constraints.py` & `netbox-routing-0.1.2/netbox_routing/migrations/0003_model_ordering_and_constraints.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/migrations/0004_alter_prefixlistentry_ge_alter_prefixlistentry_le.py` & `netbox-routing-0.1.2/netbox_routing/migrations/0004_alter_prefixlistentry_ge_alter_prefixlistentry_le.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/migrations/0005_ospf.py` & `netbox-routing-0.1.2/netbox_routing/migrations/0005_ospf.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/migrations/0006_bgp.py` & `netbox-routing-0.1.2/netbox_routing/migrations/0006_bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/migrations/0007_bgpsessiontemplate_asn_bgpsessiontemplate_bfd_and_more.py` & `netbox-routing-0.1.2/netbox_routing/migrations/0007_bgpsessiontemplate_asn_bgpsessiontemplate_bfd_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/models/bgp.py` & `netbox-routing-0.1.2/netbox_routing/models/bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/models/objects.py` & `netbox-routing-0.1.2/netbox_routing/models/objects.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/models/ospf.py` & `netbox-routing-0.1.2/netbox_routing/models/ospf.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/models/static.py` & `netbox-routing-0.1.2/netbox_routing/models/static.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/navigation/bgp.py` & `netbox-routing-0.1.2/netbox_routing/navigation/bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/navigation/objects.py` & `netbox-routing-0.1.2/netbox_routing/navigation/objects.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/navigation/ospf.py` & `netbox-routing-0.1.2/netbox_routing/navigation/ospf.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/navigation/static.py` & `netbox-routing-0.1.2/netbox_routing/navigation/static.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/tables/bgp.py` & `netbox-routing-0.1.2/netbox_routing/tables/bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/tables/objects.py` & `netbox-routing-0.1.2/netbox_routing/tables/objects.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/tables/ospf.py` & `netbox-routing-0.1.2/netbox_routing/tables/ospf.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/tables/static.py` & `netbox-routing-0.1.2/netbox_routing/tables/static.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/bgpaddressfamily.html` & `netbox-routing-0.1.2/netbox_routing/templates/netbox_routing/bgpaddressfamily.html`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/bgprouter.html` & `netbox-routing-0.1.2/netbox_routing/templates/netbox_routing/bgprouter.html`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/bgpscope.html` & `netbox-routing-0.1.2/netbox_routing/templates/netbox_routing/bgpscope.html`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/object_children.html` & `netbox-routing-0.1.2/netbox_routing/templates/netbox_routing/object_children.html`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/objecttable.html` & `netbox-routing-0.1.2/netbox_routing/templates/netbox_routing/objecttable.html`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/ospfarea.html` & `netbox-routing-0.1.2/netbox_routing/templates/netbox_routing/ospfarea.html`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/ospfinstance.html` & `netbox-routing-0.1.2/netbox_routing/templates/netbox_routing/ospfinstance.html`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/ospfinterface.html` & `netbox-routing-0.1.2/netbox_routing/templates/netbox_routing/ospfinterface.html`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/prefixlist.html` & `netbox-routing-0.1.2/netbox_routing/templates/netbox_routing/prefixlist.html`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/prefixlistentry.html` & `netbox-routing-0.1.2/netbox_routing/templates/netbox_routing/prefixlistentry.html`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/routemap.html` & `netbox-routing-0.1.2/netbox_routing/templates/netbox_routing/routemap.html`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/routemapentry.html` & `netbox-routing-0.1.2/netbox_routing/templates/netbox_routing/routemapentry.html`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/staticroute.html` & `netbox-routing-0.1.2/netbox_routing/templates/netbox_routing/staticroute.html`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/templates/netbox_routing/staticroute_devices.html` & `netbox-routing-0.1.2/netbox_routing/templates/netbox_routing/staticroute_devices.html`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/urls.py` & `netbox-routing-0.1.2/netbox_routing/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/views/__init__.py` & `netbox-routing-0.1.2/netbox_routing/views/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/views/bgp.py` & `netbox-routing-0.1.2/netbox_routing/views/bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/views/core.py` & `netbox-routing-0.1.2/netbox_routing/views/core.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/netbox_routing/views/objects.py` & `netbox-routing-0.1.2/netbox_routing/views/objects.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,21 @@
 @register_model_view(PrefixList, name='entries')
 class PrefixListEntriesView(ObjectChildrenView):
     template_name = 'netbox_routing/objecttable.html'
     queryset = PrefixList.objects.all()
     child_model = PrefixListEntry
     table = PrefixListEntryTable
     filterset = PrefixListEntryFilterSet
-    actions = ['add', 'edit', 'delete', 'bulk_edit', 'bulk_delete']
+    actions = {
+        'add': {'add'},
+        'edit': {'change'},
+        'delete': {'delete'},
+        'bulk_edit': {'change'},
+        'bulk_delete': {'delete'}
+    }
     tab = ViewTab(
         label='Entries',
         badge=lambda obj: PrefixListEntry.objects.filter(prefix_list=obj).count(),
     )
 
     def get_children(self, request, parent):
         return self.child_model.objects.filter(prefix_list=parent)
@@ -122,15 +128,21 @@
 @register_model_view(RouteMap, name='entries')
 class RouteMapEntriesView(ObjectChildrenView):
     template_name = 'netbox_routing/objecttable.html'
     queryset = RouteMap.objects.all()
     child_model = RouteMapEntry
     table = RouteMapEntryTable
     filterset = RouteMapEntryFilterSet
-    actions = ['add', 'edit', 'delete', 'bulk_edit', 'bulk_delete']
+    actions = {
+        'add': {'add'},
+        'edit': {'change'},
+        'delete': {'delete'},
+        'bulk_edit': {'change'},
+        'bulk_delete': {'delete'}
+    }
     tab = ViewTab(
         label='Entries',
         badge=lambda obj: RouteMapEntry.objects.filter(route_map=obj).count(),
     )
 
     def get_children(self, request, parent):
         return self.child_model.objects.filter(route_map=parent)
```

### Comparing `netbox-routing-0.1.1/netbox_routing/views/ospf.py` & `netbox-routing-0.1.2/netbox_routing/views/ospf.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 @register_model_view(OSPFInstance, name='interfaces')
 class OSPFInstanceInterfacesView(ObjectChildrenView):
     template_name = 'netbox_routing/object_children.html'
     queryset = OSPFInstance.objects.all()
     child_model = OSPFInterface
     table = OSPFInterfaceTable
     filterset = OSPFInterfaceFilterSet
-    actions = []
     tab = ViewTab(
         label='Interfaces',
         badge=lambda obj: OSPFInterface.objects.filter(instance=obj).count(),
         hide_if_empty=False,
     )
 
     def get_children(self, request, parent):
@@ -101,15 +100,14 @@
 @register_model_view(OSPFArea, name='interfaces')
 class OSPFAreaInterfacesView(ObjectChildrenView):
     template_name = 'netbox_routing/object_children.html'
     queryset = OSPFArea.objects.all()
     child_model = OSPFInterface
     table = OSPFInterfaceTable
     filterset = OSPFInterfaceFilterSet
-    actions = []
     tab = ViewTab(
         label='Interfaces',
         badge=lambda obj: OSPFInterface.objects.filter(area=obj).count(),
     )
 
     def get_children(self, request, parent):
         return self.child_model.objects.filter(area=parent)
```

### Comparing `netbox-routing-0.1.1/netbox_routing/views/static.py` & `netbox-routing-0.1.2/netbox_routing/views/static.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 @register_model_view(StaticRoute, name='devices')
 class StaticRouteDevicesView(ObjectChildrenView):
     template_name = 'netbox_routing/staticroute_devices.html'
     queryset = StaticRoute.objects.all()
     child_model = Device
     table = DeviceTable
     filterset = DeviceFilterSet
-    actions = []
     tab = ViewTab(
         label='Assigned Devices',
         badge=lambda obj: Device.objects.filter(static_routes=obj).count(),
     )
 
     def get_children(self, request, parent):
         return self.child_model.objects.filter(static_routes=parent)
```

### Comparing `netbox-routing-0.1.1/netbox_routing.egg-info/PKG-INFO` & `netbox-routing-0.1.2/netbox_routing.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-routing
-Version: 0.1.1
+Version: 0.1.2
 Summary: NetBox Routing
 Home-page: https://github.com/dansheps/netbox-routing/
 Download-URL: https://pypi.org/project/netbox-routing/
 Author: Daniel Sheppard
 Author-email: dans@dansheps.com
 Maintainer: Daniel Sheppard
 Maintainer-email: dans@dansheps.com
```

### Comparing `netbox-routing-0.1.1/netbox_routing.egg-info/SOURCES.txt` & `netbox-routing-0.1.2/netbox_routing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.1.1/setup.py` & `netbox-routing-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='netbox-routing',
-    version='0.1.1',
+    version='0.1.2',
     description='NetBox Routing',
     long_description='Plugin for documentation of routing configuration and objects',
     url='https://github.com/dansheps/netbox-routing/',
     download_url='https://pypi.org/project/netbox-routing/',
     author='Daniel Sheppard',
     author_email='dans@dansheps.com',
     maintainer='Daniel Sheppard',
```

