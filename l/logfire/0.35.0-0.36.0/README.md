# Comparing `tmp/logfire-0.35.0.tar.gz` & `tmp/logfire-0.36.0.tar.gz`

## Comparing `logfire-0.35.0.tar` & `logfire-0.36.0.tar`

### file list

```diff
@@ -1,130 +1,130 @@
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 logfire-0.35.0/Makefile
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/__main__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/cli.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/exceptions.py
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/propagate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/py.typed
--rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/testing.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/version.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/__init__.py
--rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/ast_utils.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/async_.py
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/auth.py
--rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/backfill.py
--rw-r--r--   0        0        0    18512 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/cli.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/collect_system_info.py
--rw-r--r--   0        0        0    56181 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/config.py
--rw-r--r--   0        0        0    11225 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/config_params.py
--rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/constants.py
--rw-r--r--   0        0        0    19127 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/formatter.py
--rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/instrument.py
--rw-r--r--   0        0        0     9035 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/json_encoder.py
--rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/json_formatter.py
--rw-r--r--   0        0        0    13081 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/json_schema.py
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/json_types.py
--rw-r--r--   0        0        0    62713 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/main.py
--rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/metrics.py
--rw-r--r--   0        0        0     8756 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/scrubbing.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/stack_info.py
--rw-r--r--   0        0        0    10602 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/tracer.py
--rw-r--r--   0        0        0     6384 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/utils.py
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/auto_trace/__init__.py
--rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/auto_trace/import_hook.py
--rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/auto_trace/rewrite_ast.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/auto_trace/types.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/exporters/__init__.py
--rw-r--r--   0        0        0    18968 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/exporters/console.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/exporters/fallback.py
--rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/exporters/file.py
--rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/exporters/otlp.py
--rw-r--r--   0        0        0     9014 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/exporters/processor_wrapper.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/exporters/remove_pending.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/exporters/wrapper.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/integrations/__init__.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/integrations/asyncpg.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/integrations/django.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/integrations/executors.py
--rw-r--r--   0        0        0    10599 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/integrations/fastapi.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/integrations/httpx.py
--rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/integrations/psycopg.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/integrations/requests.py
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/integrations/llm_providers/anthropic.py
--rw-r--r--   0        0        0     7796 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/integrations/llm_providers/llm_provider.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/integrations/llm_providers/openai.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/_internal/integrations/llm_providers/types.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/integrations/__init__.py
--rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/integrations/logging.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/integrations/loguru.py
--rw-r--r--   0        0        0    19169 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/integrations/pydantic.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 logfire-0.35.0/logfire/integrations/structlog.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/__init__.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/conftest.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/module_used_for_tests.py
--rw-r--r--   0        0        0    19034 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/test_auto_trace.py
--rw-r--r--   0        0        0     9988 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/test_backfill.py
--rw-r--r--   0        0        0    47077 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/test_cli.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/test_collect_package_resources.py
--rw-r--r--   0        0        0    53700 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/test_configure.py
--rw-r--r--   0        0        0    29388 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/test_console_exporter.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/test_formatter.py
--rw-r--r--   0        0        0    45893 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/test_json_args.py
--rw-r--r--   0        0        0    19936 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/test_json_args_formatting.py
--rw-r--r--   0        0        0   105498 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/test_logfire.py
--rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/test_loguru.py
--rw-r--r--   0        0        0    11914 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/test_metrics.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/test_no_production.py
--rw-r--r--   0        0        0    54162 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/test_pydantic_plugin.py
--rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/test_sampling.py
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/test_secret_scrubbing.py
--rw-r--r--   0        0        0     7270 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/test_slow_async_callbacks.py
--rw-r--r--   0        0        0     8126 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/test_source_code_extraction.py
--rw-r--r--   0        0        0    12334 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/test_stdlib_logging.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/test_structlog.py
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/test_testing.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/test_utils.py
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/auto_trace_samples/__init__.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/auto_trace_samples/foo.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/auto_trace_samples/simple_nesting.py
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/exporters/test_fallback_exporter.py
--rw-r--r--   0        0        0     8384 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/exporters/test_file_exporter.py
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/exporters/test_otlp_session.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/exporters/test_remove_pending.py
--rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/exporters/test_retry_fewer_spans.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/import_used_for_tests/__init__.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/import_used_for_tests/slow_async_callbacks_example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/import_used_for_tests/a/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/import_used_for_tests/a/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/otel_integrations/__init__.py
--rw-r--r--   0        0        0    24476 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/otel_integrations/test_anthropic.py
--rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/otel_integrations/test_asgi.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/otel_integrations/test_asyncpg.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/otel_integrations/test_django.py
--rw-r--r--   0        0        0    44449 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/otel_integrations/test_fastapi.py
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/otel_integrations/test_flask.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/otel_integrations/test_httpx.py
--rw-r--r--   0        0        0    44469 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/otel_integrations/test_openai.py
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/otel_integrations/test_psycopg.py
--rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/otel_integrations/test_requests.py
--rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/otel_integrations/test_sqlalchemy.py
--rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/otel_integrations/test_starlette.py
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/otel_integrations/test_wsgi.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/otel_integrations/django_test_project/__init__.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/otel_integrations/django_test_project/manage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/otel_integrations/django_test_project/django_test_app/__init__.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/otel_integrations/django_test_project/django_test_app/admin.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/otel_integrations/django_test_project/django_test_app/apps.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/otel_integrations/django_test_project/django_test_app/models.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/otel_integrations/django_test_project/django_test_app/urls.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/otel_integrations/django_test_project/django_test_app/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/otel_integrations/django_test_project/django_test_app/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/otel_integrations/django_test_project/django_test_site/__init__.py
--rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/otel_integrations/django_test_project/django_test_site/settings.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/otel_integrations/django_test_project/django_test_site/urls.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 logfire-0.35.0/tests/otel_integrations/django_test_project/django_test_site/wsgi.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 logfire-0.35.0/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 logfire-0.35.0/LICENSE
--rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 logfire-0.35.0/README.md
--rw-r--r--   0        0        0     8521 2020-02-02 00:00:00.000000 logfire-0.35.0/pyproject.toml
--rw-r--r--   0        0        0     7731 2020-02-02 00:00:00.000000 logfire-0.35.0/PKG-INFO
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 logfire-0.36.0/Makefile
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/__main__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/cli.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/exceptions.py
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/propagate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/py.typed
+-rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/testing.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/version.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/__init__.py
+-rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/ast_utils.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/async_.py
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/auth.py
+-rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/backfill.py
+-rw-r--r--   0        0        0    18512 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/cli.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/collect_system_info.py
+-rw-r--r--   0        0        0    56230 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/config.py
+-rw-r--r--   0        0        0    11225 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/config_params.py
+-rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/constants.py
+-rw-r--r--   0        0        0    19127 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/formatter.py
+-rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/instrument.py
+-rw-r--r--   0        0        0     9035 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/json_encoder.py
+-rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/json_formatter.py
+-rw-r--r--   0        0        0    13081 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/json_schema.py
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/json_types.py
+-rw-r--r--   0        0        0    63477 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/main.py
+-rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/metrics.py
+-rw-r--r--   0        0        0     8756 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/scrubbing.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/stack_info.py
+-rw-r--r--   0        0        0    10602 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/tracer.py
+-rw-r--r--   0        0        0     6384 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/utils.py
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/auto_trace/__init__.py
+-rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/auto_trace/import_hook.py
+-rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/auto_trace/rewrite_ast.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/auto_trace/types.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/exporters/__init__.py
+-rw-r--r--   0        0        0    18968 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/exporters/console.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/exporters/fallback.py
+-rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/exporters/file.py
+-rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/exporters/otlp.py
+-rw-r--r--   0        0        0     9014 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/exporters/processor_wrapper.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/exporters/remove_pending.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/exporters/wrapper.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/integrations/__init__.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/integrations/asyncpg.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/integrations/django.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/integrations/executors.py
+-rw-r--r--   0        0        0    10656 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/integrations/fastapi.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/integrations/httpx.py
+-rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/integrations/psycopg.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/integrations/requests.py
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/integrations/llm_providers/anthropic.py
+-rw-r--r--   0        0        0     7796 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/integrations/llm_providers/llm_provider.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/integrations/llm_providers/openai.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/_internal/integrations/llm_providers/types.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/integrations/__init__.py
+-rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/integrations/logging.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/integrations/loguru.py
+-rw-r--r--   0        0        0    19169 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/integrations/pydantic.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 logfire-0.36.0/logfire/integrations/structlog.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/__init__.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/conftest.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/module_used_for_tests.py
+-rw-r--r--   0        0        0    19034 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/test_auto_trace.py
+-rw-r--r--   0        0        0     9988 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/test_backfill.py
+-rw-r--r--   0        0        0    47077 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/test_cli.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/test_collect_package_resources.py
+-rw-r--r--   0        0        0    53700 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/test_configure.py
+-rw-r--r--   0        0        0    29388 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/test_console_exporter.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/test_formatter.py
+-rw-r--r--   0        0        0    45893 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/test_json_args.py
+-rw-r--r--   0        0        0    19936 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/test_json_args_formatting.py
+-rw-r--r--   0        0        0   105498 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/test_logfire.py
+-rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/test_loguru.py
+-rw-r--r--   0        0        0    11914 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/test_metrics.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/test_no_production.py
+-rw-r--r--   0        0        0    54162 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/test_pydantic_plugin.py
+-rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/test_sampling.py
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/test_secret_scrubbing.py
+-rw-r--r--   0        0        0     7270 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/test_slow_async_callbacks.py
+-rw-r--r--   0        0        0     8126 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/test_source_code_extraction.py
+-rw-r--r--   0        0        0    12334 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/test_stdlib_logging.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/test_structlog.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/test_testing.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/test_utils.py
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/auto_trace_samples/__init__.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/auto_trace_samples/foo.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/auto_trace_samples/simple_nesting.py
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/exporters/test_fallback_exporter.py
+-rw-r--r--   0        0        0     8384 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/exporters/test_file_exporter.py
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/exporters/test_otlp_session.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/exporters/test_remove_pending.py
+-rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/exporters/test_retry_fewer_spans.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/import_used_for_tests/__init__.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/import_used_for_tests/slow_async_callbacks_example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/import_used_for_tests/a/__init__.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/import_used_for_tests/a/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/otel_integrations/__init__.py
+-rw-r--r--   0        0        0    24476 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/otel_integrations/test_anthropic.py
+-rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/otel_integrations/test_asgi.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/otel_integrations/test_asyncpg.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/otel_integrations/test_django.py
+-rw-r--r--   0        0        0    44449 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/otel_integrations/test_fastapi.py
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/otel_integrations/test_flask.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/otel_integrations/test_httpx.py
+-rw-r--r--   0        0        0    44469 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/otel_integrations/test_openai.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/otel_integrations/test_psycopg.py
+-rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/otel_integrations/test_requests.py
+-rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/otel_integrations/test_sqlalchemy.py
+-rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/otel_integrations/test_starlette.py
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/otel_integrations/test_wsgi.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/otel_integrations/django_test_project/__init__.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/otel_integrations/django_test_project/manage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/otel_integrations/django_test_project/django_test_app/__init__.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/otel_integrations/django_test_project/django_test_app/admin.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/otel_integrations/django_test_project/django_test_app/apps.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/otel_integrations/django_test_project/django_test_app/models.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/otel_integrations/django_test_project/django_test_app/urls.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/otel_integrations/django_test_project/django_test_app/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/otel_integrations/django_test_project/django_test_app/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/otel_integrations/django_test_project/django_test_site/__init__.py
+-rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/otel_integrations/django_test_project/django_test_site/settings.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/otel_integrations/django_test_project/django_test_site/urls.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 logfire-0.36.0/tests/otel_integrations/django_test_project/django_test_site/wsgi.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 logfire-0.36.0/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 logfire-0.36.0/LICENSE
+-rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 logfire-0.36.0/README.md
+-rw-r--r--   0        0        0     8521 2020-02-02 00:00:00.000000 logfire-0.36.0/pyproject.toml
+-rw-r--r--   0        0        0     7731 2020-02-02 00:00:00.000000 logfire-0.36.0/PKG-INFO
```

### Comparing `logfire-0.35.0/Makefile` & `logfire-0.36.0/Makefile`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/__init__.py` & `logfire-0.36.0/logfire/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,14 +12,16 @@
     PydanticPlugin,
     configure,
 )
 from ._internal.constants import LevelName
 from ._internal.exporters.file import load_file as load_spans_from_file
 from ._internal.main import Logfire, LogfireSpan
 from ._internal.scrubbing import ScrubMatch
+from .integrations.logging import LogfireLoggingHandler
+from .integrations.structlog import LogfireProcessor as StructlogProcessor
 from .version import VERSION
 
 DEFAULT_LOGFIRE_INSTANCE = Logfire()
 span = DEFAULT_LOGFIRE_INSTANCE.span
 instrument = DEFAULT_LOGFIRE_INSTANCE.instrument
 force_flush = DEFAULT_LOGFIRE_INSTANCE.force_flush
 log_slow_async_callbacks = DEFAULT_LOGFIRE_INSTANCE.log_slow_async_callbacks
@@ -95,8 +97,10 @@
     'with_tags',
     # 'with_trace_sample_rate',
     'load_spans_from_file',
     'no_auto_trace',
     'METRICS_PREFERRED_TEMPORALITY',
     'ScrubMatch',
     'VERSION',
+    'StructlogProcessor',
+    'LogfireLoggingHandler',
 )
```

### Comparing `logfire-0.35.0/logfire/propagate.py` & `logfire-0.36.0/logfire/propagate.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/testing.py` & `logfire-0.36.0/logfire/testing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/_internal/ast_utils.py` & `logfire-0.36.0/logfire/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/_internal/async_.py` & `logfire-0.36.0/logfire/_internal/async_.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/_internal/auth.py` & `logfire-0.36.0/logfire/_internal/auth.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/_internal/backfill.py` & `logfire-0.36.0/logfire/_internal/backfill.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/_internal/cli.py` & `logfire-0.36.0/logfire/_internal/cli.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/_internal/config.py` & `logfire-0.36.0/logfire/_internal/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -669,14 +669,15 @@
                 if metric_readers is None:
                     metric_readers = [
                         PeriodicExportingMetricReader(
                             OTLPMetricExporter(
                                 endpoint=self.metrics_endpoint,
                                 headers=headers,
                                 preferred_temporality=METRICS_PREFERRED_TEMPORALITY,
+                                session=session,
                             )
                         )
                     ]
 
             tracer_provider.add_span_processor(PendingSpanProcessor(self.id_generator, tuple(processors)))
 
             metric_readers = metric_readers or []
```

### Comparing `logfire-0.35.0/logfire/_internal/config_params.py` & `logfire-0.36.0/logfire/_internal/config_params.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/_internal/constants.py` & `logfire-0.36.0/logfire/_internal/constants.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/_internal/formatter.py` & `logfire-0.36.0/logfire/_internal/formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/_internal/instrument.py` & `logfire-0.36.0/logfire/_internal/instrument.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/_internal/json_encoder.py` & `logfire-0.36.0/logfire/_internal/json_encoder.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/_internal/json_formatter.py` & `logfire-0.36.0/logfire/_internal/json_formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/_internal/json_schema.py` & `logfire-0.36.0/logfire/_internal/json_schema.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/_internal/json_types.py` & `logfire-0.36.0/logfire/_internal/json_types.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/_internal/main.py` & `logfire-0.36.0/logfire/_internal/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,14 +228,16 @@
         **attributes: Any,
     ) -> None:
         """Log a trace message.
 
         ```py
         import logfire
 
+        logfire.configure()
+
         logfire.trace('This is a trace log')
         ```
 
         Args:
             msg_template: The message to log.
             attributes: The attributes to bind to the log.
             _tags: An optional sequence of tags to include in the log.
@@ -258,14 +260,16 @@
         **attributes: Any,
     ) -> None:
         """Log a debug message.
 
         ```py
         import logfire
 
+        logfire.configure()
+
         logfire.debug('This is a debug log')
         ```
 
         Args:
             msg_template: The message to log.
             attributes: The attributes to bind to the log.
             _tags: An optional sequence of tags to include in the log.
@@ -288,14 +292,16 @@
         **attributes: Any,
     ) -> None:
         """Log an info message.
 
         ```py
         import logfire
 
+        logfire.configure()
+
         logfire.info('This is an info log')
         ```
 
         Args:
             msg_template: The message to log.
             attributes: The attributes to bind to the log.
             _tags: An optional sequence of tags to include in the log.
@@ -318,14 +324,16 @@
         **attributes: Any,
     ) -> None:
         """Log a notice message.
 
         ```py
         import logfire
 
+        logfire.configure()
+
         logfire.notice('This is a notice log')
         ```
 
         Args:
             msg_template: The message to log.
             attributes: The attributes to bind to the log.
             _tags: An optional sequence of tags to include in the log.
@@ -348,14 +356,16 @@
         **attributes: Any,
     ) -> None:
         """Log a warning message.
 
         ```py
         import logfire
 
+        logfire.configure()
+
         logfire.warn('This is a warning log')
         ```
 
         Args:
             msg_template: The message to log.
             attributes: The attributes to bind to the log.
             _tags: An optional sequence of tags to include in the log.
@@ -378,14 +388,16 @@
         **attributes: Any,
     ) -> None:
         """Log an error message.
 
         ```py
         import logfire
 
+        logfire.configure()
+
         logfire.error('This is an error log')
         ```
 
         Args:
             msg_template: The message to log.
             attributes: The attributes to bind to the log.
             _tags: An optional sequence of tags to include in the log.
@@ -408,14 +420,16 @@
         **attributes: Any,
     ) -> None:
         """Log a fatal message.
 
         ```py
         import logfire
 
+        logfire.configure()
+
         logfire.fatal('This is a fatal log')
         ```
 
         Args:
             msg_template: The message to log.
             attributes: The attributes to bind to the log.
             _tags: An optional sequence of tags to include in the log.
@@ -463,14 +477,16 @@
         **attributes: Any,
     ) -> LogfireSpan:
         """Context manager for creating a span.
 
         ```py
         import logfire
 
+        logfire.configure()
+
         with logfire.span('This is a span {a=}', a='data'):
             logfire.info('new log 1')
         ```
 
         Args:
             msg_template: The template for the span message.
             _span_name: The span name. If not provided, the `msg_template` will be used.
@@ -497,14 +513,16 @@
         extract_args: bool = True,
     ) -> Callable[[Callable[_PARAMS, _RETURN]], Callable[_PARAMS, _RETURN]]:
         """Decorator for instrumenting a function as a span.
 
         ```py
         import logfire
 
+        logfire.configure()
+
 
         @logfire.instrument('This is a span {a=}')
         def my_function(a: int):
             logfire.info('new log {a=}', a=a)
         ```
 
         !!! note
@@ -530,14 +548,16 @@
         custom_scope_suffix: str | None = None,
     ) -> None:
         """Log a message.
 
         ```py
         import logfire
 
+        logfire.configure()
+
         logfire.log('info', 'This is a log {a}', {'a': 'Apple'})
         ```
 
         Args:
             level: The level of the log.
             msg_template: The message to log.
             attributes: The attributes to bind to the log.
@@ -636,14 +656,16 @@
 
     def with_tags(self, *tags: str) -> Logfire:
         """A new Logfire instance which always uses the given tags.
 
         ```py
         import logfire
 
+        logfire.configure()
+
         local_logfire = logfire.with_tags('tag1')
         local_logfire.info('a log message', _tags=['tag2'])
 
         # This is equivalent to:
         logfire.info('a log message', _tags=['tag1', 'tag2'])
         ```
 
@@ -783,14 +805,15 @@
                 dict[str, Any],
             ],
             dict[str, Any] | None,
         ]
         | None = None,
         use_opentelemetry_instrumentation: bool = True,
         excluded_urls: str | Iterable[str] | None = None,
+        **opentelemetry_kwargs: Any,
     ) -> ContextManager[None]:
         """Instrument a FastAPI app so that spans and logs are automatically created for each request.
 
         Args:
             app: The FastAPI app to instrument.
             request_attributes_mapper: A function that takes a [`Request`][fastapi.Request] or [`WebSocket`][fastapi.WebSocket]
                 and a dictionary of attributes and returns a new dictionary of attributes.
@@ -812,14 +835,15 @@
                 If not provided, the environment variables
                 `OTEL_PYTHON_FASTAPI_EXCLUDED_URLS` and `OTEL_PYTHON_EXCLUDED_URLS` will be checked.
             use_opentelemetry_instrumentation: If True (the default) then
                 [`FastAPIInstrumentor`][opentelemetry.instrumentation.fastapi.FastAPIInstrumentor]
                 will also instrument the app.
 
                 See [OpenTelemetry FastAPI Instrumentation](https://opentelemetry-python-contrib.readthedocs.io/en/latest/instrumentation/fastapi/fastapi.html).
+            opentelemetry_kwargs: Additional keyword arguments to pass to the OpenTelemetry FastAPI instrumentation.
 
         Returns:
             A context manager that will revert the instrumentation when exited.
                 This context manager doesn't take into account threads or other concurrency.
                 Calling this method will immediately apply the instrumentation
                 without waiting for the context manager to be opened,
                 i.e. it's not necessary to use this as a context manager.
@@ -828,14 +852,15 @@
 
         return instrument_fastapi(
             self,
             app,
             request_attributes_mapper=request_attributes_mapper,
             excluded_urls=excluded_urls,
             use_opentelemetry_instrumentation=use_opentelemetry_instrumentation,
+            **opentelemetry_kwargs,
         )
 
     def instrument_openai(
         self,
         openai_client: openai.OpenAI
         | openai.AsyncOpenAI
         | type[openai.OpenAI]
@@ -858,14 +883,15 @@
         Example usage:
 
         ```python
         import logfire
         import openai
 
         client = openai.OpenAI()
+        logfire.configure()
         logfire.instrument_openai(client)
 
         response = client.chat.completions.create(
             model='gpt-4',
             messages=[
                 {'role': 'system', 'content': 'You are a helpful assistant.'},
                 {'role': 'user', 'content': 'What is four plus five?'},
@@ -929,14 +955,15 @@
         Example usage:
 
         ```python
         import logfire
         import anthropic
 
         client = anthropic.Anthropic()
+        logfire.configure()
         logfire.instrument_anthropic(client)
 
         response = client.messages.create(
             model='claude-3-haiku-20240307',
             system='You are a helpful assistant.',
             messages=[
                 {'role': 'user', 'content': 'What is four plus five?'},
@@ -1081,14 +1108,15 @@
         """Create a counter metric.
 
         A counter is a cumulative metric that represents a single numerical value that only ever goes up.
 
         ```py
         import logfire
 
+        logfire.configure()
         counter = logfire.metric_counter('exceptions', unit='1', description='Number of exceptions caught')
 
         try:
             raise Exception('oops')
         except Exception:
             counter.add(1)
         ```
@@ -1110,14 +1138,15 @@
         """Create a histogram metric.
 
         A histogram is a metric that samples observations (usually things like request durations or response sizes).
 
         ```py
         import logfire
 
+        logfire.configure()
         histogram = logfire.metric_histogram('bank.amount_transferred', unit='$', description='Amount transferred')
 
 
         def transfer(amount: int):
             histogram.record(amount)
         ```
 
@@ -1137,14 +1166,15 @@
         """Create a gauge metric.
 
         Gauge is a synchronous instrument which can be used to record non-additive measurements.
 
         ```py
         import logfire
 
+        logfire.configure()
         gauge = logfire.metric_gauge('system.cpu_usage', unit='%', description='CPU usage')
 
 
         def update_cpu_usage(cpu_percent):
             gauge.set(cpu_percent)
         ```
 
@@ -1165,14 +1195,15 @@
 
         An up-down counter is a cumulative metric that represents a single numerical value that can be adjusted up or
         down.
 
         ```py
         import logfire
 
+        logfire.configure()
         up_down_counter = logfire.metric_up_down_counter('users.logged_in', unit='1', description='Users logged in')
 
 
         def on_login(user):
             up_down_counter.add(1)
 
 
@@ -1206,14 +1237,16 @@
         The counter metric is a cumulative metric that represents a single numerical value that only ever goes up.
 
         ```py
         import logfire
         import psutil
         from opentelemetry.metrics import CallbackOptions, Observation
 
+        logfire.configure()
+
 
         def cpu_usage_callback(options: CallbackOptions):
             cpu_percents = psutil.cpu_percent(percpu=True)
 
             for i, cpu_percent in enumerate(cpu_percents):
                 yield Observation(cpu_percent, {'cpu': i})
 
@@ -1247,14 +1280,16 @@
 
         ```py
         import threading
 
         import logfire
         from opentelemetry.metrics import CallbackOptions, Observation
 
+        logfire.configure()
+
 
         def thread_count_callback(options: CallbackOptions):
             yield Observation(threading.active_count())
 
 
         logfire.metric_gauge_callback(
             'system.thread_count',
@@ -1284,14 +1319,16 @@
         The up-down counter is a cumulative metric that represents a single numerical value that can be adjusted up or
         down.
 
         ```py
         import logfire
         from opentelemetry.metrics import CallbackOptions, Observation
 
+        logfire.configure()
+
         items = []
 
 
         def inventory_callback(options: CallbackOptions):
             yield Observation(len(items))
```

### Comparing `logfire-0.35.0/logfire/_internal/metrics.py` & `logfire-0.36.0/logfire/_internal/metrics.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/_internal/scrubbing.py` & `logfire-0.36.0/logfire/_internal/scrubbing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/_internal/stack_info.py` & `logfire-0.36.0/logfire/_internal/stack_info.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/_internal/tracer.py` & `logfire-0.36.0/logfire/_internal/tracer.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/_internal/utils.py` & `logfire-0.36.0/logfire/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/_internal/auto_trace/__init__.py` & `logfire-0.36.0/logfire/_internal/auto_trace/__init__.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/_internal/auto_trace/import_hook.py` & `logfire-0.36.0/logfire/_internal/auto_trace/import_hook.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/_internal/auto_trace/rewrite_ast.py` & `logfire-0.36.0/logfire/_internal/auto_trace/rewrite_ast.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/_internal/auto_trace/types.py` & `logfire-0.36.0/logfire/_internal/auto_trace/types.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/_internal/exporters/console.py` & `logfire-0.36.0/logfire/_internal/exporters/console.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/_internal/exporters/fallback.py` & `logfire-0.36.0/logfire/_internal/exporters/fallback.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/_internal/exporters/file.py` & `logfire-0.36.0/logfire/_internal/exporters/file.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/_internal/exporters/otlp.py` & `logfire-0.36.0/logfire/_internal/exporters/otlp.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from __future__ import annotations
 
 import contextlib
+import time
+from random import random
 from typing import Any, Iterable, Sequence, cast
 
+import requests.exceptions
 from opentelemetry.sdk.trace import ReadableSpan
 from opentelemetry.sdk.trace.export import SpanExportResult
 from requests import Session
 from requests.models import PreparedRequest, Response
 
 import logfire
 
@@ -34,15 +37,28 @@
                     total = 0
                     for chunk in body:
                         total += len(chunk)
                         self._check_body_size(total)
                         yield chunk
 
                 request.body = gen()  # type: ignore
-        return super().send(request, **kwargs)
+
+        max_attempts = 7
+        for attempt in range(max_attempts):  # pragma: no branch
+            try:
+                response = super().send(request, **kwargs)
+            except requests.exceptions.RequestException:
+                if attempt < max_attempts - 1:
+                    # Exponential backoff with jitter
+                    time.sleep(2**attempt + random())
+                    continue
+                raise
+            return response
+
+        raise RuntimeError('Unreachable code')  # for pyright  # pragma: no cover
 
     def _check_body_size(self, size: int) -> None:
         if size > self.max_body_size:
             raise BodyTooLargeError(size, self.max_body_size)
 
 
 class RetryFewerSpansSpanExporter(WrapperSpanExporter):
```

### Comparing `logfire-0.35.0/logfire/_internal/exporters/processor_wrapper.py` & `logfire-0.36.0/logfire/_internal/exporters/processor_wrapper.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/_internal/exporters/remove_pending.py` & `logfire-0.36.0/logfire/_internal/exporters/remove_pending.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/_internal/exporters/wrapper.py` & `logfire-0.36.0/logfire/_internal/exporters/wrapper.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/_internal/integrations/executors.py` & `logfire-0.36.0/logfire/_internal/integrations/executors.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/_internal/integrations/fastapi.py` & `logfire-0.36.0/logfire/_internal/integrations/fastapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,26 +40,27 @@
             dict[str, Any],
         ],
         dict[str, Any] | None,
     ]
     | None = None,
     use_opentelemetry_instrumentation: bool = True,
     excluded_urls: str | Iterable[str] | None = None,
+    **opentelemetry_kwargs: Any,
 ) -> ContextManager[None]:
     """Instrument a FastAPI app so that spans and logs are automatically created for each request.
 
     See `Logfire.instrument_fastapi` for more details.
     """
     # TODO(Marcelo): This needs to be tested.
     if not isinstance(excluded_urls, (str, type(None))):  # pragma: no cover
         # FastAPIInstrumentor expects a comma-separated string, not a list.
         excluded_urls = ','.join(excluded_urls)
 
     if use_opentelemetry_instrumentation:  # pragma: no branch
-        FastAPIInstrumentor.instrument_app(app, excluded_urls=excluded_urls)  # type: ignore
+        FastAPIInstrumentor.instrument_app(app, excluded_urls=excluded_urls, **opentelemetry_kwargs)  # type: ignore
 
     registry = patch_fastapi()
     if app in registry:  # pragma: no cover
         raise ValueError('This app has already been instrumented.')
 
     registry[app] = FastAPIInstrumentation(
         logfire_instance,
```

### Comparing `logfire-0.35.0/logfire/_internal/integrations/psycopg.py` & `logfire-0.36.0/logfire/_internal/integrations/psycopg.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/_internal/integrations/llm_providers/anthropic.py` & `logfire-0.36.0/logfire/_internal/integrations/llm_providers/anthropic.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/_internal/integrations/llm_providers/llm_provider.py` & `logfire-0.36.0/logfire/_internal/integrations/llm_providers/llm_provider.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/_internal/integrations/llm_providers/openai.py` & `logfire-0.36.0/logfire/_internal/integrations/llm_providers/openai.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/integrations/logging.py` & `logfire-0.36.0/logfire/integrations/logging.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 
 import inspect
 from logging import NOTSET, Handler as LoggingHandler, LogRecord, StreamHandler
 from typing import Any, ClassVar, Mapping, cast
 
-from logfire import log
+import logfire
 
 from .._internal.constants import (
     ATTRIBUTES_LOGGING_ARGS_KEY,
     ATTRIBUTES_MESSAGE_KEY,
     ATTRIBUTES_MESSAGE_TEMPLATE_KEY,
     LOGGING_TO_OTEL_LEVEL_NUMBERS,
 )
@@ -74,15 +74,15 @@
                 if frame.f_code is code_here:
                     self.fallback.emit(record)
                     return
                 frame = frame.f_back
 
         attributes = self.fill_attributes(record)
 
-        log(
+        logfire.log(
             msg_template=attributes.pop(ATTRIBUTES_MESSAGE_TEMPLATE_KEY, record.msg),
             level=LOGGING_TO_OTEL_LEVEL_NUMBERS.get(record.levelno, record.levelno),
             attributes=attributes,
             custom_scope_suffix=self.custom_scope_suffix,
             exc_info=record.exc_info,
         )
```

### Comparing `logfire-0.35.0/logfire/integrations/loguru.py` & `logfire-0.36.0/logfire/integrations/loguru.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/integrations/pydantic.py` & `logfire-0.36.0/logfire/integrations/pydantic.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/logfire/integrations/structlog.py` & `logfire-0.36.0/logfire/integrations/structlog.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/conftest.py` & `logfire-0.36.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/test_auto_trace.py` & `logfire-0.36.0/tests/test_auto_trace.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/test_backfill.py` & `logfire-0.36.0/tests/test_backfill.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/test_cli.py` & `logfire-0.36.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/test_collect_package_resources.py` & `logfire-0.36.0/tests/test_collect_package_resources.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/test_configure.py` & `logfire-0.36.0/tests/test_configure.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/test_console_exporter.py` & `logfire-0.36.0/tests/test_console_exporter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/test_formatter.py` & `logfire-0.36.0/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/test_json_args.py` & `logfire-0.36.0/tests/test_json_args.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/test_json_args_formatting.py` & `logfire-0.36.0/tests/test_json_args_formatting.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/test_logfire.py` & `logfire-0.36.0/tests/test_logfire.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/test_loguru.py` & `logfire-0.36.0/tests/test_loguru.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/test_metrics.py` & `logfire-0.36.0/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/test_no_production.py` & `logfire-0.36.0/tests/test_no_production.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/test_pydantic_plugin.py` & `logfire-0.36.0/tests/test_pydantic_plugin.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/test_sampling.py` & `logfire-0.36.0/tests/test_sampling.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/test_secret_scrubbing.py` & `logfire-0.36.0/tests/test_secret_scrubbing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/test_slow_async_callbacks.py` & `logfire-0.36.0/tests/test_slow_async_callbacks.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/test_source_code_extraction.py` & `logfire-0.36.0/tests/test_source_code_extraction.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/test_stdlib_logging.py` & `logfire-0.36.0/tests/test_stdlib_logging.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/test_structlog.py` & `logfire-0.36.0/tests/test_structlog.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/test_testing.py` & `logfire-0.36.0/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/test_utils.py` & `logfire-0.36.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/utils.py` & `logfire-0.36.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/exporters/test_fallback_exporter.py` & `logfire-0.36.0/tests/exporters/test_fallback_exporter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/exporters/test_file_exporter.py` & `logfire-0.36.0/tests/exporters/test_file_exporter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/exporters/test_otlp_session.py` & `logfire-0.36.0/tests/exporters/test_otlp_session.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from typing import Any, Iterable, cast
+from unittest.mock import Mock
 
 import pytest
+import requests.exceptions
+from dirty_equals import IsFloat
 from requests.models import PreparedRequest, Response as Response
 from requests.sessions import HTTPAdapter
 
 from logfire._internal.exporters.otlp import BodyTooLargeError, OTLPExporterHttpSession
 
 
 class SinkHTTPAdapter(HTTPAdapter):
@@ -38,7 +41,31 @@
 def test_max_body_size_generator() -> None:
     s = OTLPExporterHttpSession(max_body_size=10)
     s.mount('http://', SinkHTTPAdapter())
     s.post('http://example.com', data=iter([b'abc'] * 3))
     with pytest.raises(BodyTooLargeError) as e:
         s.post('http://example.com', data=iter([b'abc'] * 100))
     assert str(e.value) == 'Request body is too large (12 bytes), must be less than 10 bytes.'
+
+
+def test_connection_error_retries(monkeypatch: pytest.MonkeyPatch) -> None:
+    sleep_mock = Mock(return_value=0)
+    monkeypatch.setattr('time.sleep', sleep_mock)
+
+    class ConnectionErrorAdapter(HTTPAdapter):
+        def send(self, request: PreparedRequest, *args: Any, **kwargs: Any) -> Response:
+            raise requests.exceptions.ConnectionError()
+
+    session = OTLPExporterHttpSession(max_body_size=10)
+    session.mount('http://', ConnectionErrorAdapter())
+
+    with pytest.raises(requests.exceptions.ConnectionError):
+        session.post('http://example.com', data='123')
+
+    assert [call.args for call in sleep_mock.call_args_list] == [
+        (IsFloat(gt=1, lt=2),),
+        (IsFloat(gt=2, lt=3),),
+        (IsFloat(gt=4, lt=5),),
+        (IsFloat(gt=8, lt=9),),
+        (IsFloat(gt=16, lt=17),),
+        (IsFloat(gt=32, lt=33),),
+    ]
```

### Comparing `logfire-0.35.0/tests/exporters/test_remove_pending.py` & `logfire-0.36.0/tests/exporters/test_remove_pending.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/exporters/test_retry_fewer_spans.py` & `logfire-0.36.0/tests/exporters/test_retry_fewer_spans.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/import_used_for_tests/slow_async_callbacks_example.py` & `logfire-0.36.0/tests/import_used_for_tests/slow_async_callbacks_example.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/otel_integrations/test_anthropic.py` & `logfire-0.36.0/tests/otel_integrations/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/otel_integrations/test_asgi.py` & `logfire-0.36.0/tests/otel_integrations/test_asgi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/otel_integrations/test_asyncpg.py` & `logfire-0.36.0/tests/otel_integrations/test_asyncpg.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/otel_integrations/test_django.py` & `logfire-0.36.0/tests/otel_integrations/test_django.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/otel_integrations/test_fastapi.py` & `logfire-0.36.0/tests/otel_integrations/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/otel_integrations/test_flask.py` & `logfire-0.36.0/tests/otel_integrations/test_flask.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/otel_integrations/test_httpx.py` & `logfire-0.36.0/tests/otel_integrations/test_httpx.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/otel_integrations/test_openai.py` & `logfire-0.36.0/tests/otel_integrations/test_openai.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/otel_integrations/test_psycopg.py` & `logfire-0.36.0/tests/otel_integrations/test_psycopg.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/otel_integrations/test_requests.py` & `logfire-0.36.0/tests/otel_integrations/test_requests.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/otel_integrations/test_sqlalchemy.py` & `logfire-0.36.0/tests/otel_integrations/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/otel_integrations/test_starlette.py` & `logfire-0.36.0/tests/otel_integrations/test_starlette.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/otel_integrations/test_wsgi.py` & `logfire-0.36.0/tests/otel_integrations/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/otel_integrations/django_test_project/manage.py` & `logfire-0.36.0/tests/otel_integrations/django_test_project/manage.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/tests/otel_integrations/django_test_project/django_test_site/settings.py` & `logfire-0.36.0/tests/otel_integrations/django_test_project/django_test_site/settings.py`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/LICENSE` & `logfire-0.36.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/README.md` & `logfire-0.36.0/README.md`

 * *Files identical despite different names*

### Comparing `logfire-0.35.0/pyproject.toml` & `logfire-0.36.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "logfire"
-version = "0.35.0"
+version = "0.36.0"
 description = "The best Python observability tool! 🪵🔥"
 authors = [
     { name = "Pydantic Team", email = "engineering@pydantic.dev" },
     { name = "Samuel Colvin", email = "samuel@pydantic.dev" },
     { name = "Hasan Ramezani", email = "hasan@pydantic.dev" },
     { name = "Adrian Garcia Badaracco", email = "adrian@pydantic.dev" },
     { name = "David Montague", email = "david@pydantic.dev" },
```

### Comparing `logfire-0.35.0/PKG-INFO` & `logfire-0.36.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: logfire
-Version: 0.35.0
+Version: 0.36.0
 Summary: The best Python observability tool! 🪵🔥
 Author-email: Pydantic Team <engineering@pydantic.dev>, Samuel Colvin <samuel@pydantic.dev>, Hasan Ramezani <hasan@pydantic.dev>, Adrian Garcia Badaracco <adrian@pydantic.dev>, David Montague <david@pydantic.dev>, Marcelo Trylesinski <marcelo@pydantic.dev>, David Hewitt <david.hewitt@pydantic.dev>, Alex Hall <alex@pydantic.dev>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
```

