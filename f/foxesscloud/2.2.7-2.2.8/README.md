# Comparing `tmp/foxesscloud-2.2.7.tar.gz` & `tmp/foxesscloud-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "F:\python\FoxESS-Cloud\dist\.tmp-2t3nm83_\foxesscloud-2.2.7.tar", last modified: Wed May 22 17:33:54 2024, max compression
+gzip compressed data, was "F:\python\FoxESS-Cloud\dist\.tmp-3l5j7lb9\foxesscloud-2.2.8.tar", last modified: Mon May 27 13:12:26 2024, max compression
```

## Comparing `foxesscloud-2.2.7.tar` & `foxesscloud-2.2.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 17:33:54.000000 foxesscloud-2.2.7/
--rw-rw-rw-   0        0        0     1074 2023-08-27 11:13:04.000000 foxesscloud-2.2.7/LICENCE
--rw-rw-rw-   0        0        0    41962 2024-05-22 17:33:54.000000 foxesscloud-2.2.7/PKG-INFO
--rw-rw-rw-   0        0        0    41407 2024-05-22 17:15:35.000000 foxesscloud-2.2.7/README.md
--rw-rw-rw-   0        0        0      635 2024-05-19 11:23:16.000000 foxesscloud-2.2.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-22 17:33:54.000000 foxesscloud-2.2.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-22 17:33:54.000000 foxesscloud-2.2.7/src/
-drwxrwxrwx   0        0        0        0 2024-05-22 17:33:54.000000 foxesscloud-2.2.7/src/foxesscloud/
--rw-rw-rw-   0        0        0   180405 2024-05-22 17:29:15.000000 foxesscloud-2.2.7/src/foxesscloud/foxesscloud.py
--rw-rw-rw-   0        0        0   174609 2024-05-22 17:29:15.000000 foxesscloud-2.2.7/src/foxesscloud/openapi.py
-drwxrwxrwx   0        0        0        0 2024-05-22 17:33:54.000000 foxesscloud-2.2.7/src/foxesscloud.egg-info/
--rw-rw-rw-   0        0        0    41962 2024-05-22 17:33:54.000000 foxesscloud-2.2.7/src/foxesscloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-05-22 17:33:54.000000 foxesscloud-2.2.7/src/foxesscloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 17:33:54.000000 foxesscloud-2.2.7/src/foxesscloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-22 17:33:54.000000 foxesscloud-2.2.7/src/foxesscloud.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 13:12:26.000000 foxesscloud-2.2.8/
+-rw-rw-rw-   0        0        0     1074 2023-08-27 11:13:04.000000 foxesscloud-2.2.8/LICENCE
+-rw-rw-rw-   0        0        0    42891 2024-05-27 13:12:26.000000 foxesscloud-2.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0    42336 2024-05-27 11:55:42.000000 foxesscloud-2.2.8/README.md
+-rw-rw-rw-   0        0        0      635 2024-05-24 13:57:33.000000 foxesscloud-2.2.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-27 13:12:26.000000 foxesscloud-2.2.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-27 13:12:26.000000 foxesscloud-2.2.8/src/
+drwxrwxrwx   0        0        0        0 2024-05-27 13:12:26.000000 foxesscloud-2.2.8/src/foxesscloud/
+-rw-rw-rw-   0        0        0   182371 2024-05-27 12:04:52.000000 foxesscloud-2.2.8/src/foxesscloud/foxesscloud.py
+-rw-rw-rw-   0        0        0   176693 2024-05-27 12:04:52.000000 foxesscloud-2.2.8/src/foxesscloud/openapi.py
+drwxrwxrwx   0        0        0        0 2024-05-27 13:12:26.000000 foxesscloud-2.2.8/src/foxesscloud.egg-info/
+-rw-rw-rw-   0        0        0    42891 2024-05-27 13:12:26.000000 foxesscloud-2.2.8/src/foxesscloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-05-27 13:12:26.000000 foxesscloud-2.2.8/src/foxesscloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 13:12:26.000000 foxesscloud-2.2.8/src/foxesscloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-27 13:12:26.000000 foxesscloud-2.2.8/src/foxesscloud.egg-info/top_level.txt
```

### Comparing `foxesscloud-2.2.7/LICENCE` & `foxesscloud-2.2.8/LICENCE`

 * *Files identical despite different names*

### Comparing `foxesscloud-2.2.7/PKG-INFO` & `foxesscloud-2.2.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: foxesscloud
-Version: 2.2.7
-Summary: library for accessing Fox ESS cloud data using Open API
-Author-email: Tony Matthews <tony@quasair.co.uk>
-Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
-Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
 # FoxESS-Cloud
 
 <a href="https://www.buymeacoffee.com/tonym1958" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174" align="right"></a>
 This site contains sample python code for accessing the Fox cloud data via the REST API used by the Fox ESS Cloud web site and app.
 
 There is also a number of Jupyter Lab notebooks with examples of how to run the sample code.
 
@@ -118,50 +104,48 @@
 
 ## Inverter Settings
 You can change inverter settings using:
 
 ```
 f.set_min(minSocOnGrid, minSoc)
 f.set_charge(ch1, st1, en1, ch2, st2, en2)
-f.set_group(start, end, mode, min_soc, fdsoc, fdpwr)
-f.set_strategy(strategy)
-f.charge_strategy(st1, en1, st2, en2, min_soc)
-f.set_schedule(groups, enable)
+f.set_period(start, end, mode, min_soc, fdsoc, fdpwr, segment)
+f.charge_periods(st1, en1, st2, en2, min_soc)
+f.set_schedule(periods, enable)
 ```
 
 set_min() applies new SoC settings to the inverter. The parameters update battery_settings:
 + minSocOnGrid: min Soc on Grid setting e.g. 15 = 15%
 + minSoc: min Soc setting e.g. 10 = 10%
 
 set_charge() takes the charge times from the battery_settings and applies these to the inverter. The parameters are optional and will update battery_settings. You should specify all 3 parameter for a time period:
 + ch1: enable charge from grid for period 1 (True or False)
 + st1: the start time for period 1
 + en1: the end time for period 1
 + ch2: enable charge from grid for period 2 (True or False)
 + st2: the start time for period 2
 + en2: the end time for period 2
 
-set_group() returns a time segment structure that can be used to build a list of time segments for set_schedule()
+set_period() returns a period structure that can be used to build a list for set_schedule()
 + start, end, mode: required parameters. end time is exclusive e.g. end at '07:00' will set a period end time of '06:59'
 + min_soc: optional, default is 10
 + fdsoc: optional, default is 10. Used when setting a period with ForceDischarge mode
 + fdpwr: optional, default is 0. Used when setting a period with ForceDischarge mode
 + enable: sets whether this time segment is enable (1) or disabled (0). The default is enabled.
++ segment: optional, allows the parameters for the period to be passed as a dictionary instead of individual values.
 
-set_strategy() creates a list of groups from the strategy. If strategy is not provided, it uses the strategy for the current tariff.
-
-charge_strategy(): returns a list of groups that describe the strategy for the current tariff and adds the groupd required for charging:
+charge_periods(): returns a list of periods that describe the strategy for the current tariff and adds the periods required for charging:
 + st1: the start time for the period when the battery charges from the grid
 + en1: the end time for period 1
 + st2: the start time for period when the battery is held at min_soc
 + en2: the end time for period 2
 + min_soc: the min_soc to use after the charge period, when you don't want the battery to discharge below this level
 
 set_schedule() configures a list of scheduled work mode / soc changes with enable=1. If called with enable=0, any existing schedules are disabled. To enable a schedule, you must provide a list of time segments
-+ groups: a time segment or list of time segments created using f.set_group().
++ periods: a time segment or list of time segments created using f.set_period().
 + enable: 1 to enable schedules, 0 to disable schedules. The default is 1.
 
 
 ## Real Time Data
 Real time data reports the latest values for inverter variables, collected every 5 minutes:
 
 ```
@@ -355,15 +339,17 @@
 discharge_current: None       # max battery discharge current setting in A. None uses a value derrived from the inverter model
 export_limit: None            # maximum export power in kW. None uses the inverter power rating
 discharge_loss: 0.97          # loss converting battery discharge power to grid power
 pv_loss: 0.95                 # loss converting PV power to battery charge power
 grid_loss: 0.97               # loss converting grid power to battery charge power
 charge_loss: None             # loss converting charge power to residual
 inverter_power: None          # inverter power consumption in W (dynamically set)
-bms_power: 25                 # BMS power consumption in W
+bms_power: 50                 # BMS power consumption in W
+allowed_drain: 4,             # % tolerance below min_soc before float charge starts
+float_current: 4,             # BMS float charge current in A
 bat_resistance: 0.070         # internal resistance of a battery in ohms
 volt_curve: lifepo4_curve     # battery OCV from 0% to 100% SoC
 nominal_soc: 55               # SoC for nominal open circuit voltage
 generation_days: 3            # number of days to use for average generation (1-7)
 consumption_days: 3           # number of days to use for average consumption (1-7)
 consumption_span: 'week'      # 'week' = last 7 days or 'weekday' = last 7 weekdays e.g. Saturdays
 use_today: 21.0               # hour when today's generation and consumption data will be used
@@ -538,15 +524,24 @@
 + times=[("23:00", "8:00", 3), ("12:00", "16:00", 1)]
 
 'strategy' allows you to configure times when work modes will be changed. The format is a list of dictionary items, containing:
 + 'start', 'end': times in decimal hours or time format. The end time is exclusive so setting an end time of '07:00' will set a schedule that ends at '06:59'
 + 'mode': the work mode to be used from 'SelfUse', 'Feedin', 'Backup', 'ForceCharge', 'ForceDischarge'
 + 'min_soc, 'fdsoc', 'fdpwr': optional values for each work mode. The defaults are 10, 10 and 0 respectively.
 
-The strategy should not include settings for the AM/PM charge times for the tariff. These will be added by charge_needed().
+There are a number of pre-defined strategies:
++ f.flux_strategy_1: switch to self use at 5am and feed in first at 4pm.
++ f.flux_strategy_2: as above with force charge between 2am and 4am. Move the AM charge period between 4am and 5am when using this.
++ f.flux_strategy_3: as above with force discharge between 4pm and 6pm at 6kW with fdsoc at 35%
+
+```
+f.get_strategy()
+```
+
+get_strategy() creates a list of time segments from the strategy. If strategy is not provided, it uses the strategy for the current tariff. If a strategy includes settings for the AM/PM charge times for the tariff, the times will be moved so they do not conflict with the charge time used by charge_needed().
 
 
 # PV Output
 These functions produce CSV data for upload to [pvoutput.org](https://pvoutput.org) including PV generation, Export, Load and Grid consumption by day in Wh. The functions use the energy estimates created from the raw power data (see above). The estimates include PV energy generation that are not otherwise available from the Fox Cloud. Typically, the energy results are within 3% of the values reported by the meters built into the inverter.
 
 
 ## Get PV Output Data
@@ -686,15 +681,19 @@
 + 1: information reporting (default)
 + 2: more debug information, updating of inverter settings is disabled
 + 3: internal variables and values are displayed (verbose)
 
 
 # Version Info
 
-2.2.7<br>
+2.2.8<br>
+** breaking change ** rename 'groups' to 'periods' for consistency between foxesscloud and openapi.
+Updated management of battery reserve and float charging in charge_needed().
+Added Reserve level to charts in charge_needed().
+Changed bms_power setting to 50W.
 Updated contingency to allow seasonal values for winter, spring, summer and autumn.
 Update strategy mode to support ForceCharge and ForceDischarge work modes.
 Update so min_soc setting in charge_needed() over-rides min_soc in the tariff strategy.
 Fix force charge strategy mode in charge_neded() to set min_soc correctly.
 Implement 2 second delay between calls that change inverter settings.
 Added strategy mode (timed_mode=2) to charge_needed().
 Added set_strategy() and charge_strategy() to manage charging schedules and work mode changes.
```

#### html2text {}

```diff
@@ -1,16 +1,9 @@
-Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.7 Summary: library for
-accessing Fox ESS cloud data using Open API Author-email: Tony Matthews
-quasair.co.uk> Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
-Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
-LICENCE # FoxESS-Cloud _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]This site contains sample python code
-for accessing the Fox cloud data via the REST API used by the Fox ESS Cloud web
+# FoxESS-Cloud _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]This site contains sample python code for
+accessing the Fox cloud data via the REST API used by the Fox ESS Cloud web
 site and app. There is also a number of Jupyter Lab notebooks with examples of
 how to run the sample code. This project is not endorsed by, directly
 affiliated with, maintained, authorized, or sponsored by Fox ESS. Please refer
 to the [LICENCE](https://github.com/TonyM1958/FoxESS-Cloud/blob/main/LICENCE)
 for information on copyright, permissions and warranty. # Open API This module
 builds on the Fox Open API to provide a sample code and utilities that can be
 used with your inverter and batteries. + Information on the API can be found
@@ -66,149 +59,149 @@
 result also updates f.battery. get_settings() will return the battery settings
 and is equivalent to get_charge() and get_min(). The results are stored in
 f.battery_settings. The settings include minSoc, minSocOnGrid, enable charge
 from grid and the charge times. get_flag() returns the current scheduler enable
 / support flags get_schedule() returns the current work mode / soc schedule
 settings. The result is stored in f.schedule. ## Inverter Settings You can
 change inverter settings using: ``` f.set_min(minSocOnGrid, minSoc)
-f.set_charge(ch1, st1, en1, ch2, st2, en2) f.set_group(start, end, mode,
-min_soc, fdsoc, fdpwr) f.set_strategy(strategy) f.charge_strategy(st1, en1,
-st2, en2, min_soc) f.set_schedule(groups, enable) ``` set_min() applies new SoC
-settings to the inverter. The parameters update battery_settings: +
-minSocOnGrid: min Soc on Grid setting e.g. 15 = 15% + minSoc: min Soc setting
-e.g. 10 = 10% set_charge() takes the charge times from the battery_settings and
-applies these to the inverter. The parameters are optional and will update
-battery_settings. You should specify all 3 parameter for a time period: + ch1:
-enable charge from grid for period 1 (True or False) + st1: the start time for
-period 1 + en1: the end time for period 1 + ch2: enable charge from grid for
-period 2 (True or False) + st2: the start time for period 2 + en2: the end time
-for period 2 set_group() returns a time segment structure that can be used to
-build a list of time segments for set_schedule() + start, end, mode: required
-parameters. end time is exclusive e.g. end at '07:00' will set a period end
-time of '06:59' + min_soc: optional, default is 10 + fdsoc: optional, default
-is 10. Used when setting a period with ForceDischarge mode + fdpwr: optional,
-default is 0. Used when setting a period with ForceDischarge mode + enable:
-sets whether this time segment is enable (1) or disabled (0). The default is
-enabled. set_strategy() creates a list of groups from the strategy. If strategy
-is not provided, it uses the strategy for the current tariff. charge_strategy
-(): returns a list of groups that describe the strategy for the current tariff
-and adds the groupd required for charging: + st1: the start time for the period
-when the battery charges from the grid + en1: the end time for period 1 + st2:
-the start time for period when the battery is held at min_soc + en2: the end
-time for period 2 + min_soc: the min_soc to use after the charge period, when
-you don't want the battery to discharge below this level set_schedule()
-configures a list of scheduled work mode / soc changes with enable=1. If called
-with enable=0, any existing schedules are disabled. To enable a schedule, you
-must provide a list of time segments + groups: a time segment or list of time
-segments created using f.set_group(). + enable: 1 to enable schedules, 0 to
-disable schedules. The default is 1. ## Real Time Data Real time data reports
-the latest values for inverter variables, collected every 5 minutes: ```
-f.invert_ct2 = 1 f.get_vars() f.get_real(v) ``` f.invert_ct2 determines how the
-meterPower2 data is handled. When invert_ct2 = 0, meterPower2 produces +ve
-power values during secondary generation. If meterPower2 produces -ve power
-values during secondary generation, setting invert_ct2 = 1 will flip the values
-so they are +ve when generating. The default setting is 1 (invert). f.get_vars
-() returns the list of variables that can be queried. This also stores the
-information: + f.var_table: a table, indexed by variable that contains
-information such as the name and unit. ++ f.var_list: a list of all the
-variables that are available There are also pre-defined lists: + power_vars
-lists the main power variables provided by the inverter + battery_vars lists
-the main variables relevant to the battery / BMS f.get_real returns the latest
-values for a list of variables. + v is a variable, or list of variables. The
-default is to return the latest value for all available variables ## History
-Data History data reports inverter variables, collected every 5 minutes, on a
-given date / time and period: ``` f.get_history(time_span, d, v, summary, save,
-load, plot) ``` + time_span determines the period covered by the data, for
-example, 'hour', 'day' or 'week'. The default is 'hour' + d is a date and time
-in the format 'YYYY-MM-DD HH:MM:SS'. The default is today's date and time. d
-may also be a list of dates + v is a variable, or list of variables (see above)
-+ summary is optional - see below + save: set to the root part of a filename to
+f.set_charge(ch1, st1, en1, ch2, st2, en2) f.set_period(start, end, mode,
+min_soc, fdsoc, fdpwr, segment) f.charge_periods(st1, en1, st2, en2, min_soc)
+f.set_schedule(periods, enable) ``` set_min() applies new SoC settings to the
+inverter. The parameters update battery_settings: + minSocOnGrid: min Soc on
+Grid setting e.g. 15 = 15% + minSoc: min Soc setting e.g. 10 = 10% set_charge()
+takes the charge times from the battery_settings and applies these to the
+inverter. The parameters are optional and will update battery_settings. You
+should specify all 3 parameter for a time period: + ch1: enable charge from
+grid for period 1 (True or False) + st1: the start time for period 1 + en1: the
+end time for period 1 + ch2: enable charge from grid for period 2 (True or
+False) + st2: the start time for period 2 + en2: the end time for period 2
+set_period() returns a period structure that can be used to build a list for
+set_schedule() + start, end, mode: required parameters. end time is exclusive
+e.g. end at '07:00' will set a period end time of '06:59' + min_soc: optional,
+default is 10 + fdsoc: optional, default is 10. Used when setting a period with
+ForceDischarge mode + fdpwr: optional, default is 0. Used when setting a period
+with ForceDischarge mode + enable: sets whether this time segment is enable (1)
+or disabled (0). The default is enabled. + segment: optional, allows the
+parameters for the period to be passed as a dictionary instead of individual
+values. charge_periods(): returns a list of periods that describe the strategy
+for the current tariff and adds the periods required for charging: + st1: the
+start time for the period when the battery charges from the grid + en1: the end
+time for period 1 + st2: the start time for period when the battery is held at
+min_soc + en2: the end time for period 2 + min_soc: the min_soc to use after
+the charge period, when you don't want the battery to discharge below this
+level set_schedule() configures a list of scheduled work mode / soc changes
+with enable=1. If called with enable=0, any existing schedules are disabled. To
+enable a schedule, you must provide a list of time segments + periods: a time
+segment or list of time segments created using f.set_period(). + enable: 1 to
+enable schedules, 0 to disable schedules. The default is 1. ## Real Time Data
+Real time data reports the latest values for inverter variables, collected
+every 5 minutes: ``` f.invert_ct2 = 1 f.get_vars() f.get_real(v) ```
+f.invert_ct2 determines how the meterPower2 data is handled. When invert_ct2 =
+0, meterPower2 produces +ve power values during secondary generation. If
+meterPower2 produces -ve power values during secondary generation, setting
+invert_ct2 = 1 will flip the values so they are +ve when generating. The
+default setting is 1 (invert). f.get_vars() returns the list of variables that
+can be queried. This also stores the information: + f.var_table: a table,
+indexed by variable that contains information such as the name and unit. ++
+f.var_list: a list of all the variables that are available There are also pre-
+defined lists: + power_vars lists the main power variables provided by the
+inverter + battery_vars lists the main variables relevant to the battery / BMS
+f.get_real returns the latest values for a list of variables. + v is a
+variable, or list of variables. The default is to return the latest value for
+all available variables ## History Data History data reports inverter
+variables, collected every 5 minutes, on a given date / time and period: ```
+f.get_history(time_span, d, v, summary, save, load, plot) ``` + time_span
+determines the period covered by the data, for example, 'hour', 'day' or
+'week'. The default is 'hour' + d is a date and time in the format 'YYYY-MM-DD
+HH:MM:SS'. The default is today's date and time. d may also be a list of dates
++ v is a variable, or list of variables (see above) + summary is optional - see
+below + save: set to the root part of a filename to save the results + load:
+set to the full filename to load previously saved results + plot is optional. 1
+plots the results with a chart per unit and per day. 2 plots multiple days on
+the same chart. Default is 0, no plots The setting for invert_ct2 is applied to
+history data for meterPower2, so +ve values are returned for secondary
+generation. f.sample_time is set to the sample time in minutes for the data
+processed, rounded to f.sample_rounding samples per minute. Data generation for
+the full list of raw_vars can be slow and return a lot of data, so it's best to
+select the vars you want from the list if you can. For example, this Jupyter
+Lab cell will load an inverter and return power data at 5 minute intervals for
+the 17th June 2023: ``` d = '2023-06-17 00:00:00' result=f.get_history('day',
+d=d, v=f.power_vars) ``` Setting the optional parameter 'summary' when calling
+get_raw() provides a summary of the raw data + summary = 0: basic history data,
+no summary + summary = 1: summary is calculated + summary = 2: summary is
+calculated and raw data is removed to save time / space + summary = 3: as (2)
+but for energy only, an hourly cumulative state is also generated, similar to
+the state used in Home Assistant long term statistics The summary includes the
+following attributes: + count: the number of data points + average: the average
+value of the data points + max: the maximum value of the data points +
+max_time: the time when the maximum value occured (HH:MM) + min: the minimum
+value of the data points + min_time: the time when the minimum value occured
+(HH:MM) For power values (unit = kW), the summary performs a Riemann sum of the
+data, integrating kW over the day to estimate energy in kWh. In this case, the
+following attributes are also added: + kwh: the total energy generated or
+consumed + kwh_off: the total energy consumed or generated during the off-peak
+time of use + kwh_peak: the total energy consumed or generated during the peak
+time of use + kwh_neg: the total energy from -ve power flow (all other totals
+are based on +ve power flow) This example shows power graphs for today and
+yesterday: ![image](https://github.com/TonyM1958/FoxESS-Cloud/assets/63789168/
+d84c55c9-4f4c-431d-bc55-d7796b7e4fea) ## Report Data Report data provides
+information on the energy produced by the inverter, battery charge and
+discharge energy, grid consumption and feed-in energy and home energy
+consumption: ``` f.get_report(report_type, d, v, summary, save, load, plot,
+station) ``` + report_type sets the period covered by the report and is one of
+'day', 'week', 'month', 'year': + when 'day' is selected, energy is reported
+each hour through the day + when 'week' is selected, energy is reported for the
+7 days up to and including the date + when 'month' is selected, energy is
+reported each day through the month + when 'year' is selected, energy is
+reported each month through the year + d is a date and time in the format
+'YYYY-MM-DD HH:MM:SS'. The default is yesterday. d may also be a list of dates
++ v is a variable, or list of variables. The default is to use report_vars +
+summary is optional - see below + save: set to the root part of a filename to
 save the results + load: set to the full filename to load previously saved
-results + plot is optional. 1 plots the results with a chart per unit and per
-day. 2 plots multiple days on the same chart. Default is 0, no plots The
-setting for invert_ct2 is applied to history data for meterPower2, so +ve
-values are returned for secondary generation. f.sample_time is set to the
-sample time in minutes for the data processed, rounded to f.sample_rounding
-samples per minute. Data generation for the full list of raw_vars can be slow
-and return a lot of data, so it's best to select the vars you want from the
-list if you can. For example, this Jupyter Lab cell will load an inverter and
-return power data at 5 minute intervals for the 17th June 2023: ``` d = '2023-
-06-17 00:00:00' result=f.get_history('day', d=d, v=f.power_vars) ``` Setting
-the optional parameter 'summary' when calling get_raw() provides a summary of
-the raw data + summary = 0: basic history data, no summary + summary = 1:
-summary is calculated + summary = 2: summary is calculated and raw data is
-removed to save time / space + summary = 3: as (2) but for energy only, an
-hourly cumulative state is also generated, similar to the state used in Home
-Assistant long term statistics The summary includes the following attributes: +
-count: the number of data points + average: the average value of the data
-points + max: the maximum value of the data points + max_time: the time when
-the maximum value occured (HH:MM) + min: the minimum value of the data points +
-min_time: the time when the minimum value occured (HH:MM) For power values
-(unit = kW), the summary performs a Riemann sum of the data, integrating kW
-over the day to estimate energy in kWh. In this case, the following attributes
-are also added: + kwh: the total energy generated or consumed + kwh_off: the
-total energy consumed or generated during the off-peak time of use + kwh_peak:
-the total energy consumed or generated during the peak time of use + kwh_neg:
-the total energy from -ve power flow (all other totals are based on +ve power
-flow) This example shows power graphs for today and yesterday: ![image](https:/
-/github.com/TonyM1958/FoxESS-Cloud/assets/63789168/d84c55c9-4f4c-431d-bc55-
-d7796b7e4fea) ## Report Data Report data provides information on the energy
-produced by the inverter, battery charge and discharge energy, grid consumption
-and feed-in energy and home energy consumption: ``` f.get_report(report_type,
-d, v, summary, save, load, plot, station) ``` + report_type sets the period
-covered by the report and is one of 'day', 'week', 'month', 'year': + when
-'day' is selected, energy is reported each hour through the day + when 'week'
-is selected, energy is reported for the 7 days up to and including the date +
-when 'month' is selected, energy is reported each day through the month + when
-'year' is selected, energy is reported each month through the year + d is a
-date and time in the format 'YYYY-MM-DD HH:MM:SS'. The default is yesterday. d
-may also be a list of dates + v is a variable, or list of variables. The
-default is to use report_vars + summary is optional - see below + save: set to
-the root part of a filename to save the results + load: set to the full
-filename to load previously saved results + plot is optional. 1 to plot results
-+ station is optional. 1 gets data for a site (using f.station_id), 0 gets data
-for a device (using f.device_id). The default is 0. The list of variables that
-can be reported on is stored in f.report_vars. Note that reporting by 'day'
-produces inaccurate hourly data, where the sum does not reconcile with the
-daily total given in the monthly report. To correct this, reporting by day also
-gets the monthly data and uses the daily total to correctly report the total.
-Setting the optional parameter 'summary' when calling get_report() provides a
-summary of the report data: + summary = 0: basic report data, no summary.
-report_type cannot be 'week' + summary = 1: summary is calculated + summary =
-2: corrected total only is reported to save time / space. report_type must be
-'day' The result data for each variable includes the following attributes when
-summary=2 + 'variable': name of the data set + 'total': corrected total of the
-data items When summary=1, the following items are also added: + 'data':
-'index' and 'value' of each data point + 'date': that was used to produce the
-report + 'count': the number of data items + 'sum': the sum of the data items +
-'max': the biggest value in 'data' + 'max_index': the index of the biggest
-value in 'data' + 'min': the smallest value in 'data' + 'min_index': the index
-of the smallest value in 'data' + 'average': corrected average of the data
-items For example, this Jupyter Lab cell will report energy data by day for the
-month of June 2023: ``` d = '2023-06-17' result=f.get_report('month', d=d) ```
-This example plots weekly data: ![image](https://github.com/TonyM1958/FoxESS-
-Cloud/assets/63789168/f408a010-9600-4b2f-979f-83e32d960586) # Built-in
-Utilities and Operations The previous section provides functions that can be
-used to access and control your inverter. This section covers utilities and
-operations that build upon these functions. ## Charge Needed Uses forecast PV
-yield for tomorrow to work out if charging from grid is needed tonight to
-deliver the expected consumption for tomorrow. If charging is needed, the
-charge times are configured. If charging is not needed, the charge times are
-cleared. The results are sent to the inverter. ``` f.charge_needed(forecast,
-force_charge, forecast_selection, forecast_times, update_setings, show_data,
-show_plot) ``` All the parameters are optional: + forecast: the kWh expected
-tomorrow (optional, see below) + force_charge: 1 any remaining time in a charge
-period has force charge / min_soc set, 2 charging uses the entire charge
-period, 0 None (default) + forecast_selection: if set to 1, settings are only
-updated if there is a forecast. Default is 0, generation is used when forecasts
-are not available + forecast_times: a list of hours when forecasts can be
-obtained. By default, the forecast times for the selected tariff are used (see
-below) + update_settings: 0 no changes, 1 update charge settings. The default
-is 0 + show_data: 1 show battery SoC data, 2 show battery Residual data, 3 show
-timed data, 4 show timed data before and after charging. The default is 1. +
+results + plot is optional. 1 to plot results + station is optional. 1 gets
+data for a site (using f.station_id), 0 gets data for a device (using
+f.device_id). The default is 0. The list of variables that can be reported on
+is stored in f.report_vars. Note that reporting by 'day' produces inaccurate
+hourly data, where the sum does not reconcile with the daily total given in the
+monthly report. To correct this, reporting by day also gets the monthly data
+and uses the daily total to correctly report the total. Setting the optional
+parameter 'summary' when calling get_report() provides a summary of the report
+data: + summary = 0: basic report data, no summary. report_type cannot be
+'week' + summary = 1: summary is calculated + summary = 2: corrected total only
+is reported to save time / space. report_type must be 'day' The result data for
+each variable includes the following attributes when summary=2 + 'variable':
+name of the data set + 'total': corrected total of the data items When
+summary=1, the following items are also added: + 'data': 'index' and 'value' of
+each data point + 'date': that was used to produce the report + 'count': the
+number of data items + 'sum': the sum of the data items + 'max': the biggest
+value in 'data' + 'max_index': the index of the biggest value in 'data' +
+'min': the smallest value in 'data' + 'min_index': the index of the smallest
+value in 'data' + 'average': corrected average of the data items For example,
+this Jupyter Lab cell will report energy data by day for the month of June
+2023: ``` d = '2023-06-17' result=f.get_report('month', d=d) ``` This example
+plots weekly data: ![image](https://github.com/TonyM1958/FoxESS-Cloud/assets/
+63789168/f408a010-9600-4b2f-979f-83e32d960586) # Built-in Utilities and
+Operations The previous section provides functions that can be used to access
+and control your inverter. This section covers utilities and operations that
+build upon these functions. ## Charge Needed Uses forecast PV yield for
+tomorrow to work out if charging from grid is needed tonight to deliver the
+expected consumption for tomorrow. If charging is needed, the charge times are
+configured. If charging is not needed, the charge times are cleared. The
+results are sent to the inverter. ``` f.charge_needed(forecast, force_charge,
+forecast_selection, forecast_times, update_setings, show_data, show_plot) ```
+All the parameters are optional: + forecast: the kWh expected tomorrow
+(optional, see below) + force_charge: 1 any remaining time in a charge period
+has force charge / min_soc set, 2 charging uses the entire charge period, 0
+None (default) + forecast_selection: if set to 1, settings are only updated if
+there is a forecast. Default is 0, generation is used when forecasts are not
+available + forecast_times: a list of hours when forecasts can be obtained. By
+default, the forecast times for the selected tariff are used (see below) +
+update_settings: 0 no changes, 1 update charge settings. The default is 0 +
+show_data: 1 show battery SoC data, 2 show battery Residual data, 3 show timed
+data, 4 show timed data before and after charging. The default is 1. +
 show_plot: 1 plot battery SoC data. 2 plot battery Residual, Generation and
 Consumption. 3 plot 2 + Charge and Discharge The default is 3 ### Modelling
 charge_needed() uses a number of models to better estimate the state of the
 battery. **Manual Consumption:** You can provide your 'annual_consumption' in
 kWh e.g. 5500. This figure is factored down to a daily consumption by dividing
 by 365 and applying **f.seasonality**. This normally decreases consumption in
 the summer and increases it in winter. Seasonality is a list of weightings by
@@ -259,82 +252,83 @@
 value derrived from the inverter model discharge_current: None # max battery
 discharge current setting in A. None uses a value derrived from the inverter
 model export_limit: None # maximum export power in kW. None uses the inverter
 power rating discharge_loss: 0.97 # loss converting battery discharge power to
 grid power pv_loss: 0.95 # loss converting PV power to battery charge power
 grid_loss: 0.97 # loss converting grid power to battery charge power
 charge_loss: None # loss converting charge power to residual inverter_power:
-None # inverter power consumption in W (dynamically set) bms_power: 25 # BMS
-power consumption in W bat_resistance: 0.070 # internal resistance of a battery
-in ohms volt_curve: lifepo4_curve # battery OCV from 0% to 100% SoC
-nominal_soc: 55 # SoC for nominal open circuit voltage generation_days: 3 #
-number of days to use for average generation (1-7) consumption_days: 3 # number
-of days to use for average consumption (1-7) consumption_span: 'week' # 'week'
-= last 7 days or 'weekday' = last 7 weekdays e.g. Saturdays use_today: 21.0 #
-hour when today's generation and consumption data will be used min_hours: 0.25
-# minimum charge time to set (in decimal hours) min_kwh: 0.5 # minimum charge
-to add in kwh solcast_adjust: 100 # % adjustment to make to Solcast forecast
-solar_adjust: 100 # % adjustment to make to Solar forecast forecast_selection:
-1 # 1 = only update charge times if forecast is available, 0 = use best
-available data. Default is 1. annual_consumption: None # optional annual
-consumption in kWh. If set, this replaces consumption history timed_mode: 0 # 0
-= None, 1 = use timed work mode, 2 = strategy mode special_contingency: 30 #
-contingency for special days when consumption might be higher special_days:
-['12-25', '12-26', '01-01'] full_charge: None # day of month (1-28) to do full
-charge or 'daily' or day of week: 'Mon', 'Tue' etc derate_temp: 21 # battery
-temperature in C when derating charge current is applied derate_step: 5 # step
-size for derating e.g. 21, 16, 11 derating: [24, 15, 10, 2] # derated charge
-current for each temperature step e.g. 21C, 16C, 11C, 6C force: 1 # 1 = disable
-strategy periods when setting charge. 0 = fail if strategy period has been set.
-data_wrap: 6 # data items to show per line target_soc: None # target soc for
-charging ``` These values are stored / available in f.charge_config. The
-default battery open circuit voltage curve versus SoC from 0% to 100% is: ```
-lifepo4_curve = [51.30, 52.00, 52.30, 52.40, 52.50, 52.60, 52.70, 52.80, 52.9,
-53.1, 53.50] ``` When operating in strategy mode (timed_mode=2), charge_needed
-will create a schedule that includes the strategy for the tariff with
-additional time segments added to charge from grid and (optionall) to stop the
-battery discharging. In other modes, charge_needed() will disable any schedules
-and set the battery charge times. This example shows the results reported by
-charge needed: ![image](https://github.com/TonyM1958/FoxESS-Cloud/assets/
-63789168/8b77956b-c326-43cd-b165-20d806b1e7e8) ## Battery Info Provides
-detailed information on the current state of the batteries: ``` f.battery_info
-(count, plot, log) f.battery_monitor(interval, run, log, save, count) ```
-battery_info() prints information on the battery and cells: + count: optional
-over-ride. The default is based on factorising the number of cells reported by
-16 or 18 to work out the number of batteries. + plot: 1 plot the cell voltages
-for each battery, 2 plot the cell temperatueres, 0 don't plot. The default is 1
-+ log: see below. Default is 0 battery_monitor() runs battery_info() in log
-mode on a schedule to provide information on the battery status over a period
-of time: + interval: the time in minutes between log entries. The default is 30
-minutes + run: the number of log entries to create. The default is 48 i.e.
-every 30 minues for 24 hours in total + log: 0 = display, 1 = log battery info,
-2 = add cell volts, 3 = add cell temps. The default is 1 + save: name of a CSV
-file to write log data to + count: optional over-ride for the number of
-batteries This is an example of the output from battery_info(): ![image](https:
-//github.com/TonyM1958/FoxESS-Cloud/assets/63789168/a8eb52b6-ce3f-4b58-bb76-
-5483d5e40fa7) ## Date Ranges ``` f.date_list(s, e, limit, span, today) ```
-Returns a list of dates in the format 'YYYY-MM-DD'. This function will not
-return dates in the future. The last date will be yesterday or today (if today
-is True). All parameters are optional: + s: start date + e: end date + limit:
-maximum number of days. The default is 200 + span: the range of dates. One of
-'day', 'week', 'month' or 'year', '2days' or 'weekday' + today: 1 allows today
-to be included, 2 allows future dates to be included. Default is 0, date list
-will stop at yesterday You can use 'span' as follows: + 'day' provides a single
-day + 'week' will provide the dates of 7 consequetive days + 'month' will
-provide the dates of the days up to the same date in the preceeding (or
-follwing) month + '2days' will provide the dates of yesterday and today +
-'weekday' will provide the dates of the same day of the week, going backwards
-(or forwards) up to 7 weeks ``` f.british_summer_time(d) # 1 if d is in Britsh
-Summer Time, 0 if not ``` ## Time Periods Times and time period settings are
-held as decimal hours. Functions for working with time strings with the format
-'HH:MM:SS' and decimal hours include: ``` f.time_hours(t, d=None) # convert
-time to decimal hours. t is a time string ('HH:MM' or 'HH:MM:SS'), d is
-optional and is the default time if s is None f.hours_time(h, mm=True,
-ss=False, day=False) # convert decimal hours to time (HH:MM:SS). mm = include
-minutes, ss = include seconds, day = include /n for day when hours > 24
+None # inverter power consumption in W (dynamically set) bms_power: 50 # BMS
+power consumption in W allowed_drain: 4, # % tolerance below min_soc before
+float charge starts float_current: 4, # BMS float charge current in A
+bat_resistance: 0.070 # internal resistance of a battery in ohms volt_curve:
+lifepo4_curve # battery OCV from 0% to 100% SoC nominal_soc: 55 # SoC for
+nominal open circuit voltage generation_days: 3 # number of days to use for
+average generation (1-7) consumption_days: 3 # number of days to use for
+average consumption (1-7) consumption_span: 'week' # 'week' = last 7 days or
+'weekday' = last 7 weekdays e.g. Saturdays use_today: 21.0 # hour when today's
+generation and consumption data will be used min_hours: 0.25 # minimum charge
+time to set (in decimal hours) min_kwh: 0.5 # minimum charge to add in kwh
+solcast_adjust: 100 # % adjustment to make to Solcast forecast solar_adjust:
+100 # % adjustment to make to Solar forecast forecast_selection: 1 # 1 = only
+update charge times if forecast is available, 0 = use best available data.
+Default is 1. annual_consumption: None # optional annual consumption in kWh. If
+set, this replaces consumption history timed_mode: 0 # 0 = None, 1 = use timed
+work mode, 2 = strategy mode special_contingency: 30 # contingency for special
+days when consumption might be higher special_days: ['12-25', '12-26', '01-01']
+full_charge: None # day of month (1-28) to do full charge or 'daily' or day of
+week: 'Mon', 'Tue' etc derate_temp: 21 # battery temperature in C when derating
+charge current is applied derate_step: 5 # step size for derating e.g. 21, 16,
+11 derating: [24, 15, 10, 2] # derated charge current for each temperature step
+e.g. 21C, 16C, 11C, 6C force: 1 # 1 = disable strategy periods when setting
+charge. 0 = fail if strategy period has been set. data_wrap: 6 # data items to
+show per line target_soc: None # target soc for charging ``` These values are
+stored / available in f.charge_config. The default battery open circuit voltage
+curve versus SoC from 0% to 100% is: ``` lifepo4_curve = [51.30, 52.00, 52.30,
+52.40, 52.50, 52.60, 52.70, 52.80, 52.9, 53.1, 53.50] ``` When operating in
+strategy mode (timed_mode=2), charge_needed will create a schedule that
+includes the strategy for the tariff with additional time segments added to
+charge from grid and (optionall) to stop the battery discharging. In other
+modes, charge_needed() will disable any schedules and set the battery charge
+times. This example shows the results reported by charge needed: ![image]
+(https://github.com/TonyM1958/FoxESS-Cloud/assets/63789168/8b77956b-c326-43cd-
+b165-20d806b1e7e8) ## Battery Info Provides detailed information on the current
+state of the batteries: ``` f.battery_info(count, plot, log) f.battery_monitor
+(interval, run, log, save, count) ``` battery_info() prints information on the
+battery and cells: + count: optional over-ride. The default is based on
+factorising the number of cells reported by 16 or 18 to work out the number of
+batteries. + plot: 1 plot the cell voltages for each battery, 2 plot the cell
+temperatueres, 0 don't plot. The default is 1 + log: see below. Default is 0
+battery_monitor() runs battery_info() in log mode on a schedule to provide
+information on the battery status over a period of time: + interval: the time
+in minutes between log entries. The default is 30 minutes + run: the number of
+log entries to create. The default is 48 i.e. every 30 minues for 24 hours in
+total + log: 0 = display, 1 = log battery info, 2 = add cell volts, 3 = add
+cell temps. The default is 1 + save: name of a CSV file to write log data to +
+count: optional over-ride for the number of batteries This is an example of the
+output from battery_info(): ![image](https://github.com/TonyM1958/FoxESS-Cloud/
+assets/63789168/a8eb52b6-ce3f-4b58-bb76-5483d5e40fa7) ## Date Ranges ```
+f.date_list(s, e, limit, span, today) ``` Returns a list of dates in the format
+'YYYY-MM-DD'. This function will not return dates in the future. The last date
+will be yesterday or today (if today is True). All parameters are optional: +
+s: start date + e: end date + limit: maximum number of days. The default is 200
++ span: the range of dates. One of 'day', 'week', 'month' or 'year', '2days' or
+'weekday' + today: 1 allows today to be included, 2 allows future dates to be
+included. Default is 0, date list will stop at yesterday You can use 'span' as
+follows: + 'day' provides a single day + 'week' will provide the dates of 7
+consequetive days + 'month' will provide the dates of the days up to the same
+date in the preceeding (or follwing) month + '2days' will provide the dates of
+yesterday and today + 'weekday' will provide the dates of the same day of the
+week, going backwards (or forwards) up to 7 weeks ``` f.british_summer_time(d)
+# 1 if d is in Britsh Summer Time, 0 if not ``` ## Time Periods Times and time
+period settings are held as decimal hours. Functions for working with time
+strings with the format 'HH:MM:SS' and decimal hours include: ``` f.time_hours
+(t, d=None) # convert time to decimal hours. t is a time string ('HH:MM' or
+'HH:MM:SS'), d is optional and is the default time if s is None f.hours_time(h,
+mm=True, ss=False, day=False) # convert decimal hours to time (HH:MM:SS). mm =
+include minutes, ss = include seconds, day = include /n for day when hours > 24
 f.hours_in(h, {'start': a, 'end': b}) # True if decimal hour h is in the time
 period a -> b ``` ## Tariffs Tariffs configure when your battery can be charged
 and provide time of use (TOU) periods to split your grid import and export into
 peak, off-peak and shoulder times when data is uploaded to PV Ouptut. There are
 a number of different pre-configured tariffs: + Octopus Flux: off-peak from 02:
 00 to 05:00, peak from 16:00 to 19:00, forecasts from 22:00 to 23:59. Timed
 work mode change to Self Use at 7am and Feed In First at 4pm. + Intelligent
@@ -400,108 +394,118 @@
 between 12 noon and 4pm with a 1 hour period: + times=[("23:00", "8:00", 3),
 ("12:00", "16:00", 1)] 'strategy' allows you to configure times when work modes
 will be changed. The format is a list of dictionary items, containing: +
 'start', 'end': times in decimal hours or time format. The end time is
 exclusive so setting an end time of '07:00' will set a schedule that ends at
 '06:59' + 'mode': the work mode to be used from 'SelfUse', 'Feedin', 'Backup',
 'ForceCharge', 'ForceDischarge' + 'min_soc, 'fdsoc', 'fdpwr': optional values
-for each work mode. The defaults are 10, 10 and 0 respectively. The strategy
-should not include settings for the AM/PM charge times for the tariff. These
-will be added by charge_needed(). # PV Output These functions produce CSV data
-for upload to [pvoutput.org](https://pvoutput.org) including PV generation,
-Export, Load and Grid consumption by day in Wh. The functions use the energy
-estimates created from the raw power data (see above). The estimates include PV
-energy generation that are not otherwise available from the Fox Cloud.
-Typically, the energy results are within 3% of the values reported by the
-meters built into the inverter. ## Get PV Output Data Returns CSV upload data
-using the [API format](https://pvoutput.org/help/api_specification.html#csv-
-data-parameter): ``` f.get_pvoutput(d, tou) ``` + d is the date or a list of
-dates, to get data for. The default is yesterday + tou: optional, setting tou=1
-uploads data with time of use. The default, tou=0 does not split data and is
-more accurate. You can copy and paste the output data to the pvoutput data CSV
-Loader, using the following settings: ![image](https://github.com/TonyM1958/
-FoxESS-Cloud/assets/63789168/21459cdc-a943-4e9d-a204-7efd45a422d8) For example,
-this Jupyer Lab cell will provide a CSV data upload for June 2023: ```
-f.get_pvoutput(f.date_list('2023-06-01', '2023-06-30')) ``` ## Set PV Output
-Data Loads CSV data directly using the PV Ouput API: ``` f.set_pvoutput(d,
-system_id, tou, push) ``` + d is optional and is the date, or a list of dates,
-to upload + system_id is optional and allow you to select where data is
-uploaded to (where you have more than 1 registered system) + tou: optional,
-setting tou=1 uploads data with time of use. The default, tou=0 does not split
-data and is more accurate + push: optional. 0 = do not sent to pushover, 1 =
-send summary to pushover, 2 = send first day summary only # Solar Forecasting #
-Solcast Get and display solar data from your solcast.com account using your API
-key: ``` f.solcast_api_key = "my.solcast_api_key" fcast = f.Solcast() print
-(fcast) ``` Returns a 7 day forecast. Optional parameters are: + days: number
-of days to get. The default is 7 + estimated: whether to get history /
-estimated data. 1 = yes, 0 = no. Default is 0. + reload: cached data handling.
-0 = use saved data, 1 = fetch new data, 2 = use saved data for today (default)
-+ quiet: True to stop Solcast producing progress messages Forecast data is
-saved to f.solcast_save. The default is 'solcast.txt'. ``` fcast.plot_daily()
+for each work mode. The defaults are 10, 10 and 0 respectively. There are a
+number of pre-defined strategies: + f.flux_strategy_1: switch to self use at
+5am and feed in first at 4pm. + f.flux_strategy_2: as above with force charge
+between 2am and 4am. Move the AM charge period between 4am and 5am when using
+this. + f.flux_strategy_3: as above with force discharge between 4pm and 6pm at
+6kW with fdsoc at 35% ``` f.get_strategy() ``` get_strategy() creates a list of
+time segments from the strategy. If strategy is not provided, it uses the
+strategy for the current tariff. If a strategy includes settings for the AM/PM
+charge times for the tariff, the times will be moved so they do not conflict
+with the charge time used by charge_needed(). # PV Output These functions
+produce CSV data for upload to [pvoutput.org](https://pvoutput.org) including
+PV generation, Export, Load and Grid consumption by day in Wh. The functions
+use the energy estimates created from the raw power data (see above). The
+estimates include PV energy generation that are not otherwise available from
+the Fox Cloud. Typically, the energy results are within 3% of the values
+reported by the meters built into the inverter. ## Get PV Output Data Returns
+CSV upload data using the [API format](https://pvoutput.org/help/
+api_specification.html#csv-data-parameter): ``` f.get_pvoutput(d, tou) ``` + d
+is the date or a list of dates, to get data for. The default is yesterday +
+tou: optional, setting tou=1 uploads data with time of use. The default, tou=0
+does not split data and is more accurate. You can copy and paste the output
+data to the pvoutput data CSV Loader, using the following settings: ![image]
+(https://github.com/TonyM1958/FoxESS-Cloud/assets/63789168/21459cdc-a943-4e9d-
+a204-7efd45a422d8) For example, this Jupyer Lab cell will provide a CSV data
+upload for June 2023: ``` f.get_pvoutput(f.date_list('2023-06-01', '2023-06-
+30')) ``` ## Set PV Output Data Loads CSV data directly using the PV Ouput API:
+``` f.set_pvoutput(d, system_id, tou, push) ``` + d is optional and is the
+date, or a list of dates, to upload + system_id is optional and allow you to
+select where data is uploaded to (where you have more than 1 registered system)
++ tou: optional, setting tou=1 uploads data with time of use. The default,
+tou=0 does not split data and is more accurate + push: optional. 0 = do not
+sent to pushover, 1 = send summary to pushover, 2 = send first day summary only
+# Solar Forecasting # Solcast Get and display solar data from your solcast.com
+account using your API key: ``` f.solcast_api_key = "my.solcast_api_key" fcast
+= f.Solcast() print(fcast) ``` Returns a 7 day forecast. Optional parameters
+are: + days: number of days to get. The default is 7 + estimated: whether to
+get history / estimated data. 1 = yes, 0 = no. Default is 0. + reload: cached
+data handling. 0 = use saved data, 1 = fetch new data, 2 = use saved data for
+today (default) + quiet: True to stop Solcast producing progress messages
+Forecast data is saved to f.solcast_save. The default is 'solcast.txt'. ```
+fcast.plot_daily() fcast.plot_hourly(day) ``` Plots the estimate / forecast
+data. plot_daily() plots the daily yield. plot_hourly() plots each day
+separately. + day: optional. 'today', 'tomorrow', 'all' or a specific list of
+dates. The default is to plot today and tomorrow # Forecast.solar Get and
+display solar data from forecast.solar for today and tomorrow: ```
+f.solar_array('South', lat=51.1789, lon=-1.8262, kwp=6.4) ``` You need to
+configure your solar arrays by calling f.solar_array(). This takes the
+following parameters: + name: the name of each of your arrays + lat: the
+latitude where the array is located. The default is Stonehenge. + lon: the
+longitude where the array is located. The default is Stonehenge. + dec: the
+declination of the array - 0 is lying flat and 90 is vertical. Default is 30 +
+az: azimuth of the array. 0 is pointing due South, -90 is pointing East, 90 is
+pointing West. The default is 0 + kwp: the size of the array in kWp. The
+default is 5kWp + dam: damping factor. Default is None + inv: inverter power
+limit (when the array will clip). The default is None + hor: a list of values
+describing obstructions on the horizon Add one array for each string attached
+to your inverter. If your solar production is limited by clipping, set the
+inverter power so the forecast better matches your generation. See the [API
+documentation](https://doc.forecast.solar/api) for more information on
+parameter values. ``` fcast = f.Solar() print(fcast) ``` Returns a forecast for
+today and tomorrow. Optional parameters are: + reload: cached data handling. 0
+= use saved data, 1 = fetch new data, 2 = use saved data for today (default) +
+quiet: set to True to stop Solar producing progress messages Forecast data is
+saved to f.solar_save. The default is 'solar.txt'. ``` fcast.plot_daily()
 fcast.plot_hourly(day) ``` Plots the estimate / forecast data. plot_daily()
 plots the daily yield. plot_hourly() plots each day separately. + day:
 optional. 'today', 'tomorrow', 'all' or a specific list of dates. The default
-is to plot today and tomorrow # Forecast.solar Get and display solar data from
-forecast.solar for today and tomorrow: ``` f.solar_array('South', lat=51.1789,
-lon=-1.8262, kwp=6.4) ``` You need to configure your solar arrays by calling
-f.solar_array(). This takes the following parameters: + name: the name of each
-of your arrays + lat: the latitude where the array is located. The default is
-Stonehenge. + lon: the longitude where the array is located. The default is
-Stonehenge. + dec: the declination of the array - 0 is lying flat and 90 is
-vertical. Default is 30 + az: azimuth of the array. 0 is pointing due South, -
-90 is pointing East, 90 is pointing West. The default is 0 + kwp: the size of
-the array in kWp. The default is 5kWp + dam: damping factor. Default is None +
-inv: inverter power limit (when the array will clip). The default is None +
-hor: a list of values describing obstructions on the horizon Add one array for
-each string attached to your inverter. If your solar production is limited by
-clipping, set the inverter power so the forecast better matches your
-generation. See the [API documentation](https://doc.forecast.solar/api) for
-more information on parameter values. ``` fcast = f.Solar() print(fcast) ```
-Returns a forecast for today and tomorrow. Optional parameters are: + reload:
-cached data handling. 0 = use saved data, 1 = fetch new data, 2 = use saved
-data for today (default) + quiet: set to True to stop Solar producing progress
-messages Forecast data is saved to f.solar_save. The default is 'solar.txt'.
-``` fcast.plot_daily() fcast.plot_hourly(day) ``` Plots the estimate / forecast
-data. plot_daily() plots the daily yield. plot_hourly() plots each day
-separately. + day: optional. 'today', 'tomorrow', 'all' or a specific list of
-dates. The default is to plot today and tomorrow # Pushover Send messages to a
-pushover user account: ``` f.output_spool(app_key, h) f.output(s)
-f.output_close(plot, file) f.output_message(app_key, message, plot) ``` Calling
-f.output_spool() with an app key will start the system spooling output to send
-to pushover. h is an optional header to add as the first line of the message. H
-may include \
+is to plot today and tomorrow # Pushover Send messages to a pushover user
+account: ``` f.output_spool(app_key, h) f.output(s) f.output_close(plot, file)
+f.output_message(app_key, message, plot) ``` Calling f.output_spool() with an
+app key will start the system spooling output to send to pushover. h is an
+optional header to add as the first line of the message. H may include \
 >, \
 > or \
 > and these will be set to current system time and date respectively. When
 spooling is active, any calls to f.output() add lines to the spooled message.
 If appending to the message would exceed 1024 characters, the existing spooled
 message is sent and a new message spool is started. Calling f.output_close()
 will send the spooled message and optionally attach a binary image file. You
 can set plot=1 to attach the last plot file created (when f.plot_file is set)
 or specify a file. f.output_message() is a shorcut to send a message without
 spooling output. # Troubleshooting If needed, you can add the following setting
 to increase the level of information reported by the foxesscloud module: ```
 f.debug_setting = 2 ``` This setting can be: + 0: silent mode (minimal output)
 + 1: information reporting (default) + 2: more debug information, updating of
 inverter settings is disabled + 3: internal variables and values are displayed
-(verbose) # Version Info 2.2.7
-Updated contingency to allow seasonal values for winter, spring, summer and
-autumn. Update strategy mode to support ForceCharge and ForceDischarge work
-modes. Update so min_soc setting in charge_needed() over-rides min_soc in the
-tariff strategy. Fix force charge strategy mode in charge_neded() to set
-min_soc correctly. Implement 2 second delay between calls that change inverter
-settings. Added strategy mode (timed_mode=2) to charge_needed(). Added
-set_strategy() and charge_strategy() to manage charging schedules and work mode
-changes. Refactor debug messaging. Simplify charge_needed() output. Added
-'target_soc' to charge_needed() settings Fix bat_info() giving incorrect
-temperatures when API returns 0 instead of -50 where there is no battery Fix
-key error when accessing cell volts and temps using an agent / installer
-account. Ensure output is generated if get_battery() fails using battery_info
-(). Update f.avg() to include calculation of averages in lists containng None
-values. Added 'data_wrap' to charge_config. 2.1.9
+(verbose) # Version Info 2.2.8
+** breaking change ** rename 'groups' to 'periods' for consistency between
+foxesscloud and openapi. Updated management of battery reserve and float
+charging in charge_needed(). Added Reserve level to charts in charge_needed().
+Changed bms_power setting to 50W. Updated contingency to allow seasonal values
+for winter, spring, summer and autumn. Update strategy mode to support
+ForceCharge and ForceDischarge work modes. Update so min_soc setting in
+charge_needed() over-rides min_soc in the tariff strategy. Fix force charge
+strategy mode in charge_neded() to set min_soc correctly. Implement 2 second
+delay between calls that change inverter settings. Added strategy mode
+(timed_mode=2) to charge_needed(). Added set_strategy() and charge_strategy()
+to manage charging schedules and work mode changes. Refactor debug messaging.
+Simplify charge_needed() output. Added 'target_soc' to charge_needed() settings
+Fix bat_info() giving incorrect temperatures when API returns 0 instead of -50
+where there is no battery Fix key error when accessing cell volts and temps
+using an agent / installer account. Ensure output is generated if get_battery()
+fails using battery_info(). Update f.avg() to include calculation of averages
+in lists containng None values. Added 'data_wrap' to charge_config. 2.1.9
 Update get_history() to use GMT or BST when plotting instead of mixed time
 zones. Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in
 relation to work mode. Better reporting of reason for http error code. Template
 code for get_named_settings() added - not functional in this version due to
 Open API limitations. Update set_pvoutput() to allow push=2. Fix problem in
 set_pvoutput() sending summary to pushover when tou=1. Improve accuracy of time
```

### Comparing `foxesscloud-2.2.7/README.md` & `foxesscloud-2.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: foxesscloud
+Version: 2.2.8
+Summary: library for accessing Fox ESS cloud data using Open API
+Author-email: Tony Matthews <tony@quasair.co.uk>
+Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
+Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENCE
+
 # FoxESS-Cloud
 
 <a href="https://www.buymeacoffee.com/tonym1958" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174" align="right"></a>
 This site contains sample python code for accessing the Fox cloud data via the REST API used by the Fox ESS Cloud web site and app.
 
 There is also a number of Jupyter Lab notebooks with examples of how to run the sample code.
 
@@ -104,50 +118,48 @@
 
 ## Inverter Settings
 You can change inverter settings using:
 
 ```
 f.set_min(minSocOnGrid, minSoc)
 f.set_charge(ch1, st1, en1, ch2, st2, en2)
-f.set_group(start, end, mode, min_soc, fdsoc, fdpwr)
-f.set_strategy(strategy)
-f.charge_strategy(st1, en1, st2, en2, min_soc)
-f.set_schedule(groups, enable)
+f.set_period(start, end, mode, min_soc, fdsoc, fdpwr, segment)
+f.charge_periods(st1, en1, st2, en2, min_soc)
+f.set_schedule(periods, enable)
 ```
 
 set_min() applies new SoC settings to the inverter. The parameters update battery_settings:
 + minSocOnGrid: min Soc on Grid setting e.g. 15 = 15%
 + minSoc: min Soc setting e.g. 10 = 10%
 
 set_charge() takes the charge times from the battery_settings and applies these to the inverter. The parameters are optional and will update battery_settings. You should specify all 3 parameter for a time period:
 + ch1: enable charge from grid for period 1 (True or False)
 + st1: the start time for period 1
 + en1: the end time for period 1
 + ch2: enable charge from grid for period 2 (True or False)
 + st2: the start time for period 2
 + en2: the end time for period 2
 
-set_group() returns a time segment structure that can be used to build a list of time segments for set_schedule()
+set_period() returns a period structure that can be used to build a list for set_schedule()
 + start, end, mode: required parameters. end time is exclusive e.g. end at '07:00' will set a period end time of '06:59'
 + min_soc: optional, default is 10
 + fdsoc: optional, default is 10. Used when setting a period with ForceDischarge mode
 + fdpwr: optional, default is 0. Used when setting a period with ForceDischarge mode
 + enable: sets whether this time segment is enable (1) or disabled (0). The default is enabled.
++ segment: optional, allows the parameters for the period to be passed as a dictionary instead of individual values.
 
-set_strategy() creates a list of groups from the strategy. If strategy is not provided, it uses the strategy for the current tariff.
-
-charge_strategy(): returns a list of groups that describe the strategy for the current tariff and adds the groupd required for charging:
+charge_periods(): returns a list of periods that describe the strategy for the current tariff and adds the periods required for charging:
 + st1: the start time for the period when the battery charges from the grid
 + en1: the end time for period 1
 + st2: the start time for period when the battery is held at min_soc
 + en2: the end time for period 2
 + min_soc: the min_soc to use after the charge period, when you don't want the battery to discharge below this level
 
 set_schedule() configures a list of scheduled work mode / soc changes with enable=1. If called with enable=0, any existing schedules are disabled. To enable a schedule, you must provide a list of time segments
-+ groups: a time segment or list of time segments created using f.set_group().
++ periods: a time segment or list of time segments created using f.set_period().
 + enable: 1 to enable schedules, 0 to disable schedules. The default is 1.
 
 
 ## Real Time Data
 Real time data reports the latest values for inverter variables, collected every 5 minutes:
 
 ```
@@ -341,15 +353,17 @@
 discharge_current: None       # max battery discharge current setting in A. None uses a value derrived from the inverter model
 export_limit: None            # maximum export power in kW. None uses the inverter power rating
 discharge_loss: 0.97          # loss converting battery discharge power to grid power
 pv_loss: 0.95                 # loss converting PV power to battery charge power
 grid_loss: 0.97               # loss converting grid power to battery charge power
 charge_loss: None             # loss converting charge power to residual
 inverter_power: None          # inverter power consumption in W (dynamically set)
-bms_power: 25                 # BMS power consumption in W
+bms_power: 50                 # BMS power consumption in W
+allowed_drain: 4,             # % tolerance below min_soc before float charge starts
+float_current: 4,             # BMS float charge current in A
 bat_resistance: 0.070         # internal resistance of a battery in ohms
 volt_curve: lifepo4_curve     # battery OCV from 0% to 100% SoC
 nominal_soc: 55               # SoC for nominal open circuit voltage
 generation_days: 3            # number of days to use for average generation (1-7)
 consumption_days: 3           # number of days to use for average consumption (1-7)
 consumption_span: 'week'      # 'week' = last 7 days or 'weekday' = last 7 weekdays e.g. Saturdays
 use_today: 21.0               # hour when today's generation and consumption data will be used
@@ -524,15 +538,24 @@
 + times=[("23:00", "8:00", 3), ("12:00", "16:00", 1)]
 
 'strategy' allows you to configure times when work modes will be changed. The format is a list of dictionary items, containing:
 + 'start', 'end': times in decimal hours or time format. The end time is exclusive so setting an end time of '07:00' will set a schedule that ends at '06:59'
 + 'mode': the work mode to be used from 'SelfUse', 'Feedin', 'Backup', 'ForceCharge', 'ForceDischarge'
 + 'min_soc, 'fdsoc', 'fdpwr': optional values for each work mode. The defaults are 10, 10 and 0 respectively.
 
-The strategy should not include settings for the AM/PM charge times for the tariff. These will be added by charge_needed().
+There are a number of pre-defined strategies:
++ f.flux_strategy_1: switch to self use at 5am and feed in first at 4pm.
++ f.flux_strategy_2: as above with force charge between 2am and 4am. Move the AM charge period between 4am and 5am when using this.
++ f.flux_strategy_3: as above with force discharge between 4pm and 6pm at 6kW with fdsoc at 35%
+
+```
+f.get_strategy()
+```
+
+get_strategy() creates a list of time segments from the strategy. If strategy is not provided, it uses the strategy for the current tariff. If a strategy includes settings for the AM/PM charge times for the tariff, the times will be moved so they do not conflict with the charge time used by charge_needed().
 
 
 # PV Output
 These functions produce CSV data for upload to [pvoutput.org](https://pvoutput.org) including PV generation, Export, Load and Grid consumption by day in Wh. The functions use the energy estimates created from the raw power data (see above). The estimates include PV energy generation that are not otherwise available from the Fox Cloud. Typically, the energy results are within 3% of the values reported by the meters built into the inverter.
 
 
 ## Get PV Output Data
@@ -672,15 +695,19 @@
 + 1: information reporting (default)
 + 2: more debug information, updating of inverter settings is disabled
 + 3: internal variables and values are displayed (verbose)
 
 
 # Version Info
 
-2.2.7<br>
+2.2.8<br>
+** breaking change ** rename 'groups' to 'periods' for consistency between foxesscloud and openapi.
+Updated management of battery reserve and float charging in charge_needed().
+Added Reserve level to charts in charge_needed().
+Changed bms_power setting to 50W.
 Updated contingency to allow seasonal values for winter, spring, summer and autumn.
 Update strategy mode to support ForceCharge and ForceDischarge work modes.
 Update so min_soc setting in charge_needed() over-rides min_soc in the tariff strategy.
 Fix force charge strategy mode in charge_neded() to set min_soc correctly.
 Implement 2 second delay between calls that change inverter settings.
 Added strategy mode (timed_mode=2) to charge_needed().
 Added set_strategy() and charge_strategy() to manage charging schedules and work mode changes.
```

#### html2text {}

```diff
@@ -1,9 +1,16 @@
-# FoxESS-Cloud _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]This site contains sample python code for
-accessing the Fox cloud data via the REST API used by the Fox ESS Cloud web
+Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.8 Summary: library for
+accessing Fox ESS cloud data using Open API Author-email: Tony Matthews
+quasair.co.uk> Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
+Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
+Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
+LICENCE # FoxESS-Cloud _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]This site contains sample python code
+for accessing the Fox cloud data via the REST API used by the Fox ESS Cloud web
 site and app. There is also a number of Jupyter Lab notebooks with examples of
 how to run the sample code. This project is not endorsed by, directly
 affiliated with, maintained, authorized, or sponsored by Fox ESS. Please refer
 to the [LICENCE](https://github.com/TonyM1958/FoxESS-Cloud/blob/main/LICENCE)
 for information on copyright, permissions and warranty. # Open API This module
 builds on the Fox Open API to provide a sample code and utilities that can be
 used with your inverter and batteries. + Information on the API can be found
@@ -59,149 +66,149 @@
 result also updates f.battery. get_settings() will return the battery settings
 and is equivalent to get_charge() and get_min(). The results are stored in
 f.battery_settings. The settings include minSoc, minSocOnGrid, enable charge
 from grid and the charge times. get_flag() returns the current scheduler enable
 / support flags get_schedule() returns the current work mode / soc schedule
 settings. The result is stored in f.schedule. ## Inverter Settings You can
 change inverter settings using: ``` f.set_min(minSocOnGrid, minSoc)
-f.set_charge(ch1, st1, en1, ch2, st2, en2) f.set_group(start, end, mode,
-min_soc, fdsoc, fdpwr) f.set_strategy(strategy) f.charge_strategy(st1, en1,
-st2, en2, min_soc) f.set_schedule(groups, enable) ``` set_min() applies new SoC
-settings to the inverter. The parameters update battery_settings: +
-minSocOnGrid: min Soc on Grid setting e.g. 15 = 15% + minSoc: min Soc setting
-e.g. 10 = 10% set_charge() takes the charge times from the battery_settings and
-applies these to the inverter. The parameters are optional and will update
-battery_settings. You should specify all 3 parameter for a time period: + ch1:
-enable charge from grid for period 1 (True or False) + st1: the start time for
-period 1 + en1: the end time for period 1 + ch2: enable charge from grid for
-period 2 (True or False) + st2: the start time for period 2 + en2: the end time
-for period 2 set_group() returns a time segment structure that can be used to
-build a list of time segments for set_schedule() + start, end, mode: required
-parameters. end time is exclusive e.g. end at '07:00' will set a period end
-time of '06:59' + min_soc: optional, default is 10 + fdsoc: optional, default
-is 10. Used when setting a period with ForceDischarge mode + fdpwr: optional,
-default is 0. Used when setting a period with ForceDischarge mode + enable:
-sets whether this time segment is enable (1) or disabled (0). The default is
-enabled. set_strategy() creates a list of groups from the strategy. If strategy
-is not provided, it uses the strategy for the current tariff. charge_strategy
-(): returns a list of groups that describe the strategy for the current tariff
-and adds the groupd required for charging: + st1: the start time for the period
-when the battery charges from the grid + en1: the end time for period 1 + st2:
-the start time for period when the battery is held at min_soc + en2: the end
-time for period 2 + min_soc: the min_soc to use after the charge period, when
-you don't want the battery to discharge below this level set_schedule()
-configures a list of scheduled work mode / soc changes with enable=1. If called
-with enable=0, any existing schedules are disabled. To enable a schedule, you
-must provide a list of time segments + groups: a time segment or list of time
-segments created using f.set_group(). + enable: 1 to enable schedules, 0 to
-disable schedules. The default is 1. ## Real Time Data Real time data reports
-the latest values for inverter variables, collected every 5 minutes: ```
-f.invert_ct2 = 1 f.get_vars() f.get_real(v) ``` f.invert_ct2 determines how the
-meterPower2 data is handled. When invert_ct2 = 0, meterPower2 produces +ve
-power values during secondary generation. If meterPower2 produces -ve power
-values during secondary generation, setting invert_ct2 = 1 will flip the values
-so they are +ve when generating. The default setting is 1 (invert). f.get_vars
-() returns the list of variables that can be queried. This also stores the
-information: + f.var_table: a table, indexed by variable that contains
-information such as the name and unit. ++ f.var_list: a list of all the
-variables that are available There are also pre-defined lists: + power_vars
-lists the main power variables provided by the inverter + battery_vars lists
-the main variables relevant to the battery / BMS f.get_real returns the latest
-values for a list of variables. + v is a variable, or list of variables. The
-default is to return the latest value for all available variables ## History
-Data History data reports inverter variables, collected every 5 minutes, on a
-given date / time and period: ``` f.get_history(time_span, d, v, summary, save,
-load, plot) ``` + time_span determines the period covered by the data, for
-example, 'hour', 'day' or 'week'. The default is 'hour' + d is a date and time
-in the format 'YYYY-MM-DD HH:MM:SS'. The default is today's date and time. d
-may also be a list of dates + v is a variable, or list of variables (see above)
-+ summary is optional - see below + save: set to the root part of a filename to
+f.set_charge(ch1, st1, en1, ch2, st2, en2) f.set_period(start, end, mode,
+min_soc, fdsoc, fdpwr, segment) f.charge_periods(st1, en1, st2, en2, min_soc)
+f.set_schedule(periods, enable) ``` set_min() applies new SoC settings to the
+inverter. The parameters update battery_settings: + minSocOnGrid: min Soc on
+Grid setting e.g. 15 = 15% + minSoc: min Soc setting e.g. 10 = 10% set_charge()
+takes the charge times from the battery_settings and applies these to the
+inverter. The parameters are optional and will update battery_settings. You
+should specify all 3 parameter for a time period: + ch1: enable charge from
+grid for period 1 (True or False) + st1: the start time for period 1 + en1: the
+end time for period 1 + ch2: enable charge from grid for period 2 (True or
+False) + st2: the start time for period 2 + en2: the end time for period 2
+set_period() returns a period structure that can be used to build a list for
+set_schedule() + start, end, mode: required parameters. end time is exclusive
+e.g. end at '07:00' will set a period end time of '06:59' + min_soc: optional,
+default is 10 + fdsoc: optional, default is 10. Used when setting a period with
+ForceDischarge mode + fdpwr: optional, default is 0. Used when setting a period
+with ForceDischarge mode + enable: sets whether this time segment is enable (1)
+or disabled (0). The default is enabled. + segment: optional, allows the
+parameters for the period to be passed as a dictionary instead of individual
+values. charge_periods(): returns a list of periods that describe the strategy
+for the current tariff and adds the periods required for charging: + st1: the
+start time for the period when the battery charges from the grid + en1: the end
+time for period 1 + st2: the start time for period when the battery is held at
+min_soc + en2: the end time for period 2 + min_soc: the min_soc to use after
+the charge period, when you don't want the battery to discharge below this
+level set_schedule() configures a list of scheduled work mode / soc changes
+with enable=1. If called with enable=0, any existing schedules are disabled. To
+enable a schedule, you must provide a list of time segments + periods: a time
+segment or list of time segments created using f.set_period(). + enable: 1 to
+enable schedules, 0 to disable schedules. The default is 1. ## Real Time Data
+Real time data reports the latest values for inverter variables, collected
+every 5 minutes: ``` f.invert_ct2 = 1 f.get_vars() f.get_real(v) ```
+f.invert_ct2 determines how the meterPower2 data is handled. When invert_ct2 =
+0, meterPower2 produces +ve power values during secondary generation. If
+meterPower2 produces -ve power values during secondary generation, setting
+invert_ct2 = 1 will flip the values so they are +ve when generating. The
+default setting is 1 (invert). f.get_vars() returns the list of variables that
+can be queried. This also stores the information: + f.var_table: a table,
+indexed by variable that contains information such as the name and unit. ++
+f.var_list: a list of all the variables that are available There are also pre-
+defined lists: + power_vars lists the main power variables provided by the
+inverter + battery_vars lists the main variables relevant to the battery / BMS
+f.get_real returns the latest values for a list of variables. + v is a
+variable, or list of variables. The default is to return the latest value for
+all available variables ## History Data History data reports inverter
+variables, collected every 5 minutes, on a given date / time and period: ```
+f.get_history(time_span, d, v, summary, save, load, plot) ``` + time_span
+determines the period covered by the data, for example, 'hour', 'day' or
+'week'. The default is 'hour' + d is a date and time in the format 'YYYY-MM-DD
+HH:MM:SS'. The default is today's date and time. d may also be a list of dates
++ v is a variable, or list of variables (see above) + summary is optional - see
+below + save: set to the root part of a filename to save the results + load:
+set to the full filename to load previously saved results + plot is optional. 1
+plots the results with a chart per unit and per day. 2 plots multiple days on
+the same chart. Default is 0, no plots The setting for invert_ct2 is applied to
+history data for meterPower2, so +ve values are returned for secondary
+generation. f.sample_time is set to the sample time in minutes for the data
+processed, rounded to f.sample_rounding samples per minute. Data generation for
+the full list of raw_vars can be slow and return a lot of data, so it's best to
+select the vars you want from the list if you can. For example, this Jupyter
+Lab cell will load an inverter and return power data at 5 minute intervals for
+the 17th June 2023: ``` d = '2023-06-17 00:00:00' result=f.get_history('day',
+d=d, v=f.power_vars) ``` Setting the optional parameter 'summary' when calling
+get_raw() provides a summary of the raw data + summary = 0: basic history data,
+no summary + summary = 1: summary is calculated + summary = 2: summary is
+calculated and raw data is removed to save time / space + summary = 3: as (2)
+but for energy only, an hourly cumulative state is also generated, similar to
+the state used in Home Assistant long term statistics The summary includes the
+following attributes: + count: the number of data points + average: the average
+value of the data points + max: the maximum value of the data points +
+max_time: the time when the maximum value occured (HH:MM) + min: the minimum
+value of the data points + min_time: the time when the minimum value occured
+(HH:MM) For power values (unit = kW), the summary performs a Riemann sum of the
+data, integrating kW over the day to estimate energy in kWh. In this case, the
+following attributes are also added: + kwh: the total energy generated or
+consumed + kwh_off: the total energy consumed or generated during the off-peak
+time of use + kwh_peak: the total energy consumed or generated during the peak
+time of use + kwh_neg: the total energy from -ve power flow (all other totals
+are based on +ve power flow) This example shows power graphs for today and
+yesterday: ![image](https://github.com/TonyM1958/FoxESS-Cloud/assets/63789168/
+d84c55c9-4f4c-431d-bc55-d7796b7e4fea) ## Report Data Report data provides
+information on the energy produced by the inverter, battery charge and
+discharge energy, grid consumption and feed-in energy and home energy
+consumption: ``` f.get_report(report_type, d, v, summary, save, load, plot,
+station) ``` + report_type sets the period covered by the report and is one of
+'day', 'week', 'month', 'year': + when 'day' is selected, energy is reported
+each hour through the day + when 'week' is selected, energy is reported for the
+7 days up to and including the date + when 'month' is selected, energy is
+reported each day through the month + when 'year' is selected, energy is
+reported each month through the year + d is a date and time in the format
+'YYYY-MM-DD HH:MM:SS'. The default is yesterday. d may also be a list of dates
++ v is a variable, or list of variables. The default is to use report_vars +
+summary is optional - see below + save: set to the root part of a filename to
 save the results + load: set to the full filename to load previously saved
-results + plot is optional. 1 plots the results with a chart per unit and per
-day. 2 plots multiple days on the same chart. Default is 0, no plots The
-setting for invert_ct2 is applied to history data for meterPower2, so +ve
-values are returned for secondary generation. f.sample_time is set to the
-sample time in minutes for the data processed, rounded to f.sample_rounding
-samples per minute. Data generation for the full list of raw_vars can be slow
-and return a lot of data, so it's best to select the vars you want from the
-list if you can. For example, this Jupyter Lab cell will load an inverter and
-return power data at 5 minute intervals for the 17th June 2023: ``` d = '2023-
-06-17 00:00:00' result=f.get_history('day', d=d, v=f.power_vars) ``` Setting
-the optional parameter 'summary' when calling get_raw() provides a summary of
-the raw data + summary = 0: basic history data, no summary + summary = 1:
-summary is calculated + summary = 2: summary is calculated and raw data is
-removed to save time / space + summary = 3: as (2) but for energy only, an
-hourly cumulative state is also generated, similar to the state used in Home
-Assistant long term statistics The summary includes the following attributes: +
-count: the number of data points + average: the average value of the data
-points + max: the maximum value of the data points + max_time: the time when
-the maximum value occured (HH:MM) + min: the minimum value of the data points +
-min_time: the time when the minimum value occured (HH:MM) For power values
-(unit = kW), the summary performs a Riemann sum of the data, integrating kW
-over the day to estimate energy in kWh. In this case, the following attributes
-are also added: + kwh: the total energy generated or consumed + kwh_off: the
-total energy consumed or generated during the off-peak time of use + kwh_peak:
-the total energy consumed or generated during the peak time of use + kwh_neg:
-the total energy from -ve power flow (all other totals are based on +ve power
-flow) This example shows power graphs for today and yesterday: ![image](https:/
-/github.com/TonyM1958/FoxESS-Cloud/assets/63789168/d84c55c9-4f4c-431d-bc55-
-d7796b7e4fea) ## Report Data Report data provides information on the energy
-produced by the inverter, battery charge and discharge energy, grid consumption
-and feed-in energy and home energy consumption: ``` f.get_report(report_type,
-d, v, summary, save, load, plot, station) ``` + report_type sets the period
-covered by the report and is one of 'day', 'week', 'month', 'year': + when
-'day' is selected, energy is reported each hour through the day + when 'week'
-is selected, energy is reported for the 7 days up to and including the date +
-when 'month' is selected, energy is reported each day through the month + when
-'year' is selected, energy is reported each month through the year + d is a
-date and time in the format 'YYYY-MM-DD HH:MM:SS'. The default is yesterday. d
-may also be a list of dates + v is a variable, or list of variables. The
-default is to use report_vars + summary is optional - see below + save: set to
-the root part of a filename to save the results + load: set to the full
-filename to load previously saved results + plot is optional. 1 to plot results
-+ station is optional. 1 gets data for a site (using f.station_id), 0 gets data
-for a device (using f.device_id). The default is 0. The list of variables that
-can be reported on is stored in f.report_vars. Note that reporting by 'day'
-produces inaccurate hourly data, where the sum does not reconcile with the
-daily total given in the monthly report. To correct this, reporting by day also
-gets the monthly data and uses the daily total to correctly report the total.
-Setting the optional parameter 'summary' when calling get_report() provides a
-summary of the report data: + summary = 0: basic report data, no summary.
-report_type cannot be 'week' + summary = 1: summary is calculated + summary =
-2: corrected total only is reported to save time / space. report_type must be
-'day' The result data for each variable includes the following attributes when
-summary=2 + 'variable': name of the data set + 'total': corrected total of the
-data items When summary=1, the following items are also added: + 'data':
-'index' and 'value' of each data point + 'date': that was used to produce the
-report + 'count': the number of data items + 'sum': the sum of the data items +
-'max': the biggest value in 'data' + 'max_index': the index of the biggest
-value in 'data' + 'min': the smallest value in 'data' + 'min_index': the index
-of the smallest value in 'data' + 'average': corrected average of the data
-items For example, this Jupyter Lab cell will report energy data by day for the
-month of June 2023: ``` d = '2023-06-17' result=f.get_report('month', d=d) ```
-This example plots weekly data: ![image](https://github.com/TonyM1958/FoxESS-
-Cloud/assets/63789168/f408a010-9600-4b2f-979f-83e32d960586) # Built-in
-Utilities and Operations The previous section provides functions that can be
-used to access and control your inverter. This section covers utilities and
-operations that build upon these functions. ## Charge Needed Uses forecast PV
-yield for tomorrow to work out if charging from grid is needed tonight to
-deliver the expected consumption for tomorrow. If charging is needed, the
-charge times are configured. If charging is not needed, the charge times are
-cleared. The results are sent to the inverter. ``` f.charge_needed(forecast,
-force_charge, forecast_selection, forecast_times, update_setings, show_data,
-show_plot) ``` All the parameters are optional: + forecast: the kWh expected
-tomorrow (optional, see below) + force_charge: 1 any remaining time in a charge
-period has force charge / min_soc set, 2 charging uses the entire charge
-period, 0 None (default) + forecast_selection: if set to 1, settings are only
-updated if there is a forecast. Default is 0, generation is used when forecasts
-are not available + forecast_times: a list of hours when forecasts can be
-obtained. By default, the forecast times for the selected tariff are used (see
-below) + update_settings: 0 no changes, 1 update charge settings. The default
-is 0 + show_data: 1 show battery SoC data, 2 show battery Residual data, 3 show
-timed data, 4 show timed data before and after charging. The default is 1. +
+results + plot is optional. 1 to plot results + station is optional. 1 gets
+data for a site (using f.station_id), 0 gets data for a device (using
+f.device_id). The default is 0. The list of variables that can be reported on
+is stored in f.report_vars. Note that reporting by 'day' produces inaccurate
+hourly data, where the sum does not reconcile with the daily total given in the
+monthly report. To correct this, reporting by day also gets the monthly data
+and uses the daily total to correctly report the total. Setting the optional
+parameter 'summary' when calling get_report() provides a summary of the report
+data: + summary = 0: basic report data, no summary. report_type cannot be
+'week' + summary = 1: summary is calculated + summary = 2: corrected total only
+is reported to save time / space. report_type must be 'day' The result data for
+each variable includes the following attributes when summary=2 + 'variable':
+name of the data set + 'total': corrected total of the data items When
+summary=1, the following items are also added: + 'data': 'index' and 'value' of
+each data point + 'date': that was used to produce the report + 'count': the
+number of data items + 'sum': the sum of the data items + 'max': the biggest
+value in 'data' + 'max_index': the index of the biggest value in 'data' +
+'min': the smallest value in 'data' + 'min_index': the index of the smallest
+value in 'data' + 'average': corrected average of the data items For example,
+this Jupyter Lab cell will report energy data by day for the month of June
+2023: ``` d = '2023-06-17' result=f.get_report('month', d=d) ``` This example
+plots weekly data: ![image](https://github.com/TonyM1958/FoxESS-Cloud/assets/
+63789168/f408a010-9600-4b2f-979f-83e32d960586) # Built-in Utilities and
+Operations The previous section provides functions that can be used to access
+and control your inverter. This section covers utilities and operations that
+build upon these functions. ## Charge Needed Uses forecast PV yield for
+tomorrow to work out if charging from grid is needed tonight to deliver the
+expected consumption for tomorrow. If charging is needed, the charge times are
+configured. If charging is not needed, the charge times are cleared. The
+results are sent to the inverter. ``` f.charge_needed(forecast, force_charge,
+forecast_selection, forecast_times, update_setings, show_data, show_plot) ```
+All the parameters are optional: + forecast: the kWh expected tomorrow
+(optional, see below) + force_charge: 1 any remaining time in a charge period
+has force charge / min_soc set, 2 charging uses the entire charge period, 0
+None (default) + forecast_selection: if set to 1, settings are only updated if
+there is a forecast. Default is 0, generation is used when forecasts are not
+available + forecast_times: a list of hours when forecasts can be obtained. By
+default, the forecast times for the selected tariff are used (see below) +
+update_settings: 0 no changes, 1 update charge settings. The default is 0 +
+show_data: 1 show battery SoC data, 2 show battery Residual data, 3 show timed
+data, 4 show timed data before and after charging. The default is 1. +
 show_plot: 1 plot battery SoC data. 2 plot battery Residual, Generation and
 Consumption. 3 plot 2 + Charge and Discharge The default is 3 ### Modelling
 charge_needed() uses a number of models to better estimate the state of the
 battery. **Manual Consumption:** You can provide your 'annual_consumption' in
 kWh e.g. 5500. This figure is factored down to a daily consumption by dividing
 by 365 and applying **f.seasonality**. This normally decreases consumption in
 the summer and increases it in winter. Seasonality is a list of weightings by
@@ -252,82 +259,83 @@
 value derrived from the inverter model discharge_current: None # max battery
 discharge current setting in A. None uses a value derrived from the inverter
 model export_limit: None # maximum export power in kW. None uses the inverter
 power rating discharge_loss: 0.97 # loss converting battery discharge power to
 grid power pv_loss: 0.95 # loss converting PV power to battery charge power
 grid_loss: 0.97 # loss converting grid power to battery charge power
 charge_loss: None # loss converting charge power to residual inverter_power:
-None # inverter power consumption in W (dynamically set) bms_power: 25 # BMS
-power consumption in W bat_resistance: 0.070 # internal resistance of a battery
-in ohms volt_curve: lifepo4_curve # battery OCV from 0% to 100% SoC
-nominal_soc: 55 # SoC for nominal open circuit voltage generation_days: 3 #
-number of days to use for average generation (1-7) consumption_days: 3 # number
-of days to use for average consumption (1-7) consumption_span: 'week' # 'week'
-= last 7 days or 'weekday' = last 7 weekdays e.g. Saturdays use_today: 21.0 #
-hour when today's generation and consumption data will be used min_hours: 0.25
-# minimum charge time to set (in decimal hours) min_kwh: 0.5 # minimum charge
-to add in kwh solcast_adjust: 100 # % adjustment to make to Solcast forecast
-solar_adjust: 100 # % adjustment to make to Solar forecast forecast_selection:
-1 # 1 = only update charge times if forecast is available, 0 = use best
-available data. Default is 1. annual_consumption: None # optional annual
-consumption in kWh. If set, this replaces consumption history timed_mode: 0 # 0
-= None, 1 = use timed work mode, 2 = strategy mode special_contingency: 30 #
-contingency for special days when consumption might be higher special_days:
-['12-25', '12-26', '01-01'] full_charge: None # day of month (1-28) to do full
-charge or 'daily' or day of week: 'Mon', 'Tue' etc derate_temp: 21 # battery
-temperature in C when derating charge current is applied derate_step: 5 # step
-size for derating e.g. 21, 16, 11 derating: [24, 15, 10, 2] # derated charge
-current for each temperature step e.g. 21C, 16C, 11C, 6C force: 1 # 1 = disable
-strategy periods when setting charge. 0 = fail if strategy period has been set.
-data_wrap: 6 # data items to show per line target_soc: None # target soc for
-charging ``` These values are stored / available in f.charge_config. The
-default battery open circuit voltage curve versus SoC from 0% to 100% is: ```
-lifepo4_curve = [51.30, 52.00, 52.30, 52.40, 52.50, 52.60, 52.70, 52.80, 52.9,
-53.1, 53.50] ``` When operating in strategy mode (timed_mode=2), charge_needed
-will create a schedule that includes the strategy for the tariff with
-additional time segments added to charge from grid and (optionall) to stop the
-battery discharging. In other modes, charge_needed() will disable any schedules
-and set the battery charge times. This example shows the results reported by
-charge needed: ![image](https://github.com/TonyM1958/FoxESS-Cloud/assets/
-63789168/8b77956b-c326-43cd-b165-20d806b1e7e8) ## Battery Info Provides
-detailed information on the current state of the batteries: ``` f.battery_info
-(count, plot, log) f.battery_monitor(interval, run, log, save, count) ```
-battery_info() prints information on the battery and cells: + count: optional
-over-ride. The default is based on factorising the number of cells reported by
-16 or 18 to work out the number of batteries. + plot: 1 plot the cell voltages
-for each battery, 2 plot the cell temperatueres, 0 don't plot. The default is 1
-+ log: see below. Default is 0 battery_monitor() runs battery_info() in log
-mode on a schedule to provide information on the battery status over a period
-of time: + interval: the time in minutes between log entries. The default is 30
-minutes + run: the number of log entries to create. The default is 48 i.e.
-every 30 minues for 24 hours in total + log: 0 = display, 1 = log battery info,
-2 = add cell volts, 3 = add cell temps. The default is 1 + save: name of a CSV
-file to write log data to + count: optional over-ride for the number of
-batteries This is an example of the output from battery_info(): ![image](https:
-//github.com/TonyM1958/FoxESS-Cloud/assets/63789168/a8eb52b6-ce3f-4b58-bb76-
-5483d5e40fa7) ## Date Ranges ``` f.date_list(s, e, limit, span, today) ```
-Returns a list of dates in the format 'YYYY-MM-DD'. This function will not
-return dates in the future. The last date will be yesterday or today (if today
-is True). All parameters are optional: + s: start date + e: end date + limit:
-maximum number of days. The default is 200 + span: the range of dates. One of
-'day', 'week', 'month' or 'year', '2days' or 'weekday' + today: 1 allows today
-to be included, 2 allows future dates to be included. Default is 0, date list
-will stop at yesterday You can use 'span' as follows: + 'day' provides a single
-day + 'week' will provide the dates of 7 consequetive days + 'month' will
-provide the dates of the days up to the same date in the preceeding (or
-follwing) month + '2days' will provide the dates of yesterday and today +
-'weekday' will provide the dates of the same day of the week, going backwards
-(or forwards) up to 7 weeks ``` f.british_summer_time(d) # 1 if d is in Britsh
-Summer Time, 0 if not ``` ## Time Periods Times and time period settings are
-held as decimal hours. Functions for working with time strings with the format
-'HH:MM:SS' and decimal hours include: ``` f.time_hours(t, d=None) # convert
-time to decimal hours. t is a time string ('HH:MM' or 'HH:MM:SS'), d is
-optional and is the default time if s is None f.hours_time(h, mm=True,
-ss=False, day=False) # convert decimal hours to time (HH:MM:SS). mm = include
-minutes, ss = include seconds, day = include /n for day when hours > 24
+None # inverter power consumption in W (dynamically set) bms_power: 50 # BMS
+power consumption in W allowed_drain: 4, # % tolerance below min_soc before
+float charge starts float_current: 4, # BMS float charge current in A
+bat_resistance: 0.070 # internal resistance of a battery in ohms volt_curve:
+lifepo4_curve # battery OCV from 0% to 100% SoC nominal_soc: 55 # SoC for
+nominal open circuit voltage generation_days: 3 # number of days to use for
+average generation (1-7) consumption_days: 3 # number of days to use for
+average consumption (1-7) consumption_span: 'week' # 'week' = last 7 days or
+'weekday' = last 7 weekdays e.g. Saturdays use_today: 21.0 # hour when today's
+generation and consumption data will be used min_hours: 0.25 # minimum charge
+time to set (in decimal hours) min_kwh: 0.5 # minimum charge to add in kwh
+solcast_adjust: 100 # % adjustment to make to Solcast forecast solar_adjust:
+100 # % adjustment to make to Solar forecast forecast_selection: 1 # 1 = only
+update charge times if forecast is available, 0 = use best available data.
+Default is 1. annual_consumption: None # optional annual consumption in kWh. If
+set, this replaces consumption history timed_mode: 0 # 0 = None, 1 = use timed
+work mode, 2 = strategy mode special_contingency: 30 # contingency for special
+days when consumption might be higher special_days: ['12-25', '12-26', '01-01']
+full_charge: None # day of month (1-28) to do full charge or 'daily' or day of
+week: 'Mon', 'Tue' etc derate_temp: 21 # battery temperature in C when derating
+charge current is applied derate_step: 5 # step size for derating e.g. 21, 16,
+11 derating: [24, 15, 10, 2] # derated charge current for each temperature step
+e.g. 21C, 16C, 11C, 6C force: 1 # 1 = disable strategy periods when setting
+charge. 0 = fail if strategy period has been set. data_wrap: 6 # data items to
+show per line target_soc: None # target soc for charging ``` These values are
+stored / available in f.charge_config. The default battery open circuit voltage
+curve versus SoC from 0% to 100% is: ``` lifepo4_curve = [51.30, 52.00, 52.30,
+52.40, 52.50, 52.60, 52.70, 52.80, 52.9, 53.1, 53.50] ``` When operating in
+strategy mode (timed_mode=2), charge_needed will create a schedule that
+includes the strategy for the tariff with additional time segments added to
+charge from grid and (optionall) to stop the battery discharging. In other
+modes, charge_needed() will disable any schedules and set the battery charge
+times. This example shows the results reported by charge needed: ![image]
+(https://github.com/TonyM1958/FoxESS-Cloud/assets/63789168/8b77956b-c326-43cd-
+b165-20d806b1e7e8) ## Battery Info Provides detailed information on the current
+state of the batteries: ``` f.battery_info(count, plot, log) f.battery_monitor
+(interval, run, log, save, count) ``` battery_info() prints information on the
+battery and cells: + count: optional over-ride. The default is based on
+factorising the number of cells reported by 16 or 18 to work out the number of
+batteries. + plot: 1 plot the cell voltages for each battery, 2 plot the cell
+temperatueres, 0 don't plot. The default is 1 + log: see below. Default is 0
+battery_monitor() runs battery_info() in log mode on a schedule to provide
+information on the battery status over a period of time: + interval: the time
+in minutes between log entries. The default is 30 minutes + run: the number of
+log entries to create. The default is 48 i.e. every 30 minues for 24 hours in
+total + log: 0 = display, 1 = log battery info, 2 = add cell volts, 3 = add
+cell temps. The default is 1 + save: name of a CSV file to write log data to +
+count: optional over-ride for the number of batteries This is an example of the
+output from battery_info(): ![image](https://github.com/TonyM1958/FoxESS-Cloud/
+assets/63789168/a8eb52b6-ce3f-4b58-bb76-5483d5e40fa7) ## Date Ranges ```
+f.date_list(s, e, limit, span, today) ``` Returns a list of dates in the format
+'YYYY-MM-DD'. This function will not return dates in the future. The last date
+will be yesterday or today (if today is True). All parameters are optional: +
+s: start date + e: end date + limit: maximum number of days. The default is 200
++ span: the range of dates. One of 'day', 'week', 'month' or 'year', '2days' or
+'weekday' + today: 1 allows today to be included, 2 allows future dates to be
+included. Default is 0, date list will stop at yesterday You can use 'span' as
+follows: + 'day' provides a single day + 'week' will provide the dates of 7
+consequetive days + 'month' will provide the dates of the days up to the same
+date in the preceeding (or follwing) month + '2days' will provide the dates of
+yesterday and today + 'weekday' will provide the dates of the same day of the
+week, going backwards (or forwards) up to 7 weeks ``` f.british_summer_time(d)
+# 1 if d is in Britsh Summer Time, 0 if not ``` ## Time Periods Times and time
+period settings are held as decimal hours. Functions for working with time
+strings with the format 'HH:MM:SS' and decimal hours include: ``` f.time_hours
+(t, d=None) # convert time to decimal hours. t is a time string ('HH:MM' or
+'HH:MM:SS'), d is optional and is the default time if s is None f.hours_time(h,
+mm=True, ss=False, day=False) # convert decimal hours to time (HH:MM:SS). mm =
+include minutes, ss = include seconds, day = include /n for day when hours > 24
 f.hours_in(h, {'start': a, 'end': b}) # True if decimal hour h is in the time
 period a -> b ``` ## Tariffs Tariffs configure when your battery can be charged
 and provide time of use (TOU) periods to split your grid import and export into
 peak, off-peak and shoulder times when data is uploaded to PV Ouptut. There are
 a number of different pre-configured tariffs: + Octopus Flux: off-peak from 02:
 00 to 05:00, peak from 16:00 to 19:00, forecasts from 22:00 to 23:59. Timed
 work mode change to Self Use at 7am and Feed In First at 4pm. + Intelligent
@@ -393,108 +401,118 @@
 between 12 noon and 4pm with a 1 hour period: + times=[("23:00", "8:00", 3),
 ("12:00", "16:00", 1)] 'strategy' allows you to configure times when work modes
 will be changed. The format is a list of dictionary items, containing: +
 'start', 'end': times in decimal hours or time format. The end time is
 exclusive so setting an end time of '07:00' will set a schedule that ends at
 '06:59' + 'mode': the work mode to be used from 'SelfUse', 'Feedin', 'Backup',
 'ForceCharge', 'ForceDischarge' + 'min_soc, 'fdsoc', 'fdpwr': optional values
-for each work mode. The defaults are 10, 10 and 0 respectively. The strategy
-should not include settings for the AM/PM charge times for the tariff. These
-will be added by charge_needed(). # PV Output These functions produce CSV data
-for upload to [pvoutput.org](https://pvoutput.org) including PV generation,
-Export, Load and Grid consumption by day in Wh. The functions use the energy
-estimates created from the raw power data (see above). The estimates include PV
-energy generation that are not otherwise available from the Fox Cloud.
-Typically, the energy results are within 3% of the values reported by the
-meters built into the inverter. ## Get PV Output Data Returns CSV upload data
-using the [API format](https://pvoutput.org/help/api_specification.html#csv-
-data-parameter): ``` f.get_pvoutput(d, tou) ``` + d is the date or a list of
-dates, to get data for. The default is yesterday + tou: optional, setting tou=1
-uploads data with time of use. The default, tou=0 does not split data and is
-more accurate. You can copy and paste the output data to the pvoutput data CSV
-Loader, using the following settings: ![image](https://github.com/TonyM1958/
-FoxESS-Cloud/assets/63789168/21459cdc-a943-4e9d-a204-7efd45a422d8) For example,
-this Jupyer Lab cell will provide a CSV data upload for June 2023: ```
-f.get_pvoutput(f.date_list('2023-06-01', '2023-06-30')) ``` ## Set PV Output
-Data Loads CSV data directly using the PV Ouput API: ``` f.set_pvoutput(d,
-system_id, tou, push) ``` + d is optional and is the date, or a list of dates,
-to upload + system_id is optional and allow you to select where data is
-uploaded to (where you have more than 1 registered system) + tou: optional,
-setting tou=1 uploads data with time of use. The default, tou=0 does not split
-data and is more accurate + push: optional. 0 = do not sent to pushover, 1 =
-send summary to pushover, 2 = send first day summary only # Solar Forecasting #
-Solcast Get and display solar data from your solcast.com account using your API
-key: ``` f.solcast_api_key = "my.solcast_api_key" fcast = f.Solcast() print
-(fcast) ``` Returns a 7 day forecast. Optional parameters are: + days: number
-of days to get. The default is 7 + estimated: whether to get history /
-estimated data. 1 = yes, 0 = no. Default is 0. + reload: cached data handling.
-0 = use saved data, 1 = fetch new data, 2 = use saved data for today (default)
-+ quiet: True to stop Solcast producing progress messages Forecast data is
-saved to f.solcast_save. The default is 'solcast.txt'. ``` fcast.plot_daily()
+for each work mode. The defaults are 10, 10 and 0 respectively. There are a
+number of pre-defined strategies: + f.flux_strategy_1: switch to self use at
+5am and feed in first at 4pm. + f.flux_strategy_2: as above with force charge
+between 2am and 4am. Move the AM charge period between 4am and 5am when using
+this. + f.flux_strategy_3: as above with force discharge between 4pm and 6pm at
+6kW with fdsoc at 35% ``` f.get_strategy() ``` get_strategy() creates a list of
+time segments from the strategy. If strategy is not provided, it uses the
+strategy for the current tariff. If a strategy includes settings for the AM/PM
+charge times for the tariff, the times will be moved so they do not conflict
+with the charge time used by charge_needed(). # PV Output These functions
+produce CSV data for upload to [pvoutput.org](https://pvoutput.org) including
+PV generation, Export, Load and Grid consumption by day in Wh. The functions
+use the energy estimates created from the raw power data (see above). The
+estimates include PV energy generation that are not otherwise available from
+the Fox Cloud. Typically, the energy results are within 3% of the values
+reported by the meters built into the inverter. ## Get PV Output Data Returns
+CSV upload data using the [API format](https://pvoutput.org/help/
+api_specification.html#csv-data-parameter): ``` f.get_pvoutput(d, tou) ``` + d
+is the date or a list of dates, to get data for. The default is yesterday +
+tou: optional, setting tou=1 uploads data with time of use. The default, tou=0
+does not split data and is more accurate. You can copy and paste the output
+data to the pvoutput data CSV Loader, using the following settings: ![image]
+(https://github.com/TonyM1958/FoxESS-Cloud/assets/63789168/21459cdc-a943-4e9d-
+a204-7efd45a422d8) For example, this Jupyer Lab cell will provide a CSV data
+upload for June 2023: ``` f.get_pvoutput(f.date_list('2023-06-01', '2023-06-
+30')) ``` ## Set PV Output Data Loads CSV data directly using the PV Ouput API:
+``` f.set_pvoutput(d, system_id, tou, push) ``` + d is optional and is the
+date, or a list of dates, to upload + system_id is optional and allow you to
+select where data is uploaded to (where you have more than 1 registered system)
++ tou: optional, setting tou=1 uploads data with time of use. The default,
+tou=0 does not split data and is more accurate + push: optional. 0 = do not
+sent to pushover, 1 = send summary to pushover, 2 = send first day summary only
+# Solar Forecasting # Solcast Get and display solar data from your solcast.com
+account using your API key: ``` f.solcast_api_key = "my.solcast_api_key" fcast
+= f.Solcast() print(fcast) ``` Returns a 7 day forecast. Optional parameters
+are: + days: number of days to get. The default is 7 + estimated: whether to
+get history / estimated data. 1 = yes, 0 = no. Default is 0. + reload: cached
+data handling. 0 = use saved data, 1 = fetch new data, 2 = use saved data for
+today (default) + quiet: True to stop Solcast producing progress messages
+Forecast data is saved to f.solcast_save. The default is 'solcast.txt'. ```
+fcast.plot_daily() fcast.plot_hourly(day) ``` Plots the estimate / forecast
+data. plot_daily() plots the daily yield. plot_hourly() plots each day
+separately. + day: optional. 'today', 'tomorrow', 'all' or a specific list of
+dates. The default is to plot today and tomorrow # Forecast.solar Get and
+display solar data from forecast.solar for today and tomorrow: ```
+f.solar_array('South', lat=51.1789, lon=-1.8262, kwp=6.4) ``` You need to
+configure your solar arrays by calling f.solar_array(). This takes the
+following parameters: + name: the name of each of your arrays + lat: the
+latitude where the array is located. The default is Stonehenge. + lon: the
+longitude where the array is located. The default is Stonehenge. + dec: the
+declination of the array - 0 is lying flat and 90 is vertical. Default is 30 +
+az: azimuth of the array. 0 is pointing due South, -90 is pointing East, 90 is
+pointing West. The default is 0 + kwp: the size of the array in kWp. The
+default is 5kWp + dam: damping factor. Default is None + inv: inverter power
+limit (when the array will clip). The default is None + hor: a list of values
+describing obstructions on the horizon Add one array for each string attached
+to your inverter. If your solar production is limited by clipping, set the
+inverter power so the forecast better matches your generation. See the [API
+documentation](https://doc.forecast.solar/api) for more information on
+parameter values. ``` fcast = f.Solar() print(fcast) ``` Returns a forecast for
+today and tomorrow. Optional parameters are: + reload: cached data handling. 0
+= use saved data, 1 = fetch new data, 2 = use saved data for today (default) +
+quiet: set to True to stop Solar producing progress messages Forecast data is
+saved to f.solar_save. The default is 'solar.txt'. ``` fcast.plot_daily()
 fcast.plot_hourly(day) ``` Plots the estimate / forecast data. plot_daily()
 plots the daily yield. plot_hourly() plots each day separately. + day:
 optional. 'today', 'tomorrow', 'all' or a specific list of dates. The default
-is to plot today and tomorrow # Forecast.solar Get and display solar data from
-forecast.solar for today and tomorrow: ``` f.solar_array('South', lat=51.1789,
-lon=-1.8262, kwp=6.4) ``` You need to configure your solar arrays by calling
-f.solar_array(). This takes the following parameters: + name: the name of each
-of your arrays + lat: the latitude where the array is located. The default is
-Stonehenge. + lon: the longitude where the array is located. The default is
-Stonehenge. + dec: the declination of the array - 0 is lying flat and 90 is
-vertical. Default is 30 + az: azimuth of the array. 0 is pointing due South, -
-90 is pointing East, 90 is pointing West. The default is 0 + kwp: the size of
-the array in kWp. The default is 5kWp + dam: damping factor. Default is None +
-inv: inverter power limit (when the array will clip). The default is None +
-hor: a list of values describing obstructions on the horizon Add one array for
-each string attached to your inverter. If your solar production is limited by
-clipping, set the inverter power so the forecast better matches your
-generation. See the [API documentation](https://doc.forecast.solar/api) for
-more information on parameter values. ``` fcast = f.Solar() print(fcast) ```
-Returns a forecast for today and tomorrow. Optional parameters are: + reload:
-cached data handling. 0 = use saved data, 1 = fetch new data, 2 = use saved
-data for today (default) + quiet: set to True to stop Solar producing progress
-messages Forecast data is saved to f.solar_save. The default is 'solar.txt'.
-``` fcast.plot_daily() fcast.plot_hourly(day) ``` Plots the estimate / forecast
-data. plot_daily() plots the daily yield. plot_hourly() plots each day
-separately. + day: optional. 'today', 'tomorrow', 'all' or a specific list of
-dates. The default is to plot today and tomorrow # Pushover Send messages to a
-pushover user account: ``` f.output_spool(app_key, h) f.output(s)
-f.output_close(plot, file) f.output_message(app_key, message, plot) ``` Calling
-f.output_spool() with an app key will start the system spooling output to send
-to pushover. h is an optional header to add as the first line of the message. H
-may include \
+is to plot today and tomorrow # Pushover Send messages to a pushover user
+account: ``` f.output_spool(app_key, h) f.output(s) f.output_close(plot, file)
+f.output_message(app_key, message, plot) ``` Calling f.output_spool() with an
+app key will start the system spooling output to send to pushover. h is an
+optional header to add as the first line of the message. H may include \
 >, \
 > or \
 > and these will be set to current system time and date respectively. When
 spooling is active, any calls to f.output() add lines to the spooled message.
 If appending to the message would exceed 1024 characters, the existing spooled
 message is sent and a new message spool is started. Calling f.output_close()
 will send the spooled message and optionally attach a binary image file. You
 can set plot=1 to attach the last plot file created (when f.plot_file is set)
 or specify a file. f.output_message() is a shorcut to send a message without
 spooling output. # Troubleshooting If needed, you can add the following setting
 to increase the level of information reported by the foxesscloud module: ```
 f.debug_setting = 2 ``` This setting can be: + 0: silent mode (minimal output)
 + 1: information reporting (default) + 2: more debug information, updating of
 inverter settings is disabled + 3: internal variables and values are displayed
-(verbose) # Version Info 2.2.7
-Updated contingency to allow seasonal values for winter, spring, summer and
-autumn. Update strategy mode to support ForceCharge and ForceDischarge work
-modes. Update so min_soc setting in charge_needed() over-rides min_soc in the
-tariff strategy. Fix force charge strategy mode in charge_neded() to set
-min_soc correctly. Implement 2 second delay between calls that change inverter
-settings. Added strategy mode (timed_mode=2) to charge_needed(). Added
-set_strategy() and charge_strategy() to manage charging schedules and work mode
-changes. Refactor debug messaging. Simplify charge_needed() output. Added
-'target_soc' to charge_needed() settings Fix bat_info() giving incorrect
-temperatures when API returns 0 instead of -50 where there is no battery Fix
-key error when accessing cell volts and temps using an agent / installer
-account. Ensure output is generated if get_battery() fails using battery_info
-(). Update f.avg() to include calculation of averages in lists containng None
-values. Added 'data_wrap' to charge_config. 2.1.9
+(verbose) # Version Info 2.2.8
+** breaking change ** rename 'groups' to 'periods' for consistency between
+foxesscloud and openapi. Updated management of battery reserve and float
+charging in charge_needed(). Added Reserve level to charts in charge_needed().
+Changed bms_power setting to 50W. Updated contingency to allow seasonal values
+for winter, spring, summer and autumn. Update strategy mode to support
+ForceCharge and ForceDischarge work modes. Update so min_soc setting in
+charge_needed() over-rides min_soc in the tariff strategy. Fix force charge
+strategy mode in charge_neded() to set min_soc correctly. Implement 2 second
+delay between calls that change inverter settings. Added strategy mode
+(timed_mode=2) to charge_needed(). Added set_strategy() and charge_strategy()
+to manage charging schedules and work mode changes. Refactor debug messaging.
+Simplify charge_needed() output. Added 'target_soc' to charge_needed() settings
+Fix bat_info() giving incorrect temperatures when API returns 0 instead of -50
+where there is no battery Fix key error when accessing cell volts and temps
+using an agent / installer account. Ensure output is generated if get_battery()
+fails using battery_info(). Update f.avg() to include calculation of averages
+in lists containng None values. Added 'data_wrap' to charge_config. 2.1.9
 Update get_history() to use GMT or BST when plotting instead of mixed time
 zones. Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in
 relation to work mode. Better reporting of reason for http error code. Template
 code for get_named_settings() added - not functional in this version due to
 Open API limitations. Update set_pvoutput() to allow push=2. Fix problem in
 set_pvoutput() sending summary to pushover when tou=1. Improve accuracy of time
```

### Comparing `foxesscloud-2.2.7/pyproject.toml` & `foxesscloud-2.2.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "foxesscloud"
-version = "2.2.7"
+version = "2.2.8"
 authors = [
   {name="Tony Matthews", email="tony@quasair.co.uk"},
 ]
 description = "library for accessing Fox ESS cloud data using Open API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `foxesscloud-2.2.7/src/foxesscloud/foxesscloud.py` & `foxesscloud-2.2.8/src/foxesscloud/foxesscloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################################
 """
 Module:   Fox ESS Cloud
-Updated:  22 May 2024
+Updated:  24 May 2024
 By:       Tony Matthews
 """
 ##################################################################################################
 # Code for getting and setting inverter data via the Fox ESS cloud web site, including
 # getting forecast data from solcast.com.au and sending inverter data to pvoutput.org
 # ALL RIGHTS ARE RESERVED © Tony Matthews 2023
 ##################################################################################################
 
-version = "1.3.9"
+version = "1.4.0"
 print(f"FoxESS-Cloud version {version}")
 
 debug_setting = 1
 
 # constants
 month_names = ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', 'December']
 day_names = ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday']
@@ -702,17 +702,20 @@
         else:
             output(f"** set_charge(), {errno_message(errno)}")
         return None
     else:
         output(f"success", 2) 
     return battery_settings
 
-def charge_strategy(st1 = None, en1 = None, st2 = None, en2 = None, adjust=0, min_soc=10, target_soc=None):
+def charge_periods(st1 = None, en1 = None, st2 = None, en2 = None, adjust=0, min_soc=10, target_soc=None):
     output(f"\nConfiguring schedule",1)
-    periods = set_strategy(min_soc=min_soc, quiet=0)
+    strategy = get_strategy(min_soc=min_soc, quiet=0)
+    periods = []
+    for s in strategy:
+        periods.append(set_period(segment = s, quiet=0))
     if st1 is not None and en1 is not None and st1 != en1:
         st1 = round_time(time_hours(st1) + adjust)
         en1 = round_time(time_hours(en1) + adjust)
         periods.append(set_period(start = st1, end = en1, mode = 'ForceCharge', min_soc = target_soc, quiet=0))
     if st2 is not None and en2 is not None and st2 != en2:
         st2 = round_time(time_hours(st2) + adjust)
         en2 = round_time(time_hours(en2) + adjust)
@@ -1160,18 +1163,25 @@
 
 
 ##################################################################################################
 # set schedule
 ##################################################################################################
 
 # create a period structure. Note: end time is exclusive.
-def set_period(start, end, mode=None, min_soc=None, fdsoc=None, fdpwr=None, quiet=1):
+def set_period(start=None, end=None, mode=None, min_soc=None, fdsoc=None, fdpwr=None, segment=None, quiet=1):
+    if segment is not None and type(segment) is dict:
+        start = segment.get('start')
+        end = segment.get('end')
+        mode = segment.get('mode')
+        min_soc = segement.get('min_soc')
+        fdsoc = segment.get('fdsoc')
+        fdpwr = segmenet.get('fdsoc')
     start = time_hours(start)
     end = time_hours(end)
-    if start is None or end is None:
+    if start is None or end is None or start >= end:
         return None
     end = round_time(end - 1/60)        # adjust exclusive time to inclusive
     mode = 'SelfUse' if mode is None else mode
     if mode not in work_modes:
         output(f"** mode must be one of {work_modes}")
         return None
     min_soc = 10 if min_soc is None else min_soc
@@ -1183,37 +1193,20 @@
     if fdpwr < 0 or fdpwr > 6000:
         output(f"** fdpwr must be between 0 and 6000")
         return None
     if fdsoc < min_soc or fdsoc > 100:
         output(f"** fdsoc must between {min_soc} and 100")
         return None
     if quiet == 0:
-        output(f"   {hours_time(start)} to {hours_time(end)}: {mode} with min_soc = {min_soc}%" + (f", fdPwr = {fdpwr}W and fdSoC = {fdsoc}%" if mode == 'ForceDischarge' else ""), 1)
+        output(f"   {hours_time(start)} to {hours_time(end)} {mode} with min_soc = {min_soc}%" + (f", fdPwr = {fdpwr}W and fdSoC = {fdsoc}%" if mode == 'ForceDischarge' else ""), 1)
     start_h, start_m = split_hours(start)
     end_h, end_m = split_hours(end)
     period = {'startH': start_h, 'startM': start_m, 'endH': end_h, 'endM': end_m, 'workMode': mode, 'minSocOnGrid': min_soc, 'fdSoc': fdsoc, 'fdPwr': fdpwr}
     return period
 
-# create periods from a list of strategy times:
-def set_strategy(strategy=None, min_soc=10, quiet=1):
-    global tariff
-    if strategy is None and tariff is not None:
-        strategy = tariff.get('strategy')
-    if strategy is None:
-        return []
-    if type(strategy) is not list:
-        strategy = [strategy]
-    periods = []
-    for s in strategy:
-        min_soc = s['min_soc'] if s.get('min_soc') is not None and s['min_soc'] > min_soc else min_soc
-        p = set_period(s['start'], s['end'], s['mode'], min_soc, s.get('fdsoc'), s.get('fdpwr'), quiet=quiet)
-        if p is not None:
-            periods.append(p)
-    return periods
-
 # set a schedule from a period or list of periods
 def set_schedule(periods=None, template=None, enable=1):
     global token, device_sn, debug_setting, messages, schedule, templates
     if get_flag() is None:
         return None
     if schedule.get('support') == False:
         output(f"** set_schedule(), not supported on this device")
@@ -1948,18 +1941,14 @@
 octopus_flux = {
     'name': 'Octopus Flux',
     'off_peak1': {'start': 2.0, 'end': 5.0, 'force': 1},        # off-peak period 1 / am charging period
     'off_peak2': {'start': 0.0, 'end': 0.0, 'force': 0},        # off-peak period 2 / pm charging period
     'peak': {'start': 16.0, 'end': 19.0 },                      # peak period 1
     'peak2': {'start': 0.0, 'end': 0.0 },                       # peak period 2
     'forecast_times': [22, 23],                                 # hours in a day to get a forecast
-    'strategy': [                                               # timed work mode settings
-        {'start': 0, 'end': 2, 'mode': 'Feedin'},
-        {'start': 5, 'end': 6, 'mode': 'SelfUse'},
-        {'start': 16, 'end': 24, 'mode': 'Feedin'}]
     }
 
 # time periods for Intelligent Octopus
 intelligent_octopus = {
     'name': 'Intelligent Octopus',
     'off_peak1': {'start': 23.5, 'end': 5.5, 'force': 1},
     'off_peak2': {'start': 0.0, 'end': 0.0, 'force': 0},
@@ -2027,14 +2016,72 @@
     'forecast_times': [22, 23]
     }
 
 tariff_list = [octopus_flux, intelligent_octopus, octopus_cosy, octopus_go, agile_octopus, bg_driver, economy_7, custom_periods]
 tariff = octopus_flux
 
 ##################################################################################################
+# Strategy - schedule templates
+##################################################################################################
+
+# summer strategy for Flux
+flux_strategy_1 = [
+        {'start': 5, 'end': 6, 'mode': 'SelfUse'},
+        {'start': 16, 'end': 24, 'mode': 'Feedin'}]
+
+# winter strategy for Flux
+flux_strategy_2 = [
+        {'start': 2, 'end': 4, 'mode': 'ForceCharge'},
+        {'start': 5, 'end': 6, 'mode': 'SelfUse'},
+        {'start': 16, 'end': 24, 'mode': 'Feedin'}]
+
+# revenue strategy for Flux
+flux_strategy_3 = [
+        {'start': 2, 'end': 4, 'mode': 'ForceCharge'},
+        {'start': 5, 'end': 6, 'mode': 'SelfUse'},
+        {'start': 16, 'end': 18, 'mode': 'ForceDischarge', 'fdsoc': 35, 'fdpwr': 6000},
+        {'start': 18, 'end': 24, 'mode': 'Feedin'}]
+
+flux_strategy_x = [
+        {'start': 2, 'end': 11, 'mode': 'SelfUse', 'min_soc': 80},
+        {'start': 11, 'end': 14, 'mode': 'SelfUse', 'min_soc': 10},
+        {'start': 16, 'end': 24, 'mode': 'Feedin'}]
+
+# return an updated strategy from the tariff strategy that has been filtered for charge times:
+def get_strategy(use=None, strategy=None, min_soc=10, quiet=1):
+    global tariff
+    if use is None:
+        use = tariff
+    if strategy is None and tariff is not None:
+        strategy = tariff.get('strategy')
+    if strategy is None:
+        return []
+    if type(strategy) is not list:
+        strategy = [strategy]
+    updated = []
+    for s in strategy:
+        # move start and end times so they don't overlap the charge periods
+        start = s['start']
+        start = tariff['off_peak1']['end'] if hour_in(start, use['off_peak1']) else tariff['off_peak2']['end'] if hour_in(start, use['off_peak2']) else start
+        end = s['end']
+        end = tariff['off_peak1']['start'] if hour_in(end, use['off_peak1']) else tariff['off_peak2']['start'] if hour_in(end, use['off_peak2']) else end
+        # create segment
+        if start < end:
+            min_soc_now = s['min_soc'] if s.get('min_soc') is not None and s['min_soc'] > min_soc else min_soc
+            mode = s['mode']
+            fdsoc = s.get('fdsoc')
+            fdpwr = s.get('fdpwr')
+            segment = {'start': start, 'end': end, 'mode': mode, 'min_soc': min_soc_now, 'fdsoc': fdsoc, 'fdpwr': fdpwr}
+            if quiet == 0:
+                output(f"   {hours_time(start)} to {hours_time(end)} {mode} with min_soc = {min_soc_now}%" + (f", fdPwr = {fdpwr}W and fdSoC = {fdsoc}%" if mode == 'ForceDischarge' else ""), 1)
+            updated.append(segment)
+    return updated
+
+
+##################################################################################################
 # Octopus Energy Agile Price
 ##################################################################################################
 
 # base settings
 octopus_api_url = "https://api.octopus.energy/v1/products/%PRODUCT%/electricity-tariffs/E-1R-%PRODUCT%-%REGION%/standard-unit-rates/"
 regions = {'A':'Eastern England', 'B':'East Midlands', 'C':'London', 'D':'Merseyside and Northern Wales', 'E':'West Midlands', 'F':'North Eastern England', 'G':'North Western England', 'H':'Southern England',
     'J':'South Eastern England', 'K':'Southern Wales', 'L':'South Western England', 'M':'Yorkshire', 'N':'Southern Scotland', 'P':'Northern Scotland'}
@@ -2268,30 +2315,22 @@
         use['forecast_times'] = forecast_hours
         output(f"Forecast times set to {forecast_times}")
     if strategy is not None:
         if type(strategy) is not list:
             strategy = [strategy]
         use['strategy'] = strategy
         output(f"Strategy updated")
-        set_strategy(strategy, quiet=0)
+        get_strategy(use=use, strategy=strategy, quiet=0)
     if update == 1:
         tariff = use
         output(f"\nTariff set to {tariff['name']}")
     else:
         output(f"\nNo changes made to current tariff", 1)
     return None
 
-# get work mode for a time of day based on the tariff:
-def timed_work_mode(h, default = 'SelfUse'):
-    if tariff is None or tariff.get('strategy') is None:
-        return default
-    for d in tariff['strategy']:
-        if hour_in(h, d):
-            return d['mode']
-    return default
 
 ##################################################################################################
 # CHARGE_NEEDED - calculate charge from current battery charge, forecast yield and expected load
 ##################################################################################################
 
 # how consumption varies by month across a year. 12 values.
 # month                J   F   M   A   M   J   J   A   S   O   N   D
@@ -2367,35 +2406,69 @@
     for h in range(0, 24):
         profile.append(c_float(forecast.daily[tomorrow]['hourly'].get(int(round_time(h - time_offset)))))
     timed = []
     for h in range(int(hour_now), 24):
         timed.append(c_float(forecast.daily[today]['hourly'].get(int(round_time(h - time_offset)))))
     return (timed + profile + profile)[:run_time]
 
-# take a strategy and return a timed profile:
+# build the timed work mode profile from the tariff strategy:
 def strategy_timed(timed_mode, hour_now, run_time, min_soc=10):
     global tariff
     profile = []
+    min_soc_now = min_soc
     for h in range(0, 24):
-        profile.append({'mode': 'SelfUse', 'min_soc': min_soc, 'fdpwr': 0, 'fdsoc': min_soc, 'duration': 1.0})
-        if tariff is None or tariff.get('strategy') is None or timed_mode == 0:
-            continue
-        for d in tariff['strategy']:
-            if hour_in(h, d):
-                profile[h]['mode'] = d['mode']
-                if d.get('min_soc') is not None:
-                    profile[h]['min_soc'] = d['min_soc'] if d['min_soc'] > min_soc else min_soc
-                if d.get('fdsoc') is not None:
-                    profile[h]['fdsoc'] = d['fdsoc'] if d['fdsoc'] > min_soc else min_soc
-                if d.get('fdpwr') is not None:
-                    profile[h]['fdpwr'] = d['fdpwr']
-                profile[h]['duration'] = duration_in(h, d)
+        period = {'mode': 'SelfUse', 'min_soc': min_soc_now, 'fdpwr': 0, 'fdsoc': min_soc_now, 'duration': 1.0}
+        if timed_mode > 0 and tariff is not None and tariff.get('strategy') is not None:
+            for d in get_strategy():
+                if hour_in(h, d):
+                    mode = d['mode']
+                    period['mode'] = mode
+                    min_soc_now = d['min_soc'] if d.get('min_soc') is not None and d['min_soc'] > min_soc else min_soc
+                    period['min_soc'] = min_soc_now
+                    if mode == 'ForceDischarge':
+                        if d.get('fdsoc') is not None:
+                            period['fdsoc'] = d['fdsoc'] if d['fdsoc'] > min_soc_now else min_soc_now
+                        if d.get('fdpwr') is not None:
+                            period['fdpwr'] = d['fdpwr']
+                    period['duration'] = duration_in(h, d)
+        profile.append(period)
     output(f"work mode profile = {profile}", 2)
     return (profile[int(hour_now):] + profile + profile)[:run_time]
 
+# build the timed battery residual from the charge / discharge, work mode and min_soc
+def battery_timed(kwh_timed, work_mode_timed, kwh_current, capacity, time_to_next, float_charge, kwh_min=None, reserve_drain=None):
+    global charge_config
+    bat_timed = []
+    allowed_drain = charge_config['allowed_drain'] if charge_config.get('allowed_drain') is not None else 4
+    bms_loss = charge_config['bms_power'] / 1000 if charge_config.get('bms_power') is not None else 50
+    for i in range(0, len(kwh_timed)):
+        kwh_current += kwh_timed[i]
+        min_soc_now = work_mode_timed[i]['fdsoc'] if work_mode_timed[i]['mode'] =='ForceDischarge' else work_mode_timed[i]['min_soc']
+        reserve_now = capacity * min_soc_now / 100
+        if kwh_current < reserve_now and (i <= time_to_next or kwh_min is None):
+            # battery is empty, check if charge is needed
+            reserve_drain = kwh_current if reserve_drain is None or kwh_current > reserve_drain else reserve_drain
+            kwh_current = reserve_drain
+            reserve_limit = capacity * (min_soc_now - allowed_drain) / 100
+            if reserve_drain < reserve_limit:
+                reserve_drain = min([reserve_now, reserve_drain + float_charge])
+            else:
+                # BMS power drain
+                reserve_drain -= bms_loss
+        else:
+            # reset drain level
+            reserve_drain = reserve_now
+        if kwh_current > capacity:
+            # battery is full
+            kwh_current = capacity
+        bat_timed.append(kwh_current)
+        if kwh_min is not None and kwh_current < kwh_min and i >= time_to_next:       # track minimum without charge
+            kwh_min = kwh_current
+    return (bat_timed, kwh_min)
+
 # Battery open circuit voltage (OCV) from 0% to 100% SoC
 #                 0%     10%    20%    30%    40%    50%    60%    70%    80%    90%   100%
 lifepo4_curve = [51.00, 51.50, 52.00, 52.30, 52.60, 52.80, 52.90, 53.00, 53.10, 53.30, 54.00]
 
 # charge_needed settings
 charge_config = {
     'contingency': [20,10,5,15],      # % of consumption. Single value or [winter, spring, summer, autumn]
@@ -2405,15 +2478,17 @@
     'discharge_current': None,        # max battery discharge current setting in A
     'export_limit': None,             # maximum export power in kW
     'discharge_loss': 0.97,           # loss converting battery discharge power to grid power
     'pv_loss': 0.95,                  # loss converting PV power to battery charge power
     'grid_loss': 0.95,                # loss converting grid power to battery charge power
     'charge_loss': None,              # loss converting charge power to residual
     'inverter_power': None,           # Inverter power consumption in W
-    'bms_power': 27,                  # BMS power consumption in W
+    'bms_power': 50,                  # BMS power consumption in W
+    'allowed_drain': 4,               # % tolerance below min_soc before float charge starts
+    'float_current': 4,               # BMS float charge in A
     'bat_resistance': 0.072,          # internal resistance of a battery
     'volt_curve': lifepo4_curve,      # battery OCV range from 0% to 100% SoC
     'nominal_soc': 60,                # SoC for nominal open circuit battery voltage
     'generation_days': 3,             # number of days to use for average generation (1-7)
     'consumption_days': 3,            # number of days to use for average consumption (1-7)
     'consumption_span': 'week',       # 'week' = last n days or 'weekday' = last n weekdays
     'use_today': 21.0,                # hour when todays consumption and generation can be used
@@ -2538,23 +2613,15 @@
     output(f"start_pm = {start_pm}, end_pm = {end_pm}, force_pm = {force_charge_pm}, time_to_pm = {time_to_pm}", 3)
     output(f"start_at = {start_at}, end_by = {end_by}, force_charge = {force_charge}", 3)
     output(f"base_hour = {base_hour}, hour_adjustment = {hour_adjustment}, change_hour = {change_hour}", 3)
     output(f"time_to_start = {time_to_start}, run_time = {run_time}, charge_pm = {charge_pm}", 3)
     output(f"start_hour = {start_hour}, time_to_next = {time_to_next}, full_charge = {full_charge}", 3)
     # get device and battery info from inverter
     if test_soc is None:
-        if charge_config.get('min_soc') is not None:
-            min_soc = charge_config['min_soc']
-        else:
-            get_min()
-            if battery_settings.get('minGridSoc') is not None:
-                min_soc = battery_settings['minGridSoc']
-            else:
-                print(f"\nMin SoC is not available. Please provide % via 'min_soc' parameter")
-                return None
+        min_soc = charge_config['min_soc'] if charge_config['min_soc'] is not None else 10
         get_battery()
         if battery['status'] != 1:
             output(f"\nBattery status is not available")
             return None
         current_soc = battery['soc']
         bat_volt = battery['volt']
         bat_power = battery['power']
@@ -2628,14 +2695,15 @@
     elif charge_power < charge_limit:
         charge_limit = charge_power
     # work out losses when charging / force discharging
     inverter_power = charge_config['inverter_power'] if charge_config['inverter_power'] is not None else round(device_power, 0) * 20
     operating_loss = inverter_power / 1000
     bms_power = charge_config['bms_power']
     bms_loss = bms_power / 1000
+    float_charge = (charge_config['float_current'] if charge_config.get('float_current') is not None else 4) * bat_ocv / 1000
     charge_loss = charge_config.get('charge_loss')
     if charge_loss is None:
         charge_loss = 1.0 - charge_limit * 1000 * bat_resistance / bat_ocv ** 2 - bms_loss / charge_limit
     # work out discharge limit = max power coming from the battery before ac conversion losses
     discharge_loss = charge_config['discharge_loss']
     discharge_limit = device_power
     discharge_current = device_current if charge_config['discharge_current'] is None else charge_config['discharge_current']
@@ -2790,54 +2858,29 @@
                 charge_limit * duration + charge_timed[i] * (1.0 - duration))
         elif timed_mode > 0 and work_mode == 'ForceDischarge':
             fdpwr = work_mode_timed[i]['fdpwr'] / charge_config['discharge_loss']
             fdpwr = min([discharge_limit, export_limit * 1000 + discharge_timed[i], fdpwr])
             (discharge_timed[i], charge_timed[i]) = (fdpwr * duration + discharge_timed[i] * (1.0 - duration) - charge_timed[i] * duration,
                 charge_timed[i] * (1.0 - duration))
         elif force_charge_am > 0 and hour_in(h, {'start': start_am, 'end': end_am}):
-            discharge_timed[i] = operating_loss if charge_timed[i] == 0.0 else 0.0
+            discharge_timed[i] = bms_loss
         elif force_charge_pm > 0 and hour_in(h, {'start': start_pm, 'end': end_pm}):
-            discharge_timed[i] = operating_loss if charge_timed[i] == 0.0 else 0.0
+            discharge_timed[i] = bms_loss
         elif timed_mode > 0 and work_mode == 'Backup':
-            discharge_timed[i] = operating_loss if charge_timed[i] == 0.0 else 0.0
+            discharge_timed[i] = bms_loss if charge_timed[i] == 0.0 else 0.0
         elif timed_mode > 0 and work_mode == 'Feedin':
             (discharge_timed[i], charge_timed[i]) = (bms_loss if (charge_timed[i] >= discharge_timed[i]) else (discharge_timed[i] - charge_timed[i]),
                 0.0 if (charge_timed[i] <= export_limit * 1000 + discharge_timed[i]) else (charge_timed[i] - export_limit * 1000 - discharge_timed[i]))
         else: # work_mode == 'SelfUse'
             (discharge_timed[i], charge_timed[i]) = (bms_loss if (charge_timed[i] >= discharge_timed[i]) else (discharge_timed[i] - charge_timed[i]),
                 0.0 if (charge_timed[i] <= discharge_timed[i]) else (charge_timed[i] - discharge_timed[i]))
-    # track the battery residual over the run time (if we don't add any charge)
-    # adjust residual from hour_now to what it was at the start of current hour
-    h = base_hour
+    # build the battery residual if we don't add any charge and don't limit discharge at  min_soc
     kwh_timed = [charge * charge_loss - discharge for charge, discharge in zip(charge_timed, discharge_timed)]
-    kwh_current = residual - kwh_timed[0] * (hour_now - h)
-    bat_timed = []
-    kwh_min = capacity
-    reserve_drain_now = reserve
-    min_soc_now = min_soc
-    for i in range(0, run_time):
-        reserve_now = capacity * min_soc_now / 100
-        reserve_drain = capacity * (min_soc_now - 4) / 100
-        reserve_drain_now = reserve_now if reserve_drain_now > reserve_now or reserve_drain_now < reserve_drain else reserve_drain_now
-#        print(f"h={h}, min_soc_now={min_soc_now}, reserve_now={reserve_now}, kwh_current={kwh_current}")
-        if kwh_current <= reserve_now and i <= time_to_next:
-            # battery is empty
-            kwh_current = reserve_drain_now        # stop discharge below reserve
-            reserve_drain_now -= bms_loss          # allow for BMS drain
-        else:
-            reserve_drain_now = reserve_now           # reset drain
-        if kwh_current > capacity:
-            # battery is full
-            kwh_current = capacity
-        bat_timed.append(kwh_current)
-        if kwh_current < kwh_min and i >= time_to_next:       # track minimum after next charge
-            kwh_min = kwh_current
-        kwh_current += kwh_timed[i]
-        min_soc_now = work_mode_timed[i]['fdsoc'] if work_mode_timed[i]['mode'] =='ForceDischarge' else work_mode_timed[i]['min_soc']
-        h += 1
+    kwh_current = residual - kwh_timed[0] * (hour_now % 1)
+    (bat_timed, kwh_min) = battery_timed(kwh_timed, work_mode_timed, kwh_current, capacity, time_to_next, float_charge, kwh_min=capacity)
     # work out what we need to add to stay above reserve and provide contingency or to hit target_soc
     contingency = charge_config['special_contingency'] if tomorrow[-5:] in charge_config['special_days'] else charge_config['contingency']
     contingency = contingency[quarter] if type(contingency) is list else contingency
     kwh_contingency = consumption * contingency / 100
     kwh_needed = reserve + kwh_contingency - kwh_min
     start_residual = interpolate(time_to_start, bat_timed)      # residual when charging starts
     target_soc = charge_config['target_soc'] if charge_config.get('target_soc') is not None else 10
@@ -2849,14 +2892,17 @@
         output(f"\nNo charging is needed (forecast = {expected:.1f}kWh, consumption = {consumption:.1f}kWh, contingency = {kwh_contingency:.1f}kWh)")
         charge_message = "no charge needed"
         kwh_needed = 0.0
         hours = 0.0
         end1 = start_at
         end_soc = int(start_residual / capacity * 100 + 0.5)
         output(f"   Expected SoC at {hours_time(start_at)} is {end_soc}%")
+        # rebuild the battery residual with min_soc
+        kwh_current = residual - kwh_timed[0] * (hour_now % 1)
+        (bat_timed, x) = battery_timed(kwh_timed, work_mode_timed, kwh_current, capacity, time_to_next, float_charge)
     else:
         charge_message = "with charge added"
         if test_charge is None:
             output(f"\nCharge of {kwh_needed:.2f}kWh is needed (forecast = {expected:.1f}kWh, consumption = {consumption:.1f}kWh, contingency = {kwh_contingency:.1f}kWh)")
         else:
             output(f"\nTest charge of {test_charge}kWh")
             charge_message = "** test charge **"
@@ -2867,15 +2913,14 @@
         # full charge if requested or charge time exceeded or charge needed exceeds capacity
         if full_charge is not None or force_charge == 2 or hours > charge_time or (start_residual + kwh_needed) > (capacity * 1.01):
             kwh_needed = capacity - start_residual
             hours = charge_time
             output(f"  Full charge time used")
         elif hours < charge_config['min_hours']:
             hours = charge_config['min_hours']
-#            output(f"  Minimum charge time used")
         end1 = round_time(start_at + hours)
         # rework charge and discharge
         start_timed = time_to_start      # relative start and end time 
         end_timed = start_timed + hours
         charge_timed_old = [x for x in charge_timed]
         discharge_timed_old = [x for x in discharge_timed]
         for i in range(time_to_next, int(time_to_next + hours + 2)):
@@ -2892,48 +2937,38 @@
             else:
                 t = 0.0                             # complete hour before start or after end
             if debug_setting > 2:
                 print(f"i = {i}, j = {j}, t = {t}")
             charge_added = charge_limit * t
             charge_timed[i] = charge_timed[i] + charge_added if charge_timed[i] + charge_added < charge_limit else charge_limit
             discharge_timed[i] *= (1-t)
-        # rebuild the battery residual with the charge added
-        # adjust residual from hour_now to what it was at the start of current hour
-        h = base_hour
+        # rebuild the battery residual with the charge added and min_soc
         kwh_timed = [charge * charge_loss - discharge for charge, discharge in zip(charge_timed, discharge_timed)]
-        kwh_current = residual - kwh_timed[0] * (hour_now - h)
+        kwh_current = residual - kwh_timed[0] * (hour_now % 1)
         bat_timed_old = [x for x in bat_timed]     # save for before / after comparison
         bat_timed = []
-        reserve_drain_now = reserve
-        for i in range(0, run_time):
-            reserve_now = capacity * min_soc_now / 100
-            reserve_drain = capacity * (min_soc_now - 4) / 100
-            reserve_drain_now = reserve_now if reserve_drain_now > reserve_now or reserve_drain_now < reserve_drain else reserve_drain_now 
-            if kwh_current <= reserve_now and i <= time_to_next:
-                # battery is empty
-                kwh_current = reserve_drain_now        # stop discharge below reserve
-                reserve_drain_now -= bms_loss          # allow for BMS drain
-            else:
-                reserve_drain_now = reserve_now           # reset drain
-            if kwh_current > capacity:
-                # battery is full
-                kwh_current = capacity
-            bat_timed.append(kwh_current)
-            kwh_current += kwh_timed[i]
-            min_soc_now = work_mode_timed[i]['fdsoc'] if work_mode_timed[i]['mode'] =='ForceDischarge' else work_mode_timed[i]['min_soc']
-            h += 1
+        (bat_timed, x) = battery_timed(kwh_timed, work_mode_timed, kwh_current, capacity, time_to_next, float_charge)
+        # work out the new state
         time_to_end = int(start_timed + hours) + 1
         kwh_added = bat_timed[time_to_end] - bat_timed_old[time_to_end]
         end_part_hour = end_timed - int(end_timed)
         old_residual = interpolate(end_timed, bat_timed_old)
         new_residual = capacity if old_residual + kwh_added > capacity else old_residual + kwh_added
         net_added = new_residual - start_residual
         end_soc = int(new_residual / capacity * 100 + 0.5)
         output(f"  Start SoC: {start_residual / capacity * 100:3.0f}% at {hours_time(start_at)} ({start_residual:.2f}kWh)")
         output(f"  End SoC:   {end_soc:3.0f}% at {hours_time(end1)} ({new_residual:.2f}kWh)")
+    # work out charge periods settings
+    start2 = round_time(start_at if hours == 0 else end1)
+    if force_charge > 0 and hour_in(start2, {'start':start_at, 'end': end_by}):
+        end2 = end_by
+        for i in range(0, int(charge_time + 0.5)):
+            work_mode_timed[time_to_next + i]['min_soc'] = end_soc
+    else:
+        end2 = start2
     if show_data > 2:
         output(f"\nTime, Generation, Charge, Consumption, Discharge, Residual, kWh")
         for i in range(0, run_time):
             h = base_hour + i
             output(f"  {hours_time(h)}, {generation_timed[i]:6.3f}, {charge_timed[i]:6.3f}, {consumption_timed[i]:6.3f}, {discharge_timed[i]:6.3f}, {bat_timed[i]:6.3f}")
         if kwh_needed > 0 and show_data > 3:
             output(f"\nTime, Generation, Charge, Consumption, Discharge, Residual, kWh (before charging)")
@@ -2954,44 +2989,38 @@
     if show_plot > 0:
         print()
         plt.figure(figsize=(figure_width, figure_width/2))
         x_timed = [i for i in range(0, run_time)]
         plt.xticks(ticks=x_timed, labels=[hours_time(base_hour + x - (hour_adjustment if (base_hour + x) >= change_hour else 0), day=False) for x in x_timed], rotation=90, fontsize=8, ha='center')
         if show_plot == 1:
             title = f"Battery SoC % ({charge_message})"
-            plt.plot(x_timed, [round(bat_timed[x] * 100 / capacity,1) for x in x_timed], label='Battery', color='blue')
+            plt.plot(x_timed, [round(bat_timed[x] * 100 / capacity, 1) for x in x_timed], label='Battery', color='blue')
+            plt.plot(x_timed, [work_mode_timed[x]['min_soc'] for x in x_timed], label='Reserve', color='grey', linestyle='dotted')
         else:
             title = f"Energy Flow kWh ({charge_message})"
             plt.plot(x_timed, bat_timed, label='Battery', color='blue')
             plt.plot(x_timed, generation_timed, label='Generation', color='green')
             plt.plot(x_timed, consumption_timed, label='Consumption', color='red')
-#            if kwh_needed > 0:
-#                plt.plot(x_timed, bat_timed_old, label='Battery (before charging)', color='blue', linestyle='dotted')
+            plt.plot(x_timed, [round(capacity * work_mode_timed[x]['min_soc'] / 100, 1) for x in x_timed], label='Reserve', color='grey', linestyle='dotted')
             if show_plot == 3:
                 plt.plot(x_timed, charge_timed, label='Charge', color='orange', linestyle='dotted')
                 plt.plot(x_timed, discharge_timed, label='Discharge', color='brown', linestyle='dotted')
         plt.title(title, fontsize=10)
         plt.grid()
         if show_plot > 1:
             plt.legend(fontsize=8, loc="upper right")
         plot_show()
     if test_charge is not None:
         return None
-    # work out charge periods settings
-    start2 = round_time(start_at if hours == 0 else end1)
-    if force_charge > 0 and hour_in(start2, {'start':start_at, 'end': end_by}):
-        end2 = end_by
-    else:
-            end2 = start2
     # setup charging
     if update_settings == 1:
         # adjust times for clock changes
         adjust = hour_adjustment if hour_adjustment != 0 and start_hour > change_hour else 0
         if timed_mode > 1:
-            periods = charge_strategy(st1 = start_at, en1 = end1, st2 = start2, en2 = end2, adjust = adjust, min_soc = min_soc, target_soc = end_soc if target_soc <= 10 else target_soc)
+            periods = charge_periods(st1 = start_at, en1 = end1, st2 = start2, en2 = end2, adjust = adjust, min_soc = min_soc, target_soc = end_soc if target_soc <= 10 else target_soc)
             set_schedule(periods = periods)
         else:
             set_charge(ch1 = True, st1 = start_at, en1 = end1, ch2 = False, st2 = start2, en2 = end2, adjust = adjust, force = charge_config['force'])
     else:
         print(f"\nNo changes made to charge settings")
     output_close(plot=show_plot)
     return None
```

### Comparing `foxesscloud-2.2.7/src/foxesscloud/openapi.py` & `foxesscloud-2.2.8/src/foxesscloud/openapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################################
 """
 Module:   Fox ESS Cloud using Open API
-Updated:  22 May 2024
+Updated:  24 May 2024
 By:       Tony Matthews
 """
 ##################################################################################################
 # Code for getting and setting inverter data via the Fox ESS cloud api site, including
 # getting forecast data from solcast.com.au and sending inverter data to pvoutput.org
 # ALL RIGHTS ARE RESERVED © Tony Matthews 2024
 ##################################################################################################
 
-version = "2.2.7"
+version = "2.2.8"
 print(f"FoxESS-Cloud Open API version {version}")
 
 debug_setting = 1
 
 # constants
 month_names = ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', 'December']
 day_names = ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday']
@@ -653,25 +653,28 @@
         else:
             output(f"** set_charge(), {errno_message(response)}")
         return None
     else:
         output(f"success", 2) 
     return battery_settings
 
-def charge_strategy(st1 = None, en1 = None, st2 = None, en2 = None, adjust=0, min_soc=10, target_soc=None):
+def charge_periods(st1 = None, en1 = None, st2 = None, en2 = None, adjust=0, min_soc=10, target_soc=None):
     output(f"\nConfiguring schedule", 1)
-    periods = set_strategy(min_soc = min_soc, quiet=0)
+    strategy = get_strategy(min_soc=min_soc, quiet=0)
+    periods = []
+    for s in strategy:
+        periods.append(set_period(segment = s, quiet=0))
     if st1 is not None and en1 is not None and st1 != en1:
         st1 = round_time(time_hours(st1) + adjust)
         en1 = round_time(time_hours(en1) + adjust)
-        periods.append(set_group(start = st1, end = en1, mode = 'ForceCharge', min_soc = target_soc, quiet=0))
+        periods.append(set_period(start = st1, end = en1, mode = 'ForceCharge', min_soc = target_soc, quiet=0))
     if st2 is not None and en2 is not None and st2 != en2:
         st2 = round_time(time_hours(st2) + adjust)
         en2 = round_time(time_hours(en2) + adjust)
-        periods.append(set_group(start = st2, end = en2, mode = 'SelfUse', min_soc = target_soc, quiet=0))
+        periods.append(set_period(start = st2, end = en2, mode = 'SelfUse', min_soc = target_soc, quiet=0))
     return periods
 
 ##################################################################################################
 # get min soc settings and save in battery_settings
 ##################################################################################################
 
 def get_min():
@@ -1006,15 +1009,15 @@
         output(f"** get_flag() got response code {response.status_code}: {response.reason}")
         return None
     result = response.json().get('result')
     if result is None:
         output(f"** get_flag(), no result data, {errno_message(response)}")
         return None
     if schedule is None:
-        schedule = {'enable': None, 'support': None, 'groups': None}
+        schedule = {'enable': None, 'support': None, 'periods': None}
     schedule['enable'] = result.get('enable')
     schedule['support'] = result.get('support')
     return result
 
 ##################################################################################################
 # get schedule
 ##################################################################################################
@@ -1031,30 +1034,37 @@
         output(f"** get_schedule() got response code {response.status_code}: {response.reason}")
         return None
     result = response.json().get('result')
     if result is None:
         output(f"** get_schedule(), no result data, {errno_message(response)}")
         return None
     schedule['enable'] = result['enable']
-    schedule['groups'] = []
-    # remove invalid work mode from groups
+    schedule['periods'] = []
+    # remove invalid work mode from periods
     for g in result['groups']:
         if g['workMode'] in work_modes:
-            schedule['groups'].append(g)
+            schedule['periods'].append(g)
     return schedule
 
 ##################################################################################################
 # set schedule
 ##################################################################################################
 
 # create time segment structure. Note: end time is exclusive.
-def set_group(start, end, mode=None, min_soc=None, fdsoc=None, fdpwr=None, enable=1, quiet=1):
+def set_period(start=None, end=None, mode=None, min_soc=None, fdsoc=None, fdpwr=None, segment=None, enable=1, quiet=1):
+    if segment is not None and type(segment) is dict:
+        start = segment.get('start')
+        end = segment.get('end')
+        mode = segment.get('mode')
+        min_soc = segement.get('min_soc')
+        fdsoc = segment.get('fdsoc')
+        fdpwr = segmenet.get('fdsoc')
     start = time_hours(start)
     end = time_hours(end)
-    if start is None or end is None:
+    if start is None or end is None or start >= end:
         return None
     end = round_time(end - 1/60)        # adjust exclusive time to inclusive
     mode = 'SelfUse' if mode is None else mode
     if mode not in work_modes:
         output(f"** mode must be one of {work_modes}")
         return None
     min_soc = 10 if min_soc is None else min_soc
@@ -1066,63 +1076,46 @@
     if fdpwr < 0 or fdpwr > 6000:
         output(f"** fdpwr must be between 0 and 6000")
         return None
     if fdsoc < min_soc or fdsoc > 100:
         output(f"** fdsoc must between {min_soc} and 100")
         return None
     if quiet == 0:
-        output(f"   {hours_time(start)} to {hours_time(end)}: {mode} with min_soc = {min_soc}%" + (f", fdPwr = {fdpwr/1000:.3f}kW and fdSoC = {fdsoc}%" if mode == 'ForceDischarge' else ""), 1)
+        output(f"   {hours_time(start)} to {hours_time(end)} {mode} with min_soc = {min_soc}%" + (f", fdPwr = {fdpwr/1000:.3f}kW and fdSoC = {fdsoc}%" if mode == 'ForceDischarge' else ""), 1)
     start_hour, start_minute = split_hours(start)
     end_hour, end_minute = split_hours(end)
-    group = {'enable': enable, 'startHour': start_hour, 'startMinute': start_minute, 'endHour': end_hour, 'endMinute': end_minute, 'workMode': mode, 'minSocOnGrid': min_soc, 'fdSoc': fdsoc, 'fdPwr': fdpwr}
-    return group
-
-# create groups from a list of strategy periods
-def set_strategy(strategy=None, min_soc=10, quiet=1):
-    global tariff
-    if strategy is None and tariff is not None:
-        strategy = tariff.get('strategy')
-    if strategy is None:
-        return []
-    if type(strategy) is not list:
-        strategy = [strategy]
-    periods = []
-    for s in strategy:
-        min_soc = s['min_soc'] if s.get('min_soc') is not None and s['min_soc'] > min_soc else min_soc
-        p = set_group(s['start'], s['end'], s['mode'], min_soc, s.get('fdsoc'), s.get('fdpwr'), quiet=quiet)
-        if p is not None:
-            periods.append(p)
-    return periods
+    period = {'enable': enable, 'startHour': start_hour, 'startMinute': start_minute, 'endHour': end_hour, 'endMinute': end_minute, 'workMode': mode, 'minSocOnGrid': min_soc, 'fdSoc': fdsoc, 'fdPwr': fdpwr}
+    return period
 
-# set a schedule from a period or list of time segment groups
-def set_schedule(groups=None, enable=1):
+# set a schedule from a period or list of time segment periods
+def set_schedule(periods=None, enable=1):
     global token, device_sn, debug_setting, schedule
     if get_flag() is None:
         return None
-    output(f"set_schedule(): enable = {enable}, groups = {groups}", 2)
+    output(f"set_schedule(): enable = {enable}, periods = {periods}", 2)
     if debug_setting > 1:
         return None
     if enable == 0:
         output(f"\nDisabling schedule", 1)
     else:
         output(f"\nEnabling schedule", 1)
-    if groups is not None:
-        if type(groups) is not list:
-            groups = [groups]
-        body = {'deviceSN': device_sn, 'groups': groups}
+    if periods is not None:
+        if type(periods) is not list:
+            periods = [periods]
+        body = {'deviceSN': device_sn, 'groups': periods}
         setting_delay()
         response = signed_post(path="/op/v0/device/scheduler/enable", body=body)
         if response.status_code != 200:
-            output(f"** set_schedule() groups response code {response.status_code}: {response.reason}")
+            output(f"** set_schedule() periods response code {response.status_code}: {response.reason}")
             return None
         errno = response.json().get('errno')
         if errno != 0:
             output(f"** set_schedule(), enable, {errno_message(response)}")
             return None
-        schedule['groups'] = groups
+        schedule['periods'] = periods
     body = {'deviceSN': device_sn, 'enable': enable}
     setting_delay()
     response = signed_post(path="/op/v0/device/scheduler/set/flag", body=body)
     if response.status_code != 200:
         output(f"** set_schedule() flag response code {response.status_code}: {response.reason}")
         return None
     errno = response.json().get('errno')
@@ -1822,18 +1815,14 @@
 octopus_flux = {
     'name': 'Octopus Flux',
     'off_peak1': {'start': 2.0, 'end': 5.0, 'force': 1},        # off-peak period 1 / am charging period
     'off_peak2': {'start': 0.0, 'end': 0.0, 'force': 0},        # off-peak period 2 / pm charging period
     'peak': {'start': 16.0, 'end': 19.0 },                      # peak period 1
     'peak2': {'start': 0.0, 'end': 0.0 },                       # peak period 2
     'forecast_times': [22, 23],                                 # hours in a day to get a forecast
-    'strategy': [                                               # timed work mode settings
-        {'start': 0, 'end': 2, 'mode': 'Feedin'},
-        {'start': 5, 'end': 6, 'mode': 'SelfUse'},
-        {'start': 16, 'end': 24, 'mode': 'Feedin'}]
     }
 
 # time periods for Intelligent Octopus
 intelligent_octopus = {
     'name': 'Intelligent Octopus',
     'off_peak1': {'start': 23.5, 'end': 5.5, 'force': 1},
     'off_peak2': {'start': 0.0, 'end': 0.0, 'force': 0},
@@ -1901,14 +1890,72 @@
     'forecast_times': [22, 23]
     }
 
 tariff_list = [octopus_flux, intelligent_octopus, octopus_cosy, octopus_go, agile_octopus, bg_driver, economy_7, custom_periods]
 tariff = octopus_flux
 
 ##################################################################################################
+# Strategy - schedule templates
+##################################################################################################
+
+# summer strategy for Flux
+flux_strategy_1 = [
+        {'start': 5, 'end': 6, 'mode': 'SelfUse'},
+        {'start': 16, 'end': 24, 'mode': 'Feedin'}]
+
+# winter strategy for Flux
+flux_strategy_2 = [
+        {'start': 2, 'end': 4, 'mode': 'ForceCharge'},
+        {'start': 5, 'end': 6, 'mode': 'SelfUse'},
+        {'start': 16, 'end': 24, 'mode': 'Feedin'}]
+
+# revenue strategy for Flux
+flux_strategy_3 = [
+        {'start': 2, 'end': 4, 'mode': 'ForceCharge'},
+        {'start': 5, 'end': 6, 'mode': 'SelfUse'},
+        {'start': 16, 'end': 18, 'mode': 'ForceDischarge', 'fdsoc': 35, 'fdpwr': 6000},
+        {'start': 18, 'end': 24, 'mode': 'Feedin'}]
+
+flux_strategy_x = [
+        {'start': 2, 'end': 11, 'mode': 'SelfUse', 'min_soc': 80},
+        {'start': 11, 'end': 14, 'mode': 'SelfUse', 'min_soc': 10},
+        {'start': 16, 'end': 24, 'mode': 'Feedin'}]
+
+# return an updated strategy from the tariff strategy that has been filtered for charge times:
+def get_strategy(use=None, strategy=None, min_soc=10, quiet=1):
+    global tariff
+    if use is None:
+        use = tariff
+    if strategy is None and tariff is not None:
+        strategy = tariff.get('strategy')
+    if strategy is None:
+        return []
+    if type(strategy) is not list:
+        strategy = [strategy]
+    updated = []
+    for s in strategy:
+        # move start and end times so they don't overlap the charge periods
+        start = s['start']
+        start = tariff['off_peak1']['end'] if hour_in(start, use['off_peak1']) else tariff['off_peak2']['end'] if hour_in(start, use['off_peak2']) else start
+        end = s['end']
+        end = tariff['off_peak1']['start'] if hour_in(end, use['off_peak1']) else tariff['off_peak2']['start'] if hour_in(end, use['off_peak2']) else end
+        # create segment
+        if start < end:
+            min_soc_now = s['min_soc'] if s.get('min_soc') is not None and s['min_soc'] > min_soc else min_soc
+            mode = s['mode']
+            fdsoc = s.get('fdsoc')
+            fdpwr = s.get('fdpwr')
+            segment = {'start': start, 'end': end, 'mode': mode, 'min_soc': min_soc_now, 'fdsoc': fdsoc, 'fdpwr': fdpwr}
+            if quiet == 0:
+                output(f"   {hours_time(start)} to {hours_time(end)} {mode} with min_soc = {min_soc_now}%" + (f", fdPwr = {fdpwr}W and fdSoC = {fdsoc}%" if mode == 'ForceDischarge' else ""), 1)
+            updated.append(segment)
+    return updated
+
+
+##################################################################################################
 # Octopus Energy Agile Price
 ##################################################################################################
 
 # base settings
 octopus_api_url = "https://api.octopus.energy/v1/products/%PRODUCT%/electricity-tariffs/E-1R-%PRODUCT%-%REGION%/standard-unit-rates/"
 regions = {'A':'Eastern England', 'B':'East Midlands', 'C':'London', 'D':'Merseyside and Northern Wales', 'E':'West Midlands', 'F':'North Eastern England', 'G':'North Western England', 'H':'Southern England',
     'J':'South Eastern England', 'K':'Southern Wales', 'L':'South Western England', 'M':'Yorkshire', 'N':'Southern Scotland', 'P':'Northern Scotland'}
@@ -2142,30 +2189,22 @@
         use['forecast_times'] = forecast_hours
         output(f"Forecast times set to {forecast_times}", 1)
     if strategy is not None:
         if type(strategy) is not list:
             strategy = [strategy]
         use['strategy'] = strategy
         output(f"Strategy updated")
-        set_strategy(strategy, quiet=0)
+        get_strategy(use=use, strategy=strategy, quiet=0)
     if update == 1:
         tariff = use
         output(f"\nTariff set to {tariff['name']}", 1)
     elif debug_setting > 0:
         output(f"\nNo changes made to current tariff", 1)
     return None
 
-# get work mode for a time of day based on the tariff:
-def timed_work_mode(h, default = 'SelfUse'):
-    if tariff is None or tariff.get('strategy') is None:
-        return default
-    for d in tariff['strategy']:
-        if hour_in(h, d):
-            return d['mode']
-    return default
 
 ##################################################################################################
 # CHARGE_NEEDED - calculate charge from current battery charge, forecast yield and expected load
 ##################################################################################################
 
 # how consumption varies by month across a year. 12 values.
 # month                J   F   M   A   M   J   J   A   S   O   N   D
@@ -2241,35 +2280,69 @@
     for h in range(0, 24):
         profile.append(c_float(forecast.daily[tomorrow]['hourly'].get(int(round_time(h - time_offset)))))
     timed = []
     for h in range(int(hour_now), 24):
         timed.append(c_float(forecast.daily[today]['hourly'].get(int(round_time(h - time_offset)))))
     return (timed + profile + profile)[:run_time]
 
-# take a strategy and return a timed profile:
+# build the timed work mode profile from the tariff strategy:
 def strategy_timed(timed_mode, hour_now, run_time, min_soc=10):
     global tariff
     profile = []
+    min_soc_now = min_soc
     for h in range(0, 24):
-        profile.append({'mode': 'SelfUse', 'min_soc': min_soc, 'fdpwr': 0, 'fdsoc': min_soc, 'duration': 1.0})
-        if tariff is None or tariff.get('strategy') is None or timed_mode == 0:
-            continue
-        for d in tariff['strategy']:
-            if hour_in(h, d):
-                profile[h]['mode'] = d['mode']
-                if d.get('min_soc') is not None:
-                    profile[h]['min_soc'] = d['min_soc'] if d['min_soc'] > min_soc else min_soc
-                if d.get('fdsoc') is not None:
-                    profile[h]['fdsoc'] = d['fdsoc'] if d['fdsoc'] > min_soc else min_soc
-                if d.get('fdpwr') is not None:
-                    profile[h]['fdpwr'] = d['fdpwr']
-                profile[h]['duration'] = duration_in(h, d)
+        period = {'mode': 'SelfUse', 'min_soc': min_soc_now, 'fdpwr': 0, 'fdsoc': min_soc_now, 'duration': 1.0}
+        if timed_mode > 0 and tariff is not None and tariff.get('strategy') is not None:
+            for d in tariff['strategy']:
+                if hour_in(h, d):
+                    mode = d['mode']
+                    period['mode'] = mode
+                    min_soc_now = d['min_soc'] if d.get('min_soc') is not None and d['min_soc'] > min_soc else min_soc
+                    period['min_soc'] = min_soc_now
+                    if mode == 'ForceDischarge':
+                        if d.get('fdsoc') is not None:
+                            period['fdsoc'] = d['fdsoc'] if d['fdsoc'] > min_soc_now else min_soc_now
+                        if d.get('fdpwr') is not None:
+                            period['fdpwr'] = d['fdpwr']
+                    period['duration'] = duration_in(h, d)
+        profile.append(period)
     output(f"work mode profile = {profile}", 2)
     return (profile[int(hour_now):] + profile + profile)[:run_time]
 
+# build the timed battery residual from the charge / discharge, work mode and min_soc
+def battery_timed(kwh_timed, work_mode_timed, kwh_current, capacity, time_to_next, float_charge, kwh_min=None, reserve_drain=None):
+    global charge_config
+    bat_timed = []
+    allowed_drain = charge_config['allowed_drain'] if charge_config.get('allowed_drain') is not None else 4
+    bms_loss = charge_config['bms_power'] / 1000 if charge_config.get('bms_power') is not None else 50
+    for i in range(0, len(kwh_timed)):
+        kwh_current += kwh_timed[i]
+        min_soc_now = work_mode_timed[i]['fdsoc'] if work_mode_timed[i]['mode'] =='ForceDischarge' else work_mode_timed[i]['min_soc']
+        reserve_now = capacity * min_soc_now / 100
+        if kwh_current < reserve_now and (i <= time_to_next or kwh_min is None):
+            # battery is empty, check if charge is needed
+            reserve_drain = kwh_current if reserve_drain is None or kwh_current > reserve_drain else reserve_drain
+            kwh_current = reserve_drain
+            reserve_limit = capacity * (min_soc_now - allowed_drain) / 100
+            if reserve_drain < reserve_limit:
+                reserve_drain = min([reserve_now, reserve_drain + float_charge])
+            else:
+                # BMS power drain
+                reserve_drain -= bms_loss
+        else:
+            # reset drain level
+            reserve_drain = reserve_now
+        if kwh_current > capacity:
+            # battery is full
+            kwh_current = capacity
+        bat_timed.append(kwh_current)
+        if kwh_min is not None and kwh_current < kwh_min and i >= time_to_next:       # track minimum without charge
+            kwh_min = kwh_current
+    return (bat_timed, kwh_min)
+
 # Battery open circuit voltage (OCV) from 0% to 100% SoC
 #                 0%     10%    20%    30%    40%    50%    60%    70%    80%    90%   100%
 lifepo4_curve = [51.00, 51.50, 52.00, 52.30, 52.60, 52.80, 52.90, 53.00, 53.10, 53.30, 54.00]
 
 # charge_needed settings
 charge_config = {
     'contingency': [20,10,5,15],      # % of consumption. Value or [winter, spring, summer, autumn]
@@ -2279,15 +2352,17 @@
     'discharge_current': None,        # max battery discharge current setting in A
     'export_limit': None,             # maximum export power in kW
     'discharge_loss': 0.97,           # loss converting battery discharge power to grid power
     'pv_loss': 0.95,                  # loss converting PV power to battery charge power
     'grid_loss': 0.95,                # loss converting grid power to battery charge power
     'charge_loss': None,              # loss converting charge power to residual
     'inverter_power': None,           # Inverter power consumption in W
-    'bms_power': 27,                  # BMS power consumption in W
+    'bms_power': 50,                  # BMS power consumption in W
+    'allowed_drain': 4,               # % tolerance below min_soc before float charge starts
+    'float_current': 4,               # BMS float charge in A
     'bat_resistance': 0.072,          # internal resistance of a battery
     'volt_curve': lifepo4_curve,      # battery OCV range from 0% to 100% SoC
     'nominal_soc': 60,                # SoC for nominal open circuit battery voltage
     'generation_days': 3,             # number of days to use for average generation (1-7)
     'consumption_days': 3,            # number of days to use for average consumption (1-7)
     'consumption_span': 'week',       # 'week' = last n days or 'weekday' = last n weekdays
     'use_today': 21.0,                # hour when todays consumption and generation can be used
@@ -2413,23 +2488,15 @@
     output(f"start_pm = {start_pm}, end_pm = {end_pm}, force_pm = {force_charge_pm}, time_to_pm = {time_to_pm}", 3)
     output(f"start_at = {start_at}, end_by = {end_by}, force_charge = {force_charge}", 3)
     output(f"base_hour = {base_hour}, hour_adjustment = {hour_adjustment}, change_hour = {change_hour}", 3)
     output(f"time_to_start = {time_to_start}, run_time = {run_time}, charge_pm = {charge_pm}", 3)
     output(f"start_hour = {start_hour}, time_to_next = {time_to_next}, full_charge = {full_charge}", 3)
     # get device and battery info from inverter
     if test_soc is None:
-        if charge_config.get('min_soc') is not None:
-            min_soc = charge_config['min_soc']
-        else:
-            get_min()
-            if battery_settings.get('minSocOnGrid') is not None:
-                min_soc = battery_settings['minSocOnGrid']
-            else:
-                output(f"\nMin SoC On Grid is not available. Please provide % via 'min_soc' parameter")
-                return None
+        min_soc = charge_config['min_soc'] if charge_config['min_soc'] is not None else 10
         get_battery()
         current_soc = battery['soc']
         bat_volt = battery['volt']
         bat_power = battery['power']
         bat_current = battery['current']
         temperature = battery['temperature']
         residual = battery['residual']
@@ -2500,14 +2567,15 @@
     elif charge_power < charge_limit:
         charge_limit = charge_power
     # work out losses when charging / force discharging
     inverter_power = charge_config['inverter_power'] if charge_config['inverter_power'] is not None else round(device_power, 0) * 20
     operating_loss = inverter_power / 1000
     bms_power = charge_config['bms_power']
     bms_loss = bms_power / 1000
+    float_charge = (charge_config['float_current'] if charge_config.get('float_current') is not None else 4) * bat_ocv / 1000
     charge_loss = charge_config.get('charge_loss')
     if charge_loss is None:
         charge_loss = 1.0 - charge_limit * 1000 * bat_resistance / bat_ocv ** 2 - bms_loss / charge_limit
     # work out discharge limit = max power coming from the battery before ac conversion losses
     discharge_loss = charge_config['discharge_loss']
     discharge_limit = device_power
     discharge_current = device_current if charge_config['discharge_current'] is None else charge_config['discharge_current']
@@ -2662,54 +2730,29 @@
                 charge_limit * duration + charge_timed[i] * (1.0 - duration))
         elif timed_mode > 0 and work_mode == 'ForceDischarge':
             fdpwr = work_mode_timed[i]['fdpwr'] / charge_config['discharge_loss']
             fdpwr = min([discharge_limit, export_limit * 1000 + discharge_timed[i], fdpwr])
             (discharge_timed[i], charge_timed[i]) = (fdpwr * duration + discharge_timed[i] * (1.0 - duration) - charge_timed[i] * duration,
                 charge_timed[i] * (1.0 - duration))
         elif force_charge_am == 1 and hour_in(h, {'start': start_am, 'end': end_am}):
-            discharge_timed[i] = operating_loss if charge_timed[i] == 0.0 else 0.0
+            discharge_timed[i] = bms_loss
         elif force_charge_pm == 1 and hour_in(h, {'start': start_pm, 'end': end_pm}):
-            discharge_timed[i] = operating_loss if charge_timed[i] == 0.0 else 0.0
+            discharge_timed[i] = bms_loss
         elif timed_mode > 0 and work_mode == 'Backup':
-            discharge_timed[i] = operating_loss if charge_timed[i] == 0.0 else 0.0
+            discharge_timed[i] = bms_loss if charge_timed[i] == 0.0 else 0.0
         elif timed_mode > 0 and work_mode == 'Feedin':
             (discharge_timed[i], charge_timed[i]) = (bms_loss if (charge_timed[i] >= discharge_timed[i]) else (discharge_timed[i] - charge_timed[i]),
                 0.0 if (charge_timed[i] <= export_limit * 1000 + discharge_timed[i]) else (charge_timed[i] - export_limit * 1000 - discharge_timed[i]))
         else: # work_mode == 'SelfUse'
             (discharge_timed[i], charge_timed[i]) = (bms_loss if (charge_timed[i] >= discharge_timed[i]) else (discharge_timed[i] - charge_timed[i]),
                 0.0 if (charge_timed[i] <= discharge_timed[i]) else (charge_timed[i] - discharge_timed[i]))
-    # track the battery residual over the run time (if we don't add any charge)
-    # adjust residual from hour_now to what it was at the start of current hour
-    h = base_hour
+    # build the battery residual if we don't add any charge and don't limit discharge at min_soc
     kwh_timed = [charge * charge_loss - discharge for charge, discharge in zip(charge_timed, discharge_timed)]
-    kwh_current = residual - kwh_timed[0] * (hour_now - h)
-    bat_timed = []
-    kwh_min = capacity
-    reserve_drain_now = reserve
-    min_soc_now = min_soc
-    for i in range(0, run_time):
-        reserve_now = capacity * min_soc_now / 100
-        reserve_drain = capacity * (min_soc_now - 4) / 100
-        reserve_drain_now = reserve_now if reserve_drain_now > reserve_now or reserve_drain_now < reserve_drain else reserve_drain_now
-        if kwh_current <= reserve_now and i <= time_to_next:
-            # battery is empty
-            kwh_current = reserve_drain_now       # stop discharge below reserve
-            reserve_drain_now -= bms_loss         # allow for BMS drain
-        else:
-            reserve_drain_now = reserve_now       # reset drain
-        if kwh_current > capacity:
-            # battery is full
-            kwh_current = capacity
-        bat_timed.append(kwh_current)
-        if kwh_current < kwh_min and i >= time_to_next:       # track minimum after next charge
-            kwh_min = kwh_current
-            min_hour = h
-        kwh_current += kwh_timed[i]
-        min_soc_now = work_mode_timed[i]['fdsoc'] if work_mode_timed[i]['mode'] =='ForceDischarge' else work_mode_timed[i]['min_soc']
-        h += 1
+    kwh_current = residual - kwh_timed[0] * (hour_now % 1)
+    (bat_timed, kwh_min) = battery_timed(kwh_timed, work_mode_timed, kwh_current, capacity, time_to_next, float_charge, kwh_min=capacity)
     # work out what we need to add to stay above reserve and provide contingency or to hit target_soc
     contingency = charge_config['special_contingency'] if tomorrow[-5:] in charge_config['special_days'] else charge_config['contingency']
     contingency = contingency[quarter] if type(contingency) is list else contingency
     kwh_contingency = consumption * contingency / 100
     kwh_needed = reserve + kwh_contingency - kwh_min
     start_residual = interpolate(time_to_start, bat_timed)      # residual when charging starts
     target_soc = charge_config['target_soc'] if charge_config.get('target_soc') is not None else 10
@@ -2721,14 +2764,17 @@
         output(f"\nNo charging is needed (forecast = {expected:.1f}kWh, consumption = {consumption:.1f}kWh, contingency = {kwh_contingency:.1f}kWh)")
         charge_message = "no charge needed"
         kwh_needed = 0.0
         hours = 0.0
         end1 = start_at
         end_soc = int(start_residual / capacity * 100 + 0.5)
         output(f"   Expected SoC at {hours_time(start_at)} is {end_soc}%")
+        # rebuild the battery residual with min_soc
+        kwh_current = residual - kwh_timed[0] * (hour_now % 1)
+        (bat_timed, x) = battery_timed(kwh_timed, work_mode_timed, kwh_current, capacity, time_to_next, float_charge)
     else:
         charge_message = "with charge added"
         if test_charge is None:
             output(f"\nCharge of {kwh_needed:.2f}kWh is needed (forecast = {expected:.1f}kWh, consumption = {consumption:.1f}kWh, contingency = {kwh_contingency:.1f}kWh)")
         else:
             output(f"\nTest charge of {test_charge}kWh")
             charge_message = "** test charge **"
@@ -2739,15 +2785,14 @@
         # full charge if requested or charge time exceeded or charge needed exceeds capacity
         if full_charge is not None or force_charge == 2 or hours > charge_time or (start_residual + kwh_needed) > (capacity * 1.01):
             kwh_needed = capacity - start_residual
             hours = charge_time
             output(f"  Full charge time used")
         elif hours < charge_config['min_hours']:
             hours = charge_config['min_hours']
-#            output(f"  Minimum charge time used")
         end1 = round_time(start_at + hours)
         # rework charge and discharge
         start_timed = time_to_start      # relative start and end time 
         end_timed = start_timed + hours
         charge_timed_old = [x for x in charge_timed]
         discharge_timed_old = [x for x in discharge_timed]
         for i in range(time_to_next, int(time_to_next + hours + 2)):
@@ -2763,48 +2808,38 @@
                 t = 1.0                             # complete hour inside start and end
             else:
                 t = 0.0                             # complete hour before start or after end
             output(f"i = {i}, j = {j}, t = {t}", 3)
             charge_added = charge_limit * t
             charge_timed[i] = charge_timed[i] + charge_added if charge_timed[i] + charge_added < charge_limit else charge_limit
             discharge_timed[i] *= (1-t)
-        # rebuild the battery residual with the charge added
-        # adjust residual from hour_now to what it was at the start of current hour
-        h = base_hour
+        # rebuild the battery residual with the charge added and min_soc
         kwh_timed = [charge * charge_loss - discharge for charge, discharge in zip(charge_timed, discharge_timed)]
-        kwh_current = residual - kwh_timed[0] * (hour_now - h)
+        kwh_current = residual - kwh_timed[0] * (hour_now % 1)
         bat_timed_old = [x for x in bat_timed]     # save for before / after comparison
         bat_timed = []
-        reserve_drain_now = reserve
-        for i in range(0, run_time):
-            reserve_now = capacity * min_soc_now / 100
-            reserve_drain = capacity * (min_soc_now - 4) / 100
-            reserve_drain_now = reserve_now if reserve_drain_now > reserve_now or reserve_drain_now < reserve_drain else reserve_drain_now 
-            if kwh_current <= reserve_now and i <= time_to_next:
-                # battery is empty
-                kwh_current = reserve_drain_now       # stop discharge below reserve
-                reserve_drain_now -= bms_loss         # BMS drain
-            else:
-                reserve_drain_now = reserve_now       # reset drain
-            if kwh_current > capacity:
-                # battery is full
-                kwh_current = capacity
-            bat_timed.append(kwh_current)
-            kwh_current += kwh_timed[i]
-            min_soc_now = work_mode_timed[i]['fdsoc'] if work_mode_timed[i]['mode'] =='ForceDischarge' else work_mode_timed[i]['min_soc']
-            h += 1
+        (bat_timed, x) = battery_timed(kwh_timed, work_mode_timed, kwh_current, capacity, time_to_next, float_charge)
+        # work out the new state
         time_to_end = int(start_timed + hours) + 1
         kwh_added = bat_timed[time_to_end] - bat_timed_old[time_to_end]
         end_part_hour = end_timed - int(end_timed)
         old_residual = interpolate(end_timed, bat_timed_old)
         new_residual = capacity if old_residual + kwh_added > capacity else old_residual + kwh_added
         net_added = new_residual - start_residual
         end_soc = int(new_residual / capacity * 100 + 0.5)
         output(f"  Start SoC: {start_residual / capacity * 100:3.0f}% at {hours_time(start_at)} ({start_residual:.2f}kWh)")
         output(f"  End SoC:   {end_soc:3.0f}% at {hours_time(end1)} ({new_residual:.2f}kWh)")
+    # work out charge periods settings
+    start2 = round_time(start_at if hours == 0 else end1)
+    if force_charge > 0 and hour_in(start2, {'start':start_at, 'end': end_by}):
+        end2 = end_by
+        for i in range(0, int(charge_time + 0.5)):
+            work_mode_timed[time_to_next + i]['min_soc'] = end_soc
+    else:
+        end2 = start2
     if show_data > 2:
         output(f"\nTime, Generation, Charge, Consumption, Discharge, Residual, kWh")
         for i in range(0, run_time):
             h = base_hour + i
             output(f"  {hours_time(h)}, {generation_timed[i]:6.3f}, {charge_timed[i]:6.3f}, {consumption_timed[i]:6.3f}, {discharge_timed[i]:6.3f}, {bat_timed[i]:6.3f}")
         if kwh_needed > 0 and show_data > 3:
             output(f"\nTime, Generation, Charge, Consumption, Discharge, Residual, kWh (before charging)")
@@ -2826,44 +2861,38 @@
         print()
         plt.figure(figsize=(figure_width, figure_width/2))
         x_timed = [i for i in range(0, run_time)]
         plt.xticks(ticks=x_timed, labels=[hours_time(base_hour + x - (hour_adjustment if (base_hour + x) >= change_hour else 0), day=False) for x in x_timed], rotation=90, fontsize=8, ha='center')
         if show_plot == 1:
             title = f"Battery SoC % ({charge_message})"
             plt.plot(x_timed, [round(bat_timed[x] * 100 / capacity,1) for x in x_timed], label='Battery', color='blue')
+            plt.plot(x_timed, [work_mode_timed[x]['min_soc'] for x in x_timed], label='Reserve', color='grey', linestyle='dotted')
         else:
             title = f"Energy Flow kWh ({charge_message})"
             plt.plot(x_timed, bat_timed, label='Battery', color='blue')
             plt.plot(x_timed, generation_timed, label='Generation', color='green')
             plt.plot(x_timed, consumption_timed, label='Consumption', color='red')
-#            if kwh_needed > 0:
-#                plt.plot(x_timed, bat_timed_old, label='Battery (before charging)', color='blue', linestyle='dotted')
+            plt.plot(x_timed, [round(capacity * work_mode_timed[x]['min_soc'] / 100, 1) for x in x_timed], label='Reserve', color='grey', linestyle='dotted')
             if show_plot == 3:
                 plt.plot(x_timed, charge_timed, label='Charge Avail.', color='orange', linestyle='dotted')
                 plt.plot(x_timed, discharge_timed, label='Discharge', color='brown', linestyle='dotted')
         plt.title(title, fontsize=10)
         plt.grid()
         if show_plot > 1:
             plt.legend(fontsize=8, loc="upper right")
         plot_show()
     if test_charge is not None:
         return None
-    # work out charge periods settings
-    start2 = round_time(start_at if hours == 0 else end1)
-    if force_charge > 0 and hour_in(start2, {'start':start_at, 'end': end_by}):
-        end2 = end_by
-    else:
-        end2 = start2
     # setup charging
     if update_settings == 1:
         # adjust times for clock changes
         adjust = hour_adjustment if hour_adjustment != 0 and start_hour > change_hour else 0
         if timed_mode > 1:
-            groups = charge_strategy(st1 = start_at, en1 = end1, st2 = start2, en2 = end2, adjust = adjust, min_soc = min_soc, target_soc = end_soc if target_soc <= 10 else target_soc)
-            set_schedule(groups)
+            periods = charge_periods(st1 = start_at, en1 = end1, st2 = start2, en2 = end2, adjust = adjust, min_soc = min_soc, target_soc = end_soc if target_soc <= 10 else target_soc)
+            set_schedule(periods)
         else:
             set_charge(ch1 = True, st1 = start_at, en1 = end1, ch2 = False, st2 = start2, en2 = end2, adjust = adjust, force = charge_config['force'])
     else:
         output(f"\nNo changes made to charge settings")
     output_close(plot=show_plot)
     return None
```

### Comparing `foxesscloud-2.2.7/src/foxesscloud.egg-info/PKG-INFO` & `foxesscloud-2.2.8/src/foxesscloud.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxesscloud
-Version: 2.2.7
+Version: 2.2.8
 Summary: library for accessing Fox ESS cloud data using Open API
 Author-email: Tony Matthews <tony@quasair.co.uk>
 Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -118,50 +118,48 @@
 
 ## Inverter Settings
 You can change inverter settings using:
 
 ```
 f.set_min(minSocOnGrid, minSoc)
 f.set_charge(ch1, st1, en1, ch2, st2, en2)
-f.set_group(start, end, mode, min_soc, fdsoc, fdpwr)
-f.set_strategy(strategy)
-f.charge_strategy(st1, en1, st2, en2, min_soc)
-f.set_schedule(groups, enable)
+f.set_period(start, end, mode, min_soc, fdsoc, fdpwr, segment)
+f.charge_periods(st1, en1, st2, en2, min_soc)
+f.set_schedule(periods, enable)
 ```
 
 set_min() applies new SoC settings to the inverter. The parameters update battery_settings:
 + minSocOnGrid: min Soc on Grid setting e.g. 15 = 15%
 + minSoc: min Soc setting e.g. 10 = 10%
 
 set_charge() takes the charge times from the battery_settings and applies these to the inverter. The parameters are optional and will update battery_settings. You should specify all 3 parameter for a time period:
 + ch1: enable charge from grid for period 1 (True or False)
 + st1: the start time for period 1
 + en1: the end time for period 1
 + ch2: enable charge from grid for period 2 (True or False)
 + st2: the start time for period 2
 + en2: the end time for period 2
 
-set_group() returns a time segment structure that can be used to build a list of time segments for set_schedule()
+set_period() returns a period structure that can be used to build a list for set_schedule()
 + start, end, mode: required parameters. end time is exclusive e.g. end at '07:00' will set a period end time of '06:59'
 + min_soc: optional, default is 10
 + fdsoc: optional, default is 10. Used when setting a period with ForceDischarge mode
 + fdpwr: optional, default is 0. Used when setting a period with ForceDischarge mode
 + enable: sets whether this time segment is enable (1) or disabled (0). The default is enabled.
++ segment: optional, allows the parameters for the period to be passed as a dictionary instead of individual values.
 
-set_strategy() creates a list of groups from the strategy. If strategy is not provided, it uses the strategy for the current tariff.
-
-charge_strategy(): returns a list of groups that describe the strategy for the current tariff and adds the groupd required for charging:
+charge_periods(): returns a list of periods that describe the strategy for the current tariff and adds the periods required for charging:
 + st1: the start time for the period when the battery charges from the grid
 + en1: the end time for period 1
 + st2: the start time for period when the battery is held at min_soc
 + en2: the end time for period 2
 + min_soc: the min_soc to use after the charge period, when you don't want the battery to discharge below this level
 
 set_schedule() configures a list of scheduled work mode / soc changes with enable=1. If called with enable=0, any existing schedules are disabled. To enable a schedule, you must provide a list of time segments
-+ groups: a time segment or list of time segments created using f.set_group().
++ periods: a time segment or list of time segments created using f.set_period().
 + enable: 1 to enable schedules, 0 to disable schedules. The default is 1.
 
 
 ## Real Time Data
 Real time data reports the latest values for inverter variables, collected every 5 minutes:
 
 ```
@@ -355,15 +353,17 @@
 discharge_current: None       # max battery discharge current setting in A. None uses a value derrived from the inverter model
 export_limit: None            # maximum export power in kW. None uses the inverter power rating
 discharge_loss: 0.97          # loss converting battery discharge power to grid power
 pv_loss: 0.95                 # loss converting PV power to battery charge power
 grid_loss: 0.97               # loss converting grid power to battery charge power
 charge_loss: None             # loss converting charge power to residual
 inverter_power: None          # inverter power consumption in W (dynamically set)
-bms_power: 25                 # BMS power consumption in W
+bms_power: 50                 # BMS power consumption in W
+allowed_drain: 4,             # % tolerance below min_soc before float charge starts
+float_current: 4,             # BMS float charge current in A
 bat_resistance: 0.070         # internal resistance of a battery in ohms
 volt_curve: lifepo4_curve     # battery OCV from 0% to 100% SoC
 nominal_soc: 55               # SoC for nominal open circuit voltage
 generation_days: 3            # number of days to use for average generation (1-7)
 consumption_days: 3           # number of days to use for average consumption (1-7)
 consumption_span: 'week'      # 'week' = last 7 days or 'weekday' = last 7 weekdays e.g. Saturdays
 use_today: 21.0               # hour when today's generation and consumption data will be used
@@ -538,15 +538,24 @@
 + times=[("23:00", "8:00", 3), ("12:00", "16:00", 1)]
 
 'strategy' allows you to configure times when work modes will be changed. The format is a list of dictionary items, containing:
 + 'start', 'end': times in decimal hours or time format. The end time is exclusive so setting an end time of '07:00' will set a schedule that ends at '06:59'
 + 'mode': the work mode to be used from 'SelfUse', 'Feedin', 'Backup', 'ForceCharge', 'ForceDischarge'
 + 'min_soc, 'fdsoc', 'fdpwr': optional values for each work mode. The defaults are 10, 10 and 0 respectively.
 
-The strategy should not include settings for the AM/PM charge times for the tariff. These will be added by charge_needed().
+There are a number of pre-defined strategies:
++ f.flux_strategy_1: switch to self use at 5am and feed in first at 4pm.
++ f.flux_strategy_2: as above with force charge between 2am and 4am. Move the AM charge period between 4am and 5am when using this.
++ f.flux_strategy_3: as above with force discharge between 4pm and 6pm at 6kW with fdsoc at 35%
+
+```
+f.get_strategy()
+```
+
+get_strategy() creates a list of time segments from the strategy. If strategy is not provided, it uses the strategy for the current tariff. If a strategy includes settings for the AM/PM charge times for the tariff, the times will be moved so they do not conflict with the charge time used by charge_needed().
 
 
 # PV Output
 These functions produce CSV data for upload to [pvoutput.org](https://pvoutput.org) including PV generation, Export, Load and Grid consumption by day in Wh. The functions use the energy estimates created from the raw power data (see above). The estimates include PV energy generation that are not otherwise available from the Fox Cloud. Typically, the energy results are within 3% of the values reported by the meters built into the inverter.
 
 
 ## Get PV Output Data
@@ -686,15 +695,19 @@
 + 1: information reporting (default)
 + 2: more debug information, updating of inverter settings is disabled
 + 3: internal variables and values are displayed (verbose)
 
 
 # Version Info
 
-2.2.7<br>
+2.2.8<br>
+** breaking change ** rename 'groups' to 'periods' for consistency between foxesscloud and openapi.
+Updated management of battery reserve and float charging in charge_needed().
+Added Reserve level to charts in charge_needed().
+Changed bms_power setting to 50W.
 Updated contingency to allow seasonal values for winter, spring, summer and autumn.
 Update strategy mode to support ForceCharge and ForceDischarge work modes.
 Update so min_soc setting in charge_needed() over-rides min_soc in the tariff strategy.
 Fix force charge strategy mode in charge_neded() to set min_soc correctly.
 Implement 2 second delay between calls that change inverter settings.
 Added strategy mode (timed_mode=2) to charge_needed().
 Added set_strategy() and charge_strategy() to manage charging schedules and work mode changes.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.7 Summary: library for
+Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.8 Summary: library for
 accessing Fox ESS cloud data using Open API Author-email: Tony Matthews
 quasair.co.uk> Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENCE # FoxESS-Cloud _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]This site contains sample python code
@@ -66,149 +66,149 @@
 result also updates f.battery. get_settings() will return the battery settings
 and is equivalent to get_charge() and get_min(). The results are stored in
 f.battery_settings. The settings include minSoc, minSocOnGrid, enable charge
 from grid and the charge times. get_flag() returns the current scheduler enable
 / support flags get_schedule() returns the current work mode / soc schedule
 settings. The result is stored in f.schedule. ## Inverter Settings You can
 change inverter settings using: ``` f.set_min(minSocOnGrid, minSoc)
-f.set_charge(ch1, st1, en1, ch2, st2, en2) f.set_group(start, end, mode,
-min_soc, fdsoc, fdpwr) f.set_strategy(strategy) f.charge_strategy(st1, en1,
-st2, en2, min_soc) f.set_schedule(groups, enable) ``` set_min() applies new SoC
-settings to the inverter. The parameters update battery_settings: +
-minSocOnGrid: min Soc on Grid setting e.g. 15 = 15% + minSoc: min Soc setting
-e.g. 10 = 10% set_charge() takes the charge times from the battery_settings and
-applies these to the inverter. The parameters are optional and will update
-battery_settings. You should specify all 3 parameter for a time period: + ch1:
-enable charge from grid for period 1 (True or False) + st1: the start time for
-period 1 + en1: the end time for period 1 + ch2: enable charge from grid for
-period 2 (True or False) + st2: the start time for period 2 + en2: the end time
-for period 2 set_group() returns a time segment structure that can be used to
-build a list of time segments for set_schedule() + start, end, mode: required
-parameters. end time is exclusive e.g. end at '07:00' will set a period end
-time of '06:59' + min_soc: optional, default is 10 + fdsoc: optional, default
-is 10. Used when setting a period with ForceDischarge mode + fdpwr: optional,
-default is 0. Used when setting a period with ForceDischarge mode + enable:
-sets whether this time segment is enable (1) or disabled (0). The default is
-enabled. set_strategy() creates a list of groups from the strategy. If strategy
-is not provided, it uses the strategy for the current tariff. charge_strategy
-(): returns a list of groups that describe the strategy for the current tariff
-and adds the groupd required for charging: + st1: the start time for the period
-when the battery charges from the grid + en1: the end time for period 1 + st2:
-the start time for period when the battery is held at min_soc + en2: the end
-time for period 2 + min_soc: the min_soc to use after the charge period, when
-you don't want the battery to discharge below this level set_schedule()
-configures a list of scheduled work mode / soc changes with enable=1. If called
-with enable=0, any existing schedules are disabled. To enable a schedule, you
-must provide a list of time segments + groups: a time segment or list of time
-segments created using f.set_group(). + enable: 1 to enable schedules, 0 to
-disable schedules. The default is 1. ## Real Time Data Real time data reports
-the latest values for inverter variables, collected every 5 minutes: ```
-f.invert_ct2 = 1 f.get_vars() f.get_real(v) ``` f.invert_ct2 determines how the
-meterPower2 data is handled. When invert_ct2 = 0, meterPower2 produces +ve
-power values during secondary generation. If meterPower2 produces -ve power
-values during secondary generation, setting invert_ct2 = 1 will flip the values
-so they are +ve when generating. The default setting is 1 (invert). f.get_vars
-() returns the list of variables that can be queried. This also stores the
-information: + f.var_table: a table, indexed by variable that contains
-information such as the name and unit. ++ f.var_list: a list of all the
-variables that are available There are also pre-defined lists: + power_vars
-lists the main power variables provided by the inverter + battery_vars lists
-the main variables relevant to the battery / BMS f.get_real returns the latest
-values for a list of variables. + v is a variable, or list of variables. The
-default is to return the latest value for all available variables ## History
-Data History data reports inverter variables, collected every 5 minutes, on a
-given date / time and period: ``` f.get_history(time_span, d, v, summary, save,
-load, plot) ``` + time_span determines the period covered by the data, for
-example, 'hour', 'day' or 'week'. The default is 'hour' + d is a date and time
-in the format 'YYYY-MM-DD HH:MM:SS'. The default is today's date and time. d
-may also be a list of dates + v is a variable, or list of variables (see above)
-+ summary is optional - see below + save: set to the root part of a filename to
+f.set_charge(ch1, st1, en1, ch2, st2, en2) f.set_period(start, end, mode,
+min_soc, fdsoc, fdpwr, segment) f.charge_periods(st1, en1, st2, en2, min_soc)
+f.set_schedule(periods, enable) ``` set_min() applies new SoC settings to the
+inverter. The parameters update battery_settings: + minSocOnGrid: min Soc on
+Grid setting e.g. 15 = 15% + minSoc: min Soc setting e.g. 10 = 10% set_charge()
+takes the charge times from the battery_settings and applies these to the
+inverter. The parameters are optional and will update battery_settings. You
+should specify all 3 parameter for a time period: + ch1: enable charge from
+grid for period 1 (True or False) + st1: the start time for period 1 + en1: the
+end time for period 1 + ch2: enable charge from grid for period 2 (True or
+False) + st2: the start time for period 2 + en2: the end time for period 2
+set_period() returns a period structure that can be used to build a list for
+set_schedule() + start, end, mode: required parameters. end time is exclusive
+e.g. end at '07:00' will set a period end time of '06:59' + min_soc: optional,
+default is 10 + fdsoc: optional, default is 10. Used when setting a period with
+ForceDischarge mode + fdpwr: optional, default is 0. Used when setting a period
+with ForceDischarge mode + enable: sets whether this time segment is enable (1)
+or disabled (0). The default is enabled. + segment: optional, allows the
+parameters for the period to be passed as a dictionary instead of individual
+values. charge_periods(): returns a list of periods that describe the strategy
+for the current tariff and adds the periods required for charging: + st1: the
+start time for the period when the battery charges from the grid + en1: the end
+time for period 1 + st2: the start time for period when the battery is held at
+min_soc + en2: the end time for period 2 + min_soc: the min_soc to use after
+the charge period, when you don't want the battery to discharge below this
+level set_schedule() configures a list of scheduled work mode / soc changes
+with enable=1. If called with enable=0, any existing schedules are disabled. To
+enable a schedule, you must provide a list of time segments + periods: a time
+segment or list of time segments created using f.set_period(). + enable: 1 to
+enable schedules, 0 to disable schedules. The default is 1. ## Real Time Data
+Real time data reports the latest values for inverter variables, collected
+every 5 minutes: ``` f.invert_ct2 = 1 f.get_vars() f.get_real(v) ```
+f.invert_ct2 determines how the meterPower2 data is handled. When invert_ct2 =
+0, meterPower2 produces +ve power values during secondary generation. If
+meterPower2 produces -ve power values during secondary generation, setting
+invert_ct2 = 1 will flip the values so they are +ve when generating. The
+default setting is 1 (invert). f.get_vars() returns the list of variables that
+can be queried. This also stores the information: + f.var_table: a table,
+indexed by variable that contains information such as the name and unit. ++
+f.var_list: a list of all the variables that are available There are also pre-
+defined lists: + power_vars lists the main power variables provided by the
+inverter + battery_vars lists the main variables relevant to the battery / BMS
+f.get_real returns the latest values for a list of variables. + v is a
+variable, or list of variables. The default is to return the latest value for
+all available variables ## History Data History data reports inverter
+variables, collected every 5 minutes, on a given date / time and period: ```
+f.get_history(time_span, d, v, summary, save, load, plot) ``` + time_span
+determines the period covered by the data, for example, 'hour', 'day' or
+'week'. The default is 'hour' + d is a date and time in the format 'YYYY-MM-DD
+HH:MM:SS'. The default is today's date and time. d may also be a list of dates
++ v is a variable, or list of variables (see above) + summary is optional - see
+below + save: set to the root part of a filename to save the results + load:
+set to the full filename to load previously saved results + plot is optional. 1
+plots the results with a chart per unit and per day. 2 plots multiple days on
+the same chart. Default is 0, no plots The setting for invert_ct2 is applied to
+history data for meterPower2, so +ve values are returned for secondary
+generation. f.sample_time is set to the sample time in minutes for the data
+processed, rounded to f.sample_rounding samples per minute. Data generation for
+the full list of raw_vars can be slow and return a lot of data, so it's best to
+select the vars you want from the list if you can. For example, this Jupyter
+Lab cell will load an inverter and return power data at 5 minute intervals for
+the 17th June 2023: ``` d = '2023-06-17 00:00:00' result=f.get_history('day',
+d=d, v=f.power_vars) ``` Setting the optional parameter 'summary' when calling
+get_raw() provides a summary of the raw data + summary = 0: basic history data,
+no summary + summary = 1: summary is calculated + summary = 2: summary is
+calculated and raw data is removed to save time / space + summary = 3: as (2)
+but for energy only, an hourly cumulative state is also generated, similar to
+the state used in Home Assistant long term statistics The summary includes the
+following attributes: + count: the number of data points + average: the average
+value of the data points + max: the maximum value of the data points +
+max_time: the time when the maximum value occured (HH:MM) + min: the minimum
+value of the data points + min_time: the time when the minimum value occured
+(HH:MM) For power values (unit = kW), the summary performs a Riemann sum of the
+data, integrating kW over the day to estimate energy in kWh. In this case, the
+following attributes are also added: + kwh: the total energy generated or
+consumed + kwh_off: the total energy consumed or generated during the off-peak
+time of use + kwh_peak: the total energy consumed or generated during the peak
+time of use + kwh_neg: the total energy from -ve power flow (all other totals
+are based on +ve power flow) This example shows power graphs for today and
+yesterday: ![image](https://github.com/TonyM1958/FoxESS-Cloud/assets/63789168/
+d84c55c9-4f4c-431d-bc55-d7796b7e4fea) ## Report Data Report data provides
+information on the energy produced by the inverter, battery charge and
+discharge energy, grid consumption and feed-in energy and home energy
+consumption: ``` f.get_report(report_type, d, v, summary, save, load, plot,
+station) ``` + report_type sets the period covered by the report and is one of
+'day', 'week', 'month', 'year': + when 'day' is selected, energy is reported
+each hour through the day + when 'week' is selected, energy is reported for the
+7 days up to and including the date + when 'month' is selected, energy is
+reported each day through the month + when 'year' is selected, energy is
+reported each month through the year + d is a date and time in the format
+'YYYY-MM-DD HH:MM:SS'. The default is yesterday. d may also be a list of dates
++ v is a variable, or list of variables. The default is to use report_vars +
+summary is optional - see below + save: set to the root part of a filename to
 save the results + load: set to the full filename to load previously saved
-results + plot is optional. 1 plots the results with a chart per unit and per
-day. 2 plots multiple days on the same chart. Default is 0, no plots The
-setting for invert_ct2 is applied to history data for meterPower2, so +ve
-values are returned for secondary generation. f.sample_time is set to the
-sample time in minutes for the data processed, rounded to f.sample_rounding
-samples per minute. Data generation for the full list of raw_vars can be slow
-and return a lot of data, so it's best to select the vars you want from the
-list if you can. For example, this Jupyter Lab cell will load an inverter and
-return power data at 5 minute intervals for the 17th June 2023: ``` d = '2023-
-06-17 00:00:00' result=f.get_history('day', d=d, v=f.power_vars) ``` Setting
-the optional parameter 'summary' when calling get_raw() provides a summary of
-the raw data + summary = 0: basic history data, no summary + summary = 1:
-summary is calculated + summary = 2: summary is calculated and raw data is
-removed to save time / space + summary = 3: as (2) but for energy only, an
-hourly cumulative state is also generated, similar to the state used in Home
-Assistant long term statistics The summary includes the following attributes: +
-count: the number of data points + average: the average value of the data
-points + max: the maximum value of the data points + max_time: the time when
-the maximum value occured (HH:MM) + min: the minimum value of the data points +
-min_time: the time when the minimum value occured (HH:MM) For power values
-(unit = kW), the summary performs a Riemann sum of the data, integrating kW
-over the day to estimate energy in kWh. In this case, the following attributes
-are also added: + kwh: the total energy generated or consumed + kwh_off: the
-total energy consumed or generated during the off-peak time of use + kwh_peak:
-the total energy consumed or generated during the peak time of use + kwh_neg:
-the total energy from -ve power flow (all other totals are based on +ve power
-flow) This example shows power graphs for today and yesterday: ![image](https:/
-/github.com/TonyM1958/FoxESS-Cloud/assets/63789168/d84c55c9-4f4c-431d-bc55-
-d7796b7e4fea) ## Report Data Report data provides information on the energy
-produced by the inverter, battery charge and discharge energy, grid consumption
-and feed-in energy and home energy consumption: ``` f.get_report(report_type,
-d, v, summary, save, load, plot, station) ``` + report_type sets the period
-covered by the report and is one of 'day', 'week', 'month', 'year': + when
-'day' is selected, energy is reported each hour through the day + when 'week'
-is selected, energy is reported for the 7 days up to and including the date +
-when 'month' is selected, energy is reported each day through the month + when
-'year' is selected, energy is reported each month through the year + d is a
-date and time in the format 'YYYY-MM-DD HH:MM:SS'. The default is yesterday. d
-may also be a list of dates + v is a variable, or list of variables. The
-default is to use report_vars + summary is optional - see below + save: set to
-the root part of a filename to save the results + load: set to the full
-filename to load previously saved results + plot is optional. 1 to plot results
-+ station is optional. 1 gets data for a site (using f.station_id), 0 gets data
-for a device (using f.device_id). The default is 0. The list of variables that
-can be reported on is stored in f.report_vars. Note that reporting by 'day'
-produces inaccurate hourly data, where the sum does not reconcile with the
-daily total given in the monthly report. To correct this, reporting by day also
-gets the monthly data and uses the daily total to correctly report the total.
-Setting the optional parameter 'summary' when calling get_report() provides a
-summary of the report data: + summary = 0: basic report data, no summary.
-report_type cannot be 'week' + summary = 1: summary is calculated + summary =
-2: corrected total only is reported to save time / space. report_type must be
-'day' The result data for each variable includes the following attributes when
-summary=2 + 'variable': name of the data set + 'total': corrected total of the
-data items When summary=1, the following items are also added: + 'data':
-'index' and 'value' of each data point + 'date': that was used to produce the
-report + 'count': the number of data items + 'sum': the sum of the data items +
-'max': the biggest value in 'data' + 'max_index': the index of the biggest
-value in 'data' + 'min': the smallest value in 'data' + 'min_index': the index
-of the smallest value in 'data' + 'average': corrected average of the data
-items For example, this Jupyter Lab cell will report energy data by day for the
-month of June 2023: ``` d = '2023-06-17' result=f.get_report('month', d=d) ```
-This example plots weekly data: ![image](https://github.com/TonyM1958/FoxESS-
-Cloud/assets/63789168/f408a010-9600-4b2f-979f-83e32d960586) # Built-in
-Utilities and Operations The previous section provides functions that can be
-used to access and control your inverter. This section covers utilities and
-operations that build upon these functions. ## Charge Needed Uses forecast PV
-yield for tomorrow to work out if charging from grid is needed tonight to
-deliver the expected consumption for tomorrow. If charging is needed, the
-charge times are configured. If charging is not needed, the charge times are
-cleared. The results are sent to the inverter. ``` f.charge_needed(forecast,
-force_charge, forecast_selection, forecast_times, update_setings, show_data,
-show_plot) ``` All the parameters are optional: + forecast: the kWh expected
-tomorrow (optional, see below) + force_charge: 1 any remaining time in a charge
-period has force charge / min_soc set, 2 charging uses the entire charge
-period, 0 None (default) + forecast_selection: if set to 1, settings are only
-updated if there is a forecast. Default is 0, generation is used when forecasts
-are not available + forecast_times: a list of hours when forecasts can be
-obtained. By default, the forecast times for the selected tariff are used (see
-below) + update_settings: 0 no changes, 1 update charge settings. The default
-is 0 + show_data: 1 show battery SoC data, 2 show battery Residual data, 3 show
-timed data, 4 show timed data before and after charging. The default is 1. +
+results + plot is optional. 1 to plot results + station is optional. 1 gets
+data for a site (using f.station_id), 0 gets data for a device (using
+f.device_id). The default is 0. The list of variables that can be reported on
+is stored in f.report_vars. Note that reporting by 'day' produces inaccurate
+hourly data, where the sum does not reconcile with the daily total given in the
+monthly report. To correct this, reporting by day also gets the monthly data
+and uses the daily total to correctly report the total. Setting the optional
+parameter 'summary' when calling get_report() provides a summary of the report
+data: + summary = 0: basic report data, no summary. report_type cannot be
+'week' + summary = 1: summary is calculated + summary = 2: corrected total only
+is reported to save time / space. report_type must be 'day' The result data for
+each variable includes the following attributes when summary=2 + 'variable':
+name of the data set + 'total': corrected total of the data items When
+summary=1, the following items are also added: + 'data': 'index' and 'value' of
+each data point + 'date': that was used to produce the report + 'count': the
+number of data items + 'sum': the sum of the data items + 'max': the biggest
+value in 'data' + 'max_index': the index of the biggest value in 'data' +
+'min': the smallest value in 'data' + 'min_index': the index of the smallest
+value in 'data' + 'average': corrected average of the data items For example,
+this Jupyter Lab cell will report energy data by day for the month of June
+2023: ``` d = '2023-06-17' result=f.get_report('month', d=d) ``` This example
+plots weekly data: ![image](https://github.com/TonyM1958/FoxESS-Cloud/assets/
+63789168/f408a010-9600-4b2f-979f-83e32d960586) # Built-in Utilities and
+Operations The previous section provides functions that can be used to access
+and control your inverter. This section covers utilities and operations that
+build upon these functions. ## Charge Needed Uses forecast PV yield for
+tomorrow to work out if charging from grid is needed tonight to deliver the
+expected consumption for tomorrow. If charging is needed, the charge times are
+configured. If charging is not needed, the charge times are cleared. The
+results are sent to the inverter. ``` f.charge_needed(forecast, force_charge,
+forecast_selection, forecast_times, update_setings, show_data, show_plot) ```
+All the parameters are optional: + forecast: the kWh expected tomorrow
+(optional, see below) + force_charge: 1 any remaining time in a charge period
+has force charge / min_soc set, 2 charging uses the entire charge period, 0
+None (default) + forecast_selection: if set to 1, settings are only updated if
+there is a forecast. Default is 0, generation is used when forecasts are not
+available + forecast_times: a list of hours when forecasts can be obtained. By
+default, the forecast times for the selected tariff are used (see below) +
+update_settings: 0 no changes, 1 update charge settings. The default is 0 +
+show_data: 1 show battery SoC data, 2 show battery Residual data, 3 show timed
+data, 4 show timed data before and after charging. The default is 1. +
 show_plot: 1 plot battery SoC data. 2 plot battery Residual, Generation and
 Consumption. 3 plot 2 + Charge and Discharge The default is 3 ### Modelling
 charge_needed() uses a number of models to better estimate the state of the
 battery. **Manual Consumption:** You can provide your 'annual_consumption' in
 kWh e.g. 5500. This figure is factored down to a daily consumption by dividing
 by 365 and applying **f.seasonality**. This normally decreases consumption in
 the summer and increases it in winter. Seasonality is a list of weightings by
@@ -259,82 +259,83 @@
 value derrived from the inverter model discharge_current: None # max battery
 discharge current setting in A. None uses a value derrived from the inverter
 model export_limit: None # maximum export power in kW. None uses the inverter
 power rating discharge_loss: 0.97 # loss converting battery discharge power to
 grid power pv_loss: 0.95 # loss converting PV power to battery charge power
 grid_loss: 0.97 # loss converting grid power to battery charge power
 charge_loss: None # loss converting charge power to residual inverter_power:
-None # inverter power consumption in W (dynamically set) bms_power: 25 # BMS
-power consumption in W bat_resistance: 0.070 # internal resistance of a battery
-in ohms volt_curve: lifepo4_curve # battery OCV from 0% to 100% SoC
-nominal_soc: 55 # SoC for nominal open circuit voltage generation_days: 3 #
-number of days to use for average generation (1-7) consumption_days: 3 # number
-of days to use for average consumption (1-7) consumption_span: 'week' # 'week'
-= last 7 days or 'weekday' = last 7 weekdays e.g. Saturdays use_today: 21.0 #
-hour when today's generation and consumption data will be used min_hours: 0.25
-# minimum charge time to set (in decimal hours) min_kwh: 0.5 # minimum charge
-to add in kwh solcast_adjust: 100 # % adjustment to make to Solcast forecast
-solar_adjust: 100 # % adjustment to make to Solar forecast forecast_selection:
-1 # 1 = only update charge times if forecast is available, 0 = use best
-available data. Default is 1. annual_consumption: None # optional annual
-consumption in kWh. If set, this replaces consumption history timed_mode: 0 # 0
-= None, 1 = use timed work mode, 2 = strategy mode special_contingency: 30 #
-contingency for special days when consumption might be higher special_days:
-['12-25', '12-26', '01-01'] full_charge: None # day of month (1-28) to do full
-charge or 'daily' or day of week: 'Mon', 'Tue' etc derate_temp: 21 # battery
-temperature in C when derating charge current is applied derate_step: 5 # step
-size for derating e.g. 21, 16, 11 derating: [24, 15, 10, 2] # derated charge
-current for each temperature step e.g. 21C, 16C, 11C, 6C force: 1 # 1 = disable
-strategy periods when setting charge. 0 = fail if strategy period has been set.
-data_wrap: 6 # data items to show per line target_soc: None # target soc for
-charging ``` These values are stored / available in f.charge_config. The
-default battery open circuit voltage curve versus SoC from 0% to 100% is: ```
-lifepo4_curve = [51.30, 52.00, 52.30, 52.40, 52.50, 52.60, 52.70, 52.80, 52.9,
-53.1, 53.50] ``` When operating in strategy mode (timed_mode=2), charge_needed
-will create a schedule that includes the strategy for the tariff with
-additional time segments added to charge from grid and (optionall) to stop the
-battery discharging. In other modes, charge_needed() will disable any schedules
-and set the battery charge times. This example shows the results reported by
-charge needed: ![image](https://github.com/TonyM1958/FoxESS-Cloud/assets/
-63789168/8b77956b-c326-43cd-b165-20d806b1e7e8) ## Battery Info Provides
-detailed information on the current state of the batteries: ``` f.battery_info
-(count, plot, log) f.battery_monitor(interval, run, log, save, count) ```
-battery_info() prints information on the battery and cells: + count: optional
-over-ride. The default is based on factorising the number of cells reported by
-16 or 18 to work out the number of batteries. + plot: 1 plot the cell voltages
-for each battery, 2 plot the cell temperatueres, 0 don't plot. The default is 1
-+ log: see below. Default is 0 battery_monitor() runs battery_info() in log
-mode on a schedule to provide information on the battery status over a period
-of time: + interval: the time in minutes between log entries. The default is 30
-minutes + run: the number of log entries to create. The default is 48 i.e.
-every 30 minues for 24 hours in total + log: 0 = display, 1 = log battery info,
-2 = add cell volts, 3 = add cell temps. The default is 1 + save: name of a CSV
-file to write log data to + count: optional over-ride for the number of
-batteries This is an example of the output from battery_info(): ![image](https:
-//github.com/TonyM1958/FoxESS-Cloud/assets/63789168/a8eb52b6-ce3f-4b58-bb76-
-5483d5e40fa7) ## Date Ranges ``` f.date_list(s, e, limit, span, today) ```
-Returns a list of dates in the format 'YYYY-MM-DD'. This function will not
-return dates in the future. The last date will be yesterday or today (if today
-is True). All parameters are optional: + s: start date + e: end date + limit:
-maximum number of days. The default is 200 + span: the range of dates. One of
-'day', 'week', 'month' or 'year', '2days' or 'weekday' + today: 1 allows today
-to be included, 2 allows future dates to be included. Default is 0, date list
-will stop at yesterday You can use 'span' as follows: + 'day' provides a single
-day + 'week' will provide the dates of 7 consequetive days + 'month' will
-provide the dates of the days up to the same date in the preceeding (or
-follwing) month + '2days' will provide the dates of yesterday and today +
-'weekday' will provide the dates of the same day of the week, going backwards
-(or forwards) up to 7 weeks ``` f.british_summer_time(d) # 1 if d is in Britsh
-Summer Time, 0 if not ``` ## Time Periods Times and time period settings are
-held as decimal hours. Functions for working with time strings with the format
-'HH:MM:SS' and decimal hours include: ``` f.time_hours(t, d=None) # convert
-time to decimal hours. t is a time string ('HH:MM' or 'HH:MM:SS'), d is
-optional and is the default time if s is None f.hours_time(h, mm=True,
-ss=False, day=False) # convert decimal hours to time (HH:MM:SS). mm = include
-minutes, ss = include seconds, day = include /n for day when hours > 24
+None # inverter power consumption in W (dynamically set) bms_power: 50 # BMS
+power consumption in W allowed_drain: 4, # % tolerance below min_soc before
+float charge starts float_current: 4, # BMS float charge current in A
+bat_resistance: 0.070 # internal resistance of a battery in ohms volt_curve:
+lifepo4_curve # battery OCV from 0% to 100% SoC nominal_soc: 55 # SoC for
+nominal open circuit voltage generation_days: 3 # number of days to use for
+average generation (1-7) consumption_days: 3 # number of days to use for
+average consumption (1-7) consumption_span: 'week' # 'week' = last 7 days or
+'weekday' = last 7 weekdays e.g. Saturdays use_today: 21.0 # hour when today's
+generation and consumption data will be used min_hours: 0.25 # minimum charge
+time to set (in decimal hours) min_kwh: 0.5 # minimum charge to add in kwh
+solcast_adjust: 100 # % adjustment to make to Solcast forecast solar_adjust:
+100 # % adjustment to make to Solar forecast forecast_selection: 1 # 1 = only
+update charge times if forecast is available, 0 = use best available data.
+Default is 1. annual_consumption: None # optional annual consumption in kWh. If
+set, this replaces consumption history timed_mode: 0 # 0 = None, 1 = use timed
+work mode, 2 = strategy mode special_contingency: 30 # contingency for special
+days when consumption might be higher special_days: ['12-25', '12-26', '01-01']
+full_charge: None # day of month (1-28) to do full charge or 'daily' or day of
+week: 'Mon', 'Tue' etc derate_temp: 21 # battery temperature in C when derating
+charge current is applied derate_step: 5 # step size for derating e.g. 21, 16,
+11 derating: [24, 15, 10, 2] # derated charge current for each temperature step
+e.g. 21C, 16C, 11C, 6C force: 1 # 1 = disable strategy periods when setting
+charge. 0 = fail if strategy period has been set. data_wrap: 6 # data items to
+show per line target_soc: None # target soc for charging ``` These values are
+stored / available in f.charge_config. The default battery open circuit voltage
+curve versus SoC from 0% to 100% is: ``` lifepo4_curve = [51.30, 52.00, 52.30,
+52.40, 52.50, 52.60, 52.70, 52.80, 52.9, 53.1, 53.50] ``` When operating in
+strategy mode (timed_mode=2), charge_needed will create a schedule that
+includes the strategy for the tariff with additional time segments added to
+charge from grid and (optionall) to stop the battery discharging. In other
+modes, charge_needed() will disable any schedules and set the battery charge
+times. This example shows the results reported by charge needed: ![image]
+(https://github.com/TonyM1958/FoxESS-Cloud/assets/63789168/8b77956b-c326-43cd-
+b165-20d806b1e7e8) ## Battery Info Provides detailed information on the current
+state of the batteries: ``` f.battery_info(count, plot, log) f.battery_monitor
+(interval, run, log, save, count) ``` battery_info() prints information on the
+battery and cells: + count: optional over-ride. The default is based on
+factorising the number of cells reported by 16 or 18 to work out the number of
+batteries. + plot: 1 plot the cell voltages for each battery, 2 plot the cell
+temperatueres, 0 don't plot. The default is 1 + log: see below. Default is 0
+battery_monitor() runs battery_info() in log mode on a schedule to provide
+information on the battery status over a period of time: + interval: the time
+in minutes between log entries. The default is 30 minutes + run: the number of
+log entries to create. The default is 48 i.e. every 30 minues for 24 hours in
+total + log: 0 = display, 1 = log battery info, 2 = add cell volts, 3 = add
+cell temps. The default is 1 + save: name of a CSV file to write log data to +
+count: optional over-ride for the number of batteries This is an example of the
+output from battery_info(): ![image](https://github.com/TonyM1958/FoxESS-Cloud/
+assets/63789168/a8eb52b6-ce3f-4b58-bb76-5483d5e40fa7) ## Date Ranges ```
+f.date_list(s, e, limit, span, today) ``` Returns a list of dates in the format
+'YYYY-MM-DD'. This function will not return dates in the future. The last date
+will be yesterday or today (if today is True). All parameters are optional: +
+s: start date + e: end date + limit: maximum number of days. The default is 200
++ span: the range of dates. One of 'day', 'week', 'month' or 'year', '2days' or
+'weekday' + today: 1 allows today to be included, 2 allows future dates to be
+included. Default is 0, date list will stop at yesterday You can use 'span' as
+follows: + 'day' provides a single day + 'week' will provide the dates of 7
+consequetive days + 'month' will provide the dates of the days up to the same
+date in the preceeding (or follwing) month + '2days' will provide the dates of
+yesterday and today + 'weekday' will provide the dates of the same day of the
+week, going backwards (or forwards) up to 7 weeks ``` f.british_summer_time(d)
+# 1 if d is in Britsh Summer Time, 0 if not ``` ## Time Periods Times and time
+period settings are held as decimal hours. Functions for working with time
+strings with the format 'HH:MM:SS' and decimal hours include: ``` f.time_hours
+(t, d=None) # convert time to decimal hours. t is a time string ('HH:MM' or
+'HH:MM:SS'), d is optional and is the default time if s is None f.hours_time(h,
+mm=True, ss=False, day=False) # convert decimal hours to time (HH:MM:SS). mm =
+include minutes, ss = include seconds, day = include /n for day when hours > 24
 f.hours_in(h, {'start': a, 'end': b}) # True if decimal hour h is in the time
 period a -> b ``` ## Tariffs Tariffs configure when your battery can be charged
 and provide time of use (TOU) periods to split your grid import and export into
 peak, off-peak and shoulder times when data is uploaded to PV Ouptut. There are
 a number of different pre-configured tariffs: + Octopus Flux: off-peak from 02:
 00 to 05:00, peak from 16:00 to 19:00, forecasts from 22:00 to 23:59. Timed
 work mode change to Self Use at 7am and Feed In First at 4pm. + Intelligent
@@ -400,108 +401,118 @@
 between 12 noon and 4pm with a 1 hour period: + times=[("23:00", "8:00", 3),
 ("12:00", "16:00", 1)] 'strategy' allows you to configure times when work modes
 will be changed. The format is a list of dictionary items, containing: +
 'start', 'end': times in decimal hours or time format. The end time is
 exclusive so setting an end time of '07:00' will set a schedule that ends at
 '06:59' + 'mode': the work mode to be used from 'SelfUse', 'Feedin', 'Backup',
 'ForceCharge', 'ForceDischarge' + 'min_soc, 'fdsoc', 'fdpwr': optional values
-for each work mode. The defaults are 10, 10 and 0 respectively. The strategy
-should not include settings for the AM/PM charge times for the tariff. These
-will be added by charge_needed(). # PV Output These functions produce CSV data
-for upload to [pvoutput.org](https://pvoutput.org) including PV generation,
-Export, Load and Grid consumption by day in Wh. The functions use the energy
-estimates created from the raw power data (see above). The estimates include PV
-energy generation that are not otherwise available from the Fox Cloud.
-Typically, the energy results are within 3% of the values reported by the
-meters built into the inverter. ## Get PV Output Data Returns CSV upload data
-using the [API format](https://pvoutput.org/help/api_specification.html#csv-
-data-parameter): ``` f.get_pvoutput(d, tou) ``` + d is the date or a list of
-dates, to get data for. The default is yesterday + tou: optional, setting tou=1
-uploads data with time of use. The default, tou=0 does not split data and is
-more accurate. You can copy and paste the output data to the pvoutput data CSV
-Loader, using the following settings: ![image](https://github.com/TonyM1958/
-FoxESS-Cloud/assets/63789168/21459cdc-a943-4e9d-a204-7efd45a422d8) For example,
-this Jupyer Lab cell will provide a CSV data upload for June 2023: ```
-f.get_pvoutput(f.date_list('2023-06-01', '2023-06-30')) ``` ## Set PV Output
-Data Loads CSV data directly using the PV Ouput API: ``` f.set_pvoutput(d,
-system_id, tou, push) ``` + d is optional and is the date, or a list of dates,
-to upload + system_id is optional and allow you to select where data is
-uploaded to (where you have more than 1 registered system) + tou: optional,
-setting tou=1 uploads data with time of use. The default, tou=0 does not split
-data and is more accurate + push: optional. 0 = do not sent to pushover, 1 =
-send summary to pushover, 2 = send first day summary only # Solar Forecasting #
-Solcast Get and display solar data from your solcast.com account using your API
-key: ``` f.solcast_api_key = "my.solcast_api_key" fcast = f.Solcast() print
-(fcast) ``` Returns a 7 day forecast. Optional parameters are: + days: number
-of days to get. The default is 7 + estimated: whether to get history /
-estimated data. 1 = yes, 0 = no. Default is 0. + reload: cached data handling.
-0 = use saved data, 1 = fetch new data, 2 = use saved data for today (default)
-+ quiet: True to stop Solcast producing progress messages Forecast data is
-saved to f.solcast_save. The default is 'solcast.txt'. ``` fcast.plot_daily()
+for each work mode. The defaults are 10, 10 and 0 respectively. There are a
+number of pre-defined strategies: + f.flux_strategy_1: switch to self use at
+5am and feed in first at 4pm. + f.flux_strategy_2: as above with force charge
+between 2am and 4am. Move the AM charge period between 4am and 5am when using
+this. + f.flux_strategy_3: as above with force discharge between 4pm and 6pm at
+6kW with fdsoc at 35% ``` f.get_strategy() ``` get_strategy() creates a list of
+time segments from the strategy. If strategy is not provided, it uses the
+strategy for the current tariff. If a strategy includes settings for the AM/PM
+charge times for the tariff, the times will be moved so they do not conflict
+with the charge time used by charge_needed(). # PV Output These functions
+produce CSV data for upload to [pvoutput.org](https://pvoutput.org) including
+PV generation, Export, Load and Grid consumption by day in Wh. The functions
+use the energy estimates created from the raw power data (see above). The
+estimates include PV energy generation that are not otherwise available from
+the Fox Cloud. Typically, the energy results are within 3% of the values
+reported by the meters built into the inverter. ## Get PV Output Data Returns
+CSV upload data using the [API format](https://pvoutput.org/help/
+api_specification.html#csv-data-parameter): ``` f.get_pvoutput(d, tou) ``` + d
+is the date or a list of dates, to get data for. The default is yesterday +
+tou: optional, setting tou=1 uploads data with time of use. The default, tou=0
+does not split data and is more accurate. You can copy and paste the output
+data to the pvoutput data CSV Loader, using the following settings: ![image]
+(https://github.com/TonyM1958/FoxESS-Cloud/assets/63789168/21459cdc-a943-4e9d-
+a204-7efd45a422d8) For example, this Jupyer Lab cell will provide a CSV data
+upload for June 2023: ``` f.get_pvoutput(f.date_list('2023-06-01', '2023-06-
+30')) ``` ## Set PV Output Data Loads CSV data directly using the PV Ouput API:
+``` f.set_pvoutput(d, system_id, tou, push) ``` + d is optional and is the
+date, or a list of dates, to upload + system_id is optional and allow you to
+select where data is uploaded to (where you have more than 1 registered system)
++ tou: optional, setting tou=1 uploads data with time of use. The default,
+tou=0 does not split data and is more accurate + push: optional. 0 = do not
+sent to pushover, 1 = send summary to pushover, 2 = send first day summary only
+# Solar Forecasting # Solcast Get and display solar data from your solcast.com
+account using your API key: ``` f.solcast_api_key = "my.solcast_api_key" fcast
+= f.Solcast() print(fcast) ``` Returns a 7 day forecast. Optional parameters
+are: + days: number of days to get. The default is 7 + estimated: whether to
+get history / estimated data. 1 = yes, 0 = no. Default is 0. + reload: cached
+data handling. 0 = use saved data, 1 = fetch new data, 2 = use saved data for
+today (default) + quiet: True to stop Solcast producing progress messages
+Forecast data is saved to f.solcast_save. The default is 'solcast.txt'. ```
+fcast.plot_daily() fcast.plot_hourly(day) ``` Plots the estimate / forecast
+data. plot_daily() plots the daily yield. plot_hourly() plots each day
+separately. + day: optional. 'today', 'tomorrow', 'all' or a specific list of
+dates. The default is to plot today and tomorrow # Forecast.solar Get and
+display solar data from forecast.solar for today and tomorrow: ```
+f.solar_array('South', lat=51.1789, lon=-1.8262, kwp=6.4) ``` You need to
+configure your solar arrays by calling f.solar_array(). This takes the
+following parameters: + name: the name of each of your arrays + lat: the
+latitude where the array is located. The default is Stonehenge. + lon: the
+longitude where the array is located. The default is Stonehenge. + dec: the
+declination of the array - 0 is lying flat and 90 is vertical. Default is 30 +
+az: azimuth of the array. 0 is pointing due South, -90 is pointing East, 90 is
+pointing West. The default is 0 + kwp: the size of the array in kWp. The
+default is 5kWp + dam: damping factor. Default is None + inv: inverter power
+limit (when the array will clip). The default is None + hor: a list of values
+describing obstructions on the horizon Add one array for each string attached
+to your inverter. If your solar production is limited by clipping, set the
+inverter power so the forecast better matches your generation. See the [API
+documentation](https://doc.forecast.solar/api) for more information on
+parameter values. ``` fcast = f.Solar() print(fcast) ``` Returns a forecast for
+today and tomorrow. Optional parameters are: + reload: cached data handling. 0
+= use saved data, 1 = fetch new data, 2 = use saved data for today (default) +
+quiet: set to True to stop Solar producing progress messages Forecast data is
+saved to f.solar_save. The default is 'solar.txt'. ``` fcast.plot_daily()
 fcast.plot_hourly(day) ``` Plots the estimate / forecast data. plot_daily()
 plots the daily yield. plot_hourly() plots each day separately. + day:
 optional. 'today', 'tomorrow', 'all' or a specific list of dates. The default
-is to plot today and tomorrow # Forecast.solar Get and display solar data from
-forecast.solar for today and tomorrow: ``` f.solar_array('South', lat=51.1789,
-lon=-1.8262, kwp=6.4) ``` You need to configure your solar arrays by calling
-f.solar_array(). This takes the following parameters: + name: the name of each
-of your arrays + lat: the latitude where the array is located. The default is
-Stonehenge. + lon: the longitude where the array is located. The default is
-Stonehenge. + dec: the declination of the array - 0 is lying flat and 90 is
-vertical. Default is 30 + az: azimuth of the array. 0 is pointing due South, -
-90 is pointing East, 90 is pointing West. The default is 0 + kwp: the size of
-the array in kWp. The default is 5kWp + dam: damping factor. Default is None +
-inv: inverter power limit (when the array will clip). The default is None +
-hor: a list of values describing obstructions on the horizon Add one array for
-each string attached to your inverter. If your solar production is limited by
-clipping, set the inverter power so the forecast better matches your
-generation. See the [API documentation](https://doc.forecast.solar/api) for
-more information on parameter values. ``` fcast = f.Solar() print(fcast) ```
-Returns a forecast for today and tomorrow. Optional parameters are: + reload:
-cached data handling. 0 = use saved data, 1 = fetch new data, 2 = use saved
-data for today (default) + quiet: set to True to stop Solar producing progress
-messages Forecast data is saved to f.solar_save. The default is 'solar.txt'.
-``` fcast.plot_daily() fcast.plot_hourly(day) ``` Plots the estimate / forecast
-data. plot_daily() plots the daily yield. plot_hourly() plots each day
-separately. + day: optional. 'today', 'tomorrow', 'all' or a specific list of
-dates. The default is to plot today and tomorrow # Pushover Send messages to a
-pushover user account: ``` f.output_spool(app_key, h) f.output(s)
-f.output_close(plot, file) f.output_message(app_key, message, plot) ``` Calling
-f.output_spool() with an app key will start the system spooling output to send
-to pushover. h is an optional header to add as the first line of the message. H
-may include \
+is to plot today and tomorrow # Pushover Send messages to a pushover user
+account: ``` f.output_spool(app_key, h) f.output(s) f.output_close(plot, file)
+f.output_message(app_key, message, plot) ``` Calling f.output_spool() with an
+app key will start the system spooling output to send to pushover. h is an
+optional header to add as the first line of the message. H may include \
 >, \
 > or \
 > and these will be set to current system time and date respectively. When
 spooling is active, any calls to f.output() add lines to the spooled message.
 If appending to the message would exceed 1024 characters, the existing spooled
 message is sent and a new message spool is started. Calling f.output_close()
 will send the spooled message and optionally attach a binary image file. You
 can set plot=1 to attach the last plot file created (when f.plot_file is set)
 or specify a file. f.output_message() is a shorcut to send a message without
 spooling output. # Troubleshooting If needed, you can add the following setting
 to increase the level of information reported by the foxesscloud module: ```
 f.debug_setting = 2 ``` This setting can be: + 0: silent mode (minimal output)
 + 1: information reporting (default) + 2: more debug information, updating of
 inverter settings is disabled + 3: internal variables and values are displayed
-(verbose) # Version Info 2.2.7
-Updated contingency to allow seasonal values for winter, spring, summer and
-autumn. Update strategy mode to support ForceCharge and ForceDischarge work
-modes. Update so min_soc setting in charge_needed() over-rides min_soc in the
-tariff strategy. Fix force charge strategy mode in charge_neded() to set
-min_soc correctly. Implement 2 second delay between calls that change inverter
-settings. Added strategy mode (timed_mode=2) to charge_needed(). Added
-set_strategy() and charge_strategy() to manage charging schedules and work mode
-changes. Refactor debug messaging. Simplify charge_needed() output. Added
-'target_soc' to charge_needed() settings Fix bat_info() giving incorrect
-temperatures when API returns 0 instead of -50 where there is no battery Fix
-key error when accessing cell volts and temps using an agent / installer
-account. Ensure output is generated if get_battery() fails using battery_info
-(). Update f.avg() to include calculation of averages in lists containng None
-values. Added 'data_wrap' to charge_config. 2.1.9
+(verbose) # Version Info 2.2.8
+** breaking change ** rename 'groups' to 'periods' for consistency between
+foxesscloud and openapi. Updated management of battery reserve and float
+charging in charge_needed(). Added Reserve level to charts in charge_needed().
+Changed bms_power setting to 50W. Updated contingency to allow seasonal values
+for winter, spring, summer and autumn. Update strategy mode to support
+ForceCharge and ForceDischarge work modes. Update so min_soc setting in
+charge_needed() over-rides min_soc in the tariff strategy. Fix force charge
+strategy mode in charge_neded() to set min_soc correctly. Implement 2 second
+delay between calls that change inverter settings. Added strategy mode
+(timed_mode=2) to charge_needed(). Added set_strategy() and charge_strategy()
+to manage charging schedules and work mode changes. Refactor debug messaging.
+Simplify charge_needed() output. Added 'target_soc' to charge_needed() settings
+Fix bat_info() giving incorrect temperatures when API returns 0 instead of -50
+where there is no battery Fix key error when accessing cell volts and temps
+using an agent / installer account. Ensure output is generated if get_battery()
+fails using battery_info(). Update f.avg() to include calculation of averages
+in lists containng None values. Added 'data_wrap' to charge_config. 2.1.9
 Update get_history() to use GMT or BST when plotting instead of mixed time
 zones. Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in
 relation to work mode. Better reporting of reason for http error code. Template
 code for get_named_settings() added - not functional in this version due to
 Open API limitations. Update set_pvoutput() to allow push=2. Fix problem in
 set_pvoutput() sending summary to pushover when tou=1. Improve accuracy of time
```

