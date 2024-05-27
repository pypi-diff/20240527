# Comparing `tmp/wafl-0.0.9-py3-none-any.whl.zip` & `tmp/wafl-0.0.90-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,68 +1,133 @@
-Zip file size: 1753661 bytes, number of entries: 66
--rw-rw-r--  2.0 unx        0 b- defN 21-Dec-12 17:38 wafl/__init__.py
--rw-rw-r--  2.0 unx      834 b- defN 22-Jan-06 12:13 wafl/__main__.py
--rw-rw-r--  2.0 unx     1800 b- defN 22-Oct-31 11:33 wafl/config.py
--rw-rw-r--  2.0 unx     1895 b- defN 22-Oct-07 12:12 wafl/deixis.py
--rw-rw-r--  2.0 unx       88 b- defN 22-Jan-05 11:44 wafl/exceptions.py
--rw-rw-r--  2.0 unx      261 b- defN 22-Jul-23 08:36 wafl/facts.py
--rw-rw-r--  2.0 unx      175 b- defN 21-Dec-20 11:53 wafl/rules.py
--rw-rw-r--  2.0 unx     2708 b- defN 22-Nov-02 21:14 wafl/run.py
--rw-rw-r--  2.0 unx     1675 b- defN 22-Jan-08 17:06 wafl/testcases.py
--rw-rw-r--  2.0 unx      102 b- defN 22-Feb-05 17:26 wafl/text_utils.py
--rw-rw-r--  2.0 unx        0 b- defN 21-Dec-20 15:10 wafl/conversation/__init__.py
--rw-rw-r--  2.0 unx     3352 b- defN 22-Oct-31 16:20 wafl/conversation/conversation.py
--rw-rw-r--  2.0 unx     3662 b- defN 22-Oct-16 14:32 wafl/conversation/utils.py
--rw-rw-r--  2.0 unx     1431 b- defN 22-Oct-01 09:34 wafl/conversation/working_memory.py
--rw-rw-r--  2.0 unx        0 b- defN 21-Dec-29 12:22 wafl/inference/__init__.py
--rw-rw-r--  2.0 unx    14613 b- defN 22-Nov-02 21:07 wafl/inference/backward_inference.py
--rw-rw-r--  2.0 unx     4322 b- defN 22-Oct-31 15:46 wafl/inference/utils.py
--rw-rw-r--  2.0 unx        0 b- defN 21-Dec-27 15:39 wafl/interface/__init__.py
--rw-rw-r--  2.0 unx      307 b- defN 22-Oct-01 15:28 wafl/interface/base_interface.py
--rw-rw-r--  2.0 unx     1135 b- defN 22-Nov-02 21:07 wafl/interface/command_line_interface.py
--rw-rw-r--  2.0 unx     1336 b- defN 22-Nov-02 21:07 wafl/interface/dummy_interface.py
--rw-rw-r--  2.0 unx      307 b- defN 22-Oct-01 15:28 wafl/interface/interface.py
--rw-rw-r--  2.0 unx      933 b- defN 22-Aug-29 19:15 wafl/interface/utils.py
--rw-rw-r--  2.0 unx     3882 b- defN 22-Nov-02 21:07 wafl/interface/voice_interface.py
--rw-rw-r--  2.0 unx        0 b- defN 21-Dec-20 16:15 wafl/knowledge/__init__.py
--rw-rw-r--  2.0 unx      241 b- defN 22-Jan-10 15:02 wafl/knowledge/base_knowledge.py
--rw-rw-r--  2.0 unx     8431 b- defN 22-Oct-31 15:50 wafl/knowledge/knowledge.py
--rw-rw-r--  2.0 unx     1978 b- defN 22-Oct-07 15:40 wafl/knowledge/utils.py
--rw-rw-r--  2.0 unx        0 b- defN 21-Dec-27 15:47 wafl/listener/__init__.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Oct-01 13:21 wafl/listener/utils.py
--rw-rw-r--  2.0 unx     3659 b- defN 22-Sep-03 14:25 wafl/listener/wav2vec2_listener.py
--rw-rw-r--  2.0 unx     4676 b- defN 22-Oct-31 19:32 wafl/listener/whisper_listener.py
--rw-rw-r--  2.0 unx  3752847 b- defN 22-Sep-03 10:05 wafl/models/discourse_count_vectorizer.joblib
--rw-rw-r--  2.0 unx        0 b- defN 21-Dec-29 12:23 wafl/parsing/__init__.py
--rw-rw-r--  2.0 unx     1434 b- defN 22-Oct-16 16:16 wafl/parsing/preprocess.py
--rw-rw-r--  2.0 unx     1921 b- defN 22-Oct-16 16:23 wafl/parsing/rules_parser.py
--rw-rw-r--  2.0 unx     1511 b- defN 22-Jan-06 15:30 wafl/parsing/testcase_parser.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Feb-05 17:30 wafl/parsing/utils.py
--rw-rw-r--  2.0 unx        6 b- defN 22-Oct-31 15:58 wafl/qa/__init__.py
--rw-rw-r--  2.0 unx      369 b- defN 22-Sep-03 08:44 wafl/qa/common_sense.py
--rw-rw-r--  2.0 unx      609 b- defN 22-Oct-16 16:16 wafl/qa/dataclasses.py
--rw-rw-r--  2.0 unx     2225 b- defN 22-Oct-31 16:23 wafl/qa/entailer.py
--rw-rw-r--  2.0 unx     1980 b- defN 22-Oct-31 16:22 wafl/qa/qa.py
--rw-rw-r--  2.0 unx      296 b- defN 22-Aug-27 15:08 wafl/qa/utils.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Jan-03 16:39 wafl/retriever/__init__.py
--rw-rw-r--  2.0 unx      256 b- defN 22-Jan-03 16:55 wafl/retriever/base_retriever.py
--rw-rw-r--  2.0 unx     1642 b- defN 22-Feb-13 14:55 wafl/retriever/dense_retriever.py
--rw-rw-r--  2.0 unx      499 b- defN 22-Jan-03 17:08 wafl/retriever/string_retriever.py
+Zip file size: 325216 bytes, number of entries: 131
+-rw-r--r--  2.0 unx        0 b- defN 21-Dec-12 17:38 wafl/__init__.py
+-rw-r--r--  2.0 unx       74 b- defN 24-Jan-12 18:19 wafl/__main__.py
+-rw-r--r--  2.0 unx     2492 b- defN 24-May-17 08:23 wafl/command_line.py
+-rw-r--r--  2.0 unx     1443 b- defN 24-Jan-12 18:19 wafl/config.py
+-rw-r--r--  2.0 unx       88 b- defN 22-Jan-05 11:44 wafl/exceptions.py
+-rw-r--r--  2.0 unx      299 b- defN 24-May-10 14:16 wafl/facts.py
+-rw-r--r--  2.0 unx     1648 b- defN 24-May-27 09:24 wafl/rules.py
+-rw-r--r--  2.0 unx     1460 b- defN 24-Jan-14 17:15 wafl/run.py
+-rw-r--r--  2.0 unx     3342 b- defN 24-Jan-12 18:19 wafl/testcases.py
+-rw-r--r--  2.0 unx      102 b- defN 22-Feb-05 17:26 wafl/text_utils.py
+-rw-r--r--  2.0 unx      193 b- defN 24-May-27 13:58 wafl/variables.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-12 18:19 wafl/answerer/__init__.py
+-rw-r--r--  2.0 unx      517 b- defN 24-Jan-12 18:19 wafl/answerer/answerer_implementation.py
+-rw-r--r--  2.0 unx      111 b- defN 24-Jan-12 18:19 wafl/answerer/base_answerer.py
+-rw-r--r--  2.0 unx     9217 b- defN 24-May-27 13:50 wafl/answerer/dialogue_answerer.py
+-rw-r--r--  2.0 unx     1409 b- defN 24-May-27 13:42 wafl/answerer/entailer.py
+-rw-r--r--  2.0 unx     2039 b- defN 24-May-10 14:04 wafl/answerer/rule_creator.py
+-rw-r--r--  2.0 unx     1314 b- defN 24-May-27 13:42 wafl/answerer/rule_maker.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-12 18:19 wafl/connectors/__init__.py
+-rw-r--r--  2.0 unx     1683 b- defN 24-May-25 10:17 wafl/connectors/base_llm_connector.py
+-rw-r--r--  2.0 unx      945 b- defN 24-May-25 11:37 wafl/connectors/prompt_template.py
+-rw-r--r--  2.0 unx      330 b- defN 24-May-24 10:44 wafl/connectors/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-12 18:19 wafl/connectors/bridges/__init__.py
+-rw-r--r--  2.0 unx      592 b- defN 24-Jan-12 18:19 wafl/connectors/bridges/bridge_implementation.py
+-rw-r--r--  2.0 unx     1268 b- defN 24-Jan-12 18:19 wafl/connectors/bridges/llm_chitchat_answer_bridge.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-12 18:19 wafl/connectors/clients/__init__.py
+-rw-r--r--  2.0 unx      592 b- defN 24-Jan-12 18:19 wafl/connectors/clients/clients_implementation.py
+-rw-r--r--  2.0 unx     1491 b- defN 24-May-27 13:33 wafl/connectors/clients/llm_chitchat_answer_client.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-12 18:19 wafl/connectors/factories/__init__.py
+-rw-r--r--  2.0 unx      218 b- defN 24-Jan-12 18:19 wafl/connectors/factories/llm_connector_factory.py
+-rw-r--r--  2.0 unx      291 b- defN 24-Jan-27 16:47 wafl/connectors/factories/sentence_embedder_connector_factory.py
+-rw-r--r--  2.0 unx      238 b- defN 24-Jan-12 18:19 wafl/connectors/factories/speaker_connector_factory.py
+-rw-r--r--  2.0 unx      239 b- defN 24-Jan-12 18:19 wafl/connectors/factories/whisper_connector_factory.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-12 18:19 wafl/connectors/remote/__init__.py
+-rw-r--r--  2.0 unx     3528 b- defN 24-May-25 11:07 wafl/connectors/remote/remote_llm_connector.py
+-rw-r--r--  2.0 unx     1900 b- defN 24-Jan-12 18:19 wafl/connectors/remote/remote_sentence_embedder_connector.py
+-rw-r--r--  2.0 unx     1906 b- defN 24-Jan-12 18:19 wafl/connectors/remote/remote_speaker_connector.py
+-rw-r--r--  2.0 unx     2492 b- defN 24-May-10 15:35 wafl/connectors/remote/remote_whisper_connector.py
+-rw-r--r--  2.0 unx      117 b- defN 24-Jan-12 18:19 wafl/events/BaseEventCreator.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-12 18:19 wafl/events/__init__.py
+-rw-r--r--  2.0 unx      233 b- defN 24-Jan-12 18:19 wafl/events/answerer_creator.py
+-rw-r--r--  2.0 unx     4162 b- defN 24-May-27 09:43 wafl/events/conversation_events.py
+-rw-r--r--  2.0 unx     1438 b- defN 24-Jan-12 18:19 wafl/events/conversational_memory.py
+-rw-r--r--  2.0 unx      321 b- defN 24-Jan-12 18:19 wafl/events/events_from_function_list.py
+-rw-r--r--  2.0 unx      612 b- defN 24-Jan-12 18:19 wafl/events/events_from_module_name.py
+-rw-r--r--  2.0 unx     2123 b- defN 24-Jan-12 18:19 wafl/events/narrator.py
+-rw-r--r--  2.0 unx       64 b- defN 24-Jan-12 18:19 wafl/events/suppress_huggingface_logger.py
+-rw-r--r--  2.0 unx     1503 b- defN 24-Jan-12 18:19 wafl/events/task_memory.py
+-rw-r--r--  2.0 unx      783 b- defN 24-Jan-12 18:19 wafl/events/utils.py
+-rw-r--r--  2.0 unx        6 b- defN 24-Jan-12 18:19 wafl/extractors/__init__.py
+-rw-r--r--  2.0 unx     1228 b- defN 24-Jan-12 18:19 wafl/extractors/dataclasses.py
+-rw-r--r--  2.0 unx      530 b- defN 24-Jan-12 18:19 wafl/extractors/utils.py
+-rw-r--r--  2.0 unx     4853 b- defN 24-Jan-14 17:27 wafl/frontend/index.html
+-rw-r--r--  2.0 unx      482 b- defN 24-May-10 14:16 wafl/frontend/selector.html
+-rw-r--r--  2.0 unx     2242 b- defN 24-May-10 14:13 wafl/frontend/wafl.css
+-rw-r--r--  2.0 unx      164 b- defN 24-Jan-12 18:19 wafl/frontend/wafl.js
+-rw-r--r--  2.0 unx     9201 b- defN 24-Jan-12 18:19 wafl/inference/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 21-Dec-27 15:39 wafl/interface/__init__.py
+-rw-r--r--  2.0 unx     2346 b- defN 24-May-25 14:20 wafl/interface/base_interface.py
+-rw-r--r--  2.0 unx     1143 b- defN 24-Jan-12 18:19 wafl/interface/command_line_interface.py
+-rw-r--r--  2.0 unx     3486 b- defN 24-May-25 14:13 wafl/interface/conversation.py
+-rw-r--r--  2.0 unx     2064 b- defN 24-May-25 10:31 wafl/interface/dummy_interface.py
+-rw-r--r--  2.0 unx     1878 b- defN 24-May-27 13:42 wafl/interface/list_interface.py
+-rw-r--r--  2.0 unx     1055 b- defN 24-May-25 10:31 wafl/interface/queue_interface.py
+-rw-r--r--  2.0 unx      999 b- defN 24-Jan-12 18:19 wafl/interface/utils.py
+-rw-r--r--  2.0 unx     3898 b- defN 24-May-25 10:31 wafl/interface/voice_interface.py
+-rw-r--r--  2.0 unx        0 b- defN 21-Dec-20 16:15 wafl/knowledge/__init__.py
+-rw-r--r--  2.0 unx      538 b- defN 24-Jan-12 18:19 wafl/knowledge/base_knowledge.py
+-rw-r--r--  2.0 unx     7696 b- defN 24-May-10 14:13 wafl/knowledge/single_file_knowledge.py
+-rw-r--r--  2.0 unx     2108 b- defN 24-May-10 14:13 wafl/knowledge/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 21-Dec-27 15:47 wafl/listener/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-12 18:19 wafl/listener/utils.py
+-rw-r--r--  2.0 unx     4302 b- defN 24-May-07 17:47 wafl/listener/whisper_listener.py
+-rw-r--r--  2.0 unx      357 b- defN 24-Jan-12 18:19 wafl/logger/base_logger.py
+-rw-r--r--  2.0 unx     1679 b- defN 24-Jan-12 18:19 wafl/logger/history_logger.py
+-rw-r--r--  2.0 unx      867 b- defN 24-Jan-12 18:19 wafl/logger/local_file_logger.py
+-rw-r--r--  2.0 unx        0 b- defN 21-Dec-29 12:23 wafl/parsing/__init__.py
+-rw-r--r--  2.0 unx      591 b- defN 24-Jan-12 18:19 wafl/parsing/line_rules_parser.py
+-rw-r--r--  2.0 unx     3057 b- defN 24-Jan-12 18:19 wafl/parsing/preprocess.py
+-rw-r--r--  2.0 unx      780 b- defN 24-May-10 14:13 wafl/parsing/rules_parser.py
+-rw-r--r--  2.0 unx     1679 b- defN 24-Jan-12 18:19 wafl/parsing/testcase_parser.py
+-rw-r--r--  2.0 unx      779 b- defN 24-Jan-12 18:19 wafl/parsing/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Jan-03 16:39 wafl/retriever/__init__.py
+-rw-r--r--  2.0 unx      282 b- defN 24-Jan-12 18:19 wafl/retriever/base_retriever.py
+-rw-r--r--  2.0 unx     1581 b- defN 24-Jan-12 18:19 wafl/retriever/dense_retriever.py
+-rw-r--r--  2.0 unx      525 b- defN 24-Jan-12 18:19 wafl/retriever/string_retriever.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-12 18:19 wafl/runners/__init__.py
+-rw-r--r--  2.0 unx     3800 b- defN 24-May-25 14:08 wafl/runners/functions.py
+-rw-r--r--  2.0 unx     2168 b- defN 24-May-10 15:35 wafl/runners/routes.py
+-rw-r--r--  2.0 unx     2681 b- defN 24-Jan-14 17:15 wafl/runners/run_from_actions.py
+-rw-r--r--  2.0 unx      892 b- defN 24-May-17 12:47 wafl/runners/run_from_audio.py
+-rw-r--r--  2.0 unx     2183 b- defN 24-May-17 12:47 wafl/runners/run_web_and_audio_interface.py
+-rw-r--r--  2.0 unx     2184 b- defN 24-May-17 12:47 wafl/runners/run_web_interface.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-12 18:19 wafl/scheduler/__init__.py
+-rw-r--r--  2.0 unx     3944 b- defN 24-May-25 14:28 wafl/scheduler/conversation_handler.py
+-rw-r--r--  2.0 unx     3941 b- defN 24-May-07 07:41 wafl/scheduler/conversation_loop.py
+-rw-r--r--  2.0 unx      588 b- defN 24-May-17 12:44 wafl/scheduler/generated_event_handler.py
+-rw-r--r--  2.0 unx      585 b- defN 24-Jan-12 18:19 wafl/scheduler/generated_event_loop.py
+-rw-r--r--  2.0 unx     2027 b- defN 24-May-27 13:42 wafl/scheduler/messages_creator.py
+-rw-r--r--  2.0 unx      315 b- defN 24-Jan-12 18:19 wafl/scheduler/scheduler.py
+-rw-r--r--  2.0 unx     3324 b- defN 24-May-17 12:44 wafl/scheduler/web_handler.py
+-rw-r--r--  2.0 unx      710 b- defN 24-Jan-12 18:19 wafl/scheduler/web_interface_implementation.py
+-rw-r--r--  2.0 unx     3321 b- defN 24-May-07 17:44 wafl/scheduler/web_loop.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-12 18:19 wafl/simple_text_processing/__init__.py
+-rw-r--r--  2.0 unx     2810 b- defN 24-Jan-12 18:19 wafl/simple_text_processing/deixis.py
+-rw-r--r--  2.0 unx      221 b- defN 24-Jan-12 18:19 wafl/simple_text_processing/normalize.py
+-rw-r--r--  2.0 unx     2515 b- defN 24-Jan-12 18:19 wafl/simple_text_processing/questions.py
 -rw-rw-r--  2.0 unx    90190 b- defN 22-Jul-23 08:45 wafl/sounds/activation.wav
 -rw-rw-r--  2.0 unx   108622 b- defN 22-Jul-23 08:45 wafl/sounds/deactivation.wav
--rw-rw-r--  2.0 unx    99418 b- defN 22-Oct-01 16:25 wafl/sounds/deny.wav
--rw-rw-r--  2.0 unx        0 b- defN 21-Dec-27 15:52 wafl/speaker/__init__.py
--rw-rw-r--  2.0 unx       75 b- defN 22-Jan-02 16:24 wafl/speaker/base_speaker.py
--rw-rw-r--  2.0 unx     1529 b- defN 22-Oct-08 15:31 wafl/speaker/fairseq_speaker.py
--rw-rw-r--  2.0 unx      492 b- defN 22-Jan-02 16:24 wafl/speaker/festival_speaker.py
--rw-rw-r--  2.0 unx      752 b- defN 22-Sep-03 16:29 wafl/speaker/soundfile_speaker.py
+-rw-r--r--  2.0 unx    99418 b- defN 24-Jan-12 18:19 wafl/sounds/deny.wav
+-rw-r--r--  2.0 unx        0 b- defN 21-Dec-27 15:52 wafl/speaker/__init__.py
+-rw-r--r--  2.0 unx       75 b- defN 22-Jan-02 16:24 wafl/speaker/base_speaker.py
+-rw-r--r--  2.0 unx      900 b- defN 24-Jan-12 18:19 wafl/speaker/fairseq_speaker.py
+-rw-r--r--  2.0 unx      752 b- defN 22-Sep-03 16:29 wafl/speaker/soundfile_speaker.py
+-rw-r--r--  2.0 unx      519 b- defN 24-May-07 10:17 wafl/speaker/utils.py
 -rw-rw-r--  2.0 unx        0 b- defN 21-Dec-12 18:41 wafl/templates/__init__.py
--rw-rw-r--  2.0 unx      264 b- defN 22-Oct-31 17:56 wafl/templates/config.json
--rw-rw-r--  2.0 unx      104 b- defN 22-Jan-06 14:55 wafl/templates/functions.py
--rw-rw-r--  2.0 unx      124 b- defN 22-Jan-09 11:54 wafl/templates/rules.wafl
--rw-rw-r--  2.0 unx        0 b- defN 21-Dec-12 18:21 wafl/templates/server.py
--rw-rw-r--  2.0 unx      122 b- defN 22-Jan-09 11:54 wafl/templates/testcases.txt
--rw-rw-r--  2.0 unx     1433 b- defN 22-Nov-02 21:15 wafl-0.0.9.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Nov-02 21:15 wafl-0.0.9.dist-info/WHEEL
--rw-rw-r--  2.0 unx        5 b- defN 22-Nov-02 21:15 wafl-0.0.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     5348 b- defN 22-Nov-02 21:15 wafl-0.0.9.dist-info/RECORD
-66 files, 4138642 bytes uncompressed, 1745223 bytes compressed:  57.8%
+-rw-r--r--  2.0 unx      243 b- defN 24-Jan-12 18:19 wafl/templates/actions.yaml
+-rw-r--r--  2.0 unx      627 b- defN 24-May-11 11:13 wafl/templates/config.json
+-rw-r--r--  2.0 unx       71 b- defN 24-Jan-12 18:19 wafl/templates/db.json
+-rw-r--r--  2.0 unx     3800 b- defN 24-May-25 14:08 wafl/templates/functions.py
+-rw-r--r--  2.0 unx      114 b- defN 24-Jan-12 18:19 wafl/templates/main.py
+-rw-r--r--  2.0 unx       11 b- defN 24-Jan-12 18:19 wafl/templates/requirements.txt
+-rw-r--r--  2.0 unx     3359 b- defN 24-May-27 13:56 wafl/templates/rules.yaml
+-rw-r--r--  2.0 unx       36 b- defN 24-Jan-12 18:19 wafl/templates/secrets.json
+-rw-r--r--  2.0 unx      185 b- defN 24-Jan-12 18:19 wafl/templates/start_llm.sh
+-rw-r--r--  2.0 unx      122 b- defN 24-Jan-12 18:19 wafl/templates/testcases.txt
+-rw-r--r--  2.0 unx     4226 b- defN 24-May-27 14:05 wafl-0.0.90.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-27 14:05 wafl-0.0.90.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       48 b- defN 24-May-27 14:05 wafl-0.0.90.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        5 b- defN 24-May-27 14:05 wafl-0.0.90.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    11330 b- defN 24-May-27 14:05 wafl-0.0.90.dist-info/RECORD
+131 files, 480167 bytes uncompressed, 307162 bytes compressed:  36.0%
```

## zipnote {}

```diff
@@ -1,17 +1,17 @@
 Filename: wafl/__init__.py
 Comment: 
 
 Filename: wafl/__main__.py
 Comment: 
 
-Filename: wafl/config.py
+Filename: wafl/command_line.py
 Comment: 
 
-Filename: wafl/deixis.py
+Filename: wafl/config.py
 Comment: 
 
 Filename: wafl/exceptions.py
 Comment: 
 
 Filename: wafl/facts.py
 Comment: 
@@ -24,126 +24,303 @@
 
 Filename: wafl/testcases.py
 Comment: 
 
 Filename: wafl/text_utils.py
 Comment: 
 
-Filename: wafl/conversation/__init__.py
+Filename: wafl/variables.py
+Comment: 
+
+Filename: wafl/answerer/__init__.py
+Comment: 
+
+Filename: wafl/answerer/answerer_implementation.py
+Comment: 
+
+Filename: wafl/answerer/base_answerer.py
+Comment: 
+
+Filename: wafl/answerer/dialogue_answerer.py
+Comment: 
+
+Filename: wafl/answerer/entailer.py
+Comment: 
+
+Filename: wafl/answerer/rule_creator.py
+Comment: 
+
+Filename: wafl/answerer/rule_maker.py
+Comment: 
+
+Filename: wafl/connectors/__init__.py
+Comment: 
+
+Filename: wafl/connectors/base_llm_connector.py
+Comment: 
+
+Filename: wafl/connectors/prompt_template.py
+Comment: 
+
+Filename: wafl/connectors/utils.py
+Comment: 
+
+Filename: wafl/connectors/bridges/__init__.py
+Comment: 
+
+Filename: wafl/connectors/bridges/bridge_implementation.py
+Comment: 
+
+Filename: wafl/connectors/bridges/llm_chitchat_answer_bridge.py
+Comment: 
+
+Filename: wafl/connectors/clients/__init__.py
+Comment: 
+
+Filename: wafl/connectors/clients/clients_implementation.py
+Comment: 
+
+Filename: wafl/connectors/clients/llm_chitchat_answer_client.py
+Comment: 
+
+Filename: wafl/connectors/factories/__init__.py
+Comment: 
+
+Filename: wafl/connectors/factories/llm_connector_factory.py
+Comment: 
+
+Filename: wafl/connectors/factories/sentence_embedder_connector_factory.py
+Comment: 
+
+Filename: wafl/connectors/factories/speaker_connector_factory.py
+Comment: 
+
+Filename: wafl/connectors/factories/whisper_connector_factory.py
+Comment: 
+
+Filename: wafl/connectors/remote/__init__.py
+Comment: 
+
+Filename: wafl/connectors/remote/remote_llm_connector.py
+Comment: 
+
+Filename: wafl/connectors/remote/remote_sentence_embedder_connector.py
+Comment: 
+
+Filename: wafl/connectors/remote/remote_speaker_connector.py
+Comment: 
+
+Filename: wafl/connectors/remote/remote_whisper_connector.py
+Comment: 
+
+Filename: wafl/events/BaseEventCreator.py
+Comment: 
+
+Filename: wafl/events/__init__.py
+Comment: 
+
+Filename: wafl/events/answerer_creator.py
+Comment: 
+
+Filename: wafl/events/conversation_events.py
+Comment: 
+
+Filename: wafl/events/conversational_memory.py
+Comment: 
+
+Filename: wafl/events/events_from_function_list.py
+Comment: 
+
+Filename: wafl/events/events_from_module_name.py
+Comment: 
+
+Filename: wafl/events/narrator.py
 Comment: 
 
-Filename: wafl/conversation/conversation.py
+Filename: wafl/events/suppress_huggingface_logger.py
 Comment: 
 
-Filename: wafl/conversation/utils.py
+Filename: wafl/events/task_memory.py
 Comment: 
 
-Filename: wafl/conversation/working_memory.py
+Filename: wafl/events/utils.py
 Comment: 
 
-Filename: wafl/inference/__init__.py
+Filename: wafl/extractors/__init__.py
 Comment: 
 
-Filename: wafl/inference/backward_inference.py
+Filename: wafl/extractors/dataclasses.py
+Comment: 
+
+Filename: wafl/extractors/utils.py
+Comment: 
+
+Filename: wafl/frontend/index.html
+Comment: 
+
+Filename: wafl/frontend/selector.html
+Comment: 
+
+Filename: wafl/frontend/wafl.css
+Comment: 
+
+Filename: wafl/frontend/wafl.js
 Comment: 
 
 Filename: wafl/inference/utils.py
 Comment: 
 
 Filename: wafl/interface/__init__.py
 Comment: 
 
 Filename: wafl/interface/base_interface.py
 Comment: 
 
 Filename: wafl/interface/command_line_interface.py
 Comment: 
 
+Filename: wafl/interface/conversation.py
+Comment: 
+
 Filename: wafl/interface/dummy_interface.py
 Comment: 
 
-Filename: wafl/interface/interface.py
+Filename: wafl/interface/list_interface.py
+Comment: 
+
+Filename: wafl/interface/queue_interface.py
 Comment: 
 
 Filename: wafl/interface/utils.py
 Comment: 
 
 Filename: wafl/interface/voice_interface.py
 Comment: 
 
 Filename: wafl/knowledge/__init__.py
 Comment: 
 
 Filename: wafl/knowledge/base_knowledge.py
 Comment: 
 
-Filename: wafl/knowledge/knowledge.py
+Filename: wafl/knowledge/single_file_knowledge.py
 Comment: 
 
 Filename: wafl/knowledge/utils.py
 Comment: 
 
 Filename: wafl/listener/__init__.py
 Comment: 
 
 Filename: wafl/listener/utils.py
 Comment: 
 
-Filename: wafl/listener/wav2vec2_listener.py
+Filename: wafl/listener/whisper_listener.py
 Comment: 
 
-Filename: wafl/listener/whisper_listener.py
+Filename: wafl/logger/base_logger.py
+Comment: 
+
+Filename: wafl/logger/history_logger.py
 Comment: 
 
-Filename: wafl/models/discourse_count_vectorizer.joblib
+Filename: wafl/logger/local_file_logger.py
 Comment: 
 
 Filename: wafl/parsing/__init__.py
 Comment: 
 
+Filename: wafl/parsing/line_rules_parser.py
+Comment: 
+
 Filename: wafl/parsing/preprocess.py
 Comment: 
 
 Filename: wafl/parsing/rules_parser.py
 Comment: 
 
 Filename: wafl/parsing/testcase_parser.py
 Comment: 
 
 Filename: wafl/parsing/utils.py
 Comment: 
 
-Filename: wafl/qa/__init__.py
+Filename: wafl/retriever/__init__.py
 Comment: 
 
-Filename: wafl/qa/common_sense.py
+Filename: wafl/retriever/base_retriever.py
 Comment: 
 
-Filename: wafl/qa/dataclasses.py
+Filename: wafl/retriever/dense_retriever.py
 Comment: 
 
-Filename: wafl/qa/entailer.py
+Filename: wafl/retriever/string_retriever.py
 Comment: 
 
-Filename: wafl/qa/qa.py
+Filename: wafl/runners/__init__.py
 Comment: 
 
-Filename: wafl/qa/utils.py
+Filename: wafl/runners/functions.py
 Comment: 
 
-Filename: wafl/retriever/__init__.py
+Filename: wafl/runners/routes.py
 Comment: 
 
-Filename: wafl/retriever/base_retriever.py
+Filename: wafl/runners/run_from_actions.py
 Comment: 
 
-Filename: wafl/retriever/dense_retriever.py
+Filename: wafl/runners/run_from_audio.py
 Comment: 
 
-Filename: wafl/retriever/string_retriever.py
+Filename: wafl/runners/run_web_and_audio_interface.py
+Comment: 
+
+Filename: wafl/runners/run_web_interface.py
+Comment: 
+
+Filename: wafl/scheduler/__init__.py
+Comment: 
+
+Filename: wafl/scheduler/conversation_handler.py
+Comment: 
+
+Filename: wafl/scheduler/conversation_loop.py
+Comment: 
+
+Filename: wafl/scheduler/generated_event_handler.py
+Comment: 
+
+Filename: wafl/scheduler/generated_event_loop.py
+Comment: 
+
+Filename: wafl/scheduler/messages_creator.py
+Comment: 
+
+Filename: wafl/scheduler/scheduler.py
+Comment: 
+
+Filename: wafl/scheduler/web_handler.py
+Comment: 
+
+Filename: wafl/scheduler/web_interface_implementation.py
+Comment: 
+
+Filename: wafl/scheduler/web_loop.py
+Comment: 
+
+Filename: wafl/simple_text_processing/__init__.py
+Comment: 
+
+Filename: wafl/simple_text_processing/deixis.py
+Comment: 
+
+Filename: wafl/simple_text_processing/normalize.py
+Comment: 
+
+Filename: wafl/simple_text_processing/questions.py
 Comment: 
 
 Filename: wafl/sounds/activation.wav
 Comment: 
 
 Filename: wafl/sounds/deactivation.wav
 Comment: 
@@ -156,44 +333,62 @@
 
 Filename: wafl/speaker/base_speaker.py
 Comment: 
 
 Filename: wafl/speaker/fairseq_speaker.py
 Comment: 
 
-Filename: wafl/speaker/festival_speaker.py
+Filename: wafl/speaker/soundfile_speaker.py
 Comment: 
 
-Filename: wafl/speaker/soundfile_speaker.py
+Filename: wafl/speaker/utils.py
 Comment: 
 
 Filename: wafl/templates/__init__.py
 Comment: 
 
+Filename: wafl/templates/actions.yaml
+Comment: 
+
 Filename: wafl/templates/config.json
 Comment: 
 
+Filename: wafl/templates/db.json
+Comment: 
+
 Filename: wafl/templates/functions.py
 Comment: 
 
-Filename: wafl/templates/rules.wafl
+Filename: wafl/templates/main.py
+Comment: 
+
+Filename: wafl/templates/requirements.txt
+Comment: 
+
+Filename: wafl/templates/rules.yaml
 Comment: 
 
-Filename: wafl/templates/server.py
+Filename: wafl/templates/secrets.json
+Comment: 
+
+Filename: wafl/templates/start_llm.sh
 Comment: 
 
 Filename: wafl/templates/testcases.txt
 Comment: 
 
-Filename: wafl-0.0.9.dist-info/METADATA
+Filename: wafl-0.0.90.dist-info/METADATA
+Comment: 
+
+Filename: wafl-0.0.90.dist-info/WHEEL
 Comment: 
 
-Filename: wafl-0.0.9.dist-info/WHEEL
+Filename: wafl-0.0.90.dist-info/entry_points.txt
 Comment: 
 
-Filename: wafl-0.0.9.dist-info/top_level.txt
+Filename: wafl-0.0.90.dist-info/top_level.txt
 Comment: 
 
-Filename: wafl-0.0.9.dist-info/RECORD
+Filename: wafl-0.0.90.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wafl/__main__.py

```diff
@@ -1,35 +1,4 @@
-import sys
-
-from wafl.config import create_initial_files
-from wafl.parsing.preprocess import remove_preprocessed
-from wafl.run import run_from_command_line, run_from_audio, run_testcases
-
-
-def download_models():
-    import nltk
-
-    nltk.download("averaged_perceptron_tagger")
-
+from wafl.command_line import main
 
 if __name__ == "__main__":
-    print("WAFL v0\n")
-
-    arguments = sys.argv
-    if len(arguments) > 1:
-        command = arguments[1]
-
-        if command == "init":
-            create_initial_files()
-            download_models()
-
-        if command == "run":
-            run_from_command_line()
-            remove_preprocessed("functions")
-
-        if command == "run-audio":
-            run_from_audio()
-            remove_preprocessed("functions")
-
-        if command == "test":
-            run_testcases()
-            remove_preprocessed("functions")
+    main()
```

## wafl/config.py

```diff
@@ -1,38 +1,21 @@
 import json
 import os
+import shutil
 
 _path = os.path.dirname(__file__)
 
 
 def create_initial_files():
-    _rules_template = open(os.path.join(_path, "templates/rules.wafl"))
-    _server_template = open(os.path.join(_path, "templates/server.py"))
-    _functions_template = open(os.path.join(_path, "templates/functions.py"))
-    _config_template = open(os.path.join(_path, "templates/config.json"))
-    _testcases_template = open(os.path.join(_path, "templates/testcases.txt"))
-
+    _sample_project_dir = os.path.join(_path, "templates/")
     print("+ Initializing ... ", end="")
+    shutil.copytree(_sample_project_dir, "./", dirs_exist_ok=True)
 
-    with open("rules.wafl", "w") as file:
-        file.write(_rules_template.read())
-
-    with open("server.py", "w") as file:
-        file.write(_server_template.read())
-
-    with open("functions.py", "w") as file:
-        file.write(_functions_template.read())
-
-    with open("config.json", "w") as file:
-        file.write(_config_template.read())
-
-    with open("testcases.txt", "w") as file:
-        file.write(_testcases_template.read())
-
-    os.mkdir("logs/")
+    if not os.path.exists("logs/"):
+        os.mkdir("logs/")
 
     print("Done.")
 
 
 class Configuration:
     def __init__(self, filename):
         with open(filename) as file:
@@ -58,7 +41,18 @@
             return cls("config.json")
 
         except FileNotFoundError:
             print(
                 "Cannot load 'config.json'. Does the file exist in the execution path?"
             )
             exit(0)
+
+    @classmethod
+    def load_from_filename(cls, filename):
+        try:
+            return cls(filename)
+
+        except FileNotFoundError:
+            print(
+                f"Cannot load '{filename}'. Does the file exist in the execution path?"
+            )
+            exit(0)
```

## wafl/facts.py

```diff
@@ -1,13 +1,14 @@
 from dataclasses import dataclass
+from typing import Union
 
 
 @dataclass
 class Fact:
-    text: str
+    text: Union[str, dict]
     is_question: bool = False
     variable: str = None
     is_interruption: bool = False
     source: str = None
     destination: str = None
 
     def toJSON(self):
```

## wafl/rules.py

```diff
@@ -2,10 +2,54 @@
 from typing import List
 
 
 @dataclass
 class Rule:
     effect: "Fact"
     causes: List["Fact"]
+    _max_indentation = 3
+    indent_str = "  "
 
     def toJSON(self):
         return str(self)
+
+    def get_string_using_template(self, effect_template: str) -> str:
+        rule_str = effect_template.replace("{effect}", self.effect.text)
+        rule_str = rule_str.replace("{clauses}", self._get_clauses())
+        return rule_str
+
+    def __str__(self):
+        rule_str = self.effect.text + "\n"
+        return rule_str + self._get_clauses()
+
+    def _get_clauses(self) -> str:
+        rule_str = ""
+        for cause in self.causes:
+            try:
+                rule_str += self._recursively_add_clauses(cause)
+
+            except TypeError as e:
+                print(f"Error in rule:'''\n{rule_str}'''")
+                print("Perhaps the YAML file is not well formatted.")
+                print()
+                raise e
+
+        return rule_str[:-1]
+
+    def _recursively_add_clauses(self, query: str, depth: int = 1) -> str:
+        indentation = self.indent_str * depth
+        if type(query) == str:
+            return f"{indentation}- {query}\n"
+
+        if type(query.text) == str:
+            return f"{indentation}- {query.text}\n"
+
+        if depth > self._max_indentation:
+            return ""
+
+        clause = list(query.text.keys())[0]
+        rules_text = f"{indentation}- {clause}\n"
+        for clauses in query.text.values():
+            for cause_index, clause in enumerate(clauses):
+                rules_text += self._recursively_add_clauses(clause, depth + 1)
+
+        return rules_text
```

## wafl/run.py

```diff
@@ -1,85 +1,54 @@
+import asyncio
+
 from wafl.config import Configuration
 from wafl.exceptions import CloseConversation
-from wafl.conversation.conversation import Conversation
+from wafl.events.conversation_events import ConversationEvents
 from wafl.interface.command_line_interface import CommandLineInterface
-from wafl.interface.voice_interface import VoiceInterface
 from wafl.logger.local_file_logger import LocalFileLogger
-from wafl.knowledge.knowledge import Knowledge
 from wafl.testcases import ConversationTestCases
+from wafl.variables import get_variables
+
+_logger = LocalFileLogger()
 
-_logger = LocalFileLogger(__file__)
+
+def print_incipit():
+    print()
+    print(f"Running WAFL version {get_variables()['version']}.")
+    print()
 
 
 def run_from_command_line():
-    wafl_rules = open("rules.wafl").read()
     interface = CommandLineInterface()
-    conversation = Conversation(
-        Knowledge(wafl_rules, logger=_logger),
+    config = Configuration.load_local_config()
+    conversation_events = ConversationEvents(
+        config=config,
         interface=interface,
-        code_path="functions",
         logger=_logger,
     )
-    conversation.output("Hello. How may I help you?")
+    asyncio.run(interface.output("Hello. How may I help you?"))
 
     while True:
         try:
-            conversation.input()
+            asyncio.run(conversation_events.process_next())
         except (CloseConversation, KeyboardInterrupt, EOFError):
             break
 
-    conversation.output("Goodbye!")
+    asyncio.run(interface.output("Goodbye!"))
 
 
-def run_from_audio():
+def run_testcases():
+    print("Running the testcases in testcases.txt\n")
     config = Configuration.load_local_config()
-    knowledge = Knowledge(open("rules.wafl").read(), logger=_logger)
-    interface = VoiceInterface(config)
-    interface.check_understanding(False)
-    conversation = Conversation(
-        knowledge,
-        interface=interface,
-        code_path="functions",
-        config=config,
+    test_cases_text = open("testcases.txt").read()
+    testcases = ConversationTestCases(
+        config,
+        test_cases_text,
         logger=_logger,
     )
-    conversation.output("Please say 'Computer' to activate me")
-
-    activation_word = "computer"
-    interface.add_hotwords(activation_word)
-    max_misses = 3
-    while True:
-        try:
-            result = conversation.input(activation_word=activation_word)
-            num_misses = 0
-            _logger.write(f"Conversation Result {result}", log_level=_logger.level.INFO)
-
-            if result:
-                interface.check_understanding(True)
-
-            if (
-                interface.check_understanding()
-                and not result
-                and not interface.bot_has_spoken()
-            ):
-                interface.play_deny_sound()
-                num_misses += 1
-                if num_misses >= max_misses:
-                    interface.check_understanding(False)
-
-        except CloseConversation:
-            _logger.write(f"Closing the conversation", log_level=_logger.level.INFO)
-            activation_word = "computer"
-            interface.check_understanding(False)
-            continue
+    asyncio.run(testcases.run())
 
-        except (KeyboardInterrupt, EOFError):
-            break
-
-    conversation.output("Good bye!")
 
+def download_models():
+    import nltk
 
-def run_testcases():
-    knowledge = Knowledge(open("rules.wafl").read())
-    test_cases_text = open("testcases.txt").read()
-    testcases = ConversationTestCases(test_cases_text, knowledge)
-    testcases.run()
+    nltk.download("averaged_perceptron_tagger")
```

## wafl/testcases.py

```diff
@@ -1,54 +1,91 @@
+from wafl.answerer.entailer import Entailer
+from wafl.simple_text_processing.deixis import from_user_to_bot, from_bot_to_user
 from wafl.exceptions import CloseConversation
-
-from wafl.conversation.conversation import Conversation
+from wafl.events.conversation_events import ConversationEvents
 from wafl.interface.dummy_interface import DummyInterface
-
 from wafl.parsing.testcase_parser import get_user_and_bot_lines_from_text
 
 
 class ConversationTestCases:
-    def __init__(self, text, knowledge):
+    BLUE_COLOR_START = "\033[94m"
+    RED_COLOR_START = "\033[31m"
+    GREEN_COLOR_START = "\033[32m"
+    COLOR_END = "\033[0m"
+
+    def __init__(self, config, text, logger=None):
+        self._config = config
         self._testcase_data = get_user_and_bot_lines_from_text(text)
-        self._knowledge = knowledge
+        self._entailer = Entailer(config)
 
-    def test_single_case(self, name):
+    async def test_single_case(self, name):
         if name not in self._testcase_data:
             raise RuntimeWarning(f"The testcase '{name}' does not exist")
 
         user_lines = self._testcase_data[name]["user_lines"]
-        bot_lines = self._testcase_data[name]["bot_lines"]
+        test_lines = self._testcase_data[name]["lines"]
         is_negated = self._testcase_data[name]["negated"]
         interface = DummyInterface(user_lines)
-        conversation = Conversation(
-            self._knowledge, interface=interface, code_path="functions"
-        )
+        conversation_events = ConversationEvents(self._config, interface=interface)
+        await conversation_events._knowledge._initialize_retrievers()
 
-        print(f"Running test '{name}'...", end="")
-
-        while True:
+        print(self.BLUE_COLOR_START + f"\nRunning test '{name}'." + self.COLOR_END)
+        continue_conversations = True
+        while continue_conversations:
             try:
-                conversation.input()
+                continue_conversations = await conversation_events.process_next()
 
             except (IndexError, CloseConversation):
                 break
 
-        if (bot_lines == interface.utterances and not is_negated) or (
-            bot_lines != interface.utterances and is_negated
-        ):
-            print(" [Success]")
+        is_consistent = True
+        generated_lines = interface.get_utterances_list()
+        prior_dialogue = []
+        for test_line, generated_line in zip(test_lines, generated_lines):
+            if not await self._lhs_is_similar_to(
+                generated_line, test_line, prior_dialogue
+            ):
+                print(f" [test_line] {test_line}")
+                print(f" [predicted_line] {generated_line}")
+                is_consistent = False
+                break
+
+            prior_dialogue.append(generated_line)
+
+        if (is_consistent and not is_negated) or (not is_consistent and is_negated):
+            print(self.GREEN_COLOR_START + " [Success]\n\n" + self.COLOR_END)
             return True
 
-        print(" [Fail]")
-        print("This is how the dialogue went:")
-        print(interface.get_dialogue())
+        print(self.RED_COLOR_START + " [Fail]\n\n" + self.COLOR_END)
+        print("\n This is how the dialogue went:")
+        for line in interface.get_utterances_list():
+            print(" " + line)
+
         return False
 
-    def run(self):
+    async def run(self):
         to_return = True
-
         for name in self._testcase_data:
-            result = self.test_single_case(name)
+            result = await self.test_single_case(name)
             if not result:
                 to_return = False
 
         return to_return
+
+    async def _lhs_is_similar_to(self, lhs, rhs, prior_dialogue):
+        lhs_name = lhs.split(":")[0].strip()
+        rhs_name = rhs.split(":")[0].strip()
+        if lhs_name != rhs_name:
+            return False
+
+        return await self._entailer.left_entails_right(
+            lhs, rhs, "\n".join(prior_dialogue)
+        )
+
+    def _apply_deixis(self, line):
+        name = line.split(":")[0].strip()
+
+        if name.lower() == "user":
+            return from_user_to_bot(line)
+
+        if name.lower() == "bot":
+            return from_bot_to_user(line)
```

## wafl/inference/utils.py

```diff
@@ -1,179 +1,348 @@
 import re
 
-from typing import List
+from typing import List, Dict, Tuple, Any
 from fuzzywuzzy import process
-from wafl.qa.dataclasses import Answer
+from wafl.extractors.dataclasses import Answer
+from wafl.simple_text_processing.normalize import normalized
+from wafl.simple_text_processing.questions import is_question
 
 
-def cause_is_negated(cause_text):
+def cause_is_negated(cause_text: str) -> bool:
     return cause_text.find("!") == 0
 
 
-def check_negation(cause_text):
+def check_negation(cause_text: str) -> Tuple[str, bool]:
     invert_results = False
     if cause_is_negated(cause_text):
         if cause_text[0] == "!":
             invert_results = True
             cause_text = cause_text[1:]
 
     return cause_text, invert_results
 
 
-def text_is_code(text):
+def text_is_code(text: str) -> bool:
     if "(" in text:
         return True
 
     return False
 
 
-def _make_safe(text):
+def _make_safe(text: str) -> str:
     text = str(text)
     text = text.replace('"', "'")
     text = text.replace("''", "'")
     text = text.replace('""', '"')
+    text = text.replace(r"\"", '\\"')
+    text = text.replace(r"\'", "\\'")
     return text
 
 
-def apply_substitutions(cause_text, substitutions):
+def apply_substitutions(cause_text: str, substitutions: Dict[str, str]) -> str:
     if text_is_code(cause_text):
         cause_text = cause_text.replace(" ", "")
 
     for key, value in substitutions.items():
         safe_value = _make_safe(str(value))
         cause_text = cause_text.replace(key, safe_value)
 
     return cause_text
 
 
-def text_has_say_command(text):
+def text_has_say_command(text: str) -> bool:
     words = text.strip().split()
     if words:
         return words[0].lower() == "say"
 
     return False
 
 
-def text_has_remember_command(text):
+def text_has_retrieve_command(text: str) -> bool:
+    words = text.split("=")[-1].strip().split()
+    if words:
+        return words[0].lower() == "retrieve"
+
+    return False
+
+
+def text_has_remember_command(text: str) -> bool:
     return normalized(text).find("remember") == 0
 
 
-def text_has_new_working_memory_command(text):
+def text_has_new_task_memory_command(text: str) -> bool:
     return normalized(text).find("erase memory") == 0
 
 
-def update_substitutions_from_answer(answer, substitutions):
+def update_substitutions_from_answer(answer: "Answer", substitutions: Dict[str, str]):
     safe_value = _make_safe(answer.text)
+    substitutions[f"({{{answer.variable.strip()}}})"] = f'("{safe_value}")'
+    substitutions[f"({{{answer.variable.strip()}}},"] = f'("{safe_value}",'
+    substitutions[f",{{{answer.variable.strip()}}},"] = f',"{safe_value}",'
+    substitutions[f",{{{answer.variable.strip()}}})"] = f',"{safe_value}")'
     substitutions[f"{{{answer.variable.strip()}}}"] = safe_value
     substitutions[f"({answer.variable.strip()})"] = f'("{safe_value}")'
     substitutions[f"({answer.variable.strip()},"] = f'("{safe_value}",'
     substitutions[f",{answer.variable.strip()},"] = f',"{safe_value}",'
     substitutions[f",{answer.variable.strip()})"] = f',"{safe_value}")'
 
 
 def add_function_arguments(text: str) -> str:
     text = re.sub(
-        "(.*\([\"'0-9a-zA-Z@?':\-\.,\s]+)\)$", "\\1, self, working_memory)", text
+        "(.*\([\"'0-9a-zA-Z@?':\-_\.,\s]+)\)$", "\\1, self, policy, task_memory)", text
     )
-    text = re.sub("(.*)\(\)$", "\\1(self, working_memory)", text)
+    text = re.sub("(.*)\(\)$", "\\1(self, policy, task_memory)", text)
     return text
 
 
-def update_substitutions_from_results(result, variable, substitutions):
+def update_substitutions_from_results(
+    result: str, variable: str, substitutions: Dict[str, str]
+):
     safe_value = _make_safe(result)
+    substitutions.update({f"({{{variable}}})": f'("{safe_value}")'})
+    substitutions.update({f"({{{variable}}},": f'("{safe_value}",'})
+    substitutions.update({f",{{{variable}}},": f',"{safe_value}",'})
+    substitutions.update({f",{{{variable}}})": f',"{safe_value}")'})
     substitutions.update({f"{{{variable}}}": safe_value})
     substitutions.update({f"({variable})": f'("{safe_value}")'})
     substitutions.update({f"({variable},": f'("{safe_value}",'})
     substitutions.update({f",{variable},": f',"{safe_value}",'})
     substitutions.update({f",{variable})": f',"{safe_value}")'})
 
 
-def invert_answer(answer):
+def invert_answer(answer: "Answer") -> "Answer":
     if answer.text == "False":
         return Answer(text="True")
 
     if answer.text == "True":
         return Answer(text="False")
 
+    if answer.text == "No":
+        return Answer(text="Yes")
+
+    if answer.text == "Yes":
+        return Answer(text="No")
+
     return answer
 
 
-def text_has_assigmnent(cause_text):
+def text_has_assigmnent(cause_text: str) -> bool:
     return "=" in cause_text
 
 
-def process_unknown_answer(answer):
+def process_unknown_answer(answer: "Answer") -> bool:
     if normalized(answer.text) == "unknown":
         answer = None
 
     return answer
 
 
-def normalized(text, lower_case=True):
-    text = text.strip()
-    if not text:
-        return ""
-
-    if text[-1] == ".":
-        text = text[:-1]
-
-    if lower_case:
-        text = text.lower()
-
-    return text.strip()
-
-
-def cluster_facts(facts_and_threshold):
+def cluster_facts(facts_and_threshold: List[Tuple["Fact", float]]) -> List[str]:
     if not facts_and_threshold:
         return []
 
     _cluster_margin = 0.1
 
     texts = []
     last_threshold = facts_and_threshold[0][1]
     text = ""
+    prior_facts = set()
     for fact, threshold in facts_and_threshold:
         if not fact.text:
             continue
 
+        if fact.text in prior_facts:
+            continue
+
+        prior_facts.add(fact.text)
+
         if abs(threshold - last_threshold) < _cluster_margin:
-            text += normalized(fact.text, lower_case=False) + ". "
+            text += normalized(fact.text, lower_case=False).capitalize() + ". "
 
         else:
             texts.append(text.strip())
             text = ""
             last_threshold = threshold
 
     if text:
         texts.append(text.strip())
 
     return texts
 
 
-def selected_answer(candidate_answers):
+def selected_answer(candidate_answers: List["Answer"], variable_name: str) -> bool:
     for answer in candidate_answers:
         if answer and normalized(answer.text) != "unknown":
             return answer
 
     for answer in candidate_answers:
         if answer:
             return answer
 
-    return Answer(text="False")
+    return_answer = Answer.create_neutral()
+    return_answer.variable = variable_name
+    return return_answer
 
 
-def fact_relates_to_user(text):
+def fact_relates_to_user(text: str) -> bool:
     if "the user" in normalized(text):
         return True
 
     return False
 
 
-def project_answer(answer: "Answer", candidates: List) -> "Answer":
-    if not candidates:
+def project_answer(answer: "Answer", candidates: List[str]) -> "Answer":
+    if not candidates or not answer_is_informative(answer):
         return Answer(text="unknown")
 
     extracted, score = process.extract(answer.text, candidates, limit=1)[0]
     if score < 60:
         return Answer(text="unknown")
 
     return Answer(text=extracted)
+
+
+def answer_is_informative(answer: "Answer") -> bool:
+    return not any(item == normalized(answer.text) for item in ["unknown"])
+
+
+def is_inference_task(text):
+    text = text.split("=")[-1]
+    prompt = "the user"
+    if text.strip().lower().find(prompt) == 0:
+        return True
+
+    return False
+
+
+async def text_is_text_generation_task(
+    text: str,
+    entailer: "Entailer",
+) -> bool:
+    if not "=" in text:
+        return False
+
+    if text_is_code(text):
+        return False
+
+    if is_inference_task(text):
+        return False
+
+    if is_question(text.split("=")[1]):
+        return False
+
+    if await entailer.entails(
+        text,
+        f"An instruction or request of some kind",
+        return_threshold=True,
+        threshold=0.5,
+    ):
+        return True
+
+    return False
+
+
+def escape_characters(text: str) -> str:
+    text = text.replace("\n", "\\n")
+    return text
+
+
+def string_is_python_list(text: str) -> bool:
+    try:
+        result = eval(text)
+        if type(result) == list:
+            return True
+
+    except (SyntaxError, NameError):
+        try:
+            text = text.replace("'s", "\\'s")
+            result = eval(text)
+            if type(result) == list:
+                return True
+
+        except (SyntaxError, NameError):
+            pass
+
+        pass
+
+    return False
+
+
+def get_list_from_string(text: str) -> List[Any]:
+    try:
+        result = eval(text)
+        if type(result) == list:
+            return result
+
+    except (SyntaxError, NameError):
+        text = text.replace("'s", "\\'s")
+        result = eval(text)
+        if type(result) == list:
+            return result
+
+        pass
+
+    return []
+
+
+def get_list_like_element(text: str) -> str:
+    start_pos = text.find("[")
+    if start_pos == -1:
+        return ""
+
+    end_pos = text.find("]", start_pos)
+    if end_pos == -1:
+        return ""
+
+    return text[start_pos : end_pos + 1]
+
+
+def create_python_list_from_bullet_list(text: str) -> List[str]:
+    new_list = text.split("\n")
+    if len(new_list) != 1:
+        return new_list
+
+    new_list = text.split("', '")
+    if len(new_list) != 1:
+        return new_list
+
+    new_list = text.split(",")
+    if len(new_list) != 1:
+        return new_list
+
+    return [text]
+
+
+def get_causes_list(text: str) -> List[str]:
+    """
+    If the text contains a Python list (e.g. generate a chapter with the theme ["space", "romance"] )
+    then the output becomes a list of texts where each item appears separaterly
+    (e.g. ["generate a chapter with the theme space", generate a chapter with the theme romance"]
+
+    :param text:
+    :return: a list of causes,
+    """
+    if text_is_code(text):
+        return [text]
+
+    list_like_element = get_list_like_element(text)
+    if not list_like_element:
+        return [text]
+
+    if not string_is_python_list(list_like_element):
+        items = create_python_list_from_bullet_list(list_like_element[1:-1])
+
+    else:
+        items = get_list_from_string(list_like_element)
+
+    causes_list = []
+    for item in items:
+        causes_list.append(text.replace(list_like_element, item))
+
+    return causes_list
+
+
+def create_default_substitutions(interface: "BaseInterface") -> Dict[str, str]:
+    substitutions = {}
+    dialogue = " ".join(interface.get_utterances_list())
+    update_substitutions_from_results(dialogue, "_dialogue", substitutions)
+    return substitutions
```

## wafl/interface/base_interface.py

```diff
@@ -1,12 +1,87 @@
+import re
+import time
+from typing import List
+
+from wafl.interface.conversation import Conversation, Utterance
+
+
 class BaseInterface:
-    def output(self, text: str):
-        raise NotImplemented
+    def __init__(self, decorator=None):
+        self._is_listening = True
+        self._choices = []
+        self._facts = []
+        self._utterances = Conversation()
+        self._decorator = decorator
 
-    def input(self) -> str:
-        raise NotImplemented
+    async def output(self, text: str, silent: bool = False):
+        raise NotImplementedError
+
+    async def input(self) -> str:
+        raise NotImplementedError
 
     def bot_has_spoken(self, to_set: bool = None):
-        raise NotImplemented
+        raise NotImplementedError
+
+    async def insert_input(self, text: str):
+        pass
+
+    def is_listening(self):
+        return self._is_listening
+
+    def activate(self):
+        self._is_listening = True
+
+    def deactivate(self):
+        self._is_listening = False
+        self._choices = []
+        self._facts = []
+        self._utterances = Conversation()
+
+    async def add_choice(self, text):
+        self._choices.append((time.time(), text))
+        await self.output(f"Making the choice: {text}", silent=True)
+
+    async def add_fact(self, text):
+        self._facts.append((time.time(), text))
+        await self.output(f"{text}", silent=True)
+
+    def get_choices_and_timestamp(self):
+        return self._choices
+
+    def get_facts_and_timestamp(self):
+        return self._facts
+
+    def get_utterances_list(self) -> List[str]:
+        if not self._utterances:
+            return []
+
+        return [
+            f"{utterance.speaker}: {utterance.text}"
+            for utterance in self._utterances.utterances
+        ]
+
+    def last_speaker(self):
+        return self._utterances.get_last_n(1).utterances[0].speaker
+
+    def get_utterances_list_with_timestamp(self):
+        return self._utterances
+
+    def reset_history(self):
+        self._utterances = Conversation()
+        self._choices = []
+        self._facts = []
+
+    def add_hotwords(self, hotwords):
+        pass
+
+    def _decorate_reply(self, text: str) -> str:
+        if not self._decorator:
+            return text
+
+        return self._decorator.extract(text, self._utterances)
 
-    def check_understanding(self, do_the_check: bool):
-        raise NotImplemented
+    def _insert_utterance(self, speaker, text: str):
+        text = re.sub(r"\[.*?\]", "", text)
+        self._utterances.add_utterance(
+            Utterance(text=text, speaker=speaker, timestamp=time.time())
+        )
```

## wafl/interface/command_line_interface.py

```diff
@@ -1,35 +1,39 @@
-from wafl.deixis import from_bot_to_user, from_user_to_bot
+import time
+
+from wafl.simple_text_processing.deixis import from_bot_to_user
 from wafl.interface.base_interface import BaseInterface
 from wafl.interface.utils import not_good_enough
 
 COLOR_START = "\033[94m"
 COLOR_END = "\033[0m"
 
 
 class CommandLineInterface(BaseInterface):
     def __init__(self):
+        super().__init__()
         self._bot_has_spoken = False
-        self._check_understanding = True
 
-    def output(self, text: str):
-        print(COLOR_START + "bot> " + from_bot_to_user(text) + COLOR_END)
+    async def output(self, text: str, silent: bool = False):
+        if silent:
+            print(text)
+            return
+
+        utterance = from_bot_to_user(text)
+        print(COLOR_START + "bot> " + utterance + COLOR_END)
+        self._utterances.append((time.time(), f"bot: {text}"))
         self.bot_has_spoken(True)
 
-    def input(self) -> str:
-        text = from_user_to_bot(input("user> ")).strip()
-        while self._check_understanding and not_good_enough(text):
-            self.output("I did not quite understand that")
-            text = from_user_to_bot(input("user> "))
+    async def input(self) -> str:
+        text = input("user> ").strip()
+        while not_good_enough(text):
+            await self.output("I did not quite understand that")
+            text = input("user> ")
+
+        self._utterances.append((time.time(), f"user: {text}"))
         return text
 
     def bot_has_spoken(self, to_set: bool = None):
         if to_set != None:
             self._bot_has_spoken = to_set
 
         return self._bot_has_spoken
-
-    def check_understanding(self, do_the_check: bool = None):
-        if do_the_check == None:
-            return self._check_understanding
-
-        self._check_understanding = do_the_check
```

## wafl/interface/dummy_interface.py

```diff
@@ -1,40 +1,66 @@
-from wafl.deixis import from_bot_to_user, from_user_to_bot
+import re
+import time
+
+from wafl.interface.conversation import Utterance
+from wafl.simple_text_processing.deixis import from_bot_to_user
 from wafl.interface.base_interface import BaseInterface
 from wafl.interface.utils import not_good_enough
 
+COLOR_START = "\033[94m"
+COLOR_END = "\033[0m"
+
 
 class DummyInterface(BaseInterface):
-    def __init__(self, to_utter=None):
-        self.utterances = []
+    def __init__(self, to_utter=None, print_utterances=False):
+        super().__init__()
         self._to_utter = to_utter
         self._bot_has_spoken = False
         self._dialogue = ""
-        self._check_understanding = True
+        self._print_utterances = print_utterances
 
-    def output(self, text: str):
-        self._dialogue += "bot> " + text + "\n"
-        self.utterances.append(from_bot_to_user(text))
-        self.bot_has_spoken(True)
+    async def output(self, text: str, silent: bool = False):
+        if self._print_utterances:
+            if silent:
+                print(text)
+
+            else:
+                print(COLOR_START + "bot> " + text + COLOR_END)
+
+        if not silent:
+            self._dialogue += "bot: " + text + "\n"
+            self._insert_utterance(speaker="bot", text=text)
+            self.bot_has_spoken(True)
 
-    def input(self) -> str:
+    async def input(self) -> str:
         text = self._to_utter.pop(0).strip()
-        while self._check_understanding and not_good_enough(text):
-            self.output("I did not quite understand that")
-            text = from_user_to_bot(self._to_utter.pop(0))
-        self._dialogue += "user> " + text + "\n"
-        return from_user_to_bot(text)
+        text = self.__remove_activation_word_and_normalize(text)
+        if self._print_utterances:
+            print(COLOR_START + "user> " + text + COLOR_END)
+
+        while self._is_listening and not_good_enough(text):
+            await self.output("I did not quite understand that")
+            text = self._to_utter.pop(0)
+
+        self._dialogue += "user: " + text + "\n"
+        utterance = text
+        self._insert_utterance(speaker="user", text=text)
+        return utterance
 
     def bot_has_spoken(self, to_set: bool = None):
         if to_set != None:
             self._bot_has_spoken = to_set
 
         return self._bot_has_spoken
 
     def get_dialogue(self):
         return self._dialogue
 
-    def check_understanding(self, do_the_check: bool = None):
-        if do_the_check == None:
-            return self._check_understanding
-
-        self._check_understanding = do_the_check
+    def __remove_activation_word_and_normalize(self, text):
+        activation_word = re.sub(r"\[(.*)\].*", r"\1", text)
+        text = re.sub(
+            f"^\[{activation_word}\] {activation_word} (.*)",
+            r"\1",
+            text,
+            flags=re.IGNORECASE,
+        )
+        return text
```

## wafl/interface/utils.py

```diff
@@ -1,15 +1,15 @@
 from sklearn.feature_extraction.text import CountVectorizer
 from sklearn.feature_extraction.text import ENGLISH_STOP_WORDS
-from wafl.inference.utils import normalized
+from wafl.simple_text_processing.normalize import normalized
 
 
 def get_most_common_words(text, max_num_words, count_threshold=1):
     corpus = text.split("\n")
-    cv = CountVectorizer(ngram_range=[1, 2])
+    cv = CountVectorizer(ngram_range=(1, 2))
     words_count = cv.fit_transform(corpus).sum(axis=0)
     words_freq = [
         (word, words_count[0, index])
         for word, index in cv.vocabulary_.items()
         if words_count[0, index] >= count_threshold
         and word not in ENGLISH_STOP_WORDS
         and "user" not in word
@@ -19,11 +19,14 @@
     return [word for word, _ in words_freq][:max_num_words]
 
 
 def not_good_enough(text):
     if not text:
         return True
 
+    if "[unclear]" in text:
+        return True
+
     if normalized(text) != "no" and len(text.strip().replace(" ", "")) < 3:
         return True
 
     return False
```

## wafl/interface/voice_interface.py

```diff
@@ -1,112 +1,119 @@
 import os
+import random
+import re
 
-from wafl.deixis import from_bot_to_user, from_user_to_bot
+from wafl.events.utils import remove_text_between_brackets
 from wafl.interface.base_interface import BaseInterface
-from wafl.interface.utils import get_most_common_words, not_good_enough
+from wafl.interface.utils import not_good_enough
 from wafl.listener.whisper_listener import WhisperListener
 from wafl.speaker.fairseq_speaker import FairSeqSpeaker
 from wafl.speaker.soundfile_speaker import SoundFileSpeaker
 
 _path = os.path.dirname(__file__)
 
 
 COLOR_START = "\033[94m"
 COLOR_END = "\033[0m"
 
 
 class VoiceInterface(BaseInterface):
     def __init__(self, config):
+        super().__init__()
         self._sound_speaker = SoundFileSpeaker()
         self._activation_sound_filename = self.__get_activation_sound_from_config(
             config
         )
         self._deactivation_sound_filename = self.__get_deactivation_sound_from_config(
             config
         )
-        self._deny_sound_filename = self.__get_deny_sound_from_config(config)
-
-        self.listener_model_name = config.get_value("listener_model")
-        self._speaker = FairSeqSpeaker()
-        self._listener = WhisperListener(self.listener_model_name)
-        self._listener.set_timeout(0.6)
-        self._listener.set_threshold(0.9)
-        self._bot_has_spoken = False
-        self._check_understanding = True
-
-    def add_hotwords_from_knowledge(
-        self, knowledge: "Knowledge", max_num_words: int = 100, count_threshold: int = 5
-    ):
-        hotwords = get_most_common_words(
-            knowledge.get_facts_and_rule_as_text(),
-            max_num_words=max_num_words,
-            count_threshold=count_threshold,
+        self._speaker = FairSeqSpeaker(config)
+        self._listener = WhisperListener(config)
+        self._listener.set_timeout(
+            config.get_value("listener_model")["listener_silence_timeout"]
         )
-        hotwords = [word.lower() for word in hotwords]
-        self._listener.add_hotwords(hotwords)
+        self._listener.set_volume_threshold(
+            config.get_value("listener_model")["listener_volume_threshold"]
+        )
+        self._listener.set_hotword_threshold(
+            config.get_value("listener_model")["listener_hotword_logp"]
+        )
+        self._bot_has_spoken = False
+        self._utterances = []
 
     def add_hotwords(self, hotwords):
         self._listener.add_hotwords(hotwords)
 
-    def output(self, text: str):
+    async def output(self, text: str, silent: bool = False):
+        if silent:
+            print(text)
+            return
+
+        if not text:
+            return
+
         self._listener.activate()
-        text = from_bot_to_user(text)
+        text = text
+        self._insert_utterance(speaker="bot", text=text)
         print(COLOR_START + "bot> " + text + COLOR_END)
-        self._speaker.speak(text)
+        await self._speaker.speak(text)
         self.bot_has_spoken(True)
 
-    def input(self) -> str:
+    async def input(self) -> str:
         text = ""
         while not text:
-            text = self._listener.input()
-            hotword = self._listener.get_hotword_if_present()
-            print("HOTWORD", hotword)
+            text = await self._listener.input()
+            text = self.__remove_activation_word_and_normalize(text)
+            hotword = await self._listener.get_hotword_if_present()
             if hotword:
                 text = f"[{hotword}] {text}"
 
-        while self._check_understanding and not_good_enough(text):
+        while self._is_listening and not_good_enough(text):
             print(COLOR_START + "user> " + text + COLOR_END)
-            self.output("I did not quite understand that")
-            text = self._listener.input()
+            await self.output(random.choice(["Sorry?", "Can you repeat?"]))
+            text = await self._listener.input()
 
         text = text.lower().capitalize()
         print(COLOR_START + "user> " + text + COLOR_END)
-        return from_user_to_bot(text)
+        utterance = remove_text_between_brackets(text)
+        if utterance.strip():
+            self._insert_utterance(speaker="user", text=text)
+
+        return text
 
     def bot_has_spoken(self, to_set: bool = None):
         if to_set != None:
             self._bot_has_spoken = to_set
 
         return self._bot_has_spoken
 
-    def check_understanding(self, do_the_check=None):
-        if do_the_check == None:
-            return self._check_understanding
-
-        if do_the_check and not self._check_understanding:
+    def activate(self):
+        if not self._is_listening:
             self._sound_speaker.speak(self._activation_sound_filename)
+            super().activate()
 
-        if not do_the_check and self._check_understanding:
+    def deactivate(self):
+        if self._is_listening:
             self._sound_speaker.speak(self._deactivation_sound_filename)
-
-        self._check_understanding = do_the_check
-
-    def play_deny_sound(self):
-        self._sound_speaker.speak(self._deny_sound_filename)
+            super().deactivate()
 
     def __get_activation_sound_from_config(self, config):
         if config.get_value("waking_up_sound"):
             return os.path.join(_path, "../sounds/activation.wav")
 
         return None
 
     def __get_deactivation_sound_from_config(self, config):
         if config.get_value("deactivate_sound"):
             return os.path.join(_path, "../sounds/deactivation.wav")
 
         return None
 
-    def __get_deny_sound_from_config(self, config):
-        if config.get_value("deny_sound"):
-            return os.path.join(_path, "../sounds/deny.wav")
-
-        return None
+    def __remove_activation_word_and_normalize(self, text):
+        activation_word = re.sub(r"\[(.*)\].*", r"\1", text)
+        text = re.sub(
+            f"^\[{activation_word}\] {activation_word} (.*)",
+            r"\1",
+            text,
+            flags=re.IGNORECASE,
+        )
+        return text
```

## wafl/knowledge/base_knowledge.py

```diff
@@ -1,9 +1,19 @@
 class BaseKnowledge:
-    def add(self, text):
-        raise NotImplemented()
+    root_knowledge = "/"
 
-    def ask_for_facts(self, query, is_from_user=False):
-        raise NotImplemented()
+    async def add(self, text):
+        raise NotImplementedError()
 
-    def ask_for_rule_backward(self, query):
-        raise NotImplemented()
+    async def add_rule(self, rule_text):
+        raise NotImplementedError()
+
+    async def ask_for_facts(self, query, is_from_user=False):
+        raise NotImplementedError()
+
+    async def ask_for_facts_with_threshold(
+        self, query, is_from_user=False, threshold=None
+    ):
+        raise NotImplementedError()
+
+    async def ask_for_rule_backward(self, query, threshold=None):
+        raise NotImplementedError()
```

## wafl/knowledge/utils.py

```diff
@@ -1,74 +1,75 @@
+import wafl.simple_text_processing.questions
+from wafl.simple_text_processing.questions import get_sentence_from_yn_question
+
+
 def text_is_exact_string(text):
     return text.strip() and text.strip()[0] == "_"
 
 
-def rules_are_too_different(retriever, rules):
+async def rules_are_too_different(retriever, rules):
     dot_products = []
     for item in rules[1:]:
         dot_products.append(
-            retriever.get_dot_product(item.effect.text, rules[0].effect.text)
-        )
-        print(
-            "DOT PRODUCT:",
-            retriever.get_dot_product(item.effect.text, rules[0].effect.text),
+            await retriever.get_dot_product(item.effect.text, rules[0].effect.text)
         )
 
     if dot_products and min(dot_products) < 0.39:
         return False
 
+    return True
+
 
 def get_first_cluster_of_rules(rules_and_threshold):
     if not rules_and_threshold:
         return []
 
     _cluster_margin = 0.1
 
     last_threshold = rules_and_threshold[0][1]
+    prior_rules = set()
     rules = []
     for rule, threshold in rules_and_threshold:
+        if str(rule) in prior_rules:
+            continue
+
+        prior_rules.add(str(rule))
         if abs(threshold - last_threshold) < _cluster_margin:
             rules.append(rule)
 
         else:
             break
 
     return rules
 
 
-def filter_out_rules_that_are_too_dissimilar_to_query(query, rules_and_scores):
-    num_query_words = len(query.text.split())
+async def filter_out_rules_through_entailment(entailer, query, rules_and_scores):
     new_rules_and_scores = []
-    for item in rules_and_scores:
-        rule = item[0]
-        num_rule_effect_words = len(rule.effect.text.split())
-        if num_query_words < num_rule_effect_words / 3:
-            continue
-
-        new_rules_and_scores.append(item)
-
-    return new_rules_and_scores
-
-
-def filter_out_rules_through_entailment(entailer, query, rules_and_scores):
-    new_rules_and_scores = []
-    for item in rules_and_scores:
-        rule = item[0]
+    for rule, score in rules_and_scores:
         if rule.effect.is_question:
-            new_rules_and_scores.append(item)
-            continue
+            new_rules_and_scores.append((rule, score))
 
-        if needs_substitutions(rule.effect):
-            new_rules_and_scores.append(item)
-            continue
+        elif needs_substitutions(rule.effect):
+            new_rules_and_scores.append((rule, score))
 
-        if entailer.entails(query.text, rule.effect.text) == "True":
-            new_rules_and_scores.append(item)
+        else:
+            entailment_score = await entailer.entails(
+                query.text, rule.effect.text, return_threshold=True
+            )
+            if entailment_score:
+                new_rules_and_scores.append((rule, score * entailment_score))
+                continue
+
+            entailment_score = await entailer.entails(
+                rule.effect.text, query.text, return_threshold=True
+            )
+            if entailment_score:
+                new_rules_and_scores.append((rule, score * entailment_score))
 
-    return new_rules_and_scores
+    return sorted(new_rules_and_scores, key=lambda x: -x[1])
 
 
 def needs_substitutions(effect):
     if any(item in effect.text for item in ["{", "}"]):
         return True
 
     return False
```

## wafl/listener/whisper_listener.py

```diff
@@ -1,33 +1,35 @@
+import asyncio
+import math
+
 import pyaudio
 import time
 import numpy as np
-import torch.cuda
-
-from transformers import WhisperProcessor, WhisperForConditionalGeneration
 
-device = "cuda" if torch.cuda.is_available() else "cpu"
+from wafl.connectors.factories.whisper_connector_factory import WhisperConnectorFactory
 
 
 class WhisperListener:
     _chunk = 1024
     _format = pyaudio.paInt16
     _channels = 1
     _rate = 16000
     _range = 32768
+    _generation_max_length = 15
+    _starting_tokens = [50257, 50362]
+    _ending_tokens = [50256]
 
-    def __init__(self, model_name):
+    def __init__(self, config):
         self._p = pyaudio.PyAudio()
-        self._threshold = 1
+        self._volume_threshold = 1
+        self._original_volume_threshold = self._volume_threshold
         self._timeout = 1
         self._max_timeout = 4
-        self._model = WhisperForConditionalGeneration.from_pretrained(model_name).to(
-            device
-        )
-        self._processor = WhisperProcessor.from_pretrained(model_name)
+        self._hotword_threshold = -8
+        self._connector = WhisperConnectorFactory.get_connector(config)
         self._hotwords = list()
         self.is_active = False
         self._last_waveform = None
 
     def set_hotwords(self, hotwords):
         self._hotwords = [item.lower() for item in hotwords]
 
@@ -36,28 +38,32 @@
             hotwords = [hotwords]
 
         self._hotwords.extend([item.lower() for item in hotwords])
 
     def set_timeout(self, timeout):
         self._timeout = timeout
 
-    def set_threshold(self, threshold):
-        self._threshold = threshold
+    def set_volume_threshold(self, threshold):
+        self._volume_threshold = threshold
+        self._original_volume_threshold = self._volume_threshold
+
+    def set_hotword_threshold(self, threshold):
+        self._hotword_threshold = threshold
 
     def record(self, start_with):
         rec = list()
         rec.append(start_with)
 
         current = time.time()
         end = time.time() + self._timeout
         upper_limit_end = time.time() + self._max_timeout
 
         while current <= end and current < upper_limit_end:
             data = self.stream.read(self._chunk)
-            if _rms(data) >= self._threshold:
+            if _rms(data) >= self._volume_threshold:
                 end = time.time() + self._timeout
 
             current = time.time()
             rec.append(data)
 
         return np.frombuffer(b"".join(rec), dtype=np.int16) / self._range
 
@@ -75,76 +81,61 @@
 
     def deactivate(self):
         if self.is_active:
             self.stream.stop_stream()
             self.stream.close()
             self.is_active = False
 
-    def input(self):
+    async def input(self):
         if not self.is_active:
             self.activate()
 
         while True:
-            inp = self.stream.read(self._chunk)
+            await asyncio.sleep(0)
+            try:
+                inp = self.stream.read(self._chunk)
+            except IOError:
+                self.activate()
+                inp = self.stream.read(self._chunk)
+
             rms_val = _rms(inp)
-            if rms_val > self._threshold:
+            if rms_val > self._volume_threshold:
                 waveform = self.record(start_with=inp)
-                return self.input_waveform(waveform)
+                self.deactivate()
+                return await self.input_waveform(waveform)
 
-    def input_waveform(self, waveform):
+            else:
+                new_threshold = 2 * rms_val
+                self._volume_threshold = max(
+                    new_threshold, self._original_volume_threshold
+                )
+
+    async def input_waveform(self, waveform):
         self._last_waveform = waveform
-        input_features = self._processor(waveform, return_tensors="pt").input_features
-        output = self._model.generate(
-            input_features.to(device),
-            num_beams=2,
-            return_dict_in_generate=True,
-            output_scores=True,
-        )
-        transcription = self._processor.batch_decode(
-            output.sequences, skip_special_tokens=True
-        )[0]
+        prediction = await self._connector.predict(waveform)
+        transcription = prediction["transcription"]
+        score = prediction["score"]
 
-        if torch.exp(output.sequences_scores) > 0.6:
-            self.deactivate()
+        if math.exp(score) > 0.5:
             return transcription
 
-        return ""
+        return "[unclear]"
 
-    def get_hotword_if_present(self):
+    async def get_hotword_if_present(self):
         for hotword in self._hotwords:
-            if self.hotword_is_present(hotword):
+            if await self.hotword_is_present(hotword):
                 return hotword
 
         return ""
 
-    def hotword_is_present(self, hotword):
+    async def hotword_is_present(self, hotword):
         if type(self._last_waveform) != np.ndarray:
             raise RuntimeError(
                 "The waveform has not been processed. Please call input_waveform() before hotword_is_present()"
             )
-
-        input_features = self._processor(
-            self._last_waveform, return_tensors="pt"
-        ).input_features
-        hotword_tokens = torch.tensor([self._processor.tokenizer.encode(f" {hotword}")])
-        starting_tokens = [50257, 50362]
-        input_ids = torch.tensor([starting_tokens]).to(device)
-        for _ in range(hotword_tokens.shape[1]):
-            logits = self._model(
-                input_features.to(device),
-                decoder_input_ids=input_ids,
-            ).logits
-            new_token = torch.argmax(logits, dim=-1)
-            new_token = torch.tensor([[new_token[:, -1]]]).to(device)
-            input_ids = torch.cat([input_ids, new_token], dim=-1)
-
-        logprobs = torch.log(torch.softmax(logits, dim=-1))
-        sum_logp = 0
-        for logp, index in zip(logprobs[0][1:], hotword_tokens[0]):
-            sum_logp += logp[index]
-
-        return sum_logp > -8
+        prediction = await self._connector.predict(self._last_waveform, hotword=hotword)
+        return prediction["logp"] > self._hotword_threshold
 
 
 def _rms(frame):
     data = np.frombuffer(frame, dtype=np.int16)
     return np.std(data) / len(data)
```

## wafl/parsing/preprocess.py

```diff
@@ -1,45 +1,104 @@
+import functools
 import importlib
 import os
 import re
 from inspect import getmembers, isfunction
 
-preprocessed_prefix = "__wafl_"
+_preprocessed_prefix = "__wafl_"
+_functions_standard_name = "functions"
+_python_functions_standard_name = _functions_standard_name + ".py"
 
 
 def get_all_functions_names(module_name):
     module = importlib.import_module(module_name)
     functions = [item[0] for item in getmembers(module, isfunction)]
     return functions
 
 
-def create_preprocessed(module: str):
-    function_names = get_all_functions_names(module)
-    filename = module + ".py"  ### TODO: This is not enough in general
+def clean_module_name(module_name):
+    if not module_name:
+        raise RuntimeError(
+            f"The name {module_name} is empty and cannot be used as a python module"
+        )
+
+    names = module_name.split("/")
+    return_path = []
+    for name in names:
+        if name and name != "." and name != "..":
+            return_path.append(name)
+
+        if name == "..":
+            return_path.pop()
+
+    if not return_path:
+        return ""
+
+    return_path = ".".join(return_path) + "."
+    return return_path
+
+
+@functools.lru_cache
+def create_preprocessed(
+    module: str,
+    functions_standard_name=_functions_standard_name,
+    python_functions_standard_name=_python_functions_standard_name,
+):
+    function_names = get_all_functions_names(
+        clean_module_name(module) + functions_standard_name
+    )
+    filename = "." + module + "/" + python_functions_standard_name
     with open(filename) as file:
         print(f"Preprocessing {filename}.")
         text = file.read()
-        text = text.replace('{f"%', 'inference.get_inference_answer(f"')
-        text = text.replace('{"%', 'inference.get_inference_answer(f"')
-        text = text.replace('%"}', '", working_memory)')
-
+        text = re.sub(
+            r'f?"%(.*)%"',
+            'await inference.get_inference_answer(f"\\1", policy, task_memory)',
+            text,
+        )
         for name in function_names:
             text = re.sub(
-                f"({name}\([0-9a-zA-Z,\s:]+)\)",
-                "\\1, inference, working_memory)",
+                f" ({name}\([0-9a-zA-Z,\s:_]+)\)",
+                " \\1, inference, policy, task_memory)",
                 text,
             )
-            text = re.sub(f"({name})\(\)", "\\1(inference, working_memory)", text)
+            text = re.sub(
+                f" ({name})\(\)", " \\1(inference, policy, task_memory)", text
+            )
+            text = re.sub(
+                f"(def {name}\()",
+                "async \\1",
+                text,
+            )
+            text = re.sub(f" ({name})\(", " await \\1(", text)
+            text = re.sub(f'"[\s]*await ({name})\(', '"\\1(', text)
+
+        text = text.replace("def await", "def")
 
-    with open(preprocessed_prefix + filename, "w") as file:
+    preprocessed_filename = filename.replace(
+        _python_functions_standard_name,
+        _preprocessed_prefix + _python_functions_standard_name,
+    )
+    with open(preprocessed_filename, "w") as file:
         file.write(text)
 
 
-def import_module(module_name):
-    return importlib.import_module(f"{preprocessed_prefix + module_name}")
+def import_module(
+    module_name,
+    preprocessed_prefix=_preprocessed_prefix,
+    functions_standard_name=_functions_standard_name,
+):
+    module_name = (
+        clean_module_name(module_name) + preprocessed_prefix + functions_standard_name
+    )
+    return importlib.import_module(module_name)
 
 
-def remove_preprocessed(module):
+def remove_preprocessed(
+    module, python_functions_standard_name=_python_functions_standard_name
+):
     print("Removing preprocessed files")
-    filename = module + ".py"
+    filename = (
+        "." + module + "/" + _preprocessed_prefix + python_functions_standard_name
+    )
     if os.path.isfile(filename):
-        os.remove(preprocessed_prefix + filename)
+        os.remove(filename)
```

## wafl/parsing/rules_parser.py

```diff
@@ -1,72 +1,30 @@
-from wafl.conversation.utils import is_question
+import yaml
+
 from wafl.facts import Fact
-from wafl.parsing.utils import (
-    get_lines_stripped_from_comments,
-    is_quoted_text,
-    text_has_interruption,
-    clean_text,
-)
 from wafl.rules import Rule
+from wafl.simple_text_processing.deixis import from_user_to_bot
 
 
 def get_facts_and_rules_from_text(text: str):
-    lines = get_lines_stripped_from_comments(text)
-    lines.extend(["LAST"])
+    parsed_text_dict = yaml.safe_load(text)
+    fact_strings = parsed_text_dict.get("facts", [])
+    rules_list = parsed_text_dict.get("rules", {})
 
     facts = []
-    rules = []
-
-    rule_length = 0
-    current_fact = ""
-    causes = []
-    for line in lines:
-        separation = line.find(line.strip())
-        if separation > 0:
-            rule_length += 1
-            text = line.strip()
-            causes.append(
-                Fact(
-                    text=text,
-                    is_question=is_question(text),
-                )
+    for text in fact_strings:
+        facts.append(
+            Fact(
+                text=from_user_to_bot(text),
             )
+        )
 
-        else:
-            text = line.strip()
-            if not text:
-                continue
-
-            if current_fact:
-                if rule_length == 0:
-                    facts.append(current_fact)
-
-                else:
-                    rules.append(Rule(effect=current_fact, causes=causes))
-
-                causes = []
-                rule_length = 0
-
-            if "=" in text:
-                sentence_is_question = True
-                variable, text = text.split("=")
-                text = text.strip()
-                variable = variable.strip()
-
-            else:
-                sentence_is_question = False
-                variable = None
-                if is_quoted_text(text):
-                    text = "The user says: " + text
-
-            is_interruption = text_has_interruption(text)
-            if is_interruption:
-                text = clean_text(text)
-
-            current_fact = Fact(
-                text=text,
-                is_question=sentence_is_question,
-                variable=variable,
-                is_interruption=is_interruption,
+    rules = []
+    for rule_dict in rules_list:
+        rules.append(
+            Rule(
+                effect=Fact(text=list(rule_dict.keys())[0]),
+                causes=[Fact(item) for item in list(rule_dict.values())[0]],
             )
+        )
 
     return {"facts": facts, "rules": rules}
```

## wafl/parsing/testcase_parser.py

```diff
@@ -1,57 +1,63 @@
 from wafl.parsing.utils import get_lines_stripped_from_comments
 
-_user_prompt = "user> "
-_bot_prompt = "bot> "
+_user_prompt = "user:"
+_bot_prompt = "bot:"
 
 
 def get_user_and_bot_lines_from_text(text: str):
     lines = get_lines_stripped_from_comments(text)
 
     testcase_name = ""
     testcases = {}
     to_negate = False
     bot_lines = []
     user_lines = []
+    all_lines = []
 
     for line in lines:
         if not line.strip():
             continue
 
         separation = line.find(line.strip())
         if separation == 0:
             if user_lines or bot_lines:
                 testcases[testcase_name] = {
                     "bot_lines": bot_lines,
                     "user_lines": user_lines,
+                    "lines": all_lines,
                     "negated": to_negate,
                 }
                 to_negate = False
                 bot_lines = []
                 user_lines = []
+                all_lines = []
 
             line = line.strip()
             if line.find("!") == 0:
                 to_negate = True
                 line = line[1:].strip()
 
             testcase_name = line
             testcases[testcase_name] = {}
             continue
 
         line = line.strip()
+        all_lines.append(line)
+
         if line.find(_user_prompt) == 0:
-            user_lines.append(line[len(_user_prompt) :])
+            user_lines.append(line[len(_user_prompt) :].strip())
             continue
 
         if line.find(_bot_prompt) == 0:
-            bot_lines.append(line[len(_bot_prompt) :])
+            bot_lines.append(line[len(_bot_prompt) :].strip())
             continue
 
     if user_lines or bot_lines:
         testcases[testcase_name] = {
             "bot_lines": bot_lines,
             "user_lines": user_lines,
+            "lines": all_lines,
             "negated": to_negate,
         }
 
     return testcases
```

## wafl/parsing/utils.py

```diff
@@ -30,7 +30,12 @@
         return True
 
     return False
 
 
 def clean_text(text):
     return text.replace("INTERRUPTION ", "")
+
+
+def concatenate_slashes_into_one_single_line(text):
+    text = text.replace("\\n", "")
+    return text
```

## wafl/retriever/base_retriever.py

```diff
@@ -1,9 +1,11 @@
 from typing import List, Tuple
 
 
 class BaseRetriever:
-    def add_text_and_index(self, text: str, index: str):
+    async def add_text_and_index(self, text: str, index: str):
         raise NotImplemented
 
-    def get_indices_and_scores_from_text(self, text: str) -> List[Tuple[str, float]]:
+    async def get_indices_and_scores_from_text(
+        self, text: str
+    ) -> List[Tuple[str, float]]:
         raise NotImplemented
```

## wafl/retriever/dense_retriever.py

```diff
@@ -1,49 +1,44 @@
 import os
-import torch
-import logging
 import numpy as np
 
 from typing import List, Tuple
 from gensim.models import KeyedVectors
-from sentence_transformers import SentenceTransformer
-
+from wafl.connectors.factories.sentence_embedder_connector_factory import (
+    SentenceEmbedderConnectorFactory,
+)
 from wafl.retriever.base_retriever import BaseRetriever
 
 _path = os.path.dirname(__file__)
-_logger = logging.getLogger(__file__)
-
-device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
 
 class DenseRetriever(BaseRetriever):
     _threshold_length = 5
 
-    def __init__(self, model_name):
-        self._sentence_model = SentenceTransformer(model_name)
-        self._sentence_model = self._sentence_model.to(device)
-
-        self._embeddings_model = KeyedVectors(768)
+    def __init__(self, model_name, config):
+        self._connector = SentenceEmbedderConnectorFactory.get_connector(
+            model_name, config
+        )
+        self._embeddings_model = KeyedVectors(384)
 
-    def add_text_and_index(self, text: str, index: str):
-        embeddings = self._get_embeddings_from_text(text)
+    async def add_text_and_index(self, text: str, index: str):
+        embeddings = await self._get_embeddings_from_text(text)
         self._embeddings_model.add_vectors([index], [embeddings])
         self._embeddings_model.fill_norms(force=True)
 
-    def get_indices_and_scores_from_text(self, text: str) -> List[Tuple[str, float]]:
-        if not text or len(text) < self._threshold_length:
-            return []
-
-        embeddings = self._get_embeddings_from_text(text)
-        return self._embeddings_model.similar_by_vector(embeddings, topn=2)
-
-    def _get_embeddings_from_text(self, text: str) -> "numpy.array":
-        return self._sentence_model.encode(text)
-
-    def get_dot_product(self, lhs: str, rhs: str) -> float:
-        lhs_vector = self._sentence_model.encode(lhs)
-        rhs_vector = self._sentence_model.encode(rhs)
+    async def get_indices_and_scores_from_text(
+        self, text: str
+    ) -> List[Tuple[str, float]]:
+        embeddings = await self._get_embeddings_from_text(text)
+        return self._embeddings_model.similar_by_vector(embeddings, topn=5)
+
+    async def _get_embeddings_from_text(self, text: str) -> "numpy.array":
+        return (await self._connector.predict(text))["embedding"]
+
+    async def get_dot_product(self, lhs: str, rhs: str) -> float:
+        lhs_vector = (await self._connector.predict(lhs))["embedding"]
+        rhs_vector = (await self._connector.predict(rhs))["embedding"]
         return (
             np.dot(lhs_vector, rhs_vector)
             / np.linalg.norm(lhs_vector)
             / np.linalg.norm(rhs_vector)
         )
```

## wafl/retriever/string_retriever.py

```diff
@@ -3,15 +3,17 @@
 from wafl.retriever.base_retriever import BaseRetriever
 
 
 class StringRetriever(BaseRetriever):
     def __init__(self):
         self._string_dict = {}
 
-    def add_text_and_index(self, text: str, index: str):
+    async def add_text_and_index(self, text: str, index: str):
         self._string_dict[text.strip()] = index
 
-    def get_indices_and_scores_from_text(self, text: str) -> List[Tuple[str, float]]:
+    async def get_indices_and_scores_from_text(
+        self, text: str
+    ) -> List[Tuple[str, float]]:
         if text.strip() in self._string_dict:
             return [(self._string_dict[text.strip()], 1)]
 
         return []
```

## wafl/speaker/fairseq_speaker.py

```diff
@@ -1,45 +1,29 @@
-from time import sleep
-
+import asyncio
 import pyaudio
-import torch
 
-from fairseq.checkpoint_utils import load_model_ensemble_and_task_from_hf_hub
-from fairseq.models.text_to_speech.hub_interface import TTSHubInterface
+from wafl.connectors.factories.speaker_connector_factory import SpeakerConnectorFactory
 from wafl.speaker.base_speaker import BaseSpeaker
-
-_device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+from wafl.speaker.utils import convert_numbers_to_words
 
 
 class FairSeqSpeaker(BaseSpeaker):
-    def __init__(self, voice="facebook/fastspeech2-en-ljspeech"):
-        self._chunk = 1024
-        models, cfg, self._task = load_model_ensemble_and_task_from_hf_hub(
-            voice,
-            arg_overrides={"vocoder": "hifigan", "fp16": False},
-        )
+    def __init__(self, config):
+        self._connector = SpeakerConnectorFactory.get_connector(config)
         self._p = pyaudio.PyAudio()
-        self._model = models[0]
-        TTSHubInterface.update_cfg_with_data_cfg(cfg, self._task.data_cfg)
-        self._generator = self._task.build_generator(models, cfg)
-        self._generator.model.to(_device)
-        self._generator.vocoder.model.to(_device)
-
-    def speak(self, text):
-        sample = TTSHubInterface.get_model_input(self._task, text)
-        sample["net_input"]["src_tokens"] = sample["net_input"]["src_tokens"].to(
-            _device
-        )
-        wav, rate = TTSHubInterface.get_prediction(
-            self._task, self._model, self._generator, sample
-        )
 
+    async def speak(self, text):
+        text = convert_numbers_to_words(text)
+        prediction = await self._connector.predict(text)
+        wav = prediction["wav"]
+        rate = prediction["rate"]
         stream = self._p.open(
             format=pyaudio.paFloat32,
             channels=1,
             rate=rate,
             output=True,
         )
-        stream.write(wav.cpu().numpy().tobytes())
-        sleep(0.5)
+        await asyncio.sleep(0.2)
+        stream.write(wav)
         stream.stop_stream()
         stream.close()
+        await asyncio.sleep(0.1)
```

## wafl/templates/config.json

```diff
@@ -1,17 +1,40 @@
-00000000: 7b0a 2020 2261 6363 6570 745f 7261 6e64  {.  "accept_rand
-00000010: 6f6d 5f66 6163 7473 223a 2066 616c 7365  om_facts": false
-00000020: 2c0a 2020 2261 6c6c 6f77 5f69 6e74 6572  ,.  "allow_inter
-00000030: 7275 7074 696f 6e73 223a 2074 7275 652c  ruptions": true,
-00000040: 0a20 2022 766f 6963 655f 686f 7477 6f72  .  "voice_hotwor
-00000050: 6473 223a 205b 0a20 2020 2022 434f 4d50  ds": [.    "COMP
-00000060: 5554 4552 220a 2020 5d2c 0a20 2022 7761  UTER".  ],.  "wa
-00000070: 6b69 6e67 5f75 705f 776f 7264 223a 2022  king_up_word": "
-00000080: 636f 6d70 7574 6572 222c 0a20 2022 7761  computer",.  "wa
-00000090: 6b69 6e67 5f75 705f 736f 756e 6422 3a20  king_up_sound": 
-000000a0: 7472 7565 2c0a 2020 2264 6561 6374 6976  true,.  "deactiv
-000000b0: 6174 655f 736f 756e 6422 3a20 7472 7565  ate_sound": true
-000000c0: 2c0a 2020 2264 656e 795f 736f 756e 6422  ,.  "deny_sound"
-000000d0: 3a20 7472 7565 2c0a 2020 226c 6973 7465  : true,.  "liste
-000000e0: 6e65 725f 6d6f 6465 6c22 3a20 226f 7065  ner_model": "ope
-000000f0: 6e61 692f 7768 6973 7065 722d 7469 6e79  nai/whisper-tiny
-00000100: 2e65 6e22 2c0a 7d0a                      .en",.}.
+00000000: 7b0a 2020 2277 616b 696e 675f 7570 5f77  {.  "waking_up_w
+00000010: 6f72 6422 3a20 2263 6f6d 7075 7465 7222  ord": "computer"
+00000020: 2c0a 2020 2277 616b 696e 675f 7570 5f73  ,.  "waking_up_s
+00000030: 6f75 6e64 223a 2074 7275 652c 0a20 2022  ound": true,.  "
+00000040: 6465 6163 7469 7661 7465 5f73 6f75 6e64  deactivate_sound
+00000050: 223a 2074 7275 652c 0a20 2022 7275 6c65  ": true,.  "rule
+00000060: 7322 3a20 2272 756c 6573 2e79 616d 6c22  s": "rules.yaml"
+00000070: 2c0a 2020 2266 756e 6374 696f 6e73 223a  ,.  "functions":
+00000080: 2022 6675 6e63 7469 6f6e 732e 7079 222c   "functions.py",
+00000090: 0a20 2022 6672 6f6e 7465 6e64 5f70 6f72  .  "frontend_por
+000000a0: 7422 3a20 3830 3930 2c0a 2020 226c 6c6d  t": 8090,.  "llm
+000000b0: 5f6d 6f64 656c 223a 207b 0a20 2020 2022  _model": {.    "
+000000c0: 6d6f 6465 6c5f 686f 7374 223a 2022 6c6f  model_host": "lo
+000000d0: 6361 6c68 6f73 7422 2c0a 2020 2020 226d  calhost",.    "m
+000000e0: 6f64 656c 5f70 6f72 7422 3a20 3830 3830  odel_port": 8080
+000000f0: 2c0a 2020 2020 2274 656d 7065 7261 7475  ,.    "temperatu
+00000100: 7265 223a 2030 2e34 0a20 207d 2c0a 2020  re": 0.4.  },.  
+00000110: 226c 6973 7465 6e65 725f 6d6f 6465 6c22  "listener_model"
+00000120: 3a20 7b0a 2020 2020 226d 6f64 656c 5f68  : {.    "model_h
+00000130: 6f73 7422 3a20 226c 6f63 616c 686f 7374  ost": "localhost
+00000140: 222c 0a20 2020 2022 6d6f 6465 6c5f 706f  ",.    "model_po
+00000150: 7274 223a 2038 3038 302c 0a20 2020 2022  rt": 8080,.    "
+00000160: 6c69 7374 656e 6572 5f68 6f74 776f 7264  listener_hotword
+00000170: 5f6c 6f67 7022 3a20 2d38 2c0a 2020 2020  _logp": -8,.    
+00000180: 226c 6973 7465 6e65 725f 766f 6c75 6d65  "listener_volume
+00000190: 5f74 6872 6573 686f 6c64 223a 2030 2e36  _threshold": 0.6
+000001a0: 2c0a 2020 2020 226c 6973 7465 6e65 725f  ,.    "listener_
+000001b0: 7369 6c65 6e63 655f 7469 6d65 6f75 7422  silence_timeout"
+000001c0: 3a20 302e 370a 2020 7d2c 0a20 2022 7370  : 0.7.  },.  "sp
+000001d0: 6561 6b65 725f 6d6f 6465 6c22 3a20 7b0a  eaker_model": {.
+000001e0: 2020 2020 226d 6f64 656c 5f68 6f73 7422      "model_host"
+000001f0: 3a20 226c 6f63 616c 686f 7374 222c 0a20  : "localhost",. 
+00000200: 2020 2022 6d6f 6465 6c5f 706f 7274 223a     "model_port":
+00000210: 2038 3038 300a 2020 7d2c 0a20 2022 7465   8080.  },.  "te
+00000220: 7874 5f65 6d62 6564 6469 6e67 5f6d 6f64  xt_embedding_mod
+00000230: 656c 223a 207b 0a20 2020 2022 6d6f 6465  el": {.    "mode
+00000240: 6c5f 686f 7374 223a 2022 6c6f 6361 6c68  l_host": "localh
+00000250: 6f73 7422 2c0a 2020 2020 226d 6f64 656c  ost",.    "model
+00000260: 5f70 6f72 7422 3a20 3830 3830 0a20 207d  _port": 8080.  }
+00000270: 0a7d 0a                                  .}.
```

## wafl/templates/functions.py

```diff
@@ -1,5 +1,132 @@
+import json
+import html2text
+import re
+import requests
+
+from datetime import datetime, timedelta
 from wafl.exceptions import CloseConversation
 
+_db_filename = "db.json"
+
 
 def close_conversation():
     raise CloseConversation()
+
+
+def check_today_weather():
+    today = datetime.now().strftime("%Y-%m-%d")
+    with open(_db_filename) as file:
+        db = json.load(file)
+        latitude = db["latitude"]
+        longitude = db["longitude"]
+
+    return check_weather_lat_long(latitude, longitude, today)
+
+
+def check_tomorrow_weather():
+    today = datetime.now()
+    with open(_db_filename) as file:
+        db = json.load(file)
+        latitude = db["latitude"]
+        longitude = db["longitude"]
+
+    tomorrow = (today + timedelta(days=1)).strftime("%Y-%m-%d")
+    return check_weather_lat_long(latitude, longitude, tomorrow)
+
+
+def check_weather_lat_long(latitude, longitude, day):
+    secrets = json.load(open("secrets.json"))
+    result = requests.get(
+        f"https://rgw.5878-e94b1c46.eu-gb.apiconnect.appdomain.cloud/metoffice/production/v0/forecasts/point/daily?excludeParameterMetadata=true&includeLocationName=true&latitude={latitude}&longitude={longitude}",
+        headers={
+            "X-IBM-Client-Id": secrets["key"],
+            "X-IBM-Client-Secret": secrets["secret"],
+        },
+    )
+    data = result.json()
+    if "features" not in data:
+        return "There is a connection error to the weather API. Please try later. "
+    to_say = ""
+    for item in data["features"][0]["properties"]["timeSeries"]:
+        if day in item["time"]:
+            to_say += f"The temperature should be between {int(item['dayLowerBoundMaxTemp'])} and {int(item['dayUpperBoundMaxTemp'])}. "
+            if item["dayProbabilityOfPrecipitation"] != 0:
+                to_say += f"The probability of rain is {item['dayProbabilityOfPrecipitation']} percent. "
+
+            else:
+                to_say += "There is no probability of rain. "
+
+            if item["dayProbabilityOfSnow"] != 0:
+                to_say += f"The probability of snow is {item['dayProbabilityOfSnow']} percent. "
+
+            else:
+                to_say += "There is no probability of snow. "
+
+    return to_say
+
+
+def get_website(url):
+    text = requests.get(url).content.decode("utf-8")
+    h = html2text.HTML2Text()
+    h.ignore_links = True
+    return h.handle(text).strip()[:1000]
+
+
+def get_guardian_headlines():
+    url = "https://www.theguardian.com/uk"
+    text = requests.get(url).content.decode("utf-8")
+    pattern = re.compile(r"<h4 .*?><span>(.*?)</span></h4>", re.MULTILINE)
+    matches = pattern.findall(text)
+    text = "-" + "\n-".join(matches)
+    h = html2text.HTML2Text()
+    h.ignore_links = True
+    return h.handle(text).strip()
+
+
+def get_time():
+    return datetime.now().strftime("%H,%M")
+
+
+def get_date():
+    return datetime.now().strftime("%Y-%m-%d")
+
+
+def get_day():
+    return datetime.now().strftime("%A")
+
+
+def add_to_shopping_list(list_of_items_to_add):
+    db = json.load(open(_db_filename))
+    for item in list_of_items_to_add:
+        if item not in db["shopping_list"]:
+            db["shopping_list"].append(item)
+
+    json.dump(db, open(_db_filename, "w"))
+
+    return "Item added"
+
+
+def remove_from_shopping_list(list_of_items_to_remove):
+    db = json.load(open(_db_filename))
+    for item in list_of_items_to_remove:
+        if item in db["shopping_list"]:
+            db["shopping_list"].remove(item)
+
+    json.dump(db, open(_db_filename, "w"))
+
+    return "Item removed"
+
+
+def get_shopping_list():
+    db = json.load(open(_db_filename))
+    if db["shopping_list"] == []:
+        return "nothing"
+
+    return ", ".join(db["shopping_list"])
+
+
+def write_to_file(filename, text):
+    with open(filename, "w") as file:
+        file.write(text)
+
+    return f"File {filename} saved"
```

## wafl/templates/testcases.txt

```diff
@@ -1,7 +1,7 @@
 test the greetings work
-  user> bring yourself online
-  bot> Hello there!
+  user: bring yourself online
+  bot: Hello there!
 
 test good bye
-  user> Good bye
-  bot> Good bye!
+  user: Good bye
+  bot: Good bye!
```

## Comparing `wafl/conversation/conversation.py` & `wafl/events/conversation_events.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,108 +1,125 @@
 import os
-from wafl.inference.utils import normalized
+import re
 
+from wafl.events.answerer_creator import create_answerer
+from wafl.simple_text_processing.normalize import normalized
 from wafl.config import Configuration
-from wafl.conversation.utils import is_question, get_answer_using_text, input_is_valid
+from wafl.events.utils import input_is_valid, load_knowledge
+from wafl.simple_text_processing.questions import is_question
 from wafl.exceptions import InterruptTask
-from wafl.inference.backward_inference import BackwardInference
-
 
 os.environ["PROTOCOL_BUFFERS_PYTHON_IMPLEMENTATION"] = "python"
 
 
-class Conversation:
+class ConversationEvents:
     def __init__(
         self,
-        knowledge: "BaseKnowledge",
+        config: "Configuration",
         interface: "BaseInterface",
-        code_path=None,
-        config=None,
         logger=None,
     ):
-        self._knowledge = knowledge
+        self._config = config
+        self._knowledge = load_knowledge(config, logger)
+        self._answerer = create_answerer(config, self._knowledge, interface, logger)
+        self._answerer._client._connector._cache = {}
         self._interface = interface
-        self._inference = BackwardInference(
-            self._knowledge, interface, code_path, logger=logger
-        )
-        if not config:
-            self._config = Configuration.load_local_config()
-        else:
-            self._config = config
-
         self._logger = logger
+        self._is_computing = False
         if logger:
             self._logger.set_depth(0)
 
-    def output(self, text: str):
-        self._interface.output(text)
+    async def output(self, text: str):
+        await self._interface.output(text)
 
-    def add(self, text: str):
+    async def _process_query(self, text: str):
+        self._is_computing = True
+        self._interface.bot_has_spoken(False)
         if not input_is_valid(text):
+            self._is_computing = False
             return False
 
         text_is_question = is_question(text)
-
         try:
-            answer = get_answer_using_text(self._inference, self._interface, text)
+            answer = await self._answerer.answer(text)
 
         except InterruptTask:
-            self._interface.output("Task interrupted")
+            await self._interface.output("Task interrupted")
+            self._is_computing = False
             return False
 
-        if (
-            self._config.get_value("accept_random_facts")
-            and not text_is_question
-            and answer.text == "False"
-            and not self._interface.bot_has_spoken()
-        ):
-            self._knowledge.add(text)
-            self.output("I will remember it.")
-
         if not self._interface.bot_has_spoken():
-            if not text_is_question and normalized(answer.text) in ["unknown"]:
-                self.output(answer.text)
+            if not text_is_question and not answer.is_neutral():
+                await self.output(answer.text)
 
             if text_is_question and answer.text not in ["True", "False"]:
-                self.output(answer.text)
+                await self.output(answer.text)
 
-            if text_is_question and answer.text == "False":
-                self.output("Unknown")
+            if text_is_question and answer.is_false():
+                await self.output("I don't know")
 
+            if (
+                not text_is_question
+                and self._interface.get_utterances_list()
+                and self._interface.last_speaker() == "user"
+            ):
+                await self._interface.output("I don't know what to reply")
+
+            if (
+                not text_is_question
+                and answer.is_true()
+                and not self._interface.bot_has_spoken()
+            ):
+                await self._interface.output("Yes")
+
+        self._is_computing = False
         return answer
 
-    def input(self, activation_word: str = "") -> bool:
+    async def process_next(self, activation_word: str = "") -> bool:
         try:
-            text = self._interface.input()
+            text = await self._interface.input()
+            text = text.replace("'", r"\'")
 
         except IndexError:
             return False
 
-        if not self._interface.check_understanding() and self.__activation_word_in_text(
-            activation_word, text
+        if (
+            activation_word
+            and not self._interface.is_listening()
+            and self._activation_word_in_text(activation_word, text)
         ):
-            self._interface.check_understanding(True)
-            self._logger.write(f"Activation word found {text}", depth=0)
-            if normalized(text) == normalized(activation_word):
+            self._interface.activate()
+            self._logger.set_depth(0)
+            self._logger.write(f"Activation word found {text}")
+            if normalized(text) == normalized(activation_word, lower_case=True):
                 return True
 
-            text = self.__remove_activation_word_and_normalize(activation_word, text)
-
-        if self._interface.check_understanding():
-            answer = self.add(text)
-            if answer and answer.text != "False":
+        text = self.__remove_activation_word_and_normalize(activation_word, text)
+        if self._interface.is_listening():
+            answer = await self._process_query(text)
+            if answer and not answer.is_false():
                 return True
 
         return False
 
-    def check_understanding(self, do_the_check=None):
-        return self._interface.check_understanding(do_the_check)
+    def is_computing(self):
+        return self._is_computing
+
+    def reload_knowledge(self):
+        self._knowledge = load_knowledge(self._config, self._logger)
+
+    def reset_discourse_memory(self):
+        self._answerer = create_answerer(
+            self._config, self._knowledge, self._interface, self._logger
+        )
 
-    def __activation_word_in_text(self, activation_word, text):
+    def _activation_word_in_text(self, activation_word, text):
         if f"[{normalized(activation_word)}]" in normalized(text):
             return True
 
         return False
 
     def __remove_activation_word_and_normalize(self, activation_word, text):
         to_remove = f"[{activation_word}]"
-        return text.replace(to_remove, "").strip()
+        text = text.replace(to_remove, "").strip()
+        text = re.sub(f"^{activation_word}", "", text, flags=re.IGNORECASE)
+        return text
```

## Comparing `wafl/conversation/working_memory.py` & `wafl/events/conversational_memory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-class WorkingMemory:
+class ConversationalMemory:
     def __init__(self):
         self._story = ""
         self._questions = []
         self._answers = []
         self._failed_clauses = set()
 
     def get_story(self):
```

## Comparing `wafl/knowledge/knowledge.py` & `wafl/knowledge/single_file_knowledge.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,244 +1,230 @@
+import asyncio
 import logging
+from typing import List
+
 import nltk
 
+from wafl.config import Configuration
 from wafl.facts import Fact
-from wafl.inference.utils import normalized
 from wafl.knowledge.base_knowledge import BaseKnowledge
 from wafl.knowledge.utils import (
     text_is_exact_string,
-    rules_are_too_different,
     get_first_cluster_of_rules,
-    filter_out_rules_that_are_too_dissimilar_to_query,
-    filter_out_rules_through_entailment,
 )
+from wafl.parsing.line_rules_parser import parse_rule_from_single_line
 from wafl.parsing.rules_parser import get_facts_and_rules_from_text
-from wafl.qa.entailer import Entailer
-from wafl.qa.dataclasses import Query
 from wafl.retriever.string_retriever import StringRetriever
 from wafl.retriever.dense_retriever import DenseRetriever
 from wafl.text_utils import clean_text_for_retrieval
 
 nltk.download("punkt")
 nltk.download("averaged_perceptron_tagger")
 
 _logger = logging.getLogger(__name__)
 
 
-class Knowledge(BaseKnowledge):
-    _threshold_for_questions_from_user = 0.6
+class SingleFileKnowledge(BaseKnowledge):
+    _threshold_for_questions_from_user = 0.55
     _threshold_for_questions_from_bot = 0.6
-    _threshold_for_questions_in_rules = 0.505
-    _threshold_for_facts = 0.58
-    _threshold_for_partial_facts = 0.48
-
-    def __init__(self, rules_text=None, logger=None):
-        facts_and_rules = get_facts_and_rules_from_text(rules_text)
-        self._facts_dict = {
-            f"F{index}": value for index, value in enumerate(facts_and_rules["facts"])
-        }
-        self._rules_dict = {
-            f"R{index}": value for index, value in enumerate(facts_and_rules["rules"])
-        }
-        self._facts_retriever = DenseRetriever("msmarco-distilbert-base-v3")
+    _threshold_for_questions_in_rules = 0.49
+    _threshold_for_facts = 0.7
+    _threshold_for_rules = 0.85
+    _max_rules_per_type = 3
+
+    def __init__(self, config, rules_text=None, logger=None):
+        self._logger = logger
+        self._facts_dict = {}
+        self._rules_dict = {}
+        self._facts_retriever = DenseRetriever("text_embedding_model", config)
         self._facts_retriever_for_questions = DenseRetriever(
-            "multi-qa-distilbert-dot-v1"
+            "text_embedding_model",
+            config,
         )
-        self._logger = logger
-        self._entailer = Entailer(logger)
-        self._rules_incomplete_retriever = DenseRetriever("msmarco-distilbert-base-v3")
-        self._rules_fact_retriever = DenseRetriever("msmarco-distilbert-base-v3")
-        self._rules_question_retriever = DenseRetriever("msmarco-distilbert-base-v3")
+        self._rules_retriever = DenseRetriever("text_embedding_model", config)
         self._rules_string_retriever = StringRetriever()
-        self._initialize_retrievers()
+        if rules_text:
+            facts_and_rules = get_facts_and_rules_from_text(rules_text)
+            self._facts_dict = {
+                f"F{index}": value
+                for index, value in enumerate(facts_and_rules["facts"])
+            }
+            self._rules_dict = {
+                f"R{index}": value
+                for index, value in enumerate(facts_and_rules["rules"])
+            }
+            try:
+                loop = asyncio.get_running_loop()
+
+            except RuntimeError:
+                loop = None
+
+            if not loop or not loop.is_running():
+                asyncio.run(self._initialize_retrievers())
 
-    def add(self, text):
+    async def add(self, text):
         fact_index = f"F{len(self._facts_dict)}"
         self._facts_dict[fact_index] = Fact(text=text)
-        self._facts_retriever.add_text_and_index(
+        await self._facts_retriever.add_text_and_index(
             clean_text_for_retrieval(text), fact_index
         )
-        self._facts_retriever_for_questions.add_text_and_index(
+        await self._facts_retriever_for_questions.add_text_and_index(
             clean_text_for_retrieval(text), fact_index
         )
 
-    def has_better_match(self, answer: str) -> bool:
-        if any(normalized(answer).find(item) == 0 for item in ["yes", "no"]):
-            return False
-
-        if any(normalized(answer).find(item) != -1 for item in [" yes ", " no "]):
-            return False
-
-        rules = self.ask_for_rule_backward(
-            Query(text=f"The user says to the bot: '{answer}.'", is_question=False)
+    async def add_rule(self, rule_text):
+        rule = parse_rule_from_single_line(rule_text)
+        index = str(len(self._rules_dict))
+        index = f"R{index}"
+        self._rules_dict[index] = rule
+        await self._rules_retriever.add_text_and_index(
+            clean_text_for_retrieval(rule.effect.text), index=index
         )
-        return any(rule.effect.is_interruption for rule in rules)
 
-    def ask_for_facts(self, query, is_from_user=False):
+    async def ask_for_facts(self, query, is_from_user=False, threshold=None):
         if query.is_question:
-            indices_and_scores = (
-                self._facts_retriever_for_questions.get_indices_and_scores_from_text(
-                    query.text
-                )
+            indices_and_scores = await self._facts_retriever_for_questions.get_indices_and_scores_from_text(
+                query.text
             )
 
         else:
-            indices_and_scores = self._facts_retriever.get_indices_and_scores_from_text(
-                query.text
+            indices_and_scores = (
+                await self._facts_retriever.get_indices_and_scores_from_text(query.text)
             )
-        if is_from_user:
+        if threshold == None and is_from_user:
             threshold = (
                 self._threshold_for_questions_from_user
                 if query.is_question
                 else self._threshold_for_facts
             )
-        else:
+        elif threshold == None:
             threshold = (
                 self._threshold_for_questions_from_bot
                 if query.is_question
                 else self._threshold_for_facts
             )
 
         return [
             self._facts_dict[item[0]]
             for item in indices_and_scores
             if item[1] > threshold
         ]
 
-    def ask_for_facts_with_threshold(self, query, is_from_user=False):
+    async def ask_for_facts_with_threshold(
+        self, query, is_from_user=False, threshold=None
+    ):
         if query.is_question:
-            indices_and_scores = (
-                self._facts_retriever_for_questions.get_indices_and_scores_from_text(
-                    query.text
-                )
+            indices_and_scores = await self._facts_retriever_for_questions.get_indices_and_scores_from_text(
+                query.text
             )
 
         else:
-            indices_and_scores = self._facts_retriever.get_indices_and_scores_from_text(
-                query.text
+            indices_and_scores = (
+                await self._facts_retriever.get_indices_and_scores_from_text(query.text)
             )
-        if is_from_user:
+
+        if threshold == None and is_from_user:
             threshold = (
                 self._threshold_for_questions_from_user
                 if query.is_question
                 else self._threshold_for_facts
             )
-        else:
+
+        elif threshold == None:
             threshold = (
                 self._threshold_for_questions_from_bot
                 if query.is_question
                 else self._threshold_for_facts
             )
 
         return [
             (self._facts_dict[item[0]], item[1])
             for item in indices_and_scores
             if item[1] > threshold
         ]
 
-    def ask_for_rule_backward(self, query):
-        if text_is_exact_string(query.text):
-            indices_and_scores = (
-                self._rules_string_retriever.get_indices_and_scores_from_text(
-                    query.text
-                )
-            )
-            return [self._rules_dict[item[0]] for item in indices_and_scores]
-
-        indices_and_scores = (
-            self._rules_fact_retriever.get_indices_and_scores_from_text(query.text)
-        )
-        fact_rules = [
-            (self._rules_dict[item[0]], item[1])
-            for item in indices_and_scores
-            if item[1] > self._threshold_for_facts
-        ]
-
-        indices_and_scores = (
-            self._rules_question_retriever.get_indices_and_scores_from_text(query.text)
-        )
-        question_rules = [
-            (self._rules_dict[item[0]], item[1])
-            for item in indices_and_scores
-            if item[1] > self._threshold_for_questions_in_rules
-        ]
-
-        indices_and_scores = (
-            self._rules_incomplete_retriever.get_indices_and_scores_from_text(
-                query.text
-            )
+    async def ask_for_rule_backward(self, query, threshold=None):
+        rules_and_scores = await self._ask_for_rule_backward_with_scores(
+            query, threshold=threshold
         )
-        incomplete_rules = [
-            (self._rules_dict[item[0]], item[1])
-            for item in indices_and_scores
-            if item[1] > self._threshold_for_partial_facts
-        ]
-
-        rules_and_scores = [
-            item
-            for item in sorted(
-                fact_rules + question_rules + incomplete_rules, key=lambda x: -x[1]
-            )
-        ]
-
-        rules = [item[0] for item in rules_and_scores]
-        if rules_are_too_different(self._rules_fact_retriever, rules):
-            return []
-
-        rules_and_scores = filter_out_rules_that_are_too_dissimilar_to_query(
-            query, rules_and_scores
-        )
-
-        rules_and_scores = filter_out_rules_through_entailment(
-            self._entailer, query, rules_and_scores
-        )
-
         return get_first_cluster_of_rules(rules_and_scores)
 
     def get_facts_and_rule_as_text(self):
         text = ""
         for fact in self._facts_dict.values():
             text += fact.text + "\n"
 
         for effect in self._rules_dict.values():
             text += effect.effect.text + "\n"
 
         return text
 
-    def _initialize_retrievers(self):
+    async def _initialize_retrievers(self):
         for index, fact in self._facts_dict.items():
             if text_is_exact_string(fact.text):
                 continue
 
-            self._facts_retriever.add_text_and_index(
+            await self._facts_retriever.add_text_and_index(
                 clean_text_for_retrieval(fact.text), index
             )
 
-            self._facts_retriever_for_questions.add_text_and_index(
+            await self._facts_retriever_for_questions.add_text_and_index(
                 clean_text_for_retrieval(fact.text), index
             )
 
         for index, rule in self._rules_dict.items():
             if text_is_exact_string(rule.effect.text):
                 continue
 
-            if "{" in rule.effect.text:
-                self._rules_incomplete_retriever.add_text_and_index(
-                    clean_text_for_retrieval(rule.effect.text), index
-                )
+            await self._rules_retriever.add_text_and_index(
+                clean_text_for_retrieval(rule.effect.text), index
+            )
+
+        for index, rule in self._rules_dict.items():
+            if not text_is_exact_string(rule.effect.text):
                 continue
 
-            elif rule.effect.is_question:
-                self._rules_question_retriever.add_text_and_index(
-                    clean_text_for_retrieval(rule.effect.text), index
-                )
+            await self._rules_string_retriever.add_text_and_index(
+                rule.effect.text, index
+            )
+
+    @staticmethod
+    async def create_from_list(
+        facts: List[str], config: "Configuration" = None
+    ) -> "SingleFileKnowledge":
+        if not config:
+            config = Configuration.load_local_config()
+
+        knowledge = SingleFileKnowledge(config)
+        for index, fact in enumerate(facts):
+            await knowledge.add(fact)
 
-            else:
-                self._rules_fact_retriever.add_text_and_index(
-                    clean_text_for_retrieval(rule.effect.text), index
+        return knowledge
+
+    async def _ask_for_rule_backward_with_scores(self, query, threshold=None):
+        if text_is_exact_string(query.text):
+            indices_and_scores = (
+                await self._rules_string_retriever.get_indices_and_scores_from_text(
+                    query.text
                 )
+            )
+            return [(self._rules_dict[item[0]], item[1]) for item in indices_and_scores]
 
-        for index, rule in self._rules_dict.items():
-            if not text_is_exact_string(rule.effect.text):
-                continue
+        indices_and_scores = (
+            await self._rules_retriever.get_indices_and_scores_from_text(query.text)
+        )
+
+        if threshold == None:
+            threshold = self._threshold_for_rules
+
+        rules = [
+            (self._rules_dict[item[0]], item[1])
+            for item in indices_and_scores
+            if item[1] > threshold
+        ]
+
+        rules = [item for item in sorted(rules, key=lambda x: -x[1])][
+            : self._max_rules_per_type
+        ]
 
-            self._rules_string_retriever.add_text_and_index(rule.effect.text, index)
+        rules_and_scores = rules
+        return rules_and_scores
```

