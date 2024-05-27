# Comparing `tmp/pipefyUts-1.0.5.tar.gz` & `tmp/pipefyUts-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipefyUts-1.0.5.tar", last modified: Thu May 23 21:28:09 2024, max compression
+gzip compressed data, was "pipefyUts-1.0.6.tar", last modified: Mon May 27 11:37:51 2024, max compression
```

## Comparing `pipefyUts-1.0.5.tar` & `pipefyUts-1.0.6.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 21:28:09.954315 pipefyUts-1.0.5/
--rw-rw-rw-   0        0        0      465 2023-04-28 18:31:34.000000 pipefyUts-1.0.5/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1058 2023-04-26 17:09:25.000000 pipefyUts-1.0.5/LICENCE.txt
--rw-rw-rw-   0        0        0       55 2024-05-23 13:46:23.000000 pipefyUts-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     3813 2024-05-23 21:28:09.950320 pipefyUts-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2785 2024-05-23 01:31:27.000000 pipefyUts-1.0.5/README.md
--rw-rw-rw-   0        0        0      212 2024-04-16 22:37:47.000000 pipefyUts-1.0.5/commands.txt
-drwxrwxrwx   0        0        0        0 2024-05-23 21:28:09.883315 pipefyUts-1.0.5/pipefyUts/
--rw-rw-rw-   0        0        0     4444 2024-05-23 20:43:38.000000 pipefyUts-1.0.5/pipefyUts/__init__.py
--rw-rw-rw-   0        0        0     5268 2024-05-23 20:17:00.000000 pipefyUts-1.0.5/pipefyUts/card.py
-drwxrwxrwx   0        0        0        0 2024-05-23 21:28:09.946313 pipefyUts-1.0.5/pipefyUts/graphql/
--rw-rw-rw-   0        0        0      181 2024-05-22 22:11:18.000000 pipefyUts-1.0.5/pipefyUts/graphql/createCard.gql
--rw-rw-rw-   0        0        0      336 2024-05-22 19:41:50.000000 pipefyUts-1.0.5/pipefyUts/graphql/listCardsFromPhase.gql
--rw-rw-rw-   0        0        0      137 2024-05-23 00:58:59.000000 pipefyUts-1.0.5/pipefyUts/graphql/listMembers.gql
--rw-rw-rw-   0        0        0      109 2024-05-22 19:34:03.000000 pipefyUts-1.0.5/pipefyUts/graphql/listStartFormFields.gql
--rw-rw-rw-   0        0        0      146 2024-05-22 19:24:55.000000 pipefyUts-1.0.5/pipefyUts/graphql/presignedUrl.gql
-drwxrwxrwx   0        0        0        0 2024-05-23 21:28:09.929312 pipefyUts-1.0.5/pipefyUts.egg-info/
--rw-rw-rw-   0        0        0     3813 2024-05-23 21:28:09.000000 pipefyUts-1.0.5/pipefyUts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2024-05-23 21:28:09.000000 pipefyUts-1.0.5/pipefyUts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 21:28:09.000000 pipefyUts-1.0.5/pipefyUts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-23 21:28:09.000000 pipefyUts-1.0.5/pipefyUts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-23 21:28:09.000000 pipefyUts-1.0.5/pipefyUts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5024 2024-05-23 20:56:24.000000 pipefyUts-1.0.5/run.py
--rw-rw-rw-   0        0        0       42 2024-05-23 21:28:09.954315 pipefyUts-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      819 2024-05-23 21:27:57.000000 pipefyUts-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:37:51.486017 pipefyUts-1.0.6/
+-rw-rw-rw-   0        0        0      465 2023-04-28 18:31:34.000000 pipefyUts-1.0.6/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1058 2023-04-26 17:09:25.000000 pipefyUts-1.0.6/LICENCE.txt
+-rw-rw-rw-   0        0        0       55 2024-05-23 13:46:23.000000 pipefyUts-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     3816 2024-05-27 11:37:51.482017 pipefyUts-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2788 2024-05-27 11:35:46.000000 pipefyUts-1.0.6/README.md
+-rw-rw-rw-   0        0        0      212 2024-04-16 22:37:47.000000 pipefyUts-1.0.6/commands.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 11:37:51.429017 pipefyUts-1.0.6/pipefyUts/
+-rw-rw-rw-   0        0        0     4652 2024-05-26 15:36:46.000000 pipefyUts-1.0.6/pipefyUts/__init__.py
+-rw-rw-rw-   0        0        0     5561 2024-05-27 11:31:02.000000 pipefyUts-1.0.6/pipefyUts/card.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:37:51.480018 pipefyUts-1.0.6/pipefyUts/graphql/
+-rw-rw-rw-   0        0        0      181 2024-05-22 22:11:18.000000 pipefyUts-1.0.6/pipefyUts/graphql/createCard.gql
+-rw-rw-rw-   0        0        0       72 2024-05-26 15:37:07.000000 pipefyUts-1.0.6/pipefyUts/graphql/deleteCards.gql
+-rw-rw-rw-   0        0        0      336 2024-05-22 19:41:50.000000 pipefyUts-1.0.6/pipefyUts/graphql/listCardsFromPhase.gql
+-rw-rw-rw-   0        0        0      137 2024-05-23 00:58:59.000000 pipefyUts-1.0.6/pipefyUts/graphql/listMembers.gql
+-rw-rw-rw-   0        0        0      109 2024-05-22 19:34:03.000000 pipefyUts-1.0.6/pipefyUts/graphql/listStartFormFields.gql
+-rw-rw-rw-   0        0        0      146 2024-05-22 19:24:55.000000 pipefyUts-1.0.6/pipefyUts/graphql/presignedUrl.gql
+drwxrwxrwx   0        0        0        0 2024-05-27 11:37:51.465018 pipefyUts-1.0.6/pipefyUts.egg-info/
+-rw-rw-rw-   0        0        0     3816 2024-05-27 11:37:51.000000 pipefyUts-1.0.6/pipefyUts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2024-05-27 11:37:51.000000 pipefyUts-1.0.6/pipefyUts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 11:37:51.000000 pipefyUts-1.0.6/pipefyUts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-27 11:37:51.000000 pipefyUts-1.0.6/pipefyUts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-27 11:37:51.000000 pipefyUts-1.0.6/pipefyUts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5081 2024-05-27 11:35:46.000000 pipefyUts-1.0.6/run.py
+-rw-rw-rw-   0        0        0       42 2024-05-27 11:37:51.486017 pipefyUts-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      819 2024-05-27 11:37:29.000000 pipefyUts-1.0.6/setup.py
```

### Comparing `pipefyUts-1.0.5/LICENCE.txt` & `pipefyUts-1.0.6/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `pipefyUts-1.0.5/PKG-INFO` & `pipefyUts-1.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipefyUts
-Version: 1.0.5
+Version: 1.0.6
 Summary: Pipefy manipulator
 Home-page: 
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Keywords: pipefyUts
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,14 +20,18 @@
 #
 ### Installation
 
 ```sh
 pip install pipefyUts
 ```
 
+## GitHub
+
+
+
 ## Usage
 
 <!-- //==================================================== -->
 ## Auth
 ##### python code
 ```py
 from pipefyUts import Pipefy
@@ -126,16 +130,14 @@
 
     #PIPEFY FIELDS
     description              = CardField(str)
     total_ammount            = CardField(float)
     files                    = CardField(list)
     files                    = CardField(list,is_file_path=True)
 
-    #DEFAULT
-    def __init__(self,**kwargs): NewCard.__init__(self,**kwargs)
 
 ```
 ### create card
 ```py
 #CREATE CARD OBJECT
 myNewCard = MyCard(
     description   = "AdtPro",
@@ -151,15 +153,20 @@
 
 
 ##### output
 ```json
 {"id":"card_id"}
 ```
 
+## deleteCard
+```py
+
+pfy.deleteCard(card_id="<card_id>")
 
+```
 
 Change Log
 ==========
 
 1.0.0 (2023-04-26)
 ------------------
 - First Release
```

### Comparing `pipefyUts-1.0.5/README.md` & `pipefyUts-1.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 #
 ### Installation
 
 ```sh
 pip install pipefyUts
 ```
 
+## GitHub
+
+
+
 ## Usage
 
 <!-- //==================================================== -->
 ## Auth
 ##### python code
 ```py
 from pipefyUts import Pipefy
@@ -108,16 +112,14 @@
 
     #PIPEFY FIELDS
     description              = CardField(str)
     total_ammount            = CardField(float)
     files                    = CardField(list)
     files                    = CardField(list,is_file_path=True)
 
-    #DEFAULT
-    def __init__(self,**kwargs): NewCard.__init__(self,**kwargs)
 
 ```
 ### create card
 ```py
 #CREATE CARD OBJECT
 myNewCard = MyCard(
     description   = "AdtPro",
@@ -133,7 +135,13 @@
 
 
 ##### output
 ```json
 {"id":"card_id"}
 ```
 
+## deleteCard
+```py
+
+pfy.deleteCard(card_id="<card_id>")
+
+```
```

### Comparing `pipefyUts-1.0.5/pipefyUts/__init__.py` & `pipefyUts-1.0.6/pipefyUts/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,15 +83,14 @@
         query = open(os.path.join(self.graph_folder,"listMembers.gql"),'r').read()
         query = query.replace("$org_id$",self.org_id)
 
         data = self.runQuery(query)["data"]["organizations"][0]["members"]
 
         return [x.get("user") for x in data]
         
-
     def createCard(self,card:NewCard):
         query = open(os.path.join(self.graph_folder,"createCard.gql"),'r').read()
         query = query.replace("$title$",card.__title__)
         query = query.replace("$pipe_id$",card.__pipeid__)
 
         fields = []
         for f in card.used_fields:
@@ -110,7 +109,11 @@
         
         fields = "\n,".join(fields)
         query = query.replace("$fields$",fields)
         query = query.replace('"null"',"null")
 
         return self.runQuery(query)["data"]["createCard"]["card"]
 
+    def deleteCard(self,card_id:str):
+        query = f'mutation {{ N0 :deleteCard(input:{{id: "{card_id}"}}){{ clientMutationId }}}}'
+        return self.runQuery(query)["data"]["N0"]["clientMutationId"]
+
```

### Comparing `pipefyUts-1.0.5/pipefyUts/card.py` & `pipefyUts-1.0.6/pipefyUts/card.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,18 +43,27 @@
 
         
 
 class NewCard:
     graph_folder = os.path.join(pathlib.Path(__file__).parent.resolve(),"graphql")
     used_fields = None
 
+    # def __new__(cls,*args,**kwargs):
+    #     instance = super(NewCard, cls).__new__(cls)
+    #     #instance.__init__(**kwargs)
+    #     # if isinstance(instance, Filho):
+    #     #     print("Filho foi instanciado")
+    #     return instance
+    #     # pass
+
     def __init__(self,**kwargs):
         self.validateRequired(**kwargs)
         self.validateFields(**kwargs)
         self.setFields(**kwargs)
+        pass
 
     def setFields(self,**kwargs):
         
         for key, value in kwargs.items():
             setattr(self,key,value)
         
         #SET DEFAULT FIELDS
@@ -62,19 +71,14 @@
         default_fields = [x for x in my_fields if x[1].default]
 
         not_defined = [x for x in default_fields if x[0] not in kwargs.keys()]
 
         for item in not_defined:
             setattr(self,item[0],item[1].default)
 
-
-
-
-
-
     def validateRequired(self,**kwargs):
         if not "__title__" in self.__dir__(): raise Exception("please define __title__")
         if not "__pipeid__" in self.__dir__(): raise Exception("please define __pipeid__")
 
         my_fields = [(x,object.__getattribute__(self,x)) for x in self.__dir__() if isinstance(object.__getattribute__(self,x),CardField)]
         required_ones = [x[0] for x in my_fields if x[1].required and x[1].default is None]
         missing = [x for x in required_ones if not x in kwargs]
@@ -107,9 +111,10 @@
                     for item in value:
                         if item.__class__ not in [str,int,list,float]:
                             raise Exception(f"invalid field type '{field.type}'")
                         elif field.is_file_path and not os.path.isfile(item):
                             raise Exception(f"file not found '{item}'")
                         elif field.list_sub_type == str and not isinstance(item,str):
                             raise Exception(f"invalid value '{item}'")
+        pass
```

### Comparing `pipefyUts-1.0.5/pipefyUts.egg-info/PKG-INFO` & `pipefyUts-1.0.6/pipefyUts.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipefyUts
-Version: 1.0.5
+Version: 1.0.6
 Summary: Pipefy manipulator
 Home-page: 
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Keywords: pipefyUts
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,14 +20,18 @@
 #
 ### Installation
 
 ```sh
 pip install pipefyUts
 ```
 
+## GitHub
+
+
+
 ## Usage
 
 <!-- //==================================================== -->
 ## Auth
 ##### python code
 ```py
 from pipefyUts import Pipefy
@@ -126,16 +130,14 @@
 
     #PIPEFY FIELDS
     description              = CardField(str)
     total_ammount            = CardField(float)
     files                    = CardField(list)
     files                    = CardField(list,is_file_path=True)
 
-    #DEFAULT
-    def __init__(self,**kwargs): NewCard.__init__(self,**kwargs)
 
 ```
 ### create card
 ```py
 #CREATE CARD OBJECT
 myNewCard = MyCard(
     description   = "AdtPro",
@@ -151,15 +153,20 @@
 
 
 ##### output
 ```json
 {"id":"card_id"}
 ```
 
+## deleteCard
+```py
+
+pfy.deleteCard(card_id="<card_id>")
 
+```
 
 Change Log
 ==========
 
 1.0.0 (2023-04-26)
 ------------------
 - First Release
```

### Comparing `pipefyUts-1.0.5/run.py` & `pipefyUts-1.0.6/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,26 +39,26 @@
     por_que_a_sympla_deve_absorver_a_perda = CardField(str,default="Organizador devendo valor a Sympla")
     como_o_reembolso_deve_acontecer        = CardField(str,default="Transferência bancária ")  #NAO RETIRAR O ESPAÇO
     cpf_ou_cnpj_apenas_n_meros             = CardField(str,default="null")
     copy_of_valor_do_reembolso_obrigat_rio = CardField(float)
     n_do_pedido_obrigat_rio                = CardField(str)
 
 
-    def __init__(self,**kwargs): NewCard.__init__(self,**kwargs)
+    #def __init__(self,**kwargs): NewCard.__init__(self,**kwargs)
 
 class Dias180Card(DefaultCardInfo):
 
     #PIPEFY FIELDS
     solicita_o_comprador_pedido     = CardField(str,default="Reembolso > 180 dias")
     cpf                             = CardField(str,default="null")
     valor_do_reembolso_obrigat_rio  = CardField(float)
     copy_of_n_do_pedido_obrigat_rio = CardField(str)
 
 
-    def __init__(self,**kwargs): NewCard.__init__(self,**kwargs)
+    #def __init__(self,**kwargs): NewCard.__init__(self,**kwargs)
 
 myNewCard = PerdaFinanceiraCard(
     n_do_evento_obrigat_rio                = "2310947",
     tipo_de_conta                          = "Conta-corrente",
     nome_da_pessoa_titular_da_conta        = "Hannalice Gottschalck Cavalcanti",
     #cnpj                                   = "",
     cpf_ou_cnpj_apenas_n_meros             = "46629599420",
@@ -67,37 +67,35 @@
     ag_ncia_sem_digito_obrigat_rio         = "3525",
     conta_sem_digito_obrigat_rio           = "16276",
     digito_da_conta_obrigat_rio            = "0",
     copy_of_valor_do_reembolso_obrigat_rio = 80,
     n_do_pedido_obrigat_rio                = "26GP37091SR"
 )
 
-myNewCard = Dias180Card(
-    n_do_evento_obrigat_rio         = "2310947",
-    tipo_de_conta                   = "Conta-corrente",
-    nome_da_pessoa_titular_da_conta = "Hannalice Gottschalck Cavalcanti",
-    banco                           = "Banco do Brasil",
-    c_digo_do_banco_n_o_obrigat_rio = "1",
-    ag_ncia_sem_digito_obrigat_rio  = "3525",
-    conta_sem_digito_obrigat_rio    = "16276",
-    digito_da_conta_obrigat_rio     = "0",
-    #cnpj                           = "",
-    cpf                             = "46629599420",
-    valor_do_reembolso_obrigat_rio  = 123.456,
-    copy_of_n_do_pedido_obrigat_rio = "123456"
-)
+# myNewCard = Dias180Card(
+#     n_do_evento_obrigat_rio         = "2310947",
+#     tipo_de_conta                   = "Conta-corrente",
+#     nome_da_pessoa_titular_da_conta = "Hannalice Gottschalck Cavalcanti",
+#     banco                           = "Banco do Brasil",
+#     c_digo_do_banco_n_o_obrigat_rio = "1",
+#     ag_ncia_sem_digito_obrigat_rio  = "3525",
+#     conta_sem_digito_obrigat_rio    = "16276",
+#     digito_da_conta_obrigat_rio     = "0",
+#     #cnpj                           = "",
+#     cpf                             = "46629599420",
+#     valor_do_reembolso_obrigat_rio  = 123.456,
+#     copy_of_n_do_pedido_obrigat_rio = "123456"
+# )
 
 
 
 cd_id = pfy.createCard(card=myNewCard)
 
 
-
-
-
+pfy.deleteCard(cd_id.get("id"))
 
 
 
 pfy.listMembers()
 
 pfy.listStartFormFields(pipe_id="1025104")
```

### Comparing `pipefyUts-1.0.5/setup.py` & `pipefyUts-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='pipefyUts',
-  version='1.0.5',
+  version='1.0.6',
   description='Pipefy manipulator',
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='',  
   author='Melque Lima',
   author_email='melque_ex@yahoo.com.br',
   license='MIT',
```

