# Comparing `tmp/fastapi_starter-0.1.0.tar.gz` & `tmp/fastapi_starter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_starter-0.1.0.tar", last modified: Mon May 27 20:38:05 2024, max compression
+gzip compressed data, was "fastapi_starter-0.1.1.tar", last modified: Mon May 27 20:55:18 2024, max compression
```

## Comparing `fastapi_starter-0.1.0.tar` & `fastapi_starter-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 20:38:05.617208 fastapi_starter-0.1.0/
--rw-rw-rw-   0        0        0     1110 2024-05-27 15:05:42.000000 fastapi_starter-0.1.0/LICENCE
--rw-rw-rw-   0        0        0     3056 2024-05-27 20:38:05.615206 fastapi_starter-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1280 2024-05-27 15:05:51.000000 fastapi_starter-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 20:38:05.590252 fastapi_starter-0.1.0/fastapi_starter/
--rw-rw-rw-   0        0        0        0 2024-05-27 20:28:55.000000 fastapi_starter-0.1.0/fastapi_starter/__init__.py
--rw-rw-rw-   0        0        0     1390 2024-05-27 20:30:28.000000 fastapi_starter-0.1.0/fastapi_starter/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-27 20:38:05.611206 fastapi_starter-0.1.0/fastapi_starter.egg-info/
--rw-rw-rw-   0        0        0     3056 2024-05-27 20:38:05.000000 fastapi_starter-0.1.0/fastapi_starter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2024-05-27 20:38:05.000000 fastapi_starter-0.1.0/fastapi_starter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 20:38:05.000000 fastapi_starter-0.1.0/fastapi_starter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-05-27 20:38:05.000000 fastapi_starter-0.1.0/fastapi_starter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      356 2024-05-27 20:38:05.000000 fastapi_starter-0.1.0/fastapi_starter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-27 20:38:05.000000 fastapi_starter-0.1.0/fastapi_starter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 20:38:05.618206 fastapi_starter-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1934 2024-05-27 20:36:24.000000 fastapi_starter-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:55:18.265019 fastapi_starter-0.1.1/
+-rw-rw-rw-   0        0        0     1110 2024-05-27 15:05:42.000000 fastapi_starter-0.1.1/LICENCE
+-rw-rw-rw-   0        0        0     3011 2024-05-27 20:55:18.262120 fastapi_starter-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1267 2024-05-27 20:54:40.000000 fastapi_starter-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 20:55:18.155387 fastapi_starter-0.1.1/fastapi_starter/
+-rw-rw-rw-   0        0        0        0 2024-05-27 20:28:55.000000 fastapi_starter-0.1.1/fastapi_starter/__init__.py
+-rw-rw-rw-   0        0        0     1390 2024-05-27 20:30:28.000000 fastapi_starter-0.1.1/fastapi_starter/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:55:18.258113 fastapi_starter-0.1.1/fastapi_starter.egg-info/
+-rw-rw-rw-   0        0        0     3011 2024-05-27 20:55:18.000000 fastapi_starter-0.1.1/fastapi_starter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2024-05-27 20:55:18.000000 fastapi_starter-0.1.1/fastapi_starter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 20:55:18.000000 fastapi_starter-0.1.1/fastapi_starter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-05-27 20:55:18.000000 fastapi_starter-0.1.1/fastapi_starter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      356 2024-05-27 20:55:18.000000 fastapi_starter-0.1.1/fastapi_starter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-27 20:55:18.000000 fastapi_starter-0.1.1/fastapi_starter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 20:55:18.265019 fastapi_starter-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1934 2024-05-27 20:55:01.000000 fastapi_starter-0.1.1/setup.py
```

### Comparing `fastapi_starter-0.1.0/LICENCE` & `fastapi_starter-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `fastapi_starter-0.1.0/PKG-INFO` & `fastapi_starter-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_starter
-Version: 0.1.0
+Version: 0.1.1
 Summary: A biblioteca fastapi_starter é uma ferramenta projetada para facilitar a criação rápida e eficiente de projetos baseados no framework FastAPI. Ele automatiza a criação da estrutura básica do projeto, incluindo diretórios, arquivos de configuração e rotas iniciais, além de instalar automaticamente todas as dependências necessárias. Com o fastapi_starter, os desenvolvedores podem iniciar novos projetos FastAPI com apenas alguns comandos, economizando tempo e esforço.
 Author: Jse Guilherme Lins Filho
 Author-email: zeguilhermelins@hotmail.com
 License: MIT License
 Keywords: fastapi starter
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -46,35 +46,35 @@
 Requires-Dist: uvicorn
 Requires-Dist: watchfiles
 Requires-Dist: websockets
 
 
 # FastAPI Starter
 
-A biblioteca **FastAPI Starter** oferece uma maneira rÃ¡pida e fÃ¡cil de iniciar um novo projeto usando o FastAPI. Com apenas alguns comandos, vocÃª pode criar a estrutura bÃ¡sica de um projeto FastAPI, economizando tempo e esforÃ§o na configuraÃ§Ã£o inicial.
+A biblioteca **FastAPI Starter** oferece uma maneira rapida e fÃ¡cil de iniciar um novo projeto usando o FastAPI. Com apenas alguns comandos, vocÃª pode criar a estrutura basica de um projeto FastAPI, economizando tempo e esforÃ§o na configuraÃ§Ã£o inicial.
 
-## InstalaÃ§Ã£o
+## Como Instalar
 
-Para instalar a biblioteca, vocÃª pode usar pip. Certifique-se de ter o Python e o pip instalados em seu sistema.
+Para instalar a biblioteca, voce pode usar pip. Certifique-se de ter o Python e o pip instalados em seu sistema.
 
 ```
 pip install fastapi_starter
 ```
 
 ## Uso
 
 Depois de instalar a biblioteca, vocÃª pode usar o comando \`fastapi_starter\` seguido pelo nome do projeto desejado para iniciar um novo projeto FastAPI.
 
 ```
 fastapi_starter nome_do_projeto
 ```
 
-Isso criarÃ¡ a estrutura bÃ¡sica do projeto com o nome especificado. VocÃª serÃ¡ solicitado a fornecer um nome vÃ¡lido para o projeto, e a biblioteca garantirÃ¡ que o nome atenda aos requisitos.
+Isso criara a estrutura basica do projeto com o nome especificado. Voce sera solicitado a fornecer um nome valido para o projeto, e a biblioteca garantira que o nome atenda aos requisitos.
 
 ## Contribuindo
 
-ContribuiÃ§Ãµes sÃ£o bem-vindas! Se vocÃª encontrar um problema ou tiver uma sugestÃ£o de melhoria, sinta-se Ã  vontade para abrir uma issue ou enviar um pull request para o repositÃ³rio GitHub: [link para o repositÃ³rio](https://github.com/zeguil/fastapi_starter).
+ContribuiÃ§Ãµes sao bem-vindas! Se voce encontrar um problema ou tiver uma sugestÃ£o de melhoria, sinta-se a vontade para abrir uma issue ou enviar um pull request para o repositÃ³rio GitHub: [link para o repositÃ³rio](https://github.com/zeguil/fastapi_starter).
 
 ## LicenÃ§a
 
-Este projeto estÃ¡ licenciado sob a LicenÃ§a MIT - veja o arquivo [LICENSE](LICENSE) para detalhes.
+Este projeto esta licenciado sob a Licenca MIT - veja o arquivo [LICENSE](LICENSE) para detalhes.
```

### Comparing `fastapi_starter-0.1.0/README.md` & `fastapi_starter-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 
 # FastAPI Starter
 
-A biblioteca **FastAPI Starter** oferece uma maneira rápida e fácil de iniciar um novo projeto usando o FastAPI. Com apenas alguns comandos, você pode criar a estrutura básica de um projeto FastAPI, economizando tempo e esforço na configuração inicial.
+A biblioteca **FastAPI Starter** oferece uma maneira rapida e fácil de iniciar um novo projeto usando o FastAPI. Com apenas alguns comandos, você pode criar a estrutura basica de um projeto FastAPI, economizando tempo e esforço na configuração inicial.
 
-## Instalação
+## Como Instalar
 
-Para instalar a biblioteca, você pode usar pip. Certifique-se de ter o Python e o pip instalados em seu sistema.
+Para instalar a biblioteca, voce pode usar pip. Certifique-se de ter o Python e o pip instalados em seu sistema.
 
 ```
 pip install fastapi_starter
 ```
 
 ## Uso
 
 Depois de instalar a biblioteca, você pode usar o comando \`fastapi_starter\` seguido pelo nome do projeto desejado para iniciar um novo projeto FastAPI.
 
 ```
 fastapi_starter nome_do_projeto
 ```
 
-Isso criará a estrutura básica do projeto com o nome especificado. Você será solicitado a fornecer um nome válido para o projeto, e a biblioteca garantirá que o nome atenda aos requisitos.
+Isso criara a estrutura basica do projeto com o nome especificado. Voce sera solicitado a fornecer um nome valido para o projeto, e a biblioteca garantira que o nome atenda aos requisitos.
 
 ## Contribuindo
 
-Contribuições são bem-vindas! Se você encontrar um problema ou tiver uma sugestão de melhoria, sinta-se à vontade para abrir uma issue ou enviar um pull request para o repositório GitHub: [link para o repositório](https://github.com/zeguil/fastapi_starter).
+Contribuições sao bem-vindas! Se voce encontrar um problema ou tiver uma sugestão de melhoria, sinta-se a vontade para abrir uma issue ou enviar um pull request para o repositório GitHub: [link para o repositório](https://github.com/zeguil/fastapi_starter).
 
 ## Licença
 
-Este projeto está licenciado sob a Licença MIT - veja o arquivo [LICENSE](LICENSE) para detalhes.
+Este projeto esta licenciado sob a Licenca MIT - veja o arquivo [LICENSE](LICENSE) para detalhes.
```

### Comparing `fastapi_starter-0.1.0/fastapi_starter/cli.py` & `fastapi_starter-0.1.1/fastapi_starter/cli.py`

 * *Files identical despite different names*

### Comparing `fastapi_starter-0.1.0/fastapi_starter.egg-info/PKG-INFO` & `fastapi_starter-0.1.1/fastapi_starter.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_starter
-Version: 0.1.0
+Version: 0.1.1
 Summary: A biblioteca fastapi_starter é uma ferramenta projetada para facilitar a criação rápida e eficiente de projetos baseados no framework FastAPI. Ele automatiza a criação da estrutura básica do projeto, incluindo diretórios, arquivos de configuração e rotas iniciais, além de instalar automaticamente todas as dependências necessárias. Com o fastapi_starter, os desenvolvedores podem iniciar novos projetos FastAPI com apenas alguns comandos, economizando tempo e esforço.
 Author: Jse Guilherme Lins Filho
 Author-email: zeguilhermelins@hotmail.com
 License: MIT License
 Keywords: fastapi starter
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -46,35 +46,35 @@
 Requires-Dist: uvicorn
 Requires-Dist: watchfiles
 Requires-Dist: websockets
 
 
 # FastAPI Starter
 
-A biblioteca **FastAPI Starter** oferece uma maneira rÃ¡pida e fÃ¡cil de iniciar um novo projeto usando o FastAPI. Com apenas alguns comandos, vocÃª pode criar a estrutura bÃ¡sica de um projeto FastAPI, economizando tempo e esforÃ§o na configuraÃ§Ã£o inicial.
+A biblioteca **FastAPI Starter** oferece uma maneira rapida e fÃ¡cil de iniciar um novo projeto usando o FastAPI. Com apenas alguns comandos, vocÃª pode criar a estrutura basica de um projeto FastAPI, economizando tempo e esforÃ§o na configuraÃ§Ã£o inicial.
 
-## InstalaÃ§Ã£o
+## Como Instalar
 
-Para instalar a biblioteca, vocÃª pode usar pip. Certifique-se de ter o Python e o pip instalados em seu sistema.
+Para instalar a biblioteca, voce pode usar pip. Certifique-se de ter o Python e o pip instalados em seu sistema.
 
 ```
 pip install fastapi_starter
 ```
 
 ## Uso
 
 Depois de instalar a biblioteca, vocÃª pode usar o comando \`fastapi_starter\` seguido pelo nome do projeto desejado para iniciar um novo projeto FastAPI.
 
 ```
 fastapi_starter nome_do_projeto
 ```
 
-Isso criarÃ¡ a estrutura bÃ¡sica do projeto com o nome especificado. VocÃª serÃ¡ solicitado a fornecer um nome vÃ¡lido para o projeto, e a biblioteca garantirÃ¡ que o nome atenda aos requisitos.
+Isso criara a estrutura basica do projeto com o nome especificado. Voce sera solicitado a fornecer um nome valido para o projeto, e a biblioteca garantira que o nome atenda aos requisitos.
 
 ## Contribuindo
 
-ContribuiÃ§Ãµes sÃ£o bem-vindas! Se vocÃª encontrar um problema ou tiver uma sugestÃ£o de melhoria, sinta-se Ã  vontade para abrir uma issue ou enviar um pull request para o repositÃ³rio GitHub: [link para o repositÃ³rio](https://github.com/zeguil/fastapi_starter).
+ContribuiÃ§Ãµes sao bem-vindas! Se voce encontrar um problema ou tiver uma sugestÃ£o de melhoria, sinta-se a vontade para abrir uma issue ou enviar um pull request para o repositÃ³rio GitHub: [link para o repositÃ³rio](https://github.com/zeguil/fastapi_starter).
 
 ## LicenÃ§a
 
-Este projeto estÃ¡ licenciado sob a LicenÃ§a MIT - veja o arquivo [LICENSE](LICENSE) para detalhes.
+Este projeto esta licenciado sob a Licenca MIT - veja o arquivo [LICENSE](LICENSE) para detalhes.
```

### Comparing `fastapi_starter-0.1.0/setup.py` & `fastapi_starter-0.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(
     name='fastapi_starter',
-    version='0.1.0',
+    version='0.1.1',
     license='MIT License',
     long_description=readme,
     long_description_content_type="text/markdown",
     description='A biblioteca fastapi_starter é uma ferramenta projetada para facilitar a criação rápida e eficiente de projetos baseados no framework FastAPI. Ele automatiza a criação da estrutura básica do projeto, incluindo diretórios, arquivos de configuração e rotas iniciais, além de instalar automaticamente todas as dependências necessárias. Com o fastapi_starter, os desenvolvedores podem iniciar novos projetos FastAPI com apenas alguns comandos, economizando tempo e esforço.',
     author='Jse Guilherme Lins Filho',
     author_email='zeguilhermelins@hotmail.com',
     keywords='fastapi starter',
```

