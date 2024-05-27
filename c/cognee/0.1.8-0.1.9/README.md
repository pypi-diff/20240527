# Comparing `tmp/cognee-0.1.8.tar.gz` & `tmp/cognee-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognee-0.1.8.tar", max compression
+gzip compressed data, was "cognee-0.1.9.tar", max compression
```

## Comparing `cognee-0.1.8.tar` & `cognee-0.1.9.tar`

### file list

```diff
@@ -1,570 +1,574 @@
--rw-r--r--   0        0        0    11344 2024-04-23 05:20:06.866180 cognee-0.1.8/LICENSE
--rw-r--r--   0        0        0     3943 2024-05-27 05:37:00.853829 cognee-0.1.8/README.md
--rw-r--r--   0        0        0      186 2024-05-10 20:47:32.390494 cognee-0.1.8/cognee/.data/code/e6ac18788c6a51dfaaf9b963d5bc094b.txt
--rw-r--r--   0        0        0     1257 2024-05-09 09:29:57.011777 cognee-0.1.8/cognee/.data/example/.craft.txt
--rw-r--r--   0        0        0      716 2024-05-09 09:29:57.009663 cognee-0.1.8/cognee/.data/example/.flake8.txt
--rw-r--r--   0        0        0      269 2024-05-09 09:29:57.011322 cognee-0.1.8/cognee/.data/example/.gitignore.txt
--rw-r--r--   0        0        0      124 2024-05-09 09:29:57.010913 cognee-0.1.8/cognee/.data/example/.gitmodules.txt
--rw-r--r--   0        0        0      636 2024-05-09 09:29:57.010239 cognee-0.1.8/cognee/.data/example/.pre-commit-config.txt
--rw-r--r--   0        0        0       14 2024-05-09 09:29:57.010581 cognee-0.1.8/cognee/.data/example/.tool-versions.txt
--rw-r--r--   0        0        0    97420 2024-05-09 09:29:57.010128 cognee-0.1.8/cognee/.data/example/CHANGELOG.txt
--rw-r--r--   0        0        0     1169 2024-05-09 09:29:57.010808 cognee-0.1.8/cognee/.data/example/CONTRIBUTING-aws-lambda.txt
--rw-r--r--   0        0        0     9702 2024-05-09 09:29:57.011552 cognee-0.1.8/cognee/.data/example/CONTRIBUTING.txt
--rw-r--r--   0        0        0     1093 2024-05-09 09:29:57.009989 cognee-0.1.8/cognee/.data/example/LICENSE.txt
--rw-r--r--   0        0        0       44 2024-05-09 09:29:57.010692 cognee-0.1.8/cognee/.data/example/MANIFEST.txt
--rw-r--r--   0        0        0     1751 2024-05-09 09:29:57.010349 cognee-0.1.8/cognee/.data/example/Makefile.txt
--rw-r--r--   0        0        0     4974 2024-05-09 09:29:57.011021 cognee-0.1.8/cognee/.data/example/README.txt
--rw-r--r--   0        0        0      222 2024-05-09 09:29:56.911149 cognee-0.1.8/cognee/.data/example/aws-lambda-layer-requirements.txt
--rw-r--r--   0        0        0      336 2024-05-09 09:29:57.009783 cognee-0.1.8/cognee/.data/example/codecov.txt
--rw-r--r--   0        0        0      304 2024-05-09 09:29:56.911335 cognee-0.1.8/cognee/.data/example/devenv-requirements.txt
--rw-r--r--   0        0        0        7 2024-05-09 09:29:57.053281 cognee-0.1.8/cognee/.data/example/docs/.gitignore.txt
--rw-r--r--   0        0        0        0 2024-05-09 09:29:57.053711 cognee-0.1.8/cognee/.data/example/docs/_static/.gitkeep.txt
--rw-r--r--   0        0        0     1314 2024-05-09 09:29:57.053508 cognee-0.1.8/cognee/.data/example/docs/api.txt
--rw-r--r--   0        0        0      849 2024-05-09 09:29:57.053402 cognee-0.1.8/cognee/.data/example/docs/apidocs.txt
--rw-r--r--   0        0        0     5638 2024-05-09 09:29:57.053152 cognee-0.1.8/cognee/.data/example/docs/conf.txt
--rw-r--r--   0        0        0      376 2024-05-09 09:29:57.053022 cognee-0.1.8/cognee/.data/example/docs/index.txt
--rw-r--r--   0        0        0      202 2024-05-09 09:29:57.053615 cognee-0.1.8/cognee/.data/example/docs/integrations.txt
--rw-r--r--   0        0        0       87 2024-05-09 09:29:56.911395 cognee-0.1.8/cognee/.data/example/docs-requirements.txt
--rw-r--r--   0        0        0      381 2024-05-09 09:29:56.980677 cognee-0.1.8/cognee/.data/example/linter-requirements.txt
--rw-r--r--   0        0        0     1900 2024-05-09 09:29:57.011115 cognee-0.1.8/cognee/.data/example/mypy.txt
--rw-r--r--   0        0        0      394 2024-05-09 09:29:57.010472 cognee-0.1.8/cognee/.data/example/pyproject.txt
--rw-r--r--   0        0        0      519 2024-05-09 09:29:57.009890 cognee-0.1.8/cognee/.data/example/pytest.txt
--rw-r--r--   0        0        0     1002 2024-05-09 09:29:57.053856 cognee-0.1.8/cognee/.data/example/scripts/aws-attach-layer-to-lambda-function.txt
--rw-r--r--   0        0        0      641 2024-05-09 09:29:57.054177 cognee-0.1.8/cognee/.data/example/scripts/aws-cleanup.txt
--rw-r--r--   0        0        0      464 2024-05-09 09:29:57.054550 cognee-0.1.8/cognee/.data/example/scripts/aws-delete-lamba-layer-versions.txt
--rw-r--r--   0        0        0     1065 2024-05-09 09:29:57.054071 cognee-0.1.8/cognee/.data/example/scripts/aws-deploy-local-layer.txt
--rw-r--r--   0        0        0     4709 2024-05-09 09:29:57.054423 cognee-0.1.8/cognee/.data/example/scripts/build_aws_lambda_layer.txt
--rw-r--r--   0        0        0      641 2024-05-09 09:29:57.053957 cognee-0.1.8/cognee/.data/example/scripts/bump-version.txt
--rw-r--r--   0        0        0     2975 2024-05-09 09:29:57.054281 cognee-0.1.8/cognee/.data/example/scripts/init_serverless_sdk.txt
--rw-r--r--   0        0        0      846 2024-05-09 09:29:57.054658 cognee-0.1.8/cognee/.data/example/scripts/runtox.txt
--rw-r--r--   0        0        0     9179 2024-05-09 09:29:57.054884 cognee-0.1.8/cognee/.data/example/scripts/split-tox-gh-actions/split-tox-gh-actions.txt
--rw-r--r--   0        0        0     1623 2024-05-09 09:29:57.055265 cognee-0.1.8/cognee/.data/example/scripts/split-tox-gh-actions/templates/base.txt
--rw-r--r--   0        0        0     1065 2024-05-09 09:29:57.055380 cognee-0.1.8/cognee/.data/example/scripts/split-tox-gh-actions/templates/check_permissions.txt
--rw-r--r--   0        0        0     1101 2024-05-09 09:29:57.055148 cognee-0.1.8/cognee/.data/example/scripts/split-tox-gh-actions/templates/check_required.txt
--rw-r--r--   0        0        0     3966 2024-05-09 09:29:57.055041 cognee-0.1.8/cognee/.data/example/scripts/split-tox-gh-actions/templates/test_group.txt
--rw-r--r--   0        0        0     1069 2024-05-09 09:29:57.038396 cognee-0.1.8/cognee/.data/example/sentry_sdk/__init__.txt
--rw-r--r--   0        0        0     6936 2024-05-09 09:29:57.040081 cognee-0.1.8/cognee/.data/example/sentry_sdk/_compat.txt
--rw-r--r--   0        0        0     4957 2024-05-09 09:29:57.038744 cognee-0.1.8/cognee/.data/example/sentry_sdk/_functools.txt
--rw-r--r--   0        0        0     5390 2024-05-09 09:29:57.038165 cognee-0.1.8/cognee/.data/example/sentry_sdk/_lru_cache.txt
--rw-r--r--   0        0        0    11267 2024-05-09 09:29:57.038619 cognee-0.1.8/cognee/.data/example/sentry_sdk/_queue.txt
--rw-r--r--   0        0        0     5652 2024-05-09 09:29:57.037298 cognee-0.1.8/cognee/.data/example/sentry_sdk/_types.txt
--rw-r--r--   0        0        0     3790 2024-05-09 09:29:57.037832 cognee-0.1.8/cognee/.data/example/sentry_sdk/_werkzeug.txt
--rw-r--r--   0        0        0     6242 2024-05-09 09:29:57.039448 cognee-0.1.8/cognee/.data/example/sentry_sdk/api.txt
--rw-r--r--   0        0        0     1811 2024-05-09 09:29:57.039335 cognee-0.1.8/cognee/.data/example/sentry_sdk/attachments.txt
--rw-r--r--   0        0        0    28495 2024-05-09 09:29:57.038042 cognee-0.1.8/cognee/.data/example/sentry_sdk/client.txt
--rw-r--r--   0        0        0    11598 2024-05-09 09:29:57.039201 cognee-0.1.8/cognee/.data/example/sentry_sdk/consts.txt
--rw-r--r--   0        0        0      170 2024-05-09 09:29:57.052548 cognee-0.1.8/cognee/.data/example/sentry_sdk/crons/__init__.txt
--rw-r--r--   0        0        0      953 2024-05-09 09:29:57.052320 cognee-0.1.8/cognee/.data/example/sentry_sdk/crons/_decorator.txt
--rw-r--r--   0        0        0      506 2024-05-09 09:29:57.052872 cognee-0.1.8/cognee/.data/example/sentry_sdk/crons/_decorator_py2.txt
--rw-r--r--   0        0        0     1527 2024-05-09 09:29:57.052775 cognee-0.1.8/cognee/.data/example/sentry_sdk/crons/api.txt
--rw-r--r--   0        0        0       87 2024-05-09 09:29:57.052670 cognee-0.1.8/cognee/.data/example/sentry_sdk/crons/consts.txt
--rw-r--r--   0        0        0     2401 2024-05-09 09:29:57.052446 cognee-0.1.8/cognee/.data/example/sentry_sdk/crons/decorator.txt
--rw-r--r--   0        0        0        0 2024-05-09 09:29:57.051812 cognee-0.1.8/cognee/.data/example/sentry_sdk/db/__init__.txt
--rw-r--r--   0        0        0     1534 2024-05-09 09:29:57.052073 cognee-0.1.8/cognee/.data/example/sentry_sdk/db/explain_plan/__init__.txt
--rw-r--r--   0        0        0     1597 2024-05-09 09:29:57.051960 cognee-0.1.8/cognee/.data/example/sentry_sdk/db/explain_plan/django.txt
--rw-r--r--   0        0        0     1656 2024-05-09 09:29:57.052172 cognee-0.1.8/cognee/.data/example/sentry_sdk/db/explain_plan/sqlalchemy.txt
--rw-r--r--   0        0        0     1132 2024-05-09 09:29:57.039702 cognee-0.1.8/cognee/.data/example/sentry_sdk/debug.txt
--rw-r--r--   0        0        0     9708 2024-05-09 09:29:57.040585 cognee-0.1.8/cognee/.data/example/sentry_sdk/envelope.txt
--rw-r--r--   0        0        0    22723 2024-05-09 09:29:57.038984 cognee-0.1.8/cognee/.data/example/sentry_sdk/hub.txt
--rw-r--r--   0        0        0     7298 2024-05-09 09:29:57.043701 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/__init__.txt
--rw-r--r--   0        0        0     3096 2024-05-09 09:29:57.047520 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/_asgi_common.txt
--rw-r--r--   0        0        0     5286 2024-05-09 09:29:57.042096 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/_wsgi_common.txt
--rw-r--r--   0        0        0    11591 2024-05-09 09:29:57.041477 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/aiohttp.txt
--rw-r--r--   0        0        0      963 2024-05-09 09:29:57.045018 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/argv.txt
--rw-r--r--   0        0        0     6228 2024-05-09 09:29:57.046006 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/ariadne.txt
--rw-r--r--   0        0        0     7180 2024-05-09 09:29:57.045165 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/arq.txt
--rw-r--r--   0        0        0    11873 2024-05-09 09:29:57.043130 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/asgi.txt
--rw-r--r--   0        0        0     3201 2024-05-09 09:29:57.043267 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/asyncio.txt
--rw-r--r--   0        0        0     6297 2024-05-09 09:29:57.041724 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/asyncpg.txt
--rw-r--r--   0        0        0     1846 2024-05-09 09:29:57.043827 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/atexit.txt
--rw-r--r--   0        0        0    15922 2024-05-09 09:29:57.041855 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/aws_lambda.txt
--rw-r--r--   0        0        0     5689 2024-05-09 09:29:57.046865 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/beam.txt
--rw-r--r--   0        0        0     4542 2024-05-09 09:29:57.046387 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/boto3.txt
--rw-r--r--   0        0        0     6453 2024-05-09 09:29:57.046735 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/bottle.txt
--rw-r--r--   0        0        0    21973 2024-05-09 09:29:57.045547 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/celery.txt
--rw-r--r--   0        0        0     4769 2024-05-09 09:29:57.045835 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/chalice.txt
--rw-r--r--   0        0        0     5107 2024-05-09 09:29:57.044217 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/clickhouse_driver.txt
--rw-r--r--   0        0        0     6755 2024-05-09 09:29:57.043423 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/cloud_resource_context.txt
--rw-r--r--   0        0        0     1184 2024-05-09 09:29:57.042549 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/dedupe.txt
--rw-r--r--   0        0        0    24135 2024-05-09 09:29:57.050785 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/django/__init__.txt
--rw-r--r--   0        0        0     7056 2024-05-09 09:29:57.050660 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/django/asgi.txt
--rw-r--r--   0        0        0     3692 2024-05-09 09:29:57.050997 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/django/caching.txt
--rw-r--r--   0        0        0     5967 2024-05-09 09:29:57.051109 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/django/middleware.txt
--rw-r--r--   0        0        0     3054 2024-05-09 09:29:57.050414 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/django/signals_handlers.txt
--rw-r--r--   0        0        0     5697 2024-05-09 09:29:57.050891 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/django/templates.txt
--rw-r--r--   0        0        0     5005 2024-05-09 09:29:57.050536 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/django/transactions.txt
--rw-r--r--   0        0        0     2909 2024-05-09 09:29:57.051222 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/django/views.txt
--rw-r--r--   0        0        0     2260 2024-05-09 09:29:57.047930 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/excepthook.txt
--rw-r--r--   0        0        0     2041 2024-05-09 09:29:57.044635 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/executing.txt
--rw-r--r--   0        0        0     9496 2024-05-09 09:29:57.047081 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/falcon.txt
--rw-r--r--   0        0        0     4685 2024-05-09 09:29:57.042209 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/fastapi.txt
--rw-r--r--   0        0        0     7808 2024-05-09 09:29:57.042659 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/flask.txt
--rw-r--r--   0        0        0     8273 2024-05-09 09:29:57.047406 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/gcp.txt
--rw-r--r--   0        0        0     2906 2024-05-09 09:29:57.045682 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/gnu_backtrace.txt
--rw-r--r--   0        0        0     4435 2024-05-09 09:29:57.048081 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/gql.txt
--rw-r--r--   0        0        0     3746 2024-05-09 09:29:57.046155 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/graphene.txt
--rw-r--r--   0        0        0     4979 2024-05-09 09:29:57.048716 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/grpc/__init__.txt
--rw-r--r--   0        0        0      104 2024-05-09 09:29:57.049054 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/grpc/aio/__init__.txt
--rw-r--r--   0        0        0     3078 2024-05-09 09:29:57.048946 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/grpc/aio/client.txt
--rw-r--r--   0        0        0     3901 2024-05-09 09:29:57.048847 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/grpc/aio/server.txt
--rw-r--r--   0        0        0     3235 2024-05-09 09:29:57.048587 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/grpc/client.txt
--rw-r--r--   0        0        0     2321 2024-05-09 09:29:57.048479 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/grpc/server.txt
--rw-r--r--   0        0        0     5005 2024-05-09 09:29:57.042430 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/httpx.txt
--rw-r--r--   0        0        0     5489 2024-05-09 09:29:57.041167 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/huey.txt
--rw-r--r--   0        0        0     9573 2024-05-09 09:29:57.041050 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/logging.txt
--rw-r--r--   0        0        0     3051 2024-05-09 09:29:57.047807 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/loguru.txt
--rw-r--r--   0        0        0      872 2024-05-09 09:29:57.046271 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/modules.txt
--rw-r--r--   0        0        0    11253 2024-05-09 09:29:57.044872 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/openai.txt
--rw-r--r--   0        0        0      210 2024-05-09 09:29:57.049551 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/opentelemetry/__init__.txt
--rw-r--r--   0        0        0      167 2024-05-09 09:29:57.049669 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/opentelemetry/consts.txt
--rw-r--r--   0        0        0     5830 2024-05-09 09:29:57.049999 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/opentelemetry/integration.txt
--rw-r--r--   0        0        0     3731 2024-05-09 09:29:57.050128 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/opentelemetry/propagator.txt
--rw-r--r--   0        0        0    12355 2024-05-09 09:29:57.050285 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/opentelemetry/span_processor.txt
--rw-r--r--   0        0        0     4554 2024-05-09 09:29:57.042318 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/pure_eval.txt
--rw-r--r--   0        0        0     6007 2024-05-09 09:29:57.044362 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/pymongo.txt
--rw-r--r--   0        0        0     7447 2024-05-09 09:29:57.041983 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/pyramid.txt
--rw-r--r--   0        0        0     7494 2024-05-09 09:29:57.041275 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/quart.txt
--rw-r--r--   0        0        0    11998 2024-05-09 09:29:57.049412 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/redis/__init__.txt
--rw-r--r--   0        0        0     2630 2024-05-09 09:29:57.049192 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/redis/asyncio.txt
--rw-r--r--   0        0        0     5591 2024-05-09 09:29:57.043571 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/rq.txt
--rw-r--r--   0        0        0    13424 2024-05-09 09:29:57.047678 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/sanic.txt
--rw-r--r--   0        0        0     1975 2024-05-09 09:29:57.040752 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/serverless.txt
--rw-r--r--   0        0        0     2945 2024-05-09 09:29:57.047198 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/socket.txt
--rw-r--r--   0        0        0      208 2024-05-09 09:29:57.051492 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/spark/__init__.txt
--rw-r--r--   0        0        0     8483 2024-05-09 09:29:57.051700 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/spark/spark_driver.txt
--rw-r--r--   0        0        0     4013 2024-05-09 09:29:57.051374 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/spark/spark_worker.txt
--rw-r--r--   0        0        0     5052 2024-05-09 09:29:57.045286 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/sqlalchemy.txt
--rw-r--r--   0        0        0    24295 2024-05-09 09:29:57.040853 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/starlette.txt
--rw-r--r--   0        0        0    10211 2024-05-09 09:29:57.044072 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/starlite.txt
--rw-r--r--   0        0        0     8326 2024-05-09 09:29:57.046611 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/stdlib.txt
--rw-r--r--   0        0        0    14466 2024-05-09 09:29:57.041605 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/strawberry.txt
--rw-r--r--   0        0        0     2937 2024-05-09 09:29:57.044499 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/threading.txt
--rw-r--r--   0        0        0     7337 2024-05-09 09:29:57.045409 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/tornado.txt
--rw-r--r--   0        0        0     1745 2024-05-09 09:29:57.042872 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/trytond.txt
--rw-r--r--   0        0        0     9570 2024-05-09 09:29:57.048322 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/wsgi.txt
--rw-r--r--   0        0        0    29551 2024-05-09 09:29:57.036871 cognee-0.1.8/cognee/.data/example/sentry_sdk/metrics.txt
--rw-r--r--   0        0        0     3728 2024-05-09 09:29:57.037398 cognee-0.1.8/cognee/.data/example/sentry_sdk/monitor.txt
--rw-r--r--   0        0        0    33083 2024-05-09 09:29:57.040230 cognee-0.1.8/cognee/.data/example/sentry_sdk/profiler.txt
--rw-r--r--   0        0        0        0 2024-05-09 09:29:57.039787 cognee-0.1.8/cognee/.data/example/sentry_sdk/py.txt
--rw-r--r--   0        0        0    44786 2024-05-09 09:29:57.040370 cognee-0.1.8/cognee/.data/example/sentry_sdk/scope.txt
--rw-r--r--   0        0        0     5230 2024-05-09 09:29:57.037938 cognee-0.1.8/cognee/.data/example/sentry_sdk/scrubber.txt
--rw-r--r--   0        0        0    13301 2024-05-09 09:29:57.039928 cognee-0.1.8/cognee/.data/example/sentry_sdk/serializer.txt
--rw-r--r--   0        0        0     5612 2024-05-09 09:29:57.038280 cognee-0.1.8/cognee/.data/example/sentry_sdk/session.txt
--rw-r--r--   0        0        0     6488 2024-05-09 09:29:57.037077 cognee-0.1.8/cognee/.data/example/sentry_sdk/sessions.txt
--rw-r--r--   0        0        0     1443 2024-05-09 09:29:57.036975 cognee-0.1.8/cognee/.data/example/sentry_sdk/spotlight.txt
--rw-r--r--   0        0        0    36352 2024-05-09 09:29:57.037187 cognee-0.1.8/cognee/.data/example/sentry_sdk/tracing.txt
--rw-r--r--   0        0        0    15841 2024-05-09 09:29:57.037737 cognee-0.1.8/cognee/.data/example/sentry_sdk/tracing_utils.txt
--rw-r--r--   0        0        0     1244 2024-05-09 09:29:57.036769 cognee-0.1.8/cognee/.data/example/sentry_sdk/tracing_utils_py2.txt
--rw-r--r--   0        0        0     2146 2024-05-09 09:29:57.037501 cognee-0.1.8/cognee/.data/example/sentry_sdk/tracing_utils_py3.txt
--rw-r--r--   0        0        0    21702 2024-05-09 09:29:57.037607 cognee-0.1.8/cognee/.data/example/sentry_sdk/transport.txt
--rw-r--r--   0        0        0      732 2024-05-09 09:29:57.038864 cognee-0.1.8/cognee/.data/example/sentry_sdk/types.txt
--rw-r--r--   0        0        0    54025 2024-05-09 09:29:57.039580 cognee-0.1.8/cognee/.data/example/sentry_sdk/utils.txt
--rw-r--r--   0        0        0     4485 2024-05-09 09:29:57.036658 cognee-0.1.8/cognee/.data/example/sentry_sdk/worker.txt
--rw-r--r--   0        0        0     4122 2024-05-09 09:29:57.011213 cognee-0.1.8/cognee/.data/example/setup.txt
--rw-r--r--   0        0        0      480 2024-05-09 09:29:56.995867 cognee-0.1.8/cognee/.data/example/test-requirements.txt
--rw-r--r--   0        0        0      433 2024-05-09 09:29:57.013056 cognee-0.1.8/cognee/.data/example/tests/__init__.txt
--rw-r--r--   0        0        0    20029 2024-05-09 09:29:57.012191 cognee-0.1.8/cognee/.data/example/tests/conftest.txt
--rw-r--r--   0        0        0        0 2024-05-09 09:29:57.036393 cognee-0.1.8/cognee/.data/example/tests/crons/__init__.txt
--rw-r--r--   0        0        0     9713 2024-05-09 09:29:57.036322 cognee-0.1.8/cognee/.data/example/tests/crons/test_crons.txt
--rw-r--r--   0        0        0     4240 2024-05-09 09:29:57.036502 cognee-0.1.8/cognee/.data/example/tests/crons/test_crons_async_py3.txt
--rw-r--r--   0        0        0        0 2024-05-09 09:29:57.016035 cognee-0.1.8/cognee/.data/example/tests/integrations/__init__.txt
--rw-r--r--   0        0        0       46 2024-05-09 09:29:57.016847 cognee-0.1.8/cognee/.data/example/tests/integrations/aiohttp/__init__.txt
--rw-r--r--   0        0        0    16055 2024-05-09 09:29:57.016677 cognee-0.1.8/cognee/.data/example/tests/integrations/aiohttp/test_aiohttp.txt
--rw-r--r--   0        0        0      420 2024-05-09 09:29:57.022727 cognee-0.1.8/cognee/.data/example/tests/integrations/argv/test_argv.txt
--rw-r--r--   0        0        0      106 2024-05-09 09:29:57.017767 cognee-0.1.8/cognee/.data/example/tests/integrations/ariadne/__init__.txt
--rw-r--r--   0        0        0     7492 2024-05-09 09:29:57.017895 cognee-0.1.8/cognee/.data/example/tests/integrations/ariadne/test_ariadne.txt
--rw-r--r--   0        0        0       42 2024-05-09 09:29:57.029021 cognee-0.1.8/cognee/.data/example/tests/integrations/arq/__init__.txt
--rw-r--r--   0        0        0     7441 2024-05-09 09:29:57.029147 cognee-0.1.8/cognee/.data/example/tests/integrations/arq/test_arq.txt
--rw-r--r--   0        0        0      129 2024-05-09 09:29:57.017418 cognee-0.1.8/cognee/.data/example/tests/integrations/asgi/__init__.txt
--rw-r--r--   0        0        0    19269 2024-05-09 09:29:57.017304 cognee-0.1.8/cognee/.data/example/tests/integrations/asgi/test_asgi.txt
--rw-r--r--   0        0        0        0 2024-05-09 09:29:57.033896 cognee-0.1.8/cognee/.data/example/tests/integrations/asyncio/__init__.txt
--rw-r--r--   0        0        0    10705 2024-05-09 09:29:57.033806 cognee-0.1.8/cognee/.data/example/tests/integrations/asyncio/test_asyncio_py3.txt
--rw-r--r--   0        0        0      324 2024-05-09 09:29:57.019807 cognee-0.1.8/cognee/.data/example/tests/integrations/asyncpg/__init__.txt
--rw-r--r--   0        0        0        0 2024-05-09 09:29:57.019908 cognee-0.1.8/cognee/.data/example/tests/integrations/asyncpg/asyncpg_helpers/__init__.txt
--rw-r--r--   0        0        0       94 2024-05-09 09:29:57.020039 cognee-0.1.8/cognee/.data/example/tests/integrations/asyncpg/asyncpg_helpers/helpers.txt
--rw-r--r--   0        0        0    21423 2024-05-09 09:29:57.019699 cognee-0.1.8/cognee/.data/example/tests/integrations/asyncpg/test_asyncpg.txt
--rw-r--r--   0        0        0       44 2024-05-09 09:29:57.029812 cognee-0.1.8/cognee/.data/example/tests/integrations/aws_lambda/__init__.txt
--rw-r--r--   0        0        0    12514 2024-05-09 09:29:57.029697 cognee-0.1.8/cognee/.data/example/tests/integrations/aws_lambda/client.txt
--rw-r--r--   0        0        0    28565 2024-05-09 09:29:57.029563 cognee-0.1.8/cognee/.data/example/tests/integrations/aws_lambda/test_aws.txt
--rw-r--r--   0        0        0       50 2024-05-09 09:29:57.028442 cognee-0.1.8/cognee/.data/example/tests/integrations/beam/__init__.txt
--rw-r--r--   0        0        0     5932 2024-05-09 09:29:57.028546 cognee-0.1.8/cognee/.data/example/tests/integrations/beam/test_beam.txt
--rw-r--r--   0        0        0      230 2024-05-09 09:29:57.035552 cognee-0.1.8/cognee/.data/example/tests/integrations/boto3/__init__.txt
--rw-r--r--   0        0        0      883 2024-05-09 09:29:57.035756 cognee-0.1.8/cognee/.data/example/tests/integrations/boto3/aws_mock.txt
--rw-r--r--   0        0        0      869 2024-05-09 09:29:57.035662 cognee-0.1.8/cognee/.data/example/tests/integrations/boto3/s3_list.txt
--rw-r--r--   0        0        0     4335 2024-05-09 09:29:57.035866 cognee-0.1.8/cognee/.data/example/tests/integrations/boto3/test_s3.txt
--rw-r--r--   0        0        0       45 2024-05-09 09:29:57.034716 cognee-0.1.8/cognee/.data/example/tests/integrations/bottle/__init__.txt
--rw-r--r--   0        0        0    12198 2024-05-09 09:29:57.034606 cognee-0.1.8/cognee/.data/example/tests/integrations/bottle/test_bottle.txt
--rw-r--r--   0        0        0       45 2024-05-09 09:29:57.028760 cognee-0.1.8/cognee/.data/example/tests/integrations/celery/__init__.txt
--rw-r--r--   0        0        0    18668 2024-05-09 09:29:57.028664 cognee-0.1.8/cognee/.data/example/tests/integrations/celery/test_celery.txt
--rw-r--r--   0        0        0    16058 2024-05-09 09:29:57.028884 cognee-0.1.8/cognee/.data/example/tests/integrations/celery/test_celery_beat_crons.txt
--rw-r--r--   0        0        0       46 2024-05-09 09:29:57.025974 cognee-0.1.8/cognee/.data/example/tests/integrations/chalice/__init__.txt
--rw-r--r--   0        0        0     4389 2024-05-09 09:29:57.026110 cognee-0.1.8/cognee/.data/example/tests/integrations/chalice/test_chalice.txt
--rw-r--r--   0        0        0       56 2024-05-09 09:29:57.017020 cognee-0.1.8/cognee/.data/example/tests/integrations/clickhouse_driver/__init__.txt
--rw-r--r--   0        0        0    28896 2024-05-09 09:29:57.017158 cognee-0.1.8/cognee/.data/example/tests/integrations/clickhouse_driver/test_clickhouse_driver.txt
--rw-r--r--   0        0        0        0 2024-05-09 09:29:57.035968 cognee-0.1.8/cognee/.data/example/tests/integrations/cloud_resource_context/__init__.txt
--rw-r--r--   0        0        0    12836 2024-05-09 09:29:57.036097 cognee-0.1.8/cognee/.data/example/tests/integrations/cloud_resource_context/test_cloud_resource_context.txt
--rw-r--r--   0        0        0      560 2024-05-09 09:29:57.015962 cognee-0.1.8/cognee/.data/example/tests/integrations/conftest.txt
--rw-r--r--   0        0        0      284 2024-05-09 09:29:57.030192 cognee-0.1.8/cognee/.data/example/tests/integrations/django/__init__.txt
--rw-r--r--   0        0        0       47 2024-05-09 09:29:57.031017 cognee-0.1.8/cognee/.data/example/tests/integrations/django/asgi/__init__.txt
--rw-r--r--   0        0        0      308 2024-05-09 09:29:57.031144 cognee-0.1.8/cognee/.data/example/tests/integrations/django/asgi/image.txt
--rw-r--r--   0        0        0    16055 2024-05-09 09:29:57.030892 cognee-0.1.8/cognee/.data/example/tests/integrations/django/asgi/test_asgi.txt
--rw-r--r--   0        0        0        0 2024-05-09 09:29:57.030628 cognee-0.1.8/cognee/.data/example/tests/integrations/django/django_helpers/__init__.txt
--rw-r--r--   0        0        0      302 2024-05-09 09:29:57.030737 cognee-0.1.8/cognee/.data/example/tests/integrations/django/django_helpers/views.txt
--rw-r--r--   0        0        0        0 2024-05-09 09:29:57.031355 cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/__init__.txt
--rw-r--r--   0        0        0      487 2024-05-09 09:29:57.031276 cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/asgi.txt
--rw-r--r--   0        0        0     1020 2024-05-09 09:29:57.031796 cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/custom_urls.txt
--rw-r--r--   0        0        0      284 2024-05-09 09:29:57.031695 cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/manage.txt
--rw-r--r--   0        0        0        0 2024-05-09 09:29:57.032366 cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/management/__init__.txt
--rw-r--r--   0        0        0        0 2024-05-09 09:29:57.032465 cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/management/commands/__init__.txt
--rw-r--r--   0        0        0      187 2024-05-09 09:29:57.032577 cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/management/commands/mycrash.txt
--rw-r--r--   0        0        0      784 2024-05-09 09:29:57.032028 cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/middleware.txt
--rw-r--r--   0        0        0      494 2024-05-09 09:29:57.031471 cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/routing.txt
--rw-r--r--   0        0        0     5143 2024-05-09 09:29:57.031582 cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/settings.txt
--rw-r--r--   0        0        0       75 2024-05-09 09:29:57.033264 cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/templates/error.txt
--rw-r--r--   0        0        0       24 2024-05-09 09:29:57.032917 cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/templates/trace_meta.txt
--rw-r--r--   0        0        0       35 2024-05-09 09:29:57.033115 cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/templates/user_name.txt
--rw-r--r--   0        0        0     4349 2024-05-09 09:29:57.031918 cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/urls.txt
--rw-r--r--   0        0        0     6039 2024-05-09 09:29:57.032156 cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/views.txt
--rw-r--r--   0        0        0      419 2024-05-09 09:29:57.032272 cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/wsgi.txt
--rw-r--r--   0        0        0    43217 2024-05-09 09:29:57.029965 cognee-0.1.8/cognee/.data/example/tests/integrations/django/test_basic.txt
--rw-r--r--   0        0        0     2440 2024-05-09 09:29:57.030078 cognee-0.1.8/cognee/.data/example/tests/integrations/django/test_data_scrubbing.txt
--rw-r--r--   0        0        0    15173 2024-05-09 09:29:57.030522 cognee-0.1.8/cognee/.data/example/tests/integrations/django/test_db_query_data.txt
--rw-r--r--   0        0        0     4077 2024-05-09 09:29:57.030290 cognee-0.1.8/cognee/.data/example/tests/integrations/django/test_transactions.txt
--rw-r--r--   0        0        0      729 2024-05-09 09:29:57.030404 cognee-0.1.8/cognee/.data/example/tests/integrations/django/utils.txt
--rw-r--r--   0        0        0     1733 2024-05-09 09:29:57.018268 cognee-0.1.8/cognee/.data/example/tests/integrations/excepthook/test_excepthook.txt
--rw-r--r--   0        0        0       45 2024-05-09 09:29:57.033580 cognee-0.1.8/cognee/.data/example/tests/integrations/falcon/__init__.txt
--rw-r--r--   0        0        0    12435 2024-05-09 09:29:57.033459 cognee-0.1.8/cognee/.data/example/tests/integrations/falcon/test_falcon.txt
--rw-r--r--   0        0        0       46 2024-05-09 09:29:57.027067 cognee-0.1.8/cognee/.data/example/tests/integrations/fastapi/__init__.txt
--rw-r--r--   0        0        0    14337 2024-05-09 09:29:57.026952 cognee-0.1.8/cognee/.data/example/tests/integrations/fastapi/test_fastapi.txt
--rw-r--r--   0        0        0       44 2024-05-09 09:29:57.016386 cognee-0.1.8/cognee/.data/example/tests/integrations/flask/__init__.txt
--rw-r--r--   0        0        0    27402 2024-05-09 09:29:57.016489 cognee-0.1.8/cognee/.data/example/tests/integrations/flask/test_flask.txt
--rw-r--r--   0        0        0    17513 2024-05-09 09:29:57.024038 cognee-0.1.8/cognee/.data/example/tests/integrations/gcp/test_gcp.txt
--rw-r--r--   0        0        0       42 2024-05-09 09:29:57.021775 cognee-0.1.8/cognee/.data/example/tests/integrations/gql/__init__.txt
--rw-r--r--   0        0        0     7366 2024-05-09 09:29:57.021884 cognee-0.1.8/cognee/.data/example/tests/integrations/gql/test_gql.txt
--rw-r--r--   0        0        0      107 2024-05-09 09:29:57.026643 cognee-0.1.8/cognee/.data/example/tests/integrations/graphene/__init__.txt
--rw-r--r--   0        0        0     5663 2024-05-09 09:29:57.026783 cognee-0.1.8/cognee/.data/example/tests/integrations/graphene/test_graphene_py3.txt
--rw-r--r--   0        0        0      177 2024-05-09 09:29:57.018972 cognee-0.1.8/cognee/.data/example/tests/integrations/grpc/__init__.txt
--rw-r--r--   0        0        0      403 2024-05-09 09:29:57.019314 cognee-0.1.8/cognee/.data/example/tests/integrations/grpc/compile_test_services.txt
--rw-r--r--   0        0        0     1608 2024-05-09 09:29:57.019197 cognee-0.1.8/cognee/.data/example/tests/integrations/grpc/grpc_test_service_pb2.txt
--rw-r--r--   0        0        0     7557 2024-05-09 09:29:57.019100 cognee-0.1.8/cognee/.data/example/tests/integrations/grpc/grpc_test_service_pb2_grpc.txt
--rw-r--r--   0        0        0      409 2024-05-09 09:29:57.019566 cognee-0.1.8/cognee/.data/example/tests/integrations/grpc/protos/grpc_test_service.txt
--rw-r--r--   0        0        0    10556 2024-05-09 09:29:57.018737 cognee-0.1.8/cognee/.data/example/tests/integrations/grpc/test_grpc.txt
--rw-r--r--   0        0        0     8185 2024-05-09 09:29:57.019428 cognee-0.1.8/cognee/.data/example/tests/integrations/grpc/test_grpc_aio.txt
--rw-r--r--   0        0        0       44 2024-05-09 09:29:57.026263 cognee-0.1.8/cognee/.data/example/tests/integrations/httpx/__init__.txt
--rw-r--r--   0        0        0     8965 2024-05-09 09:29:57.026483 cognee-0.1.8/cognee/.data/example/tests/integrations/httpx/test_httpx.txt
--rw-r--r--   0        0        0       43 2024-05-09 09:29:57.022292 cognee-0.1.8/cognee/.data/example/tests/integrations/huey/__init__.txt
--rw-r--r--   0        0        0     5071 2024-05-09 09:29:57.022163 cognee-0.1.8/cognee/.data/example/tests/integrations/huey/test_huey.txt
--rw-r--r--   0        0        0     6912 2024-05-09 09:29:57.034033 cognee-0.1.8/cognee/.data/example/tests/integrations/logging/test_logging.txt
--rw-r--r--   0        0        0       45 2024-05-09 09:29:57.027978 cognee-0.1.8/cognee/.data/example/tests/integrations/loguru/__init__.txt
--rw-r--r--   0        0        0     3266 2024-05-09 09:29:57.027868 cognee-0.1.8/cognee/.data/example/tests/integrations/loguru/test_loguru.txt
--rw-r--r--   0        0        0      367 2024-05-09 09:29:57.029424 cognee-0.1.8/cognee/.data/example/tests/integrations/modules/test_modules.txt
--rw-r--r--   0        0        0       45 2024-05-09 09:29:57.035193 cognee-0.1.8/cognee/.data/example/tests/integrations/openai/__init__.txt
--rw-r--r--   0        0        0     7535 2024-05-09 09:29:57.035087 cognee-0.1.8/cognee/.data/example/tests/integrations/openai/test_openai.txt
--rw-r--r--   0        0        0       52 2024-05-09 09:29:57.021548 cognee-0.1.8/cognee/.data/example/tests/integrations/opentelemetry/__init__.txt
--rw-r--r--   0        0        0      993 2024-05-09 09:29:57.021650 cognee-0.1.8/cognee/.data/example/tests/integrations/opentelemetry/test_experimental.txt
--rw-r--r--   0        0        0     7951 2024-05-09 09:29:57.021447 cognee-0.1.8/cognee/.data/example/tests/integrations/opentelemetry/test_propagator.txt
--rw-r--r--   0        0        0    21486 2024-05-09 09:29:57.021335 cognee-0.1.8/cognee/.data/example/tests/integrations/opentelemetry/test_span_processor.txt
--rw-r--r--   0        0        0       48 2024-05-09 09:29:57.018031 cognee-0.1.8/cognee/.data/example/tests/integrations/pure_eval/__init__.txt
--rw-r--r--   0        0        0     2445 2024-05-09 09:29:57.018140 cognee-0.1.8/cognee/.data/example/tests/integrations/pure_eval/test_pure_eval.txt
--rw-r--r--   0        0        0       46 2024-05-09 09:29:57.024908 cognee-0.1.8/cognee/.data/example/tests/integrations/pymongo/__init__.txt
--rw-r--r--   0        0        0    14425 2024-05-09 09:29:57.024783 cognee-0.1.8/cognee/.data/example/tests/integrations/pymongo/test_pymongo.txt
--rw-r--r--   0        0        0       46 2024-05-09 09:29:57.023114 cognee-0.1.8/cognee/.data/example/tests/integrations/pyramid/__init__.txt
--rw-r--r--   0        0        0    11072 2024-05-09 09:29:57.022983 cognee-0.1.8/cognee/.data/example/tests/integrations/pyramid/test_pyramid.txt
--rw-r--r--   0        0        0       44 2024-05-09 09:29:57.022440 cognee-0.1.8/cognee/.data/example/tests/integrations/quart/__init__.txt
--rw-r--r--   0        0        0    14540 2024-05-09 09:29:57.022568 cognee-0.1.8/cognee/.data/example/tests/integrations/quart/test_quart.txt
--rw-r--r--   0        0        0       44 2024-05-09 09:29:57.020398 cognee-0.1.8/cognee/.data/example/tests/integrations/redis/__init__.txt
--rw-r--r--   0        0        0       57 2024-05-09 09:29:57.021036 cognee-0.1.8/cognee/.data/example/tests/integrations/redis/asyncio/__init__.txt
--rw-r--r--   0        0        0     2423 2024-05-09 09:29:57.021170 cognee-0.1.8/cognee/.data/example/tests/integrations/redis/asyncio/test_redis_asyncio.txt
--rw-r--r--   0        0        0       52 2024-05-09 09:29:57.020530 cognee-0.1.8/cognee/.data/example/tests/integrations/redis/cluster/__init__.txt
--rw-r--r--   0        0        0     4441 2024-05-09 09:29:57.020647 cognee-0.1.8/cognee/.data/example/tests/integrations/redis/cluster/test_redis_cluster.txt
--rw-r--r--   0        0        0       60 2024-05-09 09:29:57.020778 cognee-0.1.8/cognee/.data/example/tests/integrations/redis/cluster_asyncio/__init__.txt
--rw-r--r--   0        0        0     4188 2024-05-09 09:29:57.020894 cognee-0.1.8/cognee/.data/example/tests/integrations/redis/cluster_asyncio/test_redis_cluster_asyncio.txt
--rw-r--r--   0        0        0     9022 2024-05-09 09:29:57.020291 cognee-0.1.8/cognee/.data/example/tests/integrations/redis/test_redis.txt
--rw-r--r--   0        0        0       51 2024-05-09 09:29:57.018400 cognee-0.1.8/cognee/.data/example/tests/integrations/rediscluster/__init__.txt
--rw-r--r--   0        0        0     5016 2024-05-09 09:29:57.018513 cognee-0.1.8/cognee/.data/example/tests/integrations/rediscluster/test_rediscluster.txt
--rw-r--r--   0        0        0       47 2024-05-09 09:29:57.025377 cognee-0.1.8/cognee/.data/example/tests/integrations/requests/__init__.txt
--rw-r--r--   0        0        0     2061 2024-05-09 09:29:57.025513 cognee-0.1.8/cognee/.data/example/tests/integrations/requests/test_requests.txt
--rw-r--r--   0        0        0       41 2024-05-09 09:29:57.034380 cognee-0.1.8/cognee/.data/example/tests/integrations/rq/__init__.txt
--rw-r--r--   0        0        0     8582 2024-05-09 09:29:57.034258 cognee-0.1.8/cognee/.data/example/tests/integrations/rq/test_rq.txt
--rw-r--r--   0        0        0       44 2024-05-09 09:29:57.027210 cognee-0.1.8/cognee/.data/example/tests/integrations/sanic/__init__.txt
--rw-r--r--   0        0        0    13506 2024-05-09 09:29:57.027348 cognee-0.1.8/cognee/.data/example/tests/integrations/sanic/test_sanic.txt
--rw-r--r--   0        0        0     1042 2024-05-09 09:29:57.022011 cognee-0.1.8/cognee/.data/example/tests/integrations/serverless/test_serverless.txt
--rw-r--r--   0        0        0       45 2024-05-09 09:29:57.035431 cognee-0.1.8/cognee/.data/example/tests/integrations/socket/__init__.txt
--rw-r--r--   0        0        0     1641 2024-05-09 09:29:57.035327 cognee-0.1.8/cognee/.data/example/tests/integrations/socket/test_socket.txt
--rw-r--r--   0        0        0       74 2024-05-09 09:29:57.034953 cognee-0.1.8/cognee/.data/example/tests/integrations/spark/__init__.txt
--rw-r--r--   0        0        0     6598 2024-05-09 09:29:57.034849 cognee-0.1.8/cognee/.data/example/tests/integrations/spark/test_spark.txt
--rw-r--r--   0        0        0      292 2024-05-09 09:29:57.024338 cognee-0.1.8/cognee/.data/example/tests/integrations/sqlalchemy/__init__.txt
--rw-r--r--   0        0        0        0 2024-05-09 09:29:57.024459 cognee-0.1.8/cognee/.data/example/tests/integrations/sqlalchemy/sqlalchemy_helpers/__init__.txt
--rw-r--r--   0        0        0      192 2024-05-09 09:29:57.024603 cognee-0.1.8/cognee/.data/example/tests/integrations/sqlalchemy/sqlalchemy_helpers/helpers.txt
--rw-r--r--   0        0        0    21401 2024-05-09 09:29:57.024205 cognee-0.1.8/cognee/.data/example/tests/integrations/sqlalchemy/test_sqlalchemy.txt
--rw-r--r--   0        0        0       48 2024-05-09 09:29:57.023271 cognee-0.1.8/cognee/.data/example/tests/integrations/starlette/__init__.txt
--rw-r--r--   0        0        0    21014 2024-05-09 09:29:57.023405 cognee-0.1.8/cognee/.data/example/tests/integrations/starlette/photo.txt
--rw-r--r--   0        0        0       24 2024-05-09 09:29:57.023706 cognee-0.1.8/cognee/.data/example/tests/integrations/starlette/templates/trace_meta.txt
--rw-r--r--   0        0        0    35093 2024-05-09 09:29:57.023542 cognee-0.1.8/cognee/.data/example/tests/integrations/starlette/test_starlette.txt
--rw-r--r--   0        0        0       47 2024-05-09 09:29:57.028320 cognee-0.1.8/cognee/.data/example/tests/integrations/starlite/__init__.txt
--rw-r--r--   0        0        0     9647 2024-05-09 09:29:57.028209 cognee-0.1.8/cognee/.data/example/tests/integrations/starlite/test_starlite.txt
--rw-r--r--   0        0        0    10655 2024-05-09 09:29:57.027727 cognee-0.1.8/cognee/.data/example/tests/integrations/stdlib/test_httplib.txt
--rw-r--r--   0        0        0     5045 2024-05-09 09:29:57.027509 cognee-0.1.8/cognee/.data/example/tests/integrations/stdlib/test_subprocess.txt
--rw-r--r--   0        0        0        0 2024-05-09 09:29:57.017516 cognee-0.1.8/cognee/.data/example/tests/integrations/strawberry/__init__.txt
--rw-r--r--   0        0        0    19273 2024-05-09 09:29:57.017631 cognee-0.1.8/cognee/.data/example/tests/integrations/strawberry/test_strawberry_py3.txt
--rw-r--r--   0        0        0    10881 2024-05-09 09:29:57.016250 cognee-0.1.8/cognee/.data/example/tests/integrations/test_gnu_backtrace.txt
--rw-r--r--   0        0        0     5769 2024-05-09 09:29:57.029284 cognee-0.1.8/cognee/.data/example/tests/integrations/threading/test_threading.txt
--rw-r--r--   0        0        0       46 2024-05-09 09:29:57.025691 cognee-0.1.8/cognee/.data/example/tests/integrations/tornado/__init__.txt
--rw-r--r--   0        0        0    13348 2024-05-09 09:29:57.025828 cognee-0.1.8/cognee/.data/example/tests/integrations/tornado/test_tornado.txt
--rw-r--r--   0        0        0       46 2024-05-09 09:29:57.025073 cognee-0.1.8/cognee/.data/example/tests/integrations/trytond/__init__.txt
--rw-r--r--   0        0        0     3584 2024-05-09 09:29:57.025212 cognee-0.1.8/cognee/.data/example/tests/integrations/trytond/test_trytond.txt
--rw-r--r--   0        0        0    13237 2024-05-09 09:29:57.023890 cognee-0.1.8/cognee/.data/example/tests/integrations/wsgi/test_wsgi.txt
--rw-r--r--   0        0        0     3681 2024-05-09 09:29:57.013923 cognee-0.1.8/cognee/.data/example/tests/test_api.txt
--rw-r--r--   0        0        0    23643 2024-05-09 09:29:57.012396 cognee-0.1.8/cognee/.data/example/tests/test_basics.txt
--rw-r--r--   0        0        0    41119 2024-05-09 09:29:57.014041 cognee-0.1.8/cognee/.data/example/tests/test_client.txt
--rw-r--r--   0        0        0     3417 2024-05-09 09:29:57.012616 cognee-0.1.8/cognee/.data/example/tests/test_conftest.txt
--rw-r--r--   0        0        0     8137 2024-05-09 09:29:57.013721 cognee-0.1.8/cognee/.data/example/tests/test_envelope.txt
--rw-r--r--   0        0        0     8578 2024-05-09 09:29:57.013472 cognee-0.1.8/cognee/.data/example/tests/test_exceptiongroup.txt
--rw-r--r--   0        0        0      784 2024-05-09 09:29:57.013826 cognee-0.1.8/cognee/.data/example/tests/test_lru_cache.txt
--rw-r--r--   0        0        0    31466 2024-05-09 09:29:57.012506 cognee-0.1.8/cognee/.data/example/tests/test_metrics.txt
--rw-r--r--   0        0        0     2702 2024-05-09 09:29:57.011977 cognee-0.1.8/cognee/.data/example/tests/test_monitor.txt
--rw-r--r--   0        0        0    24427 2024-05-09 09:29:57.013272 cognee-0.1.8/cognee/.data/example/tests/test_profiler.txt
--rw-r--r--   0        0        0     4058 2024-05-09 09:29:57.012951 cognee-0.1.8/cognee/.data/example/tests/test_scope.txt
--rw-r--r--   0        0        0     5357 2024-05-09 09:29:57.012302 cognee-0.1.8/cognee/.data/example/tests/test_scrubber.txt
--rw-r--r--   0        0        0     4816 2024-05-09 09:29:57.012842 cognee-0.1.8/cognee/.data/example/tests/test_serializer.txt
--rw-r--r--   0        0        0     4184 2024-05-09 09:29:57.012737 cognee-0.1.8/cognee/.data/example/tests/test_sessions.txt
--rw-r--r--   0        0        0     1490 2024-05-09 09:29:57.013600 cognee-0.1.8/cognee/.data/example/tests/test_spotlight.txt
--rw-r--r--   0        0        0    18416 2024-05-09 09:29:57.013163 cognee-0.1.8/cognee/.data/example/tests/test_transport.txt
--rw-r--r--   0        0        0      760 2024-05-09 09:29:57.014146 cognee-0.1.8/cognee/.data/example/tests/test_types.txt
--rw-r--r--   0        0        0    22888 2024-05-09 09:29:57.012082 cognee-0.1.8/cognee/.data/example/tests/test_utils.txt
--rw-r--r--   0        0        0     2699 2024-05-09 09:29:57.015252 cognee-0.1.8/cognee/.data/example/tests/tracing/test_baggage.txt
--rw-r--r--   0        0        0     1820 2024-05-09 09:29:57.014647 cognee-0.1.8/cognee/.data/example/tests/tracing/test_decorator_async_py3.txt
--rw-r--r--   0        0        0     1665 2024-05-09 09:29:57.015353 cognee-0.1.8/cognee/.data/example/tests/tracing/test_decorator_sync.txt
--rw-r--r--   0        0        0      575 2024-05-09 09:29:57.014757 cognee-0.1.8/cognee/.data/example/tests/tracing/test_deprecated.txt
--rw-r--r--   0        0        0     1813 2024-05-09 09:29:57.014855 cognee-0.1.8/cognee/.data/example/tests/tracing/test_http_headers.txt
--rw-r--r--   0        0        0     9610 2024-05-09 09:29:57.014389 cognee-0.1.8/cognee/.data/example/tests/tracing/test_integration_tests.txt
--rw-r--r--   0        0        0    12757 2024-05-09 09:29:57.014533 cognee-0.1.8/cognee/.data/example/tests/tracing/test_misc.txt
--rw-r--r--   0        0        0     1792 2024-05-09 09:29:57.014957 cognee-0.1.8/cognee/.data/example/tests/tracing/test_noop_span.txt
--rw-r--r--   0        0        0    10643 2024-05-09 09:29:57.015148 cognee-0.1.8/cognee/.data/example/tests/tracing/test_sampling.txt
--rw-r--r--   0        0        0       40 2024-05-09 09:29:57.015690 cognee-0.1.8/cognee/.data/example/tests/utils/__init__.txt
--rw-r--r--   0        0        0      797 2024-05-09 09:29:57.015572 cognee-0.1.8/cognee/.data/example/tests/utils/test_contextvars.txt
--rw-r--r--   0        0        0    17196 2024-05-09 09:29:57.015804 cognee-0.1.8/cognee/.data/example/tests/utils/test_general.txt
--rw-r--r--   0        0        0     1539 2024-05-09 09:29:57.015472 cognee-0.1.8/cognee/.data/example/tests/utils/test_transaction.txt
--rw-r--r--   0        0        0    20053 2024-05-09 09:29:57.011668 cognee-0.1.8/cognee/.data/example/tox.txt
--rw-r--r--   0        0        0      123 2024-04-23 06:52:58.178501 cognee-0.1.8/cognee/.data/example_dataset/271fd0a1a088575885fddc726c4dba04.txt
--rw-r--r--   0        0        0      426 2024-05-21 06:59:15.075082 cognee-0.1.8/cognee/.data/example_dataset/8e944490a15f563780e6c3f040880b19.txt
--rw-r--r--   0        0        0     3087 2024-04-02 07:24:38.404088 cognee-0.1.8/cognee/.data/explanations/062c22df-d99b-599f-90cd-2d325c8bcf69.txt
--rw-r--r--   0        0        0     9041 2024-04-23 07:36:22.827937 cognee-0.1.8/cognee/.data/explanations/6dfe01b6-07d2-5b77-83c8-1d6c11ce2aa7.txt
--rw-r--r--   0        0        0      985 2024-03-30 19:01:36.385908 cognee-0.1.8/cognee/.data/explanations/Natural language processing.txt
--rw-r--r--   0        0        0       51 2024-04-18 08:17:53.704561 cognee-0.1.8/cognee/.data/explanations/bab90046-1d9b-598c-8711-dab30f501915.txt
--rw-r--r--   0        0        0       36 2024-05-21 09:16:37.925545 cognee-0.1.8/cognee/.data/initial_test/14a27354cb3f50ffaaace292d5b7aa58.txt
--rw-r--r--   0        0        0       44 2024-05-21 09:16:37.923975 cognee-0.1.8/cognee/.data/initial_test/15a66b1d75a45fbfa2d5f8d7b2506d88.txt
--rw-r--r--   0        0        0       58 2024-05-21 09:16:37.924807 cognee-0.1.8/cognee/.data/initial_test/a881954da33b5e3c8bcf1bc63e50ae20.txt
--rw-r--r--   0        0        0      186 2024-04-29 18:24:10.776372 cognee-0.1.8/cognee/.data/test/e6ac18788c6a51dfaaf9b963d5bc094b.txt
--rw-r--r--   0        0        0      249 2024-04-23 05:20:06.890311 cognee-0.1.8/cognee/__init__.py
--rw-r--r--   0        0        0        0 2024-03-14 09:23:35.230717 cognee-0.1.8/cognee/api/__init__.py
--rw-r--r--   0        0        0     8753 2024-05-27 05:37:00.861835 cognee-0.1.8/cognee/api/client.py
--rw-r--r--   0        0        0        0 2024-03-14 09:23:35.230960 cognee-0.1.8/cognee/api/v1/__init__.py
--rw-r--r--   0        0        0       21 2024-03-14 09:23:35.231099 cognee-0.1.8/cognee/api/v1/add/__init__.py
--rw-r--r--   0        0        0     5216 2024-05-26 19:03:19.264649 cognee-0.1.8/cognee/api/v1/add/add.py
--rw-r--r--   0        0        0     1629 2024-05-26 19:03:19.265636 cognee-0.1.8/cognee/api/v1/add/add_standalone.py
--rw-r--r--   0        0        0      626 2024-03-29 12:59:22.978997 cognee-0.1.8/cognee/api/v1/add/remember.py
--rw-r--r--   0        0        0        0 2024-04-26 13:52:41.234848 cognee-0.1.8/cognee/api/v1/cognify/__init__.py
--rw-r--r--   0        0        0    12092 2024-05-27 05:37:00.862456 cognee-0.1.8/cognee/api/v1/cognify/cognify.py
--rw-r--r--   0        0        0     6884 2024-04-25 08:56:45.148041 cognee-0.1.8/cognee/api/v1/cognify/tst.py
--rw-r--r--   0        0        0       27 2024-03-29 12:59:22.979399 cognee-0.1.8/cognee/api/v1/config/__init__.py
--rw-r--r--   0        0        0     2552 2024-05-27 05:37:00.864513 cognee-0.1.8/cognee/api/v1/config/config.py
--rw-r--r--   0        0        0        0 2024-04-26 13:52:41.235161 cognee-0.1.8/cognee/api/v1/datasets/__init__.py
--rw-r--r--   0        0        0     1184 2024-05-27 05:37:00.864752 cognee-0.1.8/cognee/api/v1/datasets/datasets.py
--rw-r--r--   0        0        0       25 2024-04-23 05:20:06.891056 cognee-0.1.8/cognee/api/v1/prune/__init__.py
--rw-r--r--   0        0        0     1236 2024-05-26 19:03:19.266837 cognee-0.1.8/cognee/api/v1/prune/prune.py
--rw-r--r--   0        0        0       39 2024-03-21 16:01:22.628858 cognee-0.1.8/cognee/api/v1/search/__init__.py
--rw-r--r--   0        0        0     3973 2024-05-26 19:03:19.267387 cognee-0.1.8/cognee/api/v1/search/search.py
--rw-r--r--   0        0        0        0 2024-05-25 06:16:34.118332 cognee-0.1.8/cognee/api/v1/topology/__init__.py
--rw-r--r--   0        0        0     3845 2024-05-26 19:03:19.267657 cognee-0.1.8/cognee/api/v1/topology/add_topology.py
--rw-r--r--   0        0        0     2836 2024-05-19 13:52:43.158383 cognee-0.1.8/cognee/api/v1/topology/rrrr.py
--rw-r--r--   0        0        0      781 2024-05-27 05:37:00.865047 cognee-0.1.8/cognee/base_config.py
--rw-r--r--   0        0        0     5730 2024-05-26 19:03:19.268694 cognee-0.1.8/cognee/config.py
--rw-r--r--   0        0        0     1778 2024-04-28 19:24:05.618264 cognee-0.1.8/cognee/fetch_secret.py
--rw-r--r--   0        0        0     7145 2024-05-27 05:37:00.865343 cognee-0.1.8/cognee/infrastructure/InfrastructureConfig.py
--rw-r--r--   0        0        0       56 2024-03-14 09:23:35.235336 cognee-0.1.8/cognee/infrastructure/__init__.py
--rw-r--r--   0        0        0      110 2024-03-29 12:59:22.980107 cognee-0.1.8/cognee/infrastructure/data/__init__.py
--rw-r--r--   0        0        0     4457 2024-05-25 06:16:34.119439 cognee-0.1.8/cognee/infrastructure/data/chunking/DefaultChunkEngine.py
--rw-r--r--   0        0        0        0 2024-05-25 06:16:34.119461 cognee-0.1.8/cognee/infrastructure/data/chunking/HaystackChunkEngine.py
--rw-r--r--   0        0        0     1661 2024-05-25 06:16:34.119789 cognee-0.1.8/cognee/infrastructure/data/chunking/LangchainChunkingEngine.py
--rw-r--r--   0        0        0        0 2024-04-26 13:52:41.236173 cognee-0.1.8/cognee/infrastructure/data/chunking/__init__.py
--rw-r--r--   0        0        0      763 2024-05-26 19:03:19.270005 cognee-0.1.8/cognee/infrastructure/data/chunking/config.py
--rw-r--r--   0        0        0      889 2024-03-14 09:23:35.235567 cognee-0.1.8/cognee/infrastructure/data/models/Data.py
--rw-r--r--   0        0        0      721 2024-03-14 09:23:35.235631 cognee-0.1.8/cognee/infrastructure/data/models/Dataset.py
--rw-r--r--   0        0        0      553 2024-03-14 09:23:35.235756 cognee-0.1.8/cognee/infrastructure/data/models/DatasetData.py
--rw-r--r--   0        0        0        0 2024-03-14 09:23:35.235800 cognee-0.1.8/cognee/infrastructure/data/models/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 13:52:41.236240 cognee-0.1.8/cognee/infrastructure/data/utils/__init__.py
--rw-r--r--   0        0        0      756 2024-04-23 05:20:06.895346 cognee-0.1.8/cognee/infrastructure/data/utils/extract_keywords.py
--rw-r--r--   0        0        0        0 2024-03-14 09:23:35.235884 cognee-0.1.8/cognee/infrastructure/databases/__init__.py
--rw-r--r--   0        0        0        0 2024-03-14 09:23:35.235957 cognee-0.1.8/cognee/infrastructure/databases/graph/__init__.py
--rw-r--r--   0        0        0     1640 2024-05-26 19:03:19.270423 cognee-0.1.8/cognee/infrastructure/databases/graph/config.py
--rw-r--r--   0        0        0        0 2024-05-25 06:16:34.119846 cognee-0.1.8/cognee/infrastructure/databases/graph/falkordb/__init__.py
--rw-r--r--   0        0        0     6177 2024-05-25 06:16:34.120113 cognee-0.1.8/cognee/infrastructure/databases/graph/falkordb/adapter.py
--rw-r--r--   0        0        0     1553 2024-05-26 19:03:19.271191 cognee-0.1.8/cognee/infrastructure/databases/graph/get_graph_client.py
--rw-r--r--   0        0        0     1162 2024-04-23 05:20:06.895582 cognee-0.1.8/cognee/infrastructure/databases/graph/graph_db_interface.py
--rw-r--r--   0        0        0        0 2024-04-23 05:20:06.895611 cognee-0.1.8/cognee/infrastructure/databases/graph/neo4j_driver/__init__.py
--rw-r--r--   0        0        0     6154 2024-05-26 19:03:19.271548 cognee-0.1.8/cognee/infrastructure/databases/graph/neo4j_driver/adapter.py
--rw-r--r--   0        0        0        0 2024-03-14 09:23:35.236389 cognee-0.1.8/cognee/infrastructure/databases/graph/networkx/__init__.py
--rw-r--r--   0        0        0     5360 2024-05-25 06:16:34.120573 cognee-0.1.8/cognee/infrastructure/databases/graph/networkx/adapter.py
--rw-r--r--   0        0        0      462 2024-03-14 09:23:35.236879 cognee-0.1.8/cognee/infrastructure/databases/relational/DatabaseEngine.py
--rw-r--r--   0        0        0       76 2024-03-14 09:23:35.236991 cognee-0.1.8/cognee/infrastructure/databases/relational/ModelBase.py
--rw-r--r--   0        0        0      170 2024-03-14 09:23:35.237089 cognee-0.1.8/cognee/infrastructure/databases/relational/__init__.py
--rw-r--r--   0        0        0     1353 2024-05-27 05:37:00.865581 cognee-0.1.8/cognee/infrastructure/databases/relational/config.py
--rw-r--r--   0        0        0     6666 2024-05-27 05:37:00.866108 cognee-0.1.8/cognee/infrastructure/databases/relational/duckdb/DuckDBAdapter.py
--rw-r--r--   0        0        0        0 2024-04-26 13:52:41.237764 cognee-0.1.8/cognee/infrastructure/databases/relational/duckdb/__init__.py
--rw-r--r--   0        0        0     1006 2024-03-14 09:23:35.237616 cognee-0.1.8/cognee/infrastructure/databases/relational/relational_db_interface.py
--rw-r--r--   0        0        0     2847 2024-03-14 09:23:35.237690 cognee-0.1.8/cognee/infrastructure/databases/relational/sqlite/SqliteEngine.py
--rw-r--r--   0        0        0        0 2024-03-14 09:23:35.237716 cognee-0.1.8/cognee/infrastructure/databases/relational/sqlite/__init__.py
--rw-r--r--   0        0        0       41 2024-03-14 09:23:35.237829 cognee-0.1.8/cognee/infrastructure/databases/relational/utils/__init__.py
--rw-r--r--   0        0        0      595 2024-03-14 09:23:35.237896 cognee-0.1.8/cognee/infrastructure/databases/relational/utils/with_rollback.py
--rw-r--r--   0        0        0      230 2024-05-27 05:37:00.866399 cognee-0.1.8/cognee/infrastructure/databases/vector/__init__.py
--rw-r--r--   0        0        0     1549 2024-05-27 05:37:00.866518 cognee-0.1.8/cognee/infrastructure/databases/vector/config.py
--rw-r--r--   0        0        0     1368 2024-05-27 05:37:00.866669 cognee-0.1.8/cognee/infrastructure/databases/vector/create_vector_engine.py
--rw-r--r--   0        0        0     2381 2024-05-26 19:03:19.273200 cognee-0.1.8/cognee/infrastructure/databases/vector/embeddings/DefaultEmbeddingEngine.py
--rw-r--r--   0        0        0      243 2024-05-25 06:16:34.121382 cognee-0.1.8/cognee/infrastructure/databases/vector/embeddings/EmbeddingEngine.py
--rw-r--r--   0        0        0        0 2024-04-26 13:52:41.237831 cognee-0.1.8/cognee/infrastructure/databases/vector/embeddings/__init__.py
--rw-r--r--   0        0        0     1091 2024-05-26 19:03:19.273824 cognee-0.1.8/cognee/infrastructure/databases/vector/embeddings/config.py
--rw-r--r--   0        0        0     1474 2024-05-26 19:03:19.274145 cognee-0.1.8/cognee/infrastructure/databases/vector/falkordb/FalkorDBAdapter.py
--rw-r--r--   0        0        0     5331 2024-05-25 06:16:34.121496 cognee-0.1.8/cognee/infrastructure/databases/vector/lancedb/LanceDBAdapter.py
--rw-r--r--   0        0        0        0 2024-05-25 06:16:34.121519 cognee-0.1.8/cognee/infrastructure/databases/vector/lancedb/__init__.py
--rw-r--r--   0        0        0      138 2024-03-21 16:01:22.631437 cognee-0.1.8/cognee/infrastructure/databases/vector/models/CollectionConfig.py
--rw-r--r--   0        0        0      398 2024-05-25 06:16:34.121821 cognee-0.1.8/cognee/infrastructure/databases/vector/models/DataPoint.py
--rw-r--r--   0        0        0       69 2024-05-25 06:16:34.122276 cognee-0.1.8/cognee/infrastructure/databases/vector/models/PayloadSchema.py
--rw-r--r--   0        0        0      171 2024-03-21 16:01:22.632343 cognee-0.1.8/cognee/infrastructure/databases/vector/models/ScoredResult.py
--rw-r--r--   0        0        0      143 2024-03-21 16:01:22.633028 cognee-0.1.8/cognee/infrastructure/databases/vector/models/VectorConfig.py
--rw-r--r--   0        0        0        0 2024-04-26 13:52:41.238226 cognee-0.1.8/cognee/infrastructure/databases/vector/models/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 13:52:41.238287 cognee-0.1.8/cognee/infrastructure/databases/vector/pinecone/__init__.py
--rw-r--r--   0        0        0      256 2024-03-14 09:23:35.238527 cognee-0.1.8/cognee/infrastructure/databases/vector/pinecone/adapter.py
--rw-r--r--   0        0        0     6652 2024-05-25 06:16:34.122417 cognee-0.1.8/cognee/infrastructure/databases/vector/qdrant/QDrantAdapter.py
--rw-r--r--   0        0        0       96 2024-04-23 05:20:06.897060 cognee-0.1.8/cognee/infrastructure/databases/vector/qdrant/__init__.py
--rw-r--r--   0        0        0     1362 2024-05-25 06:16:34.122602 cognee-0.1.8/cognee/infrastructure/databases/vector/vector_db_interface.py
--rw-r--r--   0        0        0     4548 2024-05-25 06:16:34.122724 cognee-0.1.8/cognee/infrastructure/databases/vector/weaviate_db/WeaviateAdapter.py
--rw-r--r--   0        0        0       45 2024-03-21 16:01:22.635439 cognee-0.1.8/cognee/infrastructure/databases/vector/weaviate_db/__init__.py
--rw-r--r--   0        0        0      185 2024-03-14 09:23:35.239234 cognee-0.1.8/cognee/infrastructure/files/__init__.py
--rw-r--r--   0        0        0      364 2024-03-14 09:23:35.239315 cognee-0.1.8/cognee/infrastructure/files/add_file_to_storage.py
--rw-r--r--   0        0        0      320 2024-03-14 09:23:35.239384 cognee-0.1.8/cognee/infrastructure/files/remove_file_from_storage.py
--rw-r--r--   0        0        0     1549 2024-05-25 06:16:34.122827 cognee-0.1.8/cognee/infrastructure/files/storage/LocalStorage.py
--rw-r--r--   0        0        0      640 2024-03-14 09:23:35.239533 cognee-0.1.8/cognee/infrastructure/files/storage/StorageManager.py
--rw-r--r--   0        0        0       39 2024-03-14 09:23:35.239601 cognee-0.1.8/cognee/infrastructure/files/storage/__init__.py
--rw-r--r--   0        0        0        0 2024-03-14 09:23:35.239635 cognee-0.1.8/cognee/infrastructure/files/utils/__init__.py
--rw-r--r--   0        0        0      427 2024-05-26 19:03:19.274436 cognee-0.1.8/cognee/infrastructure/files/utils/extract_text_from_file.py
--rw-r--r--   0        0        0     1001 2024-05-26 19:03:19.274786 cognee-0.1.8/cognee/infrastructure/files/utils/get_file_metadata.py
--rw-r--r--   0        0        0      117 2024-05-26 19:03:19.275134 cognee-0.1.8/cognee/infrastructure/files/utils/get_file_size.py
--rw-r--r--   0        0        0     1144 2024-05-26 19:03:19.286545 cognee-0.1.8/cognee/infrastructure/files/utils/guess_file_type.py
--rw-r--r--   0        0        0      865 2024-05-26 19:03:19.286780 cognee-0.1.8/cognee/infrastructure/files/utils/is_text_content.py
--rw-r--r--   0        0        0       35 2024-05-26 19:03:19.287399 cognee-0.1.8/cognee/infrastructure/llm/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 12:59:22.982620 cognee-0.1.8/cognee/infrastructure/llm/anthropic/__init__.py
--rw-r--r--   0        0        0     1807 2024-05-25 06:16:34.123242 cognee-0.1.8/cognee/infrastructure/llm/anthropic/adapter.py
--rw-r--r--   0        0        0      597 2024-05-26 19:03:19.287741 cognee-0.1.8/cognee/infrastructure/llm/config.py
--rw-r--r--   0        0        0        0 2024-04-26 13:52:41.238931 cognee-0.1.8/cognee/infrastructure/llm/generic_llm_api/__init__.py
--rw-r--r--   0        0        0     5423 2024-05-26 19:03:19.288073 cognee-0.1.8/cognee/infrastructure/llm/generic_llm_api/adapter.py
--rw-r--r--   0        0        0     1296 2024-05-27 05:37:00.866830 cognee-0.1.8/cognee/infrastructure/llm/get_llm_client.py
--rw-r--r--   0        0        0      738 2024-05-26 19:03:19.289342 cognee-0.1.8/cognee/infrastructure/llm/llm_interface.py
--rw-r--r--   0        0        0        0 2024-03-14 09:23:35.240172 cognee-0.1.8/cognee/infrastructure/llm/openai/__init__.py
--rw-r--r--   0        0        0     5562 2024-05-26 19:03:19.289967 cognee-0.1.8/cognee/infrastructure/llm/openai/adapter.py
--rw-r--r--   0        0        0       90 2024-03-21 16:01:22.637734 cognee-0.1.8/cognee/infrastructure/llm/prompts/__init__.py
--rw-r--r--   0        0        0      112 2024-05-25 06:16:34.123926 cognee-0.1.8/cognee/infrastructure/llm/prompts/categorize_categories.txt
--rw-r--r--   0        0        0      110 2024-05-25 06:16:34.124196 cognee-0.1.8/cognee/infrastructure/llm/prompts/categorize_summary.txt
--rw-r--r--   0        0        0     5614 2024-03-29 12:59:14.138687 cognee-0.1.8/cognee/infrastructure/llm/prompts/classify_content.txt
--rw-r--r--   0        0        0      348 2024-05-25 06:16:34.124497 cognee-0.1.8/cognee/infrastructure/llm/prompts/extract_topology.txt
--rw-r--r--   0        0        0     1323 2024-04-23 05:20:06.898436 cognee-0.1.8/cognee/infrastructure/llm/prompts/generate_cog_layers.txt
--rw-r--r--   0        0        0     2192 2024-04-23 05:20:06.898603 cognee-0.1.8/cognee/infrastructure/llm/prompts/generate_graph_prompt.txt
--rw-r--r--   0        0        0      613 2024-03-21 16:01:22.638556 cognee-0.1.8/cognee/infrastructure/llm/prompts/read_query_prompt.py
--rw-r--r--   0        0        0      962 2024-03-21 16:01:22.638746 cognee-0.1.8/cognee/infrastructure/llm/prompts/render_prompt.py
--rw-r--r--   0        0        0       86 2024-03-21 16:01:22.639254 cognee-0.1.8/cognee/infrastructure/llm/prompts/summarize_content.txt
--rw-r--r--   0        0        0      889 2024-03-14 09:23:35.240981 cognee-0.1.8/cognee/infrastructure/pipeline/models/Operation.py
--rw-r--r--   0        0        0        0 2024-04-26 13:52:41.239072 cognee-0.1.8/cognee/infrastructure/pipeline/models/__init__.py
--rw-r--r--   0        0        0        0 2024-03-14 09:23:35.241109 cognee-0.1.8/cognee/modules/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 05:20:06.898696 cognee-0.1.8/cognee/modules/cognify/__init__.py
--rw-r--r--   0        0        0     1531 2024-05-26 19:03:19.290477 cognee-0.1.8/cognee/modules/cognify/config.py
--rw-r--r--   0        0        0     3298 2024-04-23 05:20:06.898825 cognee-0.1.8/cognee/modules/cognify/dataset.py
--rw-r--r--   0        0        0     2618 2024-05-25 06:16:34.124690 cognee-0.1.8/cognee/modules/cognify/evaluate.py
--rw-r--r--   0        0        0        1 2024-03-14 09:23:35.241331 cognee-0.1.8/cognee/modules/cognify/graph/__init__.py
--rw-r--r--   0        0        0     1136 2024-05-25 06:16:34.124946 cognee-0.1.8/cognee/modules/cognify/graph/add_classification_nodes.py
--rw-r--r--   0        0        0     5209 2024-05-27 05:37:00.867184 cognee-0.1.8/cognee/modules/cognify/graph/add_cognitive_layer_graphs.py
--rw-r--r--   0        0        0     1140 2024-05-25 06:16:34.125521 cognee-0.1.8/cognee/modules/cognify/graph/add_cognitive_layers.py
--rw-r--r--   0        0        0     2798 2024-05-27 05:37:00.867424 cognee-0.1.8/cognee/modules/cognify/graph/add_data_chunks.py
--rw-r--r--   0        0        0     1057 2024-05-25 06:16:34.125767 cognee-0.1.8/cognee/modules/cognify/graph/add_document_node.py
--rw-r--r--   0        0        0     2303 2024-05-26 19:03:19.292218 cognee-0.1.8/cognee/modules/cognify/graph/add_label_nodes.py
--rw-r--r--   0        0        0     7146 2024-05-26 19:03:19.293222 cognee-0.1.8/cognee/modules/cognify/graph/add_node_connections.py
--rw-r--r--   0        0        0      879 2024-05-25 06:16:34.126234 cognee-0.1.8/cognee/modules/cognify/graph/add_summary_nodes.py
--rw-r--r--   0        0        0    13112 2024-05-26 19:03:19.296197 cognee-0.1.8/cognee/modules/cognify/graph/create.py
--rw-r--r--   0        0        0        0 2024-03-14 09:23:35.242124 cognee-0.1.8/cognee/modules/cognify/llm/__init__.py
--rw-r--r--   0        0        0     1364 2024-05-27 05:37:00.867528 cognee-0.1.8/cognee/modules/cognify/llm/resolve_cross_graph_references.py
--rw-r--r--   0        0        0     7185 2024-05-25 06:16:34.128123 cognee-0.1.8/cognee/modules/cognify/test.py
--rw-r--r--   0        0        0     2667 2024-05-25 06:16:34.128231 cognee-0.1.8/cognee/modules/cognify/train.py
--rw-r--r--   0        0        0        0 2024-04-26 13:52:41.239641 cognee-0.1.8/cognee/modules/data/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 13:52:41.239714 cognee-0.1.8/cognee/modules/data/extraction/__init__.py
--rw-r--r--   0        0        0      960 2024-04-23 05:20:06.900831 cognee-0.1.8/cognee/modules/data/extraction/extract_categories.py
--rw-r--r--   0        0        0      490 2024-04-23 05:20:06.900898 cognee-0.1.8/cognee/modules/data/extraction/extract_cognitive_layers.py
--rw-r--r--   0        0        0      497 2024-04-23 05:20:06.900968 cognee-0.1.8/cognee/modules/data/extraction/extract_summary.py
--rw-r--r--   0        0        0        0 2024-04-26 13:52:41.239777 cognee-0.1.8/cognee/modules/data/extraction/knowledge_graph/__init__.py
--rw-r--r--   0        0        0      542 2024-04-23 05:20:06.901111 cognee-0.1.8/cognee/modules/data/extraction/knowledge_graph/extract_content_graph.py
--rw-r--r--   0        0        0     1041 2024-05-25 06:16:34.128718 cognee-0.1.8/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph.py
--rw-r--r--   0        0        0     4715 2024-05-25 06:16:34.128835 cognee-0.1.8/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph_module.py
--rw-r--r--   0        0        0      699 2024-05-26 19:03:19.297517 cognee-0.1.8/cognee/modules/data/get_cognitive_layers.py
--rw-r--r--   0        0        0      520 2024-05-26 19:03:19.298211 cognee-0.1.8/cognee/modules/data/get_content_categories.py
--rw-r--r--   0        0        0      559 2024-05-26 19:03:19.298864 cognee-0.1.8/cognee/modules/data/get_content_summary.py
--rw-r--r--   0        0        0     1009 2024-05-26 19:03:19.300631 cognee-0.1.8/cognee/modules/data/get_layer_graphs.py
--rw-r--r--   0        0        0       69 2024-04-23 05:20:06.901709 cognee-0.1.8/cognee/modules/discovery/__init__.py
--rw-r--r--   0        0        0      756 2024-04-23 05:20:06.901775 cognee-0.1.8/cognee/modules/discovery/discover_directory_datasets.py
--rw-r--r--   0        0        0       62 2024-03-29 12:59:22.987121 cognee-0.1.8/cognee/modules/ingestion/__init__.py
--rw-r--r--   0        0        0     1853 2024-05-26 19:03:19.301006 cognee-0.1.8/cognee/modules/ingestion/add_data_to_dataset.py
--rw-r--r--   0        0        0      549 2024-05-25 06:16:34.128937 cognee-0.1.8/cognee/modules/ingestion/classify.py
--rw-r--r--   0        0        0      941 2024-05-25 06:16:34.129049 cognee-0.1.8/cognee/modules/ingestion/data_types/BinaryData.py
--rw-r--r--   0        0        0      309 2024-05-26 19:03:19.301455 cognee-0.1.8/cognee/modules/ingestion/data_types/IngestionData.py
--rw-r--r--   0        0        0      764 2024-04-23 05:20:06.902759 cognee-0.1.8/cognee/modules/ingestion/data_types/TextData.py
--rw-r--r--   0        0        0      145 2024-03-14 09:23:35.243502 cognee-0.1.8/cognee/modules/ingestion/data_types/__init__.py
--rw-r--r--   0        0        0      125 2024-03-14 09:23:35.243619 cognee-0.1.8/cognee/modules/ingestion/exceptions.py
--rw-r--r--   0        0        0      275 2024-04-23 05:20:06.902967 cognee-0.1.8/cognee/modules/ingestion/identify.py
--rw-r--r--   0        0        0      796 2024-03-29 12:59:22.988225 cognee-0.1.8/cognee/modules/ingestion/save.py
--rw-r--r--   0        0        0     1109 2024-04-23 05:20:06.903064 cognee-0.1.8/cognee/modules/search/CogneeSearch.py
--rw-r--r--   0        0        0        0 2024-03-14 09:23:35.244581 cognee-0.1.8/cognee/modules/search/__init__.py
--rw-r--r--   0        0        0        0 2024-03-14 09:23:35.244654 cognee-0.1.8/cognee/modules/search/graph/__init__.py
--rw-r--r--   0        0        0     2086 2024-05-26 19:03:19.301634 cognee-0.1.8/cognee/modules/search/graph/search_adjacent.py
--rw-r--r--   0        0        0     3192 2024-05-26 19:03:19.301803 cognee-0.1.8/cognee/modules/search/graph/search_categories.py
--rw-r--r--   0        0        0      875 2024-05-26 19:03:19.302100 cognee-0.1.8/cognee/modules/search/graph/search_cypher.py
--rw-r--r--   0        0        0     2962 2024-05-26 19:03:19.302265 cognee-0.1.8/cognee/modules/search/graph/search_neighbour.py
--rw-r--r--   0        0        0     2999 2024-05-26 19:03:19.302427 cognee-0.1.8/cognee/modules/search/graph/search_summary.py
--rw-r--r--   0        0        0        0 2024-05-26 19:03:19.302457 cognee-0.1.8/cognee/modules/search/llm/__init__.py
--rw-r--r--   0        0        0        0 2024-05-26 19:03:19.302527 cognee-0.1.8/cognee/modules/search/llm/extraction/__init__.py
--rw-r--r--   0        0        0      667 2024-05-25 06:16:34.130219 cognee-0.1.8/cognee/modules/search/llm/extraction/categorize_relevant_category.py
--rw-r--r--   0        0        0      703 2024-05-25 06:16:34.130413 cognee-0.1.8/cognee/modules/search/llm/extraction/categorize_relevant_summary.py
--rw-r--r--   0        0        0      650 2024-05-25 06:16:34.130695 cognee-0.1.8/cognee/modules/search/llm/get_relevant_summary.py
--rw-r--r--   0        0        0        0 2024-03-14 09:23:35.244937 cognee-0.1.8/cognee/modules/search/vector/__init__.py
--rw-r--r--   0        0        0       42 2024-05-25 06:16:34.130807 cognee-0.1.8/cognee/modules/search/vector/bm25.py
--rw-r--r--   0        0        0       51 2024-05-25 06:16:34.130913 cognee-0.1.8/cognee/modules/search/vector/fusion.py
--rw-r--r--   0        0        0     2047 2024-05-27 05:37:00.867637 cognee-0.1.8/cognee/modules/search/vector/search_similarity.py
--rw-r--r--   0        0        0      141 2024-05-25 06:16:34.131198 cognee-0.1.8/cognee/modules/settings/__init__.py
--rw-r--r--   0        0        0     2643 2024-05-27 05:37:00.867737 cognee-0.1.8/cognee/modules/settings/get_settings.py
--rw-r--r--   0        0        0      678 2024-05-27 05:37:00.868700 cognee-0.1.8/cognee/modules/settings/save_llm_config.py
--rw-r--r--   0        0        0      606 2024-05-27 05:37:00.868820 cognee-0.1.8/cognee/modules/settings/save_vector_db_config.py
--rw-r--r--   0        0        0      159 2024-05-27 05:37:00.868950 cognee-0.1.8/cognee/modules/tasks/__init__.py
--rw-r--r--   0        0        0      502 2024-05-26 19:03:19.303139 cognee-0.1.8/cognee/modules/tasks/create_task_status_table.py
--rw-r--r--   0        0        0      632 2024-05-27 05:37:00.869016 cognee-0.1.8/cognee/modules/tasks/get_task_status.py
--rw-r--r--   0        0        0      376 2024-05-26 19:03:19.303304 cognee-0.1.8/cognee/modules/tasks/update_task_status.py
--rw-r--r--   0        0        0        0 2024-05-25 06:16:34.131739 cognee-0.1.8/cognee/modules/topology/__init__.py
--rw-r--r--   0        0        0        0 2024-05-26 19:03:19.303341 cognee-0.1.8/cognee/modules/topology/extraction/__init__.py
--rw-r--r--   0        0        0      505 2024-05-25 06:16:34.132108 cognee-0.1.8/cognee/modules/topology/extraction/extract_topology.py
--rw-r--r--   0        0        0      735 2024-05-26 19:03:19.303516 cognee-0.1.8/cognee/modules/topology/infer_data_topology.py
--rw-r--r--   0        0        0     5986 2024-05-26 19:03:19.303736 cognee-0.1.8/cognee/modules/topology/topology.py
--rw-r--r--   0        0        0        0 2024-03-14 09:23:35.245146 cognee-0.1.8/cognee/modules/users/__init__.py
--rw-r--r--   0        0        0      179 2024-04-28 19:24:05.619936 cognee-0.1.8/cognee/modules/users/memory/__init__.py
--rw-r--r--   0        0        0      802 2024-03-14 09:23:35.245545 cognee-0.1.8/cognee/modules/users/memory/create_information_points.py
--rw-r--r--   0        0        0      229 2024-04-28 19:24:05.620017 cognee-0.1.8/cognee/modules/users/memory/is_existing_memory.py
--rw-r--r--   0        0        0      203 2024-04-28 19:24:05.620093 cognee-0.1.8/cognee/modules/users/memory/register_memory_for_user.py
--rw-r--r--   0        0        0   124245 2024-04-23 05:20:06.904069 cognee-0.1.8/cognee/programs/extract_knowledge_graph/extract_knowledge_graph.json
--rw-r--r--   0        0        0      719 2024-05-26 19:03:19.304532 cognee-0.1.8/cognee/root_dir.py
--rw-r--r--   0        0        0      803 2024-05-25 06:16:34.132721 cognee-0.1.8/cognee/shared/GithubClassification.py
--rw-r--r--   0        0        0      984 2024-05-25 06:16:34.132929 cognee-0.1.8/cognee/shared/GithubTopology.py
--rw-r--r--   0        0        0     2009 2024-05-25 06:16:34.133146 cognee-0.1.8/cognee/shared/SourceCodeGraph.py
--rw-r--r--   0        0        0        0 2024-03-14 09:23:35.246078 cognee-0.1.8/cognee/shared/__init__.py
--rw-r--r--   0        0        0     8940 2024-05-26 19:03:19.304823 cognee-0.1.8/cognee/shared/data_models.py
--rw-r--r--   0        0        0      365 2024-03-21 16:01:22.651774 cognee-0.1.8/cognee/shared/encode_uuid.py
--rw-r--r--   0        0        0       72 2024-04-29 19:00:12.026208 cognee-0.1.8/cognee/tests/Untitled.ipynb
--rw-r--r--   0        0        0        0 2024-04-26 13:52:41.240049 cognee-0.1.8/cognee/tests/__init__.py
--rw-r--r--   0        0        0      985 2024-04-26 13:52:41.240261 cognee-0.1.8/cognee/tests/test_data/Natural_language_processing.txt
--rwxr-xr-x   0        0        0     6242 2024-05-26 19:03:19.305141 cognee-0.1.8/cognee/tests/test_library.py
--rw-r--r--   0        0        0     9603 2024-05-25 06:16:34.133633 cognee-0.1.8/cognee/utils.py
--rw-r--r--   0        0        0     3028 2024-05-27 05:37:19.734614 cognee-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     7464 1970-01-01 00:00:00.000000 cognee-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11344 2024-04-23 05:20:06.866180 cognee-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3943 2024-05-27 05:37:00.853829 cognee-0.1.9/README.md
+-rw-r--r--   0        0        0      186 2024-05-10 20:47:32.390494 cognee-0.1.9/cognee/.data/code/e6ac18788c6a51dfaaf9b963d5bc094b.txt
+-rw-r--r--   0        0        0     1257 2024-05-09 09:29:57.011777 cognee-0.1.9/cognee/.data/example/.craft.txt
+-rw-r--r--   0        0        0      716 2024-05-09 09:29:57.009663 cognee-0.1.9/cognee/.data/example/.flake8.txt
+-rw-r--r--   0        0        0      269 2024-05-09 09:29:57.011322 cognee-0.1.9/cognee/.data/example/.gitignore.txt
+-rw-r--r--   0        0        0      124 2024-05-09 09:29:57.010913 cognee-0.1.9/cognee/.data/example/.gitmodules.txt
+-rw-r--r--   0        0        0      636 2024-05-09 09:29:57.010239 cognee-0.1.9/cognee/.data/example/.pre-commit-config.txt
+-rw-r--r--   0        0        0       14 2024-05-09 09:29:57.010581 cognee-0.1.9/cognee/.data/example/.tool-versions.txt
+-rw-r--r--   0        0        0    97420 2024-05-09 09:29:57.010128 cognee-0.1.9/cognee/.data/example/CHANGELOG.txt
+-rw-r--r--   0        0        0     1169 2024-05-09 09:29:57.010808 cognee-0.1.9/cognee/.data/example/CONTRIBUTING-aws-lambda.txt
+-rw-r--r--   0        0        0     9702 2024-05-09 09:29:57.011552 cognee-0.1.9/cognee/.data/example/CONTRIBUTING.txt
+-rw-r--r--   0        0        0     1093 2024-05-09 09:29:57.009989 cognee-0.1.9/cognee/.data/example/LICENSE.txt
+-rw-r--r--   0        0        0       44 2024-05-09 09:29:57.010692 cognee-0.1.9/cognee/.data/example/MANIFEST.txt
+-rw-r--r--   0        0        0     1751 2024-05-09 09:29:57.010349 cognee-0.1.9/cognee/.data/example/Makefile.txt
+-rw-r--r--   0        0        0     4974 2024-05-09 09:29:57.011021 cognee-0.1.9/cognee/.data/example/README.txt
+-rw-r--r--   0        0        0      222 2024-05-09 09:29:56.911149 cognee-0.1.9/cognee/.data/example/aws-lambda-layer-requirements.txt
+-rw-r--r--   0        0        0      336 2024-05-09 09:29:57.009783 cognee-0.1.9/cognee/.data/example/codecov.txt
+-rw-r--r--   0        0        0      304 2024-05-09 09:29:56.911335 cognee-0.1.9/cognee/.data/example/devenv-requirements.txt
+-rw-r--r--   0        0        0        7 2024-05-09 09:29:57.053281 cognee-0.1.9/cognee/.data/example/docs/.gitignore.txt
+-rw-r--r--   0        0        0        0 2024-05-09 09:29:57.053711 cognee-0.1.9/cognee/.data/example/docs/_static/.gitkeep.txt
+-rw-r--r--   0        0        0     1314 2024-05-09 09:29:57.053508 cognee-0.1.9/cognee/.data/example/docs/api.txt
+-rw-r--r--   0        0        0      849 2024-05-09 09:29:57.053402 cognee-0.1.9/cognee/.data/example/docs/apidocs.txt
+-rw-r--r--   0        0        0     5638 2024-05-09 09:29:57.053152 cognee-0.1.9/cognee/.data/example/docs/conf.txt
+-rw-r--r--   0        0        0      376 2024-05-09 09:29:57.053022 cognee-0.1.9/cognee/.data/example/docs/index.txt
+-rw-r--r--   0        0        0      202 2024-05-09 09:29:57.053615 cognee-0.1.9/cognee/.data/example/docs/integrations.txt
+-rw-r--r--   0        0        0       87 2024-05-09 09:29:56.911395 cognee-0.1.9/cognee/.data/example/docs-requirements.txt
+-rw-r--r--   0        0        0      381 2024-05-09 09:29:56.980677 cognee-0.1.9/cognee/.data/example/linter-requirements.txt
+-rw-r--r--   0        0        0     1900 2024-05-09 09:29:57.011115 cognee-0.1.9/cognee/.data/example/mypy.txt
+-rw-r--r--   0        0        0      394 2024-05-09 09:29:57.010472 cognee-0.1.9/cognee/.data/example/pyproject.txt
+-rw-r--r--   0        0        0      519 2024-05-09 09:29:57.009890 cognee-0.1.9/cognee/.data/example/pytest.txt
+-rw-r--r--   0        0        0     1002 2024-05-09 09:29:57.053856 cognee-0.1.9/cognee/.data/example/scripts/aws-attach-layer-to-lambda-function.txt
+-rw-r--r--   0        0        0      641 2024-05-09 09:29:57.054177 cognee-0.1.9/cognee/.data/example/scripts/aws-cleanup.txt
+-rw-r--r--   0        0        0      464 2024-05-09 09:29:57.054550 cognee-0.1.9/cognee/.data/example/scripts/aws-delete-lamba-layer-versions.txt
+-rw-r--r--   0        0        0     1065 2024-05-09 09:29:57.054071 cognee-0.1.9/cognee/.data/example/scripts/aws-deploy-local-layer.txt
+-rw-r--r--   0        0        0     4709 2024-05-09 09:29:57.054423 cognee-0.1.9/cognee/.data/example/scripts/build_aws_lambda_layer.txt
+-rw-r--r--   0        0        0      641 2024-05-09 09:29:57.053957 cognee-0.1.9/cognee/.data/example/scripts/bump-version.txt
+-rw-r--r--   0        0        0     2975 2024-05-09 09:29:57.054281 cognee-0.1.9/cognee/.data/example/scripts/init_serverless_sdk.txt
+-rw-r--r--   0        0        0      846 2024-05-09 09:29:57.054658 cognee-0.1.9/cognee/.data/example/scripts/runtox.txt
+-rw-r--r--   0        0        0     9179 2024-05-09 09:29:57.054884 cognee-0.1.9/cognee/.data/example/scripts/split-tox-gh-actions/split-tox-gh-actions.txt
+-rw-r--r--   0        0        0     1623 2024-05-09 09:29:57.055265 cognee-0.1.9/cognee/.data/example/scripts/split-tox-gh-actions/templates/base.txt
+-rw-r--r--   0        0        0     1065 2024-05-09 09:29:57.055380 cognee-0.1.9/cognee/.data/example/scripts/split-tox-gh-actions/templates/check_permissions.txt
+-rw-r--r--   0        0        0     1101 2024-05-09 09:29:57.055148 cognee-0.1.9/cognee/.data/example/scripts/split-tox-gh-actions/templates/check_required.txt
+-rw-r--r--   0        0        0     3966 2024-05-09 09:29:57.055041 cognee-0.1.9/cognee/.data/example/scripts/split-tox-gh-actions/templates/test_group.txt
+-rw-r--r--   0        0        0     1069 2024-05-09 09:29:57.038396 cognee-0.1.9/cognee/.data/example/sentry_sdk/__init__.txt
+-rw-r--r--   0        0        0     6936 2024-05-09 09:29:57.040081 cognee-0.1.9/cognee/.data/example/sentry_sdk/_compat.txt
+-rw-r--r--   0        0        0     4957 2024-05-09 09:29:57.038744 cognee-0.1.9/cognee/.data/example/sentry_sdk/_functools.txt
+-rw-r--r--   0        0        0     5390 2024-05-09 09:29:57.038165 cognee-0.1.9/cognee/.data/example/sentry_sdk/_lru_cache.txt
+-rw-r--r--   0        0        0    11267 2024-05-09 09:29:57.038619 cognee-0.1.9/cognee/.data/example/sentry_sdk/_queue.txt
+-rw-r--r--   0        0        0     5652 2024-05-09 09:29:57.037298 cognee-0.1.9/cognee/.data/example/sentry_sdk/_types.txt
+-rw-r--r--   0        0        0     3790 2024-05-09 09:29:57.037832 cognee-0.1.9/cognee/.data/example/sentry_sdk/_werkzeug.txt
+-rw-r--r--   0        0        0     6242 2024-05-09 09:29:57.039448 cognee-0.1.9/cognee/.data/example/sentry_sdk/api.txt
+-rw-r--r--   0        0        0     1811 2024-05-09 09:29:57.039335 cognee-0.1.9/cognee/.data/example/sentry_sdk/attachments.txt
+-rw-r--r--   0        0        0    28495 2024-05-09 09:29:57.038042 cognee-0.1.9/cognee/.data/example/sentry_sdk/client.txt
+-rw-r--r--   0        0        0    11598 2024-05-09 09:29:57.039201 cognee-0.1.9/cognee/.data/example/sentry_sdk/consts.txt
+-rw-r--r--   0        0        0      170 2024-05-09 09:29:57.052548 cognee-0.1.9/cognee/.data/example/sentry_sdk/crons/__init__.txt
+-rw-r--r--   0        0        0      953 2024-05-09 09:29:57.052320 cognee-0.1.9/cognee/.data/example/sentry_sdk/crons/_decorator.txt
+-rw-r--r--   0        0        0      506 2024-05-09 09:29:57.052872 cognee-0.1.9/cognee/.data/example/sentry_sdk/crons/_decorator_py2.txt
+-rw-r--r--   0        0        0     1527 2024-05-09 09:29:57.052775 cognee-0.1.9/cognee/.data/example/sentry_sdk/crons/api.txt
+-rw-r--r--   0        0        0       87 2024-05-09 09:29:57.052670 cognee-0.1.9/cognee/.data/example/sentry_sdk/crons/consts.txt
+-rw-r--r--   0        0        0     2401 2024-05-09 09:29:57.052446 cognee-0.1.9/cognee/.data/example/sentry_sdk/crons/decorator.txt
+-rw-r--r--   0        0        0        0 2024-05-09 09:29:57.051812 cognee-0.1.9/cognee/.data/example/sentry_sdk/db/__init__.txt
+-rw-r--r--   0        0        0     1534 2024-05-09 09:29:57.052073 cognee-0.1.9/cognee/.data/example/sentry_sdk/db/explain_plan/__init__.txt
+-rw-r--r--   0        0        0     1597 2024-05-09 09:29:57.051960 cognee-0.1.9/cognee/.data/example/sentry_sdk/db/explain_plan/django.txt
+-rw-r--r--   0        0        0     1656 2024-05-09 09:29:57.052172 cognee-0.1.9/cognee/.data/example/sentry_sdk/db/explain_plan/sqlalchemy.txt
+-rw-r--r--   0        0        0     1132 2024-05-09 09:29:57.039702 cognee-0.1.9/cognee/.data/example/sentry_sdk/debug.txt
+-rw-r--r--   0        0        0     9708 2024-05-09 09:29:57.040585 cognee-0.1.9/cognee/.data/example/sentry_sdk/envelope.txt
+-rw-r--r--   0        0        0    22723 2024-05-09 09:29:57.038984 cognee-0.1.9/cognee/.data/example/sentry_sdk/hub.txt
+-rw-r--r--   0        0        0     7298 2024-05-09 09:29:57.043701 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/__init__.txt
+-rw-r--r--   0        0        0     3096 2024-05-09 09:29:57.047520 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/_asgi_common.txt
+-rw-r--r--   0        0        0     5286 2024-05-09 09:29:57.042096 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/_wsgi_common.txt
+-rw-r--r--   0        0        0    11591 2024-05-09 09:29:57.041477 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/aiohttp.txt
+-rw-r--r--   0        0        0      963 2024-05-09 09:29:57.045018 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/argv.txt
+-rw-r--r--   0        0        0     6228 2024-05-09 09:29:57.046006 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/ariadne.txt
+-rw-r--r--   0        0        0     7180 2024-05-09 09:29:57.045165 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/arq.txt
+-rw-r--r--   0        0        0    11873 2024-05-09 09:29:57.043130 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/asgi.txt
+-rw-r--r--   0        0        0     3201 2024-05-09 09:29:57.043267 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/asyncio.txt
+-rw-r--r--   0        0        0     6297 2024-05-09 09:29:57.041724 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/asyncpg.txt
+-rw-r--r--   0        0        0     1846 2024-05-09 09:29:57.043827 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/atexit.txt
+-rw-r--r--   0        0        0    15922 2024-05-09 09:29:57.041855 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/aws_lambda.txt
+-rw-r--r--   0        0        0     5689 2024-05-09 09:29:57.046865 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/beam.txt
+-rw-r--r--   0        0        0     4542 2024-05-09 09:29:57.046387 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/boto3.txt
+-rw-r--r--   0        0        0     6453 2024-05-09 09:29:57.046735 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/bottle.txt
+-rw-r--r--   0        0        0    21973 2024-05-09 09:29:57.045547 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/celery.txt
+-rw-r--r--   0        0        0     4769 2024-05-09 09:29:57.045835 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/chalice.txt
+-rw-r--r--   0        0        0     5107 2024-05-09 09:29:57.044217 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/clickhouse_driver.txt
+-rw-r--r--   0        0        0     6755 2024-05-09 09:29:57.043423 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/cloud_resource_context.txt
+-rw-r--r--   0        0        0     1184 2024-05-09 09:29:57.042549 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/dedupe.txt
+-rw-r--r--   0        0        0    24135 2024-05-09 09:29:57.050785 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/django/__init__.txt
+-rw-r--r--   0        0        0     7056 2024-05-09 09:29:57.050660 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/django/asgi.txt
+-rw-r--r--   0        0        0     3692 2024-05-09 09:29:57.050997 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/django/caching.txt
+-rw-r--r--   0        0        0     5967 2024-05-09 09:29:57.051109 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/django/middleware.txt
+-rw-r--r--   0        0        0     3054 2024-05-09 09:29:57.050414 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/django/signals_handlers.txt
+-rw-r--r--   0        0        0     5697 2024-05-09 09:29:57.050891 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/django/templates.txt
+-rw-r--r--   0        0        0     5005 2024-05-09 09:29:57.050536 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/django/transactions.txt
+-rw-r--r--   0        0        0     2909 2024-05-09 09:29:57.051222 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/django/views.txt
+-rw-r--r--   0        0        0     2260 2024-05-09 09:29:57.047930 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/excepthook.txt
+-rw-r--r--   0        0        0     2041 2024-05-09 09:29:57.044635 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/executing.txt
+-rw-r--r--   0        0        0     9496 2024-05-09 09:29:57.047081 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/falcon.txt
+-rw-r--r--   0        0        0     4685 2024-05-09 09:29:57.042209 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/fastapi.txt
+-rw-r--r--   0        0        0     7808 2024-05-09 09:29:57.042659 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/flask.txt
+-rw-r--r--   0        0        0     8273 2024-05-09 09:29:57.047406 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/gcp.txt
+-rw-r--r--   0        0        0     2906 2024-05-09 09:29:57.045682 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/gnu_backtrace.txt
+-rw-r--r--   0        0        0     4435 2024-05-09 09:29:57.048081 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/gql.txt
+-rw-r--r--   0        0        0     3746 2024-05-09 09:29:57.046155 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/graphene.txt
+-rw-r--r--   0        0        0     4979 2024-05-09 09:29:57.048716 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/grpc/__init__.txt
+-rw-r--r--   0        0        0      104 2024-05-09 09:29:57.049054 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/grpc/aio/__init__.txt
+-rw-r--r--   0        0        0     3078 2024-05-09 09:29:57.048946 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/grpc/aio/client.txt
+-rw-r--r--   0        0        0     3901 2024-05-09 09:29:57.048847 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/grpc/aio/server.txt
+-rw-r--r--   0        0        0     3235 2024-05-09 09:29:57.048587 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/grpc/client.txt
+-rw-r--r--   0        0        0     2321 2024-05-09 09:29:57.048479 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/grpc/server.txt
+-rw-r--r--   0        0        0     5005 2024-05-09 09:29:57.042430 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/httpx.txt
+-rw-r--r--   0        0        0     5489 2024-05-09 09:29:57.041167 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/huey.txt
+-rw-r--r--   0        0        0     9573 2024-05-09 09:29:57.041050 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/logging.txt
+-rw-r--r--   0        0        0     3051 2024-05-09 09:29:57.047807 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/loguru.txt
+-rw-r--r--   0        0        0      872 2024-05-09 09:29:57.046271 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/modules.txt
+-rw-r--r--   0        0        0    11253 2024-05-09 09:29:57.044872 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/openai.txt
+-rw-r--r--   0        0        0      210 2024-05-09 09:29:57.049551 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/opentelemetry/__init__.txt
+-rw-r--r--   0        0        0      167 2024-05-09 09:29:57.049669 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/opentelemetry/consts.txt
+-rw-r--r--   0        0        0     5830 2024-05-09 09:29:57.049999 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/opentelemetry/integration.txt
+-rw-r--r--   0        0        0     3731 2024-05-09 09:29:57.050128 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/opentelemetry/propagator.txt
+-rw-r--r--   0        0        0    12355 2024-05-09 09:29:57.050285 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/opentelemetry/span_processor.txt
+-rw-r--r--   0        0        0     4554 2024-05-09 09:29:57.042318 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/pure_eval.txt
+-rw-r--r--   0        0        0     6007 2024-05-09 09:29:57.044362 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/pymongo.txt
+-rw-r--r--   0        0        0     7447 2024-05-09 09:29:57.041983 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/pyramid.txt
+-rw-r--r--   0        0        0     7494 2024-05-09 09:29:57.041275 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/quart.txt
+-rw-r--r--   0        0        0    11998 2024-05-09 09:29:57.049412 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/redis/__init__.txt
+-rw-r--r--   0        0        0     2630 2024-05-09 09:29:57.049192 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/redis/asyncio.txt
+-rw-r--r--   0        0        0     5591 2024-05-09 09:29:57.043571 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/rq.txt
+-rw-r--r--   0        0        0    13424 2024-05-09 09:29:57.047678 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/sanic.txt
+-rw-r--r--   0        0        0     1975 2024-05-09 09:29:57.040752 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/serverless.txt
+-rw-r--r--   0        0        0     2945 2024-05-09 09:29:57.047198 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/socket.txt
+-rw-r--r--   0        0        0      208 2024-05-09 09:29:57.051492 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/spark/__init__.txt
+-rw-r--r--   0        0        0     8483 2024-05-09 09:29:57.051700 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/spark/spark_driver.txt
+-rw-r--r--   0        0        0     4013 2024-05-09 09:29:57.051374 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/spark/spark_worker.txt
+-rw-r--r--   0        0        0     5052 2024-05-09 09:29:57.045286 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/sqlalchemy.txt
+-rw-r--r--   0        0        0    24295 2024-05-09 09:29:57.040853 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/starlette.txt
+-rw-r--r--   0        0        0    10211 2024-05-09 09:29:57.044072 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/starlite.txt
+-rw-r--r--   0        0        0     8326 2024-05-09 09:29:57.046611 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/stdlib.txt
+-rw-r--r--   0        0        0    14466 2024-05-09 09:29:57.041605 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/strawberry.txt
+-rw-r--r--   0        0        0     2937 2024-05-09 09:29:57.044499 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/threading.txt
+-rw-r--r--   0        0        0     7337 2024-05-09 09:29:57.045409 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/tornado.txt
+-rw-r--r--   0        0        0     1745 2024-05-09 09:29:57.042872 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/trytond.txt
+-rw-r--r--   0        0        0     9570 2024-05-09 09:29:57.048322 cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/wsgi.txt
+-rw-r--r--   0        0        0    29551 2024-05-09 09:29:57.036871 cognee-0.1.9/cognee/.data/example/sentry_sdk/metrics.txt
+-rw-r--r--   0        0        0     3728 2024-05-09 09:29:57.037398 cognee-0.1.9/cognee/.data/example/sentry_sdk/monitor.txt
+-rw-r--r--   0        0        0    33083 2024-05-09 09:29:57.040230 cognee-0.1.9/cognee/.data/example/sentry_sdk/profiler.txt
+-rw-r--r--   0        0        0        0 2024-05-09 09:29:57.039787 cognee-0.1.9/cognee/.data/example/sentry_sdk/py.txt
+-rw-r--r--   0        0        0    44786 2024-05-09 09:29:57.040370 cognee-0.1.9/cognee/.data/example/sentry_sdk/scope.txt
+-rw-r--r--   0        0        0     5230 2024-05-09 09:29:57.037938 cognee-0.1.9/cognee/.data/example/sentry_sdk/scrubber.txt
+-rw-r--r--   0        0        0    13301 2024-05-09 09:29:57.039928 cognee-0.1.9/cognee/.data/example/sentry_sdk/serializer.txt
+-rw-r--r--   0        0        0     5612 2024-05-09 09:29:57.038280 cognee-0.1.9/cognee/.data/example/sentry_sdk/session.txt
+-rw-r--r--   0        0        0     6488 2024-05-09 09:29:57.037077 cognee-0.1.9/cognee/.data/example/sentry_sdk/sessions.txt
+-rw-r--r--   0        0        0     1443 2024-05-09 09:29:57.036975 cognee-0.1.9/cognee/.data/example/sentry_sdk/spotlight.txt
+-rw-r--r--   0        0        0    36352 2024-05-09 09:29:57.037187 cognee-0.1.9/cognee/.data/example/sentry_sdk/tracing.txt
+-rw-r--r--   0        0        0    15841 2024-05-09 09:29:57.037737 cognee-0.1.9/cognee/.data/example/sentry_sdk/tracing_utils.txt
+-rw-r--r--   0        0        0     1244 2024-05-09 09:29:57.036769 cognee-0.1.9/cognee/.data/example/sentry_sdk/tracing_utils_py2.txt
+-rw-r--r--   0        0        0     2146 2024-05-09 09:29:57.037501 cognee-0.1.9/cognee/.data/example/sentry_sdk/tracing_utils_py3.txt
+-rw-r--r--   0        0        0    21702 2024-05-09 09:29:57.037607 cognee-0.1.9/cognee/.data/example/sentry_sdk/transport.txt
+-rw-r--r--   0        0        0      732 2024-05-09 09:29:57.038864 cognee-0.1.9/cognee/.data/example/sentry_sdk/types.txt
+-rw-r--r--   0        0        0    54025 2024-05-09 09:29:57.039580 cognee-0.1.9/cognee/.data/example/sentry_sdk/utils.txt
+-rw-r--r--   0        0        0     4485 2024-05-09 09:29:57.036658 cognee-0.1.9/cognee/.data/example/sentry_sdk/worker.txt
+-rw-r--r--   0        0        0     4122 2024-05-09 09:29:57.011213 cognee-0.1.9/cognee/.data/example/setup.txt
+-rw-r--r--   0        0        0      480 2024-05-09 09:29:56.995867 cognee-0.1.9/cognee/.data/example/test-requirements.txt
+-rw-r--r--   0        0        0      433 2024-05-09 09:29:57.013056 cognee-0.1.9/cognee/.data/example/tests/__init__.txt
+-rw-r--r--   0        0        0    20029 2024-05-09 09:29:57.012191 cognee-0.1.9/cognee/.data/example/tests/conftest.txt
+-rw-r--r--   0        0        0        0 2024-05-09 09:29:57.036393 cognee-0.1.9/cognee/.data/example/tests/crons/__init__.txt
+-rw-r--r--   0        0        0     9713 2024-05-09 09:29:57.036322 cognee-0.1.9/cognee/.data/example/tests/crons/test_crons.txt
+-rw-r--r--   0        0        0     4240 2024-05-09 09:29:57.036502 cognee-0.1.9/cognee/.data/example/tests/crons/test_crons_async_py3.txt
+-rw-r--r--   0        0        0        0 2024-05-09 09:29:57.016035 cognee-0.1.9/cognee/.data/example/tests/integrations/__init__.txt
+-rw-r--r--   0        0        0       46 2024-05-09 09:29:57.016847 cognee-0.1.9/cognee/.data/example/tests/integrations/aiohttp/__init__.txt
+-rw-r--r--   0        0        0    16055 2024-05-09 09:29:57.016677 cognee-0.1.9/cognee/.data/example/tests/integrations/aiohttp/test_aiohttp.txt
+-rw-r--r--   0        0        0      420 2024-05-09 09:29:57.022727 cognee-0.1.9/cognee/.data/example/tests/integrations/argv/test_argv.txt
+-rw-r--r--   0        0        0      106 2024-05-09 09:29:57.017767 cognee-0.1.9/cognee/.data/example/tests/integrations/ariadne/__init__.txt
+-rw-r--r--   0        0        0     7492 2024-05-09 09:29:57.017895 cognee-0.1.9/cognee/.data/example/tests/integrations/ariadne/test_ariadne.txt
+-rw-r--r--   0        0        0       42 2024-05-09 09:29:57.029021 cognee-0.1.9/cognee/.data/example/tests/integrations/arq/__init__.txt
+-rw-r--r--   0        0        0     7441 2024-05-09 09:29:57.029147 cognee-0.1.9/cognee/.data/example/tests/integrations/arq/test_arq.txt
+-rw-r--r--   0        0        0      129 2024-05-09 09:29:57.017418 cognee-0.1.9/cognee/.data/example/tests/integrations/asgi/__init__.txt
+-rw-r--r--   0        0        0    19269 2024-05-09 09:29:57.017304 cognee-0.1.9/cognee/.data/example/tests/integrations/asgi/test_asgi.txt
+-rw-r--r--   0        0        0        0 2024-05-09 09:29:57.033896 cognee-0.1.9/cognee/.data/example/tests/integrations/asyncio/__init__.txt
+-rw-r--r--   0        0        0    10705 2024-05-09 09:29:57.033806 cognee-0.1.9/cognee/.data/example/tests/integrations/asyncio/test_asyncio_py3.txt
+-rw-r--r--   0        0        0      324 2024-05-09 09:29:57.019807 cognee-0.1.9/cognee/.data/example/tests/integrations/asyncpg/__init__.txt
+-rw-r--r--   0        0        0        0 2024-05-09 09:29:57.019908 cognee-0.1.9/cognee/.data/example/tests/integrations/asyncpg/asyncpg_helpers/__init__.txt
+-rw-r--r--   0        0        0       94 2024-05-09 09:29:57.020039 cognee-0.1.9/cognee/.data/example/tests/integrations/asyncpg/asyncpg_helpers/helpers.txt
+-rw-r--r--   0        0        0    21423 2024-05-09 09:29:57.019699 cognee-0.1.9/cognee/.data/example/tests/integrations/asyncpg/test_asyncpg.txt
+-rw-r--r--   0        0        0       44 2024-05-09 09:29:57.029812 cognee-0.1.9/cognee/.data/example/tests/integrations/aws_lambda/__init__.txt
+-rw-r--r--   0        0        0    12514 2024-05-09 09:29:57.029697 cognee-0.1.9/cognee/.data/example/tests/integrations/aws_lambda/client.txt
+-rw-r--r--   0        0        0    28565 2024-05-09 09:29:57.029563 cognee-0.1.9/cognee/.data/example/tests/integrations/aws_lambda/test_aws.txt
+-rw-r--r--   0        0        0       50 2024-05-09 09:29:57.028442 cognee-0.1.9/cognee/.data/example/tests/integrations/beam/__init__.txt
+-rw-r--r--   0        0        0     5932 2024-05-09 09:29:57.028546 cognee-0.1.9/cognee/.data/example/tests/integrations/beam/test_beam.txt
+-rw-r--r--   0        0        0      230 2024-05-09 09:29:57.035552 cognee-0.1.9/cognee/.data/example/tests/integrations/boto3/__init__.txt
+-rw-r--r--   0        0        0      883 2024-05-09 09:29:57.035756 cognee-0.1.9/cognee/.data/example/tests/integrations/boto3/aws_mock.txt
+-rw-r--r--   0        0        0      869 2024-05-09 09:29:57.035662 cognee-0.1.9/cognee/.data/example/tests/integrations/boto3/s3_list.txt
+-rw-r--r--   0        0        0     4335 2024-05-09 09:29:57.035866 cognee-0.1.9/cognee/.data/example/tests/integrations/boto3/test_s3.txt
+-rw-r--r--   0        0        0       45 2024-05-09 09:29:57.034716 cognee-0.1.9/cognee/.data/example/tests/integrations/bottle/__init__.txt
+-rw-r--r--   0        0        0    12198 2024-05-09 09:29:57.034606 cognee-0.1.9/cognee/.data/example/tests/integrations/bottle/test_bottle.txt
+-rw-r--r--   0        0        0       45 2024-05-09 09:29:57.028760 cognee-0.1.9/cognee/.data/example/tests/integrations/celery/__init__.txt
+-rw-r--r--   0        0        0    18668 2024-05-09 09:29:57.028664 cognee-0.1.9/cognee/.data/example/tests/integrations/celery/test_celery.txt
+-rw-r--r--   0        0        0    16058 2024-05-09 09:29:57.028884 cognee-0.1.9/cognee/.data/example/tests/integrations/celery/test_celery_beat_crons.txt
+-rw-r--r--   0        0        0       46 2024-05-09 09:29:57.025974 cognee-0.1.9/cognee/.data/example/tests/integrations/chalice/__init__.txt
+-rw-r--r--   0        0        0     4389 2024-05-09 09:29:57.026110 cognee-0.1.9/cognee/.data/example/tests/integrations/chalice/test_chalice.txt
+-rw-r--r--   0        0        0       56 2024-05-09 09:29:57.017020 cognee-0.1.9/cognee/.data/example/tests/integrations/clickhouse_driver/__init__.txt
+-rw-r--r--   0        0        0    28896 2024-05-09 09:29:57.017158 cognee-0.1.9/cognee/.data/example/tests/integrations/clickhouse_driver/test_clickhouse_driver.txt
+-rw-r--r--   0        0        0        0 2024-05-09 09:29:57.035968 cognee-0.1.9/cognee/.data/example/tests/integrations/cloud_resource_context/__init__.txt
+-rw-r--r--   0        0        0    12836 2024-05-09 09:29:57.036097 cognee-0.1.9/cognee/.data/example/tests/integrations/cloud_resource_context/test_cloud_resource_context.txt
+-rw-r--r--   0        0        0      560 2024-05-09 09:29:57.015962 cognee-0.1.9/cognee/.data/example/tests/integrations/conftest.txt
+-rw-r--r--   0        0        0      284 2024-05-09 09:29:57.030192 cognee-0.1.9/cognee/.data/example/tests/integrations/django/__init__.txt
+-rw-r--r--   0        0        0       47 2024-05-09 09:29:57.031017 cognee-0.1.9/cognee/.data/example/tests/integrations/django/asgi/__init__.txt
+-rw-r--r--   0        0        0      308 2024-05-09 09:29:57.031144 cognee-0.1.9/cognee/.data/example/tests/integrations/django/asgi/image.txt
+-rw-r--r--   0        0        0    16055 2024-05-09 09:29:57.030892 cognee-0.1.9/cognee/.data/example/tests/integrations/django/asgi/test_asgi.txt
+-rw-r--r--   0        0        0        0 2024-05-09 09:29:57.030628 cognee-0.1.9/cognee/.data/example/tests/integrations/django/django_helpers/__init__.txt
+-rw-r--r--   0        0        0      302 2024-05-09 09:29:57.030737 cognee-0.1.9/cognee/.data/example/tests/integrations/django/django_helpers/views.txt
+-rw-r--r--   0        0        0        0 2024-05-09 09:29:57.031355 cognee-0.1.9/cognee/.data/example/tests/integrations/django/myapp/__init__.txt
+-rw-r--r--   0        0        0      487 2024-05-09 09:29:57.031276 cognee-0.1.9/cognee/.data/example/tests/integrations/django/myapp/asgi.txt
+-rw-r--r--   0        0        0     1020 2024-05-09 09:29:57.031796 cognee-0.1.9/cognee/.data/example/tests/integrations/django/myapp/custom_urls.txt
+-rw-r--r--   0        0        0      284 2024-05-09 09:29:57.031695 cognee-0.1.9/cognee/.data/example/tests/integrations/django/myapp/manage.txt
+-rw-r--r--   0        0        0        0 2024-05-09 09:29:57.032366 cognee-0.1.9/cognee/.data/example/tests/integrations/django/myapp/management/__init__.txt
+-rw-r--r--   0        0        0        0 2024-05-09 09:29:57.032465 cognee-0.1.9/cognee/.data/example/tests/integrations/django/myapp/management/commands/__init__.txt
+-rw-r--r--   0        0        0      187 2024-05-09 09:29:57.032577 cognee-0.1.9/cognee/.data/example/tests/integrations/django/myapp/management/commands/mycrash.txt
+-rw-r--r--   0        0        0      784 2024-05-09 09:29:57.032028 cognee-0.1.9/cognee/.data/example/tests/integrations/django/myapp/middleware.txt
+-rw-r--r--   0        0        0      494 2024-05-09 09:29:57.031471 cognee-0.1.9/cognee/.data/example/tests/integrations/django/myapp/routing.txt
+-rw-r--r--   0        0        0     5143 2024-05-09 09:29:57.031582 cognee-0.1.9/cognee/.data/example/tests/integrations/django/myapp/settings.txt
+-rw-r--r--   0        0        0       75 2024-05-09 09:29:57.033264 cognee-0.1.9/cognee/.data/example/tests/integrations/django/myapp/templates/error.txt
+-rw-r--r--   0        0        0       24 2024-05-09 09:29:57.032917 cognee-0.1.9/cognee/.data/example/tests/integrations/django/myapp/templates/trace_meta.txt
+-rw-r--r--   0        0        0       35 2024-05-09 09:29:57.033115 cognee-0.1.9/cognee/.data/example/tests/integrations/django/myapp/templates/user_name.txt
+-rw-r--r--   0        0        0     4349 2024-05-09 09:29:57.031918 cognee-0.1.9/cognee/.data/example/tests/integrations/django/myapp/urls.txt
+-rw-r--r--   0        0        0     6039 2024-05-09 09:29:57.032156 cognee-0.1.9/cognee/.data/example/tests/integrations/django/myapp/views.txt
+-rw-r--r--   0        0        0      419 2024-05-09 09:29:57.032272 cognee-0.1.9/cognee/.data/example/tests/integrations/django/myapp/wsgi.txt
+-rw-r--r--   0        0        0    43217 2024-05-09 09:29:57.029965 cognee-0.1.9/cognee/.data/example/tests/integrations/django/test_basic.txt
+-rw-r--r--   0        0        0     2440 2024-05-09 09:29:57.030078 cognee-0.1.9/cognee/.data/example/tests/integrations/django/test_data_scrubbing.txt
+-rw-r--r--   0        0        0    15173 2024-05-09 09:29:57.030522 cognee-0.1.9/cognee/.data/example/tests/integrations/django/test_db_query_data.txt
+-rw-r--r--   0        0        0     4077 2024-05-09 09:29:57.030290 cognee-0.1.9/cognee/.data/example/tests/integrations/django/test_transactions.txt
+-rw-r--r--   0        0        0      729 2024-05-09 09:29:57.030404 cognee-0.1.9/cognee/.data/example/tests/integrations/django/utils.txt
+-rw-r--r--   0        0        0     1733 2024-05-09 09:29:57.018268 cognee-0.1.9/cognee/.data/example/tests/integrations/excepthook/test_excepthook.txt
+-rw-r--r--   0        0        0       45 2024-05-09 09:29:57.033580 cognee-0.1.9/cognee/.data/example/tests/integrations/falcon/__init__.txt
+-rw-r--r--   0        0        0    12435 2024-05-09 09:29:57.033459 cognee-0.1.9/cognee/.data/example/tests/integrations/falcon/test_falcon.txt
+-rw-r--r--   0        0        0       46 2024-05-09 09:29:57.027067 cognee-0.1.9/cognee/.data/example/tests/integrations/fastapi/__init__.txt
+-rw-r--r--   0        0        0    14337 2024-05-09 09:29:57.026952 cognee-0.1.9/cognee/.data/example/tests/integrations/fastapi/test_fastapi.txt
+-rw-r--r--   0        0        0       44 2024-05-09 09:29:57.016386 cognee-0.1.9/cognee/.data/example/tests/integrations/flask/__init__.txt
+-rw-r--r--   0        0        0    27402 2024-05-09 09:29:57.016489 cognee-0.1.9/cognee/.data/example/tests/integrations/flask/test_flask.txt
+-rw-r--r--   0        0        0    17513 2024-05-09 09:29:57.024038 cognee-0.1.9/cognee/.data/example/tests/integrations/gcp/test_gcp.txt
+-rw-r--r--   0        0        0       42 2024-05-09 09:29:57.021775 cognee-0.1.9/cognee/.data/example/tests/integrations/gql/__init__.txt
+-rw-r--r--   0        0        0     7366 2024-05-09 09:29:57.021884 cognee-0.1.9/cognee/.data/example/tests/integrations/gql/test_gql.txt
+-rw-r--r--   0        0        0      107 2024-05-09 09:29:57.026643 cognee-0.1.9/cognee/.data/example/tests/integrations/graphene/__init__.txt
+-rw-r--r--   0        0        0     5663 2024-05-09 09:29:57.026783 cognee-0.1.9/cognee/.data/example/tests/integrations/graphene/test_graphene_py3.txt
+-rw-r--r--   0        0        0      177 2024-05-09 09:29:57.018972 cognee-0.1.9/cognee/.data/example/tests/integrations/grpc/__init__.txt
+-rw-r--r--   0        0        0      403 2024-05-09 09:29:57.019314 cognee-0.1.9/cognee/.data/example/tests/integrations/grpc/compile_test_services.txt
+-rw-r--r--   0        0        0     1608 2024-05-09 09:29:57.019197 cognee-0.1.9/cognee/.data/example/tests/integrations/grpc/grpc_test_service_pb2.txt
+-rw-r--r--   0        0        0     7557 2024-05-09 09:29:57.019100 cognee-0.1.9/cognee/.data/example/tests/integrations/grpc/grpc_test_service_pb2_grpc.txt
+-rw-r--r--   0        0        0      409 2024-05-09 09:29:57.019566 cognee-0.1.9/cognee/.data/example/tests/integrations/grpc/protos/grpc_test_service.txt
+-rw-r--r--   0        0        0    10556 2024-05-09 09:29:57.018737 cognee-0.1.9/cognee/.data/example/tests/integrations/grpc/test_grpc.txt
+-rw-r--r--   0        0        0     8185 2024-05-09 09:29:57.019428 cognee-0.1.9/cognee/.data/example/tests/integrations/grpc/test_grpc_aio.txt
+-rw-r--r--   0        0        0       44 2024-05-09 09:29:57.026263 cognee-0.1.9/cognee/.data/example/tests/integrations/httpx/__init__.txt
+-rw-r--r--   0        0        0     8965 2024-05-09 09:29:57.026483 cognee-0.1.9/cognee/.data/example/tests/integrations/httpx/test_httpx.txt
+-rw-r--r--   0        0        0       43 2024-05-09 09:29:57.022292 cognee-0.1.9/cognee/.data/example/tests/integrations/huey/__init__.txt
+-rw-r--r--   0        0        0     5071 2024-05-09 09:29:57.022163 cognee-0.1.9/cognee/.data/example/tests/integrations/huey/test_huey.txt
+-rw-r--r--   0        0        0     6912 2024-05-09 09:29:57.034033 cognee-0.1.9/cognee/.data/example/tests/integrations/logging/test_logging.txt
+-rw-r--r--   0        0        0       45 2024-05-09 09:29:57.027978 cognee-0.1.9/cognee/.data/example/tests/integrations/loguru/__init__.txt
+-rw-r--r--   0        0        0     3266 2024-05-09 09:29:57.027868 cognee-0.1.9/cognee/.data/example/tests/integrations/loguru/test_loguru.txt
+-rw-r--r--   0        0        0      367 2024-05-09 09:29:57.029424 cognee-0.1.9/cognee/.data/example/tests/integrations/modules/test_modules.txt
+-rw-r--r--   0        0        0       45 2024-05-09 09:29:57.035193 cognee-0.1.9/cognee/.data/example/tests/integrations/openai/__init__.txt
+-rw-r--r--   0        0        0     7535 2024-05-09 09:29:57.035087 cognee-0.1.9/cognee/.data/example/tests/integrations/openai/test_openai.txt
+-rw-r--r--   0        0        0       52 2024-05-09 09:29:57.021548 cognee-0.1.9/cognee/.data/example/tests/integrations/opentelemetry/__init__.txt
+-rw-r--r--   0        0        0      993 2024-05-09 09:29:57.021650 cognee-0.1.9/cognee/.data/example/tests/integrations/opentelemetry/test_experimental.txt
+-rw-r--r--   0        0        0     7951 2024-05-09 09:29:57.021447 cognee-0.1.9/cognee/.data/example/tests/integrations/opentelemetry/test_propagator.txt
+-rw-r--r--   0        0        0    21486 2024-05-09 09:29:57.021335 cognee-0.1.9/cognee/.data/example/tests/integrations/opentelemetry/test_span_processor.txt
+-rw-r--r--   0        0        0       48 2024-05-09 09:29:57.018031 cognee-0.1.9/cognee/.data/example/tests/integrations/pure_eval/__init__.txt
+-rw-r--r--   0        0        0     2445 2024-05-09 09:29:57.018140 cognee-0.1.9/cognee/.data/example/tests/integrations/pure_eval/test_pure_eval.txt
+-rw-r--r--   0        0        0       46 2024-05-09 09:29:57.024908 cognee-0.1.9/cognee/.data/example/tests/integrations/pymongo/__init__.txt
+-rw-r--r--   0        0        0    14425 2024-05-09 09:29:57.024783 cognee-0.1.9/cognee/.data/example/tests/integrations/pymongo/test_pymongo.txt
+-rw-r--r--   0        0        0       46 2024-05-09 09:29:57.023114 cognee-0.1.9/cognee/.data/example/tests/integrations/pyramid/__init__.txt
+-rw-r--r--   0        0        0    11072 2024-05-09 09:29:57.022983 cognee-0.1.9/cognee/.data/example/tests/integrations/pyramid/test_pyramid.txt
+-rw-r--r--   0        0        0       44 2024-05-09 09:29:57.022440 cognee-0.1.9/cognee/.data/example/tests/integrations/quart/__init__.txt
+-rw-r--r--   0        0        0    14540 2024-05-09 09:29:57.022568 cognee-0.1.9/cognee/.data/example/tests/integrations/quart/test_quart.txt
+-rw-r--r--   0        0        0       44 2024-05-09 09:29:57.020398 cognee-0.1.9/cognee/.data/example/tests/integrations/redis/__init__.txt
+-rw-r--r--   0        0        0       57 2024-05-09 09:29:57.021036 cognee-0.1.9/cognee/.data/example/tests/integrations/redis/asyncio/__init__.txt
+-rw-r--r--   0        0        0     2423 2024-05-09 09:29:57.021170 cognee-0.1.9/cognee/.data/example/tests/integrations/redis/asyncio/test_redis_asyncio.txt
+-rw-r--r--   0        0        0       52 2024-05-09 09:29:57.020530 cognee-0.1.9/cognee/.data/example/tests/integrations/redis/cluster/__init__.txt
+-rw-r--r--   0        0        0     4441 2024-05-09 09:29:57.020647 cognee-0.1.9/cognee/.data/example/tests/integrations/redis/cluster/test_redis_cluster.txt
+-rw-r--r--   0        0        0       60 2024-05-09 09:29:57.020778 cognee-0.1.9/cognee/.data/example/tests/integrations/redis/cluster_asyncio/__init__.txt
+-rw-r--r--   0        0        0     4188 2024-05-09 09:29:57.020894 cognee-0.1.9/cognee/.data/example/tests/integrations/redis/cluster_asyncio/test_redis_cluster_asyncio.txt
+-rw-r--r--   0        0        0     9022 2024-05-09 09:29:57.020291 cognee-0.1.9/cognee/.data/example/tests/integrations/redis/test_redis.txt
+-rw-r--r--   0        0        0       51 2024-05-09 09:29:57.018400 cognee-0.1.9/cognee/.data/example/tests/integrations/rediscluster/__init__.txt
+-rw-r--r--   0        0        0     5016 2024-05-09 09:29:57.018513 cognee-0.1.9/cognee/.data/example/tests/integrations/rediscluster/test_rediscluster.txt
+-rw-r--r--   0        0        0       47 2024-05-09 09:29:57.025377 cognee-0.1.9/cognee/.data/example/tests/integrations/requests/__init__.txt
+-rw-r--r--   0        0        0     2061 2024-05-09 09:29:57.025513 cognee-0.1.9/cognee/.data/example/tests/integrations/requests/test_requests.txt
+-rw-r--r--   0        0        0       41 2024-05-09 09:29:57.034380 cognee-0.1.9/cognee/.data/example/tests/integrations/rq/__init__.txt
+-rw-r--r--   0        0        0     8582 2024-05-09 09:29:57.034258 cognee-0.1.9/cognee/.data/example/tests/integrations/rq/test_rq.txt
+-rw-r--r--   0        0        0       44 2024-05-09 09:29:57.027210 cognee-0.1.9/cognee/.data/example/tests/integrations/sanic/__init__.txt
+-rw-r--r--   0        0        0    13506 2024-05-09 09:29:57.027348 cognee-0.1.9/cognee/.data/example/tests/integrations/sanic/test_sanic.txt
+-rw-r--r--   0        0        0     1042 2024-05-09 09:29:57.022011 cognee-0.1.9/cognee/.data/example/tests/integrations/serverless/test_serverless.txt
+-rw-r--r--   0        0        0       45 2024-05-09 09:29:57.035431 cognee-0.1.9/cognee/.data/example/tests/integrations/socket/__init__.txt
+-rw-r--r--   0        0        0     1641 2024-05-09 09:29:57.035327 cognee-0.1.9/cognee/.data/example/tests/integrations/socket/test_socket.txt
+-rw-r--r--   0        0        0       74 2024-05-09 09:29:57.034953 cognee-0.1.9/cognee/.data/example/tests/integrations/spark/__init__.txt
+-rw-r--r--   0        0        0     6598 2024-05-09 09:29:57.034849 cognee-0.1.9/cognee/.data/example/tests/integrations/spark/test_spark.txt
+-rw-r--r--   0        0        0      292 2024-05-09 09:29:57.024338 cognee-0.1.9/cognee/.data/example/tests/integrations/sqlalchemy/__init__.txt
+-rw-r--r--   0        0        0        0 2024-05-09 09:29:57.024459 cognee-0.1.9/cognee/.data/example/tests/integrations/sqlalchemy/sqlalchemy_helpers/__init__.txt
+-rw-r--r--   0        0        0      192 2024-05-09 09:29:57.024603 cognee-0.1.9/cognee/.data/example/tests/integrations/sqlalchemy/sqlalchemy_helpers/helpers.txt
+-rw-r--r--   0        0        0    21401 2024-05-09 09:29:57.024205 cognee-0.1.9/cognee/.data/example/tests/integrations/sqlalchemy/test_sqlalchemy.txt
+-rw-r--r--   0        0        0       48 2024-05-09 09:29:57.023271 cognee-0.1.9/cognee/.data/example/tests/integrations/starlette/__init__.txt
+-rw-r--r--   0        0        0    21014 2024-05-09 09:29:57.023405 cognee-0.1.9/cognee/.data/example/tests/integrations/starlette/photo.txt
+-rw-r--r--   0        0        0       24 2024-05-09 09:29:57.023706 cognee-0.1.9/cognee/.data/example/tests/integrations/starlette/templates/trace_meta.txt
+-rw-r--r--   0        0        0    35093 2024-05-09 09:29:57.023542 cognee-0.1.9/cognee/.data/example/tests/integrations/starlette/test_starlette.txt
+-rw-r--r--   0        0        0       47 2024-05-09 09:29:57.028320 cognee-0.1.9/cognee/.data/example/tests/integrations/starlite/__init__.txt
+-rw-r--r--   0        0        0     9647 2024-05-09 09:29:57.028209 cognee-0.1.9/cognee/.data/example/tests/integrations/starlite/test_starlite.txt
+-rw-r--r--   0        0        0    10655 2024-05-09 09:29:57.027727 cognee-0.1.9/cognee/.data/example/tests/integrations/stdlib/test_httplib.txt
+-rw-r--r--   0        0        0     5045 2024-05-09 09:29:57.027509 cognee-0.1.9/cognee/.data/example/tests/integrations/stdlib/test_subprocess.txt
+-rw-r--r--   0        0        0        0 2024-05-09 09:29:57.017516 cognee-0.1.9/cognee/.data/example/tests/integrations/strawberry/__init__.txt
+-rw-r--r--   0        0        0    19273 2024-05-09 09:29:57.017631 cognee-0.1.9/cognee/.data/example/tests/integrations/strawberry/test_strawberry_py3.txt
+-rw-r--r--   0        0        0    10881 2024-05-09 09:29:57.016250 cognee-0.1.9/cognee/.data/example/tests/integrations/test_gnu_backtrace.txt
+-rw-r--r--   0        0        0     5769 2024-05-09 09:29:57.029284 cognee-0.1.9/cognee/.data/example/tests/integrations/threading/test_threading.txt
+-rw-r--r--   0        0        0       46 2024-05-09 09:29:57.025691 cognee-0.1.9/cognee/.data/example/tests/integrations/tornado/__init__.txt
+-rw-r--r--   0        0        0    13348 2024-05-09 09:29:57.025828 cognee-0.1.9/cognee/.data/example/tests/integrations/tornado/test_tornado.txt
+-rw-r--r--   0        0        0       46 2024-05-09 09:29:57.025073 cognee-0.1.9/cognee/.data/example/tests/integrations/trytond/__init__.txt
+-rw-r--r--   0        0        0     3584 2024-05-09 09:29:57.025212 cognee-0.1.9/cognee/.data/example/tests/integrations/trytond/test_trytond.txt
+-rw-r--r--   0        0        0    13237 2024-05-09 09:29:57.023890 cognee-0.1.9/cognee/.data/example/tests/integrations/wsgi/test_wsgi.txt
+-rw-r--r--   0        0        0     3681 2024-05-09 09:29:57.013923 cognee-0.1.9/cognee/.data/example/tests/test_api.txt
+-rw-r--r--   0        0        0    23643 2024-05-09 09:29:57.012396 cognee-0.1.9/cognee/.data/example/tests/test_basics.txt
+-rw-r--r--   0        0        0    41119 2024-05-09 09:29:57.014041 cognee-0.1.9/cognee/.data/example/tests/test_client.txt
+-rw-r--r--   0        0        0     3417 2024-05-09 09:29:57.012616 cognee-0.1.9/cognee/.data/example/tests/test_conftest.txt
+-rw-r--r--   0        0        0     8137 2024-05-09 09:29:57.013721 cognee-0.1.9/cognee/.data/example/tests/test_envelope.txt
+-rw-r--r--   0        0        0     8578 2024-05-09 09:29:57.013472 cognee-0.1.9/cognee/.data/example/tests/test_exceptiongroup.txt
+-rw-r--r--   0        0        0      784 2024-05-09 09:29:57.013826 cognee-0.1.9/cognee/.data/example/tests/test_lru_cache.txt
+-rw-r--r--   0        0        0    31466 2024-05-09 09:29:57.012506 cognee-0.1.9/cognee/.data/example/tests/test_metrics.txt
+-rw-r--r--   0        0        0     2702 2024-05-09 09:29:57.011977 cognee-0.1.9/cognee/.data/example/tests/test_monitor.txt
+-rw-r--r--   0        0        0    24427 2024-05-09 09:29:57.013272 cognee-0.1.9/cognee/.data/example/tests/test_profiler.txt
+-rw-r--r--   0        0        0     4058 2024-05-09 09:29:57.012951 cognee-0.1.9/cognee/.data/example/tests/test_scope.txt
+-rw-r--r--   0        0        0     5357 2024-05-09 09:29:57.012302 cognee-0.1.9/cognee/.data/example/tests/test_scrubber.txt
+-rw-r--r--   0        0        0     4816 2024-05-09 09:29:57.012842 cognee-0.1.9/cognee/.data/example/tests/test_serializer.txt
+-rw-r--r--   0        0        0     4184 2024-05-09 09:29:57.012737 cognee-0.1.9/cognee/.data/example/tests/test_sessions.txt
+-rw-r--r--   0        0        0     1490 2024-05-09 09:29:57.013600 cognee-0.1.9/cognee/.data/example/tests/test_spotlight.txt
+-rw-r--r--   0        0        0    18416 2024-05-09 09:29:57.013163 cognee-0.1.9/cognee/.data/example/tests/test_transport.txt
+-rw-r--r--   0        0        0      760 2024-05-09 09:29:57.014146 cognee-0.1.9/cognee/.data/example/tests/test_types.txt
+-rw-r--r--   0        0        0    22888 2024-05-09 09:29:57.012082 cognee-0.1.9/cognee/.data/example/tests/test_utils.txt
+-rw-r--r--   0        0        0     2699 2024-05-09 09:29:57.015252 cognee-0.1.9/cognee/.data/example/tests/tracing/test_baggage.txt
+-rw-r--r--   0        0        0     1820 2024-05-09 09:29:57.014647 cognee-0.1.9/cognee/.data/example/tests/tracing/test_decorator_async_py3.txt
+-rw-r--r--   0        0        0     1665 2024-05-09 09:29:57.015353 cognee-0.1.9/cognee/.data/example/tests/tracing/test_decorator_sync.txt
+-rw-r--r--   0        0        0      575 2024-05-09 09:29:57.014757 cognee-0.1.9/cognee/.data/example/tests/tracing/test_deprecated.txt
+-rw-r--r--   0        0        0     1813 2024-05-09 09:29:57.014855 cognee-0.1.9/cognee/.data/example/tests/tracing/test_http_headers.txt
+-rw-r--r--   0        0        0     9610 2024-05-09 09:29:57.014389 cognee-0.1.9/cognee/.data/example/tests/tracing/test_integration_tests.txt
+-rw-r--r--   0        0        0    12757 2024-05-09 09:29:57.014533 cognee-0.1.9/cognee/.data/example/tests/tracing/test_misc.txt
+-rw-r--r--   0        0        0     1792 2024-05-09 09:29:57.014957 cognee-0.1.9/cognee/.data/example/tests/tracing/test_noop_span.txt
+-rw-r--r--   0        0        0    10643 2024-05-09 09:29:57.015148 cognee-0.1.9/cognee/.data/example/tests/tracing/test_sampling.txt
+-rw-r--r--   0        0        0       40 2024-05-09 09:29:57.015690 cognee-0.1.9/cognee/.data/example/tests/utils/__init__.txt
+-rw-r--r--   0        0        0      797 2024-05-09 09:29:57.015572 cognee-0.1.9/cognee/.data/example/tests/utils/test_contextvars.txt
+-rw-r--r--   0        0        0    17196 2024-05-09 09:29:57.015804 cognee-0.1.9/cognee/.data/example/tests/utils/test_general.txt
+-rw-r--r--   0        0        0     1539 2024-05-09 09:29:57.015472 cognee-0.1.9/cognee/.data/example/tests/utils/test_transaction.txt
+-rw-r--r--   0        0        0    20053 2024-05-09 09:29:57.011668 cognee-0.1.9/cognee/.data/example/tox.txt
+-rw-r--r--   0        0        0      123 2024-04-23 06:52:58.178501 cognee-0.1.9/cognee/.data/example_dataset/271fd0a1a088575885fddc726c4dba04.txt
+-rw-r--r--   0        0        0      426 2024-05-21 06:59:15.075082 cognee-0.1.9/cognee/.data/example_dataset/8e944490a15f563780e6c3f040880b19.txt
+-rw-r--r--   0        0        0     3087 2024-04-02 07:24:38.404088 cognee-0.1.9/cognee/.data/explanations/062c22df-d99b-599f-90cd-2d325c8bcf69.txt
+-rw-r--r--   0        0        0     9041 2024-04-23 07:36:22.827937 cognee-0.1.9/cognee/.data/explanations/6dfe01b6-07d2-5b77-83c8-1d6c11ce2aa7.txt
+-rw-r--r--   0        0        0      985 2024-03-30 19:01:36.385908 cognee-0.1.9/cognee/.data/explanations/Natural language processing.txt
+-rw-r--r--   0        0        0       51 2024-04-18 08:17:53.704561 cognee-0.1.9/cognee/.data/explanations/bab90046-1d9b-598c-8711-dab30f501915.txt
+-rw-r--r--   0        0        0       36 2024-05-21 09:16:37.925545 cognee-0.1.9/cognee/.data/initial_test/14a27354cb3f50ffaaace292d5b7aa58.txt
+-rw-r--r--   0        0        0       44 2024-05-21 09:16:37.923975 cognee-0.1.9/cognee/.data/initial_test/15a66b1d75a45fbfa2d5f8d7b2506d88.txt
+-rw-r--r--   0        0        0       58 2024-05-21 09:16:37.924807 cognee-0.1.9/cognee/.data/initial_test/a881954da33b5e3c8bcf1bc63e50ae20.txt
+-rw-r--r--   0        0        0      985 2024-05-27 08:19:31.232678 cognee-0.1.9/cognee/.data/main/Natural_language_processing.txt
+-rw-r--r--   0        0        0     2003 2024-05-27 05:52:48.164273 cognee-0.1.9/cognee/.data/main/fff.txt
+-rw-r--r--   0        0        0     4090 2024-05-27 05:54:30.542748 cognee-0.1.9/cognee/.data/main/mkdocs.yml
+-rw-r--r--   0        0        0   138566 2024-05-27 05:45:47.626707 cognee-0.1.9/cognee/.data/main/rda svest o sebi.docx
+-rw-r--r--   0        0        0      186 2024-04-29 18:24:10.776372 cognee-0.1.9/cognee/.data/test/e6ac18788c6a51dfaaf9b963d5bc094b.txt
+-rw-r--r--   0        0        0      249 2024-04-23 05:20:06.890311 cognee-0.1.9/cognee/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-14 09:23:35.230717 cognee-0.1.9/cognee/api/__init__.py
+-rw-r--r--   0        0        0     8753 2024-05-27 05:37:00.861835 cognee-0.1.9/cognee/api/client.py
+-rw-r--r--   0        0        0        0 2024-03-14 09:23:35.230960 cognee-0.1.9/cognee/api/v1/__init__.py
+-rw-r--r--   0        0        0       21 2024-03-14 09:23:35.231099 cognee-0.1.9/cognee/api/v1/add/__init__.py
+-rw-r--r--   0        0        0     5216 2024-05-26 19:03:19.264649 cognee-0.1.9/cognee/api/v1/add/add.py
+-rw-r--r--   0        0        0     1629 2024-05-26 19:03:19.265636 cognee-0.1.9/cognee/api/v1/add/add_standalone.py
+-rw-r--r--   0        0        0      626 2024-03-29 12:59:22.978997 cognee-0.1.9/cognee/api/v1/add/remember.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:52:41.234848 cognee-0.1.9/cognee/api/v1/cognify/__init__.py
+-rw-r--r--   0        0        0    12097 2024-05-27 06:53:43.511355 cognee-0.1.9/cognee/api/v1/cognify/cognify.py
+-rw-r--r--   0        0        0     6884 2024-04-25 08:56:45.148041 cognee-0.1.9/cognee/api/v1/cognify/tst.py
+-rw-r--r--   0        0        0       27 2024-03-29 12:59:22.979399 cognee-0.1.9/cognee/api/v1/config/__init__.py
+-rw-r--r--   0        0        0     2552 2024-05-27 05:37:00.864513 cognee-0.1.9/cognee/api/v1/config/config.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:52:41.235161 cognee-0.1.9/cognee/api/v1/datasets/__init__.py
+-rw-r--r--   0        0        0     1184 2024-05-27 05:37:00.864752 cognee-0.1.9/cognee/api/v1/datasets/datasets.py
+-rw-r--r--   0        0        0       25 2024-04-23 05:20:06.891056 cognee-0.1.9/cognee/api/v1/prune/__init__.py
+-rw-r--r--   0        0        0     1177 2024-05-27 06:53:43.511632 cognee-0.1.9/cognee/api/v1/prune/prune.py
+-rw-r--r--   0        0        0       39 2024-03-21 16:01:22.628858 cognee-0.1.9/cognee/api/v1/search/__init__.py
+-rw-r--r--   0        0        0     3973 2024-05-26 19:03:19.267387 cognee-0.1.9/cognee/api/v1/search/search.py
+-rw-r--r--   0        0        0        0 2024-05-25 06:16:34.118332 cognee-0.1.9/cognee/api/v1/topology/__init__.py
+-rw-r--r--   0        0        0     3845 2024-05-26 19:03:19.267657 cognee-0.1.9/cognee/api/v1/topology/add_topology.py
+-rw-r--r--   0        0        0     2836 2024-05-19 13:52:43.158383 cognee-0.1.9/cognee/api/v1/topology/rrrr.py
+-rw-r--r--   0        0        0      781 2024-05-27 05:37:00.865047 cognee-0.1.9/cognee/base_config.py
+-rw-r--r--   0        0        0     5730 2024-05-26 19:03:19.268694 cognee-0.1.9/cognee/config.py
+-rw-r--r--   0        0        0     1778 2024-04-28 19:24:05.618264 cognee-0.1.9/cognee/fetch_secret.py
+-rw-r--r--   0        0        0     7145 2024-05-27 05:37:00.865343 cognee-0.1.9/cognee/infrastructure/InfrastructureConfig.py
+-rw-r--r--   0        0        0       56 2024-03-14 09:23:35.235336 cognee-0.1.9/cognee/infrastructure/__init__.py
+-rw-r--r--   0        0        0      110 2024-03-29 12:59:22.980107 cognee-0.1.9/cognee/infrastructure/data/__init__.py
+-rw-r--r--   0        0        0     4457 2024-05-25 06:16:34.119439 cognee-0.1.9/cognee/infrastructure/data/chunking/DefaultChunkEngine.py
+-rw-r--r--   0        0        0        0 2024-05-25 06:16:34.119461 cognee-0.1.9/cognee/infrastructure/data/chunking/HaystackChunkEngine.py
+-rw-r--r--   0        0        0     1661 2024-05-25 06:16:34.119789 cognee-0.1.9/cognee/infrastructure/data/chunking/LangchainChunkingEngine.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:52:41.236173 cognee-0.1.9/cognee/infrastructure/data/chunking/__init__.py
+-rw-r--r--   0        0        0      763 2024-05-26 19:03:19.270005 cognee-0.1.9/cognee/infrastructure/data/chunking/config.py
+-rw-r--r--   0        0        0      889 2024-03-14 09:23:35.235567 cognee-0.1.9/cognee/infrastructure/data/models/Data.py
+-rw-r--r--   0        0        0      721 2024-03-14 09:23:35.235631 cognee-0.1.9/cognee/infrastructure/data/models/Dataset.py
+-rw-r--r--   0        0        0      553 2024-03-14 09:23:35.235756 cognee-0.1.9/cognee/infrastructure/data/models/DatasetData.py
+-rw-r--r--   0        0        0        0 2024-03-14 09:23:35.235800 cognee-0.1.9/cognee/infrastructure/data/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:52:41.236240 cognee-0.1.9/cognee/infrastructure/data/utils/__init__.py
+-rw-r--r--   0        0        0      756 2024-04-23 05:20:06.895346 cognee-0.1.9/cognee/infrastructure/data/utils/extract_keywords.py
+-rw-r--r--   0        0        0        0 2024-03-14 09:23:35.235884 cognee-0.1.9/cognee/infrastructure/databases/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-14 09:23:35.235957 cognee-0.1.9/cognee/infrastructure/databases/graph/__init__.py
+-rw-r--r--   0        0        0     1640 2024-05-26 19:03:19.270423 cognee-0.1.9/cognee/infrastructure/databases/graph/config.py
+-rw-r--r--   0        0        0        0 2024-05-25 06:16:34.119846 cognee-0.1.9/cognee/infrastructure/databases/graph/falkordb/__init__.py
+-rw-r--r--   0        0        0     6177 2024-05-25 06:16:34.120113 cognee-0.1.9/cognee/infrastructure/databases/graph/falkordb/adapter.py
+-rw-r--r--   0        0        0     1553 2024-05-26 19:03:19.271191 cognee-0.1.9/cognee/infrastructure/databases/graph/get_graph_client.py
+-rw-r--r--   0        0        0     1162 2024-04-23 05:20:06.895582 cognee-0.1.9/cognee/infrastructure/databases/graph/graph_db_interface.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:20:06.895611 cognee-0.1.9/cognee/infrastructure/databases/graph/neo4j_driver/__init__.py
+-rw-r--r--   0        0        0     6154 2024-05-26 19:03:19.271548 cognee-0.1.9/cognee/infrastructure/databases/graph/neo4j_driver/adapter.py
+-rw-r--r--   0        0        0        0 2024-03-14 09:23:35.236389 cognee-0.1.9/cognee/infrastructure/databases/graph/networkx/__init__.py
+-rw-r--r--   0        0        0     5360 2024-05-25 06:16:34.120573 cognee-0.1.9/cognee/infrastructure/databases/graph/networkx/adapter.py
+-rw-r--r--   0        0        0      462 2024-03-14 09:23:35.236879 cognee-0.1.9/cognee/infrastructure/databases/relational/DatabaseEngine.py
+-rw-r--r--   0        0        0       76 2024-03-14 09:23:35.236991 cognee-0.1.9/cognee/infrastructure/databases/relational/ModelBase.py
+-rw-r--r--   0        0        0      170 2024-03-14 09:23:35.237089 cognee-0.1.9/cognee/infrastructure/databases/relational/__init__.py
+-rw-r--r--   0        0        0     1353 2024-05-27 05:37:00.865581 cognee-0.1.9/cognee/infrastructure/databases/relational/config.py
+-rw-r--r--   0        0        0     6666 2024-05-27 05:37:00.866108 cognee-0.1.9/cognee/infrastructure/databases/relational/duckdb/DuckDBAdapter.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:52:41.237764 cognee-0.1.9/cognee/infrastructure/databases/relational/duckdb/__init__.py
+-rw-r--r--   0        0        0     1006 2024-03-14 09:23:35.237616 cognee-0.1.9/cognee/infrastructure/databases/relational/relational_db_interface.py
+-rw-r--r--   0        0        0     2847 2024-03-14 09:23:35.237690 cognee-0.1.9/cognee/infrastructure/databases/relational/sqlite/SqliteEngine.py
+-rw-r--r--   0        0        0        0 2024-03-14 09:23:35.237716 cognee-0.1.9/cognee/infrastructure/databases/relational/sqlite/__init__.py
+-rw-r--r--   0        0        0       41 2024-03-14 09:23:35.237829 cognee-0.1.9/cognee/infrastructure/databases/relational/utils/__init__.py
+-rw-r--r--   0        0        0      595 2024-03-14 09:23:35.237896 cognee-0.1.9/cognee/infrastructure/databases/relational/utils/with_rollback.py
+-rw-r--r--   0        0        0      230 2024-05-27 05:37:00.866399 cognee-0.1.9/cognee/infrastructure/databases/vector/__init__.py
+-rw-r--r--   0        0        0     1549 2024-05-27 05:37:00.866518 cognee-0.1.9/cognee/infrastructure/databases/vector/config.py
+-rw-r--r--   0        0        0     1372 2024-05-27 06:53:43.511779 cognee-0.1.9/cognee/infrastructure/databases/vector/create_vector_engine.py
+-rw-r--r--   0        0        0     2381 2024-05-26 19:03:19.273200 cognee-0.1.9/cognee/infrastructure/databases/vector/embeddings/DefaultEmbeddingEngine.py
+-rw-r--r--   0        0        0      243 2024-05-25 06:16:34.121382 cognee-0.1.9/cognee/infrastructure/databases/vector/embeddings/EmbeddingEngine.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:52:41.237831 cognee-0.1.9/cognee/infrastructure/databases/vector/embeddings/__init__.py
+-rw-r--r--   0        0        0     1091 2024-05-26 19:03:19.273824 cognee-0.1.9/cognee/infrastructure/databases/vector/embeddings/config.py
+-rw-r--r--   0        0        0     1474 2024-05-26 19:03:19.274145 cognee-0.1.9/cognee/infrastructure/databases/vector/falkordb/FalkorDBAdapter.py
+-rw-r--r--   0        0        0     5331 2024-05-25 06:16:34.121496 cognee-0.1.9/cognee/infrastructure/databases/vector/lancedb/LanceDBAdapter.py
+-rw-r--r--   0        0        0        0 2024-05-25 06:16:34.121519 cognee-0.1.9/cognee/infrastructure/databases/vector/lancedb/__init__.py
+-rw-r--r--   0        0        0      138 2024-03-21 16:01:22.631437 cognee-0.1.9/cognee/infrastructure/databases/vector/models/CollectionConfig.py
+-rw-r--r--   0        0        0      398 2024-05-25 06:16:34.121821 cognee-0.1.9/cognee/infrastructure/databases/vector/models/DataPoint.py
+-rw-r--r--   0        0        0       69 2024-05-25 06:16:34.122276 cognee-0.1.9/cognee/infrastructure/databases/vector/models/PayloadSchema.py
+-rw-r--r--   0        0        0      171 2024-03-21 16:01:22.632343 cognee-0.1.9/cognee/infrastructure/databases/vector/models/ScoredResult.py
+-rw-r--r--   0        0        0      143 2024-03-21 16:01:22.633028 cognee-0.1.9/cognee/infrastructure/databases/vector/models/VectorConfig.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:52:41.238226 cognee-0.1.9/cognee/infrastructure/databases/vector/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:52:41.238287 cognee-0.1.9/cognee/infrastructure/databases/vector/pinecone/__init__.py
+-rw-r--r--   0        0        0      256 2024-03-14 09:23:35.238527 cognee-0.1.9/cognee/infrastructure/databases/vector/pinecone/adapter.py
+-rw-r--r--   0        0        0     6652 2024-05-25 06:16:34.122417 cognee-0.1.9/cognee/infrastructure/databases/vector/qdrant/QDrantAdapter.py
+-rw-r--r--   0        0        0       96 2024-04-23 05:20:06.897060 cognee-0.1.9/cognee/infrastructure/databases/vector/qdrant/__init__.py
+-rw-r--r--   0        0        0     1362 2024-05-25 06:16:34.122602 cognee-0.1.9/cognee/infrastructure/databases/vector/vector_db_interface.py
+-rw-r--r--   0        0        0     4548 2024-05-25 06:16:34.122724 cognee-0.1.9/cognee/infrastructure/databases/vector/weaviate_db/WeaviateAdapter.py
+-rw-r--r--   0        0        0       45 2024-03-21 16:01:22.635439 cognee-0.1.9/cognee/infrastructure/databases/vector/weaviate_db/__init__.py
+-rw-r--r--   0        0        0      185 2024-03-14 09:23:35.239234 cognee-0.1.9/cognee/infrastructure/files/__init__.py
+-rw-r--r--   0        0        0      364 2024-03-14 09:23:35.239315 cognee-0.1.9/cognee/infrastructure/files/add_file_to_storage.py
+-rw-r--r--   0        0        0      320 2024-03-14 09:23:35.239384 cognee-0.1.9/cognee/infrastructure/files/remove_file_from_storage.py
+-rw-r--r--   0        0        0     1549 2024-05-25 06:16:34.122827 cognee-0.1.9/cognee/infrastructure/files/storage/LocalStorage.py
+-rw-r--r--   0        0        0      640 2024-03-14 09:23:35.239533 cognee-0.1.9/cognee/infrastructure/files/storage/StorageManager.py
+-rw-r--r--   0        0        0       39 2024-03-14 09:23:35.239601 cognee-0.1.9/cognee/infrastructure/files/storage/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-14 09:23:35.239635 cognee-0.1.9/cognee/infrastructure/files/utils/__init__.py
+-rw-r--r--   0        0        0      427 2024-05-26 19:03:19.274436 cognee-0.1.9/cognee/infrastructure/files/utils/extract_text_from_file.py
+-rw-r--r--   0        0        0     1001 2024-05-26 19:03:19.274786 cognee-0.1.9/cognee/infrastructure/files/utils/get_file_metadata.py
+-rw-r--r--   0        0        0      117 2024-05-26 19:03:19.275134 cognee-0.1.9/cognee/infrastructure/files/utils/get_file_size.py
+-rw-r--r--   0        0        0     1144 2024-05-26 19:03:19.286545 cognee-0.1.9/cognee/infrastructure/files/utils/guess_file_type.py
+-rw-r--r--   0        0        0      865 2024-05-26 19:03:19.286780 cognee-0.1.9/cognee/infrastructure/files/utils/is_text_content.py
+-rw-r--r--   0        0        0       35 2024-05-26 19:03:19.287399 cognee-0.1.9/cognee/infrastructure/llm/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-29 12:59:22.982620 cognee-0.1.9/cognee/infrastructure/llm/anthropic/__init__.py
+-rw-r--r--   0        0        0     1807 2024-05-25 06:16:34.123242 cognee-0.1.9/cognee/infrastructure/llm/anthropic/adapter.py
+-rw-r--r--   0        0        0      628 2024-05-27 08:14:45.232793 cognee-0.1.9/cognee/infrastructure/llm/config.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:52:41.238931 cognee-0.1.9/cognee/infrastructure/llm/generic_llm_api/__init__.py
+-rw-r--r--   0        0        0     5423 2024-05-26 19:03:19.288073 cognee-0.1.9/cognee/infrastructure/llm/generic_llm_api/adapter.py
+-rw-r--r--   0        0        0     1322 2024-05-27 08:14:45.228237 cognee-0.1.9/cognee/infrastructure/llm/get_llm_client.py
+-rw-r--r--   0        0        0      738 2024-05-26 19:03:19.289342 cognee-0.1.9/cognee/infrastructure/llm/llm_interface.py
+-rw-r--r--   0        0        0        0 2024-03-14 09:23:35.240172 cognee-0.1.9/cognee/infrastructure/llm/openai/__init__.py
+-rw-r--r--   0        0        0     5620 2024-05-27 08:14:45.263570 cognee-0.1.9/cognee/infrastructure/llm/openai/adapter.py
+-rw-r--r--   0        0        0       90 2024-03-21 16:01:22.637734 cognee-0.1.9/cognee/infrastructure/llm/prompts/__init__.py
+-rw-r--r--   0        0        0      112 2024-05-25 06:16:34.123926 cognee-0.1.9/cognee/infrastructure/llm/prompts/categorize_categories.txt
+-rw-r--r--   0        0        0      110 2024-05-25 06:16:34.124196 cognee-0.1.9/cognee/infrastructure/llm/prompts/categorize_summary.txt
+-rw-r--r--   0        0        0     5614 2024-03-29 12:59:14.138687 cognee-0.1.9/cognee/infrastructure/llm/prompts/classify_content.txt
+-rw-r--r--   0        0        0      348 2024-05-25 06:16:34.124497 cognee-0.1.9/cognee/infrastructure/llm/prompts/extract_topology.txt
+-rw-r--r--   0        0        0     1323 2024-04-23 05:20:06.898436 cognee-0.1.9/cognee/infrastructure/llm/prompts/generate_cog_layers.txt
+-rw-r--r--   0        0        0     2192 2024-04-23 05:20:06.898603 cognee-0.1.9/cognee/infrastructure/llm/prompts/generate_graph_prompt.txt
+-rw-r--r--   0        0        0      613 2024-03-21 16:01:22.638556 cognee-0.1.9/cognee/infrastructure/llm/prompts/read_query_prompt.py
+-rw-r--r--   0        0        0      962 2024-03-21 16:01:22.638746 cognee-0.1.9/cognee/infrastructure/llm/prompts/render_prompt.py
+-rw-r--r--   0        0        0       86 2024-03-21 16:01:22.639254 cognee-0.1.9/cognee/infrastructure/llm/prompts/summarize_content.txt
+-rw-r--r--   0        0        0      889 2024-03-14 09:23:35.240981 cognee-0.1.9/cognee/infrastructure/pipeline/models/Operation.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:52:41.239072 cognee-0.1.9/cognee/infrastructure/pipeline/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-14 09:23:35.241109 cognee-0.1.9/cognee/modules/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:20:06.898696 cognee-0.1.9/cognee/modules/cognify/__init__.py
+-rw-r--r--   0        0        0     1531 2024-05-26 19:03:19.290477 cognee-0.1.9/cognee/modules/cognify/config.py
+-rw-r--r--   0        0        0     3298 2024-04-23 05:20:06.898825 cognee-0.1.9/cognee/modules/cognify/dataset.py
+-rw-r--r--   0        0        0     2618 2024-05-25 06:16:34.124690 cognee-0.1.9/cognee/modules/cognify/evaluate.py
+-rw-r--r--   0        0        0        1 2024-03-14 09:23:35.241331 cognee-0.1.9/cognee/modules/cognify/graph/__init__.py
+-rw-r--r--   0        0        0     1136 2024-05-25 06:16:34.124946 cognee-0.1.9/cognee/modules/cognify/graph/add_classification_nodes.py
+-rw-r--r--   0        0        0     5209 2024-05-27 05:37:00.867184 cognee-0.1.9/cognee/modules/cognify/graph/add_cognitive_layer_graphs.py
+-rw-r--r--   0        0        0     1140 2024-05-25 06:16:34.125521 cognee-0.1.9/cognee/modules/cognify/graph/add_cognitive_layers.py
+-rw-r--r--   0        0        0     2798 2024-05-27 05:37:00.867424 cognee-0.1.9/cognee/modules/cognify/graph/add_data_chunks.py
+-rw-r--r--   0        0        0     1057 2024-05-25 06:16:34.125767 cognee-0.1.9/cognee/modules/cognify/graph/add_document_node.py
+-rw-r--r--   0        0        0     2303 2024-05-26 19:03:19.292218 cognee-0.1.9/cognee/modules/cognify/graph/add_label_nodes.py
+-rw-r--r--   0        0        0     7146 2024-05-26 19:03:19.293222 cognee-0.1.9/cognee/modules/cognify/graph/add_node_connections.py
+-rw-r--r--   0        0        0      879 2024-05-25 06:16:34.126234 cognee-0.1.9/cognee/modules/cognify/graph/add_summary_nodes.py
+-rw-r--r--   0        0        0    13112 2024-05-26 19:03:19.296197 cognee-0.1.9/cognee/modules/cognify/graph/create.py
+-rw-r--r--   0        0        0        0 2024-03-14 09:23:35.242124 cognee-0.1.9/cognee/modules/cognify/llm/__init__.py
+-rw-r--r--   0        0        0     1364 2024-05-27 05:37:00.867528 cognee-0.1.9/cognee/modules/cognify/llm/resolve_cross_graph_references.py
+-rw-r--r--   0        0        0     7185 2024-05-25 06:16:34.128123 cognee-0.1.9/cognee/modules/cognify/test.py
+-rw-r--r--   0        0        0     2667 2024-05-25 06:16:34.128231 cognee-0.1.9/cognee/modules/cognify/train.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:52:41.239641 cognee-0.1.9/cognee/modules/data/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:52:41.239714 cognee-0.1.9/cognee/modules/data/extraction/__init__.py
+-rw-r--r--   0        0        0      960 2024-04-23 05:20:06.900831 cognee-0.1.9/cognee/modules/data/extraction/extract_categories.py
+-rw-r--r--   0        0        0      490 2024-04-23 05:20:06.900898 cognee-0.1.9/cognee/modules/data/extraction/extract_cognitive_layers.py
+-rw-r--r--   0        0        0      497 2024-04-23 05:20:06.900968 cognee-0.1.9/cognee/modules/data/extraction/extract_summary.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:52:41.239777 cognee-0.1.9/cognee/modules/data/extraction/knowledge_graph/__init__.py
+-rw-r--r--   0        0        0      542 2024-04-23 05:20:06.901111 cognee-0.1.9/cognee/modules/data/extraction/knowledge_graph/extract_content_graph.py
+-rw-r--r--   0        0        0     1041 2024-05-25 06:16:34.128718 cognee-0.1.9/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph.py
+-rw-r--r--   0        0        0     4715 2024-05-25 06:16:34.128835 cognee-0.1.9/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph_module.py
+-rw-r--r--   0        0        0      699 2024-05-26 19:03:19.297517 cognee-0.1.9/cognee/modules/data/get_cognitive_layers.py
+-rw-r--r--   0        0        0      520 2024-05-26 19:03:19.298211 cognee-0.1.9/cognee/modules/data/get_content_categories.py
+-rw-r--r--   0        0        0      559 2024-05-26 19:03:19.298864 cognee-0.1.9/cognee/modules/data/get_content_summary.py
+-rw-r--r--   0        0        0     1009 2024-05-26 19:03:19.300631 cognee-0.1.9/cognee/modules/data/get_layer_graphs.py
+-rw-r--r--   0        0        0       69 2024-04-23 05:20:06.901709 cognee-0.1.9/cognee/modules/discovery/__init__.py
+-rw-r--r--   0        0        0      756 2024-04-23 05:20:06.901775 cognee-0.1.9/cognee/modules/discovery/discover_directory_datasets.py
+-rw-r--r--   0        0        0       62 2024-03-29 12:59:22.987121 cognee-0.1.9/cognee/modules/ingestion/__init__.py
+-rw-r--r--   0        0        0     1853 2024-05-26 19:03:19.301006 cognee-0.1.9/cognee/modules/ingestion/add_data_to_dataset.py
+-rw-r--r--   0        0        0      549 2024-05-25 06:16:34.128937 cognee-0.1.9/cognee/modules/ingestion/classify.py
+-rw-r--r--   0        0        0      941 2024-05-25 06:16:34.129049 cognee-0.1.9/cognee/modules/ingestion/data_types/BinaryData.py
+-rw-r--r--   0        0        0      309 2024-05-26 19:03:19.301455 cognee-0.1.9/cognee/modules/ingestion/data_types/IngestionData.py
+-rw-r--r--   0        0        0      764 2024-04-23 05:20:06.902759 cognee-0.1.9/cognee/modules/ingestion/data_types/TextData.py
+-rw-r--r--   0        0        0      145 2024-03-14 09:23:35.243502 cognee-0.1.9/cognee/modules/ingestion/data_types/__init__.py
+-rw-r--r--   0        0        0      125 2024-03-14 09:23:35.243619 cognee-0.1.9/cognee/modules/ingestion/exceptions.py
+-rw-r--r--   0        0        0      275 2024-04-23 05:20:06.902967 cognee-0.1.9/cognee/modules/ingestion/identify.py
+-rw-r--r--   0        0        0      796 2024-03-29 12:59:22.988225 cognee-0.1.9/cognee/modules/ingestion/save.py
+-rw-r--r--   0        0        0     1109 2024-04-23 05:20:06.903064 cognee-0.1.9/cognee/modules/search/CogneeSearch.py
+-rw-r--r--   0        0        0        0 2024-03-14 09:23:35.244581 cognee-0.1.9/cognee/modules/search/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-14 09:23:35.244654 cognee-0.1.9/cognee/modules/search/graph/__init__.py
+-rw-r--r--   0        0        0     2086 2024-05-26 19:03:19.301634 cognee-0.1.9/cognee/modules/search/graph/search_adjacent.py
+-rw-r--r--   0        0        0     3192 2024-05-26 19:03:19.301803 cognee-0.1.9/cognee/modules/search/graph/search_categories.py
+-rw-r--r--   0        0        0      875 2024-05-26 19:03:19.302100 cognee-0.1.9/cognee/modules/search/graph/search_cypher.py
+-rw-r--r--   0        0        0     2962 2024-05-26 19:03:19.302265 cognee-0.1.9/cognee/modules/search/graph/search_neighbour.py
+-rw-r--r--   0        0        0     2999 2024-05-26 19:03:19.302427 cognee-0.1.9/cognee/modules/search/graph/search_summary.py
+-rw-r--r--   0        0        0        0 2024-05-26 19:03:19.302457 cognee-0.1.9/cognee/modules/search/llm/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-26 19:03:19.302527 cognee-0.1.9/cognee/modules/search/llm/extraction/__init__.py
+-rw-r--r--   0        0        0      667 2024-05-25 06:16:34.130219 cognee-0.1.9/cognee/modules/search/llm/extraction/categorize_relevant_category.py
+-rw-r--r--   0        0        0      703 2024-05-25 06:16:34.130413 cognee-0.1.9/cognee/modules/search/llm/extraction/categorize_relevant_summary.py
+-rw-r--r--   0        0        0      650 2024-05-25 06:16:34.130695 cognee-0.1.9/cognee/modules/search/llm/get_relevant_summary.py
+-rw-r--r--   0        0        0        0 2024-03-14 09:23:35.244937 cognee-0.1.9/cognee/modules/search/vector/__init__.py
+-rw-r--r--   0        0        0       42 2024-05-25 06:16:34.130807 cognee-0.1.9/cognee/modules/search/vector/bm25.py
+-rw-r--r--   0        0        0       51 2024-05-25 06:16:34.130913 cognee-0.1.9/cognee/modules/search/vector/fusion.py
+-rw-r--r--   0        0        0     2047 2024-05-27 05:37:00.867637 cognee-0.1.9/cognee/modules/search/vector/search_similarity.py
+-rw-r--r--   0        0        0      141 2024-05-25 06:16:34.131198 cognee-0.1.9/cognee/modules/settings/__init__.py
+-rw-r--r--   0        0        0     2643 2024-05-27 05:37:00.867737 cognee-0.1.9/cognee/modules/settings/get_settings.py
+-rw-r--r--   0        0        0      678 2024-05-27 05:37:00.868700 cognee-0.1.9/cognee/modules/settings/save_llm_config.py
+-rw-r--r--   0        0        0      606 2024-05-27 05:37:00.868820 cognee-0.1.9/cognee/modules/settings/save_vector_db_config.py
+-rw-r--r--   0        0        0      159 2024-05-27 05:37:00.868950 cognee-0.1.9/cognee/modules/tasks/__init__.py
+-rw-r--r--   0        0        0      502 2024-05-26 19:03:19.303139 cognee-0.1.9/cognee/modules/tasks/create_task_status_table.py
+-rw-r--r--   0        0        0      632 2024-05-27 05:37:00.869016 cognee-0.1.9/cognee/modules/tasks/get_task_status.py
+-rw-r--r--   0        0        0      376 2024-05-26 19:03:19.303304 cognee-0.1.9/cognee/modules/tasks/update_task_status.py
+-rw-r--r--   0        0        0        0 2024-05-25 06:16:34.131739 cognee-0.1.9/cognee/modules/topology/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-26 19:03:19.303341 cognee-0.1.9/cognee/modules/topology/extraction/__init__.py
+-rw-r--r--   0        0        0      505 2024-05-25 06:16:34.132108 cognee-0.1.9/cognee/modules/topology/extraction/extract_topology.py
+-rw-r--r--   0        0        0      735 2024-05-26 19:03:19.303516 cognee-0.1.9/cognee/modules/topology/infer_data_topology.py
+-rw-r--r--   0        0        0     5986 2024-05-26 19:03:19.303736 cognee-0.1.9/cognee/modules/topology/topology.py
+-rw-r--r--   0        0        0        0 2024-03-14 09:23:35.245146 cognee-0.1.9/cognee/modules/users/__init__.py
+-rw-r--r--   0        0        0      179 2024-04-28 19:24:05.619936 cognee-0.1.9/cognee/modules/users/memory/__init__.py
+-rw-r--r--   0        0        0      802 2024-03-14 09:23:35.245545 cognee-0.1.9/cognee/modules/users/memory/create_information_points.py
+-rw-r--r--   0        0        0      229 2024-04-28 19:24:05.620017 cognee-0.1.9/cognee/modules/users/memory/is_existing_memory.py
+-rw-r--r--   0        0        0      203 2024-04-28 19:24:05.620093 cognee-0.1.9/cognee/modules/users/memory/register_memory_for_user.py
+-rw-r--r--   0        0        0   124245 2024-04-23 05:20:06.904069 cognee-0.1.9/cognee/programs/extract_knowledge_graph/extract_knowledge_graph.json
+-rw-r--r--   0        0        0      719 2024-05-26 19:03:19.304532 cognee-0.1.9/cognee/root_dir.py
+-rw-r--r--   0        0        0      803 2024-05-25 06:16:34.132721 cognee-0.1.9/cognee/shared/GithubClassification.py
+-rw-r--r--   0        0        0      984 2024-05-25 06:16:34.132929 cognee-0.1.9/cognee/shared/GithubTopology.py
+-rw-r--r--   0        0        0     2009 2024-05-25 06:16:34.133146 cognee-0.1.9/cognee/shared/SourceCodeGraph.py
+-rw-r--r--   0        0        0        0 2024-03-14 09:23:35.246078 cognee-0.1.9/cognee/shared/__init__.py
+-rw-r--r--   0        0        0     8940 2024-05-26 19:03:19.304823 cognee-0.1.9/cognee/shared/data_models.py
+-rw-r--r--   0        0        0      365 2024-03-21 16:01:22.651774 cognee-0.1.9/cognee/shared/encode_uuid.py
+-rw-r--r--   0        0        0       72 2024-04-29 19:00:12.026208 cognee-0.1.9/cognee/tests/Untitled.ipynb
+-rw-r--r--   0        0        0        0 2024-04-26 13:52:41.240049 cognee-0.1.9/cognee/tests/__init__.py
+-rw-r--r--   0        0        0      985 2024-04-26 13:52:41.240261 cognee-0.1.9/cognee/tests/test_data/Natural_language_processing.txt
+-rwxr-xr-x   0        0        0     6242 2024-05-26 19:03:19.305141 cognee-0.1.9/cognee/tests/test_library.py
+-rw-r--r--   0        0        0     9603 2024-05-25 06:16:34.133633 cognee-0.1.9/cognee/utils.py
+-rw-r--r--   0        0        0     3005 2024-05-27 10:10:53.126378 cognee-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     7413 1970-01-01 00:00:00.000000 cognee-0.1.9/PKG-INFO
```

### Comparing `cognee-0.1.8/LICENSE` & `cognee-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/README.md` & `cognee-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/.craft.txt` & `cognee-0.1.9/cognee/.data/example/.craft.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/.flake8.txt` & `cognee-0.1.9/cognee/.data/example/.flake8.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/.pre-commit-config.txt` & `cognee-0.1.9/cognee/.data/example/.pre-commit-config.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/CHANGELOG.txt` & `cognee-0.1.9/cognee/.data/example/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/CONTRIBUTING-aws-lambda.txt` & `cognee-0.1.9/cognee/.data/example/CONTRIBUTING-aws-lambda.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/CONTRIBUTING.txt` & `cognee-0.1.9/cognee/.data/example/CONTRIBUTING.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/LICENSE.txt` & `cognee-0.1.9/cognee/.data/example/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/Makefile.txt` & `cognee-0.1.9/cognee/.data/example/Makefile.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/README.txt` & `cognee-0.1.9/cognee/.data/example/README.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/docs/api.txt` & `cognee-0.1.9/cognee/.data/example/docs/api.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/docs/apidocs.txt` & `cognee-0.1.9/cognee/.data/example/docs/apidocs.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/docs/conf.txt` & `cognee-0.1.9/cognee/.data/example/docs/conf.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/mypy.txt` & `cognee-0.1.9/cognee/.data/example/mypy.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/pytest.txt` & `cognee-0.1.9/cognee/.data/example/pytest.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/scripts/aws-attach-layer-to-lambda-function.txt` & `cognee-0.1.9/cognee/.data/example/scripts/aws-attach-layer-to-lambda-function.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/scripts/aws-cleanup.txt` & `cognee-0.1.9/cognee/.data/example/scripts/aws-cleanup.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/scripts/aws-deploy-local-layer.txt` & `cognee-0.1.9/cognee/.data/example/scripts/aws-deploy-local-layer.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/scripts/build_aws_lambda_layer.txt` & `cognee-0.1.9/cognee/.data/example/scripts/build_aws_lambda_layer.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/scripts/bump-version.txt` & `cognee-0.1.9/cognee/.data/example/scripts/bump-version.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/scripts/init_serverless_sdk.txt` & `cognee-0.1.9/cognee/.data/example/scripts/init_serverless_sdk.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/scripts/runtox.txt` & `cognee-0.1.9/cognee/.data/example/scripts/runtox.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/scripts/split-tox-gh-actions/split-tox-gh-actions.txt` & `cognee-0.1.9/cognee/.data/example/scripts/split-tox-gh-actions/split-tox-gh-actions.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/scripts/split-tox-gh-actions/templates/base.txt` & `cognee-0.1.9/cognee/.data/example/scripts/split-tox-gh-actions/templates/base.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/scripts/split-tox-gh-actions/templates/check_permissions.txt` & `cognee-0.1.9/cognee/.data/example/scripts/split-tox-gh-actions/templates/check_permissions.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/scripts/split-tox-gh-actions/templates/check_required.txt` & `cognee-0.1.9/cognee/.data/example/scripts/split-tox-gh-actions/templates/check_required.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/scripts/split-tox-gh-actions/templates/test_group.txt` & `cognee-0.1.9/cognee/.data/example/scripts/split-tox-gh-actions/templates/test_group.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/__init__.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/__init__.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/_compat.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/_compat.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/_functools.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/_functools.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/_lru_cache.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/_lru_cache.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/_queue.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/_queue.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/_types.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/_types.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/_werkzeug.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/_werkzeug.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/api.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/api.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/attachments.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/attachments.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/client.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/client.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/consts.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/consts.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/crons/_decorator.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/crons/_decorator.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/crons/api.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/crons/api.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/crons/decorator.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/crons/decorator.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/db/explain_plan/__init__.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/db/explain_plan/__init__.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/db/explain_plan/django.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/db/explain_plan/django.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/db/explain_plan/sqlalchemy.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/db/explain_plan/sqlalchemy.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/debug.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/debug.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/envelope.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/envelope.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/hub.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/hub.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/__init__.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/__init__.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/_asgi_common.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/_asgi_common.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/_wsgi_common.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/_wsgi_common.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/aiohttp.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/aiohttp.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/argv.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/argv.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/ariadne.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/ariadne.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/arq.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/arq.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/asgi.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/asgi.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/asyncio.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/asyncio.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/asyncpg.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/asyncpg.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/atexit.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/atexit.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/aws_lambda.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/aws_lambda.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/beam.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/beam.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/boto3.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/boto3.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/bottle.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/bottle.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/celery.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/celery.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/chalice.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/chalice.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/clickhouse_driver.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/clickhouse_driver.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/cloud_resource_context.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/cloud_resource_context.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/dedupe.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/dedupe.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/django/__init__.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/django/__init__.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/django/asgi.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/django/asgi.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/django/caching.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/django/caching.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/django/middleware.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/django/middleware.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/django/signals_handlers.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/django/signals_handlers.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/django/templates.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/django/templates.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/django/transactions.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/django/transactions.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/django/views.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/django/views.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/excepthook.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/excepthook.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/executing.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/executing.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/falcon.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/falcon.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/fastapi.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/fastapi.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/flask.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/flask.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/gcp.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/gcp.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/gnu_backtrace.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/gnu_backtrace.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/gql.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/gql.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/graphene.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/graphene.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/grpc/__init__.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/grpc/__init__.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/grpc/aio/client.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/grpc/aio/client.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/grpc/aio/server.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/grpc/aio/server.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/grpc/client.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/grpc/client.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/grpc/server.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/grpc/server.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/httpx.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/httpx.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/huey.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/huey.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/logging.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/logging.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/loguru.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/loguru.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/modules.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/modules.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/openai.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/openai.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/opentelemetry/integration.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/opentelemetry/integration.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/opentelemetry/propagator.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/opentelemetry/propagator.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/opentelemetry/span_processor.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/opentelemetry/span_processor.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/pure_eval.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/pure_eval.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/pymongo.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/pymongo.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/pyramid.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/pyramid.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/quart.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/quart.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/redis/__init__.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/redis/__init__.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/redis/asyncio.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/redis/asyncio.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/rq.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/rq.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/sanic.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/sanic.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/serverless.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/serverless.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/socket.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/socket.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/spark/spark_driver.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/spark/spark_driver.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/spark/spark_worker.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/spark/spark_worker.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/sqlalchemy.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/sqlalchemy.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/starlette.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/starlette.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/starlite.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/starlite.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/stdlib.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/stdlib.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/strawberry.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/strawberry.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/threading.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/threading.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/tornado.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/tornado.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/trytond.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/trytond.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/wsgi.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/integrations/wsgi.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/metrics.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/metrics.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/monitor.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/monitor.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/profiler.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/profiler.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/scope.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/scope.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/scrubber.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/scrubber.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/serializer.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/serializer.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/session.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/session.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/sessions.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/sessions.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/spotlight.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/spotlight.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/tracing.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/tracing.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/tracing_utils.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/tracing_utils.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/tracing_utils_py2.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/tracing_utils_py2.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/tracing_utils_py3.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/tracing_utils_py3.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/transport.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/transport.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/types.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/types.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/utils.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/utils.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/sentry_sdk/worker.txt` & `cognee-0.1.9/cognee/.data/example/sentry_sdk/worker.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/setup.txt` & `cognee-0.1.9/cognee/.data/example/setup.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/conftest.txt` & `cognee-0.1.9/cognee/.data/example/tests/conftest.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/crons/test_crons.txt` & `cognee-0.1.9/cognee/.data/example/tests/crons/test_crons.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/crons/test_crons_async_py3.txt` & `cognee-0.1.9/cognee/.data/example/tests/crons/test_crons_async_py3.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/aiohttp/test_aiohttp.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/aiohttp/test_aiohttp.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/ariadne/test_ariadne.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/ariadne/test_ariadne.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/arq/test_arq.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/arq/test_arq.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/asgi/test_asgi.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/asgi/test_asgi.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/asyncio/test_asyncio_py3.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/asyncio/test_asyncio_py3.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/asyncpg/test_asyncpg.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/asyncpg/test_asyncpg.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/aws_lambda/client.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/aws_lambda/client.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/aws_lambda/test_aws.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/aws_lambda/test_aws.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/beam/test_beam.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/beam/test_beam.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/boto3/aws_mock.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/boto3/aws_mock.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/boto3/s3_list.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/boto3/s3_list.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/boto3/test_s3.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/boto3/test_s3.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/bottle/test_bottle.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/bottle/test_bottle.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/celery/test_celery.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/celery/test_celery.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/celery/test_celery_beat_crons.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/celery/test_celery_beat_crons.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/chalice/test_chalice.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/chalice/test_chalice.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/clickhouse_driver/test_clickhouse_driver.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/clickhouse_driver/test_clickhouse_driver.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/cloud_resource_context/test_cloud_resource_context.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/cloud_resource_context/test_cloud_resource_context.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/conftest.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/conftest.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/django/asgi/test_asgi.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/django/asgi/test_asgi.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/custom_urls.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/django/myapp/custom_urls.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/middleware.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/django/myapp/middleware.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/settings.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/django/myapp/settings.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/urls.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/django/myapp/urls.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/views.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/django/myapp/views.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/django/test_basic.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/django/test_basic.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/django/test_data_scrubbing.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/django/test_data_scrubbing.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/django/test_db_query_data.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/django/test_db_query_data.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/django/test_transactions.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/django/test_transactions.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/django/utils.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/django/utils.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/excepthook/test_excepthook.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/excepthook/test_excepthook.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/falcon/test_falcon.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/falcon/test_falcon.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/fastapi/test_fastapi.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/fastapi/test_fastapi.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/flask/test_flask.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/flask/test_flask.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/gcp/test_gcp.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/gcp/test_gcp.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/gql/test_gql.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/gql/test_gql.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/graphene/test_graphene_py3.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/graphene/test_graphene_py3.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/grpc/grpc_test_service_pb2.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/grpc/grpc_test_service_pb2.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/grpc/grpc_test_service_pb2_grpc.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/grpc/grpc_test_service_pb2_grpc.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/grpc/test_grpc.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/grpc/test_grpc.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/grpc/test_grpc_aio.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/grpc/test_grpc_aio.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/httpx/test_httpx.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/httpx/test_httpx.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/huey/test_huey.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/huey/test_huey.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/logging/test_logging.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/logging/test_logging.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/loguru/test_loguru.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/loguru/test_loguru.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/openai/test_openai.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/openai/test_openai.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/opentelemetry/test_experimental.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/opentelemetry/test_experimental.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/opentelemetry/test_propagator.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/opentelemetry/test_propagator.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/opentelemetry/test_span_processor.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/opentelemetry/test_span_processor.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/pure_eval/test_pure_eval.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/pure_eval/test_pure_eval.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/pymongo/test_pymongo.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/pymongo/test_pymongo.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/pyramid/test_pyramid.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/pyramid/test_pyramid.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/quart/test_quart.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/quart/test_quart.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/redis/asyncio/test_redis_asyncio.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/redis/asyncio/test_redis_asyncio.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/redis/cluster/test_redis_cluster.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/redis/cluster/test_redis_cluster.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/redis/cluster_asyncio/test_redis_cluster_asyncio.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/redis/cluster_asyncio/test_redis_cluster_asyncio.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/redis/test_redis.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/redis/test_redis.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/rediscluster/test_rediscluster.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/rediscluster/test_rediscluster.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/requests/test_requests.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/requests/test_requests.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/rq/test_rq.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/rq/test_rq.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/sanic/test_sanic.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/sanic/test_sanic.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/serverless/test_serverless.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/serverless/test_serverless.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/socket/test_socket.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/socket/test_socket.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/spark/test_spark.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/spark/test_spark.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/sqlalchemy/test_sqlalchemy.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/sqlalchemy/test_sqlalchemy.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/starlette/photo.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/starlette/photo.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/starlette/test_starlette.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/starlette/test_starlette.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/starlite/test_starlite.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/starlite/test_starlite.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/stdlib/test_httplib.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/stdlib/test_httplib.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/stdlib/test_subprocess.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/stdlib/test_subprocess.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/strawberry/test_strawberry_py3.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/strawberry/test_strawberry_py3.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/test_gnu_backtrace.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/test_gnu_backtrace.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/threading/test_threading.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/threading/test_threading.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/tornado/test_tornado.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/tornado/test_tornado.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/trytond/test_trytond.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/trytond/test_trytond.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/integrations/wsgi/test_wsgi.txt` & `cognee-0.1.9/cognee/.data/example/tests/integrations/wsgi/test_wsgi.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/test_api.txt` & `cognee-0.1.9/cognee/.data/example/tests/test_api.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/test_basics.txt` & `cognee-0.1.9/cognee/.data/example/tests/test_basics.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/test_client.txt` & `cognee-0.1.9/cognee/.data/example/tests/test_client.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/test_conftest.txt` & `cognee-0.1.9/cognee/.data/example/tests/test_conftest.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/test_envelope.txt` & `cognee-0.1.9/cognee/.data/example/tests/test_envelope.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/test_exceptiongroup.txt` & `cognee-0.1.9/cognee/.data/example/tests/test_exceptiongroup.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/test_lru_cache.txt` & `cognee-0.1.9/cognee/.data/example/tests/test_lru_cache.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/test_metrics.txt` & `cognee-0.1.9/cognee/.data/example/tests/test_metrics.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/test_monitor.txt` & `cognee-0.1.9/cognee/.data/example/tests/test_monitor.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/test_profiler.txt` & `cognee-0.1.9/cognee/.data/example/tests/test_profiler.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/test_scope.txt` & `cognee-0.1.9/cognee/.data/example/tests/test_scope.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/test_scrubber.txt` & `cognee-0.1.9/cognee/.data/example/tests/test_scrubber.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/test_serializer.txt` & `cognee-0.1.9/cognee/.data/example/tests/test_serializer.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/test_sessions.txt` & `cognee-0.1.9/cognee/.data/example/tests/test_sessions.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/test_spotlight.txt` & `cognee-0.1.9/cognee/.data/example/tests/test_spotlight.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/test_transport.txt` & `cognee-0.1.9/cognee/.data/example/tests/test_transport.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/test_types.txt` & `cognee-0.1.9/cognee/.data/example/tests/test_types.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/test_utils.txt` & `cognee-0.1.9/cognee/.data/example/tests/test_utils.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/tracing/test_baggage.txt` & `cognee-0.1.9/cognee/.data/example/tests/tracing/test_baggage.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/tracing/test_decorator_async_py3.txt` & `cognee-0.1.9/cognee/.data/example/tests/tracing/test_decorator_async_py3.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/tracing/test_decorator_sync.txt` & `cognee-0.1.9/cognee/.data/example/tests/tracing/test_decorator_sync.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/tracing/test_deprecated.txt` & `cognee-0.1.9/cognee/.data/example/tests/tracing/test_deprecated.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/tracing/test_http_headers.txt` & `cognee-0.1.9/cognee/.data/example/tests/tracing/test_http_headers.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/tracing/test_integration_tests.txt` & `cognee-0.1.9/cognee/.data/example/tests/tracing/test_integration_tests.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/tracing/test_misc.txt` & `cognee-0.1.9/cognee/.data/example/tests/tracing/test_misc.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/tracing/test_noop_span.txt` & `cognee-0.1.9/cognee/.data/example/tests/tracing/test_noop_span.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/tracing/test_sampling.txt` & `cognee-0.1.9/cognee/.data/example/tests/tracing/test_sampling.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/utils/test_contextvars.txt` & `cognee-0.1.9/cognee/.data/example/tests/utils/test_contextvars.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/utils/test_general.txt` & `cognee-0.1.9/cognee/.data/example/tests/utils/test_general.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tests/utils/test_transaction.txt` & `cognee-0.1.9/cognee/.data/example/tests/utils/test_transaction.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/example/tox.txt` & `cognee-0.1.9/cognee/.data/example/tox.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/explanations/062c22df-d99b-599f-90cd-2d325c8bcf69.txt` & `cognee-0.1.9/cognee/.data/explanations/062c22df-d99b-599f-90cd-2d325c8bcf69.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/explanations/6dfe01b6-07d2-5b77-83c8-1d6c11ce2aa7.txt` & `cognee-0.1.9/cognee/.data/explanations/6dfe01b6-07d2-5b77-83c8-1d6c11ce2aa7.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/.data/explanations/Natural language processing.txt` & `cognee-0.1.9/cognee/.data/explanations/Natural language processing.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/api/client.py` & `cognee-0.1.9/cognee/api/client.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/api/v1/add/add.py` & `cognee-0.1.9/cognee/api/v1/add/add.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/api/v1/add/add_standalone.py` & `cognee-0.1.9/cognee/api/v1/add/add_standalone.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/api/v1/add/remember.py` & `cognee-0.1.9/cognee/api/v1/add/remember.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/api/v1/cognify/cognify.py` & `cognee-0.1.9/cognee/api/v1/cognify/cognify.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,16 @@
         async with update_status_lock:
             task_status = get_task_status([dataset_name])
 
             if task_status == "DATASET_PROCESSING_STARTED":
                 logger.error(f"Dataset {dataset_name} is already being processed.")
                 return
 
-        update_task_status(dataset_name, "DATASET_PROCESSING_STARTED")
+            update_task_status(dataset_name, "DATASET_PROCESSING_STARTED")
+
         await cognify(dataset_name)
         update_task_status(dataset_name, "DATASET_PROCESSING_FINISHED")
 
     # datasets is a list of dataset names
     if isinstance(datasets, list):
         for dataset_name in datasets:
             awaitables.append(handle_cognify_task(dataset_name))
```

### Comparing `cognee-0.1.8/cognee/api/v1/cognify/tst.py` & `cognee-0.1.9/cognee/api/v1/cognify/tst.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/api/v1/config/config.py` & `cognee-0.1.9/cognee/api/v1/config/config.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/api/v1/datasets/datasets.py` & `cognee-0.1.9/cognee/api/v1/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/api/v1/prune/prune.py` & `cognee-0.1.9/cognee/api/v1/prune/prune.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,16 +12,14 @@
     @staticmethod
     async def prune_data():
         data_root_directory = base_config.data_root_directory
         LocalStorage.remove_all(data_root_directory)
 
     @staticmethod
     async def prune_system(graph = True, vector = True):
-        infra_config = infrastructure_config.get_config()
-
         if graph:
             graph_client = await get_graph_client(graph_config.graph_engine)
             await graph_client.delete_graph()
 
         if vector:
             vector_client = vector_config.vector_engine
             await vector_client.prune()
```

### Comparing `cognee-0.1.8/cognee/api/v1/search/search.py` & `cognee-0.1.9/cognee/api/v1/search/search.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/api/v1/topology/add_topology.py` & `cognee-0.1.9/cognee/api/v1/topology/add_topology.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/api/v1/topology/rrrr.py` & `cognee-0.1.9/cognee/api/v1/topology/rrrr.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/base_config.py` & `cognee-0.1.9/cognee/base_config.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/config.py` & `cognee-0.1.9/cognee/config.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/fetch_secret.py` & `cognee-0.1.9/cognee/fetch_secret.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/InfrastructureConfig.py` & `cognee-0.1.9/cognee/infrastructure/InfrastructureConfig.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/data/chunking/DefaultChunkEngine.py` & `cognee-0.1.9/cognee/infrastructure/data/chunking/DefaultChunkEngine.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/data/chunking/LangchainChunkingEngine.py` & `cognee-0.1.9/cognee/infrastructure/data/chunking/LangchainChunkingEngine.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/data/chunking/config.py` & `cognee-0.1.9/cognee/infrastructure/data/chunking/config.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/data/models/Data.py` & `cognee-0.1.9/cognee/infrastructure/data/models/Data.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/data/models/Dataset.py` & `cognee-0.1.9/cognee/infrastructure/data/models/Dataset.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/data/models/DatasetData.py` & `cognee-0.1.9/cognee/infrastructure/data/models/DatasetData.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/data/utils/extract_keywords.py` & `cognee-0.1.9/cognee/infrastructure/data/utils/extract_keywords.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/databases/graph/config.py` & `cognee-0.1.9/cognee/infrastructure/databases/graph/config.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/databases/graph/falkordb/adapter.py` & `cognee-0.1.9/cognee/infrastructure/databases/graph/falkordb/adapter.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/databases/graph/get_graph_client.py` & `cognee-0.1.9/cognee/infrastructure/databases/graph/get_graph_client.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/databases/graph/graph_db_interface.py` & `cognee-0.1.9/cognee/infrastructure/databases/graph/graph_db_interface.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/databases/graph/neo4j_driver/adapter.py` & `cognee-0.1.9/cognee/infrastructure/databases/graph/neo4j_driver/adapter.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/databases/graph/networkx/adapter.py` & `cognee-0.1.9/cognee/infrastructure/databases/graph/networkx/adapter.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/databases/relational/config.py` & `cognee-0.1.9/cognee/infrastructure/databases/relational/config.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/databases/relational/duckdb/DuckDBAdapter.py` & `cognee-0.1.9/cognee/infrastructure/databases/relational/duckdb/DuckDBAdapter.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/databases/relational/relational_db_interface.py` & `cognee-0.1.9/cognee/infrastructure/databases/relational/relational_db_interface.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/databases/relational/sqlite/SqliteEngine.py` & `cognee-0.1.9/cognee/infrastructure/databases/relational/sqlite/SqliteEngine.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/databases/relational/utils/with_rollback.py` & `cognee-0.1.9/cognee/infrastructure/databases/relational/utils/with_rollback.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/databases/vector/config.py` & `cognee-0.1.9/cognee/infrastructure/databases/vector/config.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/databases/vector/create_vector_engine.py` & `cognee-0.1.9/cognee/infrastructure/databases/vector/create_vector_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,16 @@
             return QDrantAdapter(
                 url = config["vector_db_url"],
                 api_key = config["vector_db_key"],
                 embedding_engine = embedding_engine
             )
     else:
         from .lancedb.LanceDBAdapter import LanceDBAdapter
-        from cognee.infrastructure.files.storage import LocalStorage
+        # from cognee.infrastructure.files.storage import LocalStorage
 
-        LocalStorage.ensure_directory_exists(config["vector_db_url"])
+        # LocalStorage.ensure_directory_exists(config["vector_db_url"])
 
         return LanceDBAdapter(
             url = config["vector_db_url"],
             api_key = config["vector_db_key"],
             embedding_engine = embedding_engine,
         )
```

### Comparing `cognee-0.1.8/cognee/infrastructure/databases/vector/embeddings/DefaultEmbeddingEngine.py` & `cognee-0.1.9/cognee/infrastructure/databases/vector/embeddings/DefaultEmbeddingEngine.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/databases/vector/embeddings/config.py` & `cognee-0.1.9/cognee/infrastructure/databases/vector/embeddings/config.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/databases/vector/falkordb/FalkorDBAdapter.py` & `cognee-0.1.9/cognee/infrastructure/databases/vector/falkordb/FalkorDBAdapter.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/databases/vector/lancedb/LanceDBAdapter.py` & `cognee-0.1.9/cognee/infrastructure/databases/vector/lancedb/LanceDBAdapter.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/databases/vector/qdrant/QDrantAdapter.py` & `cognee-0.1.9/cognee/infrastructure/databases/vector/qdrant/QDrantAdapter.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/databases/vector/vector_db_interface.py` & `cognee-0.1.9/cognee/infrastructure/databases/vector/vector_db_interface.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/databases/vector/weaviate_db/WeaviateAdapter.py` & `cognee-0.1.9/cognee/infrastructure/databases/vector/weaviate_db/WeaviateAdapter.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/files/storage/LocalStorage.py` & `cognee-0.1.9/cognee/infrastructure/files/storage/LocalStorage.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/files/storage/StorageManager.py` & `cognee-0.1.9/cognee/infrastructure/files/storage/StorageManager.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/files/utils/get_file_metadata.py` & `cognee-0.1.9/cognee/infrastructure/files/utils/get_file_metadata.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/files/utils/guess_file_type.py` & `cognee-0.1.9/cognee/infrastructure/files/utils/guess_file_type.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/files/utils/is_text_content.py` & `cognee-0.1.9/cognee/infrastructure/files/utils/is_text_content.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/llm/anthropic/adapter.py` & `cognee-0.1.9/cognee/infrastructure/llm/anthropic/adapter.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/llm/config.py` & `cognee-0.1.9/cognee/infrastructure/llm/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from pydantic_settings import BaseSettings, SettingsConfigDict
 
 class LLMConfig(BaseSettings):
     llm_provider: str = "openai"
     llm_model: str = "gpt-4o"
     llm_endpoint: str = ""
     llm_api_key: str = ""
+    llm_streaming:bool = False
 
     model_config = SettingsConfigDict(env_file = ".env", extra = "allow")
 
     def to_dict(self) -> dict:
         return {
             "provider": self.llm_provider,
             "model": self.llm_model,
```

### Comparing `cognee-0.1.8/cognee/infrastructure/llm/generic_llm_api/adapter.py` & `cognee-0.1.9/cognee/infrastructure/llm/generic_llm_api/adapter.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/llm/get_llm_client.py` & `cognee-0.1.9/cognee/infrastructure/llm/get_llm_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     """Get the LLM client based on the configuration using Enums."""
     llm_config = get_llm_config()
 
     provider = LLMProvider(llm_config.llm_provider)
 
     if provider == LLMProvider.OPENAI:
         from .openai.adapter import OpenAIAdapter
-        return OpenAIAdapter(llm_config.llm_api_key, llm_config.llm_model)
+        return OpenAIAdapter(llm_config.llm_api_key, llm_config.llm_model, llm_config.llm_streaming)
     elif provider == LLMProvider.OLLAMA:
         from .generic_llm_api.adapter import GenericAPIAdapter
         return GenericAPIAdapter(llm_config.llm_endpoint, llm_config.llm_api_key, llm_config.llm_model, "Ollama")
     elif provider == LLMProvider.ANTHROPIC:
         from .anthropic.adapter import AnthropicAdapter
         return AnthropicAdapter(llm_config.llm_model)
     elif provider == LLMProvider.CUSTOM:
```

### Comparing `cognee-0.1.8/cognee/infrastructure/llm/llm_interface.py` & `cognee-0.1.9/cognee/infrastructure/llm/llm_interface.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/llm/openai/adapter.py` & `cognee-0.1.9/cognee/infrastructure/llm/openai/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,20 +28,20 @@
 
 class OpenAIAdapter(LLMInterface):
     name = "OpenAI"
     model: str
     api_key: str
   
     """Adapter for OpenAI's GPT-3, GPT=4 API"""
-    def __init__(self, api_key: str, model:str):
+    def __init__(self, api_key: str, model:str, streaming:bool = False):
         self.aclient = instructor.from_openai(AsyncOpenAI(api_key = api_key))
         self.client = instructor.from_openai(OpenAI(api_key = api_key))
         self.model = model
         self.api_key = api_key
-
+        self.streaming = streaming
     @retry(stop = stop_after_attempt(5))
     def completions_with_backoff(self, **kwargs):
         """Wrapper around ChatCompletion.create w/ backoff"""
         return openai.chat.completions.create(**kwargs)
 
     @retry(stop = stop_after_attempt(5))
     async def acompletions_with_backoff(self,**kwargs):
```

### Comparing `cognee-0.1.8/cognee/infrastructure/llm/prompts/classify_content.txt` & `cognee-0.1.9/cognee/infrastructure/llm/prompts/classify_content.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/llm/prompts/generate_cog_layers.txt` & `cognee-0.1.9/cognee/infrastructure/llm/prompts/generate_cog_layers.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/llm/prompts/generate_graph_prompt.txt` & `cognee-0.1.9/cognee/infrastructure/llm/prompts/generate_graph_prompt.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/llm/prompts/read_query_prompt.py` & `cognee-0.1.9/cognee/infrastructure/llm/prompts/read_query_prompt.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/llm/prompts/render_prompt.py` & `cognee-0.1.9/cognee/infrastructure/llm/prompts/render_prompt.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/infrastructure/pipeline/models/Operation.py` & `cognee-0.1.9/cognee/infrastructure/pipeline/models/Operation.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/cognify/config.py` & `cognee-0.1.9/cognee/modules/cognify/config.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/cognify/dataset.py` & `cognee-0.1.9/cognee/modules/cognify/dataset.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/cognify/evaluate.py` & `cognee-0.1.9/cognee/modules/cognify/evaluate.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/cognify/graph/add_classification_nodes.py` & `cognee-0.1.9/cognee/modules/cognify/graph/add_classification_nodes.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/cognify/graph/add_cognitive_layer_graphs.py` & `cognee-0.1.9/cognee/modules/cognify/graph/add_cognitive_layer_graphs.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/cognify/graph/add_cognitive_layers.py` & `cognee-0.1.9/cognee/modules/cognify/graph/add_cognitive_layers.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/cognify/graph/add_data_chunks.py` & `cognee-0.1.9/cognee/modules/cognify/graph/add_data_chunks.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/cognify/graph/add_document_node.py` & `cognee-0.1.9/cognee/modules/cognify/graph/add_document_node.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/cognify/graph/add_label_nodes.py` & `cognee-0.1.9/cognee/modules/cognify/graph/add_label_nodes.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/cognify/graph/add_node_connections.py` & `cognee-0.1.9/cognee/modules/cognify/graph/add_node_connections.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/cognify/graph/add_summary_nodes.py` & `cognee-0.1.9/cognee/modules/cognify/graph/add_summary_nodes.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/cognify/graph/create.py` & `cognee-0.1.9/cognee/modules/cognify/graph/create.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/cognify/llm/resolve_cross_graph_references.py` & `cognee-0.1.9/cognee/modules/cognify/llm/resolve_cross_graph_references.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/cognify/test.py` & `cognee-0.1.9/cognee/modules/cognify/test.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/cognify/train.py` & `cognee-0.1.9/cognee/modules/cognify/train.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/data/extraction/extract_categories.py` & `cognee-0.1.9/cognee/modules/data/extraction/extract_categories.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/data/extraction/knowledge_graph/extract_content_graph.py` & `cognee-0.1.9/cognee/modules/data/extraction/knowledge_graph/extract_content_graph.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph.py` & `cognee-0.1.9/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph_module.py` & `cognee-0.1.9/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph_module.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/data/get_cognitive_layers.py` & `cognee-0.1.9/cognee/modules/data/get_cognitive_layers.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/data/get_content_categories.py` & `cognee-0.1.9/cognee/modules/data/get_content_categories.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/data/get_content_summary.py` & `cognee-0.1.9/cognee/modules/data/get_content_summary.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/data/get_layer_graphs.py` & `cognee-0.1.9/cognee/modules/data/get_layer_graphs.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/discovery/discover_directory_datasets.py` & `cognee-0.1.9/cognee/modules/discovery/discover_directory_datasets.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/ingestion/add_data_to_dataset.py` & `cognee-0.1.9/cognee/modules/ingestion/add_data_to_dataset.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/ingestion/classify.py` & `cognee-0.1.9/cognee/modules/ingestion/classify.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/ingestion/data_types/BinaryData.py` & `cognee-0.1.9/cognee/modules/ingestion/data_types/BinaryData.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/ingestion/data_types/TextData.py` & `cognee-0.1.9/cognee/modules/ingestion/data_types/TextData.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/ingestion/save.py` & `cognee-0.1.9/cognee/modules/ingestion/save.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/search/CogneeSearch.py` & `cognee-0.1.9/cognee/modules/search/CogneeSearch.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/search/graph/search_adjacent.py` & `cognee-0.1.9/cognee/modules/search/graph/search_adjacent.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/search/graph/search_categories.py` & `cognee-0.1.9/cognee/modules/search/graph/search_categories.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/search/graph/search_cypher.py` & `cognee-0.1.9/cognee/modules/search/graph/search_cypher.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/search/graph/search_neighbour.py` & `cognee-0.1.9/cognee/modules/search/graph/search_neighbour.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/search/graph/search_summary.py` & `cognee-0.1.9/cognee/modules/search/graph/search_summary.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/search/llm/extraction/categorize_relevant_category.py` & `cognee-0.1.9/cognee/modules/search/llm/extraction/categorize_relevant_category.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/search/llm/extraction/categorize_relevant_summary.py` & `cognee-0.1.9/cognee/modules/search/llm/extraction/categorize_relevant_summary.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/search/llm/get_relevant_summary.py` & `cognee-0.1.9/cognee/modules/search/llm/get_relevant_summary.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/search/vector/search_similarity.py` & `cognee-0.1.9/cognee/modules/search/vector/search_similarity.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/settings/get_settings.py` & `cognee-0.1.9/cognee/modules/settings/get_settings.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/settings/save_llm_config.py` & `cognee-0.1.9/cognee/modules/settings/save_llm_config.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/settings/save_vector_db_config.py` & `cognee-0.1.9/cognee/modules/settings/save_vector_db_config.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/tasks/get_task_status.py` & `cognee-0.1.9/cognee/modules/tasks/get_task_status.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/topology/infer_data_topology.py` & `cognee-0.1.9/cognee/modules/topology/infer_data_topology.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/topology/topology.py` & `cognee-0.1.9/cognee/modules/topology/topology.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/modules/users/memory/create_information_points.py` & `cognee-0.1.9/cognee/modules/users/memory/create_information_points.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/programs/extract_knowledge_graph/extract_knowledge_graph.json` & `cognee-0.1.9/cognee/programs/extract_knowledge_graph/extract_knowledge_graph.json`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/root_dir.py` & `cognee-0.1.9/cognee/root_dir.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/shared/GithubClassification.py` & `cognee-0.1.9/cognee/shared/GithubClassification.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/shared/GithubTopology.py` & `cognee-0.1.9/cognee/shared/GithubTopology.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/shared/SourceCodeGraph.py` & `cognee-0.1.9/cognee/shared/SourceCodeGraph.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/shared/data_models.py` & `cognee-0.1.9/cognee/shared/data_models.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/tests/test_data/Natural_language_processing.txt` & `cognee-0.1.9/cognee/.data/main/Natural_language_processing.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/tests/test_library.py` & `cognee-0.1.9/cognee/tests/test_library.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/cognee/utils.py` & `cognee-0.1.9/cognee/utils.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.8/pyproject.toml` & `cognee-0.1.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognee"
-version = "0.1.8"
+version = "0.1.9"
 description = "Cognee - is a library for enriching LLM context with a semantic layer for better understanding and reasoning."
 authors = ["Vasilije Markovic", "Boris Arzentar"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://www.cognee.ai"
 repository = "https://github.com/topoteretes/cognee"
 classifiers = [
@@ -46,16 +46,15 @@
 duckdb-engine = "^0.11.2"
 graphistry = "^0.33.5"
 tenacity = "^8.2.3"
 weaviate-client = "^4.5.4"
 scikit-learn = "^1.4.1.post1"
 fastembed = "^0.2.5"
 pypdf = "^4.1.0"
-anthropic = "^0.21.3"
-neo4j = "^5.18.0"
+neo4j = "5.20.0"
 jinja2 = "^3.1.3"
 matplotlib = "^3.8.3"
 nest-asyncio = "^1.6.0"
 structlog = "^24.1.0"
 tiktoken = "^0.6.0"
 dspy-ai = "2.4.3"
 posthog = "^3.5.0"
@@ -65,17 +64,17 @@
 groq = "^0.5.0"
 tantivy = "^0.21.0"
 python-multipart = "^0.0.9"
 langfuse = "^2.32.0"
 spacy = "^3.7.4"
 protobuf = "<5.0.0"
 langchain-community = "0.0.38"
-deepeval = "^0.21.42"
 falkordb = "^1.0.4"
 pydantic-settings = "^2.2.1"
+anthropic = "^0.26.1"
 
 
 [tool.poetry.extras]
 parquet = ["pyarrow"]
 duckdb = ["duckdb"]
 filesystem = ["s3fs", "botocore"]
 motherduck = ["duckdb", "pyarrow"]
```

### Comparing `cognee-0.1.8/PKG-INFO` & `cognee-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognee
-Version: 0.1.8
+Version: 0.1.9
 Summary: Cognee - is a library for enriching LLM context with a semantic layer for better understanding and reasoning.
 Home-page: https://www.cognee.ai
 License: Apache-2.0
 Author: Vasilije Markovic
 Requires-Python: >=3.9.0,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -24,18 +24,17 @@
 Provides-Extra: neo4j
 Provides-Extra: notebook
 Provides-Extra: parquet
 Provides-Extra: qdrant
 Provides-Extra: weaviate
 Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
 Requires-Dist: aiosqlite (>=0.20.0,<0.21.0)
-Requires-Dist: anthropic (>=0.21.3,<0.22.0)
+Requires-Dist: anthropic (>=0.26.1,<0.27.0)
 Requires-Dist: boto3 (>=1.26.125,<2.0.0)
 Requires-Dist: debugpy (>=1.8.0,<2.0.0)
-Requires-Dist: deepeval (>=0.21.42,<0.22.0)
 Requires-Dist: dlt (==0.4.10)
 Requires-Dist: dspy-ai (==2.4.3)
 Requires-Dist: duckdb-engine (>=0.11.2,<0.12.0)
 Requires-Dist: duckdb[dlt] (>=0.10.0,<0.11.0) ; extra == "duckdb" or extra == "motherduck"
 Requires-Dist: falkordb (>=1.0.4,<2.0.0)
 Requires-Dist: fastapi (>=0.109.2,<0.110.0)
 Requires-Dist: fastembed (>=0.2.5,<0.3.0)
@@ -48,15 +47,15 @@
 Requires-Dist: instructor (==1.2.1)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: lancedb (>=0.6.10,<0.7.0)
 Requires-Dist: langchain-community (==0.0.38)
 Requires-Dist: langfuse (>=2.32.0,<3.0.0)
 Requires-Dist: litellm (>=1.37.3,<2.0.0)
 Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
-Requires-Dist: neo4j (>=5.18.0,<6.0.0) ; extra == "neo4j"
+Requires-Dist: neo4j (==5.20.0) ; extra == "neo4j"
 Requires-Dist: nest-asyncio (>=1.6.0,<2.0.0)
 Requires-Dist: networkx (>=3.2.1,<4.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: openai (==1.14.3)
 Requires-Dist: overrides (>=7.7.0,<8.0.0) ; extra == "notebook"
 Requires-Dist: pandas (>=2.2.0,<3.0.0)
 Requires-Dist: posthog (>=3.5.0,<4.0.0)
```

#### html2text {}

```diff
@@ -1,37 +1,36 @@
-Metadata-Version: 2.1 Name: cognee Version: 0.1.8 Summary: Cognee - is a
+Metadata-Version: 2.1 Name: cognee Version: 0.1.9 Summary: Cognee - is a
 library for enriching LLM context with a semantic layer for better
 understanding and reasoning. Home-page: https://www.cognee.ai License: Apache-
 2.0 Author: Vasilije Markovic Requires-Python: >=3.9.0,<3.12 Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
 :: Windows Classifier: Operating System :: POSIX :: Linux Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Topic :: Software
 Development :: Libraries Provides-Extra: cli Provides-Extra: duckdb Provides-
 Extra: filesystem Provides-Extra: motherduck Provides-Extra: neo4j Provides-
 Extra: notebook Provides-Extra: parquet Provides-Extra: qdrant Provides-Extra:
 weaviate Requires-Dist: aiofiles (>=23.2.1,<24.0.0) Requires-Dist: aiosqlite
-(>=0.20.0,<0.21.0) Requires-Dist: anthropic (>=0.21.3,<0.22.0) Requires-Dist:
+(>=0.20.0,<0.21.0) Requires-Dist: anthropic (>=0.26.1,<0.27.0) Requires-Dist:
 boto3 (>=1.26.125,<2.0.0) Requires-Dist: debugpy (>=1.8.0,<2.0.0) Requires-
-Dist: deepeval (>=0.21.42,<0.22.0) Requires-Dist: dlt (==0.4.10) Requires-Dist:
-dspy-ai (==2.4.3) Requires-Dist: duckdb-engine (>=0.11.2,<0.12.0) Requires-
-Dist: duckdb[dlt] (>=0.10.0,<0.11.0) ; extra == "duckdb" or extra ==
-"motherduck" Requires-Dist: falkordb (>=1.0.4,<2.0.0) Requires-Dist: fastapi
-(>=0.109.2,<0.110.0) Requires-Dist: fastembed (>=0.2.5,<0.3.0) Requires-Dist:
-filetype (>=1.2.0,<2.0.0) Requires-Dist: graphistry (>=0.33.5,<0.34.0)
-Requires-Dist: greenlet (>=3.0.3,<4.0.0) Requires-Dist: groq (>=0.5.0,<0.6.0)
-Requires-Dist: gunicorn (>=20.1.0,<21.0.0) Requires-Dist: importlib-metadata
-(==6.8.0) Requires-Dist: instructor (==1.2.1) Requires-Dist: jinja2
-(>=3.1.3,<4.0.0) Requires-Dist: lancedb (>=0.6.10,<0.7.0) Requires-Dist:
-langchain-community (==0.0.38) Requires-Dist: langfuse (>=2.32.0,<3.0.0)
-Requires-Dist: litellm (>=1.37.3,<2.0.0) Requires-Dist: matplotlib
-(>=3.8.3,<4.0.0) Requires-Dist: neo4j (>=5.18.0,<6.0.0) ; extra == "neo4j"
+Dist: dlt (==0.4.10) Requires-Dist: dspy-ai (==2.4.3) Requires-Dist: duckdb-
+engine (>=0.11.2,<0.12.0) Requires-Dist: duckdb[dlt] (>=0.10.0,<0.11.0) ; extra
+== "duckdb" or extra == "motherduck" Requires-Dist: falkordb (>=1.0.4,<2.0.0)
+Requires-Dist: fastapi (>=0.109.2,<0.110.0) Requires-Dist: fastembed
+(>=0.2.5,<0.3.0) Requires-Dist: filetype (>=1.2.0,<2.0.0) Requires-Dist:
+graphistry (>=0.33.5,<0.34.0) Requires-Dist: greenlet (>=3.0.3,<4.0.0)
+Requires-Dist: groq (>=0.5.0,<0.6.0) Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
+Requires-Dist: importlib-metadata (==6.8.0) Requires-Dist: instructor (==1.2.1)
+Requires-Dist: jinja2 (>=3.1.3,<4.0.0) Requires-Dist: lancedb (>=0.6.10,<0.7.0)
+Requires-Dist: langchain-community (==0.0.38) Requires-Dist: langfuse
+(>=2.32.0,<3.0.0) Requires-Dist: litellm (>=1.37.3,<2.0.0) Requires-Dist:
+matplotlib (>=3.8.3,<4.0.0) Requires-Dist: neo4j (==5.20.0) ; extra == "neo4j"
 Requires-Dist: nest-asyncio (>=1.6.0,<2.0.0) Requires-Dist: networkx
 (>=3.2.1,<4.0.0) Requires-Dist: nltk (>=3.8.1,<4.0.0) Requires-Dist: openai
 (==1.14.3) Requires-Dist: overrides (>=7.7.0,<8.0.0) ; extra == "notebook"
 Requires-Dist: pandas (>=2.2.0,<3.0.0) Requires-Dist: posthog (>=3.5.0,<4.0.0)
 Requires-Dist: protobuf (<5.0.0) Requires-Dist: pyarrow (>=15.0.0,<16.0.0) ;
 extra == "parquet" or extra == "motherduck" Requires-Dist: pydantic
 (>=2.5.0,<3.0.0) Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0) Requires-
```

