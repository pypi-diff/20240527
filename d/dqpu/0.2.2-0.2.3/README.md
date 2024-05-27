# Comparing `tmp/dqpu-0.2.2.tar.gz` & `tmp/dqpu-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dqpu-0.2.2.tar", last modified: Thu May 23 09:50:06 2024, max compression
+gzip compressed data, was "dqpu-0.2.3.tar", last modified: Mon May 27 05:50:24 2024, max compression
```

## Comparing `dqpu-0.2.2.tar` & `dqpu-0.2.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-23 09:50:06.379837 dqpu-0.2.2/
--rw-r--r--   0 dakk      (1000) dakk      (1000)    10255 2024-04-30 07:00:05.000000 dqpu-0.2.2/LICENSE
--rw-r--r--   0 dakk      (1000) dakk      (1000)     9223 2024-05-23 09:50:06.379837 dqpu-0.2.2/PKG-INFO
--rw-r--r--   0 dakk      (1000) dakk      (1000)     8395 2024-05-22 10:59:29.000000 dqpu-0.2.2/README.md
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-23 09:50:06.369836 dqpu-0.2.2/dqpu/
--rw-r--r--   0 dakk      (1000) dakk      (1000)      593 2024-05-23 09:47:45.000000 dqpu-0.2.2/dqpu/__init__.py
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-23 09:50:06.373170 dqpu-0.2.2/dqpu/backends/
--rw-r--r--   0 dakk      (1000) dakk      (1000)      569 2024-05-17 14:08:15.000000 dqpu-0.2.2/dqpu/backends/__init__.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1234 2024-05-19 08:07:22.000000 dqpu-0.2.2/dqpu/backends/base.py
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-23 09:50:06.373170 dqpu-0.2.2/dqpu/backends/qiskit/
--rw-r--r--   0 dakk      (1000) dakk      (1000)      717 2024-05-17 11:37:05.000000 dqpu-0.2.2/dqpu/backends/qiskit/__init__.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     4026 2024-05-23 09:22:47.000000 dqpu-0.2.2/dqpu/backends/qiskit/dqpubackend.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     3288 2024-05-20 10:03:30.000000 dqpu-0.2.2/dqpu/backends/qiskit/dqpujob.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1198 2024-05-19 08:07:22.000000 dqpu-0.2.2/dqpu/backends/qiskit/dqpuprovider.py
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-23 09:50:06.373170 dqpu-0.2.2/dqpu/blockchain/
--rw-r--r--   0 dakk      (1000) dakk      (1000)      726 2024-05-15 08:24:53.000000 dqpu-0.2.2/dqpu/blockchain/__init__.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1531 2024-05-22 06:01:25.000000 dqpu-0.2.2/dqpu/blockchain/blockchain.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     2495 2024-05-22 14:41:31.000000 dqpu-0.2.2/dqpu/blockchain/ipfs_gateway.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     6404 2024-05-23 09:41:09.000000 dqpu-0.2.2/dqpu/blockchain/near.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     7006 2024-05-23 09:41:33.000000 dqpu-0.2.2/dqpu/cli.py
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-23 09:50:06.376503 dqpu-0.2.2/dqpu/q/
--rw-r--r--   0 dakk      (1000) dakk      (1000)      801 2024-05-07 07:05:38.000000 dqpu-0.2.2/dqpu/q/__init__.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     6613 2024-05-23 09:41:41.000000 dqpu-0.2.2/dqpu/q/circuit.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1260 2024-05-23 08:49:53.000000 dqpu-0.2.2/dqpu/q/gate.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     2322 2024-05-23 09:22:47.000000 dqpu-0.2.2/dqpu/q/gates.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     2262 2024-05-14 10:21:28.000000 dqpu-0.2.2/dqpu/q/utils.py
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-23 09:50:06.376503 dqpu-0.2.2/dqpu/sampler/
--rw-r--r--   0 dakk      (1000) dakk      (1000)      969 2024-05-23 09:41:33.000000 dqpu-0.2.2/dqpu/sampler/__init__.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1072 2024-05-23 09:22:47.000000 dqpu-0.2.2/dqpu/sampler/aersimulatorsampler.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     5943 2024-05-15 10:21:58.000000 dqpu-0.2.2/dqpu/sampler/dasksimulatorsampler.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1185 2024-05-23 09:22:47.000000 dqpu-0.2.2/dqpu/sampler/qracksimulatorsampler.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1484 2024-05-22 06:06:47.000000 dqpu-0.2.2/dqpu/sampler/sampler.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     6025 2024-05-23 09:22:47.000000 dqpu-0.2.2/dqpu/samplernode.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1636 2024-05-23 09:22:47.000000 dqpu-0.2.2/dqpu/utils.py
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-23 09:50:06.376503 dqpu-0.2.2/dqpu/verifier/
--rw-r--r--   0 dakk      (1000) dakk      (1000)      691 2024-05-07 08:01:59.000000 dqpu-0.2.2/dqpu/verifier/__init__.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     4158 2024-05-23 09:33:18.000000 dqpu-0.2.2/dqpu/verifier/basictrapper.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     2322 2024-05-19 07:59:25.000000 dqpu-0.2.2/dqpu/verifier/trapper.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)      652 2024-05-07 05:50:44.000000 dqpu-0.2.2/dqpu/verifier/verifier.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     6374 2024-05-23 09:41:33.000000 dqpu-0.2.2/dqpu/verifiernode.py
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-23 09:50:06.373170 dqpu-0.2.2/dqpu.egg-info/
--rw-r--r--   0 dakk      (1000) dakk      (1000)     9223 2024-05-23 09:50:06.000000 dqpu-0.2.2/dqpu.egg-info/PKG-INFO
--rw-r--r--   0 dakk      (1000) dakk      (1000)      987 2024-05-23 09:50:06.000000 dqpu-0.2.2/dqpu.egg-info/SOURCES.txt
--rw-r--r--   0 dakk      (1000) dakk      (1000)        1 2024-05-23 09:50:06.000000 dqpu-0.2.2/dqpu.egg-info/dependency_links.txt
--rw-r--r--   0 dakk      (1000) dakk      (1000)      190 2024-05-23 09:50:06.000000 dqpu-0.2.2/dqpu.egg-info/entry_points.txt
--rw-r--r--   0 dakk      (1000) dakk      (1000)        1 2024-05-23 09:50:06.000000 dqpu-0.2.2/dqpu.egg-info/not-zip-safe
--rw-r--r--   0 dakk      (1000) dakk      (1000)      194 2024-05-23 09:50:06.000000 dqpu-0.2.2/dqpu.egg-info/requires.txt
--rw-r--r--   0 dakk      (1000) dakk      (1000)        5 2024-05-23 09:50:06.000000 dqpu-0.2.2/dqpu.egg-info/top_level.txt
--rw-r--r--   0 dakk      (1000) dakk      (1000)      382 2024-05-23 09:50:06.379837 dqpu-0.2.2/setup.cfg
--rw-r--r--   0 dakk      (1000) dakk      (1000)     3198 2024-05-22 05:34:05.000000 dqpu-0.2.2/setup.py
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-23 09:50:06.379837 dqpu-0.2.2/test/
--rw-r--r--   0 dakk      (1000) dakk      (1000)      741 2024-05-07 08:37:08.000000 dqpu-0.2.2/test/test_empty.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-27 05:50:24.467845 dqpu-0.2.3/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)    10255 2024-04-30 07:00:05.000000 dqpu-0.2.3/LICENSE
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     6958 2024-05-27 05:50:24.467845 dqpu-0.2.3/PKG-INFO
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     6130 2024-05-25 07:42:18.000000 dqpu-0.2.3/README.md
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-27 05:50:24.461178 dqpu-0.2.3/dqpu/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      593 2024-05-27 05:48:50.000000 dqpu-0.2.3/dqpu/__init__.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-27 05:50:24.461178 dqpu-0.2.3/dqpu/backends/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      569 2024-05-17 14:08:15.000000 dqpu-0.2.3/dqpu/backends/__init__.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1234 2024-05-19 08:07:22.000000 dqpu-0.2.3/dqpu/backends/base.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-27 05:50:24.464512 dqpu-0.2.3/dqpu/backends/qiskit/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      717 2024-05-17 11:37:05.000000 dqpu-0.2.3/dqpu/backends/qiskit/__init__.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     4026 2024-05-23 09:22:47.000000 dqpu-0.2.3/dqpu/backends/qiskit/dqpubackend.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     3288 2024-05-20 10:03:30.000000 dqpu-0.2.3/dqpu/backends/qiskit/dqpujob.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1198 2024-05-19 08:07:22.000000 dqpu-0.2.3/dqpu/backends/qiskit/dqpuprovider.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-27 05:50:24.464512 dqpu-0.2.3/dqpu/blockchain/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      726 2024-05-15 08:24:53.000000 dqpu-0.2.3/dqpu/blockchain/__init__.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1531 2024-05-22 06:01:25.000000 dqpu-0.2.3/dqpu/blockchain/blockchain.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     2495 2024-05-22 14:41:31.000000 dqpu-0.2.3/dqpu/blockchain/ipfs_gateway.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     6404 2024-05-23 09:41:09.000000 dqpu-0.2.3/dqpu/blockchain/near.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     7053 2024-05-25 13:21:17.000000 dqpu-0.2.3/dqpu/cli.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-27 05:50:24.464512 dqpu-0.2.3/dqpu/q/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      801 2024-05-07 07:05:38.000000 dqpu-0.2.3/dqpu/q/__init__.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     6613 2024-05-23 09:41:41.000000 dqpu-0.2.3/dqpu/q/circuit.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1260 2024-05-23 08:49:53.000000 dqpu-0.2.3/dqpu/q/gate.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     2322 2024-05-23 09:22:47.000000 dqpu-0.2.3/dqpu/q/gates.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     2262 2024-05-14 10:21:28.000000 dqpu-0.2.3/dqpu/q/utils.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-27 05:50:24.467845 dqpu-0.2.3/dqpu/sampler/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      969 2024-05-23 09:41:33.000000 dqpu-0.2.3/dqpu/sampler/__init__.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1072 2024-05-23 09:22:47.000000 dqpu-0.2.3/dqpu/sampler/aersimulatorsampler.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     5943 2024-05-15 10:21:58.000000 dqpu-0.2.3/dqpu/sampler/dasksimulatorsampler.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1185 2024-05-23 09:22:47.000000 dqpu-0.2.3/dqpu/sampler/qracksimulatorsampler.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1484 2024-05-22 06:06:47.000000 dqpu-0.2.3/dqpu/sampler/sampler.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     6025 2024-05-23 09:22:47.000000 dqpu-0.2.3/dqpu/samplernode.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1636 2024-05-23 09:22:47.000000 dqpu-0.2.3/dqpu/utils.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-27 05:50:24.467845 dqpu-0.2.3/dqpu/verifier/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      691 2024-05-07 08:01:59.000000 dqpu-0.2.3/dqpu/verifier/__init__.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     4158 2024-05-23 09:33:18.000000 dqpu-0.2.3/dqpu/verifier/basictrapper.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     2322 2024-05-19 07:59:25.000000 dqpu-0.2.3/dqpu/verifier/trapper.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      652 2024-05-07 05:50:44.000000 dqpu-0.2.3/dqpu/verifier/verifier.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     6374 2024-05-23 09:41:33.000000 dqpu-0.2.3/dqpu/verifiernode.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-27 05:50:24.461178 dqpu-0.2.3/dqpu.egg-info/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     6958 2024-05-27 05:50:24.000000 dqpu-0.2.3/dqpu.egg-info/PKG-INFO
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      987 2024-05-27 05:50:24.000000 dqpu-0.2.3/dqpu.egg-info/SOURCES.txt
+-rw-r--r--   0 dakk      (1000) dakk      (1000)        1 2024-05-27 05:50:24.000000 dqpu-0.2.3/dqpu.egg-info/dependency_links.txt
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      190 2024-05-27 05:50:24.000000 dqpu-0.2.3/dqpu.egg-info/entry_points.txt
+-rw-r--r--   0 dakk      (1000) dakk      (1000)        1 2024-05-27 05:50:23.000000 dqpu-0.2.3/dqpu.egg-info/not-zip-safe
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      194 2024-05-27 05:50:24.000000 dqpu-0.2.3/dqpu.egg-info/requires.txt
+-rw-r--r--   0 dakk      (1000) dakk      (1000)        5 2024-05-27 05:50:24.000000 dqpu-0.2.3/dqpu.egg-info/top_level.txt
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      382 2024-05-27 05:50:24.471179 dqpu-0.2.3/setup.cfg
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     3198 2024-05-22 05:34:05.000000 dqpu-0.2.3/setup.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-27 05:50:24.467845 dqpu-0.2.3/test/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      741 2024-05-07 08:37:08.000000 dqpu-0.2.3/test/test_empty.py
```

### Comparing `dqpu-0.2.2/LICENSE` & `dqpu-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.2/PKG-INFO` & `dqpu-0.2.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dqpu
-Version: 0.2.2
+Version: 0.2.3
 Home-page: https://github.com/dakk/dqpu
 Author: Davide Gessa
 Author-email: gessadavide@gmail.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/dakk/dqpu/issues/
 Project-URL: Documentation, https://dakk.github.io/dqpu
 Project-URL: Source, https://github.com/dakk/dqpu
@@ -26,15 +26,15 @@
 ![Contract CI Status](https://github.com/dakk/dqpu/actions/workflows/ci-contract.yaml/badge.svg)
 ![PyPI - Version](https://img.shields.io/pypi/v/dqpu)
 ![License: Apache 2.0](https://img.shields.io/badge/license-Apache_2.0-blue)
 [![Downloads](https://static.pepy.tech/badge/dqpu)](https://pepy.tech/project/dqpu)
 
 A Web3-Powered (Near), Decentralized Quantum Simulator with Verifiable Computation. 
 
-DQPU (Decentralized Quantum Processing Unit) introduces a novel, decentralized approach to quantum computing that leverages the power of blockchain and smart contracts. It addresses the challenges of securely and reliably executing quantum computations in a trustless and transparent manner, while fostering a competitive ecosystem for quantum resource providers.
+DQPU (Decentralized Quantum Processing Unit) introduces a novel, decentralized approach to quantum computing that leverages the power of blockchain and smart contracts. It addresses the challenge of securely and reliably delegating the execution of quantum computations in a trustless and transparent manner, encouraging competition between independent quantum resource providers.
 
 
 ## Workflow
 
 The DQPU system is composed of 3 actors:
 
 - *Clients*: users who need to perform a quantum sampling paying a reward
@@ -58,15 +58,15 @@
 [^1]: In this first version of the contract, *Verifiers* are trusted entities designated by the smart contract creator.
 [^2]: This step will become private in future versions of the protocol.
 [^3]: In the next version of the protocol, the client will also add its trap in order to check *verifier*'s loyalty.
 
 
 ## Smart Contract Web UI
 
-A web interface showing the smart contract status is available here: [https://dakk.github.io/dqpu/app/](https://dakk.github.io/dqpu/app/)
+A web interface showing the smart contract status is available here: [https://dqpu.io/app](https://dqpu.io/app)
 
 
 ## Installation
 
 ```pip install dqpu```
 
 Or install the latest development version:
@@ -137,117 +137,20 @@
 counts = job_result(nb, ipfs, jid)
 print(counts)
 ```
 
 
 ### Cli tool usage
 
-Generic params:
-- ```-n/--network`: Default: near-testnet
-- ```-a/--account`: Account name / uri
+Read [dqpu.io/docs/cli](https://dqpu.io/docs/cli.html) for details.
 
-Commands:
 
-#### Submit a circuit job 
+## Usage: running a sampler / verifier node node
 
-```bash
-$ dqpu-cli -a dqpu_alice.testnet submit --file ~/test.qasm --shots 1024 --reward 0.0001
-JOBID
-```
-
-#### Submit a random circuit: job
-
-```bash
-$ dqpu-cli -a dqpu_alice.testnet submit-random
-JOBID
-```
-
-#### Submit a job result
-
-```bash
-$ dpqu-cli -a dqpu_bob.testnet submit-result -i 8 -rf ~/test.qasm
-```
-
-#### Remove a job
-
-```bash
-$ dpqu-cli remove -i JOBID
-```
-
-#### Get job information
-
-```bash
-$ dpqu-cli info -i JOBID
-Job: JOBID
-Status: WAITING
-Qubits: 4
-Depth: 9
-Circuit uri: ipfs://.../test.qasm
-```
-
-#### Get job status
-
-```bash
-$ dpqu-cli status -i JOBID
-EXECUTED
-```
-
-#### Get job result
-
-```bash
-$ dpqu-cli get-result -i JOBID
-{ "0010": 1024 }
-```
-
-#### Set job validity
-
-```bash
-$ dpqu-cli -a dqpu_owner.testnet set-validity -i 9 -v false
-```
-
-#### Set job result validity
-```bash
-$ dpqu-cli -a dqpu_owner.testnet set-result-validity -i 8 -v true -t trap.json
-```
-
-
-## Usage: running a sampler node
-
-A sampler node continuously pool the DQPU smart contract waiting for new job. When a new job appear,
-the sampler checks if it can perform the sampling with its hardware. 
-
-Every sampler node can implement its own `Sampler` class, adding supports to other simulators or 
-to real quantum hardware. DQPU package offer 3 implementation:
-- AerSimulator: statevector simulator from qiskit
-- DaskSimulator: statevector simulator using Dask distributed computing library
-- NumpySimulator: statevector simulator using Numpy
-
-After every sampled job, the node receives the reward.
-
-```bash
-dqpu-sampler -a sampler_account --max-deposit 0.1 --sampler aersimulator --max-qubits 21
-```
-
-Read more on [README_SAMPLER.md](README_SAMPLER.md).
-
-## Usage: running a verifier node
-
-A verifier node continuously pool the DQPU smart contract waiting for new 'pending-validation' and 'validating-result' jobs. When a new job appear, the verifiers:
-- 'pending-validation' job are checked for quantum circuit validity, and trap qubits are inserted
-- 'validating-result' job are checked for trap verification
-
-After every validation, the verifier receives a percentage of the job reward.
-
-Verifier are special users initially selected by the smart contract creator; this will change in the future.
-
-```bash
-dqpu-verifier -a verifier_account
-```
-
-Read more on [README_VERIFIER.md](README_VERIFIER.md).
+Read [dqpu.io/nodes](https://dqpu.io/nodes) for details.
 
 
 ## Contributing
 
 Read [CONTRIBUTING](CONTRIBUTING.md) for details.
 
 ## License
```

### Comparing `dqpu-0.2.2/README.md` & `dqpu-0.2.3/dqpu.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,40 @@
+Metadata-Version: 2.1
+Name: dqpu
+Version: 0.2.3
+Home-page: https://github.com/dakk/dqpu
+Author: Davide Gessa
+Author-email: gessadavide@gmail.com
+License: Apache 2.0
+Project-URL: Bug Tracker, https://github.com/dakk/dqpu/issues/
+Project-URL: Documentation, https://dakk.github.io/dqpu
+Project-URL: Source, https://github.com/dakk/dqpu
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Operating System :: OS Independent
+Requires-Python: >= 3.9.2
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # dqpu
 
 ![CI Status](https://github.com/dakk/dqpu/actions/workflows/ci.yaml/badge.svg)
 ![Contract CI Status](https://github.com/dakk/dqpu/actions/workflows/ci-contract.yaml/badge.svg)
 ![PyPI - Version](https://img.shields.io/pypi/v/dqpu)
 ![License: Apache 2.0](https://img.shields.io/badge/license-Apache_2.0-blue)
 [![Downloads](https://static.pepy.tech/badge/dqpu)](https://pepy.tech/project/dqpu)
 
 A Web3-Powered (Near), Decentralized Quantum Simulator with Verifiable Computation. 
 
-DQPU (Decentralized Quantum Processing Unit) introduces a novel, decentralized approach to quantum computing that leverages the power of blockchain and smart contracts. It addresses the challenges of securely and reliably executing quantum computations in a trustless and transparent manner, while fostering a competitive ecosystem for quantum resource providers.
+DQPU (Decentralized Quantum Processing Unit) introduces a novel, decentralized approach to quantum computing that leverages the power of blockchain and smart contracts. It addresses the challenge of securely and reliably delegating the execution of quantum computations in a trustless and transparent manner, encouraging competition between independent quantum resource providers.
 
 
 ## Workflow
 
 The DQPU system is composed of 3 actors:
 
 - *Clients*: users who need to perform a quantum sampling paying a reward
@@ -36,15 +58,15 @@
 [^1]: In this first version of the contract, *Verifiers* are trusted entities designated by the smart contract creator.
 [^2]: This step will become private in future versions of the protocol.
 [^3]: In the next version of the protocol, the client will also add its trap in order to check *verifier*'s loyalty.
 
 
 ## Smart Contract Web UI
 
-A web interface showing the smart contract status is available here: [https://dakk.github.io/dqpu/app/](https://dakk.github.io/dqpu/app/)
+A web interface showing the smart contract status is available here: [https://dqpu.io/app](https://dqpu.io/app)
 
 
 ## Installation
 
 ```pip install dqpu```
 
 Or install the latest development version:
@@ -115,117 +137,20 @@
 counts = job_result(nb, ipfs, jid)
 print(counts)
 ```
 
 
 ### Cli tool usage
 
-Generic params:
-- ```-n/--network`: Default: near-testnet
-- ```-a/--account`: Account name / uri
-
-Commands:
-
-#### Submit a circuit job 
-
-```bash
-$ dqpu-cli -a dqpu_alice.testnet submit --file ~/test.qasm --shots 1024 --reward 0.0001
-JOBID
-```
-
-#### Submit a random circuit: job
-
-```bash
-$ dqpu-cli -a dqpu_alice.testnet submit-random
-JOBID
-```
-
-#### Submit a job result
-
-```bash
-$ dpqu-cli -a dqpu_bob.testnet submit-result -i 8 -rf ~/test.qasm
-```
-
-#### Remove a job
-
-```bash
-$ dpqu-cli remove -i JOBID
-```
-
-#### Get job information
-
-```bash
-$ dpqu-cli info -i JOBID
-Job: JOBID
-Status: WAITING
-Qubits: 4
-Depth: 9
-Circuit uri: ipfs://.../test.qasm
-```
-
-#### Get job status
-
-```bash
-$ dpqu-cli status -i JOBID
-EXECUTED
-```
+Read [dqpu.io/docs/cli](https://dqpu.io/docs/cli.html) for details.
 
-#### Get job result
 
-```bash
-$ dpqu-cli get-result -i JOBID
-{ "0010": 1024 }
-```
-
-#### Set job validity
-
-```bash
-$ dpqu-cli -a dqpu_owner.testnet set-validity -i 9 -v false
-```
-
-#### Set job result validity
-```bash
-$ dpqu-cli -a dqpu_owner.testnet set-result-validity -i 8 -v true -t trap.json
-```
-
-
-## Usage: running a sampler node
-
-A sampler node continuously pool the DQPU smart contract waiting for new job. When a new job appear,
-the sampler checks if it can perform the sampling with its hardware. 
-
-Every sampler node can implement its own `Sampler` class, adding supports to other simulators or 
-to real quantum hardware. DQPU package offer 3 implementation:
-- AerSimulator: statevector simulator from qiskit
-- DaskSimulator: statevector simulator using Dask distributed computing library
-- NumpySimulator: statevector simulator using Numpy
-
-After every sampled job, the node receives the reward.
-
-```bash
-dqpu-sampler -a sampler_account --max-deposit 0.1 --sampler aersimulator --max-qubits 21
-```
-
-Read more on [README_SAMPLER.md](README_SAMPLER.md).
-
-## Usage: running a verifier node
-
-A verifier node continuously pool the DQPU smart contract waiting for new 'pending-validation' and 'validating-result' jobs. When a new job appear, the verifiers:
-- 'pending-validation' job are checked for quantum circuit validity, and trap qubits are inserted
-- 'validating-result' job are checked for trap verification
-
-After every validation, the verifier receives a percentage of the job reward.
-
-Verifier are special users initially selected by the smart contract creator; this will change in the future.
-
-```bash
-dqpu-verifier -a verifier_account
-```
+## Usage: running a sampler / verifier node node
 
-Read more on [README_VERIFIER.md](README_VERIFIER.md).
+Read [dqpu.io/nodes](https://dqpu.io/nodes) for details.
 
 
 ## Contributing
 
 Read [CONTRIBUTING](CONTRIBUTING.md) for details.
 
 ## License
@@ -246,8 +171,8 @@
 
 ## About the author
 
 Davide Gessa (dakk)
 - https://twitter.com/dagide
 - https://mastodon.social/@dagide 
 - https://dakk.github.io/
-- https://medium.com/@dakk
+- https://medium.com/@dakk
```

### Comparing `dqpu-0.2.2/dqpu/__init__.py` & `dqpu-0.2.3/dqpu/verifier/verifier.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,9 +8,8 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-
-__version__ = "0.2.2"
+# TODO: A serializable class that hold all the things needed for verifing results
```

### Comparing `dqpu-0.2.2/dqpu/backends/__init__.py` & `dqpu-0.2.3/dqpu/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.2/dqpu/backends/base.py` & `dqpu-0.2.3/dqpu/backends/base.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.2/dqpu/backends/qiskit/__init__.py` & `dqpu-0.2.3/dqpu/backends/qiskit/__init__.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.2/dqpu/backends/qiskit/dqpubackend.py` & `dqpu-0.2.3/dqpu/backends/qiskit/dqpubackend.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.2/dqpu/backends/qiskit/dqpujob.py` & `dqpu-0.2.3/dqpu/backends/qiskit/dqpujob.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.2/dqpu/backends/qiskit/dqpuprovider.py` & `dqpu-0.2.3/dqpu/backends/qiskit/dqpuprovider.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.2/dqpu/blockchain/__init__.py` & `dqpu-0.2.3/dqpu/blockchain/__init__.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.2/dqpu/blockchain/blockchain.py` & `dqpu-0.2.3/dqpu/blockchain/blockchain.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.2/dqpu/blockchain/ipfs_gateway.py` & `dqpu-0.2.3/dqpu/blockchain/ipfs_gateway.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.2/dqpu/blockchain/near.py` & `dqpu-0.2.3/dqpu/blockchain/near.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.2/dqpu/cli.py` & `dqpu-0.2.3/dqpu/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,16 +163,18 @@
         print("Submitting...")
 
         # Upload job_file
         job_file = ipfs.upload(circuit_file)
         print(f"Circuit file is {job_file}")
 
         shots = random.choice([256, 512, 1024, 2048, 4096, 8192, 16384])
-        sh_fact = (shots / 16384) * nq
-        reward = random.randint(int(0.5 * sh_fact), int(1.1 * sh_fact)) / 1000.0
+        
+        # sh_fact = (shots / 16384) * nq
+        # reward = random.randint(int(0.5 * sh_fact), int(1.1 * sh_fact)) / 1000.0
+        reward = nq * nq / 600000
         reward = max(reward, 0.0001)
 
         print(f"Submitting with a reward of {reward:.6f} for {shots} shots")
 
         print(nb.submit_job(nq, dpt, shots, job_file, reward))
         print(f"Account balance is {nb.balance():0.5f} N")
         print(nb.get_latest_jobs()[-1]["id"])
```

### Comparing `dqpu-0.2.2/dqpu/q/__init__.py` & `dqpu-0.2.3/dqpu/q/__init__.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.2/dqpu/q/circuit.py` & `dqpu-0.2.3/dqpu/q/circuit.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.2/dqpu/q/gate.py` & `dqpu-0.2.3/dqpu/q/gate.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.2/dqpu/q/gates.py` & `dqpu-0.2.3/dqpu/q/gates.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.2/dqpu/q/utils.py` & `dqpu-0.2.3/dqpu/q/utils.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.2/dqpu/sampler/__init__.py` & `dqpu-0.2.3/dqpu/sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.2/dqpu/sampler/aersimulatorsampler.py` & `dqpu-0.2.3/dqpu/sampler/aersimulatorsampler.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.2/dqpu/sampler/dasksimulatorsampler.py` & `dqpu-0.2.3/dqpu/sampler/dasksimulatorsampler.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.2/dqpu/sampler/qracksimulatorsampler.py` & `dqpu-0.2.3/dqpu/sampler/qracksimulatorsampler.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.2/dqpu/sampler/sampler.py` & `dqpu-0.2.3/dqpu/sampler/sampler.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.2/dqpu/samplernode.py` & `dqpu-0.2.3/dqpu/samplernode.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.2/dqpu/utils.py` & `dqpu-0.2.3/dqpu/utils.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.2/dqpu/verifier/__init__.py` & `dqpu-0.2.3/dqpu/verifier/__init__.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.2/dqpu/verifier/basictrapper.py` & `dqpu-0.2.3/dqpu/verifier/basictrapper.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.2/dqpu/verifier/trapper.py` & `dqpu-0.2.3/dqpu/verifier/trapper.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.2/dqpu/verifier/verifier.py` & `dqpu-0.2.3/dqpu/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,8 +8,9 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# TODO: A serializable class that hold all the things needed for verifing results
+
+__version__ = "0.2.3"
```

### Comparing `dqpu-0.2.2/dqpu/verifiernode.py` & `dqpu-0.2.3/dqpu/verifiernode.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.2/dqpu.egg-info/SOURCES.txt` & `dqpu-0.2.3/dqpu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.2/setup.py` & `dqpu-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.2/test/test_empty.py` & `dqpu-0.2.3/test/test_empty.py`

 * *Files identical despite different names*

