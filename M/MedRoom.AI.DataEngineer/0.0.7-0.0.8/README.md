# Comparing `tmp/medroom_ai_dataengineer-0.0.7.tar.gz` & `tmp/medroom_ai_dataengineer-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medroom_ai_dataengineer-0.0.7.tar", last modified: Wed May 22 16:01:45 2024, max compression
+gzip compressed data, was "medroom_ai_dataengineer-0.0.8.tar", last modified: Mon May 27 18:09:02 2024, max compression
```

## Comparing `medroom_ai_dataengineer-0.0.7.tar` & `medroom_ai_dataengineer-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 16:01:45.244986 medroom_ai_dataengineer-0.0.7/
--rw-rw-rw-   0        0        0    11558 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.7/LICENSE
-drwxrwxrwx   0        0        0        0 2024-05-22 16:01:45.243030 medroom_ai_dataengineer-0.0.7/MedRoom.AI.DataEngineer.egg-info/
--rw-rw-rw-   0        0        0    13823 2024-05-22 16:01:45.000000 medroom_ai_dataengineer-0.0.7/MedRoom.AI.DataEngineer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      578 2024-05-22 16:01:45.000000 medroom_ai_dataengineer-0.0.7/MedRoom.AI.DataEngineer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      115 2024-05-22 16:01:45.000000 medroom_ai_dataengineer-0.0.7/MedRoom.AI.DataEngineer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-12 17:49:13.000000 medroom_ai_dataengineer-0.0.7/MedRoom.AI.DataEngineer.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      151 2024-05-22 16:01:45.000000 medroom_ai_dataengineer-0.0.7/MedRoom.AI.DataEngineer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-22 16:01:45.000000 medroom_ai_dataengineer-0.0.7/MedRoom.AI.DataEngineer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13823 2024-05-22 16:01:45.244024 medroom_ai_dataengineer-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     8428 2024-05-15 18:52:35.000000 medroom_ai_dataengineer-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 16:01:45.198265 medroom_ai_dataengineer-0.0.7/medroom/
-drwxrwxrwx   0        0        0        0 2024-05-22 16:01:45.198265 medroom_ai_dataengineer-0.0.7/medroom/dna/
-drwxrwxrwx   0        0        0        0 2024-05-22 16:01:45.238899 medroom_ai_dataengineer-0.0.7/medroom/dna/processors/
--rw-rw-rw-   0        0        0        0 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.7/medroom/dna/processors/__init__.py
--rw-rw-rw-   0        0        0      663 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.7/medroom/dna/processors/config.py
--rw-rw-rw-   0        0        0      606 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.7/medroom/dna/processors/main.py
-drwxrwxrwx   0        0        0        0 2024-05-22 16:01:45.241947 medroom_ai_dataengineer-0.0.7/medroom/dna/processors/utils/
--rw-rw-rw-   0        0        0        0 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.7/medroom/dna/processors/utils/__init__.py
--rw-rw-rw-   0        0        0     4385 2024-04-12 20:49:37.000000 medroom_ai_dataengineer-0.0.7/medroom/dna/processors/utils/evalmetrics.py
--rw-rw-rw-   0        0        0     4949 2024-04-20 21:31:01.000000 medroom_ai_dataengineer-0.0.7/medroom/dna/processors/utils/mlflow_helper.py
--rw-rw-rw-   0        0        0     2908 2024-04-12 22:02:34.000000 medroom_ai_dataengineer-0.0.7/medroom/dna/processors/utils/textclean.py
--rw-rw-rw-   0        0        0       42 2024-05-22 16:01:45.244986 medroom_ai_dataengineer-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1390 2024-05-22 15:59:39.000000 medroom_ai_dataengineer-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:09:02.237816 medroom_ai_dataengineer-0.0.8/
+-rw-rw-rw-   0        0        0    11558 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.8/LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-27 18:09:02.235760 medroom_ai_dataengineer-0.0.8/MedRoom.AI.DataEngineer.egg-info/
+-rw-rw-rw-   0        0        0    13823 2024-05-27 18:09:02.000000 medroom_ai_dataengineer-0.0.8/MedRoom.AI.DataEngineer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      578 2024-05-27 18:09:02.000000 medroom_ai_dataengineer-0.0.8/MedRoom.AI.DataEngineer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      115 2024-05-27 18:09:02.000000 medroom_ai_dataengineer-0.0.8/MedRoom.AI.DataEngineer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-12 17:49:13.000000 medroom_ai_dataengineer-0.0.8/MedRoom.AI.DataEngineer.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      151 2024-05-27 18:09:02.000000 medroom_ai_dataengineer-0.0.8/MedRoom.AI.DataEngineer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-27 18:09:02.000000 medroom_ai_dataengineer-0.0.8/MedRoom.AI.DataEngineer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13823 2024-05-27 18:09:02.236772 medroom_ai_dataengineer-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     8575 2024-05-27 17:56:40.000000 medroom_ai_dataengineer-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 18:09:02.191875 medroom_ai_dataengineer-0.0.8/medroom/
+drwxrwxrwx   0        0        0        0 2024-05-27 18:09:02.191875 medroom_ai_dataengineer-0.0.8/medroom/dna/
+drwxrwxrwx   0        0        0        0 2024-05-27 18:09:02.231059 medroom_ai_dataengineer-0.0.8/medroom/dna/processors/
+-rw-rw-rw-   0        0        0        0 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.8/medroom/dna/processors/__init__.py
+-rw-rw-rw-   0        0        0      663 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.8/medroom/dna/processors/config.py
+-rw-rw-rw-   0        0        0      606 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.8/medroom/dna/processors/main.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:09:02.235013 medroom_ai_dataengineer-0.0.8/medroom/dna/processors/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.8/medroom/dna/processors/utils/__init__.py
+-rw-rw-rw-   0        0        0     4658 2024-05-27 18:07:11.000000 medroom_ai_dataengineer-0.0.8/medroom/dna/processors/utils/evalmetrics.py
+-rw-rw-rw-   0        0        0     4949 2024-04-20 21:31:01.000000 medroom_ai_dataengineer-0.0.8/medroom/dna/processors/utils/mlflow_helper.py
+-rw-rw-rw-   0        0        0     2908 2024-04-12 22:02:34.000000 medroom_ai_dataengineer-0.0.8/medroom/dna/processors/utils/textclean.py
+-rw-rw-rw-   0        0        0       42 2024-05-27 18:09:02.237939 medroom_ai_dataengineer-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1448 2024-05-27 17:56:40.000000 medroom_ai_dataengineer-0.0.8/setup.py
```

### Comparing `medroom_ai_dataengineer-0.0.7/LICENSE` & `medroom_ai_dataengineer-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.7/MedRoom.AI.DataEngineer.egg-info/PKG-INFO` & `medroom_ai_dataengineer-0.0.8/MedRoom.AI.DataEngineer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MedRoom.AI.DataEngineer
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Natural Language Processing Data Engineer
 Home-page: https://github.com/MedRoomGitHub/MedRoom.AI.DataEngineer
 Author: Team IA
 Author-email: medroom@medroom.com.br
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `medroom_ai_dataengineer-0.0.7/MedRoom.AI.DataEngineer.egg-info/SOURCES.txt` & `medroom_ai_dataengineer-0.0.8/MedRoom.AI.DataEngineer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.7/PKG-INFO` & `medroom_ai_dataengineer-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MedRoom.AI.DataEngineer
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Natural Language Processing Data Engineer
 Home-page: https://github.com/MedRoomGitHub/MedRoom.AI.DataEngineer
 Author: Team IA
 Author-email: medroom@medroom.com.br
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `medroom_ai_dataengineer-0.0.7/README.md` & `medroom_ai_dataengineer-0.0.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 # MedRoom.AI.DataEngineer
 
 O `MedRoom.AI.DataEngineer` é um pacote que encapsula funções comuns e genéricas, proporcionando uma solução padronizada para o pré-processamento de texto, avaliação de modelos de Machine Learning e interação com MLFlow.
 
 ## :arrow_down: Instalação
 
-#### Instalar o Pacote
+#### Instalar o Pacote (Sem matplotlib e seaborn)
 ```bash
-!pip install MedRoom.AI.DataEngineer==0.0.5
+!pip install MedRoom.AI.DataEngineer==0.0.7
+```
+#### Instalar o Pacote (Com matplotlib e seaborn)
+```bash
+!pip install MedRoom.AI.DataEngineer[plotting]==0.0.7
 ```
 
 ## :book: Uso 
 
 ## :one: Pré-processamento de Texto 
 
 #### Importar Bibliotecas Necessárias
@@ -204,9 +208,9 @@
    twine upload dist/*
    ```
    Nota: Para fazer o upload no PyPI, é necessário fornecer um nome de usuário e senha. Se você tiver a autenticação de dois fatores (2FA) ativada para sua conta no PyPI, precisará usar um Token de API em vez de sua senha habitual. Para mais detalhes sobre as credenciais e outras informações relacionadas, consulte nossa [documentação no Notion](https://www.notion.so/MedRoom-AI-DataEngineer-5d3ea0613d0b411795496fbc8319fa09).
 
 ### 4. **Instalação a partir do PyPI**:
    Depois de publicar seu pacote no PyPI, ele pode ser instalado em qualquer ambiente usando:
    ```bash
-   !pip install MedRoom.AI.DataEngineer====0.0.5
+   !pip install MedRoom.AI.DataEngineer====0.0.7
    ```
```

### Comparing `medroom_ai_dataengineer-0.0.7/medroom/dna/processors/config.py` & `medroom_ai_dataengineer-0.0.8/medroom/dna/processors/config.py`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.7/medroom/dna/processors/main.py` & `medroom_ai_dataengineer-0.0.8/medroom/dna/processors/main.py`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.7/medroom/dna/processors/utils/evalmetrics.py` & `medroom_ai_dataengineer-0.0.8/medroom/dna/processors/utils/evalmetrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,21 @@
+from io import BytesIO  # Importa utilitário para manipulação de streams de bytes
+
 import matplotlib.pyplot as plt  # Importa a biblioteca para criação de gráficos
-import numpy as np               # Importa a biblioteca NumPy para operações numéricas
-import pandas as pd              # Importa a biblioteca Pandas para manipulação de dados
-import seaborn as sns            # Importa a biblioteca Seaborn para gráficos estatísticos
-from sklearn.metrics import accuracy_score, classification_report, confusion_matrix, roc_auc_score  # Importa métricas de avaliação de modelos
+import numpy as np  # Importa a biblioteca NumPy para operações numéricas
+import pandas as pd  # Importa a biblioteca Pandas para manipulação de dados
+import seaborn as sns  # Importa a biblioteca Seaborn para gráficos estatísticos
+from sklearn.metrics import (  # Importa métricas de avaliação de modelos
+    accuracy_score,
+    classification_report,
+    confusion_matrix,
+    roc_auc_score,
+)
 from sklearn.preprocessing import LabelBinarizer  # Importa utilitário para binarização de labels
-from io import BytesIO  # Importa utilitário para manipulação de streams de bytes
+
 
 class ModelEvaluator:
     @staticmethod
     def accuracy(y_true, y_pred):
         """Calcula e imprime a acurácia do modelo."""
         if len(y_true) == 0 or len(y_pred) == 0:
             raise ValueError("y_true e y_pred não devem estar vazios.")  # Valida se os inputs não estão vazios
@@ -19,44 +26,60 @@
     @staticmethod
     def flatten_classification_report(report, prefix="", suffix=""):
         """Achata o relatório de classificação em um dicionário único com prefixos e sufixos opcionais."""
         flat_report = {}  # Inicializa o dicionário achatado
         for key, value in report.items():  # Itera sobre os itens do relatório
             if isinstance(value, dict):  # Checa se o valor é um dicionário
                 for metric, metric_value in value.items():
-                    flat_report[f"{prefix} {key} {metric} {suffix}".strip()] = metric_value  # Adiciona métricas com prefixos/sufixos
+                    flat_report[f"{prefix} {key} {metric} {suffix}".strip()] = (
+                        metric_value  # Adiciona métricas com prefixos/sufixos
+                    )
             else:
                 flat_report[f"{prefix} {key} {suffix}".strip()] = value
         return flat_report
 
     @staticmethod
-    def _generate_heatmap(data, title, cmap="Greens"):
+    def _generate_heatmap(data, title, cmap="Greens", square=False, fmt="0.2f"):
         """Função auxiliar para gerar um heatmap a partir dos dados."""
         fig, ax = plt.subplots()  # Cria a figura e o eixo
-        sns.heatmap(data, cmap=cmap, linewidths=0.5, annot=True, fmt=".0%", cbar=False, square=True, ax=ax)  # Desenha o heatmap
+        sns.heatmap(
+            data, cmap=cmap, linewidths=0.5, annot=True, fmt=fmt, cbar=False, square=square, ax=ax
+        )  # Desenha o heatmap
         ax.set_title(title)  # Define o título do gráfico
         img = BytesIO()  # Cria um buffer para a imagem
-        plt.savefig(img, format='png', bbox_inches='tight')  # Salva a imagem no buffer
+        plt.savefig(img, format="png", bbox_inches="tight")  # Salva a imagem no buffer
         plt.close(fig)  # Fecha a figura para liberar memória
         img.seek(0)  # Reposiciona o cursor do buffer para o início
         return img
 
     @staticmethod
     def classification_report_img_generator(y_true, y_pred):
         report = classification_report(y_true, y_pred, output_dict=True)  # Gera relatório de classificação
         report_df = pd.DataFrame(report).transpose().drop(columns=["support"])  # Transforma o relatório em DataFrame
-        return ModelEvaluator._generate_heatmap(report_df, "Classification Report"), report  # Retorna o heatmap e o relatório
+        return (
+            ModelEvaluator._generate_heatmap(report_df, "Classification Report"),
+            report,
+        )  # Retorna o heatmap e o relatório
 
     @staticmethod
     def confusion_matrix_img_generator(y_true, y_pred):
         cnf_matrix = confusion_matrix(y_true, y_pred)  # Gera a matriz de confusão
-        report_df = pd.DataFrame(classification_report(y_true, y_pred, output_dict=True)).transpose()  # Gera DataFrame do relatório
-        cnf_matrix_df = pd.DataFrame(cnf_matrix, index=report_df.index[:-3].values, columns=report_df.index[:-3].values)  # Formata a matriz de confusão
-        cnf_matrix_normalized = cnf_matrix_df / cnf_matrix_df.sum(axis=1).values[:, np.newaxis]  # Normaliza a matriz de confusão
-        return ModelEvaluator._generate_heatmap(cnf_matrix_normalized, "Confusion Matrix"), cnf_matrix_normalized  # Retorna o heatmap e a matriz normalizada
+        report_df = pd.DataFrame(
+            classification_report(y_true, y_pred, output_dict=True)
+        ).transpose()  # Gera DataFrame do relatório
+        cnf_matrix_df = pd.DataFrame(
+            cnf_matrix, index=report_df.index[:-3].values, columns=report_df.index[:-3].values
+        )  # Formata a matriz de confusão
+        cnf_matrix_normalized = (
+            cnf_matrix_df / cnf_matrix_df.sum(axis=1).values[:, np.newaxis]
+        )  # Normaliza a matriz de confusão
+        return (
+            ModelEvaluator._generate_heatmap(cnf_matrix_normalized, "Confusion Matrix", square=True, fmt=".0%"),
+            cnf_matrix_normalized,
+        )  # Retorna o heatmap e a matriz normalizada
 
     @staticmethod
     def roc_auc(y_true, y_pred):
         lb = LabelBinarizer()  # Inicializa o binarizador de labels
         lb.fit(y_true)  # Ajusta o binarizador aos valores verdadeiros
         y_test = lb.transform(y_true)  # Transforma os valores verdadeiros
         y_pred = lb.transform(y_pred)  # Transforma os valores preditos
```

### Comparing `medroom_ai_dataengineer-0.0.7/medroom/dna/processors/utils/mlflow_helper.py` & `medroom_ai_dataengineer-0.0.8/medroom/dna/processors/utils/mlflow_helper.py`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.7/medroom/dna/processors/utils/textclean.py` & `medroom_ai_dataengineer-0.0.8/medroom/dna/processors/utils/textclean.py`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.7/setup.py` & `medroom_ai_dataengineer-0.0.8/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,39 @@
-from setuptools import find_namespace_packages, setup
-from setuptools.command.install import install
-from setuptools import setup, find_packages
-from distutils.command.install import install as _install
-
 import os
+from distutils.command.install import install as _install
 
+from setuptools import find_namespace_packages, find_packages, setup
+from setuptools.command.install import install
 
 PROJECT_DIR = os.path.dirname(__file__)
-INFO = open(os.path.join(PROJECT_DIR, 'INFO')).readlines()
-INFO = dict((line.strip().split('=') for line in INFO))
+INFO = open(os.path.join(PROJECT_DIR, "INFO")).readlines()
+INFO = dict(line.strip().split("=") for line in INFO)
 
-DEPENDENCIES = open(os.path.join(PROJECT_DIR, 'requirements.txt')).readlines()
+DEPENDENCIES = open(os.path.join(PROJECT_DIR, "requirements.txt")).readlines()
 
 setup(
-    name='MedRoom.AI.DataEngineer',
-    description='A Natural Language Processing Data Engineer',
-    version=INFO['version'],
-    author=INFO['author'],
-    author_email=INFO['author_email'],
-    url=INFO['url'],    
-    license=open(os.path.join(PROJECT_DIR, 'LICENSE')).read(),
-    packages=find_namespace_packages(include=['medroom','medroom.dna', 'medroom.dna.processors', 'medroom.dna.processors.*', 'medroom.dna.processors.utils']),
-    install_requires=[d for d in DEPENDENCIES if '://' not in d],
-    extras_require={
-        'plotting': ['matplotlib==3.7.0', 'seaborn==0.13.0']
-    },
-    python_requires='>=3.8',
-    #TO-DO: Fix dependency links : not working with bdist_wheel
-    dependency_links = ["git+https://github.com/explosion/spacy-models/releases/download/pt_core_news_sm-3.2.0/pt_core_news_sm-3.2.0.tar.gz"],
-    tests_require=['pytest', 'parameterized'],
-    zip_safe=False
-)
+    name="MedRoom.AI.DataEngineer",
+    description="A Natural Language Processing Data Engineer",
+    version=INFO["version"],
+    author=INFO["author"],
+    author_email=INFO["author_email"],
+    url=INFO["url"],
+    license=open(os.path.join(PROJECT_DIR, "LICENSE")).read(),
+    packages=find_namespace_packages(
+        include=[
+            "medroom",
+            "medroom.dna",
+            "medroom.dna.processors",
+            "medroom.dna.processors.*",
+            "medroom.dna.processors.utils",
+        ]
+    ),
+    install_requires=[d for d in DEPENDENCIES if "://" not in d],
+    extras_require={"plotting": ["matplotlib==3.7.0", "seaborn==0.13.0"]},
+    python_requires=">=3.8",
+    # TO-DO: Fix dependency links : not working with bdist_wheel
+    dependency_links=[
+        "git+https://github.com/explosion/spacy-models/releases/download/pt_core_news_sm-3.2.0/pt_core_news_sm-3.2.0.tar.gz"
+    ],
+    tests_require=["pytest", "parameterized"],
+    zip_safe=False,
+)
```

