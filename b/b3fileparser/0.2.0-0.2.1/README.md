# Comparing `tmp/b3fileparser-0.2.0.tar.gz` & `tmp/b3fileparser-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b3fileparser-0.2.0.tar", max compression
+gzip compressed data, was "b3fileparser-0.2.1.tar", max compression
```

## Comparing `b3fileparser-0.2.0.tar` & `b3fileparser-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2024-05-20 13:09:26.899061 b3fileparser-0.2.0/LICENSE
--rw-r--r--   0        0        0    12057 2024-05-25 21:17:54.094849 b3fileparser-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-05-20 13:09:26.899061 b3fileparser-0.2.0/b3fileparser/__init__.py
--rw-r--r--   0        0        0     3982 2024-05-25 18:00:30.634980 b3fileparser-0.2.0/b3fileparser/b3_meta_data.py
--rw-r--r--   0        0        0     1029 2024-05-25 21:04:41.830745 b3fileparser-0.2.0/b3fileparser/b3parser.py
--rw-r--r--   0        0        0     2827 2024-05-25 17:23:05.674178 b3fileparser-0.2.0/b3fileparser/b3parser_base.py
--rw-r--r--   0        0        0     2340 2024-05-25 17:48:53.632977 b3fileparser-0.2.0/b3fileparser/b3parser_pandas.py
--rw-r--r--   0        0        0     1712 2024-05-25 20:34:47.385480 b3fileparser-0.2.0/b3fileparser/b3parser_polars.py
--rw-r--r--   0        0        0      442 2024-05-25 21:24:17.657166 b3fileparser-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    12654 1970-01-01 00:00:00.000000 b3fileparser-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-20 13:09:26.899061 b3fileparser-0.2.1/LICENSE
+-rw-r--r--   0        0        0    12057 2024-05-27 17:17:53.836784 b3fileparser-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 13:09:26.899061 b3fileparser-0.2.1/b3fileparser/__init__.py
+-rw-r--r--   0        0        0     3687 2024-05-27 17:17:53.836784 b3fileparser-0.2.1/b3fileparser/b3_meta_data.py
+-rw-r--r--   0        0        0     1029 2024-05-27 17:17:53.836784 b3fileparser-0.2.1/b3fileparser/b3parser.py
+-rw-r--r--   0        0        0     2251 2024-05-27 17:17:53.836784 b3fileparser-0.2.1/b3fileparser/b3parser_base.py
+-rw-r--r--   0        0        0     2165 2024-05-27 17:17:53.836784 b3fileparser-0.2.1/b3fileparser/b3parser_pandas.py
+-rw-r--r--   0        0        0     3313 2024-05-27 17:17:53.836784 b3fileparser-0.2.1/b3fileparser/b3parser_polars.py
+-rw-r--r--   0        0        0      442 2024-05-27 17:17:53.836784 b3fileparser-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    12654 1970-01-01 00:00:00.000000 b3fileparser-0.2.1/PKG-INFO
```

### Comparing `b3fileparser-0.2.0/LICENSE` & `b3fileparser-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `b3fileparser-0.2.0/README.md` & `b3fileparser-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `b3fileparser-0.2.0/b3fileparser/b3_meta_data.py` & `b3fileparser-0.2.1/b3fileparser/b3_meta_data.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,79 @@
-META_DATA = {    
-    "TIPREG":{'name':"TIPO_DE_REGISTRO", 'size':2, 'dtype':'object'},
-    "DATAPR":{'name':"DATA_DO_PREGAO", 'size':8, 'dtype': 'object'},
-    "CODBDI":{'name':"CODIGO_BDI", 'size':2, 'dtype':'category'},
-    "CODNEG":{'name':"CODIGO_DE_NEGOCIACAO",'size':12,'dtype':'category'},
-    "TPMERC":{'name':"TIPO_DE_MERCADO",'size':3, 'dtype':'category'},
-    "NOMRES":{'name':"NOME_DA_EMPRESA",'size':12, 'dtype':'category'},
-    "ESPECI":{'name':"ESPECIFICACAO_DO_PAPEL",'size':10, 'dtype':'category'},
-    "PRAZOT":{'name':"PRAZO_EM_DIAS_DO_MERCADO_A_TERMO",'size':3, 'dtype':'object'},
-    "MODREF":{'name':"MOEDA_DE_REFERENCIA",'size':4, 'dtype':'category'},
-    "PREABE":{'name':"PRECO_DE_ABERTURA",'size':13, 'dtype': 'float32'},
-    "PREMAX":{'name':"PRECO_MAXIMO",'size':13, 'dtype': 'float32'},
-    "PREMIN":{'name':"PRECO_MINIMO",'size':13, 'dtype': 'float32'},
-    "PREMED":{'name':"PRECO_MEDIO",'size':13, 'dtype': 'float32'},
-    "PREULT":{'name':"PRECO_ULTIMO_NEGOCIO",'size':13, 'dtype': 'float32'},
-    "PREOFC":{'name':"PRECO_MELHOR_OFERTA_DE_COMPRA",'size':13, 'dtype': 'float32'},
-    "PREOFV":{'name':"PRECO_MELHOR_OFERTA_DE_VENDAS",'size':13, 'dtype': 'float32'},
-    "TOTNEG":{'name':"NUMERO_DE_NEGOCIOS",'size':5, 'dtype':'object'},
-    "QUATOT":{'name':"QUANTIDADE_NEGOCIADA",'size':18, 'dtype':'object'},
-    "VOLTOT":{'name':"VOLUME_TOTAL_NEGOCIADO",'size':18, 'dtype': 'float64'},
-    "PREEXE":{'name':"PRECO_DE_EXERCICIO",'size':13, 'dtype': 'float32'},
-    "INDOPC":{'name':"INDICADOR_DE_CORRECAO_DE_PRECOS",'size':1, 'dtype':'category'},
-    "DATVEN":{'name':"DATA_DE_VENCIMENTO",'size':8, 'dtype':'object'},
-    "FATCOT":{'name':"FATOR_DE_COTACAO",'size':7, 'dtype':'category'},
-    "PTOEXE":{'name':"PRECO_DE_EXERCICIO_EM_PONTOS",'size':13, 'dtype': 'float32'},
-    "CODISI":{'name':"CODIGO_ISIN",'size':12, 'dtype':'category'},
-    "DISMES":{'name':"NUMERO_DE_DISTRIBUICAO",'size':3, 'dtype':'category'}
+FIELD_SIZES = {
+    'TIPO_DE_REGISTRO': 2,
+    'DATA_DO_PREGAO': 8,
+    'CODIGO_BDI': 2,
+    'CODIGO_DE_NEGOCIACAO': 12,
+    'TIPO_DE_MERCADO': 3,
+    'NOME_DA_EMPRESA': 12,
+    'ESPECIFICACAO_DO_PAPEL': 10,
+    'PRAZO_EM_DIAS_DO_MERCADO_A_TERMO': 3,
+    'MOEDA_DE_REFERENCIA': 4,
+    'PRECO_DE_ABERTURA': 13,
+    'PRECO_MAXIMO': 13,
+    'PRECO_MINIMO': 13,
+    'PRECO_MEDIO': 13,
+    'PRECO_ULTIMO_NEGOCIO': 13,
+    'PRECO_MELHOR_OFERTA_DE_COMPRA': 13,
+    'PRECO_MELHOR_OFERTA_DE_VENDAS': 13,
+    'NUMERO_DE_NEGOCIOS': 5,
+    'QUANTIDADE_NEGOCIADA': 18,
+    'VOLUME_TOTAL_NEGOCIADO': 18,
+    'PRECO_DE_EXERCICIO': 13,
+    'INDICADOR_DE_CORRECAO_DE_PRECOS': 1,
+    'DATA_DE_VENCIMENTO': 8,
+    'FATOR_DE_COTACAO': 7,
+    'PRECO_DE_EXERCICIO_EM_PONTOS': 13,
+    'CODIGO_ISIN': 12,
+    'NUMERO_DE_DISTRIBUICAO': 3
 }
 
+DATE_COLUMNS = (
+    "DATA_DO_PREGAO",
+    "DATA_DE_VENCIMENTO"
+)
+
+FLOAT32_COLUMNS = (
+    'PRECO_DE_ABERTURA',
+    'PRECO_MAXIMO',
+    'PRECO_MINIMO',
+    'PRECO_MEDIO',
+    'PRECO_ULTIMO_NEGOCIO',
+    'PRECO_MELHOR_OFERTA_DE_COMPRA',
+    'PRECO_MELHOR_OFERTA_DE_VENDAS',
+    'PRECO_DE_EXERCICIO',
+    'PRECO_DE_EXERCICIO_EM_PONTOS',    
+)
+
+FLOAT64_COLUMNS = (
+    "VOLUME_TOTAL_NEGOCIADO",
+    "QUANTIDADE_NEGOCIADA"
+)
+
+UINT32_COLUMNS = (
+    "FATOR_DE_COTACAO",
+    "PRAZO_EM_DIAS_DO_MERCADO_A_TERMO",
+    "NUMERO_DE_NEGOCIOS",
+    "NUMERO_DE_DISTRIBUICAO",
+    'TIPO_DE_REGISTRO', 
+)
+
+STRING_COLUMNS = (
+    "CODIGO_DE_NEGOCIACAO",
+    "NOME_DA_EMPRESA",
+    "CODIGO_ISIN"
+)
+
+CATEGORY_COLUMNS = (
+    "INDICADOR_DE_CORRECAO_DE_PRECOS", 
+    'TIPO_DE_MERCADO', 
+    'CODIGO_BDI', 
+    "MOEDA_DE_REFERENCIA",
+    "ESPECIFICACAO_DO_PAPEL"
+)
 
 MARKETS = {
     '010':'VISTA',
     '012':'EXERCICIO_DE_OPCOES_DE_COMPRA',
     '013':'EXERCÍCIO_DE_OPCOES_DE_VENDA',
     '017':'LEILAO',
     '020':'FRACIONARIO',
```

### Comparing `b3fileparser-0.2.0/b3fileparser/b3parser.py` & `b3fileparser-0.2.1/b3fileparser/b3parser.py`

 * *Files identical despite different names*

### Comparing `b3fileparser-0.2.0/b3fileparser/b3parser_base.py` & `b3fileparser-0.2.1/b3fileparser/b3parser_pandas.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,14 @@
-from abc import abstractmethod, ABC
-from zipfile import ZipFile
-from io import BytesIO
-from typing import Dict
-import os
+from b3fileparser.b3parser_base import B3ParserBase
 import pandas as pd
-import polars as pl
+import b3fileparser.b3_meta_data as meta_data
 
-from b3fileparser import b3_meta_data
 
-
-class B3ParserBase(ABC):
-    def __init__(self) -> None:
-        super().__init__()
-        
-    
-    @abstractmethod
-    def read_b3_file(file_path: str, file_type: str) -> pd.DataFrame | pl.DataFrame: 
+class B3ParserPandas(B3ParserBase):
+    def read_b3_file(self, file_path, file_type='path') -> pd.DataFrame:
         """
         Reads financial data from a Brazilian B3 file, supporting both plaintext and zipped formats.
 
         Parameters:
             file_path (str): Path or bytes of the file to be read.
             file_type (str): 'path' if `file_path` is a filesystem path, 'bytes' if `file_path` is bytes data.
 
@@ -35,47 +24,29 @@
 
             # Read data from a ZIP file containing a TXT file
             df = read_b3_file('/path/to/file.ZIP')
 
             # Read data from bytes
             df = read_b3_file(b'raw binary data from file', file_type='bytes')
         """
-    @staticmethod    
-    def _load_file(file_path: str, file_type: str) -> BytesIO:
-        # Validate the file type parameter
-        if file_type not in ['path', 'bytes']:
-            raise ValueError("Invalid file_type specified. Choose 'path' or 'bytes'.")
+        file = super()._load_file(file_path, file_type)        
+
+        # Read and parse the file
+        df = pd.read_fwf(
+            file,
+            header=None,
+            names=list(meta_data.FIELD_SIZES.keys()),
+            widths=list(meta_data.FIELD_SIZES.values()),
+            encoding='latin1',
+        )[1:-1]  # Skip potential header and footer rows
         
-        # Handle file input based on type
-        if file_type == 'path':
-            if not file_path.lower().endswith(('.txt', '.zip')):
-                raise ValueError('Invalid file format! Provide a .TXT or .ZIP file containing a .TXT')
-            
-            if file_path.lower().endswith('.zip'):
-                with ZipFile(file_path, 'r') as file_zip:
-                    # Assuming the TXT file has the same base name as the ZIP file
-                    txt_filename = os.path.basename(file_path).replace('.ZIP', '.TXT')
-                    file = BytesIO(file_zip.read(txt_filename))
-            else:
-                file = file_path
-
-        elif file_type == 'bytes':
-            file = BytesIO(file_path)
-        return file
-    
-    @staticmethod    
-    def _load_meta_data() -> Dict:    
-        names, sizes,   = [], []
-        dtypes = {}
-        for v in b3_meta_data.META_DATA.values():
-            names.append(v["name"])
-            sizes.append(v["size"])
-            dtypes.update({v["name"]:v["dtype"]})
-
-        return {
-            "names": names,
-            "sizes": sizes,
-            "dtypes": dtypes,
-            "MARKETS": b3_meta_data.MARKETS,
-            "INDOPC": b3_meta_data.INDOPC,
-            "CODBDI": b3_meta_data.CODBDI,
-        }
+        df["TIPO_DE_MERCADO"] = df["TIPO_DE_MERCADO"].apply(lambda x: meta_data.MARKETS.get(x, x))
+        df["INDICADOR_DE_CORRECAO_DE_PRECOS"] = df["INDICADOR_DE_CORRECAO_DE_PRECOS"].apply(lambda x: meta_data.INDOPC.get(x, x))
+        df["CODIGO_BDI"] = df["CODIGO_BDI"].apply(lambda x: meta_data.CODBDI.get(x, x))
+        for col in meta_data.FLOAT32_COLUMNS: df[col] = df[col].astype(float) / 100
+        for col in meta_data.FLOAT64_COLUMNS: df[col] = df[col].astype(float)
+        for col in meta_data.DATE_COLUMNS:            
+                df[col] = df[col].apply(lambda x: pd.NaT if x == "99991231" else x )
+                df[col] = pd.to_datetime(df[col])
+
+        return df
+
```

### Comparing `b3fileparser-0.2.0/PKG-INFO` & `b3fileparser-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: b3fileparser
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python parser of Brazilian exchange B3 historical data files
 License: MIT
 Author: codigoquant
 Author-email: codigoquant@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

