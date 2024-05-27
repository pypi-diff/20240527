# Comparing `tmp/eyeballvul-0.3.0.tar.gz` & `tmp/eyeballvul-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eyeballvul-0.3.0.tar", max compression
+gzip compressed data, was "eyeballvul-0.4.0.tar", max compression
```

## Comparing `eyeballvul-0.3.0.tar` & `eyeballvul-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1065 2024-05-13 18:22:34.820247 eyeballvul-0.3.0/LICENSE
--rw-r--r--   0        0        0    23521 2024-05-24 08:01:01.697510 eyeballvul-0.3.0/README.md
--rw-r--r--   0        0        0      287 2024-05-24 07:27:29.716177 eyeballvul-0.3.0/eyeballvul/__init__.py
--rw-r--r--   0        0        0     9338 2024-05-24 07:35:56.581707 eyeballvul-0.3.0/eyeballvul/api.py
--rw-r--r--   0        0        0     2301 2024-05-17 10:05:37.180830 eyeballvul-0.3.0/eyeballvul/cli.py
--rw-r--r--   0        0        0       48 2024-04-24 12:29:04.251010 eyeballvul-0.3.0/eyeballvul/config/__init__.py
--rw-r--r--   0        0        0      710 2024-05-22 08:39:48.617888 eyeballvul-0.3.0/eyeballvul/config/config.toml
--rw-r--r--   0        0        0     1374 2024-05-24 07:20:46.698632 eyeballvul-0.3.0/eyeballvul/config/config_loader.py
--rw-r--r--   0        0        0    23509 2024-05-22 08:21:37.785923 eyeballvul-0.3.0/eyeballvul/converter.py
--rw-r--r--   0        0        0      731 2024-05-15 16:33:53.123068 eyeballvul-0.3.0/eyeballvul/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-25 09:14:27.186264 eyeballvul-0.3.0/eyeballvul/models/__init__.py
--rw-r--r--   0        0        0     3249 2024-05-15 15:40:32.119299 eyeballvul-0.3.0/eyeballvul/models/cache.py
--rw-r--r--   0        0        0      167 2024-05-13 18:05:00.254883 eyeballvul-0.3.0/eyeballvul/models/common.py
--rw-r--r--   0        0        0     3968 2024-05-17 10:05:11.804390 eyeballvul-0.3.0/eyeballvul/models/eyeballvul.py
--rw-r--r--   0        0        0     4039 2024-05-14 08:38:45.464076 eyeballvul-0.3.0/eyeballvul/models/osv.py
--rw-r--r--   0        0        0        0 2024-05-17 08:30:21.997460 eyeballvul-0.3.0/eyeballvul/py.typed
--rw-r--r--   0        0        0     8681 2024-05-22 08:21:37.785923 eyeballvul-0.3.0/eyeballvul/score.py
--rw-r--r--   0        0        0     6839 2024-05-21 13:35:15.816506 eyeballvul-0.3.0/eyeballvul/util.py
--rw-r--r--   0        0        0     1361 2024-05-24 07:38:49.290177 eyeballvul-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    24203 1970-01-01 00:00:00.000000 eyeballvul-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-13 18:22:34.820247 eyeballvul-0.4.0/LICENSE
+-rw-r--r--   0        0        0    25093 2024-05-27 14:31:53.885110 eyeballvul-0.4.0/README.md
+-rw-r--r--   0        0        0      263 2024-05-27 14:00:42.100975 eyeballvul-0.4.0/eyeballvul/__init__.py
+-rw-r--r--   0        0        0     8430 2024-05-27 14:32:06.013136 eyeballvul-0.4.0/eyeballvul/api.py
+-rw-r--r--   0        0        0     2392 2024-05-27 12:27:10.873062 eyeballvul-0.4.0/eyeballvul/cli.py
+-rw-r--r--   0        0        0       48 2024-04-24 12:29:04.251010 eyeballvul-0.4.0/eyeballvul/config/__init__.py
+-rw-r--r--   0        0        0      710 2024-05-22 08:39:48.617888 eyeballvul-0.4.0/eyeballvul/config/config.toml
+-rw-r--r--   0        0        0     1374 2024-05-24 07:20:46.698632 eyeballvul-0.4.0/eyeballvul/config/config_loader.py
+-rw-r--r--   0        0        0    25925 2024-05-27 12:43:05.724118 eyeballvul-0.4.0/eyeballvul/converter.py
+-rw-r--r--   0        0        0      731 2024-05-15 16:33:53.123068 eyeballvul-0.4.0/eyeballvul/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-25 09:14:27.186264 eyeballvul-0.4.0/eyeballvul/models/__init__.py
+-rw-r--r--   0        0        0     3249 2024-05-15 15:40:32.119299 eyeballvul-0.4.0/eyeballvul/models/cache.py
+-rw-r--r--   0        0        0      167 2024-05-13 18:05:00.254883 eyeballvul-0.4.0/eyeballvul/models/common.py
+-rw-r--r--   0        0        0     3968 2024-05-17 10:05:11.804390 eyeballvul-0.4.0/eyeballvul/models/eyeballvul.py
+-rw-r--r--   0        0        0     4039 2024-05-14 08:38:45.464076 eyeballvul-0.4.0/eyeballvul/models/osv.py
+-rw-r--r--   0        0        0        0 2024-05-17 08:30:21.997460 eyeballvul-0.4.0/eyeballvul/py.typed
+-rw-r--r--   0        0        0     8681 2024-05-22 08:21:37.785923 eyeballvul-0.4.0/eyeballvul/score.py
+-rw-r--r--   0        0        0     6839 2024-05-21 13:35:15.816506 eyeballvul-0.4.0/eyeballvul/util.py
+-rw-r--r--   0        0        0     1361 2024-05-27 14:33:16.997287 eyeballvul-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    25775 1970-01-01 00:00:00.000000 eyeballvul-0.4.0/PKG-INFO
```

### Comparing `eyeballvul-0.3.0/LICENSE` & `eyeballvul-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eyeballvul-0.3.0/README.md` & `eyeballvul-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 At a high level, eyeballvul converts the data stream of CVEs in open-source repositories into a small set of commits for each repository, and a set of vulnerabilities present at each of these commits.
 
 The typical use case that this benchmark enables is the following:
 1. select a list of repositories and commits for which there is at least one vulnerability published after some date;
 1. run a SAST tool (typically LLM-based) on the source code at each of these commits;
 1. compare the results of the SAST tool with the list of known vulnerabilities for each commit, especially the ones that were published after the training data cutoff.
 
-eyeballvul currently contains 28,074 vulnerabilities, in 7,432 commits and 6,425 repositories.
+eyeballvul currently contains 24,436 vulnerabilities, in 6,662 commits and 5,924 repositories.
 
 ## Table of contents
 * [Installation](#installation)
 * [Data model](#data-model)
 * [How to use](#how-to-use)
 * [Motivation](#motivation)
 * [How it works](#how-it-works)
 * [Full example](#full-example)
+* [FAQ](#faq)
 
 
 ## Installation
 ```bash
 pip install eyeballvul
 ```
 
@@ -34,17 +35,17 @@
 ```
 
 (if you want to stick to a particular version of the data, you can use `download_data(date="YYYY-MM-DD")`. See valid dates in the [eyeballvul_data](https://github.com/timothee-chauvin/eyeballvul_data/tags) repo).
 
 ## Data model
 The data can be seen in the `data` directory. There are two kinds of items: **vulnerabilities** and **revisions**. A vulnerability corresponds to an entry in the [osv.dev](https://osv.dev/) database (typically a CVE), and may be present at multiple revisions of the repository. A revision represents the state of a repository at a given commit, and may be associated with multiple vulnerabilities. Let's look at an example of each (commands explained in the [How to use](#how-to-use) section):
 ```python
->>> from eyeballvul import get_by_project, get_revision
+>>> from eyeballvul import get_vulns, get_revision
 >>> import json
->>> vulnerability = get_by_project("https://github.com/gnome/nautilus")[0]
+>>> vulnerability = get_vulns(project="https://github.com/gnome/nautilus")[0]
 >>> print(json.dumps(vulnerability.to_dict(), indent=2))
 {
   "id": "CVE-2017-14604",
   "published": "2017-09-20T08:29:00",
   "modified": "2023-11-29T06:09:43.865268",
   "details": "GNOME Nautilus before 3.23.90 allows attackers to spoof a file type by using the .desktop file extension, as demonstrated by an attack in which a .desktop file's [...]",
   "severity": [
@@ -75,41 +76,43 @@
   },
   "size": 4708779
 }
 ```
 ## How to use
 For any of the commands shown below, run `help(command_name)` to see its documentation.
 ```python
->>> from eyeballvul import get_by_commit, get_by_project, get_commits, get_projects, get_revision
+>>> from eyeballvul import get_commits, get_projects, get_vulns, get_revision
 # `get_projects`: get the list of projects
+# get_projects() -> list[str]
 >>> projects = get_projects()
->>> len(projects)
-6425
-# `get_commits`: get a list of commits, with possible filtering by date and project
->>> all_commits = get_commits()
->>> len(all_commits)
-7432
-# Commits can be filtered by date:
->>> len(get_commits(after="2023-12-01"))
-939
-# More filtering:
->>> len(get_commits(after="2023-12-01", before="2024-01-01", project="https://github.com/torvalds/linux"))
-8
+# `get_commits`: get a list of commits, with possible filtering by date and project.
+# get_commits(
+#     after: str | datetime | None = None,
+#     before: str | datetime | None = None,
+#     project: str | None = None,
+# ) -> list[str]
+>>> commits = get_commits()
+>>> commits = get_commits(after="2023-12-01")
+>>> commits = get_commits(after="2023-12-01", before="2024-03-01", project="https://github.com/torvalds/linux")
 
 # `get_revision`: get the revision corresponding to a given commit
->>> revision = get_revision("a241f8f6f37220ccec78a40b015967188490b1df")
-# <output already shown above>
+# get_revision(commit: str) -> EyeballvulRevision
+>>> revision = get_revision("some commit hash (40 characters)")
 
-# `get_by_commit`: get a list of vulnerabilities present at a given commit
->>> vulnerabilities = get_by_commit("54ecb8f7028c5eb3d740bb82b0f1d90f2df63c5c")
->>> len(vulnerabilities)
-67
->>> vulnerabilities = get_by_commit("54ecb8f7028c5eb3d740bb82b0f1d90f2df63c5c", after="2024-01-01")
->>> len(vulnerabilities)
-7
+# `get_vulns`: get a list of vulnerabilities, with possible filtering by date, project, and commit.
+# get_vulns(
+#     after: str | datetime | None = None,
+#     before: str | datetime | None = None,
+#     project: str | None = None,
+#     commit: str | None = None,
+# ) -> list[EyeballvulItem]
+>>> vulns = get_vulns()
+>>> vulns = get_vulns(after="2024-01-01")
+>>> vulns = get_vulns(after="2024-01-01", project="https://github.com/torvalds/linux")
+>>> vulns = get_vulns(before="2024-05-01", commit="some commit hash (40 characters)")
 ```
 
 ## Motivation
 I believe that AI vulnerability detection in source code will disproportionately favor cyberdefense, especially if it is deployed on a wide scale as soon as it becomes feasible. The goal of this benchmark is to be a testing ground for new designs on this problem, as well as to keep evaluating the feasibility of wide-scale deployment as new models get released.
 
 The name "eyeballvul" comes from Linus's law, the assertion that "given enough eyeballs, all bugs are shallow". eyeballvul will hopefully help with the deployment of large numbers of AI eyeballs, once they can see well enough.
 
@@ -117,19 +120,19 @@
 
 ## How it works
 To get into the details, Google's [osv.dev](https://osv.dev/) vulnerability database for open-source projects is used as input. Vulnerabilities are grouped by repository, and their affected versions are extracted. Finding the smallest set of commits that cover all the affected versions is an instance of the [hitting set problem](https://en.wikipedia.org/wiki/Set_cover_problem#Hitting_set_formulation). This is an NP-complete problem, but in practice Google's [CP-SAT](https://or-tools.github.io/docs/pdoc/ortools/sat/python/cp_model.html) solver handles it well in all the repos tested so far. First, the number of commits necessary to cover all the affected versions is minimized, then the sum of their dates is maximized (to get more recent commits, all other things equal). Repository total sizes and language breakdowns are computed at each commit using Github's [linguist](https://github.com/github-linguist/linguist), enabling filtering by repository size or language in downstream evaluations.
 
 ## Full example
 Let's see how this benchmark can be used in practice. Let's use `https://github.com/parisneo/lollms-webui` as an example repository (cherry-picked to have a reasonable size, and to have 6 easy vulnerabilities published later than March 29, 2024).
 ```python
->>> from eyeballvul import get_by_project, get_commits, get_revision
+>>> from eyeballvul import get_vulns, get_commits, get_revision
 >>> import json
->>> vulnerabilities = get_by_project("https://github.com/parisneo/lollms-webui")
->>> vulnerabilities_dicts = [v.to_dict() for v in vulnerabilities]
->>> print(json.dumps(vulnerabilities_dict, indent=2))
+>>> vulns = get_vulns(project="https://github.com/parisneo/lollms-webui")
+>>> vulns_dicts = [v.to_dict() for v in vulns]
+>>> print(json.dumps(vulns_dicts, indent=2))
 [
   {
     "id": "CVE-2024-1646",
     "published": "2024-04-16T00:15:09",
     "modified": "2024-04-17T01:16:41.423660",
     "details": "parisneo/lollms-webui is vulnerable to authentication bypass due to insufficient protection over sensitive endpoints. The application checks if the host parameter is not '0.0.0.0' to restrict access, which is inadequate when the application is bound to a specific interface, allowing unauthorized access to endpoints such as '/restart_program', '/update_software', '/check_update', '/start_recording', and '/stop_recording'. This vulnerability can lead to denial of service, unauthorized disabling or overriding of recordings, and potentially other impacts if certain features are enabled in the configuration.",
     "repo_url": "https://github.com/parisneo/lollms-webui",
@@ -413,7 +416,30 @@
 >>> recall = tp / (tp + fn)
 >>> recall
 0.5
 >>> f1 = 2 / (1 / precision + 1 / recall)
 >>> f1
 0.6666666666666666
 ```
+
+## FAQ
+### I'm GPU poor
+The sum of the repository sizes at each revision is around 75GB. Let's assume this translates to roughly 20B tokens. At $15/Mtok, you would be spending over $300k for a single pass on the benchmark if for example you used Claude 3 Opus. The solution: select a small random subset of the benchmark. A way to construct subsets that has nice properties is to use **commit hashes in alphabetical order**. If you work on a subset of the benchmark, please do that. For instance:
+```python
+>>> commits = get_commits()
+>>> commit_subset = sorted(commits)[:100]
+```
+
+To get a rough idea of the total size of different subsets, you could do:
+```python
+>>> total_size = sum(get_revision(commit).size for commit in commit_subset)
+```
+
+You may then further filter on reasonable criteria, such as repository size, language, or dates of vulnerabilities.
+
+### Where is the data?
+The data is kept in the [eyeballvul_data](https://github.com/timothee-chauvin/eyeballvul_data) repository. It is downloaded into `~/.cache/eyeballvul` when you run:
+```python
+from eyeballvul import download_data
+download_data()
+```
+The data sources (version-controlled OSV data, and eyeballvul cache) are kept in the [eyeballvul_data_sources](https://github.com/timothee-chauvin/eyeballvul_data_sources) repository.
```

### Comparing `eyeballvul-0.3.0/eyeballvul/api.py` & `eyeballvul-0.4.0/eyeballvul/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,77 +54,57 @@
     engine = create_engine(f"sqlite:///{Config.paths.db}/eyeballvul.db")
     with Session(engine) as session:
         query = select(EyeballvulItem.repo_url).distinct()
         return list(session.exec(query).all())
 
 
 @typechecked
-def get_by_commit(
-    commit_hash: str,
+def get_vulns(
     after: str | datetime | None = None,
     before: str | datetime | None = None,
+    project: str | None = None,
+    commit: str | None = None,
 ) -> list[EyeballvulItem]:
     """
-    Get the Eyeballvul items that match a commit hash.
-
-    The commit hash must be 40 characters long.
+    Get the Eyeballvul items that match the optional `after`, `before`, `project` and `commit`
+    parameters.
 
     The list can be filtered with the optional `after` and `before` parameters, which must be ISO
     8601 dates.
 
     `after` is included, and `before` is excluded, i.e. the possible options are: (1) after <= date,
     (2) after <= date < before, (3) date < before.
+
+    The list can also be filtered by the `project` parameter, a repo URL.
+
+    If provided, the commit hash (`commit`) must be 40 characters long.
     """
-    if len(commit_hash) != 40:
+    if commit and len(commit) != 40:
         raise ValueError("The commit hash must be 40 characters long.")
     engine = create_engine(f"sqlite:///{Config.paths.db}/eyeballvul.db")
     with Session(engine) as session:
-        # FIXME this isn't very clean (tests if the commit hash is part of the json string of the commit array)
-        # This SQL would be better, but I can't find a way to convert it to sqlalchemy:
-        # SELECT r.* FROM eyeballvulitem r, JSON_EACH(r.commits) as jc WHERE jc.value = 'commit_hash';
-
-        # type ignore used because EyeballvulItem.commits doesn't have
-        # a `contains` method, but this is valid sqlalchemy.
-        query = select(EyeballvulItem).where(EyeballvulItem.commits.contains(commit_hash))  # type: ignore[attr-defined]
+        query = select(EyeballvulItem)
 
+        if project:
+            query = query.where(EyeballvulItem.repo_url == project)
         if after:
             start_date = str_or_datetime_to_datetime(after)
             query = query.where(EyeballvulItem.published >= start_date)
         if before:
             end_date = str_or_datetime_to_datetime(before)
             query = query.where(EyeballvulItem.published < end_date)
 
-        return list(session.exec(query).all())
-
-
-@typechecked
-def get_by_project(
-    repo_url: str,
-    after: str | datetime | None = None,
-    before: str | datetime | None = None,
-) -> list[EyeballvulItem]:
-    """
-    Get the Eyeballvul items that match a project's repo URL.
-
-    The list can be filtered with the optional `after` and `before` parameters, which must be ISO
-    8601 dates.
-
-    `after` is included, and `before` is excluded, i.e. the possible options are: (1) after <= date,
-    (2) after <= date < before, (3) date < before.
-    """
-    engine = create_engine(f"sqlite:///{Config.paths.db}/eyeballvul.db")
-    with Session(engine) as session:
-        query = select(EyeballvulItem).where(EyeballvulItem.repo_url == repo_url)
+        # FIXME this isn't very clean (tests if the commit hash is part of the json string of the commit array)
+        # This SQL would be better, but I can't find a way to convert it to sqlalchemy:
+        # SELECT r.* FROM eyeballvulitem r, JSON_EACH(r.commits) as jc WHERE jc.value = 'commit_hash';
 
-        if after:
-            start_date = str_or_datetime_to_datetime(after)
-            query = query.where(EyeballvulItem.published >= start_date)
-        if before:
-            end_date = str_or_datetime_to_datetime(before)
-            query = query.where(EyeballvulItem.published < end_date)
+        # type ignore used because EyeballvulItem.commits doesn't have
+        # a `contains` method, but this is valid sqlalchemy.
+        if commit:
+            query = query.where(EyeballvulItem.commits.contains(commit))  # type: ignore[attr-defined]
 
         return list(session.exec(query).all())
 
 
 @typechecked
 def get_commits(
     after: str | datetime | None = None,
@@ -133,45 +113,43 @@
 ) -> list[str]:
     """
     Get a list of all commits that have at least one vuln within the date range.
 
     The list can be filtered with the optional `after` and `before` parameters, which must be ISO
     8601 dates.
 
+    Note that the date range doesn't apply to the commit date, but to the existence of at least one vuln associated with the commit within the date range.
+
     `after` is included, and `before` is excluded, i.e. the possible options are: (1) after <= date,
     (2) after <= date < before, (3) date < before.
 
     The list can also be filtered by the `project` parameter, a repo URL.
     """
-    engine = create_engine(f"sqlite:///{Config.paths.db}/eyeballvul.db")
-    with Session(engine) as session:
-        query = select(EyeballvulItem)
-        if project:
-            query = query.where(EyeballvulItem.repo_url == project)
-        if after:
-            start_date = str_or_datetime_to_datetime(after)
-            query = query.where(EyeballvulItem.published >= start_date)
-        if before:
-            end_date = str_or_datetime_to_datetime(before)
-            query = query.where(EyeballvulItem.published < end_date)
-
-        results = session.exec(query).all()
-        commits = {commit for item in results for commit in item.commits}
-        return list(commits)
+    vulns = get_vulns(after=after, before=before, project=project)
+    commits = {commit for vuln in vulns for commit in vuln.commits}
+    return list(commits)
 
 
 @typechecked
-def get_revision(commit_hash: str) -> EyeballvulRevision | None:
-    """Get the Eyeballvul revision that matches a commit hash."""
-    if len(commit_hash) != 40:
+def get_revision(commit: str) -> EyeballvulRevision:
+    """
+    Get the Eyeballvul revision that matches a commit hash.
+
+    If no revision can be found, raise a ValueError.
+    """
+    if len(commit) != 40:
         raise ValueError("The commit hash must be 40 characters long.")
     engine = create_engine(f"sqlite:///{Config.paths.db}/eyeballvul.db")
     with Session(engine) as session:
-        query = select(EyeballvulRevision).where(EyeballvulRevision.commit == commit_hash)
-        return session.exec(query).first()
+        query = select(EyeballvulRevision).where(EyeballvulRevision.commit == commit)
+        first = session.exec(query).first()
+        if first:
+            return first
+        else:
+            raise ValueError(f"Revision with commit hash {commit} not found.")
 
 
 def json_export() -> None:
     """Export the contents of the SQL database into JSON files in the data directory."""
     if Path(Config.paths.data).exists():
         raise ValueError(
             f"The data directory already exists at {Config.paths.data}.\n"
```

### Comparing `eyeballvul-0.3.0/eyeballvul/cli.py` & `eyeballvul-0.4.0/eyeballvul/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,18 @@
     def convert_all() -> None:
         return Converter().convert_all()
 
     @staticmethod
     def convert_range(start: int, end: int) -> None:
         return Converter().convert_range(start, end)
 
+    @staticmethod
+    def postprocess() -> None:
+        return Converter().postprocess()
+
 
 def json_import_cli() -> None:
     """Import the contents of the JSON files in the data directory into the SQL database."""
     json_import()
 
 
 def json_export_cli() -> None:
```

### Comparing `eyeballvul-0.3.0/eyeballvul/config/config.toml` & `eyeballvul-0.4.0/eyeballvul/config/config.toml`

 * *Files identical despite different names*

### Comparing `eyeballvul-0.3.0/eyeballvul/config/config_loader.py` & `eyeballvul-0.4.0/eyeballvul/config/config_loader.py`

 * *Files identical despite different names*

### Comparing `eyeballvul-0.3.0/eyeballvul/converter.py` & `eyeballvul-0.4.0/eyeballvul/converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -241,14 +241,64 @@
         only_print_length = [ConversionStatusCode.OK, ConversionStatusCode.NO_OSV_ITEMS_LEFT]
         logging.info("Done processing repositories. Statistics:")
         for status_code, concerned_repos in repos_by_status_code.items():
             logging.info(f"{len(concerned_repos)}/{repo_len}: {status_code}: {status_code.value}.")
             if status_code not in only_print_length:
                 logging.info(f"Concerned repos: {concerned_repos}")
 
+    def postprocess(self) -> None:
+        """Functions applied after the bulk of the conversion."""
+        self.remove_stale_revisions()
+        self.remove_empty_revisions()
+
+    def remove_stale_revisions(self) -> None:
+        """Remove all EyeballvulRevisions that don't have a corresponding EyeballvulItem."""
+        with Session(self.engine) as session:
+            revisions: dict[str, EyeballvulRevision] = {
+                revision.commit: revision
+                for revision in session.exec(select(EyeballvulRevision)).all()
+            }
+            item_commits = {
+                commit
+                for item in session.exec(select(EyeballvulItem)).all()
+                for commit in item.commits
+            }
+            stale_revision_commits = set(revisions.keys()) - item_commits
+            logging.info(f"Removing {len(stale_revision_commits)} stale revisions.")
+            for commit in stale_revision_commits:
+                session.delete(revisions[commit])
+            session.commit()
+
+    def remove_empty_revisions(self) -> None:
+        """Remove all EyeballvulRevisions for which linguist reports a size of 0 bytes, and the
+        EyeballvulItems that depended exclusively on these revisions."""
+        with Session(self.engine) as session:
+            revisions = session.exec(select(EyeballvulRevision)).all()
+            removed_commits = set()
+            for revision in revisions:
+                if revision.size == 0:
+                    logging.info(f"Removing revision {revision.commit} with size 0.")
+                    session.delete(revision)
+                    removed_commits.add(revision.commit)
+            items = session.exec(select(EyeballvulItem)).all()
+            for item in items:
+                updated_commits = [
+                    commit for commit in item.commits if commit not in removed_commits
+                ]
+                if not updated_commits:
+                    logging.info(
+                        f"Removing item {item.id} depending exclusively on empty revisions ({item.commits})."
+                    )
+                    session.delete(item)
+                elif set(updated_commits) != set(item.commits):
+                    logging.info(f"Updating item {item.id} with commits {updated_commits}.")
+                    item.commits = updated_commits
+                    session.add(item)
+            session.commit()
+
     @staticmethod
     def get_osv_items() -> list[dict]:
         """Get the items from the osv.dev dataset."""
         osv_path = Config.paths.osv
         items = []
         for ecosystem in Config.paths.osv.iterdir():
             for item_basename in ecosystem.iterdir():
```

### Comparing `eyeballvul-0.3.0/eyeballvul/exceptions.py` & `eyeballvul-0.4.0/eyeballvul/exceptions.py`

 * *Files identical despite different names*

### Comparing `eyeballvul-0.3.0/eyeballvul/models/cache.py` & `eyeballvul-0.4.0/eyeballvul/models/cache.py`

 * *Files identical despite different names*

### Comparing `eyeballvul-0.3.0/eyeballvul/models/eyeballvul.py` & `eyeballvul-0.4.0/eyeballvul/models/eyeballvul.py`

 * *Files identical despite different names*

### Comparing `eyeballvul-0.3.0/eyeballvul/models/osv.py` & `eyeballvul-0.4.0/eyeballvul/models/osv.py`

 * *Files identical despite different names*

### Comparing `eyeballvul-0.3.0/eyeballvul/score.py` & `eyeballvul-0.4.0/eyeballvul/score.py`

 * *Files identical despite different names*

### Comparing `eyeballvul-0.3.0/eyeballvul/util.py` & `eyeballvul-0.4.0/eyeballvul/util.py`

 * *Files identical despite different names*

### Comparing `eyeballvul-0.3.0/pyproject.toml` & `eyeballvul-0.4.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eyeballvul"
-version = "0.3.0"
+version = "0.4.0"
 description = ""
 authors = ["Timothee Chauvin <timothee.chauvin28@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "eyeballvul" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `eyeballvul-0.3.0/PKG-INFO` & `eyeballvul-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyeballvul
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 Author: Timothee Chauvin
 Author-email: timothee.chauvin28@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -27,23 +27,24 @@
 At a high level, eyeballvul converts the data stream of CVEs in open-source repositories into a small set of commits for each repository, and a set of vulnerabilities present at each of these commits.
 
 The typical use case that this benchmark enables is the following:
 1. select a list of repositories and commits for which there is at least one vulnerability published after some date;
 1. run a SAST tool (typically LLM-based) on the source code at each of these commits;
 1. compare the results of the SAST tool with the list of known vulnerabilities for each commit, especially the ones that were published after the training data cutoff.
 
-eyeballvul currently contains 28,074 vulnerabilities, in 7,432 commits and 6,425 repositories.
+eyeballvul currently contains 24,436 vulnerabilities, in 6,662 commits and 5,924 repositories.
 
 ## Table of contents
 * [Installation](#installation)
 * [Data model](#data-model)
 * [How to use](#how-to-use)
 * [Motivation](#motivation)
 * [How it works](#how-it-works)
 * [Full example](#full-example)
+* [FAQ](#faq)
 
 
 ## Installation
 ```bash
 pip install eyeballvul
 ```
 
@@ -54,17 +55,17 @@
 ```
 
 (if you want to stick to a particular version of the data, you can use `download_data(date="YYYY-MM-DD")`. See valid dates in the [eyeballvul_data](https://github.com/timothee-chauvin/eyeballvul_data/tags) repo).
 
 ## Data model
 The data can be seen in the `data` directory. There are two kinds of items: **vulnerabilities** and **revisions**. A vulnerability corresponds to an entry in the [osv.dev](https://osv.dev/) database (typically a CVE), and may be present at multiple revisions of the repository. A revision represents the state of a repository at a given commit, and may be associated with multiple vulnerabilities. Let's look at an example of each (commands explained in the [How to use](#how-to-use) section):
 ```python
->>> from eyeballvul import get_by_project, get_revision
+>>> from eyeballvul import get_vulns, get_revision
 >>> import json
->>> vulnerability = get_by_project("https://github.com/gnome/nautilus")[0]
+>>> vulnerability = get_vulns(project="https://github.com/gnome/nautilus")[0]
 >>> print(json.dumps(vulnerability.to_dict(), indent=2))
 {
   "id": "CVE-2017-14604",
   "published": "2017-09-20T08:29:00",
   "modified": "2023-11-29T06:09:43.865268",
   "details": "GNOME Nautilus before 3.23.90 allows attackers to spoof a file type by using the .desktop file extension, as demonstrated by an attack in which a .desktop file's [...]",
   "severity": [
@@ -95,41 +96,43 @@
   },
   "size": 4708779
 }
 ```
 ## How to use
 For any of the commands shown below, run `help(command_name)` to see its documentation.
 ```python
->>> from eyeballvul import get_by_commit, get_by_project, get_commits, get_projects, get_revision
+>>> from eyeballvul import get_commits, get_projects, get_vulns, get_revision
 # `get_projects`: get the list of projects
+# get_projects() -> list[str]
 >>> projects = get_projects()
->>> len(projects)
-6425
-# `get_commits`: get a list of commits, with possible filtering by date and project
->>> all_commits = get_commits()
->>> len(all_commits)
-7432
-# Commits can be filtered by date:
->>> len(get_commits(after="2023-12-01"))
-939
-# More filtering:
->>> len(get_commits(after="2023-12-01", before="2024-01-01", project="https://github.com/torvalds/linux"))
-8
+# `get_commits`: get a list of commits, with possible filtering by date and project.
+# get_commits(
+#     after: str | datetime | None = None,
+#     before: str | datetime | None = None,
+#     project: str | None = None,
+# ) -> list[str]
+>>> commits = get_commits()
+>>> commits = get_commits(after="2023-12-01")
+>>> commits = get_commits(after="2023-12-01", before="2024-03-01", project="https://github.com/torvalds/linux")
 
 # `get_revision`: get the revision corresponding to a given commit
->>> revision = get_revision("a241f8f6f37220ccec78a40b015967188490b1df")
-# <output already shown above>
+# get_revision(commit: str) -> EyeballvulRevision
+>>> revision = get_revision("some commit hash (40 characters)")
 
-# `get_by_commit`: get a list of vulnerabilities present at a given commit
->>> vulnerabilities = get_by_commit("54ecb8f7028c5eb3d740bb82b0f1d90f2df63c5c")
->>> len(vulnerabilities)
-67
->>> vulnerabilities = get_by_commit("54ecb8f7028c5eb3d740bb82b0f1d90f2df63c5c", after="2024-01-01")
->>> len(vulnerabilities)
-7
+# `get_vulns`: get a list of vulnerabilities, with possible filtering by date, project, and commit.
+# get_vulns(
+#     after: str | datetime | None = None,
+#     before: str | datetime | None = None,
+#     project: str | None = None,
+#     commit: str | None = None,
+# ) -> list[EyeballvulItem]
+>>> vulns = get_vulns()
+>>> vulns = get_vulns(after="2024-01-01")
+>>> vulns = get_vulns(after="2024-01-01", project="https://github.com/torvalds/linux")
+>>> vulns = get_vulns(before="2024-05-01", commit="some commit hash (40 characters)")
 ```
 
 ## Motivation
 I believe that AI vulnerability detection in source code will disproportionately favor cyberdefense, especially if it is deployed on a wide scale as soon as it becomes feasible. The goal of this benchmark is to be a testing ground for new designs on this problem, as well as to keep evaluating the feasibility of wide-scale deployment as new models get released.
 
 The name "eyeballvul" comes from Linus's law, the assertion that "given enough eyeballs, all bugs are shallow". eyeballvul will hopefully help with the deployment of large numbers of AI eyeballs, once they can see well enough.
 
@@ -137,19 +140,19 @@
 
 ## How it works
 To get into the details, Google's [osv.dev](https://osv.dev/) vulnerability database for open-source projects is used as input. Vulnerabilities are grouped by repository, and their affected versions are extracted. Finding the smallest set of commits that cover all the affected versions is an instance of the [hitting set problem](https://en.wikipedia.org/wiki/Set_cover_problem#Hitting_set_formulation). This is an NP-complete problem, but in practice Google's [CP-SAT](https://or-tools.github.io/docs/pdoc/ortools/sat/python/cp_model.html) solver handles it well in all the repos tested so far. First, the number of commits necessary to cover all the affected versions is minimized, then the sum of their dates is maximized (to get more recent commits, all other things equal). Repository total sizes and language breakdowns are computed at each commit using Github's [linguist](https://github.com/github-linguist/linguist), enabling filtering by repository size or language in downstream evaluations.
 
 ## Full example
 Let's see how this benchmark can be used in practice. Let's use `https://github.com/parisneo/lollms-webui` as an example repository (cherry-picked to have a reasonable size, and to have 6 easy vulnerabilities published later than March 29, 2024).
 ```python
->>> from eyeballvul import get_by_project, get_commits, get_revision
+>>> from eyeballvul import get_vulns, get_commits, get_revision
 >>> import json
->>> vulnerabilities = get_by_project("https://github.com/parisneo/lollms-webui")
->>> vulnerabilities_dicts = [v.to_dict() for v in vulnerabilities]
->>> print(json.dumps(vulnerabilities_dict, indent=2))
+>>> vulns = get_vulns(project="https://github.com/parisneo/lollms-webui")
+>>> vulns_dicts = [v.to_dict() for v in vulns]
+>>> print(json.dumps(vulns_dicts, indent=2))
 [
   {
     "id": "CVE-2024-1646",
     "published": "2024-04-16T00:15:09",
     "modified": "2024-04-17T01:16:41.423660",
     "details": "parisneo/lollms-webui is vulnerable to authentication bypass due to insufficient protection over sensitive endpoints. The application checks if the host parameter is not '0.0.0.0' to restrict access, which is inadequate when the application is bound to a specific interface, allowing unauthorized access to endpoints such as '/restart_program', '/update_software', '/check_update', '/start_recording', and '/stop_recording'. This vulnerability can lead to denial of service, unauthorized disabling or overriding of recordings, and potentially other impacts if certain features are enabled in the configuration.",
     "repo_url": "https://github.com/parisneo/lollms-webui",
@@ -434,7 +437,30 @@
 >>> recall
 0.5
 >>> f1 = 2 / (1 / precision + 1 / recall)
 >>> f1
 0.6666666666666666
 ```
 
+## FAQ
+### I'm GPU poor
+The sum of the repository sizes at each revision is around 75GB. Let's assume this translates to roughly 20B tokens. At $15/Mtok, you would be spending over $300k for a single pass on the benchmark if for example you used Claude 3 Opus. The solution: select a small random subset of the benchmark. A way to construct subsets that has nice properties is to use **commit hashes in alphabetical order**. If you work on a subset of the benchmark, please do that. For instance:
+```python
+>>> commits = get_commits()
+>>> commit_subset = sorted(commits)[:100]
+```
+
+To get a rough idea of the total size of different subsets, you could do:
+```python
+>>> total_size = sum(get_revision(commit).size for commit in commit_subset)
+```
+
+You may then further filter on reasonable criteria, such as repository size, language, or dates of vulnerabilities.
+
+### Where is the data?
+The data is kept in the [eyeballvul_data](https://github.com/timothee-chauvin/eyeballvul_data) repository. It is downloaded into `~/.cache/eyeballvul` when you run:
+```python
+from eyeballvul import download_data
+download_data()
+```
+The data sources (version-controlled OSV data, and eyeballvul cache) are kept in the [eyeballvul_data_sources](https://github.com/timothee-chauvin/eyeballvul_data_sources) repository.
+
```

