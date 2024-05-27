# Comparing `tmp/guarddog-1.8.1.tar.gz` & `tmp/guarddog-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guarddog-1.8.1.tar", max compression
+gzip compressed data, was "guarddog-1.8.2.tar", max compression
```

## Comparing `guarddog-1.8.1.tar` & `guarddog-1.8.2.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0    11377 2024-05-27 09:24:22.022132 guarddog-1.8.1/LICENSE
--rw-r--r--   0        0        0      314 2024-05-27 09:24:22.022132 guarddog-1.8.1/LICENSE-3rdparty.csv
--rw-r--r--   0        0        0      140 2024-05-27 09:24:22.022132 guarddog-1.8.1/NOTICE
--rw-r--r--   0        0        0      154 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/__init__.py
--rw-r--r--   0        0        0      246 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/__main__.py
--rw-r--r--   0        0        0        0 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/__init__.py
--rw-r--r--   0        0        0     9808 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/analyzer.py
--rw-r--r--   0        0        0      457 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/__init__.py
--rw-r--r--   0        0        0     1840 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/bundled_binary.py
--rw-r--r--   0        0        0      609 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/detector.py
--rw-r--r--   0        0        0     1166 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/empty_information.py
--rw-r--r--   0        0        0     1223 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/npm/__init__.py
--rw-r--r--   0        0        0      360 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/npm/bundled_binary.py
--rw-r--r--   0        0        0     2449 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/npm/direct_url_dependency.py
--rw-r--r--   0        0        0      793 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/npm/empty_information.py
--rw-r--r--   0        0        0     4428 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/npm/npm_metadata_mismatch.py
--rw-r--r--   0        0        0     1643 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/npm/potentially_compromised_email_domain.py
--rw-r--r--   0        0        0      578 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/npm/release_zero.py
--rw-r--r--   0        0        0     1732 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/npm/typosquatting.py
--rw-r--r--   0        0        0      899 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/npm/unclaimed_maintainer_email_domain.py
--rw-r--r--   0        0        0      461 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/npm/utils.py
--rw-r--r--   0        0        0     2806 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/potentially_compromised_email_domain.py
--rw-r--r--   0        0        0     1251 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/pypi/__init__.py
--rw-r--r--   0        0        0      361 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/pypi/bundled_binary.py
--rw-r--r--   0        0        0      723 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/pypi/empty_information.py
--rw-r--r--   0        0        0     1679 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/pypi/potentially_compromised_email_domain.py
--rw-r--r--   0        0        0      716 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/pypi/release_zero.py
--rw-r--r--   0        0        0    11635 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/pypi/repository_integrity_mismatch.py
--rw-r--r--   0        0        0     1369 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/pypi/single_python_file.py
--rw-r--r--   0        0        0     3490 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/pypi/typosquatting.py
--rw-r--r--   0        0        0      406 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/pypi/unclaimed_maintainer_email_domain.py
--rw-r--r--   0        0        0      199 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/pypi/utils.py
--rw-r--r--   0        0        0      438 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/release_zero.py
--rw-r--r--   0        0        0      743 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/repository_integrity_mismatch.py
--rw-r--r--   0        0        0   373303 2024-05-27 09:24:22.026133 guarddog-1.8.1/guarddog/analyzer/metadata/resources/top_npm_packages.json
--rw-r--r--   0        0        0   387251 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/metadata/resources/top_pypi_packages.json
--rw-r--r--   0        0        0     5619 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/metadata/typosquatting.py
--rw-r--r--   0        0        0     2343 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/metadata/unclaimed_maintainer_email_domain.py
--rw-r--r--   0        0        0     1603 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/metadata/utils.py
--rw-r--r--   0        0        0     1043 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/__init__.py
--rw-r--r--   0        0        0      524 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/clipboard-access.yml
--rw-r--r--   0        0        0      682 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/cmd-overwrite.yml
--rw-r--r--   0        0        0     4655 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/code-execution.yml
--rw-r--r--   0        0        0     3055 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/download-executable.yml
--rw-r--r--   0        0        0     2371 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/exec-base64.yml
--rw-r--r--   0        0        0     1815 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/exfiltrate-sensitive-data.yml
--rw-r--r--   0        0        0      576 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/npm-exec-base64.yml
--rw-r--r--   0        0        0     3011 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/npm-exfiltrate-sensitive-data.yml
--rw-r--r--   0        0        0     1067 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/npm-install-script.yml
--rw-r--r--   0        0        0     2160 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/npm-obfuscation.yml
--rw-r--r--   0        0        0      835 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/npm-serialize-environment.yml
--rw-r--r--   0        0        0     3513 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/npm-silent-process-execution.yml
--rw-r--r--   0        0        0      582 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/obfuscation.yml
--rw-r--r--   0        0        0     1609 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/shady-links.yml
--rw-r--r--   0        0        0      418 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/silent-process-execution.yml
--rw-r--r--   0        0        0      606 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/analyzer/sourcecode/steganography.yml
--rw-r--r--   0        0        0    14557 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/cli.py
--rw-r--r--   0        0        0      315 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/ecosystems.py
--rw-r--r--   0        0        0        0 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/reporters/__init__.py
--rw-r--r--   0        0        0     6189 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/reporters/sarif.py
--rw-r--r--   0        0        0      752 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/scanners/__init__.py
--rw-r--r--   0        0        0     1968 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/scanners/npm_package_scanner.py
--rw-r--r--   0        0        0     2243 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/scanners/npm_project_scanner.py
--rw-r--r--   0        0        0     2512 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/scanners/pypi_package_scanner.py
--rw-r--r--   0        0        0     5491 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/scanners/pypi_project_scanner.py
--rw-r--r--   0        0        0    11170 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/scanners/scanner.py
--rw-r--r--   0        0        0        0 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/utils/__init__.py
--rw-r--r--   0        0        0     1323 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/utils/archives.py
--rw-r--r--   0        0        0       54 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/utils/exceptions.py
--rw-r--r--   0        0        0      953 2024-05-27 09:24:22.030133 guarddog-1.8.1/guarddog/utils/package_info.py
--rw-r--r--   0        0        0       52 2024-05-27 09:24:22.034133 guarddog-1.8.1/pypi.rst
--rw-r--r--   0        0        0     1222 2024-05-27 09:24:36.698221 guarddog-1.8.1/pyproject.toml
--rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 guarddog-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0    11377 2024-05-27 10:52:24.428198 guarddog-1.8.2/LICENSE
+-rw-r--r--   0        0        0      314 2024-05-27 10:52:24.428198 guarddog-1.8.2/LICENSE-3rdparty.csv
+-rw-r--r--   0        0        0      140 2024-05-27 10:52:24.428198 guarddog-1.8.2/NOTICE
+-rw-r--r--   0        0        0      154 2024-05-27 10:52:24.432198 guarddog-1.8.2/guarddog/__init__.py
+-rw-r--r--   0        0        0      246 2024-05-27 10:52:24.432198 guarddog-1.8.2/guarddog/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-27 10:52:24.432198 guarddog-1.8.2/guarddog/analyzer/__init__.py
+-rw-r--r--   0        0        0     9808 2024-05-27 10:52:24.432198 guarddog-1.8.2/guarddog/analyzer/analyzer.py
+-rw-r--r--   0        0        0      457 2024-05-27 10:52:24.432198 guarddog-1.8.2/guarddog/analyzer/metadata/__init__.py
+-rw-r--r--   0        0        0     1840 2024-05-27 10:52:24.432198 guarddog-1.8.2/guarddog/analyzer/metadata/bundled_binary.py
+-rw-r--r--   0        0        0      609 2024-05-27 10:52:24.432198 guarddog-1.8.2/guarddog/analyzer/metadata/detector.py
+-rw-r--r--   0        0        0     1166 2024-05-27 10:52:24.432198 guarddog-1.8.2/guarddog/analyzer/metadata/empty_information.py
+-rw-r--r--   0        0        0     1223 2024-05-27 10:52:24.432198 guarddog-1.8.2/guarddog/analyzer/metadata/npm/__init__.py
+-rw-r--r--   0        0        0      360 2024-05-27 10:52:24.432198 guarddog-1.8.2/guarddog/analyzer/metadata/npm/bundled_binary.py
+-rw-r--r--   0        0        0     2449 2024-05-27 10:52:24.432198 guarddog-1.8.2/guarddog/analyzer/metadata/npm/direct_url_dependency.py
+-rw-r--r--   0        0        0      793 2024-05-27 10:52:24.432198 guarddog-1.8.2/guarddog/analyzer/metadata/npm/empty_information.py
+-rw-r--r--   0        0        0     4428 2024-05-27 10:52:24.432198 guarddog-1.8.2/guarddog/analyzer/metadata/npm/npm_metadata_mismatch.py
+-rw-r--r--   0        0        0     1643 2024-05-27 10:52:24.432198 guarddog-1.8.2/guarddog/analyzer/metadata/npm/potentially_compromised_email_domain.py
+-rw-r--r--   0        0        0      578 2024-05-27 10:52:24.432198 guarddog-1.8.2/guarddog/analyzer/metadata/npm/release_zero.py
+-rw-r--r--   0        0        0     1732 2024-05-27 10:52:24.432198 guarddog-1.8.2/guarddog/analyzer/metadata/npm/typosquatting.py
+-rw-r--r--   0        0        0      899 2024-05-27 10:52:24.432198 guarddog-1.8.2/guarddog/analyzer/metadata/npm/unclaimed_maintainer_email_domain.py
+-rw-r--r--   0        0        0      461 2024-05-27 10:52:24.432198 guarddog-1.8.2/guarddog/analyzer/metadata/npm/utils.py
+-rw-r--r--   0        0        0     2806 2024-05-27 10:52:24.432198 guarddog-1.8.2/guarddog/analyzer/metadata/potentially_compromised_email_domain.py
+-rw-r--r--   0        0        0     1251 2024-05-27 10:52:24.432198 guarddog-1.8.2/guarddog/analyzer/metadata/pypi/__init__.py
+-rw-r--r--   0        0        0      361 2024-05-27 10:52:24.432198 guarddog-1.8.2/guarddog/analyzer/metadata/pypi/bundled_binary.py
+-rw-r--r--   0        0        0      723 2024-05-27 10:52:24.432198 guarddog-1.8.2/guarddog/analyzer/metadata/pypi/empty_information.py
+-rw-r--r--   0        0        0     1679 2024-05-27 10:52:24.432198 guarddog-1.8.2/guarddog/analyzer/metadata/pypi/potentially_compromised_email_domain.py
+-rw-r--r--   0        0        0      716 2024-05-27 10:52:24.432198 guarddog-1.8.2/guarddog/analyzer/metadata/pypi/release_zero.py
+-rw-r--r--   0        0        0    11635 2024-05-27 10:52:24.432198 guarddog-1.8.2/guarddog/analyzer/metadata/pypi/repository_integrity_mismatch.py
+-rw-r--r--   0        0        0     1369 2024-05-27 10:52:24.432198 guarddog-1.8.2/guarddog/analyzer/metadata/pypi/single_python_file.py
+-rw-r--r--   0        0        0     3490 2024-05-27 10:52:24.432198 guarddog-1.8.2/guarddog/analyzer/metadata/pypi/typosquatting.py
+-rw-r--r--   0        0        0      406 2024-05-27 10:52:24.432198 guarddog-1.8.2/guarddog/analyzer/metadata/pypi/unclaimed_maintainer_email_domain.py
+-rw-r--r--   0        0        0      199 2024-05-27 10:52:24.432198 guarddog-1.8.2/guarddog/analyzer/metadata/pypi/utils.py
+-rw-r--r--   0        0        0      438 2024-05-27 10:52:24.432198 guarddog-1.8.2/guarddog/analyzer/metadata/release_zero.py
+-rw-r--r--   0        0        0      743 2024-05-27 10:52:24.432198 guarddog-1.8.2/guarddog/analyzer/metadata/repository_integrity_mismatch.py
+-rw-r--r--   0        0        0   373303 2024-05-27 10:52:24.436198 guarddog-1.8.2/guarddog/analyzer/metadata/resources/top_npm_packages.json
+-rw-r--r--   0        0        0   387251 2024-05-27 10:52:24.436198 guarddog-1.8.2/guarddog/analyzer/metadata/resources/top_pypi_packages.json
+-rw-r--r--   0        0        0     5619 2024-05-27 10:52:24.436198 guarddog-1.8.2/guarddog/analyzer/metadata/typosquatting.py
+-rw-r--r--   0        0        0     2343 2024-05-27 10:52:24.436198 guarddog-1.8.2/guarddog/analyzer/metadata/unclaimed_maintainer_email_domain.py
+-rw-r--r--   0        0        0     1603 2024-05-27 10:52:24.436198 guarddog-1.8.2/guarddog/analyzer/metadata/utils.py
+-rw-r--r--   0        0        0     1043 2024-05-27 10:52:24.436198 guarddog-1.8.2/guarddog/analyzer/sourcecode/__init__.py
+-rw-r--r--   0        0        0      524 2024-05-27 10:52:24.436198 guarddog-1.8.2/guarddog/analyzer/sourcecode/clipboard-access.yml
+-rw-r--r--   0        0        0      682 2024-05-27 10:52:24.436198 guarddog-1.8.2/guarddog/analyzer/sourcecode/cmd-overwrite.yml
+-rw-r--r--   0        0        0     4655 2024-05-27 10:52:24.436198 guarddog-1.8.2/guarddog/analyzer/sourcecode/code-execution.yml
+-rw-r--r--   0        0        0     3055 2024-05-27 10:52:24.436198 guarddog-1.8.2/guarddog/analyzer/sourcecode/download-executable.yml
+-rw-r--r--   0        0        0     2371 2024-05-27 10:52:24.436198 guarddog-1.8.2/guarddog/analyzer/sourcecode/exec-base64.yml
+-rw-r--r--   0        0        0     1815 2024-05-27 10:52:24.436198 guarddog-1.8.2/guarddog/analyzer/sourcecode/exfiltrate-sensitive-data.yml
+-rw-r--r--   0        0        0      576 2024-05-27 10:52:24.436198 guarddog-1.8.2/guarddog/analyzer/sourcecode/npm-exec-base64.yml
+-rw-r--r--   0        0        0     3011 2024-05-27 10:52:24.436198 guarddog-1.8.2/guarddog/analyzer/sourcecode/npm-exfiltrate-sensitive-data.yml
+-rw-r--r--   0        0        0     1067 2024-05-27 10:52:24.436198 guarddog-1.8.2/guarddog/analyzer/sourcecode/npm-install-script.yml
+-rw-r--r--   0        0        0     2160 2024-05-27 10:52:24.436198 guarddog-1.8.2/guarddog/analyzer/sourcecode/npm-obfuscation.yml
+-rw-r--r--   0        0        0      835 2024-05-27 10:52:24.436198 guarddog-1.8.2/guarddog/analyzer/sourcecode/npm-serialize-environment.yml
+-rw-r--r--   0        0        0     3513 2024-05-27 10:52:24.436198 guarddog-1.8.2/guarddog/analyzer/sourcecode/npm-silent-process-execution.yml
+-rw-r--r--   0        0        0      582 2024-05-27 10:52:24.436198 guarddog-1.8.2/guarddog/analyzer/sourcecode/obfuscation.yml
+-rw-r--r--   0        0        0     1609 2024-05-27 10:52:24.436198 guarddog-1.8.2/guarddog/analyzer/sourcecode/shady-links.yml
+-rw-r--r--   0        0        0      418 2024-05-27 10:52:24.440199 guarddog-1.8.2/guarddog/analyzer/sourcecode/silent-process-execution.yml
+-rw-r--r--   0        0        0      606 2024-05-27 10:52:24.440199 guarddog-1.8.2/guarddog/analyzer/sourcecode/steganography.yml
+-rw-r--r--   0        0        0    14557 2024-05-27 10:52:24.440199 guarddog-1.8.2/guarddog/cli.py
+-rw-r--r--   0        0        0      315 2024-05-27 10:52:24.440199 guarddog-1.8.2/guarddog/ecosystems.py
+-rw-r--r--   0        0        0        0 2024-05-27 10:52:24.440199 guarddog-1.8.2/guarddog/reporters/__init__.py
+-rw-r--r--   0        0        0     6231 2024-05-27 10:52:24.440199 guarddog-1.8.2/guarddog/reporters/sarif.py
+-rw-r--r--   0        0        0      752 2024-05-27 10:52:24.440199 guarddog-1.8.2/guarddog/scanners/__init__.py
+-rw-r--r--   0        0        0     1968 2024-05-27 10:52:24.440199 guarddog-1.8.2/guarddog/scanners/npm_package_scanner.py
+-rw-r--r--   0        0        0     2243 2024-05-27 10:52:24.440199 guarddog-1.8.2/guarddog/scanners/npm_project_scanner.py
+-rw-r--r--   0        0        0     2512 2024-05-27 10:52:24.440199 guarddog-1.8.2/guarddog/scanners/pypi_package_scanner.py
+-rw-r--r--   0        0        0     5491 2024-05-27 10:52:24.440199 guarddog-1.8.2/guarddog/scanners/pypi_project_scanner.py
+-rw-r--r--   0        0        0    11170 2024-05-27 10:52:24.440199 guarddog-1.8.2/guarddog/scanners/scanner.py
+-rw-r--r--   0        0        0        0 2024-05-27 10:52:24.440199 guarddog-1.8.2/guarddog/utils/__init__.py
+-rw-r--r--   0        0        0     1323 2024-05-27 10:52:24.440199 guarddog-1.8.2/guarddog/utils/archives.py
+-rw-r--r--   0        0        0       54 2024-05-27 10:52:24.440199 guarddog-1.8.2/guarddog/utils/exceptions.py
+-rw-r--r--   0        0        0      953 2024-05-27 10:52:24.440199 guarddog-1.8.2/guarddog/utils/package_info.py
+-rw-r--r--   0        0        0       52 2024-05-27 10:52:24.440199 guarddog-1.8.2/pypi.rst
+-rw-r--r--   0        0        0     1222 2024-05-27 10:52:35.992285 guarddog-1.8.2/pyproject.toml
+-rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 guarddog-1.8.2/PKG-INFO
```

### Comparing `guarddog-1.8.1/LICENSE` & `guarddog-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/analyzer.py` & `guarddog-1.8.2/guarddog/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/metadata/bundled_binary.py` & `guarddog-1.8.2/guarddog/analyzer/metadata/bundled_binary.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/metadata/detector.py` & `guarddog-1.8.2/guarddog/analyzer/metadata/detector.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/metadata/empty_information.py` & `guarddog-1.8.2/guarddog/analyzer/metadata/empty_information.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/metadata/npm/__init__.py` & `guarddog-1.8.2/guarddog/analyzer/metadata/npm/__init__.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/metadata/npm/direct_url_dependency.py` & `guarddog-1.8.2/guarddog/analyzer/metadata/npm/direct_url_dependency.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/metadata/npm/empty_information.py` & `guarddog-1.8.2/guarddog/analyzer/metadata/npm/empty_information.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/metadata/npm/npm_metadata_mismatch.py` & `guarddog-1.8.2/guarddog/analyzer/metadata/npm/npm_metadata_mismatch.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/metadata/npm/potentially_compromised_email_domain.py` & `guarddog-1.8.2/guarddog/analyzer/metadata/npm/potentially_compromised_email_domain.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/metadata/npm/release_zero.py` & `guarddog-1.8.2/guarddog/analyzer/metadata/npm/release_zero.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/metadata/npm/typosquatting.py` & `guarddog-1.8.2/guarddog/analyzer/metadata/npm/typosquatting.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/metadata/npm/unclaimed_maintainer_email_domain.py` & `guarddog-1.8.2/guarddog/analyzer/metadata/npm/unclaimed_maintainer_email_domain.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/metadata/potentially_compromised_email_domain.py` & `guarddog-1.8.2/guarddog/analyzer/metadata/potentially_compromised_email_domain.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/metadata/pypi/__init__.py` & `guarddog-1.8.2/guarddog/analyzer/metadata/pypi/__init__.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/metadata/pypi/empty_information.py` & `guarddog-1.8.2/guarddog/analyzer/metadata/pypi/empty_information.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/metadata/pypi/potentially_compromised_email_domain.py` & `guarddog-1.8.2/guarddog/analyzer/metadata/pypi/potentially_compromised_email_domain.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/metadata/pypi/release_zero.py` & `guarddog-1.8.2/guarddog/analyzer/metadata/pypi/release_zero.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/metadata/pypi/repository_integrity_mismatch.py` & `guarddog-1.8.2/guarddog/analyzer/metadata/pypi/repository_integrity_mismatch.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/metadata/pypi/single_python_file.py` & `guarddog-1.8.2/guarddog/analyzer/metadata/pypi/single_python_file.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/metadata/pypi/typosquatting.py` & `guarddog-1.8.2/guarddog/analyzer/metadata/pypi/typosquatting.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/metadata/repository_integrity_mismatch.py` & `guarddog-1.8.2/guarddog/analyzer/metadata/repository_integrity_mismatch.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/metadata/resources/top_npm_packages.json` & `guarddog-1.8.2/guarddog/analyzer/metadata/resources/top_npm_packages.json`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/metadata/resources/top_pypi_packages.json` & `guarddog-1.8.2/guarddog/analyzer/metadata/resources/top_pypi_packages.json`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/metadata/typosquatting.py` & `guarddog-1.8.2/guarddog/analyzer/metadata/typosquatting.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/metadata/unclaimed_maintainer_email_domain.py` & `guarddog-1.8.2/guarddog/analyzer/metadata/unclaimed_maintainer_email_domain.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/metadata/utils.py` & `guarddog-1.8.2/guarddog/analyzer/metadata/utils.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/sourcecode/__init__.py` & `guarddog-1.8.2/guarddog/analyzer/sourcecode/__init__.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/sourcecode/clipboard-access.yml` & `guarddog-1.8.2/guarddog/analyzer/sourcecode/clipboard-access.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/sourcecode/cmd-overwrite.yml` & `guarddog-1.8.2/guarddog/analyzer/sourcecode/cmd-overwrite.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/sourcecode/code-execution.yml` & `guarddog-1.8.2/guarddog/analyzer/sourcecode/code-execution.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/sourcecode/download-executable.yml` & `guarddog-1.8.2/guarddog/analyzer/sourcecode/download-executable.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/sourcecode/exec-base64.yml` & `guarddog-1.8.2/guarddog/analyzer/sourcecode/exec-base64.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/sourcecode/exfiltrate-sensitive-data.yml` & `guarddog-1.8.2/guarddog/analyzer/sourcecode/exfiltrate-sensitive-data.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/sourcecode/npm-exec-base64.yml` & `guarddog-1.8.2/guarddog/analyzer/sourcecode/npm-exec-base64.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/sourcecode/npm-exfiltrate-sensitive-data.yml` & `guarddog-1.8.2/guarddog/analyzer/sourcecode/npm-exfiltrate-sensitive-data.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/sourcecode/npm-install-script.yml` & `guarddog-1.8.2/guarddog/analyzer/sourcecode/npm-install-script.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/sourcecode/npm-obfuscation.yml` & `guarddog-1.8.2/guarddog/analyzer/sourcecode/npm-obfuscation.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/sourcecode/npm-serialize-environment.yml` & `guarddog-1.8.2/guarddog/analyzer/sourcecode/npm-serialize-environment.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/sourcecode/npm-silent-process-execution.yml` & `guarddog-1.8.2/guarddog/analyzer/sourcecode/npm-silent-process-execution.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/sourcecode/obfuscation.yml` & `guarddog-1.8.2/guarddog/analyzer/sourcecode/obfuscation.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/sourcecode/shady-links.yml` & `guarddog-1.8.2/guarddog/analyzer/sourcecode/shady-links.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/analyzer/sourcecode/steganography.yml` & `guarddog-1.8.2/guarddog/analyzer/sourcecode/steganography.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/cli.py` & `guarddog-1.8.2/guarddog/cli.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/reporters/sarif.py` & `guarddog-1.8.2/guarddog/reporters/sarif.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
         uri = package_path[2:] if package_path.startswith('./') else package_path
         physical_location = get_physical_location(uri, region)
         location = get_location(physical_location)
         scan_result_details = entry["result"]["results"]
         package = entry["dependency"]
         version = entry["version"]
         for rule_name in scan_result_details.keys():
-            if len(scan_result_details[rule_name]) == 0:
+            if scan_result_details[rule_name] is None or len(scan_result_details[rule_name]) == 0:
                 continue
             text = f"On package: {package} version: {version}\n" + "\n".join(map(
                 lambda x: x["message"],
                 scan_result_details[rule_name]
             )) if isinstance(scan_result_details[rule_name], list) else scan_result_details[rule_name]
             key = f"{rule_name}-{text}"
             partial_fingerprints = {
```

### Comparing `guarddog-1.8.1/guarddog/scanners/__init__.py` & `guarddog-1.8.2/guarddog/scanners/__init__.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/scanners/npm_package_scanner.py` & `guarddog-1.8.2/guarddog/scanners/npm_package_scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/scanners/npm_project_scanner.py` & `guarddog-1.8.2/guarddog/scanners/npm_project_scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/scanners/pypi_package_scanner.py` & `guarddog-1.8.2/guarddog/scanners/pypi_package_scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/scanners/pypi_project_scanner.py` & `guarddog-1.8.2/guarddog/scanners/pypi_project_scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/scanners/scanner.py` & `guarddog-1.8.2/guarddog/scanners/scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/utils/archives.py` & `guarddog-1.8.2/guarddog/utils/archives.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/guarddog/utils/package_info.py` & `guarddog-1.8.2/guarddog/utils/package_info.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.8.1/pyproject.toml` & `guarddog-1.8.2/pyproject.toml`

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
-version = "v1.8.1"
+version = "v1.8.2"
 
 [tool.poetry.scripts]
 guarddog = "guarddog.cli:cli"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4"
 semgrep = "1.67.0"
```

### Comparing `guarddog-1.8.1/PKG-INFO` & `guarddog-1.8.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guarddog
-Version: 1.8.1
+Version: 1.8.2
 Summary: GuardDog is a CLI tool to Identify malicious PyPI packages
 Home-page: https://github.com/DataDog/guarddog
 License: Apache-2.0
 Author: Ellen Wang
 Requires-Python: >=3.10,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

