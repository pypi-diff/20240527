# Comparing `tmp/plonetheme.imioapps-2.47.tar.gz` & `tmp/plonetheme.imioapps-2.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plonetheme.imioapps-2.47.tar", last modified: Wed Apr 10 07:09:59 2024, max compression
+gzip compressed data, was "dist/plonetheme.imioapps-2.48.tar", last modified: Mon May 27 10:30:19 2024, max compression
```

## Comparing `plonetheme.imioapps-2.47.tar` & `plonetheme.imioapps-2.48.tar`

### file list

```diff
@@ -1,320 +1,320 @@
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      720 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      319 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/setuphandlers.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      913 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/CODT_BuildLicence.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      651 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/coring.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Article127.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3209 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/EnvClassTwo.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/EnvironmentRubricTerm.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Division.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3379 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/goback.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/SpecificFeatureTerm.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      399 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/retire.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      977 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/OpinionEventConfig.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      940 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanTool.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      891 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/PreliminaryNotice.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      940 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Equipment.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      249 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Corporation.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1043 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/getemails.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Contact.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      784 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Division.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanConfigurationValue.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      940 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/EventConfig.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Locality.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      457 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/warning.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/EnvClassThree.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanConfigurationValue.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/OpinionRequestEventType.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      940 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/RecipientCadastre.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1043 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/question-mark.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Locality.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/AskOpinionEventType.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanTool.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/PcaTerm.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanDelay.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3197 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/EnvClassOne.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanCertificateTwo.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      859 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/CODT_IntegratedLicence.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      982 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/CODT_Inquiry.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventOpinionRequest.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      913 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/BuildLicence.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/PersonTitleTerm.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      736 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/CODT_ParcelOutLicence.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      750 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventOpinionRequest.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/BuildLicence.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/MiscDemand.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/EnvironmentLicence.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3227 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/EnvClassBordering.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanVocabularyTerm.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      982 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Inquiry.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      233 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Street.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      457 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Ticket.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/ParcellingTerm.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/EnvClassOne.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/GenericLicence.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/EventConfig.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      690 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/refuse.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9123 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/viewlet-firefox.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      859 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Article127.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      940 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/TextConfig.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/ParcellingTerm.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      859 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/CODT_Article127.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3051 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/PortionOut.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Layer.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3494 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Geometrician.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      982 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/CODT_UniqueLicenceInquiry.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2461 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/logo.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/EnvClassTwo.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      940 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/EnvironmentBase.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3494 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/FolderManager.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/RecipientCadastre.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3051 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Parcel.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      233 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/RoadDecree.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/OpinionRequestEventType.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/OrganisationTerm.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/ParcelOutLicence.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5900 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/urban-sprite.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      323 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/EnvironmentClassThree.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3494 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Contact.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/LicenceConfig.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1047 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/inacceptable.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/EnvironmentLicence.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3061 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/CODT_NotaryLetter.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3099 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanCertificateTwo.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      249 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Report.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      611 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/ExplosivesPossession.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Inquiry.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/PcaTerm.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanDoc.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      510 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/icon_add.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      940 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventType.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      736 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/ParcelOutLicence.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      608 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/schedule.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      977 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/duplicate_licence.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      826 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/linkedhistoricfolders.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      635 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/old.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3494 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Architect.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3099 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/CODT_UrbanCertificateTwo.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Corporation.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3227 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/EnvClassThree.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Parcelling.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      257 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Declaration.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1025 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/WorkLocation.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      750 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/copytoclaymants.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      951 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/attachment.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      750 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventAnnouncement.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEvent.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      683 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/xml.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/reopen.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanCertificateBase.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      240 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/PatrimonyCertificate.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/OpinionRequestEventType.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      859 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UniqueLicence.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      940 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/City.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      859 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/IntegratedLicence.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      750 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEvent.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventType.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/iscomplete.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventInquiry.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      940 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/GenericLicence.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      696 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Inspection.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/PortionOut.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Recipient.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      977 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/MiscDemand.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      940 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Lot.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3494 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Applicant.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/OrganisationTerm.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3061 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/NotaryLetter.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      940 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/FollowUpEventType.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Street.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      750 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventMayor.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/FolderManager.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      929 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/accept.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      749 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/isincomplete.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      891 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/ProjectMeeting.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/SpecificFeatureTerm.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      859 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/CODT_CommercialLicence.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/EnvironmentClassThree.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Layer.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      696 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/parcelhistoric.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/EnvironmentRubricTerm.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      249 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanDoc.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Recipient.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3087 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/CODT_UrbanCertificateOne.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/EnvironmentBase.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      859 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/CODT_UniqueLicence.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanDoc.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      819 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/linkedfolders.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      482 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/icon_add_big.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      249 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/EnvironmentLicence.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3109 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/close.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanDelay.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3087 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanCertificateOne.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      750 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventInquiry.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      940 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanCertificateBase.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      781 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/engrenage.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      750 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventAcknowledgment.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      940 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/FollowUpEventConfig.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      599 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/assign.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      750 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventNotificationCollege.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanVocabularyTerm.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      644 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/lock.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      750 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventCollege.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3494 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Notary.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3494 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Proprietary.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Declaration.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/City.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/PersonTitleTerm.png.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      249 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanConfigurationValue.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1148 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/LicenceConfig.png
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/plonemeetingskin_images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      125 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/plonemeetingskin_images/treeCollapsed.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      283 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/plonemeetingskin_images/backTo.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      135 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/plonemeetingskin_images/CONTENT.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      394 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/plonemeetingskin_images/pm_search.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      178 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/plonemeetingskin_images/backToValidatedForInput.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2534 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/plonemeetingskin_images/logo.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      320 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/plonemeetingskin_images/pm_preferences.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      481 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/plonemeetingskin_images/pm_home.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4670 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/plonemeetingskin_images/favicon.ico
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      317 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/plonemeetingskin_images/pm_config.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      123 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/plonemeetingskin_images/treeExpanded.gif
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/dmsmailskin_styles/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4463 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/dmsmailskin_styles/dmsmailskin.css.dtml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/pstskin_styles/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3477 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/pstskin_styles/pstskin.css.dtml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/plonemeetingskin_styles/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10503 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/plonemeetingskin_styles/plonemeetingskin.css.dtml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      161 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/plonemeetingskin_styles/CONTENT.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_styles/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11850 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_styles/urbanskin.css.dtml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/imioapps_styles/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1004 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/imioapps_styles/imioapps_ckeditor_moonolisa.css.dtml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7005 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/imioapps_styles/livesearch_reply.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      604 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/imioapps_styles/ploneCustom.css.dtml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1558 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/imioapps_styles/imioapps_properties.props
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      640 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/imioapps_styles/imioapps_IEFixes.css.dtml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    42202 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/imioapps_styles/imioapps.css.dtml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/imioapps_images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    33676 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/imioapps_images/spinner_small.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      326 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/imioapps_images/header-bg.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      546 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/imioapps_images/search_local_check.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      775 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/imioapps_images/filtre_sous.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       63 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/imioapps_images/exclamation.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      855 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/imioapps_images/filtre_add.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      823 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/imioapps_images/help.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      470 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/imioapps_images/search_button_icon.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    36210 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/imioapps_images/spinner.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      462 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/imioapps_images/search_local.png
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/pstskin_images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4964 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/pstskin_images/logo.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3758 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/pstskin_images/favicon.ico
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/dmsmailskin_images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1917 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/dmsmailskin_images/logo.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3362 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/dmsmailskin_images/favicon.ico
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1496 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/configure.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/locales/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      495 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/locales/eea.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/locales/en/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/locales/en/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      683 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/locales/en/LC_MESSAGES/plone.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      591 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/locales/en/LC_MESSAGES/eea.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      706 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/locales/plone.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/locales/fr/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      836 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/locales/fr/LC_MESSAGES/plone.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      620 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/locales/fr/LC_MESSAGES/eea.po
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/testing/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      171 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/testing/metadata.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/default/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      174 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/default/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      558 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/default/registry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      221 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/default/viewlets.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      616 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/default/skins.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      976 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/default/cssregistry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      337 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/default/jsregistry.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/to_123/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      601 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/to_123/skins.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/pstskin/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      173 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/pstskin/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      402 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/pstskin/viewlets.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      750 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/pstskin/skins.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      301 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/pstskin/cssregistry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/pstskin/pstskin_marker.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      399 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/pstskin/import_steps.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/plonemeetingskin/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/plonemeetingskin/plonemeetingskin_marker.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      173 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/plonemeetingskin/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1132 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/plonemeetingskin/viewlets.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      831 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/plonemeetingskin/skins.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      310 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/plonemeetingskin/cssregistry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      421 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/plonemeetingskin/import_steps.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/uninstall/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/uninstall/uninstall_marker.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1483 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/uninstall/skins.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      314 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/uninstall/import_steps.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/urbanskin/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      173 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/urbanskin/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      559 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/urbanskin/viewlets.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      768 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/urbanskin/skins.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/urbanskin/urbanskin_marker.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      303 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/urbanskin/cssregistry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      405 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/urbanskin/import_steps.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/dmsmailskin/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      173 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/dmsmailskin/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/dmsmailskin/dmsmailskin_marker.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      943 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/dmsmailskin/viewlets.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      798 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/dmsmailskin/skins.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/dmsmailskin/cssregistry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      426 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/dmsmailskin/import_steps.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      642 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/testing.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      735 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/interfaces.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     3129 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/mk_sync_locales.sh
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      569 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/testing.zcml
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)       47 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/svn.ignore
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/Extensions/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1334 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/Extensions/Install.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       24 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/Extensions/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/tests/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      798 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/tests/test_example.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/tests/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      347 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/upgrades.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      214 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/browser/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/browser/static/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1319 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/browser/static/skin.js
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      944 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/browser/overrides.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2277 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/browser/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1756 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/browser/viewlets.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/browser/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      288 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/browser/templates/viewlet_workflowstate.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       92 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/browser/templates/empty.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      265 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/browser/templates/help.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/browser/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4760 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       56 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme.imioapps.egg-info/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme.imioapps.egg-info/dependency_links.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       89 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme.imioapps.egg-info/entry_points.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       11 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme.imioapps.egg-info/namespace_packages.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       11 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme.imioapps.egg-info/top_level.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    25312 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme.imioapps.egg-info/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    17444 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/src/plonetheme.imioapps.egg-info/SOURCES.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme.imioapps.egg-info/not-zip-safe
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      100 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/src/plonetheme.imioapps.egg-info/requires.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/docs/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      729 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/docs/LICENSE.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/docs/LICENSE.GPL
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1570 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    25312 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      469 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/MANIFEST.in
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18349 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/CHANGES.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      674 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/README.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       78 2024-04-10 07:09:59.000000 plonetheme.imioapps-2.47/setup.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      333 2024-04-10 07:09:58.000000 plonetheme.imioapps-2.47/buildout.cfg
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      720 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      319 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/setuphandlers.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      913 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/CODT_BuildLicence.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      651 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/coring.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Article127.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3209 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/EnvClassTwo.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/EnvironmentRubricTerm.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Division.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3379 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/goback.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/SpecificFeatureTerm.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      399 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/retire.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      977 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/OpinionEventConfig.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      940 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanTool.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      891 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/PreliminaryNotice.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      940 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Equipment.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      249 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Corporation.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1043 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/getemails.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Contact.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      784 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Division.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanConfigurationValue.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      940 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/EventConfig.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Locality.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      457 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/warning.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/EnvClassThree.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanConfigurationValue.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/OpinionRequestEventType.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      940 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/RecipientCadastre.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1043 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/question-mark.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Locality.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/AskOpinionEventType.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanTool.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/PcaTerm.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanDelay.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3197 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/EnvClassOne.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanCertificateTwo.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      859 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/CODT_IntegratedLicence.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      982 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/CODT_Inquiry.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventOpinionRequest.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      913 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/BuildLicence.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/PersonTitleTerm.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      736 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/CODT_ParcelOutLicence.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      750 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventOpinionRequest.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/BuildLicence.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/MiscDemand.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/EnvironmentLicence.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3227 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/EnvClassBordering.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanVocabularyTerm.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      982 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Inquiry.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      233 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Street.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      457 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Ticket.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/ParcellingTerm.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/EnvClassOne.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/GenericLicence.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/EventConfig.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      690 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/refuse.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9123 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/viewlet-firefox.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      859 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Article127.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      940 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/TextConfig.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/ParcellingTerm.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      859 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/CODT_Article127.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3051 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/PortionOut.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Layer.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3494 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Geometrician.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      982 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/CODT_UniqueLicenceInquiry.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2461 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/logo.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/EnvClassTwo.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      940 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/EnvironmentBase.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3494 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/FolderManager.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/RecipientCadastre.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3051 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Parcel.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      233 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/RoadDecree.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/OpinionRequestEventType.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/OrganisationTerm.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/ParcelOutLicence.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5900 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/urban-sprite.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      323 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/EnvironmentClassThree.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3494 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Contact.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/LicenceConfig.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1047 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/inacceptable.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/EnvironmentLicence.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3061 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/CODT_NotaryLetter.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3099 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanCertificateTwo.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      249 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Report.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      611 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/ExplosivesPossession.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Inquiry.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/PcaTerm.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanDoc.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      510 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/icon_add.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      940 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventType.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      736 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/ParcelOutLicence.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      608 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/schedule.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      977 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/duplicate_licence.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      826 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/linkedhistoricfolders.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      635 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/old.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3494 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Architect.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3099 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/CODT_UrbanCertificateTwo.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Corporation.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3227 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/EnvClassThree.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Parcelling.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      257 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Declaration.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1025 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/WorkLocation.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      750 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/copytoclaymants.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      951 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/attachment.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      750 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventAnnouncement.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEvent.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      683 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/xml.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/reopen.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanCertificateBase.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      240 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/PatrimonyCertificate.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/OpinionRequestEventType.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      859 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UniqueLicence.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      940 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/City.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      859 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/IntegratedLicence.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      750 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEvent.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventType.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/iscomplete.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventInquiry.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      940 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/GenericLicence.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      696 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Inspection.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/PortionOut.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Recipient.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      977 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/MiscDemand.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      940 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Lot.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3494 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Applicant.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/OrganisationTerm.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3061 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/NotaryLetter.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      940 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/FollowUpEventType.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Street.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      750 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventMayor.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/FolderManager.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      929 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/accept.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      749 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/isincomplete.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      891 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/ProjectMeeting.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/SpecificFeatureTerm.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      859 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/CODT_CommercialLicence.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/EnvironmentClassThree.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Layer.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      696 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/parcelhistoric.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/EnvironmentRubricTerm.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      249 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanDoc.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Recipient.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3087 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/CODT_UrbanCertificateOne.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/EnvironmentBase.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      859 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/CODT_UniqueLicence.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanDoc.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      819 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/linkedfolders.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      482 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/icon_add_big.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      249 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/EnvironmentLicence.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3109 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/close.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanDelay.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3087 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanCertificateOne.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      750 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventInquiry.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      940 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanCertificateBase.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      781 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/engrenage.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      750 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventAcknowledgment.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      940 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/FollowUpEventConfig.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      599 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/assign.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      750 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventNotificationCollege.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanVocabularyTerm.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      644 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/lock.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      750 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventCollege.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3494 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Notary.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3494 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Proprietary.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Declaration.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/City.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/PersonTitleTerm.png.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      249 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanConfigurationValue.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1148 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/LicenceConfig.png
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/plonemeetingskin_images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      125 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/plonemeetingskin_images/treeCollapsed.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      283 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/plonemeetingskin_images/backTo.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      135 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/plonemeetingskin_images/CONTENT.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      394 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/plonemeetingskin_images/pm_search.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      178 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/plonemeetingskin_images/backToValidatedForInput.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2534 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/plonemeetingskin_images/logo.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      320 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/plonemeetingskin_images/pm_preferences.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      481 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/plonemeetingskin_images/pm_home.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4670 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/plonemeetingskin_images/favicon.ico
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      317 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/plonemeetingskin_images/pm_config.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      123 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/plonemeetingskin_images/treeExpanded.gif
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/dmsmailskin_styles/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4463 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/dmsmailskin_styles/dmsmailskin.css.dtml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/pstskin_styles/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3477 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/pstskin_styles/pstskin.css.dtml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/plonemeetingskin_styles/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10503 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/plonemeetingskin_styles/plonemeetingskin.css.dtml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      161 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/plonemeetingskin_styles/CONTENT.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_styles/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11850 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_styles/urbanskin.css.dtml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/imioapps_styles/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1004 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/imioapps_styles/imioapps_ckeditor_moonolisa.css.dtml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7005 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/imioapps_styles/livesearch_reply.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      604 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/imioapps_styles/ploneCustom.css.dtml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1558 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/imioapps_styles/imioapps_properties.props
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      640 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/imioapps_styles/imioapps_IEFixes.css.dtml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    42202 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/imioapps_styles/imioapps.css.dtml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/imioapps_images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    33676 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/imioapps_images/spinner_small.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      326 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/imioapps_images/header-bg.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      546 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/imioapps_images/search_local_check.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      775 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/imioapps_images/filtre_sous.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       63 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/imioapps_images/exclamation.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      855 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/imioapps_images/filtre_add.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      823 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/imioapps_images/help.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      470 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/imioapps_images/search_button_icon.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    36210 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/imioapps_images/spinner.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      462 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/imioapps_images/search_local.png
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/pstskin_images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4964 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/pstskin_images/logo.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3758 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/pstskin_images/favicon.ico
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/dmsmailskin_images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1917 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/dmsmailskin_images/logo.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3362 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/dmsmailskin_images/favicon.ico
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1496 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/configure.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/locales/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      495 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/locales/eea.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/locales/en/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      683 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/locales/en/LC_MESSAGES/plone.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      591 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/locales/en/LC_MESSAGES/eea.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      706 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/locales/plone.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/locales/fr/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      836 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/locales/fr/LC_MESSAGES/plone.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      620 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/locales/fr/LC_MESSAGES/eea.po
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/testing/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      171 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/testing/metadata.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/default/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      174 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/default/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      558 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/default/registry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      221 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/default/viewlets.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      616 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/default/skins.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      976 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/default/cssregistry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      337 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/default/jsregistry.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/to_123/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      601 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/to_123/skins.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/pstskin/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      173 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/pstskin/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      402 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/pstskin/viewlets.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      750 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/pstskin/skins.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      301 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/pstskin/cssregistry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/pstskin/pstskin_marker.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      399 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/pstskin/import_steps.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/plonemeetingskin/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/plonemeetingskin/plonemeetingskin_marker.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      173 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/plonemeetingskin/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1132 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/plonemeetingskin/viewlets.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      831 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/plonemeetingskin/skins.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      310 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/plonemeetingskin/cssregistry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      421 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/plonemeetingskin/import_steps.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/uninstall/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/uninstall/uninstall_marker.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1483 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/uninstall/skins.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      314 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/uninstall/import_steps.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/urbanskin/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      173 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/urbanskin/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      559 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/urbanskin/viewlets.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      768 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/urbanskin/skins.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/urbanskin/urbanskin_marker.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      303 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/urbanskin/cssregistry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      405 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/urbanskin/import_steps.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/dmsmailskin/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      173 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/dmsmailskin/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/dmsmailskin/dmsmailskin_marker.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      943 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/dmsmailskin/viewlets.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      798 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/dmsmailskin/skins.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/dmsmailskin/cssregistry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      426 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/dmsmailskin/import_steps.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      642 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/testing.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      735 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/interfaces.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     3129 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/mk_sync_locales.sh
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      569 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/testing.zcml
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)       47 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/svn.ignore
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/Extensions/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1334 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/Extensions/Install.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       24 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/Extensions/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/tests/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      798 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/tests/test_example.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/tests/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      347 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/upgrades.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      214 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/browser/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/browser/static/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1296 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/browser/static/skin.js
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      944 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/browser/overrides.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2277 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/browser/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1756 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/browser/viewlets.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/browser/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      288 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/browser/templates/viewlet_workflowstate.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       92 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/browser/templates/empty.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      265 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/browser/templates/help.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/browser/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4760 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       56 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/src/plonetheme/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme.imioapps.egg-info/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme.imioapps.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       89 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme.imioapps.egg-info/entry_points.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       11 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme.imioapps.egg-info/namespace_packages.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       11 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme.imioapps.egg-info/top_level.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    25566 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme.imioapps.egg-info/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    17444 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme.imioapps.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme.imioapps.egg-info/not-zip-safe
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      100 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/src/plonetheme.imioapps.egg-info/requires.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/docs/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      729 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/docs/LICENSE.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/docs/LICENSE.GPL
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1570 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    25566 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      469 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/MANIFEST.in
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18547 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/CHANGES.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      674 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/README.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       78 2024-05-27 10:30:19.000000 plonetheme.imioapps-2.48/setup.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      333 2024-05-27 10:30:18.000000 plonetheme.imioapps-2.48/buildout.cfg
```

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins.zcml` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins.zcml`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/CODT_BuildLicence.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/CODT_BuildLicence.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/coring.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/coring.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/EnvClassTwo.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/EnvClassTwo.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/EnvironmentRubricTerm.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/EnvironmentRubricTerm.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/goback.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/goback.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/OpinionEventConfig.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/OpinionEventConfig.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanTool.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanTool.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/PreliminaryNotice.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/PreliminaryNotice.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Equipment.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Equipment.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/getemails.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/getemails.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Division.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Division.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanConfigurationValue.gif` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanConfigurationValue.gif`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/EventConfig.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/EventConfig.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Locality.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Locality.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/OpinionRequestEventType.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/OpinionRequestEventType.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/RecipientCadastre.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/RecipientCadastre.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/question-mark.gif` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/question-mark.gif`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/AskOpinionEventType.gif` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/AskOpinionEventType.gif`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanDelay.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanDelay.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/EnvClassOne.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/EnvClassOne.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/CODT_IntegratedLicence.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/CODT_IntegratedLicence.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/CODT_Inquiry.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/CODT_Inquiry.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/BuildLicence.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/BuildLicence.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/PersonTitleTerm.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/PersonTitleTerm.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/CODT_ParcelOutLicence.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/CODT_ParcelOutLicence.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventOpinionRequest.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventOpinionRequest.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/EnvironmentLicence.gif` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/EnvironmentLicence.gif`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/EnvClassBordering.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/EnvClassBordering.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanVocabularyTerm.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanVocabularyTerm.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Inquiry.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Inquiry.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/ParcellingTerm.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/ParcellingTerm.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/refuse.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/refuse.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/viewlet-firefox.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/viewlet-firefox.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Article127.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Article127.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/TextConfig.gif` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/TextConfig.gif`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/CODT_Article127.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/CODT_Article127.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/PortionOut.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/PortionOut.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Geometrician.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Geometrician.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/CODT_UniqueLicenceInquiry.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/CODT_UniqueLicenceInquiry.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/logo.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/logo.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/EnvironmentBase.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/EnvironmentBase.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/FolderManager.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/FolderManager.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Parcel.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Parcel.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/OpinionRequestEventType.gif` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/OpinionRequestEventType.gif`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/urban-sprite.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/urban-sprite.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Contact.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Contact.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/inacceptable.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/inacceptable.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/CODT_NotaryLetter.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/CODT_NotaryLetter.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanCertificateTwo.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanCertificateTwo.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/ExplosivesPossession.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/ExplosivesPossession.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/PcaTerm.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/PcaTerm.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventType.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventType.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/ParcelOutLicence.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/ParcelOutLicence.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/schedule.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/schedule.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/duplicate_licence.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/duplicate_licence.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/linkedhistoricfolders.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/linkedhistoricfolders.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/old.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/old.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Architect.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Architect.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/CODT_UrbanCertificateTwo.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/CODT_UrbanCertificateTwo.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/EnvClassThree.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/EnvClassThree.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Parcelling.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Parcelling.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/WorkLocation.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/WorkLocation.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/copytoclaymants.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/copytoclaymants.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/attachment.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/attachment.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventAnnouncement.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventAnnouncement.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/xml.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/xml.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/reopen.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/reopen.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UniqueLicence.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UniqueLicence.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/City.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/City.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/IntegratedLicence.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/IntegratedLicence.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEvent.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEvent.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/iscomplete.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/iscomplete.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/GenericLicence.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/GenericLicence.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Inspection.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Inspection.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Recipient.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Recipient.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/MiscDemand.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/MiscDemand.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Lot.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Lot.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Applicant.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Applicant.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/OrganisationTerm.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/OrganisationTerm.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/NotaryLetter.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/NotaryLetter.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/FollowUpEventType.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/FollowUpEventType.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventMayor.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventMayor.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/accept.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/accept.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/isincomplete.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/isincomplete.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/ProjectMeeting.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/ProjectMeeting.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/SpecificFeatureTerm.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/SpecificFeatureTerm.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/CODT_CommercialLicence.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/CODT_CommercialLicence.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Layer.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Layer.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/parcelhistoric.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/parcelhistoric.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/CODT_UrbanCertificateOne.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/CODT_UrbanCertificateOne.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/CODT_UniqueLicence.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/CODT_UniqueLicence.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanDoc.gif` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanDoc.gif`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/linkedfolders.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/linkedfolders.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/close.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/close.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanCertificateOne.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanCertificateOne.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventInquiry.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventInquiry.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanCertificateBase.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanCertificateBase.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/engrenage.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/engrenage.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventAcknowledgment.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventAcknowledgment.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/FollowUpEventConfig.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/FollowUpEventConfig.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/assign.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/assign.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventNotificationCollege.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventNotificationCollege.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/lock.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/lock.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventCollege.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/UrbanEventCollege.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Notary.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Notary.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/Proprietary.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/Proprietary.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_images/LicenceConfig.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_images/LicenceConfig.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/plonemeetingskin_images/logo.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/plonemeetingskin_images/logo.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/plonemeetingskin_images/favicon.ico` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/plonemeetingskin_images/favicon.ico`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/dmsmailskin_styles/dmsmailskin.css.dtml` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/dmsmailskin_styles/dmsmailskin.css.dtml`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/pstskin_styles/pstskin.css.dtml` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/pstskin_styles/pstskin.css.dtml`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/plonemeetingskin_styles/plonemeetingskin.css.dtml` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/plonemeetingskin_styles/plonemeetingskin.css.dtml`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/urbanskin_styles/urbanskin.css.dtml` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/urbanskin_styles/urbanskin.css.dtml`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/imioapps_styles/imioapps_ckeditor_moonolisa.css.dtml` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/imioapps_styles/imioapps_ckeditor_moonolisa.css.dtml`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/imioapps_styles/livesearch_reply.py` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/imioapps_styles/livesearch_reply.py`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/imioapps_styles/ploneCustom.css.dtml` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/imioapps_styles/ploneCustom.css.dtml`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/imioapps_styles/imioapps_properties.props` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/imioapps_styles/imioapps_properties.props`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/imioapps_styles/imioapps_IEFixes.css.dtml` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/imioapps_styles/imioapps_IEFixes.css.dtml`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/imioapps_styles/imioapps.css.dtml` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/imioapps_styles/imioapps.css.dtml`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/imioapps_images/spinner_small.gif` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/imioapps_images/spinner_small.gif`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/imioapps_images/search_local_check.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/imioapps_images/search_local_check.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/imioapps_images/filtre_sous.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/imioapps_images/filtre_sous.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/imioapps_images/filtre_add.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/imioapps_images/filtre_add.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/imioapps_images/help.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/imioapps_images/help.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/imioapps_images/spinner.gif` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/imioapps_images/spinner.gif`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/pstskin_images/logo.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/pstskin_images/logo.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/pstskin_images/favicon.ico` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/pstskin_images/favicon.ico`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/dmsmailskin_images/logo.png` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/dmsmailskin_images/logo.png`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/skins/dmsmailskin_images/favicon.ico` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/skins/dmsmailskin_images/favicon.ico`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/configure.zcml` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/configure.zcml`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/locales/en/LC_MESSAGES/plone.po` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/locales/en/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/locales/en/LC_MESSAGES/eea.po` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/locales/en/LC_MESSAGES/eea.po`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/locales/plone.pot` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/locales/plone.pot`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/locales/fr/LC_MESSAGES/plone.po` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/locales/fr/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/locales/fr/LC_MESSAGES/eea.po` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/locales/fr/LC_MESSAGES/eea.po`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/default/registry.xml` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/default/skins.xml` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/default/skins.xml`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/default/cssregistry.xml` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/default/cssregistry.xml`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/to_123/skins.xml` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/to_123/skins.xml`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/pstskin/skins.xml` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/pstskin/skins.xml`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/plonemeetingskin/viewlets.xml` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/plonemeetingskin/viewlets.xml`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/plonemeetingskin/skins.xml` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/plonemeetingskin/skins.xml`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/uninstall/skins.xml` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/uninstall/skins.xml`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/urbanskin/viewlets.xml` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/urbanskin/viewlets.xml`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/urbanskin/skins.xml` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/urbanskin/skins.xml`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/dmsmailskin/viewlets.xml` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/dmsmailskin/viewlets.xml`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles/dmsmailskin/skins.xml` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles/dmsmailskin/skins.xml`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/testing.py` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/testing.py`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/interfaces.py` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/interfaces.py`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/mk_sync_locales.sh` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/mk_sync_locales.sh`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/testing.zcml` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/testing.zcml`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/Extensions/Install.py` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/Extensions/Install.py`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/tests/test_example.py` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/tests/test_example.py`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/browser/static/skin.js` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/browser/static/skin.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -15,15 +15,15 @@
     document.body.appendChild(sheet);
 }
 $(window).resize(resizeHeader);
 
 // when using a imio-test instance, highlight header
 function highlightTest() {
     var url = $("link[rel='canonical']").attr('href');
-    if (url.includes('imio-test') || url.includes('preprod')) {
+    if (url.includes('.imio-test.be')) {
         $("div#portal-header")[0].style.background = "#d00";
     }
 }
 
 var isChrome = /chrom/.test(navigator.userAgent.toLowerCase());
 var isFirefox = /firefox/.test(navigator.userAgent.toLowerCase());
```

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/browser/overrides.py` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/browser/overrides.py`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/browser/configure.zcml` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/browser/viewlets.py` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/browser/viewlets.py`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme/imioapps/profiles.zcml` & `plonetheme.imioapps-2.48/src/plonetheme/imioapps/profiles.zcml`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/src/plonetheme.imioapps.egg-info/PKG-INFO` & `plonetheme.imioapps-2.48/src/plonetheme.imioapps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plonetheme.imioapps
-Version: 2.47
+Version: 2.48
 Summary: Plone theme for most Imio applications
 Home-page: https://github.com/IMIO/plonetheme.imioapps/
 Author: IMIO team
 Author-email: devs@imio.be
 License: gpl
 Description: ====================
         ploneteme.imioapps
@@ -43,14 +43,21 @@
           }
         
         
         Changelog
         =========
         
         
+        2.48 (2024-05-27)
+        -----------------
+        
+        - Be more defensive when changing header color to red for test instances
+          to avoid elements containing imio-test in id url being wrongly skinned.
+          [gbastien]
+        
         2.47 (2024-04-10)
         -----------------
         
         - URB-3007. Make caduc and abandoned workflow state grey in urban
           [jchandelle]
         - Add justice contact icon
           [ndemonte]
```

### Comparing `plonetheme.imioapps-2.47/src/plonetheme.imioapps.egg-info/SOURCES.txt` & `plonetheme.imioapps-2.48/src/plonetheme.imioapps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/docs/LICENSE.txt` & `plonetheme.imioapps-2.48/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/docs/LICENSE.GPL` & `plonetheme.imioapps-2.48/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plonetheme.imioapps-2.47/setup.py` & `plonetheme.imioapps-2.48/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = '2.47'
+version = '2.48'
 
 long_description = (
     open('README.rst').read()
     + '\n\n' +
     open('CHANGES.rst').read()
     + '\n')
```

### Comparing `plonetheme.imioapps-2.47/PKG-INFO` & `plonetheme.imioapps-2.48/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plonetheme.imioapps
-Version: 2.47
+Version: 2.48
 Summary: Plone theme for most Imio applications
 Home-page: https://github.com/IMIO/plonetheme.imioapps/
 Author: IMIO team
 Author-email: devs@imio.be
 License: gpl
 Description: ====================
         ploneteme.imioapps
@@ -43,14 +43,21 @@
           }
         
         
         Changelog
         =========
         
         
+        2.48 (2024-05-27)
+        -----------------
+        
+        - Be more defensive when changing header color to red for test instances
+          to avoid elements containing imio-test in id url being wrongly skinned.
+          [gbastien]
+        
         2.47 (2024-04-10)
         -----------------
         
         - URB-3007. Make caduc and abandoned workflow state grey in urban
           [jchandelle]
         - Add justice contact icon
           [ndemonte]
```

### Comparing `plonetheme.imioapps-2.47/CHANGES.rst` & `plonetheme.imioapps-2.48/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 Changelog
 =========
 
 
+2.48 (2024-05-27)
+-----------------
+
+- Be more defensive when changing header color to red for test instances
+  to avoid elements containing imio-test in id url being wrongly skinned.
+  [gbastien]
+
 2.47 (2024-04-10)
 -----------------
 
 - URB-3007. Make caduc and abandoned workflow state grey in urban
   [jchandelle]
 - Add justice contact icon
   [ndemonte]
```

### Comparing `plonetheme.imioapps-2.47/README.rst` & `plonetheme.imioapps-2.48/README.rst`

 * *Files identical despite different names*

