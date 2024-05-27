# Comparing `tmp/guarddog-1.8.0.tar.gz` & `tmp/guarddog-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guarddog-1.8.0.tar", max compression
+gzip compressed data, was "guarddog-1.8.1.tar", max compression
```

## Comparing `guarddog-1.8.0.tar` & `guarddog-1.8.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0    11377 2024-05-23 11:15:19.322424 guarddog-1.8.0/LICENSE
--rw-r--r--   0        0        0      314 2024-05-23 11:15:19.322424 guarddog-1.8.0/LICENSE-3rdparty.csv
--rw-r--r--   0        0        0      140 2024-05-23 11:15:19.322424 guarddog-1.8.0/NOTICE
--rw-r--r--   0        0        0      154 2024-05-23 11:15:19.322424 guarddog-1.8.0/guarddog/__init__.py
--rw-r--r--   0        0        0      246 2024-05-23 11:15:19.322424 guarddog-1.8.0/guarddog/__main__.py
--rw-r--r--   0        0        0        0 2024-05-23 11:15:19.322424 guarddog-1.8.0/guarddog/analyzer/__init__.py
--rw-r--r--   0        0        0     9791 2024-05-23 11:15:19.322424 guarddog-1.8.0/guarddog/analyzer/analyzer.py
--rw-r--r--   0        0        0      457 2024-05-23 11:15:19.322424 guarddog-1.8.0/guarddog/analyzer/metadata/__init__.py
--rw-r--r--   0        0        0     1840 2024-05-23 11:15:19.322424 guarddog-1.8.0/guarddog/analyzer/metadata/bundled_binary.py
--rw-r--r--   0        0        0      609 2024-05-23 11:15:19.322424 guarddog-1.8.0/guarddog/analyzer/metadata/detector.py
--rw-r--r--   0        0        0     1166 2024-05-23 11:15:19.322424 guarddog-1.8.0/guarddog/analyzer/metadata/empty_information.py
--rw-r--r--   0        0        0     1223 2024-05-23 11:15:19.322424 guarddog-1.8.0/guarddog/analyzer/metadata/npm/__init__.py
--rw-r--r--   0        0        0      360 2024-05-23 11:15:19.322424 guarddog-1.8.0/guarddog/analyzer/metadata/npm/bundled_binary.py
--rw-r--r--   0        0        0     2449 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/npm/direct_url_dependency.py
--rw-r--r--   0        0        0      793 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/npm/empty_information.py
--rw-r--r--   0        0        0     4428 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/npm/npm_metadata_mismatch.py
--rw-r--r--   0        0        0     1643 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/npm/potentially_compromised_email_domain.py
--rw-r--r--   0        0        0      578 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/npm/release_zero.py
--rw-r--r--   0        0        0     1732 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/npm/typosquatting.py
--rw-r--r--   0        0        0      899 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/npm/unclaimed_maintainer_email_domain.py
--rw-r--r--   0        0        0      461 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/npm/utils.py
--rw-r--r--   0        0        0     2806 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/potentially_compromised_email_domain.py
--rw-r--r--   0        0        0     1251 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/pypi/__init__.py
--rw-r--r--   0        0        0      361 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/pypi/bundled_binary.py
--rw-r--r--   0        0        0      723 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/pypi/empty_information.py
--rw-r--r--   0        0        0     1679 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/pypi/potentially_compromised_email_domain.py
--rw-r--r--   0        0        0      716 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/pypi/release_zero.py
--rw-r--r--   0        0        0    11635 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/pypi/repository_integrity_mismatch.py
--rw-r--r--   0        0        0     1369 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/pypi/single_python_file.py
--rw-r--r--   0        0        0     3490 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/pypi/typosquatting.py
--rw-r--r--   0        0        0      406 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/pypi/unclaimed_maintainer_email_domain.py
--rw-r--r--   0        0        0      199 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/pypi/utils.py
--rw-r--r--   0        0        0      438 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/release_zero.py
--rw-r--r--   0        0        0      743 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/repository_integrity_mismatch.py
--rw-r--r--   0        0        0   373303 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/resources/top_npm_packages.json
--rw-r--r--   0        0        0   387251 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/metadata/resources/top_pypi_packages.json
--rw-r--r--   0        0        0     5619 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/metadata/typosquatting.py
--rw-r--r--   0        0        0     2343 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/metadata/unclaimed_maintainer_email_domain.py
--rw-r--r--   0        0        0     1603 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/metadata/utils.py
--rw-r--r--   0        0        0     1043 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/__init__.py
--rw-r--r--   0        0        0      524 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/clipboard-access.yml
--rw-r--r--   0        0        0      682 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/cmd-overwrite.yml
--rw-r--r--   0        0        0     4655 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/code-execution.yml
--rw-r--r--   0        0        0     3055 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/download-executable.yml
--rw-r--r--   0        0        0     2371 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/exec-base64.yml
--rw-r--r--   0        0        0     1815 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/exfiltrate-sensitive-data.yml
--rw-r--r--   0        0        0      576 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/npm-exec-base64.yml
--rw-r--r--   0        0        0     3011 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/npm-exfiltrate-sensitive-data.yml
--rw-r--r--   0        0        0     1067 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/npm-install-script.yml
--rw-r--r--   0        0        0     2100 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/npm-obfuscation.yml
--rw-r--r--   0        0        0      835 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/npm-serialize-environment.yml
--rw-r--r--   0        0        0     3513 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/npm-silent-process-execution.yml
--rw-r--r--   0        0        0      582 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/obfuscation.yml
--rw-r--r--   0        0        0     1609 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/shady-links.yml
--rw-r--r--   0        0        0      418 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/silent-process-execution.yml
--rw-r--r--   0        0        0      606 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/steganography.yml
--rw-r--r--   0        0        0    13215 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/cli.py
--rw-r--r--   0        0        0      315 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/ecosystems.py
--rw-r--r--   0        0        0        0 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/reporters/__init__.py
--rw-r--r--   0        0        0     6189 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/reporters/sarif.py
--rw-r--r--   0        0        0      752 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/scanners/__init__.py
--rw-r--r--   0        0        0     1968 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/scanners/npm_package_scanner.py
--rw-r--r--   0        0        0     2243 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/scanners/npm_project_scanner.py
--rw-r--r--   0        0        0     2512 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/scanners/pypi_package_scanner.py
--rw-r--r--   0        0        0     5491 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/scanners/pypi_project_scanner.py
--rw-r--r--   0        0        0    11170 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/scanners/scanner.py
--rw-r--r--   0        0        0        0 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/utils/__init__.py
--rw-r--r--   0        0        0     1323 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/utils/archives.py
--rw-r--r--   0        0        0       54 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/utils/exceptions.py
--rw-r--r--   0        0        0      953 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/utils/package_info.py
--rw-r--r--   0        0        0       52 2024-05-23 11:15:19.330424 guarddog-1.8.0/pypi.rst
--rw-r--r--   0        0        0     1222 2024-05-23 11:15:28.242414 guarddog-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 guarddog-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11377 2024-05-27 09:24:22.022132 guarddog-1.8.1/LICENSE
+-rw-r--r--   0        0        0      314 2024-05-27 09:24:22.022132 guarddog-1.8.1/LICENSE-3rdparty.csv
+-rw-r--r--   0        0        0      140 2024-05-27 09:24:22.022132 guarddog-1.8.1/NOTICE
+-rw-r--r--   0        0        0      154 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/__init__.py
+-rw-r--r--   0        0        0      246 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/__init__.py
+-rw-r--r--   0        0        0     9808 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/analyzer.py
+-rw-r--r--   0        0        0      457 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/__init__.py
+-rw-r--r--   0        0        0     1840 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/bundled_binary.py
+-rw-r--r--   0        0        0      609 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/detector.py
+-rw-r--r--   0        0        0     1166 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/empty_information.py
+-rw-r--r--   0        0        0     1223 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/npm/__init__.py
+-rw-r--r--   0        0        0      360 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/npm/bundled_binary.py
+-rw-r--r--   0        0        0     2449 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/npm/direct_url_dependency.py
+-rw-r--r--   0        0        0      793 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/npm/empty_information.py
+-rw-r--r--   0        0        0     4428 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/npm/npm_metadata_mismatch.py
+-rw-r--r--   0        0        0     1643 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/npm/potentially_compromised_email_domain.py
+-rw-r--r--   0        0        0      578 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/npm/release_zero.py
+-rw-r--r--   0        0        0     1732 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/npm/typosquatting.py
+-rw-r--r--   0        0        0      899 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/npm/unclaimed_maintainer_email_domain.py
+-rw-r--r--   0        0        0      461 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/npm/utils.py
+-rw-r--r--   0        0        0     2806 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/potentially_compromised_email_domain.py
+-rw-r--r--   0        0        0     1251 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/pypi/__init__.py
+-rw-r--r--   0        0        0      361 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/pypi/bundled_binary.py
+-rw-r--r--   0        0        0      723 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/pypi/empty_information.py
+-rw-r--r--   0        0        0     1679 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/pypi/potentially_compromised_email_domain.py
+-rw-r--r--   0        0        0      716 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/pypi/release_zero.py
+-rw-r--r--   0        0        0    11635 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/pypi/repository_integrity_mismatch.py
+-rw-r--r--   0        0        0     1369 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/pypi/single_python_file.py
+-rw-r--r--   0        0        0     3490 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/pypi/typosquatting.py
+-rw-r--r--   0        0        0      406 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/pypi/unclaimed_maintainer_email_domain.py
+-rw-r--r--   0        0        0      199 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/pypi/utils.py
+-rw-r--r--   0        0        0      438 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/release_zero.py
+-rw-r--r--   0        0        0      743 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/repository_integrity_mismatch.py
+-rw-r--r--   0        0        0   373303 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/resources/top_npm_packages.json
+-rw-r--r--   0        0        0   387251 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/metadata/resources/top_pypi_packages.json
+-rw-r--r--   0        0        0     5619 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/metadata/typosquatting.py
+-rw-r--r--   0        0        0     2343 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/metadata/unclaimed_maintainer_email_domain.py
+-rw-r--r--   0        0        0     1603 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/metadata/utils.py
+-rw-r--r--   0        0        0     1043 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/__init__.py
+-rw-r--r--   0        0        0      524 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/clipboard-access.yml
+-rw-r--r--   0        0        0      682 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/cmd-overwrite.yml
+-rw-r--r--   0        0        0     4655 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/code-execution.yml
+-rw-r--r--   0        0        0     3055 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/download-executable.yml
+-rw-r--r--   0        0        0     2371 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/exec-base64.yml
+-rw-r--r--   0        0        0     1815 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/exfiltrate-sensitive-data.yml
+-rw-r--r--   0        0        0      576 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/npm-exec-base64.yml
+-rw-r--r--   0        0        0     3011 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/npm-exfiltrate-sensitive-data.yml
+-rw-r--r--   0        0        0     1067 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/npm-install-script.yml
+-rw-r--r--   0        0        0     2160 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/npm-obfuscation.yml
+-rw-r--r--   0        0        0      835 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/npm-serialize-environment.yml
+-rw-r--r--   0        0        0     3513 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/npm-silent-process-execution.yml
+-rw-r--r--   0        0        0      582 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/obfuscation.yml
+-rw-r--r--   0        0        0     1609 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/shady-links.yml
+-rw-r--r--   0        0        0      418 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/silent-process-execution.yml
+-rw-r--r--   0        0        0      606 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/steganography.yml
+-rw-r--r--   0        0        0    14557 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/cli.py
+-rw-r--r--   0        0        0      315 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/ecosystems.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/reporters/__init__.py
+-rw-r--r--   0        0        0     6189 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/reporters/sarif.py
+-rw-r--r--   0        0        0      752 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/scanners/__init__.py
+-rw-r--r--   0        0        0     1968 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/scanners/npm_package_scanner.py
+-rw-r--r--   0        0        0     2243 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/scanners/npm_project_scanner.py
+-rw-r--r--   0        0        0     2512 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/scanners/pypi_package_scanner.py
+-rw-r--r--   0        0        0     5491 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/scanners/pypi_project_scanner.py
+-rw-r--r--   0        0        0    11170 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/scanners/scanner.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/utils/__init__.py
+-rw-r--r--   0        0        0     1323 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/utils/archives.py
+-rw-r--r--   0        0        0       54 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/utils/exceptions.py
+-rw-r--r--   0        0        0      953 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/utils/package_info.py
+-rw-r--r--   0        0        0       52 2024-05-27 09:24:22.034133 guarddog-1.8.1/pypi.rst
+-rw-r--r--   0        0        0     1222 2024-05-27 09:24:36.698221 guarddog-1.8.1/pyproject.toml
+-rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 guarddog-1.8.1/PKG-INFO
```

### Comparing `guarddog-1.8.0/LICENSE` & `guarddog-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/analyzer.py` & `guarddog-1.8.1/guarddog/analyzer/analyzer.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,24 +3,18 @@
 import os
 import subprocess
 from collections import defaultdict
 from pathlib import Path
 from typing import Iterable, List, Optional
 
 from guarddog.analyzer.metadata import get_metadata_detectors
+from guarddog.analyzer.sourcecode import SOURCECODE_RULES
 from guarddog.ecosystems import ECOSYSTEM
 
-
-def get_rules(file_extension, path):
-    return set(rule.replace(file_extension, "") for rule in os.listdir(path) if rule.endswith(file_extension))
-
-
 SEMGREP_MAX_TARGET_BYTES = 10_000_000
-SEMGREP_RULES_PATH = os.path.join(os.path.dirname(__file__), "sourcecode")
-SEMGREP_RULE_NAMES = get_rules(".yml", SEMGREP_RULES_PATH)
 
 log = logging.getLogger("guarddog")
 
 
 class Analyzer:
     """
     Analyzes a local directory for threats found by source code or metadata rules
@@ -41,15 +35,15 @@
 
         self.ecosystem = ecosystem
 
         # Rules and associated detectors
         self.metadata_detectors = get_metadata_detectors(ecosystem)
 
         self.metadata_ruleset = self.metadata_detectors.keys()
-        self.sourcecode_ruleset = SEMGREP_RULE_NAMES
+        self.sourcecode_ruleset = [rule["id"] for rule in SOURCECODE_RULES[ecosystem]]
 
         # Define paths to exclude from sourcecode analysis
         self.exclude = [
             "helm",
             ".idea",
             "venv",
             "test",
@@ -124,22 +118,26 @@
             rules (set, optional): Set of metadata rules to analyze. Defaults to all rules.
 
         Returns:
             dict[str]: map from each metadata rule and their corresponding output
         """
 
         all_rules = rules if rules is not None else self.metadata_ruleset
-        results = {}
+
+        # for each metadata rule, is expected to have an nulleable string as result
+        # None value represents that the rule was not matched
+        results: dict[str, Optional[str]] = {}
         errors = {}
         issues = 0
 
         for rule in all_rules:
             try:
                 log.debug(f"Running rule {rule} against package '{name}'")
                 rule_matches, message = self.metadata_detectors[rule].detect(info, path, name, version)
+                results[rule] = None
                 if rule_matches:
                     issues += 1
                     results[rule] = message
             except Exception as e:
                 errors[rule] = f"failed to run rule {rule}: {str(e)}"
 
         return {"results": results, "errors": errors, "issues": issues}
```

### Comparing `guarddog-1.8.0/guarddog/analyzer/metadata/bundled_binary.py` & `guarddog-1.8.1/guarddog/analyzer/metadata/bundled_binary.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/metadata/detector.py` & `guarddog-1.8.1/guarddog/analyzer/metadata/detector.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/metadata/empty_information.py` & `guarddog-1.8.1/guarddog/analyzer/metadata/empty_information.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/metadata/npm/__init__.py` & `guarddog-1.8.1/guarddog/analyzer/metadata/npm/__init__.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/metadata/npm/direct_url_dependency.py` & `guarddog-1.8.1/guarddog/analyzer/metadata/npm/direct_url_dependency.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/metadata/npm/empty_information.py` & `guarddog-1.8.1/guarddog/analyzer/metadata/npm/empty_information.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/metadata/npm/npm_metadata_mismatch.py` & `guarddog-1.8.1/guarddog/analyzer/metadata/npm/npm_metadata_mismatch.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/metadata/npm/potentially_compromised_email_domain.py` & `guarddog-1.8.1/guarddog/analyzer/metadata/npm/potentially_compromised_email_domain.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/metadata/npm/release_zero.py` & `guarddog-1.8.1/guarddog/analyzer/metadata/npm/release_zero.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/metadata/npm/typosquatting.py` & `guarddog-1.8.1/guarddog/analyzer/metadata/npm/typosquatting.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/metadata/npm/unclaimed_maintainer_email_domain.py` & `guarddog-1.8.1/guarddog/analyzer/metadata/npm/unclaimed_maintainer_email_domain.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/metadata/potentially_compromised_email_domain.py` & `guarddog-1.8.1/guarddog/analyzer/metadata/potentially_compromised_email_domain.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/metadata/pypi/__init__.py` & `guarddog-1.8.1/guarddog/analyzer/metadata/pypi/__init__.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/metadata/pypi/empty_information.py` & `guarddog-1.8.1/guarddog/analyzer/metadata/pypi/empty_information.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/metadata/pypi/potentially_compromised_email_domain.py` & `guarddog-1.8.1/guarddog/analyzer/metadata/pypi/potentially_compromised_email_domain.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/metadata/pypi/release_zero.py` & `guarddog-1.8.1/guarddog/analyzer/metadata/pypi/release_zero.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/metadata/pypi/repository_integrity_mismatch.py` & `guarddog-1.8.1/guarddog/analyzer/metadata/pypi/repository_integrity_mismatch.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/metadata/pypi/single_python_file.py` & `guarddog-1.8.1/guarddog/analyzer/metadata/pypi/single_python_file.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/metadata/pypi/typosquatting.py` & `guarddog-1.8.1/guarddog/analyzer/metadata/pypi/typosquatting.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/metadata/repository_integrity_mismatch.py` & `guarddog-1.8.1/guarddog/analyzer/metadata/repository_integrity_mismatch.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/metadata/resources/top_npm_packages.json` & `guarddog-1.8.1/guarddog/analyzer/metadata/resources/top_npm_packages.json`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/metadata/resources/top_pypi_packages.json` & `guarddog-1.8.1/guarddog/analyzer/metadata/resources/top_pypi_packages.json`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/metadata/typosquatting.py` & `guarddog-1.8.1/guarddog/analyzer/metadata/typosquatting.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/metadata/unclaimed_maintainer_email_domain.py` & `guarddog-1.8.1/guarddog/analyzer/metadata/unclaimed_maintainer_email_domain.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/metadata/utils.py` & `guarddog-1.8.1/guarddog/analyzer/metadata/utils.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/sourcecode/__init__.py` & `guarddog-1.8.1/guarddog/analyzer/sourcecode/__init__.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/sourcecode/clipboard-access.yml` & `guarddog-1.8.1/guarddog/analyzer/sourcecode/clipboard-access.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/sourcecode/cmd-overwrite.yml` & `guarddog-1.8.1/guarddog/analyzer/sourcecode/cmd-overwrite.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/sourcecode/code-execution.yml` & `guarddog-1.8.1/guarddog/analyzer/sourcecode/code-execution.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/sourcecode/download-executable.yml` & `guarddog-1.8.1/guarddog/analyzer/sourcecode/download-executable.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/sourcecode/exec-base64.yml` & `guarddog-1.8.1/guarddog/analyzer/sourcecode/exec-base64.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/sourcecode/exfiltrate-sensitive-data.yml` & `guarddog-1.8.1/guarddog/analyzer/sourcecode/exfiltrate-sensitive-data.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/sourcecode/npm-exec-base64.yml` & `guarddog-1.8.1/guarddog/analyzer/sourcecode/npm-exec-base64.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/sourcecode/npm-exfiltrate-sensitive-data.yml` & `guarddog-1.8.1/guarddog/analyzer/sourcecode/npm-exfiltrate-sensitive-data.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/sourcecode/npm-install-script.yml` & `guarddog-1.8.1/guarddog/analyzer/sourcecode/npm-install-script.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/sourcecode/npm-obfuscation.yml` & `guarddog-1.8.1/guarddog/analyzer/sourcecode/npm-obfuscation.yml`

 * *Files 8% similar despite different names*

```diff
@@ -51,13 +51,15 @@
               regex: ("\w+"|'\w+'|,)*
           - pattern: '<...$PARAM...>'
           - metavariable-analysis:
               analyzer: entropy
               metavariable: $PARAM
 
         # JSFuck 
-        - pattern-regex: ^\s*[\[\]\(\)\+\!]{10,}\s*$
+        - patterns:
+          - pattern-not-inside: "..."
+          - pattern-regex: ^\s*[\[\]\(\)\+\!]{10,}\s*$
     languages:
       - javascript
     severity: WARNING
     options: 
       symbolic_propagation: true
```

### Comparing `guarddog-1.8.0/guarddog/analyzer/sourcecode/npm-serialize-environment.yml` & `guarddog-1.8.1/guarddog/analyzer/sourcecode/npm-serialize-environment.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/sourcecode/npm-silent-process-execution.yml` & `guarddog-1.8.1/guarddog/analyzer/sourcecode/npm-silent-process-execution.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/sourcecode/obfuscation.yml` & `guarddog-1.8.1/guarddog/analyzer/sourcecode/obfuscation.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/sourcecode/shady-links.yml` & `guarddog-1.8.1/guarddog/analyzer/sourcecode/shady-links.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/analyzer/sourcecode/steganography.yml` & `guarddog-1.8.1/guarddog/analyzer/sourcecode/steganography.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/cli.py` & `guarddog-1.8.1/guarddog/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,138 @@
 """ PyPI Package Malware Scanner
 
 CLI command that scans a PyPI package version for user-specified malware flags.
 Includes rules based on package registry metadata and source code analysis.
 """
+
 import logging
 import os
 import sys
 from typing import cast, Optional
+import json as js
 
 import click
 from prettytable import PrettyTable
 from termcolor import colored
 
-from guarddog.analyzer.analyzer import SEMGREP_RULE_NAMES
 from guarddog.analyzer.metadata import get_metadata_detectors
 from guarddog.analyzer.sourcecode import SOURCECODE_RULES
 from guarddog.ecosystems import ECOSYSTEM
 from guarddog.reporters.sarif import report_verify_sarif
 from guarddog.scanners import get_scanner
 from guarddog.scanners.scanner import PackageScanner
 
-ALL_RULES = \
-    set(get_metadata_detectors(ECOSYSTEM.NPM).keys()) \
-    | set(get_metadata_detectors(ECOSYSTEM.PYPI).keys()) | SEMGREP_RULE_NAMES
-NPM_RULES = set(get_metadata_detectors(ECOSYSTEM.NPM).keys()) | SEMGREP_RULE_NAMES
-PYPI_RULES = set(get_metadata_detectors(ECOSYSTEM.PYPI).keys()) | SEMGREP_RULE_NAMES
+ALL_RULES = (
+    set(get_metadata_detectors(ECOSYSTEM.NPM).keys())
+    | set(get_metadata_detectors(ECOSYSTEM.PYPI).keys())
+    | set(map(lambda r: r["id"], SOURCECODE_RULES[ECOSYSTEM.NPM]))
+    | set(map(lambda r: r["id"], SOURCECODE_RULES[ECOSYSTEM.PYPI]))
+)
+NPM_RULES = set(get_metadata_detectors(ECOSYSTEM.NPM).keys()) | set(
+    map(lambda r: r["id"], SOURCECODE_RULES[ECOSYSTEM.NPM])
+)
+PYPI_RULES = set(get_metadata_detectors(ECOSYSTEM.PYPI).keys()) | set(
+    map(lambda r: r["id"], SOURCECODE_RULES[ECOSYSTEM.PYPI])
+)
 EXIT_CODE_ISSUES_FOUND = 1
 
-AVAILABLE_LOG_LEVELS = {
-    logging.DEBUG,
-    logging.INFO,
-    logging.WARN,
-    logging.ERROR
-}
-AVAILABLE_LOG_LEVELS_NAMES = list(map(lambda level: logging.getLevelName(level), AVAILABLE_LOG_LEVELS))
+AVAILABLE_LOG_LEVELS = {logging.DEBUG, logging.INFO, logging.WARN, logging.ERROR}
+AVAILABLE_LOG_LEVELS_NAMES = list(
+    map(lambda level: logging.getLevelName(level), AVAILABLE_LOG_LEVELS)
+)
 
-log = logging.getLogger('guarddog')
+log = logging.getLogger("guarddog")
 
 
 def common_options(fn):
-    fn = click.option("--exit-non-zero-on-finding", default=False, is_flag=True,
-                      help="Exit with a non-zero status code if at least one issue is identified")(fn)
+    fn = click.option(
+        "--exit-non-zero-on-finding",
+        default=False,
+        is_flag=True,
+        help="Exit with a non-zero status code if at least one issue is identified",
+    )(fn)
     fn = click.argument("target")(fn)
     return fn
 
 
 def legacy_rules_options(fn):
-    fn = click.option("-r", "--rules", multiple=True, type=click.Choice(ALL_RULES, case_sensitive=False))(fn)
-    fn = click.option("-x", "--exclude-rules", multiple=True, type=click.Choice(ALL_RULES, case_sensitive=False))(fn)
+    fn = click.option(
+        "-r",
+        "--rules",
+        multiple=True,
+        type=click.Choice(ALL_RULES, case_sensitive=False),
+    )(fn)
+    fn = click.option(
+        "-x",
+        "--exclude-rules",
+        multiple=True,
+        type=click.Choice(ALL_RULES, case_sensitive=False),
+    )(fn)
     return fn
 
 
 def npm_options(fn):
-    fn = click.option("-r", "--rules", multiple=True, type=click.Choice(NPM_RULES, case_sensitive=False))(fn)
-    fn = click.option("-x", "--exclude-rules", multiple=True, type=click.Choice(NPM_RULES, case_sensitive=False))(fn)
+    fn = click.option(
+        "-r",
+        "--rules",
+        multiple=True,
+        type=click.Choice(NPM_RULES, case_sensitive=False),
+    )(fn)
+    fn = click.option(
+        "-x",
+        "--exclude-rules",
+        multiple=True,
+        type=click.Choice(NPM_RULES, case_sensitive=False),
+    )(fn)
     return fn
 
 
 def pypi_options(fn):
-    fn = click.option("-r", "--rules", multiple=True, type=click.Choice(PYPI_RULES, case_sensitive=False))(fn)
-    fn = click.option("-x", "--exclude-rules", multiple=True, type=click.Choice(PYPI_RULES, case_sensitive=False))(fn)
+    fn = click.option(
+        "-r",
+        "--rules",
+        multiple=True,
+        type=click.Choice(PYPI_RULES, case_sensitive=False),
+    )(fn)
+    fn = click.option(
+        "-x",
+        "--exclude-rules",
+        multiple=True,
+        type=click.Choice(PYPI_RULES, case_sensitive=False),
+    )(fn)
     return fn
 
 
 def verify_options(fn):
-    fn = click.option("--output-format", default=None, type=click.Choice(["json", "sarif"], case_sensitive=False))(fn)
+    fn = click.option(
+        "--output-format",
+        default=None,
+        type=click.Choice(["json", "sarif"], case_sensitive=False),
+    )(fn)
     return fn
 
 
 def scan_options(fn):
-    fn = click.option("--output-format", default=None, type=click.Choice(["json"], case_sensitive=False))(fn)
-    fn = click.option("-v", "--version", default=None, help="Specify a version to scan")(fn)
+    fn = click.option(
+        "--output-format",
+        default=None,
+        type=click.Choice(["json"], case_sensitive=False),
+    )(fn)
+    fn = click.option(
+        "-v", "--version", default=None, help="Specify a version to scan"
+    )(fn)
     return fn
 
 
 def logging_options(fn):
-    fn = click.option("--log-level", default="INFO",
-                      type=click.Choice(AVAILABLE_LOG_LEVELS_NAMES, case_sensitive=False))(fn)
+    fn = click.option(
+        "--log-level",
+        default="INFO",
+        type=click.Choice(AVAILABLE_LOG_LEVELS_NAMES, case_sensitive=False),
+    )(fn)
     return fn
 
 
 @click.group
 @logging_options
 def cli(log_level):
     """
@@ -88,293 +140,394 @@
 
     Supports PyPI and npm
 
     Example: guarddog pypi scan semantic-version
 
     Use --help for the detail of all commands and subcommands
     """
-    logger = logging.getLogger('guarddog')
+    logger = logging.getLogger("guarddog")
     logger.setLevel(logging.getLevelName(log_level))
     stdoutHandler = logging.StreamHandler(stream=sys.stdout)
     stdoutHandler.setFormatter(logging.Formatter("%(levelname)s: %(message)s"))
     logger.addHandler(stdoutHandler)
     pass
 
 
 def _get_rule_param(rules, exclude_rules, ecosystem):
     rule_param = None
     if len(rules) > 0:
         rule_param = rules
 
     if len(exclude_rules) > 0:
-        all_rules = SEMGREP_RULE_NAMES
-        if ecosystem == ECOSYSTEM.NPM:
-            all_rules |= set(get_metadata_detectors(ECOSYSTEM.NPM).keys())
-        elif ecosystem == ECOSYSTEM.PYPI:
-            all_rules |= set(get_metadata_detectors(ECOSYSTEM.PYPI).keys())
+        all_rules = set(map(lambda x: x["id"], SOURCECODE_RULES[ecosystem])) | set(
+            get_metadata_detectors(ecosystem).keys()
+        )
 
         rule_param = all_rules - set(exclude_rules)
 
         if len(rules) > 0:
             print("--rules and --exclude-rules cannot be used together")
             sys.exit(1)
 
     return rule_param
 
 
-def _verify(path, rules, exclude_rules, output_format, exit_non_zero_on_finding, ecosystem):
+def _verify(
+    path, rules, exclude_rules, output_format, exit_non_zero_on_finding, ecosystem
+):
     """Verify a requirements.txt file
 
     Args:
         path (str): path to requirements.txt file
     """
     return_value = None
     rule_param = _get_rule_param(rules, exclude_rules, ecosystem)
     scanner = get_scanner(ecosystem, True)
     if scanner is None:
         sys.stderr.write(f"Command verify is not supported for ecosystem {ecosystem}")
         exit(1)
 
     def display_result(result: dict) -> None:
-        identifier = result['dependency'] if result['version'] is None \
+        identifier = (
+            result["dependency"]
+            if result["version"] is None
             else f"{result['dependency']} version {result['version']}"
+        )
         if output_format is None:
-            print_scan_results(result.get('result'), identifier)
+            print_scan_results(result.get("result"), identifier)
 
-        if len(result.get('errors', [])) > 0:
-            print_errors(result.get('error'), identifier)
+        if len(result.get("errors", [])) > 0:
+            print_errors(result.get("error"), identifier)
 
     results = scanner.scan_local(path, rule_param, display_result)
     if output_format == "json":
-        import json as js
+
         return_value = js.dumps(results)
 
     if output_format == "sarif":
         sarif_rules = PYPI_RULES if ecosystem == ECOSYSTEM.PYPI else NPM_RULES
         return_value = report_verify_sarif(path, list(sarif_rules), results, ecosystem)
 
     if output_format is not None:
         print(return_value)
 
     if exit_non_zero_on_finding:
-        exit_with_status_code([result['result'] for result in results])
+        exit_with_status_code([result["result"] for result in results])
 
     return return_value  # this is mostly for testing
 
 
 def is_local_target(identifier: str) -> bool:
     """
     @param identifier:  The name/path of the package as passed to "guarddog ecosystem scan"
     @return:            Whether the identifier should be considered a local path
     """
-    if identifier.startswith("/") or identifier.startswith("./") or identifier.startswith("../"):
+    if (
+        identifier.startswith("/")
+        or identifier.startswith("./")
+        or identifier.startswith("../")
+    ):
         return True
 
     if identifier == ".":
         return True
 
     # If this looks like an archive, consider it as a local target if the target exists on the local filesystem
-    if identifier.endswith(".tar.gz") or identifier.endswith(".zip") or identifier.endswith(".whl"):
+    if (
+        identifier.endswith(".tar.gz")
+        or identifier.endswith(".zip")
+        or identifier.endswith(".whl")
+    ):
         return os.path.exists(identifier)
 
     return False
 
 
-def _scan(identifier, version, rules, exclude_rules, output_format, exit_non_zero_on_finding, ecosystem: ECOSYSTEM):
+def _scan(
+    identifier,
+    version,
+    rules,
+    exclude_rules,
+    output_format,
+    exit_non_zero_on_finding,
+    ecosystem: ECOSYSTEM,
+):
     """Scan a package
 
     Args:
         identifier (str): name or path to the package
         version (str): version of the package (ex. 1.0.0), defaults to most recent
         rules (list[str]): specific rules to run, defaults to all
     """
 
     rule_param = _get_rule_param(rules, exclude_rules, ecosystem)
     scanner = cast(Optional[PackageScanner], get_scanner(ecosystem, False))
     if scanner is None:
         sys.stderr.write(f"Command scan is not supported for ecosystem {ecosystem}")
         sys.exit(1)
+
     results = []
     if is_local_target(identifier):
-        log.debug(f"Considering that '{identifier}' is a local target, scanning filesystem")
+        log.debug(
+            f"Considering that '{identifier}' is a local target, scanning filesystem"
+        )
         if os.path.isdir(identifier):
             log.debug(f"Considering that '{identifier}' as a local directory")
             for package in os.listdir(identifier):
-                results.append({'package': package} | scanner.scan_local(f"{identifier}/{package}", rule_param))
+                result = scanner.scan_local(f"{identifier}/{package}", rule_param)
+                result["package"] = package
+                results.append(result)
         else:
-            results.append({'package': identifier} | scanner.scan_local(identifier, rule_param))
+            result = scanner.scan_local(identifier, rule_param)
+            result["package"] = identifier
+            results.append(result)
     else:
         log.debug(f"Considering that '{identifier}' is a remote target")
         try:
-            results.append({'package': identifier} | scanner.scan_remote(identifier, version, rule_param))
+            result = scanner.scan_remote(identifier, version, rule_param)
+            result["package"] = identifier
+            results.append(result)
         except Exception as e:
             sys.stderr.write(f"\nError '{e}' occurred while scanning remote package.")
             sys.exit(1)
 
     if output_format == "json":
-        import json as js
         if len(results) == 1:
             # return only a json like {}
             print(js.dumps(results[0]))
         else:
             # Return a list of result like [{},{}]
             print(js.dumps(results))
     else:
         for result in results:
-            print_scan_results(result, result['package'])
+            print_scan_results(result, result["package"])
 
     if exit_non_zero_on_finding:
         exit_with_status_code(results)
 
 
 def _list_rules(ecosystem):
     table = PrettyTable()
     table.align = "l"
     table.field_names = ["Rule type", "Rule name", "Description"]
 
     for rule in SOURCECODE_RULES[ecosystem]:
-        table.add_row(["Source code", rule['id'], rule.get('metadata', {}).get('description')])
+        table.add_row(
+            ["Source code", rule["id"], rule.get("metadata", {}).get("description")]
+        )
 
     metadata_rules = get_metadata_detectors(ecosystem)
     for ruleName in metadata_rules:
         rule = metadata_rules[ruleName]
         table.add_row(["Package metadata", rule.get_name(), rule.get_description()])
 
     print(table)
 
 
 @cli.group
 def npm(**kwargs):
-    """ Scan a npm package or verify a npm project
-    """
+    """Scan a npm package or verify a npm project"""
     pass
 
 
 @cli.group
 def pypi(**kwargs):
-    """ Scan a PyPI package or verify a PyPI project
-    """
+    """Scan a PyPI package or verify a PyPI project"""
     pass
 
 
 @npm.command("scan")
 @common_options
 @scan_options
 @npm_options
-def scan_npm(target, version, rules, exclude_rules, output_format, exit_non_zero_on_finding):
-    """ Scan a given npm package
-    """
-    return _scan(target, version, rules, exclude_rules, output_format, exit_non_zero_on_finding, ECOSYSTEM.NPM)
+def scan_npm(
+    target, version, rules, exclude_rules, output_format, exit_non_zero_on_finding
+):
+    """Scan a given npm package"""
+    return _scan(
+        target,
+        version,
+        rules,
+        exclude_rules,
+        output_format,
+        exit_non_zero_on_finding,
+        ECOSYSTEM.NPM,
+    )
 
 
 @npm.command("verify")
 @common_options
 @verify_options
 @npm_options
 def verify_npm(target, rules, exclude_rules, output_format, exit_non_zero_on_finding):
-    """ Verify a given npm project
-    """
-    return _verify(target, rules, exclude_rules, output_format, exit_non_zero_on_finding, ECOSYSTEM.NPM)
+    """Verify a given npm project"""
+    return _verify(
+        target,
+        rules,
+        exclude_rules,
+        output_format,
+        exit_non_zero_on_finding,
+        ECOSYSTEM.NPM,
+    )
 
 
 @pypi.command("scan")
 @common_options
 @scan_options
 @pypi_options
-def scan_pypi(target, version, rules, exclude_rules, output_format, exit_non_zero_on_finding):
-    """ Scan a given PyPI package
-    """
-    return _scan(target, version, rules, exclude_rules, output_format, exit_non_zero_on_finding, ECOSYSTEM.PYPI)
+def scan_pypi(
+    target, version, rules, exclude_rules, output_format, exit_non_zero_on_finding
+):
+    """Scan a given PyPI package"""
+    return _scan(
+        target,
+        version,
+        rules,
+        exclude_rules,
+        output_format,
+        exit_non_zero_on_finding,
+        ECOSYSTEM.PYPI,
+    )
 
 
 @pypi.command("verify")
 @common_options
 @verify_options
 @pypi_options
 def verify_pypi(target, rules, exclude_rules, output_format, exit_non_zero_on_finding):
-    """ Verify a given Pypi project
-    """
-    return _verify(target, rules, exclude_rules, output_format, exit_non_zero_on_finding, ECOSYSTEM.PYPI)
+    """Verify a given Pypi project"""
+    return _verify(
+        target,
+        rules,
+        exclude_rules,
+        output_format,
+        exit_non_zero_on_finding,
+        ECOSYSTEM.PYPI,
+    )
 
 
 @pypi.command("list-rules")
 def list_rules_pypi():
-    """ Print available rules for PyPI
-    """
+    """Print available rules for PyPI"""
     return _list_rules(ECOSYSTEM.PYPI)
 
 
 @npm.command("list-rules")
 def list_rules_npm():
-    """ Print available rules for npm
-    """
+    """Print available rules for npm"""
     return _list_rules(ECOSYSTEM.NPM)
 
 
 @cli.command("verify", deprecated=True)
 @common_options
 @verify_options
 @legacy_rules_options
 def verify(target, rules, exclude_rules, output_format, exit_non_zero_on_finding):
-    return _verify(target, rules, exclude_rules, output_format, exit_non_zero_on_finding, ECOSYSTEM.PYPI)
+    return _verify(
+        target,
+        rules,
+        exclude_rules,
+        output_format,
+        exit_non_zero_on_finding,
+        ECOSYSTEM.PYPI,
+    )
 
 
 @cli.command("scan", deprecated=True)
 @common_options
 @scan_options
 @legacy_rules_options
-def scan(target, version, rules, exclude_rules, output_format, exit_non_zero_on_finding):
-    return _scan(target, version, rules, exclude_rules, output_format, exit_non_zero_on_finding, ECOSYSTEM.PYPI)
+def scan(
+    target, version, rules, exclude_rules, output_format, exit_non_zero_on_finding
+):
+    return _scan(
+        target,
+        version,
+        rules,
+        exclude_rules,
+        output_format,
+        exit_non_zero_on_finding,
+        ECOSYSTEM.PYPI,
+    )
 
 
 # Pretty prints scan results for the console
 def print_scan_results(results, identifier):
-    num_issues = results.get('issues')
-    errors = results.get('errors', [])
+    num_issues = results.get("issues")
+    errors = results.get("errors", [])
 
     if num_issues == 0:
-        print("Found " + colored('0 potentially malicious indicators', 'green',
-                                 attrs=['bold']) + " scanning " + colored(identifier, None, attrs=['bold']))
+        print(
+            "Found "
+            + colored("0 potentially malicious indicators", "green", attrs=["bold"])
+            + " scanning "
+            + colored(identifier, None, attrs=["bold"])
+        )
         print()
     else:
-        print("Found " + colored(str(num_issues) + ' potentially malicious indicators', 'red',
-                                 attrs=['bold']) + " in " + colored(identifier, None, attrs=['bold']))
+        print(
+            "Found "
+            + colored(
+                str(num_issues) + " potentially malicious indicators",
+                "red",
+                attrs=["bold"],
+            )
+            + " in "
+            + colored(identifier, None, attrs=["bold"])
+        )
         print()
 
-        findings = results.get('results', [])
+        findings = results.get("results", [])
         for finding in findings:
             description = findings[finding]
             if isinstance(description, str):  # package metadata
-                print(colored(finding, None, attrs=['bold']) + ': ' + description)
+                print(colored(finding, None, attrs=["bold"]) + ": " + description)
                 print()
             elif isinstance(description, list):  # semgrep rule result:
                 source_code_findings = description
-                print(colored(finding, None,
-                              attrs=['bold']) + ': found ' + str(len(source_code_findings)) + ' source code matches')
+                print(
+                    colored(finding, None, attrs=["bold"])
+                    + ": found "
+                    + str(len(source_code_findings))
+                    + " source code matches"
+                )
                 for finding in source_code_findings:
-                    print('  * ' + finding['message']
-                          + ' at ' + finding['location'] + '\n    ' + format_code_line_for_output(finding['code']))
+                    print(
+                        "  * "
+                        + finding["message"]
+                        + " at "
+                        + finding["location"]
+                        + "\n    "
+                        + format_code_line_for_output(finding["code"])
+                    )
                 print()
 
     if len(errors) > 0:
         print_errors(errors, identifier)
-        print('\n')
+        print("\n")
 
 
 def print_errors(errors, identifier):
-    print(colored("Some rules failed to run while scanning " + identifier + ":", "yellow"))
+    print(
+        colored("Some rules failed to run while scanning " + identifier + ":", "yellow")
+    )
     print()
     for rule in errors:
-        print(f'* {rule}: {errors[rule]}')
+        print(f"* {rule}: {errors[rule]}")
     print()
 
 
 def format_code_line_for_output(code):
-    return '    ' + colored(code.strip().replace('\n', '\n    ').replace('\t', '  '), None, 'on_red', attrs=['bold'])
+    return "    " + colored(
+        code.strip().replace("\n", "\n    ").replace("\t", "  "),
+        None,
+        "on_red",
+        attrs=["bold"],
+    )
 
 
 # Given the results, exit with the appropriate status code
 def exit_with_status_code(results):
     for result in results:
-        num_issues = result.get('issues', 0)
+        num_issues = result.get("issues", 0)
         if num_issues > 0:
             exit(EXIT_CODE_ISSUES_FOUND)
```

### Comparing `guarddog-1.8.0/guarddog/reporters/sarif.py` & `guarddog-1.8.1/guarddog/reporters/sarif.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/scanners/__init__.py` & `guarddog-1.8.1/guarddog/scanners/__init__.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/scanners/npm_package_scanner.py` & `guarddog-1.8.1/guarddog/scanners/npm_package_scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/scanners/npm_project_scanner.py` & `guarddog-1.8.1/guarddog/scanners/npm_project_scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/scanners/pypi_package_scanner.py` & `guarddog-1.8.1/guarddog/scanners/pypi_package_scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/scanners/pypi_project_scanner.py` & `guarddog-1.8.1/guarddog/scanners/pypi_project_scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/scanners/scanner.py` & `guarddog-1.8.1/guarddog/scanners/scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/utils/archives.py` & `guarddog-1.8.1/guarddog/utils/archives.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/guarddog/utils/package_info.py` & `guarddog-1.8.1/guarddog/utils/package_info.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.0/pyproject.toml` & `guarddog-1.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "guarddog"
 description = "GuardDog is a CLI tool to Identify malicious PyPI packages"
 authors = ["Ellen Wang", "Christophe Tafani-Dereeper"]
 license = "Apache-2.0"
 readme = "pypi.rst"
 repository = "https://github.com/DataDog/guarddog"
-version = "v1.8.0"
+version = "v1.8.1"
 
 [tool.poetry.scripts]
 guarddog = "guarddog.cli:cli"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4"
 semgrep = "1.67.0"
```

### Comparing `guarddog-1.8.0/PKG-INFO` & `guarddog-1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guarddog
-Version: 1.8.0
+Version: 1.8.1
 Summary: GuardDog is a CLI tool to Identify malicious PyPI packages
 Home-page: https://github.com/DataDog/guarddog
 License: Apache-2.0
 Author: Ellen Wang
 Requires-Python: >=3.10,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

