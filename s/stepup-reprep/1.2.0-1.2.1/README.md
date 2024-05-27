# Comparing `tmp/stepup_reprep-1.2.0.tar.gz` & `tmp/stepup_reprep-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stepup_reprep-1.2.0.tar", last modified: Mon May 20 13:32:39 2024, max compression
+gzip compressed data, was "stepup_reprep-1.2.1.tar", last modified: Mon May 27 07:25:54 2024, max compression
```

## Comparing `stepup_reprep-1.2.0.tar` & `stepup_reprep-1.2.1.tar`

### file list

```diff
@@ -1,357 +1,360 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.018039 stepup_reprep-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.966039 stepup_reprep-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.974039 stepup_reprep-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/.github/workflows/mkdocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-20 13:32:39.018039 stepup_reprep-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.974039 stepup_reprep-1.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.974039 stepup_reprep-1.2.0/docs/advanced_topics/
--rw-r--r--   0 runner    (1001) docker     (127)     7573 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/advanced_topics/archive_git.md
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/advanced_topics/good_practices.md
--rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/advanced_topics/inventory_files.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.978039 stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    22692 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/figure.png
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/hexagon.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)      114 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/pentagon.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)      278 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/square.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      413 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/triangle.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs.md
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/clean_stdout.sed
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/development.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.978039 stepup_reprep-1.2.0/docs/from_scratch/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/from_scratch/introduction.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.978039 stepup_reprep-1.2.0/docs/from_template/
--rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/from_template/before_you_begin.md
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/from_template/create_or_clone_a_project.md
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/from_template/introduction.md
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/from_template/working_on_a_project.md
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/license.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.978039 stepup_reprep-1.2.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/reference/stepup.reprep.api.md
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/reference/stepup.reprep.tile_pdf.md
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 13:32:39.018039 stepup_reprep-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.966039 stepup_reprep-1.2.0/stepup/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.982039 stepup_reprep-1.2.0/stepup/reprep/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/add_notes_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    24955 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/bibtex_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/check_hrefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/check_inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/convert_inkscape.py
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/convert_markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/latex.py
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/latex_deps.py
--rw-r--r--   0 runner    (1001) docker     (127)     7006 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/latex_flat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/latex_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/make_inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/normalize_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/nup_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/pytest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/raster_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/render.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/tile_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/zip_inventory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.018039 stepup_reprep-1.2.0/stepup_reprep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-20 13:32:38.000000 stepup_reprep-1.2.0/stepup_reprep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11921 2024-05-20 13:32:38.000000 stepup_reprep-1.2.0/stepup_reprep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:32:38.000000 stepup_reprep-1.2.0/stepup_reprep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-20 13:32:38.000000 stepup_reprep-1.2.0/stepup_reprep.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-20 13:32:38.000000 stepup_reprep-1.2.0/stepup_reprep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 13:32:38.000000 stepup_reprep-1.2.0/stepup_reprep.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.982039 stepup_reprep-1.2.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.970039 stepup_reprep-1.2.0/tests/cases/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.982039 stepup_reprep-1.2.0/tests/cases/add_notes_pdf/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/add_notes_pdf/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/add_notes_pdf/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/add_notes_pdf/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/add_notes_pdf/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1113 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/add_notes_pdf/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/add_notes_pdf/notes.pdf
--rwxr-xr-x   0 runner    (1001) docker     (127)      182 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/add_notes_pdf/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/add_notes_pdf/src.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.986039 stepup_reprep-1.2.0/tests/cases/cat_pdf/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/cat_pdf/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/cat_pdf/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/cat_pdf/doc1.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/cat_pdf/doc2.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/cat_pdf/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/cat_pdf/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1113 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/cat_pdf/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      172 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/cat_pdf/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/cat_pdf/reproducibility_inventory.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.986039 stepup_reprep-1.2.0/tests/cases/check_hrefs_html/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_html/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_html/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_html/check_hrefs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_html/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_html/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      749 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_html/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_html/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_html/test.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.986039 stepup_reprep-1.2.0/tests/cases/check_hrefs_md/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_md/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_md/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_md/check_hrefs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_md/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_md/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      749 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_md/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      174 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_md/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_md/test.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.990039 stepup_reprep-1.2.0/tests/cases/check_hrefs_pdf/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_pdf/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_pdf/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_pdf/check_hrefs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_pdf/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_pdf/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      883 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_pdf/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_pdf/main.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      202 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_pdf/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.990039 stepup_reprep-1.2.0/tests/cases/convert_inkscape/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape/glasses.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1340 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      244 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape/smile.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.994039 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_050.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_055.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_060.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_065.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_070.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_075.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_080.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_085.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_090.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_095.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_100.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_105.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_110.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_115.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_120.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5907 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_125.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_130.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_135.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_140.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_145.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2045 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      163 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.994039 stepup_reprep-1.2.0/tests/cases/convert_libreoffice/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_libreoffice/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_libreoffice/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_libreoffice/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_libreoffice/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1146 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_libreoffice/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      153 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_libreoffice/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)    13660 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_libreoffice/slide.odp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.994039 stepup_reprep-1.2.0/tests/cases/convert_libreoffice_concurrency/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_libreoffice_concurrency/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)     2039 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_libreoffice_concurrency/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      242 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_libreoffice_concurrency/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)    10286 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_libreoffice_concurrency/something.odt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.998039 stepup_reprep-1.2.0/tests/cases/convert_markdown/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_markdown/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_markdown/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_markdown/demo.css
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_markdown/demo.md
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_markdown/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_markdown/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_markdown/macros.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)     1134 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_markdown/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      202 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_markdown/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.998039 stepup_reprep-1.2.0/tests/cases/convert_mutool/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_mutool/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_mutool/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_mutool/example.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_mutool/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_mutool/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1115 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_mutool/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      173 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_mutool/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_mutool/reproducibility_inventory.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.998039 stepup_reprep-1.2.0/tests/cases/convert_weasyprint/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_weasyprint/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_weasyprint/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_weasyprint/doc.html
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_weasyprint/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_weasyprint/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1121 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_weasyprint/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_weasyprint/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.998039 stepup_reprep-1.2.0/tests/cases/latex_diff/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_diff/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_diff/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_diff/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_diff/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1062 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_diff/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_diff/new.tex
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_diff/old.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      173 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_diff/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.002039 stepup_reprep-1.2.0/tests/cases/latex_flat/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat/article_structured.tex
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat/expected_article.tex
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1442 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat/part1.tex
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat/part2.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat/plan_01.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      249 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat/plan_02.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.002039 stepup_reprep-1.2.0/tests/cases/latex_flat/sub/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat/sub/original.tex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.002039 stepup_reprep-1.2.0/tests/cases/latex_flat_subdir/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat_subdir/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat_subdir/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat_subdir/expected_article.tex
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat_subdir/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat_subdir/expected_inventory.txt
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat_subdir/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat_subdir/inventory.def
--rwxr-xr-x   0 runner    (1001) docker     (127)      969 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat_subdir/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      238 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat_subdir/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.002039 stepup_reprep-1.2.0/tests/cases/latex_flat_subdir/sub/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat_subdir/sub/article_structured.tex
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat_subdir/sub/part1.tex
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat_subdir/sub/part2.tex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.006039 stepup_reprep-1.2.0/tests/cases/lualatex_simple/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/lualatex_simple/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/lualatex_simple/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/lualatex_simple/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1263 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/lualatex_simple/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/lualatex_simple/paper.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      134 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/lualatex_simple/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.006039 stepup_reprep-1.2.0/tests/cases/make_inventory_list/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/make_inventory_list/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/make_inventory_list/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/make_inventory_list/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/make_inventory_list/expected_inventory.txt
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/make_inventory_list/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      790 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/make_inventory_list/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      171 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/make_inventory_list/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.006039 stepup_reprep-1.2.0/tests/cases/nup_pdf/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/nup_pdf/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/nup_pdf/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/nup_pdf/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/nup_pdf/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1083 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/nup_pdf/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/nup_pdf/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/nup_pdf/reproducibility_inventory.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9122 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/nup_pdf/src.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.006039 stepup_reprep-1.2.0/tests/cases/pdflatex_bbl/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_bbl/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_bbl/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_bbl/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1231 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_bbl/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_bbl/paper.bbl
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_bbl/paper.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      172 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_bbl/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.010039 stepup_reprep-1.2.0/tests/cases/pdflatex_bibtex/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_bibtex/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_bibtex/bibsane.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_bibtex/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_bibtex/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1513 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_bibtex/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_bibtex/paper.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      190 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_bibtex/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_bibtex/references.bib
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.010039 stepup_reprep-1.2.0/tests/cases/pdflatex_input/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_input/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_input/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_input/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1276 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_input/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_input/paper.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      224 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_input/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_input/smile.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.010039 stepup_reprep-1.2.0/tests/cases/raster_pdf/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/raster_pdf/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/raster_pdf/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/raster_pdf/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/raster_pdf/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1162 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/raster_pdf/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      181 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/raster_pdf/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/raster_pdf/smile.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.010039 stepup_reprep-1.2.0/tests/cases/render_basic/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_basic/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_basic/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_basic/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_basic/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      849 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_basic/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      188 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_basic/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_basic/template.md
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_basic/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.014039 stepup_reprep-1.2.0/tests/cases/render_relpath/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_relpath/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_relpath/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_relpath/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1084 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_relpath/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      270 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_relpath/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.014039 stepup_reprep-1.2.0/tests/cases/render_relpath/static/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_relpath/static/main.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      213 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_relpath/static/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_relpath/static/preamble.inc.tex
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_relpath/static/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_relpath/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.014039 stepup_reprep-1.2.0/tests/cases/tile_pdf/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/tile_pdf/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/tile_pdf/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    15675 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/tile_pdf/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/tile_pdf/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/tile_pdf/hexagon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/tile_pdf/horizontal.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1531 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/tile_pdf/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/tile_pdf/pentagon.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)      227 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/tile_pdf/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/tile_pdf/square.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)      674 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/tile_pdf/tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/tile_pdf/triangle.svg
--rw-r--r--   0 runner    (1001) docker     (127)    65932 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/tile_pdf/vera.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/tile_pdf/vertical.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.014039 stepup_reprep-1.2.0/tests/cases/xelatex_input/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/xelatex_input/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/xelatex_input/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/xelatex_input/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1377 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/xelatex_input/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/xelatex_input/paper.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      348 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/xelatex_input/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/xelatex_input/smile.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.018039 stepup_reprep-1.2.0/tests/cases/zip_inventory/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/zip_inventory/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/zip_inventory/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/zip_inventory/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/zip_inventory/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1153 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/zip_inventory/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      296 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/zip_inventory/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/zip_inventory/static.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/reprep_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/test_bibtex_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/test_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/test_inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/test_latex_deps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/test_latex_flat.py
--rw-r--r--   0 runner    (1001) docker     (127)    14002 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/test_latex_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/test_zip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.674698 stepup_reprep-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.622697 stepup_reprep-1.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.626697 stepup_reprep-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/.github/workflows/mkdocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-27 07:25:54.674698 stepup_reprep-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.626697 stepup_reprep-1.2.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.626697 stepup_reprep-1.2.1/docs/advanced_topics/
+-rw-r--r--   0 runner    (1001) docker     (127)     7573 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/docs/advanced_topics/archive_git.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/docs/advanced_topics/good_practices.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/docs/advanced_topics/inventory_files.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.630698 stepup_reprep-1.2.1/docs/advanced_topics/tile_pdfs/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/docs/advanced_topics/tile_pdfs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    22692 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/docs/advanced_topics/tile_pdfs/figure.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/docs/advanced_topics/tile_pdfs/hexagon.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      114 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/docs/advanced_topics/tile_pdfs/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/docs/advanced_topics/tile_pdfs/pentagon.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      278 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/docs/advanced_topics/tile_pdfs/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/docs/advanced_topics/tile_pdfs/square.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/docs/advanced_topics/tile_pdfs/stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      413 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/docs/advanced_topics/tile_pdfs/tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/docs/advanced_topics/tile_pdfs/triangle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/docs/advanced_topics/tile_pdfs.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/docs/clean_stdout.sed
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/docs/development.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.630698 stepup_reprep-1.2.1/docs/from_scratch/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/docs/from_scratch/introduction.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.630698 stepup_reprep-1.2.1/docs/from_template/
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/docs/from_template/before_you_begin.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/docs/from_template/create_or_clone_a_project.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/docs/from_template/introduction.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/docs/from_template/working_on_a_project.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/docs/license.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.630698 stepup_reprep-1.2.1/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/docs/reference/stepup.reprep.api.md
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/docs/reference/stepup.reprep.tile_pdf.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 07:25:54.674698 stepup_reprep-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.622697 stepup_reprep-1.2.1/stepup/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.634698 stepup_reprep-1.2.1/stepup/reprep/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/stepup/reprep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/stepup/reprep/add_notes_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25278 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/stepup/reprep/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/stepup/reprep/bibtex_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/stepup/reprep/check_hrefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/stepup/reprep/check_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/stepup/reprep/convert_inkscape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/stepup/reprep/convert_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/stepup/reprep/convert_weasyprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/stepup/reprep/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/stepup/reprep/latex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/stepup/reprep/latex_deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/stepup/reprep/latex_flat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/stepup/reprep/latex_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/stepup/reprep/make_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/stepup/reprep/normalize_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/stepup/reprep/nup_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/stepup/reprep/pytest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/stepup/reprep/raster_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/stepup/reprep/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/stepup/reprep/tile_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/stepup/reprep/zip_inventory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.670698 stepup_reprep-1.2.1/stepup_reprep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-27 07:25:54.000000 stepup_reprep-1.2.1/stepup_reprep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12039 2024-05-27 07:25:54.000000 stepup_reprep-1.2.1/stepup_reprep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 07:25:54.000000 stepup_reprep-1.2.1/stepup_reprep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-27 07:25:54.000000 stepup_reprep-1.2.1/stepup_reprep.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-27 07:25:54.000000 stepup_reprep-1.2.1/stepup_reprep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-27 07:25:54.000000 stepup_reprep-1.2.1/stepup_reprep.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.638697 stepup_reprep-1.2.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.626697 stepup_reprep-1.2.1/tests/cases/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.638697 stepup_reprep-1.2.1/tests/cases/add_notes_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/add_notes_pdf/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/add_notes_pdf/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/add_notes_pdf/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/add_notes_pdf/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1113 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/add_notes_pdf/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/add_notes_pdf/notes.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (127)      182 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/add_notes_pdf/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/add_notes_pdf/src.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.638697 stepup_reprep-1.2.1/tests/cases/cat_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/cat_pdf/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/cat_pdf/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/cat_pdf/doc1.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/cat_pdf/doc2.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/cat_pdf/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/cat_pdf/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1113 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/cat_pdf/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      172 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/cat_pdf/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/cat_pdf/reproducibility_inventory.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.642698 stepup_reprep-1.2.1/tests/cases/check_hrefs_html/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/check_hrefs_html/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/check_hrefs_html/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/check_hrefs_html/check_hrefs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/check_hrefs_html/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/check_hrefs_html/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      749 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/check_hrefs_html/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/check_hrefs_html/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/check_hrefs_html/test.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.642698 stepup_reprep-1.2.1/tests/cases/check_hrefs_md/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/check_hrefs_md/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/check_hrefs_md/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/check_hrefs_md/check_hrefs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/check_hrefs_md/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/check_hrefs_md/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      749 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/check_hrefs_md/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      174 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/check_hrefs_md/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/check_hrefs_md/test.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.642698 stepup_reprep-1.2.1/tests/cases/check_hrefs_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/check_hrefs_pdf/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/check_hrefs_pdf/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/check_hrefs_pdf/check_hrefs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/check_hrefs_pdf/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/check_hrefs_pdf/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      883 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/check_hrefs_pdf/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/check_hrefs_pdf/main.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      202 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/check_hrefs_pdf/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.642698 stepup_reprep-1.2.1/tests/cases/convert_inkscape/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_inkscape/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_inkscape/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_inkscape/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_inkscape/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_inkscape/glasses.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1340 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_inkscape/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      244 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_inkscape/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_inkscape/smile.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.646698 stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_050.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_055.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_060.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_065.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_070.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_075.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_080.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_085.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_090.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_095.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_100.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_105.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_110.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_115.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_120.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5907 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_125.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_130.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_135.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_140.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_145.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2045 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      163 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.650698 stepup_reprep-1.2.1/tests/cases/convert_libreoffice/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_libreoffice/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_libreoffice/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_libreoffice/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_libreoffice/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1146 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_libreoffice/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      153 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_libreoffice/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13660 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_libreoffice/slide.odp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.650698 stepup_reprep-1.2.1/tests/cases/convert_libreoffice_concurrency/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_libreoffice_concurrency/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2039 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_libreoffice_concurrency/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      242 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_libreoffice_concurrency/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10286 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_libreoffice_concurrency/something.odt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.650698 stepup_reprep-1.2.1/tests/cases/convert_markdown/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_markdown/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_markdown/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_markdown/demo.css
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_markdown/demo.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_markdown/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_markdown/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_markdown/macros.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1134 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_markdown/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      202 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_markdown/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.650698 stepup_reprep-1.2.1/tests/cases/convert_mutool/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_mutool/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_mutool/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_mutool/example.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_mutool/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_mutool/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1115 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_mutool/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      173 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_mutool/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_mutool/reproducibility_inventory.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.654698 stepup_reprep-1.2.1/tests/cases/convert_weasyprint/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_weasyprint/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_weasyprint/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_weasyprint/block.png
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_weasyprint/doc.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_weasyprint/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_weasyprint/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1121 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_weasyprint/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      183 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_weasyprint/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/convert_weasyprint/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.654698 stepup_reprep-1.2.1/tests/cases/latex_diff/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_diff/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_diff/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_diff/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_diff/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1062 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_diff/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_diff/new.tex
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_diff/old.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      173 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_diff/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.654698 stepup_reprep-1.2.1/tests/cases/latex_flat/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_flat/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_flat/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_flat/article_structured.tex
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_flat/expected_article.tex
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_flat/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_flat/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_flat/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_flat/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1442 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_flat/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_flat/part1.tex
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_flat/part2.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_flat/plan_01.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      249 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_flat/plan_02.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.654698 stepup_reprep-1.2.1/tests/cases/latex_flat/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_flat/sub/original.tex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.658698 stepup_reprep-1.2.1/tests/cases/latex_flat_subdir/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_flat_subdir/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_flat_subdir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_flat_subdir/expected_article.tex
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_flat_subdir/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_flat_subdir/expected_inventory.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_flat_subdir/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_flat_subdir/inventory.def
+-rwxr-xr-x   0 runner    (1001) docker     (127)      969 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_flat_subdir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      238 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_flat_subdir/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.658698 stepup_reprep-1.2.1/tests/cases/latex_flat_subdir/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_flat_subdir/sub/article_structured.tex
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_flat_subdir/sub/part1.tex
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/latex_flat_subdir/sub/part2.tex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.658698 stepup_reprep-1.2.1/tests/cases/lualatex_simple/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/lualatex_simple/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/lualatex_simple/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/lualatex_simple/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1263 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/lualatex_simple/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/lualatex_simple/paper.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      134 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/lualatex_simple/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.658698 stepup_reprep-1.2.1/tests/cases/make_inventory_list/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/make_inventory_list/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/make_inventory_list/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/make_inventory_list/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/make_inventory_list/expected_inventory.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/make_inventory_list/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      790 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/make_inventory_list/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      171 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/make_inventory_list/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.662698 stepup_reprep-1.2.1/tests/cases/nup_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/nup_pdf/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/nup_pdf/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/nup_pdf/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/nup_pdf/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1083 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/nup_pdf/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/nup_pdf/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/nup_pdf/reproducibility_inventory.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9122 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/nup_pdf/src.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.662698 stepup_reprep-1.2.1/tests/cases/pdflatex_bbl/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/pdflatex_bbl/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/pdflatex_bbl/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/pdflatex_bbl/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1231 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/pdflatex_bbl/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/pdflatex_bbl/paper.bbl
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/pdflatex_bbl/paper.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      172 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/pdflatex_bbl/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.662698 stepup_reprep-1.2.1/tests/cases/pdflatex_bibtex/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/pdflatex_bibtex/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/pdflatex_bibtex/bibsane.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/pdflatex_bibtex/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/pdflatex_bibtex/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1513 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/pdflatex_bibtex/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/pdflatex_bibtex/paper.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      190 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/pdflatex_bibtex/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/pdflatex_bibtex/references.bib
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.662698 stepup_reprep-1.2.1/tests/cases/pdflatex_input/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/pdflatex_input/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/pdflatex_input/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/pdflatex_input/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1276 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/pdflatex_input/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/pdflatex_input/paper.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      224 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/pdflatex_input/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/pdflatex_input/smile.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.666698 stepup_reprep-1.2.1/tests/cases/raster_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/raster_pdf/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/raster_pdf/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/raster_pdf/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/raster_pdf/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1162 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/raster_pdf/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      181 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/raster_pdf/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/raster_pdf/smile.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.666698 stepup_reprep-1.2.1/tests/cases/render_basic/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/render_basic/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/render_basic/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/render_basic/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/render_basic/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      849 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/render_basic/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      188 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/render_basic/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/render_basic/template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/render_basic/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.666698 stepup_reprep-1.2.1/tests/cases/render_relpath/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/render_relpath/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/render_relpath/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/render_relpath/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1084 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/render_relpath/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      270 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/render_relpath/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.666698 stepup_reprep-1.2.1/tests/cases/render_relpath/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/render_relpath/static/main.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      213 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/render_relpath/static/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/render_relpath/static/preamble.inc.tex
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/render_relpath/static/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/render_relpath/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.670698 stepup_reprep-1.2.1/tests/cases/tile_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/tile_pdf/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/tile_pdf/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    15675 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/tile_pdf/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/tile_pdf/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/tile_pdf/hexagon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/tile_pdf/horizontal.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1531 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/tile_pdf/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/tile_pdf/pentagon.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      227 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/tile_pdf/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/tile_pdf/square.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      674 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/tile_pdf/tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/tile_pdf/triangle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    65932 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/tile_pdf/vera.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/tile_pdf/vertical.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.670698 stepup_reprep-1.2.1/tests/cases/xelatex_input/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/xelatex_input/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/xelatex_input/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/xelatex_input/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1377 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/xelatex_input/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/xelatex_input/paper.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      348 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/xelatex_input/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/xelatex_input/smile.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:25:54.670698 stepup_reprep-1.2.1/tests/cases/zip_inventory/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/zip_inventory/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/zip_inventory/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/zip_inventory/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/zip_inventory/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1153 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/zip_inventory/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      296 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/zip_inventory/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/cases/zip_inventory/static.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/reprep_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/test_bibtex_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/test_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/test_latex_deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/test_latex_flat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14026 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/test_latex_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-27 07:25:48.000000 stepup_reprep-1.2.1/tests/test_zip.py
```

### Comparing `stepup_reprep-1.2.0/.github/workflows/release.yaml` & `stepup_reprep-1.2.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/.pre-commit-config.yaml` & `stepup_reprep-1.2.1/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -21,16 +21,16 @@
       args: ["--autofix", "--no-sort-keys"]
     - id: trailing-whitespace
 - repo: https://github.com/Lucas-C/pre-commit-hooks
   rev: v1.5.5
   hooks:
     - id: remove-crlf
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: v0.4.3
+  rev: v0.4.5
   hooks:
     - id: ruff-format
     - id: ruff
       args: ["--fix", "--show-fixes"]
 - repo: https://github.com/python-jsonschema/check-jsonschema
-  rev: 0.28.2
+  rev: 0.28.4
   hooks:
     - id: check-github-workflows
```

### Comparing `stepup_reprep-1.2.0/LICENSE` & `stepup_reprep-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/PKG-INFO` & `stepup_reprep-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stepup-reprep
-Version: 1.2.0
+Version: 1.2.1
 Summary: StepUp RepRep is the StepUp extension for Reproducible Reporting
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 Project-URL: Documentation, https://reproducible-reporting.github.io/stepup-reprep/
 Project-URL: Issues, https://github.com/reproducible-reporting/stepup-reprep/issues
 Project-URL: Source, https://github.com/reproducible-reporting/stepup-reprep/
 Project-URL: Changelog, https://reproducible-reporting.github.io/stepup-reprep/changelog/
 Classifier: Environment :: Console
@@ -24,15 +24,15 @@
 Requires-Dist: markdown
 Requires-Dist: markdown_katex
 Requires-Dist: numpy
 Requires-Dist: path
 Requires-Dist: pymupdf
 Requires-Dist: pyyaml
 Requires-Dist: scipy
-Requires-Dist: stepup>=1.2.3
+Requires-Dist: stepup>=1.2.4
 Requires-Dist: weasyprint
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
```

### Comparing `stepup_reprep-1.2.0/README.md` & `stepup_reprep-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/docs/advanced_topics/archive_git.md` & `stepup_reprep-1.2.1/docs/advanced_topics/archive_git.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/docs/advanced_topics/inventory_files.md` & `stepup_reprep-1.2.1/docs/advanced_topics/inventory_files.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/figure.png` & `stepup_reprep-1.2.1/docs/advanced_topics/tile_pdfs/figure.png`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/hexagon.svg` & `stepup_reprep-1.2.1/docs/advanced_topics/tile_pdfs/hexagon.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/pentagon.svg` & `stepup_reprep-1.2.1/docs/advanced_topics/tile_pdfs/pentagon.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/square.svg` & `stepup_reprep-1.2.1/docs/advanced_topics/tile_pdfs/square.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/stdout.txt` & `stepup_reprep-1.2.1/docs/advanced_topics/tile_pdfs/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/triangle.svg` & `stepup_reprep-1.2.1/docs/advanced_topics/tile_pdfs/triangle.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs.md` & `stepup_reprep-1.2.1/docs/advanced_topics/tile_pdfs.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/docs/changelog.md` & `stepup_reprep-1.2.1/docs/changelog.md`

 * *Files 21% similar despite different names*

```diff
@@ -3,14 +3,30 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [1.2.1] - 2024-05-27
+
+### Changed
+
+- Conversion from HTML to weasyprint is now a two-step process and includes detection
+  of implicit input files used in the HTML to PDF conversion. (Images and exteral CCS)
+- Improved reusability of script modules:
+  `add_notes_pdf`, `check_hrefs`, `convert_inkscape`, `convert_markdown`,
+  `convert_weasyprint`, `latex`, `latex_flat`, `make_inventory`, `normalized_pdf`,
+  `nup_pdf`, `raster_pdf`, `render` and `zip_inventory`.
+
+### Fixed
+
+- Fixed a few errors in the HTML generated by `convert_markdown()`
+
+
 ## [1.2.0] - 2024-05-20
 
 ### Added
 
 - `reprep-zip-inventory` command to manually create a reproducible ZIP file from an `inventory.txt` file.
 - More documentation on how to work with inventory files.
 - Tutorial for archiving StepUp publication Git repositories.
```

### Comparing `stepup_reprep-1.2.0/docs/development.md` & `stepup_reprep-1.2.1/docs/development.md`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 cd stepup-reprep
 pre-commit install
 python -m venv venv
 echo 'source venv/bin/activate' > .envrc
 direnv allow
 pip install -U pip
 pip install -e .[dev]
-pip install -e ../stepup-core  # optional
+pip install -e ../stepup-core[dev]  # optional
 pytest -vv
 ```
 
 ## Documentation
 
 The documentation is created with [MkDocs](https://www.mkdocs.org/).
```

### Comparing `stepup_reprep-1.2.0/docs/from_template/before_you_begin.md` & `stepup_reprep-1.2.1/docs/from_template/before_you_begin.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/docs/from_template/create_or_clone_a_project.md` & `stepup_reprep-1.2.1/docs/from_template/create_or_clone_a_project.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/docs/from_template/introduction.md` & `stepup_reprep-1.2.1/docs/from_template/introduction.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/docs/from_template/working_on_a_project.md` & `stepup_reprep-1.2.1/docs/from_template/working_on_a_project.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/docs/index.md` & `stepup_reprep-1.2.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/docs/installation.md` & `stepup_reprep-1.2.1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/docs/license.md` & `stepup_reprep-1.2.1/docs/license.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/mkdocs.yml` & `stepup_reprep-1.2.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/stepup/reprep/__init__.py` & `stepup_reprep-1.2.1/stepup/reprep/__init__.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/stepup/reprep/add_notes_pdf.py` & `stepup_reprep-1.2.1/stepup/reprep/add_notes_pdf.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,39 +23,37 @@
 import sys
 
 import fitz
 
 __all__ = ("add_notes_pdf",)
 
 
-def main() -> int:
+def main(argv: list[str] | None = None):
     """Main program."""
-    args = parse_args()
+    args = parse_args(argv)
     add_notes_pdf(args.path_src, args.path_notes, args.path_dst)
-    return 0
 
 
-def parse_args() -> argparse.Namespace:
+def parse_args(argv: list[str] | None = None) -> argparse.Namespace:
     """Parse command-line arguments."""
     parser = argparse.ArgumentParser(
         prog="reprep-add-notes-pdf",
         description="Add a notes page at every even page of a PDF file.",
     )
     parser.add_argument("path_src", help="The source pdf to which notes should be added.")
     parser.add_argument("path_notes", help="The pdf with the notes page(s).")
     parser.add_argument("path_dst", help="The output pdf.")
-    return parser.parse_args()
+    return parser.parse_args(argv)
 
 
 def add_notes_pdf(path_src: str, path_notes: str, path_dst: str):
     """Insert notes pages at every even page."""
     for path_pdf in path_src, path_notes, path_dst:
         if not path_pdf.endswith(".pdf"):
-            print(f"All arguments must have a `.pdf` extension, got: {path_pdf}", file=sys.stderr)
-            return 2
+            raise ValueError(f"All arguments must have a `.pdf` extension, got: {path_pdf}")
     src = fitz.open(path_src)
     notes = fitz.open(path_notes)
 
     # Create the combined PDF
     dst = fitz.open()
     for isrc in range(len(src)):
         final = isrc == len(src) - 1
```

### Comparing `stepup_reprep-1.2.0/stepup/reprep/api.py` & `stepup_reprep-1.2.1/stepup/reprep/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,17 +130,14 @@
     inp_paths = [path_src]
     if path_config is not None:
         inp_paths.append(path_config)
         command += f" -c {path_config}"
     step(command, inp=inp_paths, block=block)
 
 
-pool("markdown_katex", 1)
-
-
 def convert_markdown(
     path_md: str,
     out: str | None = None,
     *,
     katex: bool = False,
     path_macro: str | None = None,
     optional: bool = False,
@@ -167,52 +164,61 @@
         path_md = subs(path_md)
         out = subs(out)
     if not path_md.endswith(".md"):
         raise ValueError("The Markdown file must have extension .md")
     path_html = make_path_out(path_md, out, ".html")
     inp = [path_md]
     command = f"python -m stepup.reprep.convert_markdown {path_md} {path_html}"
-    pool = None
+    pool_name = None
     if katex:
         command += " --katex"
-        pool = "markdown_katex"
+        pool_name = "markdown_katex"
+        pool(pool_name, 1)
         if path_macro is not None:
             command += f" --katex-macros={path_macro}"
             inp.append(path_macro)
-    step(command, inp=inp, out=path_html, pool=pool, optional=optional, block=block)
+    step(command, inp=inp, out=path_html, pool=pool_name, optional=optional, block=block)
 
 
 def convert_weasyprint(
     path_html: str,
     out: str | None = None,
     *,
+    weasyprint: str | None = None,
     optional: bool = False,
     block: bool = False,
 ):
     """Convert a HTML document to PDF.
 
     Parameters
     ----------
     path_html
         The HTML input file.
     out
         Output destination: `None`, a directory or a file.
+    weasyprint
+        The path to the weasyprint executable.
+        Defaults to `${REPREP_WEASYPRINT}` variable or `weasyprint` if the variable is unset.
     optional
         When `True`, the step is only executed when needed by other steps.
     block
         When `True`, the step will always remain pending.
     """
     with subs_env_vars() as subs:
         path_html = subs(path_html)
         out = subs(out)
     if not path_html.endswith(".html"):
         raise ValueError("The HTML file must have extension .html")
     path_pdf = make_path_out(path_html, out, ".pdf")
-    command = "weasyprint ${inp} ${out}"
-    step(command, inp=path_html, out=path_pdf, optional=optional, block=block)
+    command = f"python -m stepup.reprep.convert_weasyprint {path_html} {path_pdf}"
+    if weasyprint is not None:
+        command += f" --weasyprint={weasyprint}"
+    if optional:
+        command += " --optional"
+    step(command, inp=path_html, block=block)
 
 
 def convert_odf_pdf(
     path_odf: str,
     out: str | None = None,
     *,
     libreoffice: str | None = None,
@@ -364,15 +370,15 @@
     the following bug: https://gitlab.com/inkscape/inkscape/-/issues/4716
     """
     with subs_env_vars() as subs:
         path_svg = subs(path_svg)
         path_out = subs(path_out)
     if not path_svg.endswith(".svg"):
         raise ValueError("The SVG file must have extension .svg")
-    elif not (path_out.endswith(".pdf") or path_out.endswith(".png")):
+    if not (path_out.endswith((".pdf", ".png"))):
         raise ValueError("The output file must have extension .pdf or .png")
     command = f"python -m stepup.reprep.convert_inkscape {path_svg} {path_out}"
     if inkscape is not None:
         command += f" --inkscape={inkscape}"
     if inkscape_args is not None:
         command += f" -- {inkscape_args}"
     if optional:
```

### Comparing `stepup_reprep-1.2.0/stepup/reprep/bibtex_log.py` & `stepup_reprep-1.2.1/stepup/reprep/bibtex_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             if "---" in line and "file " in line:
                 last_src = line.rsplit(maxsplit=1)[-1]
                 recorded = []
             recorded.append(line[:-1])
             if line.startswith("I'm skipping whatever remains"):
                 error = True
                 break
-            elif line.startswith(r"I found no \bibstyle command"):
+            if line.startswith(r"I found no \bibstyle command"):
                 last_src = line.split()[-1]
                 recorded = [line[:-1]]
                 error = True
                 break
 
     message = "\n".join(recorded) if error else DEFAULT_MESSAGE.format(path=path_blg)
     return ErrorInfo("BibTeX", last_src, message=message)
```

### Comparing `stepup_reprep-1.2.0/stepup/reprep/check_hrefs.py` & `stepup_reprep-1.2.1/stepup/reprep/check_hrefs.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,53 +31,54 @@
 from bs4 import BeautifulSoup
 from path import Path
 
 from stepup.core.api import amend, getenv
 from stepup.core.utils import mynormpath
 
 
-@attrs.define
-class Config:
-    accept: set[str] = attrs.field(factory=set)
-    subs: list[tuple[str, str]] = attrs.field(factory=list)
-
-
-def main() -> int:
+def main(argv: list[str] | None = None):
     """Main program."""
-    args = parse_args()
+    args = parse_args(argv)
     if args.path_config is None:
         args.path_config = getenv("REPREP_CHECK_HREFS_CONFIG", "check_hrefs.yaml", is_path=True)
-        amend(inp=args.path_config)
+        if not amend(inp=args.path_config):
+            sys.exit(3)
     config = load_config(args.path_config)
     hrefs = collect_hrefs(args.path_src)
     make_url_substitutions(hrefs, config.subs)
-    return check_hrefs(hrefs, Path(args.path_src).parent.normpath(), config.accept)
-
-
-def load_config(path_config) -> Config:
-    converter = cattrs.preconf.pyyaml.PyyamlConverter(forbid_extra_keys=True)
-    with open(path_config) as fh:
-        state = yaml.safe_load(fh)
-        return converter.structure(state, Config)
+    check_hrefs(hrefs, Path(args.path_src).parent.normpath(), config.accept)
 
 
-def parse_args() -> argparse.Namespace:
+def parse_args(argv: list[str] | None = None) -> argparse.Namespace:
     """Parse command-line arguments."""
     parser = argparse.ArgumentParser(
         prog="reprep-check-hrefs", description="Check hyper references Markdown, HTML or PDF files."
     )
     parser.add_argument("path_src", help="Markdown, HTML or PDF file.")
     parser.add_argument(
         "-c",
         "--config",
         dest="path_config",
         help="Configuration yaml file. "
         "The default is ${REPREP_CHECK_HREFS_CONFIG} or check_hrefs.yaml if it is not set.",
     )
-    return parser.parse_args()
+    return parser.parse_args(argv)
+
+
+@attrs.define
+class Config:
+    accept: set[str] = attrs.field(factory=set)
+    subs: list[tuple[str, str]] = attrs.field(factory=list)
+
+
+def load_config(path_config) -> Config:
+    converter = cattrs.preconf.pyyaml.PyyamlConverter(forbid_extra_keys=True)
+    with open(path_config) as fh:
+        state = yaml.safe_load(fh)
+        return converter.structure(state, Config)
 
 
 @attrs.define
 class HRef:
     """A hyper reference to be checked."""
 
     url: str = attrs.field()
@@ -133,35 +134,36 @@
         if "#" in href.url:
             url = url[: href.url.find("#")]
         for pattern, replacement in subs:
             url = re.sub(pattern, replacement, url)
         href.translated = url
 
 
-def check_hrefs(hrefs: list[HRef], root: Path, accept: set[str]) -> int:
+def check_hrefs(hrefs: list[HRef], root: Path, accept: set[str]):
     """Check the hyper references."""
     seen = set()
-    result = 0
+    some_failed = False
     for href in hrefs:
         if href.url in seen:
             continue
-        result |= check_href(href, root, accept)
+        some_failed |= check_href(href, root, accept)
         seen.add(href.url)
-    return result
+    if some_failed:
+        raise ValueError("Some hyper references were invalid.")
 
 
-def check_href(href: HRef, root: Path, accept: set[str]) -> int:
+def check_href(href: HRef, root: Path, accept: set[str]) -> bool:
+    """Check a hyper reference and return True if an error was found."""
     if href.url.startswith("mailto:"):
-        return 0
-    elif "://" in href.translated:
+        return False
+    if "://" in href.translated:
         if href.translated in accept:
-            return 0
-        else:
-            print(f"FAILED LINK: {href.url}", file=sys.stderr)
-            return 1
+            return False
+        print(f"FAILED LINK: {href.url}", file=sys.stderr)
+        return True
     path = mynormpath(root / Path(href.translated))
     amend(inp=path)
-    return 0
+    return False
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `stepup_reprep-1.2.0/stepup/reprep/check_inventory.py` & `stepup_reprep-1.2.1/stepup/reprep/check_inventory.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,16 +40,15 @@
 
 def parse_args(argv: list[str] | None = None) -> argparse.Namespace:
     """Parse command-line arguments."""
     parser = argparse.ArgumentParser(
         prog="reprep-check-inventory", description="Check an inventory.txt."
     )
     parser.add_argument("inventory_txt", help="An inventory.txt file generated with RepRep")
-    args = parser.parse_args(argv)
-    return args
+    return parser.parse_args(argv)
 
 
 def iter_inventory(path_inventory: str) -> Iterator[FileSummary]:
     with open(path_inventory) as fh:
         for iline, line in enumerate(fh):
             try:
                 fs = parse_summary(line)
```

### Comparing `stepup_reprep-1.2.0/stepup/reprep/convert_inkscape.py` & `stepup_reprep-1.2.1/stepup/reprep/convert_inkscape.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,47 +13,46 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
-"""Wrapper for SVG to PDF convrsion."""
+"""Wrapper for SVG to PDF conversion."""
 
 import argparse
 import re
 import sys
+from collections.abc import Iterator
+from xml.etree import ElementTree
 
 from path import Path
 
 from stepup.core.api import getenv, step
 
 
-def main() -> int:
+def main(argv: list[str] | None = None):
     """Main program."""
-    args = parse_args()
+    args = parse_args(argv)
     path_out = Path(args.path_out)
     allowed_extensions = [".pdf", ".png"]
     if not any(path_out.endswith(ext) for ext in allowed_extensions):
-        print(
-            f"The output must have one of the following extensions: {allowed_extensions}",
-            file=sys.stderr,
+        raise ValueError(
+            f"The output must have one of the following extensions: {allowed_extensions}"
         )
-        return -1
     if args.inkscape is None:
         args.inkscape = getenv("REPREP_INKSCAPE", "inkscape")
     if len(args.inkscape_args) == 0:
         inkscape_args = getenv(f"REPREP_INKSCAPE_{path_out.suffix[1:].upper()}_ARGS", "")
     else:
         inkscape_args = " ".join(args.inkscape_args)
     convert_svg_pdf(args.path_svg, path_out, args.inkscape, inkscape_args, args.optional)
-    return 0
 
 
-def parse_args() -> argparse.Namespace:
+def parse_args(argv: list[str] | None = None) -> argparse.Namespace:
     """Parse command-line arguments."""
     parser = argparse.ArgumentParser(
         prog="reprep-convert-inkscape",
         description="Convert an SVG to PDF or PNG, with dependency tracking.",
     )
     parser.add_argument("path_svg", help="The input SVG file.")
     parser.add_argument("path_out", help="The output PDF or PNG file.")
@@ -72,57 +71,74 @@
     )
     parser.add_argument(
         "--optional",
         default=False,
         action="store_true",
         help="With this option, the conversion becomes optional.",
     )
-    return parser.parse_args()
+    return parser.parse_args(argv)
 
 
 def convert_svg_pdf(
     path_svg: str, path_out: Path, inkscape: str, inkscape_args: str, optional: bool
 ):
     inp_paths = search_svg_deps(path_svg)
-    ffmt = path_out.suffix[1:]
+    fmt = path_out.suffix[1:]
     step(
         f"SELF_CALL=x {inkscape} {path_svg} {inkscape_args} "
-        f"--export-filename={path_out} --export-type={ffmt}",
+        f"--export-filename={path_out} --export-type={fmt}",
         inp=[path_svg, *inp_paths],
         out=path_out,
         optional=optional,
     )
 
 
-RE_OPTIONS = re.MULTILINE | re.DOTALL
-RE_SVG_HREF = re.compile(rb"<image\s[^<]*?href=\"(?!#)(?!data:)(.*?)\"[^<]*?>", RE_OPTIONS)
-
-
 def search_svg_deps(src: str) -> list[str]:
     """Search implicit dependencies in SVG files, specifically (recursively) included images."""
     implicit = []
     todo = [src]
     idep = 0
     while idep < len(todo):
         path_svg = Path(todo[idep])
-        # It is generally a poor practice to parse XML with a regular expression,
-        # unless performance becomes an issue...
-        with open(path_svg, "rb") as fh:
-            hrefs = re.findall(RE_SVG_HREF, fh.read())
-
-        # Process hrefs
-        for href in hrefs:
-            href = href.decode("utf-8")
+        for href in iter_svg_image_hrefs(path_svg):
             if href.startswith("file://"):
                 href = href[7:]
             if "://" not in href:
                 if not href.startswith("/"):
                     href = path_svg.parent / href
                 implicit.append(href)
                 if href.endswith(".svg"):
                     todo.append(href)
         idep += 1
     return implicit
 
 
+def iter_svg_image_hrefs(path_svg: str) -> Iterator[str]:
+    parser = ElementTree.iterparse(path_svg, events=("start",))
+    for event, elem in parser:
+        if event == "start":
+            tag = elem.tag.rpartition("}")[2]
+            if tag == "image":
+                for key in "href", "{http://www.w3.org/1999/xlink}href":
+                    href = elem.attrib.get(key)
+                    if href is not None and "data:image" not in href:
+                        yield href
+                        break
+        elem.clear()
+
+
+# TODO: the following can be deleted eventually
+RE_OPTIONS = re.MULTILINE | re.DOTALL
+RE_SVG_HREF = re.compile(rb"<image\s[^<]*?href=\"(?!#)(?!data:)(.*?)\"[^<]*?>", RE_OPTIONS)
+
+
+# TODO: the following can be deleted eventually
+def _iter_svg_image_hrefs(path_svg: str) -> Iterator[str]:
+    # It is generally a poor practice to parse XML with a regular expression,
+    # unless performance becomes an issue...
+    with open(path_svg, "rb") as fh:
+        for href in re.findall(RE_SVG_HREF, fh.read()):
+            yield href.decode("utf-8")
+
+
 if __name__ == "__main__":
-    sys.exit(main())
+    main(sys.argv[1:])
```

### Comparing `stepup_reprep-1.2.0/stepup/reprep/convert_markdown.py` & `stepup_reprep-1.2.1/stepup/reprep/convert_markdown.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,16 +26,38 @@
 import markdown
 
 from .render import render
 
 __all__ = ("convert_markdown",)
 
 
+def main(argv: list[str] | None = None):
+    """Main program."""
+    args = parse_args(argv)
+    if not args.markdown.endswith(".md"):
+        raise ValueError("The markdown file must end with the .md extension.")
+    with open(args.markdown) as fm, open(args.html, "w") as fh:
+        fh.write(convert_markdown(fm.read(), args.katex, args.katex_macros))
+
+
+def parse_args(argv: list[str] | None = None) -> argparse.Namespace:
+    """Parse command-line arguments."""
+    parser = argparse.ArgumentParser(
+        prog="reprep-convert-markdown", description="Convert Markdown to HTML"
+    )
+    parser.add_argument("markdown", help="A Markdown file with extension `.md`")
+    parser.add_argument("html", help="A HTML output filename")
+    parser.add_argument("--katex", default=False, action="store_true", help="Enable KaTeX")
+    parser.add_argument("--katex-macros", default=None, help="KaTeX macro file")
+    return parser.parse_args(argv)
+
+
 HTML_TEMPLATE = """\
 <!DOCTYPE html>
+<html>
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes" />
   <title>{{ title }}</title>
   {{ css | indent(width=2) }}
 </head>
 <body>
@@ -85,37 +107,16 @@
 
     # Convert to HTML
     body = md_ctx.convert(text_md)
     variables = {
         "body": body,
         "title": md_ctx.Meta.get("title", ["Untitled"])[0],
         "css": "\n".join(
-            f'<link rel="stylesheet" href="{path_css}">' for path_css in md_ctx.Meta.get("css", [])
+            f'<link rel="stylesheet" href="{path_css}" />'
+            for path_css in md_ctx.Meta.get("css", [])
         ),
     }
     return render("HTML_TEMPLATE", variables, str_in=HTML_TEMPLATE)
 
 
-def parse_args() -> argparse.Namespace:
-    """Parse command-line arguments."""
-    parser = argparse.ArgumentParser(
-        prog="reprep-convert-markdown", description="Convert Markdown to HTML"
-    )
-    parser.add_argument("markdown", help="A Markdown file with extension `.md`")
-    parser.add_argument("html", help="A HTML output filename")
-    parser.add_argument("--katex", default=False, action="store_true", help="Enable KaTeX")
-    parser.add_argument("--katex-macros", default=None, help="KaTeX macro file")
-    return parser.parse_args()
-
-
-def main() -> int:
-    """Main program."""
-    args = parse_args()
-    if not args.markdown.endswith(".md"):
-        raise ValueError("The markdown file must end with the .md extension.")
-    with open(args.markdown) as fm, open(args.html, "w") as fh:
-        fh.write(convert_markdown(fm.read(), args.katex, args.katex_macros))
-    return 0
-
-
 if __name__ == "__main__":
-    sys.exit(main())
+    main(sys.argv[1:])
```

### Comparing `stepup_reprep-1.2.0/stepup/reprep/inventory.py` & `stepup_reprep-1.2.1/stepup/reprep/inventory.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/stepup/reprep/latex.py` & `stepup_reprep-1.2.1/stepup/reprep/latex.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,17 +30,17 @@
 from stepup.reprep.make_inventory import write_inventory
 
 from .bibtex_log import parse_bibtex_log
 from .latex_deps import scan_latex_deps
 from .latex_log import ErrorInfo, parse_latex_log
 
 
-def main() -> int:
+def main(argv: list[str] | None = None):
     """Main program."""
-    args = parse_args()
+    args = parse_args(argv)
 
     workdir, fn_tex = Path(args.path_tex).splitpath()
     workdir = workdir.normpath()
     if not fn_tex.endswith(".tex"):
         raise ValueError("The LaTeX source must have extension .tex")
     stem = fn_tex[:-4]
     path_aux = workdir / f"{stem}.aux"
@@ -60,15 +60,15 @@
     # Get LaTeX executable
     if args.latex is None:
         args.latex = getenv("REPREP_LATEX", "pdflatex")
 
     aux_digest_hist = []
     if len(bib) == 0:
         if not amend(inp=implicit):
-            return 0
+            sys.exit(3)
         inventory_files = list(implicit)
     elif args.run_bibtex:
         # Get other executables and files
         if args.bibtex is None:
             args.bibtex = getenv("REPREP_BIBTEX", "bibtex")
         if args.bibsane is None:
             args.bibsane = getenv("REPREP_BIBSANE", "bibsane")
@@ -77,15 +77,15 @@
             args.bibsane_config = getenv("REPREP_BIBSANE_CONFIG", "bibsane.yaml", is_path=True)
             paths_config.append(args.bibsane_config)
 
         if not amend(
             inp=implicit + bib + paths_config,
             out=[f"{stem}.bbl"],
         ):
-            return 0
+            sys.exit(3)
         inventory_files = [*implicit, *bib, f"{stem}.bbl"]
 
         # LaTeX
         cp = subprocess.run(
             [
                 args.latex,
                 "-interaction=errorstopmode",
@@ -98,15 +98,15 @@
             check=False,
             cwd=workdir,
         )
         if cp.returncode != 0:
             path_log = workdir / f"{stem}.log"
             error_info = parse_latex_log(path_log)
             error_info.print(path_log)
-            return 1
+            sys.exit(1)
 
         aux_digest_hist.append(compute_file_digest(path_aux))
 
         # BibTeX
         cp = subprocess.run(
             [args.bibtex, stem],
             stdin=subprocess.DEVNULL,
@@ -115,15 +115,15 @@
             check=False,
             cwd=workdir,
         )
         if cp.returncode != 0:
             path_blg = workdir / f"{stem}.blg"
             error_info = parse_bibtex_log(path_blg)
             error_info.print(path_blg)
-            return 2
+            sys.exit(1)
 
         # BibSane
         cp = subprocess.run(
             [args.bibsane, f"{stem}.aux", f"--config={args.bibsane_config}"],
             cwd=workdir,
             text=True,
             stdin=subprocess.DEVNULL,
@@ -131,18 +131,18 @@
             stderr=subprocess.STDOUT,
             check=False,
         )
         if cp.returncode != 0:
             error_info = ErrorInfo("BibSane", src=f"{workdir}/{stem}.aux")
             error_info.print()
             sys.stdout.write(cp.stdout)
-            return 3
+            sys.exit(1)
     else:
         if not amend(inp=[*implicit, f"{stem}.bbl"]):
-            return 0
+            sys.exit(3)
         inventory_files = [*implicit, f"{stem}.bbl"]
 
     for _ in range(args.maxrep):
         # LaTeX
         cp = subprocess.run(
             [args.latex, "-interaction=errorstopmode", stem],
             stdin=subprocess.DEVNULL,
@@ -151,41 +151,41 @@
             check=False,
             cwd=workdir,
         )
         path_log = workdir / f"{stem}.log"
         error_info = parse_latex_log(path_log)
         if cp.returncode != 0:
             error_info.print(path_log)
-            return 4
+            sys.exit(1)
         aux_digest_hist.append(compute_file_digest(path_aux))
         if len(aux_digest_hist) > 1 and aux_digest_hist[-1] == aux_digest_hist[-2]:
             break
     else:
         print(
             f"\033[1;31;40mAux file did not converge in {args.maxrep} iterations!\033[0;0m",
             file=sys.stderr,
         )
         print(path_aux, file=sys.stderr)
         for digest in aux_digest_hist:
             print(digest.hex(), file=sys.stderr)
-        return -3
+        sys.exit(1)
 
     inventory_files.extend([f"{stem}.tex", f"{stem}.aux", f"{stem}.pdf"])
     path_inventory = f"{stem}-inventory.txt"
     write_inventory(path_inventory, inventory_files)
 
     vol_paths = []
     for path in Path(".").glob(f"{stem}.*"):
         path = path.normpath()
         if not (path in inventory_files or path == path_inventory):
             vol_paths.append(path)
     amend(vol=vol_paths)
 
 
-def parse_args() -> argparse.Namespace:
+def parse_args(argv: list[str] | None = None) -> argparse.Namespace:
     """Parse command-line arguments."""
     parser = argparse.ArgumentParser(
         prog="reprep-latex",
         description="Compile a LaTeX document and print essence from log file.",
     )
     parser.add_argument("path_tex", help="The main LaTeX source file.")
     parser.add_argument(
@@ -218,12 +218,12 @@
         "The default is ${REPREP_BIBSANE} or bibsane if the variable is not defined.",
     )
     parser.add_argument(
         "--bibsane-config",
         help="The BibSane configuration file. The default is ${REPREP_BIBSANE_CONFIG} or "
         "bibsane.yaml if the variables is not defined.",
     )
-    return parser.parse_args()
+    return parser.parse_args(argv)
 
 
 if __name__ == "__main__":
-    sys.exit(main())
+    main(sys.argv[1:])
```

### Comparing `stepup_reprep-1.2.0/stepup/reprep/latex_deps.py` & `stepup_reprep-1.2.1/stepup/reprep/latex_deps.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/stepup/reprep/latex_flat.py` & `stepup_reprep-1.2.1/stepup/reprep/latex_flat.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,54 +34,62 @@
 It expects that ``\input`` and ``\import`` commands are the only ones present on their line,
 to avoid ambiguities. If this is not the case, the script will fail.
 The script also assumes the ``\includgraphics``, ``\thebibliography`` and ``\verbatiminput``
 commands are contained within a single line.
 """
 
 import argparse
+import enum
 import re
 import sys
 import tempfile
 from typing import TextIO
 
 from path import Path
 
+from stepup.core.api import amend
 
-def main() -> int:
+
+def main(argv: list[str] | None = None):
     """Main program."""
-    args = parse_args()
+    args = parse_args(argv)
     with tempfile.TemporaryDirectory("reprep-latex-flat") as tmpdir:
         tmpdir = Path(tmpdir)
         path_flat_tmp = tmpdir / "flat.tex"
         with open(path_flat_tmp, "w") as fh_out:
             out_root = Path(args.path_flat).parent
-            result, inp_paths = flatten_latex(args.path_tex, fh_out, out_root)
-        if len(inp_paths) > 0:
-            from stepup.core.api import amend
-
-            amend(inp=inp_paths)
-        if result == 0:
+            status, inp_paths = flatten_latex(args.path_tex, fh_out, out_root)
+        if not amend(inp=inp_paths):
+            sys.exit(3)
+        if status == FlattenStatus.SUCCESS:
             path_flat_tmp.copy(args.path_flat)
-    return result
+        else:
+            sys.exit(1)
 
 
-def parse_args() -> argparse.Namespace:
+def parse_args(argv: list[str] | None = None) -> argparse.Namespace:
     """Parse command-line arguments."""
     parser = argparse.ArgumentParser(
         prog="reprep-latex-flat",
         description="Flatten input and import commands in a LaTeX file.",
     )
     parser.add_argument("path_tex", help="The top-level tex file.")
     parser.add_argument("path_flat", help="The flattened output tex file.")
-    return parser.parse_args()
+    return parser.parse_args(argv)
+
+
+class FlattenStatus(enum.Enum):
+    SUCCESS = 0
+    FILE_NOT_FOUND = 1
+    ILL_FORMATTED = 2
 
 
 def flatten_latex(
     path_tex: str, fh_out: TextIO, out_root: str, tex_root: str | None = None
-) -> tuple[int, list[str]]:
+) -> tuple[FlattenStatus, list[str]]:
     """Write a flattened LaTeX file
 
     Parameters
     ----------
     path_tex
         The LaTeX source to be flattened, may be the main file or
         an included file in one of the recursions.
@@ -91,88 +99,88 @@
         The directory of the output file, needed to fix relative paths.
     tex_root
         The directory with respect to which paths in the LaTeX source must
         be interpreted.
 
     Returns
     -------
-    returncode
-        Zero when successful.
+    success
+        True when successful.
     inp_paths
         A list of additional inputs used.
     """
     inp_paths = []
     path_tex = Path(path_tex)
     tex_root = path_tex.parent.normpath() if tex_root is None else Path(tex_root)
     with open(path_tex) as fh:
         for iline, line in enumerate(fh):
             # Reduce line to standard form
             stripped = line[: line.find("%")].strip()
             stripped = stripped.replace(" ", "").replace("\t", "")
 
             # Try to find input or import
-            status = 0
+            status = FlattenStatus.SUCCESS
             sub_path_tex = None
             new_root = tex_root
             if r"\input{" in stripped:
                 if stripped.startswith(r"\input{") and stripped.endswith("}"):
                     sub_path_tex = tex_root / stripped[7:-1]
                     if not sub_path_tex.endswith(".tex"):
                         sub_path_tex = sub_path_tex.with_suffix(".tex")
                     if not sub_path_tex.is_file():
-                        status = -1
+                        status = FlattenStatus.FILE_NOT_FOUND
                 else:
-                    status = -2
+                    status = FlattenStatus.ILL_FORMATTED
             elif r"\import{" in stripped:
                 if stripped.startswith(r"\import{") and "}{" in stripped and stripped.endswith("}"):
                     new_root, sub_path_tex = stripped[8:-1].split("}{")
                     new_root = (tex_root / new_root).normpath()
                     sub_path_tex = new_root / sub_path_tex
                     if not sub_path_tex.endswith(".tex"):
                         sub_path_tex = sub_path_tex.with_suffix(".tex")
                     if not sub_path_tex.is_file():
-                        status = -1
+                        status = FlattenStatus.FILE_NOT_FOUND
                 else:
-                    status = -2
+                    status = FlattenStatus.ILL_FORMATTED
 
             # Handle result
             if isinstance(sub_path_tex, str):
                 inp_paths.append(sub_path_tex)
-            if status < 0:
-                if status == -1:
+            if status != FlattenStatus.SUCCESS:
+                if status == FlattenStatus.FILE_NOT_FOUND:
                     print(
                         f"Could not locate input file '{sub_path_tex}' "
                         f"on line {iline+1} in '{path_tex}'",
                         file=sys.stderr,
                     )
-                elif status == -2:
+                elif status == FlattenStatus.ILL_FORMATTED:
                     print(
                         f"Could not parse '{stripped}' on line {iline+1} in '{path_tex}'",
                         file=sys.stderr,
                     )
                 else:
                     print("Unknown error", file=sys.stderr)
                 break
-            elif isinstance(sub_path_tex, str):
+            if isinstance(sub_path_tex, str):
                 status, sub_inp_paths = flatten_latex(sub_path_tex, fh_out, out_root, new_root)
                 inp_paths.extend(sub_inp_paths)
-                if status != 0:
+                if status != FlattenStatus.SUCCESS:
                     break
             else:
                 fh_out.write(rewrite_line(line, tex_root, out_root))
     return status, inp_paths
 
 
 RE_REWRITE = re.compile(
     r"(?P<comopt>\\(?:includegraphics|thebibliography|verbatiminput)"
     r"(?:\s*\[.*?])?\s*)\{(?P<path>.*?)}"
 )
 
 
-def rewrite_line(line: str, tex_root: Path, out_root: Path) -> str:
+def rewrite_line(line: str, tex_root: Path, out_root: str) -> str:
     """Rewrite the path in a source line.
 
     Parameters
     ----------
     line
         A line of LaTeX source code, possibly containing ``\\includegraphics``
         or ``\\thebibliography`` commands that need fixing.
@@ -194,8 +202,8 @@
         new_path = (tex_root / old_path).relpath(out_root).normpath()
         return m.group("comopt") + "{" + new_path + "}"
 
     return RE_REWRITE.sub(repl, line)
 
 
 if __name__ == "__main__":
-    sys.exit(main())
+    main(sys.argv[1:])
```

### Comparing `stepup_reprep-1.2.0/stepup/reprep/latex_log.py` & `stepup_reprep-1.2.1/stepup/reprep/latex_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,16 +72,15 @@
     unmatched: bool = attrs.field(init=False, default=False)
 
     @property
     def current(self) -> str:
         """The current file to which the error message belongs."""
         if len(self.stack) == 0:
             return "(could not detect source file)"
-        else:
-            return self.stack[-1]
+        return self.stack[-1]
 
     def feed(self, line: str):
         # Check if we need to anticipate line wrapping
         full = len(line) == 80
         if full:
             # Some exceptions: guess when 80-char lines end exactly with a filename.
             # This is fragile, but LaTeX log files are just a mess to parse.
```

### Comparing `stepup_reprep-1.2.0/stepup/reprep/make_inventory.py` & `stepup_reprep-1.2.1/stepup/reprep/make_inventory.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,16 +87,15 @@
     )
     parser.add_argument(
         "paths",
         nargs="*",
     )
     parser.add_argument("-i", "--inventory-def", help="An inventory input file.", default=None)
     parser.add_argument("-o", "--inventory-txt", help="An inventory output file.", default=None)
-    args = parser.parse_args(argv)
-    return args
+    return parser.parse_args(argv)
 
 
 def get_file_list_nglob(i: int, args: list[str]) -> Collection[str]:
     if len(args) == 0:
         raise ValueError(
             f"Error on line {i} of the inventory input: include or exclude has no arguments."
         )
@@ -197,8 +196,8 @@
     root = path_txt.parent.normpath()
     with open(path_txt, "w") as fh:
         for path in paths:
             print(format_summary(get_summary(path, root)), file=fh)
 
 
 if __name__ == "__main__":
-    sys.exit(main(sys.argv))
+    main(sys.argv[1:])
```

### Comparing `stepup_reprep-1.2.0/stepup/reprep/normalize_pdf.py` & `stepup_reprep-1.2.1/stepup/reprep/normalize_pdf.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,41 +26,39 @@
 
 import fitz
 from path import Path
 
 __all__ = ("pdf_normalize",)
 
 
-def main() -> int:
+def main(argv: list[str] | None = None):
     """Main program."""
-    pdf_normalize(parse_args().path_pdf)
-    return 0
+    pdf_normalize(parse_args(argv).path_pdf)
 
 
-def parse_args() -> argparse.Namespace:
+def parse_args(argv: list[str] | None = None) -> argparse.Namespace:
     """Parse command-line arguments."""
     parser = argparse.ArgumentParser(
-        prog="reprep-mupdf-normalize", description="Normalize a PDF file."
+        prog="reprep-normalize-pdf", description="Normalize a PDF file."
     )
     parser.add_argument("path_pdf", help="The pdf to be normalized (in place).")
-    return parser.parse_args()
+    return parser.parse_args(argv)
 
 
 def pdf_normalize(path_pdf: str):
     """Replace a PDF file by its normalized equivalent. This helps making PDFs reproducible."""
     if not path_pdf.endswith(".pdf"):
-        print(f"The input must have a `.pdf` extension, got: {path_pdf}", file=sys.stderr)
-        return 2
+        raise ValueError(f"The input must have a `.pdf` extension, got: {path_pdf}")
     pdf = fitz.open(path_pdf)
     pdf.set_metadata({})
     pdf.del_xml_metadata()
     pdf.xref_set_key(-1, "ID", "null")
     pdf.scrub()
     with tempfile.TemporaryDirectory(suffix="reprep-normalize-pdf", prefix="rr") as dn:
         path_out = Path(dn) / "out.pdf"
         pdf.save(path_out, garbage=4, deflate=True, linear=True, no_new_id=True)
         pdf.close()
         shutil.copy(path_out, path_pdf)
 
 
 if __name__ == "__main__":
-    sys.exit(main())
+    main(sys.argv[1:])
```

### Comparing `stepup_reprep-1.2.0/stepup/reprep/nup_pdf.py` & `stepup_reprep-1.2.1/stepup/reprep/nup_pdf.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,30 +25,29 @@
 import fitz
 
 from stepup.core.api import getenv
 
 __all__ = ("nup_pdf",)
 
 
-def main() -> int:
+def main(argv: list[str] | None = None):
     """Main program."""
-    args = parse_args()
+    args = parse_args(argv)
     if args.nrow is None:
         args.nrow = int(getenv("REPREP_NUP_NROW", "2"))
     if args.ncol is None:
         args.ncol = int(getenv("REPREP_NUP_NCOL", "2"))
     if args.margin is None:
         args.margin = float(getenv("REPREP_NUP_MARGIN", "10.0"))
     if args.page_format is None:
         args.page_format = getenv("REPREP_NUP_PAGE_FORMAT", "A4-L")
     nup_pdf(args.path_src, args.path_dst, args.nrow, args.ncol, args.margin, args.page_format)
-    return 0
 
 
-def parse_args() -> argparse.Namespace:
+def parse_args(argv: list[str] | None = None) -> argparse.Namespace:
     """Parse command-line arguments."""
     parser = argparse.ArgumentParser(
         prog="reprep-nup-pdf", description="Put multiple pages per sheet using a fixed layout."
     )
     parser.add_argument("path_src", help="The source pdf to which notes should be added.")
     parser.add_argument("path_dst", help="The output pdf.")
     parser.add_argument(
@@ -74,15 +73,15 @@
     )
     parser.add_argument(
         "-p",
         "--page-format",
         help="The output page format. "
         "The default is ${REPREP_NUP_PAGE_FORMAT} or A4-L if the variable is not set.",
     )
-    return parser.parse_args()
+    return parser.parse_args(argv)
 
 
 def nup_pdf(
     path_src: str,
     path_dst: str,
     nrow: int,
     ncol: int,
@@ -104,16 +103,17 @@
     margin
         The margin and (minimal) spacing between small pages in millimeter.
     page_format
         A string describing the output page size.
     """
     for path_pdf in path_src, path_dst:
         if not path_pdf.endswith(".pdf"):
-            print(f"All arguments must have a `.pdf` extension, got: {path_pdf}", file=sys.stderr)
-            return 2
+            raise ValueError(
+                f"All arguments must have a `.pdf` extension, got: {path_pdf}", file=sys.stderr
+            )
     src = fitz.open(path_src)
     dst = fitz.open()
 
     nup = nrow * ncol
     unit = 72 / 25.4
     # Convert distances in mm to points
     margin *= unit
@@ -149,8 +149,8 @@
     dst.save(path_dst, garbage=4, deflate=True, no_new_id=True)
 
     dst.close()
     src.close()
 
 
 if __name__ == "__main__":
-    sys.exit(main())
+    main(sys.argv[1:])
```

### Comparing `stepup_reprep-1.2.0/stepup/reprep/pytest.py` & `stepup_reprep-1.2.1/stepup/reprep/pytest.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/stepup/reprep/raster_pdf.py` & `stepup_reprep-1.2.1/stepup/reprep/raster_pdf.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,48 +29,46 @@
 import fitz
 
 from stepup.core.api import amend
 
 __all__ = ("raster_pdf",)
 
 
-def main() -> int:
+def main(argv: list[str] | None = None):
     """Main program."""
-    args = parse_args()
+    args = parse_args(argv)
     if args.resolution is None:
         amend(env=["REPREP_RASTER_RESOLUTION"])
         args.resolution = int(os.environ.get("REPREP_RASTER_RESOLUTION", "100"))
     if args.quality is None:
         amend(env=["REPREP_RASTER_QUALITY"])
         args.quality = int(os.environ.get("REPREP_RASTER_QUALITY", "50"))
 
     raster_pdf(args.path_inp, args.path_out, args.resolution, args.quality)
     return 0
 
 
-def parse_args() -> argparse.Namespace:
+def parse_args(argv: list[str] | None = None) -> argparse.Namespace:
     """Parse command-line arguments."""
     parser = argparse.ArgumentParser(prog="reprep-raster-pdf", description="Raster a PDF file.")
     parser.add_argument("path_inp", help="The input PDF file.")
     parser.add_argument("path_out", help="The output PDF file.")
     parser.add_argument("-r", "--resolution", type=int, help="Bitmap resolution")
     parser.add_argument("-q", "--quality", type=int, help="JPEG quality")
-    return parser.parse_args()
+    return parser.parse_args(argv)
 
 
 def raster_pdf(path_inp: str, path_out: str, resolution: int, quality: int):
     """Convert a PDF into a rasterized version."""
     if not path_inp.endswith(".pdf"):
-        print(f"The input must have a `.pdf` extension, got: {path_inp}", file=sys.stderr)
-        return 2
+        raise ValueError(f"The input must have a `.pdf` extension, got: {path_inp}")
     if not path_out.endswith(".pdf"):
-        print(f"The output must have a `.pdf` extension, got: {path_out}", file=sys.stderr)
-        return 2
+        raise ValueError(f"The output must have a `.pdf` extension, got: {path_out}")
     if resolution <= 0:
-        print(f"The resolution must be strictly positive, git: {resolution}", file=sys.stderr)
+        raise ValueError(f"The resolution must be strictly positive, git: {resolution}")
     with fitz.open(path_inp) as src:
         dst = fitz.open()
         for src_page in src:
             src_page.wrap_contents()
             if src_page.rotation in (90, 270):
                 height, width = src_page.mediabox_size
             else:
@@ -79,8 +77,8 @@
             stream = pix.tobytes(output="jpg", jpg_quality=quality)
             dst_page = dst.new_page(-1, width, height)
             dst_page.insert_image(dst_page.rect, stream=stream)
         dst.save(path_out, garbage=4, deflate=True, linear=True, no_new_id=True)
 
 
 if __name__ == "__main__":
-    sys.exit(main())
+    main(sys.argv[1:])
```

### Comparing `stepup_reprep-1.2.0/stepup/reprep/render.py` & `stepup_reprep-1.2.1/stepup/reprep/render.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 import jinja2
 from path import Path
 
 from stepup.core.utils import load_module_file
 
 
-def main(argv: list[str]) -> int:
+def main(argv: list[str] | None = None):
     """Main program."""
     args = parse_args(argv)
     if args.mode == "plain":
         latex = False
     elif args.mode == "latex":
         latex = True
     elif args.mode == "auto":
@@ -48,27 +48,27 @@
     variables = load_variables(args.paths_variables, dir_out)
     result = render(args.path_in, variables, latex)
     with open(args.path_out, "w") as fh:
         fh.write(result)
     return 0
 
 
-def parse_args(argv) -> argparse.Namespace:
+def parse_args(argv: list[str] | None = None) -> argparse.Namespace:
     """Parse command-line arguments."""
     parser = argparse.ArgumentParser(prog="reprep-render", description="Render a file with Jinja2.")
     parser.add_argument("path_in", help="The input file")
     parser.add_argument("paths_variables", nargs="+", help="Python files defining variables")
     parser.add_argument("path_out", help="The output file")
     parser.add_argument(
         "--mode",
         choices=["auto", "plain", "latex"],
         help="The delimiter style to use",
         default="auto",
     )
-    return parser.parse_args(argv[1:])
+    return parser.parse_args(argv)
 
 
 def load_variables(paths_variables: list[str], dir_out: str) -> dict[str, str]:
     """Load user-defined variable from Python files.
 
     Parameters
     ----------
@@ -152,8 +152,8 @@
             str_in = f.read()
     template = env.from_string(str_in)
     template.filename = path_template
     return template.render(**variables)
 
 
 if __name__ == "__main__":
-    sys.exit(main(sys.argv))
+    main(sys.argv[1:])
```

### Comparing `stepup_reprep-1.2.0/stepup/reprep/tile_pdf.py` & `stepup_reprep-1.2.1/stepup/reprep/tile_pdf.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/stepup/reprep/zip_inventory.py` & `stepup_reprep-1.2.1/stepup/reprep/zip_inventory.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,8 +113,8 @@
             path_inventory.copy(dst)
             dst.utime((TIMESTAMP, TIMESTAMP))
             fz.write(dst, path_inventory[nskip:], zipfile.ZIP_DEFLATED)
         path_zip_tmp.move(path_zip)
 
 
 if __name__ == "__main__":
-    sys.exit(main())
+    main(sys.argv[1:])
```

### Comparing `stepup_reprep-1.2.0/stepup_reprep.egg-info/PKG-INFO` & `stepup_reprep-1.2.1/stepup_reprep.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stepup-reprep
-Version: 1.2.0
+Version: 1.2.1
 Summary: StepUp RepRep is the StepUp extension for Reproducible Reporting
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 Project-URL: Documentation, https://reproducible-reporting.github.io/stepup-reprep/
 Project-URL: Issues, https://github.com/reproducible-reporting/stepup-reprep/issues
 Project-URL: Source, https://github.com/reproducible-reporting/stepup-reprep/
 Project-URL: Changelog, https://reproducible-reporting.github.io/stepup-reprep/changelog/
 Classifier: Environment :: Console
@@ -24,15 +24,15 @@
 Requires-Dist: markdown
 Requires-Dist: markdown_katex
 Requires-Dist: numpy
 Requires-Dist: path
 Requires-Dist: pymupdf
 Requires-Dist: pyyaml
 Requires-Dist: scipy
-Requires-Dist: stepup>=1.2.3
+Requires-Dist: stepup>=1.2.4
 Requires-Dist: weasyprint
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
```

### Comparing `stepup_reprep-1.2.0/stepup_reprep.egg-info/SOURCES.txt` & `stepup_reprep-1.2.1/stepup_reprep.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 stepup/reprep/add_notes_pdf.py
 stepup/reprep/api.py
 stepup/reprep/bibtex_log.py
 stepup/reprep/check_hrefs.py
 stepup/reprep/check_inventory.py
 stepup/reprep/convert_inkscape.py
 stepup/reprep/convert_markdown.py
+stepup/reprep/convert_weasyprint.py
 stepup/reprep/inventory.py
 stepup/reprep/latex.py
 stepup/reprep/latex_deps.py
 stepup/reprep/latex_flat.py
 stepup/reprep/latex_log.py
 stepup/reprep/make_inventory.py
 stepup/reprep/normalize_pdf.py
@@ -170,19 +171,21 @@
 tests/cases/convert_mutool/expected_graph.txt
 tests/cases/convert_mutool/expected_stdout.txt
 tests/cases/convert_mutool/main.sh
 tests/cases/convert_mutool/plan.py
 tests/cases/convert_mutool/reproducibility_inventory.txt
 tests/cases/convert_weasyprint/.gitignore
 tests/cases/convert_weasyprint/README.md
+tests/cases/convert_weasyprint/block.png
 tests/cases/convert_weasyprint/doc.html
 tests/cases/convert_weasyprint/expected_graph.txt
 tests/cases/convert_weasyprint/expected_stdout.txt
 tests/cases/convert_weasyprint/main.sh
 tests/cases/convert_weasyprint/plan.py
+tests/cases/convert_weasyprint/style.css
 tests/cases/latex_diff/.gitignore
 tests/cases/latex_diff/README.md
 tests/cases/latex_diff/expected_graph.txt
 tests/cases/latex_diff/expected_stdout.txt
 tests/cases/latex_diff/main.sh
 tests/cases/latex_diff/new.tex
 tests/cases/latex_diff/old.tex
```

### Comparing `stepup_reprep-1.2.0/tests/cases/add_notes_pdf/expected_graph.txt` & `stepup_reprep-1.2.1/tests/cases/add_notes_pdf/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/add_notes_pdf/expected_stdout.txt` & `stepup_reprep-1.2.1/tests/cases/add_notes_pdf/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/add_notes_pdf/main.sh` & `stepup_reprep-1.2.1/tests/cases/add_notes_pdf/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/add_notes_pdf/notes.pdf` & `stepup_reprep-1.2.1/tests/cases/add_notes_pdf/notes.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/add_notes_pdf/src.pdf` & `stepup_reprep-1.2.1/tests/cases/add_notes_pdf/src.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/cat_pdf/doc1.pdf` & `stepup_reprep-1.2.1/tests/cases/cat_pdf/doc1.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/cat_pdf/doc2.pdf` & `stepup_reprep-1.2.1/tests/cases/cat_pdf/doc2.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/cat_pdf/expected_graph.txt` & `stepup_reprep-1.2.1/tests/cases/cat_pdf/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/cat_pdf/expected_stdout.txt` & `stepup_reprep-1.2.1/tests/cases/cat_pdf/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/cat_pdf/main.sh` & `stepup_reprep-1.2.1/tests/cases/cat_pdf/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/check_hrefs_html/expected_graph.txt` & `stepup_reprep-1.2.1/tests/cases/check_hrefs_html/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/check_hrefs_html/expected_stdout.txt` & `stepup_reprep-1.2.1/tests/cases/check_hrefs_html/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/check_hrefs_html/main.sh` & `stepup_reprep-1.2.1/tests/cases/check_hrefs_html/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/check_hrefs_html/test.html` & `stepup_reprep-1.2.1/tests/cases/check_hrefs_html/test.html`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/check_hrefs_md/expected_graph.txt` & `stepup_reprep-1.2.1/tests/cases/check_hrefs_md/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/check_hrefs_md/expected_stdout.txt` & `stepup_reprep-1.2.1/tests/cases/check_hrefs_md/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/check_hrefs_md/main.sh` & `stepup_reprep-1.2.1/tests/cases/check_hrefs_md/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/check_hrefs_pdf/expected_graph.txt` & `stepup_reprep-1.2.1/tests/cases/check_hrefs_pdf/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/check_hrefs_pdf/expected_stdout.txt` & `stepup_reprep-1.2.1/tests/cases/check_hrefs_pdf/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/check_hrefs_pdf/main.sh` & `stepup_reprep-1.2.1/tests/cases/check_hrefs_pdf/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/check_hrefs_pdf/main.tex` & `stepup_reprep-1.2.1/tests/cases/check_hrefs_pdf/main.tex`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_inkscape/expected_graph.txt` & `stepup_reprep-1.2.1/tests/cases/convert_inkscape/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_inkscape/expected_stdout.txt` & `stepup_reprep-1.2.1/tests/cases/convert_inkscape/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_inkscape/glasses.svg` & `stepup_reprep-1.2.1/tests/cases/convert_inkscape/glasses.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_inkscape/main.sh` & `stepup_reprep-1.2.1/tests/cases/convert_inkscape/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_inkscape/smile.svg` & `stepup_reprep-1.2.1/tests/cases/convert_inkscape/smile.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_050.svg` & `stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_050.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_055.svg` & `stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_055.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_060.svg` & `stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_060.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_065.svg` & `stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_065.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_070.svg` & `stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_070.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_075.svg` & `stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_075.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_080.svg` & `stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_080.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_085.svg` & `stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_085.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_090.svg` & `stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_090.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_095.svg` & `stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_095.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_100.svg` & `stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_100.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_105.svg` & `stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_105.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_110.svg` & `stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_110.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_115.svg` & `stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_115.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_120.svg` & `stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_120.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_125.svg` & `stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_125.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_130.svg` & `stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_130.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_135.svg` & `stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_135.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_140.svg` & `stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_140.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_145.svg` & `stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/dots_145.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/main.sh` & `stepup_reprep-1.2.1/tests/cases/convert_inkscape_concurrency/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_libreoffice/expected_graph.txt` & `stepup_reprep-1.2.1/tests/cases/convert_libreoffice/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_libreoffice/expected_stdout.txt` & `stepup_reprep-1.2.1/tests/cases/convert_libreoffice/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_libreoffice/main.sh` & `stepup_reprep-1.2.1/tests/cases/convert_libreoffice/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_libreoffice/slide.odp` & `stepup_reprep-1.2.1/tests/cases/convert_libreoffice/slide.odp`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_libreoffice_concurrency/main.sh` & `stepup_reprep-1.2.1/tests/cases/convert_libreoffice_concurrency/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_libreoffice_concurrency/something.odt` & `stepup_reprep-1.2.1/tests/cases/convert_libreoffice_concurrency/something.odt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_markdown/expected_graph.txt` & `stepup_reprep-1.2.1/tests/cases/convert_markdown/expected_graph.txt`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
             supplies   step:./plan.py
             supplies   step:python -m stepup.reprep.convert_markdown demo.md demo.html --katex --katex-macros=macros.tex
 
 step:./plan.py
              workdir = ./
              command = ./plan.py
                state = SUCCEEDED
+        defined pool = markdown_katex=1
           created by   root:
             consumes   file:./
             consumes   file:plan.py
              creates   file:demo.md
              creates   file:macros.tex
              creates   step:python -m stepup.reprep.convert_markdown demo.md demo.html --katex --katex-macros=macros.tex
```

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_markdown/expected_stdout.txt` & `stepup_reprep-1.2.1/tests/cases/convert_markdown/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_markdown/main.sh` & `stepup_reprep-1.2.1/tests/cases/convert_markdown/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_mutool/example.pdf` & `stepup_reprep-1.2.1/tests/cases/convert_mutool/example.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_mutool/expected_graph.txt` & `stepup_reprep-1.2.1/tests/cases/convert_mutool/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_mutool/expected_stdout.txt` & `stepup_reprep-1.2.1/tests/cases/convert_mutool/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_mutool/main.sh` & `stepup_reprep-1.2.1/tests/cases/convert_mutool/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_weasyprint/expected_graph.txt` & `stepup_reprep-1.2.1/tests/cases/convert_weasyprint/expected_graph.txt`

 * *Files 22% similar despite different names*

```diff
@@ -11,44 +11,76 @@
             consumes   file:./
             supplies   step:./plan.py
 
 file:./
                 path = ./
                state = STATIC
           created by   root:
+            supplies   file:block.png
             supplies   file:doc.html
             supplies   file:doc.pdf
             supplies   file:plan.py
+            supplies   file:style.css
             supplies   step:./plan.py
+            supplies   step:python -m stepup.reprep.convert_weasyprint doc.html doc.pdf
             supplies   step:weasyprint doc.html doc.pdf
 
 step:./plan.py
              workdir = ./
              command = ./plan.py
                state = SUCCEEDED
           created by   root:
             consumes   file:./
             consumes   file:plan.py
+             creates   file:block.png
              creates   file:doc.html
-             creates   step:weasyprint doc.html doc.pdf
+             creates   file:style.css
+             creates   step:python -m stepup.reprep.convert_weasyprint doc.html doc.pdf
+
+file:block.png
+                path = block.png
+               state = STATIC
+          created by   step:./plan.py
+            consumes   file:./
+            supplies   step:weasyprint doc.html doc.pdf
 
 file:doc.html
                 path = doc.html
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
+            supplies   step:python -m stepup.reprep.convert_weasyprint doc.html doc.pdf
             supplies   step:weasyprint doc.html doc.pdf
 
+file:style.css
+                path = style.css
+               state = STATIC
+          created by   step:./plan.py
+            consumes   file:./
+            supplies   step:weasyprint doc.html doc.pdf
+
+step:python -m stepup.reprep.convert_weasyprint doc.html doc.pdf
+             workdir = ./
+             command = python -m stepup.reprep.convert_weasyprint doc.html doc.pdf
+               state = SUCCEEDED
+   env_var (amended) = REPREP_WEASYPRINT
+          created by   step:./plan.py
+            consumes   file:./
+            consumes   file:doc.html
+             creates   step:weasyprint doc.html doc.pdf
+
 step:weasyprint doc.html doc.pdf
              workdir = ./
              command = weasyprint doc.html doc.pdf
                state = SUCCEEDED
-          created by   step:./plan.py
+          created by   step:python -m stepup.reprep.convert_weasyprint doc.html doc.pdf
             consumes   file:./
+            consumes   file:block.png
             consumes   file:doc.html
+            consumes   file:style.css
              creates   file:doc.pdf
             supplies   file:doc.pdf
 
 file:doc.pdf
                 path = doc.pdf
                state = BUILT
           created by   step:weasyprint doc.html doc.pdf
```

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_weasyprint/expected_stdout.txt` & `stepup_reprep-1.2.1/tests/cases/convert_weasyprint/expected_stdout.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,13 @@
   DIRECTOR │ Launched worker 0
      PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
+     START │ python -m stepup.reprep.convert_weasyprint doc.html doc.pdf
+   SUCCESS │ python -m stepup.reprep.convert_weasyprint doc.html doc.pdf
      START │ weasyprint doc.html doc.pdf
    SUCCESS │ weasyprint doc.html doc.pdf
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
    DELETED │ doc.pdf
      PHASE │ run
      START │ weasyprint doc.html doc.pdf
```

### Comparing `stepup_reprep-1.2.0/tests/cases/convert_weasyprint/main.sh` & `stepup_reprep-1.2.1/tests/cases/convert_weasyprint/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/latex_diff/expected_graph.txt` & `stepup_reprep-1.2.1/tests/cases/latex_diff/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/latex_diff/expected_stdout.txt` & `stepup_reprep-1.2.1/tests/cases/latex_diff/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/latex_diff/main.sh` & `stepup_reprep-1.2.1/tests/cases/latex_diff/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/latex_flat/expected_graph_01.txt` & `stepup_reprep-1.2.1/tests/cases/latex_flat/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/latex_flat/expected_graph_02.txt` & `stepup_reprep-1.2.1/tests/cases/latex_flat/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/latex_flat/expected_stdout_01.txt` & `stepup_reprep-1.2.1/tests/cases/latex_flat/expected_stdout_01.txt`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
      PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ python -m stepup.reprep.latex_flat article_structured.tex article.tex
 RESCHEDULE │ python -m stepup.reprep.latex_flat article_structured.tex article.tex
 ────────────────────────────────── Step info ───────────────────────────────────
 Command               python -m stepup.reprep.latex_flat article_structured.tex article.tex
-Return code           255
+Return code           3
 ──────────────── Rescheduling due to unavailable amended inputs ────────────────
 sub/other.tex
 ──────────────────────────────── Standard error ────────────────────────────────
 (stripped)
 ────────────────────────────────────────────────────────────────────────────────
    WARNING │ 1 step remains pending due to incomplete requirements
 ───────────────────────────────── PENDING Step ─────────────────────────────────
```

### Comparing `stepup_reprep-1.2.0/tests/cases/latex_flat/main.sh` & `stepup_reprep-1.2.1/tests/cases/latex_flat/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/latex_flat_subdir/expected_graph.txt` & `stepup_reprep-1.2.1/tests/cases/latex_flat_subdir/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/latex_flat_subdir/expected_inventory.txt` & `stepup_reprep-1.2.1/tests/cases/latex_flat_subdir/expected_inventory.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/latex_flat_subdir/main.sh` & `stepup_reprep-1.2.1/tests/cases/latex_flat_subdir/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/lualatex_simple/expected_graph.txt` & `stepup_reprep-1.2.1/tests/cases/lualatex_simple/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/lualatex_simple/expected_stdout.txt` & `stepup_reprep-1.2.1/tests/cases/lualatex_simple/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/lualatex_simple/main.sh` & `stepup_reprep-1.2.1/tests/cases/lualatex_simple/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/make_inventory_list/expected_graph.txt` & `stepup_reprep-1.2.1/tests/cases/make_inventory_list/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/make_inventory_list/main.sh` & `stepup_reprep-1.2.1/tests/cases/make_inventory_list/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/nup_pdf/expected_graph.txt` & `stepup_reprep-1.2.1/tests/cases/nup_pdf/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/nup_pdf/expected_stdout.txt` & `stepup_reprep-1.2.1/tests/cases/nup_pdf/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/nup_pdf/main.sh` & `stepup_reprep-1.2.1/tests/cases/nup_pdf/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/nup_pdf/src.pdf` & `stepup_reprep-1.2.1/tests/cases/nup_pdf/src.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/pdflatex_bbl/expected_graph.txt` & `stepup_reprep-1.2.1/tests/cases/pdflatex_bbl/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/pdflatex_bbl/expected_stdout.txt` & `stepup_reprep-1.2.1/tests/cases/pdflatex_bbl/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/pdflatex_bbl/main.sh` & `stepup_reprep-1.2.1/tests/cases/pdflatex_bbl/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/pdflatex_bibtex/expected_graph.txt` & `stepup_reprep-1.2.1/tests/cases/pdflatex_bibtex/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/pdflatex_bibtex/expected_stdout.txt` & `stepup_reprep-1.2.1/tests/cases/pdflatex_bibtex/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/pdflatex_bibtex/main.sh` & `stepup_reprep-1.2.1/tests/cases/pdflatex_bibtex/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/pdflatex_input/expected_graph.txt` & `stepup_reprep-1.2.1/tests/cases/pdflatex_input/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/pdflatex_input/expected_stdout.txt` & `stepup_reprep-1.2.1/tests/cases/pdflatex_input/expected_stdout.txt`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
      PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ python -m stepup.reprep.latex paper.tex --run-bibtex
 RESCHEDULE │ python -m stepup.reprep.latex paper.tex --run-bibtex
 ────────────────────────────────── Step info ───────────────────────────────────
 Command               python -m stepup.reprep.latex paper.tex --run-bibtex
-Return code           0
+Return code           3
 ──────────────── Rescheduling due to unavailable amended inputs ────────────────
 generated.tex
 ────────────────────────────────────────────────────────────────────────────────
      START │ echo 'Hi there!' > generated.tex
    SUCCESS │ echo 'Hi there!' > generated.tex
      START │ python -m stepup.reprep.latex paper.tex --run-bibtex
    SUCCESS │ python -m stepup.reprep.latex paper.tex --run-bibtex
```

### Comparing `stepup_reprep-1.2.0/tests/cases/pdflatex_input/main.sh` & `stepup_reprep-1.2.1/tests/cases/pdflatex_input/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/pdflatex_input/smile.pdf` & `stepup_reprep-1.2.1/tests/cases/pdflatex_input/smile.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/raster_pdf/expected_graph.txt` & `stepup_reprep-1.2.1/tests/cases/raster_pdf/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/raster_pdf/expected_stdout.txt` & `stepup_reprep-1.2.1/tests/cases/raster_pdf/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/raster_pdf/main.sh` & `stepup_reprep-1.2.1/tests/cases/raster_pdf/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/raster_pdf/smile.pdf` & `stepup_reprep-1.2.1/tests/cases/raster_pdf/smile.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/render_basic/expected_graph.txt` & `stepup_reprep-1.2.1/tests/cases/render_basic/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/render_basic/main.sh` & `stepup_reprep-1.2.1/tests/cases/render_basic/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/render_relpath/expected_graph.txt` & `stepup_reprep-1.2.1/tests/cases/render_relpath/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/render_relpath/expected_stdout.txt` & `stepup_reprep-1.2.1/tests/cases/render_relpath/expected_stdout.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
      START │ python -m stepup.reprep.render main.tex ../variables.py variables.py ../public/main.tex  # wd=static/
    SUCCESS │ python -m stepup.reprep.render main.tex ../variables.py variables.py ../public/main.tex  # wd=static/
      START │ python -m stepup.reprep.latex main.tex --run-bibtex  # wd=public/
 RESCHEDULE │ python -m stepup.reprep.latex main.tex --run-bibtex  # wd=public/
 ────────────────────────────────── Step info ───────────────────────────────────
 Command               python -m stepup.reprep.latex main.tex --run-bibtex
 Working directory     public/
-Return code           0
+Return code           3
 ──────────────── Rescheduling due to unavailable amended inputs ────────────────
 public/preamble.inc.tex
 ────────────────────────────────────────────────────────────────────────────────
      START │ cp -aT static/preamble.inc.tex public/preamble.inc.tex
    SUCCESS │ cp -aT static/preamble.inc.tex public/preamble.inc.tex
      START │ python -m stepup.reprep.latex main.tex --run-bibtex  # wd=public/
    SUCCESS │ python -m stepup.reprep.latex main.tex --run-bibtex  # wd=public/
```

### Comparing `stepup_reprep-1.2.0/tests/cases/render_relpath/main.sh` & `stepup_reprep-1.2.1/tests/cases/render_relpath/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/tile_pdf/expected_graph.txt` & `stepup_reprep-1.2.1/tests/cases/tile_pdf/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/tile_pdf/expected_stdout.txt` & `stepup_reprep-1.2.1/tests/cases/tile_pdf/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/tile_pdf/hexagon.svg` & `stepup_reprep-1.2.1/tests/cases/tile_pdf/hexagon.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/tile_pdf/horizontal.svg` & `stepup_reprep-1.2.1/tests/cases/tile_pdf/horizontal.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/tile_pdf/main.sh` & `stepup_reprep-1.2.1/tests/cases/tile_pdf/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/tile_pdf/pentagon.svg` & `stepup_reprep-1.2.1/tests/cases/tile_pdf/pentagon.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/tile_pdf/square.svg` & `stepup_reprep-1.2.1/tests/cases/tile_pdf/square.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/tile_pdf/tile.py` & `stepup_reprep-1.2.1/tests/cases/tile_pdf/tile.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/tile_pdf/triangle.svg` & `stepup_reprep-1.2.1/tests/cases/tile_pdf/triangle.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/tile_pdf/vera.ttf` & `stepup_reprep-1.2.1/tests/cases/tile_pdf/vera.ttf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/tile_pdf/vertical.svg` & `stepup_reprep-1.2.1/tests/cases/tile_pdf/vertical.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/xelatex_input/expected_graph.txt` & `stepup_reprep-1.2.1/tests/cases/xelatex_input/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/xelatex_input/expected_stdout.txt` & `stepup_reprep-1.2.1/tests/cases/xelatex_input/expected_stdout.txt`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
    SUCCESS │ ./plan.py
      START │ mkdir -p subdir/
    SUCCESS │ mkdir -p subdir/
      START │ python -m stepup.reprep.latex paper.tex --run-bibtex
 RESCHEDULE │ python -m stepup.reprep.latex paper.tex --run-bibtex
 ────────────────────────────────── Step info ───────────────────────────────────
 Command               python -m stepup.reprep.latex paper.tex --run-bibtex
-Return code           0
+Return code           3
 ──────────────── Rescheduling due to unavailable amended inputs ────────────────
 subdir/generated.tex
 ────────────────────────────────────────────────────────────────────────────────
      START │ echo '2 + 2' > subdir/code.txt
    SUCCESS │ echo '2 + 2' > subdir/code.txt
      START │ echo 'Verbatim input:\verbatiminput{code.txt}' > subdir/generated.tex
    SUCCESS │ echo 'Verbatim input:\verbatiminput{code.txt}' > subdir/generated.tex
```

### Comparing `stepup_reprep-1.2.0/tests/cases/xelatex_input/main.sh` & `stepup_reprep-1.2.1/tests/cases/xelatex_input/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/xelatex_input/smile.pdf` & `stepup_reprep-1.2.1/tests/cases/xelatex_input/smile.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/zip_inventory/expected_graph.txt` & `stepup_reprep-1.2.1/tests/cases/zip_inventory/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/zip_inventory/expected_stdout.txt` & `stepup_reprep-1.2.1/tests/cases/zip_inventory/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/cases/zip_inventory/main.sh` & `stepup_reprep-1.2.1/tests/cases/zip_inventory/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/conftest.py` & `stepup_reprep-1.2.1/tests/conftest.py`

 * *Files 24% similar despite different names*

```diff
@@ -21,10 +21,10 @@
 
 import pytest
 from path import Path
 
 pytest.register_assert_rewrite("stepup.core.pytest", "stepup.reprep.pytest")
 
 
-@pytest.fixture
+@pytest.fixture()
 def path_tmp(tmpdir: str) -> Path:
     return Path(tmpdir)
```

### Comparing `stepup_reprep-1.2.0/tests/reprep_common.py` & `stepup_reprep-1.2.1/tests/reprep_common.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/test_bibtex_log.py` & `stepup_reprep-1.2.1/tests/test_bibtex_log.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/test_cases.py` & `stepup_reprep-1.2.1/tests/test_cases.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         "make_inventory_list",
         "nup_pdf",
         "raster_pdf",
         "render_basic",
         "zip_inventory",
     ],
 )
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_example(tmpdir, name: str):
     await run_example(Path("tests/cases") / name, tmpdir, OVERWRITE_EXPECTED)
 
 
 def has_texlive_2023():
     if not shutil.which("lualatex"):
         return False
@@ -91,40 +91,40 @@
         "pdflatex_bbl",
         "pdflatex_bibtex",
         "pdflatex_input",
         "render_relpath",
         "xelatex_input",
     ],
 )
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_latex_example(tmpdir, name: str):
     await run_example(Path("tests/cases") / name, tmpdir, OVERWRITE_EXPECTED)
 
 
 @pytest.mark.skipif(not shutil.which("inkscape"), reason="No Inkscape")
 @pytest.mark.parametrize(
     "name",
     ["convert_inkscape", "convert_inkscape_concurrency", "tile_pdf"],
 )
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_inkscape_example(tmpdir, name: str):
     await run_example(Path("tests/cases") / name, tmpdir, OVERWRITE_EXPECTED)
 
 
 @pytest.mark.skipif(not shutil.which("mutool"), reason="No Mutool")
 @pytest.mark.parametrize(
     "name",
     ["convert_mutool", "cat_pdf"],
 )
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_mutool_example(tmpdir, name: str):
     await run_example(Path("tests/cases") / name, tmpdir, OVERWRITE_EXPECTED)
 
 
 @pytest.mark.skipif(not shutil.which("libreoffice"), reason="No LibreOffice")
 @pytest.mark.parametrize(
     "name",
     ["convert_libreoffice", "convert_libreoffice_concurrency"],
 )
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_libreoffice_example(tmpdir, name: str):
     await run_example(Path("tests/cases") / name, tmpdir, OVERWRITE_EXPECTED)
```

### Comparing `stepup_reprep-1.2.0/tests/test_inventory.py` & `stepup_reprep-1.2.1/tests/test_inventory.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/test_latex_deps.py` & `stepup_reprep-1.2.1/tests/test_latex_deps.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/test_latex_flat.py` & `stepup_reprep-1.2.1/tests/test_latex_flat.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.2.0/tests/test_latex_log.py` & `stepup_reprep-1.2.1/tests/test_latex_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,15 +267,15 @@
         lss.feed(line + "\n")
     assert lss.stack == stack
     assert lss.unfinished == unfinished
     assert not lss.unmatched
 
 
 @pytest.mark.parametrize(
-    "nline, stack, unfinished",
+    ("nline", "stack", "unfinished"),
     [
         (7, ["./solutions.tex"], None),
         (
             9,
             ["./solutions.tex"],
             "L3 programming layer <2022-12-17> (/usr/share/texlive/texmf-dist/tex/latex/base",
         ),
@@ -376,15 +376,15 @@
 Package: infwarerr 2019/12/03 v1.5 Providing info/warning/error messages (HO)
 )
 )
 """
 
 
 @pytest.mark.parametrize(
-    "nline, stack, unfinished",
+    ("nline", "stack", "unfinished"),
     [
         (2, ["./pdftexcmds.sty"], None),
         (
             3,
             ["./pdftexcmds.sty"],
             "Package: pdftexcmds 2020-06-27 v0.33 Utility functions of pdfTeX for LuaTeX (HO",
         ),
@@ -403,15 +403,15 @@
 (/usr/share/texlive/texmf-dist/tex/generic/pgf/basiclayer/pgfcorequick.code.tex
 File: pgfcorequick.code.tex 2021/05/15 v3.1.9a (3.1.9a)
 )
 """
 
 
 @pytest.mark.parametrize(
-    "nline, stack, unfinished",
+    ("nline", "stack", "unfinished"),
     [
         (
             3,
             ["/usr/share/texlive/texmf-dist/tex/generic/pgf/basiclayer/pgfcorequick.code.tex"],
             None,
         ),
     ],
@@ -425,15 +425,15 @@
 Bluh
 (./second.tex))
 Blah
 """
 
 
 @pytest.mark.parametrize(
-    "nline, stack, unfinished",
+    ("nline", "stack", "unfinished"),
     [
         (2, ["./first.tex"], None),
         (3, ["./first.tex"], None),
         (4, [], None),
         (5, [], None),
     ],
 )
```

### Comparing `stepup_reprep-1.2.0/tests/test_zip.py` & `stepup_reprep-1.2.1/tests/test_zip.py`

 * *Files identical despite different names*

