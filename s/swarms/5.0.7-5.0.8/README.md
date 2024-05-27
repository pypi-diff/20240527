# Comparing `tmp/swarms-5.0.7.tar.gz` & `tmp/swarms-5.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-5.0.7.tar", max compression
+gzip compressed data, was "swarms-5.0.8.tar", max compression
```

## Comparing `swarms-5.0.7.tar` & `swarms-5.0.8.tar`

### file list

```diff
@@ -1,209 +1,213 @@
--rw-r--r--   0        0        0    15674 2024-05-20 23:12:19.525914 swarms-5.0.7/LICENSE
--rw-r--r--   0        0        0    33713 2024-05-21 21:17:55.232096 swarms-5.0.7/README.md
--rw-r--r--   0        0        0     1790 2024-05-24 17:37:48.017729 swarms-5.0.7/pyproject.toml
--rw-r--r--   0        0        0      590 2024-05-20 23:12:19.584595 swarms-5.0.7/swarms/__init__.py
--rw-r--r--   0        0        0      864 2024-05-20 23:12:19.584679 swarms-5.0.7/swarms/agents/__init__.py
--rw-r--r--   0        0        0      881 2024-05-20 23:12:19.584738 swarms-5.0.7/swarms/agents/agent_wrapper.py
--rw-r--r--   0        0        0     3342 2024-05-20 23:12:19.584796 swarms-5.0.7/swarms/agents/base.py
--rw-r--r--   0        0        0     4201 2024-05-20 23:12:19.584880 swarms-5.0.7/swarms/agents/developer_agents.py
--rw-r--r--   0        0        0     2950 2024-05-20 23:12:19.584947 swarms-5.0.7/swarms/agents/omni_modal_agent.py
--rw-r--r--   0        0        0     3491 2024-05-20 23:12:19.585001 swarms-5.0.7/swarms/agents/simple_agent.py
--rw-r--r--   0        0        0      484 2024-05-20 23:12:19.585048 swarms-5.0.7/swarms/agents/stopping_conditions.py
--rw-r--r--   0        0        0     4940 2024-05-20 23:12:19.585129 swarms-5.0.7/swarms/agents/tool_agent.py
--rw-r--r--   0        0        0     5504 2024-05-20 23:12:19.585192 swarms-5.0.7/swarms/agents/worker_agent.py
--rw-r--r--   0        0        0      167 2024-05-20 23:12:19.585283 swarms-5.0.7/swarms/artifacts/__init__.py
--rw-r--r--   0        0        0     1675 2024-05-20 23:12:19.585343 swarms-5.0.7/swarms/artifacts/base_artifact.py
--rw-r--r--   0        0        0     2299 2024-05-20 23:12:19.585425 swarms-5.0.7/swarms/artifacts/text_artifact.py
--rw-r--r--   0        0        0      613 2024-05-20 23:12:19.585515 swarms-5.0.7/swarms/memory/__init__.py
--rw-r--r--   0        0        0      433 2024-05-20 23:12:19.585565 swarms-5.0.7/swarms/memory/action_subtask.py
--rw-r--r--   0        0        0     3475 2024-05-20 23:12:19.585621 swarms-5.0.7/swarms/memory/base_db.py
--rw-r--r--   0        0        0     2823 2024-05-20 23:12:19.585702 swarms-5.0.7/swarms/memory/base_vectordb.py
--rw-r--r--   0        0        0     2895 2024-05-20 23:12:19.585767 swarms-5.0.7/swarms/memory/dict_internal_memory.py
--rw-r--r--   0        0        0     3306 2024-05-20 23:12:19.585826 swarms-5.0.7/swarms/memory/dict_shared_memory.py
--rw-r--r--   0        0        0     5499 2024-05-20 23:12:19.585895 swarms-5.0.7/swarms/memory/short_term_memory.py
--rw-r--r--   0        0        0     3371 2024-05-20 23:12:19.585978 swarms-5.0.7/swarms/memory/visual_memory.py
--rw-r--r--   0        0        0     2392 2024-05-21 05:06:54.045652 swarms-5.0.7/swarms/models/__init__.py
--rw-r--r--   0        0        0     2052 2024-05-21 00:48:59.027928 swarms-5.0.7/swarms/models/base_embedding_model.py
--rw-r--r--   0        0        0    13168 2024-05-20 23:12:19.586207 swarms-5.0.7/swarms/models/base_llm.py
--rw-r--r--   0        0        0    12604 2024-05-20 23:12:19.586302 swarms-5.0.7/swarms/models/base_multimodal_model.py
--rw-r--r--   0        0        0     2475 2024-05-20 23:12:19.586361 swarms-5.0.7/swarms/models/base_tts.py
--rw-r--r--   0        0        0     3163 2024-05-20 23:12:19.586416 swarms-5.0.7/swarms/models/base_ttv.py
--rw-r--r--   0        0        0    16743 2024-05-20 23:12:19.586490 swarms-5.0.7/swarms/models/cog_vlm.py
--rw-r--r--   0        0        0    10760 2024-05-20 23:12:19.586608 swarms-5.0.7/swarms/models/dalle3.py
--rw-r--r--   0        0        0     6449 2024-05-20 23:12:19.586690 swarms-5.0.7/swarms/models/distilled_whisperx.py
--rw-r--r--   0        0        0      682 2024-05-20 23:12:19.586747 swarms-5.0.7/swarms/models/embeddings_base.py
--rw-r--r--   0        0        0     3022 2024-05-20 23:12:19.586804 swarms-5.0.7/swarms/models/fuyu.py
--rw-r--r--   0        0        0     7762 2024-05-20 23:12:19.586891 swarms-5.0.7/swarms/models/gemini.py
--rw-r--r--   0        0        0    14236 2024-05-20 23:12:19.586973 swarms-5.0.7/swarms/models/gpt4_vision_api.py
--rw-r--r--   0        0        0    12996 2024-05-20 23:12:19.587047 swarms-5.0.7/swarms/models/huggingface.py
--rw-r--r--   0        0        0     1826 2024-05-20 23:12:19.587108 swarms-5.0.7/swarms/models/huggingface_pipeline.py
--rw-r--r--   0        0        0     5601 2024-05-20 23:12:19.587202 swarms-5.0.7/swarms/models/idefics.py
--rw-r--r--   0        0        0    10672 2024-05-20 23:12:19.587276 swarms-5.0.7/swarms/models/kosmos_two.py
--rw-r--r--   0        0        0     1448 2024-05-20 23:12:19.587347 swarms-5.0.7/swarms/models/layoutlm_document_qa.py
--rw-r--r--   0        0        0     2599 2024-05-21 05:06:21.835242 swarms-5.0.7/swarms/models/llama3_hosted.py
--rw-r--r--   0        0        0     6581 2024-05-20 23:12:19.587506 swarms-5.0.7/swarms/models/llama_function_caller.py
--rw-r--r--   0        0        0     2762 2024-05-20 23:12:19.587573 swarms-5.0.7/swarms/models/llava.py
--rw-r--r--   0        0        0     2056 2024-05-20 23:12:19.587792 swarms-5.0.7/swarms/models/moondream_mm.py
--rw-r--r--   0        0        0     2881 2024-05-20 23:12:19.587858 swarms-5.0.7/swarms/models/nougat.py
--rw-r--r--   0        0        0     2366 2024-05-20 23:12:19.587917 swarms-5.0.7/swarms/models/open_dalle.py
--rw-r--r--   0        0        0     2464 2024-05-20 23:12:19.587972 swarms-5.0.7/swarms/models/open_router.py
--rw-r--r--   0        0        0      106 2024-05-20 23:12:19.588047 swarms-5.0.7/swarms/models/openai_embeddings.py
--rw-r--r--   0        0        0     3167 2024-05-20 23:12:19.588099 swarms-5.0.7/swarms/models/openai_tts.py
--rw-r--r--   0        0        0       93 2024-05-20 23:12:19.588149 swarms-5.0.7/swarms/models/palm.py
--rw-r--r--   0        0        0     2160 2024-05-20 23:12:19.588204 swarms-5.0.7/swarms/models/popular_llms.py
--rw-r--r--   0        0        0     4813 2024-05-20 23:12:19.588296 swarms-5.0.7/swarms/models/qwen.py
--rw-r--r--   0        0        0     3561 2024-05-20 23:12:19.588355 swarms-5.0.7/swarms/models/sam.py
--rw-r--r--   0        0        0    12675 2024-05-20 23:12:19.588421 swarms-5.0.7/swarms/models/sampling_params.py
--rw-r--r--   0        0        0     8244 2024-05-20 23:12:19.588474 swarms-5.0.7/swarms/models/ssd_1b.py
--rw-r--r--   0        0        0     3948 2024-05-20 23:12:19.588553 swarms-5.0.7/swarms/models/together.py
--rw-r--r--   0        0        0      592 2024-05-20 23:12:19.588607 swarms-5.0.7/swarms/models/types.py
--rw-r--r--   0        0        0     1731 2024-05-20 23:12:19.588664 swarms-5.0.7/swarms/models/vilt.py
--rw-r--r--   0        0        0     2846 2024-05-20 23:12:19.588711 swarms-5.0.7/swarms/models/vip_llava.py
--rw-r--r--   0        0        0     3666 2024-05-20 23:12:19.588784 swarms-5.0.7/swarms/models/zeroscope.py
--rw-r--r--   0        0        0        0 2024-05-20 23:12:19.588836 swarms-5.0.7/swarms/prebuilt_swarms/__init__.py
--rw-r--r--   0        0        0      692 2024-05-20 23:12:19.588923 swarms-5.0.7/swarms/prompts/__init__.py
--rw-r--r--   0        0        0    11320 2024-05-20 23:12:19.588988 swarms-5.0.7/swarms/prompts/accountant_swarm_prompts.py
--rw-r--r--   0        0        0     9156 2024-05-20 23:12:19.589069 swarms-5.0.7/swarms/prompts/aga.py
--rw-r--r--   0        0        0     1451 2024-05-20 23:12:19.589128 swarms-5.0.7/swarms/prompts/agent_output_parser.py
--rw-r--r--   0        0        0     2705 2024-05-20 23:12:19.589180 swarms-5.0.7/swarms/prompts/agent_prompt.py
--rw-r--r--   0        0        0     6886 2024-05-20 23:12:19.589236 swarms-5.0.7/swarms/prompts/agent_prompts.py
--rw-r--r--   0        0        0     7113 2024-05-20 23:12:19.589316 swarms-5.0.7/swarms/prompts/agent_system_prompts.py
--rw-r--r--   0        0        0     5233 2024-05-20 23:12:19.589377 swarms-5.0.7/swarms/prompts/ai_research_team.py
--rw-r--r--   0        0        0     1148 2024-05-20 23:12:19.589426 swarms-5.0.7/swarms/prompts/aot_prompt.py
--rw-r--r--   0        0        0    13981 2024-05-20 23:12:19.589498 swarms-5.0.7/swarms/prompts/autobloggen.py
--rw-r--r--   0        0        0     5605 2024-05-20 23:12:19.589584 swarms-5.0.7/swarms/prompts/autoswarm.py
--rw-r--r--   0        0        0     7542 2024-05-20 23:12:19.589647 swarms-5.0.7/swarms/prompts/base.py
--rw-r--r--   0        0        0     3801 2024-05-20 23:12:19.589703 swarms-5.0.7/swarms/prompts/chat_prompt.py
--rw-r--r--   0        0        0     2235 2024-05-20 23:12:19.589756 swarms-5.0.7/swarms/prompts/code_interpreter.py
--rw-r--r--   0        0        0     4106 2024-05-20 23:12:19.589834 swarms-5.0.7/swarms/prompts/code_spawner.py
--rw-r--r--   0        0        0     1566 2024-05-20 23:12:19.589885 swarms-5.0.7/swarms/prompts/debate.py
--rw-r--r--   0        0        0     7157 2024-05-23 01:40:32.871666 swarms-5.0.7/swarms/prompts/documentation.py
--rw-r--r--   0        0        0     1767 2024-05-20 23:12:19.590009 swarms-5.0.7/swarms/prompts/education.py
--rw-r--r--   0        0        0     4180 2024-05-20 23:12:19.590089 swarms-5.0.7/swarms/prompts/finance_agent_prompt.py
--rw-r--r--   0        0        0     4117 2024-05-20 23:12:19.590152 swarms-5.0.7/swarms/prompts/growth_agent_prompt.py
--rw-r--r--   0        0        0      880 2024-05-20 23:12:19.590207 swarms-5.0.7/swarms/prompts/idea2img.py
--rw-r--r--   0        0        0     3346 2024-05-20 23:12:19.590267 swarms-5.0.7/swarms/prompts/legal_agent_prompt.py
--rw-r--r--   0        0        0     4785 2024-05-20 23:12:19.590358 swarms-5.0.7/swarms/prompts/logistics.py
--rw-r--r--   0        0        0     3374 2024-05-20 23:12:19.590418 swarms-5.0.7/swarms/prompts/meta_system_prompt.py
--rw-r--r--   0        0        0    10662 2024-05-20 23:12:19.590489 swarms-5.0.7/swarms/prompts/multi_modal_autonomous_instruction_prompt.py
--rw-r--r--   0        0        0     3511 2024-05-20 23:12:19.590550 swarms-5.0.7/swarms/prompts/multi_modal_prompts.py
--rw-r--r--   0        0        0     3225 2024-05-20 23:12:19.590626 swarms-5.0.7/swarms/prompts/multi_modal_visual_prompts.py
--rw-r--r--   0        0        0     3454 2024-05-20 23:12:19.590685 swarms-5.0.7/swarms/prompts/operations_agent_prompt.py
--rw-r--r--   0        0        0     2149 2024-05-20 23:12:19.590738 swarms-5.0.7/swarms/prompts/personal_stylist.py
--rw-r--r--   0        0        0     8333 2024-05-20 23:12:19.590803 swarms-5.0.7/swarms/prompts/product_agent_prompt.py
--rw-r--r--   0        0        0    10144 2024-05-20 23:12:19.590895 swarms-5.0.7/swarms/prompts/programming.py
--rw-r--r--   0        0        0     2128 2024-05-20 23:12:19.590958 swarms-5.0.7/swarms/prompts/project_manager.py
--rw-r--r--   0        0        0    13215 2024-05-20 23:12:19.591020 swarms-5.0.7/swarms/prompts/python.py
--rw-r--r--   0        0        0     2960 2024-05-20 23:12:19.591076 swarms-5.0.7/swarms/prompts/react.py
--rw-r--r--   0        0        0        0 2024-05-20 23:12:19.591117 swarms-5.0.7/swarms/prompts/refiner_agent_prompt.py
--rw-r--r--   0        0        0     5126 2024-05-20 23:12:19.591208 swarms-5.0.7/swarms/prompts/sales.py
--rw-r--r--   0        0        0     5013 2024-05-20 23:12:19.591263 swarms-5.0.7/swarms/prompts/sales_prompts.py
--rw-r--r--   0        0        0     2679 2024-05-20 23:12:19.591326 swarms-5.0.7/swarms/prompts/security_team.py
--rw-r--r--   0        0        0     3252 2024-05-20 23:12:19.591419 swarms-5.0.7/swarms/prompts/self_operating_prompt.py
--rw-r--r--   0        0        0     4147 2024-05-20 23:12:19.591487 swarms-5.0.7/swarms/prompts/sop_generator_agent_prompt.py
--rw-r--r--   0        0        0     4640 2024-05-20 23:12:19.591551 swarms-5.0.7/swarms/prompts/summaries_prompts.py
--rw-r--r--   0        0        0     3984 2024-05-20 23:12:19.591612 swarms-5.0.7/swarms/prompts/support_agent_prompt.py
--rw-r--r--   0        0        0     4280 2024-05-20 23:12:19.591714 swarms-5.0.7/swarms/prompts/swarm_manager_agent.py
--rw-r--r--   0        0        0      728 2024-05-20 23:12:19.591774 swarms-5.0.7/swarms/prompts/task_assignment_prompt.py
--rw-r--r--   0        0        0     4271 2024-05-20 23:12:19.591847 swarms-5.0.7/swarms/prompts/tests.py
--rw-r--r--   0        0        0     6577 2024-05-24 17:25:52.060992 swarms-5.0.7/swarms/prompts/tools.py
--rw-r--r--   0        0        0     2398 2024-05-20 23:12:19.592013 swarms-5.0.7/swarms/prompts/urban_planning.py
--rw-r--r--   0        0        0     3675 2024-05-20 23:12:19.592103 swarms-5.0.7/swarms/prompts/visual_cot.py
--rw-r--r--   0        0        0     5554 2024-05-20 23:12:19.592180 swarms-5.0.7/swarms/prompts/worker_prompt.py
--rw-r--r--   0        0        0     2349 2024-05-20 23:12:19.592230 swarms-5.0.7/swarms/prompts/xray_swarm_prompt.py
--rw-r--r--   0        0        0        0 2024-05-21 03:27:54.652576 swarms-5.0.7/swarms/schemas/__init__.py
--rw-r--r--   0        0        0     3168 2024-05-24 00:43:53.750806 swarms-5.0.7/swarms/schemas/hass_agent_schema.py
--rw-r--r--   0        0        0      182 2024-05-21 05:06:25.218133 swarms-5.0.7/swarms/schemas/plan.py
--rw-r--r--   0        0        0     6764 2024-05-20 23:12:19.594641 swarms-5.0.7/swarms/schemas/schemas.py
--rw-r--r--   0        0        0      709 2024-05-20 23:12:19.594792 swarms-5.0.7/swarms/schemas/step.py
--rw-r--r--   0        0        0     4084 2024-05-24 14:40:28.251160 swarms-5.0.7/swarms/structs/__init__.py
--rw-r--r--   0        0        0    61796 2024-05-24 17:32:12.443311 swarms-5.0.7/swarms/structs/agent.py
--rw-r--r--   0        0        0      574 2024-05-20 23:12:19.592548 swarms-5.0.7/swarms/structs/agent_job.py
--rw-r--r--   0        0        0     2937 2024-05-20 23:12:19.592611 swarms-5.0.7/swarms/structs/agent_process.py
--rw-r--r--   0        0        0     3777 2024-05-20 23:12:19.592668 swarms-5.0.7/swarms/structs/async_workflow.py
--rw-r--r--   0        0        0     6624 2024-05-20 23:12:19.592755 swarms-5.0.7/swarms/structs/auto_swarm.py
--rw-r--r--   0        0        0    12437 2024-05-20 23:12:19.592817 swarms-5.0.7/swarms/structs/base_structure.py
--rw-r--r--   0        0        0    19446 2024-05-20 23:12:19.592905 swarms-5.0.7/swarms/structs/base_swarm.py
--rw-r--r--   0        0        0    12161 2024-05-20 23:12:19.593000 swarms-5.0.7/swarms/structs/base_workflow.py
--rw-r--r--   0        0        0     5265 2024-05-21 00:48:59.119899 swarms-5.0.7/swarms/structs/company.py
--rw-r--r--   0        0        0     4738 2024-05-21 03:30:50.037223 swarms-5.0.7/swarms/structs/concurrent_workflow.py
--rw-r--r--   0        0        0    14685 2024-05-20 23:12:19.593392 swarms-5.0.7/swarms/structs/conversation.py
--rw-r--r--   0        0        0    12608 2024-05-20 23:12:19.593456 swarms-5.0.7/swarms/structs/debate.py
--rw-r--r--   0        0        0     4834 2024-05-20 23:12:19.593607 swarms-5.0.7/swarms/structs/groupchat.py
--rw-r--r--   0        0        0     8747 2024-05-24 15:44:24.762519 swarms-5.0.7/swarms/structs/hiearchical_swarm.py
--rw-r--r--   0        0        0     7012 2024-05-20 23:12:19.593787 swarms-5.0.7/swarms/structs/majority_voting.py
--rw-r--r--   0        0        0      621 2024-05-21 05:06:56.355487 swarms-5.0.7/swarms/structs/message.py
--rw-r--r--   0        0        0     7397 2024-05-20 23:12:19.593913 swarms-5.0.7/swarms/structs/message_pool.py
--rw-r--r--   0        0        0      855 2024-05-20 23:12:19.593973 swarms-5.0.7/swarms/structs/meta_system_prompt.py
--rw-r--r--   0        0        0     8193 2024-05-24 00:28:06.786449 swarms-5.0.7/swarms/structs/multi_agent_collab.py
--rw-r--r--   0        0        0     5623 2024-05-20 23:12:19.594191 swarms-5.0.7/swarms/structs/multi_process_workflow.py
--rw-r--r--   0        0        0     5272 2024-05-20 23:12:19.594250 swarms-5.0.7/swarms/structs/multi_threaded_workflow.py
--rw-r--r--   0        0        0      371 2024-05-20 23:12:19.594301 swarms-5.0.7/swarms/structs/omni_agent_types.py
--rw-r--r--   0        0        0     9900 2024-05-21 03:26:12.085452 swarms-5.0.7/swarms/structs/rearrange.py
--rw-r--r--   0        0        0     3011 2024-05-20 23:12:19.594499 swarms-5.0.7/swarms/structs/recursive_workflow.py
--rw-r--r--   0        0        0     3256 2024-05-20 23:12:19.594554 swarms-5.0.7/swarms/structs/round_robin.py
--rw-r--r--   0        0        0     2956 2024-05-20 23:12:19.594695 swarms-5.0.7/swarms/structs/sequential_workflow.py
--rw-r--r--   0        0        0     2442 2024-05-20 23:12:19.594743 swarms-5.0.7/swarms/structs/sermon_swarm.py
--rw-r--r--   0        0        0     1396 2024-05-23 01:40:40.668233 swarms-5.0.7/swarms/structs/society_of_agents.py
--rw-r--r--   0        0        0    11249 2024-05-24 16:15:05.490950 swarms-5.0.7/swarms/structs/swarm_load_balancer.py
--rw-r--r--   0        0        0    10684 2024-05-20 23:12:19.594876 swarms-5.0.7/swarms/structs/swarm_net.py
--rw-r--r--   0        0        0     6426 2024-05-20 23:12:19.594944 swarms-5.0.7/swarms/structs/swarming_architectures.py
--rw-r--r--   0        0        0     8251 2024-05-20 23:12:19.595011 swarms-5.0.7/swarms/structs/task.py
--rw-r--r--   0        0        0     1989 2024-05-20 23:12:19.595073 swarms-5.0.7/swarms/structs/task_queue_base.py
--rw-r--r--   0        0        0     3646 2024-05-23 01:40:40.674259 swarms-5.0.7/swarms/structs/utils.py
--rw-r--r--   0        0        0     7403 2024-05-20 23:12:19.595210 swarms-5.0.7/swarms/structs/yaml_model.py
--rw-r--r--   0        0        0      891 2024-05-20 23:12:19.595297 swarms-5.0.7/swarms/telemetry/__init__.py
--rw-r--r--   0        0        0      513 2024-05-20 23:12:19.595348 swarms-5.0.7/swarms/telemetry/auto_upgrade_swarms.py
--rw-r--r--   0        0        0      385 2024-05-20 23:12:19.595426 swarms-5.0.7/swarms/telemetry/bootup.py
--rw-r--r--   0        0        0     1073 2024-05-20 23:12:19.595476 swarms-5.0.7/swarms/telemetry/check_update.py
--rw-r--r--   0        0        0      807 2024-05-20 23:12:19.595528 swarms-5.0.7/swarms/telemetry/log_all.py
--rw-r--r--   0        0        0      496 2024-05-20 23:12:19.595576 swarms-5.0.7/swarms/telemetry/sentry_active.py
--rw-r--r--   0        0        0     2675 2024-05-20 23:12:19.595649 swarms-5.0.7/swarms/telemetry/sys_info.py
--rw-r--r--   0        0        0     1879 2024-05-20 23:12:19.595698 swarms-5.0.7/swarms/telemetry/user_utils.py
--rw-r--r--   0        0        0     1401 2024-05-24 17:17:36.428364 swarms-5.0.7/swarms/tools/__init__.py
--rw-r--r--   0        0        0    13734 2024-05-24 16:46:49.761815 swarms-5.0.7/swarms/tools/base_tool.py
--rw-r--r--   0        0        0     6653 2024-05-20 23:12:19.595923 swarms-5.0.7/swarms/tools/code_interpreter.py
--rw-r--r--   0        0        0      773 2024-05-20 23:12:19.596031 swarms-5.0.7/swarms/tools/function_util.py
--rw-r--r--   0        0        0    14241 2024-05-20 23:12:19.596094 swarms-5.0.7/swarms/tools/json_former.py
--rw-r--r--   0        0        0     1316 2024-05-20 23:12:19.596178 swarms-5.0.7/swarms/tools/json_utils.py
--rw-r--r--   0        0        0     2455 2024-05-20 23:12:19.596226 swarms-5.0.7/swarms/tools/logits_processor.py
--rw-r--r--   0        0        0     1461 2024-05-20 23:12:19.596276 swarms-5.0.7/swarms/tools/math_eval.py
--rw-r--r--   0        0        0      978 2024-05-20 23:12:19.596325 swarms-5.0.7/swarms/tools/openai_func_calling_schema_pydantic.py
--rw-r--r--   0        0        0     8790 2024-05-24 17:01:49.491453 swarms-5.0.7/swarms/tools/openai_tool_creator_decorator.py
--rw-r--r--   0        0        0    15564 2024-05-20 23:12:19.596483 swarms-5.0.7/swarms/tools/py_func_to_openai_func_str.py
--rw-r--r--   0        0        0     4275 2024-05-20 23:12:19.596541 swarms-5.0.7/swarms/tools/pydantic_to_json.py
--rw-r--r--   0        0        0      171 2024-05-24 17:15:20.974172 swarms-5.0.7/swarms/tools/tool.py
--rw-r--r--   0        0        0     7152 2024-05-24 17:20:34.711837 swarms-5.0.7/swarms/tools/tool_utils.py
--rw-r--r--   0        0        0     5466 2024-05-20 23:12:19.596758 swarms-5.0.7/swarms/utils/README.md
--rw-r--r--   0        0        0     1956 2024-05-20 23:12:19.596815 swarms-5.0.7/swarms/utils/__init__.py
--rw-r--r--   0        0        0     3507 2024-05-20 23:12:19.596872 swarms-5.0.7/swarms/utils/apa.py
--rw-r--r--   0        0        0     6065 2024-05-20 23:12:19.596962 swarms-5.0.7/swarms/utils/check_function_result.py
--rw-r--r--   0        0        0     1008 2024-05-20 23:12:19.597020 swarms-5.0.7/swarms/utils/class_args_wrapper.py
--rw-r--r--   0        0        0     1234 2024-05-20 23:12:19.597075 swarms-5.0.7/swarms/utils/concurrent_utils.py
--rw-r--r--   0        0        0     1865 2024-05-20 23:12:19.597130 swarms-5.0.7/swarms/utils/data_to_text.py
--rw-r--r--   0        0        0     2451 2024-05-20 23:12:19.597203 swarms-5.0.7/swarms/utils/decorators.py
--rw-r--r--   0        0        0     1311 2024-05-20 23:12:19.597263 swarms-5.0.7/swarms/utils/disable_logging.py
--rw-r--r--   0        0        0      890 2024-05-20 23:12:19.597318 swarms-5.0.7/swarms/utils/download_img.py
--rw-r--r--   0        0        0     1127 2024-05-20 23:12:19.597370 swarms-5.0.7/swarms/utils/execute_futures.py
--rw-r--r--   0        0        0     1113 2024-05-20 23:12:19.597441 swarms-5.0.7/swarms/utils/exponential_backoff.py
--rw-r--r--   0        0        0      854 2024-05-20 23:12:19.597496 swarms-5.0.7/swarms/utils/fetch_init_params.py
--rw-r--r--   0        0        0      500 2024-05-20 23:12:19.597550 swarms-5.0.7/swarms/utils/file_extension_seach.py
--rw-r--r--   0        0        0     3266 2024-05-20 23:12:19.597606 swarms-5.0.7/swarms/utils/file_processing.py
--rw-r--r--   0        0        0      630 2024-05-20 23:12:19.597693 swarms-5.0.7/swarms/utils/find_img_path.py
--rw-r--r--   0        0        0     4184 2024-05-20 23:12:19.597767 swarms-5.0.7/swarms/utils/get_logger.py
--rw-r--r--   0        0        0     4232 2024-05-20 23:12:19.597842 swarms-5.0.7/swarms/utils/get_total_gpus.py
--rw-r--r--   0        0        0     2848 2024-05-20 23:12:19.597905 swarms-5.0.7/swarms/utils/json_output_parser.py
--rw-r--r--   0        0        0     1831 2024-05-20 23:12:19.597994 swarms-5.0.7/swarms/utils/jsonl_utils.py
--rw-r--r--   0        0        0      932 2024-05-20 23:12:19.598063 swarms-5.0.7/swarms/utils/llm_metrics_decorator.py
--rw-r--r--   0        0        0     2209 2024-05-20 23:12:19.598133 swarms-5.0.7/swarms/utils/logger.py
--rw-r--r--   0        0        0    16186 2024-05-20 23:12:19.598202 swarms-5.0.7/swarms/utils/loggers.py
--rw-r--r--   0        0        0      453 2024-05-20 23:12:19.598285 swarms-5.0.7/swarms/utils/loguru_logger.py
--rw-r--r--   0        0        0      711 2024-05-20 23:12:19.598349 swarms-5.0.7/swarms/utils/markdown_message.py
--rw-r--r--   0        0        0      600 2024-05-20 23:12:19.598408 swarms-5.0.7/swarms/utils/parse_code.py
--rw-r--r--   0        0        0     1177 2024-05-20 23:12:19.598470 swarms-5.0.7/swarms/utils/pdf_to_text.py
--rw-r--r--   0        0        0     1353 2024-05-20 23:12:19.598561 swarms-5.0.7/swarms/utils/remove_json_whitespace.py
--rw-r--r--   0        0        0     1278 2024-05-20 23:12:19.598619 swarms-5.0.7/swarms/utils/save_logs.py
--rw-r--r--   0        0        0     4774 2024-05-20 23:12:19.598696 swarms-5.0.7/swarms/utils/serializable.py
--rw-r--r--   0        0        0     1315 2024-05-20 23:12:19.598755 swarms-5.0.7/swarms/utils/try_except_wrapper.py
--rw-r--r--   0        0        0     2668 2024-05-20 23:12:19.598843 swarms-5.0.7/swarms/utils/yaml_output_parser.py
--rw-r--r--   0        0        0    35219 1970-01-01 00:00:00.000000 swarms-5.0.7/PKG-INFO
+-rw-r--r--   0        0        0    15674 2024-05-20 23:12:19.525914 swarms-5.0.8/LICENSE
+-rw-r--r--   0        0        0    33743 2024-05-25 00:26:35.052802 swarms-5.0.8/README.md
+-rw-r--r--   0        0        0     1790 2024-05-27 04:35:03.351567 swarms-5.0.8/pyproject.toml
+-rw-r--r--   0        0        0      590 2024-05-20 23:12:19.584595 swarms-5.0.8/swarms/__init__.py
+-rw-r--r--   0        0        0      864 2024-05-20 23:12:19.584679 swarms-5.0.8/swarms/agents/__init__.py
+-rw-r--r--   0        0        0      881 2024-05-20 23:12:19.584738 swarms-5.0.8/swarms/agents/agent_wrapper.py
+-rw-r--r--   0        0        0     3342 2024-05-20 23:12:19.584796 swarms-5.0.8/swarms/agents/base.py
+-rw-r--r--   0        0        0     4201 2024-05-20 23:12:19.584880 swarms-5.0.8/swarms/agents/developer_agents.py
+-rw-r--r--   0        0        0     2950 2024-05-20 23:12:19.584947 swarms-5.0.8/swarms/agents/omni_modal_agent.py
+-rw-r--r--   0        0        0     3491 2024-05-20 23:12:19.585001 swarms-5.0.8/swarms/agents/simple_agent.py
+-rw-r--r--   0        0        0      484 2024-05-20 23:12:19.585048 swarms-5.0.8/swarms/agents/stopping_conditions.py
+-rw-r--r--   0        0        0     4940 2024-05-20 23:12:19.585129 swarms-5.0.8/swarms/agents/tool_agent.py
+-rw-r--r--   0        0        0     5504 2024-05-20 23:12:19.585192 swarms-5.0.8/swarms/agents/worker_agent.py
+-rw-r--r--   0        0        0      167 2024-05-20 23:12:19.585283 swarms-5.0.8/swarms/artifacts/__init__.py
+-rw-r--r--   0        0        0     1675 2024-05-20 23:12:19.585343 swarms-5.0.8/swarms/artifacts/base_artifact.py
+-rw-r--r--   0        0        0     2299 2024-05-20 23:12:19.585425 swarms-5.0.8/swarms/artifacts/text_artifact.py
+-rw-r--r--   0        0        0      613 2024-05-20 23:12:19.585515 swarms-5.0.8/swarms/memory/__init__.py
+-rw-r--r--   0        0        0      433 2024-05-20 23:12:19.585565 swarms-5.0.8/swarms/memory/action_subtask.py
+-rw-r--r--   0        0        0     3475 2024-05-20 23:12:19.585621 swarms-5.0.8/swarms/memory/base_db.py
+-rw-r--r--   0        0        0     2823 2024-05-20 23:12:19.585702 swarms-5.0.8/swarms/memory/base_vectordb.py
+-rw-r--r--   0        0        0     2895 2024-05-20 23:12:19.585767 swarms-5.0.8/swarms/memory/dict_internal_memory.py
+-rw-r--r--   0        0        0     3306 2024-05-20 23:12:19.585826 swarms-5.0.8/swarms/memory/dict_shared_memory.py
+-rw-r--r--   0        0        0     5499 2024-05-20 23:12:19.585895 swarms-5.0.8/swarms/memory/short_term_memory.py
+-rw-r--r--   0        0        0     3371 2024-05-20 23:12:19.585978 swarms-5.0.8/swarms/memory/visual_memory.py
+-rw-r--r--   0        0        0     2392 2024-05-21 05:06:54.045652 swarms-5.0.8/swarms/models/__init__.py
+-rw-r--r--   0        0        0     2052 2024-05-21 00:48:59.027928 swarms-5.0.8/swarms/models/base_embedding_model.py
+-rw-r--r--   0        0        0    13168 2024-05-20 23:12:19.586207 swarms-5.0.8/swarms/models/base_llm.py
+-rw-r--r--   0        0        0    12604 2024-05-20 23:12:19.586302 swarms-5.0.8/swarms/models/base_multimodal_model.py
+-rw-r--r--   0        0        0     2475 2024-05-20 23:12:19.586361 swarms-5.0.8/swarms/models/base_tts.py
+-rw-r--r--   0        0        0     3163 2024-05-20 23:12:19.586416 swarms-5.0.8/swarms/models/base_ttv.py
+-rw-r--r--   0        0        0    16743 2024-05-20 23:12:19.586490 swarms-5.0.8/swarms/models/cog_vlm.py
+-rw-r--r--   0        0        0    10760 2024-05-20 23:12:19.586608 swarms-5.0.8/swarms/models/dalle3.py
+-rw-r--r--   0        0        0     6449 2024-05-20 23:12:19.586690 swarms-5.0.8/swarms/models/distilled_whisperx.py
+-rw-r--r--   0        0        0      682 2024-05-20 23:12:19.586747 swarms-5.0.8/swarms/models/embeddings_base.py
+-rw-r--r--   0        0        0     3022 2024-05-20 23:12:19.586804 swarms-5.0.8/swarms/models/fuyu.py
+-rw-r--r--   0        0        0     7762 2024-05-20 23:12:19.586891 swarms-5.0.8/swarms/models/gemini.py
+-rw-r--r--   0        0        0    14236 2024-05-20 23:12:19.586973 swarms-5.0.8/swarms/models/gpt4_vision_api.py
+-rw-r--r--   0        0        0    12996 2024-05-20 23:12:19.587047 swarms-5.0.8/swarms/models/huggingface.py
+-rw-r--r--   0        0        0     1826 2024-05-20 23:12:19.587108 swarms-5.0.8/swarms/models/huggingface_pipeline.py
+-rw-r--r--   0        0        0     5601 2024-05-20 23:12:19.587202 swarms-5.0.8/swarms/models/idefics.py
+-rw-r--r--   0        0        0    10672 2024-05-20 23:12:19.587276 swarms-5.0.8/swarms/models/kosmos_two.py
+-rw-r--r--   0        0        0     1448 2024-05-20 23:12:19.587347 swarms-5.0.8/swarms/models/layoutlm_document_qa.py
+-rw-r--r--   0        0        0     2599 2024-05-21 05:06:21.835242 swarms-5.0.8/swarms/models/llama3_hosted.py
+-rw-r--r--   0        0        0     6581 2024-05-20 23:12:19.587506 swarms-5.0.8/swarms/models/llama_function_caller.py
+-rw-r--r--   0        0        0     2762 2024-05-20 23:12:19.587573 swarms-5.0.8/swarms/models/llava.py
+-rw-r--r--   0        0        0     2056 2024-05-20 23:12:19.587792 swarms-5.0.8/swarms/models/moondream_mm.py
+-rw-r--r--   0        0        0     2881 2024-05-20 23:12:19.587858 swarms-5.0.8/swarms/models/nougat.py
+-rw-r--r--   0        0        0     2366 2024-05-20 23:12:19.587917 swarms-5.0.8/swarms/models/open_dalle.py
+-rw-r--r--   0        0        0     2464 2024-05-20 23:12:19.587972 swarms-5.0.8/swarms/models/open_router.py
+-rw-r--r--   0        0        0      106 2024-05-20 23:12:19.588047 swarms-5.0.8/swarms/models/openai_embeddings.py
+-rw-r--r--   0        0        0     3167 2024-05-20 23:12:19.588099 swarms-5.0.8/swarms/models/openai_tts.py
+-rw-r--r--   0        0        0       93 2024-05-20 23:12:19.588149 swarms-5.0.8/swarms/models/palm.py
+-rw-r--r--   0        0        0     2160 2024-05-20 23:12:19.588204 swarms-5.0.8/swarms/models/popular_llms.py
+-rw-r--r--   0        0        0     4813 2024-05-20 23:12:19.588296 swarms-5.0.8/swarms/models/qwen.py
+-rw-r--r--   0        0        0     3561 2024-05-20 23:12:19.588355 swarms-5.0.8/swarms/models/sam.py
+-rw-r--r--   0        0        0    12675 2024-05-20 23:12:19.588421 swarms-5.0.8/swarms/models/sampling_params.py
+-rw-r--r--   0        0        0     8244 2024-05-20 23:12:19.588474 swarms-5.0.8/swarms/models/ssd_1b.py
+-rw-r--r--   0        0        0     3948 2024-05-20 23:12:19.588553 swarms-5.0.8/swarms/models/together.py
+-rw-r--r--   0        0        0      592 2024-05-20 23:12:19.588607 swarms-5.0.8/swarms/models/types.py
+-rw-r--r--   0        0        0     1731 2024-05-20 23:12:19.588664 swarms-5.0.8/swarms/models/vilt.py
+-rw-r--r--   0        0        0     2846 2024-05-20 23:12:19.588711 swarms-5.0.8/swarms/models/vip_llava.py
+-rw-r--r--   0        0        0     3666 2024-05-20 23:12:19.588784 swarms-5.0.8/swarms/models/zeroscope.py
+-rw-r--r--   0        0        0        0 2024-05-20 23:12:19.588836 swarms-5.0.8/swarms/prebuilt_swarms/__init__.py
+-rw-r--r--   0        0        0      692 2024-05-20 23:12:19.588923 swarms-5.0.8/swarms/prompts/__init__.py
+-rw-r--r--   0        0        0    11320 2024-05-20 23:12:19.588988 swarms-5.0.8/swarms/prompts/accountant_swarm_prompts.py
+-rw-r--r--   0        0        0     9156 2024-05-20 23:12:19.589069 swarms-5.0.8/swarms/prompts/aga.py
+-rw-r--r--   0        0        0     1451 2024-05-20 23:12:19.589128 swarms-5.0.8/swarms/prompts/agent_output_parser.py
+-rw-r--r--   0        0        0     2705 2024-05-20 23:12:19.589180 swarms-5.0.8/swarms/prompts/agent_prompt.py
+-rw-r--r--   0        0        0     6886 2024-05-20 23:12:19.589236 swarms-5.0.8/swarms/prompts/agent_prompts.py
+-rw-r--r--   0        0        0     7113 2024-05-20 23:12:19.589316 swarms-5.0.8/swarms/prompts/agent_system_prompts.py
+-rw-r--r--   0        0        0     5233 2024-05-20 23:12:19.589377 swarms-5.0.8/swarms/prompts/ai_research_team.py
+-rw-r--r--   0        0        0     1148 2024-05-20 23:12:19.589426 swarms-5.0.8/swarms/prompts/aot_prompt.py
+-rw-r--r--   0        0        0    13981 2024-05-20 23:12:19.589498 swarms-5.0.8/swarms/prompts/autobloggen.py
+-rw-r--r--   0        0        0     5605 2024-05-20 23:12:19.589584 swarms-5.0.8/swarms/prompts/autoswarm.py
+-rw-r--r--   0        0        0     7542 2024-05-20 23:12:19.589647 swarms-5.0.8/swarms/prompts/base.py
+-rw-r--r--   0        0        0     3801 2024-05-20 23:12:19.589703 swarms-5.0.8/swarms/prompts/chat_prompt.py
+-rw-r--r--   0        0        0     2235 2024-05-20 23:12:19.589756 swarms-5.0.8/swarms/prompts/code_interpreter.py
+-rw-r--r--   0        0        0     4106 2024-05-20 23:12:19.589834 swarms-5.0.8/swarms/prompts/code_spawner.py
+-rw-r--r--   0        0        0     1566 2024-05-20 23:12:19.589885 swarms-5.0.8/swarms/prompts/debate.py
+-rw-r--r--   0        0        0     7157 2024-05-23 01:40:32.871666 swarms-5.0.8/swarms/prompts/documentation.py
+-rw-r--r--   0        0        0     1767 2024-05-20 23:12:19.590009 swarms-5.0.8/swarms/prompts/education.py
+-rw-r--r--   0        0        0     4180 2024-05-20 23:12:19.590089 swarms-5.0.8/swarms/prompts/finance_agent_prompt.py
+-rw-r--r--   0        0        0     4117 2024-05-20 23:12:19.590152 swarms-5.0.8/swarms/prompts/growth_agent_prompt.py
+-rw-r--r--   0        0        0      880 2024-05-20 23:12:19.590207 swarms-5.0.8/swarms/prompts/idea2img.py
+-rw-r--r--   0        0        0     3346 2024-05-20 23:12:19.590267 swarms-5.0.8/swarms/prompts/legal_agent_prompt.py
+-rw-r--r--   0        0        0     4785 2024-05-20 23:12:19.590358 swarms-5.0.8/swarms/prompts/logistics.py
+-rw-r--r--   0        0        0     3374 2024-05-20 23:12:19.590418 swarms-5.0.8/swarms/prompts/meta_system_prompt.py
+-rw-r--r--   0        0        0    10662 2024-05-20 23:12:19.590489 swarms-5.0.8/swarms/prompts/multi_modal_autonomous_instruction_prompt.py
+-rw-r--r--   0        0        0     3511 2024-05-20 23:12:19.590550 swarms-5.0.8/swarms/prompts/multi_modal_prompts.py
+-rw-r--r--   0        0        0     3225 2024-05-20 23:12:19.590626 swarms-5.0.8/swarms/prompts/multi_modal_visual_prompts.py
+-rw-r--r--   0        0        0     3454 2024-05-20 23:12:19.590685 swarms-5.0.8/swarms/prompts/operations_agent_prompt.py
+-rw-r--r--   0        0        0     2149 2024-05-20 23:12:19.590738 swarms-5.0.8/swarms/prompts/personal_stylist.py
+-rw-r--r--   0        0        0     8333 2024-05-20 23:12:19.590803 swarms-5.0.8/swarms/prompts/product_agent_prompt.py
+-rw-r--r--   0        0        0    10144 2024-05-20 23:12:19.590895 swarms-5.0.8/swarms/prompts/programming.py
+-rw-r--r--   0        0        0     2128 2024-05-20 23:12:19.590958 swarms-5.0.8/swarms/prompts/project_manager.py
+-rw-r--r--   0        0        0    13215 2024-05-20 23:12:19.591020 swarms-5.0.8/swarms/prompts/python.py
+-rw-r--r--   0        0        0     2960 2024-05-20 23:12:19.591076 swarms-5.0.8/swarms/prompts/react.py
+-rw-r--r--   0        0        0        0 2024-05-20 23:12:19.591117 swarms-5.0.8/swarms/prompts/refiner_agent_prompt.py
+-rw-r--r--   0        0        0     5126 2024-05-20 23:12:19.591208 swarms-5.0.8/swarms/prompts/sales.py
+-rw-r--r--   0        0        0     5013 2024-05-20 23:12:19.591263 swarms-5.0.8/swarms/prompts/sales_prompts.py
+-rw-r--r--   0        0        0     2679 2024-05-20 23:12:19.591326 swarms-5.0.8/swarms/prompts/security_team.py
+-rw-r--r--   0        0        0     3252 2024-05-20 23:12:19.591419 swarms-5.0.8/swarms/prompts/self_operating_prompt.py
+-rw-r--r--   0        0        0     4147 2024-05-20 23:12:19.591487 swarms-5.0.8/swarms/prompts/sop_generator_agent_prompt.py
+-rw-r--r--   0        0        0     4640 2024-05-20 23:12:19.591551 swarms-5.0.8/swarms/prompts/summaries_prompts.py
+-rw-r--r--   0        0        0     3984 2024-05-20 23:12:19.591612 swarms-5.0.8/swarms/prompts/support_agent_prompt.py
+-rw-r--r--   0        0        0     4280 2024-05-20 23:12:19.591714 swarms-5.0.8/swarms/prompts/swarm_manager_agent.py
+-rw-r--r--   0        0        0      728 2024-05-20 23:12:19.591774 swarms-5.0.8/swarms/prompts/task_assignment_prompt.py
+-rw-r--r--   0        0        0     4271 2024-05-20 23:12:19.591847 swarms-5.0.8/swarms/prompts/tests.py
+-rw-r--r--   0        0        0     6576 2024-05-24 17:56:40.206770 swarms-5.0.8/swarms/prompts/tools.py
+-rw-r--r--   0        0        0     2398 2024-05-20 23:12:19.592013 swarms-5.0.8/swarms/prompts/urban_planning.py
+-rw-r--r--   0        0        0     3675 2024-05-20 23:12:19.592103 swarms-5.0.8/swarms/prompts/visual_cot.py
+-rw-r--r--   0        0        0     5554 2024-05-20 23:12:19.592180 swarms-5.0.8/swarms/prompts/worker_prompt.py
+-rw-r--r--   0        0        0     2349 2024-05-20 23:12:19.592230 swarms-5.0.8/swarms/prompts/xray_swarm_prompt.py
+-rw-r--r--   0        0        0        0 2024-05-21 03:27:54.652576 swarms-5.0.8/swarms/schemas/__init__.py
+-rw-r--r--   0        0        0     3168 2024-05-24 00:43:53.750806 swarms-5.0.8/swarms/schemas/hass_agent_schema.py
+-rw-r--r--   0        0        0      182 2024-05-21 05:06:25.218133 swarms-5.0.8/swarms/schemas/plan.py
+-rw-r--r--   0        0        0     6764 2024-05-20 23:12:19.594641 swarms-5.0.8/swarms/schemas/schemas.py
+-rw-r--r--   0        0        0      709 2024-05-20 23:12:19.594792 swarms-5.0.8/swarms/schemas/step.py
+-rw-r--r--   0        0        0     4084 2024-05-24 14:40:28.251160 swarms-5.0.8/swarms/structs/__init__.py
+-rw-r--r--   0        0        0    61682 2024-05-25 00:11:23.269052 swarms-5.0.8/swarms/structs/agent.py
+-rw-r--r--   0        0        0      574 2024-05-20 23:12:19.592548 swarms-5.0.8/swarms/structs/agent_job.py
+-rw-r--r--   0        0        0     2937 2024-05-20 23:12:19.592611 swarms-5.0.8/swarms/structs/agent_process.py
+-rw-r--r--   0        0        0     3777 2024-05-20 23:12:19.592668 swarms-5.0.8/swarms/structs/async_workflow.py
+-rw-r--r--   0        0        0     6624 2024-05-20 23:12:19.592755 swarms-5.0.8/swarms/structs/auto_swarm.py
+-rw-r--r--   0        0        0    12437 2024-05-20 23:12:19.592817 swarms-5.0.8/swarms/structs/base_structure.py
+-rw-r--r--   0        0        0    19446 2024-05-20 23:12:19.592905 swarms-5.0.8/swarms/structs/base_swarm.py
+-rw-r--r--   0        0        0    12161 2024-05-20 23:12:19.593000 swarms-5.0.8/swarms/structs/base_workflow.py
+-rw-r--r--   0        0        0     5265 2024-05-21 00:48:59.119899 swarms-5.0.8/swarms/structs/company.py
+-rw-r--r--   0        0        0     6181 2024-05-25 00:30:33.743749 swarms-5.0.8/swarms/structs/concurrent_workflow.py
+-rw-r--r--   0        0        0    14685 2024-05-20 23:12:19.593392 swarms-5.0.8/swarms/structs/conversation.py
+-rw-r--r--   0        0        0    12608 2024-05-20 23:12:19.593456 swarms-5.0.8/swarms/structs/debate.py
+-rw-r--r--   0        0        0     4834 2024-05-20 23:12:19.593607 swarms-5.0.8/swarms/structs/groupchat.py
+-rw-r--r--   0        0        0     8721 2024-05-27 04:34:55.663377 swarms-5.0.8/swarms/structs/hiearchical_swarm.py
+-rw-r--r--   0        0        0     7012 2024-05-20 23:12:19.593787 swarms-5.0.8/swarms/structs/majority_voting.py
+-rw-r--r--   0        0        0      621 2024-05-21 05:06:56.355487 swarms-5.0.8/swarms/structs/message.py
+-rw-r--r--   0        0        0     7397 2024-05-20 23:12:19.593913 swarms-5.0.8/swarms/structs/message_pool.py
+-rw-r--r--   0        0        0      855 2024-05-20 23:12:19.593973 swarms-5.0.8/swarms/structs/meta_system_prompt.py
+-rw-r--r--   0        0        0     8193 2024-05-24 00:28:06.786449 swarms-5.0.8/swarms/structs/multi_agent_collab.py
+-rw-r--r--   0        0        0     5623 2024-05-20 23:12:19.594191 swarms-5.0.8/swarms/structs/multi_process_workflow.py
+-rw-r--r--   0        0        0     5272 2024-05-20 23:12:19.594250 swarms-5.0.8/swarms/structs/multi_threaded_workflow.py
+-rw-r--r--   0        0        0      371 2024-05-20 23:12:19.594301 swarms-5.0.8/swarms/structs/omni_agent_types.py
+-rw-r--r--   0        0        0     9900 2024-05-21 03:26:12.085452 swarms-5.0.8/swarms/structs/rearrange.py
+-rw-r--r--   0        0        0     3011 2024-05-20 23:12:19.594499 swarms-5.0.8/swarms/structs/recursive_workflow.py
+-rw-r--r--   0        0        0     3256 2024-05-20 23:12:19.594554 swarms-5.0.8/swarms/structs/round_robin.py
+-rw-r--r--   0        0        0     2956 2024-05-20 23:12:19.594695 swarms-5.0.8/swarms/structs/sequential_workflow.py
+-rw-r--r--   0        0        0     2442 2024-05-20 23:12:19.594743 swarms-5.0.8/swarms/structs/sermon_swarm.py
+-rw-r--r--   0        0        0     1396 2024-05-23 01:40:40.668233 swarms-5.0.8/swarms/structs/society_of_agents.py
+-rw-r--r--   0        0        0    11249 2024-05-24 16:15:05.490950 swarms-5.0.8/swarms/structs/swarm_load_balancer.py
+-rw-r--r--   0        0        0    10684 2024-05-20 23:12:19.594876 swarms-5.0.8/swarms/structs/swarm_net.py
+-rw-r--r--   0        0        0     6426 2024-05-20 23:12:19.594944 swarms-5.0.8/swarms/structs/swarming_architectures.py
+-rw-r--r--   0        0        0     8251 2024-05-20 23:12:19.595011 swarms-5.0.8/swarms/structs/task.py
+-rw-r--r--   0        0        0     1989 2024-05-20 23:12:19.595073 swarms-5.0.8/swarms/structs/task_queue_base.py
+-rw-r--r--   0        0        0     3829 2024-05-24 20:02:02.841193 swarms-5.0.8/swarms/structs/tree_of_thoughts.py
+-rw-r--r--   0        0        0     3646 2024-05-23 01:40:40.674259 swarms-5.0.8/swarms/structs/utils.py
+-rw-r--r--   0        0        0     7403 2024-05-20 23:12:19.595210 swarms-5.0.8/swarms/structs/yaml_model.py
+-rw-r--r--   0        0        0      891 2024-05-20 23:12:19.595297 swarms-5.0.8/swarms/telemetry/__init__.py
+-rw-r--r--   0        0        0      513 2024-05-20 23:12:19.595348 swarms-5.0.8/swarms/telemetry/auto_upgrade_swarms.py
+-rw-r--r--   0        0        0      385 2024-05-20 23:12:19.595426 swarms-5.0.8/swarms/telemetry/bootup.py
+-rw-r--r--   0        0        0     1073 2024-05-20 23:12:19.595476 swarms-5.0.8/swarms/telemetry/check_update.py
+-rw-r--r--   0        0        0      807 2024-05-20 23:12:19.595528 swarms-5.0.8/swarms/telemetry/log_all.py
+-rw-r--r--   0        0        0      496 2024-05-20 23:12:19.595576 swarms-5.0.8/swarms/telemetry/sentry_active.py
+-rw-r--r--   0        0        0     2675 2024-05-20 23:12:19.595649 swarms-5.0.8/swarms/telemetry/sys_info.py
+-rw-r--r--   0        0        0     1879 2024-05-20 23:12:19.595698 swarms-5.0.8/swarms/telemetry/user_utils.py
+-rw-r--r--   0        0        0     1457 2024-05-25 00:11:23.032620 swarms-5.0.8/swarms/tools/__init__.py
+-rw-r--r--   0        0        0    13754 2024-05-25 00:08:34.660101 swarms-5.0.8/swarms/tools/base_tool.py
+-rw-r--r--   0        0        0     6258 2024-05-25 00:03:55.372791 swarms-5.0.8/swarms/tools/func_calling_executor.py
+-rw-r--r--   0        0        0     1115 2024-05-25 00:08:48.921190 swarms-5.0.8/swarms/tools/func_to_str.py
+-rw-r--r--   0        0        0      773 2024-05-25 00:03:54.059716 swarms-5.0.8/swarms/tools/function_util.py
+-rw-r--r--   0        0        0    14241 2024-05-20 23:12:19.596094 swarms-5.0.8/swarms/tools/json_former.py
+-rw-r--r--   0        0        0     1316 2024-05-20 23:12:19.596178 swarms-5.0.8/swarms/tools/json_utils.py
+-rw-r--r--   0        0        0     2455 2024-05-20 23:12:19.596226 swarms-5.0.8/swarms/tools/logits_processor.py
+-rw-r--r--   0        0        0      978 2024-05-20 23:12:19.596325 swarms-5.0.8/swarms/tools/openai_func_calling_schema_pydantic.py
+-rw-r--r--   0        0        0     2578 2024-05-25 00:03:55.373001 swarms-5.0.8/swarms/tools/openai_tool_creator_decorator.py
+-rw-r--r--   0        0        0      205 2024-05-25 00:23:02.813589 swarms-5.0.8/swarms/tools/prebuilt/__init__.py
+-rw-r--r--   0        0        0     6653 2024-05-20 23:12:19.595923 swarms-5.0.8/swarms/tools/prebuilt/code_interpreter.py
+-rw-r--r--   0        0        0     1461 2024-05-20 23:12:19.596276 swarms-5.0.8/swarms/tools/prebuilt/math_eval.py
+-rw-r--r--   0        0        0    15564 2024-05-20 23:12:19.596483 swarms-5.0.8/swarms/tools/py_func_to_openai_func_str.py
+-rw-r--r--   0        0        0     3183 2024-05-25 00:08:48.931693 swarms-5.0.8/swarms/tools/pydantic_to_json.py
+-rw-r--r--   0        0        0     7179 2024-05-24 17:56:40.227742 swarms-5.0.8/swarms/tools/tool_utils.py
+-rw-r--r--   0        0        0     5466 2024-05-20 23:12:19.596758 swarms-5.0.8/swarms/utils/README.md
+-rw-r--r--   0        0        0     1983 2024-05-25 00:11:23.037330 swarms-5.0.8/swarms/utils/__init__.py
+-rw-r--r--   0        0        0     3507 2024-05-20 23:12:19.596872 swarms-5.0.8/swarms/utils/apa.py
+-rw-r--r--   0        0        0     6065 2024-05-20 23:12:19.596962 swarms-5.0.8/swarms/utils/check_function_result.py
+-rw-r--r--   0        0        0     1008 2024-05-20 23:12:19.597020 swarms-5.0.8/swarms/utils/class_args_wrapper.py
+-rw-r--r--   0        0        0     1234 2024-05-20 23:12:19.597075 swarms-5.0.8/swarms/utils/concurrent_utils.py
+-rw-r--r--   0        0        0     1865 2024-05-20 23:12:19.597130 swarms-5.0.8/swarms/utils/data_to_text.py
+-rw-r--r--   0        0        0     2451 2024-05-20 23:12:19.597203 swarms-5.0.8/swarms/utils/decorators.py
+-rw-r--r--   0        0        0     1311 2024-05-20 23:12:19.597263 swarms-5.0.8/swarms/utils/disable_logging.py
+-rw-r--r--   0        0        0      890 2024-05-20 23:12:19.597318 swarms-5.0.8/swarms/utils/download_img.py
+-rw-r--r--   0        0        0     1127 2024-05-20 23:12:19.597370 swarms-5.0.8/swarms/utils/execute_futures.py
+-rw-r--r--   0        0        0     1113 2024-05-20 23:12:19.597441 swarms-5.0.8/swarms/utils/exponential_backoff.py
+-rw-r--r--   0        0        0      854 2024-05-20 23:12:19.597496 swarms-5.0.8/swarms/utils/fetch_init_params.py
+-rw-r--r--   0        0        0      500 2024-05-20 23:12:19.597550 swarms-5.0.8/swarms/utils/file_extension_seach.py
+-rw-r--r--   0        0        0     3266 2024-05-20 23:12:19.597606 swarms-5.0.8/swarms/utils/file_processing.py
+-rw-r--r--   0        0        0      630 2024-05-20 23:12:19.597693 swarms-5.0.8/swarms/utils/find_img_path.py
+-rw-r--r--   0        0        0     4184 2024-05-20 23:12:19.597767 swarms-5.0.8/swarms/utils/get_logger.py
+-rw-r--r--   0        0        0     4232 2024-05-20 23:12:19.597842 swarms-5.0.8/swarms/utils/get_total_gpus.py
+-rw-r--r--   0        0        0     2848 2024-05-20 23:12:19.597905 swarms-5.0.8/swarms/utils/json_output_parser.py
+-rw-r--r--   0        0        0     1831 2024-05-20 23:12:19.597994 swarms-5.0.8/swarms/utils/jsonl_utils.py
+-rw-r--r--   0        0        0      932 2024-05-20 23:12:19.598063 swarms-5.0.8/swarms/utils/llm_metrics_decorator.py
+-rw-r--r--   0        0        0     2209 2024-05-20 23:12:19.598133 swarms-5.0.8/swarms/utils/logger.py
+-rw-r--r--   0        0        0    16186 2024-05-20 23:12:19.598202 swarms-5.0.8/swarms/utils/loggers.py
+-rw-r--r--   0        0        0      453 2024-05-20 23:12:19.598285 swarms-5.0.8/swarms/utils/loguru_logger.py
+-rw-r--r--   0        0        0      711 2024-05-20 23:12:19.598349 swarms-5.0.8/swarms/utils/markdown_message.py
+-rw-r--r--   0        0        0     2173 2024-05-26 03:54:20.425670 swarms-5.0.8/swarms/utils/optimized_loop.py
+-rw-r--r--   0        0        0      600 2024-05-20 23:12:19.598408 swarms-5.0.8/swarms/utils/parse_code.py
+-rw-r--r--   0        0        0     1177 2024-05-20 23:12:19.598470 swarms-5.0.8/swarms/utils/pdf_to_text.py
+-rw-r--r--   0        0        0     1353 2024-05-20 23:12:19.598561 swarms-5.0.8/swarms/utils/remove_json_whitespace.py
+-rw-r--r--   0        0        0     1278 2024-05-20 23:12:19.598619 swarms-5.0.8/swarms/utils/save_logs.py
+-rw-r--r--   0        0        0     4774 2024-05-20 23:12:19.598696 swarms-5.0.8/swarms/utils/serializable.py
+-rw-r--r--   0        0        0     1315 2024-05-20 23:12:19.598755 swarms-5.0.8/swarms/utils/try_except_wrapper.py
+-rw-r--r--   0        0        0     2668 2024-05-20 23:12:19.598843 swarms-5.0.8/swarms/utils/yaml_output_parser.py
+-rw-r--r--   0        0        0    35249 1970-01-01 00:00:00.000000 swarms-5.0.8/PKG-INFO
```

### Comparing `swarms-5.0.7/LICENSE` & `swarms-5.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/README.md` & `swarms-5.0.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -105,26 +105,25 @@
 ```
 
 
 # `Agent` with Long Term Memory ++ Tools!
 An LLM equipped with long term memory and tools, a full stack agent capable of automating all and any digital tasks given a good prompt.
 
 ```python
-from swarms import Agent, ChromaDB, OpenAIChat, tool
+from swarms import Agent, ChromaDB, OpenAIChat
 
 # Making an instance of the ChromaDB class
 memory = ChromaDB(
     metric="cosine",
     n_results=3,
     output_dir="results",
     docs_folder="docs",
 )
 
 # Initialize a tool
-@tool
 def search_api(query: str):
     # Add your logic here
     return query
 
 # Initializing the agent with the Gemini instance and other parameters
 agent = Agent(
     agent_name="Covid-19-Chat",
@@ -181,24 +180,23 @@
 ```
 
 ## Devin
 Implementation of Devil in less than 90 lines of code with several tools:
 terminal, browser, and edit files!
 
 ```python
-from swarms import Agent, Anthropic, tool
+from swarms import Agent, Anthropic
 import subprocess
 
 # Model
 llm = Anthropic(
     temperature=0.1,
 )
 
 # Tools
-@tool
 def terminal(
     code: str,
 ):
     """
     Run code in the terminal.
 
     Args:
@@ -208,16 +206,14 @@
         str: The output of the code.
     """
     out = subprocess.run(
         code, shell=True, capture_output=True, text=True
     ).stdout
     return str(out)
 
-
-@tool
 def browser(query: str):
     """
     Search the query in the browser with the `browser` tool.
 
     Args:
         query (str): The query to search in the browser.
 
@@ -226,15 +222,14 @@
     """
     import webbrowser
 
     url = f"https://www.google.com/search?q={query}"
     webbrowser.open(url)
     return f"Searching for {query} in the browser."
 
-@tool
 def create_file(file_path: str, content: str):
     """
     Create a file using the file editor tool.
 
     Args:
         file_path (str): The path to the file.
         content (str): The content to write to the file.
@@ -242,15 +237,14 @@
     Returns:
         str: The result of the file creation operation.
     """
     with open(file_path, "w") as file:
         file.write(content)
     return f"File {file_path} created successfully."
 
-@tool
 def file_editor(file_path: str, mode: str, content: str):
     """
     Edit a file using the file editor tool.
 
     Args:
         file_path (str): The path to the file.
         mode (str): The mode to open the file in.
@@ -1105,14 +1099,22 @@
 
 ```
 
 ## `HierarhicalSwarm`
 Coming soon...
 
 
+## `AgentLoadBalancer`
+Coming soon...
+
+
+## `GraphSwarm`
+Coming soon...
+
+
 ---
 
 ## Documentation
 Documentation is located here at: [swarms.apac.ai](https://swarms.apac.ai)
 
 ----
```

### Comparing `swarms-5.0.7/pyproject.toml` & `swarms-5.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "swarms"
-version = "5.0.7"
+version = "5.0.8"
 description = "Swarms - Pytorch"
 license = "MIT"
 authors = ["Kye Gomez <kye@apac.ai>"]
 homepage = "https://github.com/kyegomez/swarms"
 documentation = "https://swarms.world"
 readme = "README.md"
 repository = "https://github.com/kyegomez/swarms"
```

### Comparing `swarms-5.0.7/swarms/__init__.py` & `swarms-5.0.8/swarms/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/agents/__init__.py` & `swarms-5.0.8/swarms/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/agents/agent_wrapper.py` & `swarms-5.0.8/swarms/agents/agent_wrapper.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/agents/base.py` & `swarms-5.0.8/swarms/agents/base.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/agents/developer_agents.py` & `swarms-5.0.8/swarms/agents/developer_agents.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/agents/omni_modal_agent.py` & `swarms-5.0.8/swarms/agents/omni_modal_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/agents/simple_agent.py` & `swarms-5.0.8/swarms/agents/simple_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/agents/tool_agent.py` & `swarms-5.0.8/swarms/agents/tool_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/agents/worker_agent.py` & `swarms-5.0.8/swarms/agents/worker_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/artifacts/base_artifact.py` & `swarms-5.0.8/swarms/artifacts/base_artifact.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/artifacts/text_artifact.py` & `swarms-5.0.8/swarms/artifacts/text_artifact.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/memory/__init__.py` & `swarms-5.0.8/swarms/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/memory/base_db.py` & `swarms-5.0.8/swarms/memory/base_db.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/memory/base_vectordb.py` & `swarms-5.0.8/swarms/memory/base_vectordb.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/memory/dict_internal_memory.py` & `swarms-5.0.8/swarms/memory/dict_internal_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/memory/dict_shared_memory.py` & `swarms-5.0.8/swarms/memory/dict_shared_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/memory/short_term_memory.py` & `swarms-5.0.8/swarms/memory/short_term_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/memory/visual_memory.py` & `swarms-5.0.8/swarms/memory/visual_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/__init__.py` & `swarms-5.0.8/swarms/models/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/base_embedding_model.py` & `swarms-5.0.8/swarms/models/base_embedding_model.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/base_llm.py` & `swarms-5.0.8/swarms/models/base_llm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/base_multimodal_model.py` & `swarms-5.0.8/swarms/models/base_multimodal_model.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/base_tts.py` & `swarms-5.0.8/swarms/models/base_tts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/base_ttv.py` & `swarms-5.0.8/swarms/models/base_ttv.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/cog_vlm.py` & `swarms-5.0.8/swarms/models/cog_vlm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/dalle3.py` & `swarms-5.0.8/swarms/models/dalle3.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/distilled_whisperx.py` & `swarms-5.0.8/swarms/models/distilled_whisperx.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/embeddings_base.py` & `swarms-5.0.8/swarms/models/embeddings_base.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/fuyu.py` & `swarms-5.0.8/swarms/models/fuyu.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/gemini.py` & `swarms-5.0.8/swarms/models/gemini.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/gpt4_vision_api.py` & `swarms-5.0.8/swarms/models/gpt4_vision_api.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/huggingface.py` & `swarms-5.0.8/swarms/models/huggingface.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/huggingface_pipeline.py` & `swarms-5.0.8/swarms/models/huggingface_pipeline.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/idefics.py` & `swarms-5.0.8/swarms/models/idefics.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/kosmos_two.py` & `swarms-5.0.8/swarms/models/kosmos_two.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/layoutlm_document_qa.py` & `swarms-5.0.8/swarms/models/layoutlm_document_qa.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/llama3_hosted.py` & `swarms-5.0.8/swarms/models/llama3_hosted.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/llama_function_caller.py` & `swarms-5.0.8/swarms/models/llama_function_caller.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/llava.py` & `swarms-5.0.8/swarms/models/llava.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/moondream_mm.py` & `swarms-5.0.8/swarms/models/moondream_mm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/nougat.py` & `swarms-5.0.8/swarms/models/nougat.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/open_dalle.py` & `swarms-5.0.8/swarms/models/open_dalle.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/open_router.py` & `swarms-5.0.8/swarms/models/open_router.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/openai_tts.py` & `swarms-5.0.8/swarms/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/popular_llms.py` & `swarms-5.0.8/swarms/models/popular_llms.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/qwen.py` & `swarms-5.0.8/swarms/models/qwen.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/sam.py` & `swarms-5.0.8/swarms/models/sam.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/sampling_params.py` & `swarms-5.0.8/swarms/models/sampling_params.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/ssd_1b.py` & `swarms-5.0.8/swarms/models/ssd_1b.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/together.py` & `swarms-5.0.8/swarms/models/together.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/types.py` & `swarms-5.0.8/swarms/models/types.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/vilt.py` & `swarms-5.0.8/swarms/models/vilt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/vip_llava.py` & `swarms-5.0.8/swarms/models/vip_llava.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/models/zeroscope.py` & `swarms-5.0.8/swarms/models/zeroscope.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/__init__.py` & `swarms-5.0.8/swarms/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/accountant_swarm_prompts.py` & `swarms-5.0.8/swarms/prompts/accountant_swarm_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/aga.py` & `swarms-5.0.8/swarms/prompts/aga.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/agent_output_parser.py` & `swarms-5.0.8/swarms/prompts/agent_output_parser.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/agent_prompt.py` & `swarms-5.0.8/swarms/prompts/agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/agent_prompts.py` & `swarms-5.0.8/swarms/prompts/agent_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/agent_system_prompts.py` & `swarms-5.0.8/swarms/prompts/agent_system_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/ai_research_team.py` & `swarms-5.0.8/swarms/prompts/ai_research_team.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/aot_prompt.py` & `swarms-5.0.8/swarms/prompts/aot_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/autobloggen.py` & `swarms-5.0.8/swarms/prompts/autobloggen.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/autoswarm.py` & `swarms-5.0.8/swarms/prompts/autoswarm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/base.py` & `swarms-5.0.8/swarms/prompts/base.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/chat_prompt.py` & `swarms-5.0.8/swarms/prompts/chat_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/code_interpreter.py` & `swarms-5.0.8/swarms/prompts/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/code_spawner.py` & `swarms-5.0.8/swarms/prompts/code_spawner.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/debate.py` & `swarms-5.0.8/swarms/prompts/debate.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/documentation.py` & `swarms-5.0.8/swarms/prompts/documentation.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/education.py` & `swarms-5.0.8/swarms/prompts/education.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/finance_agent_prompt.py` & `swarms-5.0.8/swarms/prompts/finance_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/growth_agent_prompt.py` & `swarms-5.0.8/swarms/prompts/growth_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/idea2img.py` & `swarms-5.0.8/swarms/prompts/idea2img.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/legal_agent_prompt.py` & `swarms-5.0.8/swarms/prompts/legal_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/logistics.py` & `swarms-5.0.8/swarms/prompts/logistics.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/meta_system_prompt.py` & `swarms-5.0.8/swarms/prompts/meta_system_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/multi_modal_autonomous_instruction_prompt.py` & `swarms-5.0.8/swarms/prompts/multi_modal_autonomous_instruction_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/multi_modal_prompts.py` & `swarms-5.0.8/swarms/prompts/multi_modal_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/multi_modal_visual_prompts.py` & `swarms-5.0.8/swarms/prompts/multi_modal_visual_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/operations_agent_prompt.py` & `swarms-5.0.8/swarms/prompts/operations_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/personal_stylist.py` & `swarms-5.0.8/swarms/prompts/personal_stylist.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/product_agent_prompt.py` & `swarms-5.0.8/swarms/prompts/product_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/programming.py` & `swarms-5.0.8/swarms/prompts/programming.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/project_manager.py` & `swarms-5.0.8/swarms/prompts/project_manager.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/python.py` & `swarms-5.0.8/swarms/prompts/python.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/react.py` & `swarms-5.0.8/swarms/prompts/react.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/sales.py` & `swarms-5.0.8/swarms/prompts/sales.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/sales_prompts.py` & `swarms-5.0.8/swarms/prompts/sales_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/security_team.py` & `swarms-5.0.8/swarms/prompts/security_team.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/self_operating_prompt.py` & `swarms-5.0.8/swarms/prompts/self_operating_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/sop_generator_agent_prompt.py` & `swarms-5.0.8/swarms/prompts/sop_generator_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/summaries_prompts.py` & `swarms-5.0.8/swarms/prompts/summaries_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/support_agent_prompt.py` & `swarms-5.0.8/swarms/prompts/support_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/swarm_manager_agent.py` & `swarms-5.0.8/swarms/prompts/swarm_manager_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/task_assignment_prompt.py` & `swarms-5.0.8/swarms/prompts/task_assignment_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/tests.py` & `swarms-5.0.8/swarms/prompts/tests.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/tools.py` & `swarms-5.0.8/swarms/prompts/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,16 +125,14 @@
     ‘‘‘
     # Response
     ‘‘‘
     """
     return PROMPT
 
 
-
-
 def tool_sop_prompt() -> str:
     return """
 
 
     You've been granted tools to assist users by always providing outputs in JSON format for tool usage. 
     Whenever a tool usage is required, you must output the JSON wrapped inside markdown for clarity. 
     Provide a commentary on the tool usage and the user's request and ensure that the JSON output adheres to the tool's schema.
@@ -191,8 +189,8 @@
         }
     }
     }
     ```
 
     Please proceed with your task accordingly.
 
-    """
+    """
```

### Comparing `swarms-5.0.7/swarms/prompts/urban_planning.py` & `swarms-5.0.8/swarms/prompts/urban_planning.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/visual_cot.py` & `swarms-5.0.8/swarms/prompts/visual_cot.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/worker_prompt.py` & `swarms-5.0.8/swarms/prompts/worker_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/prompts/xray_swarm_prompt.py` & `swarms-5.0.8/swarms/prompts/xray_swarm_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/schemas/hass_agent_schema.py` & `swarms-5.0.8/swarms/schemas/hass_agent_schema.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/schemas/schemas.py` & `swarms-5.0.8/swarms/schemas/schemas.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/schemas/step.py` & `swarms-5.0.8/swarms/schemas/step.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/structs/__init__.py` & `swarms-5.0.8/swarms/structs/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/structs/agent.py` & `swarms-5.0.8/swarms/structs/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,29 +20,32 @@
 from swarms.prompts.multi_modal_autonomous_instruction_prompt import (
     MULTI_MODAL_AUTO_AGENT_SYSTEM_PROMPT_1,
 )
 from swarms.structs.conversation import Conversation
 from swarms.structs.yaml_model import YamlModel
 from swarms.telemetry.user_utils import get_user_device_data
 from swarms.tools.base_tool import BaseTool
-from swarms.tools.code_interpreter import SubprocessCodeInterpreter
+from swarms.tools.prebuilt.code_interpreter import (
+    SubprocessCodeInterpreter,
+)
 from swarms.tools.pydantic_to_json import (
     base_model_to_openai_function,
     multi_base_model_to_openai_function,
 )
 from swarms.utils.data_to_text import data_to_text
 from swarms.utils.parse_code import extract_code_from_markdown
 from swarms.utils.pdf_to_text import pdf_to_text
 from swarms.tools.py_func_to_openai_func_str import (
     get_openai_function_schema_from_func,
 )
-from swarms.tools.openai_tool_creator_decorator import openai_tool_executor
+from swarms.tools.func_calling_executor import openai_tool_executor
 from swarms.structs.base_structure import BaseStructure
 from swarms.prompts.tools import tool_sop_prompt
 
+
 # Utils
 # Custom stopping condition
 def stop_when_repeats(response: str) -> bool:
     # Stop if the word stop appears in the response
     return "stop" in response.lower()
 
 
@@ -378,20 +381,17 @@
         #     self.truncate_history()
 
         # If verbose is enabled then set the logger level to info
         # if verbose:
         #     logger.setLevel(logging.INFO)
 
         if tools is not None:
-            
+
             # Add the tool prompt to the memory
-            self.short_memory.add(
-                role="System", content=tool_sop_prompt()
-            )
-            
+            self.short_memory.add(role="System", content=tool_sop_prompt())
 
             # # BaseTool
             # self.base_tool = BaseTool(
             #     functions=tools,
             #     verbose=verbose,
             #     auto_execute_tool=execute_tool,
             #     autocheck=True,
@@ -413,15 +413,15 @@
 
                 # Transform the tool into a openai function calling schema
                 tool_schema_list = get_openai_function_schema_from_func(
                     tool,
                     name=tool.__name__,
                     description=tool.__doc__,
                 )
-                
+
                 # Transform the dictionary to a string
                 tool_schema_list = json.dumps(tool_schema_list, indent=4)
                 # print(tool_schema_list)
 
                 # Add the tool schema to the short memory
                 self.short_memory.add(
                     role="System", content=tool_schema_list
@@ -987,17 +987,16 @@
                     logger.error(
                         "Failed to generate a valid response after"
                         " retry attempts."
                     )
                     break  # Exit the loop if all retry attempts fail
 
                 # Check stopping conditions
-                if self.stopping_token is not None:
-                    if self.stopping_token in response:
-                        break
+                # if self.stopping_token in response:
+                #     break
                 elif (
                     self.stopping_condition is not None
                     and self._check_stopping_condition(response)
                 ):
                     break
                 elif self.stopping_func is not None and self.stopping_func(
                     response
@@ -1033,15 +1032,15 @@
             if self.output_cleaner is not None:
                 logger.info("Applying output cleaner to response.")
                 response = self.output_cleaner(response)
                 logger.info(f"Response after output cleaner: {response}")
 
             # Prepare the output for the output model
             if self.output_type is not None:
-                logger.info("Preparing output for output model.")
+                # logger.info("Preparing output for output model.")
                 response = self.prepare_output_for_output_model(response)
                 print(f"Response after output model: {response}")
 
             # print(response)
 
             return response
         except Exception as error:
```

### Comparing `swarms-5.0.7/swarms/structs/agent_job.py` & `swarms-5.0.8/swarms/structs/agent_job.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/structs/agent_process.py` & `swarms-5.0.8/swarms/structs/agent_process.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/structs/async_workflow.py` & `swarms-5.0.8/swarms/structs/async_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/structs/auto_swarm.py` & `swarms-5.0.8/swarms/structs/auto_swarm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/structs/base_structure.py` & `swarms-5.0.8/swarms/structs/base_structure.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/structs/base_swarm.py` & `swarms-5.0.8/swarms/structs/base_swarm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/structs/base_workflow.py` & `swarms-5.0.8/swarms/structs/base_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/structs/company.py` & `swarms-5.0.8/swarms/structs/company.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/structs/concurrent_workflow.py` & `swarms-5.0.8/swarms/structs/concurrent_workflow.py`

 * *Files 20% similar despite different names*

```diff
@@ -85,43 +85,78 @@
             return_results (bool): Whether to return the results of each task. Default is False.
 
         Returns:
             List[Any]: A list of the results of each task, if return_results is True. Otherwise, returns None.
         """
         loop = 0
         while loop < self.max_loops:
-            with concurrent.futures.ThreadPoolExecutor(
-                max_workers=self.max_workers
-            ) as executor:
-                futures = {
-                    executor.submit(task.execute): task
-                    for task in self.task_pool
-                }
-                results = []
-
-                for future in concurrent.futures.as_completed(futures):
-                    task = futures[future]
-                    try:
-                        result = future.result()
-                        if self.print_results:
-                            logger.info(f"Task {task}: {result}")
-                        if self.return_results:
-                            results.append(result)
-                    except Exception as e:
-                        logger.error(
-                            f"Task {task} generated an exception: {e}"
-                        )
-
-            loop += 1
-            if self.stopping_condition and self.stopping_condition(
-                results
-            ):
+
+            if self.tasks is not None:
+                with concurrent.futures.ThreadPoolExecutor(
+                    max_workers=self.max_workers
+                ) as executor:
+                    futures = {
+                        executor.submit(task.execute): task
+                        for task in self.task_pool
+                    }
+                    results = []
+
+                    for future in concurrent.futures.as_completed(futures):
+                        task = futures[future]
+                        try:
+                            result = future.result()
+                            if self.print_results:
+                                logger.info(f"Task {task}: {result}")
+                            if self.return_results:
+                                results.append(result)
+                        except Exception as e:
+                            logger.error(
+                                f"Task {task} generated an exception: {e}"
+                            )
+
+                loop += 1
+                if self.stopping_condition and self.stopping_condition(
+                    results
+                ):
+                    break
+
+            elif self.agents is not None:
+                with concurrent.futures.ThreadPoolExecutor(
+                    max_workers=self.max_workers
+                ) as executor:
+                    futures = {
+                        executor.submit(agent.run): agent
+                        for agent in self.agents
+                    }
+                    results = []
+
+                    for future in concurrent.futures.as_completed(futures):
+                        agent = futures[future]
+                        try:
+                            result = future.result()
+                            if self.print_results:
+                                logger.info(f"Agent {agent}: {result}")
+                            if self.return_results:
+                                results.append(result)
+                        except Exception as e:
+                            logger.error(
+                                f"Agent {agent} generated an exception: {e}"
+                            )
+
+                loop += 1
+                if self.stopping_condition and self.stopping_condition(
+                    results
+                ):
+                    break
+
+            else:
+                logger.warning("No tasks or agents found in the workflow.")
                 break
 
-        return results if self.return_results else None
+            return results if self.return_results else None
 
     def list_tasks(self):
         """Prints a list of the tasks in the workflow."""
         for task in self.task_pool:
             logger.info(task)
 
     def save(self):
```

### Comparing `swarms-5.0.7/swarms/structs/conversation.py` & `swarms-5.0.8/swarms/structs/conversation.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/structs/debate.py` & `swarms-5.0.8/swarms/structs/debate.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/structs/groupchat.py` & `swarms-5.0.8/swarms/structs/groupchat.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/structs/hiearchical_swarm.py` & `swarms-5.0.8/swarms/structs/hiearchical_swarm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from typing import List
 
-from beartype import beartype
+# from beartype import beartype
 
 from swarms.structs.agent import Agent
 from swarms.structs.base_swarm import BaseSwarm
 from swarms.utils.loguru_logger import logger
 from pydantic import BaseModel, Field
 from swarms.structs.conversation import Conversation
 
@@ -210,15 +210,14 @@
                 )
 
                 return response
         except json.JSONDecodeError:
             logger.error("Invalid JSON data, try again.")
             raise json.JSONDecodeError
 
-    @beartype
     def select_agent_and_send_task(
         self, name: str = None, task: str = None, *args, **kwargs
     ):
         """
         Select an agent from the list and send a task to them.
 
         Args:
@@ -242,15 +241,14 @@
             response = agent.run(task, *args, **kwargs)
 
             return response
         except Exception as e:
             logger.error(f"Error: {e}")
             raise e
 
-    @beartype
     def run(self, task: str = None, *args, **kwargs):
         """
         Run the hierarchical swarm.
 
         Args:
             task (str): The task to send to the director agent.
```

### Comparing `swarms-5.0.7/swarms/structs/majority_voting.py` & `swarms-5.0.8/swarms/structs/majority_voting.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/structs/message.py` & `swarms-5.0.8/swarms/structs/message.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/structs/message_pool.py` & `swarms-5.0.8/swarms/structs/message_pool.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/structs/meta_system_prompt.py` & `swarms-5.0.8/swarms/structs/meta_system_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/structs/multi_agent_collab.py` & `swarms-5.0.8/swarms/structs/multi_agent_collab.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/structs/multi_process_workflow.py` & `swarms-5.0.8/swarms/structs/multi_process_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/structs/multi_threaded_workflow.py` & `swarms-5.0.8/swarms/structs/multi_threaded_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/structs/rearrange.py` & `swarms-5.0.8/swarms/structs/rearrange.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/structs/recursive_workflow.py` & `swarms-5.0.8/swarms/structs/recursive_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/structs/round_robin.py` & `swarms-5.0.8/swarms/structs/round_robin.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/structs/sequential_workflow.py` & `swarms-5.0.8/swarms/structs/sequential_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/structs/sermon_swarm.py` & `swarms-5.0.8/swarms/structs/sermon_swarm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/structs/society_of_agents.py` & `swarms-5.0.8/swarms/structs/society_of_agents.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/structs/swarm_load_balancer.py` & `swarms-5.0.8/swarms/structs/swarm_load_balancer.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/structs/swarm_net.py` & `swarms-5.0.8/swarms/structs/swarm_net.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/structs/swarming_architectures.py` & `swarms-5.0.8/swarms/structs/swarming_architectures.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/structs/task.py` & `swarms-5.0.8/swarms/structs/task.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/structs/task_queue_base.py` & `swarms-5.0.8/swarms/structs/task_queue_base.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/structs/utils.py` & `swarms-5.0.8/swarms/structs/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/structs/yaml_model.py` & `swarms-5.0.8/swarms/structs/yaml_model.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/telemetry/__init__.py` & `swarms-5.0.8/swarms/telemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/telemetry/auto_upgrade_swarms.py` & `swarms-5.0.8/swarms/telemetry/auto_upgrade_swarms.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/telemetry/check_update.py` & `swarms-5.0.8/swarms/telemetry/check_update.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/telemetry/log_all.py` & `swarms-5.0.8/swarms/telemetry/log_all.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/telemetry/sys_info.py` & `swarms-5.0.8/swarms/telemetry/sys_info.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/telemetry/user_utils.py` & `swarms-5.0.8/swarms/telemetry/user_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/tools/base_tool.py` & `swarms-5.0.8/swarms/tools/base_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import json
 from pydantic import BaseModel
 from swarms.utils.loguru_logger import logger
 from swarms.tools.py_func_to_openai_func_str import (
     get_openai_function_schema_from_func,
     load_basemodels_if_needed,
 )
-from swarms.tools.openai_tool_creator_decorator import openai_tool_executor
+from swarms.tools.func_calling_executor import openai_tool_executor
 from typing import Callable, Optional, Any, Dict, List
 from swarms.tools.pydantic_to_json import (
     base_model_to_openai_function,
     multi_base_model_to_openai_function,
-    function_to_str,
-    functions_to_str,
 )
+from swarms.tools.func_to_str import function_to_str, functions_to_str
 from swarms.tools.function_util import process_tool_docs
 from typing import Union
 
 ToolType = Union[BaseModel, Dict[str, Any], Callable[..., Any]]
 
 
 class BaseTool(BaseModel):
```

### Comparing `swarms-5.0.7/swarms/tools/code_interpreter.py` & `swarms-5.0.8/swarms/tools/prebuilt/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/tools/function_util.py` & `swarms-5.0.8/swarms/tools/function_util.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/tools/json_former.py` & `swarms-5.0.8/swarms/tools/json_former.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/tools/json_utils.py` & `swarms-5.0.8/swarms/tools/json_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/tools/logits_processor.py` & `swarms-5.0.8/swarms/tools/logits_processor.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/tools/math_eval.py` & `swarms-5.0.8/swarms/tools/prebuilt/math_eval.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/tools/openai_func_calling_schema_pydantic.py` & `swarms-5.0.8/swarms/tools/openai_func_calling_schema_pydantic.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/tools/py_func_to_openai_func_str.py` & `swarms-5.0.8/swarms/tools/py_func_to_openai_func_str.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/tools/pydantic_to_json.py` & `swarms-5.0.8/swarms/tools/pydantic_to_json.py`

 * *Files 22% similar despite different names*

```diff
@@ -106,46 +106,7 @@
         for pydantic_type in pydantic_types
     ]
 
     return {
         "function_call": "auto",
         "functions": functions,
     }
-
-
-def function_to_str(function: dict[str, Any]) -> str:
-    """
-    Convert a function dictionary to a string representation.
-
-    Args:
-        function (dict[str, Any]): The function dictionary to convert.
-
-    Returns:
-        str: The string representation of the function.
-
-    """
-    function_str = f"Function: {function['name']}\n"
-    function_str += f"Description: {function['description']}\n"
-    function_str += "Parameters:\n"
-
-    for param, details in function["parameters"]["properties"].items():
-        function_str += f"  {param} ({details['type']}): {details.get('description', '')}\n"
-
-    return function_str
-
-
-def functions_to_str(functions: list[dict[str, Any]]) -> str:
-    """
-    Convert a list of function dictionaries to a string representation.
-
-    Args:
-        functions (list[dict[str, Any]]): The list of function dictionaries to convert.
-
-    Returns:
-        str: The string representation of the functions.
-
-    """
-    functions_str = ""
-    for function in functions:
-        functions_str += function_to_str(function) + "\n"
-
-    return functions_str
```

### Comparing `swarms-5.0.7/swarms/tools/tool_utils.py` & `swarms-5.0.8/swarms/tools/tool_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,15 +178,17 @@
     ‘‘‘
     # Response
     ‘‘‘
     """
     return PROMPT
 
 
-def is_str_valid_func_output(output: str = None, function_map: callable = None):
+def is_str_valid_func_output(
+    output: str = None, function_map: callable = None
+):
     """
     Check if the output is a valid JSON string, and if the function name in the JSON matches any name in the function map.
 
     Args:
         output (str): The output to check.
         function_map (dict): A dictionary mapping function names to functions.
 
@@ -194,20 +196,22 @@
         bool: True if the output is valid and the function name matches, False otherwise.
     """
     try:
         # Parse the output as JSON
         data = json.loads(output)
 
         # Check if the output matches the schema
-        if (data.get('type') == 'function' and 
-            'function' in data and 
-            'name' in data['function']):
+        if (
+            data.get("type") == "function"
+            and "function" in data
+            and "name" in data["function"]
+        ):
 
             # Check if the function name matches any name in the function map
-            function_name = data['function']['name']
+            function_name = data["function"]["name"]
             if function_name in function_map:
                 return True
 
     except json.JSONDecodeError:
         pass
 
-    return False
+    return False
```

### Comparing `swarms-5.0.7/swarms/utils/README.md` & `swarms-5.0.8/swarms/utils/README.md`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/utils/__init__.py` & `swarms-5.0.8/swarms/utils/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from swarms.utils.class_args_wrapper import print_class_parameters
-from swarms.tools.code_interpreter import SubprocessCodeInterpreter
+from swarms.tools.prebuilt.code_interpreter import (
+    SubprocessCodeInterpreter,
+)
 from swarms.utils.data_to_text import (
     csv_to_text,
     data_to_text,
     json_to_text,
     txt_to_text,
 )
 from swarms.utils.download_img import download_img_from_url
@@ -15,15 +17,15 @@
     create_file_in_folder,
     zip_folders,
 )
 from swarms.utils.find_img_path import find_image_path
 from swarms.utils.json_output_parser import JsonOutputParser
 from swarms.utils.llm_metrics_decorator import metrics_decorator
 from swarms.utils.markdown_message import display_markdown_message
-from swarms.tools.math_eval import math_eval
+from swarms.tools.prebuilt.math_eval import math_eval
 from swarms.utils.parse_code import extract_code_from_markdown
 from swarms.utils.pdf_to_text import pdf_to_text
 from swarms.utils.remove_json_whitespace import (
     remove_whitespace_from_json,
     remove_whitespace_from_yaml,
 )
 from swarms.utils.save_logs import parse_log_file
```

### Comparing `swarms-5.0.7/swarms/utils/apa.py` & `swarms-5.0.8/swarms/utils/apa.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/utils/check_function_result.py` & `swarms-5.0.8/swarms/utils/check_function_result.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/utils/class_args_wrapper.py` & `swarms-5.0.8/swarms/utils/class_args_wrapper.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/utils/concurrent_utils.py` & `swarms-5.0.8/swarms/utils/concurrent_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/utils/data_to_text.py` & `swarms-5.0.8/swarms/utils/data_to_text.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/utils/decorators.py` & `swarms-5.0.8/swarms/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/utils/disable_logging.py` & `swarms-5.0.8/swarms/utils/disable_logging.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/utils/download_img.py` & `swarms-5.0.8/swarms/utils/download_img.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/utils/execute_futures.py` & `swarms-5.0.8/swarms/utils/execute_futures.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/utils/exponential_backoff.py` & `swarms-5.0.8/swarms/utils/exponential_backoff.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/utils/fetch_init_params.py` & `swarms-5.0.8/swarms/utils/fetch_init_params.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/utils/file_processing.py` & `swarms-5.0.8/swarms/utils/file_processing.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/utils/find_img_path.py` & `swarms-5.0.8/swarms/utils/find_img_path.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/utils/get_logger.py` & `swarms-5.0.8/swarms/utils/get_logger.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/utils/get_total_gpus.py` & `swarms-5.0.8/swarms/utils/get_total_gpus.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/utils/json_output_parser.py` & `swarms-5.0.8/swarms/utils/json_output_parser.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/utils/jsonl_utils.py` & `swarms-5.0.8/swarms/utils/jsonl_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/utils/llm_metrics_decorator.py` & `swarms-5.0.8/swarms/utils/llm_metrics_decorator.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/utils/logger.py` & `swarms-5.0.8/swarms/utils/logger.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/utils/loggers.py` & `swarms-5.0.8/swarms/utils/loggers.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/utils/markdown_message.py` & `swarms-5.0.8/swarms/utils/markdown_message.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/utils/parse_code.py` & `swarms-5.0.8/swarms/utils/parse_code.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/utils/pdf_to_text.py` & `swarms-5.0.8/swarms/utils/pdf_to_text.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/utils/remove_json_whitespace.py` & `swarms-5.0.8/swarms/utils/remove_json_whitespace.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/utils/save_logs.py` & `swarms-5.0.8/swarms/utils/save_logs.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/utils/serializable.py` & `swarms-5.0.8/swarms/utils/serializable.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/utils/try_except_wrapper.py` & `swarms-5.0.8/swarms/utils/try_except_wrapper.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/swarms/utils/yaml_output_parser.py` & `swarms-5.0.8/swarms/utils/yaml_output_parser.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.7/PKG-INFO` & `swarms-5.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 5.0.7
+Version: 5.0.8
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering,swarms,agents
 Author: Kye Gomez
 Author-email: kye@apac.ai
 Requires-Python: >=3.10,<4.0
@@ -146,26 +146,25 @@
 ```
 
 
 # `Agent` with Long Term Memory ++ Tools!
 An LLM equipped with long term memory and tools, a full stack agent capable of automating all and any digital tasks given a good prompt.
 
 ```python
-from swarms import Agent, ChromaDB, OpenAIChat, tool
+from swarms import Agent, ChromaDB, OpenAIChat
 
 # Making an instance of the ChromaDB class
 memory = ChromaDB(
     metric="cosine",
     n_results=3,
     output_dir="results",
     docs_folder="docs",
 )
 
 # Initialize a tool
-@tool
 def search_api(query: str):
     # Add your logic here
     return query
 
 # Initializing the agent with the Gemini instance and other parameters
 agent = Agent(
     agent_name="Covid-19-Chat",
@@ -222,24 +221,23 @@
 ```
 
 ## Devin
 Implementation of Devil in less than 90 lines of code with several tools:
 terminal, browser, and edit files!
 
 ```python
-from swarms import Agent, Anthropic, tool
+from swarms import Agent, Anthropic
 import subprocess
 
 # Model
 llm = Anthropic(
     temperature=0.1,
 )
 
 # Tools
-@tool
 def terminal(
     code: str,
 ):
     """
     Run code in the terminal.
 
     Args:
@@ -249,16 +247,14 @@
         str: The output of the code.
     """
     out = subprocess.run(
         code, shell=True, capture_output=True, text=True
     ).stdout
     return str(out)
 
-
-@tool
 def browser(query: str):
     """
     Search the query in the browser with the `browser` tool.
 
     Args:
         query (str): The query to search in the browser.
 
@@ -267,15 +263,14 @@
     """
     import webbrowser
 
     url = f"https://www.google.com/search?q={query}"
     webbrowser.open(url)
     return f"Searching for {query} in the browser."
 
-@tool
 def create_file(file_path: str, content: str):
     """
     Create a file using the file editor tool.
 
     Args:
         file_path (str): The path to the file.
         content (str): The content to write to the file.
@@ -283,15 +278,14 @@
     Returns:
         str: The result of the file creation operation.
     """
     with open(file_path, "w") as file:
         file.write(content)
     return f"File {file_path} created successfully."
 
-@tool
 def file_editor(file_path: str, mode: str, content: str):
     """
     Edit a file using the file editor tool.
 
     Args:
         file_path (str): The path to the file.
         mode (str): The mode to open the file in.
@@ -1146,14 +1140,22 @@
 
 ```
 
 ## `HierarhicalSwarm`
 Coming soon...
 
 
+## `AgentLoadBalancer`
+Coming soon...
+
+
+## `GraphSwarm`
+Coming soon...
+
+
 ---
 
 ## Documentation
 Documentation is located here at: [swarms.apac.ai](https://swarms.apac.ai)
 
 ----
```

