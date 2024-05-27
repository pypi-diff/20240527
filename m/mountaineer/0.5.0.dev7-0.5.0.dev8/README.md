# Comparing `tmp/mountaineer-0.5.0.dev7.tar.gz` & `tmp/mountaineer-0.5.0.dev8.tar.gz`

## Comparing `mountaineer-0.5.0.dev7.tar` & `mountaineer-0.5.0.dev8.tar`

### file list

```diff
@@ -1,296 +1,296 @@
--rw-r--r--   0     1001      127      269 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/src_go/Cargo.toml
--rw-r--r--   0     1001      127     1995 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/src_go/build.rs
--rw-r--r--   0     1001      127     4195 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/src_go/go/js_build.go
--rw-r--r--   0     1001      127      168 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/src_go/go.mod
--rw-r--r--   0     1001      127      376 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/src_go/go.sum
--rw-r--r--   0     1001      127     6499 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/src_go/src/lib.rs
--rw-r--r--   0        0        0     1055 1970-01-01 00:00:00.000000 mountaineer-0.5.0.dev7/Cargo.toml
--rw-r--r--   0     1001      127      133 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/.git-blame-ignore-revs
--rw-r--r--   0     1001      127      138 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/.gitattributes
--rw-r--r--   0     1001      127        0 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/.github/README_SCRIPTS.md
--rw-r--r--   0     1001      127    15100 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/.github/poetry.lock
--rw-r--r--   0     1001      127      767 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/.github/pyproject.toml
--rw-r--r--   0     1001      127        0 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/.github/scripts/__init__.py
--rw-r--r--   0     1001      127     3032 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/.github/scripts/__tests__/test_update_version.py
--rw-r--r--   0     1001      127     2181 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/.github/scripts/check_dependencies.py
--rw-r--r--   0     1001      127     3382 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/.github/scripts/update_version.py
--rw-r--r--   0     1001      127     1321 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/.github/workflows/publish_docs.yml
--rw-r--r--   0     1001      127    20647 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/.github/workflows/test.yml
--rw-r--r--   0     1001      127      504 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/.github/workflows/validate.yml
--rw-r--r--   0     1001      127     3414 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/.gitignore
--rw-r--r--   0     1001      127     1750 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/Dockerfile
--rw-r--r--   0     1001      127     1079 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/LICENSE
--rw-r--r--   0     1001      127     5159 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/Makefile
--rw-r--r--   0     1001      127    14891 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/README.md
--rw-r--r--   0     1001      127      105 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/benchmarking/README.md
--rw-r--r--   0     1001      127        0 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/benchmarking/benchmarking/__init__.py
--rw-r--r--   0     1001      127      425 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/benchmarking/benchmarking/simple_render.py
--rw-r--r--   0     1001      127   127218 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/benchmarking/poetry.lock
--rw-r--r--   0     1001      127      291 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/benchmarking/pyproject.toml
--rw-r--r--   0     1001      127      850 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/ci_webapp/README.md
--rw-r--r--   0     1001      127        1 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/__init__.py
--rw-r--r--   0     1001      127      886 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/app.py
--rw-r--r--   0     1001      127      603 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/cli.py
--rw-r--r--   0     1001      127      111 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/config.py
--rw-r--r--   0     1001      127        1 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/controllers/__init__.py
--rw-r--r--   0     1001      127     1433 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/controllers/complex.py
--rw-r--r--   0     1001      127      581 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/controllers/detail.py
--rw-r--r--   0     1001      127     1658 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/controllers/home.py
--rw-r--r--   0     1001      127      649 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/controllers/root_layout.py
--rw-r--r--   0     1001      127      559 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/controllers/stream.py
--rw-r--r--   0     1001      127       77 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/main.py
--rw-r--r--   0     1001      127      208 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/views/__init__.py
--rw-r--r--   0     1001      127     2261 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/views/app/complex/page.tsx
--rw-r--r--   0     1001      127      453 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/views/app/detail/page.tsx
--rw-r--r--   0     1001      127     2822 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/views/app/home/page.tsx
--rw-r--r--   0     1001      127      645 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/views/app/layout.tsx
--rw-r--r--   0     1001      127       59 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/views/app/main.css
--rw-r--r--   0     1001      127      708 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/views/app/stream/page.tsx
--rw-r--r--   0     1001      127   125408 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/views/package-lock.json
--rw-r--r--   0     1001      127      453 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/views/package.json
--rw-r--r--   0     1001      127       83 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/views/postcss.config.js
--rw-r--r--   0     1001      127      161 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/views/tailwind.config.js
--rw-r--r--   0     1001      127   111131 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/ci_webapp/poetry.lock
--rw-r--r--   0     1001      127      754 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/ci_webapp/pyproject.toml
--rw-r--r--   0     1001      127     1593 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/README.md
--rw-r--r--   0     1001      127        1 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/__init__.py
--rw-r--r--   0     1001      127        0 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/__tests__/__init__.py
--rw-r--r--   0     1001      127     1055 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/__tests__/common.py
--rw-r--r--   0     1001      127     8021 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py
--rw-r--r--   0     1001      127      292 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/__tests__/test_cli.py
--rw-r--r--   0     1001      127      816 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py
--rw-r--r--   0     1001      127     4277 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/builder.py
--rw-r--r--   0     1001      127     4656 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/cli.py
--rw-r--r--   0     1001      127        0 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/environments/__init__.py
--rw-r--r--   0     1001      127     1383 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/environments/base.py
--rw-r--r--   0     1001      127     4591 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/environments/poetry.py
--rw-r--r--   0     1001      127     1832 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/environments/venv.py
--rw-r--r--   0     1001      127     1336 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/external.py
--rw-r--r--   0     1001      127     1919 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/generation.py
--rw-r--r--   0     1001      127      327 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/io.py
--rw-r--r--   0     1001      127       30 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/.zed/settings.json
--rw-r--r--   0     1001      127      212 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/__init__.py
--rw-r--r--   0     1001      127      246 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vim/.vimrc
--rw-r--r--   0     1001      127      162 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vscode/.vscode/settings.json
--rw-r--r--   0     1001      127      109 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/zed/pyrightconfig.json
--rw-r--r--   0     1001      127      170 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/project/.env
--rw-r--r--   0     1001      127     3383 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore
--rw-r--r--   0     1001      127      645 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/project/README.md
--rw-r--r--   0     1001      127       17 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/__init__.py
--rw-r--r--   0     1001      127      767 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py
--rw-r--r--   0     1001      127      947 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py
--rw-r--r--   0     1001      127      282 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/config.py
--rw-r--r--   0     1001      127      227 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/__init__.py
--rw-r--r--   0     1001      127     1702 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py
--rw-r--r--   0     1001      127     1124 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py
--rw-r--r--   0     1001      127       84 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/main.py
--rw-r--r--   0     1001      127      157 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/__init__.py
--rw-r--r--   0     1001      127      208 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/detail.py
--rw-r--r--   0     1001      127        0 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/__init__.py
--rw-r--r--   0     1001      127     1219 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx
--rw-r--r--   0     1001      127      995 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx
--rw-r--r--   0     1001      127       95 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/main.css
--rw-r--r--   0     1001      127      524 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json
--rw-r--r--   0     1001      127      117 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/postcss.config.js
--rw-r--r--   0     1001      127      195 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/tailwind.config.js
--rw-r--r--   0     1001      127      332 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/project/docker-compose.yml
--rw-r--r--   0     1001      127     1493 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml
--rw-r--r--   0     1001      127    63125 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/poetry.lock
--rw-r--r--   0     1001      127     1318 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/create_mountaineer_app/pyproject.toml
--rw-r--r--   0     1001      127      324 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docker-compose.test.yml
--rw-r--r--   0     1001      127       30 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/.zed/settings.json
--rw-r--r--   0     1001      127      107 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/README.md
--rw-r--r--   0     1001      127       15 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/CNAME
--rw-r--r--   0     1001      127      318 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/api/actions.md
--rw-r--r--   0     1001      127      454 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/api/api_exception.md
--rw-r--r--   0     1001      127       99 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/api/app-controller.md
--rw-r--r--   0     1001      127      281 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/api/build_plugins/base.md
--rw-r--r--   0     1001      127       57 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/api/build_plugins/javascript.md
--rw-r--r--   0     1001      127       62 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/api/build_plugins/postcss.md
--rw-r--r--   0     1001      127      411 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/api/cli.md
--rw-r--r--   0     1001      127      376 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/api/config.md
--rw-r--r--   0     1001      127      138 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/api/controller.md
--rw-r--r--   0     1001      127       67 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/api/core_dependencies.md
--rw-r--r--   0     1001      127       66 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/api/database/config.md
--rw-r--r--   0     1001      127       71 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/api/database/dependencies.md
--rw-r--r--   0     1001      127      507 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/api/database/migrations.md
--rw-r--r--   0     1001      127       80 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/api/logging.md
--rw-r--r--   0     1001      127      479 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/api/render.md
--rw-r--r--   0     1001      127      365 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/api/ssr.md
--rw-r--r--   0     1001      127      299 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/api/watch_server.md
--rw-r--r--   0     1001      127     9379 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/client_actions.md
--rw-r--r--   0     1001      127      753 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/cma.md
--rw-r--r--   0     1001      127     3021 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/database.md
--rw-r--r--   0     1001      127     8216 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/database_migrations.md
--rw-r--r--   0     1001      127     4690 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/deploy.md
--rw-r--r--   0     1001      127     7698 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/error_handling.md
--rw-r--r--   0     1001      127     1081 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/index.md
--rw-r--r--   0     1001      127     1541 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/internal/core_library.md
--rw-r--r--   0     1001      127     2156 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/links.md
--rw-r--r--   0     1001      127   365251 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/media/final_todo_list.png
--rw-r--r--   0     1001      127   148261 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/media/ide_typehints.png
--rw-r--r--   0     1001      127   545494 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/media/network_debug.png
--rw-r--r--   0     1001      127   346903 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/media/server_side_rendering.png
--rw-r--r--   0     1001      127     2263 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/metadata.md
--rw-r--r--   0     1001      127     2347 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/postcss.md
--rw-r--r--   0     1001      127    12263 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/quickstart.md
--rw-r--r--   0     1001      127     4875 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/static_analysis.md
--rw-r--r--   0     1001      127     2490 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/structure.md
--rw-r--r--   0     1001      127     1219 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/stylesheets/extra.css
--rw-r--r--   0     1001      127     9534 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/docs/views.md
--rw-r--r--   0     1001      127     1887 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/mkdocs.yml
--rw-r--r--   0     1001      127      109 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/overrides/partials/footer.html
--rw-r--r--   0     1001      127   156250 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/poetry.lock
--rw-r--r--   0     1001      127      500 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/docs_website/pyproject.toml
--rw-r--r--   0     1001      127   675789 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/media/header.png
--rw-r--r--   0     1001      127     1103 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__init__.py
--rw-r--r--   0     1001      127        0 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/__init__.py
--rw-r--r--   0     1001      127        0 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/actions/__init__.py
--rw-r--r--   0     1001      127     8123 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/actions/test_fields.py
--rw-r--r--   0     1001      127     9711 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/actions/test_passthrough_dec.py
--rw-r--r--   0     1001      127     9086 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/actions/test_sideeffect_dec.py
--rw-r--r--   0     1001      127        0 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/client_builder/__init__.py
--rw-r--r--   0     1001      127    14334 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/client_builder/test_build_actions.py
--rw-r--r--   0     1001      127     5031 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/client_builder/test_build_links.py
--rw-r--r--   0     1001      127    10127 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/client_builder/test_build_schemas.py
--rw-r--r--   0     1001      127     6322 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/client_builder/test_builder.py
--rw-r--r--   0     1001      127     4818 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/client_builder/test_typescript.py
--rw-r--r--   0     1001      127      319 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/common.py
--rw-r--r--   0     1001      127      497 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/conftest.py
--rw-r--r--   0     1001      127        0 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/database/__init__.py
--rw-r--r--   0     1001      127        0 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/database/dependencies/__init__.py
--rw-r--r--   0     1001      127      208 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/database/dependencies/conftest.py
--rw-r--r--   0     1001      127      801 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/database/dependencies/test_core.py
--rw-r--r--   0     1001      127      627 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/database/test_config.py
--rw-r--r--   0     1001      127      616 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/database/test_sqlmodel.py
--rw-r--r--   0     1001      127        0 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/dependencies/__init__.py
--rw-r--r--   0     1001      127     2567 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/dependencies/test_base.py
--rw-r--r--   0     1001      127      211 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/fixtures/__init__.py
--rw-r--r--   0     1001      127   571338 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js
--rw-r--r--   0     1001      127  1638568 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/fixtures/home_controller_source_map.js.map
--rw-r--r--   0     1001      127   575422 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js
--rw-r--r--   0     1001      127        0 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/js_compiler/__init__.py
--rw-r--r--   0     1001      127     9973 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/js_compiler/test_javascript.py
--rw-r--r--   0     1001      127      808 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/js_compiler/test_postcss.py
--rw-r--r--   0     1001      127     2823 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/js_compiler/test_source_maps.py
--rw-r--r--   0     1001      127        0 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/migrations/__init__.py
--rw-r--r--   0     1001      127     4187 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/migrations/conftest.py
--rw-r--r--   0     1001      127    23753 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/migrations/test_actions.py
--rw-r--r--   0     1001      127     5242 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/migrations/test_db_memory_serializer.py
--rw-r--r--   0     1001      127    12619 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/migrations/test_db_serializer.py
--rw-r--r--   0     1001      127      795 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/migrations/test_db_stubs.py
--rw-r--r--   0     1001      127     4527 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/migrations/test_generator.py
--rw-r--r--   0     1001      127     2672 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/migrations/test_generics.py
--rw-r--r--   0     1001      127    11671 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/migrations/test_handlers.py
--rw-r--r--   0     1001      127     1236 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/test_annotation_helpers.py
--rw-r--r--   0     1001      127    12749 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/test_app.py
--rw-r--r--   0     1001      127     3021 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/test_cache.py
--rw-r--r--   0     1001      127     5304 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/test_cli.py
--rw-r--r--   0     1001      127     2301 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/test_compat.py
--rw-r--r--   0     1001      127      494 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/test_config.py
--rw-r--r--   0     1001      127     6824 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/test_controller.py
--rw-r--r--   0     1001      127     1126 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/test_controller_layout.py
--rw-r--r--   0     1001      127     3239 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/test_cropper.py
--rw-r--r--   0     1001      127     1227 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/test_exceptions.py
--rw-r--r--   0     1001      127      583 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/test_generics.py
--rw-r--r--   0     1001      127     1065 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/test_io.py
--rw-r--r--   0     1001      127     1924 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/test_logging.py
--rw-r--r--   0     1001      127     8494 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/test_paths.py
--rw-r--r--   0     1001      127     2667 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/test_ssr.py
--rw-r--r--   0     1001      127     3177 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/__tests__/test_watch.py
--rw-r--r--   0     1001      127      405 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/actions/__init__.py
--rw-r--r--   0     1001      127    12444 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/actions/fields.py
--rw-r--r--   0     1001      127     6841 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/actions/passthrough_dec.py
--rw-r--r--   0     1001      127    11993 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/actions/sideeffect_dec.py
--rw-r--r--   0     1001      127     4671 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/annotation_helpers.py
--rw-r--r--   0     1001      127    28407 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/app.py
--rw-r--r--   0     1001      127     4523 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/cache.py
--rw-r--r--   0     1001      127    19195 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/cli.py
--rw-r--r--   0     1001      127    11390 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/client_builder/build_actions.py
--rw-r--r--   0     1001      127     4002 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/client_builder/build_links.py
--rw-r--r--   0     1001      127    10296 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/client_builder/build_schemas.py
--rw-r--r--   0     1001      127    30960 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/client_builder/builder.py
--rw-r--r--   0     1001      127    11429 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/client_builder/openapi.py
--rw-r--r--   0     1001      127     5629 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/client_builder/typescript.py
--rw-r--r--   0     1001      127     1808 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/compat.py
--rw-r--r--   0     1001      127     2424 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/config.py
--rw-r--r--   0     1001      127      197 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/console.py
--rw-r--r--   0     1001      127       40 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/constants.py
--rw-r--r--   0     1001      127    16758 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/controller.py
--rw-r--r--   0     1001      127      881 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/controller_layout.py
--rw-r--r--   0     1001      127        0 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/controllers/__init__.py
--rw-r--r--   0     1001      127     1216 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/controllers/exception_controller.py
--rw-r--r--   0     1001      127    10375 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/cropper.py
--rw-r--r--   0     1001      127      327 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/database/__init__.py
--rw-r--r--   0     1001      127     1866 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/database/cli.py
--rw-r--r--   0     1001      127     1822 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/database/config.py
--rw-r--r--   0     1001      127      133 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/database/dependencies/__init__.py
--rw-r--r--   0     1001      127     3425 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/database/dependencies/core.py
--rw-r--r--   0     1001      127     7969 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/database/sqlmodel.py
--rw-r--r--   0     1001      127     8737 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/database/validator.py
--rw-r--r--   0     1001      127      251 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/dependencies/__init__.py
--rw-r--r--   0     1001      127     5122 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/dependencies/base.py
--rw-r--r--   0     1001      127      116 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/dependencies/core/__init__.py
--rw-r--r--   0     1001      127     1069 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/dependencies/core/core.py
--rw-r--r--   0     1001      127     3317 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/exceptions.py
--rw-r--r--   0     1001      127     1740 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/generics.py
--rw-r--r--   0     1001      127     1781 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/io.py
--rw-r--r--   0     1001      127        1 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/js_compiler/__init__.py
--rw-r--r--   0     1001      127     1731 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/js_compiler/base.py
--rw-r--r--   0     1001      127      199 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/js_compiler/exceptions.py
--rw-r--r--   0     1001      127    17413 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/js_compiler/javascript.py
--rw-r--r--   0     1001      127     4163 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/js_compiler/postcss.py
--rw-r--r--   0     1001      127     5614 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/js_compiler/source_maps.py
--rw-r--r--   0     1001      127     2313 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/logging.py
--rw-r--r--   0     1001      127        0 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/migrations/__init__.py
--rw-r--r--   0     1001      127    20278 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/migrations/actions.py
--rw-r--r--   0     1001      127     8239 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/migrations/cli.py
--rw-r--r--   0     1001      127     2319 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/migrations/client_io.py
--rw-r--r--   0     1001      127     8866 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/migrations/db_memory_serializer.py
--rw-r--r--   0     1001      127    10101 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/migrations/db_serializer.py
--rw-r--r--   0     1001      127    12263 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/migrations/db_stubs.py
--rw-r--r--   0     1001      127       99 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/migrations/dependency/__init__.py
--rw-r--r--   0     1001      127       47 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/migrations/dependency/core/__init__.py
--rw-r--r--   0     1001      127      356 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/migrations/dependency/core/core.py
--rw-r--r--   0     1001      127     8619 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/migrations/generator.py
--rw-r--r--   0     1001      127     3078 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/migrations/generics.py
--rw-r--r--   0     1001      127    25065 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/migrations/handlers.py
--rw-r--r--   0     1001      127     1926 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/migrations/migration.py
--rw-r--r--   0     1001      127     3994 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/migrations/migrator.py
--rw-r--r--   0     1001      127    13337 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/paths.py
--rw-r--r--   0     1001      127        0 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/py.typed
--rw-r--r--   0     1001      127     5816 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/render.py
--rw-r--r--   0     1001      127     3237 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/ssr.py
--rw-r--r--   0     1001      127      210 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/static/__init__.py
--rw-r--r--   0     1001      127     6556 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/static/api.ts
--rw-r--r--   0     1001      127     3976 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/static/live_reload.ts
--rw-r--r--   0     1001      127      323 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/static/ssr_polyfills.js
--rw-r--r--   0     1001      127     7261 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/test_utilities.py
--rw-r--r--   0     1001      127      213 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/views/__init__.py
--rw-r--r--   0     1001      127      432 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/views/core/exception/page.tsx
--rw-r--r--   0     1001      127      178 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/views/core/layout.tsx
--rw-r--r--   0     1001      127       59 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/views/core/main.css
--rw-r--r--   0     1001      127     1478 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/views/package-lock.json
--rw-r--r--   0     1001      127      257 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/views/package.json
--rw-r--r--   0     1001      127       83 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/views/postcss.config.js
--rw-r--r--   0     1001      127      162 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/views/tailwind.config.js
--rw-r--r--   0     1001      127     8427 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/watch.py
--rw-r--r--   0     1001      127     4062 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/watch_server.py
--rw-r--r--   0     1001      127     1213 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/mountaineer/webservice.py
--rw-r--r--   0     1001      127   129036 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/poetry.lock
--rw-r--r--   0     1001      127   453080 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/src/benches/fixtures/complex_sourcemap_mapping.txt
--rw-r--r--   0     1001      127   575422 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/src/benches/fixtures/home_controller_ssr_with_react.js
--rw-r--r--   0     1001      127      322 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/src/benches/fixtures/ssr_polyfill_archive.js
--rw-r--r--   0     1001      127      899 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/src/benches/lexers_benchmark.rs
--rw-r--r--   0     1001      127     1089 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/src/benches/source_map_benchmark.rs
--rw-r--r--   0     1001      127     1595 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/src/benches/ssr_benchmark.rs
--rw-r--r--   0     1001      127      499 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/src/errors.rs
--rw-r--r--   0     1001      127     4648 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/src/lexers.rs
--rw-r--r--   0     1001      127     9118 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/src/lib.rs
--rw-r--r--   0     1001      127      680 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/src/logging.rs
--rw-r--r--   0     1001      127    17549 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/src/source_map.rs
--rw-r--r--   0     1001      127    15113 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/src/ssr.rs
--rw-r--r--   0     1001      127     3998 2024-05-23 03:52:05.000000 mountaineer-0.5.0.dev7/src/timeout.rs
--rw-r--r--   0     1001      127    32093 2024-05-23 03:52:22.000000 mountaineer-0.5.0.dev7/Cargo.lock
--rw-r--r--   0     1001      127     1624 2024-05-23 03:52:19.000000 mountaineer-0.5.0.dev7/pyproject.toml
--rw-r--r--   0        0        0    15354 1970-01-01 00:00:00.000000 mountaineer-0.5.0.dev7/PKG-INFO
+-rw-r--r--   0     1001      127      269 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/src_go/Cargo.toml
+-rw-r--r--   0     1001      127     1995 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/src_go/build.rs
+-rw-r--r--   0     1001      127     4195 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/src_go/go/js_build.go
+-rw-r--r--   0     1001      127      168 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/src_go/go.mod
+-rw-r--r--   0     1001      127      376 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/src_go/go.sum
+-rw-r--r--   0     1001      127     6499 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/src_go/src/lib.rs
+-rw-r--r--   0        0        0     1055 1970-01-01 00:00:00.000000 mountaineer-0.5.0.dev8/Cargo.toml
+-rw-r--r--   0     1001      127      133 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/.git-blame-ignore-revs
+-rw-r--r--   0     1001      127      138 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/.gitattributes
+-rw-r--r--   0     1001      127        0 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/.github/README_SCRIPTS.md
+-rw-r--r--   0     1001      127    15100 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/.github/poetry.lock
+-rw-r--r--   0     1001      127      767 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/.github/pyproject.toml
+-rw-r--r--   0     1001      127        0 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/.github/scripts/__init__.py
+-rw-r--r--   0     1001      127     3032 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/.github/scripts/__tests__/test_update_version.py
+-rw-r--r--   0     1001      127     2181 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/.github/scripts/check_dependencies.py
+-rw-r--r--   0     1001      127     3382 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/.github/scripts/update_version.py
+-rw-r--r--   0     1001      127     1321 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/.github/workflows/publish_docs.yml
+-rw-r--r--   0     1001      127    20647 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/.github/workflows/test.yml
+-rw-r--r--   0     1001      127      504 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/.github/workflows/validate.yml
+-rw-r--r--   0     1001      127     3414 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/.gitignore
+-rw-r--r--   0     1001      127     1750 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/Dockerfile
+-rw-r--r--   0     1001      127     1079 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/LICENSE
+-rw-r--r--   0     1001      127     5164 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/Makefile
+-rw-r--r--   0     1001      127    14891 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/README.md
+-rw-r--r--   0     1001      127      105 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/benchmarking/README.md
+-rw-r--r--   0     1001      127        0 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/benchmarking/benchmarking/__init__.py
+-rw-r--r--   0     1001      127      425 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/benchmarking/benchmarking/simple_render.py
+-rw-r--r--   0     1001      127   127218 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/benchmarking/poetry.lock
+-rw-r--r--   0     1001      127      291 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/benchmarking/pyproject.toml
+-rw-r--r--   0     1001      127      850 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/ci_webapp/README.md
+-rw-r--r--   0     1001      127        1 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/__init__.py
+-rw-r--r--   0     1001      127      886 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/app.py
+-rw-r--r--   0     1001      127      603 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/cli.py
+-rw-r--r--   0     1001      127      111 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/config.py
+-rw-r--r--   0     1001      127        1 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/controllers/__init__.py
+-rw-r--r--   0     1001      127     1433 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/controllers/complex.py
+-rw-r--r--   0     1001      127      581 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/controllers/detail.py
+-rw-r--r--   0     1001      127     1658 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/controllers/home.py
+-rw-r--r--   0     1001      127      649 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/controllers/root_layout.py
+-rw-r--r--   0     1001      127      559 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/controllers/stream.py
+-rw-r--r--   0     1001      127       77 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/main.py
+-rw-r--r--   0     1001      127      208 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/views/__init__.py
+-rw-r--r--   0     1001      127     2261 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/views/app/complex/page.tsx
+-rw-r--r--   0     1001      127      453 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/views/app/detail/page.tsx
+-rw-r--r--   0     1001      127     2822 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/views/app/home/page.tsx
+-rw-r--r--   0     1001      127      645 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/views/app/layout.tsx
+-rw-r--r--   0     1001      127       59 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/views/app/main.css
+-rw-r--r--   0     1001      127      708 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/views/app/stream/page.tsx
+-rw-r--r--   0     1001      127   125408 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/views/package-lock.json
+-rw-r--r--   0     1001      127      453 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/views/package.json
+-rw-r--r--   0     1001      127       83 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/views/postcss.config.js
+-rw-r--r--   0     1001      127      161 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/views/tailwind.config.js
+-rw-r--r--   0     1001      127   111131 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/ci_webapp/poetry.lock
+-rw-r--r--   0     1001      127      754 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/ci_webapp/pyproject.toml
+-rw-r--r--   0     1001      127     1593 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/README.md
+-rw-r--r--   0     1001      127        1 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/__tests__/__init__.py
+-rw-r--r--   0     1001      127     1055 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/__tests__/common.py
+-rw-r--r--   0     1001      127     8021 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py
+-rw-r--r--   0     1001      127      292 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/__tests__/test_cli.py
+-rw-r--r--   0     1001      127      816 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py
+-rw-r--r--   0     1001      127     4277 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/builder.py
+-rw-r--r--   0     1001      127     4656 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/cli.py
+-rw-r--r--   0     1001      127        0 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/environments/__init__.py
+-rw-r--r--   0     1001      127     1383 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/environments/base.py
+-rw-r--r--   0     1001      127     4591 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/environments/poetry.py
+-rw-r--r--   0     1001      127     1832 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/environments/venv.py
+-rw-r--r--   0     1001      127     1336 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/external.py
+-rw-r--r--   0     1001      127     1919 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/generation.py
+-rw-r--r--   0     1001      127      327 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/io.py
+-rw-r--r--   0     1001      127       30 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/.zed/settings.json
+-rw-r--r--   0     1001      127      212 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/__init__.py
+-rw-r--r--   0     1001      127      246 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vim/.vimrc
+-rw-r--r--   0     1001      127      162 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vscode/.vscode/settings.json
+-rw-r--r--   0     1001      127      109 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/zed/pyrightconfig.json
+-rw-r--r--   0     1001      127      170 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/project/.env
+-rw-r--r--   0     1001      127     3383 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore
+-rw-r--r--   0     1001      127      645 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/project/README.md
+-rw-r--r--   0     1001      127       17 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/__init__.py
+-rw-r--r--   0     1001      127      767 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py
+-rw-r--r--   0     1001      127      947 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py
+-rw-r--r--   0     1001      127      282 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/config.py
+-rw-r--r--   0     1001      127      227 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/__init__.py
+-rw-r--r--   0     1001      127     1702 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py
+-rw-r--r--   0     1001      127     1124 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py
+-rw-r--r--   0     1001      127       84 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/main.py
+-rw-r--r--   0     1001      127      157 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/__init__.py
+-rw-r--r--   0     1001      127      208 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/detail.py
+-rw-r--r--   0     1001      127        0 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/__init__.py
+-rw-r--r--   0     1001      127     1219 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx
+-rw-r--r--   0     1001      127      995 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx
+-rw-r--r--   0     1001      127       95 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/main.css
+-rw-r--r--   0     1001      127      524 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json
+-rw-r--r--   0     1001      127      117 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/postcss.config.js
+-rw-r--r--   0     1001      127      195 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/tailwind.config.js
+-rw-r--r--   0     1001      127      332 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/project/docker-compose.yml
+-rw-r--r--   0     1001      127     1493 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml
+-rw-r--r--   0     1001      127    63125 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/poetry.lock
+-rw-r--r--   0     1001      127     1318 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/create_mountaineer_app/pyproject.toml
+-rw-r--r--   0     1001      127      324 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docker-compose.test.yml
+-rw-r--r--   0     1001      127       30 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/.zed/settings.json
+-rw-r--r--   0     1001      127      107 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/README.md
+-rw-r--r--   0     1001      127       15 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/CNAME
+-rw-r--r--   0     1001      127      318 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/api/actions.md
+-rw-r--r--   0     1001      127      454 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/api/api_exception.md
+-rw-r--r--   0     1001      127       99 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/api/app-controller.md
+-rw-r--r--   0     1001      127      281 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/api/build_plugins/base.md
+-rw-r--r--   0     1001      127       57 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/api/build_plugins/javascript.md
+-rw-r--r--   0     1001      127       62 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/api/build_plugins/postcss.md
+-rw-r--r--   0     1001      127      411 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/api/cli.md
+-rw-r--r--   0     1001      127      376 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/api/config.md
+-rw-r--r--   0     1001      127      138 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/api/controller.md
+-rw-r--r--   0     1001      127       67 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/api/core_dependencies.md
+-rw-r--r--   0     1001      127       66 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/api/database/config.md
+-rw-r--r--   0     1001      127       71 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/api/database/dependencies.md
+-rw-r--r--   0     1001      127      507 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/api/database/migrations.md
+-rw-r--r--   0     1001      127       80 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/api/logging.md
+-rw-r--r--   0     1001      127      479 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/api/render.md
+-rw-r--r--   0     1001      127      365 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/api/ssr.md
+-rw-r--r--   0     1001      127      299 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/api/watch_server.md
+-rw-r--r--   0     1001      127     9379 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/client_actions.md
+-rw-r--r--   0     1001      127      753 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/cma.md
+-rw-r--r--   0     1001      127     3021 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/database.md
+-rw-r--r--   0     1001      127     8216 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/database_migrations.md
+-rw-r--r--   0     1001      127     4690 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/deploy.md
+-rw-r--r--   0     1001      127     7698 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/error_handling.md
+-rw-r--r--   0     1001      127     1081 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/index.md
+-rw-r--r--   0     1001      127     1541 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/internal/core_library.md
+-rw-r--r--   0     1001      127     2156 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/links.md
+-rw-r--r--   0     1001      127   365251 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/media/final_todo_list.png
+-rw-r--r--   0     1001      127   148261 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/media/ide_typehints.png
+-rw-r--r--   0     1001      127   545494 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/media/network_debug.png
+-rw-r--r--   0     1001      127   346903 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/media/server_side_rendering.png
+-rw-r--r--   0     1001      127     2263 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/metadata.md
+-rw-r--r--   0     1001      127     2347 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/postcss.md
+-rw-r--r--   0     1001      127    12263 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/quickstart.md
+-rw-r--r--   0     1001      127     4875 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/static_analysis.md
+-rw-r--r--   0     1001      127     2490 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/structure.md
+-rw-r--r--   0     1001      127     1219 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/stylesheets/extra.css
+-rw-r--r--   0     1001      127     9534 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/docs/views.md
+-rw-r--r--   0     1001      127     1887 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/mkdocs.yml
+-rw-r--r--   0     1001      127      109 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/overrides/partials/footer.html
+-rw-r--r--   0     1001      127   156250 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/poetry.lock
+-rw-r--r--   0     1001      127      500 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/docs_website/pyproject.toml
+-rw-r--r--   0     1001      127   675789 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/media/header.png
+-rw-r--r--   0     1001      127     1103 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/actions/__init__.py
+-rw-r--r--   0     1001      127     8123 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/actions/test_fields.py
+-rw-r--r--   0     1001      127     9711 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/actions/test_passthrough_dec.py
+-rw-r--r--   0     1001      127    10065 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/actions/test_sideeffect_dec.py
+-rw-r--r--   0     1001      127        0 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/client_builder/__init__.py
+-rw-r--r--   0     1001      127    14334 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/client_builder/test_build_actions.py
+-rw-r--r--   0     1001      127     5031 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/client_builder/test_build_links.py
+-rw-r--r--   0     1001      127    10127 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/client_builder/test_build_schemas.py
+-rw-r--r--   0     1001      127     6322 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/client_builder/test_builder.py
+-rw-r--r--   0     1001      127     4818 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/client_builder/test_typescript.py
+-rw-r--r--   0     1001      127      319 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/common.py
+-rw-r--r--   0     1001      127      760 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/conftest.py
+-rw-r--r--   0     1001      127        0 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/database/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/database/dependencies/__init__.py
+-rw-r--r--   0     1001      127      208 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/database/dependencies/conftest.py
+-rw-r--r--   0     1001      127      801 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/database/dependencies/test_core.py
+-rw-r--r--   0     1001      127      627 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/database/test_config.py
+-rw-r--r--   0     1001      127      616 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/database/test_sqlmodel.py
+-rw-r--r--   0     1001      127        0 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/dependencies/__init__.py
+-rw-r--r--   0     1001      127     2567 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/dependencies/test_base.py
+-rw-r--r--   0     1001      127      211 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/fixtures/__init__.py
+-rw-r--r--   0     1001      127   571338 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js
+-rw-r--r--   0     1001      127  1638568 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/fixtures/home_controller_source_map.js.map
+-rw-r--r--   0     1001      127   575422 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js
+-rw-r--r--   0     1001      127        0 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/js_compiler/__init__.py
+-rw-r--r--   0     1001      127     9973 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/js_compiler/test_javascript.py
+-rw-r--r--   0     1001      127      808 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/js_compiler/test_postcss.py
+-rw-r--r--   0     1001      127     2823 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/js_compiler/test_source_maps.py
+-rw-r--r--   0     1001      127        0 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/migrations/__init__.py
+-rw-r--r--   0     1001      127     4187 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/migrations/conftest.py
+-rw-r--r--   0     1001      127    23753 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/migrations/test_actions.py
+-rw-r--r--   0     1001      127     5242 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/migrations/test_db_memory_serializer.py
+-rw-r--r--   0     1001      127    12619 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/migrations/test_db_serializer.py
+-rw-r--r--   0     1001      127      795 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/migrations/test_db_stubs.py
+-rw-r--r--   0     1001      127     4527 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/migrations/test_generator.py
+-rw-r--r--   0     1001      127     2672 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/migrations/test_generics.py
+-rw-r--r--   0     1001      127    11671 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/migrations/test_handlers.py
+-rw-r--r--   0     1001      127     1236 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/test_annotation_helpers.py
+-rw-r--r--   0     1001      127    12749 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/test_app.py
+-rw-r--r--   0     1001      127     3021 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/test_cache.py
+-rw-r--r--   0     1001      127     5304 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/test_cli.py
+-rw-r--r--   0     1001      127     2301 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/test_compat.py
+-rw-r--r--   0     1001      127      494 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/test_config.py
+-rw-r--r--   0     1001      127     6824 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/test_controller.py
+-rw-r--r--   0     1001      127     1126 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/test_controller_layout.py
+-rw-r--r--   0     1001      127     3239 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/test_cropper.py
+-rw-r--r--   0     1001      127     1227 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/test_exceptions.py
+-rw-r--r--   0     1001      127      583 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/test_generics.py
+-rw-r--r--   0     1001      127     1065 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/test_io.py
+-rw-r--r--   0     1001      127     1924 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/test_logging.py
+-rw-r--r--   0     1001      127     8494 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/test_paths.py
+-rw-r--r--   0     1001      127     2667 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/test_ssr.py
+-rw-r--r--   0     1001      127     3177 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/__tests__/test_watch.py
+-rw-r--r--   0     1001      127      405 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/actions/__init__.py
+-rw-r--r--   0     1001      127    12444 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/actions/fields.py
+-rw-r--r--   0     1001      127     6841 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/actions/passthrough_dec.py
+-rw-r--r--   0     1001      127    12280 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/actions/sideeffect_dec.py
+-rw-r--r--   0     1001      127     4671 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/annotation_helpers.py
+-rw-r--r--   0     1001      127    28407 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/app.py
+-rw-r--r--   0     1001      127     4523 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/cache.py
+-rw-r--r--   0     1001      127    19296 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/cli.py
+-rw-r--r--   0     1001      127    11390 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/client_builder/build_actions.py
+-rw-r--r--   0     1001      127     4002 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/client_builder/build_links.py
+-rw-r--r--   0     1001      127    10296 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/client_builder/build_schemas.py
+-rw-r--r--   0     1001      127    30960 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/client_builder/builder.py
+-rw-r--r--   0     1001      127    11429 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/client_builder/openapi.py
+-rw-r--r--   0     1001      127     5629 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/client_builder/typescript.py
+-rw-r--r--   0     1001      127     1808 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/compat.py
+-rw-r--r--   0     1001      127     2424 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/config.py
+-rw-r--r--   0     1001      127      197 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/console.py
+-rw-r--r--   0     1001      127       40 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/constants.py
+-rw-r--r--   0     1001      127    16758 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/controller.py
+-rw-r--r--   0     1001      127      881 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/controller_layout.py
+-rw-r--r--   0     1001      127        0 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/controllers/__init__.py
+-rw-r--r--   0     1001      127     1216 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/controllers/exception_controller.py
+-rw-r--r--   0     1001      127    10375 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/cropper.py
+-rw-r--r--   0     1001      127      327 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/database/__init__.py
+-rw-r--r--   0     1001      127     1866 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/database/cli.py
+-rw-r--r--   0     1001      127     1822 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/database/config.py
+-rw-r--r--   0     1001      127      133 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/database/dependencies/__init__.py
+-rw-r--r--   0     1001      127     3425 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/database/dependencies/core.py
+-rw-r--r--   0     1001      127     7969 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/database/sqlmodel.py
+-rw-r--r--   0     1001      127     8737 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/database/validator.py
+-rw-r--r--   0     1001      127      251 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/dependencies/__init__.py
+-rw-r--r--   0     1001      127     5122 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/dependencies/base.py
+-rw-r--r--   0     1001      127      116 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/dependencies/core/__init__.py
+-rw-r--r--   0     1001      127     1069 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/dependencies/core/core.py
+-rw-r--r--   0     1001      127     3317 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/exceptions.py
+-rw-r--r--   0     1001      127     1740 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/generics.py
+-rw-r--r--   0     1001      127     1781 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/io.py
+-rw-r--r--   0     1001      127        1 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/js_compiler/__init__.py
+-rw-r--r--   0     1001      127     1731 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/js_compiler/base.py
+-rw-r--r--   0     1001      127      199 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/js_compiler/exceptions.py
+-rw-r--r--   0     1001      127    17413 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/js_compiler/javascript.py
+-rw-r--r--   0     1001      127     4163 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/js_compiler/postcss.py
+-rw-r--r--   0     1001      127     5614 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/js_compiler/source_maps.py
+-rw-r--r--   0     1001      127     2313 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/logging.py
+-rw-r--r--   0     1001      127        0 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/migrations/__init__.py
+-rw-r--r--   0     1001      127    20278 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/migrations/actions.py
+-rw-r--r--   0     1001      127     8239 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/migrations/cli.py
+-rw-r--r--   0     1001      127     2319 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/migrations/client_io.py
+-rw-r--r--   0     1001      127     8866 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/migrations/db_memory_serializer.py
+-rw-r--r--   0     1001      127    10101 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/migrations/db_serializer.py
+-rw-r--r--   0     1001      127    12263 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/migrations/db_stubs.py
+-rw-r--r--   0     1001      127       99 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/migrations/dependency/__init__.py
+-rw-r--r--   0     1001      127       47 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/migrations/dependency/core/__init__.py
+-rw-r--r--   0     1001      127      356 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/migrations/dependency/core/core.py
+-rw-r--r--   0     1001      127     8619 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/migrations/generator.py
+-rw-r--r--   0     1001      127     3078 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/migrations/generics.py
+-rw-r--r--   0     1001      127    25065 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/migrations/handlers.py
+-rw-r--r--   0     1001      127     1926 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/migrations/migration.py
+-rw-r--r--   0     1001      127     3994 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/migrations/migrator.py
+-rw-r--r--   0     1001      127    13337 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/paths.py
+-rw-r--r--   0     1001      127        0 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/py.typed
+-rw-r--r--   0     1001      127     5816 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/render.py
+-rw-r--r--   0     1001      127     3237 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/ssr.py
+-rw-r--r--   0     1001      127      210 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/static/__init__.py
+-rw-r--r--   0     1001      127     6556 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/static/api.ts
+-rw-r--r--   0     1001      127     3976 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/static/live_reload.ts
+-rw-r--r--   0     1001      127      323 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/static/ssr_polyfills.js
+-rw-r--r--   0     1001      127     7261 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/test_utilities.py
+-rw-r--r--   0     1001      127      213 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/views/__init__.py
+-rw-r--r--   0     1001      127      432 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/views/core/exception/page.tsx
+-rw-r--r--   0     1001      127      178 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/views/core/layout.tsx
+-rw-r--r--   0     1001      127       59 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/views/core/main.css
+-rw-r--r--   0     1001      127     1478 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/views/package-lock.json
+-rw-r--r--   0     1001      127      257 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/views/package.json
+-rw-r--r--   0     1001      127       83 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/views/postcss.config.js
+-rw-r--r--   0     1001      127      162 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/views/tailwind.config.js
+-rw-r--r--   0     1001      127     8427 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/watch.py
+-rw-r--r--   0     1001      127     4062 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/watch_server.py
+-rw-r--r--   0     1001      127     1213 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/mountaineer/webservice.py
+-rw-r--r--   0     1001      127   129036 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/poetry.lock
+-rw-r--r--   0     1001      127   453080 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/src/benches/fixtures/complex_sourcemap_mapping.txt
+-rw-r--r--   0     1001      127   575422 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/src/benches/fixtures/home_controller_ssr_with_react.js
+-rw-r--r--   0     1001      127      322 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/src/benches/fixtures/ssr_polyfill_archive.js
+-rw-r--r--   0     1001      127      899 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/src/benches/lexers_benchmark.rs
+-rw-r--r--   0     1001      127     1089 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/src/benches/source_map_benchmark.rs
+-rw-r--r--   0     1001      127     1595 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/src/benches/ssr_benchmark.rs
+-rw-r--r--   0     1001      127      499 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/src/errors.rs
+-rw-r--r--   0     1001      127     4648 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/src/lexers.rs
+-rw-r--r--   0     1001      127     9118 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/src/lib.rs
+-rw-r--r--   0     1001      127      680 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/src/logging.rs
+-rw-r--r--   0     1001      127    17549 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/src/source_map.rs
+-rw-r--r--   0     1001      127    15113 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/src/ssr.rs
+-rw-r--r--   0     1001      127     3998 2024-05-27 09:32:42.000000 mountaineer-0.5.0.dev8/src/timeout.rs
+-rw-r--r--   0     1001      127    32093 2024-05-27 09:32:57.000000 mountaineer-0.5.0.dev8/Cargo.lock
+-rw-r--r--   0     1001      127     1624 2024-05-27 09:32:54.000000 mountaineer-0.5.0.dev8/pyproject.toml
+-rw-r--r--   0        0        0    15354 1970-01-01 00:00:00.000000 mountaineer-0.5.0.dev8/PKG-INFO
```

### Comparing `mountaineer-0.5.0.dev7/src_go/build.rs` & `mountaineer-0.5.0.dev8/src_go/build.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/src_go/go/js_build.go` & `mountaineer-0.5.0.dev8/src_go/go/js_build.go`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/src_go/src/lib.rs` & `mountaineer-0.5.0.dev8/src_go/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/Cargo.toml` & `mountaineer-0.5.0.dev8/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 [[bench]]
 path = "src/benches/lexers_benchmark.rs"
 name = "lexers_benchmark"
 harness = false
 
 [package]
 name = "mountaineer"
-version = "0.5.0-dev7"
+version = "0.5.0-dev8"
 edition = "2021"
 
 [dependencies]
 v8 = "0.89.0"
 deno_core_icudata = "0.73.0"
 lazy_static = "1.4.0"
 serde_json = "1.0"
```

### Comparing `mountaineer-0.5.0.dev7/.github/poetry.lock` & `mountaineer-0.5.0.dev8/.github/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/.github/pyproject.toml` & `mountaineer-0.5.0.dev8/.github/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/.github/scripts/__tests__/test_update_version.py` & `mountaineer-0.5.0.dev8/.github/scripts/__tests__/test_update_version.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/.github/scripts/check_dependencies.py` & `mountaineer-0.5.0.dev8/.github/scripts/check_dependencies.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/.github/scripts/update_version.py` & `mountaineer-0.5.0.dev8/.github/scripts/update_version.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/.github/workflows/publish_docs.yml` & `mountaineer-0.5.0.dev8/.github/workflows/publish_docs.yml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/.github/workflows/test.yml` & `mountaineer-0.5.0.dev8/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/.gitignore` & `mountaineer-0.5.0.dev8/.gitignore`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/Dockerfile` & `mountaineer-0.5.0.dev8/Dockerfile`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/LICENSE` & `mountaineer-0.5.0.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/Makefile` & `mountaineer-0.5.0.dev8/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
 #
 # Common helper functions
 #
 
 define test-common
 	echo "Running tests for $(2)..."
-	@(cd $(1) && poetry run pytest -W error $(test-args) $(2))
+	@(cd $(1) && poetry run pytest -vvv -W error $(test-args) $(2))
 endef
 
 define test-rust-common
 	echo "Running rust tests for $(2)..."
 	@(cd $(1) && cargo test --all)
 endef
```

### Comparing `mountaineer-0.5.0.dev7/README.md` & `mountaineer-0.5.0.dev8/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/benchmarking/poetry.lock` & `mountaineer-0.5.0.dev8/benchmarking/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/ci_webapp/README.md` & `mountaineer-0.5.0.dev8/ci_webapp/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/app.py` & `mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/app.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/cli.py` & `mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/controllers/complex.py` & `mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/controllers/complex.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/controllers/detail.py` & `mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/controllers/detail.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/controllers/home.py` & `mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/controllers/home.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/controllers/root_layout.py` & `mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/controllers/root_layout.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/controllers/stream.py` & `mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/controllers/stream.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/views/app/complex/page.tsx` & `mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/views/app/complex/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/views/app/home/page.tsx` & `mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/views/app/home/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/views/app/layout.tsx` & `mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/views/app/layout.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/views/app/stream/page.tsx` & `mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/views/app/stream/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/ci_webapp/ci_webapp/views/package-lock.json` & `mountaineer-0.5.0.dev8/ci_webapp/ci_webapp/views/package-lock.json`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/ci_webapp/poetry.lock` & `mountaineer-0.5.0.dev8/ci_webapp/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/ci_webapp/pyproject.toml` & `mountaineer-0.5.0.dev8/ci_webapp/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/create_mountaineer_app/README.md` & `mountaineer-0.5.0.dev8/create_mountaineer_app/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/__tests__/common.py` & `mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/__tests__/common.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py` & `mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py` & `mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/builder.py` & `mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/builder.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/cli.py` & `mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/environments/base.py` & `mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/environments/base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/environments/poetry.py` & `mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/environments/poetry.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/environments/venv.py` & `mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/environments/venv.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/external.py` & `mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/external.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/generation.py` & `mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/generation.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore` & `mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/project/README.md` & `mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/project/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py` & `mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py` & `mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py` & `mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py` & `mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx` & `mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx` & `mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json` & `mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml` & `mountaineer-0.5.0.dev8/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/create_mountaineer_app/poetry.lock` & `mountaineer-0.5.0.dev8/create_mountaineer_app/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/create_mountaineer_app/pyproject.toml` & `mountaineer-0.5.0.dev8/create_mountaineer_app/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/docs_website/docs/client_actions.md` & `mountaineer-0.5.0.dev8/docs_website/docs/client_actions.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/docs_website/docs/cma.md` & `mountaineer-0.5.0.dev8/docs_website/docs/cma.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/docs_website/docs/database.md` & `mountaineer-0.5.0.dev8/docs_website/docs/database.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/docs_website/docs/database_migrations.md` & `mountaineer-0.5.0.dev8/docs_website/docs/database_migrations.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/docs_website/docs/deploy.md` & `mountaineer-0.5.0.dev8/docs_website/docs/deploy.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/docs_website/docs/error_handling.md` & `mountaineer-0.5.0.dev8/docs_website/docs/error_handling.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/docs_website/docs/index.md` & `mountaineer-0.5.0.dev8/docs_website/docs/index.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/docs_website/docs/internal/core_library.md` & `mountaineer-0.5.0.dev8/docs_website/docs/internal/core_library.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/docs_website/docs/links.md` & `mountaineer-0.5.0.dev8/docs_website/docs/links.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/docs_website/docs/media/final_todo_list.png` & `mountaineer-0.5.0.dev8/docs_website/docs/media/final_todo_list.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/docs_website/docs/media/ide_typehints.png` & `mountaineer-0.5.0.dev8/docs_website/docs/media/ide_typehints.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/docs_website/docs/media/network_debug.png` & `mountaineer-0.5.0.dev8/docs_website/docs/media/network_debug.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/docs_website/docs/media/server_side_rendering.png` & `mountaineer-0.5.0.dev8/docs_website/docs/media/server_side_rendering.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/docs_website/docs/metadata.md` & `mountaineer-0.5.0.dev8/docs_website/docs/metadata.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/docs_website/docs/postcss.md` & `mountaineer-0.5.0.dev8/docs_website/docs/postcss.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/docs_website/docs/quickstart.md` & `mountaineer-0.5.0.dev8/docs_website/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/docs_website/docs/static_analysis.md` & `mountaineer-0.5.0.dev8/docs_website/docs/static_analysis.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/docs_website/docs/structure.md` & `mountaineer-0.5.0.dev8/docs_website/docs/structure.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/docs_website/docs/stylesheets/extra.css` & `mountaineer-0.5.0.dev8/docs_website/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/docs_website/docs/views.md` & `mountaineer-0.5.0.dev8/docs_website/docs/views.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/docs_website/mkdocs.yml` & `mountaineer-0.5.0.dev8/docs_website/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/docs_website/poetry.lock` & `mountaineer-0.5.0.dev8/docs_website/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/media/header.png` & `mountaineer-0.5.0.dev8/media/header.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__init__.py` & `mountaineer-0.5.0.dev8/mountaineer/__init__.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/actions/test_fields.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/actions/test_fields.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/actions/test_passthrough_dec.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/actions/test_passthrough_dec.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/actions/test_sideeffect_dec.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/actions/test_sideeffect_dec.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from contextlib import asynccontextmanager
 from pathlib import Path
 from time import monotonic_ns
+from typing import Any
 from unittest.mock import patch
 
 import pytest
 from fastapi import Depends, Request
 from fastapi.testclient import TestClient
 from pydantic.main import BaseModel
 from starlette.datastructures import Headers
@@ -153,15 +154,50 @@
                 value_b="World",
             )
 
     await call_sideeffect_common(ExampleController())
 
 
 @pytest.mark.asyncio
-async def test_get_render_parameters():
+@pytest.mark.parametrize(
+    "referer, expected_resolved",
+    [
+        # Fully specified query parameters
+        (
+            "http://example.com/test/5/?url_query_param=test-query-value",
+            {
+                "cookie_dependency": "cookie-value",
+                "path_param": 5,
+                "url_query_param": "test-query-value",
+            },
+        ),
+        # Unspecified query parameters should be None
+        (
+            "http://example.com/test/5/",
+            {
+                "cookie_dependency": "cookie-value",
+                "path_param": 5,
+                "url_query_param": None,
+            },
+        ),
+        # Partially specified query param url
+        (
+            "http://example.com/test/5/?url_query_param=",
+            {
+                "cookie_dependency": "cookie-value",
+                "path_param": 5,
+                "url_query_param": "",
+            },
+        ),
+    ],
+)
+async def test_get_render_parameters(
+    referer: str,
+    expected_resolved: dict[str, Any],
+):
     """
     Given a controller, reproduce the logic of FastAPI to sniff the render()
     function for dependencies and resolve them.
 
     """
     from mountaineer.actions.sideeffect_dec import get_render_parameters
 
@@ -169,19 +205,20 @@
 
     def grab_cookie_dependency(request: Request):
         nonlocal found_cookie
         found_cookie = request.cookies.get("test-cookie")
         return found_cookie
 
     class TestController(ControllerBase):
-        url: str = "/test/{query_id}/"
+        url: str = "/test/{path_param}/"
 
         def render(
             self,
-            query_id: int,
+            path_param: int,
+            url_query_param: str | None = None,
             cookie_dependency: str = Depends(grab_cookie_dependency),
         ) -> ExampleRenderModel:
             return ExampleRenderModel(
                 value_a="Hello",
                 value_b="World",
             )
 
@@ -195,33 +232,30 @@
         {
             "type": "http",
             "headers": Headers(
                 {
                     "cookie": "test-cookie=cookie-value",
                     # Its important the referer aligns with the controller url, since that is expected
                     # to be the original view page that is calling this sub-function
-                    "referer": "http://example.com/test/5/",
+                    "referer": referer,
                 }
             ).raw,
             "http_version": "1.1",
             "scheme": "",
             "client": "",
             "server": "",
             # The URL and method should both be different, to test whether we are able
             # to map the request to the correct endpoint
             "method": "POST",
             "url": "http://localhost/related_action_endpoint",
         }
     )
 
     async with get_render_parameters(controller, fake_request) as resolved_dependencies:
-        assert resolved_dependencies == {
-            "cookie_dependency": "cookie-value",
-            "query_id": 5,
-        }
+        assert resolved_dependencies == expected_resolved
 
 
 @pytest.mark.parametrize(
     "use_experimental,min_time,max_time",
     [
         (False, 1, None),
         (True, None, 0.10),
```

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/client_builder/test_build_actions.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/client_builder/test_build_actions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/client_builder/test_build_links.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/client_builder/test_build_links.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/client_builder/test_build_schemas.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/client_builder/test_build_schemas.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/client_builder/test_builder.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/client_builder/test_builder.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/client_builder/test_typescript.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/client_builder/test_typescript.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/database/dependencies/test_core.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/database/dependencies/test_core.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/database/test_config.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/database/test_config.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/database/test_sqlmodel.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/database/test_sqlmodel.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/dependencies/test_base.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/dependencies/test_base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/fixtures/home_controller_source_map.js.map` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/fixtures/home_controller_source_map.js.map`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/js_compiler/test_javascript.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/js_compiler/test_javascript.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/js_compiler/test_postcss.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/js_compiler/test_postcss.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/js_compiler/test_source_maps.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/js_compiler/test_source_maps.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/migrations/conftest.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/migrations/conftest.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/migrations/test_actions.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/migrations/test_actions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/migrations/test_db_memory_serializer.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/migrations/test_db_memory_serializer.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/migrations/test_db_serializer.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/migrations/test_db_serializer.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/migrations/test_db_stubs.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/migrations/test_db_stubs.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/migrations/test_generator.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/migrations/test_generator.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/migrations/test_generics.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/migrations/test_generics.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/migrations/test_handlers.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/migrations/test_handlers.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/test_annotation_helpers.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/test_annotation_helpers.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/test_app.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/test_app.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/test_cache.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/test_cache.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/test_cli.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/test_cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/test_compat.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/test_compat.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/test_controller.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/test_controller.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/test_controller_layout.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/test_controller_layout.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/test_cropper.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/test_cropper.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/test_exceptions.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/test_generics.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/test_generics.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/test_io.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/test_io.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/test_logging.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/test_logging.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/test_paths.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/test_paths.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/test_ssr.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/test_ssr.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/__tests__/test_watch.py` & `mountaineer-0.5.0.dev8/mountaineer/__tests__/test_watch.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/actions/fields.py` & `mountaineer-0.5.0.dev8/mountaineer/actions/fields.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/actions/passthrough_dec.py` & `mountaineer-0.5.0.dev8/mountaineer/actions/passthrough_dec.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/actions/sideeffect_dec.py` & `mountaineer-0.5.0.dev8/mountaineer/actions/sideeffect_dec.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,24 +220,26 @@
     the same way that FastAPI/Starlette do, so we're able to pretend as if a new request
     is coming into the view endpoint.
 
     NOTE: We exclude calls to background tasks, since these are rarely intended for
     automatic calls to the rendering due to side-effects.
 
     """
-    # Create a synethic request object that we would use to access the core
+    # Create a synthetic request object that we would use to access the core
     # html. This will be passed through the dependency resolution pipeline so to
     # render() it's indistinguishable from a real request and therefore will render
     # in the same way.
     # The referrer should capture the page that they're actually on
     referer = request.headers.get("referer")
+    parsed_path = urlparse(referer or controller.url)
     view_request = Request(
         {
             "type": request.scope["type"],
-            "path": urlparse(referer or controller.url).path,
+            "path": parsed_path.path,
+            "query_string": parsed_path.query,
             "headers": request.headers.raw,
             "http_version": request.scope["http_version"],
             "method": "GET",
             "scheme": request.scope["scheme"],
             "client": request.scope["client"],
             "server": request.scope["server"],
         }
@@ -261,28 +263,33 @@
     ):
         match, child_scope = route.matches(view_request.scope)
         if match != Match.FULL:
             raise RuntimeError(
                 f"Route {route} did not match ({match}) {view_request.scope}"
             )
         view_request.scope = {
-            **view_request.scope,
+            # Make sure we're populating the path params with some values
+            # even if they're not extracted in either the view or the child definition
             "path_params": {},
-            "query_string": "",
+            **view_request.scope,
             **child_scope,
         }
 
     try:
         async with get_function_dependencies(
             callable=controller.render,
-            url=controller.url
-            if not isinstance(controller, LayoutControllerBase)
-            else None,
-            request=view_request
-            if not isinstance(controller, LayoutControllerBase)
-            else None,
+            url=(
+                controller.url
+                if not isinstance(controller, LayoutControllerBase)
+                else None
+            ),
+            request=(
+                view_request
+                if not isinstance(controller, LayoutControllerBase)
+                else None
+            ),
         ) as values:
             yield values
     except RuntimeError as e:
         raise RuntimeError(
             f"Error occurred while resolving dependencies for render(): {controller}: {e}"
         ) from e
```

### Comparing `mountaineer-0.5.0.dev7/mountaineer/annotation_helpers.py` & `mountaineer-0.5.0.dev8/mountaineer/annotation_helpers.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/app.py` & `mountaineer-0.5.0.dev8/mountaineer/app.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/cache.py` & `mountaineer-0.5.0.dev8/mountaineer/cache.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/cli.py` & `mountaineer-0.5.0.dev8/mountaineer/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                 for builder in app_controller.builders:
                     builder.global_state = self.build_config.build_state
 
             self.run_build(app_controller)
 
             # If the client passed a rebuild channel, we'll listen for rebuild requests
             if self.build_config.allow_js_reloads:
-                self.listen_for_rebuilds(app_controller)
+                self.rebuild_thread = self.listen_for_rebuilds(app_controller)
 
         if self.runserver_config is not None:
             thread = UvicornThread(
                 app=app_controller.app,
                 port=self.runserver_config.port,
             )
             thread.start()
@@ -210,16 +210,17 @@
             while True:
                 rebuild = self.rebuild_channel.get()
                 if rebuild is None:
                     break
                 self.run_build(app_controller)
 
         LOGGER.debug("Will launch rebuild thread")
-        rebuild_thread = Thread(target=wait_for_rebuild)
+        rebuild_thread = Thread(target=wait_for_rebuild, daemon=True)
         rebuild_thread.start()
+        return rebuild_thread
 
     def run_build(self, app_controller: AppController):
         start = time()
         js_compiler = ClientBuilder(
             app_controller,
             live_reload_port=(
                 self.runserver_config.live_reload_port
@@ -252,14 +253,16 @@
 
         if self.rebuild_channel is not None:
             self.rebuild_channel.put(None)
 
         if self.runserver_config is not None:
             self.close_signal.set()
 
+        self.rebuild_thread.join()
+
         # Try to give the process time to shut down gracefully
         while self.is_alive() and hard_timeout > 0:
             self.join(1)
             hard_timeout -= 1
 
         if hard_timeout == 0:
             CONSOLE.print(
```

### Comparing `mountaineer-0.5.0.dev7/mountaineer/client_builder/build_actions.py` & `mountaineer-0.5.0.dev8/mountaineer/client_builder/build_actions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/client_builder/build_links.py` & `mountaineer-0.5.0.dev8/mountaineer/client_builder/build_links.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/client_builder/build_schemas.py` & `mountaineer-0.5.0.dev8/mountaineer/client_builder/build_schemas.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/client_builder/builder.py` & `mountaineer-0.5.0.dev8/mountaineer/client_builder/builder.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/client_builder/openapi.py` & `mountaineer-0.5.0.dev8/mountaineer/client_builder/openapi.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/client_builder/typescript.py` & `mountaineer-0.5.0.dev8/mountaineer/client_builder/typescript.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/compat.py` & `mountaineer-0.5.0.dev8/mountaineer/compat.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/config.py` & `mountaineer-0.5.0.dev8/mountaineer/config.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/controller.py` & `mountaineer-0.5.0.dev8/mountaineer/controller.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/controller_layout.py` & `mountaineer-0.5.0.dev8/mountaineer/controller_layout.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/controllers/exception_controller.py` & `mountaineer-0.5.0.dev8/mountaineer/controllers/exception_controller.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/cropper.py` & `mountaineer-0.5.0.dev8/mountaineer/cropper.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/database/cli.py` & `mountaineer-0.5.0.dev8/mountaineer/database/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/database/config.py` & `mountaineer-0.5.0.dev8/mountaineer/database/config.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/database/dependencies/core.py` & `mountaineer-0.5.0.dev8/mountaineer/database/dependencies/core.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/database/sqlmodel.py` & `mountaineer-0.5.0.dev8/mountaineer/database/sqlmodel.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/database/validator.py` & `mountaineer-0.5.0.dev8/mountaineer/database/validator.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/dependencies/base.py` & `mountaineer-0.5.0.dev8/mountaineer/dependencies/base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/dependencies/core/core.py` & `mountaineer-0.5.0.dev8/mountaineer/dependencies/core/core.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/exceptions.py` & `mountaineer-0.5.0.dev8/mountaineer/exceptions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/generics.py` & `mountaineer-0.5.0.dev8/mountaineer/generics.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/io.py` & `mountaineer-0.5.0.dev8/mountaineer/io.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/js_compiler/base.py` & `mountaineer-0.5.0.dev8/mountaineer/js_compiler/base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/js_compiler/javascript.py` & `mountaineer-0.5.0.dev8/mountaineer/js_compiler/javascript.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/js_compiler/postcss.py` & `mountaineer-0.5.0.dev8/mountaineer/js_compiler/postcss.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/js_compiler/source_maps.py` & `mountaineer-0.5.0.dev8/mountaineer/js_compiler/source_maps.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/logging.py` & `mountaineer-0.5.0.dev8/mountaineer/logging.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/migrations/actions.py` & `mountaineer-0.5.0.dev8/mountaineer/migrations/actions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/migrations/cli.py` & `mountaineer-0.5.0.dev8/mountaineer/migrations/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/migrations/client_io.py` & `mountaineer-0.5.0.dev8/mountaineer/migrations/client_io.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/migrations/db_memory_serializer.py` & `mountaineer-0.5.0.dev8/mountaineer/migrations/db_memory_serializer.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/migrations/db_serializer.py` & `mountaineer-0.5.0.dev8/mountaineer/migrations/db_serializer.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/migrations/db_stubs.py` & `mountaineer-0.5.0.dev8/mountaineer/migrations/db_stubs.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/migrations/generator.py` & `mountaineer-0.5.0.dev8/mountaineer/migrations/generator.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/migrations/generics.py` & `mountaineer-0.5.0.dev8/mountaineer/migrations/generics.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/migrations/handlers.py` & `mountaineer-0.5.0.dev8/mountaineer/migrations/handlers.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/migrations/migration.py` & `mountaineer-0.5.0.dev8/mountaineer/migrations/migration.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/migrations/migrator.py` & `mountaineer-0.5.0.dev8/mountaineer/migrations/migrator.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/paths.py` & `mountaineer-0.5.0.dev8/mountaineer/paths.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/render.py` & `mountaineer-0.5.0.dev8/mountaineer/render.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/ssr.py` & `mountaineer-0.5.0.dev8/mountaineer/ssr.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/static/api.ts` & `mountaineer-0.5.0.dev8/mountaineer/static/api.ts`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/static/live_reload.ts` & `mountaineer-0.5.0.dev8/mountaineer/static/live_reload.ts`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/test_utilities.py` & `mountaineer-0.5.0.dev8/mountaineer/test_utilities.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/views/package-lock.json` & `mountaineer-0.5.0.dev8/mountaineer/views/package-lock.json`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/watch.py` & `mountaineer-0.5.0.dev8/mountaineer/watch.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/watch_server.py` & `mountaineer-0.5.0.dev8/mountaineer/watch_server.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/mountaineer/webservice.py` & `mountaineer-0.5.0.dev8/mountaineer/webservice.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/poetry.lock` & `mountaineer-0.5.0.dev8/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/src/benches/fixtures/complex_sourcemap_mapping.txt` & `mountaineer-0.5.0.dev8/src/benches/fixtures/complex_sourcemap_mapping.txt`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/src/benches/fixtures/home_controller_ssr_with_react.js` & `mountaineer-0.5.0.dev8/src/benches/fixtures/home_controller_ssr_with_react.js`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/src/benches/lexers_benchmark.rs` & `mountaineer-0.5.0.dev8/src/benches/lexers_benchmark.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/src/benches/source_map_benchmark.rs` & `mountaineer-0.5.0.dev8/src/benches/source_map_benchmark.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/src/benches/ssr_benchmark.rs` & `mountaineer-0.5.0.dev8/src/benches/ssr_benchmark.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/src/lexers.rs` & `mountaineer-0.5.0.dev8/src/lexers.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/src/lib.rs` & `mountaineer-0.5.0.dev8/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/src/logging.rs` & `mountaineer-0.5.0.dev8/src/logging.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/src/source_map.rs` & `mountaineer-0.5.0.dev8/src/source_map.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/src/ssr.rs` & `mountaineer-0.5.0.dev8/src/ssr.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/src/timeout.rs` & `mountaineer-0.5.0.dev8/src/timeout.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.5.0.dev7/Cargo.lock` & `mountaineer-0.5.0.dev8/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -531,15 +531,15 @@
 checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mountaineer"
-version = "0.5.0-dev7"
+version = "0.5.0-dev8"
 dependencies = [
  "criterion",
  "deno_core_icudata",
  "env_logger",
  "lazy_static",
  "libc",
  "log",
```

### Comparing `mountaineer-0.5.0.dev7/pyproject.toml` & `mountaineer-0.5.0.dev8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "mountaineer"
 dependencies = [ "pydantic", "fastapi", "inflection", "click", "uvicorn[standard]", "packaging", "watchdog", "pydantic-settings", "sqlmodel", "asyncpg", "sqlalchemy[asyncio]", "rich",]
 exclude = [ "fixtures", "ci_webapp", "create_mountaineer_app", "media", "docs_website", "benchmarking",]
 
 [tool.poetry]
 name = "mountaineer"
-version = "0.5.0.dev7"
+version = "0.5.0.dev8"
 description = ""
 authors = [ "Pierce Freeman <pierce@freeman.vc>",]
 readme = "README.md"
 
 [tool.mypy]
 warn_return_any = true
 warn_unused_configs = true
```

### Comparing `mountaineer-0.5.0.dev7/PKG-INFO` & `mountaineer-0.5.0.dev8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mountaineer
-Version: 0.5.0.dev7
+Version: 0.5.0.dev8
 Requires-Dist: pydantic
 Requires-Dist: fastapi
 Requires-Dist: inflection
 Requires-Dist: click
 Requires-Dist: uvicorn[standard]
 Requires-Dist: packaging
 Requires-Dist: watchdog
```

