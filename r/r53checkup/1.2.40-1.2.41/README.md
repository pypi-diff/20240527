# Comparing `tmp/r53checkup-1.2.40.tar.gz` & `tmp/r53checkup-1.2.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r53checkup-1.2.40.tar", last modified: Wed Nov 15 15:28:37 2023, max compression
+gzip compressed data, was "r53checkup-1.2.41.tar", last modified: Mon May 27 10:49:16 2024, max compression
```

## Comparing `r53checkup-1.2.40.tar` & `r53checkup-1.2.41.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mmajeed    (502) staff       (20)        0 2023-11-15 15:28:37.355415 r53checkup-1.2.40/
--rw-r--r--   0 mmajeed    (502) staff       (20)     1065 2023-11-12 16:00:09.000000 r53checkup-1.2.40/LICENSE
--rw-r--r--   0 mmajeed    (502) staff       (20)      880 2023-11-15 15:28:37.355302 r53checkup-1.2.40/PKG-INFO
--rw-r--r--   0 mmajeed    (502) staff       (20)     4498 2023-11-15 15:17:12.000000 r53checkup-1.2.40/README.md
-drwxr-xr-x   0 mmajeed    (502) staff       (20)        0 2023-11-15 15:28:37.354397 r53checkup-1.2.40/r53checkup.egg-info/
--rw-r--r--   0 mmajeed    (502) staff       (20)      880 2023-11-15 15:28:37.000000 r53checkup-1.2.40/r53checkup.egg-info/PKG-INFO
--rw-r--r--   0 mmajeed    (502) staff       (20)      274 2023-11-15 15:28:37.000000 r53checkup-1.2.40/r53checkup.egg-info/SOURCES.txt
--rw-r--r--   0 mmajeed    (502) staff       (20)        1 2023-11-15 15:28:37.000000 r53checkup-1.2.40/r53checkup.egg-info/dependency_links.txt
--rw-r--r--   0 mmajeed    (502) staff       (20)       56 2023-11-15 15:28:37.000000 r53checkup-1.2.40/r53checkup.egg-info/entry_points.txt
--rw-r--r--   0 mmajeed    (502) staff       (20)       69 2023-11-15 15:28:37.000000 r53checkup-1.2.40/r53checkup.egg-info/requires.txt
--rw-r--r--   0 mmajeed    (502) staff       (20)        8 2023-11-15 15:28:37.000000 r53checkup-1.2.40/r53checkup.egg-info/top_level.txt
-drwxr-xr-x   0 mmajeed    (502) staff       (20)        0 2023-11-15 15:28:37.354837 r53checkup-1.2.40/scripts/
--rw-r--r--   0 mmajeed    (502) staff       (20)       29 2023-11-15 14:48:22.000000 r53checkup-1.2.40/scripts/__init__.py
--rw-r--r--   0 mmajeed    (502) staff       (20)    32000 2023-11-15 15:17:12.000000 r53checkup-1.2.40/scripts/r53checkup.py
--rw-r--r--   0 mmajeed    (502) staff       (20)       38 2023-11-15 15:28:37.355470 r53checkup-1.2.40/setup.cfg
--rw-r--r--   0 mmajeed    (502) staff       (20)     1309 2023-11-15 15:28:14.000000 r53checkup-1.2.40/setup.py
+drwxr-xr-x   0 mmajeed    (502) staff       (20)        0 2024-05-27 10:49:16.973768 r53checkup-1.2.41/
+-rw-r--r--   0 mmajeed    (502) staff       (20)     1065 2024-05-27 10:45:20.000000 r53checkup-1.2.41/LICENSE
+-rw-r--r--   0 mmajeed    (502) staff       (20)      880 2024-05-27 10:49:16.973617 r53checkup-1.2.41/PKG-INFO
+-rw-r--r--   0 mmajeed    (502) staff       (20)     4574 2024-05-27 10:45:20.000000 r53checkup-1.2.41/README.md
+drwxr-xr-x   0 mmajeed    (502) staff       (20)        0 2024-05-27 10:49:16.972906 r53checkup-1.2.41/r53checkup.egg-info/
+-rw-r--r--   0 mmajeed    (502) staff       (20)      880 2024-05-27 10:49:16.000000 r53checkup-1.2.41/r53checkup.egg-info/PKG-INFO
+-rw-r--r--   0 mmajeed    (502) staff       (20)      274 2024-05-27 10:49:16.000000 r53checkup-1.2.41/r53checkup.egg-info/SOURCES.txt
+-rw-r--r--   0 mmajeed    (502) staff       (20)        1 2024-05-27 10:49:16.000000 r53checkup-1.2.41/r53checkup.egg-info/dependency_links.txt
+-rw-r--r--   0 mmajeed    (502) staff       (20)       56 2024-05-27 10:49:16.000000 r53checkup-1.2.41/r53checkup.egg-info/entry_points.txt
+-rw-r--r--   0 mmajeed    (502) staff       (20)       69 2024-05-27 10:49:16.000000 r53checkup-1.2.41/r53checkup.egg-info/requires.txt
+-rw-r--r--   0 mmajeed    (502) staff       (20)        8 2024-05-27 10:49:16.000000 r53checkup-1.2.41/r53checkup.egg-info/top_level.txt
+drwxr-xr-x   0 mmajeed    (502) staff       (20)        0 2024-05-27 10:49:16.973343 r53checkup-1.2.41/scripts/
+-rw-r--r--   0 mmajeed    (502) staff       (20)       29 2024-05-27 10:45:20.000000 r53checkup-1.2.41/scripts/__init__.py
+-rw-r--r--   0 mmajeed    (502) staff       (20)    32251 2024-05-27 10:46:05.000000 r53checkup-1.2.41/scripts/r53checkup.py
+-rw-r--r--   0 mmajeed    (502) staff       (20)       38 2024-05-27 10:49:16.973831 r53checkup-1.2.41/setup.cfg
+-rw-r--r--   0 mmajeed    (502) staff       (20)     1309 2024-05-27 10:49:11.000000 r53checkup-1.2.41/setup.py
```

### Comparing `r53checkup-1.2.40/LICENSE` & `r53checkup-1.2.41/LICENSE`

 * *Files identical despite different names*

### Comparing `r53checkup-1.2.40/PKG-INFO` & `r53checkup-1.2.41/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r53checkup
-Version: 1.2.40
+Version: 1.2.41
 Summary: Checkup all route53 records distributed across yours accounts in aws org.
 Home-page: UNKNOWN
 Author: maerifat (Maerifat Majeed)
 Author-email: <maerifat@gmail.com>
 License: UNKNOWN
 Keywords: python,route53,excel,sso,aws,aws org,subdomains,dangling,certificates
 Platform: UNKNOWN
```

### Comparing `r53checkup-1.2.40/README.md` & `r53checkup-1.2.41/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,36 @@
-# Route53 Record Collector ( r53checkup)
+# Route53 Record Analyzer ( r53checkup)
 
 ## Overview
 This Python tool collects DNS records from AWS Route53 across multiple accounts using AWS SSO (Single Sign-On). It provides various options for listing, filtering, storing and analyzing the data.
 
 
-![Screen Shot](images/usage.png)
+![Screen Shot](images/usage_new.png)
 
 
 ## Installation
 
 Use the package manager [pip3](https://pip.pypa.io/en/stable/) to install  r53checkup.
 
 ```bash
 pip3 install  r53checkup
 ```
 
 
 
-## Usage
+## Usage (using -o flag is recommended, to get results in excel format)
+
+```bash
+r53checkup -u https://d-1010ad440.awsapps.com/start
+```
+
+```bash 
+r53checkup -u https://d-1010ad440.awsapps.com/start -cd -o myrecords.xlsx
+```
 
-` r53checkup -u https://d-1010ad440.awsapps.com/start`
-` r53checkup -u https://d-1010ad440.awsapps.com/start -cd -o myrecords.xlsx  `
 ```bash
  r53checkup -u https://d-1010ad440.awsapps.com/start -a 144313609872,330936112098,692902471034 -t a,cname,aaaa -e "^_.*|.*_(domainkey|dkim).*" -cd -o myrecords.xlsx 
 ```
 
 
 ## Detailed Features
 
@@ -32,63 +38,63 @@
 ''
 ''
 
   ### Every time you run this tool it will open up your default browser to authorize the device. You don't need any credentials or profiles separately to make it work.
 
 - Run accross all accounts
   - With out using --accounts/-a, the tool will gather all accounts you have privilege to and fetch details of dns records. . Example:  
-    - _ r53checkup -u https://d-1010ad440.awsapps.com/start_
+    - _r53checkup -u https://d-1010ad440.awsapps.com/start_
   ```python
    r53checkup -u <SSO Start URL>
   
 - Run accross selective account[s].
   - To get results from selective accounts, use --accounts/-a. Multiple accounts can be selected separated by comma. Example:
-    - _ r53checkup -u https://d-1010ad440.awsapps.com/start -a 144313609872,330936112098,692902471034_
+    - _r53checkup -u https://d-1010ad440.awsapps.com/start -a 144313609872,330936112098,692902471034_
   ```python
    r53checkup -u <SSO Start URL> -a <Account IDs> 
 
 - Filter record types.
   - To get desired DNS record types only, use -types/-t. Multiple types can be selected separated by comma. Example:
-    - _ r53checkup -u https://d-1010ad440.awsapps.com/start -t cname,a,aaaa_
+    - _r53checkup -u https://d-1010ad440.awsapps.com/start -t cname,a,aaaa_
   ```python
    r53checkup -u <SSO Start URL> -t <Record Type> 
 
 - Exclude record names using regex.
   - If you want to filterout the undesired subdomains(record names) like containing '\_domainkey' or '\_dkim' or records starting with '\_', you can select regex after --exclude/-e. Example:
-    - _ r53checkup -u https://d-1010ad440.awsapps.com/start -e "^\_.\*|.\*\_(domainkey|dkim).\*"_
+    - _r53checkup -u https://d-1010ad440.awsapps.com/start -e "^\_.\*|.\*\_(domainkey|dkim).\*"_
   ```python
    r53checkup -u <SSO Start URL> -e <Regex> 
 
 - Save output to a file.
   - If you want to save the output to a file, use --output/-o. You have two format options xlsx(recommended) and txt. Format is recognised from the filename extension. Txt extension is recommended only in case you want to store subdomains in a text file, which can be later used to feed other tools for reconnaissance . Example:
-    - _ r53checkup -u https://d-1010ad440.awsapps.com/start -o myrecords.xlsx_
+    - _r53checkup -u https://d-1010ad440.awsapps.com/start -o myrecords.xlsx_
   ```python
    r53checkup -u <SSO Start URL> -o <Output FileLocation> 
 
 - check if the record is dangling.
   - If you want to check whether the DNS record is dangling or not, use --check-dangling/-cd . Use output filename extension as xlsx along with it. Example: 
-    - _ r53checkup -u https://d-1010ad440.awsapps.com/start -cd -o myrecords.xlsx_
+    - _r53checkup -u https://d-1010ad440.awsapps.com/start -cd -o myrecords.xlsx_
   ```python
    r53checkup -u <SSO Start URL> -cd -o <Output FileLocation> 
 
 - check if the certificates served are valid.
   - If you want to check whether the certificates served by dns record names are valid, use --check-cert/-cc. Use output filename extension as xlsx along with it. Apart from certificate host name validation, it will also save Cipher,CN,SAN,Issue_Date,Expiry_Date in output file. Example: 
-    - _ r53checkup -u https://d-1010ad440.awsapps.com/start -cd -cc -o myrecords.xlsx_
+    - _r53checkup -u https://d-1010ad440.awsapps.com/start -cd -cc -o myrecords.xlsx_
   ```python
    r53checkup -u <SSO Start URL> -cd -cc -o <Output FileLocation> 
 
 - Disable verbose.
   - If you want to disable the verbose, use --no-verbose/-nc . Example: 
-    - _ r53checkup -u https://d-1010ad440.awsapps.com/start -cd -o myrecords.xlsx -nc_
+    - _r53checkup -u https://d-1010ad440.awsapps.com/start -cd -o myrecords.xlsx -nc_
   ```python
    r53checkup -u <SSO Start URL> -cd -o <Output FileLocation> -nc 
 
 - List unique subdomains.
   - If you want to only list unique subdomains, use --list/-l . This is helpful while combining it with other tools using pipe. Example: 
-    - _ r53checkup -u https://d-1010ad440.awsapps.com/start -l_
+    - _r53checkup -u https://d-1010ad440.awsapps.com/start -l_
   ```python
    r53checkup -u <SSO Start URL>  -l 
 
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
```

### Comparing `r53checkup-1.2.40/r53checkup.egg-info/PKG-INFO` & `r53checkup-1.2.41/r53checkup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r53checkup
-Version: 1.2.40
+Version: 1.2.41
 Summary: Checkup all route53 records distributed across yours accounts in aws org.
 Home-page: UNKNOWN
 Author: maerifat (Maerifat Majeed)
 Author-email: <maerifat@gmail.com>
 License: UNKNOWN
 Keywords: python,route53,excel,sso,aws,aws org,subdomains,dangling,certificates
 Platform: UNKNOWN
```

### Comparing `r53checkup-1.2.40/scripts/r53checkup.py` & `r53checkup-1.2.41/scripts/r53checkup.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
     def assign_default_values():
         print()
 
 
 #Some important functions
     def is_accessible(hostname):
         global accessibility
-        if args.output or args.check_cert:
+        if args.output or args.check_cert or args.check_dangling:
             if ("acm-validations.aws" not in get_dns_value()) and ( record['Type']=='CNAME' or record['Type']=='A' or record['Type']=='AAAA'):
                 try:
                     ip_address = socket.gethostbyname(hostname)
                 
                     private_ranges = [
                         ('10.0.0.0', '10.255.255.255'),
                         ('172.16.0.0', '172.31.255.255'),
@@ -170,32 +170,32 @@
                     for start, end in private_ranges:
                         start_int = int.from_bytes(socket.inet_aton(start), byteorder='big')
                         end_int = int.from_bytes(socket.inet_aton(end), byteorder='big')
                         if start_int <= ip_int <= end_int:
                             print_event("Accessiblity :","blue","on_light_grey",attrs=['bold'],end='')
                             print_event(f" Private","yellow",None)
                             accessibility="Private"
-                            return "Private"
+                            return accessibility
                     print_event("Accessiblity :","blue","on_light_grey",attrs=['bold'],end='')
                     print_event(f" Public","yellow",None)
                     accessibility="Public"
-                    return "Public"
+                    return accessibility
                 except:
                     print_event("Accessiblity :","blue","on_light_grey",attrs=['bold'],end='')
                     print_event(f" Unreachable","yellow",None)
                     accessibility="Unreachable"
-                    return "Unreachable"
+                    return accessibility
             else:
                 print_event("Accessiblity :","blue","on_light_grey",attrs=['bold'],end='')
                 print_event(f" NA","yellow",None)
                 accessibility="NA"
-                return "NA"
+                return accessibility
         else:
             accessibility="NA"
-            return "NA"
+            return accessibility
 
 
     def check_cert(host, port=443):
         global cipher,cipher_name,san,cn,issue_date,expiry_date,validation
         if args.check_cert:
             if is_accessible(record['Name']) == "Public":
                 host = host.rstrip('.')
@@ -371,14 +371,15 @@
             dns_value="dnsvalueerror2"
         return dns_value
     
 
     def is_dangling(dns_value):
         global is_dangling_var
         if args.check_dangling:
+            is_accessible(dns_value)
             if record['Type'] == 'CNAME' or is_alias:
                 try:
                     result = dns.resolver.resolve(dns_value)
                     if result:
                         is_dangling_var= "No"
                         print_event("Is_Dangling :","blue","on_light_grey",attrs=['bold'],end='')
                         print_event(f" {is_dangling_var}","yellow",None)
@@ -481,31 +482,34 @@
                     #if record['Type']  in ['SOA', 'NS', 'MX', 'TXT'] and not record['Name'].startswith('_'):
                     if args.types and not args.exclude:
                         dns_types = list(map(str.upper, args.types))
                         if record['Type'] in dns_types:
                             get_dns_value()
                             assign_default_values()
                             print_event(f"{record['Type']} : {record['Name']} ==> {get_dns_value()}","magenta",on_color=None)
-                            is_dangling(dns_value)
-                            check_cert(record['Name'].rstrip('.'))
+                            if args.check_dangling:
+                                is_dangling(dns_value)
+                            if args.check_cert:
+                                check_cert(record['Name'].rstrip('.'))
                             if is_excel():
                                 append_row_to_sheet()
                             
                             
                             subdomains.append(record['Name'].rstrip('.'))
                             combined_subdomains.add(record['Name'].rstrip('.'))
                             
 
                     elif args.exclude and not args.types:
                         regex_pattern = args.exclude
                         if not re.match(regex_pattern, record['Name'].rstrip('.')):
                             assign_default_values()
                             get_dns_value()
                             print_event(f"{record['Type']} : {record['Name']} ==> {get_dns_value()}","magenta",on_color=None)
-                            is_dangling(dns_value)
+                            if args.check_dangling:
+                                is_dangling(dns_value)
                             check_cert(record['Name'].rstrip('.'))
                             if is_excel():
                                 append_row_to_sheet()
                             
                             
                             subdomains.append(record['Name'].rstrip('.'))
                             combined_subdomains.add(record['Name'].rstrip('.'))
```

### Comparing `r53checkup-1.2.40/setup.py` & `r53checkup-1.2.41/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = '1.2.40'
+VERSION = '1.2.41'
 DESCRIPTION = 'Checkup all route53 records distributed across yours accounts in aws org.'
 LONG_DESCRIPTION = 'This python tool collects DNS records from AWS Route53 across multiple accounts using AWS SSO (Single Sign-On) and provides various options for listing, filtering, storing and analyzing the data.'
 
 # Setting up
 setup(
     name="r53checkup",
     version=VERSION,
```

