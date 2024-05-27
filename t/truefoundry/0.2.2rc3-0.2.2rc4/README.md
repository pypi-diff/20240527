# Comparing `tmp/truefoundry-0.2.2rc3.tar.gz` & `tmp/truefoundry-0.2.2rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truefoundry-0.2.2rc3.tar", max compression
+gzip compressed data, was "truefoundry-0.2.2rc4.tar", max compression
```

## Comparing `truefoundry-0.2.2rc3.tar` & `truefoundry-0.2.2rc4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      871 2024-05-20 05:56:02.128657 truefoundry-0.2.2rc3/README.md
--rw-r--r--   0        0        0     1148 2024-05-20 05:56:17.004603 truefoundry-0.2.2rc3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-20 05:56:02.128657 truefoundry-0.2.2rc3/truefoundry/__init__.py
--rw-r--r--   0        0        0        0 2024-05-20 05:56:02.128657 truefoundry-0.2.2rc3/truefoundry/autodeploy/__init__.py
--rw-r--r--   0        0        0        0 2024-05-20 05:56:02.128657 truefoundry-0.2.2rc3/truefoundry/autodeploy/agents/__init__.py
--rw-r--r--   0        0        0     6405 2024-05-20 05:56:02.128657 truefoundry-0.2.2rc3/truefoundry/autodeploy/agents/base.py
--rw-r--r--   0        0        0     4126 2024-05-20 05:56:02.128657 truefoundry-0.2.2rc3/truefoundry/autodeploy/agents/developer.py
--rw-r--r--   0        0        0     4504 2024-05-20 05:56:02.128657 truefoundry-0.2.2rc3/truefoundry/autodeploy/agents/project_identifier.py
--rw-r--r--   0        0        0     2402 2024-05-20 05:56:02.128657 truefoundry-0.2.2rc3/truefoundry/autodeploy/agents/tester.py
--rw-r--r--   0        0        0    13806 2024-05-20 05:56:02.128657 truefoundry-0.2.2rc3/truefoundry/autodeploy/cli.py
--rw-r--r--   0        0        0     1553 2024-05-20 05:56:02.128657 truefoundry-0.2.2rc3/truefoundry/autodeploy/constants.py
--rw-r--r--   0        0        0      158 2024-05-20 05:56:02.128657 truefoundry-0.2.2rc3/truefoundry/autodeploy/exception.py
--rw-r--r--   0        0        0      325 2024-05-20 05:56:02.128657 truefoundry-0.2.2rc3/truefoundry/autodeploy/logger.py
--rw-r--r--   0        0        0      875 2024-05-20 05:56:02.128657 truefoundry-0.2.2rc3/truefoundry/autodeploy/tools/__init__.py
--rw-r--r--   0        0        0      856 2024-05-20 05:56:02.132657 truefoundry-0.2.2rc3/truefoundry/autodeploy/tools/ask.py
--rw-r--r--   0        0        0      779 2024-05-20 05:56:02.132657 truefoundry-0.2.2rc3/truefoundry/autodeploy/tools/base.py
--rw-r--r--   0        0        0     6036 2024-05-20 05:56:02.132657 truefoundry-0.2.2rc3/truefoundry/autodeploy/tools/commit.py
--rw-r--r--   0        0        0     4000 2024-05-20 05:56:02.132657 truefoundry-0.2.2rc3/truefoundry/autodeploy/tools/docker_build.py
--rw-r--r--   0        0        0     5061 2024-05-20 05:56:02.132657 truefoundry-0.2.2rc3/truefoundry/autodeploy/tools/docker_run.py
--rw-r--r--   0        0        0     2338 2024-05-20 05:56:02.132657 truefoundry-0.2.2rc3/truefoundry/autodeploy/tools/file_type_counts.py
--rw-r--r--   0        0        0     2644 2024-05-20 05:56:02.132657 truefoundry-0.2.2rc3/truefoundry/autodeploy/tools/list_files.py
--rw-r--r--   0        0        0     2254 2024-05-20 05:56:02.132657 truefoundry-0.2.2rc3/truefoundry/autodeploy/tools/read_file.py
--rw-r--r--   0        0        0     1680 2024-05-20 05:56:02.132657 truefoundry-0.2.2rc3/truefoundry/autodeploy/tools/send_request.py
--rw-r--r--   0        0        0     3130 2024-05-20 05:56:02.132657 truefoundry-0.2.2rc3/truefoundry/autodeploy/tools/write_file.py
--rw-r--r--   0        0        0      453 2024-05-20 05:56:02.132657 truefoundry-0.2.2rc3/truefoundry/autodeploy/utils/client.py
--rw-r--r--   0        0        0     5358 2024-05-20 05:56:02.132657 truefoundry-0.2.2rc3/truefoundry/autodeploy/utils/diff.py
--rw-r--r--   0        0        0      412 2024-05-20 05:56:02.132657 truefoundry-0.2.2rc3/truefoundry/autodeploy/utils/pydantic_compat.py
--rw-r--r--   0        0        0        0 2024-05-20 05:56:02.132657 truefoundry-0.2.2rc3/truefoundry/cli/__init__.py
--rw-r--r--   0        0        0      916 2024-05-20 05:56:02.132657 truefoundry-0.2.2rc3/truefoundry/cli/__main__.py
--rw-r--r--   0        0        0       43 2024-05-20 05:56:02.132657 truefoundry-0.2.2rc3/truefoundry/deploy/__init__.py
--rw-r--r--   0        0        0        0 2024-05-20 05:56:02.132657 truefoundry-0.2.2rc3/truefoundry/deploy/cli/__init__.py
--rw-r--r--   0        0        0     3143 2024-05-20 05:56:02.132657 truefoundry-0.2.2rc3/truefoundry/deploy/cli/cli.py
--rw-r--r--   0        0        0     5105 2024-05-20 05:56:02.132657 truefoundry-0.2.2rc3/truefoundry/deploy/cli/deploy.py
--rw-r--r--   0        0        0      127 2024-05-20 05:56:02.132657 truefoundry-0.2.2rc3/truefoundry/deploy/cli/version.py
--rw-r--r--   0        0        0       53 2024-05-20 05:56:02.132657 truefoundry-0.2.2rc3/truefoundry/langchain/__init__.py
--rw-r--r--   0        0        0      179 2024-05-20 05:56:02.132657 truefoundry-0.2.2rc3/truefoundry/ml/__init__.py
--rw-r--r--   0        0        0     1839 1970-01-01 00:00:00.000000 truefoundry-0.2.2rc3/PKG-INFO
+-rw-r--r--   0        0        0      871 2024-05-21 07:37:19.033511 truefoundry-0.2.2rc4/README.md
+-rw-r--r--   0        0        0     1148 2024-05-21 07:37:31.653349 truefoundry-0.2.2rc4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/autodeploy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/autodeploy/agents/__init__.py
+-rw-r--r--   0        0        0     6405 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/autodeploy/agents/base.py
+-rw-r--r--   0        0        0     4126 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/autodeploy/agents/developer.py
+-rw-r--r--   0        0        0     4504 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/autodeploy/agents/project_identifier.py
+-rw-r--r--   0        0        0     2402 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/autodeploy/agents/tester.py
+-rw-r--r--   0        0        0    13989 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/autodeploy/cli.py
+-rw-r--r--   0        0        0     1273 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/autodeploy/constants.py
+-rw-r--r--   0        0        0      158 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/autodeploy/exception.py
+-rw-r--r--   0        0        0      325 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/autodeploy/logger.py
+-rw-r--r--   0        0        0      875 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/autodeploy/tools/__init__.py
+-rw-r--r--   0        0        0      856 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/autodeploy/tools/ask.py
+-rw-r--r--   0        0        0      779 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/autodeploy/tools/base.py
+-rw-r--r--   0        0        0     6036 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/autodeploy/tools/commit.py
+-rw-r--r--   0        0        0     4000 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/autodeploy/tools/docker_build.py
+-rw-r--r--   0        0        0     5061 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/autodeploy/tools/docker_run.py
+-rw-r--r--   0        0        0     2354 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/autodeploy/tools/file_type_counts.py
+-rw-r--r--   0        0        0     2643 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/autodeploy/tools/list_files.py
+-rw-r--r--   0        0        0     2254 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/autodeploy/tools/read_file.py
+-rw-r--r--   0        0        0     1688 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/autodeploy/tools/send_request.py
+-rw-r--r--   0        0        0     3130 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/autodeploy/tools/write_file.py
+-rw-r--r--   0        0        0      453 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/autodeploy/utils/client.py
+-rw-r--r--   0        0        0     5358 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/autodeploy/utils/diff.py
+-rw-r--r--   0        0        0      412 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/autodeploy/utils/pydantic_compat.py
+-rw-r--r--   0        0        0        0 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/cli/__init__.py
+-rw-r--r--   0        0        0      916 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/cli/__main__.py
+-rw-r--r--   0        0        0       43 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/deploy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/deploy/cli/__init__.py
+-rw-r--r--   0        0        0     3143 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/deploy/cli/cli.py
+-rw-r--r--   0        0        0     4767 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/deploy/cli/deploy.py
+-rw-r--r--   0        0        0      127 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/deploy/cli/version.py
+-rw-r--r--   0        0        0       53 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/langchain/__init__.py
+-rw-r--r--   0        0        0      179 2024-05-21 07:37:19.037511 truefoundry-0.2.2rc4/truefoundry/ml/__init__.py
+-rw-r--r--   0        0        0     1839 1970-01-01 00:00:00.000000 truefoundry-0.2.2rc4/PKG-INFO
```

### Comparing `truefoundry-0.2.2rc3/README.md` & `truefoundry-0.2.2rc4/README.md`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.2rc3/pyproject.toml` & `truefoundry-0.2.2rc4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "truefoundry"
-version = "0.2.2rc3"
+version = "0.2.2rc4"
 description = "Truefoundry CLI"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.13"
 servicefoundry = "0.10.11"
```

### Comparing `truefoundry-0.2.2rc3/truefoundry/autodeploy/agents/base.py` & `truefoundry-0.2.2rc4/truefoundry/autodeploy/agents/base.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.2rc3/truefoundry/autodeploy/agents/developer.py` & `truefoundry-0.2.2rc4/truefoundry/autodeploy/agents/developer.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.2rc3/truefoundry/autodeploy/agents/project_identifier.py` & `truefoundry-0.2.2rc4/truefoundry/autodeploy/agents/project_identifier.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.2rc3/truefoundry/autodeploy/agents/tester.py` & `truefoundry-0.2.2rc4/truefoundry/autodeploy/agents/tester.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.2rc3/truefoundry/autodeploy/cli.py` & `truefoundry-0.2.2rc4/truefoundry/autodeploy/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 from truefoundry.autodeploy.agents.project_identifier import (
     ComponentType,
     ProjectIdentifier,
 )
 from truefoundry.autodeploy.agents.tester import Tester
 from truefoundry.autodeploy.constants import (
     ABOUT_AUTODEPLOY,
-    AUTODEPLOY_INTRO_MESSAGE,
     AUTODEPLOY_OPENAI_API_KEY,
     AUTODEPLOY_OPENAI_BASE_URL,
     AUTODEPLOY_TFY_BASE_URL,
 )
 from truefoundry.autodeploy.exception import InvalidRequirementsException
 from truefoundry.autodeploy.tools.ask import AskQuestion
 from truefoundry.autodeploy.tools.commit import CommitConfirmation
@@ -184,15 +183,15 @@
         )
         console.print(
             "[bold red]Error:[/] Unable to switch to the new branch. It's possible that this branch already exists."
         )
         sys.exit(1)
 
 
-def _update_status(event, status: Status):
+def _update_status(event, status: Status, component_type: ComponentType):
     if isinstance(event, (AskQuestion, CommitConfirmation)):
         status.stop()
 
     if isinstance(
         event, (Developer.Request, ProjectIdentifier.Response, Tester.Response)
     ):
         status.update(
@@ -206,17 +205,22 @@
 
     if isinstance(event, (Tester.Request, DockerRun.Response)):
         status.update(
             "[bold magenta]TrueFoundry[/] is currently running tests on the project..."
         )
 
     if isinstance(event, DockerRunLog):
-        status.update(
-            "[bold cyan]Running:[/] [bold magenta]TrueFoundry[/] is running your app in a Docker container. You can view logs here for potential warnings/errors. If you do not see any issues then you can press [yellow]control + c[/] to move to the next step."
-        )
+        if component_type == ComponentType.SERVICE:
+            status.update(
+                "[bold cyan]Running:[/] [bold magenta]TrueFoundry[/] is running your app in a Docker container. Press ctrl+c once your app is ready for testing."
+            )
+        else:
+            status.update(
+                "[bold cyan]Running:[/] [bold magenta]TrueFoundry[/] is running your app in a Docker container and waiting for completion."
+            )
 
 
 def _get_default_project_name(project_root_path: str):
     path = os.path.abspath(project_root_path).rstrip(os.path.sep)
     name = path.split(os.path.sep)[-1].lower()
     name = re.sub(r"[^a-z0-9]", "-", name)
     name = "-".join(n for n in name.split("-") if n)[:30]
@@ -234,15 +238,14 @@
 
 def cli(project_root_path: str, deploy: bool, workspace_fqn: str = None):
     console = Console()
     openai_client = _get_openai_client()
     docker_client = _get_docker(console)
     project_root_path = os.path.abspath(project_root_path)
     console.print(ABOUT_AUTODEPLOY)
-    console.print(AUTODEPLOY_INTRO_MESSAGE)
     console.print(
         "[bold reverse]You will need to have Docker and Git installed on your machine for this to work[/]"
     )
     if AUTODEPLOY_OPENAI_BASE_URL is not None and AUTODEPLOY_OPENAI_API_KEY is not None:
         console.print(
             "[bold green]OpenAI credentials found in environment variables.[/]"
         )
@@ -324,15 +327,17 @@
         developer_run = developer.run(developer.Request(command=command, name=name))
         inp = None
         response = None
         while True:
             try:
                 status.start()
                 event = developer_run.send(inp)
-                _update_status(event=event, status=status)
+                _update_status(
+                    event=event, status=status, component_type=component_type
+                )
                 inp = event.render(console)
             except StopIteration as ex:
                 response = ex.value
                 break
 
     if deploy:
         console.rule("[bold green]Deploying to Truefoundry[/]")
```

### Comparing `truefoundry-0.2.2rc3/truefoundry/autodeploy/constants.py` & `truefoundry-0.2.2rc4/truefoundry/autodeploy/constants.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,23 +6,17 @@
     "AUTODEPLOY_TFY_BASE_URL", "https://app.truefoundry.com"
 ).strip("/")
 AUTODEPLOY_OPENAI_BASE_URL = os.environ.get("AUTODEPLOY_OPENAI_BASE_URL")
 AUTODEPLOY_OPENAI_API_KEY = os.environ.get("AUTODEPLOY_OPENAI_API_KEY")
 AUTODEPLOY_MODEL_NAME = os.environ.get(
     "AUTODEPLOY_MODEL_NAME", "auto-deploy-openai/gpt-4-turbo-2024-04-09"
 )
-AUTODEPLOY_INTRO_MESSAGE = """Truefoundry will first check for a [blue]Dockerfile[/] in your project.
-If it's not present, Truefoundry will generate one for you.
-Then, it will attempt to build a Docker image on your machine.
-If any issues are encountered during this process, Truefoundry will attempt to automatically fix them.
-Finally, it will run the application to verify that everything is set up correctly.
-"""
-ABOUT_AUTODEPLOY = """To deploy your project, we will generate the deployment configuration using AI.
-We will analyze your codebase using our AI agent and make the required changes so that we can build and deploy the code.
-We will confirm all the changes with you.
+ABOUT_AUTODEPLOY = """We'll use AI to build and deploy your project automatically.
+Our AI Agent analyzes your codebase, checks for a Dockerfile, creates one if missing, builds a Docker image, fixes any issues, and runs the application to ensure we have built it correctly.
+If you don't want to use our AI Agent to deploy automatically, create a [green]truefoundry.yaml[/] file in your project's root.
 """
 # The maximum file size to read is set to 10KB.
 # This limit is determined by the token limit of the LLM used, which is 128,000 tokens.
 # Given that one token is approximately equivalent to 4 English characters,
 # a 10KB file size limit (or ~10,000 characters |  ~2500 tokens) ensures that the file content,
 # along with any additional context and instructions for the LLM, fits within the model's token limit.
 MAX_FILE_SIZE_READ = 10 * 1024
```

### Comparing `truefoundry-0.2.2rc3/truefoundry/autodeploy/tools/__init__.py` & `truefoundry-0.2.2rc4/truefoundry/autodeploy/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.2rc3/truefoundry/autodeploy/tools/ask.py` & `truefoundry-0.2.2rc4/truefoundry/autodeploy/tools/ask.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.2rc3/truefoundry/autodeploy/tools/base.py` & `truefoundry-0.2.2rc4/truefoundry/autodeploy/tools/base.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.2rc3/truefoundry/autodeploy/tools/commit.py` & `truefoundry-0.2.2rc4/truefoundry/autodeploy/tools/commit.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.2rc3/truefoundry/autodeploy/tools/docker_build.py` & `truefoundry-0.2.2rc4/truefoundry/autodeploy/tools/docker_build.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.2rc3/truefoundry/autodeploy/tools/docker_run.py` & `truefoundry-0.2.2rc4/truefoundry/autodeploy/tools/docker_run.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.2rc3/truefoundry/autodeploy/tools/file_type_counts.py` & `truefoundry-0.2.2rc4/truefoundry/autodeploy/tools/file_type_counts.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     def __init__(self, project_root_path: str):
         self.project_root_path = project_root_path
 
     def run(
         self, request: FileTypeCounts.Request
     ) -> Generator[Event, Any, ResponseEvent]:
         counter = Counter()
-        yield Rule(message="List Files")
+        yield Rule(message="[bold green]File Counts[/]")
         yield Message(
             message="[bold cyan]Processing:[/] Scanning for various file types..."
         )
 
         def gitignore(_):
             return False
```

### Comparing `truefoundry-0.2.2rc3/truefoundry/autodeploy/tools/list_files.py` & `truefoundry-0.2.2rc4/truefoundry/autodeploy/tools/list_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         )
         error: Optional[str] = Field(None)
 
     def __init__(self, project_root_path: str):
         self.project_root_path = project_root_path
 
     def run(self, request: ListFiles.Request) -> Generator[Event, Any, ResponseEvent]:
-        yield Rule(message="[bold green] List Files[/]")
+        yield Rule(message="[bold green]List Files[/]")
         yield Message(
             message=f"[bold cyan]Searching:[/] 🔍 Looking for files matching the pattern [magenta]{request.pattern}[/]"
         )
 
         paths: List[str] = []
 
         def gitignore(_):
```

### Comparing `truefoundry-0.2.2rc3/truefoundry/autodeploy/tools/read_file.py` & `truefoundry-0.2.2rc4/truefoundry/autodeploy/tools/read_file.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.2rc3/truefoundry/autodeploy/tools/send_request.py` & `truefoundry-0.2.2rc4/truefoundry/autodeploy/tools/send_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     class Response(ResponseEvent):
         response_code: Optional[int] = Field(None, description="Response Code")
         response_body: Optional[str] = None
         error: Optional[str] = Field(None, description="Error.")
 
     def run(self, request: SendRequest.Request) -> Generator[Event, Any, ResponseEvent]:
         self.call_count += 1
-        yield Rule(message="[bold green] Request send[/]")
+        yield Rule(message="[bold green]Endpoint Verification[/]")
         yield Message(
             message=f"[bold cyan]Testing:[/] Sending a [magenta]{request.method.upper()}[/] request to [magenta]{request.url}[/]"
         )
         try:
             response = requests.request(request.method.lower(), url=request.url)
             yield Message(
                 message=f"[bold green]Success:[/] Received response with status code [magenta]{response.status_code}[/]"
```

### Comparing `truefoundry-0.2.2rc3/truefoundry/autodeploy/tools/write_file.py` & `truefoundry-0.2.2rc4/truefoundry/autodeploy/tools/write_file.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.2rc3/truefoundry/autodeploy/utils/diff.py` & `truefoundry-0.2.2rc4/truefoundry/autodeploy/utils/diff.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.2rc3/truefoundry/cli/__main__.py` & `truefoundry-0.2.2rc4/truefoundry/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.2rc3/truefoundry/deploy/cli/cli.py` & `truefoundry-0.2.2rc4/truefoundry/deploy/cli/cli.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.2rc3/truefoundry/deploy/cli/deploy.py` & `truefoundry-0.2.2rc4/truefoundry/deploy/cli/deploy.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,21 +85,14 @@
                 'Please create a truefoundry.yaml or pass the file name with "--file file_name"',
                 fg="yellow",
             ),
             color=True,
         )
         sys.exit(1)
 
-    click.echo(
-        click.style(
-            'We will be using TrueFoundry AI to build your project.\nIf you wish to proceed without TrueFoundry AI,\nyou need to either have a truefoundry.yaml file in your project root or\npass the path to a yaml file using the "--file file_name" option.',
-            fg="yellow",
-        ),
-    )
-
     try:
         autodeploy_cli(project_root_path=".", deploy=True, workspace_fqn=workspace_fqn)
     except InvalidRequirementsException as e:
         raise UsageError(message=e.message) from e
     except Exception as e:
         raise UsageError(message=str(e)) from e
```

### Comparing `truefoundry-0.2.2rc3/PKG-INFO` & `truefoundry-0.2.2rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truefoundry
-Version: 0.2.2rc3
+Version: 0.2.2rc4
 Summary: Truefoundry CLI
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

