# Comparing `tmp/inspqcommun-2.6.0.tar.gz` & `tmp/inspqcommun-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inspqcommun-2.6.0.tar", last modified: Tue May 21 20:49:32 2024, max compression
+gzip compressed data, was "inspqcommun-2.7.0.tar", last modified: Mon May 27 20:41:22 2024, max compression
```

## Comparing `inspqcommun-2.6.0.tar` & `inspqcommun-2.7.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-21 20:49:32.708910 inspqcommun-2.6.0/
--rw-r--r--   0 jenkins    (114) jenkins    (119)    12567 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/LICENSE
--rw-r--r--   0 jenkins    (114) jenkins    (119)     1059 2024-05-21 20:49:32.708910 inspqcommun-2.6.0/PKG-INFO
--rw-r--r--   0 jenkins    (114) jenkins    (119)      509 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/README.md
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-21 20:49:32.680910 inspqcommun-2.6.0/inspqcommun/
--rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/__init__.py
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-21 20:49:32.684910 inspqcommun-2.6.0/inspqcommun/fa/
--rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fa/__init__.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     9076 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fa/chargement_service.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     1337 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fa/chargeur_fichiers.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     3487 2024-05-14 15:44:50.000000 inspqcommun-2.6.0/inspqcommun/fa/configuration.py
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-21 20:49:32.684910 inspqcommun-2.6.0/inspqcommun/fa/convertisseurs/
--rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fa/convertisseurs/__init__.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     5077 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fa/convertisseurs/convertisseur_acte_vaccinal.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)      514 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fa/convertisseurs/convertisseur_base.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     4638 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fa/convertisseurs/convertisseur_usager.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     9403 2024-05-16 21:04:23.000000 inspqcommun-2.6.0/inspqcommun/fa/injecteur.py
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-21 20:49:32.688910 inspqcommun-2.6.0/inspqcommun/fa/ressources/
--rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fa/ressources/__init__.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     2610 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fa/ressources/acte_vaccinal.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)      515 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fa/ressources/lieu_vaccination.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)      318 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fa/ressources/organisation.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)      983 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fa/ressources/ressource.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     2610 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fa/ressources/usager.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)      567 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fa/ressources/vaccinateur.py
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-21 20:49:32.688910 inspqcommun-2.6.0/inspqcommun/fa/validateurs/
--rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fa/validateurs/__init__.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     1351 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fa/validateurs/validateur.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)    12238 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fa/validateurs/validateur_acte_vaccinal.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     9263 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fa/validateurs/validateur_usager.py
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-21 20:49:32.688910 inspqcommun-2.6.0/inspqcommun/fhir/
--rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fhir/__init__.py
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-21 20:49:32.692910 inspqcommun-2.6.0/inspqcommun/fhir/clients/
--rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fhir/clients/__init__.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     2831 2024-05-16 21:04:23.000000 inspqcommun-2.6.0/inspqcommun/fhir/clients/base_client.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     4285 2024-05-21 20:49:19.000000 inspqcommun-2.6.0/inspqcommun/fhir/clients/immunization_client.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     4539 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fhir/clients/location_client.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     1344 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fhir/clients/medication_client.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     4890 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fhir/clients/organization_client.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     5202 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fhir/clients/patient_client.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     2557 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fhir/clients/practitioner_client.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     3800 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fhir/clients/value_set_client.py
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-21 20:49:32.700910 inspqcommun-2.6.0/inspqcommun/fhir/visitors/
--rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fhir/visitors/__init__.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     3226 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fhir/visitors/base.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     1668 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fhir/visitors/bundle.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     2233 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fhir/visitors/condition.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)    19838 2024-05-21 20:49:19.000000 inspqcommun-2.6.0/inspqcommun/fhir/visitors/immunization.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     4624 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fhir/visitors/location.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     2516 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fhir/visitors/medication.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)      972 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fhir/visitors/operation_outcome.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     5399 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fhir/visitors/organization.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     1257 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fhir/visitors/parameters.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)    11042 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fhir/visitors/patient.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)      859 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fhir/visitors/practitioner.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     1364 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/fhir/visitors/value_set.py
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-21 20:49:32.704910 inspqcommun-2.6.0/inspqcommun/identity/
--rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/identity/__init__.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)   164019 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/identity/keycloak.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     1413 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/identity/keycloak_token.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)    10764 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/identity/keycloak_tools.py
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-21 20:49:32.704910 inspqcommun-2.6.0/inspqcommun/kafka/
--rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/kafka/__init__.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     7943 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/kafka/consommateur.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     5280 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/kafka/producteur.py
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-21 20:49:32.708910 inspqcommun-2.6.0/inspqcommun/userprovisioning/
--rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/userprovisioning/__init__.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     9944 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/inspqcommun/userprovisioning/scim.py
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-21 20:49:32.708910 inspqcommun-2.6.0/inspqcommun.egg-info/
--rw-r--r--   0 jenkins    (114) jenkins    (119)     1059 2024-05-21 20:49:32.000000 inspqcommun-2.6.0/inspqcommun.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (114) jenkins    (119)     2321 2024-05-21 20:49:32.000000 inspqcommun-2.6.0/inspqcommun.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (114) jenkins    (119)        1 2024-05-21 20:49:32.000000 inspqcommun-2.6.0/inspqcommun.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (114) jenkins    (119)      104 2024-05-21 20:49:32.000000 inspqcommun-2.6.0/inspqcommun.egg-info/requires.txt
--rw-r--r--   0 jenkins    (114) jenkins    (119)       12 2024-05-21 20:49:32.000000 inspqcommun-2.6.0/inspqcommun.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (114) jenkins    (119)       38 2024-05-21 20:49:32.708910 inspqcommun-2.6.0/setup.cfg
--rw-r--r--   0 jenkins    (114) jenkins    (119)     1373 2024-05-09 15:48:27.000000 inspqcommun-2.6.0/setup.py
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-27 20:41:22.120912 inspqcommun-2.7.0/
+-rw-r--r--   0 jenkins    (114) jenkins    (119)    12567 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/LICENSE
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     1059 2024-05-27 20:41:22.120912 inspqcommun-2.7.0/PKG-INFO
+-rw-r--r--   0 jenkins    (114) jenkins    (119)      509 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/README.md
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-27 20:41:22.092912 inspqcommun-2.7.0/inspqcommun/
+-rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/__init__.py
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-27 20:41:22.092912 inspqcommun-2.7.0/inspqcommun/fa/
+-rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/__init__.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     9076 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/chargement_service.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     1337 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/chargeur_fichiers.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     3747 2024-05-27 20:41:09.000000 inspqcommun-2.7.0/inspqcommun/fa/configuration.py
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-27 20:41:22.096912 inspqcommun-2.7.0/inspqcommun/fa/convertisseurs/
+-rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/convertisseurs/__init__.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     5077 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/convertisseurs/convertisseur_acte_vaccinal.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)      514 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/convertisseurs/convertisseur_base.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     4638 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/convertisseurs/convertisseur_usager.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     9403 2024-05-16 21:04:23.000000 inspqcommun-2.7.0/inspqcommun/fa/injecteur.py
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-27 20:41:22.100912 inspqcommun-2.7.0/inspqcommun/fa/ressources/
+-rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/ressources/__init__.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     2610 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/ressources/acte_vaccinal.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)      515 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/ressources/lieu_vaccination.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)      318 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/ressources/organisation.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)      983 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/ressources/ressource.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     2610 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/ressources/usager.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)      567 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/ressources/vaccinateur.py
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-27 20:41:22.100912 inspqcommun-2.7.0/inspqcommun/fa/validateurs/
+-rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/validateurs/__init__.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     1351 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/validateurs/validateur.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)    12238 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/validateurs/validateur_acte_vaccinal.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     9263 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/validateurs/validateur_usager.py
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-27 20:41:22.100912 inspqcommun-2.7.0/inspqcommun/fhir/
+-rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/__init__.py
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-27 20:41:22.104912 inspqcommun-2.7.0/inspqcommun/fhir/clients/
+-rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/clients/__init__.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     2831 2024-05-16 21:04:23.000000 inspqcommun-2.7.0/inspqcommun/fhir/clients/base_client.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     5013 2024-05-27 20:41:09.000000 inspqcommun-2.7.0/inspqcommun/fhir/clients/immunization_client.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     4539 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/clients/location_client.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     1344 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/clients/medication_client.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     4890 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/clients/organization_client.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     5202 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/clients/patient_client.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     2557 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/clients/practitioner_client.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     3800 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/clients/value_set_client.py
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-27 20:41:22.112912 inspqcommun-2.7.0/inspqcommun/fhir/visitors/
+-rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/visitors/__init__.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     3226 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/visitors/base.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     1668 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/visitors/bundle.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     2233 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/visitors/condition.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)    21783 2024-05-27 20:41:09.000000 inspqcommun-2.7.0/inspqcommun/fhir/visitors/immunization.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     4624 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/visitors/location.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     2516 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/visitors/medication.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)      972 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/visitors/operation_outcome.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     5399 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/visitors/organization.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     1257 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/visitors/parameters.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)    11042 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/visitors/patient.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)      859 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/visitors/practitioner.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     1364 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/visitors/value_set.py
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-27 20:41:22.116912 inspqcommun-2.7.0/inspqcommun/identity/
+-rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/identity/__init__.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)   164019 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/identity/keycloak.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     1413 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/identity/keycloak_token.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)    11219 2024-05-27 20:41:09.000000 inspqcommun-2.7.0/inspqcommun/identity/keycloak_tools.py
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-27 20:41:22.116912 inspqcommun-2.7.0/inspqcommun/kafka/
+-rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/kafka/__init__.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     7943 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/kafka/consommateur.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     5280 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/kafka/producteur.py
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-27 20:41:22.120912 inspqcommun-2.7.0/inspqcommun/userprovisioning/
+-rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/userprovisioning/__init__.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     9944 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/userprovisioning/scim.py
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-27 20:41:22.120912 inspqcommun-2.7.0/inspqcommun.egg-info/
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     1059 2024-05-27 20:41:22.000000 inspqcommun-2.7.0/inspqcommun.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     2321 2024-05-27 20:41:22.000000 inspqcommun-2.7.0/inspqcommun.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (114) jenkins    (119)        1 2024-05-27 20:41:22.000000 inspqcommun-2.7.0/inspqcommun.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (114) jenkins    (119)      104 2024-05-27 20:41:22.000000 inspqcommun-2.7.0/inspqcommun.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (114) jenkins    (119)       12 2024-05-27 20:41:22.000000 inspqcommun-2.7.0/inspqcommun.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (114) jenkins    (119)       38 2024-05-27 20:41:22.120912 inspqcommun-2.7.0/setup.cfg
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     1373 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/setup.py
```

### Comparing `inspqcommun-2.6.0/LICENSE` & `inspqcommun-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/PKG-INFO` & `inspqcommun-2.7.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspqcommun
-Version: 2.6.0
+Version: 2.7.0
 Summary: Librairies communes de INSPQ
 Home-page: https://gitlab.forge.gouv.qc.ca/inspq/commun/python/inspqcommun.git
 Author: Philippe Gauthier
 Author-email: philippe.gauthier@inspq.qc.ca
 License: LiLiQ
 License-File: LICENSE
 Requires-Dist: fhirclient==1.0.3
```

### Comparing `inspqcommun-2.6.0/inspqcommun/fa/chargement_service.py` & `inspqcommun-2.7.0/inspqcommun/fa/chargement_service.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/fa/chargeur_fichiers.py` & `inspqcommun-2.7.0/inspqcommun/fa/chargeur_fichiers.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/fa/configuration.py` & `inspqcommun-2.7.0/inspqcommun/fa/configuration.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,17 +11,20 @@
 DEFAULT_KEYCLOAK_AUTH_USER: str = 'PERMISSIONS'
 DEFAULT_KEYCLOAK_AUTH_PASSWORD: str = ''
 DEFAULT_KEYCLOAK_AUTH_CLIENT_ID: str = "admin-cli"
 DEFAULT_KEYCLOAK_ENABLED: str = "False"
 DEFAULT_VALIDATE_CERTS: str = "true"
 class Configuration:
     client_roles = ["fa-utilisateur", "fa-saisie"]
-    def __init__(self, client_roles=None) -> None:
-        if client_roles is not None:
+    def __init__(self, client_roles:list=None, username:str=None, password=None) -> None:
+        if client_roles is not None and len(client_roles) > 0:
             self.client_roles = client_roles
+        
+        self.username = username
+        self.password = password
 
     def __str_to_bool(self, value: str) -> bool:
         bool_value = False
         try:
             bool_value = ast.literal_eval(value)
         except (SyntaxError, ValueError):
             return False
@@ -43,15 +46,17 @@
         url = os.environ.get("KEYCLOAK_BASE_URL", default_value) 
         return url if url.endswith("/auth") else url + "/auth"
         
     def get_keycloak_auth_realm(self, default_value=DEFAULT_KEYCLOAK_AUTH_REALM) -> str:
         return os.environ.get("KEYCLOAK_AUTH_REALM", default_value)
     
     def get_keycloak_auth_user(self, default_value=DEFAULT_KEYCLOAK_AUTH_USER) -> str:
-        return os.environ.get("KEYCLOAK_AUTH_USER", default_value)
+        if self.username is None:
+            return os.environ.get("KEYCLOAK_AUTH_USER", default_value)
+        return self.username
 
     def get_keycloak_auth_password(self, default_value=DEFAULT_KEYCLOAK_AUTH_PASSWORD) -> str:
         return os.environ.get("KEYCLOAK_AUTH_PASSWORD", default_value)
 
     def get_keycloak_auth_client_id(self, default_value=DEFAULT_KEYCLOAK_AUTH_CLIENT_ID) -> str:
         return os.environ.get("KEYCLOAK_AUTH_CLIENT_ID", default_value)
 
@@ -66,10 +71,10 @@
             defaultAuthRealm=self.get_keycloak_auth_realm(),
             defaultAuthUser=self.get_keycloak_auth_user(),
             defaultAuthPassword=self.get_keycloak_auth_password(),
             defaultBaseKeycloakUrl=self.get_keycloak_base_url(),
             defaultKeycloakEnabled=self.get_keycloak_enabled(),
             defaultAuthClientId=self.get_keycloak_auth_client_id(),
             defaultValidateCert=self.get_validate_certs())
-        headers = kcenv.authenticate(client_roles=self.client_roles)
+        headers = kcenv.authenticate(client_roles=self.client_roles, username=self.username, password=self.password)
         return headers.get('Authorization')
```

### Comparing `inspqcommun-2.6.0/inspqcommun/fa/convertisseurs/convertisseur_acte_vaccinal.py` & `inspqcommun-2.7.0/inspqcommun/fa/convertisseurs/convertisseur_acte_vaccinal.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/fa/convertisseurs/convertisseur_base.py` & `inspqcommun-2.7.0/inspqcommun/fa/convertisseurs/convertisseur_base.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/fa/convertisseurs/convertisseur_usager.py` & `inspqcommun-2.7.0/inspqcommun/fa/convertisseurs/convertisseur_usager.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/fa/injecteur.py` & `inspqcommun-2.7.0/inspqcommun/fa/injecteur.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/fa/ressources/acte_vaccinal.py` & `inspqcommun-2.7.0/inspqcommun/fa/ressources/acte_vaccinal.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/fa/ressources/lieu_vaccination.py` & `inspqcommun-2.7.0/inspqcommun/fa/ressources/lieu_vaccination.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/fa/ressources/ressource.py` & `inspqcommun-2.7.0/inspqcommun/fa/ressources/ressource.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/fa/ressources/usager.py` & `inspqcommun-2.7.0/inspqcommun/fa/ressources/usager.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/fa/ressources/vaccinateur.py` & `inspqcommun-2.7.0/inspqcommun/fa/ressources/vaccinateur.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/fa/validateurs/validateur.py` & `inspqcommun-2.7.0/inspqcommun/fa/validateurs/validateur.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/fa/validateurs/validateur_acte_vaccinal.py` & `inspqcommun-2.7.0/inspqcommun/fa/validateurs/validateur_acte_vaccinal.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/fa/validateurs/validateur_usager.py` & `inspqcommun-2.7.0/inspqcommun/fa/validateurs/validateur_usager.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/fhir/clients/base_client.py` & `inspqcommun-2.7.0/inspqcommun/fhir/clients/base_client.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/fhir/clients/immunization_client.py` & `inspqcommun-2.7.0/inspqcommun/fhir/clients/immunization_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class ImmunizationClient(BaseClient):
 
     immunization_endpoint = "{base_url}/Immunization"
     immunization_id_endpoint = "{base_url}/Immunization/{id}"
     immunization_id_override_endpoint = immunization_id_endpoint + '/$override'
     immunization_id_settoforecast_endpoint = immunization_id_endpoint + '/$settoforecast'
-
+    immunization_id_delete_immunization_endpoint = immunization_id_endpoint + '/$delete-immunization'
     def __init__(self, base_url=None, base_uri=None, token_header=None, validate_certs=True) -> None:
         super().__init__(base_url=base_url, base_uri=base_uri, token_header=token_header)
         self.validate_certs = validate_certs
 
     def create(self, immunization: Immunization):
         immunization.meta = None
         response = requests.post(
@@ -86,13 +86,26 @@
             url=self.immunization_id_settoforecast_endpoint.format(base_url=self.get_fhir_url(), id=immunization.id),
             data=json.dumps(res),
             headers=self.headers,
             verify=self.validate_certs)
         log.info("POST Immunization settoforecast : {}".format(response.status_code))
         return response
 
+    def delete_immunization(self, immunization: Immunization):
+        parametre = ParametersVisitor()
+        parametre.add_parameter(valeur=immunization, name='immunization',)
+        res = parametre.getFhirResource().as_json()
+
+        response = requests.post(
+            url=self.immunization_id_delete_immunization_endpoint.format(base_url=self.get_fhir_url(), id=immunization.id),
+            data=json.dumps(res),
+            headers=self.headers,
+            verify=self.validate_certs)
+        log.info("POST Immunization delete-immunization : {}".format(response.status_code))
+        return response
+
     def extract_immunization_from_response(self, response: Response) -> Immunization:
         if response.status_code == 200 or response.status_code == 201:
             content = json.loads(response.content)
             return Immunization(jsondict=content)
         else:
             return None
```

### Comparing `inspqcommun-2.6.0/inspqcommun/fhir/clients/location_client.py` & `inspqcommun-2.7.0/inspqcommun/fhir/clients/location_client.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/fhir/clients/medication_client.py` & `inspqcommun-2.7.0/inspqcommun/fhir/clients/medication_client.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/fhir/clients/organization_client.py` & `inspqcommun-2.7.0/inspqcommun/fhir/clients/organization_client.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/fhir/clients/patient_client.py` & `inspqcommun-2.7.0/inspqcommun/fhir/clients/patient_client.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/fhir/clients/practitioner_client.py` & `inspqcommun-2.7.0/inspqcommun/fhir/clients/practitioner_client.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/fhir/clients/value_set_client.py` & `inspqcommun-2.7.0/inspqcommun/fhir/clients/value_set_client.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/fhir/visitors/base.py` & `inspqcommun-2.7.0/inspqcommun/fhir/visitors/base.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/fhir/visitors/bundle.py` & `inspqcommun-2.7.0/inspqcommun/fhir/visitors/bundle.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/fhir/visitors/condition.py` & `inspqcommun-2.7.0/inspqcommun/fhir/visitors/condition.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/fhir/visitors/immunization.py` & `inspqcommun-2.7.0/inspqcommun/fhir/visitors/immunization.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 from datetime import date, datetime
 from typing import List
 
 class ImmunizationVisitor(BaseVisitor):
         
     OVERRIDE_STATUS_URL = "http://www.santepublique.rtss.qc.ca/sipmi/fa/1.0.0/extensions/#immunization/overridestatus"
     OVERRIDE_REASON_URL = "http://www.santepublique.rtss.qc.ca/sipmi/fa/1.0.0/extensions/#immunization/overridereason"
+    REASON_FOR_DELETION_URL = "http://www.santepublique.rtss.qc.ca/sipmi/fa/1.0.0/extensions/#immunization/reasonfordeletion"
+    OTHER_REASON_FOR_DELETION_URL = "http://www.santepublique.rtss.qc.ca/sipmi/fa/1.0.0/extensions/#immunization/otherreasonfordeletion"
     ANTIGEN_STATUS_ANTIGEN_URL = "antigen"
     ANTIGEN_STATUS_STATUS_URL = "status"
     ANTIGEN_STATUS_DOSE_NUMER_URL = "doseNumber"
     LOT_ID_URL = "http://www.santepublique.rtss.qc.ca/sipmi/fa/1.0.0/extensions/#immunization/lotid"
     TRADE_NAME_URL = 'http://www.santepublique.rtss.qc.ca/sipmi/fa/1.0.0/extensions/#immunization/tradename'
     ANTIGEN_STATUS_URL = "http://www.santepublique.rtss.qc.ca/sipmi/fa/1.0.0/extensions/#immunization/antigenstatus"
     PROFILE_URL = 'http://www.santepublique.rtss.qc.ca/sipmi/fa/1.0.0/profiles/InspqImmunization.structuredefinition.xml'
@@ -147,22 +149,23 @@
     def get_override_reason(self) -> CodeableConcept:
         if self.getFhirResource().extension is not None:
             for ext in self.getFhirResource().extension:
                 if ext.url == self.OVERRIDE_REASON_URL:
                     return ext.valueCodeableConcept
         return None
 
-    def set_override_reason(self, status_code:str=None, status_display:str=None):
+    def set_override_reason(self, reason_code:str=None, status_display:str=None):
         status_codeable_concept = self._to_codeable_concept(
-            code=status_code,
+            code=reason_code,
             display=status_display,
             coding_system=ImmunizationVisitor.DEFAULT_CODING_SYSTEM,
             coding_version=ImmunizationVisitor.DEFAULT_CODING_VERSION)
         self.getFhirResource().extension = super().add_or_update_extension_to_extensions(extension=self._creer_extension(self.OVERRIDE_REASON_URL, valueCodeableConcept=status_codeable_concept), 
                                                                                          extensions=self.getFhirResource().extension)
+
     def set_antigen_status(self, antigen_code:str=None, antigen_display:str=None, dose_number:int=None, status_code:str=None, status_display:str=None):
         antigen_status_ext = Extension()
         antigen_status_ext.url = self.ANTIGEN_STATUS_URL
 
         antigen_codeable_concept = self._to_codeable_concept(
             code=antigen_code,
             display=antigen_display,
@@ -373,8 +376,34 @@
         return self.getFhirResource().status
 
     def set_status(self, immunization=None, status=None):
         if immunization is None:
             immunization = self.fhir_resource
         if status is not None:
             self.status = status
-        immunization.status = self.status
+        immunization.status = self.status
+
+    def get_reason_for_deletion(self) -> CodeableConcept:
+        if self.getFhirResource().extension is not None:
+            for ext in self.getFhirResource().extension:
+                if ext.url == self.REASON_FOR_DELETION_URL:
+                    return ext.valueCodeableConcept
+        return None
+
+    def get_other_reason_for_deletion(self) -> str:
+        if self.getFhirResource().extension is not None:
+            for ext in self.getFhirResource().extension:
+                if ext.url == self.OTHER_REASON_FOR_DELETION_URL:
+                    return ext.valueString
+        return ""
+
+    def set_reason_for_deletion(self, reason_code:str=None, other_reason_for_deletion:str=None):
+        status_codeable_concept = self._to_codeable_concept(
+            code=reason_code,
+            coding_system=ImmunizationVisitor.DEFAULT_CODING_SYSTEM,
+            coding_version=ImmunizationVisitor.DEFAULT_CODING_VERSION)
+        self.getFhirResource().extension =  super().add_or_update_extension_to_extensions(extension=self._creer_extension(self.REASON_FOR_DELETION_URL, valueCodeableConcept=status_codeable_concept), 
+                                                                                         extensions=self.getFhirResource().extension)
+        if other_reason_for_deletion is not None:
+            self.getFhirResource().extension =  super().add_or_update_extension_to_extensions(extension=self._creer_extension(self.OTHER_REASON_FOR_DELETION_URL, valueString=other_reason_for_deletion), 
+                                                                                         extensions=self.getFhirResource().extension)
+
```

### Comparing `inspqcommun-2.6.0/inspqcommun/fhir/visitors/location.py` & `inspqcommun-2.7.0/inspqcommun/fhir/visitors/location.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/fhir/visitors/medication.py` & `inspqcommun-2.7.0/inspqcommun/fhir/visitors/medication.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/fhir/visitors/operation_outcome.py` & `inspqcommun-2.7.0/inspqcommun/fhir/visitors/operation_outcome.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/fhir/visitors/organization.py` & `inspqcommun-2.7.0/inspqcommun/fhir/visitors/organization.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/fhir/visitors/parameters.py` & `inspqcommun-2.7.0/inspqcommun/fhir/visitors/parameters.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/fhir/visitors/patient.py` & `inspqcommun-2.7.0/inspqcommun/fhir/visitors/patient.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/fhir/visitors/practitioner.py` & `inspqcommun-2.7.0/inspqcommun/fhir/visitors/practitioner.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/fhir/visitors/value_set.py` & `inspqcommun-2.7.0/inspqcommun/fhir/visitors/value_set.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/identity/keycloak.py` & `inspqcommun-2.7.0/inspqcommun/identity/keycloak.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/identity/keycloak_token.py` & `inspqcommun-2.7.0/inspqcommun/identity/keycloak_token.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/identity/keycloak_tools.py` & `inspqcommun-2.7.0/inspqcommun/identity/keycloak_tools.py`

 * *Files 16% similar despite different names*

```diff
@@ -73,22 +73,27 @@
                          auth_client_secret=None,
                          validate_certs=self.validate_certs)
         else:
             kcapi = None
         
         return kcapi
     
-    def authenticate(self, client_roles=[], realm_roles=[], given_name=None, family_name=None):
+    def authenticate(self, client_roles=[], realm_roles=[], given_name=None, family_name=None, username=None, password=None):
         if self.keycloak_enabled:
             if not self.keycloak_auth_user or not self.keycloak_auth_password:
                 return self.__authenticate_by_service_account()
             else:
-                return self.__authenticate_by_username_password()
+                return self.__authenticate_by_username_password(username=username, password=password)
         else:
-            return self.__get_test_access_token(client_roles=client_roles, realm_roles=realm_roles, given_name=given_name, family_name=family_name)
+            return self.__get_test_access_token(
+                client_roles=client_roles,
+                realm_roles=realm_roles,
+                given_name=given_name,
+                family_name=family_name,
+                preferred_username=username)
 
     def get_token_url(self):
         token_url = KeycloakAPI.format_token_url(baseurl=self.keycloak_url, realm=self.keycloak_auth_realm)
         return token_url
 
     def get_client_secret(self, client_id, realm=None):
         if realm is None:
@@ -114,27 +119,30 @@
                 auth_realm=self.keycloak_auth_realm,
                 client_id=client,
                 client_secret=self.keycloak_auth_client_secret,
                 validate_certs=self.validate_certs) if self.keycloak_auth_client_secret is not None else {}
         self.headers = headers
         return headers
 
-    def __authenticate_by_username_password(self):
+    def __authenticate_by_username_password(self, username=None, password=None):
         headers = {}
         if self.keycloak_enabled:
             if (self.keycloak_auth_client_secret is None or len(self.keycloak_auth_client_secret) == 0) and (self.kc is not None or self.init_keycloak_api() is not None):
                 self.keycloak_auth_client_secret = self.get_client_secret(client_id=self.keycloak_auth_client_id, realm=self.keycloak_auth_realm)
-
+            if username is None:
+                username = self.keycloak_auth_user
+            if password is None:
+                password = self.keycloak_auth_password
             headers = get_token(
                 base_url=self.keycloak_url,
                 validate_certs=self.validate_certs,
                 auth_realm=self.keycloak_auth_realm,
                 client_id=self.keycloak_auth_client_id,
-                auth_username=self.keycloak_auth_user,
-                auth_password=self.keycloak_auth_password, 
+                auth_username=username,
+                auth_password=password, 
                 client_secret=self.keycloak_auth_client_secret) if self.keycloak_auth_client_secret is not None else {}
         self.headers = headers
         return headers
 
     def __str_to_bool(self, value: str) -> bool:
         if value.upper() == "TRUE":
             value = "True"
@@ -143,29 +151,32 @@
         bool_value = False
         try:
             bool_value = ast.literal_eval(value)
         except (SyntaxError, ValueError):
             return False
         return bool(bool_value)
     
-    def __get_test_access_token(self, client_roles, realm_roles, given_name, family_name):
+    def __get_test_access_token(self, client_roles, realm_roles, given_name, family_name, preferred_username):
         if len(client_roles) == 0:
             client_roles = [
                 "fa-saisie",
                 "fa-utilisateur",
                 "superuser"]
         if len(realm_roles) == 0:
             realm_roles = [
                 "offline_access",
                 "default-roles-msss",
                 "uma_authorization"]
         if given_name is None:
             given_name = "Super"
         if family_name is None:
             family_name = "Permissions"
+        if preferred_username is None:
+            preferred_username = self.keycloak_auth_user
+
         decoded_access_token = {
             "exp": round(time.time()) + 300,
             "iat": round(time.time()),
             "auth_time": round(time.time()),
             "jti": str(uuid.uuid1()),
             "iss": "{}/realms/{}".format(self.keycloak_url, self.keycloak_auth_realm),
             "aud": self.keycloak_auth_client_id,
@@ -179,15 +190,15 @@
             "groups": [
                 "create-realm",
                 "offline_access",
                 "admin",
                 "uma_authorization",
                 "cluster-admin"
             ],
-            "preferred_username": self.keycloak_auth_user,
+            "preferred_username": preferred_username,
             "allowed-origins": [
                 "*"
             ],
             "realm_access": {
                 "roles": realm_roles
             },
             "resource_access": {
```

### Comparing `inspqcommun-2.6.0/inspqcommun/kafka/consommateur.py` & `inspqcommun-2.7.0/inspqcommun/kafka/consommateur.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/kafka/producteur.py` & `inspqcommun-2.7.0/inspqcommun/kafka/producteur.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun/userprovisioning/scim.py` & `inspqcommun-2.7.0/inspqcommun/userprovisioning/scim.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/inspqcommun.egg-info/PKG-INFO` & `inspqcommun-2.7.0/inspqcommun.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspqcommun
-Version: 2.6.0
+Version: 2.7.0
 Summary: Librairies communes de INSPQ
 Home-page: https://gitlab.forge.gouv.qc.ca/inspq/commun/python/inspqcommun.git
 Author: Philippe Gauthier
 Author-email: philippe.gauthier@inspq.qc.ca
 License: LiLiQ
 License-File: LICENSE
 Requires-Dist: fhirclient==1.0.3
```

### Comparing `inspqcommun-2.6.0/inspqcommun.egg-info/SOURCES.txt` & `inspqcommun-2.7.0/inspqcommun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.6.0/setup.py` & `inspqcommun-2.7.0/setup.py`

 * *Files identical despite different names*

