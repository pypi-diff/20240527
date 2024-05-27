# Comparing `tmp/dspy-ai-2.4.9.tar.gz` & `tmp/dspy_ai-2.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dspy-ai-2.4.9.tar", last modified: Mon Apr 29 20:58:33 2024, max compression
+gzip compressed data, was "dspy_ai-2.5.0rc1.tar", max compression
```

## Comparing `dspy-ai-2.4.9.tar` & `dspy_ai-2.5.0rc1.tar`

### file list

```diff
@@ -1,167 +1,92 @@
-drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.829986 dspy-ai-2.4.9/
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     1085 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/LICENSE
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    36243 2024-04-29 20:58:33.829986 dspy-ai-2.4.9/PKG-INFO
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    35291 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/README.md
-drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.805975 dspy-ai-2.4.9/dsp/
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     1532 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/__init__.py
-drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.805975 dspy-ai-2.4.9/dsp/evaluation/
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)        1 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/evaluation/__init__.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     2586 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/evaluation/utils.py
-drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.813979 dspy-ai-2.4.9/dsp/modules/
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      760 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/__init__.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     4439 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/anthropic.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    10296 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/aws_models.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     4525 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/aws_providers.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     9756 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/azure_openai.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3135 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/azurecognitivesearch.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     1018 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/cache_utils.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3008 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/clarifai.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3313 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/cohere.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     2156 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/colbertv2.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     5278 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/databricks.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3788 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/dummy_lm.py
-drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.813979 dspy-ai-2.4.9/dsp/modules/finetuning/
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)       26 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/finetuning/__init__.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    15071 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/finetuning/finetune_hf.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     4552 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/google.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     5992 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/googlevertexai.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     8562 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/gpt3.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     4859 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/groq_client.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     8119 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/hf.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    17704 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/hf_client.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     2087 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/hf_server.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3721 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/lm.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3655 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/mistral.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     6751 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/ollama.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3152 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/pyserini.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      693 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/sbert.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     7787 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/sentence_vectorizer.py
-drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.813979 dspy-ai-2.4.9/dsp/primitives/
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      145 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/primitives/__init__.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     5185 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/primitives/compiler.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     5789 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/primitives/demonstrate.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     2471 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/primitives/inspect.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     8432 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/primitives/predict.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     1439 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/primitives/primitives.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     2727 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/primitives/search.py
-drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.813979 dspy-ai-2.4.9/dsp/templates/
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)       76 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/templates/__init__.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    10226 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/templates/template_v2.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     2334 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/templates/template_v3.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     1900 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/templates/utils.py
-drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.813979 dspy-ai-2.4.9/dsp/utils/
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      123 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/utils/__init__.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     4903 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/utils/ann_utils.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     7110 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/utils/dpr.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     5933 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/utils/metrics.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3215 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/utils/settings.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     2828 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/utils/settings_v2.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     5623 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/utils/utils.py
-drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.813979 dspy-ai-2.4.9/dspy/
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     1059 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/__init__.py
-drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.813979 dspy-ai-2.4.9/dspy/adapters/
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/adapters/__init__.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/adapters/basic_adapter.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/adapters/chatml_adapter.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/adapters/llamachat_adapter.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/adapters/vicuna_adapter.py
-drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.817980 dspy-ai-2.4.9/dspy/datasets/
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      122 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/datasets/__init__.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     2986 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/datasets/colors.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     4949 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/datasets/dataloader.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     4098 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/datasets/dataset.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     2618 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/datasets/gsm8k.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3286 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/datasets/hotpotqa.py
-drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.817980 dspy-ai-2.4.9/dspy/evaluate/
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      127 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/evaluate/__init__.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     1421 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/evaluate/auto_evaluation.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    10081 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/evaluate/evaluate.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      882 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/evaluate/metrics.py
-drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.817980 dspy-ai-2.4.9/dspy/experimental/
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)       57 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/experimental/__init__.py
-drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.817980 dspy-ai-2.4.9/dspy/experimental/synthesizer/
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)       26 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/experimental/synthesizer/__init__.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      834 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/experimental/synthesizer/config.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      527 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/experimental/synthesizer/instruction_suffixes.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     5543 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/experimental/synthesizer/signatures.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     9723 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/experimental/synthesizer/synthesizer.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      599 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/experimental/synthesizer/utils.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     4237 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/experimental/synthetic_data.py
-drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.817980 dspy-ai-2.4.9/dspy/functional/
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)       94 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/functional/__init__.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    19499 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/functional/functional.py
-drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.817980 dspy-ai-2.4.9/dspy/predict/
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      348 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/predict/__init__.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     1842 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/predict/aggregation.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3589 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/predict/chain_of_thought.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     1527 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/predict/chain_of_thought_with_hint.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     1017 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/predict/knn.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     6117 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/predict/langchain.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     1659 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/predict/multi_chain_comparison.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)       58 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/predict/parameter.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     5580 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/predict/predict.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     7603 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/predict/program_of_thought.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     4458 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/predict/react.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     2827 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/predict/retry.py
-drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.821982 dspy-ai-2.4.9/dspy/primitives/
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      132 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/primitives/__init__.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    11407 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/primitives/assertions.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     7779 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/primitives/box.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3471 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/primitives/example.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3831 2024-04-29 20:58:28.000000 dspy-ai-2.4.9/dspy/primitives/module.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     2807 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/primitives/prediction.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3366 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/primitives/program.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    25710 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/primitives/python_interpreter.py
-drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.825984 dspy-ai-2.4.9/dspy/retrieve/
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)       30 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/__init__.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    17405 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/azureaisearch_rm.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     5719 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/chromadb_rm.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3275 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/clarifai_rm.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     6604 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/databricks_rm.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3897 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/deeplake_rm.py
--rwxrwxr-x   0 okhattab  (1000) okhattab  (1000)     6605 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/faiss_rm.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3459 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/marqo_rm.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3998 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/milvus_rm.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3774 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/mongodb_atlas_rm.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     6213 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/neo4j_rm.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     5930 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/pgvector_rm.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    10476 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/pinecone_rm.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3271 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/qdrant_rm.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     2425 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/ragatouille_rm.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     1442 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/retrieve.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     5659 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/vectara_rm.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     4491 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/weaviate_rm.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      438 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/weaviate_rm_test.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     1678 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/you_rm.py
-drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.825984 dspy-ai-2.4.9/dspy/signatures/
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)       46 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/signatures/__init__.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     2758 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/signatures/field.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    14464 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/signatures/signature.py
-drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.825984 dspy-ai-2.4.9/dspy/teleprompt/
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      390 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/teleprompt/__init__.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     9532 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/teleprompt/bootstrap.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    17739 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/teleprompt/copro_optimizer.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     1359 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/teleprompt/ensemble.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     6292 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/teleprompt/finetune.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      879 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/teleprompt/knn_fewshot.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    31087 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/teleprompt/mipro_optimizer.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     8130 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/teleprompt/random_search.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     2673 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/teleprompt/signature_opt.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3878 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/teleprompt/signature_opt_bayesian.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    11876 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/teleprompt/signature_opt_typed.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)       57 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/teleprompt/teleprompt.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3208 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/teleprompt/teleprompt_optuna.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      948 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/teleprompt/vanilla.py
-drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.825984 dspy-ai-2.4.9/dspy/utils/
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)       46 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/utils/__init__.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     5643 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/utils/dummies.py
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3193 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/utils/logging.py
-drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.829986 dspy-ai-2.4.9/dspy_ai.egg-info/
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    36243 2024-04-29 20:58:33.000000 dspy-ai-2.4.9/dspy_ai.egg-info/PKG-INFO
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3981 2024-04-29 20:58:33.000000 dspy-ai-2.4.9/dspy_ai.egg-info/SOURCES.txt
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)        1 2024-04-29 20:58:33.000000 dspy-ai-2.4.9/dspy_ai.egg-info/dependency_links.txt
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      766 2024-04-29 20:58:33.000000 dspy-ai-2.4.9/dspy_ai.egg-info/requires.txt
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)        9 2024-04-29 20:58:33.000000 dspy-ai-2.4.9/dspy_ai.egg-info/top_level.txt
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     7322 2024-04-29 20:58:28.000000 dspy-ai-2.4.9/pyproject.toml
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)       38 2024-04-29 20:58:33.829986 dspy-ai-2.4.9/setup.cfg
--rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     1599 2024-04-29 20:58:28.000000 dspy-ai-2.4.9/setup.py
+-rw-r--r--   0        0        0     1085 2024-01-27 20:16:46.845164 dspy_ai-2.5.0rc1/LICENSE
+-rw-r--r--   0        0        0    35950 2024-05-27 13:53:59.380701 dspy_ai-2.5.0rc1/README.md
+-rw-r--r--   0        0        0     1180 2024-05-27 13:54:02.462908 dspy_ai-2.5.0rc1/dspy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 13:54:02.462971 dspy_ai-2.5.0rc1/dspy/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 13:54:02.463017 dspy_ai-2.5.0rc1/dspy/adapters/basic_adapter.py
+-rw-r--r--   0        0        0        0 2024-05-27 13:54:02.463052 dspy_ai-2.5.0rc1/dspy/adapters/chatml_adapter.py
+-rw-r--r--   0        0        0        0 2024-05-27 13:54:02.463085 dspy_ai-2.5.0rc1/dspy/adapters/llamachat_adapter.py
+-rw-r--r--   0        0        0        0 2024-05-27 13:54:02.463120 dspy_ai-2.5.0rc1/dspy/adapters/vicuna_adapter.py
+-rw-r--r--   0        0        0      122 2024-04-05 16:07:52.848121 dspy_ai-2.5.0rc1/dspy/datasets/__init__.py
+-rw-r--r--   0        0        0     2986 2024-04-05 16:07:52.848222 dspy_ai-2.5.0rc1/dspy/datasets/colors.py
+-rw-r--r--   0        0        0     4949 2024-05-27 13:54:02.463273 dspy_ai-2.5.0rc1/dspy/datasets/dataloader.py
+-rw-r--r--   0        0        0     4098 2024-04-05 16:07:52.848414 dspy_ai-2.5.0rc1/dspy/datasets/dataset.py
+-rw-r--r--   0        0        0     2618 2024-04-05 16:07:52.848498 dspy_ai-2.5.0rc1/dspy/datasets/gsm8k.py
+-rw-r--r--   0        0        0     3286 2024-04-05 16:07:52.848598 dspy_ai-2.5.0rc1/dspy/datasets/hotpotqa.py
+-rw-r--r--   0        0        0      127 2024-04-05 16:07:52.848699 dspy_ai-2.5.0rc1/dspy/evaluate/__init__.py
+-rw-r--r--   0        0        0     1421 2024-04-05 16:07:52.848822 dspy_ai-2.5.0rc1/dspy/evaluate/auto_evaluation.py
+-rw-r--r--   0        0        0    11414 2024-05-27 13:53:59.390403 dspy_ai-2.5.0rc1/dspy/evaluate/evaluate.py
+-rw-r--r--   0        0        0      882 2024-04-05 16:07:52.852527 dspy_ai-2.5.0rc1/dspy/evaluate/metrics.py
+-rw-r--r--   0        0        0       57 2024-04-05 16:07:52.852610 dspy_ai-2.5.0rc1/dspy/experimental/__init__.py
+-rw-r--r--   0        0        0       26 2024-04-05 16:07:52.852700 dspy_ai-2.5.0rc1/dspy/experimental/synthesizer/__init__.py
+-rw-r--r--   0        0        0      834 2024-04-05 16:07:52.852759 dspy_ai-2.5.0rc1/dspy/experimental/synthesizer/config.py
+-rw-r--r--   0        0        0      527 2024-04-05 16:07:52.852825 dspy_ai-2.5.0rc1/dspy/experimental/synthesizer/instruction_suffixes.py
+-rw-r--r--   0        0        0     5543 2024-04-05 16:07:52.852897 dspy_ai-2.5.0rc1/dspy/experimental/synthesizer/signatures.py
+-rw-r--r--   0        0        0     9723 2024-05-27 13:54:02.463457 dspy_ai-2.5.0rc1/dspy/experimental/synthesizer/synthesizer.py
+-rw-r--r--   0        0        0      599 2024-04-05 16:07:52.853143 dspy_ai-2.5.0rc1/dspy/experimental/synthesizer/utils.py
+-rw-r--r--   0        0        0     4237 2024-05-27 13:53:59.390647 dspy_ai-2.5.0rc1/dspy/experimental/synthetic_data.py
+-rw-r--r--   0        0        0       94 2024-04-05 16:07:52.853820 dspy_ai-2.5.0rc1/dspy/functional/__init__.py
+-rw-r--r--   0        0        0    19491 2024-05-27 13:54:02.463645 dspy_ai-2.5.0rc1/dspy/functional/functional.py
+-rw-r--r--   0        0        0      348 2024-04-05 16:07:52.854456 dspy_ai-2.5.0rc1/dspy/predict/__init__.py
+-rw-r--r--   0        0        0     1842 2024-05-27 13:54:02.463800 dspy_ai-2.5.0rc1/dspy/predict/aggregation.py
+-rw-r--r--   0        0        0     3589 2024-04-05 16:07:52.854648 dspy_ai-2.5.0rc1/dspy/predict/chain_of_thought.py
+-rw-r--r--   0        0        0     1527 2024-04-05 16:07:52.854742 dspy_ai-2.5.0rc1/dspy/predict/chain_of_thought_with_hint.py
+-rw-r--r--   0        0        0     1133 2024-05-27 13:53:59.392833 dspy_ai-2.5.0rc1/dspy/predict/knn.py
+-rw-r--r--   0        0        0     6129 2024-05-27 13:53:59.392953 dspy_ai-2.5.0rc1/dspy/predict/langchain.py
+-rw-r--r--   0        0        0     1659 2024-04-05 16:07:52.855060 dspy_ai-2.5.0rc1/dspy/predict/multi_chain_comparison.py
+-rw-r--r--   0        0        0       58 2024-01-27 20:16:47.215842 dspy_ai-2.5.0rc1/dspy/predict/parameter.py
+-rw-r--r--   0        0        0     5580 2024-05-27 13:54:02.463936 dspy_ai-2.5.0rc1/dspy/predict/predict.py
+-rw-r--r--   0        0        0     7603 2024-05-27 13:54:02.464078 dspy_ai-2.5.0rc1/dspy/predict/program_of_thought.py
+-rw-r--r--   0        0        0     4614 2024-05-27 13:53:59.393278 dspy_ai-2.5.0rc1/dspy/predict/react.py
+-rw-r--r--   0        0        0     2977 2024-05-27 13:54:02.464208 dspy_ai-2.5.0rc1/dspy/predict/retry.py
+-rw-r--r--   0        0        0      132 2024-04-05 16:07:52.855575 dspy_ai-2.5.0rc1/dspy/primitives/__init__.py
+-rw-r--r--   0        0        0    11319 2024-05-27 13:53:59.393559 dspy_ai-2.5.0rc1/dspy/primitives/assertions.py
+-rw-r--r--   0        0        0     7779 2024-01-27 20:16:47.216399 dspy_ai-2.5.0rc1/dspy/primitives/box.py
+-rw-r--r--   0        0        0     3471 2024-05-27 13:54:02.464335 dspy_ai-2.5.0rc1/dspy/primitives/example.py
+-rw-r--r--   0        0        0     3831 2024-05-27 13:53:59.393756 dspy_ai-2.5.0rc1/dspy/primitives/module.py
+-rw-r--r--   0        0        0     2807 2024-05-27 13:54:02.464463 dspy_ai-2.5.0rc1/dspy/primitives/prediction.py
+-rw-r--r--   0        0        0     3366 2024-04-05 16:07:52.856229 dspy_ai-2.5.0rc1/dspy/primitives/program.py
+-rw-r--r--   0        0        0    25710 2024-04-05 16:07:52.856677 dspy_ai-2.5.0rc1/dspy/primitives/python_interpreter.py
+-rw-r--r--   0        0        0       30 2024-01-27 20:16:47.216808 dspy_ai-2.5.0rc1/dspy/retrieve/__init__.py
+-rw-r--r--   0        0        0    17405 2024-05-27 13:53:59.393937 dspy_ai-2.5.0rc1/dspy/retrieve/azureaisearch_rm.py
+-rw-r--r--   0        0        0     5719 2024-05-27 13:54:02.464622 dspy_ai-2.5.0rc1/dspy/retrieve/chromadb_rm.py
+-rw-r--r--   0        0        0     3275 2024-05-27 13:54:02.464778 dspy_ai-2.5.0rc1/dspy/retrieve/clarifai_rm.py
+-rw-r--r--   0        0        0     6604 2024-05-27 13:53:59.394297 dspy_ai-2.5.0rc1/dspy/retrieve/databricks_rm.py
+-rw-r--r--   0        0        0     3897 2024-05-27 13:54:02.464886 dspy_ai-2.5.0rc1/dspy/retrieve/deeplake_rm.py
+-rwxr-xr-x   0        0        0     6605 2024-05-27 13:53:59.394532 dspy_ai-2.5.0rc1/dspy/retrieve/faiss_rm.py
+-rw-r--r--   0        0        0     2937 2024-05-27 13:53:59.394597 dspy_ai-2.5.0rc1/dspy/retrieve/llama_index_rm.py
+-rw-r--r--   0        0        0     3459 2024-04-05 16:07:52.857777 dspy_ai-2.5.0rc1/dspy/retrieve/marqo_rm.py
+-rw-r--r--   0        0        0     3998 2024-05-27 13:53:59.394660 dspy_ai-2.5.0rc1/dspy/retrieve/milvus_rm.py
+-rw-r--r--   0        0        0     3774 2024-04-05 16:07:52.857887 dspy_ai-2.5.0rc1/dspy/retrieve/mongodb_atlas_rm.py
+-rw-r--r--   0        0        0     6213 2024-04-05 16:07:52.857964 dspy_ai-2.5.0rc1/dspy/retrieve/neo4j_rm.py
+-rw-r--r--   0        0        0     5930 2024-05-27 13:54:02.465032 dspy_ai-2.5.0rc1/dspy/retrieve/pgvector_rm.py
+-rw-r--r--   0        0        0    10476 2024-04-05 16:07:52.858267 dspy_ai-2.5.0rc1/dspy/retrieve/pinecone_rm.py
+-rw-r--r--   0        0        0     4951 2024-05-27 13:53:59.394882 dspy_ai-2.5.0rc1/dspy/retrieve/qdrant_rm.py
+-rw-r--r--   0        0        0     2425 2024-05-27 13:53:59.394959 dspy_ai-2.5.0rc1/dspy/retrieve/ragatouille_rm.py
+-rw-r--r--   0        0        0     1442 2024-05-27 13:54:02.465140 dspy_ai-2.5.0rc1/dspy/retrieve/retrieve.py
+-rw-r--r--   0        0        0     4575 2024-05-27 13:53:59.395131 dspy_ai-2.5.0rc1/dspy/retrieve/snowflake_rm.py
+-rw-r--r--   0        0        0     5923 2024-05-27 13:53:59.395244 dspy_ai-2.5.0rc1/dspy/retrieve/vectara_rm.py
+-rw-r--r--   0        0        0     4491 2024-05-27 13:54:02.465274 dspy_ai-2.5.0rc1/dspy/retrieve/weaviate_rm.py
+-rw-r--r--   0        0        0      438 2024-02-10 21:45:26.556459 dspy_ai-2.5.0rc1/dspy/retrieve/weaviate_rm_test.py
+-rw-r--r--   0        0        0     1678 2024-04-05 16:07:52.859233 dspy_ai-2.5.0rc1/dspy/retrieve/you_rm.py
+-rw-r--r--   0        0        0       46 2024-01-27 20:16:47.217346 dspy_ai-2.5.0rc1/dspy/signatures/__init__.py
+-rw-r--r--   0        0        0     2758 2024-04-05 16:07:52.859642 dspy_ai-2.5.0rc1/dspy/signatures/field.py
+-rw-r--r--   0        0        0    14509 2024-05-27 13:54:02.465439 dspy_ai-2.5.0rc1/dspy/signatures/signature.py
+-rw-r--r--   0        0        0      390 2024-04-05 16:07:52.860050 dspy_ai-2.5.0rc1/dspy/teleprompt/__init__.py
+-rw-r--r--   0        0        0    10819 2024-05-27 13:54:02.465612 dspy_ai-2.5.0rc1/dspy/teleprompt/bootstrap.py
+-rw-r--r--   0        0        0    18048 2024-05-27 13:54:02.465752 dspy_ai-2.5.0rc1/dspy/teleprompt/copro_optimizer.py
+-rw-r--r--   0        0        0     1359 2024-04-05 16:07:52.860514 dspy_ai-2.5.0rc1/dspy/teleprompt/ensemble.py
+-rw-r--r--   0        0        0     6292 2024-04-05 16:07:52.860625 dspy_ai-2.5.0rc1/dspy/teleprompt/finetune.py
+-rw-r--r--   0        0        0     1002 2024-05-27 13:53:59.396186 dspy_ai-2.5.0rc1/dspy/teleprompt/knn_fewshot.py
+-rw-r--r--   0        0        0    31123 2024-05-27 13:54:02.465932 dspy_ai-2.5.0rc1/dspy/teleprompt/mipro_optimizer.py
+-rw-r--r--   0        0        0     8130 2024-05-27 13:53:59.396477 dspy_ai-2.5.0rc1/dspy/teleprompt/random_search.py
+-rw-r--r--   0        0        0     2673 2024-05-27 13:53:59.396900 dspy_ai-2.5.0rc1/dspy/teleprompt/signature_opt.py
+-rw-r--r--   0        0        0     3878 2024-04-05 16:07:52.861256 dspy_ai-2.5.0rc1/dspy/teleprompt/signature_opt_bayesian.py
+-rw-r--r--   0        0        0    11876 2024-04-05 16:07:52.861442 dspy_ai-2.5.0rc1/dspy/teleprompt/signature_opt_typed.py
+-rw-r--r--   0        0        0       57 2024-04-05 16:07:52.861522 dspy_ai-2.5.0rc1/dspy/teleprompt/teleprompt.py
+-rw-r--r--   0        0        0     3206 2024-05-27 13:53:59.397045 dspy_ai-2.5.0rc1/dspy/teleprompt/teleprompt_optuna.py
+-rw-r--r--   0        0        0      948 2024-04-05 16:07:52.861703 dspy_ai-2.5.0rc1/dspy/teleprompt/vanilla.py
+-rw-r--r--   0        0        0       46 2024-05-27 13:53:59.397185 dspy_ai-2.5.0rc1/dspy/utils/__init__.py
+-rw-r--r--   0        0        0     5643 2024-05-27 13:54:02.466118 dspy_ai-2.5.0rc1/dspy/utils/dummies.py
+-rw-r--r--   0        0        0     3193 2024-05-27 13:53:59.397403 dspy_ai-2.5.0rc1/dspy/utils/logging.py
+-rw-r--r--   0        0        0     7736 2024-05-27 14:12:47.032650 dspy_ai-2.5.0rc1/pyproject.toml
+-rw-r--r--   0        0        0    38956 1970-01-01 00:00:00.000000 dspy_ai-2.5.0rc1/PKG-INFO
```

### Comparing `dspy-ai-2.4.9/LICENSE` & `dspy_ai-2.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/PKG-INFO` & `dspy_ai-2.5.0rc1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: dspy-ai
-Version: 2.4.9
-Summary: DSPy
-Home-page: https://github.com/stanfordnlp/dsp
-Author: Omar Khattab
-Author-email: Omar Khattab <okhattab@stanford.edu>
-License: MIT License
-Project-URL: homepage, https://github.com/stanfordnlp/dspy
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: chromadb
-Provides-Extra: qdrant
-Provides-Extra: marqo
-Provides-Extra: mongodb
-Provides-Extra: pinecone
-Provides-Extra: weaviate
-Provides-Extra: faiss-cpu
-Provides-Extra: milvus
-Provides-Extra: google-vertex-ai
-Provides-Extra: anthropic
-Provides-Extra: aws
-Provides-Extra: docs
-Provides-Extra: dev
-License-File: LICENSE
-
 <p align="center">
   <img align="center" src="docs/images/DSPy8.png" width="460px" />
 </p>
 <p align="left">
 
 
 ## DSPy: _Programming_—not prompting—Foundation Models
@@ -100,19 +68,19 @@
 pip install git+https://github.com/stanfordnlp/dspy.git
 ````
 
 Or open our intro notebook in Google Colab: [<img align="center" src="https://colab.research.google.com/assets/colab-badge.svg" />](https://colab.research.google.com/github/stanfordnlp/dspy/blob/main/intro.ipynb)
 
 By default, DSPy installs the latest `openai` from pip. However, if you install old version before OpenAI changed their API `openai~=0.28.1`, the library will use that just fine. Both are supported.
 
-For the optional (alphabetically sorted) [Chromadb](https://github.com/chroma-core/chroma), [Qdrant](https://github.com/qdrant/qdrant), [Marqo](https://github.com/marqo-ai/marqo), Pinecone, [Weaviate](https://github.com/weaviate/weaviate),
+For the optional (alphabetically sorted) [Chromadb](https://github.com/chroma-core/chroma), [Qdrant](https://github.com/qdrant/qdrant), [Marqo](https://github.com/marqo-ai/marqo), Pinecone, [Snowflake](https://github.com/snowflakedb/snowpark-python) [Weaviate](https://github.com/weaviate/weaviate),
 or [Milvus](https://github.com/milvus-io/milvus) retrieval integration(s), include the extra(s) below:
 
 ```
-pip install dspy-ai[chromadb]  # or [qdrant] or [marqo] or [mongodb] or [pinecone] or [weaviate] or [milvus]
+pip install dspy-ai[chromadb]  # or [qdrant] or [marqo] or [mongodb] or [pinecone] or [snowflake] or [weaviate] or [milvus]
 ```
 
 ## 2) Documentation
 
 The DSPy documentation is divided into **tutorials** (step-by-step illustration of solving a task in DSPy), **guides** (how to use specific parts of the API), and **examples** (self-contained programs that illustrate usage).
 
 ### A) Tutorials
@@ -129,18 +97,19 @@
 | Advanced | [**Information Extraction**](https://twitter.com/KarelDoostrlnck/status/1724991014207930696) | [<img align="center" src="https://colab.research.google.com/assets/colab-badge.svg" />](https://colab.research.google.com/drive/1CpsOiLiLYKeGrhmq579_FmtGsD5uZ3Qe) | Tackles extracting information from long articles (biomedical research papers). Combines in-context learning and retrieval to set SOTA on BioDEX. Contributed by [Karel D’Oosterlinck](https://twitter.com/KarelDoostrlnck/status/1724991014207930696).  |
 
 
 **Other resources people find useful**:
 
 - [DSPy talk at ScaleByTheBay Nov 2023](https://www.youtube.com/watch?v=Dt3H2ninoeY).
 - [DSPy webinar with MLOps Learners](https://www.youtube.com/watch?v=im7bCLW2aM4), a bit longer with Q&A.
-- Hands-on Overviews of DSPy by the community: [DSPy Explained! by Connor Shorten](https://www.youtube.com/watch?v=41EfOY0Ldkc), [DSPy explained by code_your_own_ai](https://www.youtube.com/watch?v=ycfnKPxBMck), [DSPy Crash Course by AI Bites](https://youtu.be/5-zgASQKkKQ?si=3gnmVouT5_rpk_nu)
+- Hands-on Overviews of DSPy by the community: [DSPy Explained! by Connor Shorten](https://www.youtube.com/watch?v=41EfOY0Ldkc), [DSPy explained by code_your_own_ai](https://www.youtube.com/watch?v=ycfnKPxBMck), [DSPy Crash Course by AI Bites](https://youtu.be/5-zgASQKkKQ?si=3gnmVouT5_rpk_nu), [DSPy Paper Explained by Unify](https://youtu.be/kFB8kFchCH4?si=FuM6L5H5lweanckz)
 - Interviews: [Weaviate Podcast in-person](https://www.youtube.com/watch?v=CDung1LnLbY), and you can find 6-7 other remote podcasts on YouTube from a few different perspectives/audiences.
 - **Tracing in DSPy** with Arize Phoenix: [Tutorial for tracing your prompts and the steps of your DSPy programs](https://colab.research.google.com/github/Arize-ai/phoenix/blob/main/tutorials/tracing/dspy_tracing_tutorial.ipynb)
 - [DSPy: Not Your Average Prompt Engineering](https://jina.ai/news/dspy-not-your-average-prompt-engineering), why it's crucial for future prompt engineering, and yet why it is challenging for prompt engineers to learn.
+- **Tracing & Optimization Tracking in DSPy** with Parea AI: [Tutorial on tracing & evaluating a DSPy RAG program](https://docs.parea.ai/tutorials/dspy-rag-trace-evaluate/tutorial)
 
 ### B) Guides
 
 If you're new to DSPy, it's probably best to go in sequential order. You will probably refer to these guides frequently after that, e.g. to copy/paste snippets that you can edit for your own DSPy programs.
 
 
 1. **[Language Models](https://dspy-docs.vercel.app/docs/building-blocks/language_models)**
@@ -164,32 +133,36 @@
 
 There's a bunch of examples in the `examples/` directory and in the top-level directory. We welcome contributions!
 
 You can find other examples tweeted by [@lateinteraction](https://twitter.com/lateinteraction) on Twitter/X.
 
 **Some other examples (not exhaustive, feel free to add more via PR):**
 
+
+- [DSPy Optimizers Benchmark on a bunch of different tasks, by Michael Ryan](https://github.com/stanfordnlp/dspy/tree/main/testing/tasks)
+- [Sophisticated Extreme Multi-Class Classification, IReRa, by Karel D’Oosterlinck](https://github.com/KarelDO/xmc.dspy)
+- [Haize Lab's Red Teaming with DSPy](https://blog.haizelabs.com/posts/dspy/) and see [their DSPy code](https://github.com/haizelabs/dspy-redteam)
 - Applying DSPy Assertions
   - [Long-form Answer Generation with Citations, by Arnav Singhvi](https://colab.research.google.com/github/stanfordnlp/dspy/blob/main/examples/longformqa/longformqa_assertions.ipynb)
   - [Generating Answer Choices for Quiz Questions, by Arnav Singhvi](https://colab.research.google.com/github/stanfordnlp/dspy/blob/main/examples/quiz/quiz_assertions.ipynb)
   - [Generating Tweets for QA, by Arnav Singhvi](https://colab.research.google.com/github/stanfordnlp/dspy/blob/main/examples/tweets/tweets_assertions.ipynb)
 - [Compiling LCEL runnables from LangChain in DSPy](https://github.com/stanfordnlp/dspy/blob/main/examples/tweets/compiling_langchain.ipynb)
 - [AI feedback, or writing LM-based metrics in DSPy](https://github.com/stanfordnlp/dspy/blob/main/examples/tweets/tweet_metric.py)
-- [DSPy Optimizers Benchmark on a bunch of different tasks, by Michael Ryan](https://github.com/stanfordnlp/dspy/tree/main/testing/tasks)
+- [DSPy Optimizers Benchmark on a bunch of different tasks, by Michael Ryan](https://github.com/stanfordnlp/dspy/tree/main/testing/README.md)
 - [Indian Languages NLI with gains due to compiling by Saiful Haq](https://github.com/saifulhaq95/DSPy-Indic/blob/main/indicxlni.ipynb)
-- [Sophisticated Extreme Multi-Class Classification, IReRa, by Karel D’Oosterlinck](https://github.com/KarelDO/xmc.dspy)
 - [DSPy on BIG-Bench Hard Example, by Chris Levy](https://drchrislevy.github.io/posts/dspy/dspy.html)
 - [Using Ollama with DSPy for Mistral (quantized) by @jrknox1977](https://gist.github.com/jrknox1977/78c17e492b5a75ee5bbaf9673aee4641)
-- [Using DSPy, "The Unreasonable Effectiveness of Eccentric Automatic Prompts" (paper) by VMware's Rick Battle & Teja Gollapudi, and interview at TheRegister](https://www.theregister.com/2024/02/22/prompt_engineering_ai_models/)
+- [Using DSPy, "The Unreasonable Effectiveness of Eccentric Automatic Prompts" (paper) by VMware's Rick Battle & Teja Gollapudi](https://arxiv.org/abs/2402.10949), and [interview at TheRegister](https://www.theregister.com/2024/02/22/prompt_engineering_ai_models/)
 - [Optimizing Performance of Open Source LM for Text-to-SQL using DSPy and vLLM, by Juan Ovalle](https://github.com/jjovalle99/DSPy-Text2SQL)
 - Typed DSPy (contributed by [@normal-computing](https://github.com/normal-computing))
   - [Using DSPy to train Gpt 3.5 on HumanEval by Thomas Ahle](https://github.com/stanfordnlp/dspy/blob/main/examples/functional/functional.ipynb)
   - [Building a chess playing agent using DSPy by Franck SN](https://medium.com/thoughts-on-machine-learning/building-a-chess-playing-agent-using-dspy-9b87c868f71e)
 
-TODO: Add links to the state-of-the-art results on Theory of Mind (ToM) by Plastic Labs, the results by Haize Labs for Red Teaming with DSPy, and the DSPy pipeline from Replit.
+
+TODO: Add links to the state-of-the-art results by the University of Toronto on Clinical NLP, on Theory of Mind (ToM) by Plastic Labs, and the DSPy pipeline from Replit.
 
 There are also recent cool examples at [Weaviate's DSPy cookbook](https://github.com/weaviate/recipes/tree/main/integrations/dspy) by Connor Shorten. [See tutorial on YouTube](https://www.youtube.com/watch?v=CEuUG4Umfxs).
 
 ## 3) Syntax: You're in charge of the workflow—it's free-form Python code!
 
 **DSPy** hides tedious prompt engineering, but it cleanly exposes the important decisions you need to make: **[1]** what's your system design going to look like? **[2]** what are the important constraints on the behavior of your program?
```

### Comparing `dspy-ai-2.4.9/README.md` & `dspy_ai-2.5.0rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,77 @@
+Metadata-Version: 2.1
+Name: dspy-ai
+Version: 2.5.0rc1
+Summary: DSPy: The framework for programming—not prompting—foundation models
+Home-page: https://github.com/stanfordnlp/dspy
+License: MIT
+Keywords: dspy,ai,language models,llm,openai
+Author: Omar Khattab
+Author-email: okhattab@stanford.edu
+Maintainer: Cyrus Nouroozi
+Maintainer-email: cyrus@edendaolab.com
+Requires-Python: >=3.9,<3.13
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: aws
+Provides-Extra: chromadb
+Provides-Extra: docs
+Provides-Extra: fastembed
+Provides-Extra: marqo
+Provides-Extra: milvus
+Provides-Extra: pinecone
+Provides-Extra: postgres
+Provides-Extra: qdrant
+Provides-Extra: weaviate
+Requires-Dist: anthropic (>=0.18.0,<0.19.0)
+Requires-Dist: autodoc_pydantic ; extra == "docs"
+Requires-Dist: backoff (>=2.2.1,<3.0.0)
+Requires-Dist: boto3 (>=1.34.78,<2.0.0) ; extra == "aws"
+Requires-Dist: chromadb (>=0.4.14,<0.5.0) ; extra == "chromadb"
+Requires-Dist: datasets (>=2.14.6,<3.0.0)
+Requires-Dist: docutils (<0.17) ; extra == "docs"
+Requires-Dist: fastembed (>=0.2.0) ; extra == "qdrant" or extra == "fastembed"
+Requires-Dist: furo (>=2023.3.27) ; extra == "docs"
+Requires-Dist: groq (>=0.4.2,<0.5.0)
+Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
+Requires-Dist: joblib (>=1.3.2,<2.0.0)
+Requires-Dist: llama-index (>=0.10.30,<0.11.0)
+Requires-Dist: m2r2 ; extra == "docs"
+Requires-Dist: marqo ; extra == "marqo"
+Requires-Dist: myst-nb ; extra == "docs"
+Requires-Dist: myst-parser ; extra == "docs"
+Requires-Dist: openai (>=0.28.1,<2.0.0)
+Requires-Dist: optuna (>=3.4.0,<4.0.0)
+Requires-Dist: pandas (>=2.1.1,<3.0.0)
+Requires-Dist: pgvector (>=0.2.5,<0.3.0) ; extra == "postgres"
+Requires-Dist: pinecone-client (>=2.2.4,<3.0.0) ; extra == "pinecone"
+Requires-Dist: psycopg2 (>=2.9.9,<3.0.0) ; extra == "postgres"
+Requires-Dist: pydantic (>=2.0,<3.0)
+Requires-Dist: pymilvus (>=2.3.6,<3.0.0) ; extra == "milvus"
+Requires-Dist: qdrant-client (>=1.6.2,<2.0.0) ; extra == "qdrant"
+Requires-Dist: regex (>=2023.10.3,<2024.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
+Requires-Dist: snowflake-snowpark-python ; python_version >= "3.9" and python_version < "3.12"
+Requires-Dist: sphinx (>=4.3.0) ; extra == "docs"
+Requires-Dist: sphinx-autobuild ; extra == "docs"
+Requires-Dist: sphinx-automodapi (==0.16.0) ; extra == "docs"
+Requires-Dist: sphinx-reredirects (>=0.1.2,<0.2.0) ; extra == "docs"
+Requires-Dist: sphinx_rtd_theme ; extra == "docs"
+Requires-Dist: structlog (>=24.1.0,<25.0.0)
+Requires-Dist: tqdm (>=4.66.1,<5.0.0)
+Requires-Dist: ujson (>=5.8.0,<6.0.0)
+Requires-Dist: weaviate-client (>=4.5.4,<5.0.0) ; extra == "weaviate"
+Project-URL: Repository, https://github.com/stanfordnlp/dspy
+Description-Content-Type: text/markdown
+
 <p align="center">
   <img align="center" src="docs/images/DSPy8.png" width="460px" />
 </p>
 <p align="left">
 
 
 ## DSPy: _Programming_—not prompting—Foundation Models
@@ -68,19 +138,19 @@
 pip install git+https://github.com/stanfordnlp/dspy.git
 ````
 
 Or open our intro notebook in Google Colab: [<img align="center" src="https://colab.research.google.com/assets/colab-badge.svg" />](https://colab.research.google.com/github/stanfordnlp/dspy/blob/main/intro.ipynb)
 
 By default, DSPy installs the latest `openai` from pip. However, if you install old version before OpenAI changed their API `openai~=0.28.1`, the library will use that just fine. Both are supported.
 
-For the optional (alphabetically sorted) [Chromadb](https://github.com/chroma-core/chroma), [Qdrant](https://github.com/qdrant/qdrant), [Marqo](https://github.com/marqo-ai/marqo), Pinecone, [Weaviate](https://github.com/weaviate/weaviate),
+For the optional (alphabetically sorted) [Chromadb](https://github.com/chroma-core/chroma), [Qdrant](https://github.com/qdrant/qdrant), [Marqo](https://github.com/marqo-ai/marqo), Pinecone, [Snowflake](https://github.com/snowflakedb/snowpark-python) [Weaviate](https://github.com/weaviate/weaviate),
 or [Milvus](https://github.com/milvus-io/milvus) retrieval integration(s), include the extra(s) below:
 
 ```
-pip install dspy-ai[chromadb]  # or [qdrant] or [marqo] or [mongodb] or [pinecone] or [weaviate] or [milvus]
+pip install dspy-ai[chromadb]  # or [qdrant] or [marqo] or [mongodb] or [pinecone] or [snowflake] or [weaviate] or [milvus]
 ```
 
 ## 2) Documentation
 
 The DSPy documentation is divided into **tutorials** (step-by-step illustration of solving a task in DSPy), **guides** (how to use specific parts of the API), and **examples** (self-contained programs that illustrate usage).
 
 ### A) Tutorials
@@ -97,18 +167,19 @@
 | Advanced | [**Information Extraction**](https://twitter.com/KarelDoostrlnck/status/1724991014207930696) | [<img align="center" src="https://colab.research.google.com/assets/colab-badge.svg" />](https://colab.research.google.com/drive/1CpsOiLiLYKeGrhmq579_FmtGsD5uZ3Qe) | Tackles extracting information from long articles (biomedical research papers). Combines in-context learning and retrieval to set SOTA on BioDEX. Contributed by [Karel D’Oosterlinck](https://twitter.com/KarelDoostrlnck/status/1724991014207930696).  |
 
 
 **Other resources people find useful**:
 
 - [DSPy talk at ScaleByTheBay Nov 2023](https://www.youtube.com/watch?v=Dt3H2ninoeY).
 - [DSPy webinar with MLOps Learners](https://www.youtube.com/watch?v=im7bCLW2aM4), a bit longer with Q&A.
-- Hands-on Overviews of DSPy by the community: [DSPy Explained! by Connor Shorten](https://www.youtube.com/watch?v=41EfOY0Ldkc), [DSPy explained by code_your_own_ai](https://www.youtube.com/watch?v=ycfnKPxBMck), [DSPy Crash Course by AI Bites](https://youtu.be/5-zgASQKkKQ?si=3gnmVouT5_rpk_nu)
+- Hands-on Overviews of DSPy by the community: [DSPy Explained! by Connor Shorten](https://www.youtube.com/watch?v=41EfOY0Ldkc), [DSPy explained by code_your_own_ai](https://www.youtube.com/watch?v=ycfnKPxBMck), [DSPy Crash Course by AI Bites](https://youtu.be/5-zgASQKkKQ?si=3gnmVouT5_rpk_nu), [DSPy Paper Explained by Unify](https://youtu.be/kFB8kFchCH4?si=FuM6L5H5lweanckz)
 - Interviews: [Weaviate Podcast in-person](https://www.youtube.com/watch?v=CDung1LnLbY), and you can find 6-7 other remote podcasts on YouTube from a few different perspectives/audiences.
 - **Tracing in DSPy** with Arize Phoenix: [Tutorial for tracing your prompts and the steps of your DSPy programs](https://colab.research.google.com/github/Arize-ai/phoenix/blob/main/tutorials/tracing/dspy_tracing_tutorial.ipynb)
 - [DSPy: Not Your Average Prompt Engineering](https://jina.ai/news/dspy-not-your-average-prompt-engineering), why it's crucial for future prompt engineering, and yet why it is challenging for prompt engineers to learn.
+- **Tracing & Optimization Tracking in DSPy** with Parea AI: [Tutorial on tracing & evaluating a DSPy RAG program](https://docs.parea.ai/tutorials/dspy-rag-trace-evaluate/tutorial)
 
 ### B) Guides
 
 If you're new to DSPy, it's probably best to go in sequential order. You will probably refer to these guides frequently after that, e.g. to copy/paste snippets that you can edit for your own DSPy programs.
 
 
 1. **[Language Models](https://dspy-docs.vercel.app/docs/building-blocks/language_models)**
@@ -132,32 +203,36 @@
 
 There's a bunch of examples in the `examples/` directory and in the top-level directory. We welcome contributions!
 
 You can find other examples tweeted by [@lateinteraction](https://twitter.com/lateinteraction) on Twitter/X.
 
 **Some other examples (not exhaustive, feel free to add more via PR):**
 
+
+- [DSPy Optimizers Benchmark on a bunch of different tasks, by Michael Ryan](https://github.com/stanfordnlp/dspy/tree/main/testing/tasks)
+- [Sophisticated Extreme Multi-Class Classification, IReRa, by Karel D’Oosterlinck](https://github.com/KarelDO/xmc.dspy)
+- [Haize Lab's Red Teaming with DSPy](https://blog.haizelabs.com/posts/dspy/) and see [their DSPy code](https://github.com/haizelabs/dspy-redteam)
 - Applying DSPy Assertions
   - [Long-form Answer Generation with Citations, by Arnav Singhvi](https://colab.research.google.com/github/stanfordnlp/dspy/blob/main/examples/longformqa/longformqa_assertions.ipynb)
   - [Generating Answer Choices for Quiz Questions, by Arnav Singhvi](https://colab.research.google.com/github/stanfordnlp/dspy/blob/main/examples/quiz/quiz_assertions.ipynb)
   - [Generating Tweets for QA, by Arnav Singhvi](https://colab.research.google.com/github/stanfordnlp/dspy/blob/main/examples/tweets/tweets_assertions.ipynb)
 - [Compiling LCEL runnables from LangChain in DSPy](https://github.com/stanfordnlp/dspy/blob/main/examples/tweets/compiling_langchain.ipynb)
 - [AI feedback, or writing LM-based metrics in DSPy](https://github.com/stanfordnlp/dspy/blob/main/examples/tweets/tweet_metric.py)
-- [DSPy Optimizers Benchmark on a bunch of different tasks, by Michael Ryan](https://github.com/stanfordnlp/dspy/tree/main/testing/tasks)
+- [DSPy Optimizers Benchmark on a bunch of different tasks, by Michael Ryan](https://github.com/stanfordnlp/dspy/tree/main/testing/README.md)
 - [Indian Languages NLI with gains due to compiling by Saiful Haq](https://github.com/saifulhaq95/DSPy-Indic/blob/main/indicxlni.ipynb)
-- [Sophisticated Extreme Multi-Class Classification, IReRa, by Karel D’Oosterlinck](https://github.com/KarelDO/xmc.dspy)
 - [DSPy on BIG-Bench Hard Example, by Chris Levy](https://drchrislevy.github.io/posts/dspy/dspy.html)
 - [Using Ollama with DSPy for Mistral (quantized) by @jrknox1977](https://gist.github.com/jrknox1977/78c17e492b5a75ee5bbaf9673aee4641)
-- [Using DSPy, "The Unreasonable Effectiveness of Eccentric Automatic Prompts" (paper) by VMware's Rick Battle & Teja Gollapudi, and interview at TheRegister](https://www.theregister.com/2024/02/22/prompt_engineering_ai_models/)
+- [Using DSPy, "The Unreasonable Effectiveness of Eccentric Automatic Prompts" (paper) by VMware's Rick Battle & Teja Gollapudi](https://arxiv.org/abs/2402.10949), and [interview at TheRegister](https://www.theregister.com/2024/02/22/prompt_engineering_ai_models/)
 - [Optimizing Performance of Open Source LM for Text-to-SQL using DSPy and vLLM, by Juan Ovalle](https://github.com/jjovalle99/DSPy-Text2SQL)
 - Typed DSPy (contributed by [@normal-computing](https://github.com/normal-computing))
   - [Using DSPy to train Gpt 3.5 on HumanEval by Thomas Ahle](https://github.com/stanfordnlp/dspy/blob/main/examples/functional/functional.ipynb)
   - [Building a chess playing agent using DSPy by Franck SN](https://medium.com/thoughts-on-machine-learning/building-a-chess-playing-agent-using-dspy-9b87c868f71e)
 
-TODO: Add links to the state-of-the-art results on Theory of Mind (ToM) by Plastic Labs, the results by Haize Labs for Red Teaming with DSPy, and the DSPy pipeline from Replit.
+
+TODO: Add links to the state-of-the-art results by the University of Toronto on Clinical NLP, on Theory of Mind (ToM) by Plastic Labs, and the DSPy pipeline from Replit.
 
 There are also recent cool examples at [Weaviate's DSPy cookbook](https://github.com/weaviate/recipes/tree/main/integrations/dspy) by Connor Shorten. [See tutorial on YouTube](https://www.youtube.com/watch?v=CEuUG4Umfxs).
 
 ## 3) Syntax: You're in charge of the workflow—it's free-form Python code!
 
 **DSPy** hides tedious prompt engineering, but it cleanly exposes the important decisions you need to make: **[1]** what's your system design going to look like? **[2]** what are the important constraints on the behavior of your program?
 
@@ -461,7 +536,8 @@
 
 
 > _Note: If you're looking for Demonstrate-Search-Predict (DSP), which is the previous version of DSPy, you can find it on the [v1](https://github.com/stanfordnlp/dspy/tree/v1) branch of this repo._
 
 
 
 
+
```

### Comparing `dspy-ai-2.4.9/dsp/templates/template_v2.py` & `dspy_ai-2.5.0rc1/dspy/experimental/synthesizer/synthesizer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,281 +1,260 @@
-import re
-from collections import namedtuple
-from typing import Any, Union
+import random
+from collections.abc import Mapping
+from typing import List, Optional, Union
+
+from datasets import Dataset
+from rich import print as rprint
+from tqdm import tqdm, trange
+
+import dspy
+
+from .config import SynthesizerArguments
+from .instruction_suffixes import (
+    INPUT_GENERATION_TASK_WITH_EXAMPLES_SUFFIX,
+    INPUT_GENERATION_TASK_WITH_FEEDBACK_SUFFIX,
+)
+from .signatures import (
+    ExplainTask,
+    GenerateFieldDescription,
+    GenerateInputFieldsData,
+    GenerateOutputFieldsData,
+    GetFeedbackOnGeneration,
+    UnderstandTask,
+    UpdateTaskDescriptionBasedOnFeedback,
+)
+from .utils import format_examples
+
+__all__ = [
+    "Synthesizer",
+    "SynthesizerArguments",
+]
+
+class Synthesizer:
+    def __init__(self, config: SynthesizerArguments):
+        self.config = config
+        self.input_lm = config.input_lm_model or dspy.settings.lm
+        self.output_lm = config.output_lm_model or dspy.settings.lm
+
+        self.explain_task = dspy.Predict(ExplainTask)
+        self.understand_task = dspy.Predict(UnderstandTask)
+        self.get_feedback_on_generation = dspy.Predict(GetFeedbackOnGeneration)
+        self.generate_field_description = dspy.Predict(GenerateFieldDescription)
+        self.update_task_description = dspy.Predict(UpdateTaskDescriptionBasedOnFeedback)
+
+        self.generate_input_data = GenerateInputFieldsData
+        self.generate_output_data = GenerateOutputFieldsData
+
+    def _gather_feedback(self, examples: dspy.Example) -> str:
+        if self.config.feedback_mode == "human":
+            input_keys = examples.inputs().keys()
+
+            print("-"*75)
+            print_text = "[bold blue]Generated Data:[bold blue]\n[bold red]Inputs:[bold red]\n"
+            
+            for key in input_keys:
+                print_text += f"\t[bold yellow]{key}[bold yellow]: [green]{examples[key]}[green]\n"
+            
+            rprint(print_text)
+            feedback = input("Provide feedback on the generated data: ")
+            print("-"*75)
+
+            return feedback
+        
+        elif self.config.feedback_mode == "llm":
+            feedback = self.get_feedback_on_generation(
+                synthetic_data=[examples],
+                task_description=self.generate_output_data.__doc__,
+            )
 
-import dsp
-from dsp.primitives.demonstrate import Example
+            return feedback.feedback
 
-from .utils import format_answers, passages2text
+        else:
+            raise ValueError("Feedback mode should be either 'human' or 'llm'.")
 
-Field = namedtuple("Field", "name separator input_variable output_variable description")
+    def _get_field_data(self, key: str, keys_dict: Mapping[str, str]):
+        if key.startswith("$"):
+            field_details = self.generate_field_description(
+                task_description=keys_dict["task_description"],
+                field_name=key,
+            )
 
-# TODO: de-duplicate with dsp/templates/template.py
+            field_name = key
+            field_description = field_details.field_description
 
+            return field_name, field_description
 
-class TemplateV2:
-    def __init__(
-        self,
-        template,
-        format_handlers={
-            "passages": passages2text,
-            "context": passages2text,
-            "answer": format_answers,
-            "answers": format_answers,
-        },
-    ):
-        self.format_handlers = format_handlers
+        else:
+            field_name = key
+            field_description = keys_dict[key]
 
-        template = template.strip()
+            return field_name, field_description
 
-        self.instructions = re.search("(.*)\n", template).group(1)
-        template = template[len(self.instructions) :].strip()
+    def _prepare_synthetic_data_predictors(
+        self,
+        input_keys: Mapping[str, str],
+        output_keys: Mapping[str, str],
+        ground_source: Optional[Union[List[dspy.Example], dspy.Signature]] = None,
+    ):
+        for key in tqdm(input_keys, desc="Preparing Input Fields"):
+            field_name, field_description = self._get_field_data(key, input_keys)
 
-        self.fields = []
-        while len(template) > 0:
-            match = re.search("(.*)(\s){(.*)}\s(.*\${.*})", template)
-            if match is not None:
-                name = match.group(1)
-                separator = match.group(2)
-                variable = match.group(3)
-                description = match.group(4)
-            else:
-                match = re.search("(.*)(\s){(.*)}", template)
-                if match is not None:
-                    name = match.group(1)
-                    separator = match.group(2)
-                    variable = match.group(3)
-                    description = None
-                else:
-                    raise ValueError("Could not parse template")
-
-            var_match = re.match("(.*) -> (.*)", variable)
-            if var_match is not None:
-                input_variable = var_match.group(1)
-                output_variable = var_match.group(2)
-            else:
-                input_variable = variable
-                output_variable = variable
-
-            self.fields.append(
-                Field(
-                    name=name,
-                    separator=separator,
-                    input_variable=input_variable,
-                    output_variable=output_variable,
-                    description=description,
-                ),
+            output_field = dspy.OutputField(
+                prefix=f"{field_name}:",
+                desc=field_description,
+            )
+            self.generate_input_data = self.generate_input_data.insert(
+                -1,
+                field_name,
+                output_field,
             )
 
-            template = template[len(match.group(0)) :].strip()
+            if ground_source:
+                self.generate_input_data = self.generate_input_data.insert(
+                    -1,
+                    "ground_source",
+                    dspy.InputField(
+                        prefix="Pre-Generated Examples:",
+                        desc="Pre-Generated Examples to differ the inputs around.",
+                        format=format_examples,
+                    ),
+                )
 
-    def query(self, example: Example, is_demo: bool = False) -> str:
-        """Retrieves the input variables from the example and formats them into a query string."""
-        result: list[str] = []
-
-        # If not a demo, find the last field that doesn't have a value set in `example` and set it to ""
-        # This creates the "Output:" prefix at the end of the prompt.
-        if not is_demo:
-            has_value = [
-                field.input_variable in example
-                and example[field.input_variable] is not None
-                and example[field.input_variable] != ""
-                for field in self.fields
-            ]
-
-            # If there are no inputs, set the first field to ""
-            if not any(has_value):
-                example[self.fields[0].input_variable] = ""
-            # Otherwise find the first field without a value.
-            else:
-                for i in range(1, len(has_value)):
-                    if has_value[i - 1] and not any(has_value[i:]):
-                        example[self.fields[i].input_variable] = ""
-                        break
-
-        for field in self.fields:
-            if field.input_variable in example and example[field.input_variable] is not None:
-                if field.input_variable in self.format_handlers:
-                    format_handler = self.format_handlers[field.input_variable]
-                else:
-
-                    def format_handler(x):
-                        assert type(x) == str, f"Need format_handler for {field.input_variable} of type {type(x)}"
-                        return " ".join(x.split())
+            input_field = dspy.InputField(
+                prefix=f"{field_name}:",
+                desc=field_description,
+            )
+            self.generate_output_data = self.generate_output_data.insert(
+                -1,
+                field_name,
+                input_field,
+            )
 
-                formatted_value = format_handler(example[field.input_variable])
-                separator = "\n" if field.separator == " " and "\n" in formatted_value else field.separator
+        for key in tqdm(output_keys, desc="Preparing Output Fields"):
+            field_name, field_description = self._get_field_data(key, output_keys)
 
-                result.append(
-                    f"{field.name}{separator}{formatted_value}",
-                )
+            output_field = dspy.OutputField(
+                prefix=f"{field_name}:",
+                desc=field_description,
+            )
+            self.generate_output_data = self.generate_output_data.insert(
+                -1,
+                field_name,
+                output_field,
+            )
 
-        if self._has_augmented_guidelines() and (example.get("augmented", False)):
-            return "\n\n".join([r for r in result if r])
-        return "\n".join([r for r in result if r])
-
-    def guidelines(self, show_guidelines=True) -> str:
-        """Returns the task guidelines as described in the lm prompt"""
-        if (not show_guidelines) or (hasattr(dsp.settings, "show_guidelines") and not dsp.settings.show_guidelines):
-            return ""
-
-        result = "Follow the following format.\n\n"
-
-        example = dsp.Example()
-        for field in self.fields:
-            example[field.input_variable] = field.description
-        example.augmented = self._has_augmented_guidelines()
-
-        result += self.query(example)
-        return result
-
-    def _has_augmented_guidelines(self):
-        return len(self.fields) > 3 or any(
-            ("\n" in field.separator) or ("\n" in field.description) for field in self.fields
-        )
+        return dspy.ChainOfThought(self.generate_input_data), dspy.Predict(self.generate_output_data)
 
-    def extract(
-        self,
-        example: Union[Example, dict[str, Any]],
-        raw_pred: str,
-    ) -> Example:
-        """Extracts the answer from the LM raw prediction using the template structure
-
-        Args:
-            example (Union[Example, dict[str, Any]]): Contains the input variables that raw_pred was completed on.
-            raw_pred (str): LM generated string
-
-        Returns:
-            Example: The example with the output variables filled in
-        """
-        example = dsp.Example(example)
-
-        raw_pred = raw_pred.strip()
-
-        idx = 0
-        while idx < len(self.fields):
-            if self.fields[idx].input_variable not in example or example[self.fields[idx].input_variable] is None:
-                break
-            idx += 1
-
-        import dspy
-
-        idx = min(idx, len(self.fields) - 1)
-        while raw_pred != "" and idx < len(self.fields):
-            if idx < len(self.fields) - 1:
-                next_field_name = "\n" + self.fields[idx + 1].name
-                offset = raw_pred.find(next_field_name)
-
-                if offset >= 0:
-                    if dspy.settings.release >= 20231003:
-                        example[self.fields[idx].output_variable] = raw_pred[:offset].strip().rstrip("---").strip()
-                        raw_pred = raw_pred[offset + len(next_field_name) :].strip().rstrip("---").strip()
-                    else:
-                        example[self.fields[idx].output_variable] = raw_pred[:offset].strip()
-                        raw_pred = raw_pred[offset + len(next_field_name) :].strip()
+    def _get_dataset_metadata(self, ground_source: Union[List[dspy.Example], dspy.Signature]):
+        if isinstance(ground_source, dspy.SignatureMeta):
+            task_description = ground_source.__doc__
+            if task_description.startswith("Given the fields"):
+                task_description = self.understand_task(examples=ground_source.__doc__).explanation
+            
+            input_keys = {k:v.json_schema_extra["desc"] for k,v in ground_source.input_fields.items()}
+            output_keys = {k:v.json_schema_extra["desc"] for k,v in ground_source.output_fields.items()}
+
+            return task_description, input_keys, output_keys
+
+        elif isinstance(ground_source, list) and isinstance(ground_source[0], dspy.Example):
+            task_description = self.explain_task(examples=ground_source).explanation
+            input_keys = {key:f"${{{key}}}" for key in ground_source[0].inputs()}
+            output_keys = {key:f"${{{key}}}" for key in ground_source[0].labels()}
 
-                    idx += 1
-                else:
-                    if dspy.settings.release >= 20231003:
-                        example[self.fields[idx].output_variable] = raw_pred.strip().rstrip("---").strip()
-                    else:
-                        example[self.fields[idx].output_variable] = raw_pred.strip()
+            return task_description, input_keys, output_keys
 
-                    raw_pred = ""
-                    idx += 1
-                    break
+        else:
+            raise ValueError("Ground source must be either a list of examples or a signature.")
 
-            else:
-                assert idx == len(self.fields) - 1, (idx, len(self.fields))
+    def generate(
+        self,
+        ground_source: Union[List[dspy.Example], dspy.Signature],
+        num_data: int,
+        batch_size: int = 1,
+    ):
+        batch_size = batch_size or 1
+        task_description, input_keys, output_keys = self._get_dataset_metadata(ground_source)
 
-                if dspy.settings.release >= 20231003:
-                    example[self.fields[idx].output_variable] = raw_pred.strip().rstrip("---").strip()
-                else:
-                    example[self.fields[idx].output_variable] = raw_pred.strip()
+        if self.config.num_example_for_optim:
+            self.generate_input_data.__doc__ += INPUT_GENERATION_TASK_WITH_EXAMPLES_SUFFIX
+        
+        if self.config.feedback_mode:
+            self.generate_input_data.__doc__ += INPUT_GENERATION_TASK_WITH_FEEDBACK_SUFFIX
+
+        self.generate_output_data.__doc__ = task_description
+
+        self.input_predictor, self.output_predictor = self._prepare_synthetic_data_predictors(
+            input_keys=input_keys,
+            output_keys=output_keys,
+            ground_source=ground_source if self.config.num_example_for_optim else None,
+        )
 
-                break
+        data = []
+        feedback = ""
 
-        return example
+        for idx in trange(0, num_data, batch_size, desc="Generating Synthetic Data"):
+            iter_temperature = 0.7+0.01*idx
+            iter_seed = random.randint(0, 1000000)
+
+            kwargs = {
+                "task_description": task_description,
+                "knowledge_seed": iter_seed,
+                "config": dict(temperature=iter_temperature, n=batch_size),
+            }
+
+            if self.config.num_example_for_optim:
+                if not isinstance(ground_source, list):
+                    raise ValueError("Ground source must be a list of examples when `num_example_for_optim` is provided.")
+                kwargs["ground_source"] = random.sample(ground_source, k=self.config.num_example_for_optim)
+            
+            with dspy.context(lm=self.input_lm):
+                inputs = self.input_predictor(**kwargs)
+
+            input_kwargs = [{
+                key: getattr(completions, key)
+                for key in input_keys
+            } for completions in inputs.completions]
+
+            for kwargs in input_kwargs:
+                outputs = None
+
+                with dspy.context(lm=self.output_lm, temperature=iter_temperature):
+                    if self.config.output_teacher_module:
+                        outputs = self.config.output_teacher_module(**kwargs)
 
-    def __call__(self, example, show_guidelines=True) -> str:
-        example = dsp.Example(example)
+                    else:
+                        outputs = self.output_predictor(**kwargs, config=dict(temperature=iter_temperature))
 
-        if hasattr(dsp.settings, "query_only") and dsp.settings.query_only:
-            return self.query(example)
+                output_kwargs = {
+                    key: getattr(outputs, key)
+                    for key in output_keys
+                }
+
+                data.append(dspy.Example(**kwargs, **output_kwargs).with_inputs(*input_keys))
+            
+            if self.config.feedback_mode and idx < self.config.num_example_for_feedback:
+                feedback = self._gather_feedback(data[-1])
+               
+                task_description = self.update_task_description(
+                    task_description=task_description,
+                    feedback=feedback,
+                ).updated_task_description
+
+                self.output_predictor.signature.__doc__ = task_description
 
-        # The training data should not contain the output variable
-        if self.fields[-1].input_variable in example:
-            del example[self.fields[-1].input_variable]
+        return data
 
-        rdemos = [
-            self.query(demo, is_demo=True)
-            for demo in example.demos
-            if (
-                (not demo.get("augmented", False))
-                and (  # validate that the training example has the same primitive input var as the template
-                    self.fields[-1].input_variable in demo and demo[self.fields[-1].input_variable] is not None
-                )
-            )
-        ]
+    def export(self, data: List[dspy.Example], path: str, mode: str = None, **kwargs):
+        extention = mode or path.split(".")[-1]
 
-        ademos = [self.query(demo, is_demo=True) for demo in example.demos if demo.get("augmented", False)]
+        dataset = Dataset.from_list(
+            [example.toDict() for example in data],
+        )
 
-        # Move the rdemos to ademos if rdemo has all the fields filled in
-        rdemos_ = []
-        new_ademos = []
-        for rdemo in rdemos:
-            if all((field.name in rdemo) for field in self.fields if field.input_variable in example):
-                import dspy
-
-                if dspy.settings.release >= 20230928:
-                    new_ademos.append(rdemo)
-                else:
-                    ademos.append(rdemo)
-            else:
-                rdemos_.append(rdemo)
-
-        ademos = new_ademos + ademos
-        rdemos = rdemos_
-
-        long_query = self._has_augmented_guidelines()
-
-        if long_query:
-            example["augmented"] = True
-
-        query = self.query(example)
-
-        # if it has more lines than fields
-        if len(query.split("\n")) > len(self.fields):
-            long_query = True
-
-            if not example.get("augmented", False):
-                example["augmented"] = True
-                query = self.query(example)
-
-        rdemos = "\n\n".join(rdemos)
-
-        if len(rdemos) >= 1 and len(ademos) == 0 and not long_query:
-            rdemos_and_query = "\n\n".join([rdemos, query])
-            parts = [
-                self.instructions,
-                self.guidelines(show_guidelines),
-                rdemos_and_query,
-            ]
-        elif len(rdemos) == 0:
-            parts = [
-                self.instructions,
-                self.guidelines(show_guidelines),
-                *ademos,
-                query,
-            ]
-        else:
-            parts = [
-                self.instructions,
-                rdemos,
-                self.guidelines(show_guidelines),
-                *ademos,
-                query,
-            ]
+        if extention == "csv":
+            dataset.to_csv(path_or_buf=path, **kwargs)
 
-        prompt = "\n\n---\n\n".join([p.strip() for p in parts if p])
+        elif extention == "json":
+            dataset.to_json(path_or_buf=path, **kwargs)
 
-        return prompt.strip()
+        elif extention == "arrow" or extention == "hf":
+            dataset.save_to_disk(path)
```

### Comparing `dspy-ai-2.4.9/dspy/__init__.py` & `dspy_ai-2.5.0rc1/dspy/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 import dsp
 from dsp.modules.hf_client import ChatModuleClient, HFClientSGLang, HFClientVLLM, HFServerTGI
 
 from .predict import *
 from .primitives import *
 from .retrieve import *
 from .signatures import *
+from .utils.logging import logger, set_log_output
 
 # Functional must be imported after primitives, predict and signatures
 from .functional import *  # isort: skip
-from .utils.logging import logger, set_log_output
 
 settings = dsp.settings
 
 LM = dsp.LM
 
 AzureOpenAI = dsp.AzureOpenAI
 OpenAI = dsp.GPT3
 Mistral = dsp.Mistral
 Databricks = dsp.Databricks
 Cohere = dsp.Cohere
 ColBERTv2 = dsp.ColBERTv2
 Pyserini = dsp.PyseriniRetriever
 Clarifai = dsp.ClarifaiLLM
+CloudflareAI = dsp.CloudflareAI
 Google = dsp.Google
 GoogleVertexAI = dsp.GoogleVertexAI
 GROQ = dsp.GroqLM
+Snowflake = dsp.Snowflake
+Claude = dsp.Claude
 
 HFClientTGI = dsp.HFClientTGI
 HFClientVLLM = HFClientVLLM
 
 Anyscale = dsp.Anyscale
 Together = dsp.Together
 HFModel = dsp.HFModel
@@ -37,9 +40,12 @@
 Bedrock = dsp.Bedrock
 Sagemaker = dsp.Sagemaker
 AWSModel = dsp.AWSModel
 AWSMistral = dsp.AWSMistral
 AWSAnthropic = dsp.AWSAnthropic
 AWSMeta = dsp.AWSMeta
 
+Watsonx = dsp.Watsonx
+PremAI = dsp.PremAI
+
 configure = settings.configure
 context = settings.context
```

### Comparing `dspy-ai-2.4.9/dspy/datasets/colors.py` & `dspy_ai-2.5.0rc1/dspy/datasets/colors.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/datasets/dataloader.py` & `dspy_ai-2.5.0rc1/dspy/datasets/dataloader.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/datasets/dataset.py` & `dspy_ai-2.5.0rc1/dspy/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/datasets/gsm8k.py` & `dspy_ai-2.5.0rc1/dspy/datasets/gsm8k.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/datasets/hotpotqa.py` & `dspy_ai-2.5.0rc1/dspy/datasets/hotpotqa.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/evaluate/auto_evaluation.py` & `dspy_ai-2.5.0rc1/dspy/evaluate/auto_evaluation.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/evaluate/evaluate.py` & `dspy_ai-2.5.0rc1/dspy/evaluate/evaluate.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import contextlib
+import signal
 import sys
 import threading
 import types
 
 import pandas as pd
 import tqdm
 from tqdm.contrib.logging import logging_redirect_tqdm
@@ -10,26 +12,22 @@
 
 try:
     from IPython.display import HTML
     from IPython.display import display as ipython_display
 except ImportError:
     ipython_display = print
 
-    def HTML(x):
+    def HTML(x) -> str:  # noqa: N802
         return x
 
 
 from concurrent.futures import ThreadPoolExecutor, as_completed
 
-from dsp.evaluation.utils import *
-
-"""
-TODO: Counting failures and having a max_failure count. When that is exceeded (also just at the end),
-we print the number of failures, the first N examples that failed, and the first N exceptions raised.
-"""
+# TODO: Counting failures and having a max_failure count. When that is exceeded (also just at the end),
+# we print the number of failures, the first N examples that failed, and the first N exceptions raised.
 
 
 class Evaluate:
     def __init__(
         self,
         *,
         devset,
@@ -45,19 +43,21 @@
         self.metric = metric
         self.num_threads = num_threads
         self.display_progress = display_progress
         self.display_table = display_table
         self.max_errors = max_errors
         self.error_count = 0
         self.error_lock = threading.Lock()
+        self.cancel_jobs = threading.Event()
         self.return_outputs = return_outputs
 
         if "display" in _kwargs:
             dspy.logger.warning(
-                "DeprecationWarning: 'display' has been deprecated. To see all information for debugging, use 'dspy.set_log_level('debug')'. In the future this will raise an error.",
+                "DeprecationWarning: 'display' has been deprecated. To see all information for debugging,"
+                " use 'dspy.set_log_level('debug')'. In the future this will raise an error.",
             )
 
     def _execute_single_thread(self, wrapped_program, devset, display_progress):
         ncorrect = 0
         ntotal = 0
         reordered_devset = []
 
@@ -74,27 +74,60 @@
 
         return reordered_devset, ncorrect, ntotal
 
     def _execute_multi_thread(self, wrapped_program, devset, num_threads, display_progress):
         ncorrect = 0
         ntotal = 0
         reordered_devset = []
+        job_cancelled = "cancelled"
+
+        # context manger to handle sigint
+        @contextlib.contextmanager
+        def interrupt_handler_manager():
+            """Sets the cancel_jobs event when a SIGINT is received."""
+            default_handler = signal.getsignal(signal.SIGINT)
+
+            def interrupt_handler(sig, frame):
+                self.cancel_jobs.set()
+                dspy.logger.warning("Received SIGINT. Cancelling evaluation.")
+                default_handler(sig, frame)
+
+            signal.signal(signal.SIGINT, interrupt_handler)
+            yield
+            # reset to the default handler
+            signal.signal(signal.SIGINT, default_handler)
+
+        def cancellable_wrapped_program(idx, arg):
+            # If the cancel_jobs event is set, return the cancelled_job literal
+            if self.cancel_jobs.is_set():
+                return None, None, job_cancelled, None
+            return wrapped_program(idx, arg)
 
-        with ThreadPoolExecutor(max_workers=num_threads) as executor:
-            futures = {executor.submit(wrapped_program, idx, arg) for idx, arg in devset}
+        with ThreadPoolExecutor(max_workers=num_threads) as executor, interrupt_handler_manager():
+            futures = {executor.submit(cancellable_wrapped_program, idx, arg) for idx, arg in devset}
             pbar = tqdm.tqdm(total=len(devset), dynamic_ncols=True, disable=not display_progress)
 
             for future in as_completed(futures):
                 example_idx, example, prediction, score = future.result()
+
+                # use the cancelled_job literal to check if the job was cancelled - use "is" not "=="
+                # in case the prediction is "cancelled" for some reason.
+                if prediction is job_cancelled:
+                    continue
+
                 reordered_devset.append((example_idx, example, prediction, score))
                 ncorrect += score
                 ntotal += 1
                 self._update_progress(pbar, ncorrect, ntotal)
             pbar.close()
 
+        if self.cancel_jobs.is_set():
+            dspy.logger.warning("Evaluation was cancelled. The results may be incomplete.")
+            raise KeyboardInterrupt
+
         return reordered_devset, ncorrect, ntotal
 
     def _update_progress(self, pbar, ncorrect, ntotal):
         pbar.set_description(f"Average Metric: {ncorrect} / {ntotal}  ({round(100 * ncorrect / ntotal, 1)})")
         pbar.update()
 
     def __call__(
@@ -171,33 +204,30 @@
         if return_outputs:  # Handle the return_outputs logic
             results = [(example, prediction, score) for _, example, prediction, score in predicted_devset]
 
         data = [
             merge_dicts(example, prediction) | {"correct": score} for _, example, prediction, score in predicted_devset
         ]
 
-        df = pd.DataFrame(data)
+        result_df = pd.DataFrame(data)
 
-        # Truncate every cell in the DataFrame
-        if hasattr(df, "map"):  # DataFrame.applymap was renamed to DataFrame.map in Pandas 2.1.0
-            df = df.map(truncate_cell)
-        else:
-            df = df.applymap(truncate_cell)
+        # Truncate every cell in the DataFrame (DataFrame.applymap was renamed to DataFrame.map in Pandas 2.1.0)
+        result_df = result_df.map(truncate_cell) if hasattr(result_df, "map") else result_df.applymap(truncate_cell)
 
         # Rename the 'correct' column to the name of the metric object
         metric_name = metric.__name__ if isinstance(metric, types.FunctionType) else metric.__class__.__name__
-        df.rename(columns={"correct": metric_name}, inplace=True)
+        result_df = result_df.rename(columns={"correct": metric_name})
 
         if display_table:
-            if isinstance(display_table, int):
-                df_to_display = df.head(display_table).copy()
-                truncated_rows = len(df) - display_table
-            else:
-                df_to_display = df.copy()
+            if isinstance(display_table, bool):
+                df_to_display = result_df.copy()
                 truncated_rows = 0
+            else:
+                df_to_display = result_df.head(display_table).copy()
+                truncated_rows = len(result_df) - display_table
 
             styled_df = configure_dataframe_display(df_to_display, metric_name)
 
             ipython_display(styled_df)
 
             if truncated_rows > 0:
                 # Simplified message about the truncated rows
@@ -211,23 +241,23 @@
                     ... {truncated_rows} more rows not displayed ...
                 </div>
                 """
                 ipython_display(HTML(message))
 
         if return_all_scores and return_outputs:
             return round(100 * ncorrect / ntotal, 2), results, [score for *_, score in predicted_devset]
-        elif return_all_scores:
+        if return_all_scores:
             return round(100 * ncorrect / ntotal, 2), [score for *_, score in predicted_devset]
-        elif return_outputs:
+        if return_outputs:
             return round(100 * ncorrect / ntotal, 2), results
 
         return round(100 * ncorrect / ntotal, 2)
 
 
-def merge_dicts(d1, d2):
+def merge_dicts(d1, d2) -> dict:
     merged = {}
     for k, v in d1.items():
         if k in d2:
             merged[f"example_{k}"] = v
         else:
             merged[k] = v
 
@@ -236,33 +266,30 @@
             merged[f"pred_{k}"] = v
         else:
             merged[k] = v
 
     return merged
 
 
-def truncate_cell(content):
+def truncate_cell(content) -> str:
     """Truncate content of a cell to 25 words."""
     words = str(content).split()
     if len(words) > 25:
         return " ".join(words[:25]) + "..."
     return content
 
 
-def configure_dataframe_display(df, metric_name):
+def configure_dataframe_display(df, metric_name) -> pd.DataFrame:
     """Set various pandas display options for DataFrame."""
     pd.options.display.max_colwidth = None
     pd.set_option("display.max_colwidth", 20)  # Adjust the number as needed
     pd.set_option("display.width", 400)  # Adjust
 
-    # df[metric_name] = df[metric_name].apply(lambda x: f'✔️ [{x}]' if x is True else f'❌ [{x}]')
-    # df.loc[:, metric_name] = df[metric_name].apply(lambda x: f"✔️ [{x}]" if x is True else f"{x}")
     df[metric_name] = df[metric_name].apply(lambda x: f"✔️ [{x}]" if x else str(x))
 
-
     # Return styled DataFrame
     return df.style.set_table_styles(
         [
             {"selector": "th", "props": [("text-align", "left")]},
             {"selector": "td", "props": [("text-align", "left")]},
         ],
     ).set_properties(
@@ -272,8 +299,9 @@
             "word-wrap": "break-word",
             "max-width": "400px",
         },
     )
 
 
 # FIXME: TODO: The merge_dicts stuff above is way too quick and dirty.
-# TODO: the display_table can't handle False but can handle 0! Not sure how it works with True exactly, probably fails too.
+# TODO: the display_table can't handle False but can handle 0!
+# Not sure how it works with True exactly, probably fails too.
```

### Comparing `dspy-ai-2.4.9/dspy/evaluate/metrics.py` & `dspy_ai-2.5.0rc1/dspy/evaluate/metrics.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/experimental/synthesizer/config.py` & `dspy_ai-2.5.0rc1/dspy/experimental/synthesizer/config.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/experimental/synthesizer/instruction_suffixes.py` & `dspy_ai-2.5.0rc1/dspy/experimental/synthesizer/instruction_suffixes.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/experimental/synthesizer/signatures.py` & `dspy_ai-2.5.0rc1/dspy/experimental/synthesizer/signatures.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/experimental/synthesizer/utils.py` & `dspy_ai-2.5.0rc1/dspy/experimental/synthesizer/utils.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/experimental/synthetic_data.py` & `dspy_ai-2.5.0rc1/dspy/experimental/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/functional/functional.py` & `dspy_ai-2.5.0rc1/dspy/functional/functional.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,29 +18,29 @@
     def _predictor(func) -> dspy.Module:
         """Decorator that creates a predictor module based on the provided function."""
         signature = _func_to_signature(func)
         *_, output_key = signature.output_fields.keys()
         return _StripOutput(TypedPredictor(signature, **kwargs), output_key)
 
     # if we have only a single callable argument, the decorator was invoked with no key word arguments
-    #  so we just return the wrapped function 
+    #  so we just return the wrapped function
     if len(args) == 1 and callable(args[0]) and len(kwargs) == 0:
         return _predictor(args[0])
     return _predictor
 
 
 def cot(*args, **kwargs):
     def _cot(func) -> dspy.Module:
         """Decorator that creates a chain of thought module based on the provided function."""
         signature = _func_to_signature(func)
         *_, output_key = signature.output_fields.keys()
         return _StripOutput(TypedChainOfThought(signature, **kwargs), output_key)
 
     # if we have only a single callable argument, the decorator was invoked with no key word arguments
-    #  so we just return the wrapped function 
+    #  so we just return the wrapped function
     if len(args) == 1 and callable(args[0]) and len(kwargs) == 0:
         return _cot(args[0])
     return _cot
 
 
 class _StripOutput(dspy.Module):
     def __init__(self, predictor, output_key):
@@ -213,15 +213,15 @@
                     signature = signature.with_updated_fields(
                         name,
                         desc=field.json_schema_extra.get("desc", "")
                         + (" (Respond with true or false)" if type_ != str else ""),
                         format=lambda x: x if isinstance(x, str) else str(x),
                         parser=parse,
                     )
-                elif type_ in (str, int, float, bool):
+                elif type_ in (str, int, float):
                     signature = signature.with_updated_fields(
                         name,
                         desc=field.json_schema_extra.get("desc", "")
                         + (f" (Respond with a single {type_.__name__} value)" if type_ != str else ""),
                         format=lambda x: x if isinstance(x, str) else str(x),
                         parser=type_,
                     )
```

### Comparing `dspy-ai-2.4.9/dspy/predict/aggregation.py` & `dspy_ai-2.5.0rc1/dspy/predict/aggregation.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/predict/chain_of_thought.py` & `dspy_ai-2.5.0rc1/dspy/predict/chain_of_thought.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/predict/chain_of_thought_with_hint.py` & `dspy_ai-2.5.0rc1/dspy/predict/chain_of_thought_with_hint.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/predict/knn.py` & `dspy_ai-2.5.0rc1/dspy/predict/knn.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-from typing import List
+from typing import List, Optional
 
 import numpy as np
 
 import dsp
 
 
 class KNN:
-    def __init__(self, k: int, trainset: List[dsp.Example]):
+    def __init__(self, k: int, trainset: List[dsp.Example], vectorizer: Optional[dsp.BaseSentenceVectorizer] = None):
         self.k = k
         self.trainset = trainset
-        self.vectorizer = dsp.SentenceTransformersVectorizer()
-        trainset_casted_to_vectorize = [" | ".join([f"{key}: {value}" for key, value in example.items() if key in example._input_keys]) for example in self.trainset]
+        self.vectorizer = vectorizer or dsp.SentenceTransformersVectorizer()
+        trainset_casted_to_vectorize = [
+            " | ".join([f"{key}: {value}" for key, value in example.items() if key in example._input_keys])
+            for example in self.trainset
+        ]
         self.trainset_vectors = self.vectorizer(trainset_casted_to_vectorize).astype(np.float32)
 
     def __call__(self, **kwargs) -> List[dsp.Example]:
         with dsp.settings.context(vectorizer=self.vectorizer):
             input_example_vector = self.vectorizer([" | ".join([f"{key}: {val}" for key, val in kwargs.items()])])
             scores = np.dot(self.trainset_vectors, input_example_vector.T).squeeze()
-            nearest_samples_idxs = scores.argsort()[-self.k:][::-1]
+            nearest_samples_idxs = scores.argsort()[-self.k :][::-1]
             train_sampled = [self.trainset[cur_idx] for cur_idx in nearest_samples_idxs]
             return train_sampled
```

### Comparing `dspy-ai-2.4.9/dspy/predict/langchain.py` & `dspy_ai-2.5.0rc1/dspy/predict/langchain.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from langchain_core.runnables import Runnable
 
 import dsp
 import dspy
 from dspy.predict.parameter import Parameter
 from dspy.predict.predict import Predict
 from dspy.primitives.prediction import Prediction
-from dspy.signatures.field import InputField, OutputField
+from dspy.signatures.field import OldInputField, OldOutputField
 from dspy.signatures.signature import infer_prefix
 
 # TODO: This class is currently hard to test, because it hardcodes gpt-4 usage:
 # gpt4T = dspy.OpenAI(model='gpt-4-1106-preview', max_tokens=4000, model_type='chat')
 
 class Template2Signature(dspy.Signature):
     """You are a processor for prompts. I will give you a prompt template (Python f-string) for an arbitrary task for other LMs.
@@ -69,16 +69,16 @@
         return self.forward(**kwargs)
     
     def _build_signature(self, template):
         gpt4T = dspy.OpenAI(model='gpt-4-1106-preview', max_tokens=4000, model_type='chat')
 
         with dspy.context(lm=gpt4T): parts = dspy.Predict(Template2Signature)(template=template)
 
-        inputs = {k.strip(): InputField() for k in parts.input_keys.split(',')}
-        outputs = {k.strip(): OutputField() for k in parts.output_key.split(',')}
+        inputs = {k.strip(): OldInputField() for k in parts.input_keys.split(',')}
+        outputs = {k.strip(): OldOutputField() for k in parts.output_key.split(',')}
 
         for k, v in inputs.items():
             v.finalize(k, infer_prefix(k))  # TODO: Generate from the template at dspy.Predict(Template2Signature)
 
         for k, v in outputs.items():
             output_field_key = k
             v.finalize(k, infer_prefix(k))
```

### Comparing `dspy-ai-2.4.9/dspy/predict/multi_chain_comparison.py` & `dspy_ai-2.5.0rc1/dspy/predict/multi_chain_comparison.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/predict/predict.py` & `dspy_ai-2.5.0rc1/dspy/predict/predict.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/predict/program_of_thought.py` & `dspy_ai-2.5.0rc1/dspy/predict/program_of_thought.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/predict/react.py` & `dspy_ai-2.5.0rc1/dspy/predict/react.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,19 +24,24 @@
         self.output_fields = self.signature.output_fields
 
         assert len(self.output_fields) == 1, "ReAct only supports one output field."
 
         inputs_ = ", ".join([f"`{k}`" for k in self.input_fields.keys()])
         outputs_ = ", ".join([f"`{k}`" for k in self.output_fields.keys()])
 
-        instr = [
+        instr = []
+        
+        if self.signature.instructions is not None:
+            instr.append(f"{self.signature.instructions}\n")
+        
+        instr.extend([
             f"You will be given {inputs_} and you will respond with {outputs_}.\n",
             "To do this, you will interleave Thought, Action, and Observation steps.\n",
             "Thought can reason about the current situation, and Action can be the following types:\n",
-        ]
+        ])
 
         self.tools["Finish"] = dspy.Example(
             name="Finish",
             input_variable=outputs_.strip("`"),
             desc=f"returns the final {outputs_} and finishes the task",
         )
```

### Comparing `dspy-ai-2.4.9/dspy/predict/retry.py` & `dspy_ai-2.5.0rc1/dspy/predict/retry.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 from .predict import Predict
 
 
 class Retry(Predict):
     def __init__(self, module):
         super().__init__(module.signature)
         self.module = module
-        self.original_signature = module.signature
+        self.original_signature = module.extended_signature if isinstance(module, dspy.ChainOfThought) else module.signature
         self.original_forward = module.forward
         self.new_signature = self._create_new_signature(self.original_signature)
 
     def _create_new_signature(self, signature):
         # Add "Past" input fields for each output field
         for key, value in signature.output_fields.items():
+            actual_prefix = value.json_schema_extra["prefix"].split(":")[0] + ":"
             signature = signature.append(f"past_{key}", dspy.InputField(
-                prefix="Past " + value.json_schema_extra["prefix"],
-                desc="past output with errors",
+                prefix="Previous " + actual_prefix,
+                desc=f"past {actual_prefix} with errors",
                 format=value.json_schema_extra.get("format"),
             ))
 
         signature = signature.append("feedback", dspy.InputField(
             prefix="Instructions:",
             desc="Some instructions you must satisfy",
             format=str,
```

### Comparing `dspy-ai-2.4.9/dspy/primitives/assertions.py` & `dspy_ai-2.5.0rc1/dspy/primitives/assertions.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,18 +101,18 @@
     """DSPy Suggestion"""
 
     def __call__(self) -> Any:
         if isinstance(self.result, bool):
             if self.result:
                 return True
             elif dspy.settings.bypass_suggest:
-                dspy.logger.error(f"SuggestionFailed: {self.msg}")
+                dspy.logger.info(f"SuggestionFailed: {self.msg}")
                 return True
             else:
-                dspy.logger.error(f"SuggestionFailed: {self.msg}")
+                dspy.logger.info(f"SuggestionFailed: {self.msg}")
                 raise DSPySuggestionError(
                     id=self.id,
                     msg=self.msg,
                     target_module=self.target_module,
                     state=dsp.settings.trace,
                     is_metric=self.is_metric,
                 )
@@ -253,16 +253,15 @@
                             # save unique feedback message for predictor
                             if error_msg not in dspy.settings.predictor_feedbacks.setdefault(
                                 dspy.settings.backtrack_to,
                                 [],
                             ):
                                 dspy.settings.predictor_feedbacks[dspy.settings.backtrack_to].append(error_msg)
 
-                            # assert isinstance(error_state[0].signature, dspy.Signature)
-                            output_fields = error_state[0].signature.output_fields
+                            output_fields = error_state[0].new_signature.output_fields
                             past_outputs = {}
                             for field_name in output_fields.keys():
                                 past_outputs[field_name] = getattr(
                                     error_state[2],
                                     field_name,
                                     None,
                                 )
```

### Comparing `dspy-ai-2.4.9/dspy/primitives/box.py` & `dspy_ai-2.5.0rc1/dspy/primitives/box.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/primitives/example.py` & `dspy_ai-2.5.0rc1/dspy/primitives/example.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/primitives/module.py` & `dspy_ai-2.5.0rc1/dspy/primitives/module.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/primitives/prediction.py` & `dspy_ai-2.5.0rc1/dspy/primitives/prediction.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/primitives/program.py` & `dspy_ai-2.5.0rc1/dspy/primitives/program.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/primitives/python_interpreter.py` & `dspy_ai-2.5.0rc1/dspy/primitives/python_interpreter.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/retrieve/azureaisearch_rm.py` & `dspy_ai-2.5.0rc1/dspy/retrieve/azureaisearch_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/retrieve/chromadb_rm.py` & `dspy_ai-2.5.0rc1/dspy/retrieve/chromadb_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/retrieve/clarifai_rm.py` & `dspy_ai-2.5.0rc1/dspy/retrieve/clarifai_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/retrieve/databricks_rm.py` & `dspy_ai-2.5.0rc1/dspy/retrieve/databricks_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/retrieve/deeplake_rm.py` & `dspy_ai-2.5.0rc1/dspy/retrieve/deeplake_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/retrieve/faiss_rm.py` & `dspy_ai-2.5.0rc1/dspy/retrieve/faiss_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/retrieve/marqo_rm.py` & `dspy_ai-2.5.0rc1/dspy/retrieve/marqo_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/retrieve/milvus_rm.py` & `dspy_ai-2.5.0rc1/dspy/retrieve/milvus_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/retrieve/mongodb_atlas_rm.py` & `dspy_ai-2.5.0rc1/dspy/retrieve/mongodb_atlas_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/retrieve/neo4j_rm.py` & `dspy_ai-2.5.0rc1/dspy/retrieve/neo4j_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/retrieve/pgvector_rm.py` & `dspy_ai-2.5.0rc1/dspy/retrieve/pgvector_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/retrieve/pinecone_rm.py` & `dspy_ai-2.5.0rc1/dspy/retrieve/pinecone_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/retrieve/ragatouille_rm.py` & `dspy_ai-2.5.0rc1/dspy/retrieve/ragatouille_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/retrieve/retrieve.py` & `dspy_ai-2.5.0rc1/dspy/retrieve/retrieve.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/retrieve/vectara_rm.py` & `dspy_ai-2.5.0rc1/dspy/retrieve/vectara_rm.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 def remove_snippet(s: str) -> str:
     return s.replace(START_SNIPPET, "").replace(END_SNIPPET, "")
 
 class VectaraRM(dspy.Retrieve):
     """
     A retrieval module that uses Vectara to return the top passages for a given query.
 
-    Assumes that a Vectara corpus has been created and populated with the following payload:
+    Assumes that a Vectara corpora have been created and populated with the following payload:
         - document: The text of the passage
 
     Args:
         vectara_customer_id (str): Vectara Customer ID. defaults to VECTARA_CUSTOMER_ID environment variable
         vectara_corpus_id (str): Vectara Corpus ID. defaults to VECTARA_CORPUS_ID environment variable
         vectara_api_key (str): Vectara API Key. defaults to VECTARA_API_KEY environment variable
         k (int, optional): The default number of top passages to retrieve. Defaults to 3.
@@ -63,39 +63,43 @@
         self._n_sentences_before = self._n_sentences_after = 2
         self._vectara_timeout = 120
         super().__init__(k=k)
 
     def _vectara_query(
         self,
         query: str,
-        limit: int = 3,
+        limit: int = 5,
     ) -> List[str]:
         """Query Vectara index to get for top k matching passages.
         Args:
             query: query string
         """
-        corpus_key = {
-            "customerId": self._vectara_customer_id,
-            "corpusId": self._vectara_corpus_id,
-            "lexicalInterpolationConfig": {"lambda": 0.025 },
-        }
+        # If multiple corpus ids are provided (comma-separated), create a list of corpus keys
+        # otherwise by default, the `split(',')` is a no-op so retains the single corpus id
+        corpus_key = [
+            {
+                "customerId": self._vectara_customer_id,
+                "corpusId": corpus_id,
+                "lexicalInterpolationConfig": {"lambda": 0.025 },
+            } for corpus_id in self._vectara_corpus_id.split(',')
+        ]
 
         data = {
             "query": [
                 {
                     "query": query,
                     "start": 0,
                     "numResults": limit,
                     "contextConfig": {
                         "sentencesBefore": self._n_sentences_before,
                         "sentencesAfter": self._n_sentences_after,
                         "startTag": START_SNIPPET,
                         "endTag": END_SNIPPET,
                     },
-                    "corpusKey": [corpus_key],
+                    "corpusKey": corpus_key,
                 },
             ],
         }
 
         headers = {
             "x-api-key": self._vectara_api_key,
             "customer-id": self._vectara_customer_id,
```

### Comparing `dspy-ai-2.4.9/dspy/retrieve/weaviate_rm.py` & `dspy_ai-2.5.0rc1/dspy/retrieve/weaviate_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/retrieve/you_rm.py` & `dspy_ai-2.5.0rc1/dspy/retrieve/you_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/signatures/field.py` & `dspy_ai-2.5.0rc1/dspy/signatures/field.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/signatures/signature.py` & `dspy_ai-2.5.0rc1/dspy/signatures/signature.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import ast
+import inspect
 import re
 import types
 import typing
 from copy import deepcopy
 from typing import Any, Dict, Tuple, Type, Union  # noqa: UP035
 
 from pydantic import BaseModel, Field, create_model
@@ -84,15 +85,15 @@
     def signature(cls) -> str:
         in_args = ", ".join(cls.input_fields.keys())
         out_args = ", ".join(cls.output_fields.keys())
         return f"{in_args} -> {out_args}"
 
     @property
     def instructions(cls) -> str:
-        return getattr(cls, "__doc__", "")
+        return inspect.cleandoc(getattr(cls, "__doc__", ""))
 
     def with_instructions(cls, instructions: str) -> Type["Signature"]:
         return Signature(cls.fields, instructions)
 
     @property
     def fields(cls) -> dict[str, FieldInfo]:
         # Make sure to give input fields before output fields
@@ -213,17 +214,17 @@
         return Signature(signature, instructions)
     if instructions is not None:
         raise ValueError("Don't specify instructions when initializing with a Signature")
     return signature
 
 
 def make_signature(
-    signature: Union[str, Dict[str, Tuple[type, FieldInfo]]],
-    instructions: str = None,
-    signature_name: str = "StringSignature",
+        signature: Union[str, Dict[str, Tuple[type, FieldInfo]]],
+        instructions: str = None,
+        signature_name: str = "StringSignature",
 ) -> Type[Signature]:
     """Create a new Signature type with the given fields and instructions.
 
     Note:
         Even though we're calling a type, we're not making an instance of the type.
         In general, instances of Signature types are not allowed to be made. The call
         syntax is provided for convenience.
```

### Comparing `dspy-ai-2.4.9/dspy/teleprompt/bootstrap.py` & `dspy_ai-2.5.0rc1/dspy/teleprompt/bootstrap.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import random
 import threading
+from typing import Dict, Optional
 
 import tqdm
 
 import dsp
 import dspy
 from dspy.primitives import Example
 
@@ -11,54 +12,76 @@
 from .vanilla import LabeledFewShot
 
 # TODO: metrics should return an object with __bool__ basically, but fine if they're more complex.
 # They can also be sortable.
 
 # TODO: Switch here from dsp.Example to dspy.Example. Right now, it's okay because it's internal only (predictors).
 # NOTE: Notice the places where we don't shuffle examples. I do like that this one doesn't shuffle.
-# Other ones that consider options may want to use both unshuffled and then shuffle a few times, when considering candidates.
+# Other ones that consider options may want to use both unshuffled and then shuffle a few times, when
+# considering candidates.
 
 # TODO: the max_rounds via branch_idx to get past the cache, not just temperature.
 # In principle, we can also sample multiple outputs from the final generation step
 # (or even each step, in case the validation function just wants *one* thing that works, but nah)
 # and try them all. Having a pretty solid guess on the "final step" of each example isn't hard by the second round,
 # in the sense that we have the trace from the first round. (Yes it may change but that's an edge case that
 # won't hurt our "best effort" guarantees.)
 
 # TODO: When this bootstraps for another teleprompter like finetune, we want all demos we gather.
-# But when it's for direct use we may want to sample ONE demo per predictor--example pair. This is important for "multi-use" modules.
+# But when it's for direct use we may want to sample ONE demo per predictor--example pair.
+# This is important for "multi-use" modules.
 
 # TODO: Add baselines=[...]
 
-
 class BootstrapFewShot(Teleprompter):
     def __init__(
         self,
         metric=None,
         metric_threshold=None,
-        teacher_settings={},
+        teacher_settings: Optional[Dict]=None,
         max_bootstrapped_demos=4,
         max_labeled_demos=16,
         max_rounds=1,
         max_errors=5,
     ):
+        """
+        A Teleprompter class that composes a set of demos/examples to go into a predictor's prompt.
+        These demos come from a combination of labeled examples in the training set, and bootstrapped demos.
+
+        Parameters
+        ----------
+        metric: Callable
+            A function that compares an expected value and predicted value, outputting the result of that comparison. 
+        metric_threshold: optional float, default `None`
+            If the metric yields a numerical value, then check it against this threshold when
+            deciding whether or not to accept a bootstrap example.
+        teacher_settings: dict, optional
+            Settings for the `teacher` model.
+        max_bootstrapped_demos: int, default 4
+            Maximum number of bootstrapped demonstrations to include
+        max_labeled_demos: int, default 16
+            Maximum number of labeled demonstrations to include.
+        max_rounds: int, default 1
+            Number of iterations to attempt generating the required bootstrap examples. If unsuccessful after `max_rounds`, the program ends.
+        max_errors: int, default 5
+            Maximum number of errors until program ends.
+        """
         self.metric = metric
         self.metric_threshold = metric_threshold
-        self.teacher_settings = teacher_settings
+        self.teacher_settings = {} if teacher_settings is None else teacher_settings
 
         self.max_bootstrapped_demos = max_bootstrapped_demos
         self.max_labeled_demos = max_labeled_demos
         self.max_rounds = max_rounds
         self.max_errors = max_errors
         self.error_count = 0
         self.error_lock = threading.Lock()
 
-    def compile(self, student, *, teacher=None, trainset, valset=None):
+    def compile(self, student, *, teacher=None, trainset):
         self.trainset = trainset
-        self.valset = valset
 
         self._prepare_student_and_teacher(student, teacher)
         self._prepare_predictor_mappings()
         self._bootstrap()
 
         self.student = self._train()
         self.student._compiled = True
@@ -87,15 +110,17 @@
             teacher.predictors(),
         ), "Student and teacher must have the same number of predictors."
 
         for (name1, predictor1), (name2, predictor2) in zip(student.named_predictors(), teacher.named_predictors()):
             assert name1 == name2, "Student and teacher must have the same program structure."
             assert predictor1.signature.equals(
                 predictor2.signature,
-            ), f"Student and teacher must have the same signatures. {type(predictor1.signature)} != {type(predictor2.signature)}"
+            ), (f"Student and teacher must have the same signatures. "
+                f"{type(predictor1.signature)} != {type(predictor2.signature)}"
+                )
             assert id(predictor1) != id(predictor2), "Student and teacher must be different objects."
 
             name2predictor[name1] = None  # dict(student=predictor1, teacher=predictor2)
             predictor2name[id(predictor1)] = name1
 
             # FIXME(shangyint): This is an ugly hack to bind traces of
             # retry.module to retry
@@ -129,15 +154,15 @@
         )
 
         # Unbootstrapped training examples
 
         self.validation = [x for idx, x in enumerate(self.trainset) if idx not in bootstrapped]
         random.Random(0).shuffle(self.validation)
 
-        self.validation = self.valset or self.validation
+        self.validation = self.validation
 
         # NOTE: Can't yet use evaluate because we need to trace *per example*
         # evaluate = Evaluate(program=self.teacher, metric=self.metric, num_threads=12)
         # score = evaluate(self.metric, display_table=False, display_progress=True)
 
     def _bootstrap_one_example(self, example, round_idx=0):
         name2traces = self.name2traces
```

### Comparing `dspy-ai-2.4.9/dspy/teleprompt/copro_optimizer.py` & `dspy_ai-2.5.0rc1/dspy/teleprompt/copro_optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,25 @@
     def _set_signature(self, predictor, updated_signature):
         if hasattr(predictor, "extended_signature"):
             predictor.extended_signature = updated_signature
         elif hasattr(predictor, "signature"):
             predictor.signature = updated_signature
 
     def compile(self, student, *, trainset, eval_kwargs):
-        """student is a program that needs to be optimized, note that it may be zero-shot or already pre-optimized for demos != []"""
+        """
+        optimizes `signature` of `student` program - note that it may be zero-shot or already pre-optimized (demos already chosen - `demos != []`)
+
+        parameters:
+        student: program to optimize and left modified.
+        trainset: iterable of `Example`s
+        eval_kwargs: optional, dict
+           Additional keywords to go into `Evaluate` for the metric.
+
+        Returns optimized version of `student`.
+        """
         module = student.deepcopy()
         evaluate = Evaluate(devset=trainset, metric=self.metric, **eval_kwargs)
         total_calls = 0
         results_best = {
             id(p): {"depth": [], "max": [], "average": [], "min": [], "std": []} for p in module.predictors()
         }
         results_latest = {
```

### Comparing `dspy-ai-2.4.9/dspy/teleprompt/ensemble.py` & `dspy_ai-2.5.0rc1/dspy/teleprompt/ensemble.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/teleprompt/finetune.py` & `dspy_ai-2.5.0rc1/dspy/teleprompt/finetune.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/teleprompt/knn_fewshot.py` & `dspy_ai-2.5.0rc1/dspy/teleprompt/knn_fewshot.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import types
-from typing import List
+from typing import List, Optional
 
 import dsp
+from dspy.predict.knn import KNN
 from dspy.teleprompt import BootstrapFewShot
 
 from .teleprompt import Teleprompter
 
 
 class KNNFewShot(Teleprompter):
-    def __init__(self, KNN, k: int, trainset: List[dsp.Example]):
-        self.KNN = KNN(k, trainset)
+    def __init__(self, k: int, trainset: List[dsp.Example], vectorizer: Optional[dsp.BaseSentenceVectorizer] = None):
+        self.KNN = KNN(k, trainset, vectorizer=vectorizer)
 
-    def compile(self, student, *, teacher=None, trainset, valset=None):
+    def compile(self, student, *, teacher=None, trainset=None, valset=None):
         student_copy = student.reset_copy()
 
         def forward_pass(*args, **kwargs):
             knn_trainset = self.KNN(**kwargs)
             few_shot_bootstrap = BootstrapFewShot()
             compiled_program = few_shot_bootstrap.compile(
                 student,
```

### Comparing `dspy-ai-2.4.9/dspy/teleprompt/mipro_optimizer.py` & `dspy_ai-2.5.0rc1/dspy/teleprompt/mipro_optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,27 +14,29 @@
 from dspy.signatures.signature import signature_to_template
 from dspy.teleprompt import BootstrapFewShot
 from dspy.teleprompt.teleprompt import Teleprompter
 
 """
 USAGE SUGGESTIONS:
 
-The following code can be used to compile a optimized signature teleprompter using the MIPRO, and evaluate it on an end task:
+The following code can be used to compile a optimized signature teleprompter using MIPRO, and evaluate it on an end task:
 
+``` python
 from dspy.teleprompt import MIPRO
 
 teleprompter = MIPRO(prompt_model=prompt_model, task_model=task_model, metric=metric, num_candidates=10, init_temperature=1.0)
 kwargs = dict(num_threads=NUM_THREADS, display_progress=True, display_table=0)
 compiled_prompt_opt = teleprompter.compile(program, trainset=trainset[:TRAIN_NUM], num_trials=100, max_bootstrapped_demos=3, max_labeled_demos=5, eval_kwargs=kwargs)
 eval_score = evaluate(compiled_prompt_opt, devset=evalset[:EVAL_NUM], **kwargs)
+```
 
 Note that this teleprompter takes in the following parameters:
 
-* prompt_model: The model used for prompt generation. When unspecified, defaults to the model set in settings (ie. dspy.settings.configure(lm=task_model)).
-* task_model: The model used for prompt generation. When unspecified, defaults to the model set in settings (ie. dspy.settings.configure(lm=task_model)).
+* prompt_model: The model used for prompt generation. When unspecified, defaults to the model set in settings (i.e., dspy.settings.configure(lm=task_model)).
+* task_model: The model used for prompt generation. When unspecified, defaults to the model set in settings (i.e., dspy.settings.configure(lm=task_model)).
 * metric: The task metric used for optimization.
 * num_candidates: The number of new prompts and sets of fewshot examples to generate and evaluate. Default=10.
 * init_temperature: The temperature used to generate new prompts. Higher roughly equals more creative. Default=1.0.
 * verbose: Tells the method whether or not to print intermediate steps.
 * track_stats: Tells the method whether or not to track statistics about the optimization process.
                 If True, the method will track a dictionary with a key corresponding to the trial number, 
                 and a value containing a dict with the following keys:
@@ -389,15 +391,15 @@
 
             {YELLOW}- Reducing the number of trials (`num_trials`), the size of the trainset, or the number of LM calls in your program.{ENDC}
             {YELLOW}- Using a cheaper task model to optimize the prompt.{ENDC}""")
 
         user_confirmation_message = textwrap.dedent(f"""\
             To proceed with the execution of this program, please confirm by typing {BLUE}'y'{ENDC} for yes or {BLUE}'n'{ENDC} for no.
 
-            If you would like to bypass this confirmation step in future executions, set the {YELLOW}`requires_permission_to_run`{ENDC} flag to {YELLOW}`False`.{ENDC}
+            If you would like to bypass this confirmation step in future executions, set the {YELLOW}`requires_permission_to_run`{ENDC} flag to {YELLOW}`False` when calling compile.{ENDC}
 
             {YELLOW}Awaiting your input...{ENDC}
         """)
 
         print(user_message)
 
         sys.stdout.flush()  # Flush the output buffer to force the message to print
```

### Comparing `dspy-ai-2.4.9/dspy/teleprompt/random_search.py` & `dspy_ai-2.5.0rc1/dspy/teleprompt/random_search.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/teleprompt/signature_opt.py` & `dspy_ai-2.5.0rc1/dspy/teleprompt/signature_opt.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/teleprompt/signature_opt_bayesian.py` & `dspy_ai-2.5.0rc1/dspy/teleprompt/signature_opt_bayesian.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/teleprompt/signature_opt_typed.py` & `dspy_ai-2.5.0rc1/dspy/teleprompt/signature_opt_typed.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/teleprompt/teleprompt_optuna.py` & `dspy_ai-2.5.0rc1/dspy/teleprompt/teleprompt_optuna.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         evaluate = Evaluate(
             devset=self.valset,
             metric=self.metric,
             num_threads=self.num_threads,
             display_table=False,
             display_progress=True,
         )
-        score, _ = evaluate(program2, return_all_scores=True)
+        score = evaluate(program2, return_all_scores=False)
         trial.set_user_attr("program", program2)
         return score
 
     def compile(self, student, *, teacher=None, max_demos, trainset, valset=None):
         self.trainset = trainset
         self.valset = valset or trainset
         self.student = student.reset_copy()
```

### Comparing `dspy-ai-2.4.9/dspy/teleprompt/vanilla.py` & `dspy_ai-2.5.0rc1/dspy/teleprompt/vanilla.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/utils/dummies.py` & `dspy_ai-2.5.0rc1/dspy/utils/dummies.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/dspy/utils/logging.py` & `dspy_ai-2.5.0rc1/dspy/utils/logging.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.9/pyproject.toml` & `dspy_ai-2.5.0rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,52 +1,51 @@
 [build-system]
 requires = ["setuptools>=40.8.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dspy-ai"
-version = "2.4.9"
+version = "2.5.0rc1"
 description = "DSPy"
 readme = "README.md"
 authors = [{ name = "Omar Khattab", email = "okhattab@stanford.edu" }]
 license = { text = "MIT License" }
-requires-python = ">=3.9, <3.12"
+requires-python = ">=3.9, <3.13"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
-    "Programming Language :: Python :: 3",    # removed 3.8
+    "Programming Language :: Python :: 3", # removed 3.8
     "Programming Language :: Python :: 3.9",
 ]
-
 # We have both project and tool.poetry.dependencies. Should we remove one?
 # tool.poetry.dependencies is a convenience thing for poetry users.
 # project dependencies function similarly to requirements.txt,
 # `pip install .` will pull from pyproject.toml dependencies
-
 dependencies = [
     "backoff~=2.2.1",
     "joblib~=1.3.2",
     "openai>=0.28.1,<2.0.0",
     "pandas",
     "regex",
     "ujson",
     "tqdm",
-    "datasets~=2.14.6,<3.0.0",
+    "datasets>=2.14.6,<3.0.0",
     "requests",
     "optuna",
     "pydantic~=2.0",
     "structlog",
+    "jinja2"
 ]
 
 [project.optional-dependencies]
 anthropic = ["anthropic~=0.18.0"]
 chromadb = ["chromadb~=0.4.14"]
-qdrant = ["qdrant-client>=1.6.2", "fastembed>=0.1.0"]
+qdrant = ["qdrant-client>=1.6.2", "fastembed>=0.2.0"]
 marqo = ["marqo"]
 pinecone = ["pinecone-client~=2.2.4"]
 weaviate = ["weaviate-client~=4.5.4"]
 milvus = ["pymilvus~=2.3.7"]
 aws = ["boto3~=1.34.78"]
 docs = [
     "sphinx>=4.3.0",
@@ -58,48 +57,50 @@
     "sphinx-autobuild",
     "sphinx_rtd_theme",
     "autodoc_pydantic",
     "sphinx-reredirects>=0.1.2",
     "sphinx-automodapi==0.16.0",
 ]
 dev = ["pytest>=6.2.5"]
+fastembed = ["fastembed>=0.2.0"]
 
 [project.urls]
 homepage = "https://github.com/stanfordnlp/dspy"
 
 [tool.poetry]
-name = "dspy"
-version = "2.0.8"
-description = "DSPy"
+name = "dspy-ai"
+version = "2.5.0rc1"
+description = "DSPy: The framework for programming—not prompting—foundation models"
 authors = ["Omar Khattab <okhattab@stanford.edu>"]
+maintainers = ["Cyrus Nouroozi <cyrus@edendaolab.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/stanfordnlp/dspy"
 repository = "https://github.com/stanfordnlp/dspy"
 # documentation = "https://dspy-ai.readthedocs.io"
 keywords = ["dspy", "ai", "language models", "llm", "openai"]
-# may be a bit much
-
+packages = [{ include = "dspy" }]
 
+# may be a bit much
 [tool.poetry.dependencies]
-python = ">=3.9,<3.12"
+python = ">=3.9,<3.13"
 pydantic = "^2.0"
 backoff = "^2.2.1"
 joblib = "^1.3.2"
 openai = ">=0.28.1,<2.0.0"
 pandas = "^2.1.1"
 regex = "^2023.10.3"
 ujson = "^5.8.0"
 tqdm = "^4.66.1"
 datasets = "^2.14.6"
 requests = "^2.31.0"
 optuna = "^3.4.0"
 anthropic = { version = "^0.18.0", optional = true }
 chromadb = { version = "^0.4.14", optional = true }
-fastembed = { version = "^0.1.0", optional = true }
+fastembed = { version = ">=0.2.0", optional = true }
 marqo = { version = "*", optional = true }
 qdrant-client = { version = "^1.6.2", optional = true }
 pinecone-client = { version = "^2.2.4", optional = true }
 weaviate-client = { version = "^4.5.4", optional = true }
 pymilvus = { version = "^2.3.6", optional = true }
 boto3 = { version = "^1.34.78", optional = true }
 sphinx = { version = ">=4.3.0", optional = true }
@@ -114,24 +115,27 @@
 sphinx-reredirects = { version = "^0.1.2", optional = true }
 sphinx-automodapi = { version = "0.16.0", optional = true }
 groq = { version = "^0.4.2", optional = true }
 rich = "^13.7.1"
 psycopg2 = { version = "^2.9.9", optional = true }
 pgvector = { version = "^0.2.5", optional = true }
 structlog = "^24.1.0"
-
+llama-index = { version = "^0.10.30", optional = true }
+snowflake-snowpark-python = { version = "*", optional = true, python = ">=3.9,<3.12" }
+jinja2 = "^3.1.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.2.5"
 transformers = "^4.38.2"
 torch = "^2.2.1"
 pytest-mock = "^3.12.0"
 ruff = "^0.3.0"
 black = "^24.2.0"
 pre-commit = "^3.7.0"
+ipykernel = "^6.29.4"
 
 [tool.poetry.extras]
 chromadb = ["chromadb"]
 qdrant = ["qdrant-client", "fastembed"]
 marqo = ["marqo"]
 pinecone = ["pinecone-client"]
 weaviate = ["weaviate-client"]
@@ -147,14 +151,15 @@
     "myst-nb",
     "sphinx-autobuild",
     "sphinx_rtd_theme",
     "autodoc_pydantic",
     "sphinx-reredirects",
     "sphinx-automodapi",
 ]
+fastembed = ["fastembed"]
 
 [tool.poetry.group.doc.dependencies]
 mkdocs = ">=1.5.3"
 mkdocs-material = ">=9.0.6"
 mkdocs-material-extensions = ">=1.3.1"
 mkdocs-gen-files = "^0.5.0"
 mkdocstrings-python = "^1.7.5"
@@ -275,15 +280,14 @@
     "D102",
     "D103",
     # Inline lambdas
     "E731",
     # Sometimes we need List and Tuple
     "UP006",
 ]
-
 # Allow fix for all enabled rules (when `--fix`) is provided.
 fixable = ["ALL"]
 unfixable = []
 
 [tool.ruff.format]
 docstring-code-format = true
 quote-style = "double"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

