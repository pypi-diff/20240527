# Comparing `tmp/openmargin-0.0.4.tar.gz` & `tmp/openmargin-0.0.5.tar.gz`

## Comparing `openmargin-0.0.4.tar` & `openmargin-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 openmargin-0.0.4/arrow-markets.png
--rw-r--r--   0        0        0    36803 2020-02-02 00:00:00.000000 openmargin-0.0.4/options_data.png
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 openmargin-0.0.4/requirements.txt
--rw-r--r--   0        0        0    11457 2020-02-02 00:00:00.000000 openmargin-0.0.4/src/openmargin/auxiliary.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 openmargin-0.0.4/src/openmargin/example.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 openmargin-0.0.4/src/openmargin/init.py
--rw-r--r--   0        0        0    13614 2020-02-02 00:00:00.000000 openmargin-0.0.4/src/openmargin/risk.py
--rw-r--r--   0        0        0    35801 2020-02-02 00:00:00.000000 openmargin-0.0.4/LICENSE
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 openmargin-0.0.4/README.md
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 openmargin-0.0.4/pyproject.toml
--rw-r--r--   0        0        0    45388 2020-02-02 00:00:00.000000 openmargin-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 openmargin-0.0.5/arrow-markets.png
+-rw-r--r--   0        0        0    36803 2020-02-02 00:00:00.000000 openmargin-0.0.5/options_data.png
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 openmargin-0.0.5/requirements.txt
+-rw-r--r--   0        0        0    11457 2020-02-02 00:00:00.000000 openmargin-0.0.5/src/openmargin/auxiliary.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 openmargin-0.0.5/src/openmargin/example.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 openmargin-0.0.5/src/openmargin/init.py
+-rw-r--r--   0        0        0    13609 2020-02-02 00:00:00.000000 openmargin-0.0.5/src/openmargin/risk.py
+-rw-r--r--   0        0        0    35801 2020-02-02 00:00:00.000000 openmargin-0.0.5/LICENSE
+-rw-r--r--   0        0        0     6718 2020-02-02 00:00:00.000000 openmargin-0.0.5/README.md
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 openmargin-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    47770 2020-02-02 00:00:00.000000 openmargin-0.0.5/PKG-INFO
```

### Comparing `openmargin-0.0.4/arrow-markets.png` & `openmargin-0.0.5/arrow-markets.png`

 * *Files identical despite different names*

### Comparing `openmargin-0.0.4/options_data.png` & `openmargin-0.0.5/options_data.png`

 * *Files identical despite different names*

### Comparing `openmargin-0.0.4/src/openmargin/auxiliary.py` & `openmargin-0.0.5/src/openmargin/auxiliary.py`

 * *Files identical despite different names*

### Comparing `openmargin-0.0.4/src/openmargin/example.py` & `openmargin-0.0.5/src/openmargin/example.py`

 * *Files identical despite different names*

### Comparing `openmargin-0.0.4/src/openmargin/risk.py` & `openmargin-0.0.5/src/openmargin/risk.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         self.kwargs = kwargs
 
 class PricePathGenerator:
     def __init__(self, 
                  ticker: str,
                  risk_params: RiskConfig,
                  spot = None,
-                 number_of_paths = 1_000,
+                 number_of_paths = 10_000,
                  historical_prices = None):
 
         self.ticker = ticker
         self.risk_params = risk_params
     
         if spot is None:
             self.spot = get_underlier_price(ticker)
@@ -150,18 +150,19 @@
             elif type(position) == np.int_:
                 continue
             else:
                 self.input_check = False
                 print("Option positions need to be a vector of floats, e.g 1.0")
                 break
         
+        spot = get_underlier_price(ticker)
+
         if self.input_check:
             if self.options_data is None:
                 self.utcnow = datetime.datetime.now(tz=datetime.timezone.utc)
-                spot = get_underlier_price(ticker)
                 (expiration_datetimes, yearly_times_to_expiration, strikes, log_moneynesses, contract_types, spot_prices, yearly_mark_implied_volatilities, mark_prices, prices) = deribit_option_data(ticker, self.utcnow)
                 options_data = pd.DataFrame([spot_prices, expiration_datetimes, yearly_times_to_expiration, strikes, log_moneynesses, contract_types, yearly_mark_implied_volatilities, mark_prices, prices]).T
                 options_data.columns = ['spot', 'expiration','tte','strike', 'log_money', 'kind','mark_iv','mark_price', 'price']
                 options_data = options_data.reset_index(drop=True)
                 options_data['spot'] = spot
                 options_data['log_money'] = np.log(options_data['strike'].astype(float) / spot)
                 self.options_data = options_data
```

### Comparing `openmargin-0.0.4/LICENSE` & `openmargin-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openmargin-0.0.4/README.md` & `openmargin-0.0.5/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,108 +1,116 @@
 <p align="center"><img width=20% src="https://github.com/Arrow-Markets-Research/openmargin/raw/main/arrow-markets.png"></p>
 
 ![Python](https://img.shields.io/badge/python-v3.8+-green.svg)
-![Version](https://img.shields.io/badge/version-0.0.4-red.svg)
+![Version](https://img.shields.io/badge/version-0.0.5-red.svg)
 ![License](https://img.shields.io/badge/license-GNU-blue.svg)
 
 # Open Margin
 
-Arrow Markets open source repository to calculate margin requirements for risky asset portfolios including crypto options portfolios.
+Arrow Markets open source repository to compute margin requirements for risky asset portfolios, including crypto options portfolios.
 
 ## Overview
 
-This repository includes a simplified version of the proprietary Arrow Markets margin calculator. It uses VAR/CVAR methodology to compute the necessary margin required for a portfolio of BTC or ETH options. <br />
-Negative values refer to the cash margin needed for a given portfolio, while positive margin values count as credits. For further details, please refer to the white paper ["Automated Margin Systems in Practice"](https://drive.google.com/file/d/1y_113sCg4kOkU8lRDnyRjCovNpDMLNcM/view?usp=drive_link)
+This repository uses VAR/CVAR methodology to compute the necessary margin required for a portfolio of BTC or ETH options. Negative values refer to the cash margin needed for a given portfolio, while positive margin values count as credits. For further details, please refer to the white paper ["Automated Margin Systems in Practice"](https://drive.google.com/file/d/1y_113sCg4kOkU8lRDnyRjCovNpDMLNcM/view?usp=drive_link).
 
 ## Installation
 
 ```bash
 pip install openmargin
 ```
 
-## Dependencies
-
-```bash
-pip install -r requirements.txt
-```
 ## Usage
 
-Open Margin calculates the risk of an options portfolio through RiskCalc. <br />
-Once a compatible ticker and an options portfolio are provided portfolio margin can be computed with default parameters via: <br />
+Open Margin calculates the risk of an options portfolio through RiskCalc. 
+A compatible ticker and an options portfolio are the minimum inputs needed to generate the corresponding margin values.
 
 ```python
 import datetime
 import pandas as pd
-from openmargin.risk import RiskCalc
 
 ticker = "eth"
 
 expiration = datetime.datetime.strptime('2024-09-27 08:00:00', "%Y-%m-%d %H:%M:%S")
 strike = 7000.0
 kind = "C"
 position = -1
 portfolio = {'expiration': expiration, 'strike': strike, 'kind': kind, 'position': position}
 portfolio = pd.DataFrame([portfolio],columns = ["expiration", "strike", "kind", "position"])
+```
+
+Once the ticker and the options data are ready, margin can be computed with default parameters:
 
+```python
+from openmargin.risk import RiskCalc
 risk_calculator = RiskCalc(ticker, portfolio)
 risk_calculator.get_margin()
-
 ```
 
-RiskCalc has four pillars that can be modified to generate the required margin.
+RiskCalc has four pillars that can be modified to generate the required margin. 
+All of the examples below assume that minimum inputs and corresponding package imports are complete.
 
 ### Options Data
-Open Margin uses the current options data for BTC and ETH from Deribit. <br />
-To provide a different dataset, please provide a pandas dataframe containing options data similar to the one shown below: 
+Open Margin uses the current options data for BTC and ETH from Deribit. To provide a different dataset, please provide a pandas dataframe containing options data similar to the one shown below: 
 
 <p align="left"><img src="https://github.com/Arrow-Markets-Research/openmargin/raw/main/options_data.png"></p>
 
+To download and save the most recent options data:
+
 ```python
+from openmargin.auxiliary import deribit_option_data
+
+utcnow = datetime.datetime.now(tz=datetime.timezone.utc)
+(expiration_datetimes, yearly_times_to_expiration, strikes, log_moneynesses, contract_types, spot_prices, yearly_mark_implied_volatilities, mark_prices, prices) = deribit_option_data(ticker, utcnow)
+options_data = pd.DataFrame([spot_prices, expiration_datetimes, yearly_times_to_expiration, strikes, log_moneynesses, contract_types, yearly_mark_implied_volatilities, mark_prices, prices]).T
+options_data.columns = ['spot', 'expiration','tte','strike', 'log_money', 'kind','mark_iv','mark_price', 'price']
+options_data = options_data.reset_index(drop=True)
+options_data.to_csv(f'options_data.csv', index = False)
+```
+
+Providing the options data as a dataframe to Open Margin substantially reduces margin computation times. 
+To load a cahced option dataset and get the corresponding margin values: 
+
+```python
+options_data = pd.read_csv('options_data.csv', parse_dates=['expiration'])
 risk_calculator = RiskCalc(ticker, portfolio, options_data)
 risk_calculator.get_margin()
 ```
 
 ### Risk Configuration
-Three main risk factors are configured under RiskConfig. <br />
-Interest rate, sampling frequency and steps are the key parameters currently allowed for user customization. <br />
-Sampling frequency multiplied by steps determine the trading horizon that will be used to calculate margin values.
+Three main risk factors are configured under RiskConfig. Interest rate, sampling frequency and steps are the key parameters currently allowed for user customization. Sampling frequency multiplied by steps determine the trading horizon that will be used to calculate margin values.
 
 ```python
 from openmargin.risk import RiskConfig, RiskCalc
 
 r = 0.02
 sampling_frequency = 4 # hours
 steps = 6
 risk_params = RiskConfig(r, sampling_frequency, steps)
 
 risk_calculator = RiskCalc(ticker, portfolio, risk_params = risk_params)
 risk_calculator.get_margin()
 ```
 
 ### Risk Model
-RiskModel class determines the margin method used.
-Open Margin only allows VAR type margin methods in this public version.
-To select between VAR and CVAR and to change margin threshold:
+RiskModel class determines the margin method used. Open Margin only allows VAR type margin methods in this public version. To select between VAR and CVAR and to change margin threshold:
 
 ```python
 from openmargin.risk import VAR, RiskModel, RiskCalc
 
 var_type = 'VAR'
 var_threshold = 0.05
 margin_method = VAR(var_type, var_threshold)
 risk_model = RiskModel(margin_method)
 
 risk_calculator = RiskCalc(ticker, portfolio, risk_model = risk_model)
 risk_calculator.get_margin()
 ```
 
 ### Price Paths
-Path dependant methods like VAR/CVAR depend on future price paths. <br />
-1,000 paths are generated by default by PricePathGenerator. <br />
-Changes to the default number of paths can be made via:
+Path dependant methods like VAR/CVAR depend on future price paths. 1,000 paths are generated by default by PricePathGenerator. Changes to the default number of paths can be made via:
 
 ```python
 from openmargin.auxiliary import get_underlier_price
 from openmargin.risk import PricePathGenerator, RiskCalc
 
 spot = get_underlier_price(ticker)
 number_of_paths = 10_000
@@ -115,7 +123,55 @@
 The paths can be generated with:
 
 ```python
 sample_paths = price_paths.generate_paths()
 ```
 
 Further customization examples can be found under example.py.
+
+## Clone Repo Directly
+The repo can also be cloned directly.  This is advisable for doing work on the openmargin repo itself.  Please see our guidelines for submitting pull requests.  Community contributions are welcome!
+
+```bash
+git clone https://github.com/Arrow-Markets-Research/openmargin
+cd openmargin
+```
+### venv
+
+Initialize a virtual environment (Windows)
+```bash
+python3 -m venv venv
+venv/Scripts/activate.bat
+```
+### Dependencies
+
+From the venv, run
+```bash
+pip install -r requirements.txt
+```
+Create a test file in the `src/openmargin` directory called `om-test.py`:
+
+```python
+import datetime
+import pandas as pd
+from openmargin.risk import RiskCalc
+
+ticker = "eth"
+
+expiration = datetime.datetime.strptime('2024-09-27 08:00:00', "%Y-%m-%d %H:%M:%S")
+strike = 7000.0
+kind = "C"
+position = -1
+portfolio = {'expiration': expiration, 'strike': strike, 'kind': kind, 'position': position}
+portfolio = pd.DataFrame([portfolio],columns = ["expiration", "strike", "kind", "position"])
+
+risk_calculator = RiskCalc(ticker, portfolio)
+m = risk_calculator.get_margin()
+
+print("portfolio:\n", portfolio, "\nspot:", float(risk_calculator.portfolio.spot), "\ninitial margin:", m[0])
+
+```
+Now, to compute the intitial margin for the chosen portfolio, switch to the `src` directory and run
+
+```bash
+python3 -m openmargin.om-test
+```
```

### Comparing `openmargin-0.0.4/pyproject.toml` & `openmargin-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/openmargin"]
 
 [project]
 name = "openmargin"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Arrow Markets Research", email="ata@subharmonic.tech"},
 ]
 description = "Arrow Markets repository for calculation margin requirements for crypto option portfolios."
 readme = "README.md"
 license = {file = 'LICENSE'}
 requires-python = ">=3.8"
```

### Comparing `openmargin-0.0.4/PKG-INFO` & `openmargin-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: openmargin
-Version: 0.0.4
+Version: 0.0.5
 Summary: Arrow Markets repository for calculation margin requirements for crypto option portfolios.
 Project-URL: Homepage, https://github.com/Arrow-Markets-Research/openmargin
 Author-email: Arrow Markets Research <ata@subharmonic.tech>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -689,112 +689,120 @@
 Requires-Dist: requests>=2.31
 Requires-Dist: scipy>=1.10
 Description-Content-Type: text/markdown
 
 <p align="center"><img width=20% src="https://github.com/Arrow-Markets-Research/openmargin/raw/main/arrow-markets.png"></p>
 
 ![Python](https://img.shields.io/badge/python-v3.8+-green.svg)
-![Version](https://img.shields.io/badge/version-0.0.4-red.svg)
+![Version](https://img.shields.io/badge/version-0.0.5-red.svg)
 ![License](https://img.shields.io/badge/license-GNU-blue.svg)
 
 # Open Margin
 
-Arrow Markets open source repository to calculate margin requirements for risky asset portfolios including crypto options portfolios.
+Arrow Markets open source repository to compute margin requirements for risky asset portfolios, including crypto options portfolios.
 
 ## Overview
 
-This repository includes a simplified version of the proprietary Arrow Markets margin calculator. It uses VAR/CVAR methodology to compute the necessary margin required for a portfolio of BTC or ETH options. <br />
-Negative values refer to the cash margin needed for a given portfolio, while positive margin values count as credits. For further details, please refer to the white paper ["Automated Margin Systems in Practice"](https://drive.google.com/file/d/1y_113sCg4kOkU8lRDnyRjCovNpDMLNcM/view?usp=drive_link)
+This repository uses VAR/CVAR methodology to compute the necessary margin required for a portfolio of BTC or ETH options. Negative values refer to the cash margin needed for a given portfolio, while positive margin values count as credits. For further details, please refer to the white paper ["Automated Margin Systems in Practice"](https://drive.google.com/file/d/1y_113sCg4kOkU8lRDnyRjCovNpDMLNcM/view?usp=drive_link).
 
 ## Installation
 
 ```bash
 pip install openmargin
 ```
 
-## Dependencies
-
-```bash
-pip install -r requirements.txt
-```
 ## Usage
 
-Open Margin calculates the risk of an options portfolio through RiskCalc. <br />
-Once a compatible ticker and an options portfolio are provided portfolio margin can be computed with default parameters via: <br />
+Open Margin calculates the risk of an options portfolio through RiskCalc. 
+A compatible ticker and an options portfolio are the minimum inputs needed to generate the corresponding margin values.
 
 ```python
 import datetime
 import pandas as pd
-from openmargin.risk import RiskCalc
 
 ticker = "eth"
 
 expiration = datetime.datetime.strptime('2024-09-27 08:00:00', "%Y-%m-%d %H:%M:%S")
 strike = 7000.0
 kind = "C"
 position = -1
 portfolio = {'expiration': expiration, 'strike': strike, 'kind': kind, 'position': position}
 portfolio = pd.DataFrame([portfolio],columns = ["expiration", "strike", "kind", "position"])
+```
+
+Once the ticker and the options data are ready, margin can be computed with default parameters:
 
+```python
+from openmargin.risk import RiskCalc
 risk_calculator = RiskCalc(ticker, portfolio)
 risk_calculator.get_margin()
-
 ```
 
-RiskCalc has four pillars that can be modified to generate the required margin.
+RiskCalc has four pillars that can be modified to generate the required margin. 
+All of the examples below assume that minimum inputs and corresponding package imports are complete.
 
 ### Options Data
-Open Margin uses the current options data for BTC and ETH from Deribit. <br />
-To provide a different dataset, please provide a pandas dataframe containing options data similar to the one shown below: 
+Open Margin uses the current options data for BTC and ETH from Deribit. To provide a different dataset, please provide a pandas dataframe containing options data similar to the one shown below: 
 
 <p align="left"><img src="https://github.com/Arrow-Markets-Research/openmargin/raw/main/options_data.png"></p>
 
+To download and save the most recent options data:
+
 ```python
+from openmargin.auxiliary import deribit_option_data
+
+utcnow = datetime.datetime.now(tz=datetime.timezone.utc)
+(expiration_datetimes, yearly_times_to_expiration, strikes, log_moneynesses, contract_types, spot_prices, yearly_mark_implied_volatilities, mark_prices, prices) = deribit_option_data(ticker, utcnow)
+options_data = pd.DataFrame([spot_prices, expiration_datetimes, yearly_times_to_expiration, strikes, log_moneynesses, contract_types, yearly_mark_implied_volatilities, mark_prices, prices]).T
+options_data.columns = ['spot', 'expiration','tte','strike', 'log_money', 'kind','mark_iv','mark_price', 'price']
+options_data = options_data.reset_index(drop=True)
+options_data.to_csv(f'options_data.csv', index = False)
+```
+
+Providing the options data as a dataframe to Open Margin substantially reduces margin computation times. 
+To load a cahced option dataset and get the corresponding margin values: 
+
+```python
+options_data = pd.read_csv('options_data.csv', parse_dates=['expiration'])
 risk_calculator = RiskCalc(ticker, portfolio, options_data)
 risk_calculator.get_margin()
 ```
 
 ### Risk Configuration
-Three main risk factors are configured under RiskConfig. <br />
-Interest rate, sampling frequency and steps are the key parameters currently allowed for user customization. <br />
-Sampling frequency multiplied by steps determine the trading horizon that will be used to calculate margin values.
+Three main risk factors are configured under RiskConfig. Interest rate, sampling frequency and steps are the key parameters currently allowed for user customization. Sampling frequency multiplied by steps determine the trading horizon that will be used to calculate margin values.
 
 ```python
 from openmargin.risk import RiskConfig, RiskCalc
 
 r = 0.02
 sampling_frequency = 4 # hours
 steps = 6
 risk_params = RiskConfig(r, sampling_frequency, steps)
 
 risk_calculator = RiskCalc(ticker, portfolio, risk_params = risk_params)
 risk_calculator.get_margin()
 ```
 
 ### Risk Model
-RiskModel class determines the margin method used.
-Open Margin only allows VAR type margin methods in this public version.
-To select between VAR and CVAR and to change margin threshold:
+RiskModel class determines the margin method used. Open Margin only allows VAR type margin methods in this public version. To select between VAR and CVAR and to change margin threshold:
 
 ```python
 from openmargin.risk import VAR, RiskModel, RiskCalc
 
 var_type = 'VAR'
 var_threshold = 0.05
 margin_method = VAR(var_type, var_threshold)
 risk_model = RiskModel(margin_method)
 
 risk_calculator = RiskCalc(ticker, portfolio, risk_model = risk_model)
 risk_calculator.get_margin()
 ```
 
 ### Price Paths
-Path dependant methods like VAR/CVAR depend on future price paths. <br />
-1,000 paths are generated by default by PricePathGenerator. <br />
-Changes to the default number of paths can be made via:
+Path dependant methods like VAR/CVAR depend on future price paths. 1,000 paths are generated by default by PricePathGenerator. Changes to the default number of paths can be made via:
 
 ```python
 from openmargin.auxiliary import get_underlier_price
 from openmargin.risk import PricePathGenerator, RiskCalc
 
 spot = get_underlier_price(ticker)
 number_of_paths = 10_000
@@ -807,7 +815,55 @@
 The paths can be generated with:
 
 ```python
 sample_paths = price_paths.generate_paths()
 ```
 
 Further customization examples can be found under example.py.
+
+## Clone Repo Directly
+The repo can also be cloned directly.  This is advisable for doing work on the openmargin repo itself.  Please see our guidelines for submitting pull requests.  Community contributions are welcome!
+
+```bash
+git clone https://github.com/Arrow-Markets-Research/openmargin
+cd openmargin
+```
+### venv
+
+Initialize a virtual environment (Windows)
+```bash
+python3 -m venv venv
+venv/Scripts/activate.bat
+```
+### Dependencies
+
+From the venv, run
+```bash
+pip install -r requirements.txt
+```
+Create a test file in the `src/openmargin` directory called `om-test.py`:
+
+```python
+import datetime
+import pandas as pd
+from openmargin.risk import RiskCalc
+
+ticker = "eth"
+
+expiration = datetime.datetime.strptime('2024-09-27 08:00:00', "%Y-%m-%d %H:%M:%S")
+strike = 7000.0
+kind = "C"
+position = -1
+portfolio = {'expiration': expiration, 'strike': strike, 'kind': kind, 'position': position}
+portfolio = pd.DataFrame([portfolio],columns = ["expiration", "strike", "kind", "position"])
+
+risk_calculator = RiskCalc(ticker, portfolio)
+m = risk_calculator.get_margin()
+
+print("portfolio:\n", portfolio, "\nspot:", float(risk_calculator.portfolio.spot), "\ninitial margin:", m[0])
+
+```
+Now, to compute the intitial margin for the chosen portfolio, switch to the `src` directory and run
+
+```bash
+python3 -m openmargin.om-test
+```
```

