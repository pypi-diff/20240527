# Comparing `tmp/ragdaemon-0.7.1.tar.gz` & `tmp/ragdaemon-0.7.2.tar.gz`

## Comparing `ragdaemon-0.7.1.tar` & `ragdaemon-0.7.2.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0    63754 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/scratch.ipynb
--rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tutorial.ipynb
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/__main__.py
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/app.py
--rw-r--r--   0        0        0    10833 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/context.py
--rw-r--r--   0        0        0     7975 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/daemon.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/errors.py
--rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/get_paths.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/graph.py
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/locate.py
--rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/utils.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/annotators/__init__.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/annotators/base_annotator.py
--rw-r--r--   0        0        0    10688 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/annotators/call_graph.py
--rw-r--r--   0        0        0     6234 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/annotators/diff.py
--rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/annotators/hierarchy.py
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/annotators/layout_hierarchy.py
--rw-r--r--   0        0        0    12430 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/annotators/summarizer.py
--rw-r--r--   0        0        0     8410 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/annotators/chunker/__init__.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/annotators/chunker/chunk_astroid.py
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/annotators/chunker/chunk_line.py
--rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/annotators/chunker/chunk_llm.py
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/annotators/chunker/utils.py
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/database/__init__.py
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/database/chroma_database.py
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/database/database.py
--rw-r--r--   0        0        0     3573 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/database/lite_database.py
--rw-r--r--   0        0        0     6727 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/database/pg_database.py
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/prompts/call_graph.toml
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/prompts/chunk_llm.toml
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/prompts/locate.toml
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/prompts/summarizer/base.txt
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/prompts/summarizer/chunk.txt
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/prompts/summarizer/directory.txt
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/prompts/summarizer/file.txt
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/prompts/summarizer/root.txt
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/prompts/summarizer/user.txt
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/static/favicon.ico
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/static/js/controlPanel.js
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/static/js/main.js
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/static/js/three/camera.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/static/js/three/controls.js
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/static/js/three/edge.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/static/js/three/node.js
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/static/js/three/raycaster.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/static/js/three/renderer.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/static/js/three/scene.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/templates/index.html
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/templates/search_results.html
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/conftest.py
--rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/test_comments.py
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/test_context.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/test_daemon.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/test_database.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/test_get_paths.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/test_sample.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/annotators/test_chunker.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/annotators/test_diff.py
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/annotators/test_hierarchy.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/annotators/test_layout_hierarchy.py
--rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/annotators/test_summarizer.py
--rw-r--r--   0        0        0     8531 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/data/chunker_graph.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/data/context_message.txt
--rw-r--r--   0        0        0    10570 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/data/diff_graph.json
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/data/hard_to_chunk.txt
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/data/hierarchy_graph.json
--rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/data/layout_hierarchy_graph.json
--rw-r--r--   0        0        0    17442 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/data/summarizer_graph.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/sample/README.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/sample/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/sample/src/__init__.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/sample/src/interface.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/sample/src/operations.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/.gitignore
--rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/README.md
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    63754 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/scratch.ipynb
+-rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/tutorial.ipynb
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/__main__.py
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/app.py
+-rw-r--r--   0        0        0    10833 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/context.py
+-rw-r--r--   0        0        0     7975 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/daemon.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/errors.py
+-rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/get_paths.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/graph.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/locate.py
+-rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/utils.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/annotators/__init__.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/annotators/base_annotator.py
+-rw-r--r--   0        0        0    10688 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/annotators/call_graph.py
+-rw-r--r--   0        0        0     6234 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/annotators/diff.py
+-rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/annotators/hierarchy.py
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/annotators/layout_hierarchy.py
+-rw-r--r--   0        0        0    12492 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/annotators/summarizer.py
+-rw-r--r--   0        0        0     8410 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/annotators/chunker/__init__.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/annotators/chunker/chunk_astroid.py
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/annotators/chunker/chunk_line.py
+-rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/annotators/chunker/chunk_llm.py
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/annotators/chunker/utils.py
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/database/__init__.py
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/database/chroma_database.py
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/database/database.py
+-rw-r--r--   0        0        0     3573 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/database/lite_database.py
+-rw-r--r--   0        0        0     6727 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/database/pg_database.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/prompts/call_graph.toml
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/prompts/chunk_llm.toml
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/prompts/locate.toml
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/prompts/summarizer/base.txt
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/prompts/summarizer/chunk.txt
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/prompts/summarizer/directory.txt
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/prompts/summarizer/file.txt
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/prompts/summarizer/root.txt
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/prompts/summarizer/user.txt
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/static/favicon.ico
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/static/js/controlPanel.js
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/static/js/main.js
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/static/js/three/camera.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/static/js/three/controls.js
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/static/js/three/edge.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/static/js/three/node.js
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/static/js/three/raycaster.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/static/js/three/renderer.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/static/js/three/scene.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/templates/index.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/ragdaemon/templates/search_results.html
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/tests/conftest.py
+-rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/tests/test_comments.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/tests/test_context.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/tests/test_daemon.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/tests/test_database.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/tests/test_get_paths.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/tests/test_sample.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/tests/annotators/test_chunker.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/tests/annotators/test_diff.py
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/tests/annotators/test_hierarchy.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/tests/annotators/test_layout_hierarchy.py
+-rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/tests/annotators/test_summarizer.py
+-rw-r--r--   0        0        0     8531 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/tests/data/chunker_graph.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/tests/data/context_message.txt
+-rw-r--r--   0        0        0    10570 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/tests/data/diff_graph.json
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/tests/data/hard_to_chunk.txt
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/tests/data/hierarchy_graph.json
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/tests/data/layout_hierarchy_graph.json
+-rw-r--r--   0        0        0    17442 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/tests/data/summarizer_graph.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/tests/sample/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/tests/sample/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/tests/sample/src/__init__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/tests/sample/src/interface.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/tests/sample/src/operations.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/.gitignore
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/README.md
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 ragdaemon-0.7.2/PKG-INFO
```

### Comparing `ragdaemon-0.7.1/scratch.ipynb` & `ragdaemon-0.7.2/scratch.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/tutorial.ipynb` & `ragdaemon-0.7.2/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/.github/workflows/run-tests.yml` & `ragdaemon-0.7.2/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/app.py` & `ragdaemon-0.7.2/ragdaemon/app.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/context.py` & `ragdaemon-0.7.2/ragdaemon/context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/daemon.py` & `ragdaemon-0.7.2/ragdaemon/daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/get_paths.py` & `ragdaemon-0.7.2/ragdaemon/get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/graph.py` & `ragdaemon-0.7.2/ragdaemon/graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/locate.py` & `ragdaemon-0.7.2/ragdaemon/locate.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,53 +1,59 @@
 import asyncio
+from functools import partial
 
 from spice import Spice, SpiceMessages
 from spice.models import TextModel
 
 from ragdaemon.annotators.summarizer import get_leaf_nodes
 from ragdaemon.graph import KnowledgeGraph
 
 
+def validate(text: str, n_items: int) -> bool:
+    if not text:
+        return True
+    try:
+        ints = [int(i) for i in text.split(",")]
+    except ValueError:
+        return False
+
+    if not all(1 <= i <= n_items for i in ints):
+        print(f"OFFENDING TEXT: {text}")
+        return False
+
+    return True
+
+
 async def scan(
     nodes: list[str],
     graph: KnowledgeGraph,
     edge_type: str,
     spice_client: Spice,
     instruction: str,
     query: str,
     model: TextModel,
 ) -> list[str]:
     """Use an LLM to select relevant nodes from a list."""
     items = []
     for i, node in enumerate(nodes):
         children = get_leaf_nodes(graph, node, edge_type)
-        message = f"{i+1}: {node} | {len(children)} children: {', '.join(children[:10])}"
-        if len(children) > 10:
-            message += "..."
+        message = f"{i+1}: {node} ({len(children)} children)"
         items.append(message)
 
-    def validator(text: str) -> bool:
-        if not text:
-            return True
-        try:
-            _ = [int(i) for i in text.split(",")]
-            return True
-        except ValueError:
-            return False
-
+    validator = partial(validate, n_items=len(items))
     messages = SpiceMessages(spice_client)
     messages.add_system_prompt("locate.base")
     messages.add_user_prompt(
         "locate.user", instruction=instruction, query=query, items=items
     )
     response = await spice_client.get_response(
         messages=messages,
         model=model,
         validator=validator,
-        retries=1,
+        retries=2,
     )
 
     selected = response.text
     if not selected:
         return []
     return [nodes[int(i) - 1] for i in selected.split(",")]
```

### Comparing `ragdaemon-0.7.1/ragdaemon/utils.py` & `ragdaemon-0.7.2/ragdaemon/utils.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/annotators/__init__.py` & `ragdaemon-0.7.2/ragdaemon/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/annotators/base_annotator.py` & `ragdaemon-0.7.2/ragdaemon/annotators/base_annotator.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/annotators/call_graph.py` & `ragdaemon-0.7.2/ragdaemon/annotators/call_graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/annotators/diff.py` & `ragdaemon-0.7.2/ragdaemon/annotators/diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/annotators/hierarchy.py` & `ragdaemon-0.7.2/ragdaemon/annotators/hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/annotators/layout_hierarchy.py` & `ragdaemon-0.7.2/ragdaemon/annotators/layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/annotators/summarizer.py` & `ragdaemon-0.7.2/ragdaemon/annotators/summarizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,19 @@
     queue: deque = deque([node])
     leaf_nodes: List[str] = []
 
     while queue:
         current = queue.popleft()
         if current not in seen:
             seen.add(current)
-            children = [edge[1] for edge in graph.out_edges(current, data=True) if edge[-1].get("type") == edge_type]
+            children = [
+                edge[1]
+                for edge in graph.out_edges(current, data=True)
+                if edge[-1].get("type") == edge_type
+            ]
             if children:
                 queue.extend(children)
             else:
                 leaf_nodes.append(current)
 
     return leaf_nodes
```

### Comparing `ragdaemon-0.7.1/ragdaemon/annotators/chunker/__init__.py` & `ragdaemon-0.7.2/ragdaemon/annotators/chunker/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/annotators/chunker/chunk_astroid.py` & `ragdaemon-0.7.2/ragdaemon/annotators/chunker/chunk_astroid.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/annotators/chunker/chunk_line.py` & `ragdaemon-0.7.2/ragdaemon/annotators/chunker/chunk_line.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/annotators/chunker/chunk_llm.py` & `ragdaemon-0.7.2/ragdaemon/annotators/chunker/chunk_llm.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/annotators/chunker/utils.py` & `ragdaemon-0.7.2/ragdaemon/annotators/chunker/utils.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/database/__init__.py` & `ragdaemon-0.7.2/ragdaemon/database/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/database/chroma_database.py` & `ragdaemon-0.7.2/ragdaemon/database/chroma_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/database/database.py` & `ragdaemon-0.7.2/ragdaemon/database/database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/database/lite_database.py` & `ragdaemon-0.7.2/ragdaemon/database/lite_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/database/pg_database.py` & `ragdaemon-0.7.2/ragdaemon/database/pg_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/prompts/call_graph.toml` & `ragdaemon-0.7.2/ragdaemon/prompts/call_graph.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/prompts/chunk_llm.toml` & `ragdaemon-0.7.2/ragdaemon/prompts/chunk_llm.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/prompts/locate.toml` & `ragdaemon-0.7.2/ragdaemon/prompts/locate.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 base="""\
 Read the user's query and item summaries, and return a list of indices of items which fulfill their instructions.
 Respond with a comma-separated string of integers and nothing else.
+Take the number at the beginning of each line as the index.
+If no items are relevant, return an empty string. Do NOT return 0.
 
 Unless explicitly instructed otherwise:
 * Err on the side of inclusivity. Especially with directories - if there's a chance it may be relevant, include it.
 * You include no items, one item or multiple items. You decide what is relevant.
 
 EXAMPLE:
 --------------------------------------------------------------------------------
```

### Comparing `ragdaemon-0.7.1/ragdaemon/prompts/summarizer/base.txt` & `ragdaemon-0.7.2/ragdaemon/prompts/summarizer/base.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/prompts/summarizer/chunk.txt` & `ragdaemon-0.7.2/ragdaemon/prompts/summarizer/chunk.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/prompts/summarizer/directory.txt` & `ragdaemon-0.7.2/ragdaemon/prompts/summarizer/directory.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/prompts/summarizer/file.txt` & `ragdaemon-0.7.2/ragdaemon/prompts/summarizer/file.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/prompts/summarizer/root.txt` & `ragdaemon-0.7.2/ragdaemon/prompts/summarizer/root.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/static/favicon.ico` & `ragdaemon-0.7.2/ragdaemon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/static/js/controlPanel.js` & `ragdaemon-0.7.2/ragdaemon/static/js/controlPanel.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/static/js/main.js` & `ragdaemon-0.7.2/ragdaemon/static/js/main.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/static/js/three/edge.js` & `ragdaemon-0.7.2/ragdaemon/static/js/three/edge.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/static/js/three/node.js` & `ragdaemon-0.7.2/ragdaemon/static/js/three/node.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/static/js/three/raycaster.js` & `ragdaemon-0.7.2/ragdaemon/static/js/three/raycaster.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/ragdaemon/templates/index.html` & `ragdaemon-0.7.2/ragdaemon/templates/index.html`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/tests/conftest.py` & `ragdaemon-0.7.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/tests/test_comments.py` & `ragdaemon-0.7.2/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/tests/test_context.py` & `ragdaemon-0.7.2/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/tests/test_daemon.py` & `ragdaemon-0.7.2/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/tests/test_get_paths.py` & `ragdaemon-0.7.2/tests/test_get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/tests/test_sample.py` & `ragdaemon-0.7.2/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/tests/annotators/test_chunker.py` & `ragdaemon-0.7.2/tests/annotators/test_chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/tests/annotators/test_diff.py` & `ragdaemon-0.7.2/tests/annotators/test_diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/tests/annotators/test_hierarchy.py` & `ragdaemon-0.7.2/tests/annotators/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/tests/annotators/test_layout_hierarchy.py` & `ragdaemon-0.7.2/tests/annotators/test_layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/tests/annotators/test_summarizer.py` & `ragdaemon-0.7.2/tests/annotators/test_summarizer.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/tests/data/chunker_graph.json` & `ragdaemon-0.7.2/tests/data/chunker_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/tests/data/context_message.txt` & `ragdaemon-0.7.2/tests/data/context_message.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/tests/data/diff_graph.json` & `ragdaemon-0.7.2/tests/data/diff_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/tests/data/hard_to_chunk.txt` & `ragdaemon-0.7.2/tests/data/hard_to_chunk.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/tests/data/hierarchy_graph.json` & `ragdaemon-0.7.2/tests/data/hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/tests/data/layout_hierarchy_graph.json` & `ragdaemon-0.7.2/tests/data/layout_hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/tests/data/summarizer_graph.json` & `ragdaemon-0.7.2/tests/data/summarizer_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/tests/sample/src/interface.py` & `ragdaemon-0.7.2/tests/sample/src/interface.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/LICENSE` & `ragdaemon-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/README.md` & `ragdaemon-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.1/pyproject.toml` & `ragdaemon-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages=["ragdaemon"]
 
 [project]
 name = "ragdaemon"
-version = "0.7.1"
+version = "0.7.2"
 description = "Generate and render a call graph for a Python project."
 readme = "README.md"
 dependencies = [
     "astroid==3.2.2",
     "chromadb==0.4.24",
     "dict2xml==1.7.5",
     "fastapi==0.109.2",
```

### Comparing `ragdaemon-0.7.1/PKG-INFO` & `ragdaemon-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragdaemon
-Version: 0.7.1
+Version: 0.7.2
 Summary: Generate and render a call graph for a Python project.
 Project-URL: Homepage, https://github.com/AbanteAI/ragdaemon
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

