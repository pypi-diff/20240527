# Comparing `tmp/gpt-researcher-0.5.4.tar.gz` & `tmp/gpt-researcher-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-researcher-0.5.4.tar", last modified: Sat May 25 06:45:01 2024, max compression
+gzip compressed data, was "gpt-researcher-0.6.0.tar", last modified: Mon May 27 07:04:25 2024, max compression
```

## Comparing `gpt-researcher-0.5.4.tar` & `gpt-researcher-0.6.0.tar`

### file list

```diff
@@ -1,106 +1,121 @@
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.119402 gpt-researcher-0.5.4/
--rw-r--r--   0 assafel    (501) staff       (20)     1069 2024-04-22 11:21:41.000000 gpt-researcher-0.5.4/LICENSE
--rw-r--r--   0 assafel    (501) staff       (20)    13156 2024-05-25 06:45:01.118579 gpt-researcher-0.5.4/PKG-INFO
--rw-r--r--   0 assafel    (501) staff       (20)    12433 2024-05-25 06:33:59.000000 gpt-researcher-0.5.4/README.md
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.061152 gpt-researcher-0.5.4/backend/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.4/backend/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.062386 gpt-researcher-0.5.4/backend/report_type/
--rw-r--r--   0 assafel    (501) staff       (20)      165 2024-04-22 11:21:41.000000 gpt-researcher-0.5.4/backend/report_type/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.064471 gpt-researcher-0.5.4/backend/report_type/basic_report/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.4/backend/report_type/basic_report/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      859 2024-05-20 06:53:38.000000 gpt-researcher-0.5.4/backend/report_type/basic_report/basic_report.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.066075 gpt-researcher-0.5.4/backend/report_type/detailed_report/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.4/backend/report_type/detailed_report/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     6151 2024-05-20 06:53:38.000000 gpt-researcher-0.5.4/backend/report_type/detailed_report/detailed_report.py
--rw-r--r--   0 assafel    (501) staff       (20)     2405 2024-05-20 06:53:38.000000 gpt-researcher-0.5.4/backend/server.py
--rw-r--r--   0 assafel    (501) staff       (20)     2720 2024-05-20 05:44:03.000000 gpt-researcher-0.5.4/backend/utils.py
--rw-r--r--   0 assafel    (501) staff       (20)     2986 2024-05-20 06:53:38.000000 gpt-researcher-0.5.4/backend/websocket_manager.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.067197 gpt-researcher-0.5.4/gpt_researcher/
--rw-r--r--   0 assafel    (501) staff       (20)      100 2023-11-13 18:29:19.000000 gpt-researcher-0.5.4/gpt_researcher/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.073089 gpt-researcher-0.5.4/gpt_researcher/config/
--rw-r--r--   0 assafel    (501) staff       (20)       48 2023-11-13 18:29:19.000000 gpt-researcher-0.5.4/gpt_researcher/config/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2388 2024-05-20 06:53:38.000000 gpt-researcher-0.5.4/gpt_researcher/config/config.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.076362 gpt-researcher-0.5.4/gpt_researcher/context/
--rw-r--r--   0 assafel    (501) staff       (20)      140 2023-11-19 07:01:11.000000 gpt-researcher-0.5.4/gpt_researcher/context/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1796 2024-05-09 12:40:13.000000 gpt-researcher-0.5.4/gpt_researcher/context/compression.py
--rw-r--r--   0 assafel    (501) staff       (20)      801 2023-11-19 07:01:11.000000 gpt-researcher-0.5.4/gpt_researcher/context/retriever.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.078599 gpt-researcher-0.5.4/gpt_researcher/document/
--rw-r--r--   0 assafel    (501) staff       (20)       67 2024-05-20 06:53:38.000000 gpt-researcher-0.5.4/gpt_researcher/document/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2229 2024-05-20 06:53:38.000000 gpt-researcher-0.5.4/gpt_researcher/document/document.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.079623 gpt-researcher-0.5.4/gpt_researcher/llm_provider/
--rw-r--r--   0 assafel    (501) staff       (20)      282 2024-05-25 06:42:57.000000 gpt-researcher-0.5.4/gpt_researcher/llm_provider/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.081008 gpt-researcher-0.5.4/gpt_researcher/llm_provider/azureopenai/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.4/gpt_researcher/llm_provider/azureopenai/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     3068 2024-04-22 11:21:41.000000 gpt-researcher-0.5.4/gpt_researcher/llm_provider/azureopenai/azureopenai.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.082880 gpt-researcher-0.5.4/gpt_researcher/llm_provider/google/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.4/gpt_researcher/llm_provider/google/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     3670 2024-04-22 11:21:41.000000 gpt-researcher-0.5.4/gpt_researcher/llm_provider/google/google.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.084643 gpt-researcher-0.5.4/gpt_researcher/llm_provider/groq/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-05-25 06:42:57.000000 gpt-researcher-0.5.4/gpt_researcher/llm_provider/groq/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2074 2024-05-25 06:42:57.000000 gpt-researcher-0.5.4/gpt_researcher/llm_provider/groq/groq.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.085999 gpt-researcher-0.5.4/gpt_researcher/llm_provider/openai/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.4/gpt_researcher/llm_provider/openai/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2457 2024-05-21 05:23:12.000000 gpt-researcher-0.5.4/gpt_researcher/llm_provider/openai/openai.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.089506 gpt-researcher-0.5.4/gpt_researcher/master/
--rw-r--r--   0 assafel    (501) staff       (20)       61 2023-11-13 18:29:19.000000 gpt-researcher-0.5.4/gpt_researcher/master/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)    10219 2024-05-21 05:18:28.000000 gpt-researcher-0.5.4/gpt_researcher/master/agent.py
--rw-r--r--   0 assafel    (501) staff       (20)    12330 2024-05-25 06:33:59.000000 gpt-researcher-0.5.4/gpt_researcher/master/functions.py
--rw-r--r--   0 assafel    (501) staff       (20)    14933 2024-05-25 06:42:57.000000 gpt-researcher-0.5.4/gpt_researcher/master/prompts.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.091342 gpt-researcher-0.5.4/gpt_researcher/memory/
--rw-r--r--   0 assafel    (501) staff       (20)       31 2023-11-19 07:01:11.000000 gpt-researcher-0.5.4/gpt_researcher/memory/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1697 2024-05-25 06:42:57.000000 gpt-researcher-0.5.4/gpt_researcher/memory/embeddings.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.091951 gpt-researcher-0.5.4/gpt_researcher/retrievers/
--rw-r--r--   0 assafel    (501) staff       (20)      445 2024-05-25 06:33:59.000000 gpt-researcher-0.5.4/gpt_researcher/retrievers/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.093279 gpt-researcher-0.5.4/gpt_researcher/retrievers/bing/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-08 11:24:31.000000 gpt-researcher-0.5.4/gpt_researcher/retrievers/bing/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2240 2023-12-08 11:24:31.000000 gpt-researcher-0.5.4/gpt_researcher/retrievers/bing/bing.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.094991 gpt-researcher-0.5.4/gpt_researcher/retrievers/duckduckgo/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.4/gpt_researcher/retrievers/duckduckgo/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      479 2024-05-06 05:46:56.000000 gpt-researcher-0.5.4/gpt_researcher/retrievers/duckduckgo/duckduckgo.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.096614 gpt-researcher-0.5.4/gpt_researcher/retrievers/google/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.4/gpt_researcher/retrievers/google/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2535 2023-11-19 07:01:11.000000 gpt-researcher-0.5.4/gpt_researcher/retrievers/google/google.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.098303 gpt-researcher-0.5.4/gpt_researcher/retrievers/searx/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.4/gpt_researcher/retrievers/searx/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1294 2024-04-22 11:21:41.000000 gpt-researcher-0.5.4/gpt_researcher/retrievers/searx/searx.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.100010 gpt-researcher-0.5.4/gpt_researcher/retrievers/serpapi/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.4/gpt_researcher/retrievers/serpapi/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2418 2024-05-16 08:47:07.000000 gpt-researcher-0.5.4/gpt_researcher/retrievers/serpapi/serpapi.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.101550 gpt-researcher-0.5.4/gpt_researcher/retrievers/serper/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.4/gpt_researcher/retrievers/serper/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2149 2024-05-16 08:47:07.000000 gpt-researcher-0.5.4/gpt_researcher/retrievers/serper/serper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.103031 gpt-researcher-0.5.4/gpt_researcher/retrievers/tavily_search/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.4/gpt_researcher/retrievers/tavily_search/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1926 2024-05-25 06:33:59.000000 gpt-researcher-0.5.4/gpt_researcher/retrievers/tavily_search/tavily_search.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.104624 gpt-researcher-0.5.4/gpt_researcher/scraper/
--rw-r--r--   0 assafel    (501) staff       (20)      398 2024-03-17 08:29:46.000000 gpt-researcher-0.5.4/gpt_researcher/scraper/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.106019 gpt-researcher-0.5.4/gpt_researcher/scraper/arxiv/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.5.4/gpt_researcher/scraper/arxiv/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      762 2024-03-12 13:09:58.000000 gpt-researcher-0.5.4/gpt_researcher/scraper/arxiv/arxiv.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.107625 gpt-researcher-0.5.4/gpt_researcher/scraper/beautiful_soup/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.5.4/gpt_researcher/scraper/beautiful_soup/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1992 2024-03-12 13:09:58.000000 gpt-researcher-0.5.4/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.109277 gpt-researcher-0.5.4/gpt_researcher/scraper/newspaper/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.5.4/gpt_researcher/scraper/newspaper/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1312 2024-03-12 13:09:58.000000 gpt-researcher-0.5.4/gpt_researcher/scraper/newspaper/newspaper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.110959 gpt-researcher-0.5.4/gpt_researcher/scraper/pymupdf/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.5.4/gpt_researcher/scraper/pymupdf/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      640 2024-03-12 13:09:58.000000 gpt-researcher-0.5.4/gpt_researcher/scraper/pymupdf/pymupdf.py
--rw-r--r--   0 assafel    (501) staff       (20)     3111 2024-03-17 08:29:46.000000 gpt-researcher-0.5.4/gpt_researcher/scraper/scraper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.112711 gpt-researcher-0.5.4/gpt_researcher/scraper/web_base_loader/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.5.4/gpt_researcher/scraper/web_base_loader/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1074 2024-03-12 13:09:58.000000 gpt-researcher-0.5.4/gpt_researcher/scraper/web_base_loader/web_base_loader.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.116835 gpt-researcher-0.5.4/gpt_researcher/utils/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.4/gpt_researcher/utils/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      341 2024-05-20 06:53:38.000000 gpt-researcher-0.5.4/gpt_researcher/utils/enum.py
--rw-r--r--   0 assafel    (501) staff       (20)     5323 2024-05-25 06:42:57.000000 gpt-researcher-0.5.4/gpt_researcher/utils/llm.py
--rw-r--r--   0 assafel    (501) staff       (20)      216 2024-04-22 11:21:41.000000 gpt-researcher-0.5.4/gpt_researcher/utils/validators.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.071230 gpt-researcher-0.5.4/gpt_researcher.egg-info/
--rw-r--r--   0 assafel    (501) staff       (20)    13156 2024-05-25 06:45:00.000000 gpt-researcher-0.5.4/gpt_researcher.egg-info/PKG-INFO
--rw-r--r--   0 assafel    (501) staff       (20)     2782 2024-05-25 06:45:00.000000 gpt-researcher-0.5.4/gpt_researcher.egg-info/SOURCES.txt
--rw-r--r--   0 assafel    (501) staff       (20)        1 2024-05-25 06:45:00.000000 gpt-researcher-0.5.4/gpt_researcher.egg-info/dependency_links.txt
--rw-r--r--   0 assafel    (501) staff       (20)      392 2024-05-25 06:45:00.000000 gpt-researcher-0.5.4/gpt_researcher.egg-info/requires.txt
--rw-r--r--   0 assafel    (501) staff       (20)       23 2024-05-25 06:45:00.000000 gpt-researcher-0.5.4/gpt_researcher.egg-info/top_level.txt
--rw-r--r--   0 assafel    (501) staff       (20)     1182 2024-05-20 06:53:38.000000 gpt-researcher-0.5.4/pyproject.toml
--rw-r--r--   0 assafel    (501) staff       (20)       38 2024-05-25 06:45:01.119677 gpt-researcher-0.5.4/setup.cfg
--rw-r--r--   0 assafel    (501) staff       (20)     1176 2024-05-25 06:42:57.000000 gpt-researcher-0.5.4/setup.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.057073 gpt-researcher-0.6.0/
+-rw-r--r--   0 assafel    (501) staff       (20)     1069 2024-04-22 11:21:41.000000 gpt-researcher-0.6.0/LICENSE
+-rw-r--r--   0 assafel    (501) staff       (20)    13395 2024-05-27 07:04:25.056505 gpt-researcher-0.6.0/PKG-INFO
+-rw-r--r--   0 assafel    (501) staff       (20)    12672 2024-05-26 12:12:16.000000 gpt-researcher-0.6.0/README.md
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:24.996781 gpt-researcher-0.6.0/backend/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.6.0/backend/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:24.997722 gpt-researcher-0.6.0/backend/report_type/
+-rw-r--r--   0 assafel    (501) staff       (20)      165 2024-04-22 11:21:41.000000 gpt-researcher-0.6.0/backend/report_type/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:24.999100 gpt-researcher-0.6.0/backend/report_type/basic_report/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.6.0/backend/report_type/basic_report/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      859 2024-05-20 06:53:38.000000 gpt-researcher-0.6.0/backend/report_type/basic_report/basic_report.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.000600 gpt-researcher-0.6.0/backend/report_type/detailed_report/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.6.0/backend/report_type/detailed_report/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     6151 2024-05-20 06:53:38.000000 gpt-researcher-0.6.0/backend/report_type/detailed_report/detailed_report.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2405 2024-05-20 06:53:38.000000 gpt-researcher-0.6.0/backend/server.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2720 2024-05-20 05:44:03.000000 gpt-researcher-0.6.0/backend/utils.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2986 2024-05-20 06:53:38.000000 gpt-researcher-0.6.0/backend/websocket_manager.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.001717 gpt-researcher-0.6.0/gpt_researcher/
+-rw-r--r--   0 assafel    (501) staff       (20)      100 2023-11-13 18:29:19.000000 gpt-researcher-0.6.0/gpt_researcher/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.006260 gpt-researcher-0.6.0/gpt_researcher/config/
+-rw-r--r--   0 assafel    (501) staff       (20)       48 2023-11-13 18:29:19.000000 gpt-researcher-0.6.0/gpt_researcher/config/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2454 2024-05-27 05:45:21.000000 gpt-researcher-0.6.0/gpt_researcher/config/config.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.008963 gpt-researcher-0.6.0/gpt_researcher/context/
+-rw-r--r--   0 assafel    (501) staff       (20)      140 2023-11-19 07:01:11.000000 gpt-researcher-0.6.0/gpt_researcher/context/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1796 2024-05-09 12:40:13.000000 gpt-researcher-0.6.0/gpt_researcher/context/compression.py
+-rw-r--r--   0 assafel    (501) staff       (20)      801 2023-11-19 07:01:11.000000 gpt-researcher-0.6.0/gpt_researcher/context/retriever.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.010868 gpt-researcher-0.6.0/gpt_researcher/document/
+-rw-r--r--   0 assafel    (501) staff       (20)       67 2024-05-20 06:53:38.000000 gpt-researcher-0.6.0/gpt_researcher/document/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2229 2024-05-20 06:53:38.000000 gpt-researcher-0.6.0/gpt_researcher/document/document.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.011739 gpt-researcher-0.6.0/gpt_researcher/llm_provider/
+-rw-r--r--   0 assafel    (501) staff       (20)      644 2024-05-27 06:43:44.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.012729 gpt-researcher-0.6.0/gpt_researcher/llm_provider/anthropic/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-05-27 06:15:55.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/anthropic/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2116 2024-05-27 06:42:16.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/anthropic/anthropic.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.013967 gpt-researcher-0.6.0/gpt_researcher/llm_provider/azureopenai/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/azureopenai/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3068 2024-04-22 11:21:41.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/azureopenai/azureopenai.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.016825 gpt-researcher-0.6.0/gpt_researcher/llm_provider/google/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/google/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3670 2024-04-22 11:21:41.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/google/google.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.018732 gpt-researcher-0.6.0/gpt_researcher/llm_provider/groq/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-05-26 12:12:16.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/groq/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2074 2024-05-26 12:12:16.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/groq/groq.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.020780 gpt-researcher-0.6.0/gpt_researcher/llm_provider/huggingface/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-05-27 06:16:19.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/huggingface/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2130 2024-05-27 06:41:57.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/huggingface/huggingface.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.021988 gpt-researcher-0.6.0/gpt_researcher/llm_provider/mistral/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-05-27 06:16:34.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/mistral/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2108 2024-05-27 06:42:02.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/mistral/mistral.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.023201 gpt-researcher-0.6.0/gpt_researcher/llm_provider/ollama/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-05-27 05:45:21.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/ollama/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2037 2024-05-27 05:45:21.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/ollama/ollama.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.024969 gpt-researcher-0.6.0/gpt_researcher/llm_provider/openai/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/openai/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2457 2024-05-21 05:23:12.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/openai/openai.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.026484 gpt-researcher-0.6.0/gpt_researcher/llm_provider/together/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-05-27 06:36:44.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/together/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2106 2024-05-27 06:42:09.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/together/together.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.030226 gpt-researcher-0.6.0/gpt_researcher/master/
+-rw-r--r--   0 assafel    (501) staff       (20)       61 2023-11-13 18:29:19.000000 gpt-researcher-0.6.0/gpt_researcher/master/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)    10219 2024-05-21 05:18:28.000000 gpt-researcher-0.6.0/gpt_researcher/master/agent.py
+-rw-r--r--   0 assafel    (501) staff       (20)    12330 2024-05-26 12:12:16.000000 gpt-researcher-0.6.0/gpt_researcher/master/functions.py
+-rw-r--r--   0 assafel    (501) staff       (20)    14933 2024-05-25 06:42:57.000000 gpt-researcher-0.6.0/gpt_researcher/master/prompts.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.032146 gpt-researcher-0.6.0/gpt_researcher/memory/
+-rw-r--r--   0 assafel    (501) staff       (20)       31 2023-11-19 07:01:11.000000 gpt-researcher-0.6.0/gpt_researcher/memory/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1721 2024-05-27 05:45:21.000000 gpt-researcher-0.6.0/gpt_researcher/memory/embeddings.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.033049 gpt-researcher-0.6.0/gpt_researcher/retrievers/
+-rw-r--r--   0 assafel    (501) staff       (20)      445 2024-05-26 12:12:16.000000 gpt-researcher-0.6.0/gpt_researcher/retrievers/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.034685 gpt-researcher-0.6.0/gpt_researcher/retrievers/bing/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-08 11:24:31.000000 gpt-researcher-0.6.0/gpt_researcher/retrievers/bing/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2240 2023-12-08 11:24:31.000000 gpt-researcher-0.6.0/gpt_researcher/retrievers/bing/bing.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.036144 gpt-researcher-0.6.0/gpt_researcher/retrievers/duckduckgo/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.6.0/gpt_researcher/retrievers/duckduckgo/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      479 2024-05-06 05:46:56.000000 gpt-researcher-0.6.0/gpt_researcher/retrievers/duckduckgo/duckduckgo.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.037971 gpt-researcher-0.6.0/gpt_researcher/retrievers/google/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.6.0/gpt_researcher/retrievers/google/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2535 2023-11-19 07:01:11.000000 gpt-researcher-0.6.0/gpt_researcher/retrievers/google/google.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.039402 gpt-researcher-0.6.0/gpt_researcher/retrievers/searx/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.6.0/gpt_researcher/retrievers/searx/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1294 2024-04-22 11:21:41.000000 gpt-researcher-0.6.0/gpt_researcher/retrievers/searx/searx.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.040865 gpt-researcher-0.6.0/gpt_researcher/retrievers/serpapi/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.6.0/gpt_researcher/retrievers/serpapi/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2418 2024-05-16 08:47:07.000000 gpt-researcher-0.6.0/gpt_researcher/retrievers/serpapi/serpapi.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.042340 gpt-researcher-0.6.0/gpt_researcher/retrievers/serper/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.6.0/gpt_researcher/retrievers/serper/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2149 2024-05-16 08:47:07.000000 gpt-researcher-0.6.0/gpt_researcher/retrievers/serper/serper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.043728 gpt-researcher-0.6.0/gpt_researcher/retrievers/tavily_search/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.6.0/gpt_researcher/retrievers/tavily_search/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1926 2024-05-26 12:12:16.000000 gpt-researcher-0.6.0/gpt_researcher/retrievers/tavily_search/tavily_search.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.045598 gpt-researcher-0.6.0/gpt_researcher/scraper/
+-rw-r--r--   0 assafel    (501) staff       (20)      398 2024-03-17 08:29:46.000000 gpt-researcher-0.6.0/gpt_researcher/scraper/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.046879 gpt-researcher-0.6.0/gpt_researcher/scraper/arxiv/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.6.0/gpt_researcher/scraper/arxiv/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      762 2024-03-12 13:09:58.000000 gpt-researcher-0.6.0/gpt_researcher/scraper/arxiv/arxiv.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.048402 gpt-researcher-0.6.0/gpt_researcher/scraper/beautiful_soup/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.6.0/gpt_researcher/scraper/beautiful_soup/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1992 2024-03-12 13:09:58.000000 gpt-researcher-0.6.0/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.049886 gpt-researcher-0.6.0/gpt_researcher/scraper/newspaper/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.6.0/gpt_researcher/scraper/newspaper/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1312 2024-03-12 13:09:58.000000 gpt-researcher-0.6.0/gpt_researcher/scraper/newspaper/newspaper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.051121 gpt-researcher-0.6.0/gpt_researcher/scraper/pymupdf/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.6.0/gpt_researcher/scraper/pymupdf/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      640 2024-03-12 13:09:58.000000 gpt-researcher-0.6.0/gpt_researcher/scraper/pymupdf/pymupdf.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3111 2024-03-17 08:29:46.000000 gpt-researcher-0.6.0/gpt_researcher/scraper/scraper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.052432 gpt-researcher-0.6.0/gpt_researcher/scraper/web_base_loader/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.6.0/gpt_researcher/scraper/web_base_loader/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1074 2024-03-12 13:09:58.000000 gpt-researcher-0.6.0/gpt_researcher/scraper/web_base_loader/web_base_loader.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.055461 gpt-researcher-0.6.0/gpt_researcher/utils/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.6.0/gpt_researcher/utils/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      341 2024-05-20 06:53:38.000000 gpt-researcher-0.6.0/gpt_researcher/utils/enum.py
+-rw-r--r--   0 assafel    (501) staff       (20)     6062 2024-05-27 06:45:30.000000 gpt-researcher-0.6.0/gpt_researcher/utils/llm.py
+-rw-r--r--   0 assafel    (501) staff       (20)      216 2024-04-22 11:21:41.000000 gpt-researcher-0.6.0/gpt_researcher/utils/validators.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.004843 gpt-researcher-0.6.0/gpt_researcher.egg-info/
+-rw-r--r--   0 assafel    (501) staff       (20)    13395 2024-05-27 07:04:24.000000 gpt-researcher-0.6.0/gpt_researcher.egg-info/PKG-INFO
+-rw-r--r--   0 assafel    (501) staff       (20)     3275 2024-05-27 07:04:24.000000 gpt-researcher-0.6.0/gpt_researcher.egg-info/SOURCES.txt
+-rw-r--r--   0 assafel    (501) staff       (20)        1 2024-05-27 07:04:24.000000 gpt-researcher-0.6.0/gpt_researcher.egg-info/dependency_links.txt
+-rw-r--r--   0 assafel    (501) staff       (20)      458 2024-05-27 07:04:24.000000 gpt-researcher-0.6.0/gpt_researcher.egg-info/requires.txt
+-rw-r--r--   0 assafel    (501) staff       (20)       23 2024-05-27 07:04:24.000000 gpt-researcher-0.6.0/gpt_researcher.egg-info/top_level.txt
+-rw-r--r--   0 assafel    (501) staff       (20)     1182 2024-05-20 06:53:38.000000 gpt-researcher-0.6.0/pyproject.toml
+-rw-r--r--   0 assafel    (501) staff       (20)       38 2024-05-27 07:04:25.057226 gpt-researcher-0.6.0/setup.cfg
+-rw-r--r--   0 assafel    (501) staff       (20)     1176 2024-05-27 07:04:02.000000 gpt-researcher-0.6.0/setup.py
```

### Comparing `gpt-researcher-0.5.4/LICENSE` & `gpt-researcher-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.4/PKG-INFO` & `gpt-researcher-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-researcher
-Version: 0.5.4
+Version: 0.6.0
 Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
 Home-page: https://github.com/assafelovic/gpt-researcher
 Author: Assaf Elovic
 Author-email: assaf.elovic@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -12,15 +12,19 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# 🔎 GPT Researcher
+<h1 style="display: flex; align-items: center; gap: 10px;">
+  <img src="https://github.com/assafelovic/gpt-researcher/assets/13554167/a45bac7c-092c-42e5-8eb6-69acbf20dde5" alt="Logo" width="25">
+  GPT Researcher
+</h1>
+
 [![Official Website](https://img.shields.io/badge/Official%20Website-gptr.dev-teal?style=for-the-badge&logo=world&logoColor=white)](https://gptr.dev)
 [![Official Website](https://img.shields.io/badge/Documentation-GPTR-pink?logo=googledocs&logoColor=white&style=for-the-badge)](https://docs.gptr.dev)
 [![Discord Follow](https://dcbadge.vercel.app/api/server/SK3KKuSD?style=for-the-badge)](https://discord.gg/SK3KKuSD)
 
 [![GitHub Repo stars](https://img.shields.io/github/stars/assafelovic/gpt-researcher?style=social)](https://github.com/assafelovic/gpt-researcher)
 [![Twitter Follow](https://img.shields.io/twitter/follow/assaf_elovic?style=social)](https://twitter.com/assaf_elovic)
 [![PyPI version](https://badge.fury.io/py/gpt-researcher.svg)](https://badge.fury.io/py/gpt-researcher)
@@ -51,18 +55,19 @@
 https://github.com/assafelovic/gpt-researcher/assets/13554167/dd6cf08f-b31e-40c6-9907-1915f52a7110
 
 ## Architecture
 The main idea is to run "planner" and "execution" agents, whereas the planner generates questions to research, and the execution agents seek the most related information based on each generated research question. Finally, the planner filters and aggregates all related information and creates a research report. <br /> <br /> 
 The agents leverage both `gpt3.5-turbo` and `gpt-4o` (128K context) to complete a research task. We optimize for costs using each only when necessary. **The average research task takes around 3 minutes to complete, and costs ~$0.1.**
 
 <div align="center">
-<img align="center" height="500" src="https://cowriter-images.s3.amazonaws.com/architecture.png">
+<img align="center" height="600" src="https://github.com/assafelovic/gpt-researcher/assets/13554167/4ac896fd-63ab-4b77-9688-ff62aafcc527">
 </div>
 
 
+
 More specifically:
 * Create a domain specific agent based on research query or task.
 * Generate a set of research questions that together form an objective opinion on any given task. 
 * For each research question, trigger a crawler agent that scrapes online resources for information relevant to the given task.
 * For each scraped resources, summarize based on relevant information and keep track of its sources.
 * Finally, filter and aggregate all summarized sources and generate a final research report.
```

### Comparing `gpt-researcher-0.5.4/README.md` & `gpt-researcher-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-# 🔎 GPT Researcher
+<h1 style="display: flex; align-items: center; gap: 10px;">
+  <img src="https://github.com/assafelovic/gpt-researcher/assets/13554167/a45bac7c-092c-42e5-8eb6-69acbf20dde5" alt="Logo" width="25">
+  GPT Researcher
+</h1>
+
 [![Official Website](https://img.shields.io/badge/Official%20Website-gptr.dev-teal?style=for-the-badge&logo=world&logoColor=white)](https://gptr.dev)
 [![Official Website](https://img.shields.io/badge/Documentation-GPTR-pink?logo=googledocs&logoColor=white&style=for-the-badge)](https://docs.gptr.dev)
 [![Discord Follow](https://dcbadge.vercel.app/api/server/SK3KKuSD?style=for-the-badge)](https://discord.gg/SK3KKuSD)
 
 [![GitHub Repo stars](https://img.shields.io/github/stars/assafelovic/gpt-researcher?style=social)](https://github.com/assafelovic/gpt-researcher)
 [![Twitter Follow](https://img.shields.io/twitter/follow/assaf_elovic?style=social)](https://twitter.com/assaf_elovic)
 [![PyPI version](https://badge.fury.io/py/gpt-researcher.svg)](https://badge.fury.io/py/gpt-researcher)
@@ -33,18 +37,19 @@
 https://github.com/assafelovic/gpt-researcher/assets/13554167/dd6cf08f-b31e-40c6-9907-1915f52a7110
 
 ## Architecture
 The main idea is to run "planner" and "execution" agents, whereas the planner generates questions to research, and the execution agents seek the most related information based on each generated research question. Finally, the planner filters and aggregates all related information and creates a research report. <br /> <br /> 
 The agents leverage both `gpt3.5-turbo` and `gpt-4o` (128K context) to complete a research task. We optimize for costs using each only when necessary. **The average research task takes around 3 minutes to complete, and costs ~$0.1.**
 
 <div align="center">
-<img align="center" height="500" src="https://cowriter-images.s3.amazonaws.com/architecture.png">
+<img align="center" height="600" src="https://github.com/assafelovic/gpt-researcher/assets/13554167/4ac896fd-63ab-4b77-9688-ff62aafcc527">
 </div>
 
 
+
 More specifically:
 * Create a domain specific agent based on research query or task.
 * Generate a set of research questions that together form an objective opinion on any given task. 
 * For each research question, trigger a crawler agent that scrapes online resources for information relevant to the given task.
 * For each scraped resources, summarize based on relevant information and keep track of its sources.
 * Finally, filter and aggregate all summarized sources and generate a final research report.
```

### Comparing `gpt-researcher-0.5.4/backend/report_type/basic_report/basic_report.py` & `gpt-researcher-0.6.0/backend/report_type/basic_report/basic_report.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.4/backend/report_type/detailed_report/detailed_report.py` & `gpt-researcher-0.6.0/backend/report_type/detailed_report/detailed_report.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.4/backend/server.py` & `gpt-researcher-0.6.0/backend/server.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.4/backend/utils.py` & `gpt-researcher-0.6.0/backend/utils.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.4/backend/websocket_manager.py` & `gpt-researcher-0.6.0/backend/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.4/gpt_researcher/config/config.py` & `gpt-researcher-0.6.0/gpt_researcher/config/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
     def __init__(self, config_file: str = None):
         """Initialize the config class."""
         self.config_file = os.path.expanduser(config_file) if config_file else os.getenv('CONFIG_FILE')
         self.retriever = os.getenv('RETRIEVER', "tavily")
         self.embedding_provider = os.getenv('EMBEDDING_PROVIDER', 'openai')
         self.llm_provider = os.getenv('LLM_PROVIDER', "openai")
+        self.ollama_base_url = os.getenv('OLLAMA_BASE_URL', None)
         self.fast_llm_model = os.getenv('FAST_LLM_MODEL', "gpt-3.5-turbo-16k")
         self.smart_llm_model = os.getenv('SMART_LLM_MODEL', "gpt-4o")
         self.fast_token_limit = int(os.getenv('FAST_TOKEN_LIMIT', 2000))
         self.smart_token_limit = int(os.getenv('SMART_TOKEN_LIMIT', 4000))
         self.browse_chunk_max_length = int(os.getenv('BROWSE_CHUNK_MAX_LENGTH', 8192))
         self.summary_token_limit = int(os.getenv('SUMMARY_TOKEN_LIMIT', 700))
         self.temperature = float(os.getenv('TEMPERATURE', 0.55))
```

### Comparing `gpt-researcher-0.5.4/gpt_researcher/context/compression.py` & `gpt-researcher-0.6.0/gpt_researcher/context/compression.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.4/gpt_researcher/context/retriever.py` & `gpt-researcher-0.6.0/gpt_researcher/context/retriever.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.4/gpt_researcher/document/document.py` & `gpt-researcher-0.6.0/gpt_researcher/document/document.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.4/gpt_researcher/llm_provider/azureopenai/azureopenai.py` & `gpt-researcher-0.6.0/gpt_researcher/llm_provider/azureopenai/azureopenai.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.4/gpt_researcher/llm_provider/google/google.py` & `gpt-researcher-0.6.0/gpt_researcher/llm_provider/google/google.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.4/gpt_researcher/llm_provider/groq/groq.py` & `gpt-researcher-0.6.0/gpt_researcher/llm_provider/groq/groq.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.4/gpt_researcher/llm_provider/openai/openai.py` & `gpt-researcher-0.6.0/gpt_researcher/llm_provider/openai/openai.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.4/gpt_researcher/master/agent.py` & `gpt-researcher-0.6.0/gpt_researcher/master/agent.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.4/gpt_researcher/master/functions.py` & `gpt-researcher-0.6.0/gpt_researcher/master/functions.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.4/gpt_researcher/master/prompts.py` & `gpt-researcher-0.6.0/gpt_researcher/master/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.4/gpt_researcher/memory/embeddings.py` & `gpt-researcher-0.6.0/gpt_researcher/memory/embeddings.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,23 +4,22 @@
 
 class Memory:
     def __init__(self, embedding_provider, **kwargs):
 
         _embeddings = None
         match embedding_provider:
             case "ollama":
-                from langchain.embeddings import OllamaEmbeddings
-                _embeddings = OllamaEmbeddings(model="llama2")
+                from langchain_community.embeddings import OllamaEmbeddings
+                _embeddings = OllamaEmbeddings(model=os.environ["OLLAMA_EMBEDDING_MODEL"], base_url=os.environ["OLLAMA_BASE_URL"])
             case "custom":
                 from langchain_openai import OpenAIEmbeddings
                 _embeddings = OpenAIEmbeddings(model=os.environ.get("OPENAI_EMBEDDING_MODEL", "custom"),
                                                    openai_api_key=os.environ.get("OPENAI_API_KEY", "custom"), 
                                                    openai_api_base=os.environ.get("OPENAI_BASE_URL", "http://localhost:1234/v1"), #default for lmstudio
-                                                   check_embedding_ctx_length=False, #quick fix for lmstudio
-                                                   ) 
+                                                   check_embedding_ctx_length=False) #quick fix for lmstudio
             case "openai":
                 from langchain_openai import OpenAIEmbeddings
                 _embeddings = OpenAIEmbeddings(model="text-embedding-3-small")
             case "azureopenai":
                 from langchain_openai import AzureOpenAIEmbeddings
                 _embeddings = AzureOpenAIEmbeddings(deployment=os.environ["AZURE_EMBEDDING_MODEL"], chunk_size=16)
             case "huggingface":
```

### Comparing `gpt-researcher-0.5.4/gpt_researcher/retrievers/bing/bing.py` & `gpt-researcher-0.6.0/gpt_researcher/retrievers/bing/bing.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.4/gpt_researcher/retrievers/google/google.py` & `gpt-researcher-0.6.0/gpt_researcher/retrievers/google/google.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.4/gpt_researcher/retrievers/searx/searx.py` & `gpt-researcher-0.6.0/gpt_researcher/retrievers/searx/searx.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.4/gpt_researcher/retrievers/serpapi/serpapi.py` & `gpt-researcher-0.6.0/gpt_researcher/retrievers/serpapi/serpapi.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.4/gpt_researcher/retrievers/serper/serper.py` & `gpt-researcher-0.6.0/gpt_researcher/retrievers/serper/serper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.4/gpt_researcher/retrievers/tavily_search/tavily_search.py` & `gpt-researcher-0.6.0/gpt_researcher/retrievers/tavily_search/tavily_search.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.4/gpt_researcher/scraper/arxiv/arxiv.py` & `gpt-researcher-0.6.0/gpt_researcher/scraper/arxiv/arxiv.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.4/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py` & `gpt-researcher-0.6.0/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.4/gpt_researcher/scraper/newspaper/newspaper.py` & `gpt-researcher-0.6.0/gpt_researcher/scraper/newspaper/newspaper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.4/gpt_researcher/scraper/pymupdf/pymupdf.py` & `gpt-researcher-0.6.0/gpt_researcher/scraper/pymupdf/pymupdf.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.4/gpt_researcher/scraper/scraper.py` & `gpt-researcher-0.6.0/gpt_researcher/scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.4/gpt_researcher/scraper/web_base_loader/web_base_loader.py` & `gpt-researcher-0.6.0/gpt_researcher/scraper/web_base_loader/web_base_loader.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.4/gpt_researcher/utils/llm.py` & `gpt-researcher-0.6.0/gpt_researcher/utils/llm.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import logging
 from typing import Optional
 
 from colorama import Fore, Style
 from fastapi import WebSocket
 from langchain.output_parsers import PydanticOutputParser
 from langchain.prompts import PromptTemplate
-from langchain_openai import ChatOpenAI
 
 from gpt_researcher.master.prompts import auto_agent_instructions, generate_subtopics_prompt
 
 from .validators import Subtopics
 
 
 def get_provider(llm_provider):
@@ -23,20 +22,36 @@
             llm_provider = OpenAIProvider
         case "azureopenai":
             from ..llm_provider import AzureOpenAIProvider
             llm_provider = AzureOpenAIProvider
         case "google":
             from ..llm_provider import GoogleProvider
             llm_provider = GoogleProvider
+        case "ollama":
+            from ..llm_provider import OllamaProvider
+            llm_provider = OllamaProvider
         case "groq":
             from ..llm_provider import GroqProvider
             llm_provider = GroqProvider
-
+        case "together":
+            from ..llm_provider import TogetherProvider
+            llm_provider = TogetherProvider
+        case "huggingface":
+            from ..llm_provider import HugginFaceProvider
+            llm_provider = HugginFaceProvider
+        case "mistral":
+            from ..llm_provider import MistralProvider
+            llm_provider = MistralProvider
+        case "anthropic":
+            from ..llm_provider import AnthropicProvider
+            llm_provider = AnthropicProvider
         case _:
-            raise Exception("LLM provider not found.")
+            raise Exception("LLM provider not found. "
+                            "Check here to learn more about support LLMs: "
+                            "https://docs.gptr.dev/docs/gpt-researcher/llms")
 
     return llm_provider
 
 
 async def create_chat_completion(
         messages: list,  # type: ignore
         model: Optional[str] = None,
```

### Comparing `gpt-researcher-0.5.4/gpt_researcher.egg-info/PKG-INFO` & `gpt-researcher-0.6.0/gpt_researcher.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-researcher
-Version: 0.5.4
+Version: 0.6.0
 Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
 Home-page: https://github.com/assafelovic/gpt-researcher
 Author: Assaf Elovic
 Author-email: assaf.elovic@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -12,15 +12,19 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# 🔎 GPT Researcher
+<h1 style="display: flex; align-items: center; gap: 10px;">
+  <img src="https://github.com/assafelovic/gpt-researcher/assets/13554167/a45bac7c-092c-42e5-8eb6-69acbf20dde5" alt="Logo" width="25">
+  GPT Researcher
+</h1>
+
 [![Official Website](https://img.shields.io/badge/Official%20Website-gptr.dev-teal?style=for-the-badge&logo=world&logoColor=white)](https://gptr.dev)
 [![Official Website](https://img.shields.io/badge/Documentation-GPTR-pink?logo=googledocs&logoColor=white&style=for-the-badge)](https://docs.gptr.dev)
 [![Discord Follow](https://dcbadge.vercel.app/api/server/SK3KKuSD?style=for-the-badge)](https://discord.gg/SK3KKuSD)
 
 [![GitHub Repo stars](https://img.shields.io/github/stars/assafelovic/gpt-researcher?style=social)](https://github.com/assafelovic/gpt-researcher)
 [![Twitter Follow](https://img.shields.io/twitter/follow/assaf_elovic?style=social)](https://twitter.com/assaf_elovic)
 [![PyPI version](https://badge.fury.io/py/gpt-researcher.svg)](https://badge.fury.io/py/gpt-researcher)
@@ -51,18 +55,19 @@
 https://github.com/assafelovic/gpt-researcher/assets/13554167/dd6cf08f-b31e-40c6-9907-1915f52a7110
 
 ## Architecture
 The main idea is to run "planner" and "execution" agents, whereas the planner generates questions to research, and the execution agents seek the most related information based on each generated research question. Finally, the planner filters and aggregates all related information and creates a research report. <br /> <br /> 
 The agents leverage both `gpt3.5-turbo` and `gpt-4o` (128K context) to complete a research task. We optimize for costs using each only when necessary. **The average research task takes around 3 minutes to complete, and costs ~$0.1.**
 
 <div align="center">
-<img align="center" height="500" src="https://cowriter-images.s3.amazonaws.com/architecture.png">
+<img align="center" height="600" src="https://github.com/assafelovic/gpt-researcher/assets/13554167/4ac896fd-63ab-4b77-9688-ff62aafcc527">
 </div>
 
 
+
 More specifically:
 * Create a domain specific agent based on research query or task.
 * Generate a set of research questions that together form an objective opinion on any given task. 
 * For each research question, trigger a crawler agent that scrapes online resources for information relevant to the given task.
 * For each scraped resources, summarize based on relevant information and keep track of its sources.
 * Finally, filter and aggregate all summarized sources and generate a final research report.
```

### Comparing `gpt-researcher-0.5.4/gpt_researcher.egg-info/SOURCES.txt` & `gpt-researcher-0.6.0/gpt_researcher.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -21,22 +21,32 @@
 gpt_researcher/config/config.py
 gpt_researcher/context/__init__.py
 gpt_researcher/context/compression.py
 gpt_researcher/context/retriever.py
 gpt_researcher/document/__init__.py
 gpt_researcher/document/document.py
 gpt_researcher/llm_provider/__init__.py
+gpt_researcher/llm_provider/anthropic/__init__.py
+gpt_researcher/llm_provider/anthropic/anthropic.py
 gpt_researcher/llm_provider/azureopenai/__init__.py
 gpt_researcher/llm_provider/azureopenai/azureopenai.py
 gpt_researcher/llm_provider/google/__init__.py
 gpt_researcher/llm_provider/google/google.py
 gpt_researcher/llm_provider/groq/__init__.py
 gpt_researcher/llm_provider/groq/groq.py
+gpt_researcher/llm_provider/huggingface/__init__.py
+gpt_researcher/llm_provider/huggingface/huggingface.py
+gpt_researcher/llm_provider/mistral/__init__.py
+gpt_researcher/llm_provider/mistral/mistral.py
+gpt_researcher/llm_provider/ollama/__init__.py
+gpt_researcher/llm_provider/ollama/ollama.py
 gpt_researcher/llm_provider/openai/__init__.py
 gpt_researcher/llm_provider/openai/openai.py
+gpt_researcher/llm_provider/together/__init__.py
+gpt_researcher/llm_provider/together/together.py
 gpt_researcher/master/__init__.py
 gpt_researcher/master/agent.py
 gpt_researcher/master/functions.py
 gpt_researcher/master/prompts.py
 gpt_researcher/memory/__init__.py
 gpt_researcher/memory/embeddings.py
 gpt_researcher/retrievers/__init__.py
```

### Comparing `gpt-researcher-0.5.4/pyproject.toml` & `gpt-researcher-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.4/setup.py` & `gpt-researcher-0.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt", "r") as f:
     reqs = [line.strip() for line in f if ('selenium' not in line and 'webdriver' not in line)]
 
 setup(
     name="gpt-researcher",
-    version="0.5.4",
+    version="0.6.0",
     description="GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.",
     package_dir={'gpt_researcher': 'gpt_researcher'},
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/assafelovic/gpt-researcher",
     author="Assaf Elovic",
```

