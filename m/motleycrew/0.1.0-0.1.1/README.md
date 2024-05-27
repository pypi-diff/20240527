# Comparing `tmp/motleycrew-0.1.0.tar.gz` & `tmp/motleycrew-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motleycrew-0.1.0.tar", max compression
+gzip compressed data, was "motleycrew-0.1.1.tar", max compression
```

## Comparing `motleycrew-0.1.0.tar` & `motleycrew-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,75 @@
--rw-r--r--   0        0        0     2873 2024-04-17 17:05:38.173370 motleycrew-0.1.0/README.md
--rw-r--r--   0        0        0       93 2024-04-17 16:44:57.067364 motleycrew-0.1.0/motleycrew/__init__.py
--rw-r--r--   0        0        0      147 2024-04-18 13:15:06.135101 motleycrew-0.1.0/motleycrew/agent/__init__.py
--rw-r--r--   0        0        0      223 2024-04-17 16:44:57.067779 motleycrew-0.1.0/motleycrew/agent/coordinator.py
--rw-r--r--   0        0        0       88 2024-04-17 16:44:57.068494 motleycrew-0.1.0/motleycrew/agent/crewai/__init__.py
--rw-r--r--   0        0        0     4732 2024-04-18 19:49:53.513440 motleycrew-0.1.0/motleycrew/agent/crewai/crewai.py
--rw-r--r--   0        0        0      803 2024-04-18 19:49:08.719936 motleycrew-0.1.0/motleycrew/agent/crewai/crewai_agent.py
--rw-r--r--   0        0        0      148 2024-04-17 16:44:57.070413 motleycrew-0.1.0/motleycrew/agent/langchain/__init__.py
--rw-r--r--   0        0        0     4424 2024-04-18 19:49:08.720319 motleycrew-0.1.0/motleycrew/agent/langchain/langchain.py
--rw-r--r--   0        0        0     7824 2024-04-18 19:49:08.720675 motleycrew-0.1.0/motleycrew/agent/langchain/openai_tools_react.py
--rw-r--r--   0        0        0     1135 2024-04-18 19:50:05.176558 motleycrew-0.1.0/motleycrew/agent/langchain/react.py
--rw-r--r--   0        0        0      111 2024-04-17 16:44:57.071642 motleycrew-0.1.0/motleycrew/agent/llama_index/__init__.py
--rw-r--r--   0        0        0     2826 2024-04-18 19:50:15.144681 motleycrew-0.1.0/motleycrew/agent/llama_index/llama_index.py
--rw-r--r--   0        0        0     1488 2024-04-17 16:44:57.071914 motleycrew-0.1.0/motleycrew/agent/llama_index/llama_index_react.py
--rw-r--r--   0        0        0      427 2024-04-18 19:49:08.722128 motleycrew-0.1.0/motleycrew/agent/parent.py
--rw-r--r--   0        0        0     3996 2024-04-18 19:49:08.722579 motleycrew-0.1.0/motleycrew/agent/shared.py
--rw-r--r--   0        0        0      171 2024-04-18 19:49:08.722922 motleycrew-0.1.0/motleycrew/common/__init__.py
--rw-r--r--   0        0        0      188 2024-04-18 19:49:08.723211 motleycrew-0.1.0/motleycrew/common/defaults.py
--rw-r--r--   0        0        0      121 2024-04-17 16:44:57.073693 motleycrew-0.1.0/motleycrew/common/enums.py
--rw-r--r--   0        0        0     1100 2024-04-17 16:44:57.075053 motleycrew-0.1.0/motleycrew/common/exceptions.py
--rw-r--r--   0        0        0     1312 2024-04-17 16:44:57.075618 motleycrew-0.1.0/motleycrew/common/llms.py
--rw-r--r--   0        0        0      488 2024-04-18 19:49:08.723526 motleycrew-0.1.0/motleycrew/common/types.py
--rw-r--r--   0        0        0     1217 2024-04-19 15:25:11.868912 motleycrew-0.1.0/motleycrew/common/utils.py
--rw-r--r--   0        0        0     5170 2024-04-18 19:49:08.724216 motleycrew-0.1.0/motleycrew/crew.py
--rw-r--r--   0        0        0      171 2024-04-17 16:44:57.066424 motleycrew-0.1.0/motleycrew/tasks/__init__.py
--rw-r--r--   0        0        0     1020 2024-04-17 16:44:57.066147 motleycrew-0.1.0/motleycrew/tasks/graph.py
--rw-r--r--   0        0        0     3388 2024-04-18 19:49:08.724751 motleycrew-0.1.0/motleycrew/tasks/task.py
--rw-r--r--   0        0        0       29 2024-04-17 16:44:57.076591 motleycrew-0.1.0/motleycrew/tool/__init__.py
--rw-r--r--   0        0        0     3188 2024-04-19 17:01:22.779797 motleycrew-0.1.0/motleycrew/tool/image_generation.py
--rw-r--r--   0        0        0     1459 2024-04-17 16:44:57.076317 motleycrew-0.1.0/motleycrew/tool/llm_tool.py
--rw-r--r--   0        0        0      772 2024-04-17 16:44:57.076847 motleycrew-0.1.0/motleycrew/tool/python_repl.py
--rw-r--r--   0        0        0     2100 2024-04-17 16:44:57.077097 motleycrew-0.1.0/motleycrew/tool/tool.py
--rw-r--r--   0        0        0      614 2024-04-19 10:30:25.808545 motleycrew-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3581 1970-01-01 00:00:00.000000 motleycrew-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      145 2024-05-27 12:55:05.190253 motleycrew-0.1.1/README.md
+-rw-r--r--   0        0        0       53 2024-05-21 10:34:37.680086 motleycrew-0.1.1/motleycrew/__init__.py
+-rw-r--r--   0        0        0      135 2024-05-24 08:48:30.495129 motleycrew-0.1.1/motleycrew/agents/__init__.py
+-rw-r--r--   0        0        0      487 2024-05-15 12:11:44.101756 motleycrew-0.1.1/motleycrew/agents/abstract_parent.py
+-rw-r--r--   0        0        0      141 2024-05-15 12:11:44.101852 motleycrew-0.1.1/motleycrew/agents/crewai/__init__.py
+-rw-r--r--   0        0        0     2200 2024-05-16 14:36:06.179031 motleycrew-0.1.1/motleycrew/agents/crewai/agent_with_config.py
+-rw-r--r--   0        0        0     2651 2024-05-24 08:48:30.495596 motleycrew-0.1.1/motleycrew/agents/crewai/crewai.py
+-rw-r--r--   0        0        0     1716 2024-05-21 10:34:37.682259 motleycrew-0.1.1/motleycrew/agents/crewai/crewai_agent.py
+-rw-r--r--   0        0        0      142 2024-05-21 10:34:37.682423 motleycrew-0.1.1/motleycrew/agents/langchain/__init__.py
+-rw-r--r--   0        0        0     3996 2024-05-27 12:52:47.846043 motleycrew-0.1.1/motleycrew/agents/langchain/langchain.py
+-rw-r--r--   0        0        0     7770 2024-05-24 08:48:30.497640 motleycrew-0.1.1/motleycrew/agents/langchain/openai_tools_react.py
+-rw-r--r--   0        0        0     1111 2024-05-26 14:34:10.745868 motleycrew-0.1.1/motleycrew/agents/langchain/react.py
+-rw-r--r--   0        0        0      105 2024-05-21 10:34:37.683449 motleycrew-0.1.1/motleycrew/agents/llama_index/__init__.py
+-rw-r--r--   0        0        0     1795 2024-05-24 08:48:30.498486 motleycrew-0.1.1/motleycrew/agents/llama_index/llama_index.py
+-rw-r--r--   0        0        0     1791 2024-05-24 08:48:30.498726 motleycrew-0.1.1/motleycrew/agents/llama_index/llama_index_react.py
+-rw-r--r--   0        0        0     4617 2024-05-27 12:54:12.875533 motleycrew-0.1.1/motleycrew/agents/parent.py
+-rw-r--r--   0        0        0        0 2024-05-15 07:11:07.625750 motleycrew-0.1.1/motleycrew/applications/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 07:11:07.625844 motleycrew-0.1.1/motleycrew/applications/research_agent/__init__.py
+-rw-r--r--   0        0        0     1723 2024-05-27 12:54:12.875989 motleycrew-0.1.1/motleycrew/applications/research_agent/answer_task.py
+-rw-r--r--   0        0        0     1026 2024-05-21 10:34:37.685104 motleycrew-0.1.1/motleycrew/applications/research_agent/question.py
+-rw-r--r--   0        0        0     4602 2024-05-27 12:22:47.948226 motleycrew-0.1.1/motleycrew/applications/research_agent/question_answerer.py
+-rw-r--r--   0        0        0     5807 2024-05-27 12:54:12.876196 motleycrew-0.1.1/motleycrew/applications/research_agent/question_generator.py
+-rw-r--r--   0        0        0     4255 2024-05-15 12:11:44.104459 motleycrew-0.1.1/motleycrew/applications/research_agent/question_prioritizer.py
+-rw-r--r--   0        0        0     2931 2024-05-27 12:54:12.876335 motleycrew-0.1.1/motleycrew/applications/research_agent/question_task.py
+-rw-r--r--   0        0        0     2520 2024-05-03 09:18:26.693503 motleycrew-0.1.1/motleycrew/caching/2024-05-03_13-18-26/2024-05-03_13-18-26.pkl
+-rw-r--r--   0        0        0     2840 2024-05-03 09:18:28.337412 motleycrew-0.1.1/motleycrew/caching/2024-05-03_13-18-26/2024-05-03_13-18-28.pkl
+-rw-r--r--   0        0        0     4372 2024-05-03 09:18:31.764846 motleycrew-0.1.1/motleycrew/caching/2024-05-03_13-18-26/2024-05-03_13-18-31.pkl
+-rw-r--r--   0        0        0     4231 2024-05-03 09:18:32.128876 motleycrew-0.1.1/motleycrew/caching/2024-05-03_13-18-26/2024-05-03_13-18-32.pkl
+-rw-r--r--   0        0        0     7067 2024-05-03 09:18:54.694931 motleycrew-0.1.1/motleycrew/caching/2024-05-03_13-18-26/2024-05-03_13-18-54.pkl
+-rw-r--r--   0        0        0      355 2024-05-27 12:54:12.876594 motleycrew-0.1.1/motleycrew/common/__init__.py
+-rw-r--r--   0        0        0      456 2024-05-23 12:20:41.080735 motleycrew-0.1.1/motleycrew/common/defaults.py
+-rw-r--r--   0        0        0      473 2024-05-21 10:34:37.688106 motleycrew-0.1.1/motleycrew/common/enums.py
+-rw-r--r--   0        0        0     2061 2024-05-24 08:48:30.500198 motleycrew-0.1.1/motleycrew/common/exceptions.py
+-rw-r--r--   0        0        0     1493 2024-05-21 10:34:37.688478 motleycrew-0.1.1/motleycrew/common/llms.py
+-rw-r--r--   0        0        0      512 2024-05-27 12:54:12.876695 motleycrew-0.1.1/motleycrew/common/logging.py
+-rw-r--r--   0        0        0      496 2024-05-24 08:48:30.500743 motleycrew-0.1.1/motleycrew/common/types.py
+-rw-r--r--   0        0        0     1445 2024-05-27 12:54:12.877296 motleycrew-0.1.1/motleycrew/common/utils.py
+-rw-r--r--   0        0        0     6274 2024-05-27 12:54:12.877570 motleycrew-0.1.1/motleycrew/crew.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:31:59.156086 motleycrew-0.1.1/motleycrew/kuzu_db/.lock
+-rw-r--r--   0        0        0        0 2024-05-14 16:32:00.127631 motleycrew-0.1.1/motleycrew/kuzu_db/.wal
+-rw-r--r--   0        0        0      737 2024-05-14 16:31:59.196900 motleycrew-0.1.1/motleycrew/kuzu_db/catalog.kz
+-rw-r--r--   0        0        0  5795840 2024-05-14 16:32:00.127613 motleycrew-0.1.1/motleycrew/kuzu_db/data.kz
+-rw-r--r--   0        0        0   589824 2024-05-14 16:32:00.126829 motleycrew-0.1.1/motleycrew/kuzu_db/metadata.kz
+-rw-r--r--   0        0        0      557 2024-05-14 16:31:59.874035 motleycrew-0.1.1/motleycrew/kuzu_db/nodes.statistics_and_deleted.ids
+-rw-r--r--   0        0        0      396 2024-05-14 16:31:59.427789 motleycrew-0.1.1/motleycrew/kuzu_db/rels.statistics
+-rw-r--r--   0        0        0      179 2024-05-15 07:11:07.628327 motleycrew-0.1.1/motleycrew/storage/__init__.py
+-rw-r--r--   0        0        0     1500 2024-05-15 07:11:07.628508 motleycrew-0.1.1/motleycrew/storage/graph_node.py
+-rw-r--r--   0        0        0     3519 2024-05-27 12:22:47.948891 motleycrew-0.1.1/motleycrew/storage/graph_store.py
+-rw-r--r--   0        0        0      823 2024-05-27 12:54:12.877705 motleycrew-0.1.1/motleycrew/storage/graph_store_utils.py
+-rw-r--r--   0        0        0    21034 2024-05-27 12:54:12.877853 motleycrew-0.1.1/motleycrew/storage/kuzu_graph_store.py
+-rw-r--r--   0        0        0      248 2024-05-21 10:34:37.688985 motleycrew-0.1.1/motleycrew/tasks/__init__.py
+-rw-r--r--   0        0        0     3954 2024-05-27 12:54:12.878007 motleycrew-0.1.1/motleycrew/tasks/simple.py
+-rw-r--r--   0        0        0     5727 2024-05-27 12:22:47.950197 motleycrew-0.1.1/motleycrew/tasks/task.py
+-rw-r--r--   0        0        0     1269 2024-05-21 10:34:37.690529 motleycrew-0.1.1/motleycrew/tasks/task_unit.py
+-rw-r--r--   0        0        0      270 2024-05-27 12:22:47.950724 motleycrew-0.1.1/motleycrew/tools/__init__.py
+-rw-r--r--   0        0        0     2552 2024-05-23 12:20:41.083826 motleycrew-0.1.1/motleycrew/tools/autogen_chat_tool.py
+-rw-r--r--   0        0        0        0 2024-05-27 12:22:47.950782 motleycrew-0.1.1/motleycrew/tools/image/__init__.py
+-rw-r--r--   0        0        0     5236 2024-05-27 12:54:12.878228 motleycrew-0.1.1/motleycrew/tools/image/dall_e.py
+-rw-r--r--   0        0        0     1906 2024-05-20 06:50:36.818970 motleycrew-0.1.1/motleycrew/tools/llm_tool.py
+-rw-r--r--   0        0        0     3291 2024-05-23 12:20:41.084432 motleycrew-0.1.1/motleycrew/tools/mermaid_evaluator_tool.py
+-rw-r--r--   0        0        0      847 2024-05-23 12:20:41.084715 motleycrew-0.1.1/motleycrew/tools/python_repl.py
+-rw-r--r--   0        0        0     2890 2024-05-23 12:20:41.085052 motleycrew-0.1.1/motleycrew/tools/simple_retriever_tool.py
+-rw-r--r--   0        0        0        0 2024-04-26 09:57:58.418285 motleycrew-0.1.1/motleycrew/tools/test1/.lock
+-rw-r--r--   0        0        0        0 2024-04-26 09:57:58.450438 motleycrew-0.1.1/motleycrew/tools/test1/.wal
+-rw-r--r--   0        0        0      342 2024-04-26 09:57:58.433976 motleycrew-0.1.1/motleycrew/tools/test1/catalog.kz
+-rw-r--r--   0        0        0  1814528 2024-04-26 09:57:58.450295 motleycrew-0.1.1/motleycrew/tools/test1/data.kz
+-rw-r--r--   0        0        0   425984 2024-04-26 09:57:58.450334 motleycrew-0.1.1/motleycrew/tools/test1/metadata.kz
+-rw-r--r--   0        0        0      237 2024-04-26 09:57:58.449111 motleycrew-0.1.1/motleycrew/tools/test1/nodes.statistics_and_deleted.ids
+-rw-r--r--   0        0        0      303 2024-04-26 09:57:58.450388 motleycrew-0.1.1/motleycrew/tools/test1/rels.statistics
+-rw-r--r--   0        0        0     3069 2024-05-24 08:48:30.502368 motleycrew-0.1.1/motleycrew/tools/tool.py
+-rw-r--r--   0        0        0       89 2024-04-24 12:30:04.639837 motleycrew-0.1.1/motleycrew/tracking/__init__.py
+-rw-r--r--   0        0        0     8544 2024-05-27 12:54:12.878643 motleycrew-0.1.1/motleycrew/tracking/callbacks.py
+-rw-r--r--   0        0        0     3839 2024-05-27 12:54:12.878769 motleycrew-0.1.1/motleycrew/tracking/utils.py
+-rw-r--r--   0        0        0     1241 2024-05-27 12:56:13.626010 motleycrew-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1452 1970-01-01 00:00:00.000000 motleycrew-0.1.1/PKG-INFO
```

### Comparing `motleycrew-0.1.0/motleycrew/agent/langchain/langchain.py` & `motleycrew-0.1.1/motleycrew/agents/langchain/langchain.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,122 +1,109 @@
 from typing import Any, Optional, Sequence, Callable
 
 from langchain.agents import AgentExecutor
 from langchain_core.runnables import RunnableConfig
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.prompts.chat import ChatPromptTemplate
 
-from motleycrew.agent.parent import MotleyAgentAbstractParent
-from motleycrew.agent.shared import MotleyAgentParent
-from motleycrew.tasks import Task
+from motleycrew.agents.parent import MotleyAgentParent
+from motleycrew.agents.abstract_parent import MotleyAgentAbstractParent
 
-from motleycrew.tool import MotleyTool
+from motleycrew.tools import MotleyTool
+from motleycrew.tracking import add_default_callbacks_to_langchain_config
 from motleycrew.common import MotleySupportedTool
 from motleycrew.common import MotleyAgentFactory
 from motleycrew.common import LLMFramework
 from motleycrew.common.llms import init_llm
 
 
-class LangchainMotleyAgentParent(MotleyAgentParent):
+class LangchainMotleyAgent(MotleyAgentParent):
     def __init__(
         self,
-        goal: str,
+        description: str,
         name: str | None = None,
         agent_factory: MotleyAgentFactory | None = None,
-        delegation: bool | Sequence[MotleyAgentAbstractParent] = False,
         tools: Sequence[MotleySupportedTool] | None = None,
         verbose: bool = False,
     ):
         super().__init__(
-            goal=goal,
+            description=description,
             name=name,
             agent_factory=agent_factory,
-            delegation=delegation,
             tools=tools,
-            verbose=verbose
+            verbose=verbose,
         )
 
     def invoke(
         self,
-        task: Task | str,
+        task_dict: dict,
         config: Optional[RunnableConfig] = None,
         **kwargs: Any,
-    ) -> Task:
+    ) -> Any:
         self.materialize()
-        self.agent: AgentExecutor
 
-        if isinstance(task, str):
-            assert self.crew, "can't create a task outside a crew"
-            # TODO: feed in context/task.message_history correctly
-            # TODO: attach the current task, if any, as a dependency of the new task
-            task = Task(
-                description=task,
-                name=task,
-                agent=self,
-                crew=self.crew
-            )
-        elif not isinstance(task, Task):
-            raise ValueError(f"`task` must be a string or a Task, not {type(task)}")
-
-        out = self.agent.invoke({"input": task.description}, config, **kwargs)
-        task.outputs = [out["output"]]
-        return task
+        prompt = task_dict.get("prompt")
+        if not prompt:
+            raise ValueError("Task must have a prompt")
+
+        config = add_default_callbacks_to_langchain_config(config)
+
+        result = self.agent.invoke({"input": prompt}, config, **kwargs)
+        output = result.get("output")
+        if output is None:
+            raise Exception("Agent {} result does not contain output: {}".format(self, result))
+        return output
 
     @staticmethod
     def from_function(
         function: Callable[..., Any],
-        goal: str,
+        description: str,
+        name: str | None = None,
         llm: BaseLanguageModel | None = None,
         delegation: bool | Sequence[MotleyAgentAbstractParent] = False,
         tools: Sequence[MotleySupportedTool] | None = None,
         prompt: ChatPromptTemplate | Sequence[ChatPromptTemplate] | None = None,
         require_tools: bool = False,
         verbose: bool = False,
-    ) -> "LangchainMotleyAgentParent":
+    ) -> "LangchainMotleyAgent":
         if llm is None:
             llm = init_llm(llm_framework=LLMFramework.LANGCHAIN)
 
         if require_tools and not tools:
             raise ValueError("You must provide at least one tool to the ReactMotleyAgent")
 
         def agent_factory(tools: dict[str, MotleyTool]):
             langchain_tools = [t.to_langchain_tool() for t in tools.values()]
-            # TODO: feed goal into the agent's prompt
+            # TODO: feed description into the agent's prompt
             agent = function(llm=llm, tools=langchain_tools, prompt=prompt)
             agent_executor = AgentExecutor(
                 agent=agent,
                 tools=langchain_tools,
                 verbose=verbose,
             )
             return agent_executor
 
-        return LangchainMotleyAgentParent(
-            goal=goal,
+        return LangchainMotleyAgent(
+            description=description,
+            name=name,
             agent_factory=agent_factory,
-            delegation=delegation,
             tools=tools,
             verbose=verbose,
         )
 
     @staticmethod
     def from_agent(
         agent: AgentExecutor,
         goal: str,
-        delegation: bool | Sequence[MotleyAgentAbstractParent] = False,
         tools: Sequence[MotleySupportedTool] | None = None,
-        verbose: bool = False
-    ) -> "LangchainMotleyAgentParent":
+        verbose: bool = False,
+    ) -> "LangchainMotleyAgent":
         # TODO: do we really need to unite the tools implicitly like this?
         # TODO: confused users might pass tools both ways at the same time
         # TODO: and we will silently unite them, which can have side effects (e.g. doubled tools)
         # TODO: besides, getting tools can be tricky for other frameworks (e.g. LlamaIndex)
         if tools or agent.tools:
             tools = list(tools or []) + list(agent.tools or [])
 
-        wrapped_agent = LangchainMotleyAgentParent(
-            goal=goal,
-            delegation=delegation,
-            tools=tools,
-            verbose=verbose
-        )
+        wrapped_agent = LangchainMotleyAgent(description=goal, tools=tools, verbose=verbose)
         wrapped_agent._agent = agent
         return wrapped_agent
```

### Comparing `motleycrew-0.1.0/motleycrew/agent/langchain/openai_tools_react.py` & `motleycrew-0.1.1/motleycrew/agents/langchain/openai_tools_react.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 from langchain_core.prompts.chat import ChatPromptTemplate
 from langchain_core.runnables import Runnable, RunnablePassthrough, RunnableLambda
 from langchain_core.tools import BaseTool
 from langchain_core.utils.function_calling import convert_to_openai_tool
 from langchain.tools.render import render_text_description
 from langchain_core.agents import AgentFinish, AgentActionMessageLog
 
-from langchain.agents.format_scratchpad.openai_tools import format_to_openai_tool_messages
+from langchain.agents.format_scratchpad.openai_tools import (
+    format_to_openai_tool_messages,
+)
 from langchain.agents.output_parsers.openai_tools import OpenAIToolsAgentOutputParser
 
-from motleycrew.agent.parent import MotleyAgentAbstractParent
-from motleycrew.agent.langchain.langchain import LangchainMotleyAgentParent
+from motleycrew.agents.abstract_parent import MotleyAgentAbstractParent
+from motleycrew.agents.langchain.langchain import LangchainMotleyAgent
 from motleycrew.common import MotleySupportedTool
-
+from motleycrew.common.utils import print_passthrough
 
 default_think_prompt = ChatPromptTemplate.from_template(
     """
 Answer the following questions as best you can; think carefully, one step at a time, and outline the next step
 towards answering the question.
 
 You will later have access to the following tools:
@@ -63,18 +65,14 @@
 
 Question: {input}
 Thought:{agent_scratchpad}
 """
 )
 
 
-def print_passthrough(x):
-    return x
-
-
 def add_thought_to_background(x: dict):
     out = x["background"]
     out["agent_scratchpad"] += [x["thought"]]
     return out
 
 
 def check_variables(prompt: ChatPromptTemplate):
@@ -176,17 +174,15 @@
         | RunnableLambda(print_passthrough)
         | OpenAIToolsAgentOutputParser()
     )
 
     agent = (
         RunnableLambda(print_passthrough)
         | RunnablePassthrough.assign(
-            agent_scratchpad=lambda x: format_to_openai_tool_messages(
-                x["intermediate_steps"]
-            )
+            agent_scratchpad=lambda x: format_to_openai_tool_messages(x["intermediate_steps"])
         )
         | {"thought": think_prompt | llm, "background": RunnablePassthrough()}
         | RunnableLambda(print_passthrough)
         | {"action": second_llm_call, "thought": RunnableLambda(lambda x: x["thought"])}
         | RunnableLambda(print_passthrough)
         | RunnableLambda(lambda x: add_messages_to_action(x["action"], [x["thought"]]))
         | RunnableLambda(print_passthrough)
@@ -199,27 +195,27 @@
 ) -> List[AgentActionMessageLog] | AgentFinish:
     if not isinstance(actions, AgentFinish):
         for action in actions:
             action.message_log = messages + list(action.message_log)
     return actions
 
 
-class ReactOpenAIToolsAgent(LangchainMotleyAgentParent):
+class ReactOpenAIToolsAgent(LangchainMotleyAgent):
     def __new__(
         cls,
         tools: Sequence[MotleySupportedTool],
         goal: str = "",  # gets ignored at the moment
+        name: str | None = None,
         prompt: ChatPromptTemplate | Sequence[ChatPromptTemplate] | None = None,
         llm: BaseLanguageModel | None = None,
-        delegation: bool | Sequence[MotleyAgentAbstractParent] = False,
         verbose: bool = False,
     ):
         return cls.from_function(
-            goal=goal,
+            description=goal,
+            name=name,
             llm=llm,
-            delegation=delegation,
             tools=tools,
             prompt=prompt,
             function=create_openai_tools_react_agent,
             require_tools=True,
             verbose=verbose,
         )
```

### Comparing `motleycrew-0.1.0/motleycrew/agent/langchain/react.py` & `motleycrew-0.1.1/motleycrew/agents/langchain/react.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from typing import Sequence
 
 from langchain import hub
 from langchain_core.language_models import BaseLanguageModel
 from langchain.agents import create_react_agent
 
-from motleycrew.agent.parent import MotleyAgentAbstractParent
-from motleycrew.agent.langchain.langchain import LangchainMotleyAgentParent
+from motleycrew.agents.abstract_parent import MotleyAgentAbstractParent
+from motleycrew.agents.langchain.langchain import LangchainMotleyAgent
 from motleycrew.common import MotleySupportedTool
 
 
-class ReactMotleyAgent(LangchainMotleyAgentParent):
+class ReactMotleyAgent(LangchainMotleyAgent):
     def __new__(
         cls,
         tools: Sequence[MotleySupportedTool],
-        goal: str = "",  # gets ignored at the moment
+        description: str = "",  # gets ignored at the moment
+        name: str | None = None,
         prompt: str | None = None,
         llm: BaseLanguageModel | None = None,
-        delegation: bool | Sequence[MotleyAgentAbstractParent] = False,
         verbose: bool = False,
     ):
         if prompt is None:
-            # TODO: feed goal into the agent's prompt
+            # TODO: feed description into the agent's prompt
             prompt = hub.pull("hwchase17/react")
         return cls.from_function(
-            goal=goal,
+            description=description,
+            name=name,
             llm=llm,
-            delegation=delegation,
             tools=tools,
             prompt=prompt,
             function=create_react_agent,
             require_tools=True,
             verbose=verbose,
         )
```

### Comparing `motleycrew-0.1.0/motleycrew/agent/llama_index/llama_index_react.py` & `motleycrew-0.1.1/motleycrew/agents/llama_index/llama_index_react.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,51 @@
 from typing import Sequence
-from llama_index.core.agent import ReActAgent
-from llama_index.core.llms import LLM
 
-from motleycrew.agent.llama_index import LlamaIndexMotleyAgentParent
-from motleycrew.agent.parent import MotleyAgentAbstractParent
-from motleycrew.tool import MotleyTool
+try:
+    from llama_index.core.agent import ReActAgent
+    from llama_index.core.llms import LLM
+    from llama_index.core.callbacks import CallbackManager
+except ImportError:
+    LLM = object
+
+from motleycrew.agents.llama_index import LlamaIndexMotleyAgent
+from motleycrew.agents.abstract_parent import MotleyAgentAbstractParent
+from motleycrew.tools import MotleyTool
 from motleycrew.common import MotleySupportedTool
 from motleycrew.common import LLMFramework
 from motleycrew.common.llms import init_llm
+from motleycrew.tracking import get_default_callbacks_list
+from motleycrew.common.utils import ensure_module_is_installed
 
 
-class ReActLlamaIndexMotleyAgent(LlamaIndexMotleyAgentParent):
-    def __init__(self,
-                 goal: str,
-                 name: str | None = None,
-                 delegation: bool | Sequence[MotleyAgentAbstractParent] = False,
-                 tools: Sequence[MotleySupportedTool] | None = None,
-                 llm: LLM | None = None,
-                 verbose: bool = False):
+class ReActLlamaIndexMotleyAgent(LlamaIndexMotleyAgent):
+    def __init__(
+        self,
+        description: str,
+        name: str | None = None,
+        tools: Sequence[MotleySupportedTool] | None = None,
+        llm: LLM | None = None,
+        verbose: bool = False,
+    ):
+        ensure_module_is_installed("llama_index")
         if llm is None:
             llm = init_llm(llm_framework=LLMFramework.LLAMA_INDEX)
 
         def agent_factory(tools: dict[str, MotleyTool]):
             llama_index_tools = [t.to_llama_index_tool() for t in tools.values()]
-            # TODO: feed goal into the agent's prompt
+            # TODO: feed description into the agent's prompt
+            callbacks = get_default_callbacks_list(LLMFramework.LLAMA_INDEX)
             agent = ReActAgent.from_tools(
                 tools=llama_index_tools,
                 llm=llm,
                 verbose=verbose,
+                callback_manager=CallbackManager(callbacks),
             )
             return agent
 
         super().__init__(
-            goal=goal,
+            description=description,
             name=name,
             agent_factory=agent_factory,
-            delegation=delegation,
             tools=tools,
-            verbose=verbose
+            verbose=verbose,
         )
```

### Comparing `motleycrew-0.1.0/motleycrew/agent/shared.py` & `motleycrew-0.1.1/motleycrew/agents/parent.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,113 +1,127 @@
-import logging
-import json
-from typing import TYPE_CHECKING, Any, Sequence
+from typing import TYPE_CHECKING, Optional, Sequence
 
 from langchain_core.tools import Tool
+from langchain_core.runnables import Runnable
+from pydantic import BaseModel
 
-from motleycrew.agent.parent import MotleyAgentAbstractParent
-from motleycrew.tasks import Task
-from motleycrew.tool import MotleyTool
-
-from motleycrew.common import MotleySupportedTool
-from motleycrew.common import MotleyAgentFactory
-from motleycrew.common.exceptions import AgentNotMaterialized
-from motleycrew.common.exceptions import CannotModifyMaterializedAgent
+from motleycrew.agents.abstract_parent import MotleyAgentAbstractParent
+from motleycrew.tools import MotleyTool
+from motleycrew.common import MotleyAgentFactory, MotleySupportedTool
+from motleycrew.common.exceptions import AgentNotMaterialized, CannotModifyMaterializedAgent
+from motleycrew.common import logger
 
 if TYPE_CHECKING:
-    from motleycrew.crew import MotleyCrew
+    from motleycrew import MotleyCrew
 
 
-class MotleyAgentParent(MotleyAgentAbstractParent):
+class MotleyAgentParent(MotleyAgentAbstractParent, Runnable):
     def __init__(
         self,
-        goal: str,
+        description: str,
         name: str | None = None,
         agent_factory: MotleyAgentFactory | None = None,
-        delegation: bool | Sequence[MotleyAgentAbstractParent] = False,
         tools: Sequence[MotleySupportedTool] | None = None,
         verbose: bool = False,
     ):
-        self.name = name or goal
-        self.goal = goal  # becomes tool description
+        self.name = name or description
+        self.description = description  # becomes tool description
         self.agent_factory = agent_factory
-        self.delegation = delegation  # will be init'd at crew creation
         self.tools: dict[str, MotleyTool] = {}
         self.verbose = verbose
         self.crew: MotleyCrew | None = None
 
         self._agent = None
 
         if tools:
             self.add_tools(tools)
 
+    def __repr__(self):
+        return f"Agent(name={self.name})"
+
+    def __str__(self):
+        return self.__repr__()
+
     @property
     def agent(self):
         """
         Getter for the inner agent that makes sure it's already materialized.
-        The inner agent should always be accesed via this property method.
+        The inner agent should always be accessed via this property method.
         """
         if not self.is_materialized:
             raise AgentNotMaterialized(agent_name=self.name)
         return self._agent
 
     @property
     def is_materialized(self):
         return self._agent is not None
 
     def materialize(self):
         if self.is_materialized:
-            logging.info("Agent is already materialized, skipping materialization")
+            logger.info("Agent is already materialized, skipping materialization")
             return
         assert self.agent_factory, "Cannot materialize agent without a factory provided"
         self._agent = self.agent_factory(tools=self.tools)
 
     def add_tools(self, tools: Sequence[MotleySupportedTool]):
-        if self.is_materialized:
+        if self.is_materialized and tools:
             raise CannotModifyMaterializedAgent(agent_name=self.name)
 
         for t in tools:
             motley_tool = MotleyTool.from_supported_tool(t)
             if motley_tool.name not in self.tools:
                 self.tools[motley_tool.name] = motley_tool
 
-    def as_tool(self) -> MotleyTool:
+    def as_tool(self, input_schema: Optional[BaseModel] = None) -> MotleyTool:
+        def call_agent(*args, **kwargs):
+            # TODO: this thing is hacky, we should have a better way to pass structured input
+            if args:
+                return self.invoke({"prompt": args[0]})
+            if len(kwargs) == 1:
+                return self.invoke({"prompt": list(kwargs.values())[0]})
+            return self.invoke(kwargs)
+
         # To be specialized if we expect structured input
         return MotleyTool.from_langchain_tool(
-            Tool(name=self.name, description=self.goal, func=self.call_as_tool)
+            Tool(
+                name=self.name,
+                description=self.description,
+                func=call_agent,
+                args_schema=input_schema,
+            )
         )
 
-    def call_as_tool(self, *args, **kwargs) -> Any:
-        logging.info("Entering delegation for %s", self.name)
-        assert self.crew, "can't accept delegated task outside of a crew"
-
-        if len(args) > 0:
-            input_ = args[0]
-        elif "tool_input" in kwargs:
-            # Is this a crewai notation?
-            input_ = kwargs["tool_input"]
-        else:
-            input_ = json.dumps(kwargs)
-
-        logging.info("Made the args: %s", input_)
-
-        # TODO: pass context of parent task to agent nicely?
-        # TODO: mark the current task as depending on the new task
-        task = Task(
-            description=input_,
-            name=input_,
-            agent=self,
-            # TODO inject the new subtask as a dep and reschedule the parent
-            # TODO probably can't do this from here since we won't know if
-            # there are other tasks to schedule
-            crew=self.crew,
-        )
-
-        # TODO: make sure tools return task objects, which are properly used by callers
-        logging.info("Executing subtask '%s'", task.name)
-        self.crew.task_graph.set_task_running(task=task)
-        result = self.crew.execute(task, return_result=True)
-
-        logging.info("Finished subtask '%s' - %s", task.name, result)
-        self.crew.task_graph.set_task_done(task=task)
-
-        return result
+    # def call_as_tool(self, *args, **kwargs) -> Any:
+    #     logger.info("Entering delegation for %s", self.name)
+    #     assert self.crew, "can't accept delegated task outside of a crew"
+    #
+    #     if len(args) > 0:
+    #         input_ = args[0]
+    #     elif "tool_input" in kwargs:
+    #         # Is this a crewai notation?
+    #         input_ = kwargs["tool_input"]
+    #     else:
+    #         input_ = json.dumps(kwargs)
+    #
+    #     logger.info("Made the args: %s", input_)
+    #
+    #     # TODO: pass context of parent task to agent nicely?
+    #     # TODO: mark the current task as depending on the new task
+    #     task = SimpleTaskRecipe(
+    #         description=input_,
+    #         name=input_,
+    #         agent=self,
+    #         # TODO inject the new subtask as a dep and reschedule the parent
+    #         # TODO probably can't do this from here since we won't know if
+    #         # there are other tasks to schedule
+    #         crew=self.crew,
+    #     )
+    #
+    #     # TODO: make sure tools return task objects, which are properly used by callers
+    #     logger.info("Executing subtask '%s'", task.name)
+    #     self.crew.task_graph.set_task_running(task=task)
+    #     result = self.crew.execute(task, return_result=True)
+    #
+    #     logger.info("Finished subtask '%s' - %s", task.name, result)
+    #     self.crew.task_graph.set_task_done(task=task)
+    #
+    #     return result
```

### Comparing `motleycrew-0.1.0/motleycrew/common/llms.py` & `motleycrew-0.1.1/motleycrew/common/llms.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 from motleycrew.common import Defaults
 from motleycrew.common import LLMFamily, LLMFramework
 from motleycrew.common.exceptions import LLMFamilyNotSupported, LLMFrameworkNotSupported
+from motleycrew.common.utils import ensure_module_is_installed
 
 
 def langchain_openai_llm(
     llm_name: str = Defaults.DEFAULT_LLM_NAME,
     llm_temperature: float = Defaults.DEFAULT_LLM_TEMPERATURE,
+    **kwargs,
 ):
     from langchain_openai import ChatOpenAI
 
-    return ChatOpenAI(model=llm_name, temperature=llm_temperature)
+    return ChatOpenAI(model=llm_name, temperature=llm_temperature, **kwargs)
 
 
 def llama_index_openai_llm(
     llm_name: str = Defaults.DEFAULT_LLM_NAME,
     llm_temperature: float = Defaults.DEFAULT_LLM_TEMPERATURE,
+    **kwargs,
 ):
+    ensure_module_is_installed("llama_index")
     from llama_index.llms.openai import OpenAI
 
-    return OpenAI(model=llm_name, temperature=llm_temperature)
+    return OpenAI(model=llm_name, temperature=llm_temperature, **kwargs)
 
 
 Defaults.LLM_MAP = {
     (LLMFramework.LANGCHAIN, LLMFamily.OPENAI): langchain_openai_llm,
     (LLMFramework.LLAMA_INDEX, LLMFamily.OPENAI): llama_index_openai_llm,
 }
 
 
 def init_llm(
     llm_framework: str,
     llm_family: str = Defaults.DEFAULT_LLM_FAMILY,
     llm_name: str = Defaults.DEFAULT_LLM_NAME,
     llm_temperature: float = Defaults.DEFAULT_LLM_TEMPERATURE,
+    **kwargs,
 ):
 
     func = Defaults.LLM_MAP.get((llm_framework, llm_family), None)
     if func is not None:
-        return func(llm_name=llm_name, llm_temperature=llm_temperature)
+        return func(llm_name=llm_name, llm_temperature=llm_temperature, **kwargs)
 
     raise LLMFamilyNotSupported(llm_framework=llm_framework, llm_family=llm_family)
```

### Comparing `motleycrew-0.1.0/motleycrew/tool/llm_tool.py` & `motleycrew-0.1.1/motleycrew/tools/llm_tool.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,64 @@
-from typing import Optional
+from typing import Optional, Type
 
-from langchain_core.tools import Tool
+from langchain_core.tools import StructuredTool
 from langchain_core.prompts import PromptTemplate
+from langchain_core.prompts.base import BasePromptTemplate
 from langchain_core.language_models import BaseLanguageModel
-from langchain_core.pydantic_v1 import BaseModel, Field
+from langchain_core.pydantic_v1 import BaseModel, Field, create_model
 
-from motleycrew.tool import MotleyTool
+from motleycrew.tools import MotleyTool
 from motleycrew.common import LLMFramework
 from motleycrew.common.llms import init_llm
 
 
 class LLMTool(MotleyTool):
     def __init__(
         self,
         name: str,
         description: str,
-        prompt: str,
+        prompt: str | BasePromptTemplate,
         llm: Optional[BaseLanguageModel] = None,
+        input_schema: Optional[Type[BaseModel]] = None,
     ):
-        langchain_tool = create_llm_langchain_tool(name, description, prompt, llm)
+        langchain_tool = create_llm_langchain_tool(
+            name=name,
+            description=description,
+            prompt=prompt,
+            llm=llm,
+            input_schema=input_schema,
+        )
         super().__init__(langchain_tool)
 
 
 def create_llm_langchain_tool(
     name: str,
     description: str,
-    prompt: str,
+    prompt: str | BasePromptTemplate,
     llm: Optional[BaseLanguageModel] = None,
-    input_description: Optional[str] = "Input for the tool.",
+    input_schema: Optional[Type[BaseModel]] = None,
 ):
     if llm is None:
         llm = init_llm(llm_framework=LLMFramework.LANGCHAIN)
 
-    class LLMToolInput(BaseModel):
-        """Input for the tool."""
+    if not isinstance(prompt, BasePromptTemplate):
+        prompt = PromptTemplate.from_template(prompt)
 
-        input: str = Field(description=input_description)
+    if input_schema is None:
+        fields = {
+            var: (str, Field(description=f"Input {var} for the tool."))
+            for var in prompt.input_variables
+        }
+
+        # Create the LLMToolInput class dynamically
+        input_schema = create_model("LLMToolInput", **fields)
+
+    def call_llm(**kwargs) -> str:
+        chain = prompt | llm
+        return chain.invoke(kwargs)
 
-    p = PromptTemplate.from_template(prompt)
-    assert "input" in p.input_variables, "Prompt must contain an `input` variable"
-
-    def call_llm(input: str) -> str:
-        chain = p | llm
-        return chain.invoke({"input": input})
-
-    return Tool.from_function(
+    return StructuredTool.from_function(
         func=call_llm,
         name=name,
         description=description,
-        args_schema=LLMToolInput,
+        args_schema=input_schema,
     )
```

### Comparing `motleycrew-0.1.0/motleycrew/tool/tool.py` & `motleycrew-0.1.1/motleycrew/tools/tool.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,91 @@
-from typing import Union
+from typing import Union, Annotated
 
 from langchain.tools import BaseTool
+from langchain_core.runnables import Runnable
 
-from llama_index.core.tools import BaseTool as LlamaIndex__BaseTool
-from llama_index.core.tools import FunctionTool as LlamaIndex__FunctionTool
+try:
+    from llama_index.core.tools import BaseTool as LlamaIndex__BaseTool
+    from llama_index.core.tools import FunctionTool as LlamaIndex__FunctionTool
+except ImportError:
+    LlamaIndex__BaseTool = None
+
+from motleycrew.common.utils import ensure_module_is_installed
+from motleycrew.agents.abstract_parent import MotleyAgentAbstractParent
 
 
 def normalize_input(args, kwargs):
     if "tool_input" in kwargs:
         return kwargs["tool_input"]
     else:
         return args[0]
 
 
-class MotleyTool:
+class MotleyTool(Runnable):
     """
     Base tool class compatible with MotleyAgents.
     It is a wrapper for LangChain's BaseTool, containing all necessary adapters and converters.
     """
+
     def __init__(self, tool: BaseTool):
         self.tool = tool
 
     @property
     def name(self):
-        #TODO: do we really want to make a thin wrapper in this fashion?
+        # TODO: do we really want to make a thin wrapper in this fashion?
         return self.tool.name
 
     def invoke(self, *args, **kwargs):
         return self.tool.invoke(*args, **kwargs)
 
     @staticmethod
     def from_langchain_tool(langchain_tool: BaseTool) -> "MotleyTool":
         return MotleyTool(tool=langchain_tool)
 
     @staticmethod
     def from_llama_index_tool(llama_index_tool: LlamaIndex__BaseTool) -> "MotleyTool":
+        ensure_module_is_installed("llama_index")
         langchain_tool = llama_index_tool.to_langchain_tool()
         return MotleyTool.from_langchain_tool(langchain_tool=langchain_tool)
 
     @staticmethod
-    def from_supported_tool(tool: Union["MotleyTool", BaseTool, LlamaIndex__BaseTool]):
+    def from_supported_tool(
+        tool: Union["MotleyTool", BaseTool, LlamaIndex__BaseTool, MotleyAgentAbstractParent]
+    ):
         if isinstance(tool, MotleyTool):
             return tool
         elif isinstance(tool, BaseTool):
             return MotleyTool.from_langchain_tool(tool)
         elif isinstance(tool, LlamaIndex__BaseTool):
             return MotleyTool.from_llama_index_tool(tool)
+        elif isinstance(tool, MotleyAgentAbstractParent):
+            return tool.as_tool()
         else:
-            raise Exception(f"Tool type `{type(tool)}` is not supported, please convert to MotleyTool first")
+            raise Exception(
+                f"Tool type `{type(tool)}` is not supported, please convert to MotleyTool first"
+            )
 
     def to_langchain_tool(self) -> BaseTool:
         return self.tool
 
     def to_llama_index_tool(self) -> LlamaIndex__BaseTool:
+        ensure_module_is_installed("llama_index")
         llama_index_tool = LlamaIndex__FunctionTool.from_defaults(
             fn=self.tool._run,
             name=self.tool.name,
             description=self.tool.description,
-            fn_schema=self.tool.args_schema
+            fn_schema=self.tool.args_schema,
         )
         return llama_index_tool
+
+    def to_autogen_tool(self):
+        fields = list(self.tool.args_schema.__fields__.values())
+        if len(fields) != 1:
+            raise Exception("Multiple input fields are not supported in to_autogen_tool")
+
+        field_name = fields[0].name
+        field_type = fields[0].annotation
+
+        def autogen_tool_fn(input: field_type) -> str:
+            return self.invoke({field_name: input})
+
+        return autogen_tool_fn
```

### Comparing `motleycrew-0.1.0/pyproject.toml` & `motleycrew-0.1.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,50 @@
 [tool.poetry]
 name = "motleycrew"
-version = "0.1.0"
+version = "0.1.1"
 description = "A lightweight agent interaction framework."
 authors = ["MotleyCrew <github@motleycrew.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<=3.13"
 langchain = "^0.1"
-crewai = "^0.16"
-setuptools = "^69.2.0"
-duckduckgo-search = "^5.2.1"
-llama-index = "^0.10.27"
+crewai = { version = "^0.16", optional = true }
+setuptools = "^67.6.2"
+duckduckgo-search = "5.3.0b4"
+llama-index = { version = "^0.10.27", optional = true }
 langchain-experimental = "^0.0.57"
+python-dotenv = "^1.0.0"
+lunary = "^1.0.21"
+langchainhub = "^0.1.15"
+kuzu = "^0.4.2"
+cloudpickle = "^3.0.0"
+platformdirs = "^4.2.1"
+pydantic = "^2.7.1"
+# TODO: The following dependencies for caching package should be optional
+requests = "^2.31.0"
+curl-cffi = "^0.6.4"
+httpx = "^0.27.0"
+autogen = {version = "^1.0.16", optional = true}
+motleycache = "^0.0.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.2.0"
 pytest = "^8.0.2"
 pytest-cov = "^4.1.0"
 flake8 = "^7.0.0"
 mypy = "^1.8.0"
 isort = "^5.13.2"
+sphinx = "^7.3.7"
+sphinx-rtd-theme = "^2.0.0"
+nbsphinx = "^0.9.4"
+ipykernel = "^6.29.4"
+nbsphinx-link = "^1.3.0"
+nbformat = "^5.10.4"
+
+[tool.poetry.extras]
+crewai = ["crewai"]
+llama-index = ["llama-index"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

