# Comparing `tmp/openepd-3.1.4.tar.gz` & `tmp/openepd-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openepd-3.1.4.tar", max compression
+gzip compressed data, was "openepd-3.2.0.tar", max compression
```

## Comparing `openepd-3.1.4.tar` & `openepd-3.2.0.tar`

### file list

```diff
@@ -1,92 +1,93 @@
--rw-r--r--   0        0        0    11357 2024-05-03 19:13:58.242853 openepd-3.1.4/LICENSE
--rw-r--r--   0        0        0     6786 2024-05-03 19:13:58.242853 openepd-3.1.4/README.md
--rw-r--r--   0        0        0     3147 2024-05-03 19:13:58.242853 openepd-3.1.4/pyproject.toml
--rw-r--r--   0        0        0      837 2024-05-03 19:13:58.242853 openepd-3.1.4/src/openepd/__init__.py
--rw-r--r--   0        0        0      855 2024-05-03 19:13:58.242853 openepd-3.1.4/src/openepd/__version__.py
--rw-r--r--   0        0        0      837 2024-05-03 19:13:58.246853 openepd-3.1.4/src/openepd/api/__init__.py
--rw-r--r--   0        0        0    21142 2024-05-03 19:13:58.246853 openepd-3.1.4/src/openepd/api/base_sync_client.py
--rw-r--r--   0        0        0      837 2024-05-03 19:13:58.246853 openepd-3.1.4/src/openepd/api/category/__init__.py
--rw-r--r--   0        0        0     1067 2024-05-03 19:13:58.246853 openepd-3.1.4/src/openepd/api/category/dto.py
--rw-r--r--   0        0        0     1588 2024-05-03 19:13:58.246853 openepd-3.1.4/src/openepd/api/category/sync_api.py
--rw-r--r--   0        0        0     8681 2024-05-03 19:13:58.246853 openepd-3.1.4/src/openepd/api/common.py
--rw-r--r--   0        0        0      837 2024-05-03 19:13:58.246853 openepd-3.1.4/src/openepd/api/dto/__init__.py
--rw-r--r--   0        0        0     1250 2024-05-03 19:13:58.246853 openepd-3.1.4/src/openepd/api/dto/base.py
--rw-r--r--   0        0        0     4705 2024-05-03 19:13:58.246853 openepd-3.1.4/src/openepd/api/dto/common.py
--rw-r--r--   0        0        0     2377 2024-05-03 19:13:58.246853 openepd-3.1.4/src/openepd/api/dto/meta.py
--rw-r--r--   0        0        0     2211 2024-05-03 19:13:58.246853 openepd-3.1.4/src/openepd/api/dto/mf.py
--rw-r--r--   0        0        0      837 2024-05-03 19:13:58.246853 openepd-3.1.4/src/openepd/api/dto/params.py
--rw-r--r--   0        0        0      837 2024-05-03 19:13:58.246853 openepd-3.1.4/src/openepd/api/epd/__init__.py
--rw-r--r--   0        0        0     5091 2024-05-03 19:13:58.246853 openepd-3.1.4/src/openepd/api/epd/dto.py
--rw-r--r--   0        0        0     4391 2024-05-03 19:13:58.246853 openepd-3.1.4/src/openepd/api/epd/sync_api.py
--rw-r--r--   0        0        0     2376 2024-05-03 19:13:58.246853 openepd-3.1.4/src/openepd/api/errors.py
--rw-r--r--   0        0        0      837 2024-05-03 19:13:58.246853 openepd-3.1.4/src/openepd/api/pcr/__init__.py
--rw-r--r--   0        0        0     1649 2024-05-03 19:13:58.246853 openepd-3.1.4/src/openepd/api/pcr/dto.py
--rw-r--r--   0        0        0     1805 2024-05-03 19:13:58.246853 openepd-3.1.4/src/openepd/api/pcr/sync_api.py
--rw-r--r--   0        0        0     2504 2024-05-03 19:13:58.246853 openepd-3.1.4/src/openepd/api/sync_client.py
--rw-r--r--   0        0        0      837 2024-05-03 19:13:58.246853 openepd-3.1.4/src/openepd/api/test/__init__.py
--rw-r--r--   0        0        0      837 2024-05-03 19:13:58.246853 openepd-3.1.4/src/openepd/bundle/__init__.py
--rw-r--r--   0        0        0     7086 2024-05-03 19:13:58.246853 openepd-3.1.4/src/openepd/bundle/base.py
--rw-r--r--   0        0        0     2663 2024-05-03 19:13:58.246853 openepd-3.1.4/src/openepd/bundle/model.py
--rw-r--r--   0        0        0     6904 2024-05-03 19:13:58.246853 openepd-3.1.4/src/openepd/bundle/reader.py
--rw-r--r--   0        0        0     8353 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/bundle/writer.py
--rw-r--r--   0        0        0      837 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/compat/__init__.py
--rw-r--r--   0        0        0     1051 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/compat/compat_functional_validators.py
--rw-r--r--   0        0        0     1363 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/compat/pydantic.py
--rw-r--r--   0        0        0      837 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/__init__.py
--rw-r--r--   0        0        0     9154 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/base.py
--rw-r--r--   0        0        0     1856 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/category.py
--rw-r--r--   0        0        0     5659 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/common.py
--rw-r--r--   0        0        0    14299 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/epd.py
--rw-r--r--   0        0        0     1918 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/factory.py
--rw-r--r--   0        0        0    17165 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/lcia.py
--rw-r--r--   0        0        0     4013 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/org.py
--rw-r--r--   0        0        0     4620 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/pcr.py
--rw-r--r--   0        0        0      862 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/README.md
--rw-r--r--   0        0        0     5176 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/__init__.py
--rw-r--r--   0        0        0     3549 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/asphalt.py
--rw-r--r--   0        0        0     2697 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/base.py
--rw-r--r--   0        0        0     9810 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/concrete.py
--rw-r--r--   0        0        0     1934 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/accessories.py
--rw-r--r--   0        0        0     3161 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/aggregates.py
--rw-r--r--   0        0        0     2440 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/aluminium.py
--rw-r--r--   0        0        0     3365 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/asphalt.py
--rw-r--r--   0        0        0     1034 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/bulk_materials.py
--rw-r--r--   0        0        0     1058 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/cast_decks_and_underlayment.py
--rw-r--r--   0        0        0     6475 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/cladding.py
--rw-r--r--   0        0        0     2000 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/cmu.py
--rw-r--r--   0        0        0     1117 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/common.py
--rw-r--r--   0        0        0     7204 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/concrete.py
--rw-r--r--   0        0        0     1986 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/conveying_equipment.py
--rw-r--r--   0        0        0     9996 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/electrical.py
--rw-r--r--   0        0        0     2117 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/electrical_transmission_and_distribution_equipment.py
--rw-r--r--   0        0        0     1029 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/electricity.py
--rw-r--r--   0        0        0    58482 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/enums.py
--rw-r--r--   0        0        0    20292 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/finishes.py
--rw-r--r--   0        0        0     2665 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/fire_and_smoke_protection.py
--rw-r--r--   0        0        0     2940 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/furnishings.py
--rw-r--r--   0        0        0     1023 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/grouting.py
--rw-r--r--   0        0        0     4599 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/manufacturing_inputs.py
--rw-r--r--   0        0        0     3216 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/masonry.py
--rw-r--r--   0        0        0     1225 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/material_handling.py
--rw-r--r--   0        0        0     8388 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/mechanical.py
--rw-r--r--   0        0        0     1714 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/mechanical_insulation.py
--rw-r--r--   0        0        0     7924 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/network_infrastructure.py
--rw-r--r--   0        0        0    19035 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/openings.py
--rw-r--r--   0        0        0     1057 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/other_electrical_equipment.py
--rw-r--r--   0        0        0     3453 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/other_materials.py
--rw-r--r--   0        0        0     4652 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/plumbing.py
--rw-r--r--   0        0        0     2490 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/precast_concrete.py
--rw-r--r--   0        0        0     3516 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/sheathing.py
--rw-r--r--   0        0        0    10118 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/steel.py
--rw-r--r--   0        0        0     7368 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/thermal_moisture_protection.py
--rw-r--r--   0        0        0     2372 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/utility_piping.py
--rw-r--r--   0        0        0     6027 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/wood.py
--rw-r--r--   0        0        0     1880 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/specs/generated/wood_joists.py
--rw-r--r--   0        0        0     1535 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/standard.py
--rw-r--r--   0        0        0      837 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/validation/__init__.py
--rw-r--r--   0        0        0     2652 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/validation/common.py
--rw-r--r--   0        0        0     1105 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/validation/numbers.py
--rw-r--r--   0        0        0     7402 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/validation/quantity.py
--rw-r--r--   0        0        0     4690 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/model/versioning.py
--rw-r--r--   0        0        0        0 2024-05-03 19:13:58.250853 openepd-3.1.4/src/openepd/py.typed
--rw-r--r--   0        0        0     7790 1970-01-01 00:00:00.000000 openepd-3.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-27 14:03:07.508798 openepd-3.2.0/LICENSE
+-rw-r--r--   0        0        0     6786 2024-05-27 14:03:07.508798 openepd-3.2.0/README.md
+-rw-r--r--   0        0        0     3147 2024-05-27 14:03:07.508798 openepd-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0      837 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/__init__.py
+-rw-r--r--   0        0        0      855 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/__version__.py
+-rw-r--r--   0        0        0      837 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/__init__.py
+-rw-r--r--   0        0        0    21142 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/base_sync_client.py
+-rw-r--r--   0        0        0      837 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/category/__init__.py
+-rw-r--r--   0        0        0     1067 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/category/dto.py
+-rw-r--r--   0        0        0     1588 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/category/sync_api.py
+-rw-r--r--   0        0        0     8681 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/common.py
+-rw-r--r--   0        0        0      837 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/dto/__init__.py
+-rw-r--r--   0        0        0     1250 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/dto/base.py
+-rw-r--r--   0        0        0     4705 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/dto/common.py
+-rw-r--r--   0        0        0     2377 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/dto/meta.py
+-rw-r--r--   0        0        0     2211 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/dto/mf.py
+-rw-r--r--   0        0        0      837 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/dto/params.py
+-rw-r--r--   0        0        0      837 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/epd/__init__.py
+-rw-r--r--   0        0        0     5091 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/epd/dto.py
+-rw-r--r--   0        0        0     4391 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/epd/sync_api.py
+-rw-r--r--   0        0        0     2376 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/errors.py
+-rw-r--r--   0        0        0      837 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/pcr/__init__.py
+-rw-r--r--   0        0        0     1649 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/pcr/dto.py
+-rw-r--r--   0        0        0     1805 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/pcr/sync_api.py
+-rw-r--r--   0        0        0     2504 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/sync_client.py
+-rw-r--r--   0        0        0      837 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/test/__init__.py
+-rw-r--r--   0        0        0      837 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/bundle/__init__.py
+-rw-r--r--   0        0        0     7086 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/bundle/base.py
+-rw-r--r--   0        0        0     2663 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/bundle/model.py
+-rw-r--r--   0        0        0     6904 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/bundle/reader.py
+-rw-r--r--   0        0        0     8353 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/bundle/writer.py
+-rw-r--r--   0        0        0      837 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/compat/__init__.py
+-rw-r--r--   0        0        0     1051 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/compat/compat_functional_validators.py
+-rw-r--r--   0        0        0     1363 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/compat/pydantic.py
+-rw-r--r--   0        0        0      837 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/__init__.py
+-rw-r--r--   0        0        0     9154 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/base.py
+-rw-r--r--   0        0        0     1856 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/category.py
+-rw-r--r--   0        0        0     5659 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/common.py
+-rw-r--r--   0        0        0    14299 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/epd.py
+-rw-r--r--   0        0        0     1918 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/factory.py
+-rw-r--r--   0        0        0    17165 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/lcia.py
+-rw-r--r--   0        0        0     4013 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/org.py
+-rw-r--r--   0        0        0     4620 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/pcr.py
+-rw-r--r--   0        0        0      862 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/README.md
+-rw-r--r--   0        0        0     5176 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/__init__.py
+-rw-r--r--   0        0        0     3549 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/asphalt.py
+-rw-r--r--   0        0        0     2697 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/base.py
+-rw-r--r--   0        0        0     9810 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/concrete.py
+-rw-r--r--   0        0        0      837 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/generated/__init__.py
+-rw-r--r--   0        0        0     2230 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/generated/accessories.py
+-rw-r--r--   0        0        0     3161 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/generated/aggregates.py
+-rw-r--r--   0        0        0     2630 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/generated/aluminium.py
+-rw-r--r--   0        0        0     3369 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/generated/asphalt.py
+-rw-r--r--   0        0        0     1092 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/generated/bulk_materials.py
+-rw-r--r--   0        0        0     1172 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/generated/cast_decks_and_underlayment.py
+-rw-r--r--   0        0        0     6779 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/generated/cladding.py
+-rw-r--r--   0        0        0     2011 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/generated/cmu.py
+-rw-r--r--   0        0        0     1117 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/generated/common.py
+-rw-r--r--   0        0        0     7204 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/generated/concrete.py
+-rw-r--r--   0        0        0     2034 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/generated/conveying_equipment.py
+-rw-r--r--   0        0        0    10972 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/generated/electrical.py
+-rw-r--r--   0        0        0     2195 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/generated/electrical_transmission_and_distribution_equipment.py
+-rw-r--r--   0        0        0     1040 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/electricity.py
+-rw-r--r--   0        0        0    58546 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/enums.py
+-rw-r--r--   0        0        0    21338 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/finishes.py
+-rw-r--r--   0        0        0     3285 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/fire_and_smoke_protection.py
+-rw-r--r--   0        0        0     2798 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/furnishings.py
+-rw-r--r--   0        0        0     1151 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/grouting.py
+-rw-r--r--   0        0        0     5320 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/manufacturing_inputs.py
+-rw-r--r--   0        0        0     3286 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/masonry.py
+-rw-r--r--   0        0        0     1491 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/material_handling.py
+-rw-r--r--   0        0        0     9494 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/mechanical.py
+-rw-r--r--   0        0        0     1834 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/mechanical_insulation.py
+-rw-r--r--   0        0        0     8374 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/network_infrastructure.py
+-rw-r--r--   0        0        0    19035 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/openings.py
+-rw-r--r--   0        0        0     1031 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/other_electrical_equipment.py
+-rw-r--r--   0        0        0     3715 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/other_materials.py
+-rw-r--r--   0        0        0     4795 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/plumbing.py
+-rw-r--r--   0        0        0     2529 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/precast_concrete.py
+-rw-r--r--   0        0        0     3853 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/sheathing.py
+-rw-r--r--   0        0        0    10118 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/steel.py
+-rw-r--r--   0        0        0     8422 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/thermal_moisture_protection.py
+-rw-r--r--   0        0        0     2710 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/utility_piping.py
+-rw-r--r--   0        0        0     6756 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/wood.py
+-rw-r--r--   0        0        0     2079 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/wood_joists.py
+-rw-r--r--   0        0        0     1535 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/standard.py
+-rw-r--r--   0        0        0      837 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/validation/__init__.py
+-rw-r--r--   0        0        0     2652 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/validation/common.py
+-rw-r--r--   0        0        0     1105 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/validation/numbers.py
+-rw-r--r--   0        0        0     7402 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/validation/quantity.py
+-rw-r--r--   0        0        0     4690 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/versioning.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/py.typed
+-rw-r--r--   0        0        0     7790 1970-01-01 00:00:00.000000 openepd-3.2.0/PKG-INFO
```

### Comparing `openepd-3.1.4/LICENSE` & `openepd-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/README.md` & `openepd-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/pyproject.toml` & `openepd-3.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openepd"
-version = "3.1.4"
+version = "3.2.0"
 license = "Apache-2.0"
 description = "Python library to work with OpenEPD format"
 authors = ["C-Change Labs <support@c-change-labs.com>"]
 maintainers = ["C-Change Labs <open-source@c-change-labs.com>"]
 repository = "https://github.com/cchangelabs/openepd"
 keywords = []
 classifiers = [
```

### Comparing `openepd-3.1.4/src/openepd/__init__.py` & `openepd-3.2.0/src/openepd/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/__version__.py` & `openepd-3.2.0/src/openepd/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-VERSION = "3.1.4"
+VERSION = "3.2.0"
```

### Comparing `openepd-3.1.4/src/openepd/api/__init__.py` & `openepd-3.2.0/src/openepd/api/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/api/base_sync_client.py` & `openepd-3.2.0/src/openepd/api/base_sync_client.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/api/category/__init__.py` & `openepd-3.2.0/src/openepd/api/category/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/api/category/dto.py` & `openepd-3.2.0/src/openepd/api/category/dto.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/api/category/sync_api.py` & `openepd-3.2.0/src/openepd/api/category/sync_api.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/api/common.py` & `openepd-3.2.0/src/openepd/api/common.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/api/dto/__init__.py` & `openepd-3.2.0/src/openepd/api/dto/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/api/dto/base.py` & `openepd-3.2.0/src/openepd/api/dto/base.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/api/dto/common.py` & `openepd-3.2.0/src/openepd/api/dto/common.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/api/dto/meta.py` & `openepd-3.2.0/src/openepd/api/dto/meta.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/api/dto/mf.py` & `openepd-3.2.0/src/openepd/api/dto/mf.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/api/dto/params.py` & `openepd-3.2.0/src/openepd/api/dto/params.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/api/epd/__init__.py` & `openepd-3.2.0/src/openepd/api/epd/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/api/epd/dto.py` & `openepd-3.2.0/src/openepd/api/epd/dto.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/api/epd/sync_api.py` & `openepd-3.2.0/src/openepd/api/epd/sync_api.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/api/errors.py` & `openepd-3.2.0/src/openepd/api/errors.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/api/pcr/__init__.py` & `openepd-3.2.0/src/openepd/api/pcr/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/api/pcr/dto.py` & `openepd-3.2.0/src/openepd/api/pcr/dto.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/api/pcr/sync_api.py` & `openepd-3.2.0/src/openepd/api/pcr/sync_api.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/api/sync_client.py` & `openepd-3.2.0/src/openepd/api/sync_client.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/api/test/__init__.py` & `openepd-3.2.0/src/openepd/api/test/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/bundle/__init__.py` & `openepd-3.2.0/src/openepd/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/bundle/base.py` & `openepd-3.2.0/src/openepd/bundle/base.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/bundle/model.py` & `openepd-3.2.0/src/openepd/bundle/model.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/bundle/reader.py` & `openepd-3.2.0/src/openepd/bundle/reader.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/bundle/writer.py` & `openepd-3.2.0/src/openepd/bundle/writer.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/compat/__init__.py` & `openepd-3.2.0/src/openepd/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/compat/compat_functional_validators.py` & `openepd-3.2.0/src/openepd/compat/compat_functional_validators.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/compat/pydantic.py` & `openepd-3.2.0/src/openepd/compat/pydantic.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/model/__init__.py` & `openepd-3.2.0/src/openepd/model/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/model/base.py` & `openepd-3.2.0/src/openepd/model/base.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/model/category.py` & `openepd-3.2.0/src/openepd/model/category.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/model/common.py` & `openepd-3.2.0/src/openepd/model/common.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/model/epd.py` & `openepd-3.2.0/src/openepd/model/epd.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/model/factory.py` & `openepd-3.2.0/src/openepd/model/factory.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/model/lcia.py` & `openepd-3.2.0/src/openepd/model/lcia.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/model/org.py` & `openepd-3.2.0/src/openepd/model/org.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/model/pcr.py` & `openepd-3.2.0/src/openepd/model/pcr.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/model/specs/README.md` & `openepd-3.2.0/src/openepd/model/specs/README.md`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/model/specs/__init__.py` & `openepd-3.2.0/src/openepd/model/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/model/specs/asphalt.py` & `openepd-3.2.0/src/openepd/model/specs/asphalt.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/model/specs/base.py` & `openepd-3.2.0/src/openepd/model/specs/base.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/model/specs/concrete.py` & `openepd-3.2.0/src/openepd/model/specs/concrete.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/accessories.py` & `openepd-3.2.0/src/openepd/model/specs/generated/accessories.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,45 +17,50 @@
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
 
 
 class BlanketFacingV1(BaseOpenEpdHierarchicalSpec):
-    """Blanket facing performance specification."""
+    """
+    Facing materials for insulation products.
+
+    Such as kraft, white vinyl sheeting, or aluminum foil, which can serve as air barrier, vapor barrier, radiant
+    barrier, or flame resistive layer.
+    """
 
     _EXT_VERSION = "1.0"
 
 
 class DoorsHardwareV1(BaseOpenEpdHierarchicalSpec):
-    """Doors hardware performance specification."""
+    """Door hardware, including automatic and security door hardware."""
 
     _EXT_VERSION = "1.0"
 
 
 class FlooringAccessoriesV1(BaseOpenEpdHierarchicalSpec):
-    """Flooring accessories performance specification."""
+    """Products used in flooring, other than the actual flooring product itself."""
 
     _EXT_VERSION = "1.0"
 
 
 class MortarV1(BaseOpenEpdHierarchicalSpec):
-    """Mortar performance specification."""
+    """Cementitious paste used to bind building blocks such as stones, bricks, and concrete masonry."""
 
     _EXT_VERSION = "1.0"
 
 
 class TileGroutV1(BaseOpenEpdHierarchicalSpec):
-    """Tile grout performance specification."""
+    """Water-cement-sand mixture for laying ceramic tile."""
 
     _EXT_VERSION = "1.0"
 
 
 class AccessoriesV1(BaseOpenEpdHierarchicalSpec):
-    """Accessories performance specification."""
+    """Materials that are used alongside other materials."""
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
     BlanketFacing: BlanketFacingV1 | None = None
     DoorsHardware: DoorsHardwareV1 | None = None
     FlooringAccessories: FlooringAccessoriesV1 | None = None
```

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/aggregates.py` & `openepd-3.2.0/src/openepd/model/specs/generated/aggregates.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/aluminium.py` & `openepd-3.2.0/src/openepd/model/specs/generated/aluminium.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,42 +19,45 @@
 #
 from openepd.compat.pydantic import pyd
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
 from openepd.model.specs.generated.enums import AluminiumAlloy
 
 
 class AluminiumBilletsV1(BaseOpenEpdHierarchicalSpec):
-    """Aluminium billets performance specification."""
+    """Cast Aluminium ingots or billets for use in manufacturing more finished products."""
 
     _EXT_VERSION = "1.0"
 
 
 class AluminiumExtrusionsV1(BaseOpenEpdHierarchicalSpec):
-    """Aluminium extrusions performance specification."""
+    """Extruded aluminum products used in construction.
+
+    Includes range of finish options including mill finish, painted, and anodized.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     thermally_improved: bool | None = pyd.Field(default=None, description="", example=True)
 
 
 class AluminiumSheetGoodsV1(BaseOpenEpdHierarchicalSpec):
-    """Aluminium sheet goods performance specification."""
+    """Rolled and/or Stamped Aluminium coil or sheets, often used in flashing, trim, panels, and deck."""
 
     _EXT_VERSION = "1.0"
 
 
 class AluminiumSuspensionAssemblyV1(BaseOpenEpdHierarchicalSpec):
-    """Aluminium suspension assembly performance specification."""
+    """Aluminum suspension assemblies for acoustical ceiling systems."""
 
     _EXT_VERSION = "1.0"
 
 
 class AluminiumV1(BaseOpenEpdHierarchicalSpec):
-    """Material definition for objects made primarily from Aluminium and its alloys."""
+    """Broad category for construction materials made primarily from Aluminium and its alloys."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     alloy: AluminiumAlloy | None = pyd.Field(default=None, description="", example=str(AluminiumAlloy.ALLOY_1XXX))
     anodized: bool | None = pyd.Field(default=None, description="", example=True)
     painted: bool | None = pyd.Field(default=None, description="", example=True)
```

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/asphalt.py` & `openepd-3.2.0/src/openepd/model/specs/generated/asphalt.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
 from openepd.model.specs.generated.enums import AsphaltGradation, AsphaltMixType
 from openepd.model.validation.numbers import RatioFloat
 from openepd.model.validation.quantity import LengthMmStr, TemperatureCStr
 
 
 class AsphaltV1(BaseOpenEpdHierarchicalSpec):
-    """Asphalt performance specification."""
+    """General category for asphalt mixtures."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     aggregate_size_max: LengthMmStr | None = pyd.Field(default=None, description="Max aggregate size", example="20 mm")
     rap: RatioFloat | None = pyd.Field(
         default=None,
```

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/bulk_materials.py` & `openepd-3.2.0/src/openepd/model/specs/generated/bulk_materials.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,10 +17,10 @@
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
 
 
 class BulkMaterialsV1(BaseOpenEpdHierarchicalSpec):
-    """Bulk materials performance specification."""
+    """A generic category for materials whose declared unit is mass and which are not in another category."""
 
     _EXT_VERSION = "1.0"
```

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/cast_decks_and_underlayment.py` & `openepd-3.2.0/src/openepd/model/specs/generated/other_electrical_equipment.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,11 +16,11 @@
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
 
 
-class CastDecksAndUnderlaymentV1(BaseOpenEpdHierarchicalSpec):
-    """Cast decks and underlayment performance specification."""
+class OtherElectricalEquipmentV1(BaseOpenEpdHierarchicalSpec):
+    """Other Electrical Equipment."""
 
     _EXT_VERSION = "1.0"
```

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/cladding.py` & `openepd-3.2.0/src/openepd/model/specs/generated/cladding.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,109 +20,113 @@
 from openepd.compat.pydantic import pyd
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
 from openepd.model.specs.generated.enums import CladdingFacingMaterial, CladdingInsulatingMaterial, SidingFormFactor
 from openepd.model.validation.quantity import LengthMmStr, LengthMStr, RValueStr, validate_unit_factory
 
 
 class AluminiumSidingV1(BaseOpenEpdHierarchicalSpec):
-    """Aluminium siding performance specification."""
+    """Exterior siding product made primarily from aluminium."""
 
     _EXT_VERSION = "1.0"
 
 
 class SteelSidingV1(BaseOpenEpdHierarchicalSpec):
-    """Steel siding performance specification."""
+    """Exterior siding product made primarily from steel."""
 
     _EXT_VERSION = "1.0"
 
 
 class ZincSidingV1(BaseOpenEpdHierarchicalSpec):
-    """Zinc siding performance specification."""
+    """Exterior siding product made primarily from zinc."""
 
     _EXT_VERSION = "1.0"
 
 
 class ShingleAndShakeSidingV1(BaseOpenEpdHierarchicalSpec):
-    """Shingle and shake siding performance specification."""
+    """Shingle & shake siding."""
 
     _EXT_VERSION = "1.0"
 
 
 class MetalSidingV1(BaseOpenEpdHierarchicalSpec):
-    """Metal siding performance specification."""
+    """Exterior siding product made of metal such as steel, aluminum, etc."""
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
     AluminiumSiding: AluminiumSidingV1 | None = None
     SteelSiding: SteelSidingV1 | None = None
     ZincSiding: ZincSidingV1 | None = None
 
 
 class CompositionSidingV1(BaseOpenEpdHierarchicalSpec):
-    """Composition siding performance specification."""
+    """Composite wood siding composed of wood wafers and resin."""
 
     _EXT_VERSION = "1.0"
 
 
 class FiberCementSidingV1(BaseOpenEpdHierarchicalSpec):
-    """Fiber cement siding performance specification."""
+    """Composite siding product made of cement and cellulose fibers."""
 
     _EXT_VERSION = "1.0"
 
 
 class InsulatedVinylSidingV1(BaseOpenEpdHierarchicalSpec):
-    """Insulated vinyl siding performance specification."""
+    """Vinyl cladding product integrated with manufacturer-installed insulation."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     thickness: LengthMmStr | None = pyd.Field(default=None, description="", example="1 mm")
 
     _vinyl_siding_thickness_is_quantity_validator = pyd.validator("thickness", allow_reuse=True)(
         validate_unit_factory("m")
     )
 
 
 class PlywoodSidingV1(BaseOpenEpdHierarchicalSpec):
-    """Plywood siding performance specification."""
+    """Siding made of plywood boards."""
 
     _EXT_VERSION = "1.0"
 
 
 class PolypropyleneSidingV1(BaseOpenEpdHierarchicalSpec):
-    """Polypropylene siding performance specification."""
+    """Exterior wall cladding made from polypropylene, which may contain fillers or reinforcements."""
 
     _EXT_VERSION = "1.0"
 
 
 class SolidWoodSidingV1(BaseOpenEpdHierarchicalSpec):
-    """Solid wood siding performance specification."""
+    """Siding products made of wood including shingle & shake siding."""
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
     ShingleAndShakeSiding: ShingleAndShakeSidingV1 | None = None
 
 
 class VinylSidingV1(BaseOpenEpdHierarchicalSpec):
-    """Vinyl siding performance specification."""
+    """Exterior wall cladding made principally from rigid polyvinyl chloride (PVC)."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     thickness: LengthMmStr | None = pyd.Field(default=None, description="", example="5 mm")
 
     _vinyl_siding_thickness_is_quantity_validator = pyd.validator("thickness", allow_reuse=True)(
         validate_unit_factory("m")
     )
 
 
 class SidingV1(BaseOpenEpdHierarchicalSpec):
-    """Siding performance specification."""
+    """
+    Long narrow products for exterior wall face of building.
+
+    Typically made of, e.g., metal, solid wood, plywood, plastic, composition, fiber cement, etc.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     insulated: bool | None = pyd.Field(default=None, description="", example=True)
     ventilated: bool | None = pyd.Field(default=None, description="", example=True)
     paint_or_stain_required: bool | None = pyd.Field(default=None, description="", example=True)
```

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/cmu.py` & `openepd-3.2.0/src/openepd/model/specs/generated/cmu.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from openepd.compat.pydantic import pyd
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
 from openepd.model.specs.generated.enums import CmuBlockType, CmuWeightClassification
 from openepd.model.validation.quantity import GwpKgCo2eStr, PressureMPaStr
 
 
 class CMUV1(BaseOpenEpdHierarchicalSpec):
-    """CMU performance specification."""
+    """Pre-manufactured concrete masonry blocks."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     white_cement: bool | None = pyd.Field(default=None, description="", example=True)
     strength_28d: PressureMPaStr | None = pyd.Field(default=None, description="", example="1 MPa")
     weight_classification: CmuWeightClassification | None = pyd.Field(default=None, description="", example="Normal")
```

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/common.py` & `openepd-3.2.0/src/openepd/model/specs/generated/common.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/concrete.py` & `openepd-3.2.0/src/openepd/model/specs/generated/concrete.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/conveying_equipment.py` & `openepd-3.2.0/src/openepd/model/specs/generated/conveying_equipment.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 from openepd.compat.pydantic import pyd
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
 from openepd.model.specs.generated.enums import ElevatorsBuildingRise, ElevatorsUsageIntensity
 from openepd.model.validation.quantity import LengthMStr, MassKgStr, SpeedStr
 
 
 class ElevatorsV1(BaseOpenEpdHierarchicalSpec):
-    """Elevators performance specification."""
+    """Car that moves in a vertical shaft to carry passengers or freight between the levels of a multistory building."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     usage_intensity: list[ElevatorsUsageIntensity] | None = pyd.Field(
         default=None, description="", example=["Very low"]
     )
     travel_length: LengthMStr | None = pyd.Field(default=None, description="", example="1 m")
     rated_load: MassKgStr | None = pyd.Field(default=None, description="", example="1 kg")
     rated_speed: SpeedStr | None = pyd.Field(default=None, description="", example="1 m / s")
     building_rise: ElevatorsBuildingRise | None = pyd.Field(default=None, description="", example="Low-rise")
 
 
 class ConveyingEquipmentV1(BaseOpenEpdHierarchicalSpec):
-    """Conveying equipment performance specification."""
+    """Conveying Equipment."""
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
     Elevators: ElevatorsV1 | None = None
```

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/electrical.py` & `openepd-3.2.0/src/openepd/model/specs/generated/electrical.py`

 * *Files 15% similar despite different names*

```diff
@@ -30,39 +30,39 @@
     validate_quantity_ge_factory,
     validate_quantity_le_factory,
     validate_unit_factory,
 )
 
 
 class LowVoltBusesV1(BaseOpenEpdHierarchicalSpec):
-    """Low volt buses performance specification."""
+    """Busbars and Busways of 600V or less."""
 
     _EXT_VERSION = "1.0"
 
 
 class MedVoltBusesV1(BaseOpenEpdHierarchicalSpec):
-    """Med volt buses performance specification."""
+    """Busbars and Busways over 600V."""
 
     _EXT_VERSION = "1.0"
 
 
 class BatteriesV1(BaseOpenEpdHierarchicalSpec):
-    """Batteries performance specification."""
+    """Battery equipment, including central batteries, battery charging, and UPS."""
 
     _EXT_VERSION = "1.0"
 
 
 class OtherElectricalPowerStorageV1(BaseOpenEpdHierarchicalSpec):
     """Other electrical power storage performance specification."""
 
     _EXT_VERSION = "1.0"
 
 
 class CableTraysV1(BaseOpenEpdHierarchicalSpec):
-    """Cable trays performance specification."""
+    """Mechanical support for electrial or communications cabling, typically suspended from a roof or wall."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     height: LengthMmStr | None = pyd.Field(default=None, description="", example="100 mm")
     width: LengthMmStr | None = pyd.Field(default=None, description="", example="100 mm")
     depth: LengthMmStr | None = pyd.Field(default=None, description="", example="100 mm")
@@ -70,180 +70,193 @@
     ventilated: bool | None = pyd.Field(
         default=None, description="At least 40% of the tray base is open to air flow", example=True
     )
     cable_trays_material: CableTraysMaterial | None = pyd.Field(default=None, description="", example="Stainless Steel")
 
 
 class ElectricalBusesV1(BaseOpenEpdHierarchicalSpec):
-    """Electrical buses performance specification."""
+    """
+    Power distribution, in the form of busbars or of insulted ducts made of copper or aluminum busbars.
+
+    It is an alternative means of conducting electricity compared toto power cables or cable bus. Also called
+    bus ducts.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
     LowVoltBuses: LowVoltBusesV1 | None = None
     MedVoltBuses: MedVoltBusesV1 | None = None
 
 
 class FloorEquipmentBoxesV1(BaseOpenEpdHierarchicalSpec):
-    """Floor equipment boxes performance specification."""
+    """Equipment boxes for power or electronic equipment embedded in an accessible floor."""
 
     _EXT_VERSION = "1.0"
 
 
 class PowerDistributionUnitsV1(BaseOpenEpdHierarchicalSpec):
-    """Power distribution units performance specification."""
+    """Switched electrical distribution units placed very close to the point of consumption, for example inside a rack of electronic equipment."""
 
     _EXT_VERSION = "1.0"
 
 
 class RacewaysV1(BaseOpenEpdHierarchicalSpec):
-    """Raceways performance specification."""
+    """Mechanical guideways for eletrical communications cabling, typically embedded in an accessible floor."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     width: LengthMStr | None = pyd.Field(default=None, description="", example="100 mm")
     depth: LengthMStr | None = pyd.Field(default=None, description="", example="100 mm")
     painted: bool | None = pyd.Field(default=None, description="", example=True)
     divided: bool | None = pyd.Field(default=None, description="", example=True)
     raceways_material: RacewaysMaterial | None = pyd.Field(default=None, description="", example="Aluminum")
 
 
 class FueledElectricalGeneratorsV1(BaseOpenEpdHierarchicalSpec):
-    """Fueled electrical generators performance specification."""
+    """Fueled electrical generators."""
 
     _EXT_VERSION = "1.0"
 
 
 class OtherGenerationV1(BaseOpenEpdHierarchicalSpec):
-    """Other generation performance specification."""
+    """Other generation."""
 
     _EXT_VERSION = "1.0"
 
 
 class PhotovoltaicsV1(BaseOpenEpdHierarchicalSpec):
-    """Photovoltaics performance specification."""
+    """Solar photovoltaics, rated on a nameplate capacity basis."""
 
     _EXT_VERSION = "1.0"
 
 
 class WindTurbinesV1(BaseOpenEpdHierarchicalSpec):
-    """Wind turbines performance specification."""
+    """Wind generators, rated on a nameplate capacity basis."""
 
     _EXT_VERSION = "1.0"
 
 
 class ElectricityFromPowerGridV1(BaseOpenEpdHierarchicalSpec):
-    """Electricity from power grid performance specification."""
+    """Electrical energy drawn from a specific utility grid."""
 
     _EXT_VERSION = "1.0"
 
 
 class ElectricityFromSpecificGeneratorV1(BaseOpenEpdHierarchicalSpec):
-    """Electricity from specific generator performance specification."""
+    """Electrical energy from a specific power plant, such as a wind farm using a specific type of turbine."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     energy_source: EnergySource | None = pyd.Field(default=None, description="", example="Grid")
 
 
 class PowerPurchaseAgreementsV1(BaseOpenEpdHierarchicalSpec):
-    """Power purchase agreements performance specification."""
+    """
+    Electrical energy subject to a verified power purchase agreement.
+
+    The impact of electricity generation is allocated specifically to the agreement and not to the general grid.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     energy_source: EnergySource | None = pyd.Field(default=None, description="", example="Grid")
 
 
 class LightbulbsV1(BaseOpenEpdHierarchicalSpec):
-    """Lightbulbs performance specification."""
+    """Various types of light bulbs, including LED, CFL, halogen, and incandescent."""
 
     _EXT_VERSION = "1.0"
 
 
 class LightingControlsV1(BaseOpenEpdHierarchicalSpec):
-    """Lighting controls performance specification."""
+    """Devices used to control the operation of lighting, including dimmers, sensors, and smart controls."""
 
     _EXT_VERSION = "1.0"
 
 
 class LightingFixturesV1(BaseOpenEpdHierarchicalSpec):
-    """Lighting fixtures performance specification."""
+    """Permanent lighting fixtures for interior spaces, including ceiling, wall-mounted, and pendant fixtures."""
 
     _EXT_VERSION = "1.0"
 
 
 class OutdoorLightingV1(BaseOpenEpdHierarchicalSpec):
-    """Outdoor lighting performance specification."""
+    """Lighting products designed for outdoor use, including landscape and security lighting."""
 
     _EXT_VERSION = "1.0"
 
 
 class SpecialtyLightingV1(BaseOpenEpdHierarchicalSpec):
-    """Specialty lighting performance specification."""
+    """Specialized lighting for niche applications like emergency, medical, or theatrical lighting."""
 
     _EXT_VERSION = "1.0"
 
 
 class TaskLightingV1(BaseOpenEpdHierarchicalSpec):
-    """Task lighting performance specification."""
+    """Lighting designed for specific tasks such as desk lamps, under-cabinet lighting, and reading lamps."""
 
     _EXT_VERSION = "1.0"
 
 
 class ElectricalPowerStorageV1(BaseOpenEpdHierarchicalSpec):
-    """Electrical power storage performance specification."""
+    """Electrical Power Storage."""
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
     Batteries: BatteriesV1 | None = None
     OtherElectricalPowerStorage: OtherElectricalPowerStorageV1 | None = None
 
 
 class LowVoltageElectricalDistributionV1(BaseOpenEpdHierarchicalSpec):
-    """Low voltage electrical distribution performance specification."""
+    """Low Voltage Electrical Distribution."""
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
     CableTrays: CableTraysV1 | None = None
     ElectricalBuses: ElectricalBusesV1 | None = None
     FloorEquipmentBoxes: FloorEquipmentBoxesV1 | None = None
     PowerDistributionUnits: PowerDistributionUnitsV1 | None = None
     Raceways: RacewaysV1 | None = None
 
 
 class ElectricalGenerationEquipmentV1(BaseOpenEpdHierarchicalSpec):
-    """Electrical generation equipment performance specification."""
+    """
+    Equipment for generating electrical power.
+
+    This category is primarily for smaller-scale. (e.g. on premises) generation, rather than utility-scale equipment.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
     FueledElectricalGenerators: FueledElectricalGeneratorsV1 | None = None
     OtherGeneration: OtherGenerationV1 | None = None
     Photovoltaics: PhotovoltaicsV1 | None = None
     WindTurbines: WindTurbinesV1 | None = None
 
 
 class ElectricPowerV1(BaseOpenEpdHierarchicalSpec):
-    """Electric power performance specification."""
+    """Electrical energy drawn from a utility grid."""
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
     ElectricityFromPowerGrid: ElectricityFromPowerGridV1 | None = None
     ElectricityFromSpecificGenerator: ElectricityFromSpecificGeneratorV1 | None = None
     PowerPurchaseAgreements: PowerPurchaseAgreementsV1 | None = None
 
 
 class LightingV1(BaseOpenEpdHierarchicalSpec):
-    """Lighting performance specification."""
+    """Lamps and lightbulbs and lamp components."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     color_temperature: ColorTemperatureStr | None = pyd.Field(default=None, description="", example="1 K")
     typical_utilization: str | None = pyd.Field(default=None, description="", example="1 h / yr")
     luminosity: LuminosityStr | None = pyd.Field(default=None, description="", example="1 lumen")
@@ -278,15 +291,15 @@
     LightingFixtures: LightingFixturesV1 | None = None
     OutdoorLighting: OutdoorLightingV1 | None = None
     SpecialtyLighting: SpecialtyLightingV1 | None = None
     TaskLighting: TaskLightingV1 | None = None
 
 
 class ElectricalV1(BaseOpenEpdHierarchicalSpec):
-    """Electrical performance specification."""
+    """Electric power and equipment."""
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
     ElectricalPowerStorage: ElectricalPowerStorageV1 | None = None
     LowVoltageElectricalDistribution: LowVoltageElectricalDistributionV1 | None = None
     ElectricalGenerationEquipment: ElectricalGenerationEquipmentV1 | None = None
```

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/electrical_transmission_and_distribution_equipment.py` & `openepd-3.2.0/src/openepd/model/specs/generated/electrical_transmission_and_distribution_equipment.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,45 +17,49 @@
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
 
 
 class AcTransformersV1(BaseOpenEpdHierarchicalSpec):
-    """AC transformers performance specification."""
+    """Equipment for transforming between higher and lower voltage AC power."""
 
     _EXT_VERSION = "1.0"
 
 
 class ElectricalInsulatorsV1(BaseOpenEpdHierarchicalSpec):
-    """Electrical insulators performance specification."""
+    """Passive electrical isolation."""
 
     _EXT_VERSION = "1.0"
 
 
 class ElectricalSubstationsV1(BaseOpenEpdHierarchicalSpec):
     """Electrical substations performance specification."""
 
     _EXT_VERSION = "1.0"
 
 
 class ElectricalSwitchgearV1(BaseOpenEpdHierarchicalSpec):
-    """Electrical switchgear performance specification."""
+    """
+    Equipment for interrupting and controlling high-power electrical flows.
+
+    Used for protection, isolation, or control of electrical equipment.
+    """
 
     _EXT_VERSION = "1.0"
 
 
 class PowerCablingV1(BaseOpenEpdHierarchicalSpec):
-    """Power cabling performance specification."""
+    """High-voltage electrical cabling."""
 
     _EXT_VERSION = "1.0"
 
 
 class ElectricalTransmissionAndDistributionEquipmentV1(BaseOpenEpdHierarchicalSpec):
-    """Electrical transmission and distribution equipment performance specification."""
+    """Electrical Transmission & Distribution Equipment."""
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
     AcTransformers: AcTransformersV1 | None = None
     ElectricalInsulators: ElectricalInsulatorsV1 | None = None
     ElectricalSubstations: ElectricalSubstationsV1 | None = None
```

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/electricity.py` & `openepd-3.2.0/src/openepd/model/specs/generated/electricity.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,10 +17,10 @@
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
 
 
 class ElectricityV1(BaseOpenEpdHierarchicalSpec):
-    """Electricity performance specification."""
+    """Electrical equipment and components and supplies."""
 
     _EXT_VERSION = "1.0"
```

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/enums.py` & `openepd-3.2.0/src/openepd/model/specs/generated/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,21 +197,23 @@
     """
     Gypsum fire rating.
 
      - -: -
      - X: X
      - C: C
      - F: F
+     - Other: Not one of the listed options
 
     """
 
     REGULAR = "-"
     X = "X"
     C = "C"
     F = "F"
+    OTHER = "Other"
 
 
 class MembraneRoofingReinforcement(StrEnum):
     """
     Membrane roofing reinforcement.
 
      - Polyester: Polyester
```

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/finishes.py` & `openepd-3.2.0/src/openepd/model/specs/generated/finishes.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,15 +56,20 @@
     validate_quantity_ge_factory,
     validate_quantity_le_factory,
     validate_unit_factory,
 )
 
 
 class AccessFlooringV1(BaseOpenEpdHierarchicalSpec):
-    """Access flooring performance specification."""
+    """
+    Elevated floor system built on top of concrete slab surface.
+
+    It thereby creates a hidden void between the two floors that is used for the passage of mechanical and electrical
+    services. The system consists of panels, stringers, and pedestals.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     core_material: AccessFlooringCoreMaterial | None = pyd.Field(default=None, description="", example="Cementitious")
     finish_material: AccessFlooringFinishMaterial | None = pyd.Field(default=None, description="", example="Linoleum")
     stringers: AccessFlooringStringers | None = pyd.Field(default=None, description="", example="Standard")
@@ -86,15 +91,15 @@
     )(validate_unit_factory("N"))
     _access_flooring_rolling_load_10000_pass_is_quantity_validator = pyd.validator(
         "rolling_load_10000_pass", allow_reuse=True
     )(validate_unit_factory("N"))
 
 
 class CarpetV1(BaseOpenEpdHierarchicalSpec):
-    """Carpet performance specification."""
+    """Textile Floor Coverings."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     length: LengthMStr | None = pyd.Field(default=None, description="", example="1 m")
     width: LengthMStr | None = pyd.Field(default=None, description="", example="1 m")
     intended_application: list[CarpetIntendedApplication] | None = pyd.Field(
@@ -113,27 +118,31 @@
     gwp_factor_yarn: GwpKgCo2eStr | None = pyd.Field(default=None, description="", example="1 kgCO2e")
 
     _yarn_weight_is_quantity_validator = pyd.validator("yarn_weight", allow_reuse=True)(validate_unit_factory("g / m2"))
     _yarn_weight_ge_validator = pyd.validator("yarn_weight", allow_reuse=True)(validate_quantity_ge_factory("0 g / m2"))
 
 
 class LaminateV1(BaseOpenEpdHierarchicalSpec):
-    """Laminate performance specification."""
+    """Laminate flooring."""
 
     _EXT_VERSION = "1.0"
 
 
 class OtherFlooringV1(BaseOpenEpdHierarchicalSpec):
-    """Other flooring performance specification."""
+    """Other not yet classified kinds of flooring."""
 
     _EXT_VERSION = "1.0"
 
 
 class ResilientFlooringV1(BaseOpenEpdHierarchicalSpec):
-    """Resilient flooring performance specification."""
+    """
+    Resilient floor products.
+
+    Includes vinyl, rubber, linoleum, composition cork, etc. in modular square or rectangle shapes.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     length: LengthMStr | None = pyd.Field(default=None, description="", example="1 m")
     width: LengthMStr | None = pyd.Field(default=None, description="", example="1 m")
     form_factor: ResilientFlooringFormFactor | None = pyd.Field(default=None, description="", example="Loose Lay")
@@ -146,45 +155,50 @@
     conductive_flooring: bool | None = pyd.Field(default=None, description="", example=True)
     zwtl: bool | None = pyd.Field(default=None, description="", example=True)
     floor_score: bool | None = pyd.Field(default=None, description="", example=True)
     nsf332: bool | None = pyd.Field(default=None, description="", example=True)
 
 
 class WallBaseV1(BaseOpenEpdHierarchicalSpec):
-    """Wall base performance specification."""
+    """Wall base made to help cover gaps between wall and vinyl, rubber, wood, or tile flooring."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     wall_base_material: WallBaseMaterial | None = pyd.Field(default=None, description="", example="Rubber")
 
 
 class WoodFlooringV1(BaseOpenEpdHierarchicalSpec, HasForestPracticesCertifiers):
-    """Wood flooring performance specification."""
+    """
+    Wood flooring for interior applications.
+
+    Includes hardwood strip and plank flooring, engineered hardwood flooring, wood parquet flooring, coordinated
+    transitions, and molding pieces.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     thickness: LengthMmStr | None = pyd.Field(default=None, description="", example="10 mm")
     timber_species: WoodFlooringTimberSpecies | None = pyd.Field(default=None, description="", example="Oak")
     fabrication: WoodFlooringFabrication | None = pyd.Field(default=None, description="", example="Solid hardwood")
     forest_practices_certifiers: list[OrgRef] | None = pyd.Field(default=None, description="")
 
 
 class AcousticalCeilingsV1(BaseOpenEpdHierarchicalSpec):
-    """Acoustical ceilings performance specification."""
+    """Acoustical ceiling panels."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     thickness: LengthMmStr | None = pyd.Field(default=None, description="", example="10 mm")
 
 
 class CeramicTileV1(BaseOpenEpdHierarchicalSpec):
-    """Ceramic tile performance specification."""
+    """Ceramic tiles, including porcelain, quarry, pressed floor tile, wall tile, mosaic tile, etc."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     porcelain: bool | None = pyd.Field(
         default=None, description="A dense and durable ceramic tile made from fine porcelain clay.", example=True
     )
@@ -215,15 +229,19 @@
         description="A unique and customized type of tile, often made from unconventional materials or with "
         "specialized designs or finishes.",
         example=True,
     )
 
 
 class GaugedTileV1(BaseOpenEpdHierarchicalSpec):
-    """Gauged tile performance specification."""
+    """
+    Specially manufactured porcelain tile with extra-large panels/slabs.
+
+    Manufactured to a specific thickness ranging from 2-20 mm.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     tile_panels: bool | None = pyd.Field(
         default=None,
         description="Large-format porcelain or natural stone tiles that are typically over 3 feet in length and width, "
@@ -237,15 +255,15 @@
         "applications, such as patios, walkways, and driveways, due to their high resistance to weather "
         "and wear.",
         example=True,
     )
 
 
 class GlassTileV1(BaseOpenEpdHierarchicalSpec):
-    """Glass tile performance specification."""
+    """Glass Tiles."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     regular: bool | None = pyd.Field(
         default=None,
         description="Glass tile that is typically square or rectangular in shape, and used for a variety of "
@@ -269,36 +287,36 @@
         description="Glass tile that is larger in size than regular glass tile, often used to create a dramatic and "
         "modern effect in commercial and residential spaces.",
         example=True,
     )
 
 
 class GypsumSupportsV1(BaseOpenEpdHierarchicalSpec):
-    """Gypsum supports performance specification."""
+    """Supports for suspended and furred gypsum wall and ceiling assemblies."""
 
     _EXT_VERSION = "1.0"
 
 
 class FlooringV1(BaseOpenEpdHierarchicalSpec):
-    """Flooring performance specification."""
+    """General category - finishes for floors."""
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
     AccessFlooring: AccessFlooringV1 | None = None
     Carpet: CarpetV1 | None = None
     Laminate: LaminateV1 | None = None
     OtherFlooring: OtherFlooringV1 | None = None
     ResilientFlooring: ResilientFlooringV1 | None = None
     WallBase: WallBaseV1 | None = None
     WoodFlooring: WoodFlooringV1 | None = None
 
 
 class CeilingPanelV1(BaseOpenEpdHierarchicalSpec):
-    """Ceiling panel performance specification."""
+    """Acoustical and other specialty ceiling panels."""
 
     _EXT_VERSION = "1.0"
     """Modular Ceiling Panels"""
 
     # Own fields:
     fire_rating: CeilingPanelFireRating | None = pyd.Field(default=None, description="", example="Class A")
     core_material: CeilingPanelCoreMaterial | None = pyd.Field(default=None, description="", example="Fiberglass")
@@ -314,36 +332,40 @@
     )
 
     # Nested specs:
     AcousticalCeilings: AcousticalCeilingsV1 | None = None
 
 
 class BackingAndUnderlayV1(BaseOpenEpdHierarchicalSpec):
-    """Backing and underlay performance specification."""
+    """Cementitious, glass-mat faced gypsum, and fibered gypsum backing boards to support finish materials."""
 
     _EXT_VERSION = "1.0"
 
 
 class CementBoardV1(BaseOpenEpdHierarchicalSpec):
-    """Cement board performance specification."""
+    """Hard cementitious boards, typically used as a tile backer."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     thickness: CementBoardThickness | None = pyd.Field(
         default=None, description="", example=str(CementBoardThickness.INCH_1_2)
     )
 
     _cement_board_thickness_is_quantity_validator = pyd.validator("thickness", allow_reuse=True)(
         validate_unit_factory("m")
     )
 
 
 class TilingV1(BaseOpenEpdHierarchicalSpec):
-    """Tiling performance specification."""
+    """
+    Decorative building materials that includes a variety of ceramic, porcelain, and glass tiles.
+
+    Used for covering and enhancing surfaces such as floors, walls, and countertops.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     thickness: LengthMmStr | None = pyd.Field(default=None, description="", example="9 mm")
     flooring: bool | None = pyd.Field(default=None, description="Tiling intended for walking.", example=True)
     wall_finish: bool | None = pyd.Field(
@@ -394,38 +416,38 @@
     # Nested specs:
     CeramicTile: CeramicTileV1 | None = None
     GaugedTile: GaugedTileV1 | None = None
     GlassTile: GlassTileV1 | None = None
 
 
 class DeckingBoardsV1(BaseOpenEpdHierarchicalSpec, HasForestPracticesCertifiers):
-    """Decking boards performance specification."""
+    """Decking boards provide the finished surface of a deck and support the weight of people and furniture."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     timber_species: SawnTimberSpecies | None = pyd.Field(default=None, description="", example="Alaska Cedar")
     fabrication: AllFabrication | None = pyd.Field(default=None, description="", example="LVL")
     forest_practices_certifiers: list[OrgRef] | None = pyd.Field(default=None, description="")
     weather_exposed: bool | None = pyd.Field(default=None, description="", example=True)
     fire_retardant: bool | None = pyd.Field(default=None, description="", example=True)
     decay_resistant: bool | None = pyd.Field(default=None, description="", example=True)
     material: DeckingBoardMaterial | None = pyd.Field(default=None, description="", example="Wood")
 
 
 class GlassFiberReinforcedGypsumFabricationsV1(BaseOpenEpdHierarchicalSpec):
-    """Glass fiber reinforced gypsum fabrications performance specification."""
+    """Gypsum with integrated glass fiber reinforcement, which may be fabricated in complex shapes or as a board."""
 
     _EXT_VERSION = "1.0"
 
 
 class GypsumV1(BaseOpenEpdHierarchicalSpec):
-    """Gypsum Sheet and Board."""
+    """Gypsum board used for interior walls, ceilings, and similar applications."""
 
-    _EXT_VERSION = "1.0"
+    _EXT_VERSION = "1.1"
 
     # Own fields:
     fire_rating: GypsumFireRating | None = pyd.Field(default=None, description="", example="-")
     thickness: GypsumThickness | None = pyd.Field(default=None, description="", example="1 m")
     facing: GypsumFacing | None = pyd.Field(default=None, description="", example="Paper")
     r_factor: str | None = pyd.Field(default=None, description="", example="1 RSI")
     flame_spread_astm_e84: int | None = pyd.Field(default=None, description="", example=3)
@@ -442,36 +464,36 @@
     _gypsum_r_factor_is_quantity_validator = pyd.validator("r_factor", allow_reuse=True)(validate_unit_factory("RSI"))
 
     # Nested specs:
     GypsumSupports: GypsumSupportsV1 | None = None
 
 
 class MirrorsV1(BaseOpenEpdHierarchicalSpec):
-    """Mirrors performance specification."""
+    """Mirrors."""
 
     _EXT_VERSION = "1.0"
 
 
 class PaintingAndCoatingV1(BaseOpenEpdHierarchicalSpec):
-    """Painting and coating performance specification."""
+    """Paintings and coatings."""
 
     _EXT_VERSION = "1.0"
 
 
 class WallFinishesV1(BaseOpenEpdHierarchicalSpec):
-    """Wall finishes performance specification."""
+    """Interior wall coverings including fabric, textile, wood, stone, and metal products."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     thickness: LengthMmStr | None = pyd.Field(default=None, description="", example="10 mm")
 
 
 class FinishesV1(BaseOpenEpdHierarchicalSpec):
-    """Finishes performance specification."""
+    """General category - finishes for interior ceilings, floors, walls."""
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
     Flooring: FlooringV1 | None = None
     CeilingPanel: CeilingPanelV1 | None = None
     BackingAndUnderlay: BackingAndUnderlayV1 | None = None
```

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/fire_and_smoke_protection.py` & `openepd-3.2.0/src/openepd/model/specs/generated/fire_and_smoke_protection.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,54 +24,76 @@
     SprayFireproofingDensity,
     SprayFireproofingMaterialType,
 )
 from openepd.model.validation.quantity import LengthMmStr
 
 
 class IntumescentFireproofingV1(BaseOpenEpdHierarchicalSpec):
-    """Intumescent fireproofing performance specification."""
+    """
+    Fireproofing material applied to structural materials, which swells as a result of heat exposure.
+
+    As a result it increases in volume and decreasing in density.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     material_type: IntumescentFireproofingMaterialType | None = pyd.Field(default=None, description="", example="Epoxy")
 
 
 class SprayFireproofingV1(BaseOpenEpdHierarchicalSpec):
-    """Spray fireproofing performance specification."""
+    """
+    Spray fireproofing.
+
+    A passive fire protection system that reduces the rate of temperature increase in concrete or steel during a fire.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     material_type: SprayFireproofingMaterialType | None = pyd.Field(
         default=None, description="", example="Gypsum-based"
     )
     density: SprayFireproofingDensity | None = pyd.Field(default=None, description="", example="Standard")
 
 
 class AppliedFireproofingV1(BaseOpenEpdHierarchicalSpec):
-    """Applied fireproofing performance specification."""
+    """
+    Fireproofing material applied to structural materials.
+
+    Materials include: cement aggregate, cementitious, magnesium-oxychloride, intumescent, magnesium cement, mineral
+    fiber, and mineral fiber fireproofing products.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     thickness: LengthMmStr | None = pyd.Field(default=None, description="", example="10 mm")
 
     # Nested specs:
     IntumescentFireproofing: IntumescentFireproofingV1 | None = None
     SprayFireproofing: SprayFireproofingV1 | None = None
 
 
 class FirestoppingV1(BaseOpenEpdHierarchicalSpec):
-    """Firestopping performance specification."""
+    """
+    Seals and protects openings and joints in fire rate assemblies.
+
+    Typically sealants, sprays, and caulks.
+    """
 
     _EXT_VERSION = "1.0"
 
 
 class FireAndSmokeProtectionV1(BaseOpenEpdHierarchicalSpec):
-    """Fire and smoke protection performance specification."""
+    """
+    Fire and smoke protection.
+
+    General category of materials whose function is to provide protection of materials, spaces, and occupants from
+    fire and smoke damage.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
     AppliedFireproofing: AppliedFireproofingV1 | None = None
     Firestopping: FirestoppingV1 | None = None
```

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/furnishings.py` & `openepd-3.2.0/src/openepd/model/specs/generated/furnishings.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,70 +20,70 @@
 from openepd.compat.pydantic import pyd
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
 from openepd.model.specs.generated.enums import CountertopMaterial
 from openepd.model.validation.quantity import LengthMmStr
 
 
 class DemountablePartitionTrackV1(BaseOpenEpdHierarchicalSpec):
-    """Demountable partition track performance specification."""
+    """Track for modular partitions."""
 
     _EXT_VERSION = "1.0"
 
 
 class ChairsV1(BaseOpenEpdHierarchicalSpec):
-    """Chairs performance specification."""
+    """Chairs."""
 
     _EXT_VERSION = "1.0"
 
 
 class CountertopsV1(BaseOpenEpdHierarchicalSpec):
-    """Countertops performance specification."""
+    """Raised, flat, and horizontal surfaces often used in kitchens, bathrooms, and workrooms."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     thickness: LengthMmStr | None = pyd.Field(default=None, description="", example="30 mm")
     countertop_material: CountertopMaterial | None = pyd.Field(default=None, description="", example="Stone")
 
 
 class DemountablePartitionsV1(BaseOpenEpdHierarchicalSpec):
-    """Demountable partitions performance specification."""
+    """Demountable partitions."""
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
     DemountablePartitionTrack: DemountablePartitionTrackV1 | None = None
 
 
 class OtherFurnishingsV1(BaseOpenEpdHierarchicalSpec):
-    """Other furnishings performance specification."""
+    """Other furnishings."""
 
     _EXT_VERSION = "1.0"
 
 
 class StorageFurnitureV1(BaseOpenEpdHierarchicalSpec):
-    """Storage furniture performance specification."""
+    """Storage Furniture."""
 
     _EXT_VERSION = "1.0"
 
 
 class TablesV1(BaseOpenEpdHierarchicalSpec):
-    """Tables performance specification."""
+    """Tables."""
 
     _EXT_VERSION = "1.0"
 
 
 class WorkSurfacesV1(BaseOpenEpdHierarchicalSpec):
-    """Work surfaces performance specification."""
+    """Work surfaces."""
 
     _EXT_VERSION = "1.0"
 
 
 class FurnishingsV1(BaseOpenEpdHierarchicalSpec):
-    """Furnishings performance specification."""
+    """Home and office furnishings."""
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
     Chairs: ChairsV1 | None = None
     Countertops: CountertopsV1 | None = None
     DemountablePartitions: DemountablePartitionsV1 | None = None
```

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/grouting.py` & `openepd-3.2.0/src/openepd/model/validation/numbers.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
+from typing import Annotated
 
+from openepd.compat.pydantic import pyd
 
-class GroutingV1(BaseOpenEpdHierarchicalSpec):
-    """Grouting performance specification."""
-
-    _EXT_VERSION = "1.0"
+# todo when move to pydantic 2, check that validators are being enforced.
+RatioFloat = Annotated[float, pyd.Field(ge=0, le=1, example=0.5)]
+PositiveInt = Annotated[int, pyd.Field(ge=0, example=1)]
```

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/manufacturing_inputs.py` & `openepd-3.2.0/src/openepd/model/specs/generated/manufacturing_inputs.py`

 * *Files 17% similar despite different names*

```diff
@@ -30,48 +30,61 @@
     CementScm,
     MasonryCementAstmC91Type,
     TextilesFabricType,
 )
 
 
 class CementV1(BaseOpenEpdHierarchicalSpec):
-    """Cement performance specification."""
+    """
+    Cements.
+
+    Includes Portland and blended cements, that can serve as the primary binder in a concrete mix.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     cementitious: Cementitious | None = pyd.Field(default=None, description="")
     white_cement: bool | None = pyd.Field(default=None, description="", example=True)
     astm_type: CementAstmType | None = pyd.Field(default=None, description="", example="C150 Type I")
     c1157: list[CementC1157] | None = pyd.Field(default=None, description="", example=["GU"])
     csa_a3001: list[CementCsaA3001] | None = pyd.Field(default=None, description="", example=["A3001 GU"])
     en197_1: CementEn197_1 | None = pyd.Field(default=None, description="", example="CEM I")
     oil_well_cement: bool | None = pyd.Field(default=None, description="", example=True)
 
 
 class MasonryCementV1(BaseOpenEpdHierarchicalSpec):
-    """Masonry cement performance specification."""
+    """
+    A cementitious product typically composed of Portland cement and hydrated lime.
+
+    Masonry cement is combined with sand to make mortar.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     astm_c91_type: MasonryCementAstmC91Type | None = pyd.Field(default=None, description="", example="Type N")
 
 
 class SupplementaryCementitiousMaterialsV1(BaseOpenEpdHierarchicalSpec):
-    """Supplementary cementitious materials performance specification."""
+    """Cementitious materials that are not effective binders when used on their own."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     cement_scm: list[CementScm] | None = pyd.Field(default=None, description="", example=["ggbs"])
 
 
 class AccessFlooringPedestalsV1(BaseOpenEpdHierarchicalSpec):
-    """Access flooring pedestals performance specification."""
+    """
+    Part of an access floor system.
+
+    Pedestals are laid out on top of a floor slab and support access floor panels, creating a void space between the
+    floor slab and finish floor.
+    """
 
     _EXT_VERSION = "1.0"
 
 
 class CarpetBackingV1(BaseOpenEpdHierarchicalSpec):
     """Fabric backing holding a carpet together."""
 
@@ -96,33 +109,44 @@
     # Nested specs:
     Cement: CementV1 | None = None
     MasonryCement: MasonryCementV1 | None = None
     SupplementaryCementitiousMaterials: SupplementaryCementitiousMaterialsV1 | None = None
 
 
 class ConcreteAdmixturesV1(BaseOpenEpdHierarchicalSpec):
-    """Concrete admixtures performance specification."""
+    """
+    Concrete admixtures.
+
+    Chemical additives that are added to fresh concrete immediately before or during mixing. Admixtures have distinct
+    functions and are categorized as: air-entraining, water-reducing, retarding, accelerating, and plasticizers
+    (i.e., superplasticizers).
+    """
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     effects: list[AdmixtureEffects] | None = pyd.Field(default=None, description="", example=["Air Entrainer"])
 
 
 class TextilesV1(BaseOpenEpdHierarchicalSpec):
-    """Textiles performance specification."""
+    """Textiles for use in manufacturing end products."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     fabric_type: list[TextilesFabricType] | None = pyd.Field(default=None, description="", example=["Leather"])
 
 
 class ManufacturingInputsV1(BaseOpenEpdHierarchicalSpec):
-    """Manufacturing inputs performance specification."""
+    """
+    Manufacturing inputs.
+
+    Broad category for collecting materials primarily used as manufacturing inputs, rather than directly used in
+    a construction.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
     AccessFlooringPedestals: AccessFlooringPedestalsV1 | None = None
     CarpetBacking: CarpetBackingV1 | None = None
     CarpetFiber: CarpetFiberV1 | None = None
```

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/masonry.py` & `openepd-3.2.0/src/openepd/model/specs/generated/masonry.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,21 +19,21 @@
 #
 from openepd.compat.pydantic import pyd
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
 from openepd.model.validation.quantity import PressureMPaStr, validate_quantity_ge_factory, validate_unit_factory
 
 
 class GMUV1(BaseOpenEpdHierarchicalSpec):
-    """Glass Masonry Unit performance specification."""
+    """Glass masonry unit."""
 
     _EXT_VERSION = "1.0"
 
 
 class AutoclavedAeratedConcreteV1(BaseOpenEpdHierarchicalSpec):
-    """Autoclaved aerated concrete performance specification."""
+    """A lightweight, precast, foamed concrete masonry building material."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     strength_28d: PressureMPaStr | None = pyd.Field(default=None, description="", example="1 MPa")
     thermal_conductivity: str | None = pyd.Field(default=None, description="", example="1 W / (m * K)")
     white: bool | None = pyd.Field(default=None, description="", example=True)
@@ -44,15 +44,15 @@
 
     _aac_thermal_conductivity_min_validator = pyd.validator("thermal_conductivity", allow_reuse=True)(
         validate_quantity_ge_factory("0 W / (m * K)")
     )
 
 
 class BrickV1(BaseOpenEpdHierarchicalSpec):
-    """Brick performance specification."""
+    """Solid masonry units made from clay or shale."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     building: bool | None = pyd.Field(default=None, description="", example=True)
     facing: bool | None = pyd.Field(default=None, description="", example=True)
     floor: bool | None = pyd.Field(default=None, description="", example=True)
@@ -61,15 +61,15 @@
     other: bool | None = pyd.Field(default=None, description="", example=True)
     chemical_resistant: bool | None = pyd.Field(default=None, description="", example=True)
     glazed: bool | None = pyd.Field(default=None, description="", example=True)
     tiles: bool | None = pyd.Field(default=None, description="", example=True)
 
 
 class MasonryV1(BaseOpenEpdHierarchicalSpec):
-    """Masonry performance specification."""
+    """Structural and/or enclosure system based on individual rigid units stacked and bound together with mortar."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     white_cement: bool | None = pyd.Field(default=None, description="", example=True)
 
     # Nested specs:
```

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/material_handling.py` & `openepd-3.2.0/src/openepd/model/specs/generated/material_handling.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,19 +17,27 @@
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
 
 
 class ConveyorsV1(BaseOpenEpdHierarchicalSpec):
-    """Conveyors performance specification."""
+    """
+    Machinery and tools designed to move materials within a facility, both manually and automatically.
+
+    This includes various types of conveyors such as belt, roller, and overhead conveyors.
+    """
 
     _EXT_VERSION = "1.0"
 
 
 class MaterialHandlingV1(BaseOpenEpdHierarchicalSpec):
-    """Material handling performance specification."""
+    """
+    Material handling.
+
+    Equipment and supplies for moving, storing, administering, and protecting materials during the handling process.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
     Conveyors: ConveyorsV1 | None = None
```

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/mechanical.py` & `openepd-3.2.0/src/openepd/model/specs/generated/mechanical.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,63 +31,68 @@
     MechanicalInstallation,
     MechanicalRefrigerants,
 )
 from openepd.model.validation.quantity import AirflowStr, FlowRateStr, PowerStr, PressureMPaStr, VolumeStr
 
 
 class HvacVrfControlV1(BaseOpenEpdHierarchicalSpec):
-    """Hvac vrf control performance specification."""
+    """Controller for adjusting airflow across the VRF system."""
 
     _EXT_VERSION = "1.0"
 
 
 class HvacVrfIndoorV1(BaseOpenEpdHierarchicalSpec):
-    """Hvac vrf indoor performance specification."""
+    """Heating and cooling unit located on the inside of a building and supplies air to specific indoor zones."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     refrigerants: list[MechanicalRefrigerants] | None = pyd.Field(default=None, description="", example=["R11"])
     heating_capacity: PowerStr | None = pyd.Field(default=None, description="", example="1000.0 W")
     cooling_capacity: PowerStr | None = pyd.Field(default=None, description="", example="1000.0 W")
     airflow_rate: AirflowStr | None = pyd.Field(default=None, description="", example="1 m3 / s")
     air_volume: VolumeStr | None = pyd.Field(default=None, description="", example="1 m3")
 
 
 class HvacVrfOutdoorV1(BaseOpenEpdHierarchicalSpec):
-    """Hvac vrf outdoor performance specification."""
+    """Heating and cooling unit that is on the outside of a building and distributes air to the indoor units."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     refrigerants: list[MechanicalRefrigerants] | None = pyd.Field(default=None, description="", example=["R11"])
     heating_capacity: PowerStr | None = pyd.Field(default=None, description="", example="1000.0 W")
     cooling_capacity: PowerStr | None = pyd.Field(default=None, description="", example="1000.0 W")
     airflow_rate: AirflowStr | None = pyd.Field(default=None, description="", example="1 m3 / s")
     air_volume: VolumeStr | None = pyd.Field(default=None, description="", example="1 m3")
 
 
 class HvacAirDiffusersV1(BaseOpenEpdHierarchicalSpec):
-    """Hvac air diffusers performance specification."""
+    """Room-side terminals for air distribution. This is different from Terminal Heating & Cooling Units."""
 
     _EXT_VERSION = "1.0"
 
 
 class HvacAirFiltersV1(BaseOpenEpdHierarchicalSpec):
-    """Hvac air filters performance specification."""
+    """Device for filtering particles of dust, soot, etc., from the air passing through it."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     merv_rating: AirFiltersMervRating | None = pyd.Field(default=None, description="", example="MERV 1")
     media_type: AirFiltersMediaType | None = pyd.Field(default=None, description="", example="Acrylic")
 
 
 class HvacAHUsV1(BaseOpenEpdHierarchicalSpec):
-    """Hvac a h us performance specification."""
+    """
+    Device which provides healthy, dust free air to buildings with a good energy efficiency.
+
+    Usually a large metal box containing a blower, heating or cooling elements, filter racks or chambers, sound
+    attenuators, and dampers.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     refrigerants: list[MechanicalRefrigerants] | None = pyd.Field(default=None, description="", example=["R11"])
     installation: MechanicalInstallation | None = pyd.Field(default=None, description="", example="Indoor")
     airflow_rate: AirflowStr | None = pyd.Field(default=None, description="", example="1 m3 / s")
@@ -95,90 +100,110 @@
     cooling_capacity: PowerStr | None = pyd.Field(default=None, description="", example="1000.0 W")
     heating_capacity: PowerStr | None = pyd.Field(default=None, description="", example="1000.0 W")
     airflow_control: AhuAirflowControl | None = pyd.Field(default=None, description="", example="CAV")
     zone_control: AhuZoneControl | None = pyd.Field(default=None, description="", example="Single Zone")
 
 
 class HvacBoilersV1(BaseOpenEpdHierarchicalSpec):
-    """Hvac boilers performance specification."""
+    """Closed vessel for heating fluid."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     flow_rate: FlowRateStr | None = pyd.Field(default=None, description="", example="1 l / min")
     heating_capacity: PowerStr | None = pyd.Field(default=None, description="", example="1000.0 W")
     configuration: BoilerConfiguration | None = pyd.Field(default=None, description="", example="Hot water")
     fuel_type: BoilerEquipmentFuelType | None = pyd.Field(default=None, description="", example="Coal")
 
 
 class HvacChillersV1(BaseOpenEpdHierarchicalSpec):
-    """Hvac chillers performance specification."""
+    """
+    Machine that removes heat from a liquid coolant.
+
+    Uses a vapor-compression, adsorption refrigeration, or absorption refrigeration cycles. Incldues centrifugal,
+    water-cooled chillers, etc.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     refrigerants: list[MechanicalRefrigerants] | None = pyd.Field(default=None, description="", example=["R11"])
     installation: MechanicalInstallation | None = pyd.Field(default=None, description="", example="Indoor")
     heating_capacity: PowerStr | None = pyd.Field(default=None, description="", example="1000.0 W")
     cooling_capacity: PowerStr | None = pyd.Field(default=None, description="", example="1000.0 W")
     air_volume: VolumeStr | None = pyd.Field(default=None, description="", example="1 m3")
     airflow_rate: AirflowStr | None = pyd.Field(default=None, description="", example="1 m3 / s")
 
 
 class HvacFansV1(BaseOpenEpdHierarchicalSpec):
-    """Hvac fans performance specification."""
+    """Apparatus with rotating blades that creates a current of air for cooling or ventilation."""
 
     _EXT_VERSION = "1.0"
 
 
 class HvacHeatPumpsV1(BaseOpenEpdHierarchicalSpec):
-    """Hvac heat pumps performance specification."""
+    """Device that transfers thermal energy between spaces, including ground and air source heat pumps."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     refrigerants: list[MechanicalRefrigerants] | None = pyd.Field(default=None, description="", example=["R11"])
     cooling_capacity: PowerStr | None = pyd.Field(default=None, description="", example="1000.0 W")
     heating_capacity: PowerStr | None = pyd.Field(default=None, description="", example="1000.0 W")
     air_volume: VolumeStr | None = pyd.Field(default=None, description="", example="1 m3")
     airflow_rate: AirflowStr | None = pyd.Field(default=None, description="", example="1 m3 / s")
     heat_pumps_type: HeatPumpType | None = pyd.Field(default=None, description="", example="Air-to-Water")
 
 
 class HvacHeatExV1(BaseOpenEpdHierarchicalSpec):
-    """Hvac heat exchangers performance specification."""
+    """
+    HVAC heat exchangers.
+
+    Systems that with heat exchange cell which recovers and retains the heat that would otherwise be lost from the
+    extracted air.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     refrigerants: list[MechanicalRefrigerants] | None = pyd.Field(default=None, description="", example=["R11"])
     heat_exchangers_type: HvacHeatExchangersType | None = pyd.Field(
         default=None, description="", example="Shell and Tube"
     )
 
 
 class HvacPumpsV1(BaseOpenEpdHierarchicalSpec):
-    """Hvac pumps performance specification."""
+    """
+    Pumps.
+
+    Mechanical device using suction or pressure to raise or move liquids, compress gases, or force air into
+    inflatable objects such as tires.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     flow_rate: FlowRateStr | None = pyd.Field(default=None, description="", example="1 l / min")
     pump_discharge_pressure: PressureMPaStr | None = pyd.Field(default=None, description="", example="1 MPa")
     pump_horsepower: PowerStr | None = pyd.Field(default=None, description="", example="1000.0 W")
 
 
 class HvacRTUsV1(BaseOpenEpdHierarchicalSpec):
-    """Hvac r t us performance specification."""
+    """An air handler designed for outdoor use, typically on roofs."""
 
     _EXT_VERSION = "1.0"
 
 
 class HvacVrfSystemsV1(BaseOpenEpdHierarchicalSpec):
-    """Hvac vrf systems performance specification."""
+    """
+    Variable refrigerant flow (VRF).
+
+    Also known as variable refrigerant volume (VRV), is an HVAC technology that allows for varying degrees of cooling
+    in more specific areas.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
     HvacVrfControl: HvacVrfControlV1 | None = None
     HvacVrfIndoor: HvacVrfIndoorV1 | None = None
     HvacVrfOutdoor: HvacVrfOutdoorV1 | None = None
```

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/mechanical_insulation.py` & `openepd-3.2.0/src/openepd/model/specs/generated/mechanical_insulation.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,19 @@
 from openepd.compat.pydantic import pyd
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
 from openepd.model.specs.generated.enums import InsulatingMaterial, InsulationIntendedApplication
 from openepd.model.validation.quantity import LengthMmStr
 
 
 class MechanicalInsulationV1(BaseOpenEpdHierarchicalSpec):
-    """Mechanical insulation performance specification."""
+    """
+    Insulation products whose primary purpose is for mechanical systems rather than for building envelope.
+
+    Includes HVAC, plumbing, and acoustic insulations.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     r_value: float | None = pyd.Field(default=None, description="", example=2.3)
     material: InsulatingMaterial | None = pyd.Field(default=None, description="", example="Mineral Wool")
     intended_application: list[InsulationIntendedApplication] | None = pyd.Field(
```

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/network_infrastructure.py` & `openepd-3.2.0/src/openepd/model/specs/generated/network_infrastructure.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,41 +31,41 @@
     RacewaysMaterial,
     RackType,
 )
 from openepd.model.validation.quantity import ElectricalCurrentStr, LengthMmStr, MassKgStr, validate_unit_factory
 
 
 class PDUV1(BaseOpenEpdHierarchicalSpec):
-    """P d u performance specification."""
+    """Devices with multiple outputs designed to distribute power, often in a data center cabinet."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     amperage: ElectricalCurrentStr | None = pyd.Field(default=None, description="", example="1 A")
     outlet_level_metering: bool | None = pyd.Field(default=None, description="", example=True)
     outlet_level_switching: bool | None = pyd.Field(default=None, description="", example=True)
     pdu_technology: PduTechnology | None = pyd.Field(default=None, description="", example="Basic")
     pdu_outlets: int | None = pyd.Field(default=None, description="", example=3, le=200)
 
     _amperage_is_quantity_validator = pyd.validator("amperage", allow_reuse=True)(validate_unit_factory("A"))
 
 
 class CabinetsRacksAndEnclosuresV1(BaseOpenEpdHierarchicalSpec):
-    """Cabinets racks and enclosures performance specification."""
+    """Physical support upon which network equipment is mounted. Includes cabinets, racks, frames, and enclosures."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     static_load: MassKgStr | None = pyd.Field(default=None, description="", example="1 kg")
     total_racking_units: int | None = pyd.Field(default=None, description="", example=3)
     rack_type: RackType | None = pyd.Field(default=None, description="", example="Cabinet")
 
 
 class DataCablingV1(BaseOpenEpdHierarchicalSpec):
-    """Data cabling performance specification."""
+    """Telecommunications cabling for buildings."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     outdoor: bool | None = pyd.Field(default=None, description="", example=True)
     cabling_category: CablingCategory | None = pyd.Field(default=None, description="", example="Cat7")
     fire_rating: CablingFireRating | None = pyd.Field(default=None, description="", example="CMP")
@@ -90,15 +90,19 @@
         "have handling advantages and tend to have a reduced impact, but also reduced channel length. "
         "See TIA 568.2-D Annex G.",
         example=True,
     )
 
 
 class FloorBoxesAndAccessoriesV1(BaseOpenEpdHierarchicalSpec):
-    """Floor boxes and accessories performance specification."""
+    """
+    Electrical boxes that are installed in the floor.
+
+    Used to provide power and/or data connections to devices in a room or space.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     painted: bool | None = pyd.Field(default=None, description="", example=True)
     fire_classified: bool | None = pyd.Field(
         default=None, description="Includes hardware to maintain fire rating of the floor", example=True
@@ -121,15 +125,20 @@
     )
     material: FloorBoxMaterial | None = pyd.Field(default=None, description="", example="Metallic Box")
     cover_material: FloorBoxCoverMaterial | None = pyd.Field(default=None, description="", example="Brass")
     floor_material: FloorBoxFloorMaterial | None = pyd.Field(default=None, description="", example="Concrete")
 
 
 class NetworkingCableTraysV1(BaseOpenEpdHierarchicalSpec):
-    """Networking cable trays performance specification."""
+    """
+    Cable trays.
+
+    Mechanical support systems that provide a rigid structural system for cables used for communication and
+    power distribution.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     height: LengthMmStr | None = pyd.Field(default=None, description="", example="100 mm")
     width: LengthMmStr | None = pyd.Field(default=None, description="", example="100 mm")
     depth: LengthMmStr | None = pyd.Field(default=None, description="Depth of enclosure system", example="1 m")
@@ -137,15 +146,19 @@
     ventilated: bool | None = pyd.Field(
         default=None, description="At least 40% of the tray base is open to air flow", example=True
     )
     material: CableTraysMaterial | None = pyd.Field(default=None, description="", example="Stainless Steel")
 
 
 class NetworkingRacewaysV1(BaseOpenEpdHierarchicalSpec):
-    """Networking raceways performance specification."""
+    """
+    Surface-mounted systems along the perimeter of walls to route, conceal, and protect cables.
+
+    Often called trunking.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     width: LengthMmStr | None = pyd.Field(default=None, description="", example="100 mm")
     depth: LengthMmStr | None = pyd.Field(default=None, description="Depth of enclosure system", example="100 mm")
     painted: bool | None = pyd.Field(default=None, description="", example=True)
@@ -154,15 +167,15 @@
         description="Dual service raceway for high and low voltage data and power applications",
         example=True,
     )
     raceways_material: RacewaysMaterial | None = pyd.Field(default=None, description="", example="Aluminum")
 
 
 class NetworkInfrastructureV1(BaseOpenEpdHierarchicalSpec):
-    """Network infrastructure performance specification."""
+    """General category for network infrastructure products for data centers and commercial and residential buildings."""
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
     PDU: PDUV1 | None = None
     CabinetsRacksAndEnclosures: CabinetsRacksAndEnclosuresV1 | None = None
     DataCabling: DataCablingV1 | None = None
```

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/openings.py` & `openepd-3.2.0/src/openepd/model/specs/generated/openings.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/other_electrical_equipment.py` & `openepd-3.2.0/src/openepd/model/specs/generated/grouting.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,11 +16,16 @@
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
 
 
-class OtherElectricalEquipmentV1(BaseOpenEpdHierarchicalSpec):
-    """Other electrical equipment performance specification."""
+class GroutingV1(BaseOpenEpdHierarchicalSpec):
+    """
+    Grouting.
+
+    Water-cement-sand mixture for embedding rebar in masonry walls, connecting sections of precast concrete, and
+    filling joints and voids.
+    """
 
     _EXT_VERSION = "1.0"
```

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/plumbing.py` & `openepd-3.2.0/src/openepd/model/specs/generated/plumbing.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,117 +20,122 @@
 from openepd.compat.pydantic import pyd
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
 from openepd.model.specs.generated.enums import FireProtectionPipingMaterial, PipingAnsiSchedule, PlumbingPipingMaterial
 from openepd.model.validation.quantity import LengthMmStr, MassPerLengthStr
 
 
 class BathtubsV1(BaseOpenEpdHierarchicalSpec):
-    """Bathtubs performance specification."""
+    """Bathtubs."""
 
     _EXT_VERSION = "1.0"
 
 
 class FaucetsV1(BaseOpenEpdHierarchicalSpec):
-    """Faucets performance specification."""
+    """Faucets."""
 
     _EXT_VERSION = "1.0"
 
 
 class OtherPlumbingFixturesV1(BaseOpenEpdHierarchicalSpec):
-    """Other plumbing fixtures performance specification."""
+    """Other plumbing fixtures."""
 
     _EXT_VERSION = "1.0"
 
 
 class WaterClosetsV1(BaseOpenEpdHierarchicalSpec):
-    """Water closets performance specification."""
+    """Water Closets."""
 
     _EXT_VERSION = "1.0"
 
 
 class FireProtectionPipingV1(BaseOpenEpdHierarchicalSpec):
-    """Fire protection piping performance specification."""
+    """System of pipes used to supply fire-suppression fluids to homes and/or businesses."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     thickness: LengthMmStr | None = pyd.Field(default=None, description="", example="6 mm")
     piping_diameter: LengthMmStr | None = pyd.Field(default=None, description="", example="120 mm")
     mass_per_unit_length: MassPerLengthStr | None = pyd.Field(default=None, description="", example="1 kg / m")
     piping_ansi_schedule: PipingAnsiSchedule | None = pyd.Field(default=None, description="", example="5")
     fire_protection_piping_material: FireProtectionPipingMaterial | None = pyd.Field(
         default=None, description="", example="PVC"
     )
 
 
 class FireSprinklersV1(BaseOpenEpdHierarchicalSpec):
-    """Fire sprinklers performance specification."""
+    """Fire sprinklers."""
 
     _EXT_VERSION = "1.0"
 
 
 class StorageTanksV1(BaseOpenEpdHierarchicalSpec):
-    """Storage tanks performance specification."""
+    """Storage tanks."""
 
     _EXT_VERSION = "1.0"
 
 
 class WaterHeatersV1(BaseOpenEpdHierarchicalSpec):
-    """Water heaters performance specification."""
+    """Water heaters."""
 
     _EXT_VERSION = "1.0"
 
 
 class PlumbingFixturesV1(BaseOpenEpdHierarchicalSpec):
-    """Plumbing fixtures performance specification."""
+    """Residential and commercial water closets, urinals, lavatories, sinks, bathtubs, showers, faucets, etc."""
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
     Bathtubs: BathtubsV1 | None = None
     Faucets: FaucetsV1 | None = None
     OtherPlumbingFixtures: OtherPlumbingFixturesV1 | None = None
     WaterClosets: WaterClosetsV1 | None = None
 
 
 class FireSuppressionV1(BaseOpenEpdHierarchicalSpec):
-    """Fire suppression performance specification."""
+    """Systems used to extinguish, control, or prevent fires."""
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
     FireProtectionPiping: FireProtectionPipingV1 | None = None
     FireSprinklers: FireSprinklersV1 | None = None
 
 
 class PipingV1(BaseOpenEpdHierarchicalSpec):
-    """Piping performance specification."""
+    """
+    Piping.
+
+    System of pipes used to provide water and fuel, remove wastewater, allow venting of gases, or supply
+    fire-suppression fluids to homes, businesses, or other facilities.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     thickness: LengthMmStr | None = pyd.Field(default=None, description="", example="6 mm")
     piping_diameter: LengthMmStr | None = pyd.Field(default=None, description="", example="120 mm")
     mass_per_unit_length: MassPerLengthStr | None = pyd.Field(default=None, description="", example="1 kg / m")
     piping_ansi_schedule: PipingAnsiSchedule | None = pyd.Field(default=None, description="", example="5")
     plumbing_piping_material: PlumbingPipingMaterial | None = pyd.Field(default=None, description="", example="PVC")
 
 
 class PlumbingEquipmentV1(BaseOpenEpdHierarchicalSpec):
-    """Plumbing equipment performance specification."""
+    """Water softeners, filtration equipment, water heaters, and other plumbing equipment."""
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
     StorageTanks: StorageTanksV1 | None = None
     WaterHeaters: WaterHeatersV1 | None = None
 
 
 class PlumbingV1(BaseOpenEpdHierarchicalSpec):
-    """Plumbing performance specification."""
+    """Residential and commercial plumbing equipment and fixtures."""
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
     PlumbingFixtures: PlumbingFixturesV1 | None = None
     FireSuppression: FireSuppressionV1 | None = None
     Piping: PipingV1 | None = None
```

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/precast_concrete.py` & `openepd-3.2.0/src/openepd/model/specs/generated/precast_concrete.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,33 +20,33 @@
 from openepd.compat.pydantic import pyd
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
 from openepd.model.validation.numbers import RatioFloat
 from openepd.model.validation.quantity import PressureMPaStr
 
 
 class ArchitecturalPrecastV1(BaseOpenEpdHierarchicalSpec):
-    """Architectural precast performance specification."""
+    """Precast concrete cladding used for architectural purposes."""
 
     _EXT_VERSION = "1.0"
 
 
 class StructuralPrecastV1(BaseOpenEpdHierarchicalSpec):
-    """Structural precast performance specification."""
+    """Precast concrete used for structural purposes."""
 
     _EXT_VERSION = "1.0"
 
 
 class UtilityUndergroundPrecastV1(BaseOpenEpdHierarchicalSpec):
-    """Utility underground precast performance specification."""
+    """Precast concrete for utility vaults, manhole, drain inlets. Excludes piping."""
 
     _EXT_VERSION = "1.0"
 
 
 class PrecastConcreteV1(BaseOpenEpdHierarchicalSpec):
-    """Precast concrete performance specification."""
+    """General category for precast concrete components."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     lightweight: bool | None = pyd.Field(default=None, description="", example=True)
     concrete_compressive_strength_28d: PressureMPaStr | None = pyd.Field(default=None, description="", example="1 MPa")
     insulated: bool | None = pyd.Field(default=None, description="", example=True)
```

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/sheathing.py` & `openepd-3.2.0/src/openepd/model/specs/generated/sheathing.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,30 +20,39 @@
 from openepd.compat.pydantic import pyd
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
 from openepd.model.specs.generated.enums import GypsumFacing, GypsumFireRating, GypsumThickness
 from openepd.model.validation.quantity import LengthMmStr, validate_unit_factory
 
 
 class CementitiousSheathingBoardV1(BaseOpenEpdHierarchicalSpec):
-    """Cementitious sheathing board performance specification."""
+    """
+    Cementitious sheathing board.
+
+    Cementitious non-gypsum board used for sheathing exteriors, shaft walls, and interior walls/ceilings requiring
+    moisture resistance.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     cement_board_thickness: LengthMmStr | None = pyd.Field(default=None, description="", example="10 mm")
 
     _cement_board_thickness_is_quantity_validator = pyd.validator("cement_board_thickness", allow_reuse=True)(
         validate_unit_factory("m")
     )
 
 
 class GypsumSheathingBoardV1(BaseOpenEpdHierarchicalSpec):
-    """Gypsum sheathing board performance specification."""
+    """
+    Cementitious sheathing board.
 
-    _EXT_VERSION = "1.0"
+    Gypsum board used for sheathing exteriors, shaft walls, and interior walls/ceilings requiring moisture resistance.
+    """
+
+    _EXT_VERSION = "1.1"
 
     # Own fields:
     fire_rating: GypsumFireRating | None = pyd.Field(default=None, description="", example="-")
     thickness: GypsumThickness | None = pyd.Field(default=None, description="", example="9 mm")
     facing: GypsumFacing | None = pyd.Field(default=None, description="", example="Paper")
 
     r_factor: str | None = pyd.Field(default=None, description="", example="1 RSI")
@@ -61,14 +70,18 @@
     abuse_resistant: bool | None = pyd.Field(default=None, description="", example=True)
 
     _gypsum_thickness_is_quantity_validator = pyd.validator("thickness", allow_reuse=True)(validate_unit_factory("m"))
     _gypsum_r_factor_is_quantity_validator = pyd.validator("r_factor", allow_reuse=True)(validate_unit_factory("RSI"))
 
 
 class SheathingV1(BaseOpenEpdHierarchicalSpec):
-    """Sheathing performance specification."""
+    """
+    Sheathing.
+
+    Boards or panels used in floor, wall and roof assemblies as a surface onto which other materials can be applied.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
     CementitiousSheathingBoard: CementitiousSheathingBoardV1 | None = None
     GypsumSheathingBoard: GypsumSheathingBoardV1 | None = None
```

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/steel.py` & `openepd-3.2.0/src/openepd/model/specs/generated/steel.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/thermal_moisture_protection.py` & `openepd-3.2.0/src/openepd/model/specs/generated/thermal_moisture_protection.py`

 * *Files 19% similar despite different names*

```diff
@@ -28,99 +28,116 @@
     RoofCoverBoardsMaterial,
 )
 from openepd.model.validation.numbers import RatioFloat
 from openepd.model.validation.quantity import LengthMmStr, PressureMPaStr
 
 
 class BituminousRoofingV1(BaseOpenEpdHierarchicalSpec):
-    """Bituminous roofing performance specification."""
+    """
+    Bituminous roofing.
+
+    Premanufactured membrane roofing sheets consisting of asphalt, reinforcing layers, and in some cases a surfacing.
+    """
 
     _EXT_VERSION = "1.0"
 
 
 class SinglePlyEPDMV1(BaseOpenEpdHierarchicalSpec):
-    """Single ply e p d m performance specification."""
+    """Ethylene propylene diene monomer (EPDM) rubber membrane."""
 
     _EXT_VERSION = "1.0"
 
 
 class SinglePlyKEEV1(BaseOpenEpdHierarchicalSpec):
-    """Single ply k e e performance specification."""
+    """
+    Ketone Ethylene Ester (KEE) roof membranes.
+
+    Consist of PVC resin and KEE plasticizer, with KEE exceeding 50% of the polymer content by weight.
+    """
 
     _EXT_VERSION = "1.0"
 
 
 class SinglePlyOtherV1(BaseOpenEpdHierarchicalSpec):
     """Single ply other performance specification."""
 
     _EXT_VERSION = "1.0"
 
 
 class SinglePlyPolyurethaneV1(BaseOpenEpdHierarchicalSpec):
-    """Single ply polyurethane performance specification."""
+    """Polyurethane liquid for flat roof waterproofing."""
 
     _EXT_VERSION = "1.0"
 
 
 class SinglePlyPVCV1(BaseOpenEpdHierarchicalSpec):
-    """Single ply p v c performance specification."""
+    """Polyvinyl chloride (PVC) thermoplastic membrane."""
 
     _EXT_VERSION = "1.0"
 
 
 class SinglePlyTPOV1(BaseOpenEpdHierarchicalSpec):
-    """Single ply t p o performance specification."""
+    """Thermoplastic Polyolefin (TPO) membrane."""
 
     _EXT_VERSION = "1.0"
 
 
 class BlanketInsulationV1(BaseOpenEpdHierarchicalSpec):
-    """Blanket insulation performance specification."""
+    """Non-rigid insulation batts, blankets, and rolls."""
 
     _EXT_VERSION = "1.0"
 
 
 class BlownInsulationV1(BaseOpenEpdHierarchicalSpec):
-    """Blown insulation performance specification."""
+    """Loose-fill insulation for blow-in or closed cavity applications."""
 
     _EXT_VERSION = "1.0"
 
 
 class BoardInsulationV1(BaseOpenEpdHierarchicalSpec):
-    """Board insulation performance specification."""
+    """Rigid insulation products including rigid foams, wood fiberboard insulation, and rigid mineral wool boards."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     compressive_strength: PressureMPaStr | None = pyd.Field(default=None, description="", example="1 MPa")
 
 
 class FoamedInPlaceV1(BaseOpenEpdHierarchicalSpec):
-    """Foamed in place performance specification."""
+    """Open and closed cell spray foam insulation."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     foam_type: FoamType | None = pyd.Field(default=None, description="", example="Open-Cell")
 
 
 class SprayedInsulationV1(BaseOpenEpdHierarchicalSpec):
-    """Sprayed insulation performance specification."""
+    """
+    Spray-on insulation, such as spray-on cellulose.
+
+    Foaming sprays are categorized separately under foamed-in-place.
+    """
 
     _EXT_VERSION = "1.0"
 
 
 class AirBarriersV1(BaseOpenEpdHierarchicalSpec):
-    """Air barriers performance specification."""
+    """Air Infiltration Barrier."""
 
     _EXT_VERSION = "1.0"
 
 
 class MembraneRoofingV1(BaseOpenEpdHierarchicalSpec):
-    """Membrane roofing performance specification."""
+    """
+    Membrane roofing.
+
+    Built-up bituminous, modified bituminous, elastomeric, thermoplastic, fluid-applied, and hot-applied rubberized
+    asphalt membrane roofing.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     thickness: LengthMmStr | None = pyd.Field(default=None, description="", example="10 mm")
     sri: float | None = pyd.Field(default=None, description="", example=2.3)
     total_recycled_content: RatioFloat | None = pyd.Field(default=None, description="", example=0.5, ge=0, le=1)
@@ -137,15 +154,15 @@
     SinglePlyOther: SinglePlyOtherV1 | None = None
     SinglePlyPolyurethane: SinglePlyPolyurethaneV1 | None = None
     SinglePlyPVC: SinglePlyPVCV1 | None = None
     SinglePlyTPO: SinglePlyTPOV1 | None = None
 
 
 class InsulationV1(BaseOpenEpdHierarchicalSpec):
-    """Insulation performance specification."""
+    """Thermal insulation materials for use in construction."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     r_value: float | None = pyd.Field(default=None, description="", example=2.3)
     material: InsulatingMaterial | None = pyd.Field(default=None, description="", example="Mineral Wool")
     intended_application: list[InsulationIntendedApplication] | None = pyd.Field(
@@ -158,56 +175,70 @@
     BlownInsulation: BlownInsulationV1 | None = None
     BoardInsulation: BoardInsulationV1 | None = None
     FoamedInPlace: FoamedInPlaceV1 | None = None
     SprayedInsulation: SprayedInsulationV1 | None = None
 
 
 class DampproofingAndWaterproofingV1(BaseOpenEpdHierarchicalSpec):
-    """Dampproofing and waterproofing performance specification."""
+    """
+    Dampproofing and waterproofing.
+
+    Dampproofing, and built-up bituminous, sheet, fluid-applied, cementitious, reactive, and bentonite waterproofing.
+    """
 
     _EXT_VERSION = "1.0"
 
 
 class FlashingAndSheetMetalV1(BaseOpenEpdHierarchicalSpec):
-    """Flashing and sheet metal performance specification."""
+    """Exposed sheet metal items, typically for drainage."""
 
     _EXT_VERSION = "1.0"
 
 
 class JointProtectionV1(BaseOpenEpdHierarchicalSpec):
-    """Joint protection performance specification."""
+    """Preformed joint seals and sealants, expansion control joint cover assemblies."""
 
     _EXT_VERSION = "1.0"
 
 
 class RoofCoverBoardsV1(BaseOpenEpdHierarchicalSpec):
-    """Roof cover boards performance specification."""
+    """
+    Boards installed between the insulation and membrane layers on a roof system.
+
+    It provides additional durability, fire protection, thermal, and vapor performance to a roof system, especially
+    in low-slope, high foot traffic applications.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     material: RoofCoverBoardsMaterial | None = pyd.Field(default=None, description="", example="Gypsum Fiber")
     facing: list[RoofCoverBoardsFacing] | None = pyd.Field(default=None, description="", example=["Paper"])
     thickness: LengthMmStr | None = pyd.Field(default=None, description="", example="1 m")
 
 
 class SteepSlopeRoofingV1(BaseOpenEpdHierarchicalSpec):
-    """Steep slope roofing performance specification."""
+    """Roofing materials typically for slopes of 3:12 and greater."""
 
     _EXT_VERSION = "1.0"
 
 
 class WeatherBarriersV1(BaseOpenEpdHierarchicalSpec):
-    """Weather barriers performance specification."""
+    """Vapor retarders and sheet or membrane air barriers."""
 
     _EXT_VERSION = "1.0"
 
 
 class ThermalMoistureProtectionV1(BaseOpenEpdHierarchicalSpec):
-    """Thermal moisture protection performance specification."""
+    """
+    Thermal moisture protection.
+
+    Broad category of materials whose function is to provide moisture and thermal protection between spaces (e.g.,
+    between the exterior and interior of a building).
+    """
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
     AirBarriers: AirBarriersV1 | None = None
     MembraneRoofing: MembraneRoofingV1 | None = None
     Insulation: InsulationV1 | None = None
```

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/utility_piping.py` & `openepd-3.2.0/src/openepd/model/specs/generated/utility_piping.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,32 +20,42 @@
 from openepd.compat.pydantic import pyd
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
 from openepd.model.specs.generated.enums import BuriedPipingType, PipingAnsiSchedule, UtilityPipingMaterial
 from openepd.model.validation.quantity import LengthMmStr, MassPerLengthStr
 
 
 class BuildingHeatingPipingV1(BaseOpenEpdHierarchicalSpec):
-    """Building heating piping performance specification."""
+    """
+    Heating piping.
+
+    System of pipes used to supply heated fluids (liquids or steam) for purposes of controlling temperature inside a
+    home, business, or other building facility.
+    """
 
     _EXT_VERSION = "1.0"
 
 
 class BuriedPipingV1(BaseOpenEpdHierarchicalSpec):
-    """Buried piping performance specification."""
+    """System of pipes used to provide or transport fluids (liquids and gases) underground."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     buried_piping_type: list[BuriedPipingType] | None = pyd.Field(
         default=None, description="", example=["Water Utilities"]
     )
 
 
 class UtilityPipingV1(BaseOpenEpdHierarchicalSpec):
-    """Utility piping performance specification."""
+    """
+    Utility piping.
+
+    System of pipes used to convey fluids (liquids and gases) from one location to another. Piping can be metal,
+    plastic, concrete, fiberglass, or other materials.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     thickness: LengthMmStr | None = pyd.Field(default=None, description="", example="6 m")
     piping_diameter: LengthMmStr | None = pyd.Field(default=None, description="", example="200 mm")
     mass_per_unit_length: MassPerLengthStr | None = pyd.Field(default=None, description="", example="1 kg / m")
```

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/wood.py` & `openepd-3.2.0/src/openepd/model/specs/generated/wood.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,107 +31,129 @@
     SheathingPanelsFabrication,
 )
 from openepd.model.validation.numbers import RatioFloat
 from openepd.model.validation.quantity import LengthMmStr
 
 
 class WoodDeckingV1(BaseOpenEpdHierarchicalSpec):
-    """Wood used for decking."""
+    """Dimensional boards for exterior decking."""
 
     _EXT_VERSION = "1.0"
 
 
 class WoodFramingV1(BaseOpenEpdHierarchicalSpec):
-    """Lumber for framing, typically softwood."""
+    """
+    Dimension lumber for light framing.
+
+    Includes solid and finger-jointed lumber. Standard shapes include 2x4, 2x6, and 2x8.
+    """
 
     _EXT_VERSION = "1.0"
 
 
 class PrefabricatedWoodInsulatedPanelsV1(BaseOpenEpdHierarchicalSpec):
-    """Prefabricated wood insulated panels performance specification."""
+    """
+    Structural insulated panels (SIPs).
+
+    Consist of wood sheet layer(s) combined with (typically foam) insulation layer(s).
+    """
 
     _EXT_VERSION = "1.0"
 
 
 class PrefabricatedWoodTrussV1(BaseOpenEpdHierarchicalSpec):
-    """Prefabricated wood truss performance specification."""
+    """Shop-fabricated wood truss."""
 
     _EXT_VERSION = "1.0"
 
 
 class CompositeLumberV1(BaseOpenEpdHierarchicalSpec):
-    """Composite lumber performance specification."""
+    """
+    Shop-fabricated structural Lumber.
+
+    Includes Laminated Strand Lumber (LSL), Parallel Strand Lumber (PSL), and Laminated Veneer Lumber (LVL).
+    """
 
     _EXT_VERSION = "1.0"
 
     fabrication: CompositeLumberFabrication | None = pyd.Field(default=None, description="", example="LVL")
     timber_species: EngineeredTimberSpecies | None = pyd.Field(default=None, description="", example="Alaska Cedar")
 
 
 class DimensionLumberV1(BaseOpenEpdHierarchicalSpec):
-    """Dimension lumber performance specification."""
+    """Dimension lumber for framing, decking, and other purposes."""
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
     timber_species: SawnTimberSpecies | None = pyd.Field(default=None, description="", example="Alaska Cedar")
     WoodDecking: WoodDeckingV1 | None = None
     WoodFraming: WoodFramingV1 | None = None
 
 
 class HeavyTimberV1(BaseOpenEpdHierarchicalSpec):
-    """Large format natural timber."""
+    """Large format, unfinished natural timber."""
 
     _EXT_VERSION = "1.0"
 
 
 class MassTimberV1(BaseOpenEpdHierarchicalSpec):
-    """Manufactured structural wood elements, such a CLT and LVL."""
+    """
+    Engineered heavy timber products.
+
+    Includes glue laminated (glulam), cross-laminated timber (CLT), dowel laminated timber (DLT), and nail laminated
+    timber (NLT).
+    """
 
     _EXT_VERSION = "1.0"
 
     fabrication: MassTimberFabrication | None = pyd.Field(default=None, description="", example="CLT")
     timber_species: EngineeredTimberSpecies | None = pyd.Field(default=None, description="", example="Alaska Cedar")
 
 
 class NonStructuralWoodV1(BaseOpenEpdHierarchicalSpec):
-    """Wood products that are not meant for structural use."""
+    """Non-structural interior and exterior wood products for trim, cabinets, countertops, etc."""
 
     _EXT_VERSION = "1.0"
 
 
 class PrefabricatedWoodV1(BaseOpenEpdHierarchicalSpec):
-    """Prefabricated wood performance specification."""
+    """
+    Prefabricated wood structural members made primarily from one or more types of wood.
+
+    Includes products made with metallic connectors, insulation, etc. Excludes products where the wood is merely
+    decorative.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Nested specs:
     PrefabricatedWoodInsulatedPanels: PrefabricatedWoodInsulatedPanelsV1 | None = None
     PrefabricatedWoodTruss: PrefabricatedWoodTrussV1 | None = None
 
 
 class SheathingPanelsV1(BaseOpenEpdHierarchicalSpec):
-    """Structural Wood Panels."""
+    """Wood sheets used for structural sheathing, including plywood and Oriented Strand Board."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     fabrication: SheathingPanelsFabrication | None = pyd.Field(default=None, description="", example="Plywood")
     wood_board_thickness: LengthMmStr | None = pyd.Field(default=None, description="", example="10 mm")
     timber_species: EngineeredTimberSpecies | None = pyd.Field(default=None, description="", example="Alaska Cedar")
 
 
 class UnfinishedWoodV1(BaseOpenEpdHierarchicalSpec):
-    """Unfinished or 'green' timber."""
+    """Raw logs and other unfinished wood products."""
 
     _EXT_VERSION = "1.0"
 
 
 class WoodV1(BaseOpenEpdHierarchicalSpec, HasForestPracticesCertifiers):
-    """Wood performance specification."""
+    """Structural Wood Products used in construction."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     timber_species: AllTimberSpecies | None = pyd.Field(
         default=None, description="Timber species", example="Alaska Cedar"
     )
```

### Comparing `openepd-3.1.4/src/openepd/model/specs/generated/wood_joists.py` & `openepd-3.2.0/src/openepd/model/specs/generated/wood_joists.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,20 @@
 from openepd.model.org import OrgRef
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
 from openepd.model.specs.generated.common import HasForestPracticesCertifiers
 from openepd.model.specs.generated.enums import AllFabrication, AllTimberSpecies
 
 
 class WoodJoistsV1(BaseOpenEpdHierarchicalSpec, HasForestPracticesCertifiers):
-    """Wood joists performance specification."""
+    """
+    Wood joists.
+
+    Prefabricated I-shaped engineered wood structural members made primarily from one or more types of wood. Includes
+    products made with metallic webbing. Excludes products where the wood is merely decorative.
+    """
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
     timber_species: AllTimberSpecies | None = pyd.Field(default=None, description="", example="Alaska Cedar")
     fabrication: AllFabrication | None = pyd.Field(default=None, description="", example="LVL")
     forest_practices_certifiers: list[OrgRef] | None = pyd.Field(default=None, description="")
```

### Comparing `openepd-3.1.4/src/openepd/model/standard.py` & `openepd-3.2.0/src/openepd/model/standard.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/model/validation/__init__.py` & `openepd-3.2.0/src/openepd/model/specs/generated/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/model/validation/common.py` & `openepd-3.2.0/src/openepd/model/validation/common.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/model/validation/numbers.py` & `openepd-3.2.0/src/openepd/model/validation/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,14 +13,7 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-from typing import Annotated
-
-from openepd.compat.pydantic import pyd
-
-# todo when move to pydantic 2, check that validators are being enforced.
-RatioFloat = Annotated[float, pyd.Field(ge=0, le=1, example=0.5)]
-PositiveInt = Annotated[int, pyd.Field(ge=0, example=1)]
```

### Comparing `openepd-3.1.4/src/openepd/model/validation/quantity.py` & `openepd-3.2.0/src/openepd/model/validation/quantity.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/src/openepd/model/versioning.py` & `openepd-3.2.0/src/openepd/model/versioning.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.4/PKG-INFO` & `openepd-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openepd
-Version: 3.1.4
+Version: 3.2.0
 Summary: Python library to work with OpenEPD format
 Home-page: https://github.com/cchangelabs/openepd
 License: Apache-2.0
 Author: C-Change Labs
 Author-email: support@c-change-labs.com
 Maintainer: C-Change Labs
 Maintainer-email: open-source@c-change-labs.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openepd Version: 3.1.4 Summary: Python library to
+Metadata-Version: 2.1 Name: openepd Version: 3.2.0 Summary: Python library to
 work with OpenEPD format Home-page: https://github.com/cchangelabs/openepd
 License: Apache-2.0 Author: C-Change Labs Author-email: support@c-change-
 labs.com Maintainer: C-Change Labs Maintainer-email: open-source@c-change-
 labs.com Requires-Python: >=3.11,<4.0 Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
```

