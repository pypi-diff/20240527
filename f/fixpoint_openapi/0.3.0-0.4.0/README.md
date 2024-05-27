# Comparing `tmp/fixpoint_openapi-0.3.0.tar.gz` & `tmp/fixpoint_openapi-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixpoint_openapi-0.3.0.tar", max compression
+gzip compressed data, was "fixpoint_openapi-0.4.0.tar", max compression
```

## Comparing `fixpoint_openapi-0.3.0.tar` & `fixpoint_openapi-0.4.0.tar`

### file list

```diff
@@ -1,80 +1,99 @@
--rw-r--r--   0        0        0    11338 2024-04-21 21:28:48.772887 fixpoint_openapi-0.3.0/LICENSE
--rw-r--r--   0        0        0     9316 2024-04-21 21:28:48.772887 fixpoint_openapi-0.3.0/README.md
--rw-r--r--   0        0        0     6363 2024-04-21 21:28:48.772887 fixpoint_openapi-0.3.0/fixpoint_openapi/__init__.py
--rw-r--r--   0        0        0      106 2024-04-21 21:28:48.772887 fixpoint_openapi-0.3.0/fixpoint_openapi/api/__init__.py
--rw-r--r--   0        0        0   213297 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/api/fixpoint_api.py
--rw-r--r--   0        0        0    25831 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/api_client.py
--rw-r--r--   0        0        0      652 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/api_response.py
--rw-r--r--   0        0        0    14504 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/configuration.py
--rw-r--r--   0        0        0     6000 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/exceptions.py
--rw-r--r--   0        0        0     5743 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/__init__.py
--rw-r--r--   0        0        0      858 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/app_log_level_type.py
--rw-r--r--   0        0        0     4657 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/fixpoint_create_open_ai_chat_input_log_request.py
--rw-r--r--   0        0        0     4385 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/fixpoint_create_open_ai_chat_output_log_request.py
--rw-r--r--   0        0        0     2654 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/fixpoint_post_dataset_logs_request.py
--rw-r--r--   0        0        0     3208 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/fixpoint_update_spending_totals_request.py
--rw-r--r--   0        0        0     3534 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/fixpointv1_model.py
--rw-r--r--   0        0        0     3150 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/protobuf_any.py
--rw-r--r--   0        0        0      940 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/protobuf_null_value.py
--rw-r--r--   0        0        0     3164 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/rpc_status.py
--rw-r--r--   0        0        0     2768 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/tool_call_function.py
--rw-r--r--   0        0        0     3215 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_api_secret.py
--rw-r--r--   0        0        0      888 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_api_secret_provider.py
--rw-r--r--   0        0        0     3252 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_app_log.py
--rw-r--r--   0        0        0     2645 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_attribute_filters.py
--rw-r--r--   0        0        0     4316 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_chat_completion.py
--rw-r--r--   0        0        0     3118 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_chat_completion_choice.py
--rw-r--r--   0        0        0     2951 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_chat_completion_usage.py
--rw-r--r--   0        0        0     2958 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_create_api_secret_request.py
--rw-r--r--   0        0        0     3050 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_create_app_logs_request.py
--rw-r--r--   0        0        0     2577 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_create_app_logs_response.py
--rw-r--r--   0        0        0     2999 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_create_dataset_request.py
--rw-r--r--   0        0        0     2847 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_create_dataset_response.py
--rw-r--r--   0        0        0     2997 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_create_likes_request.py
--rw-r--r--   0        0        0     2569 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_create_likes_response.py
--rw-r--r--   0        0        0     2977 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_create_log_attribute_request.py
--rw-r--r--   0        0        0     2981 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_create_log_attribute_response.py
--rw-r--r--   0        0        0     5310 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_create_multi_llm_chat_completion_request.py
--rw-r--r--   0        0        0     3556 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_create_multi_llm_chat_completion_request_model.py
--rw-r--r--   0        0        0     3667 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_create_routing_config_request.py
--rw-r--r--   0        0        0     3073 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_dataset.py
--rw-r--r--   0        0        0     2618 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_dataset_filters.py
--rw-r--r--   0        0        0     2597 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_delete_log_attribute_response.py
--rw-r--r--   0        0        0      873 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_fallback_strategy.py
--rw-r--r--   0        0        0     2621 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_input_message.py
--rw-r--r--   0        0        0     3369 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_like.py
--rw-r--r--   0        0        0     2674 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_like_filter.py
--rw-r--r--   0        0        0     3091 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_like_ingest.py
--rw-r--r--   0        0        0     3100 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_list_api_secrets_response.py
--rw-r--r--   0        0        0     3046 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_list_app_logs_response.py
--rw-r--r--   0        0        0     3019 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_list_datasets_response.py
--rw-r--r--   0        0        0     2968 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_list_likes_response.py
--rw-r--r--   0        0        0     3154 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_list_log_attributes_response.py
--rw-r--r--   0        0        0     3596 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_list_open_ai_chat_logs_response.py
--rw-r--r--   0        0        0     3341 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_list_routing_configs_response.py
--rw-r--r--   0        0        0     3144 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_log_attribute.py
--rw-r--r--   0        0        0      847 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_mode.py
--rw-r--r--   0        0        0     4484 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_multi_llm_chat_completion.py
--rw-r--r--   0        0        0     3973 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_open_ai_chat_input_log.py
--rw-r--r--   0        0        0     4674 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_open_ai_chat_log.py
--rw-r--r--   0        0        0     5221 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_open_ai_chat_logs_filters.py
--rw-r--r--   0        0        0     4564 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_open_ai_chat_output_log.py
--rw-r--r--   0        0        0     3144 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_open_ai_chat_output_log_choice.py
--rw-r--r--   0        0        0     2971 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_open_ai_chat_output_log_usage.py
--rw-r--r--   0        0        0      863 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_origin_type.py
--rw-r--r--   0        0        0     3431 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_output_message.py
--rw-r--r--   0        0        0     2585 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_post_dataset_logs_response.py
--rw-r--r--   0        0        0     2613 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_relative_date_time_filters.py
--rw-r--r--   0        0        0      960 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_reset_interval.py
--rw-r--r--   0        0        0     3991 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_routing_config.py
--rw-r--r--   0        0        0     2857 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_spend_cap.py
--rw-r--r--   0        0        0     1074 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_terminal_state.py
--rw-r--r--   0        0        0      851 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_thumbs_reaction.py
--rw-r--r--   0        0        0     3000 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_tool_call.py
--rw-r--r--   0        0        0     3537 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_tracing.py
--rw-r--r--   0        0        0     3525 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_tracing_filters.py
--rw-r--r--   0        0        0     2971 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_usage_totals.py
--rw-r--r--   0        0        0        0 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/py.typed
--rw-r--r--   0        0        0     9262 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/fixpoint_openapi/rest.py
--rw-r--r--   0        0        0     2157 2024-04-21 21:28:48.776887 fixpoint_openapi-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    10377 1970-01-01 00:00:00.000000 fixpoint_openapi-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11338 2024-05-27 15:08:16.302734 fixpoint_openapi-0.4.0/LICENSE
+-rw-r--r--   0        0        0    11028 2024-05-27 15:08:16.302734 fixpoint_openapi-0.4.0/README.md
+-rw-r--r--   0        0        0     7694 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/__init__.py
+-rw-r--r--   0        0        0      106 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/api/__init__.py
+-rw-r--r--   0        0        0   268495 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/api/fixpoint_api.py
+-rw-r--r--   0        0        0    25831 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/api_client.py
+-rw-r--r--   0        0        0      652 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/api_response.py
+-rw-r--r--   0        0        0    14504 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/configuration.py
+-rw-r--r--   0        0        0     6000 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/exceptions.py
+-rw-r--r--   0        0        0     7074 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/__init__.py
+-rw-r--r--   0        0        0      858 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/app_log_level_type.py
+-rw-r--r--   0        0        0     2672 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/fixpoint_batch_delete_dataset_logs_request.py
+-rw-r--r--   0        0        0     4657 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/fixpoint_create_open_ai_chat_input_log_request.py
+-rw-r--r--   0        0        0     4385 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/fixpoint_create_open_ai_chat_output_log_request.py
+-rw-r--r--   0        0        0     2654 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/fixpoint_post_dataset_logs_request.py
+-rw-r--r--   0        0        0     3210 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/fixpoint_update_spending_totals_request.py
+-rw-r--r--   0        0        0     3534 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/fixpointv1_model.py
+-rw-r--r--   0        0        0     2889 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/fixpointv1_spend_cap.py
+-rw-r--r--   0        0        0     3150 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/protobuf_any.py
+-rw-r--r--   0        0        0      940 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/protobuf_null_value.py
+-rw-r--r--   0        0        0     3131 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/routing_block_ab.py
+-rw-r--r--   0        0        0     3164 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/rpc_status.py
+-rw-r--r--   0        0        0     2768 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/tool_call_function.py
+-rw-r--r--   0        0        0     4138 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_ab_chat_completion.py
+-rw-r--r--   0        0        0     3215 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_api_secret.py
+-rw-r--r--   0        0        0      888 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_api_secret_provider.py
+-rw-r--r--   0        0        0     3252 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_app_log.py
+-rw-r--r--   0        0        0     2645 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_attribute_filters.py
+-rw-r--r--   0        0        0     3480 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_batch_create_fine_tune_jobs_request.py
+-rw-r--r--   0        0        0     3169 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_batch_create_fine_tune_jobs_response.py
+-rw-r--r--   0        0        0     4316 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_chat_completion.py
+-rw-r--r--   0        0        0     3118 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_chat_completion_choice.py
+-rw-r--r--   0        0        0     2951 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_chat_completion_usage.py
+-rw-r--r--   0        0        0     5292 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_create_ab_chat_completion_request.py
+-rw-r--r--   0        0        0     2958 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_create_api_secret_request.py
+-rw-r--r--   0        0        0     3050 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_create_app_logs_request.py
+-rw-r--r--   0        0        0     2577 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_create_app_logs_response.py
+-rw-r--r--   0        0        0     2999 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_create_dataset_request.py
+-rw-r--r--   0        0        0     2847 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_create_dataset_response.py
+-rw-r--r--   0        0        0     2997 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_create_likes_request.py
+-rw-r--r--   0        0        0     2569 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_create_likes_response.py
+-rw-r--r--   0        0        0     2977 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_create_log_attribute_request.py
+-rw-r--r--   0        0        0     2981 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_create_log_attribute_response.py
+-rw-r--r--   0        0        0     5580 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_create_multi_llm_chat_completion_request.py
+-rw-r--r--   0        0        0     3556 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_create_multi_llm_chat_completion_request_model.py
+-rw-r--r--   0        0        0     4225 2024-05-27 15:08:16.306733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_create_routing_config_request.py
+-rw-r--r--   0        0        0     3073 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_dataset.py
+-rw-r--r--   0        0        0     2618 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_dataset_filters.py
+-rw-r--r--   0        0        0     2641 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_delete_dataset_logs_response.py
+-rw-r--r--   0        0        0     2625 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_delete_dataset_response.py
+-rw-r--r--   0        0        0     2597 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_delete_log_attribute_response.py
+-rw-r--r--   0        0        0      873 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_fallback_strategy.py
+-rw-r--r--   0        0        0     4596 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_fine_tune_job.py
+-rw-r--r--   0        0        0     1181 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_fine_tune_status.py
+-rw-r--r--   0        0        0     2547 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_hyperparameters.py
+-rw-r--r--   0        0        0     2621 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_input_message.py
+-rw-r--r--   0        0        0     3369 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_like.py
+-rw-r--r--   0        0        0     2674 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_like_filter.py
+-rw-r--r--   0        0        0     3091 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_like_ingest.py
+-rw-r--r--   0        0        0     3100 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_list_api_secrets_response.py
+-rw-r--r--   0        0        0     3046 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_list_app_logs_response.py
+-rw-r--r--   0        0        0     3019 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_list_datasets_response.py
+-rw-r--r--   0        0        0     3141 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_list_fine_tune_jobs_response.py
+-rw-r--r--   0        0        0     2968 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_list_likes_response.py
+-rw-r--r--   0        0        0     3154 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_list_log_attributes_response.py
+-rw-r--r--   0        0        0     3596 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_list_open_ai_chat_logs_response.py
+-rw-r--r--   0        0        0     3341 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_list_routing_configs_response.py
+-rw-r--r--   0        0        0     3144 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_log_attribute.py
+-rw-r--r--   0        0        0      847 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_mode.py
+-rw-r--r--   0        0        0     3392 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_model.py
+-rw-r--r--   0        0        0     4696 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_multi_llm_chat_completion.py
+-rw-r--r--   0        0        0     3973 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_open_ai_chat_input_log.py
+-rw-r--r--   0        0        0     4674 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_open_ai_chat_log.py
+-rw-r--r--   0        0        0     5221 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_open_ai_chat_logs_filters.py
+-rw-r--r--   0        0        0     4564 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_open_ai_chat_output_log.py
+-rw-r--r--   0        0        0     3144 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_open_ai_chat_output_log_choice.py
+-rw-r--r--   0        0        0     2971 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_open_ai_chat_output_log_usage.py
+-rw-r--r--   0        0        0      863 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_origin_type.py
+-rw-r--r--   0        0        0     3431 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_output_message.py
+-rw-r--r--   0        0        0     2585 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_post_dataset_logs_response.py
+-rw-r--r--   0        0        0     2613 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_relative_date_time_filters.py
+-rw-r--r--   0        0        0      960 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_reset_interval.py
+-rw-r--r--   0        0        0     3440 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_routing_block.py
+-rw-r--r--   0        0        0     3524 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_routing_block_spend_cap.py
+-rw-r--r--   0        0        0      939 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_routing_block_type.py
+-rw-r--r--   0        0        0     4549 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_routing_config.py
+-rw-r--r--   0        0        0     2857 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_spend_cap.py
+-rw-r--r--   0        0        0     3566 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_spend_cap_model.py
+-rw-r--r--   0        0        0     1074 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_terminal_state.py
+-rw-r--r--   0        0        0      851 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_thumbs_reaction.py
+-rw-r--r--   0        0        0     3000 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_tool_call.py
+-rw-r--r--   0        0        0     3537 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_tracing.py
+-rw-r--r--   0        0        0     3525 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_tracing_filters.py
+-rw-r--r--   0        0        0     3245 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_tuning_configuration.py
+-rw-r--r--   0        0        0     2971 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_usage_totals.py
+-rw-r--r--   0        0        0        0 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/py.typed
+-rw-r--r--   0        0        0     9262 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/fixpoint_openapi/rest.py
+-rw-r--r--   0        0        0     2157 2024-05-27 15:08:16.310733 fixpoint_openapi-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    12089 1970-01-01 00:00:00.000000 fixpoint_openapi-0.4.0/PKG-INFO
```

### Comparing `fixpoint_openapi-0.3.0/LICENSE` & `fixpoint_openapi-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/README.md` & `fixpoint_openapi-0.4.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -63,120 +63,140 @@
 
 
 
 # Enter a context with an instance of the API client
 with fixpoint_openapi.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = fixpoint_openapi.FixpointApi(api_client)
-    body = fixpoint_openapi.V1CreateApiSecretRequest() # V1CreateApiSecretRequest | 
+    body = fixpoint_openapi.V1BatchCreateFineTuneJobsRequest() # V1BatchCreateFineTuneJobsRequest | 
 
     try:
-        # Store LLM inference API secret
-        api_response = api_instance.fixpoint_create_api_secret(body)
-        print("The response of FixpointApi->fixpoint_create_api_secret:\n")
+        api_response = api_instance.fixpoint_batch_create_fine_tune_jobs(body)
+        print("The response of FixpointApi->fixpoint_batch_create_fine_tune_jobs:\n")
         pprint(api_response)
     except ApiException as e:
-        print("Exception when calling FixpointApi->fixpoint_create_api_secret: %s\n" % e)
+        print("Exception when calling FixpointApi->fixpoint_batch_create_fine_tune_jobs: %s\n" % e)
 
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *http://localhost*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
+*FixpointApi* | [**fixpoint_batch_create_fine_tune_jobs**](docs/FixpointApi.md#fixpoint_batch_create_fine_tune_jobs) | **POST** /v1/fine_tune_jobs:batchCreate | 
+*FixpointApi* | [**fixpoint_batch_delete_dataset_logs**](docs/FixpointApi.md#fixpoint_batch_delete_dataset_logs) | **POST** /v1/datasets/{datasetId}/logs:deleteLogs | 
+*FixpointApi* | [**fixpoint_create_ab_chat_completion**](docs/FixpointApi.md#fixpoint_create_ab_chat_completion) | **POST** /v1/chat/completions/ab | Create A/B routed chat completion
 *FixpointApi* | [**fixpoint_create_api_secret**](docs/FixpointApi.md#fixpoint_create_api_secret) | **POST** /v1/api_secrets | Store LLM inference API secret
 *FixpointApi* | [**fixpoint_create_app_logs**](docs/FixpointApi.md#fixpoint_create_app_logs) | **POST** /v1/app_logs | Create application logs
 *FixpointApi* | [**fixpoint_create_dataset**](docs/FixpointApi.md#fixpoint_create_dataset) | **POST** /v1/datasets | Create LLM dataset
 *FixpointApi* | [**fixpoint_create_likes**](docs/FixpointApi.md#fixpoint_create_likes) | **POST** /v1/likes | Add LLM log feedback (\&quot;likes\&quot;)
 *FixpointApi* | [**fixpoint_create_log_attribute**](docs/FixpointApi.md#fixpoint_create_log_attribute) | **POST** /v1/attributes | Attach attribute to LLM log
 *FixpointApi* | [**fixpoint_create_multi_llm_chat_completion**](docs/FixpointApi.md#fixpoint_create_multi_llm_chat_completion) | **POST** /v1/chat/completions/multi_llm | 
 *FixpointApi* | [**fixpoint_create_open_ai_chat_input_log**](docs/FixpointApi.md#fixpoint_create_open_ai_chat_input_log) | **POST** /v1/openai_chats/{modelName}/input_logs | Create an LLM input log
 *FixpointApi* | [**fixpoint_create_open_ai_chat_output_log**](docs/FixpointApi.md#fixpoint_create_open_ai_chat_output_log) | **POST** /v1/openai_chats/{modelName}/output_logs | Create an LLM output log
 *FixpointApi* | [**fixpoint_create_routing_config**](docs/FixpointApi.md#fixpoint_create_routing_config) | **POST** /v1/routing_configs | Create LLM routing config
+*FixpointApi* | [**fixpoint_delete_dataset**](docs/FixpointApi.md#fixpoint_delete_dataset) | **DELETE** /v1/datasets/{datasetId} | 
 *FixpointApi* | [**fixpoint_delete_log_attribute**](docs/FixpointApi.md#fixpoint_delete_log_attribute) | **DELETE** /v1/attributes/{name} | Remove LLM log attribute
 *FixpointApi* | [**fixpoint_list_api_secrets**](docs/FixpointApi.md#fixpoint_list_api_secrets) | **GET** /v1/api_secrets | List LLM inference API secrets
 *FixpointApi* | [**fixpoint_list_app_logs**](docs/FixpointApi.md#fixpoint_list_app_logs) | **GET** /v1/app_logs | List application logs
 *FixpointApi* | [**fixpoint_list_datasets**](docs/FixpointApi.md#fixpoint_list_datasets) | **GET** /v1/datasets | List LLM datasets
+*FixpointApi* | [**fixpoint_list_fine_tune_jobs**](docs/FixpointApi.md#fixpoint_list_fine_tune_jobs) | **GET** /v1/fine_tune_jobs | 
 *FixpointApi* | [**fixpoint_list_likes**](docs/FixpointApi.md#fixpoint_list_likes) | **GET** /v1/likes | List LLM log feedback (\&quot;likes\&quot;)
 *FixpointApi* | [**fixpoint_list_log_attributes**](docs/FixpointApi.md#fixpoint_list_log_attributes) | **GET** /v1/attributes | List attributes on an LLM log
 *FixpointApi* | [**fixpoint_list_open_ai_chat_logs**](docs/FixpointApi.md#fixpoint_list_open_ai_chat_logs) | **GET** /v1/{parent}/logs | DEPRECATED: List LLM logs
 *FixpointApi* | [**fixpoint_list_routing_configs**](docs/FixpointApi.md#fixpoint_list_routing_configs) | **GET** /v1/routing_configs | List LLM routing configs
 *FixpointApi* | [**fixpoint_post_dataset_logs**](docs/FixpointApi.md#fixpoint_post_dataset_logs) | **POST** /v1/datasets/{name}/logs | Add logs to a dataset
-*FixpointApi* | [**fixpoint_update_spending_totals**](docs/FixpointApi.md#fixpoint_update_spending_totals) | **PATCH** /v1/routing_configs/{routeConfigId} | Update routing config spending totals
+*FixpointApi* | [**fixpoint_update_spending_totals**](docs/FixpointApi.md#fixpoint_update_spending_totals) | **PATCH** /v1/routing_configs/{routingConfigId} | Update routing config spending totals
 
 
 ## Documentation For Models
 
  - [AppLogLevelType](docs/AppLogLevelType.md)
+ - [FixpointBatchDeleteDatasetLogsRequest](docs/FixpointBatchDeleteDatasetLogsRequest.md)
  - [FixpointCreateOpenAIChatInputLogRequest](docs/FixpointCreateOpenAIChatInputLogRequest.md)
  - [FixpointCreateOpenAIChatOutputLogRequest](docs/FixpointCreateOpenAIChatOutputLogRequest.md)
  - [FixpointPostDatasetLogsRequest](docs/FixpointPostDatasetLogsRequest.md)
  - [FixpointUpdateSpendingTotalsRequest](docs/FixpointUpdateSpendingTotalsRequest.md)
- - [Fixpointv1Model](docs/Fixpointv1Model.md)
+ - [Fixpointv1SpendCap](docs/Fixpointv1SpendCap.md)
  - [ProtobufAny](docs/ProtobufAny.md)
  - [ProtobufNullValue](docs/ProtobufNullValue.md)
+ - [RoutingBlockAB](docs/RoutingBlockAB.md)
  - [RpcStatus](docs/RpcStatus.md)
  - [ToolCallFunction](docs/ToolCallFunction.md)
+ - [V1AbChatCompletion](docs/V1AbChatCompletion.md)
  - [V1ApiSecret](docs/V1ApiSecret.md)
  - [V1ApiSecretProvider](docs/V1ApiSecretProvider.md)
  - [V1AppLog](docs/V1AppLog.md)
  - [V1AttributeFilters](docs/V1AttributeFilters.md)
+ - [V1BatchCreateFineTuneJobsRequest](docs/V1BatchCreateFineTuneJobsRequest.md)
+ - [V1BatchCreateFineTuneJobsResponse](docs/V1BatchCreateFineTuneJobsResponse.md)
  - [V1ChatCompletion](docs/V1ChatCompletion.md)
  - [V1ChatCompletionChoice](docs/V1ChatCompletionChoice.md)
  - [V1ChatCompletionUsage](docs/V1ChatCompletionUsage.md)
+ - [V1CreateABChatCompletionRequest](docs/V1CreateABChatCompletionRequest.md)
  - [V1CreateApiSecretRequest](docs/V1CreateApiSecretRequest.md)
  - [V1CreateAppLogsRequest](docs/V1CreateAppLogsRequest.md)
  - [V1CreateAppLogsResponse](docs/V1CreateAppLogsResponse.md)
  - [V1CreateDatasetRequest](docs/V1CreateDatasetRequest.md)
  - [V1CreateDatasetResponse](docs/V1CreateDatasetResponse.md)
  - [V1CreateLikesRequest](docs/V1CreateLikesRequest.md)
  - [V1CreateLikesResponse](docs/V1CreateLikesResponse.md)
  - [V1CreateLogAttributeRequest](docs/V1CreateLogAttributeRequest.md)
  - [V1CreateLogAttributeResponse](docs/V1CreateLogAttributeResponse.md)
  - [V1CreateMultiLLMChatCompletionRequest](docs/V1CreateMultiLLMChatCompletionRequest.md)
- - [V1CreateMultiLLMChatCompletionRequestModel](docs/V1CreateMultiLLMChatCompletionRequestModel.md)
  - [V1CreateRoutingConfigRequest](docs/V1CreateRoutingConfigRequest.md)
  - [V1Dataset](docs/V1Dataset.md)
  - [V1DatasetFilters](docs/V1DatasetFilters.md)
+ - [V1DeleteDatasetLogsResponse](docs/V1DeleteDatasetLogsResponse.md)
+ - [V1DeleteDatasetResponse](docs/V1DeleteDatasetResponse.md)
  - [V1DeleteLogAttributeResponse](docs/V1DeleteLogAttributeResponse.md)
  - [V1FallbackStrategy](docs/V1FallbackStrategy.md)
+ - [V1FineTuneJob](docs/V1FineTuneJob.md)
+ - [V1FineTuneStatus](docs/V1FineTuneStatus.md)
+ - [V1Hyperparameters](docs/V1Hyperparameters.md)
  - [V1InputMessage](docs/V1InputMessage.md)
  - [V1Like](docs/V1Like.md)
  - [V1LikeFilter](docs/V1LikeFilter.md)
  - [V1LikeIngest](docs/V1LikeIngest.md)
  - [V1ListApiSecretsResponse](docs/V1ListApiSecretsResponse.md)
  - [V1ListAppLogsResponse](docs/V1ListAppLogsResponse.md)
  - [V1ListDatasetsResponse](docs/V1ListDatasetsResponse.md)
+ - [V1ListFineTuneJobsResponse](docs/V1ListFineTuneJobsResponse.md)
  - [V1ListLikesResponse](docs/V1ListLikesResponse.md)
  - [V1ListLogAttributesResponse](docs/V1ListLogAttributesResponse.md)
  - [V1ListOpenAIChatLogsResponse](docs/V1ListOpenAIChatLogsResponse.md)
  - [V1ListRoutingConfigsResponse](docs/V1ListRoutingConfigsResponse.md)
  - [V1LogAttribute](docs/V1LogAttribute.md)
  - [V1Mode](docs/V1Mode.md)
+ - [V1Model](docs/V1Model.md)
  - [V1MultiLLMChatCompletion](docs/V1MultiLLMChatCompletion.md)
  - [V1OpenAIChatInputLog](docs/V1OpenAIChatInputLog.md)
  - [V1OpenAIChatLog](docs/V1OpenAIChatLog.md)
  - [V1OpenAIChatLogsFilters](docs/V1OpenAIChatLogsFilters.md)
  - [V1OpenAIChatOutputLog](docs/V1OpenAIChatOutputLog.md)
  - [V1OpenAIChatOutputLogChoice](docs/V1OpenAIChatOutputLogChoice.md)
  - [V1OpenAIChatOutputLogUsage](docs/V1OpenAIChatOutputLogUsage.md)
  - [V1OriginType](docs/V1OriginType.md)
  - [V1OutputMessage](docs/V1OutputMessage.md)
  - [V1PostDatasetLogsResponse](docs/V1PostDatasetLogsResponse.md)
  - [V1RelativeDateTimeFilters](docs/V1RelativeDateTimeFilters.md)
  - [V1ResetInterval](docs/V1ResetInterval.md)
+ - [V1RoutingBlock](docs/V1RoutingBlock.md)
+ - [V1RoutingBlockSpendCap](docs/V1RoutingBlockSpendCap.md)
+ - [V1RoutingBlockType](docs/V1RoutingBlockType.md)
  - [V1RoutingConfig](docs/V1RoutingConfig.md)
- - [V1SpendCap](docs/V1SpendCap.md)
+ - [V1SpendCapModel](docs/V1SpendCapModel.md)
  - [V1TerminalState](docs/V1TerminalState.md)
  - [V1ThumbsReaction](docs/V1ThumbsReaction.md)
  - [V1ToolCall](docs/V1ToolCall.md)
  - [V1Tracing](docs/V1Tracing.md)
  - [V1TracingFilters](docs/V1TracingFilters.md)
+ - [V1TuningConfiguration](docs/V1TuningConfiguration.md)
  - [V1UsageTotals](docs/V1UsageTotals.md)
 
 
 <a id="documentation-for-authorization"></a>
 ## Documentation For Authorization
 
 Endpoints do not require authorization.
```

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/__init__.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,99 +1,98 @@
 # coding: utf-8
 
 # flake8: noqa
-
 """
     fixpoint/v1/service.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: version not set
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "0.1.0"
-
-# import apis into sdk package
-from fixpoint_openapi.api.fixpoint_api import FixpointApi
-
-# import ApiClient
-from fixpoint_openapi.api_response import ApiResponse
-from fixpoint_openapi.api_client import ApiClient
-from fixpoint_openapi.configuration import Configuration
-from fixpoint_openapi.exceptions import OpenApiException
-from fixpoint_openapi.exceptions import ApiTypeError
-from fixpoint_openapi.exceptions import ApiValueError
-from fixpoint_openapi.exceptions import ApiKeyError
-from fixpoint_openapi.exceptions import ApiAttributeError
-from fixpoint_openapi.exceptions import ApiException
-
-# import models into sdk package
+# import models into model package
 from fixpoint_openapi.models.app_log_level_type import AppLogLevelType
+from fixpoint_openapi.models.fixpoint_batch_delete_dataset_logs_request import FixpointBatchDeleteDatasetLogsRequest
 from fixpoint_openapi.models.fixpoint_create_open_ai_chat_input_log_request import FixpointCreateOpenAIChatInputLogRequest
 from fixpoint_openapi.models.fixpoint_create_open_ai_chat_output_log_request import FixpointCreateOpenAIChatOutputLogRequest
 from fixpoint_openapi.models.fixpoint_post_dataset_logs_request import FixpointPostDatasetLogsRequest
 from fixpoint_openapi.models.fixpoint_update_spending_totals_request import FixpointUpdateSpendingTotalsRequest
-from fixpoint_openapi.models.fixpointv1_model import Fixpointv1Model
+from fixpoint_openapi.models.fixpointv1_spend_cap import Fixpointv1SpendCap
 from fixpoint_openapi.models.protobuf_any import ProtobufAny
 from fixpoint_openapi.models.protobuf_null_value import ProtobufNullValue
+from fixpoint_openapi.models.routing_block_ab import RoutingBlockAB
 from fixpoint_openapi.models.rpc_status import RpcStatus
 from fixpoint_openapi.models.tool_call_function import ToolCallFunction
+from fixpoint_openapi.models.v1_ab_chat_completion import V1AbChatCompletion
 from fixpoint_openapi.models.v1_api_secret import V1ApiSecret
 from fixpoint_openapi.models.v1_api_secret_provider import V1ApiSecretProvider
 from fixpoint_openapi.models.v1_app_log import V1AppLog
 from fixpoint_openapi.models.v1_attribute_filters import V1AttributeFilters
+from fixpoint_openapi.models.v1_batch_create_fine_tune_jobs_request import V1BatchCreateFineTuneJobsRequest
+from fixpoint_openapi.models.v1_batch_create_fine_tune_jobs_response import V1BatchCreateFineTuneJobsResponse
 from fixpoint_openapi.models.v1_chat_completion import V1ChatCompletion
 from fixpoint_openapi.models.v1_chat_completion_choice import V1ChatCompletionChoice
 from fixpoint_openapi.models.v1_chat_completion_usage import V1ChatCompletionUsage
+from fixpoint_openapi.models.v1_create_ab_chat_completion_request import V1CreateABChatCompletionRequest
 from fixpoint_openapi.models.v1_create_api_secret_request import V1CreateApiSecretRequest
 from fixpoint_openapi.models.v1_create_app_logs_request import V1CreateAppLogsRequest
 from fixpoint_openapi.models.v1_create_app_logs_response import V1CreateAppLogsResponse
 from fixpoint_openapi.models.v1_create_dataset_request import V1CreateDatasetRequest
 from fixpoint_openapi.models.v1_create_dataset_response import V1CreateDatasetResponse
 from fixpoint_openapi.models.v1_create_likes_request import V1CreateLikesRequest
 from fixpoint_openapi.models.v1_create_likes_response import V1CreateLikesResponse
 from fixpoint_openapi.models.v1_create_log_attribute_request import V1CreateLogAttributeRequest
 from fixpoint_openapi.models.v1_create_log_attribute_response import V1CreateLogAttributeResponse
 from fixpoint_openapi.models.v1_create_multi_llm_chat_completion_request import V1CreateMultiLLMChatCompletionRequest
-from fixpoint_openapi.models.v1_create_multi_llm_chat_completion_request_model import V1CreateMultiLLMChatCompletionRequestModel
 from fixpoint_openapi.models.v1_create_routing_config_request import V1CreateRoutingConfigRequest
 from fixpoint_openapi.models.v1_dataset import V1Dataset
 from fixpoint_openapi.models.v1_dataset_filters import V1DatasetFilters
+from fixpoint_openapi.models.v1_delete_dataset_logs_response import V1DeleteDatasetLogsResponse
+from fixpoint_openapi.models.v1_delete_dataset_response import V1DeleteDatasetResponse
 from fixpoint_openapi.models.v1_delete_log_attribute_response import V1DeleteLogAttributeResponse
 from fixpoint_openapi.models.v1_fallback_strategy import V1FallbackStrategy
+from fixpoint_openapi.models.v1_fine_tune_job import V1FineTuneJob
+from fixpoint_openapi.models.v1_fine_tune_status import V1FineTuneStatus
+from fixpoint_openapi.models.v1_hyperparameters import V1Hyperparameters
 from fixpoint_openapi.models.v1_input_message import V1InputMessage
 from fixpoint_openapi.models.v1_like import V1Like
 from fixpoint_openapi.models.v1_like_filter import V1LikeFilter
 from fixpoint_openapi.models.v1_like_ingest import V1LikeIngest
 from fixpoint_openapi.models.v1_list_api_secrets_response import V1ListApiSecretsResponse
 from fixpoint_openapi.models.v1_list_app_logs_response import V1ListAppLogsResponse
 from fixpoint_openapi.models.v1_list_datasets_response import V1ListDatasetsResponse
+from fixpoint_openapi.models.v1_list_fine_tune_jobs_response import V1ListFineTuneJobsResponse
 from fixpoint_openapi.models.v1_list_likes_response import V1ListLikesResponse
 from fixpoint_openapi.models.v1_list_log_attributes_response import V1ListLogAttributesResponse
 from fixpoint_openapi.models.v1_list_open_ai_chat_logs_response import V1ListOpenAIChatLogsResponse
 from fixpoint_openapi.models.v1_list_routing_configs_response import V1ListRoutingConfigsResponse
 from fixpoint_openapi.models.v1_log_attribute import V1LogAttribute
 from fixpoint_openapi.models.v1_mode import V1Mode
+from fixpoint_openapi.models.v1_model import V1Model
 from fixpoint_openapi.models.v1_multi_llm_chat_completion import V1MultiLLMChatCompletion
 from fixpoint_openapi.models.v1_open_ai_chat_input_log import V1OpenAIChatInputLog
 from fixpoint_openapi.models.v1_open_ai_chat_log import V1OpenAIChatLog
 from fixpoint_openapi.models.v1_open_ai_chat_logs_filters import V1OpenAIChatLogsFilters
 from fixpoint_openapi.models.v1_open_ai_chat_output_log import V1OpenAIChatOutputLog
 from fixpoint_openapi.models.v1_open_ai_chat_output_log_choice import V1OpenAIChatOutputLogChoice
 from fixpoint_openapi.models.v1_open_ai_chat_output_log_usage import V1OpenAIChatOutputLogUsage
 from fixpoint_openapi.models.v1_origin_type import V1OriginType
 from fixpoint_openapi.models.v1_output_message import V1OutputMessage
 from fixpoint_openapi.models.v1_post_dataset_logs_response import V1PostDatasetLogsResponse
 from fixpoint_openapi.models.v1_relative_date_time_filters import V1RelativeDateTimeFilters
 from fixpoint_openapi.models.v1_reset_interval import V1ResetInterval
+from fixpoint_openapi.models.v1_routing_block import V1RoutingBlock
+from fixpoint_openapi.models.v1_routing_block_spend_cap import V1RoutingBlockSpendCap
+from fixpoint_openapi.models.v1_routing_block_type import V1RoutingBlockType
 from fixpoint_openapi.models.v1_routing_config import V1RoutingConfig
-from fixpoint_openapi.models.v1_spend_cap import V1SpendCap
+from fixpoint_openapi.models.v1_spend_cap_model import V1SpendCapModel
 from fixpoint_openapi.models.v1_terminal_state import V1TerminalState
 from fixpoint_openapi.models.v1_thumbs_reaction import V1ThumbsReaction
 from fixpoint_openapi.models.v1_tool_call import V1ToolCall
 from fixpoint_openapi.models.v1_tracing import V1Tracing
 from fixpoint_openapi.models.v1_tracing_filters import V1TracingFilters
+from fixpoint_openapi.models.v1_tuning_configuration import V1TuningConfiguration
 from fixpoint_openapi.models.v1_usage_totals import V1UsageTotals
```

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/api/fixpoint_api.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/api/fixpoint_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,34 +15,42 @@
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictBool, StrictInt, StrictStr, field_validator
 from typing import List, Optional
 from typing_extensions import Annotated
+from fixpoint_openapi.models.fixpoint_batch_delete_dataset_logs_request import FixpointBatchDeleteDatasetLogsRequest
 from fixpoint_openapi.models.fixpoint_create_open_ai_chat_input_log_request import FixpointCreateOpenAIChatInputLogRequest
 from fixpoint_openapi.models.fixpoint_create_open_ai_chat_output_log_request import FixpointCreateOpenAIChatOutputLogRequest
 from fixpoint_openapi.models.fixpoint_post_dataset_logs_request import FixpointPostDatasetLogsRequest
 from fixpoint_openapi.models.fixpoint_update_spending_totals_request import FixpointUpdateSpendingTotalsRequest
+from fixpoint_openapi.models.v1_ab_chat_completion import V1AbChatCompletion
 from fixpoint_openapi.models.v1_api_secret import V1ApiSecret
+from fixpoint_openapi.models.v1_batch_create_fine_tune_jobs_request import V1BatchCreateFineTuneJobsRequest
+from fixpoint_openapi.models.v1_batch_create_fine_tune_jobs_response import V1BatchCreateFineTuneJobsResponse
+from fixpoint_openapi.models.v1_create_ab_chat_completion_request import V1CreateABChatCompletionRequest
 from fixpoint_openapi.models.v1_create_api_secret_request import V1CreateApiSecretRequest
 from fixpoint_openapi.models.v1_create_app_logs_request import V1CreateAppLogsRequest
 from fixpoint_openapi.models.v1_create_app_logs_response import V1CreateAppLogsResponse
 from fixpoint_openapi.models.v1_create_dataset_request import V1CreateDatasetRequest
 from fixpoint_openapi.models.v1_create_dataset_response import V1CreateDatasetResponse
 from fixpoint_openapi.models.v1_create_likes_request import V1CreateLikesRequest
 from fixpoint_openapi.models.v1_create_likes_response import V1CreateLikesResponse
 from fixpoint_openapi.models.v1_create_log_attribute_request import V1CreateLogAttributeRequest
 from fixpoint_openapi.models.v1_create_log_attribute_response import V1CreateLogAttributeResponse
 from fixpoint_openapi.models.v1_create_multi_llm_chat_completion_request import V1CreateMultiLLMChatCompletionRequest
 from fixpoint_openapi.models.v1_create_routing_config_request import V1CreateRoutingConfigRequest
+from fixpoint_openapi.models.v1_delete_dataset_logs_response import V1DeleteDatasetLogsResponse
+from fixpoint_openapi.models.v1_delete_dataset_response import V1DeleteDatasetResponse
 from fixpoint_openapi.models.v1_delete_log_attribute_response import V1DeleteLogAttributeResponse
 from fixpoint_openapi.models.v1_list_api_secrets_response import V1ListApiSecretsResponse
 from fixpoint_openapi.models.v1_list_app_logs_response import V1ListAppLogsResponse
 from fixpoint_openapi.models.v1_list_datasets_response import V1ListDatasetsResponse
+from fixpoint_openapi.models.v1_list_fine_tune_jobs_response import V1ListFineTuneJobsResponse
 from fixpoint_openapi.models.v1_list_likes_response import V1ListLikesResponse
 from fixpoint_openapi.models.v1_list_log_attributes_response import V1ListLogAttributesResponse
 from fixpoint_openapi.models.v1_list_open_ai_chat_logs_response import V1ListOpenAIChatLogsResponse
 from fixpoint_openapi.models.v1_list_routing_configs_response import V1ListRoutingConfigsResponse
 from fixpoint_openapi.models.v1_multi_llm_chat_completion import V1MultiLLMChatCompletion
 from fixpoint_openapi.models.v1_open_ai_chat_input_log import V1OpenAIChatInputLog
 from fixpoint_openapi.models.v1_open_ai_chat_output_log import V1OpenAIChatOutputLog
@@ -64,14 +72,833 @@
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
+    def fixpoint_batch_create_fine_tune_jobs(
+        self,
+        body: V1BatchCreateFineTuneJobsRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> V1BatchCreateFineTuneJobsResponse:
+        """fixpoint_batch_create_fine_tune_jobs
+
+
+        :param body: (required)
+        :type body: V1BatchCreateFineTuneJobsRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._fixpoint_batch_create_fine_tune_jobs_serialize(
+            body=body,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "V1BatchCreateFineTuneJobsResponse",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def fixpoint_batch_create_fine_tune_jobs_with_http_info(
+        self,
+        body: V1BatchCreateFineTuneJobsRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[V1BatchCreateFineTuneJobsResponse]:
+        """fixpoint_batch_create_fine_tune_jobs
+
+
+        :param body: (required)
+        :type body: V1BatchCreateFineTuneJobsRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._fixpoint_batch_create_fine_tune_jobs_serialize(
+            body=body,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "V1BatchCreateFineTuneJobsResponse",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def fixpoint_batch_create_fine_tune_jobs_without_preload_content(
+        self,
+        body: V1BatchCreateFineTuneJobsRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """fixpoint_batch_create_fine_tune_jobs
+
+
+        :param body: (required)
+        :type body: V1BatchCreateFineTuneJobsRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._fixpoint_batch_create_fine_tune_jobs_serialize(
+            body=body,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "V1BatchCreateFineTuneJobsResponse",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _fixpoint_batch_create_fine_tune_jobs_serialize(
+        self,
+        body,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+        if body is not None:
+            _body_params = body
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
+
+        # authentication setting
+        _auth_settings: List[str] = [
+        ]
+
+        return self.api_client.param_serialize(
+            method='POST',
+            resource_path='/v1/fine_tune_jobs:batchCreate',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def fixpoint_batch_delete_dataset_logs(
+        self,
+        dataset_id: StrictStr,
+        body: FixpointBatchDeleteDatasetLogsRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> V1DeleteDatasetLogsResponse:
+        """fixpoint_batch_delete_dataset_logs
+
+
+        :param dataset_id: (required)
+        :type dataset_id: str
+        :param body: (required)
+        :type body: FixpointBatchDeleteDatasetLogsRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._fixpoint_batch_delete_dataset_logs_serialize(
+            dataset_id=dataset_id,
+            body=body,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "V1DeleteDatasetLogsResponse",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def fixpoint_batch_delete_dataset_logs_with_http_info(
+        self,
+        dataset_id: StrictStr,
+        body: FixpointBatchDeleteDatasetLogsRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[V1DeleteDatasetLogsResponse]:
+        """fixpoint_batch_delete_dataset_logs
+
+
+        :param dataset_id: (required)
+        :type dataset_id: str
+        :param body: (required)
+        :type body: FixpointBatchDeleteDatasetLogsRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._fixpoint_batch_delete_dataset_logs_serialize(
+            dataset_id=dataset_id,
+            body=body,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "V1DeleteDatasetLogsResponse",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def fixpoint_batch_delete_dataset_logs_without_preload_content(
+        self,
+        dataset_id: StrictStr,
+        body: FixpointBatchDeleteDatasetLogsRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """fixpoint_batch_delete_dataset_logs
+
+
+        :param dataset_id: (required)
+        :type dataset_id: str
+        :param body: (required)
+        :type body: FixpointBatchDeleteDatasetLogsRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._fixpoint_batch_delete_dataset_logs_serialize(
+            dataset_id=dataset_id,
+            body=body,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "V1DeleteDatasetLogsResponse",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _fixpoint_batch_delete_dataset_logs_serialize(
+        self,
+        dataset_id,
+        body,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if dataset_id is not None:
+            _path_params['datasetId'] = dataset_id
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+        if body is not None:
+            _body_params = body
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
+
+        # authentication setting
+        _auth_settings: List[str] = [
+        ]
+
+        return self.api_client.param_serialize(
+            method='POST',
+            resource_path='/v1/datasets/{datasetId}/logs:deleteLogs',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def fixpoint_create_ab_chat_completion(
+        self,
+        body: V1CreateABChatCompletionRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> V1AbChatCompletion:
+        """Create A/B routed chat completion
+
+        Create a chat completion that is routed to one of the A/B experiment arms.
+
+        :param body: (required)
+        :type body: V1CreateABChatCompletionRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._fixpoint_create_ab_chat_completion_serialize(
+            body=body,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "V1AbChatCompletion",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def fixpoint_create_ab_chat_completion_with_http_info(
+        self,
+        body: V1CreateABChatCompletionRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[V1AbChatCompletion]:
+        """Create A/B routed chat completion
+
+        Create a chat completion that is routed to one of the A/B experiment arms.
+
+        :param body: (required)
+        :type body: V1CreateABChatCompletionRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._fixpoint_create_ab_chat_completion_serialize(
+            body=body,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "V1AbChatCompletion",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def fixpoint_create_ab_chat_completion_without_preload_content(
+        self,
+        body: V1CreateABChatCompletionRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """Create A/B routed chat completion
+
+        Create a chat completion that is routed to one of the A/B experiment arms.
+
+        :param body: (required)
+        :type body: V1CreateABChatCompletionRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._fixpoint_create_ab_chat_completion_serialize(
+            body=body,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "V1AbChatCompletion",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _fixpoint_create_ab_chat_completion_serialize(
+        self,
+        body,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+        if body is not None:
+            _body_params = body
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
+
+        # authentication setting
+        _auth_settings: List[str] = [
+        ]
+
+        return self.api_client.param_serialize(
+            method='POST',
+            resource_path='/v1/chat/completions/ab',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
     def fixpoint_create_api_secret(
         self,
         body: V1CreateApiSecretRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
@@ -2515,14 +3342,268 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
+    def fixpoint_delete_dataset(
+        self,
+        dataset_id: StrictStr,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> V1DeleteDatasetResponse:
+        """fixpoint_delete_dataset
+
+
+        :param dataset_id: (required)
+        :type dataset_id: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._fixpoint_delete_dataset_serialize(
+            dataset_id=dataset_id,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "V1DeleteDatasetResponse",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def fixpoint_delete_dataset_with_http_info(
+        self,
+        dataset_id: StrictStr,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[V1DeleteDatasetResponse]:
+        """fixpoint_delete_dataset
+
+
+        :param dataset_id: (required)
+        :type dataset_id: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._fixpoint_delete_dataset_serialize(
+            dataset_id=dataset_id,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "V1DeleteDatasetResponse",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def fixpoint_delete_dataset_without_preload_content(
+        self,
+        dataset_id: StrictStr,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """fixpoint_delete_dataset
+
+
+        :param dataset_id: (required)
+        :type dataset_id: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._fixpoint_delete_dataset_serialize(
+            dataset_id=dataset_id,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "V1DeleteDatasetResponse",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _fixpoint_delete_dataset_serialize(
+        self,
+        dataset_id,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if dataset_id is not None:
+            _path_params['datasetId'] = dataset_id
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+        ]
+
+        return self.api_client.param_serialize(
+            method='DELETE',
+            resource_path='/v1/datasets/{datasetId}',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
     def fixpoint_delete_log_attribute(
         self,
         name: StrictStr,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
@@ -2771,14 +3852,15 @@
 
 
 
 
     @validate_call
     def fixpoint_list_api_secrets(
         self,
+        alias: Annotated[Optional[StrictStr], Field(description="optional alias to filter by")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -2787,14 +3869,16 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> V1ListApiSecretsResponse:
         """List LLM inference API secrets
 
 
+        :param alias: optional alias to filter by
+        :type alias: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2810,14 +3894,15 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._fixpoint_list_api_secrets_serialize(
+            alias=alias,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -2833,14 +3918,15 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     def fixpoint_list_api_secrets_with_http_info(
         self,
+        alias: Annotated[Optional[StrictStr], Field(description="optional alias to filter by")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -2849,14 +3935,16 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[V1ListApiSecretsResponse]:
         """List LLM inference API secrets
 
 
+        :param alias: optional alias to filter by
+        :type alias: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2872,14 +3960,15 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._fixpoint_list_api_secrets_serialize(
+            alias=alias,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -2895,14 +3984,15 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     def fixpoint_list_api_secrets_without_preload_content(
         self,
+        alias: Annotated[Optional[StrictStr], Field(description="optional alias to filter by")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -2911,14 +4001,16 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """List LLM inference API secrets
 
 
+        :param alias: optional alias to filter by
+        :type alias: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2934,14 +4026,15 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._fixpoint_list_api_secrets_serialize(
+            alias=alias,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -2952,14 +4045,15 @@
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _fixpoint_list_api_secrets_serialize(
         self,
+        alias,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -2972,14 +4066,18 @@
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
+        if alias is not None:
+            
+            _query_params.append(('alias', alias))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -3540,14 +4638,322 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
+    def fixpoint_list_fine_tune_jobs(
+        self,
+        job_ids: Optional[List[StrictStr]] = None,
+        mode: Optional[StrictStr] = None,
+        query_provider_for_status_and_update: Annotated[Optional[StrictBool], Field(description="When set to true calls an llm provider like openai to get the status of fine tune job")] = None,
+        dataset_id: Optional[StrictStr] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> V1ListFineTuneJobsResponse:
+        """fixpoint_list_fine_tune_jobs
+
+
+        :param job_ids:
+        :type job_ids: List[str]
+        :param mode:
+        :type mode: str
+        :param query_provider_for_status_and_update: When set to true calls an llm provider like openai to get the status of fine tune job
+        :type query_provider_for_status_and_update: bool
+        :param dataset_id:
+        :type dataset_id: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._fixpoint_list_fine_tune_jobs_serialize(
+            job_ids=job_ids,
+            mode=mode,
+            query_provider_for_status_and_update=query_provider_for_status_and_update,
+            dataset_id=dataset_id,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "V1ListFineTuneJobsResponse",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def fixpoint_list_fine_tune_jobs_with_http_info(
+        self,
+        job_ids: Optional[List[StrictStr]] = None,
+        mode: Optional[StrictStr] = None,
+        query_provider_for_status_and_update: Annotated[Optional[StrictBool], Field(description="When set to true calls an llm provider like openai to get the status of fine tune job")] = None,
+        dataset_id: Optional[StrictStr] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[V1ListFineTuneJobsResponse]:
+        """fixpoint_list_fine_tune_jobs
+
+
+        :param job_ids:
+        :type job_ids: List[str]
+        :param mode:
+        :type mode: str
+        :param query_provider_for_status_and_update: When set to true calls an llm provider like openai to get the status of fine tune job
+        :type query_provider_for_status_and_update: bool
+        :param dataset_id:
+        :type dataset_id: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._fixpoint_list_fine_tune_jobs_serialize(
+            job_ids=job_ids,
+            mode=mode,
+            query_provider_for_status_and_update=query_provider_for_status_and_update,
+            dataset_id=dataset_id,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "V1ListFineTuneJobsResponse",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def fixpoint_list_fine_tune_jobs_without_preload_content(
+        self,
+        job_ids: Optional[List[StrictStr]] = None,
+        mode: Optional[StrictStr] = None,
+        query_provider_for_status_and_update: Annotated[Optional[StrictBool], Field(description="When set to true calls an llm provider like openai to get the status of fine tune job")] = None,
+        dataset_id: Optional[StrictStr] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """fixpoint_list_fine_tune_jobs
+
+
+        :param job_ids:
+        :type job_ids: List[str]
+        :param mode:
+        :type mode: str
+        :param query_provider_for_status_and_update: When set to true calls an llm provider like openai to get the status of fine tune job
+        :type query_provider_for_status_and_update: bool
+        :param dataset_id:
+        :type dataset_id: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._fixpoint_list_fine_tune_jobs_serialize(
+            job_ids=job_ids,
+            mode=mode,
+            query_provider_for_status_and_update=query_provider_for_status_and_update,
+            dataset_id=dataset_id,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "V1ListFineTuneJobsResponse",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _fixpoint_list_fine_tune_jobs_serialize(
+        self,
+        job_ids,
+        mode,
+        query_provider_for_status_and_update,
+        dataset_id,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+            'jobIds': 'multi',
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        # process the query parameters
+        if job_ids is not None:
+            
+            _query_params.append(('jobIds', job_ids))
+            
+        if mode is not None:
+            
+            _query_params.append(('mode', mode))
+            
+        if query_provider_for_status_and_update is not None:
+            
+            _query_params.append(('queryProviderForStatusAndUpdate', query_provider_for_status_and_update))
+            
+        if dataset_id is not None:
+            
+            _query_params.append(('datasetId', dataset_id))
+            
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+        ]
+
+        return self.api_client.param_serialize(
+            method='GET',
+            resource_path='/v1/fine_tune_jobs',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
     def fixpoint_list_likes(
         self,
         page_size: Optional[StrictInt] = None,
         log_name: Optional[StrictStr] = None,
         user_id: Optional[StrictStr] = None,
         origin: Optional[StrictStr] = None,
         thumbs_reaction: Optional[StrictStr] = None,
@@ -5125,15 +6531,15 @@
 
 
 
 
     @validate_call
     def fixpoint_update_spending_totals(
         self,
-        route_config_id: StrictStr,
+        routing_config_id: StrictStr,
         body: FixpointUpdateSpendingTotalsRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
@@ -5144,16 +6550,16 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> V1RoutingConfig:
         """Update routing config spending totals
 
         Update spending totals on a routing config.
 
-        :param route_config_id: (required)
-        :type route_config_id: str
+        :param routing_config_id: (required)
+        :type routing_config_id: str
         :param body: (required)
         :type body: FixpointUpdateSpendingTotalsRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -5171,15 +6577,15 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._fixpoint_update_spending_totals_serialize(
-            route_config_id=route_config_id,
+            routing_config_id=routing_config_id,
             body=body,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -5196,15 +6602,15 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     def fixpoint_update_spending_totals_with_http_info(
         self,
-        route_config_id: StrictStr,
+        routing_config_id: StrictStr,
         body: FixpointUpdateSpendingTotalsRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
@@ -5215,16 +6621,16 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[V1RoutingConfig]:
         """Update routing config spending totals
 
         Update spending totals on a routing config.
 
-        :param route_config_id: (required)
-        :type route_config_id: str
+        :param routing_config_id: (required)
+        :type routing_config_id: str
         :param body: (required)
         :type body: FixpointUpdateSpendingTotalsRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -5242,15 +6648,15 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._fixpoint_update_spending_totals_serialize(
-            route_config_id=route_config_id,
+            routing_config_id=routing_config_id,
             body=body,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -5267,15 +6673,15 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     def fixpoint_update_spending_totals_without_preload_content(
         self,
-        route_config_id: StrictStr,
+        routing_config_id: StrictStr,
         body: FixpointUpdateSpendingTotalsRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
@@ -5286,16 +6692,16 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Update routing config spending totals
 
         Update spending totals on a routing config.
 
-        :param route_config_id: (required)
-        :type route_config_id: str
+        :param routing_config_id: (required)
+        :type routing_config_id: str
         :param body: (required)
         :type body: FixpointUpdateSpendingTotalsRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -5313,15 +6719,15 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._fixpoint_update_spending_totals_serialize(
-            route_config_id=route_config_id,
+            routing_config_id=routing_config_id,
             body=body,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -5333,15 +6739,15 @@
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _fixpoint_update_spending_totals_serialize(
         self,
-        route_config_id,
+        routing_config_id,
         body,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
@@ -5354,16 +6760,16 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if route_config_id is not None:
-            _path_params['routeConfigId'] = route_config_id
+        if routing_config_id is not None:
+            _path_params['routingConfigId'] = routing_config_id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
         if body is not None:
             _body_params = body
 
@@ -5391,15 +6797,15 @@
 
         # authentication setting
         _auth_settings: List[str] = [
         ]
 
         return self.api_client.param_serialize(
             method='PATCH',
-            resource_path='/v1/routing_configs/{routeConfigId}',
+            resource_path='/v1/routing_configs/{routingConfigId}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
```

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/api_client.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/api_client.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/api_response.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/api_response.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/configuration.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/configuration.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/exceptions.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/app_log_level_type.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/app_log_level_type.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/fixpoint_create_open_ai_chat_input_log_request.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/fixpoint_create_open_ai_chat_input_log_request.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/fixpoint_create_open_ai_chat_output_log_request.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/fixpoint_create_open_ai_chat_output_log_request.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/fixpoint_post_dataset_logs_request.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/fixpoint_post_dataset_logs_request.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/fixpoint_update_spending_totals_request.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/fixpoint_update_spending_totals_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field
 from typing import Any, ClassVar, Dict, List, Optional
-from fixpoint_openapi.models.fixpointv1_model import Fixpointv1Model
+from fixpoint_openapi.models.v1_spend_cap_model import V1SpendCapModel
 from typing import Optional, Set
 from typing_extensions import Self
 
 class FixpointUpdateSpendingTotalsRequest(BaseModel):
     """
     FixpointUpdateSpendingTotalsRequest
     """ # noqa: E501
-    models: Optional[List[Fixpointv1Model]] = Field(default=None, description="Spend cap and totals for each model are deltas so that the client cannot alter usage metrics.")
+    models: Optional[List[V1SpendCapModel]] = Field(default=None, description="Spend cap and totals for each model are deltas so that the client cannot alter usage metrics.")
     __properties: ClassVar[List[str]] = ["models"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -84,12 +84,12 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "models": [Fixpointv1Model.from_dict(_item) for _item in obj["models"]] if obj.get("models") is not None else None
+            "models": [V1SpendCapModel.from_dict(_item) for _item in obj["models"]] if obj.get("models") is not None else None
         })
         return _obj
```

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/fixpointv1_model.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/fixpointv1_model.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/protobuf_any.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/protobuf_null_value.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/protobuf_null_value.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/rpc_status.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/rpc_status.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/tool_call_function.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/tool_call_function.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_api_secret.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_api_secret.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_api_secret_provider.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_api_secret_provider.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_app_log.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_app_log.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_attribute_filters.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_attribute_filters.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_chat_completion.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_chat_completion.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_chat_completion_choice.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_chat_completion_choice.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_chat_completion_usage.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_chat_completion_usage.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_create_api_secret_request.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_create_api_secret_request.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_create_app_logs_request.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_create_app_logs_request.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_create_app_logs_response.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_create_app_logs_response.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_create_dataset_request.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_create_dataset_request.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_create_dataset_response.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_create_dataset_response.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_create_likes_request.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_create_likes_request.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_create_likes_response.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_create_likes_response.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_create_log_attribute_request.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_create_log_attribute_request.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_create_log_attribute_response.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_create_log_attribute_response.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_create_multi_llm_chat_completion_request.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_create_ab_chat_completion_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,33 +15,34 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from fixpoint_openapi.models.v1_create_multi_llm_chat_completion_request_model import V1CreateMultiLLMChatCompletionRequestModel
 from fixpoint_openapi.models.v1_input_message import V1InputMessage
 from fixpoint_openapi.models.v1_log_attribute import V1LogAttribute
 from fixpoint_openapi.models.v1_mode import V1Mode
+from fixpoint_openapi.models.v1_model import V1Model
 from fixpoint_openapi.models.v1_tracing import V1Tracing
 from typing import Optional, Set
 from typing_extensions import Self
 
-class V1CreateMultiLLMChatCompletionRequest(BaseModel):
+class V1CreateABChatCompletionRequest(BaseModel):
     """
-    V1CreateMultiLLMChatCompletionRequest
+    V1CreateABChatCompletionRequest
     """ # noqa: E501
-    models: Optional[List[V1CreateMultiLLMChatCompletionRequestModel]] = Field(default=None, description="The models we will route all inference requests to. We return the inference response from the first model in the list to the client.")
-    tracing: Optional[V1Tracing] = None
+    models: Optional[List[V1Model]] = Field(default=None, description="The models we will route all inference requests to. We return the inference response from the first model in the list to the client.")
+    experiment_id: Optional[StrictStr] = Field(default=None, alias="experimentId")
     user_id: Optional[StrictStr] = Field(default=None, alias="userId")
+    tracing: Optional[V1Tracing] = None
     messages: Optional[List[V1InputMessage]] = None
     mode: Optional[V1Mode] = None
     log_attributes: Optional[List[V1LogAttribute]] = Field(default=None, description="Optional attributes to attach to LLM logs created.", alias="logAttributes")
-    __properties: ClassVar[List[str]] = ["models", "tracing", "userId", "messages", "mode", "logAttributes"]
+    __properties: ClassVar[List[str]] = ["models", "experimentId", "userId", "tracing", "messages", "mode", "logAttributes"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -53,15 +54,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of V1CreateMultiLLMChatCompletionRequest from a JSON string"""
+        """Create an instance of V1CreateABChatCompletionRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -102,25 +103,26 @@
                 if _item:
                     _items.append(_item.to_dict())
             _dict['logAttributes'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of V1CreateMultiLLMChatCompletionRequest from a dict"""
+        """Create an instance of V1CreateABChatCompletionRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "models": [V1CreateMultiLLMChatCompletionRequestModel.from_dict(_item) for _item in obj["models"]] if obj.get("models") is not None else None,
-            "tracing": V1Tracing.from_dict(obj["tracing"]) if obj.get("tracing") is not None else None,
+            "models": [V1Model.from_dict(_item) for _item in obj["models"]] if obj.get("models") is not None else None,
+            "experimentId": obj.get("experimentId"),
             "userId": obj.get("userId"),
+            "tracing": V1Tracing.from_dict(obj["tracing"]) if obj.get("tracing") is not None else None,
             "messages": [V1InputMessage.from_dict(_item) for _item in obj["messages"]] if obj.get("messages") is not None else None,
             "mode": obj.get("mode"),
             "logAttributes": [V1LogAttribute.from_dict(_item) for _item in obj["logAttributes"]] if obj.get("logAttributes") is not None else None
         })
         return _obj
```

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_create_multi_llm_chat_completion_request_model.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_create_multi_llm_chat_completion_request_model.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_create_routing_config_request.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_list_open_ai_chat_logs_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,29 +15,26 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from fixpoint_openapi.models.fixpointv1_model import Fixpointv1Model
-from fixpoint_openapi.models.v1_fallback_strategy import V1FallbackStrategy
-from fixpoint_openapi.models.v1_terminal_state import V1TerminalState
+from fixpoint_openapi.models.v1_open_ai_chat_log import V1OpenAIChatLog
 from typing import Optional, Set
 from typing_extensions import Self
 
-class V1CreateRoutingConfigRequest(BaseModel):
+class V1ListOpenAIChatLogsResponse(BaseModel):
     """
-    V1CreateRoutingConfigRequest
+    V1ListOpenAIChatLogsResponse
     """ # noqa: E501
-    models: Optional[List[Fixpointv1Model]] = None
-    description: Optional[StrictStr] = None
-    fallback_strategy: Optional[V1FallbackStrategy] = Field(default=None, alias="fallbackStrategy")
-    terminal_state: Optional[V1TerminalState] = Field(default=None, alias="terminalState")
-    __properties: ClassVar[List[str]] = ["models", "description", "fallbackStrategy", "terminalState"]
+    logs: Optional[List[V1OpenAIChatLog]] = None
+    next_page_token: Optional[StrictStr] = Field(default=None, alias="nextPageToken")
+    total_entries: Optional[StrictStr] = Field(default=None, alias="totalEntries")
+    __properties: ClassVar[List[str]] = ["logs", "nextPageToken", "totalEntries"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -49,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of V1CreateRoutingConfigRequest from a JSON string"""
+        """Create an instance of V1ListOpenAIChatLogsResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,34 +67,38 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in models (list)
+        # override the default output from pydantic by calling `to_dict()` of each item in logs (list)
         _items = []
-        if self.models:
-            for _item in self.models:
+        if self.logs:
+            for _item in self.logs:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['models'] = _items
+            _dict['logs'] = _items
+        # set to None if total_entries (nullable) is None
+        # and model_fields_set contains the field
+        if self.total_entries is None and "total_entries" in self.model_fields_set:
+            _dict['totalEntries'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of V1CreateRoutingConfigRequest from a dict"""
+        """Create an instance of V1ListOpenAIChatLogsResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "models": [Fixpointv1Model.from_dict(_item) for _item in obj["models"]] if obj.get("models") is not None else None,
-            "description": obj.get("description"),
-            "fallbackStrategy": obj.get("fallbackStrategy"),
-            "terminalState": obj.get("terminalState")
+            "logs": [V1OpenAIChatLog.from_dict(_item) for _item in obj["logs"]] if obj.get("logs") is not None else None,
+            "nextPageToken": obj.get("nextPageToken"),
+            "totalEntries": obj.get("totalEntries")
         })
         return _obj
```

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_dataset.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_dataset.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_dataset_filters.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_dataset_filters.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_delete_log_attribute_response.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_delete_log_attribute_response.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_fallback_strategy.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_fallback_strategy.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_input_message.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_input_message.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_like.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_like.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_like_filter.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_like_filter.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_like_ingest.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_like_ingest.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_list_api_secrets_response.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_list_api_secrets_response.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_list_app_logs_response.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_list_app_logs_response.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_list_datasets_response.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_list_datasets_response.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_list_likes_response.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_list_likes_response.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_list_log_attributes_response.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_list_log_attributes_response.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_list_open_ai_chat_logs_response.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_spend_cap_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,26 +15,28 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from fixpoint_openapi.models.v1_open_ai_chat_log import V1OpenAIChatLog
+from fixpoint_openapi.models.fixpointv1_spend_cap import Fixpointv1SpendCap
+from fixpoint_openapi.models.v1_usage_totals import V1UsageTotals
 from typing import Optional, Set
 from typing_extensions import Self
 
-class V1ListOpenAIChatLogsResponse(BaseModel):
+class V1SpendCapModel(BaseModel):
     """
-    V1ListOpenAIChatLogsResponse
+    V1SpendCapModel
     """ # noqa: E501
-    logs: Optional[List[V1OpenAIChatLog]] = None
-    next_page_token: Optional[StrictStr] = Field(default=None, alias="nextPageToken")
-    total_entries: Optional[StrictStr] = Field(default=None, alias="totalEntries")
-    __properties: ClassVar[List[str]] = ["logs", "nextPageToken", "totalEntries"]
+    provider: Optional[StrictStr] = None
+    name: Optional[StrictStr] = None
+    spend_cap: Optional[Fixpointv1SpendCap] = Field(default=None, alias="spendCap")
+    usage_totals: Optional[V1UsageTotals] = Field(default=None, alias="usageTotals")
+    __properties: ClassVar[List[str]] = ["provider", "name", "spendCap", "usageTotals"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -46,15 +48,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of V1ListOpenAIChatLogsResponse from a JSON string"""
+        """Create an instance of V1SpendCapModel from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,38 +69,33 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in logs (list)
-        _items = []
-        if self.logs:
-            for _item in self.logs:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['logs'] = _items
-        # set to None if total_entries (nullable) is None
-        # and model_fields_set contains the field
-        if self.total_entries is None and "total_entries" in self.model_fields_set:
-            _dict['totalEntries'] = None
-
+        # override the default output from pydantic by calling `to_dict()` of spend_cap
+        if self.spend_cap:
+            _dict['spendCap'] = self.spend_cap.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of usage_totals
+        if self.usage_totals:
+            _dict['usageTotals'] = self.usage_totals.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of V1ListOpenAIChatLogsResponse from a dict"""
+        """Create an instance of V1SpendCapModel from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "logs": [V1OpenAIChatLog.from_dict(_item) for _item in obj["logs"]] if obj.get("logs") is not None else None,
-            "nextPageToken": obj.get("nextPageToken"),
-            "totalEntries": obj.get("totalEntries")
+            "provider": obj.get("provider"),
+            "name": obj.get("name"),
+            "spendCap": Fixpointv1SpendCap.from_dict(obj["spendCap"]) if obj.get("spendCap") is not None else None,
+            "usageTotals": V1UsageTotals.from_dict(obj["usageTotals"]) if obj.get("usageTotals") is not None else None
         })
         return _obj
```

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_list_routing_configs_response.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_list_routing_configs_response.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_log_attribute.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_log_attribute.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_mode.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_mode.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_multi_llm_chat_completion.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_multi_llm_chat_completion.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,33 +13,34 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from fixpoint_openapi.models.v1_chat_completion import V1ChatCompletion
 from fixpoint_openapi.models.v1_mode import V1Mode
 from fixpoint_openapi.models.v1_tracing import V1Tracing
 from typing import Optional, Set
 from typing_extensions import Self
 
 class V1MultiLLMChatCompletion(BaseModel):
     """
     V1MultiLLMChatCompletion
     """ # noqa: E501
     id: StrictStr = Field(description="This is the ID of the multi-LLM chat completion. It is also the LLM log ID/name of the input/output log for the primary LLM (aka the completion we return to the client).  If we failed to log the request but succeeded in making the chat completion, we will still return a success, but the \"id\" will be empty. In that case, you can use the primary_external_id to find the logged completions.")
     primary_external_id: Optional[StrictStr] = Field(default=None, description="The external ID of the first model in the multi-LLM inference request. This is the primary model, whose response we return to the client. We can only return the first model ID because other model inference occurs asynchronously.", alias="primaryExternalId")
     model_names: List[StrictStr] = Field(alias="modelNames")
+    display_model: Optional[StrictInt] = Field(default=None, description="The index of the model displayed.", alias="displayModel")
     tracing: Optional[V1Tracing] = None
     completion: V1ChatCompletion
     mode: V1Mode
-    __properties: ClassVar[List[str]] = ["id", "primaryExternalId", "modelNames", "tracing", "completion", "mode"]
+    __properties: ClassVar[List[str]] = ["id", "primaryExternalId", "modelNames", "displayModel", "tracing", "completion", "mode"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -95,14 +96,15 @@
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "id": obj.get("id"),
             "primaryExternalId": obj.get("primaryExternalId"),
             "modelNames": obj.get("modelNames"),
+            "displayModel": obj.get("displayModel"),
             "tracing": V1Tracing.from_dict(obj["tracing"]) if obj.get("tracing") is not None else None,
             "completion": V1ChatCompletion.from_dict(obj["completion"]) if obj.get("completion") is not None else None,
             "mode": obj.get("mode")
         })
         return _obj
```

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_open_ai_chat_input_log.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_open_ai_chat_input_log.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_open_ai_chat_log.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_open_ai_chat_log.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_open_ai_chat_logs_filters.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_open_ai_chat_logs_filters.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_open_ai_chat_output_log.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_open_ai_chat_output_log.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_open_ai_chat_output_log_choice.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_open_ai_chat_output_log_choice.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_open_ai_chat_output_log_usage.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_open_ai_chat_output_log_usage.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_origin_type.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_origin_type.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_output_message.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_output_message.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_post_dataset_logs_response.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_post_dataset_logs_response.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_relative_date_time_filters.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_relative_date_time_filters.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_reset_interval.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_reset_interval.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_routing_config.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_routing_block_spend_cap.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,35 +13,30 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from datetime import datetime
-from pydantic import BaseModel, ConfigDict, Field, StrictStr
+from pydantic import BaseModel, ConfigDict, Field
 from typing import Any, ClassVar, Dict, List, Optional
-from fixpoint_openapi.models.fixpointv1_model import Fixpointv1Model
 from fixpoint_openapi.models.v1_fallback_strategy import V1FallbackStrategy
+from fixpoint_openapi.models.v1_spend_cap_model import V1SpendCapModel
 from fixpoint_openapi.models.v1_terminal_state import V1TerminalState
 from typing import Optional, Set
 from typing_extensions import Self
 
-class V1RoutingConfig(BaseModel):
+class V1RoutingBlockSpendCap(BaseModel):
     """
-    V1RoutingConfig
+    V1RoutingBlockSpendCap
     """ # noqa: E501
-    id: Optional[StrictStr] = None
     fallback_strategy: Optional[V1FallbackStrategy] = Field(default=None, alias="fallbackStrategy")
     terminal_state: Optional[V1TerminalState] = Field(default=None, alias="terminalState")
-    models: Optional[List[Fixpointv1Model]] = None
-    description: Optional[StrictStr] = None
-    created_at: Optional[datetime] = Field(default=None, alias="createdAt")
-    updated_at: Optional[datetime] = Field(default=None, alias="updatedAt")
-    __properties: ClassVar[List[str]] = ["id", "fallbackStrategy", "terminalState", "models", "description", "createdAt", "updatedAt"]
+    models: Optional[List[V1SpendCapModel]] = None
+    __properties: ClassVar[List[str]] = ["fallbackStrategy", "terminalState", "models"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -53,15 +48,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of V1RoutingConfig from a JSON string"""
+        """Create an instance of V1RoutingBlockSpendCap from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -85,26 +80,22 @@
                 if _item:
                     _items.append(_item.to_dict())
             _dict['models'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of V1RoutingConfig from a dict"""
+        """Create an instance of V1RoutingBlockSpendCap from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "id": obj.get("id"),
             "fallbackStrategy": obj.get("fallbackStrategy"),
             "terminalState": obj.get("terminalState"),
-            "models": [Fixpointv1Model.from_dict(_item) for _item in obj["models"]] if obj.get("models") is not None else None,
-            "description": obj.get("description"),
-            "createdAt": obj.get("createdAt"),
-            "updatedAt": obj.get("updatedAt")
+            "models": [V1SpendCapModel.from_dict(_item) for _item in obj["models"]] if obj.get("models") is not None else None
         })
         return _obj
```

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_spend_cap.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_spend_cap.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_terminal_state.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_terminal_state.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_thumbs_reaction.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_thumbs_reaction.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_tool_call.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_tool_call.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_tracing.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_tracing.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_tracing_filters.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_tracing_filters.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/models/v1_usage_totals.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/models/v1_usage_totals.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/fixpoint_openapi/rest.py` & `fixpoint_openapi-0.4.0/fixpoint_openapi/rest.py`

 * *Files identical despite different names*

### Comparing `fixpoint_openapi-0.3.0/pyproject.toml` & `fixpoint_openapi-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fixpoint_openapi"
-version = "0.3.0"
+version = "0.4.0"
 description = "OpenAPI client for Fixpoint - Auto-improvement to make your LLM apps smarter"
 authors = ["Fixpoint <team@fixpoint.co>"]
 
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: Apache Software License"
 ]
```

### Comparing `fixpoint_openapi-0.3.0/PKG-INFO` & `fixpoint_openapi-0.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixpoint_openapi
-Version: 0.3.0
+Version: 0.4.0
 Summary: OpenAPI client for Fixpoint - Auto-improvement to make your LLM apps smarter
 Home-page: https://github.com/gofixpoint/python-openapi-client
 License: License :: OSI Approved :: Apache Software License
 Keywords: OpenAPI,OpenAPI-Generator
 Author: Fixpoint
 Author-email: team@fixpoint.co
 Requires-Python: >=3.8,<4.0
@@ -88,120 +88,140 @@
 
 
 
 # Enter a context with an instance of the API client
 with fixpoint_openapi.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = fixpoint_openapi.FixpointApi(api_client)
-    body = fixpoint_openapi.V1CreateApiSecretRequest() # V1CreateApiSecretRequest | 
+    body = fixpoint_openapi.V1BatchCreateFineTuneJobsRequest() # V1BatchCreateFineTuneJobsRequest | 
 
     try:
-        # Store LLM inference API secret
-        api_response = api_instance.fixpoint_create_api_secret(body)
-        print("The response of FixpointApi->fixpoint_create_api_secret:\n")
+        api_response = api_instance.fixpoint_batch_create_fine_tune_jobs(body)
+        print("The response of FixpointApi->fixpoint_batch_create_fine_tune_jobs:\n")
         pprint(api_response)
     except ApiException as e:
-        print("Exception when calling FixpointApi->fixpoint_create_api_secret: %s\n" % e)
+        print("Exception when calling FixpointApi->fixpoint_batch_create_fine_tune_jobs: %s\n" % e)
 
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *http://localhost*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
+*FixpointApi* | [**fixpoint_batch_create_fine_tune_jobs**](docs/FixpointApi.md#fixpoint_batch_create_fine_tune_jobs) | **POST** /v1/fine_tune_jobs:batchCreate | 
+*FixpointApi* | [**fixpoint_batch_delete_dataset_logs**](docs/FixpointApi.md#fixpoint_batch_delete_dataset_logs) | **POST** /v1/datasets/{datasetId}/logs:deleteLogs | 
+*FixpointApi* | [**fixpoint_create_ab_chat_completion**](docs/FixpointApi.md#fixpoint_create_ab_chat_completion) | **POST** /v1/chat/completions/ab | Create A/B routed chat completion
 *FixpointApi* | [**fixpoint_create_api_secret**](docs/FixpointApi.md#fixpoint_create_api_secret) | **POST** /v1/api_secrets | Store LLM inference API secret
 *FixpointApi* | [**fixpoint_create_app_logs**](docs/FixpointApi.md#fixpoint_create_app_logs) | **POST** /v1/app_logs | Create application logs
 *FixpointApi* | [**fixpoint_create_dataset**](docs/FixpointApi.md#fixpoint_create_dataset) | **POST** /v1/datasets | Create LLM dataset
 *FixpointApi* | [**fixpoint_create_likes**](docs/FixpointApi.md#fixpoint_create_likes) | **POST** /v1/likes | Add LLM log feedback (\&quot;likes\&quot;)
 *FixpointApi* | [**fixpoint_create_log_attribute**](docs/FixpointApi.md#fixpoint_create_log_attribute) | **POST** /v1/attributes | Attach attribute to LLM log
 *FixpointApi* | [**fixpoint_create_multi_llm_chat_completion**](docs/FixpointApi.md#fixpoint_create_multi_llm_chat_completion) | **POST** /v1/chat/completions/multi_llm | 
 *FixpointApi* | [**fixpoint_create_open_ai_chat_input_log**](docs/FixpointApi.md#fixpoint_create_open_ai_chat_input_log) | **POST** /v1/openai_chats/{modelName}/input_logs | Create an LLM input log
 *FixpointApi* | [**fixpoint_create_open_ai_chat_output_log**](docs/FixpointApi.md#fixpoint_create_open_ai_chat_output_log) | **POST** /v1/openai_chats/{modelName}/output_logs | Create an LLM output log
 *FixpointApi* | [**fixpoint_create_routing_config**](docs/FixpointApi.md#fixpoint_create_routing_config) | **POST** /v1/routing_configs | Create LLM routing config
+*FixpointApi* | [**fixpoint_delete_dataset**](docs/FixpointApi.md#fixpoint_delete_dataset) | **DELETE** /v1/datasets/{datasetId} | 
 *FixpointApi* | [**fixpoint_delete_log_attribute**](docs/FixpointApi.md#fixpoint_delete_log_attribute) | **DELETE** /v1/attributes/{name} | Remove LLM log attribute
 *FixpointApi* | [**fixpoint_list_api_secrets**](docs/FixpointApi.md#fixpoint_list_api_secrets) | **GET** /v1/api_secrets | List LLM inference API secrets
 *FixpointApi* | [**fixpoint_list_app_logs**](docs/FixpointApi.md#fixpoint_list_app_logs) | **GET** /v1/app_logs | List application logs
 *FixpointApi* | [**fixpoint_list_datasets**](docs/FixpointApi.md#fixpoint_list_datasets) | **GET** /v1/datasets | List LLM datasets
+*FixpointApi* | [**fixpoint_list_fine_tune_jobs**](docs/FixpointApi.md#fixpoint_list_fine_tune_jobs) | **GET** /v1/fine_tune_jobs | 
 *FixpointApi* | [**fixpoint_list_likes**](docs/FixpointApi.md#fixpoint_list_likes) | **GET** /v1/likes | List LLM log feedback (\&quot;likes\&quot;)
 *FixpointApi* | [**fixpoint_list_log_attributes**](docs/FixpointApi.md#fixpoint_list_log_attributes) | **GET** /v1/attributes | List attributes on an LLM log
 *FixpointApi* | [**fixpoint_list_open_ai_chat_logs**](docs/FixpointApi.md#fixpoint_list_open_ai_chat_logs) | **GET** /v1/{parent}/logs | DEPRECATED: List LLM logs
 *FixpointApi* | [**fixpoint_list_routing_configs**](docs/FixpointApi.md#fixpoint_list_routing_configs) | **GET** /v1/routing_configs | List LLM routing configs
 *FixpointApi* | [**fixpoint_post_dataset_logs**](docs/FixpointApi.md#fixpoint_post_dataset_logs) | **POST** /v1/datasets/{name}/logs | Add logs to a dataset
-*FixpointApi* | [**fixpoint_update_spending_totals**](docs/FixpointApi.md#fixpoint_update_spending_totals) | **PATCH** /v1/routing_configs/{routeConfigId} | Update routing config spending totals
+*FixpointApi* | [**fixpoint_update_spending_totals**](docs/FixpointApi.md#fixpoint_update_spending_totals) | **PATCH** /v1/routing_configs/{routingConfigId} | Update routing config spending totals
 
 
 ## Documentation For Models
 
  - [AppLogLevelType](docs/AppLogLevelType.md)
+ - [FixpointBatchDeleteDatasetLogsRequest](docs/FixpointBatchDeleteDatasetLogsRequest.md)
  - [FixpointCreateOpenAIChatInputLogRequest](docs/FixpointCreateOpenAIChatInputLogRequest.md)
  - [FixpointCreateOpenAIChatOutputLogRequest](docs/FixpointCreateOpenAIChatOutputLogRequest.md)
  - [FixpointPostDatasetLogsRequest](docs/FixpointPostDatasetLogsRequest.md)
  - [FixpointUpdateSpendingTotalsRequest](docs/FixpointUpdateSpendingTotalsRequest.md)
- - [Fixpointv1Model](docs/Fixpointv1Model.md)
+ - [Fixpointv1SpendCap](docs/Fixpointv1SpendCap.md)
  - [ProtobufAny](docs/ProtobufAny.md)
  - [ProtobufNullValue](docs/ProtobufNullValue.md)
+ - [RoutingBlockAB](docs/RoutingBlockAB.md)
  - [RpcStatus](docs/RpcStatus.md)
  - [ToolCallFunction](docs/ToolCallFunction.md)
+ - [V1AbChatCompletion](docs/V1AbChatCompletion.md)
  - [V1ApiSecret](docs/V1ApiSecret.md)
  - [V1ApiSecretProvider](docs/V1ApiSecretProvider.md)
  - [V1AppLog](docs/V1AppLog.md)
  - [V1AttributeFilters](docs/V1AttributeFilters.md)
+ - [V1BatchCreateFineTuneJobsRequest](docs/V1BatchCreateFineTuneJobsRequest.md)
+ - [V1BatchCreateFineTuneJobsResponse](docs/V1BatchCreateFineTuneJobsResponse.md)
  - [V1ChatCompletion](docs/V1ChatCompletion.md)
  - [V1ChatCompletionChoice](docs/V1ChatCompletionChoice.md)
  - [V1ChatCompletionUsage](docs/V1ChatCompletionUsage.md)
+ - [V1CreateABChatCompletionRequest](docs/V1CreateABChatCompletionRequest.md)
  - [V1CreateApiSecretRequest](docs/V1CreateApiSecretRequest.md)
  - [V1CreateAppLogsRequest](docs/V1CreateAppLogsRequest.md)
  - [V1CreateAppLogsResponse](docs/V1CreateAppLogsResponse.md)
  - [V1CreateDatasetRequest](docs/V1CreateDatasetRequest.md)
  - [V1CreateDatasetResponse](docs/V1CreateDatasetResponse.md)
  - [V1CreateLikesRequest](docs/V1CreateLikesRequest.md)
  - [V1CreateLikesResponse](docs/V1CreateLikesResponse.md)
  - [V1CreateLogAttributeRequest](docs/V1CreateLogAttributeRequest.md)
  - [V1CreateLogAttributeResponse](docs/V1CreateLogAttributeResponse.md)
  - [V1CreateMultiLLMChatCompletionRequest](docs/V1CreateMultiLLMChatCompletionRequest.md)
- - [V1CreateMultiLLMChatCompletionRequestModel](docs/V1CreateMultiLLMChatCompletionRequestModel.md)
  - [V1CreateRoutingConfigRequest](docs/V1CreateRoutingConfigRequest.md)
  - [V1Dataset](docs/V1Dataset.md)
  - [V1DatasetFilters](docs/V1DatasetFilters.md)
+ - [V1DeleteDatasetLogsResponse](docs/V1DeleteDatasetLogsResponse.md)
+ - [V1DeleteDatasetResponse](docs/V1DeleteDatasetResponse.md)
  - [V1DeleteLogAttributeResponse](docs/V1DeleteLogAttributeResponse.md)
  - [V1FallbackStrategy](docs/V1FallbackStrategy.md)
+ - [V1FineTuneJob](docs/V1FineTuneJob.md)
+ - [V1FineTuneStatus](docs/V1FineTuneStatus.md)
+ - [V1Hyperparameters](docs/V1Hyperparameters.md)
  - [V1InputMessage](docs/V1InputMessage.md)
  - [V1Like](docs/V1Like.md)
  - [V1LikeFilter](docs/V1LikeFilter.md)
  - [V1LikeIngest](docs/V1LikeIngest.md)
  - [V1ListApiSecretsResponse](docs/V1ListApiSecretsResponse.md)
  - [V1ListAppLogsResponse](docs/V1ListAppLogsResponse.md)
  - [V1ListDatasetsResponse](docs/V1ListDatasetsResponse.md)
+ - [V1ListFineTuneJobsResponse](docs/V1ListFineTuneJobsResponse.md)
  - [V1ListLikesResponse](docs/V1ListLikesResponse.md)
  - [V1ListLogAttributesResponse](docs/V1ListLogAttributesResponse.md)
  - [V1ListOpenAIChatLogsResponse](docs/V1ListOpenAIChatLogsResponse.md)
  - [V1ListRoutingConfigsResponse](docs/V1ListRoutingConfigsResponse.md)
  - [V1LogAttribute](docs/V1LogAttribute.md)
  - [V1Mode](docs/V1Mode.md)
+ - [V1Model](docs/V1Model.md)
  - [V1MultiLLMChatCompletion](docs/V1MultiLLMChatCompletion.md)
  - [V1OpenAIChatInputLog](docs/V1OpenAIChatInputLog.md)
  - [V1OpenAIChatLog](docs/V1OpenAIChatLog.md)
  - [V1OpenAIChatLogsFilters](docs/V1OpenAIChatLogsFilters.md)
  - [V1OpenAIChatOutputLog](docs/V1OpenAIChatOutputLog.md)
  - [V1OpenAIChatOutputLogChoice](docs/V1OpenAIChatOutputLogChoice.md)
  - [V1OpenAIChatOutputLogUsage](docs/V1OpenAIChatOutputLogUsage.md)
  - [V1OriginType](docs/V1OriginType.md)
  - [V1OutputMessage](docs/V1OutputMessage.md)
  - [V1PostDatasetLogsResponse](docs/V1PostDatasetLogsResponse.md)
  - [V1RelativeDateTimeFilters](docs/V1RelativeDateTimeFilters.md)
  - [V1ResetInterval](docs/V1ResetInterval.md)
+ - [V1RoutingBlock](docs/V1RoutingBlock.md)
+ - [V1RoutingBlockSpendCap](docs/V1RoutingBlockSpendCap.md)
+ - [V1RoutingBlockType](docs/V1RoutingBlockType.md)
  - [V1RoutingConfig](docs/V1RoutingConfig.md)
- - [V1SpendCap](docs/V1SpendCap.md)
+ - [V1SpendCapModel](docs/V1SpendCapModel.md)
  - [V1TerminalState](docs/V1TerminalState.md)
  - [V1ThumbsReaction](docs/V1ThumbsReaction.md)
  - [V1ToolCall](docs/V1ToolCall.md)
  - [V1Tracing](docs/V1Tracing.md)
  - [V1TracingFilters](docs/V1TracingFilters.md)
+ - [V1TuningConfiguration](docs/V1TuningConfiguration.md)
  - [V1UsageTotals](docs/V1UsageTotals.md)
 
 
 <a id="documentation-for-authorization"></a>
 ## Documentation For Authorization
 
 Endpoints do not require authorization.
```

