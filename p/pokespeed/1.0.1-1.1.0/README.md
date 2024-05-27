# Comparing `tmp/pokespeed-1.0.1.tar.gz` & `tmp/pokespeed-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokespeed-1.0.1.tar", last modified: Sat Jan 20 02:58:09 2024, max compression
+gzip compressed data, was "pokespeed-1.1.0.tar", last modified: Mon May 27 19:44:55 2024, max compression
```

## Comparing `pokespeed-1.0.1.tar` & `pokespeed-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-01-20 02:58:09.021888 pokespeed-1.0.1/
--rw-rw-rw-   0        0        0    11558 2024-01-20 02:06:08.000000 pokespeed-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      126 2023-11-05 05:34:16.000000 pokespeed-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      368 2024-01-20 02:58:09.021888 pokespeed-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1919 2024-01-20 02:57:47.000000 pokespeed-1.0.1/README.md
--rw-rw-rw-   0        0        0    34849 2024-01-20 02:55:05.000000 pokespeed-1.0.1/outspeed_benchmarks.csv
-drwxrwxrwx   0        0        0        0 2024-01-20 02:58:09.018964 pokespeed-1.0.1/pokespeed/
--rw-rw-rw-   0        0        0   131671 2024-01-20 02:58:01.000000 pokespeed-1.0.1/pokespeed/__coconut__.py
--rw-rw-rw-   0        0        0    57019 2024-01-20 02:54:21.000000 pokespeed-1.0.1/pokespeed/__init__.py
--rw-rw-rw-   0        0        0     4836 2024-01-20 02:25:22.000000 pokespeed-1.0.1/pokespeed/__main__.py
-drwxrwxrwx   0        0        0        0 2024-01-20 02:58:09.020888 pokespeed-1.0.1/pokespeed.egg-info/
--rw-rw-rw-   0        0        0      141 2024-01-20 02:58:08.000000 pokespeed-1.0.1/pokespeed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       74 2024-01-20 02:58:09.022939 pokespeed-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      588 2024-01-20 02:57:57.000000 pokespeed-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 19:44:54.996782 pokespeed-1.1.0/
+-rw-rw-rw-   0        0        0    11558 2024-01-20 02:06:08.000000 pokespeed-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      126 2023-11-05 05:34:16.000000 pokespeed-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      368 2024-05-27 19:44:54.996782 pokespeed-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2135 2024-05-27 19:44:09.000000 pokespeed-1.1.0/README.md
+-rw-rw-rw-   0        0        0    34058 2024-05-27 19:39:37.000000 pokespeed-1.1.0/outspeed_benchmarks.csv
+drwxrwxrwx   0        0        0        0 2024-05-27 19:44:54.987782 pokespeed-1.1.0/pokespeed/
+-rw-rw-rw-   0        0        0   132337 2024-05-27 19:44:46.000000 pokespeed-1.1.0/pokespeed/__coconut__.py
+-rw-rw-rw-   0        0        0    59789 2024-05-27 19:39:19.000000 pokespeed-1.1.0/pokespeed/__init__.py
+-rw-rw-rw-   0        0        0     4973 2024-05-27 19:38:23.000000 pokespeed-1.1.0/pokespeed/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 19:44:54.993783 pokespeed-1.1.0/pokespeed-source/
+drwxrwxrwx   0        0        0        0 2024-05-27 19:44:54.994782 pokespeed-1.1.0/pokespeed-source/__coconut_cache__/
+-rw-rw-rw-   0        0        0   117367 2024-05-27 19:35:05.000000 pokespeed-1.1.0/pokespeed-source/__coconut_cache__/__main__.py
+-rw-rw-rw-   0        0        0    34058 2024-05-27 19:35:31.000000 pokespeed-1.1.0/pokespeed-source/outspeed_benchmarks.csv
+drwxrwxrwx   0        0        0        0 2024-05-27 19:44:54.995795 pokespeed-1.1.0/pokespeed.egg-info/
+-rw-rw-rw-   0        0        0      255 2024-05-27 19:44:54.000000 pokespeed-1.1.0/pokespeed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       74 2024-05-27 19:44:54.997782 pokespeed-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      588 2024-05-27 19:41:54.000000 pokespeed-1.1.0/setup.py
+-rw-rw-rw-   0        0        0    65608 2024-05-27 19:40:18.000000 pokespeed-1.1.0/underspeed_benchmarks.csv
```

### Comparing `pokespeed-1.0.1/LICENSE` & `pokespeed-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pokespeed-1.0.1/README.md` & `pokespeed-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,27 +8,29 @@
 ```
 
 To use, just run:
 ```
 pokespeed
 ```
 
-Or optionally supply the CSV location, Pikalytics URL (supplying a Pikalytics url like `https://www.pikalytics.com/pokedex/gen9vgc2023regulatione` will let you specify the format), or Pokemon level (defaults shown below):
+Or optionally supply the CSV location, `--underspeed` for underspeed benchmarks, Pikalytics URL (supplying a Pikalytics url like `https://www.pikalytics.com/pokedex/gen9vgc2023regulatione` will let you specify the format), or Pokemon level (defaults shown below):
 ```
 pokespeed --out ./outspeed_benchmarks.csv --url https://ww.pikalytics.com --level 50
 ```
 
 Then, view the resulting CSV file in your favorite spreadsheet viewer (e.g. Google Sheets) to see the generated output. Interpreting the output is relatively straightforward:
 * Each row corresponds to a speed.
 * Each column corresponds to a stat stage:
   * `-1` is a negative stat change (e.g. icy wind).
   * `+0` is no stat change.
   * `-1 x2` is a negative stat change (e.g. icy wind) multiplied by 2 (e.g. tailwind).
   * `+1` is a positive stat change (e.g. dragon dance, choice scarf, speed booster energy).
   * `+2` is two positive stat changes (e.g. tailwind).
   * `+1 x2` is a positive stat change (e.g. choice scarf) multiplied by 2 (e.g. tailwind).
-* Each cell corresponds to the Pokemon you **outspeed** if you have that row's speed and you are under the effects of that column's speed modifier. (So the speed in the row isn't the speed that each of the listed Pokemon hit; it's the speed you need to outspeed them.)
+* Each cell corresponds to the Pokemon you **outspeed** (or underspeed if you passed `--underspeed`) if you have that row's speed and you are under the effects of that column's speed modifier. (So the speed in the row isn't the speed that each of the listed Pokemon hit; it's the speed you need to outspeed them.)
   * `pokemon+` means `252+` in speed (e.g. timid or jolly).
   * `pokemon=` means `252` in speed (e.g. modest or adamant).
+  * `pokemon0` means `0` in speed (`0` evs, `31` ivs).
+  * `pokemon-` means `0-` in speed (negative nature, `0` evs, `0` ivs).
   * `+1 pokemon+` means `252+` in speed with a stat modifier of `+1` (these modifiers are exactly as in the columns).
 
 For an example of what this tool's output looks like, see [here](https://docs.google.com/spreadsheets/d/11ml2mJ-k86F5jxlj2Ziav7uw73nNfJkA_19DEM1uDFM/edit?usp=sharing).
```

### Comparing `pokespeed-1.0.1/outspeed_benchmarks.csv` & `pokespeed-1.1.0/outspeed_benchmarks.csv`

 * *Files 18% similar despite different names*

```diff
@@ -1,335 +1,363 @@
 Speed: \ Stage:,-1,+0,-1 x2,+1,+2,+1 x2
 923,"+1 x2 flutter-mane+, +1 x2 chien-pao+",,,,,
-842,"+1 x2 chien-pao=, +1 x2 flutter-mane=",,,,,
+842,"+1 x2 flutter-mane=, +1 x2 chien-pao=",,,,,
 830,+1 x2 whimsicott+,,,,,
 806,+1 x2 tornadus-incarnate+,,,,,
 803,+1 x2 ogerpon+,,,,,
-797,+1 x2 walking-wake+,,,,,
+797,+1 x2 ninetales-alola+,,,,,
 758,"+1 x2 whimsicott=, +1 x2 landorus-incarnate+",,,,,
-752,"+1 x2 entei+, +1 x2 chi-yu+",,,,,
-743,+1 x2 iron-crown+,,,,,
-734,"+1 x2 tornadus-incarnate=, +1 x2 urshifu-rapid-strike+, +1 x2 urshifu-single-strike+",,,,,
+752,+1 x2 chi-yu+,,,,,
+734,"+1 x2 urshifu-rapid-strike+, +1 x2 urshifu-single-strike+, +1 x2 tornadus-incarnate=",,,,,
 731,+1 x2 ogerpon=,,,,,
-725,+1 x2 walking-wake=,,,,,
-707,+1 x2 landorus-therian+,,,,,
+725,+1 x2 ninetales-alola=,,,,,
+707,+1 x2 gouging-fire+,,,,,
+704,+1 x2 arcanine-hisui+,,,,,
 689,+1 x2 landorus-incarnate=,,,,,
-686,"+1 x2 chi-yu=, +1 x2 entei=",,,,,
-677,"+1 x2 indeedee-female+, +1 x2 rillaboom+, +1 x2 archaludon+, +1 x2 iron-crown=",,,,,
-671,"+1 x2 urshifu-single-strike=, +1 x2 urshifu-rapid-strike=, +1 x2 gholdengo+",,,,,
+686,+1 x2 chi-yu=,,,,,
+677,"+1 x2 articuno+, +1 x2 indeedee-female+, +1 x2 rillaboom+",,,,,
+671,"+1 x2 urshifu-rapid-strike=, +1 x2 gholdengo+, +1 x2 urshifu-single-strike=",,,,,
 653,+1 x2 dragonite+,,,,,
-644,+1 x2 landorus-therian=,,,,,
+644,+1 x2 gouging-fire=,,,,,
+641,+1 x2 arcanine-hisui=,,,,,
 626,+1 x2 raging-bolt+,,,,,
-617,"+1 x2 indeedee-female=, +2 flutter-mane+, +1 x2 rillaboom=, +2 chien-pao+, +1 x2 archaludon=",,,,,
+617,"+1 x2 indeedee-female=, +1 x2 rillaboom=, +1 x2 articuno=, +2 chien-pao+, +2 flutter-mane+",,,,,
 615,,"+1 x2 flutter-mane+, +1 x2 chien-pao+",,,,
 614,+1 x2 gholdengo=,,,,,
 596,+1 x2 dragonite=,,,,,
 572,+1 x2 raging-bolt=,,,,,
-563,"+2 chien-pao=, +2 flutter-mane=",,,,,
-561,,"+1 x2 chien-pao=, +1 x2 flutter-mane=",,,,
-554,"+1 x2 incineroar+, +1 x2 farigiraf+, +2 whimsicott+",,,,,
+563,"+2 flutter-mane=, +2 chien-pao=",,,,,
+561,,"+1 x2 flutter-mane=, +1 x2 chien-pao=",,,,
+554,"+2 whimsicott+, +1 x2 farigiraf+, +1 x2 grimmsnarl+, +1 x2 incineroar+",,,,,
 553,,+1 x2 whimsicott+,,,,
 539,+2 tornadus-incarnate+,,,,,
 537,,+1 x2 tornadus-incarnate+,,,,
 536,+2 ogerpon+,,,,,
 535,,+1 x2 ogerpon+,,,,
-533,+2 walking-wake+,,,,,
-531,,+1 x2 walking-wake+,,,,
-506,"+2 landorus-incarnate+, +2 whimsicott=, +1 x2 farigiraf=, +1 x2 incineroar=, +1 x2 iron-hands+, +1 x2 kingambit+",,,,,
+533,+2 ninetales-alola+,,,,,
+531,,+1 x2 ninetales-alola+,,,,
+506,"+2 landorus-incarnate+, +1 x2 farigiraf=, +1 x2 incineroar=, +2 whimsicott=, +1 x2 grimmsnarl=",,,,,
 505,,"+1 x2 whimsicott=, +1 x2 landorus-incarnate+",,,,
-503,"+2 entei+, +2 chi-yu+",,,,,
-501,,"+1 x2 entei+, +1 x2 chi-yu+",,,,
-497,+2 iron-crown+,,,,,
-495,,+1 x2 iron-crown+,,,,
-491,"+2 urshifu-rapid-strike+, +2 urshifu-single-strike+, +2 tornadus-incarnate=",,,,,
-489,,"+1 x2 tornadus-incarnate=, +1 x2 urshifu-rapid-strike+, +1 x2 urshifu-single-strike+",,,,
+503,+2 chi-yu+,,,,,
+501,,+1 x2 chi-yu+,,,,
+491,"+2 tornadus-incarnate=, +2 urshifu-rapid-strike+, +2 urshifu-single-strike+",,,,,
+489,,"+1 x2 urshifu-rapid-strike+, +1 x2 urshifu-single-strike+, +1 x2 tornadus-incarnate=",,,,
 488,+2 ogerpon=,,,,,
 487,,+1 x2 ogerpon=,,,,
-485,+2 walking-wake=,,,,,
-483,,+1 x2 walking-wake=,,,,
-473,+2 landorus-therian+,,,,,
-471,,+1 x2 landorus-therian+,,,,
+485,+2 ninetales-alola=,,,,,
+483,,+1 x2 ninetales-alola=,,,,
+479,+1 x2 ting-lu+,,,,,
+473,+2 gouging-fire+,,,,,
+471,,+1 x2 gouging-fire+,,,,
+470,+2 arcanine-hisui+,,,,,
+469,,+1 x2 arcanine-hisui+,,,,
 462,"+1 chien-pao+, +1 flutter-mane+",,"+1 x2 flutter-mane+, +1 x2 chien-pao+",,,
-461,"+1 x2 iron-hands=, +1 x2 kingambit=, +2 landorus-incarnate=",,,,,
+461,+2 landorus-incarnate=,,,,,
 459,,+1 x2 landorus-incarnate=,,,,
-458,"+2 entei=, +2 chi-yu=",,,,,
-457,,"+1 x2 chi-yu=, +1 x2 entei=",,,,
-452,"+2 iron-crown=, +2 archaludon+, +2 indeedee-female+, +2 rillaboom+",,,,,
-451,,"+1 x2 indeedee-female+, +1 x2 rillaboom+, +1 x2 archaludon+, +1 x2 iron-crown=",,,,
-449,"+2 gholdengo+, +2 urshifu-single-strike=, +2 urshifu-rapid-strike=",,,,,
-447,,"+1 x2 urshifu-single-strike=, +1 x2 urshifu-rapid-strike=, +1 x2 gholdengo+",,,,
-437,+2 dragonite+,,,,,
+458,+2 chi-yu=,,,,,
+457,,+1 x2 chi-yu=,,,,
+452,"+2 articuno+, +2 indeedee-female+, +2 rillaboom+",,,,,
+451,,"+1 x2 articuno+, +1 x2 indeedee-female+, +1 x2 rillaboom+",,,,
+449,"+2 urshifu-rapid-strike=, +2 urshifu-single-strike=, +2 gholdengo+",,,,,
+447,,"+1 x2 urshifu-rapid-strike=, +1 x2 gholdengo+, +1 x2 urshifu-single-strike=",,,,
+437,"+2 dragonite+, +1 x2 ting-lu=",,,,,
 435,,+1 x2 dragonite+,,,,
-431,+2 landorus-therian=,,,,,
-429,,+1 x2 landorus-therian=,,,,
-422,"+1 flutter-mane=, +1 chien-pao=",,"+1 x2 chien-pao=, +1 x2 flutter-mane=",,,
+431,+2 gouging-fire=,,,,,
+429,,+1 x2 gouging-fire=,,,,
+428,"+2 arcanine-hisui=, +1 x2 dondozo+",,,,,
+427,,+1 x2 arcanine-hisui=,,,,
+422,"+1 flutter-mane=, +1 chien-pao=",,"+1 x2 flutter-mane=, +1 x2 chien-pao=",,,
 419,+2 raging-bolt+,,,,,
 417,,+1 x2 raging-bolt+,,,,
 416,+1 whimsicott+,,+1 x2 whimsicott+,,,
-413,"+2 archaludon=, +2 indeedee-female=, +2 rillaboom=",,,,,
-411,,"+1 x2 indeedee-female=, +2 flutter-mane+, +1 x2 rillaboom=, +2 chien-pao+, +1 x2 archaludon=",,,,
-410,"-1 x2 flutter-mane+, -1 x2 chien-pao+, +2 gholdengo=",,,"+1 x2 flutter-mane+, +1 x2 chien-pao+",,
+413,"+2 indeedee-female=, +2 articuno=, +2 rillaboom=",,,,,
+411,,"+1 x2 indeedee-female=, +1 x2 rillaboom=, +1 x2 articuno=, +2 chien-pao+, +2 flutter-mane+",,,,
+410,"-1 x2 chien-pao+, +2 gholdengo=, -1 x2 flutter-mane+",,,"+1 x2 flutter-mane+, +1 x2 chien-pao+",,
 409,,+1 x2 gholdengo=,,,,
 407,+1 x2 amoonguss+,,,,,
 404,+1 tornadus-incarnate+,,+1 x2 tornadus-incarnate+,,,
 402,+1 ogerpon+,,+1 x2 ogerpon+,,,
-399,+1 walking-wake+,,+1 x2 walking-wake+,,,
+399,+1 ninetales-alola+,,+1 x2 ninetales-alola+,,,
 398,+2 dragonite=,,,,,
 397,,+1 x2 dragonite=,,,,
+392,+1 x2 dondozo=,,,,,
 383,+2 raging-bolt=,,,,,
 381,,+1 x2 raging-bolt=,,,,
 380,"+1 landorus-incarnate+, +1 whimsicott=",,"+1 x2 whimsicott=, +1 x2 landorus-incarnate+",,,
-377,"+1 chi-yu+, +1 entei+",,"+1 x2 entei+, +1 x2 chi-yu+",,,
-375,,"+2 chien-pao=, +2 flutter-mane=",,,,
-374,"-1 x2 flutter-mane=, -1 x2 chien-pao=",,,"+1 x2 chien-pao=, +1 x2 flutter-mane=",,
-372,+1 iron-crown+,,+1 x2 iron-crown+,,,
-371,"+1 x2 amoonguss=, +2 incineroar+, +2 farigiraf+",,,,,
-369,,"+1 x2 incineroar+, +1 x2 farigiraf+, +2 whimsicott+",,+1 x2 whimsicott+,,
-368,"-1 x2 whimsicott+, +1 urshifu-rapid-strike+, +1 tornadus-incarnate=, +1 urshifu-single-strike+",,"+1 x2 tornadus-incarnate=, +1 x2 urshifu-rapid-strike+, +1 x2 urshifu-single-strike+",,,
+377,+1 chi-yu+,,+1 x2 chi-yu+,,,
+375,,"+2 flutter-mane=, +2 chien-pao=",,,,
+374,"-1 x2 flutter-mane=, -1 x2 chien-pao=",,,"+1 x2 flutter-mane=, +1 x2 chien-pao=",,
+371,"+2 incineroar+, +2 farigiraf+, +2 grimmsnarl+, +1 x2 amoonguss=",,,,,
+369,,"+2 whimsicott+, +1 x2 farigiraf+, +1 x2 grimmsnarl+, +1 x2 incineroar+",,+1 x2 whimsicott+,,
+368,"-1 x2 whimsicott+, +1 urshifu-single-strike+, +1 tornadus-incarnate=, +1 urshifu-rapid-strike+",,"+1 x2 urshifu-rapid-strike+, +1 x2 urshifu-single-strike+, +1 x2 tornadus-incarnate=",,,
 366,+1 ogerpon=,,+1 x2 ogerpon=,,,
-363,+1 walking-wake=,,+1 x2 walking-wake=,,,
+363,+1 ninetales-alola=,,+1 x2 ninetales-alola=,,,
 359,-1 x2 tornadus-incarnate+,+2 tornadus-incarnate+,,,,
 358,,,,+1 x2 tornadus-incarnate+,,
 357,,+2 ogerpon+,,+1 x2 ogerpon+,,
-356,"-1 x2 ogerpon+, +1 x2 torkoal+, -1 x2 walking-wake+",,,,,
-355,,+2 walking-wake+,,,,
-354,+1 landorus-therian+,,+1 x2 landorus-therian+,+1 x2 walking-wake+,,
+356,"-1 x2 ogerpon+, -1 x2 ninetales-alola+",,,,,
+355,,+2 ninetales-alola+,,,,
+354,+1 gouging-fire+,,+1 x2 gouging-fire+,+1 x2 ninetales-alola+,,
+353,+1 arcanine-hisui+,,+1 x2 arcanine-hisui+,,,
 345,+1 landorus-incarnate=,,+1 x2 landorus-incarnate=,,,
-344,"+1 entei=, +1 chi-yu=",,"+1 x2 chi-yu=, +1 x2 entei=",,,
-339,"+1 archaludon+, +1 rillaboom+, +1 indeedee-female+, +1 iron-crown=",,"+1 x2 indeedee-female+, +1 x2 rillaboom+, +1 x2 archaludon+, +1 x2 iron-crown=",,,
-338,"+2 incineroar=, +2 farigiraf=, +2 kingambit+, -1 x2 whimsicott=, -1 x2 landorus-incarnate+, +2 iron-hands+",,,,,
-337,,"+2 landorus-incarnate+, +2 whimsicott=, +1 x2 farigiraf=, +1 x2 incineroar=, +1 x2 iron-hands+, +1 x2 kingambit+",,"+1 x2 whimsicott=, +1 x2 landorus-incarnate+",,
-336,"+1 urshifu-single-strike=, +1 gholdengo+, +1 urshifu-rapid-strike=",,"+1 x2 urshifu-single-strike=, +1 x2 urshifu-rapid-strike=, +1 x2 gholdengo+",,,
-335,"-1 x2 entei+, -1 x2 chi-yu+","+2 entei+, +2 chi-yu+",,,,
-334,,,,"+1 x2 entei+, +1 x2 chi-yu+",,
-332,-1 x2 iron-crown+,,,,,
-331,,+2 iron-crown+,,,,
-330,,,,+1 x2 iron-crown+,,
-327,+1 dragonite+,"+2 urshifu-rapid-strike+, +2 urshifu-single-strike+, +2 tornadus-incarnate=",+1 x2 dragonite+,,,
-326,"-1 x2 tornadus-incarnate=, +1 x2 torkoal=, -1 x2 urshifu-single-strike+, -1 x2 urshifu-rapid-strike+, -1 x2 ogerpon=",,,"+1 x2 tornadus-incarnate=, +1 x2 urshifu-rapid-strike+, +1 x2 urshifu-single-strike+",,
+344,+1 chi-yu=,,+1 x2 chi-yu=,,,
+339,"+1 rillaboom+, +1 articuno+, +1 indeedee-female+",,"+1 x2 articuno+, +1 x2 indeedee-female+, +1 x2 rillaboom+",,,
+338,"+2 farigiraf=, -1 x2 whimsicott=, +2 incineroar=, +2 grimmsnarl=, -1 x2 landorus-incarnate+",,,,,
+337,,"+2 landorus-incarnate+, +1 x2 farigiraf=, +1 x2 incineroar=, +2 whimsicott=, +1 x2 grimmsnarl=",,"+1 x2 whimsicott=, +1 x2 landorus-incarnate+",,
+336,"+1 urshifu-single-strike=, +1 gholdengo+, +1 urshifu-rapid-strike=",,"+1 x2 urshifu-rapid-strike=, +1 x2 gholdengo+, +1 x2 urshifu-single-strike=",,,
+335,-1 x2 chi-yu+,+2 chi-yu+,,,,
+334,,,,+1 x2 chi-yu+,,
+327,+1 dragonite+,"+2 tornadus-incarnate=, +2 urshifu-rapid-strike+, +2 urshifu-single-strike+",+1 x2 dragonite+,,,
+326,"-1 x2 urshifu-rapid-strike+, -1 x2 tornadus-incarnate=, -1 x2 urshifu-single-strike+, -1 x2 ogerpon=",,,"+1 x2 urshifu-rapid-strike+, +1 x2 urshifu-single-strike+, +1 x2 tornadus-incarnate=",,
 325,,+2 ogerpon=,,+1 x2 ogerpon=,,
-323,"-1 x2 walking-wake=, +1 landorus-therian=",+2 walking-wake=,+1 x2 landorus-therian=,,,
-322,,,,+1 x2 walking-wake=,,
-315,,+2 landorus-therian+,,,,
-314,"-1 x2 landorus-therian+, +1 raging-bolt+",,+1 x2 raging-bolt+,+1 x2 landorus-therian+,,
-309,"+1 indeedee-female=, +1 archaludon=, flutter-mane+, chien-pao+, +1 rillaboom=",,"+1 x2 indeedee-female=, +2 flutter-mane+, +1 x2 rillaboom=, +2 chien-pao+, +1 x2 archaludon=",,,
-308,"+2 iron-hands=, +2 kingambit=, +1 gholdengo=, -1 x2 landorus-incarnate=","+1 chien-pao+, +1 flutter-mane+",+1 x2 gholdengo=,,"+1 x2 flutter-mane+, +1 x2 chien-pao+",
-307,,"+1 x2 iron-hands=, +1 x2 kingambit=, +2 landorus-incarnate=",,,,
+323,"+1 gouging-fire=, -1 x2 ninetales-alola=",+2 ninetales-alola=,+1 x2 gouging-fire=,,,
+322,,,,+1 x2 ninetales-alola=,,
+321,+1 arcanine-hisui=,,+1 x2 arcanine-hisui=,,,
+320,+2 ting-lu+,,,,,
+319,,+1 x2 ting-lu+,,,,
+315,,+2 gouging-fire+,,,,
+314,"-1 x2 gouging-fire+, +1 raging-bolt+, -1 x2 arcanine-hisui+",,+1 x2 raging-bolt+,+1 x2 gouging-fire+,,
+313,,+2 arcanine-hisui+,,+1 x2 arcanine-hisui+,,
+309,"+1 articuno=, flutter-mane+, +1 rillaboom=, chien-pao+, +1 indeedee-female=",,"+1 x2 indeedee-female=, +1 x2 rillaboom=, +1 x2 articuno=, +2 chien-pao+, +2 flutter-mane+",,,
+308,"-1 x2 landorus-incarnate=, +1 gholdengo=","+1 chien-pao+, +1 flutter-mane+",+1 x2 gholdengo=,,"+1 x2 flutter-mane+, +1 x2 chien-pao+",
+307,,+2 landorus-incarnate=,,,,
 306,,,,+1 x2 landorus-incarnate=,,
-305,"-1 x2 entei=, -1 x2 chi-yu=","+2 entei=, +2 chi-yu=",,"+1 x2 chi-yu=, +1 x2 entei=",,
-302,"-1 x2 indeedee-female+, -1 x2 rillaboom+, -1 x2 iron-crown=, -1 x2 archaludon+",,,,,
-301,,"+2 iron-crown=, +2 archaludon+, +2 indeedee-female+, +2 rillaboom+",,"+1 x2 indeedee-female+, +1 x2 rillaboom+, +1 x2 archaludon+, +1 x2 iron-crown=",,
-299,"+1 dragonite=, -1 x2 urshifu-rapid-strike=, -1 x2 urshifu-single-strike=, -1 x2 gholdengo+","+2 gholdengo+, +2 urshifu-single-strike=, +2 urshifu-rapid-strike=",+1 x2 dragonite=,,,
-298,,,,"+1 x2 urshifu-single-strike=, +1 x2 urshifu-rapid-strike=, +1 x2 gholdengo+",,
-291,,+2 dragonite+,,,,
+305,-1 x2 chi-yu=,+2 chi-yu=,,+1 x2 chi-yu=,,
+302,"-1 x2 indeedee-female+, -1 x2 rillaboom+, -1 x2 articuno+",,,,,
+301,,"+2 articuno+, +2 indeedee-female+, +2 rillaboom+",,"+1 x2 articuno+, +1 x2 indeedee-female+, +1 x2 rillaboom+",,
+299,"+1 dragonite=, -1 x2 gholdengo+, -1 x2 urshifu-single-strike=, -1 x2 urshifu-rapid-strike=","+2 urshifu-rapid-strike=, +2 urshifu-single-strike=, +2 gholdengo+",+1 x2 dragonite=,,,
+298,,,,"+1 x2 urshifu-rapid-strike=, +1 x2 gholdengo+, +1 x2 urshifu-single-strike=",,
+293,+2 ting-lu=,,,,,
+291,,"+2 dragonite+, +1 x2 ting-lu=",,,,
 290,-1 x2 dragonite+,,,+1 x2 dragonite+,,
-287,"-1 x2 landorus-therian=, +1 raging-bolt=",+2 landorus-therian=,+1 x2 raging-bolt=,,,
-286,,,,+1 x2 landorus-therian=,,
-282,"flutter-mane=, chien-pao=",,"+2 chien-pao=, +2 flutter-mane=",,,
-281,,"+1 flutter-mane=, +1 chien-pao=",,,"+1 x2 chien-pao=, +1 x2 flutter-mane=",
+287,"+2 dondozo+, +1 raging-bolt=, -1 x2 gouging-fire=",+2 gouging-fire=,+1 x2 raging-bolt=,,,
+286,,,,+1 x2 gouging-fire=,,
+285,,"+2 arcanine-hisui=, +1 x2 dondozo+",,+1 x2 arcanine-hisui=,,
+284,-1 x2 arcanine-hisui=,,,,,
+282,"flutter-mane=, chien-pao=",,"+2 flutter-mane=, +2 chien-pao=",,,
+281,,"+1 flutter-mane=, +1 chien-pao=",,,"+1 x2 flutter-mane=, +1 x2 chien-pao=",
 279,,+2 raging-bolt+,,,,
-278,"+1 incineroar+, -1 x2 raging-bolt+, whimsicott+, +1 farigiraf+",,"+1 x2 incineroar+, +1 x2 farigiraf+, +2 whimsicott+",+1 x2 raging-bolt+,,
+278,"whimsicott+, +1 grimmsnarl+, -1 x2 raging-bolt+, +1 farigiraf+, +1 incineroar+",,"+2 whimsicott+, +1 x2 farigiraf+, +1 x2 grimmsnarl+, +1 x2 incineroar+",+1 x2 raging-bolt+,,
 277,,+1 whimsicott+,,,+1 x2 whimsicott+,
-275,"-1 x2 rillaboom=, -1 x2 indeedee-female=, -1 x2 archaludon=","+2 archaludon=, +2 indeedee-female=, +2 rillaboom=",,,,
-274,,,,"+1 x2 indeedee-female=, +2 flutter-mane+, +1 x2 rillaboom=, +2 chien-pao+, +1 x2 archaludon=",,
-273,,"-1 x2 flutter-mane+, -1 x2 chien-pao+, +2 gholdengo=",,+1 x2 gholdengo=,,
-272,"+2 amoonguss+, -1 x2 gholdengo=",,,,,
+275,"-1 x2 indeedee-female=, -1 x2 articuno=, -1 x2 rillaboom=","+2 indeedee-female=, +2 articuno=, +2 rillaboom=",,,,
+274,,,,"+1 x2 indeedee-female=, +1 x2 rillaboom=, +1 x2 articuno=, +2 chien-pao+, +2 flutter-mane+",,
+273,,"-1 x2 chien-pao+, +2 gholdengo=, -1 x2 flutter-mane+",,+1 x2 gholdengo=,,
+272,"-1 x2 gholdengo=, +2 amoonguss+",,,,,
 271,,+1 x2 amoonguss+,,,,
 270,tornadus-incarnate+,,+2 tornadus-incarnate+,,,
 269,ogerpon+,+1 tornadus-incarnate+,+2 ogerpon+,,+1 x2 tornadus-incarnate+,
 268,,+1 ogerpon+,,,+1 x2 ogerpon+,
-267,walking-wake+,,+2 walking-wake+,,,
-266,-1 x2 dragonite=,+1 walking-wake+,,,+1 x2 walking-wake+,
+267,ninetales-alola+,,+2 ninetales-alola+,,,
+266,-1 x2 dragonite=,+1 ninetales-alola+,,,+1 x2 ninetales-alola+,
 265,,+2 dragonite=,,+1 x2 dragonite=,,
+263,+2 dondozo=,,,,,
+261,,+1 x2 dondozo=,,,,
 255,,+2 raging-bolt=,,,,
-254,"-1 x2 raging-bolt=, whimsicott=, +1 iron-hands+, +1 incineroar=, landorus-incarnate+, +1 kingambit+, +1 farigiraf=",,"+2 landorus-incarnate+, +2 whimsicott=, +1 x2 farigiraf=, +1 x2 incineroar=, +1 x2 iron-hands+, +1 x2 kingambit+",+1 x2 raging-bolt=,,
+254,"+1 farigiraf=, whimsicott=, landorus-incarnate+, +1 incineroar=, -1 x2 raging-bolt=, +1 grimmsnarl=",,"+2 landorus-incarnate+, +1 x2 farigiraf=, +1 x2 incineroar=, +2 whimsicott=, +1 x2 grimmsnarl=",+1 x2 raging-bolt=,,
 253,,"+1 landorus-incarnate+, +1 whimsicott=",,,"+1 x2 whimsicott=, +1 x2 landorus-incarnate+",
-252,"entei+, chi-yu+",,"+2 entei+, +2 chi-yu+",,,
-251,,"+1 chi-yu+, +1 entei+",,,"+1 x2 entei+, +1 x2 chi-yu+",
-250,,,,"+2 chien-pao=, +2 flutter-mane=",,
-249,iron-crown+,"-1 x2 flutter-mane=, -1 x2 chien-pao=",+2 iron-crown+,,,
-248,"-1 x2 farigiraf+, +2 amoonguss=, -1 x2 incineroar+",+1 iron-crown+,,,+1 x2 iron-crown+,
-247,,"+1 x2 amoonguss=, +2 incineroar+, +2 farigiraf+",,,,
-246,"tornadus-incarnate=, urshifu-single-strike+, urshifu-rapid-strike+",,"+2 urshifu-rapid-strike+, +2 urshifu-single-strike+, +2 tornadus-incarnate=","+1 x2 incineroar+, +1 x2 farigiraf+, +2 whimsicott+",,
-245,ogerpon=,"-1 x2 whimsicott+, +1 urshifu-rapid-strike+, +1 tornadus-incarnate=, +1 urshifu-single-strike+",+2 ogerpon=,,"+1 x2 tornadus-incarnate=, +1 x2 urshifu-rapid-strike+, +1 x2 urshifu-single-strike+",
+252,chi-yu+,,+2 chi-yu+,,,
+251,,+1 chi-yu+,,,+1 x2 chi-yu+,
+250,,,,"+2 flutter-mane=, +2 chien-pao=",,
+249,,"-1 x2 flutter-mane=, -1 x2 chien-pao=",,,,
+248,"-1 x2 farigiraf+, -1 x2 incineroar+, -1 x2 grimmsnarl+, +2 amoonguss=",,,,,
+247,,"+2 incineroar+, +2 farigiraf+, +2 grimmsnarl+, +1 x2 amoonguss=",,,,
+246,"tornadus-incarnate=, urshifu-rapid-strike+, urshifu-single-strike+",,"+2 tornadus-incarnate=, +2 urshifu-rapid-strike+, +2 urshifu-single-strike+","+2 whimsicott+, +1 x2 farigiraf+, +1 x2 grimmsnarl+, +1 x2 incineroar+",,
+245,ogerpon=,"-1 x2 whimsicott+, +1 urshifu-single-strike+, +1 tornadus-incarnate=, +1 urshifu-rapid-strike+",+2 ogerpon=,,"+1 x2 urshifu-rapid-strike+, +1 x2 urshifu-single-strike+, +1 x2 tornadus-incarnate=",
 244,,+1 ogerpon=,,,+1 x2 ogerpon=,
-243,walking-wake=,,+2 walking-wake=,,,
-242,,+1 walking-wake=,,,+1 x2 walking-wake=,
-240,,,,+2 tornadus-incarnate+,,
-239,+2 torkoal+,-1 x2 tornadus-incarnate+,,,,
+243,ninetales-alola=,,+2 ninetales-alola=,,,
+242,,+1 ninetales-alola=,,,+1 x2 ninetales-alola=,
+240,+1 ting-lu+,,+1 x2 ting-lu+,+2 tornadus-incarnate+,,
+239,,-1 x2 tornadus-incarnate+,,,,
 238,,,,+2 ogerpon+,,
-237,landorus-therian+,"-1 x2 ogerpon+, +1 x2 torkoal+, -1 x2 walking-wake+",+2 landorus-therian+,+2 walking-wake+,,
-236,,+1 landorus-therian+,,,+1 x2 landorus-therian+,
-231,"+1 kingambit=, +1 iron-hands=, landorus-incarnate=",,"+1 x2 iron-hands=, +1 x2 kingambit=, +1 chien-pao+, +2 landorus-incarnate=, +1 flutter-mane+",,,
-230,"chi-yu=, entei=",+1 landorus-incarnate=,"+2 entei=, +2 chi-yu=",,+1 x2 landorus-incarnate=,
-229,,"+1 entei=, +1 chi-yu=",,,"+1 x2 chi-yu=, +1 x2 entei=",
-227,"iron-crown=, archaludon+, indeedee-female+, rillaboom+",,"+2 iron-crown=, +2 archaludon+, +2 indeedee-female+, +2 rillaboom+",,,
-226,,"+1 archaludon+, +1 rillaboom+, +1 indeedee-female+, +1 iron-crown=",,,"+1 x2 indeedee-female+, +1 x2 rillaboom+, +1 x2 archaludon+, +1 x2 iron-crown=",
-225,"urshifu-rapid-strike=, urshifu-single-strike=, gholdengo+","+2 incineroar=, +2 farigiraf=, +2 kingambit+, -1 x2 whimsicott=, -1 x2 landorus-incarnate+, +2 iron-hands+","+2 gholdengo+, +2 urshifu-single-strike=, +2 urshifu-rapid-strike=","+2 landorus-incarnate+, +2 whimsicott=, +1 x2 farigiraf=, +1 x2 incineroar=, +1 x2 iron-hands+, +1 x2 kingambit+",,
-224,"-1 x2 incineroar=, -1 x2 farigiraf=, -1 x2 iron-hands+, -1 x2 kingambit+","+1 urshifu-single-strike=, +1 gholdengo+, +1 urshifu-rapid-strike=",,"+2 entei+, +2 chi-yu+","+1 x2 urshifu-single-strike=, +1 x2 urshifu-rapid-strike=, +1 x2 gholdengo+",
-223,,"-1 x2 entei+, -1 x2 chi-yu+",,,,
-221,,-1 x2 iron-crown+,,+2 iron-crown+,,
-219,dragonite+,,+2 dragonite+,,,
-218,+2 torkoal=,+1 dragonite+,,"+2 urshifu-rapid-strike+, +2 urshifu-single-strike+, +2 tornadus-incarnate=",+1 x2 dragonite+,
-217,,"-1 x2 tornadus-incarnate=, +1 x2 torkoal=, -1 x2 urshifu-single-strike+, -1 x2 urshifu-rapid-strike+, -1 x2 ogerpon=",,+2 ogerpon=,,
-216,landorus-therian=,,+2 landorus-therian=,+2 walking-wake=,,
-215,,"-1 x2 walking-wake=, +1 landorus-therian=",,,+1 x2 landorus-therian=,
-212,,,"+1 flutter-mane=, +1 chien-pao=",,,
-210,raging-bolt+,,+2 raging-bolt+,+2 landorus-therian+,,
-209,,"-1 x2 landorus-therian+, +1 raging-bolt+",+1 whimsicott+,,+1 x2 raging-bolt+,
-207,"rillaboom=, indeedee-female=, archaludon=",,"+2 archaludon=, +2 indeedee-female=, +2 rillaboom=",,,
-206,"-1 x2 iron-hands=, gholdengo=, -1 chien-pao+, -1 flutter-mane+, -1 x2 kingambit=","+1 indeedee-female=, +1 archaludon=, flutter-mane+, chien-pao+, +1 rillaboom=","-1 x2 flutter-mane+, -1 x2 chien-pao+, +2 gholdengo=","+1 chien-pao+, +1 flutter-mane+","+1 x2 indeedee-female=, +2 flutter-mane+, +1 x2 rillaboom=, +2 chien-pao+, +1 x2 archaludon=","+1 x2 flutter-mane+, +1 x2 chien-pao+"
-205,,"+2 iron-hands=, +2 kingambit=, +1 gholdengo=, -1 x2 landorus-incarnate=",,"+1 x2 iron-hands=, +1 x2 kingambit=, +2 landorus-incarnate=",+1 x2 gholdengo=,
-204,+1 amoonguss+,,+1 x2 amoonguss+,"+2 entei=, +2 chi-yu=",,
-203,,"-1 x2 entei=, -1 x2 chi-yu=",+1 tornadus-incarnate+,,,
-201,,"-1 x2 indeedee-female+, -1 x2 rillaboom+, -1 x2 iron-crown=, -1 x2 archaludon+",+1 ogerpon+,"+2 iron-crown=, +2 archaludon+, +2 indeedee-female+, +2 rillaboom+",,
-200,dragonite=,,"+2 dragonite=, +1 walking-wake+","+2 gholdengo+, +2 urshifu-single-strike=, +2 urshifu-rapid-strike=",,
-199,,"+1 dragonite=, -1 x2 urshifu-rapid-strike=, -1 x2 urshifu-single-strike=, -1 x2 gholdengo+",,,+1 x2 dragonite=,
-194,,,,+2 dragonite+,,
+237,gouging-fire+,"-1 x2 ogerpon+, -1 x2 ninetales-alola+",+2 gouging-fire+,+2 ninetales-alola+,,
+236,arcanine-hisui+,+1 gouging-fire+,+2 arcanine-hisui+,,+1 x2 gouging-fire+,
+235,,+1 arcanine-hisui+,,,+1 x2 arcanine-hisui+,
+231,landorus-incarnate=,,"+2 landorus-incarnate=, +1 chien-pao+, +1 flutter-mane+",,,
+230,chi-yu=,+1 landorus-incarnate=,+2 chi-yu=,,+1 x2 landorus-incarnate=,
+229,,+1 chi-yu=,,,+1 x2 chi-yu=,
+227,"articuno+, indeedee-female+, rillaboom+",,"+2 articuno+, +2 indeedee-female+, +2 rillaboom+",,,
+226,,"+1 rillaboom+, +1 articuno+, +1 indeedee-female+",,,"+1 x2 articuno+, +1 x2 indeedee-female+, +1 x2 rillaboom+",
+225,"gholdengo+, urshifu-single-strike=, urshifu-rapid-strike=","+2 farigiraf=, -1 x2 whimsicott=, +2 incineroar=, +2 grimmsnarl=, -1 x2 landorus-incarnate+","+2 urshifu-rapid-strike=, +2 urshifu-single-strike=, +2 gholdengo+","+2 landorus-incarnate+, +1 x2 farigiraf=, +1 x2 incineroar=, +2 whimsicott=, +1 x2 grimmsnarl=",,
+224,"-1 x2 farigiraf=, -1 x2 incineroar=, -1 x2 grimmsnarl=","+1 urshifu-single-strike=, +1 gholdengo+, +1 urshifu-rapid-strike=",,+2 chi-yu+,"+1 x2 urshifu-rapid-strike=, +1 x2 gholdengo+, +1 x2 urshifu-single-strike=",
+223,,-1 x2 chi-yu+,,,,
+219,"dragonite+, +1 ting-lu=",,"+2 dragonite+, +1 x2 ting-lu=",,,
+218,,+1 dragonite+,,"+2 tornadus-incarnate=, +2 urshifu-rapid-strike+, +2 urshifu-single-strike+",+1 x2 dragonite+,
+217,,"-1 x2 urshifu-rapid-strike+, -1 x2 tornadus-incarnate=, -1 x2 urshifu-single-strike+, -1 x2 ogerpon=",,+2 ogerpon=,,
+216,gouging-fire=,,+2 gouging-fire=,+2 ninetales-alola=,,
+215,"arcanine-hisui=, +1 dondozo+","+1 gouging-fire=, -1 x2 ninetales-alola=","+2 arcanine-hisui=, +1 x2 dondozo+",,+1 x2 gouging-fire=,
+214,,+1 arcanine-hisui=,,,+1 x2 arcanine-hisui=,
+213,,+2 ting-lu+,,+1 x2 ting-lu+,,
+212,-1 x2 ting-lu+,,"+1 flutter-mane=, +1 chien-pao=",,,
+210,raging-bolt+,,+2 raging-bolt+,+2 gouging-fire+,,
+209,,"-1 x2 gouging-fire+, +1 raging-bolt+, -1 x2 arcanine-hisui+",+1 whimsicott+,+2 arcanine-hisui+,+1 x2 raging-bolt+,
+207,"articuno=, indeedee-female=, rillaboom=",,"+2 indeedee-female=, +2 articuno=, +2 rillaboom=",,,
+206,"-1 flutter-mane+, -1 chien-pao+, gholdengo=","+1 articuno=, flutter-mane+, +1 rillaboom=, chien-pao+, +1 indeedee-female=","-1 x2 chien-pao+, +2 gholdengo=, -1 x2 flutter-mane+","+1 chien-pao+, +1 flutter-mane+","+1 x2 indeedee-female=, +1 x2 rillaboom=, +1 x2 articuno=, +2 chien-pao+, +2 flutter-mane+","+1 x2 flutter-mane+, +1 x2 chien-pao+"
+205,,"-1 x2 landorus-incarnate=, +1 gholdengo=",,+2 landorus-incarnate=,+1 x2 gholdengo=,
+204,+1 amoonguss+,,+1 x2 amoonguss+,+2 chi-yu=,,
+203,,-1 x2 chi-yu=,+1 tornadus-incarnate+,,,
+201,,"-1 x2 indeedee-female+, -1 x2 rillaboom+, -1 x2 articuno+",+1 ogerpon+,"+2 articuno+, +2 indeedee-female+, +2 rillaboom+",,
+200,dragonite=,,"+1 ninetales-alola+, +2 dragonite=","+2 urshifu-rapid-strike=, +2 urshifu-single-strike=, +2 gholdengo+",,
+199,,"+1 dragonite=, -1 x2 gholdengo+, -1 x2 urshifu-single-strike=, -1 x2 urshifu-rapid-strike=",,,+1 x2 dragonite=,
+197,+1 dondozo=,,+1 x2 dondozo=,,,
+195,,+2 ting-lu=,,,,
+194,-1 x2 ting-lu=,,,"+2 dragonite+, +1 x2 ting-lu=",,
 193,,-1 x2 dragonite+,,,,
-192,raging-bolt=,,+2 raging-bolt=,+2 landorus-therian=,,
-191,,"-1 x2 landorus-therian=, +1 raging-bolt=","+1 landorus-incarnate+, +1 whimsicott=",,+1 x2 raging-bolt=,
-189,,,"+1 chi-yu+, +1 entei+",,,
-188,"-1 flutter-mane=, -1 chien-pao=","flutter-mane=, chien-pao=","-1 x2 flutter-mane=, -1 x2 chien-pao=","+1 flutter-mane=, +1 chien-pao=","+2 chien-pao=, +2 flutter-mane=","+1 x2 chien-pao=, +1 x2 flutter-mane="
-186,"farigiraf+, +1 amoonguss=, incineroar+",,"+1 x2 amoonguss=, +1 iron-crown+, +2 incineroar+, +2 farigiraf+",+2 raging-bolt+,,
-185,-1 whimsicott+,"+1 incineroar+, -1 x2 raging-bolt+, whimsicott+, +1 farigiraf+","-1 x2 whimsicott+, +1 urshifu-rapid-strike+, +1 tornadus-incarnate=, +1 urshifu-single-strike+",+1 whimsicott+,"+1 x2 incineroar+, +1 x2 farigiraf+, +2 whimsicott+",+1 x2 whimsicott+
-184,,,,"+2 archaludon=, +2 indeedee-female=, +2 rillaboom=",,
-183,,"-1 x2 rillaboom=, -1 x2 indeedee-female=, -1 x2 archaludon=",+1 ogerpon=,,,
-182,-1 x2 amoonguss+,,+1 walking-wake=,"-1 x2 flutter-mane+, -1 x2 chien-pao+, +2 gholdengo=",,
-181,,"+2 amoonguss+, -1 x2 gholdengo=",,+1 x2 amoonguss+,,
+192,raging-bolt=,,+2 raging-bolt=,+2 gouging-fire=,,
+191,-1 x2 dondozo+,"+2 dondozo+, +1 raging-bolt=, -1 x2 gouging-fire=","+1 landorus-incarnate+, +1 whimsicott=",,+1 x2 raging-bolt=,
+190,,,,"+2 arcanine-hisui=, +1 x2 dondozo+",,
+189,,-1 x2 arcanine-hisui=,+1 chi-yu+,,,
+188,"-1 flutter-mane=, -1 chien-pao=","flutter-mane=, chien-pao=","-1 x2 flutter-mane=, -1 x2 chien-pao=","+1 flutter-mane=, +1 chien-pao=","+2 flutter-mane=, +2 chien-pao=","+1 x2 flutter-mane=, +1 x2 chien-pao="
+186,"incineroar+, farigiraf+, grimmsnarl+, +1 amoonguss=",,"+2 incineroar+, +2 farigiraf+, +2 grimmsnarl+, +1 x2 amoonguss=",+2 raging-bolt+,,
+185,-1 whimsicott+,"whimsicott+, +1 grimmsnarl+, -1 x2 raging-bolt+, +1 farigiraf+, +1 incineroar+","-1 x2 whimsicott+, +1 urshifu-single-strike+, +1 tornadus-incarnate=, +1 urshifu-rapid-strike+",+1 whimsicott+,"+2 whimsicott+, +1 x2 farigiraf+, +1 x2 grimmsnarl+, +1 x2 incineroar+",+1 x2 whimsicott+
+184,,,,"+2 indeedee-female=, +2 articuno=, +2 rillaboom=",,
+183,,"-1 x2 indeedee-female=, -1 x2 articuno=, -1 x2 rillaboom=",+1 ogerpon=,,,
+182,-1 x2 amoonguss+,,+1 ninetales-alola=,"-1 x2 chien-pao+, +2 gholdengo=, -1 x2 flutter-mane+",,
+181,,"-1 x2 gholdengo=, +2 amoonguss+",,+1 x2 amoonguss+,,
 180,-1 tornadus-incarnate+,tornadus-incarnate+,-1 x2 tornadus-incarnate+,+1 tornadus-incarnate+,+2 tornadus-incarnate+,+1 x2 tornadus-incarnate+
-179,"+1 torkoal+, -1 walking-wake+, -1 ogerpon+",ogerpon+,"-1 x2 ogerpon+, +1 x2 torkoal+, -1 x2 walking-wake+",+1 ogerpon+,+2 ogerpon+,+1 x2 ogerpon+
-178,,walking-wake+,,+1 walking-wake+,+2 walking-wake+,+1 x2 walking-wake+
-177,,-1 x2 dragonite=,+1 landorus-therian+,+2 dragonite=,,
-173,,,"+1 entei=, +1 landorus-incarnate=, +1 chi-yu=",,,
-170,"-1 whimsicott=, incineroar=, farigiraf=, iron-hands+, kingambit+, -1 landorus-incarnate+",,"+2 incineroar=, +2 farigiraf=, +1 archaludon+, +2 kingambit+, +1 rillaboom+, -1 x2 whimsicott=, -1 x2 landorus-incarnate+, +2 iron-hands+, +1 indeedee-female+, +1 iron-crown=",+2 raging-bolt=,,
-169,,"-1 x2 raging-bolt=, whimsicott=, +1 iron-hands+, +1 incineroar=, landorus-incarnate+, +1 kingambit+, +1 farigiraf=",,"+1 landorus-incarnate+, +1 whimsicott=","+2 landorus-incarnate+, +2 whimsicott=, +1 x2 farigiraf=, +1 x2 incineroar=, +1 x2 iron-hands+, +1 x2 kingambit+","+1 x2 whimsicott=, +1 x2 landorus-incarnate+"
-168,"-1 chi-yu+, -1 entei+","entei+, chi-yu+","+1 urshifu-single-strike=, -1 x2 entei+, +1 gholdengo+, +1 urshifu-rapid-strike=, -1 x2 chi-yu+","+1 chi-yu+, +1 entei+","+2 entei+, +2 chi-yu+","+1 x2 entei+, +1 x2 chi-yu+"
-167,-1 iron-crown+,,-1 x2 iron-crown+,,,
-166,,iron-crown+,,"+1 iron-crown+, -1 x2 flutter-mane=, -1 x2 chien-pao=",+2 iron-crown+,+1 x2 iron-crown+
-165,,"-1 x2 farigiraf+, +2 amoonguss=, -1 x2 incineroar+",,"+1 x2 amoonguss=, +2 incineroar+, +2 farigiraf+",,
-164,"-1 x2 amoonguss=, -1 urshifu-rapid-strike+, -1 urshifu-single-strike+, +1 torkoal=, -1 ogerpon=, -1 tornadus-incarnate=","tornadus-incarnate=, urshifu-single-strike+, urshifu-rapid-strike+","-1 x2 tornadus-incarnate=, +1 x2 torkoal=, -1 x2 urshifu-single-strike+, -1 x2 urshifu-rapid-strike+, +1 dragonite+, -1 x2 ogerpon=","-1 x2 whimsicott+, +1 urshifu-rapid-strike+, +1 tornadus-incarnate=, +1 urshifu-single-strike+","+2 urshifu-rapid-strike+, +2 urshifu-single-strike+, +2 tornadus-incarnate=","+1 x2 tornadus-incarnate=, +1 x2 urshifu-rapid-strike+, +1 x2 urshifu-single-strike+"
+179,"-1 ogerpon+, -1 ninetales-alola+",ogerpon+,"-1 x2 ogerpon+, -1 x2 ninetales-alola+",+1 ogerpon+,+2 ogerpon+,+1 x2 ogerpon+
+178,,ninetales-alola+,,+1 ninetales-alola+,+2 ninetales-alola+,+1 x2 ninetales-alola+
+177,,-1 x2 dragonite=,"+1 arcanine-hisui+, +1 gouging-fire+",+2 dragonite=,,
+176,-1 x2 dondozo=,,,,,
+175,,+2 dondozo=,,,,
+174,,,,+1 x2 dondozo=,,
+173,,,"+1 landorus-incarnate=, +1 chi-yu=",,,
+170,"farigiraf=, -1 whimsicott=, incineroar=, grimmsnarl=, -1 landorus-incarnate+",,"+1 rillaboom+, +2 farigiraf=, -1 x2 whimsicott=, +1 articuno+, +2 incineroar=, +2 grimmsnarl=, -1 x2 landorus-incarnate+, +1 indeedee-female+",+2 raging-bolt=,,
+169,,"+1 farigiraf=, whimsicott=, landorus-incarnate+, +1 incineroar=, -1 x2 raging-bolt=, +1 grimmsnarl=",,"+1 landorus-incarnate+, +1 whimsicott=","+2 landorus-incarnate+, +1 x2 farigiraf=, +1 x2 incineroar=, +2 whimsicott=, +1 x2 grimmsnarl=","+1 x2 whimsicott=, +1 x2 landorus-incarnate+"
+168,-1 chi-yu+,chi-yu+,"+1 urshifu-single-strike=, +1 gholdengo+, -1 x2 chi-yu+, +1 urshifu-rapid-strike=",+1 chi-yu+,+2 chi-yu+,+1 x2 chi-yu+
+166,,,,"-1 x2 flutter-mane=, -1 x2 chien-pao=",,
+165,,"-1 x2 farigiraf+, -1 x2 incineroar+, -1 x2 grimmsnarl+, +2 amoonguss=",,"+2 incineroar+, +2 farigiraf+, +2 grimmsnarl+, +1 x2 amoonguss=",,
+164,"-1 urshifu-single-strike+, -1 urshifu-rapid-strike+, -1 x2 amoonguss=, -1 ogerpon=, -1 tornadus-incarnate=","tornadus-incarnate=, urshifu-rapid-strike+, urshifu-single-strike+","-1 x2 urshifu-rapid-strike+, +1 dragonite+, -1 x2 tornadus-incarnate=, -1 x2 urshifu-single-strike+, -1 x2 ogerpon=","-1 x2 whimsicott+, +1 urshifu-single-strike+, +1 tornadus-incarnate=, +1 urshifu-rapid-strike+","+2 tornadus-incarnate=, +2 urshifu-rapid-strike+, +2 urshifu-single-strike+","+1 x2 urshifu-rapid-strike+, +1 x2 urshifu-single-strike+, +1 x2 tornadus-incarnate="
 163,,ogerpon=,,+1 ogerpon=,+2 ogerpon=,+1 x2 ogerpon=
-162,-1 walking-wake=,walking-wake=,"-1 x2 walking-wake=, +1 landorus-therian=",+1 walking-wake=,+2 walking-wake=,+1 x2 walking-wake=
-160,,,,-1 x2 tornadus-incarnate+,,
-159,,+2 torkoal+,,,,
-158,"-1 x2 torkoal+, -1 landorus-therian+",landorus-therian+,"-1 x2 landorus-therian+, +1 raging-bolt+","-1 x2 ogerpon+, +1 landorus-therian+, +1 x2 torkoal+, -1 x2 walking-wake+",+2 landorus-therian+,+1 x2 landorus-therian+
-155,"kingambit=, -1 landorus-incarnate=, iron-hands=",,"+1 indeedee-female=, +2 iron-hands=, +1 archaludon=, flutter-mane+, chien-pao+, +2 kingambit=, +1 gholdengo=, -1 x2 landorus-incarnate=, +1 rillaboom=",,,
-154,,"+1 kingambit=, +1 iron-hands=, landorus-incarnate=",,+1 landorus-incarnate=,"+1 x2 iron-hands=, +1 x2 kingambit=, +1 chien-pao+, +2 landorus-incarnate=, +1 flutter-mane+",+1 x2 landorus-incarnate=
-153,"-1 chi-yu=, -1 entei=","chi-yu=, entei=","-1 x2 entei=, -1 x2 chi-yu=","+1 entei=, +1 chi-yu=","+2 entei=, +2 chi-yu=","+1 x2 chi-yu=, +1 x2 entei="
-152,"-1 iron-crown=, -1 rillaboom+, -1 indeedee-female+, -1 archaludon+",,"-1 x2 indeedee-female+, -1 x2 rillaboom+, -1 x2 iron-crown=, -1 x2 archaludon+",,,
-151,,"iron-crown=, archaludon+, indeedee-female+, rillaboom+",,"+1 archaludon+, +1 rillaboom+, +1 indeedee-female+, +1 iron-crown=","+2 iron-crown=, +2 archaludon+, +2 indeedee-female+, +2 rillaboom+","+1 x2 indeedee-female+, +1 x2 rillaboom+, +1 x2 archaludon+, +1 x2 iron-crown="
-150,"-1 gholdengo+, -1 urshifu-single-strike=, -1 urshifu-rapid-strike=","urshifu-rapid-strike=, urshifu-single-strike=, gholdengo+","+1 dragonite=, -1 x2 urshifu-rapid-strike=, -1 x2 urshifu-single-strike=, -1 x2 gholdengo+","+2 incineroar=, +2 farigiraf=, +2 kingambit+, +1 urshifu-single-strike=, -1 x2 whimsicott=, -1 x2 landorus-incarnate+, +1 gholdengo+, +1 urshifu-rapid-strike=, +2 iron-hands+","+2 gholdengo+, +2 urshifu-single-strike=, +2 urshifu-rapid-strike=","+1 x2 urshifu-single-strike=, +1 x2 urshifu-rapid-strike=, +1 x2 gholdengo+"
-149,,"-1 x2 incineroar=, -1 x2 farigiraf=, -1 x2 iron-hands+, -1 x2 kingambit+",,"-1 x2 entei+, -1 x2 chi-yu+",,
-148,,,,-1 x2 iron-crown+,,
-146,"-1 dragonite+, -1 x2 torkoal=",dragonite+,-1 x2 dragonite+,+1 dragonite+,+2 dragonite+,+1 x2 dragonite+
-145,,+2 torkoal=,,"-1 x2 tornadus-incarnate=, +1 x2 torkoal=, -1 x2 urshifu-single-strike+, -1 x2 urshifu-rapid-strike+, -1 x2 ogerpon=",,
-144,-1 landorus-therian=,landorus-therian=,"-1 x2 landorus-therian=, +1 raging-bolt=","-1 x2 walking-wake=, +1 landorus-therian=",+2 landorus-therian=,+1 x2 landorus-therian=
-141,,,"flutter-mane=, chien-pao=",,"+1 flutter-mane=, +1 chien-pao=",
-140,-1 raging-bolt+,raging-bolt+,"+1 incineroar+, -1 x2 raging-bolt+, whimsicott+, +1 farigiraf+","-1 x2 landorus-therian+, +1 raging-bolt+",+2 raging-bolt+,+1 x2 raging-bolt+
+162,-1 ninetales-alola=,ninetales-alola=,"+1 gouging-fire=, -1 x2 ninetales-alola=",+1 ninetales-alola=,+2 ninetales-alola=,+1 x2 ninetales-alola=
+161,ting-lu+,,"+1 arcanine-hisui=, +2 ting-lu+",,,
+160,,+1 ting-lu+,,-1 x2 tornadus-incarnate+,+1 x2 ting-lu+,
+158,"-1 arcanine-hisui+, -1 gouging-fire+",gouging-fire+,"-1 x2 gouging-fire+, +1 raging-bolt+, -1 x2 arcanine-hisui+","+1 gouging-fire+, -1 x2 ogerpon+, -1 x2 ninetales-alola+",+2 gouging-fire+,+1 x2 gouging-fire+
+157,,arcanine-hisui+,,+1 arcanine-hisui+,+2 arcanine-hisui+,+1 x2 arcanine-hisui+
+155,-1 landorus-incarnate=,,"+1 articuno=, flutter-mane+, +1 rillaboom=, -1 x2 landorus-incarnate=, chien-pao+, +1 gholdengo=, +1 indeedee-female=",,,
+154,,landorus-incarnate=,,+1 landorus-incarnate=,"+2 landorus-incarnate=, +1 chien-pao+, +1 flutter-mane+",+1 x2 landorus-incarnate=
+153,-1 chi-yu=,chi-yu=,-1 x2 chi-yu=,+1 chi-yu=,+2 chi-yu=,+1 x2 chi-yu=
+152,"-1 rillaboom+, -1 articuno+, -1 indeedee-female+",,"-1 x2 indeedee-female+, -1 x2 rillaboom+, -1 x2 articuno+",,,
+151,,"articuno+, indeedee-female+, rillaboom+",,"+1 rillaboom+, +1 articuno+, +1 indeedee-female+","+2 articuno+, +2 indeedee-female+, +2 rillaboom+","+1 x2 articuno+, +1 x2 indeedee-female+, +1 x2 rillaboom+"
+150,"-1 urshifu-rapid-strike=, -1 urshifu-single-strike=, -1 gholdengo+","gholdengo+, urshifu-single-strike=, urshifu-rapid-strike=","+1 dragonite=, -1 x2 gholdengo+, -1 x2 urshifu-single-strike=, -1 x2 urshifu-rapid-strike=","+1 urshifu-single-strike=, +1 gholdengo+, +2 farigiraf=, -1 x2 whimsicott=, +2 incineroar=, +1 urshifu-rapid-strike=, +2 grimmsnarl=, -1 x2 landorus-incarnate+","+2 urshifu-rapid-strike=, +2 urshifu-single-strike=, +2 gholdengo+","+1 x2 urshifu-rapid-strike=, +1 x2 gholdengo+, +1 x2 urshifu-single-strike="
+149,,"-1 x2 farigiraf=, -1 x2 incineroar=, -1 x2 grimmsnarl=",,-1 x2 chi-yu+,,
+147,ting-lu=,,+2 ting-lu=,,,
+146,-1 dragonite+,"dragonite+, +1 ting-lu=",-1 x2 dragonite+,+1 dragonite+,"+2 dragonite+, +1 x2 ting-lu=",+1 x2 dragonite+
+145,,,,"-1 x2 urshifu-rapid-strike+, -1 x2 tornadus-incarnate=, -1 x2 urshifu-single-strike+, -1 x2 ogerpon=",,
+144,"dondozo+, -1 gouging-fire=",gouging-fire=,"+2 dondozo+, +1 raging-bolt=, -1 x2 gouging-fire=","+1 gouging-fire=, -1 x2 ninetales-alola=",+2 gouging-fire=,+1 x2 gouging-fire=
+143,-1 arcanine-hisui=,"arcanine-hisui=, +1 dondozo+",-1 x2 arcanine-hisui=,+1 arcanine-hisui=,"+2 arcanine-hisui=, +1 x2 dondozo+",+1 x2 arcanine-hisui=
+142,,,,+2 ting-lu+,,
+141,,-1 x2 ting-lu+,"flutter-mane=, chien-pao=",,"+1 flutter-mane=, +1 chien-pao=",
+140,-1 raging-bolt+,raging-bolt+,"whimsicott+, +1 grimmsnarl+, -1 x2 raging-bolt+, +1 farigiraf+, +1 incineroar+","-1 x2 gouging-fire+, +1 raging-bolt+, -1 x2 arcanine-hisui+",+2 raging-bolt+,+1 x2 raging-bolt+
 139,,,,,+1 whimsicott+,
-138,"-1 archaludon=, -1 rillaboom=, -1 indeedee-female=","rillaboom=, indeedee-female=, archaludon=","-1 x2 rillaboom=, -1 x2 indeedee-female=, -1 x2 archaludon=","+1 indeedee-female=, +1 archaludon=, flutter-mane+, chien-pao+, +1 rillaboom=","+2 archaludon=, +2 indeedee-female=, +2 rillaboom=","+1 x2 indeedee-female=, +2 flutter-mane+, +1 x2 rillaboom=, +2 chien-pao+, +1 x2 archaludon="
-137,"-1 gholdengo=, amoonguss+","-1 x2 iron-hands=, gholdengo=, -1 chien-pao+, -1 flutter-mane+, -1 x2 kingambit=","+2 amoonguss+, -1 x2 gholdengo=","+2 iron-hands=, +2 kingambit=, +1 gholdengo=, -1 x2 landorus-incarnate=","-1 x2 flutter-mane+, -1 x2 chien-pao+, +2 gholdengo=",+1 x2 gholdengo=
-136,,+1 amoonguss+,,"-1 x2 entei=, -1 x2 chi-yu=",+1 x2 amoonguss+,
-135,,,"tornadus-incarnate+, ogerpon+",,+1 tornadus-incarnate+,
-134,-1 dragonite=,,"-1 x2 dragonite=, walking-wake+","-1 x2 indeedee-female+, -1 x2 rillaboom+, -1 x2 iron-crown=, -1 x2 archaludon+",+1 ogerpon+,
-133,,dragonite=,,"+1 dragonite=, -1 x2 urshifu-rapid-strike=, -1 x2 urshifu-single-strike=, -1 x2 gholdengo+","+2 dragonite=, +1 walking-wake+",+1 x2 dragonite=
-129,,,,-1 x2 dragonite+,,
-128,-1 raging-bolt=,raging-bolt=,"-1 x2 raging-bolt=, whimsicott=, +1 iron-hands+, +1 incineroar=, landorus-incarnate+, +1 kingambit+, +1 farigiraf=","-1 x2 landorus-therian=, +1 raging-bolt=",+2 raging-bolt=,+1 x2 raging-bolt=
-127,,,,,"+1 landorus-incarnate+, +1 whimsicott=",
-126,,,"entei+, chi-yu+","flutter-mane=, chien-pao=","+1 chi-yu+, +1 entei+","+2 chien-pao=, +2 flutter-mane="
-125,"-1 incineroar+, -1 farigiraf+, amoonguss=","-1 flutter-mane=, -1 chien-pao=","-1 x2 farigiraf+, iron-crown+, +2 amoonguss=, -1 x2 incineroar+",,"-1 x2 flutter-mane=, -1 x2 chien-pao=",
-124,,"farigiraf+, +1 amoonguss=, incineroar+",,"+1 incineroar+, -1 x2 raging-bolt+, whimsicott+, +1 farigiraf+","+1 x2 amoonguss=, +1 iron-crown+, +2 incineroar+, +2 farigiraf+","+1 x2 incineroar+, +1 x2 farigiraf+, +2 whimsicott+"
-123,,-1 whimsicott+,"tornadus-incarnate=, urshifu-single-strike+, urshifu-rapid-strike+, ogerpon=",,"-1 x2 whimsicott+, +1 urshifu-rapid-strike+, +1 tornadus-incarnate=, +1 urshifu-single-strike+",
-122,,,walking-wake=,"-1 x2 rillaboom=, -1 x2 indeedee-female=, -1 x2 archaludon=",+1 ogerpon=,
-121,,-1 x2 amoonguss+,,"+2 amoonguss+, -1 x2 gholdengo=",+1 walking-wake=,
-120,torkoal+,-1 tornadus-incarnate+,+2 torkoal+,"tornadus-incarnate+, ogerpon+",-1 x2 tornadus-incarnate+,"+2 tornadus-incarnate+, +2 ogerpon+"
-119,,"+1 torkoal+, -1 walking-wake+, -1 ogerpon+",landorus-therian+,walking-wake+,"-1 x2 ogerpon+, +1 x2 torkoal+, -1 x2 walking-wake+",+2 walking-wake+
-118,,,,-1 x2 dragonite=,+1 landorus-therian+,
-116,,,"chi-yu=, +1 kingambit=, +1 iron-hands=, entei=, landorus-incarnate=",,,
-115,,,,,"+1 entei=, +1 landorus-incarnate=, +1 chi-yu=",
-114,,,"iron-crown=, archaludon+, indeedee-female+, rillaboom+",,,
-113,"-1 iron-hands+, -1 kingambit+, -1 incineroar=, -1 farigiraf=","-1 whimsicott=, incineroar=, farigiraf=, iron-hands+, kingambit+, -1 landorus-incarnate+","urshifu-rapid-strike=, -1 x2 incineroar=, -1 x2 farigiraf=, -1 x2 iron-hands+, -1 x2 kingambit+, urshifu-single-strike=, gholdengo+","-1 x2 raging-bolt=, whimsicott=, +1 iron-hands+, +1 incineroar=, landorus-incarnate+, +1 kingambit+, +1 farigiraf=","+2 incineroar=, +2 farigiraf=, +1 archaludon+, +2 kingambit+, +1 rillaboom+, -1 x2 whimsicott=, -1 x2 landorus-incarnate+, +2 iron-hands+, +1 indeedee-female+, +1 iron-crown=","+2 landorus-incarnate+, +2 whimsicott=, +1 x2 farigiraf=, +1 x2 incineroar=, +1 x2 iron-hands+, +1 x2 kingambit+"
-112,,"-1 chi-yu+, -1 entei+",,"entei+, chi-yu+","+1 urshifu-single-strike=, -1 x2 entei+, +1 gholdengo+, +1 urshifu-rapid-strike=, -1 x2 chi-yu+","+2 entei+, +2 chi-yu+"
-111,,-1 iron-crown+,,iron-crown+,-1 x2 iron-crown+,+2 iron-crown+
-110,torkoal=,,"+2 torkoal=, dragonite+","-1 x2 farigiraf+, tornadus-incarnate=, +2 amoonguss=, urshifu-single-strike+, -1 x2 incineroar+, urshifu-rapid-strike+",,"+2 urshifu-rapid-strike+, +2 urshifu-single-strike+, +2 tornadus-incarnate="
-109,,"-1 x2 amoonguss=, -1 urshifu-rapid-strike+, -1 urshifu-single-strike+, +1 torkoal=, -1 ogerpon=, -1 tornadus-incarnate=",,ogerpon=,"-1 x2 tornadus-incarnate=, +1 x2 torkoal=, -1 x2 urshifu-single-strike+, -1 x2 urshifu-rapid-strike+, +1 dragonite+, -1 x2 ogerpon=",+2 ogerpon=
-108,,-1 walking-wake=,landorus-therian=,walking-wake=,"-1 x2 walking-wake=, +1 landorus-therian=",+2 walking-wake=
-106,,,,"landorus-therian+, +2 torkoal+",,+2 landorus-therian+
-105,,"-1 x2 torkoal+, -1 landorus-therian+",raging-bolt+,,"-1 x2 landorus-therian+, +1 raging-bolt+",
-104,"-1 kingambit=, -1 iron-hands=",,"-1 x2 iron-hands=, rillaboom=, gholdengo=, -1 chien-pao+, -1 flutter-mane+, indeedee-female=, -1 x2 kingambit=, archaludon=",,,
-103,,"kingambit=, -1 landorus-incarnate=, iron-hands=",,"+1 kingambit=, +1 iron-hands=, landorus-incarnate=","+1 indeedee-female=, +2 iron-hands=, +1 archaludon=, flutter-mane+, chien-pao+, +2 kingambit=, +1 gholdengo=, -1 x2 landorus-incarnate=, +1 rillaboom=","+1 x2 iron-hands=, +1 x2 kingambit=, +1 chien-pao+, +2 landorus-incarnate=, +1 flutter-mane+"
-102,,"-1 chi-yu=, -1 entei=",+1 amoonguss+,"chi-yu=, entei=","-1 x2 entei=, -1 x2 chi-yu=","+2 entei=, +2 chi-yu="
-101,,"-1 iron-crown=, -1 rillaboom+, -1 indeedee-female+, -1 archaludon+",dragonite=,"iron-crown=, archaludon+, indeedee-female+, rillaboom+","-1 x2 indeedee-female+, -1 x2 rillaboom+, -1 x2 iron-crown=, -1 x2 archaludon+","+2 iron-crown=, +2 archaludon+, +2 indeedee-female+, +2 rillaboom+"
-100,,"-1 gholdengo+, -1 urshifu-single-strike=, -1 urshifu-rapid-strike=",,"urshifu-rapid-strike=, -1 x2 incineroar=, -1 x2 farigiraf=, -1 x2 iron-hands+, -1 x2 kingambit+, urshifu-single-strike=, gholdengo+","+1 dragonite=, -1 x2 urshifu-rapid-strike=, -1 x2 urshifu-single-strike=, -1 x2 gholdengo+","+2 gholdengo+, +2 urshifu-single-strike=, +2 urshifu-rapid-strike="
-98,,,,dragonite+,,+2 dragonite+
-97,,"-1 dragonite+, -1 x2 torkoal=",,+2 torkoal=,-1 x2 dragonite+,
-96,,-1 landorus-therian=,raging-bolt=,landorus-therian=,"-1 x2 landorus-therian=, +1 raging-bolt=",+2 landorus-therian=
-95,,,"-1 flutter-mane=, -1 chien-pao=",,,
-94,,,,raging-bolt+,"flutter-mane=, chien-pao=","+2 raging-bolt+, +1 flutter-mane=, +1 chien-pao="
-93,,-1 raging-bolt+,"farigiraf+, +1 amoonguss=, incineroar+, -1 whimsicott+",,"+1 incineroar+, -1 x2 raging-bolt+, whimsicott+, +1 farigiraf+",+1 whimsicott+
-92,-1 amoonguss+,"-1 archaludon=, -1 rillaboom=, -1 indeedee-female=",-1 x2 amoonguss+,"-1 x2 iron-hands=, rillaboom=, gholdengo=, -1 chien-pao+, -1 flutter-mane+, indeedee-female=, -1 x2 kingambit=, archaludon=","-1 x2 rillaboom=, -1 x2 indeedee-female=, -1 x2 archaludon=","-1 x2 flutter-mane+, +2 archaludon=, +2 indeedee-female=, -1 x2 chien-pao+, +2 gholdengo=, +2 rillaboom="
-91,,"-1 gholdengo=, amoonguss+",,+1 amoonguss+,"+2 amoonguss+, -1 x2 gholdengo=",+1 x2 amoonguss+
-90,,,"+1 torkoal+, -1 tornadus-incarnate+, -1 walking-wake+, -1 ogerpon+",,"tornadus-incarnate+, ogerpon+","+1 ogerpon+, +1 tornadus-incarnate+"
-89,,-1 dragonite=,,dragonite=,"-1 x2 dragonite=, walking-wake+","+2 dragonite=, +1 walking-wake+"
-86,,,"-1 whimsicott=, incineroar=, farigiraf=, iron-hands+, kingambit+, -1 landorus-incarnate+",raging-bolt=,,+2 raging-bolt=
-85,,-1 raging-bolt=,,,"-1 x2 raging-bolt=, whimsicott=, +1 iron-hands+, +1 incineroar=, landorus-incarnate+, +1 kingambit+, +1 farigiraf=","+1 landorus-incarnate+, +1 whimsicott="
-84,,,"-1 chi-yu+, -1 entei+, -1 iron-crown+","-1 flutter-mane=, -1 chien-pao=","entei+, chi-yu+","+1 chi-yu+, +1 entei+, -1 x2 flutter-mane=, -1 x2 chien-pao="
-83,-1 amoonguss=,"-1 incineroar+, -1 farigiraf+, amoonguss=","-1 x2 amoonguss=, -1 urshifu-rapid-strike+, -1 urshifu-single-strike+, +1 torkoal=, -1 ogerpon=, -1 tornadus-incarnate=","farigiraf+, +1 amoonguss=, incineroar+","-1 x2 farigiraf+, iron-crown+, +2 amoonguss=, -1 x2 incineroar+","+1 x2 amoonguss=, +1 iron-crown+, +2 incineroar+, +2 farigiraf+"
-82,,,,-1 whimsicott+,"tornadus-incarnate=, urshifu-single-strike+, urshifu-rapid-strike+, ogerpon=","-1 x2 whimsicott+, +1 urshifu-rapid-strike+, +1 ogerpon=, +1 tornadus-incarnate=, +1 urshifu-single-strike+"
-81,,,-1 walking-wake=,-1 x2 amoonguss+,walking-wake=,+1 walking-wake=
-80,-1 torkoal+,torkoal+,"-1 x2 torkoal+, -1 landorus-therian+","+1 torkoal+, -1 tornadus-incarnate+, -1 walking-wake+, -1 ogerpon+",+2 torkoal+,"-1 x2 ogerpon+, +1 x2 torkoal+, -1 x2 tornadus-incarnate+, -1 x2 walking-wake+"
-79,,,,,landorus-therian+,+1 landorus-therian+
-78,,,"kingambit=, -1 landorus-incarnate=, iron-hands=",,,
-77,,,"-1 iron-crown=, -1 rillaboom+, -1 indeedee-female+, -1 chi-yu=, -1 entei=, -1 archaludon+",,"chi-yu=, +1 kingambit=, +1 iron-hands=, entei=, landorus-incarnate=","+1 entei=, +1 landorus-incarnate=, +1 chi-yu="
-76,,,,"-1 whimsicott=, incineroar=, farigiraf=, iron-hands+, kingambit+, -1 landorus-incarnate+","iron-crown=, archaludon+, indeedee-female+, rillaboom+","+2 incineroar=, +2 farigiraf=, +1 archaludon+, +2 kingambit+, +1 rillaboom+, -1 x2 whimsicott=, -1 x2 landorus-incarnate+, +2 iron-hands+, +1 indeedee-female+, +1 iron-crown="
-75,,"-1 iron-hands+, -1 kingambit+, -1 incineroar=, -1 farigiraf=","-1 gholdengo+, -1 urshifu-single-strike=, -1 urshifu-rapid-strike=","-1 chi-yu+, -1 entei+","urshifu-rapid-strike=, -1 x2 incineroar=, -1 x2 farigiraf=, -1 x2 iron-hands+, -1 x2 kingambit+, urshifu-single-strike=, gholdengo+","+1 urshifu-single-strike=, -1 x2 entei+, +1 gholdengo+, +1 urshifu-rapid-strike=, -1 x2 chi-yu+"
-74,-1 torkoal=,,"-1 dragonite+, -1 x2 torkoal=",-1 iron-crown+,,-1 x2 iron-crown+
-73,,torkoal=,,"-1 x2 amoonguss=, -1 urshifu-rapid-strike+, -1 urshifu-single-strike+, +1 torkoal=, -1 ogerpon=, -1 tornadus-incarnate=","+2 torkoal=, dragonite+","-1 x2 tornadus-incarnate=, +1 x2 torkoal=, -1 x2 urshifu-single-strike+, -1 x2 urshifu-rapid-strike+, +1 dragonite+, -1 x2 ogerpon="
-72,,,-1 landorus-therian=,-1 walking-wake=,landorus-therian=,"-1 x2 walking-wake=, +1 landorus-therian="
-71,,,-1 raging-bolt+,,,
-70,,,,"-1 x2 torkoal+, -1 landorus-therian+",raging-bolt+,"-1 x2 landorus-therian+, +1 raging-bolt+"
-69,,"-1 kingambit=, -1 iron-hands=","-1 archaludon=, -1 gholdengo=, amoonguss+, -1 rillaboom=, -1 indeedee-female=","kingambit=, -1 landorus-incarnate=, iron-hands=","-1 x2 iron-hands=, rillaboom=, gholdengo=, -1 chien-pao+, -1 flutter-mane+, indeedee-female=, -1 x2 kingambit=, archaludon=","+1 indeedee-female=, +2 iron-hands=, +1 archaludon=, flutter-mane+, chien-pao+, +2 kingambit=, +1 gholdengo=, -1 x2 landorus-incarnate=, +1 rillaboom="
-68,,,-1 dragonite=,"-1 iron-crown=, -1 rillaboom+, -1 indeedee-female+, -1 chi-yu=, -1 entei=, -1 archaludon+",+1 amoonguss+,"-1 x2 indeedee-female+, -1 x2 rillaboom+, -1 x2 iron-crown=, -1 x2 archaludon+, -1 x2 entei=, -1 x2 chi-yu="
-67,,,,"-1 gholdengo+, -1 urshifu-single-strike=, -1 urshifu-rapid-strike=",dragonite=,"+1 dragonite=, -1 x2 urshifu-rapid-strike=, -1 x2 urshifu-single-strike=, -1 x2 gholdengo+"
-65,,,-1 raging-bolt=,"-1 dragonite+, -1 x2 torkoal=",,-1 x2 dragonite+
-64,,,,-1 landorus-therian=,raging-bolt=,"-1 x2 landorus-therian=, +1 raging-bolt="
-63,,,"-1 incineroar+, -1 farigiraf+, amoonguss=",,"-1 flutter-mane=, -1 chien-pao=","flutter-mane=, chien-pao="
-62,,,,"-1 archaludon=, -1 raging-bolt+, -1 rillaboom=, -1 indeedee-female=","farigiraf+, +1 amoonguss=, incineroar+, -1 whimsicott+","-1 x2 rillaboom=, +1 incineroar+, -1 x2 indeedee-female=, -1 x2 archaludon=, -1 x2 raging-bolt+, whimsicott+, +1 farigiraf+"
-61,,-1 amoonguss+,,"-1 gholdengo=, amoonguss+",-1 x2 amoonguss+,"+2 amoonguss+, -1 x2 gholdengo="
-60,,,torkoal+,-1 dragonite=,"+1 torkoal+, -1 tornadus-incarnate+, -1 walking-wake+, -1 ogerpon+","-1 x2 dragonite=, tornadus-incarnate+, walking-wake+, ogerpon+"
-57,,,"-1 iron-hands+, -1 kingambit+, -1 incineroar=, -1 farigiraf=",-1 raging-bolt=,"-1 whimsicott=, incineroar=, farigiraf=, iron-hands+, kingambit+, -1 landorus-incarnate+","-1 x2 raging-bolt=, whimsicott=, +1 iron-hands+, +1 incineroar=, landorus-incarnate+, +1 kingambit+, +1 farigiraf="
-56,,,torkoal=,"-1 incineroar+, -1 farigiraf+, amoonguss=","-1 chi-yu+, -1 entei+, -1 iron-crown+","entei+, -1 x2 farigiraf+, iron-crown+, +2 amoonguss=, -1 x2 incineroar+, chi-yu+"
-55,,-1 amoonguss=,,,"-1 x2 amoonguss=, -1 urshifu-rapid-strike+, -1 urshifu-single-strike+, +1 torkoal=, -1 ogerpon=, -1 tornadus-incarnate=","tornadus-incarnate=, urshifu-single-strike+, urshifu-rapid-strike+, ogerpon="
-54,,,,torkoal+,-1 walking-wake=,"walking-wake=, +2 torkoal+"
-53,,-1 torkoal+,"-1 kingambit=, -1 iron-hands=",,"-1 x2 torkoal+, -1 landorus-therian+",landorus-therian+
-52,,,,,"kingambit=, -1 landorus-incarnate=, iron-hands=","chi-yu=, +1 kingambit=, +1 iron-hands=, entei=, landorus-incarnate="
-51,,,,,"-1 iron-crown=, -1 rillaboom+, -1 indeedee-female+, -1 chi-yu=, -1 entei=, -1 archaludon+","iron-crown=, archaludon+, indeedee-female+, rillaboom+"
-50,,,,"-1 iron-hands+, -1 kingambit+, -1 incineroar=, -1 farigiraf=","-1 gholdengo+, -1 urshifu-single-strike=, -1 urshifu-rapid-strike=","urshifu-rapid-strike=, -1 x2 incineroar=, -1 x2 farigiraf=, -1 x2 iron-hands+, -1 x2 kingambit+, urshifu-single-strike=, gholdengo+"
-49,,-1 torkoal=,,torkoal=,"-1 dragonite+, -1 x2 torkoal=","+2 torkoal=, dragonite+"
-48,,,,,-1 landorus-therian=,landorus-therian=
+138,"-1 articuno=, -1 indeedee-female=, -1 rillaboom=","articuno=, indeedee-female=, rillaboom=","-1 x2 indeedee-female=, -1 x2 articuno=, -1 x2 rillaboom=","+1 articuno=, flutter-mane+, +1 rillaboom=, chien-pao+, +1 indeedee-female=","+2 indeedee-female=, +2 articuno=, +2 rillaboom=","+1 x2 indeedee-female=, +1 x2 rillaboom=, +1 x2 articuno=, +2 chien-pao+, +2 flutter-mane+"
+137,"-1 gholdengo=, amoonguss+","-1 flutter-mane+, -1 chien-pao+, gholdengo=","-1 x2 gholdengo=, +2 amoonguss+","-1 x2 landorus-incarnate=, +1 gholdengo=","-1 x2 chien-pao+, +2 gholdengo=, -1 x2 flutter-mane+",+1 x2 gholdengo=
+136,,+1 amoonguss+,,-1 x2 chi-yu=,+1 x2 amoonguss+,
+135,,,"ogerpon+, tornadus-incarnate+",,+1 tornadus-incarnate+,
+134,-1 dragonite=,,"-1 x2 dragonite=, ninetales-alola+","-1 x2 indeedee-female+, -1 x2 rillaboom+, -1 x2 articuno+",+1 ogerpon+,
+133,,dragonite=,,"+1 dragonite=, -1 x2 gholdengo+, -1 x2 urshifu-single-strike=, -1 x2 urshifu-rapid-strike=","+1 ninetales-alola+, +2 dragonite=",+1 x2 dragonite=
+132,dondozo=,,+2 dondozo=,,,
+131,,+1 dondozo=,,,+1 x2 dondozo=,
+130,,,,+2 ting-lu=,,
+129,,-1 x2 ting-lu=,,-1 x2 dragonite+,,
+128,-1 raging-bolt=,raging-bolt=,"+1 farigiraf=, whimsicott=, landorus-incarnate+, +1 incineroar=, -1 x2 raging-bolt=, +1 grimmsnarl=","+2 dondozo+, +1 raging-bolt=, -1 x2 gouging-fire=",+2 raging-bolt=,+1 x2 raging-bolt=
+127,,-1 x2 dondozo+,,,"+1 landorus-incarnate+, +1 whimsicott=",
+126,,,chi-yu+,"-1 x2 arcanine-hisui=, flutter-mane=, chien-pao=",+1 chi-yu+,"+2 flutter-mane=, +2 chien-pao="
+125,"-1 incineroar+, -1 farigiraf+, -1 grimmsnarl+, amoonguss=","-1 flutter-mane=, -1 chien-pao=","-1 x2 farigiraf+, -1 x2 incineroar+, -1 x2 grimmsnarl+, +2 amoonguss=",,"-1 x2 flutter-mane=, -1 x2 chien-pao=",
+124,,"incineroar+, farigiraf+, grimmsnarl+, +1 amoonguss=",,"whimsicott+, +1 grimmsnarl+, -1 x2 raging-bolt+, +1 farigiraf+, +1 incineroar+","+2 incineroar+, +2 farigiraf+, +2 grimmsnarl+, +1 x2 amoonguss=","+2 whimsicott+, +1 x2 farigiraf+, +1 x2 grimmsnarl+, +1 x2 incineroar+"
+123,,-1 whimsicott+,"tornadus-incarnate=, urshifu-rapid-strike+, ogerpon=, urshifu-single-strike+",,"-1 x2 whimsicott+, +1 urshifu-single-strike+, +1 tornadus-incarnate=, +1 urshifu-rapid-strike+",
+122,,,ninetales-alola=,"-1 x2 indeedee-female=, -1 x2 articuno=, -1 x2 rillaboom=",+1 ogerpon=,
+121,,-1 x2 amoonguss+,,"-1 x2 gholdengo=, +2 amoonguss+",+1 ninetales-alola=,
+120,,-1 tornadus-incarnate+,+1 ting-lu+,"ogerpon+, tornadus-incarnate+",-1 x2 tornadus-incarnate+,"+2 tornadus-incarnate+, +2 ogerpon+"
+119,,"-1 ogerpon+, -1 ninetales-alola+","gouging-fire+, arcanine-hisui+",ninetales-alola+,"-1 x2 ogerpon+, -1 x2 ninetales-alola+",+2 ninetales-alola+
+118,,,,-1 x2 dragonite=,"+1 arcanine-hisui+, +1 gouging-fire+",
+117,,-1 x2 dondozo=,,+2 dondozo=,,
+116,,,"chi-yu=, landorus-incarnate=",,,
+115,,,,,"+1 landorus-incarnate=, +1 chi-yu=",
+114,,,"articuno+, indeedee-female+, rillaboom+",,,
+113,"-1 farigiraf=, -1 grimmsnarl=, -1 incineroar=","farigiraf=, -1 whimsicott=, incineroar=, grimmsnarl=, -1 landorus-incarnate+","-1 x2 farigiraf=, -1 x2 incineroar=, -1 x2 grimmsnarl=, gholdengo+, urshifu-single-strike=, urshifu-rapid-strike=","+1 farigiraf=, whimsicott=, landorus-incarnate+, +1 incineroar=, -1 x2 raging-bolt=, +1 grimmsnarl=","+1 rillaboom+, +2 farigiraf=, -1 x2 whimsicott=, +1 articuno+, +2 incineroar=, +2 grimmsnarl=, -1 x2 landorus-incarnate+, +1 indeedee-female+","+2 landorus-incarnate+, +1 x2 farigiraf=, +1 x2 incineroar=, +2 whimsicott=, +1 x2 grimmsnarl="
+112,,-1 chi-yu+,,chi-yu+,"+1 urshifu-single-strike=, +1 gholdengo+, -1 x2 chi-yu+, +1 urshifu-rapid-strike=",+2 chi-yu+
+110,,,"dragonite+, +1 ting-lu=","-1 x2 farigiraf+, tornadus-incarnate=, urshifu-rapid-strike+, -1 x2 incineroar+, -1 x2 grimmsnarl+, urshifu-single-strike+, +2 amoonguss=",,"+2 tornadus-incarnate=, +2 urshifu-rapid-strike+, +2 urshifu-single-strike+"
+109,,"-1 urshifu-single-strike+, -1 urshifu-rapid-strike+, -1 x2 amoonguss=, -1 ogerpon=, -1 tornadus-incarnate=",,ogerpon=,"-1 x2 urshifu-rapid-strike+, +1 dragonite+, -1 x2 tornadus-incarnate=, -1 x2 urshifu-single-strike+, -1 x2 ogerpon=",+2 ogerpon=
+108,,-1 ninetales-alola=,"arcanine-hisui=, gouging-fire=, +1 dondozo+",ninetales-alola=,"+1 gouging-fire=, -1 x2 ninetales-alola=",+2 ninetales-alola=
+107,-1 ting-lu+,ting-lu+,-1 x2 ting-lu+,+1 ting-lu+,"+1 arcanine-hisui=, +2 ting-lu+",+1 x2 ting-lu+
+106,,,,gouging-fire+,,+2 gouging-fire+
+105,,"-1 arcanine-hisui+, -1 gouging-fire+",raging-bolt+,arcanine-hisui+,"-1 x2 gouging-fire+, +1 raging-bolt+, -1 x2 arcanine-hisui+",+2 arcanine-hisui+
+104,,,"-1 flutter-mane+, -1 chien-pao+, articuno=, indeedee-female=, rillaboom=, gholdengo=",,,
+103,,-1 landorus-incarnate=,,landorus-incarnate=,"+1 articuno=, flutter-mane+, +1 rillaboom=, -1 x2 landorus-incarnate=, chien-pao+, +1 gholdengo=, +1 indeedee-female=","+2 landorus-incarnate=, +1 chien-pao+, +1 flutter-mane+"
+102,,-1 chi-yu=,+1 amoonguss+,chi-yu=,-1 x2 chi-yu=,+2 chi-yu=
+101,,"-1 rillaboom+, -1 articuno+, -1 indeedee-female+",dragonite=,"articuno+, indeedee-female+, rillaboom+","-1 x2 indeedee-female+, -1 x2 rillaboom+, -1 x2 articuno+","+2 articuno+, +2 indeedee-female+, +2 rillaboom+"
+100,,"-1 urshifu-rapid-strike=, -1 urshifu-single-strike=, -1 gholdengo+",,"-1 x2 farigiraf=, -1 x2 incineroar=, -1 x2 grimmsnarl=, gholdengo+, urshifu-single-strike=, urshifu-rapid-strike=","+1 dragonite=, -1 x2 gholdengo+, -1 x2 urshifu-single-strike=, -1 x2 urshifu-rapid-strike=","+2 urshifu-rapid-strike=, +2 urshifu-single-strike=, +2 gholdengo+"
+99,,,+1 dondozo=,,,
+98,-1 ting-lu=,ting-lu=,-1 x2 ting-lu=,"dragonite+, +1 ting-lu=",+2 ting-lu=,"+2 dragonite+, +1 x2 ting-lu="
+97,,-1 dragonite+,,,-1 x2 dragonite+,
+96,-1 dondozo+,"dondozo+, -1 gouging-fire=","-1 x2 dondozo+, raging-bolt=","arcanine-hisui=, gouging-fire=, +1 dondozo+","+2 dondozo+, +1 raging-bolt=, -1 x2 gouging-fire=","+2 arcanine-hisui=, +1 x2 dondozo+, +2 gouging-fire="
+95,,-1 arcanine-hisui=,"-1 flutter-mane=, -1 chien-pao=",,-1 x2 arcanine-hisui=,
+94,,,,"-1 x2 ting-lu+, raging-bolt+","flutter-mane=, chien-pao=","+2 raging-bolt+, +1 flutter-mane=, +1 chien-pao="
+93,,-1 raging-bolt+,"incineroar+, farigiraf+, -1 whimsicott+, grimmsnarl+, +1 amoonguss=",,"whimsicott+, +1 grimmsnarl+, -1 x2 raging-bolt+, +1 farigiraf+, +1 incineroar+",+1 whimsicott+
+92,-1 amoonguss+,"-1 articuno=, -1 indeedee-female=, -1 rillaboom=",-1 x2 amoonguss+,"-1 flutter-mane+, -1 chien-pao+, articuno=, indeedee-female=, rillaboom=, gholdengo=","-1 x2 indeedee-female=, -1 x2 articuno=, -1 x2 rillaboom=","+2 indeedee-female=, -1 x2 chien-pao+, +2 articuno=, +2 gholdengo=, +2 rillaboom=, -1 x2 flutter-mane+"
+91,,"-1 gholdengo=, amoonguss+",,+1 amoonguss+,"-1 x2 gholdengo=, +2 amoonguss+",+1 x2 amoonguss+
+90,,,"-1 ogerpon+, -1 tornadus-incarnate+, -1 ninetales-alola+",,"ogerpon+, tornadus-incarnate+","+1 tornadus-incarnate+, +1 ogerpon+"
+89,-1 dondozo=,-1 dragonite=,-1 x2 dondozo=,dragonite=,"-1 x2 dragonite=, ninetales-alola+","+1 ninetales-alola+, +2 dragonite="
+88,,dondozo=,,+1 dondozo=,+2 dondozo=,+1 x2 dondozo=
+86,,,"farigiraf=, -1 whimsicott=, incineroar=, grimmsnarl=, -1 landorus-incarnate+","raging-bolt=, -1 x2 ting-lu=",,+2 raging-bolt=
+85,,-1 raging-bolt=,,-1 x2 dondozo+,"+1 farigiraf=, whimsicott=, landorus-incarnate+, +1 incineroar=, -1 x2 raging-bolt=, +1 grimmsnarl=","+1 landorus-incarnate+, +1 whimsicott="
+84,,,-1 chi-yu+,"-1 flutter-mane=, -1 chien-pao=",chi-yu+,"+1 chi-yu+, -1 x2 flutter-mane=, -1 x2 chien-pao="
+83,-1 amoonguss=,"-1 incineroar+, -1 farigiraf+, -1 grimmsnarl+, amoonguss=","-1 urshifu-single-strike+, -1 urshifu-rapid-strike+, -1 x2 amoonguss=, -1 ogerpon=, -1 tornadus-incarnate=","incineroar+, farigiraf+, grimmsnarl+, +1 amoonguss=","-1 x2 farigiraf+, -1 x2 incineroar+, -1 x2 grimmsnarl+, +2 amoonguss=","+2 incineroar+, +2 farigiraf+, +2 grimmsnarl+, +1 x2 amoonguss="
+82,,,,-1 whimsicott+,"tornadus-incarnate=, urshifu-rapid-strike+, ogerpon=, urshifu-single-strike+","-1 x2 whimsicott+, +1 urshifu-single-strike+, +1 ogerpon=, +1 tornadus-incarnate=, +1 urshifu-rapid-strike+"
+81,,,"ting-lu+, -1 ninetales-alola=",-1 x2 amoonguss+,ninetales-alola=,+1 ninetales-alola=
+80,,,"-1 arcanine-hisui+, -1 gouging-fire+","-1 ogerpon+, -1 tornadus-incarnate+, -1 ninetales-alola+",+1 ting-lu+,"-1 x2 ogerpon+, -1 x2 tornadus-incarnate+, -1 x2 ninetales-alola+"
+79,,,,,"gouging-fire+, arcanine-hisui+","+1 arcanine-hisui+, +1 gouging-fire+"
+78,,,-1 landorus-incarnate=,-1 x2 dondozo=,,
+77,,,"-1 rillaboom+, -1 articuno+, -1 indeedee-female+, -1 chi-yu=",,"chi-yu=, landorus-incarnate=","+1 landorus-incarnate=, +1 chi-yu="
+76,,,,"farigiraf=, -1 whimsicott=, incineroar=, grimmsnarl=, -1 landorus-incarnate+","articuno+, indeedee-female+, rillaboom+","+1 rillaboom+, +2 farigiraf=, -1 x2 whimsicott=, +1 articuno+, +2 incineroar=, +2 grimmsnarl=, -1 x2 landorus-incarnate+, +1 indeedee-female+"
+75,,"-1 farigiraf=, -1 grimmsnarl=, -1 incineroar=","-1 urshifu-rapid-strike=, -1 urshifu-single-strike=, -1 gholdengo+",-1 chi-yu+,"-1 x2 farigiraf=, -1 x2 incineroar=, -1 x2 grimmsnarl=, gholdengo+, urshifu-single-strike=, urshifu-rapid-strike=","+1 urshifu-single-strike=, +1 gholdengo+, -1 x2 chi-yu+, +1 urshifu-rapid-strike="
+74,,,"-1 dragonite+, ting-lu=",,,
+73,,,,"-1 urshifu-single-strike+, -1 urshifu-rapid-strike+, -1 x2 amoonguss=, -1 ogerpon=, -1 tornadus-incarnate=","dragonite+, +1 ting-lu=","-1 x2 urshifu-rapid-strike+, +1 dragonite+, -1 x2 tornadus-incarnate=, -1 x2 urshifu-single-strike+, -1 x2 ogerpon="
+72,,,"dondozo+, -1 gouging-fire=, -1 arcanine-hisui=","ting-lu+, -1 ninetales-alola=","arcanine-hisui=, gouging-fire=, +1 dondozo+","+1 arcanine-hisui=, +2 ting-lu+, +1 gouging-fire=, -1 x2 ninetales-alola="
+71,,-1 ting-lu+,-1 raging-bolt+,,-1 x2 ting-lu+,
+70,,,,"-1 arcanine-hisui+, -1 gouging-fire+",raging-bolt+,"-1 x2 gouging-fire+, +1 raging-bolt+, -1 x2 arcanine-hisui+"
+69,,,"-1 gholdengo=, -1 articuno=, -1 indeedee-female=, -1 rillaboom=, amoonguss+",-1 landorus-incarnate=,"-1 flutter-mane+, -1 chien-pao+, articuno=, indeedee-female=, rillaboom=, gholdengo=","+1 articuno=, flutter-mane+, +1 rillaboom=, -1 x2 landorus-incarnate=, chien-pao+, +1 gholdengo=, +1 indeedee-female="
+68,,,-1 dragonite=,"-1 rillaboom+, -1 articuno+, -1 indeedee-female+, -1 chi-yu=",+1 amoonguss+,"-1 x2 chi-yu=, -1 x2 indeedee-female+, -1 x2 rillaboom+, -1 x2 articuno+"
+67,,,,"-1 urshifu-rapid-strike=, -1 urshifu-single-strike=, -1 gholdengo+",dragonite=,"+1 dragonite=, -1 x2 gholdengo+, -1 x2 urshifu-single-strike=, -1 x2 urshifu-rapid-strike="
+66,,,dondozo=,ting-lu=,+1 dondozo=,+2 ting-lu=
+65,,-1 ting-lu=,-1 raging-bolt=,-1 dragonite+,-1 x2 ting-lu=,-1 x2 dragonite+
+64,,-1 dondozo+,,"dondozo+, -1 gouging-fire=, -1 arcanine-hisui=","-1 x2 dondozo+, raging-bolt=","+2 dondozo+, -1 x2 arcanine-hisui=, +1 raging-bolt=, -1 x2 gouging-fire="
+63,,,"-1 incineroar+, -1 farigiraf+, -1 grimmsnarl+, amoonguss=",,"-1 flutter-mane=, -1 chien-pao=","flutter-mane=, chien-pao="
+62,,,,"-1 articuno=, -1 raging-bolt+, -1 indeedee-female=, -1 rillaboom=","incineroar+, farigiraf+, -1 whimsicott+, grimmsnarl+, +1 amoonguss=","-1 x2 indeedee-female=, whimsicott+, -1 x2 articuno=, +1 grimmsnarl+, -1 x2 raging-bolt+, -1 x2 rillaboom=, +1 farigiraf+, +1 incineroar+"
+61,,-1 amoonguss+,,"-1 gholdengo=, amoonguss+",-1 x2 amoonguss+,"-1 x2 gholdengo=, +2 amoonguss+"
+60,,,,-1 dragonite=,"-1 ogerpon+, -1 tornadus-incarnate+, -1 ninetales-alola+","-1 x2 dragonite=, ogerpon+, ninetales-alola+, tornadus-incarnate+"
+59,,-1 dondozo=,,dondozo=,-1 x2 dondozo=,+2 dondozo=
+57,,,"-1 farigiraf=, -1 grimmsnarl=, -1 incineroar=",-1 raging-bolt=,"farigiraf=, -1 whimsicott=, incineroar=, grimmsnarl=, -1 landorus-incarnate+","+1 farigiraf=, whimsicott=, landorus-incarnate+, +1 incineroar=, -1 x2 raging-bolt=, +1 grimmsnarl="
+56,,,,"-1 incineroar+, -1 farigiraf+, -1 grimmsnarl+, amoonguss=",-1 chi-yu+,"-1 x2 farigiraf+, chi-yu+, -1 x2 incineroar+, -1 x2 grimmsnarl+, +2 amoonguss="
+55,,-1 amoonguss=,,,"-1 urshifu-single-strike+, -1 urshifu-rapid-strike+, -1 x2 amoonguss=, -1 ogerpon=, -1 tornadus-incarnate=","tornadus-incarnate=, urshifu-rapid-strike+, ogerpon=, urshifu-single-strike+"
+54,,,-1 ting-lu+,,"ting-lu+, -1 ninetales-alola=","+1 ting-lu+, ninetales-alola="
+53,,,,,"-1 arcanine-hisui+, -1 gouging-fire+","gouging-fire+, arcanine-hisui+"
+52,,,,,-1 landorus-incarnate=,"chi-yu=, landorus-incarnate="
+51,,,,,"-1 rillaboom+, -1 articuno+, -1 indeedee-female+, -1 chi-yu=","articuno+, indeedee-female+, rillaboom+"
+50,,,-1 ting-lu=,"-1 farigiraf=, -1 grimmsnarl=, -1 incineroar=","-1 urshifu-rapid-strike=, -1 urshifu-single-strike=, -1 gholdengo+","-1 x2 farigiraf=, -1 x2 incineroar=, -1 x2 grimmsnarl=, gholdengo+, urshifu-single-strike=, urshifu-rapid-strike="
+49,,,,,"-1 dragonite+, ting-lu=","dragonite+, +1 ting-lu="
+48,,,-1 dondozo+,-1 ting-lu+,"dondozo+, -1 gouging-fire=, -1 arcanine-hisui=","-1 x2 ting-lu+, arcanine-hisui=, gouging-fire=, +1 dondozo+"
 47,,,-1 amoonguss+,,-1 raging-bolt+,raging-bolt+
-46,,,,"-1 kingambit=, -1 iron-hands=","-1 archaludon=, -1 gholdengo=, amoonguss+, -1 rillaboom=, -1 indeedee-female=","-1 x2 iron-hands=, +1 amoonguss+, rillaboom=, gholdengo=, -1 chien-pao+, -1 flutter-mane+, indeedee-female=, -1 x2 kingambit=, archaludon="
-45,,,,,-1 dragonite=,dragonite=
-43,,,,,-1 raging-bolt=,raging-bolt=
-42,,,-1 amoonguss=,,"-1 incineroar+, -1 farigiraf+, amoonguss=","farigiraf+, -1 flutter-mane=, +1 amoonguss=, incineroar+, -1 whimsicott+, -1 chien-pao="
-41,,,-1 torkoal+,-1 amoonguss+,,-1 x2 amoonguss+
-40,,,,,torkoal+,"+1 torkoal+, -1 tornadus-incarnate+, -1 walking-wake+, -1 ogerpon+"
-38,,,-1 torkoal=,,"-1 iron-hands+, -1 kingambit+, -1 incineroar=, -1 farigiraf=","-1 whimsicott=, incineroar=, farigiraf=, iron-hands+, -1 chi-yu+, kingambit+, -1 entei+, -1 landorus-incarnate+, -1 iron-crown+"
-37,,,,-1 amoonguss=,torkoal=,"-1 x2 amoonguss=, -1 urshifu-rapid-strike+, -1 urshifu-single-strike+, +1 torkoal=, -1 ogerpon=, -1 tornadus-incarnate="
-36,,,,-1 torkoal+,,"-1 walking-wake=, -1 x2 torkoal+, -1 landorus-therian+"
-35,,,,,"-1 kingambit=, -1 iron-hands=","kingambit=, -1 landorus-incarnate=, iron-hands="
-34,,,,,,"-1 gholdengo+, -1 iron-crown=, -1 rillaboom+, -1 indeedee-female+, -1 urshifu-single-strike=, -1 urshifu-rapid-strike=, -1 chi-yu=, -1 entei=, -1 archaludon+"
-33,,,,-1 torkoal=,,"-1 dragonite+, -1 x2 torkoal="
-32,,,,,,"-1 landorus-therian=, -1 raging-bolt+"
-31,,,,,-1 amoonguss+,"-1 archaludon=, -1 gholdengo=, amoonguss+, -1 rillaboom=, -1 indeedee-female="
-30,,,,,,-1 dragonite=
+46,,,,,"-1 gholdengo=, -1 articuno=, -1 indeedee-female=, -1 rillaboom=, amoonguss+","-1 flutter-mane+, +1 amoonguss+, -1 chien-pao+, articuno=, indeedee-female=, rillaboom=, gholdengo="
+45,,,-1 dondozo=,,-1 dragonite=,dragonite=
+44,,,,-1 ting-lu=,dondozo=,"+1 dondozo=, -1 x2 ting-lu="
+43,,,,-1 dondozo+,-1 raging-bolt=,"-1 x2 dondozo+, raging-bolt="
+42,,,-1 amoonguss=,,"-1 incineroar+, -1 farigiraf+, -1 grimmsnarl+, amoonguss=","incineroar+, farigiraf+, -1 flutter-mane=, -1 chien-pao=, -1 whimsicott+, grimmsnarl+, +1 amoonguss="
+41,,,,-1 amoonguss+,,-1 x2 amoonguss+
+40,,,,-1 dondozo=,,"-1 x2 dondozo=, -1 ogerpon+, -1 tornadus-incarnate+, -1 ninetales-alola+"
+38,,,,,"-1 farigiraf=, -1 grimmsnarl=, -1 incineroar=","farigiraf=, -1 whimsicott=, incineroar=, grimmsnarl=, -1 chi-yu+, -1 landorus-incarnate+"
+37,,,,-1 amoonguss=,,"-1 urshifu-single-strike+, -1 urshifu-rapid-strike+, -1 x2 amoonguss=, -1 ogerpon=, -1 tornadus-incarnate="
+36,,,,,-1 ting-lu+,"ting-lu+, -1 arcanine-hisui+, -1 gouging-fire+, -1 ninetales-alola="
+35,,,,,,-1 landorus-incarnate=
+34,,,,,,"-1 urshifu-rapid-strike=, -1 rillaboom+, -1 urshifu-single-strike=, -1 gholdengo+, -1 articuno+, -1 indeedee-female+, -1 chi-yu="
+33,,,,,-1 ting-lu=,"-1 dragonite+, ting-lu="
+32,,,,,-1 dondozo+,"dondozo+, -1 raging-bolt+, -1 gouging-fire=, -1 arcanine-hisui="
+31,,,,,-1 amoonguss+,"-1 gholdengo=, -1 articuno=, -1 indeedee-female=, -1 rillaboom=, amoonguss+"
+30,,,,,-1 dondozo=,"-1 dragonite=, dondozo="
 29,,,,,,-1 raging-bolt=
-28,,,,,-1 amoonguss=,"-1 incineroar+, -1 farigiraf+, amoonguss="
-27,,,,,-1 torkoal+,torkoal+
-26,,,,,,"-1 iron-hands+, -1 kingambit+, -1 incineroar=, -1 farigiraf="
-25,,,,,-1 torkoal=,torkoal=
-24,,,,,,"-1 kingambit=, -1 iron-hands="
+28,,,,,-1 amoonguss=,"-1 incineroar+, -1 farigiraf+, -1 grimmsnarl+, amoonguss="
+26,,,,,,"-1 farigiraf=, -1 grimmsnarl=, -1 incineroar="
+24,,,,,,-1 ting-lu+
+22,,,,,,"-1 ting-lu=, -1 dondozo+"
 21,,,,,,-1 amoonguss+
+20,,,,,,-1 dondozo=
 19,,,,,,-1 amoonguss=
-18,,,,,,-1 torkoal+
-17,,,,,,-1 torkoal=
```

### Comparing `pokespeed-1.0.1/pokespeed/__coconut__.py` & `pokespeed-1.1.0/pokespeed/__coconut__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # type: ignore
 
-# Compiled with Coconut version 3.0.4-post_dev17
+# Compiled with Coconut version 3.1.0-post_dev13
 
 """Built-in Coconut utilities."""
 
 # Coconut Header: -------------------------------------------------------------
 
 import sys as _coconut_sys
 import os as _coconut_os
-_coconut_header_info = ('3.0.4-post_dev17', '3', True)
+_coconut_header_info = ('3.1.0-post_dev13', '3', True)
 try:
     __file__ = _coconut_os.path.abspath(__file__) if __file__ else __file__
 except NameError:
     pass
 else:
     if __file__ and '__coconut_cache__' in __file__:
         _coconut_file_comps = []
@@ -24,19 +24,43 @@
                 _coconut_file_comps.append(__file__)
                 break
             if _coconut_file_comp != '__coconut_cache__':
                 _coconut_file_comps.append(_coconut_file_comp)
         __file__ = _coconut_os.path.join(*reversed(_coconut_file_comps))
 _coconut_cached__coconut__ = _coconut_sys.modules.get('_coconut_cached__coconut__', _coconut_sys.modules.get('__coconut__'))
 from builtins import chr, dict, hex, input, int, map, object, oct, open, print, range, str, super, zip, filter, reversed, enumerate, repr
-py_chr, py_dict, py_hex, py_input, py_int, py_map, py_object, py_oct, py_open, py_print, py_range, py_str, py_super, py_zip, py_filter, py_reversed, py_enumerate, py_repr = chr, dict, hex, input, int, map, object, oct, open, print, range, str, super, zip, filter, reversed, enumerate, repr
-_coconut_py_str, _coconut_py_super, _coconut_py_dict = str, super, dict
+py_bytes, py_chr, py_dict, py_hex, py_input, py_int, py_map, py_object, py_oct, py_open, py_print, py_range, py_str, py_super, py_zip, py_filter, py_reversed, py_enumerate, py_repr, py_min, py_max = bytes, chr, dict, hex, input, int, map, object, oct, open, print, range, str, super, zip, filter, reversed, enumerate, repr, min, max
+_coconut_py_str, _coconut_py_super, _coconut_py_dict, _coconut_py_min, _coconut_py_max = str, super, dict, min, max
 from functools import wraps as _coconut_wraps
 exec("_coconut_exec = exec")
+if _coconut_sys.version_info >= (3, 7):
+    py_breakpoint = breakpoint
+if _coconut_sys.version_info < (3, 4):
+    def min(*args, **kwargs):
+        if len(args) == 1 and "default" in kwargs:
+            obj = tuple(args[0])
+            default = kwargs.pop("default")
+            if len(obj):
+                return _coconut_py_min(obj, **kwargs)
+            else:
+                return default
+        else:
+            return _coconut_py_min(*args, **kwargs)
+    def max(*args, **kwargs):
+        if len(args) == 1 and "default" in kwargs:
+            obj = tuple(args[0])
+            default = kwargs.pop("default")
+            if len(obj):
+                return _coconut_py_max(obj, **kwargs)
+            else:
+                return default
+        else:
+            return _coconut_py_max(*args, **kwargs)
 if _coconut_sys.version_info < (3, 7):
+    from collections import OrderedDict as _coconut_OrderedDict
     def _coconut_default_breakpointhook(*args, **kwargs):
         hookname = _coconut.os.getenv("PYTHONBREAKPOINT")
         if hookname != "0":
             if not hookname:
                 hookname = "pdb.set_trace"
             modname, dot, funcname = hookname.rpartition(".")
             if not dot:
@@ -49,18 +73,14 @@
                 module = imp.load_module(modname, *imp.find_module(modname))
             hook = _coconut.getattr(module, funcname)
             return hook(*args, **kwargs)
     if not hasattr(_coconut_sys, "__breakpointhook__"):
         _coconut_sys.__breakpointhook__ = _coconut_default_breakpointhook
     def breakpoint(*args, **kwargs):
         return _coconut.getattr(_coconut_sys, "breakpointhook", _coconut_default_breakpointhook)(*args, **kwargs)
-else:
-    py_breakpoint = breakpoint
-if _coconut_sys.version_info < (3, 7):
-    from collections import OrderedDict as _coconut_OrderedDict
     class _coconut_dict_base(_coconut_OrderedDict):
         __slots__ = ()
         __doc__ = getattr(_coconut_OrderedDict, "__doc__", "<see help(py_dict)>")
         __eq__ = _coconut_py_dict.__eq__
         def __repr__(self):
             return "{" + ", ".join("{k!r}: {v!r}".format(k=k, v=v) for k, v in self.items()) + "}"
         def __or__(self, other):
@@ -239,23 +259,23 @@
     zip_longest = itertools.zip_longest
     try:
         import numpy
     except ImportError as numpy_import_err:
         numpy = _coconut_missing_module(numpy_import_err)
     else:
         abc.Sequence.register(numpy.ndarray)
-    numpy_modules = ('numpy', 'torch', 'xarray', 'pandas', 'jaxlib')
+    numpy_modules = ('numpy', 'torch', 'jaxlib', 'pandas', 'xarray')
     xarray_modules = ('xarray',)
     pandas_modules = ('pandas',)
     jax_numpy_modules = ('jaxlib',)
     tee_type = type(itertools.tee((), 1)[0])
     reiterables = abc.Sequence, abc.Mapping, abc.Set
-    fmappables = list, tuple, dict, set, frozenset
+    fmappables = list, tuple, dict, set, frozenset, bytes, bytearray
     abc.Sequence.register(collections.deque)
-    Ellipsis, NotImplemented, NotImplementedError, Exception, AttributeError, ImportError, IndexError, KeyError, NameError, TypeError, ValueError, StopIteration, RuntimeError, all, any, bool, bytes, callable, classmethod, complex, dict, enumerate, filter, float, frozenset, getattr, hasattr, hash, id, int, isinstance, issubclass, iter, len, list, locals, globals, map, min, max, next, object, property, range, reversed, set, setattr, slice, str, sum, super, tuple, type, vars, zip, repr, print = Ellipsis, NotImplemented, NotImplementedError, Exception, AttributeError, ImportError, IndexError, KeyError, NameError, TypeError, ValueError, StopIteration, RuntimeError, all, any, bool, bytes, callable, classmethod, complex, dict, enumerate, filter, float, frozenset, getattr, hasattr, hash, id, int, isinstance, issubclass, iter, len, list, locals, globals, map, min, max, next, object, property, range, reversed, set, setattr, slice, str, sum, super, tuple, type, vars, zip, repr, print
+    Ellipsis, NotImplemented, NotImplementedError, Exception, AttributeError, ImportError, IndexError, KeyError, NameError, TypeError, ValueError, StopIteration, RuntimeError, all, any, bool, bytes, callable, chr, classmethod, complex, dict, enumerate, filter, float, frozenset, getattr, hasattr, hash, id, int, isinstance, issubclass, iter, len, list, locals, globals, map, min, max, next, object, ord, property, range, reversed, set, setattr, slice, str, sum, super, tuple, type, vars, zip, repr, print = Ellipsis, NotImplemented, NotImplementedError, Exception, AttributeError, ImportError, IndexError, KeyError, NameError, TypeError, ValueError, StopIteration, RuntimeError, all, any, bool, bytes, callable, chr, classmethod, complex, dict, enumerate, filter, float, frozenset, getattr, hasattr, hash, id, int, isinstance, issubclass, iter, len, list, locals, globals, map, min, max, next, object, ord, property, range, reversed, set, setattr, slice, str, sum, super, tuple, type, vars, zip, repr, print
 @_coconut.functools.wraps(_coconut.functools.partial)
 def _coconut_partial(_coconut_func, *args, **kwargs):
     partial_func = _coconut.functools.partial(_coconut_func, *args, **kwargs)
     partial_func.__name__ = _coconut.getattr(_coconut_func, "__name__", None)
     return partial_func
 def _coconut_handle_cls_kwargs(**kwargs):
     """Some code taken from six under the terms of its MIT license."""
@@ -322,14 +342,18 @@
         return obj.to_pandas()
 def _coconut_xarray_to_numpy(obj):
     import xarray
     if isinstance(obj, xarray.Dataset):
         return obj.to_dataframe().to_numpy()
     else:
         return obj.to_numpy()
+class CoconutWarning(Warning):
+    """Exception class used for all Coconut warnings."""
+    __slots__ = ()
+_coconut_CoconutWarning = CoconutWarning
 class MatchError(_coconut_baseclass, Exception):
     """Pattern-matching error. Has attributes .pattern, .value, and .message."""
     max_val_repr_len = 500
     def __init__(self, pattern=None, value=None):
         self.pattern = pattern
         self.value = value
         self._message = None
@@ -1010,18 +1034,15 @@
             iterables = ()
             repeat = 1
         if repeat < 0:
             raise _coconut.ValueError("cartesian_product: repeat cannot be negative")
         if iterables:
             it_modules = [_coconut_get_base_module(it) for it in iterables]
             if _coconut.all(mod in _coconut.numpy_modules for mod in it_modules):
-                if _coconut.any(mod in _coconut.xarray_modules for mod in it_modules):
-                    iterables = tuple((_coconut_xarray_to_numpy(it) if mod in _coconut.xarray_modules else it) for it, mod in _coconut.zip(iterables, it_modules))
-                if _coconut.any(mod in _coconut.pandas_modules for mod in it_modules):
-                    iterables = tuple((it.to_numpy() if mod in _coconut.pandas_modules else it) for it, mod in _coconut.zip(iterables, it_modules))
+                iterables = tuple((it.to_numpy() if mod in _coconut.pandas_modules else _coconut_xarray_to_numpy(it) if mod in _coconut.xarray_modules else it) for it, mod in _coconut.zip(iterables, it_modules))
                 if _coconut.any(mod in _coconut.jax_numpy_modules for mod in it_modules):
                     from jax import numpy
                 else:
                     numpy = _coconut.numpy
                 iterables *= repeat
                 dtype = numpy.result_type(*iterables)
                 arr = numpy.empty([_coconut.len(a) for a in iterables] + [_coconut.len(iterables)], dtype=dtype)
@@ -1086,15 +1107,15 @@
             return self.__class__(self.func, *(_coconut_iter_getitem(it, index) for it in self.iters))
         return self.func(*(_coconut_iter_getitem(it, index) for it in self.iters))
     def __reversed__(self):
         return self.__class__(self.func, *(reversed(it) for it in self.iters))
     def __len__(self):
         if not _coconut.all(_coconut.isinstance(it, _coconut.abc.Sized) for it in self.iters):
             return _coconut.NotImplemented
-        return _coconut.min(_coconut.len(it) for it in self.iters)
+        return _coconut.min((_coconut.len(it) for it in self.iters), default=0)
     def __repr__(self):
         return "%s(%r, %s)" % (self.__class__.__name__, self.func, ", ".join((_coconut.repr(it) for it in self.iters)))
     def __reduce__(self):
         return (self.__class__, (self.func,) + self.iters)
     def __copy__(self):
         self.iters = _coconut.tuple(reiterable(it) for it in self.iters)
         return self.__class__(self.func, *self.iters)
@@ -1228,15 +1249,15 @@
             return self.__class__(*(_coconut_iter_getitem(it, index) for it in self.iters), strict=self.strict)
         return _coconut.tuple(_coconut_iter_getitem(it, index) for it in self.iters)
     def __reversed__(self):
         return self.__class__(*(reversed(it) for it in self.iters), strict=self.strict)
     def __len__(self):
         if not _coconut.all(_coconut.isinstance(it, _coconut.abc.Sized) for it in self.iters):
             return _coconut.NotImplemented
-        return _coconut.min(_coconut.len(it) for it in self.iters)
+        return _coconut.min((_coconut.len(it) for it in self.iters), default=0)
     def __repr__(self):
         return "zip(%s%s)" % (", ".join((_coconut.repr(it) for it in self.iters)), ", strict=True" if self.strict else "")
     def __reduce__(self):
         return (self.__class__, self.iters, {"strict": self.strict})
     def __copy__(self):
         self.iters = _coconut.tuple(reiterable(it) for it in self.iters)
         return self.__class__(*self.iters, strict=self.strict)
@@ -1282,15 +1303,15 @@
                 got_non_default = True
         if not got_non_default:
             raise _coconut.IndexError("zip_longest index out of range")
         return _coconut.tuple(result)
     def __len__(self):
         if not _coconut.all(_coconut.isinstance(it, _coconut.abc.Sized) for it in self.iters):
             return _coconut.NotImplemented
-        return _coconut.max(_coconut.len(it) for it in self.iters)
+        return _coconut.max((_coconut.len(it) for it in self.iters), default=0)
     def __repr__(self):
         return "zip_longest(%s, fillvalue=%s)" % (", ".join((_coconut.repr(it) for it in self.iters)), _coconut.repr(self.fillvalue))
     def __reduce__(self):
         return (self.__class__, self.iters, {"fillvalue": self.fillvalue})
     def __copy__(self):
         self.iters = _coconut.tuple(reiterable(it) for it in self.iters)
         return self.__class__(*self.iters, fillvalue=self.fillvalue)
@@ -1346,20 +1367,15 @@
             return _coconut.NotImplemented
         return _coconut.len(self.iter)
 class multi_enumerate(_coconut_has_iter):
     """Enumerate an iterable of iterables. Works like enumerate, but indexes
     through inner iterables and produces a tuple index representing the index
     in each inner iterable. Supports indexing.
 
-    For numpy arrays, effectively equivalent to:
-        it = np.nditer(iterable, flags=["multi_index", "refs_ok"])
-        for x in it:
-            yield it.multi_index, x
-
-    Also supports len for numpy arrays.
+    For numpy arrays, uses np.nditer under the hood and supports len.
     """
     __slots__ = ()
     def __repr__(self):
         return "multi_enumerate(%s)" % (_coconut.repr(self.iter),)
     def __reduce__(self):
         return (self.__class__, (self.iter,))
     def __copy__(self):
@@ -1687,15 +1703,15 @@
     """Decorator to add new cases to a pattern-matching function (where the new case is checked last).
 
     Pass allow_any_func=True to allow any object as the base_func rather than just pattern-matching functions.
     If add_funcs are passed, addpattern(base_func, add_func) is equivalent to addpattern(base_func)(add_func).
     """
     allow_any_func = kwargs.pop("allow_any_func", False)
     if not allow_any_func and not _coconut.getattr(base_func, "_coconut_is_match", False):
-        _coconut.warnings.warn("Possible misuse of addpattern with non-pattern-matching function " + _coconut.repr(base_func) + " (pass allow_any_func=True to dismiss)", stacklevel=2)
+        _coconut.warnings.warn("Possible misuse of addpattern with non-pattern-matching function " + _coconut.repr(base_func) + " (pass allow_any_func=True to dismiss)", _coconut_CoconutWarning, 2)
     if kwargs:
         raise _coconut.TypeError("addpattern() got unexpected keyword arguments " + _coconut.repr(kwargs))
     if add_funcs:
         return _coconut_base_pattern_func(base_func, *add_funcs)
     return _coconut_partial(_coconut_base_pattern_func, base_func)
 _coconut_addpattern = addpattern
 class _coconut_complex_partial(_coconut_base_callable):
@@ -1929,15 +1945,15 @@
             _coconut_exec('async def __anext__(self):\n    return self.func(await self.aiter.__anext__())', _coconut___anext___ns)
             __anext__ = _coconut___anext___ns["__anext__"]
 def fmap(func, obj, **kwargs):
     """fmap(func, obj) creates a copy of obj with func applied to its contents.
 
     Supports:
     * Coconut data types
-    * `str`, `dict`, `list`, `tuple`, `set`, `frozenset`
+    * `str`, `dict`, `list`, `tuple`, `set`, `frozenset`, `bytes`, `bytearray`
     * `dict` (maps over .items())
     * asynchronous iterables
     * numpy arrays (uses np.vectorize)
     * pandas objects (uses .apply)
 
     Override by defining obj.__fmap__(func).
     """
@@ -1971,18 +1987,19 @@
         try:
             aiter = obj_aiter()
         except _coconut.NotImplementedError:
             pass
         else:
             if aiter is not _coconut.NotImplemented:
                 return _coconut_amap(func, aiter)
-    if starmap_over_mappings:
-        return _coconut_base_makedata(obj.__class__, starmap(func, obj.items()) if _coconut.isinstance(obj, _coconut.abc.Mapping) else map(func, obj), from_fmap=True, fallback_to_init=fallback_to_init)
+    if _coconut.isinstance(obj, _coconut.abc.Mapping):
+        mapped_obj = (starmap if starmap_over_mappings else map)(func, obj.items())
     else:
-        return _coconut_base_makedata(obj.__class__, map(func, obj.items() if _coconut.isinstance(obj, _coconut.abc.Mapping) else obj), from_fmap=True, fallback_to_init=fallback_to_init)
+        mapped_obj = _coconut_map(func, obj)
+    return _coconut_base_makedata(obj.__class__, mapped_obj, from_fmap=True, fallback_to_init=fallback_to_init)
 def _coconut_memoize_helper(maxsize=None, typed=False):
     return maxsize, typed
 def memoize(*args, **kwargs):
     """Decorator that memoizes a function, preventing it from being recomputed
     if it is called multiple times with the same arguments."""
     if not kwargs and _coconut.len(args) == 1 and _coconut.callable(args[0]):
         return _coconut.functools.lru_cache(maxsize=None)(args[0])
@@ -2042,21 +2059,24 @@
     Accepts one keyword-only argument, side_effect, which specifies a function to call on the argument before it is returned."""
     side_effect = kwargs.pop("side_effect", None)
     if kwargs:
         raise _coconut.TypeError("ident() got unexpected keyword arguments " + _coconut.repr(kwargs))
     if side_effect is not None:
         side_effect(x)
     return x
-def call(_coconut_f, *args, **kwargs):
-    """Function application operator function.
+if _coconut_sys.version_info < (3, 11):
+    def call(_coconut_f, *args, **kwargs):
+        """Function application operator function.
 
-    Equivalent to:
-        def call(f, /, *args, **kwargs) = f(*args, **kwargs).
-    """
-    return _coconut_f(*args, **kwargs)
+        Equivalent to:
+            def call(f, /, *args, **kwargs) = f(*args, **kwargs).
+        """
+        return _coconut_f(*args, **kwargs)
+else:
+    call = _coconut.operator.call
 def safe_call(_coconut_f, *args, **kwargs):
     """safe_call is a version of call that catches any Exceptions and
     returns an Expected containing either the result or the error.
 
     Equivalent to:
         def safe_call(f, /, *args, **kwargs):
             try:
@@ -2295,18 +2315,18 @@
     """For a given iterable, check whether all elements in that iterable are equal to each other.
     If 'to' is passed, check that all the elements are equal to that value.
 
     Supports numpy arrays. Assumes transitivity and 'x != y' being equivalent to 'not (x == y)'.
     """
     iterable_module = _coconut_get_base_module(iterable)
     if iterable_module in _coconut.numpy_modules:
-        if iterable_module in _coconut.xarray_modules:
-            iterable = _coconut_xarray_to_numpy(iterable)
-        elif iterable_module in _coconut.pandas_modules:
+        if iterable_module in _coconut.pandas_modules:
             iterable = iterable.to_numpy()
+        elif iterable_module in _coconut.xarray_modules:
+            iterable = _coconut_xarray_to_numpy(iterable)
         return not _coconut.len(iterable) or (iterable == (iterable[0] if to is _coconut_sentinel else to)).all()
     first_item = to
     for item in iterable:
         if first_item is _coconut_sentinel:
             first_item = item
         elif first_item != item:
             return False
@@ -2430,15 +2450,15 @@
     arr_dims.append(dim)
     max_arr_dim = _coconut.max(arr_dims)
     return _coconut_concatenate(arrs, max_arr_dim - dim)
 def _coconut_call_or_coefficient(func, *args):
     if _coconut.callable(func):
         return func(*args)
     if not _coconut.isinstance(func, (_coconut.int, _coconut.float, _coconut.complex)) and _coconut_get_base_module(func) not in _coconut.numpy_modules:
-        raise _coconut.TypeError("implicit function application and coefficient syntax only supported for Callable, int, float, complex, and numpy objects")
+        raise _coconut.TypeError("first object in implicit function application and coefficient syntax must be Callable, int, float, complex, or numpy")
     func = func
     for x in args:
         func = func * x
     return func
 class _coconut_SupportsAdd(_coconut.typing.Protocol):
     """Coconut (+) Protocol. Equivalent to:
```

### Comparing `pokespeed-1.0.1/pokespeed/__init__.py` & `pokespeed-1.1.0/pokespeed/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# __coconut_hash__ = 0x5ef0d68e
+# __coconut_hash__ = 0x941c2e58
 
-# Compiled with Coconut version 3.0.4-post_dev17
+# Compiled with Coconut version 3.1.0-post_dev13
 
 # Coconut Header: -------------------------------------------------------------
 
 import sys as _coconut_sys
 import os as _coconut_os
-_coconut_header_info = ('3.0.4-post_dev17', '3', True)
+_coconut_header_info = ('3.1.0-post_dev13', '3', True)
 _coconut_cached__coconut__ = _coconut_sys.modules.get('__coconut__')
 _coconut_file_dir = _coconut_os.path.dirname(_coconut_os.path.abspath(__file__))
 _coconut_pop_path = False
-if _coconut_cached__coconut__ is None or getattr(_coconut_cached__coconut__, "_coconut_header_info", None) != _coconut_header_info and _coconut_os.path.dirname(_coconut_cached__coconut__.__file__ or "") != _coconut_file_dir:
+if _coconut_cached__coconut__ is None or getattr(_coconut_cached__coconut__, "_coconut_header_info", None) != _coconut_header_info and _coconut_os.path.dirname(_coconut_cached__coconut__.__file__ or "") != _coconut_file_dir:  # type: ignore
     if _coconut_cached__coconut__ is not None:
         _coconut_sys.modules['_coconut_cached__coconut__'] = _coconut_cached__coconut__
         del _coconut_sys.modules['__coconut__']
     _coconut_sys.path.insert(0, _coconut_file_dir)
     _coconut_pop_path = True
     _coconut_module_name = _coconut_os.path.splitext(_coconut_os.path.basename(_coconut_file_dir))[0]
-    if _coconut_module_name and _coconut_module_name[0].isalpha() and all(c.isalpha() or c.isdigit() for c in _coconut_module_name) and "__init__.py" in _coconut_os.listdir(_coconut_file_dir):
-        _coconut_full_module_name = str(_coconut_module_name + ".__coconut__")
+    if _coconut_module_name and _coconut_module_name[0].isalpha() and all(c.isalpha() or c.isdigit() for c in _coconut_module_name) and "__init__.py" in _coconut_os.listdir(_coconut_file_dir):  # type: ignore
+        _coconut_full_module_name = str(_coconut_module_name + ".__coconut__")  # type: ignore
         import __coconut__ as _coconut__coconut__
         _coconut__coconut__.__name__ = _coconut_full_module_name
-        for _coconut_v in vars(_coconut__coconut__).values():
-            if getattr(_coconut_v, "__module__", None) == '__coconut__':
+        for _coconut_v in vars(_coconut__coconut__).values():  # type: ignore
+            if getattr(_coconut_v, "__module__", None) == '__coconut__':  # type: ignore
                 try:
                     _coconut_v.__module__ = _coconut_full_module_name
                 except AttributeError:
-                    _coconut_v_type = type(_coconut_v)
-                    if getattr(_coconut_v_type, "__module__", None) == '__coconut__':
+                    _coconut_v_type = type(_coconut_v)  # type: ignore
+                    if getattr(_coconut_v_type, "__module__", None) == '__coconut__':  # type: ignore
                         _coconut_v_type.__module__ = _coconut_full_module_name
         _coconut_sys.modules[_coconut_full_module_name] = _coconut__coconut__
 from __coconut__ import *
-from __coconut__ import _coconut_tail_call, _coconut_tco, _coconut_call_set_names, _namedtuple_of, _coconut, _coconut_Expected, _coconut_MatchError, _coconut_SupportsAdd, _coconut_SupportsMinus, _coconut_SupportsMul, _coconut_SupportsPow, _coconut_SupportsTruediv, _coconut_SupportsFloordiv, _coconut_SupportsMod, _coconut_SupportsAnd, _coconut_SupportsXor, _coconut_SupportsOr, _coconut_SupportsLshift, _coconut_SupportsRshift, _coconut_SupportsMatmul, _coconut_SupportsInv, _coconut_iter_getitem, _coconut_base_compose, _coconut_forward_compose, _coconut_back_compose, _coconut_forward_star_compose, _coconut_back_star_compose, _coconut_forward_dubstar_compose, _coconut_back_dubstar_compose, _coconut_pipe, _coconut_star_pipe, _coconut_dubstar_pipe, _coconut_back_pipe, _coconut_back_star_pipe, _coconut_back_dubstar_pipe, _coconut_none_pipe, _coconut_none_star_pipe, _coconut_none_dubstar_pipe, _coconut_bool_and, _coconut_bool_or, _coconut_none_coalesce, _coconut_minus, _coconut_map, _coconut_partial, _coconut_complex_partial, _coconut_get_function_match_error, _coconut_base_pattern_func, _coconut_addpattern, _coconut_sentinel, _coconut_assert, _coconut_raise, _coconut_mark_as_match, _coconut_reiterable, _coconut_self_match_types, _coconut_dict_merge, _coconut_exec, _coconut_comma_op, _coconut_arr_concat_op, _coconut_mk_anon_namedtuple, _coconut_matmul, _coconut_py_str, _coconut_flatten, _coconut_multiset, _coconut_back_none_pipe, _coconut_back_none_star_pipe, _coconut_back_none_dubstar_pipe, _coconut_forward_none_compose, _coconut_back_none_compose, _coconut_forward_none_star_compose, _coconut_back_none_star_compose, _coconut_forward_none_dubstar_compose, _coconut_back_none_dubstar_compose, _coconut_call_or_coefficient, _coconut_in, _coconut_not_in, _coconut_attritemgetter, _coconut_if_op
+from __coconut__ import _coconut_tail_call, _coconut_tco, _coconut_call_set_names, _namedtuple_of, _coconut, _coconut_Expected, _coconut_MatchError, _coconut_SupportsAdd, _coconut_SupportsMinus, _coconut_SupportsMul, _coconut_SupportsPow, _coconut_SupportsTruediv, _coconut_SupportsFloordiv, _coconut_SupportsMod, _coconut_SupportsAnd, _coconut_SupportsXor, _coconut_SupportsOr, _coconut_SupportsLshift, _coconut_SupportsRshift, _coconut_SupportsMatmul, _coconut_SupportsInv, _coconut_iter_getitem, _coconut_base_compose, _coconut_forward_compose, _coconut_back_compose, _coconut_forward_star_compose, _coconut_back_star_compose, _coconut_forward_dubstar_compose, _coconut_back_dubstar_compose, _coconut_pipe, _coconut_star_pipe, _coconut_dubstar_pipe, _coconut_back_pipe, _coconut_back_star_pipe, _coconut_back_dubstar_pipe, _coconut_none_pipe, _coconut_none_star_pipe, _coconut_none_dubstar_pipe, _coconut_bool_and, _coconut_bool_or, _coconut_none_coalesce, _coconut_minus, _coconut_map, _coconut_partial, _coconut_complex_partial, _coconut_get_function_match_error, _coconut_base_pattern_func, _coconut_addpattern, _coconut_sentinel, _coconut_assert, _coconut_raise, _coconut_mark_as_match, _coconut_reiterable, _coconut_self_match_types, _coconut_dict_merge, _coconut_exec, _coconut_comma_op, _coconut_arr_concat_op, _coconut_mk_anon_namedtuple, _coconut_matmul, _coconut_py_str, _coconut_flatten, _coconut_multiset, _coconut_back_none_pipe, _coconut_back_none_star_pipe, _coconut_back_none_dubstar_pipe, _coconut_forward_none_compose, _coconut_back_none_compose, _coconut_forward_none_star_compose, _coconut_back_none_star_compose, _coconut_forward_none_dubstar_compose, _coconut_back_none_dubstar_compose, _coconut_call_or_coefficient, _coconut_in, _coconut_not_in, _coconut_attritemgetter, _coconut_if_op, _coconut_CoconutWarning
 if _coconut_pop_path:
     _coconut_sys.path.pop(0)
 try:
     __file__ = _coconut_os.path.abspath(__file__) if __file__ else __file__
 except NameError:
     pass
 else:
@@ -83,64 +83,76 @@
             else:  #46 (line in Coconut source)
                 break  #47 (line in Coconut source)
         else:  #48 (line in Coconut source)
             warn("failed to find pokemon {_coconut_format_0}".format(_coconut_format_0=(name)))  #49 (line in Coconut source)
 
 
 
-class Nature(_coconut.collections.namedtuple("Nature", ('multiplier', 'identifier'))):  #52 (line in Coconut source)
+class Nature(_coconut.collections.namedtuple("Nature", ('multiplier', 'identifier', 'min_ev', 'min_iv'))):  #52 (line in Coconut source)
     __slots__ = ()  #52 (line in Coconut source)
     _coconut_is_data = True  #52 (line in Coconut source)
-    __match_args__ = ('multiplier', 'identifier')  #52 (line in Coconut source)
+    __match_args__ = ('multiplier', 'identifier', 'min_ev', 'min_iv')  #52 (line in Coconut source)
     def __add__(self, other): return _coconut.NotImplemented  #52 (line in Coconut source)
     def __mul__(self, other): return _coconut.NotImplemented  #52 (line in Coconut source)
     def __rmul__(self, other): return _coconut.NotImplemented  #52 (line in Coconut source)
     __ne__ = _coconut.object.__ne__  #52 (line in Coconut source)
     def __eq__(self, other):  #52 (line in Coconut source)
         return self.__class__ is other.__class__ and _coconut.tuple.__eq__(self, other)  #52 (line in Coconut source)
     def __hash__(self):  #52 (line in Coconut source)
-        return _coconut.tuple.__hash__(self) ^ hash(self.__class__)  #52 (line in Coconut source)
+        return _coconut.tuple.__hash__(self) ^ _coconut.hash(self.__class__)  #52 (line in Coconut source)
+    def __new__(_coconut_cls, multiplier, identifier, min_ev=False, min_iv=False):  #52 (line in Coconut source)
+        return _coconut.tuple.__new__(_coconut_cls, (multiplier, identifier, min_ev, min_iv))  #52 (line in Coconut source)
+    _coconut_data_defaults = {2: __new__.__defaults__[0], 3: __new__.__defaults__[1]}  # type: ignore  #52 (line in Coconut source)
     @_coconut_tco  #52 (line in Coconut source)
     def apply(self, stat):  #52 (line in Coconut source)
         return _coconut_tail_call(int, stat * self.multiplier)  #53 (line in Coconut source)
 
     def __str__(self):  #54 (line in Coconut source)
         return self.identifier  #54 (line in Coconut source)
 
+    @property  #55 (line in Coconut source)
+    def ev(self):  #56 (line in Coconut source)
+        return 0 if self.min_ev else 252  #56 (line in Coconut source)
+
+    @property  #57 (line in Coconut source)
+    def iv(self):  #58 (line in Coconut source)
+        return 0 if self.min_iv else 31  #58 (line in Coconut source)
 
-_coconut_call_set_names(Nature)  #56 (line in Coconut source)
-Helpful = Nature(1.1, "+")  #56 (line in Coconut source)
-Harmful = Nature(0.9, "-")  #57 (line in Coconut source)
-Neutral = Nature(1, "=")  #58 (line in Coconut source)
 
-important_natures = (Helpful, Neutral)  #60 (line in Coconut source)
+_coconut_call_set_names(Nature)  #60 (line in Coconut source)
+Helpful = Nature(1.1, "+")  #60 (line in Coconut source)
+Neutral = Nature(1, "=")  #61 (line in Coconut source)
+Uninvested = Nature(1, "0", min_ev=True)  #62 (line in Coconut source)
+Harmful = Nature(0.9, "-", min_ev=True, min_iv=True)  #63 (line in Coconut source)
 
 
 class Stage(_coconut.collections.namedtuple("Stage", ('stat_stage', 'stat_modifier'))):  #66 (line in Coconut source)
     __slots__ = ()  #66 (line in Coconut source)
     _coconut_is_data = True  #66 (line in Coconut source)
     __match_args__ = ('stat_stage', 'stat_modifier')  #66 (line in Coconut source)
     def __add__(self, other): return _coconut.NotImplemented  #66 (line in Coconut source)
     def __mul__(self, other): return _coconut.NotImplemented  #66 (line in Coconut source)
     def __rmul__(self, other): return _coconut.NotImplemented  #66 (line in Coconut source)
     __ne__ = _coconut.object.__ne__  #66 (line in Coconut source)
     def __eq__(self, other):  #66 (line in Coconut source)
         return self.__class__ is other.__class__ and _coconut.tuple.__eq__(self, other)  #66 (line in Coconut source)
     def __hash__(self):  #66 (line in Coconut source)
-        return _coconut.tuple.__hash__(self) ^ hash(self.__class__)  #66 (line in Coconut source)
+        return _coconut.tuple.__hash__(self) ^ _coconut.hash(self.__class__)  #66 (line in Coconut source)
     def __new__(_coconut_cls, _coconut_match_first_arg=_coconut_sentinel, *_coconut_match_args, **_coconut_match_kwargs):  #66 (line in Coconut source)
         _coconut_match_check_6 = False  #66 (line in Coconut source)
         _coconut_match_set_name_stat_modifier = _coconut_sentinel  #66 (line in Coconut source)
         _coconut_FunctionMatchError = _coconut_get_function_match_error()  #66 (line in Coconut source)
         if _coconut_match_first_arg is not _coconut_sentinel:  #66 (line in Coconut source)
             _coconut_match_args = (_coconut_match_first_arg,) + _coconut_match_args  #66 (line in Coconut source)
         if (_coconut.len(_coconut_match_args) <= 2) and (_coconut.sum((_coconut.len(_coconut_match_args) > 0, "stat_stage" in _coconut_match_kwargs)) == 1) and (_coconut.sum((_coconut.len(_coconut_match_args) > 1, "stat_modifier" in _coconut_match_kwargs)) <= 1):  #66 (line in Coconut source)
             _coconut_match_temp_10 = _coconut_match_args[0] if _coconut.len(_coconut_match_args) > 0 else _coconut_match_kwargs.pop("stat_stage")  #66 (line in Coconut source)
-            _coconut_match_temp_15 = _coconut_match_args[1] if _coconut.len(_coconut_match_args) > 1 else _coconut_match_kwargs.pop("stat_modifier") if "stat_modifier" in _coconut_match_kwargs else 1  #66 (line in Coconut source)
+            _coconut_match_temp_15 = _coconut_match_args[1] if _coconut.len(_coconut_match_args) > 1 else _coconut_match_kwargs.pop("stat_modifier") if "stat_modifier" in _coconut_match_kwargs else _coconut_sentinel  #66 (line in Coconut source)
             _coconut_match_temp_11 = _coconut.getattr(int, "_coconut_is_data", False) or _coconut.isinstance(int, _coconut.tuple) and _coconut.all(_coconut.getattr(_coconut_x, "_coconut_is_data", False) for _coconut_x in int)  # type: ignore  #66 (line in Coconut source)
+            if _coconut_match_temp_15 is _coconut_sentinel:  #66 (line in Coconut source)
+                _coconut_match_temp_15 = 1  #66 (line in Coconut source)
             _coconut_match_set_name_stat_modifier = _coconut_match_temp_15  #66 (line in Coconut source)
             if not _coconut_match_kwargs:  #66 (line in Coconut source)
                 _coconut_match_check_6 = True  #66 (line in Coconut source)
         if _coconut_match_check_6:  #66 (line in Coconut source)
             _coconut_match_check_6 = False  #66 (line in Coconut source)
             if not _coconut_match_check_6:  #66 (line in Coconut source)
                 _coconut_match_set_name_stat_stage = _coconut_sentinel  #66 (line in Coconut source)
@@ -221,14 +233,15 @@
             raise _coconut_FunctionMatchError('match def apply(self, stat if self.stat_modifier != 1) =', _coconut_match_args)  #66 (line in Coconut source)
 
         return _coconut_tail_call((int), self._replace(stat_modifier=1).apply(stat) * self.stat_modifier)  #68 (line in Coconut source)
 
     try:  #69 (line in Coconut source)
         _coconut_addpattern_0 = _coconut_addpattern(apply)  # type: ignore  #69 (line in Coconut source)
     except _coconut.NameError:  #69 (line in Coconut source)
+        _coconut.warnings.warn("Deprecated use of 'addpattern def apply' with no pre-existing 'apply' function (use 'match def apply' for the first definition or switch to 'case def' syntax)", _coconut_CoconutWarning)  #69 (line in Coconut source)
         _coconut_addpattern_0 = lambda f: f  #69 (line in Coconut source)
     @_coconut_addpattern_0  #69 (line in Coconut source)
     @_coconut_mark_as_match  #69 (line in Coconut source)
     def apply(_coconut_match_first_arg=_coconut_sentinel, *_coconut_match_args, **_coconut_match_kwargs):  #69 (line in Coconut source)
         _coconut_match_check_1 = False  #69 (line in Coconut source)
         _coconut_match_set_name_self = _coconut_sentinel  #69 (line in Coconut source)
         _coconut_match_set_name_stat = _coconut_sentinel  #69 (line in Coconut source)
@@ -253,14 +266,15 @@
             raise _coconut_FunctionMatchError('addpattern def apply(self, stat if self.stat_stage > 0) =', _coconut_match_args)  #69 (line in Coconut source)
 
         return stat * (2 + self.stat_stage) // 2  #70 (line in Coconut source)
 
     try:  #71 (line in Coconut source)
         _coconut_addpattern_1 = _coconut_addpattern(apply)  # type: ignore  #71 (line in Coconut source)
     except _coconut.NameError:  #71 (line in Coconut source)
+        _coconut.warnings.warn("Deprecated use of 'addpattern def apply' with no pre-existing 'apply' function (use 'match def apply' for the first definition or switch to 'case def' syntax)", _coconut_CoconutWarning)  #71 (line in Coconut source)
         _coconut_addpattern_1 = lambda f: f  #71 (line in Coconut source)
     @_coconut_addpattern_1  #71 (line in Coconut source)
     @_coconut_mark_as_match  #71 (line in Coconut source)
     def apply(_coconut_match_first_arg=_coconut_sentinel, *_coconut_match_args, **_coconut_match_kwargs):  #71 (line in Coconut source)
         _coconut_match_check_2 = False  #71 (line in Coconut source)
         _coconut_match_set_name_self = _coconut_sentinel  #71 (line in Coconut source)
         _coconut_match_set_name_stat = _coconut_sentinel  #71 (line in Coconut source)
@@ -285,14 +299,15 @@
             raise _coconut_FunctionMatchError('addpattern def apply(self, stat if self.stat_stage < 0) =', _coconut_match_args)  #71 (line in Coconut source)
 
         return stat * 2 // (2 - self.stat_stage)  #72 (line in Coconut source)
 
     try:  #73 (line in Coconut source)
         _coconut_addpattern_2 = _coconut_addpattern(apply)  # type: ignore  #73 (line in Coconut source)
     except _coconut.NameError:  #73 (line in Coconut source)
+        _coconut.warnings.warn("Deprecated use of 'addpattern def apply' with no pre-existing 'apply' function (use 'match def apply' for the first definition or switch to 'case def' syntax)", _coconut_CoconutWarning)  #73 (line in Coconut source)
         _coconut_addpattern_2 = lambda f: f  #73 (line in Coconut source)
     @_coconut_addpattern_2  #73 (line in Coconut source)
     @_coconut_mark_as_match  #73 (line in Coconut source)
     def apply(_coconut_match_first_arg=_coconut_sentinel, *_coconut_match_args, **_coconut_match_kwargs):  #73 (line in Coconut source)
         _coconut_match_check_3 = False  #73 (line in Coconut source)
         _coconut_match_set_name_self = _coconut_sentinel  #73 (line in Coconut source)
         _coconut_match_set_name_stat = _coconut_sentinel  #73 (line in Coconut source)
@@ -316,311 +331,319 @@
         if not _coconut_match_check_3:  #73 (line in Coconut source)
             raise _coconut_FunctionMatchError('addpattern def apply(self, stat if self.stat_stage == 0) = stat', _coconut_match_args)  #73 (line in Coconut source)
 
         return stat  #73 (line in Coconut source)
 
 
     def __str__(self):  #75 (line in Coconut source)
-        return "{_coconut_format_0:+}".format(_coconut_format_0=(self.stat_stage)) + (" x{_coconut_format_0}".format(_coconut_format_0=(self.stat_modifier)) if self.stat_modifier != 1 else "")  #75 (line in Coconut source)
+        return "{_coconut_format_0:+}".format(_coconut_format_0=(self.stat_stage)) + (" x{_coconut_format_0}".format(_coconut_format_0=(self.stat_modifier)) if self.stat_modifier != 1 else "")  #76 (line in Coconut source)
 
 
-    @_coconut_mark_as_match  #77 (line in Coconut source)
-    def modifier_str(_coconut_match_first_arg=_coconut_sentinel, *_coconut_match_args, **_coconut_match_kwargs):  #77 (line in Coconut source)
-        _coconut_match_check_4 = False  #77 (line in Coconut source)
-        _coconut_match_set_name_self = _coconut_sentinel  #77 (line in Coconut source)
-        _coconut_FunctionMatchError = _coconut_get_function_match_error()  #77 (line in Coconut source)
-        if _coconut_match_first_arg is not _coconut_sentinel:  #77 (line in Coconut source)
-            _coconut_match_args = (_coconut_match_first_arg,) + _coconut_match_args  #77 (line in Coconut source)
-        if (_coconut.len(_coconut_match_args) <= 1) and (_coconut.sum((_coconut.len(_coconut_match_args) > 0, "self" in _coconut_match_kwargs)) == 1):  #77 (line in Coconut source)
-            _coconut_match_temp_8 = _coconut_match_args[0] if _coconut.len(_coconut_match_args) > 0 else _coconut_match_kwargs.pop("self")  #77 (line in Coconut source)
-            _coconut_match_set_name_self = _coconut_match_temp_8  #77 (line in Coconut source)
-            if not _coconut_match_kwargs:  #77 (line in Coconut source)
-                _coconut_match_check_4 = True  #77 (line in Coconut source)
-        if _coconut_match_check_4:  #77 (line in Coconut source)
-            if _coconut_match_set_name_self is not _coconut_sentinel:  #77 (line in Coconut source)
-                self = _coconut_match_set_name_self  #77 (line in Coconut source)
-        if _coconut_match_check_4 and not (self.stat_stage == 0):  #77 (line in Coconut source)
-            _coconut_match_check_4 = False  #77 (line in Coconut source)
-        if not _coconut_match_check_4:  #77 (line in Coconut source)
-            raise _coconut_FunctionMatchError('match def modifier_str(self if self.stat_stage == 0) = ""', _coconut_match_args)  #77 (line in Coconut source)
-
-        return ""  #77 (line in Coconut source)
-
-    try:  #78 (line in Coconut source)
-        _coconut_addpattern_3 = _coconut_addpattern(modifier_str)  # type: ignore  #78 (line in Coconut source)
-    except _coconut.NameError:  #78 (line in Coconut source)
-        _coconut_addpattern_3 = lambda f: f  #78 (line in Coconut source)
-    @_coconut_addpattern_3  #78 (line in Coconut source)
     @_coconut_mark_as_match  #78 (line in Coconut source)
     def modifier_str(_coconut_match_first_arg=_coconut_sentinel, *_coconut_match_args, **_coconut_match_kwargs):  #78 (line in Coconut source)
-        _coconut_match_check_5 = False  #78 (line in Coconut source)
+        _coconut_match_check_4 = False  #78 (line in Coconut source)
         _coconut_match_set_name_self = _coconut_sentinel  #78 (line in Coconut source)
         _coconut_FunctionMatchError = _coconut_get_function_match_error()  #78 (line in Coconut source)
         if _coconut_match_first_arg is not _coconut_sentinel:  #78 (line in Coconut source)
             _coconut_match_args = (_coconut_match_first_arg,) + _coconut_match_args  #78 (line in Coconut source)
         if (_coconut.len(_coconut_match_args) <= 1) and (_coconut.sum((_coconut.len(_coconut_match_args) > 0, "self" in _coconut_match_kwargs)) == 1):  #78 (line in Coconut source)
-            _coconut_match_temp_9 = _coconut_match_args[0] if _coconut.len(_coconut_match_args) > 0 else _coconut_match_kwargs.pop("self")  #78 (line in Coconut source)
-            _coconut_match_set_name_self = _coconut_match_temp_9  #78 (line in Coconut source)
+            _coconut_match_temp_8 = _coconut_match_args[0] if _coconut.len(_coconut_match_args) > 0 else _coconut_match_kwargs.pop("self")  #78 (line in Coconut source)
+            _coconut_match_set_name_self = _coconut_match_temp_8  #78 (line in Coconut source)
             if not _coconut_match_kwargs:  #78 (line in Coconut source)
-                _coconut_match_check_5 = True  #78 (line in Coconut source)
-        if _coconut_match_check_5:  #78 (line in Coconut source)
+                _coconut_match_check_4 = True  #78 (line in Coconut source)
+        if _coconut_match_check_4:  #78 (line in Coconut source)
             if _coconut_match_set_name_self is not _coconut_sentinel:  #78 (line in Coconut source)
                 self = _coconut_match_set_name_self  #78 (line in Coconut source)
-        if not _coconut_match_check_5:  #78 (line in Coconut source)
-            raise _coconut_FunctionMatchError('addpattern def modifier_str(self) = str(self) + " "', _coconut_match_args)  #78 (line in Coconut source)
+        if _coconut_match_check_4 and not (self.stat_stage == 0):  #78 (line in Coconut source)
+            _coconut_match_check_4 = False  #78 (line in Coconut source)
+        if not _coconut_match_check_4:  #78 (line in Coconut source)
+            raise _coconut_FunctionMatchError('match def modifier_str(self if self.stat_stage == 0) = ""', _coconut_match_args)  #78 (line in Coconut source)
+
+        return ""  #78 (line in Coconut source)
+
+    try:  #79 (line in Coconut source)
+        _coconut_addpattern_3 = _coconut_addpattern(modifier_str)  # type: ignore  #79 (line in Coconut source)
+    except _coconut.NameError:  #79 (line in Coconut source)
+        _coconut.warnings.warn("Deprecated use of 'addpattern def modifier_str' with no pre-existing 'modifier_str' function (use 'match def modifier_str' for the first definition or switch to 'case def' syntax)", _coconut_CoconutWarning)  #79 (line in Coconut source)
+        _coconut_addpattern_3 = lambda f: f  #79 (line in Coconut source)
+    @_coconut_addpattern_3  #79 (line in Coconut source)
+    @_coconut_mark_as_match  #79 (line in Coconut source)
+    def modifier_str(_coconut_match_first_arg=_coconut_sentinel, *_coconut_match_args, **_coconut_match_kwargs):  #79 (line in Coconut source)
+        _coconut_match_check_5 = False  #79 (line in Coconut source)
+        _coconut_match_set_name_self = _coconut_sentinel  #79 (line in Coconut source)
+        _coconut_FunctionMatchError = _coconut_get_function_match_error()  #79 (line in Coconut source)
+        if _coconut_match_first_arg is not _coconut_sentinel:  #79 (line in Coconut source)
+            _coconut_match_args = (_coconut_match_first_arg,) + _coconut_match_args  #79 (line in Coconut source)
+        if (_coconut.len(_coconut_match_args) <= 1) and (_coconut.sum((_coconut.len(_coconut_match_args) > 0, "self" in _coconut_match_kwargs)) == 1):  #79 (line in Coconut source)
+            _coconut_match_temp_9 = _coconut_match_args[0] if _coconut.len(_coconut_match_args) > 0 else _coconut_match_kwargs.pop("self")  #79 (line in Coconut source)
+            _coconut_match_set_name_self = _coconut_match_temp_9  #79 (line in Coconut source)
+            if not _coconut_match_kwargs:  #79 (line in Coconut source)
+                _coconut_match_check_5 = True  #79 (line in Coconut source)
+        if _coconut_match_check_5:  #79 (line in Coconut source)
+            if _coconut_match_set_name_self is not _coconut_sentinel:  #79 (line in Coconut source)
+                self = _coconut_match_set_name_self  #79 (line in Coconut source)
+        if not _coconut_match_check_5:  #79 (line in Coconut source)
+            raise _coconut_FunctionMatchError('addpattern def modifier_str(self) = str(self) + " "', _coconut_match_args)  #79 (line in Coconut source)
+
+        return str(self) + " "  #79 (line in Coconut source)
+
+
+
+_coconut_call_set_names(Stage)  #82 (line in Coconut source)
+@_coconut_tco  #82 (line in Coconut source)
+def calc_stat(base, stage, nature, level,):  #82 (line in Coconut source)
+    return _coconut_tail_call((stage.apply), (nature.apply)(((2 * base) + nature.iv + nature.ev // 4) * level // 100 + 5))  #82 (line in Coconut source)
+
+
+
+important_stages = (Stage(-1), Stage(0), Stage(-1, stat_modifier=2), Stage(+1), Stage(+2), Stage(+1, stat_modifier=2))  #94 (line in Coconut source)
+
+class PokemonSpeed(_coconut.collections.namedtuple("PokemonSpeed", ('name', 'base_speed', 'speed_stage', 'speed_nature', 'level'))):  #105 (line in Coconut source)
+    __slots__ = ()  #105 (line in Coconut source)
+    _coconut_is_data = True  #105 (line in Coconut source)
+    __match_args__ = ('name', 'base_speed', 'speed_stage', 'speed_nature', 'level')  #105 (line in Coconut source)
+    def __add__(self, other): return _coconut.NotImplemented  #105 (line in Coconut source)
+    def __mul__(self, other): return _coconut.NotImplemented  #105 (line in Coconut source)
+    def __rmul__(self, other): return _coconut.NotImplemented  #105 (line in Coconut source)
+    __ne__ = _coconut.object.__ne__  #105 (line in Coconut source)
+    def __eq__(self, other):  #105 (line in Coconut source)
+        return self.__class__ is other.__class__ and _coconut.tuple.__eq__(self, other)  #105 (line in Coconut source)
+    def __hash__(self):  #105 (line in Coconut source)
+        return _coconut.tuple.__hash__(self) ^ _coconut.hash(self.__class__)  #105 (line in Coconut source)
+    def __new__(_coconut_cls, _coconut_match_first_arg=_coconut_sentinel, *_coconut_match_args, **_coconut_match_kwargs):  #105 (line in Coconut source)
+        _coconut_match_check_7 = False  #105 (line in Coconut source)
+        _coconut_match_set_name_speed_stage = _coconut_sentinel  #105 (line in Coconut source)
+        _coconut_match_set_name_speed_nature = _coconut_sentinel  #105 (line in Coconut source)
+        _coconut_FunctionMatchError = _coconut_get_function_match_error()  #105 (line in Coconut source)
+        if _coconut_match_first_arg is not _coconut_sentinel:  #105 (line in Coconut source)
+            _coconut_match_args = (_coconut_match_first_arg,) + _coconut_match_args  #105 (line in Coconut source)
+        if (_coconut.len(_coconut_match_args) <= 5) and (_coconut.sum((_coconut.len(_coconut_match_args) > 0, "name" in _coconut_match_kwargs)) == 1) and (_coconut.sum((_coconut.len(_coconut_match_args) > 1, "base_speed" in _coconut_match_kwargs)) == 1) and (_coconut.sum((_coconut.len(_coconut_match_args) > 2, "speed_stage" in _coconut_match_kwargs)) == 1) and (_coconut.sum((_coconut.len(_coconut_match_args) > 3, "speed_nature" in _coconut_match_kwargs)) == 1) and (_coconut.sum((_coconut.len(_coconut_match_args) > 4, "level" in _coconut_match_kwargs)) == 1):  #105 (line in Coconut source)
+            _coconut_match_temp_16 = _coconut_match_args[0] if _coconut.len(_coconut_match_args) > 0 else _coconut_match_kwargs.pop("name")  #105 (line in Coconut source)
+            _coconut_match_temp_21 = _coconut_match_args[1] if _coconut.len(_coconut_match_args) > 1 else _coconut_match_kwargs.pop("base_speed")  #105 (line in Coconut source)
+            _coconut_match_temp_26 = _coconut_match_args[2] if _coconut.len(_coconut_match_args) > 2 else _coconut_match_kwargs.pop("speed_stage")  #105 (line in Coconut source)
+            _coconut_match_temp_27 = _coconut_match_args[3] if _coconut.len(_coconut_match_args) > 3 else _coconut_match_kwargs.pop("speed_nature")  #105 (line in Coconut source)
+            _coconut_match_temp_28 = _coconut_match_args[4] if _coconut.len(_coconut_match_args) > 4 else _coconut_match_kwargs.pop("level")  #105 (line in Coconut source)
+            if ((isinstance)(_coconut_match_temp_26, Stage)) and ((isinstance)(_coconut_match_temp_27, Nature)):  #105 (line in Coconut source)
+                _coconut_match_temp_17 = _coconut.getattr(str, "_coconut_is_data", False) or _coconut.isinstance(str, _coconut.tuple) and _coconut.all(_coconut.getattr(_coconut_x, "_coconut_is_data", False) for _coconut_x in str)  # type: ignore  #105 (line in Coconut source)
+                _coconut_match_temp_22 = _coconut.getattr(int, "_coconut_is_data", False) or _coconut.isinstance(int, _coconut.tuple) and _coconut.all(_coconut.getattr(_coconut_x, "_coconut_is_data", False) for _coconut_x in int)  # type: ignore  #105 (line in Coconut source)
+                _coconut_match_set_name_speed_stage = _coconut_match_temp_26  #105 (line in Coconut source)
+                _coconut_match_set_name_speed_nature = _coconut_match_temp_27  #105 (line in Coconut source)
+                _coconut_match_temp_29 = _coconut.getattr(int, "_coconut_is_data", False) or _coconut.isinstance(int, _coconut.tuple) and _coconut.all(_coconut.getattr(_coconut_x, "_coconut_is_data", False) for _coconut_x in int)  # type: ignore  #105 (line in Coconut source)
+                if not _coconut_match_kwargs:  #105 (line in Coconut source)
+                    _coconut_match_check_7 = True  #105 (line in Coconut source)
+        if _coconut_match_check_7:  #105 (line in Coconut source)
+            _coconut_match_check_7 = False  #105 (line in Coconut source)
+            if not _coconut_match_check_7:  #105 (line in Coconut source)
+                _coconut_match_set_name_name = _coconut_sentinel  #105 (line in Coconut source)
+                if (_coconut_match_temp_17) and (_coconut.isinstance(_coconut_match_temp_16, str)) and (_coconut.len(_coconut_match_temp_16) >= 1):  #105 (line in Coconut source)
+                    _coconut_match_set_name_name = _coconut_match_temp_16[0]  #105 (line in Coconut source)
+                    _coconut_match_temp_18 = _coconut.len(_coconut_match_temp_16) <= _coconut.max(1, _coconut.len(_coconut_match_temp_16.__match_args__)) and _coconut.all(i in _coconut.getattr(_coconut_match_temp_16, "_coconut_data_defaults", {}) and _coconut_match_temp_16[i] == _coconut.getattr(_coconut_match_temp_16, "_coconut_data_defaults", {})[i] for i in _coconut.range(1, _coconut.len(_coconut_match_temp_16.__match_args__))) if _coconut.hasattr(_coconut_match_temp_16, "__match_args__") else _coconut.len(_coconut_match_temp_16) == 1  # type: ignore  #105 (line in Coconut source)
+                    if _coconut_match_temp_18:  #105 (line in Coconut source)
+                        _coconut_match_check_7 = True  #105 (line in Coconut source)
+                if _coconut_match_check_7:  #105 (line in Coconut source)
+                    if _coconut_match_set_name_name is not _coconut_sentinel:  #105 (line in Coconut source)
+                        name = _coconut_match_set_name_name  #105 (line in Coconut source)
+
+            if not _coconut_match_check_7:  #105 (line in Coconut source)
+                if (not _coconut_match_temp_17) and (_coconut.isinstance(_coconut_match_temp_16, str)):  #105 (line in Coconut source)
+                    _coconut_match_check_7 = True  #105 (line in Coconut source)
+                if _coconut_match_check_7:  #105 (line in Coconut source)
+                    _coconut_match_check_7 = False  #105 (line in Coconut source)
+                    if not _coconut_match_check_7:  #105 (line in Coconut source)
+                        _coconut_match_set_name_name = _coconut_sentinel  #105 (line in Coconut source)
+                        if _coconut.type(_coconut_match_temp_16) in _coconut_self_match_types:  #105 (line in Coconut source)
+                            _coconut_match_set_name_name = _coconut_match_temp_16  #105 (line in Coconut source)
+                            _coconut_match_check_7 = True  #105 (line in Coconut source)
+                        if _coconut_match_check_7:  #105 (line in Coconut source)
+                            if _coconut_match_set_name_name is not _coconut_sentinel:  #105 (line in Coconut source)
+                                name = _coconut_match_set_name_name  #105 (line in Coconut source)
+
+                    if not _coconut_match_check_7:  #105 (line in Coconut source)
+                        _coconut_match_set_name_name = _coconut_sentinel  #105 (line in Coconut source)
+                        if not _coconut.type(_coconut_match_temp_16) in _coconut_self_match_types:  #105 (line in Coconut source)
+                            _coconut_match_temp_19 = _coconut.getattr(str, '__match_args__', ())  # type: _coconut.typing.Any  # type: ignore  #105 (line in Coconut source)
+                            if not _coconut.isinstance(_coconut_match_temp_19, _coconut.tuple):  #105 (line in Coconut source)
+                                raise _coconut.TypeError("str.__match_args__ must be a tuple")  #105 (line in Coconut source)
+                            if _coconut.len(_coconut_match_temp_19) < 1:  #105 (line in Coconut source)
+                                raise _coconut.TypeError("too many positional args in class match (pattern requires 1; 'str' only supports %s)" % (_coconut.len(_coconut_match_temp_19),))  #105 (line in Coconut source)
+                            _coconut_match_temp_20 = _coconut.getattr(_coconut_match_temp_16, _coconut_match_temp_19[0], _coconut_sentinel)  #105 (line in Coconut source)
+                            if _coconut_match_temp_20 is not _coconut_sentinel:  #105 (line in Coconut source)
+                                _coconut_match_set_name_name = _coconut_match_temp_20  #105 (line in Coconut source)
+                                _coconut_match_check_7 = True  #105 (line in Coconut source)
+                        if _coconut_match_check_7:  #105 (line in Coconut source)
+                            if _coconut_match_set_name_name is not _coconut_sentinel:  #105 (line in Coconut source)
+                                name = _coconut_match_set_name_name  #105 (line in Coconut source)
+
+
+
+
+        if _coconut_match_check_7:  #105 (line in Coconut source)
+            _coconut_match_check_7 = False  #105 (line in Coconut source)
+            if not _coconut_match_check_7:  #105 (line in Coconut source)
+                _coconut_match_set_name_base_speed = _coconut_sentinel  #105 (line in Coconut source)
+                if (_coconut_match_temp_22) and (_coconut.isinstance(_coconut_match_temp_21, int)) and (_coconut.len(_coconut_match_temp_21) >= 1):  #105 (line in Coconut source)
+                    _coconut_match_set_name_base_speed = _coconut_match_temp_21[0]  #105 (line in Coconut source)
+                    _coconut_match_temp_23 = _coconut.len(_coconut_match_temp_21) <= _coconut.max(1, _coconut.len(_coconut_match_temp_21.__match_args__)) and _coconut.all(i in _coconut.getattr(_coconut_match_temp_21, "_coconut_data_defaults", {}) and _coconut_match_temp_21[i] == _coconut.getattr(_coconut_match_temp_21, "_coconut_data_defaults", {})[i] for i in _coconut.range(1, _coconut.len(_coconut_match_temp_21.__match_args__))) if _coconut.hasattr(_coconut_match_temp_21, "__match_args__") else _coconut.len(_coconut_match_temp_21) == 1  # type: ignore  #105 (line in Coconut source)
+                    if _coconut_match_temp_23:  #105 (line in Coconut source)
+                        _coconut_match_check_7 = True  #105 (line in Coconut source)
+                if _coconut_match_check_7:  #105 (line in Coconut source)
+                    if _coconut_match_set_name_base_speed is not _coconut_sentinel:  #105 (line in Coconut source)
+                        base_speed = _coconut_match_set_name_base_speed  #105 (line in Coconut source)
+
+            if not _coconut_match_check_7:  #105 (line in Coconut source)
+                if (not _coconut_match_temp_22) and (_coconut.isinstance(_coconut_match_temp_21, int)):  #105 (line in Coconut source)
+                    _coconut_match_check_7 = True  #105 (line in Coconut source)
+                if _coconut_match_check_7:  #105 (line in Coconut source)
+                    _coconut_match_check_7 = False  #105 (line in Coconut source)
+                    if not _coconut_match_check_7:  #105 (line in Coconut source)
+                        _coconut_match_set_name_base_speed = _coconut_sentinel  #105 (line in Coconut source)
+                        if _coconut.type(_coconut_match_temp_21) in _coconut_self_match_types:  #105 (line in Coconut source)
+                            _coconut_match_set_name_base_speed = _coconut_match_temp_21  #105 (line in Coconut source)
+                            _coconut_match_check_7 = True  #105 (line in Coconut source)
+                        if _coconut_match_check_7:  #105 (line in Coconut source)
+                            if _coconut_match_set_name_base_speed is not _coconut_sentinel:  #105 (line in Coconut source)
+                                base_speed = _coconut_match_set_name_base_speed  #105 (line in Coconut source)
+
+                    if not _coconut_match_check_7:  #105 (line in Coconut source)
+                        _coconut_match_set_name_base_speed = _coconut_sentinel  #105 (line in Coconut source)
+                        if not _coconut.type(_coconut_match_temp_21) in _coconut_self_match_types:  #105 (line in Coconut source)
+                            _coconut_match_temp_24 = _coconut.getattr(int, '__match_args__', ())  # type: _coconut.typing.Any  # type: ignore  #105 (line in Coconut source)
+                            if not _coconut.isinstance(_coconut_match_temp_24, _coconut.tuple):  #105 (line in Coconut source)
+                                raise _coconut.TypeError("int.__match_args__ must be a tuple")  #105 (line in Coconut source)
+                            if _coconut.len(_coconut_match_temp_24) < 1:  #105 (line in Coconut source)
+                                raise _coconut.TypeError("too many positional args in class match (pattern requires 1; 'int' only supports %s)" % (_coconut.len(_coconut_match_temp_24),))  #105 (line in Coconut source)
+                            _coconut_match_temp_25 = _coconut.getattr(_coconut_match_temp_21, _coconut_match_temp_24[0], _coconut_sentinel)  #105 (line in Coconut source)
+                            if _coconut_match_temp_25 is not _coconut_sentinel:  #105 (line in Coconut source)
+                                _coconut_match_set_name_base_speed = _coconut_match_temp_25  #105 (line in Coconut source)
+                                _coconut_match_check_7 = True  #105 (line in Coconut source)
+                        if _coconut_match_check_7:  #105 (line in Coconut source)
+                            if _coconut_match_set_name_base_speed is not _coconut_sentinel:  #105 (line in Coconut source)
+                                base_speed = _coconut_match_set_name_base_speed  #105 (line in Coconut source)
+
+
+
+
+        if _coconut_match_check_7:  #105 (line in Coconut source)
+            _coconut_match_check_7 = False  #105 (line in Coconut source)
+            if not _coconut_match_check_7:  #105 (line in Coconut source)
+                _coconut_match_set_name_level = _coconut_sentinel  #105 (line in Coconut source)
+                if (_coconut_match_temp_29) and (_coconut.isinstance(_coconut_match_temp_28, int)) and (_coconut.len(_coconut_match_temp_28) >= 1):  #105 (line in Coconut source)
+                    _coconut_match_set_name_level = _coconut_match_temp_28[0]  #105 (line in Coconut source)
+                    _coconut_match_temp_30 = _coconut.len(_coconut_match_temp_28) <= _coconut.max(1, _coconut.len(_coconut_match_temp_28.__match_args__)) and _coconut.all(i in _coconut.getattr(_coconut_match_temp_28, "_coconut_data_defaults", {}) and _coconut_match_temp_28[i] == _coconut.getattr(_coconut_match_temp_28, "_coconut_data_defaults", {})[i] for i in _coconut.range(1, _coconut.len(_coconut_match_temp_28.__match_args__))) if _coconut.hasattr(_coconut_match_temp_28, "__match_args__") else _coconut.len(_coconut_match_temp_28) == 1  # type: ignore  #105 (line in Coconut source)
+                    if _coconut_match_temp_30:  #105 (line in Coconut source)
+                        _coconut_match_check_7 = True  #105 (line in Coconut source)
+                if _coconut_match_check_7:  #105 (line in Coconut source)
+                    if _coconut_match_set_name_level is not _coconut_sentinel:  #105 (line in Coconut source)
+                        level = _coconut_match_set_name_level  #105 (line in Coconut source)
+
+            if not _coconut_match_check_7:  #105 (line in Coconut source)
+                if (not _coconut_match_temp_29) and (_coconut.isinstance(_coconut_match_temp_28, int)):  #105 (line in Coconut source)
+                    _coconut_match_check_7 = True  #105 (line in Coconut source)
+                if _coconut_match_check_7:  #105 (line in Coconut source)
+                    _coconut_match_check_7 = False  #105 (line in Coconut source)
+                    if not _coconut_match_check_7:  #105 (line in Coconut source)
+                        _coconut_match_set_name_level = _coconut_sentinel  #105 (line in Coconut source)
+                        if _coconut.type(_coconut_match_temp_28) in _coconut_self_match_types:  #105 (line in Coconut source)
+                            _coconut_match_set_name_level = _coconut_match_temp_28  #105 (line in Coconut source)
+                            _coconut_match_check_7 = True  #105 (line in Coconut source)
+                        if _coconut_match_check_7:  #105 (line in Coconut source)
+                            if _coconut_match_set_name_level is not _coconut_sentinel:  #105 (line in Coconut source)
+                                level = _coconut_match_set_name_level  #105 (line in Coconut source)
+
+                    if not _coconut_match_check_7:  #105 (line in Coconut source)
+                        _coconut_match_set_name_level = _coconut_sentinel  #105 (line in Coconut source)
+                        if not _coconut.type(_coconut_match_temp_28) in _coconut_self_match_types:  #105 (line in Coconut source)
+                            _coconut_match_temp_31 = _coconut.getattr(int, '__match_args__', ())  # type: _coconut.typing.Any  # type: ignore  #105 (line in Coconut source)
+                            if not _coconut.isinstance(_coconut_match_temp_31, _coconut.tuple):  #105 (line in Coconut source)
+                                raise _coconut.TypeError("int.__match_args__ must be a tuple")  #105 (line in Coconut source)
+                            if _coconut.len(_coconut_match_temp_31) < 1:  #105 (line in Coconut source)
+                                raise _coconut.TypeError("too many positional args in class match (pattern requires 1; 'int' only supports %s)" % (_coconut.len(_coconut_match_temp_31),))  #105 (line in Coconut source)
+                            _coconut_match_temp_32 = _coconut.getattr(_coconut_match_temp_28, _coconut_match_temp_31[0], _coconut_sentinel)  #105 (line in Coconut source)
+                            if _coconut_match_temp_32 is not _coconut_sentinel:  #105 (line in Coconut source)
+                                _coconut_match_set_name_level = _coconut_match_temp_32  #105 (line in Coconut source)
+                                _coconut_match_check_7 = True  #105 (line in Coconut source)
+                        if _coconut_match_check_7:  #105 (line in Coconut source)
+                            if _coconut_match_set_name_level is not _coconut_sentinel:  #105 (line in Coconut source)
+                                level = _coconut_match_set_name_level  #105 (line in Coconut source)
+
+
+
+
+        if _coconut_match_check_7:  #105 (line in Coconut source)
+            if _coconut_match_set_name_speed_stage is not _coconut_sentinel:  #105 (line in Coconut source)
+                speed_stage = _coconut_match_set_name_speed_stage  #105 (line in Coconut source)
+            if _coconut_match_set_name_speed_nature is not _coconut_sentinel:  #105 (line in Coconut source)
+                speed_nature = _coconut_match_set_name_speed_nature  #105 (line in Coconut source)
+
+        if not _coconut_match_check_7:  #105 (line in Coconut source)
+            raise _coconut_FunctionMatchError('data PokemonSpeed(', _coconut_match_args)  #105 (line in Coconut source)
+
+        return _coconut.tuple.__new__(_coconut_cls, (name, base_speed, speed_stage, speed_nature, level))  #105 (line in Coconut source)
+    def __str__(self):  #105 (line in Coconut source)
+        return self.speed_stage.modifier_str() + self.name + str(self.speed_nature)  #112 (line in Coconut source)
+
+    @property  #113 (line in Coconut source)
+    @_coconut_tco  #114 (line in Coconut source)
+    def stat(self):  #114 (line in Coconut source)
+        return _coconut_tail_call(calc_stat, self.base_speed, self.speed_stage, self.speed_nature, self.level)  #114 (line in Coconut source)
+
+
+_coconut_call_set_names(PokemonSpeed)  #116 (line in Coconut source)
+def get_all_speeds(url, level, natures):  #116 (line in Coconut source)
+    for mon, stage, nature in cartesian_product(get_mons(url), important_stages, natures):  #117 (line in Coconut source)
+        yield PokemonSpeed(mon.name, mon.base_stats.speed, stage, nature, level)  #122 (line in Coconut source)
+
+
+
+important_natures = _coconut.dict((("outspeed", (Helpful, Neutral)), ("underspeed", (Helpful, Neutral, Uninvested, Harmful))))  #125 (line in Coconut source)
+
+def get_benchmarks(url, level, underspeed=False):  #138 (line in Coconut source)
+    natures = important_natures["underspeed" if underspeed else "outspeed"]  #139 (line in Coconut source)
+    speeds = set(get_all_speeds(url, level, natures))  #140 (line in Coconut source)
+
+    benchmarks = defaultdict(_coconut_partial(defaultdict, list))  # type: dict[int, dict[Stage, list[PokemonSpeed]]]  #142 (line in Coconut source)
+    if "__annotations__" not in _coconut.locals():  #142 (line in Coconut source)
+        __annotations__ = {}  # type: ignore  #142 (line in Coconut source)
+    __annotations__["benchmarks"] = dict[int, dict[Stage, list[PokemonSpeed]]]  #142 (line in Coconut source)
+    for stage in important_stages:  #143 (line in Coconut source)
+        base_speed = 1000 if underspeed else 1  #144 (line in Coconut source)
+        unused_speeds = speeds.copy()  #145 (line in Coconut source)
+        while unused_speeds:  #146 (line in Coconut source)
+            check_speed = (stage.apply)(base_speed)  #147 (line in Coconut source)
+            for pokemon_speed in tuple(unused_speeds):  #148 (line in Coconut source)
+                if (((_coconut.operator.lt) if underspeed else (_coconut.operator.gt)))(check_speed, pokemon_speed.stat):  #149 (line in Coconut source)
+                    benchmarks[base_speed][stage].append(pokemon_speed)  #150 (line in Coconut source)
+                    unused_speeds.remove(pokemon_speed)  #151 (line in Coconut source)
+            base_speed += -1 if underspeed else 1  #152 (line in Coconut source)
+    return benchmarks  #153 (line in Coconut source)
+
+
+
+def write_csv(filename, url, level, **kwargs):  #156 (line in Coconut source)
+    benchmarks = get_benchmarks(url, level, **kwargs)  #157 (line in Coconut source)
+    with open(filename, "w", newline="") as csvfile:  #158 (line in Coconut source)
+        writer = csv.writer(csvfile)  #159 (line in Coconut source)
+        writer.writerow(["Speed: \\ Stage:",] + [str(stage) for stage in important_stages])  #160 (line in Coconut source)
+        for base_speed in (sorted)(benchmarks, reverse=True):  #161 (line in Coconut source)
+            row = [base_speed,]  #162 (line in Coconut source)
+            for stage in important_stages:  #163 (line in Coconut source)
+                pokemon_speeds = benchmarks[base_speed][stage]  #164 (line in Coconut source)
+                row.append((", ".join)((map)(str, pokemon_speeds)))  #165 (line in Coconut source)
+            writer.writerow(row)  #170 (line in Coconut source)
 
-        return str(self) + " "  #78 (line in Coconut source)
 
 
-_coconut_call_set_names(Stage)  #80 (line in Coconut source)
-important_stages = (Stage(-1), Stage(0), Stage(-1, stat_modifier=2), Stage(+1), Stage(+2), Stage(+1, stat_modifier=2))  #80 (line in Coconut source)
-
-
-@_coconut_tco  #92 (line in Coconut source)
-def calc_stat(base, stage=Stage(0), nature=Helpful, level=50, ev=252, iv=31,):  #92 (line in Coconut source)
-    return _coconut_tail_call((stage.apply), (nature.apply)(((2 * base) + iv + ev // 4) * level // 100 + 5))  #92 (line in Coconut source)
-
-
-
-class PokemonSpeed(_coconut.collections.namedtuple("PokemonSpeed", ('name', 'base_speed', 'speed_stage', 'speed_nature', 'level'))):  #106 (line in Coconut source)
-    __slots__ = ()  #106 (line in Coconut source)
-    _coconut_is_data = True  #106 (line in Coconut source)
-    __match_args__ = ('name', 'base_speed', 'speed_stage', 'speed_nature', 'level')  #106 (line in Coconut source)
-    def __add__(self, other): return _coconut.NotImplemented  #106 (line in Coconut source)
-    def __mul__(self, other): return _coconut.NotImplemented  #106 (line in Coconut source)
-    def __rmul__(self, other): return _coconut.NotImplemented  #106 (line in Coconut source)
-    __ne__ = _coconut.object.__ne__  #106 (line in Coconut source)
-    def __eq__(self, other):  #106 (line in Coconut source)
-        return self.__class__ is other.__class__ and _coconut.tuple.__eq__(self, other)  #106 (line in Coconut source)
-    def __hash__(self):  #106 (line in Coconut source)
-        return _coconut.tuple.__hash__(self) ^ hash(self.__class__)  #106 (line in Coconut source)
-    def __new__(_coconut_cls, _coconut_match_first_arg=_coconut_sentinel, *_coconut_match_args, **_coconut_match_kwargs):  #106 (line in Coconut source)
-        _coconut_match_check_7 = False  #106 (line in Coconut source)
-        _coconut_match_set_name_speed_stage = _coconut_sentinel  #106 (line in Coconut source)
-        _coconut_match_set_name_speed_nature = _coconut_sentinel  #106 (line in Coconut source)
-        _coconut_FunctionMatchError = _coconut_get_function_match_error()  #106 (line in Coconut source)
-        if _coconut_match_first_arg is not _coconut_sentinel:  #106 (line in Coconut source)
-            _coconut_match_args = (_coconut_match_first_arg,) + _coconut_match_args  #106 (line in Coconut source)
-        if (_coconut.len(_coconut_match_args) <= 5) and (_coconut.sum((_coconut.len(_coconut_match_args) > 0, "name" in _coconut_match_kwargs)) == 1) and (_coconut.sum((_coconut.len(_coconut_match_args) > 1, "base_speed" in _coconut_match_kwargs)) == 1) and (_coconut.sum((_coconut.len(_coconut_match_args) > 2, "speed_stage" in _coconut_match_kwargs)) == 1) and (_coconut.sum((_coconut.len(_coconut_match_args) > 3, "speed_nature" in _coconut_match_kwargs)) == 1) and (_coconut.sum((_coconut.len(_coconut_match_args) > 4, "level" in _coconut_match_kwargs)) == 1):  #106 (line in Coconut source)
-            _coconut_match_temp_16 = _coconut_match_args[0] if _coconut.len(_coconut_match_args) > 0 else _coconut_match_kwargs.pop("name")  #106 (line in Coconut source)
-            _coconut_match_temp_21 = _coconut_match_args[1] if _coconut.len(_coconut_match_args) > 1 else _coconut_match_kwargs.pop("base_speed")  #106 (line in Coconut source)
-            _coconut_match_temp_26 = _coconut_match_args[2] if _coconut.len(_coconut_match_args) > 2 else _coconut_match_kwargs.pop("speed_stage")  #106 (line in Coconut source)
-            _coconut_match_temp_27 = _coconut_match_args[3] if _coconut.len(_coconut_match_args) > 3 else _coconut_match_kwargs.pop("speed_nature")  #106 (line in Coconut source)
-            _coconut_match_temp_28 = _coconut_match_args[4] if _coconut.len(_coconut_match_args) > 4 else _coconut_match_kwargs.pop("level")  #106 (line in Coconut source)
-            if ((isinstance)(_coconut_match_temp_26, Stage)) and ((isinstance)(_coconut_match_temp_27, Nature)):  #106 (line in Coconut source)
-                _coconut_match_temp_17 = _coconut.getattr(str, "_coconut_is_data", False) or _coconut.isinstance(str, _coconut.tuple) and _coconut.all(_coconut.getattr(_coconut_x, "_coconut_is_data", False) for _coconut_x in str)  # type: ignore  #106 (line in Coconut source)
-                _coconut_match_temp_22 = _coconut.getattr(int, "_coconut_is_data", False) or _coconut.isinstance(int, _coconut.tuple) and _coconut.all(_coconut.getattr(_coconut_x, "_coconut_is_data", False) for _coconut_x in int)  # type: ignore  #106 (line in Coconut source)
-                _coconut_match_set_name_speed_stage = _coconut_match_temp_26  #106 (line in Coconut source)
-                _coconut_match_set_name_speed_nature = _coconut_match_temp_27  #106 (line in Coconut source)
-                _coconut_match_temp_29 = _coconut.getattr(int, "_coconut_is_data", False) or _coconut.isinstance(int, _coconut.tuple) and _coconut.all(_coconut.getattr(_coconut_x, "_coconut_is_data", False) for _coconut_x in int)  # type: ignore  #106 (line in Coconut source)
-                if not _coconut_match_kwargs:  #106 (line in Coconut source)
-                    _coconut_match_check_7 = True  #106 (line in Coconut source)
-        if _coconut_match_check_7:  #106 (line in Coconut source)
-            _coconut_match_check_7 = False  #106 (line in Coconut source)
-            if not _coconut_match_check_7:  #106 (line in Coconut source)
-                _coconut_match_set_name_name = _coconut_sentinel  #106 (line in Coconut source)
-                if (_coconut_match_temp_17) and (_coconut.isinstance(_coconut_match_temp_16, str)) and (_coconut.len(_coconut_match_temp_16) >= 1):  #106 (line in Coconut source)
-                    _coconut_match_set_name_name = _coconut_match_temp_16[0]  #106 (line in Coconut source)
-                    _coconut_match_temp_18 = _coconut.len(_coconut_match_temp_16) <= _coconut.max(1, _coconut.len(_coconut_match_temp_16.__match_args__)) and _coconut.all(i in _coconut.getattr(_coconut_match_temp_16, "_coconut_data_defaults", {}) and _coconut_match_temp_16[i] == _coconut.getattr(_coconut_match_temp_16, "_coconut_data_defaults", {})[i] for i in _coconut.range(1, _coconut.len(_coconut_match_temp_16.__match_args__))) if _coconut.hasattr(_coconut_match_temp_16, "__match_args__") else _coconut.len(_coconut_match_temp_16) == 1  # type: ignore  #106 (line in Coconut source)
-                    if _coconut_match_temp_18:  #106 (line in Coconut source)
-                        _coconut_match_check_7 = True  #106 (line in Coconut source)
-                if _coconut_match_check_7:  #106 (line in Coconut source)
-                    if _coconut_match_set_name_name is not _coconut_sentinel:  #106 (line in Coconut source)
-                        name = _coconut_match_set_name_name  #106 (line in Coconut source)
-
-            if not _coconut_match_check_7:  #106 (line in Coconut source)
-                if (not _coconut_match_temp_17) and (_coconut.isinstance(_coconut_match_temp_16, str)):  #106 (line in Coconut source)
-                    _coconut_match_check_7 = True  #106 (line in Coconut source)
-                if _coconut_match_check_7:  #106 (line in Coconut source)
-                    _coconut_match_check_7 = False  #106 (line in Coconut source)
-                    if not _coconut_match_check_7:  #106 (line in Coconut source)
-                        _coconut_match_set_name_name = _coconut_sentinel  #106 (line in Coconut source)
-                        if _coconut.type(_coconut_match_temp_16) in _coconut_self_match_types:  #106 (line in Coconut source)
-                            _coconut_match_set_name_name = _coconut_match_temp_16  #106 (line in Coconut source)
-                            _coconut_match_check_7 = True  #106 (line in Coconut source)
-                        if _coconut_match_check_7:  #106 (line in Coconut source)
-                            if _coconut_match_set_name_name is not _coconut_sentinel:  #106 (line in Coconut source)
-                                name = _coconut_match_set_name_name  #106 (line in Coconut source)
-
-                    if not _coconut_match_check_7:  #106 (line in Coconut source)
-                        _coconut_match_set_name_name = _coconut_sentinel  #106 (line in Coconut source)
-                        if not _coconut.type(_coconut_match_temp_16) in _coconut_self_match_types:  #106 (line in Coconut source)
-                            _coconut_match_temp_19 = _coconut.getattr(str, '__match_args__', ())  # type: _coconut.typing.Any  # type: ignore  #106 (line in Coconut source)
-                            if not _coconut.isinstance(_coconut_match_temp_19, _coconut.tuple):  #106 (line in Coconut source)
-                                raise _coconut.TypeError("str.__match_args__ must be a tuple")  #106 (line in Coconut source)
-                            if _coconut.len(_coconut_match_temp_19) < 1:  #106 (line in Coconut source)
-                                raise _coconut.TypeError("too many positional args in class match (pattern requires 1; 'str' only supports %s)" % (_coconut.len(_coconut_match_temp_19),))  #106 (line in Coconut source)
-                            _coconut_match_temp_20 = _coconut.getattr(_coconut_match_temp_16, _coconut_match_temp_19[0], _coconut_sentinel)  #106 (line in Coconut source)
-                            if _coconut_match_temp_20 is not _coconut_sentinel:  #106 (line in Coconut source)
-                                _coconut_match_set_name_name = _coconut_match_temp_20  #106 (line in Coconut source)
-                                _coconut_match_check_7 = True  #106 (line in Coconut source)
-                        if _coconut_match_check_7:  #106 (line in Coconut source)
-                            if _coconut_match_set_name_name is not _coconut_sentinel:  #106 (line in Coconut source)
-                                name = _coconut_match_set_name_name  #106 (line in Coconut source)
-
-
-
-
-        if _coconut_match_check_7:  #106 (line in Coconut source)
-            _coconut_match_check_7 = False  #106 (line in Coconut source)
-            if not _coconut_match_check_7:  #106 (line in Coconut source)
-                _coconut_match_set_name_base_speed = _coconut_sentinel  #106 (line in Coconut source)
-                if (_coconut_match_temp_22) and (_coconut.isinstance(_coconut_match_temp_21, int)) and (_coconut.len(_coconut_match_temp_21) >= 1):  #106 (line in Coconut source)
-                    _coconut_match_set_name_base_speed = _coconut_match_temp_21[0]  #106 (line in Coconut source)
-                    _coconut_match_temp_23 = _coconut.len(_coconut_match_temp_21) <= _coconut.max(1, _coconut.len(_coconut_match_temp_21.__match_args__)) and _coconut.all(i in _coconut.getattr(_coconut_match_temp_21, "_coconut_data_defaults", {}) and _coconut_match_temp_21[i] == _coconut.getattr(_coconut_match_temp_21, "_coconut_data_defaults", {})[i] for i in _coconut.range(1, _coconut.len(_coconut_match_temp_21.__match_args__))) if _coconut.hasattr(_coconut_match_temp_21, "__match_args__") else _coconut.len(_coconut_match_temp_21) == 1  # type: ignore  #106 (line in Coconut source)
-                    if _coconut_match_temp_23:  #106 (line in Coconut source)
-                        _coconut_match_check_7 = True  #106 (line in Coconut source)
-                if _coconut_match_check_7:  #106 (line in Coconut source)
-                    if _coconut_match_set_name_base_speed is not _coconut_sentinel:  #106 (line in Coconut source)
-                        base_speed = _coconut_match_set_name_base_speed  #106 (line in Coconut source)
-
-            if not _coconut_match_check_7:  #106 (line in Coconut source)
-                if (not _coconut_match_temp_22) and (_coconut.isinstance(_coconut_match_temp_21, int)):  #106 (line in Coconut source)
-                    _coconut_match_check_7 = True  #106 (line in Coconut source)
-                if _coconut_match_check_7:  #106 (line in Coconut source)
-                    _coconut_match_check_7 = False  #106 (line in Coconut source)
-                    if not _coconut_match_check_7:  #106 (line in Coconut source)
-                        _coconut_match_set_name_base_speed = _coconut_sentinel  #106 (line in Coconut source)
-                        if _coconut.type(_coconut_match_temp_21) in _coconut_self_match_types:  #106 (line in Coconut source)
-                            _coconut_match_set_name_base_speed = _coconut_match_temp_21  #106 (line in Coconut source)
-                            _coconut_match_check_7 = True  #106 (line in Coconut source)
-                        if _coconut_match_check_7:  #106 (line in Coconut source)
-                            if _coconut_match_set_name_base_speed is not _coconut_sentinel:  #106 (line in Coconut source)
-                                base_speed = _coconut_match_set_name_base_speed  #106 (line in Coconut source)
-
-                    if not _coconut_match_check_7:  #106 (line in Coconut source)
-                        _coconut_match_set_name_base_speed = _coconut_sentinel  #106 (line in Coconut source)
-                        if not _coconut.type(_coconut_match_temp_21) in _coconut_self_match_types:  #106 (line in Coconut source)
-                            _coconut_match_temp_24 = _coconut.getattr(int, '__match_args__', ())  # type: _coconut.typing.Any  # type: ignore  #106 (line in Coconut source)
-                            if not _coconut.isinstance(_coconut_match_temp_24, _coconut.tuple):  #106 (line in Coconut source)
-                                raise _coconut.TypeError("int.__match_args__ must be a tuple")  #106 (line in Coconut source)
-                            if _coconut.len(_coconut_match_temp_24) < 1:  #106 (line in Coconut source)
-                                raise _coconut.TypeError("too many positional args in class match (pattern requires 1; 'int' only supports %s)" % (_coconut.len(_coconut_match_temp_24),))  #106 (line in Coconut source)
-                            _coconut_match_temp_25 = _coconut.getattr(_coconut_match_temp_21, _coconut_match_temp_24[0], _coconut_sentinel)  #106 (line in Coconut source)
-                            if _coconut_match_temp_25 is not _coconut_sentinel:  #106 (line in Coconut source)
-                                _coconut_match_set_name_base_speed = _coconut_match_temp_25  #106 (line in Coconut source)
-                                _coconut_match_check_7 = True  #106 (line in Coconut source)
-                        if _coconut_match_check_7:  #106 (line in Coconut source)
-                            if _coconut_match_set_name_base_speed is not _coconut_sentinel:  #106 (line in Coconut source)
-                                base_speed = _coconut_match_set_name_base_speed  #106 (line in Coconut source)
-
-
-
-
-        if _coconut_match_check_7:  #106 (line in Coconut source)
-            _coconut_match_check_7 = False  #106 (line in Coconut source)
-            if not _coconut_match_check_7:  #106 (line in Coconut source)
-                _coconut_match_set_name_level = _coconut_sentinel  #106 (line in Coconut source)
-                if (_coconut_match_temp_29) and (_coconut.isinstance(_coconut_match_temp_28, int)) and (_coconut.len(_coconut_match_temp_28) >= 1):  #106 (line in Coconut source)
-                    _coconut_match_set_name_level = _coconut_match_temp_28[0]  #106 (line in Coconut source)
-                    _coconut_match_temp_30 = _coconut.len(_coconut_match_temp_28) <= _coconut.max(1, _coconut.len(_coconut_match_temp_28.__match_args__)) and _coconut.all(i in _coconut.getattr(_coconut_match_temp_28, "_coconut_data_defaults", {}) and _coconut_match_temp_28[i] == _coconut.getattr(_coconut_match_temp_28, "_coconut_data_defaults", {})[i] for i in _coconut.range(1, _coconut.len(_coconut_match_temp_28.__match_args__))) if _coconut.hasattr(_coconut_match_temp_28, "__match_args__") else _coconut.len(_coconut_match_temp_28) == 1  # type: ignore  #106 (line in Coconut source)
-                    if _coconut_match_temp_30:  #106 (line in Coconut source)
-                        _coconut_match_check_7 = True  #106 (line in Coconut source)
-                if _coconut_match_check_7:  #106 (line in Coconut source)
-                    if _coconut_match_set_name_level is not _coconut_sentinel:  #106 (line in Coconut source)
-                        level = _coconut_match_set_name_level  #106 (line in Coconut source)
-
-            if not _coconut_match_check_7:  #106 (line in Coconut source)
-                if (not _coconut_match_temp_29) and (_coconut.isinstance(_coconut_match_temp_28, int)):  #106 (line in Coconut source)
-                    _coconut_match_check_7 = True  #106 (line in Coconut source)
-                if _coconut_match_check_7:  #106 (line in Coconut source)
-                    _coconut_match_check_7 = False  #106 (line in Coconut source)
-                    if not _coconut_match_check_7:  #106 (line in Coconut source)
-                        _coconut_match_set_name_level = _coconut_sentinel  #106 (line in Coconut source)
-                        if _coconut.type(_coconut_match_temp_28) in _coconut_self_match_types:  #106 (line in Coconut source)
-                            _coconut_match_set_name_level = _coconut_match_temp_28  #106 (line in Coconut source)
-                            _coconut_match_check_7 = True  #106 (line in Coconut source)
-                        if _coconut_match_check_7:  #106 (line in Coconut source)
-                            if _coconut_match_set_name_level is not _coconut_sentinel:  #106 (line in Coconut source)
-                                level = _coconut_match_set_name_level  #106 (line in Coconut source)
-
-                    if not _coconut_match_check_7:  #106 (line in Coconut source)
-                        _coconut_match_set_name_level = _coconut_sentinel  #106 (line in Coconut source)
-                        if not _coconut.type(_coconut_match_temp_28) in _coconut_self_match_types:  #106 (line in Coconut source)
-                            _coconut_match_temp_31 = _coconut.getattr(int, '__match_args__', ())  # type: _coconut.typing.Any  # type: ignore  #106 (line in Coconut source)
-                            if not _coconut.isinstance(_coconut_match_temp_31, _coconut.tuple):  #106 (line in Coconut source)
-                                raise _coconut.TypeError("int.__match_args__ must be a tuple")  #106 (line in Coconut source)
-                            if _coconut.len(_coconut_match_temp_31) < 1:  #106 (line in Coconut source)
-                                raise _coconut.TypeError("too many positional args in class match (pattern requires 1; 'int' only supports %s)" % (_coconut.len(_coconut_match_temp_31),))  #106 (line in Coconut source)
-                            _coconut_match_temp_32 = _coconut.getattr(_coconut_match_temp_28, _coconut_match_temp_31[0], _coconut_sentinel)  #106 (line in Coconut source)
-                            if _coconut_match_temp_32 is not _coconut_sentinel:  #106 (line in Coconut source)
-                                _coconut_match_set_name_level = _coconut_match_temp_32  #106 (line in Coconut source)
-                                _coconut_match_check_7 = True  #106 (line in Coconut source)
-                        if _coconut_match_check_7:  #106 (line in Coconut source)
-                            if _coconut_match_set_name_level is not _coconut_sentinel:  #106 (line in Coconut source)
-                                level = _coconut_match_set_name_level  #106 (line in Coconut source)
-
-
-
-
-        if _coconut_match_check_7:  #106 (line in Coconut source)
-            if _coconut_match_set_name_speed_stage is not _coconut_sentinel:  #106 (line in Coconut source)
-                speed_stage = _coconut_match_set_name_speed_stage  #106 (line in Coconut source)
-            if _coconut_match_set_name_speed_nature is not _coconut_sentinel:  #106 (line in Coconut source)
-                speed_nature = _coconut_match_set_name_speed_nature  #106 (line in Coconut source)
-
-        if not _coconut_match_check_7:  #106 (line in Coconut source)
-            raise _coconut_FunctionMatchError('data PokemonSpeed(', _coconut_match_args)  #106 (line in Coconut source)
-
-        return _coconut.tuple.__new__(_coconut_cls, (name, base_speed, speed_stage, speed_nature, level))  #106 (line in Coconut source)
-    def __str__(self):  #106 (line in Coconut source)
-        return self.speed_stage.modifier_str() + self.name + str(self.speed_nature)  #113 (line in Coconut source)
-
-    @property  #114 (line in Coconut source)
-    @_coconut_tco  #115 (line in Coconut source)
-    def stat(self):  #115 (line in Coconut source)
-        return _coconut_tail_call(calc_stat, self.base_speed, self.speed_stage, self.speed_nature, self.level)  #115 (line in Coconut source)
-
-
-_coconut_call_set_names(PokemonSpeed)  #117 (line in Coconut source)
-def get_all_speeds(url, level):  #117 (line in Coconut source)
-    for mon, stage, nature in cartesian_product(get_mons(url), important_stages, important_natures):  #118 (line in Coconut source)
-        yield PokemonSpeed(mon.name, mon.base_stats.speed, stage, nature, level)  #123 (line in Coconut source)
-
-
-
-def get_outspeed_benchmarks(url, level):  #126 (line in Coconut source)
-    outspeed_benchmarks = defaultdict(_coconut_partial(defaultdict, list))  # type: dict[int, dict[Stage, list[PokemonSpeed]]]  #127 (line in Coconut source)
-    if "__annotations__" not in _coconut.locals():  #127 (line in Coconut source)
-        __annotations__ = {}  # type: ignore  #127 (line in Coconut source)
-    __annotations__["outspeed_benchmarks"] = 'dict[int, dict[Stage, list[PokemonSpeed]]]'  #127 (line in Coconut source)
-    speeds = set(get_all_speeds(url, level))  #128 (line in Coconut source)
-    for stage in important_stages:  #129 (line in Coconut source)
-        base_speed = 1  #130 (line in Coconut source)
-        unused_speeds = speeds.copy()  #131 (line in Coconut source)
-        while unused_speeds:  #132 (line in Coconut source)
-            check_speed = (stage.apply)(base_speed)  #133 (line in Coconut source)
-            for pokemon_speed in tuple(unused_speeds):  #134 (line in Coconut source)
-                if check_speed > pokemon_speed.stat:  #135 (line in Coconut source)
-                    outspeed_benchmarks[base_speed][stage].append(pokemon_speed)  #136 (line in Coconut source)
-                    unused_speeds.remove(pokemon_speed)  #137 (line in Coconut source)
-            base_speed += 1  #138 (line in Coconut source)
-    return outspeed_benchmarks  #139 (line in Coconut source)
-
-
-
-def write_csv(filename, url, level):  #142 (line in Coconut source)
-    outspeed_benchmarks = get_outspeed_benchmarks(url, level)  #143 (line in Coconut source)
-    with open(filename, "w", newline="") as csvfile:  #144 (line in Coconut source)
-        writer = csv.writer(csvfile)  #145 (line in Coconut source)
-        writer.writerow(["Speed: \\ Stage:",] + [str(stage) for stage in important_stages])  #146 (line in Coconut source)
-        for base_speed in (sorted)(outspeed_benchmarks, reverse=True):  #147 (line in Coconut source)
-            row = [base_speed,]  #148 (line in Coconut source)
-            for stage in important_stages:  #149 (line in Coconut source)
-                pokemon_speeds = outspeed_benchmarks[base_speed][stage]  #150 (line in Coconut source)
-                row.append((", ".join)((map)(str, pokemon_speeds)))  #151 (line in Coconut source)
-            writer.writerow(row)  #156 (line in Coconut source)
-
-
-
-def main(*, out="./outspeed_benchmarks.csv", url="https://www.pikalytics.com", level=50,):  #159 (line in Coconut source)
+def main(*, out: str="", underspeed: bool=False, url: str="https://www.pikalytics.com", level: int=50,):  #173 (line in Coconut source)
     """Write Pokemon speed tier data in csv format.
 
     :param out: The csv file to write the speed tier data to.
+    :param underspeed: Whether to calculate underspeed benchmarks instead of outspeed benchmarks.
     :param url: The Pikalytics url to get Pokemon from.
     :param level: The level of the Pokemon to compute speeds at.
-    """  #170 (line in Coconut source)
-    write_csv(out, url, level)  #171 (line in Coconut source)
+    """  #186 (line in Coconut source)
+    if not out:  #187 (line in Coconut source)
+        out = "./underspeed_benchmarks.csv" if underspeed else "./outspeed_benchmarks.csv"  #188 (line in Coconut source)
+    write_csv(out, url, level, underspeed=underspeed)  #189 (line in Coconut source)
 
 
 
-run_main = _coconut_partial(run, main)  #174 (line in Coconut source)
+run_main = _coconut_partial(run, main)  #192 (line in Coconut source)
```

### Comparing `pokespeed-1.0.1/pokespeed/__main__.py` & `pokespeed-1.1.0/pokespeed/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# __coconut_hash__ = 0xad9798d9
+# __coconut_hash__ = 0x4c4d0926
 
-# Compiled with Coconut version 3.0.4-post_dev17
+# Compiled with Coconut version 3.1.0-post_dev13
 
 # Coconut Header: -------------------------------------------------------------
 
 import sys as _coconut_sys
 import os as _coconut_os
-_coconut_header_info = ('3.0.4-post_dev17', '3', True)
+_coconut_header_info = ('3.1.0-post_dev13', '3', True)
 _coconut_cached__coconut__ = _coconut_sys.modules.get('__coconut__')
 _coconut_file_dir = _coconut_os.path.dirname(_coconut_os.path.abspath(__file__))
 _coconut_pop_path = False
-if _coconut_cached__coconut__ is None or getattr(_coconut_cached__coconut__, "_coconut_header_info", None) != _coconut_header_info and _coconut_os.path.dirname(_coconut_cached__coconut__.__file__ or "") != _coconut_file_dir:
+if _coconut_cached__coconut__ is None or getattr(_coconut_cached__coconut__, "_coconut_header_info", None) != _coconut_header_info and _coconut_os.path.dirname(_coconut_cached__coconut__.__file__ or "") != _coconut_file_dir:  # type: ignore
     if _coconut_cached__coconut__ is not None:
         _coconut_sys.modules['_coconut_cached__coconut__'] = _coconut_cached__coconut__
         del _coconut_sys.modules['__coconut__']
     _coconut_sys.path.insert(0, _coconut_file_dir)
     _coconut_pop_path = True
     _coconut_module_name = _coconut_os.path.splitext(_coconut_os.path.basename(_coconut_file_dir))[0]
-    if _coconut_module_name and _coconut_module_name[0].isalpha() and all(c.isalpha() or c.isdigit() for c in _coconut_module_name) and "__init__.py" in _coconut_os.listdir(_coconut_file_dir):
-        _coconut_full_module_name = str(_coconut_module_name + ".__coconut__")
+    if _coconut_module_name and _coconut_module_name[0].isalpha() and all(c.isalpha() or c.isdigit() for c in _coconut_module_name) and "__init__.py" in _coconut_os.listdir(_coconut_file_dir):  # type: ignore
+        _coconut_full_module_name = str(_coconut_module_name + ".__coconut__")  # type: ignore
         import __coconut__ as _coconut__coconut__
         _coconut__coconut__.__name__ = _coconut_full_module_name
-        for _coconut_v in vars(_coconut__coconut__).values():
-            if getattr(_coconut_v, "__module__", None) == '__coconut__':
+        for _coconut_v in vars(_coconut__coconut__).values():  # type: ignore
+            if getattr(_coconut_v, "__module__", None) == '__coconut__':  # type: ignore
                 try:
                     _coconut_v.__module__ = _coconut_full_module_name
                 except AttributeError:
-                    _coconut_v_type = type(_coconut_v)
-                    if getattr(_coconut_v_type, "__module__", None) == '__coconut__':
+                    _coconut_v_type = type(_coconut_v)  # type: ignore
+                    if getattr(_coconut_v_type, "__module__", None) == '__coconut__':  # type: ignore
                         _coconut_v_type.__module__ = _coconut_full_module_name
         _coconut_sys.modules[_coconut_full_module_name] = _coconut__coconut__
 from __coconut__ import *
-from __coconut__ import _coconut_tail_call, _coconut_tco, _coconut_call_set_names, _namedtuple_of, _coconut, _coconut_Expected, _coconut_MatchError, _coconut_SupportsAdd, _coconut_SupportsMinus, _coconut_SupportsMul, _coconut_SupportsPow, _coconut_SupportsTruediv, _coconut_SupportsFloordiv, _coconut_SupportsMod, _coconut_SupportsAnd, _coconut_SupportsXor, _coconut_SupportsOr, _coconut_SupportsLshift, _coconut_SupportsRshift, _coconut_SupportsMatmul, _coconut_SupportsInv, _coconut_iter_getitem, _coconut_base_compose, _coconut_forward_compose, _coconut_back_compose, _coconut_forward_star_compose, _coconut_back_star_compose, _coconut_forward_dubstar_compose, _coconut_back_dubstar_compose, _coconut_pipe, _coconut_star_pipe, _coconut_dubstar_pipe, _coconut_back_pipe, _coconut_back_star_pipe, _coconut_back_dubstar_pipe, _coconut_none_pipe, _coconut_none_star_pipe, _coconut_none_dubstar_pipe, _coconut_bool_and, _coconut_bool_or, _coconut_none_coalesce, _coconut_minus, _coconut_map, _coconut_partial, _coconut_complex_partial, _coconut_get_function_match_error, _coconut_base_pattern_func, _coconut_addpattern, _coconut_sentinel, _coconut_assert, _coconut_raise, _coconut_mark_as_match, _coconut_reiterable, _coconut_self_match_types, _coconut_dict_merge, _coconut_exec, _coconut_comma_op, _coconut_arr_concat_op, _coconut_mk_anon_namedtuple, _coconut_matmul, _coconut_py_str, _coconut_flatten, _coconut_multiset, _coconut_back_none_pipe, _coconut_back_none_star_pipe, _coconut_back_none_dubstar_pipe, _coconut_forward_none_compose, _coconut_back_none_compose, _coconut_forward_none_star_compose, _coconut_back_none_star_compose, _coconut_forward_none_dubstar_compose, _coconut_back_none_dubstar_compose, _coconut_call_or_coefficient, _coconut_in, _coconut_not_in, _coconut_attritemgetter, _coconut_if_op
+from __coconut__ import _coconut_tail_call, _coconut_tco, _coconut_call_set_names, _namedtuple_of, _coconut, _coconut_Expected, _coconut_MatchError, _coconut_SupportsAdd, _coconut_SupportsMinus, _coconut_SupportsMul, _coconut_SupportsPow, _coconut_SupportsTruediv, _coconut_SupportsFloordiv, _coconut_SupportsMod, _coconut_SupportsAnd, _coconut_SupportsXor, _coconut_SupportsOr, _coconut_SupportsLshift, _coconut_SupportsRshift, _coconut_SupportsMatmul, _coconut_SupportsInv, _coconut_iter_getitem, _coconut_base_compose, _coconut_forward_compose, _coconut_back_compose, _coconut_forward_star_compose, _coconut_back_star_compose, _coconut_forward_dubstar_compose, _coconut_back_dubstar_compose, _coconut_pipe, _coconut_star_pipe, _coconut_dubstar_pipe, _coconut_back_pipe, _coconut_back_star_pipe, _coconut_back_dubstar_pipe, _coconut_none_pipe, _coconut_none_star_pipe, _coconut_none_dubstar_pipe, _coconut_bool_and, _coconut_bool_or, _coconut_none_coalesce, _coconut_minus, _coconut_map, _coconut_partial, _coconut_complex_partial, _coconut_get_function_match_error, _coconut_base_pattern_func, _coconut_addpattern, _coconut_sentinel, _coconut_assert, _coconut_raise, _coconut_mark_as_match, _coconut_reiterable, _coconut_self_match_types, _coconut_dict_merge, _coconut_exec, _coconut_comma_op, _coconut_arr_concat_op, _coconut_mk_anon_namedtuple, _coconut_matmul, _coconut_py_str, _coconut_flatten, _coconut_multiset, _coconut_back_none_pipe, _coconut_back_none_star_pipe, _coconut_back_none_dubstar_pipe, _coconut_forward_none_compose, _coconut_back_none_compose, _coconut_forward_none_star_compose, _coconut_back_none_star_compose, _coconut_forward_none_dubstar_compose, _coconut_back_none_dubstar_compose, _coconut_call_or_coefficient, _coconut_in, _coconut_not_in, _coconut_attritemgetter, _coconut_if_op, _coconut_CoconutWarning
 if _coconut_pop_path:
     _coconut_sys.path.pop(0)
 try:
     __file__ = _coconut_os.path.abspath(__file__) if __file__ else __file__
 except NameError:
     pass
 else:
```

### Comparing `pokespeed-1.0.1/setup.py` & `pokespeed-1.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 
 setuptools.setup(
     name="pokespeed",
-    version="1.0.1",
+    version="1.1.0",
     description="Calculate Pokemon speed tiers.",
     long_description="Run `pokespeed` to generate a csv of speed tiers.",
     url="https://github.com/evhub/pokespeed",
     author="Evan Hubinger",
     packages=setuptools.find_packages(),
     install_requires=[
         "requests",
```

