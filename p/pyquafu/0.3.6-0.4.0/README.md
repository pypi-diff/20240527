# Comparing `tmp/pyquafu-0.3.6-cp39-cp39-win_amd64.whl.zip` & `tmp/pyquafu-0.4.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,65 +1,119 @@
-Zip file size: 196721 bytes, number of entries: 63
--rw-rw-rw-  2.0 fat      362 b- defN 23-Oct-28 08:24 quafu/__init__.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Oct-28 08:24 quafu/backends/__init__.py
--rw-rw-rw-  2.0 fat     4844 b- defN 23-Oct-28 08:24 quafu/backends/backends.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Oct-28 08:24 quafu/benchmark/__init__.py
--rw-rw-rw-  2.0 fat     2698 b- defN 23-Oct-28 08:24 quafu/benchmark/adder.py
--rw-rw-rw-  2.0 fat     1722 b- defN 23-Oct-28 08:24 quafu/benchmark/deutsch_jozsa.py
--rw-rw-rw-  2.0 fat      266 b- defN 23-Oct-28 08:24 quafu/benchmark/unitary_test.py
--rw-rw-rw-  2.0 fat     1504 b- defN 23-Oct-28 08:24 quafu/benchmark/variational_n4.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Oct-28 08:24 quafu/circuits/__init__.py
--rw-rw-rw-  2.0 fat      939 b- defN 23-Oct-28 08:24 quafu/circuits/para_circuit.py
--rw-rw-rw-  2.0 fat    30117 b- defN 23-Oct-28 08:24 quafu/circuits/quantum_circuit.py
--rw-rw-rw-  2.0 fat        2 b- defN 23-Oct-28 08:24 quafu/dagcircuits/__init__.py
--rw-rw-rw-  2.0 fat    16335 b- defN 23-Oct-28 08:24 quafu/dagcircuits/circuit_dag.py
--rw-rw-rw-  2.0 fat    12136 b- defN 23-Oct-28 08:24 quafu/dagcircuits/dag_circuit.py
--rw-rw-rw-  2.0 fat     1699 b- defN 23-Oct-28 08:24 quafu/dagcircuits/instruction_node.py
--rw-rw-rw-  2.0 fat      198 b- defN 23-Oct-28 08:24 quafu/elements/__init__.py
--rw-rw-rw-  2.0 fat     3601 b- defN 23-Oct-28 08:24 quafu/elements/instruction.py
--rw-rw-rw-  2.0 fat     8219 b- defN 23-Oct-28 08:24 quafu/elements/pulses.py
--rw-rw-rw-  2.0 fat     7337 b- defN 23-Oct-28 08:24 quafu/elements/quantum_gate.py
--rw-rw-rw-  2.0 fat      986 b- defN 23-Oct-28 08:24 quafu/elements/element_gates/__init__.py
--rw-rw-rw-  2.0 fat     2025 b- defN 23-Oct-28 08:24 quafu/elements/element_gates/c11.py
--rw-rw-rw-  2.0 fat      382 b- defN 23-Oct-28 08:24 quafu/elements/element_gates/c12.py
--rw-rw-rw-  2.0 fat     1276 b- defN 23-Oct-28 08:24 quafu/elements/element_gates/clifford.py
--rw-rw-rw-  2.0 fat     1819 b- defN 23-Oct-28 08:24 quafu/elements/element_gates/cm1.py
--rw-rw-rw-  2.0 fat     3115 b- defN 23-Oct-28 08:24 quafu/elements/element_gates/pauli.py
--rw-rw-rw-  2.0 fat      482 b- defN 23-Oct-28 08:24 quafu/elements/element_gates/phase.py
--rw-rw-rw-  2.0 fat     2299 b- defN 23-Oct-28 08:24 quafu/elements/element_gates/rotation.py
--rw-rw-rw-  2.0 fat      997 b- defN 23-Oct-28 08:24 quafu/elements/element_gates/swap.py
--rw-rw-rw-  2.0 fat       45 b- defN 23-Oct-28 08:24 quafu/elements/element_gates/unitary/__init__.py
--rw-rw-rw-  2.0 fat    11713 b- defN 23-Oct-28 08:24 quafu/elements/element_gates/unitary/decomposer.py
--rw-rw-rw-  2.0 fat       86 b- defN 23-Oct-28 08:24 quafu/elements/matrices/__init__.py
--rw-rw-rw-  2.0 fat     5508 b- defN 23-Oct-28 08:24 quafu/elements/matrices/mat_lib.py
--rw-rw-rw-  2.0 fat     3877 b- defN 23-Oct-28 08:24 quafu/elements/matrices/mat_utils.py
--rw-rw-rw-  2.0 fat       30 b- defN 23-Oct-28 08:24 quafu/exceptions/__init__.py
--rw-rw-rw-  2.0 fat      285 b- defN 23-Oct-28 08:24 quafu/exceptions/circuit_error.py
--rw-rw-rw-  2.0 fat      746 b- defN 23-Oct-28 08:24 quafu/exceptions/quafu_error.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Oct-28 08:24 quafu/qfasm/__init__.py
--rw-rw-rw-  2.0 fat      840 b- defN 23-Oct-28 08:24 quafu/qfasm/qfasm_convertor.py
--rw-rw-rw-  2.0 fat     6082 b- defN 23-Oct-28 08:24 quafu/qfasm/qfasm_parser.py
--rw-rw-rw-  2.0 fat     2443 b- defN 23-Oct-28 08:24 quafu/qfasm/qfasmlex.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Oct-28 08:24 quafu/results/__init__.py
--rw-rw-rw-  2.0 fat     6977 b- defN 23-Oct-28 08:24 quafu/results/results.py
--rw-rw-rw-  2.0 fat        1 b- defN 23-Oct-28 08:24 quafu/simulators/__init__.py
--rw-rw-rw-  2.0 fat     3683 b- defN 23-Oct-28 08:24 quafu/simulators/default_simulator.py
--rw-rw-rw-  2.0 fat   322048 b- defN 23-Oct-28 08:24 quafu/simulators/qfvm.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     3915 b- defN 23-Oct-28 08:24 quafu/simulators/simulator.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Oct-28 08:24 quafu/tasks/__init__.py
--rw-rw-rw-  2.0 fat     6081 b- defN 23-Oct-28 08:24 quafu/tasks/task_database.py
--rw-rw-rw-  2.0 fat    13160 b- defN 23-Oct-28 08:24 quafu/tasks/tasks.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Oct-28 08:24 quafu/users/__init__.py
--rw-rw-rw-  2.0 fat      233 b- defN 23-Oct-28 08:24 quafu/users/exceptions.py
--rw-rw-rw-  2.0 fat     4254 b- defN 23-Oct-28 08:24 quafu/users/userapi.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Oct-28 08:24 quafu/utils/__init__.py
--rw-rw-rw-  2.0 fat     1060 b- defN 23-Oct-28 08:24 quafu/utils/basis.py
--rw-rw-rw-  2.0 fat     1234 b- defN 23-Oct-28 08:24 quafu/utils/paulis.py
--rw-rw-rw-  2.0 fat      432 b- defN 23-Oct-28 08:24 quafu/utils/platform.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Oct-28 08:24 quafu/visualisation/__init__.py
--rw-rw-rw-  2.0 fat    22162 b- defN 23-Oct-28 08:24 quafu/visualisation/circuitPlot.py
--rw-rw-rw-  2.0 fat    11556 b- defN 23-Oct-28 08:24 pyquafu-0.3.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2362 b- defN 23-Oct-28 08:24 pyquafu-0.3.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       94 b- defN 23-Oct-28 08:24 pyquafu-0.3.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Oct-28 08:24 pyquafu-0.3.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     5401 b- defN 23-Oct-28 08:24 pyquafu-0.3.6.dist-info/RECORD
-63 files, 541674 bytes uncompressed, 188087 bytes compressed:  65.3%
+Zip file size: 1916874 bytes, number of entries: 117
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-27 13:50 pyquafu-0.4.0.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-27 13:50 quafu/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-27 13:50 pyquafu.libs/
+-rw-r--r--  2.0 unx      142 b- defN 24-May-27 13:50 pyquafu-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 24-May-27 13:50 pyquafu-0.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     8126 b- defN 24-May-27 13:50 pyquafu-0.4.0.dist-info/RECORD
+-rw-r--r--  2.0 unx     2870 b- defN 24-May-27 13:50 pyquafu-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx    11557 b- defN 24-May-27 13:50 pyquafu-0.4.0.dist-info/LICENSE
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-27 13:50 quafu/dagcircuits/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-27 13:50 quafu/exceptions/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-27 13:50 quafu/benchmark/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-27 13:50 quafu/utils/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-27 13:50 quafu/tasks/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-27 13:50 quafu/simulators/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-27 13:50 quafu/results/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-27 13:50 quafu/synthesis/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-27 13:50 quafu/users/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-27 13:50 quafu/qfasm/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-27 13:50 quafu/circuits/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-27 13:50 quafu/visualisation/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-27 13:50 quafu/algorithms/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-27 13:50 quafu/backends/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-27 13:50 quafu/elements/
+-rw-r--r--  2.0 unx      561 b- defN 24-May-27 13:50 quafu/__init__.py
+-rwxr-xr-x  2.0 unx        0 b- defN 24-May-27 13:50 quafu/dagcircuits/__init__.py
+-rw-r--r--  2.0 unx     1559 b- defN 24-May-27 13:50 quafu/dagcircuits/instruction_node.py
+-rw-r--r--  2.0 unx    12528 b- defN 24-May-27 13:50 quafu/dagcircuits/dag_circuit.py
+-rw-r--r--  2.0 unx    14202 b- defN 24-May-27 13:50 quafu/dagcircuits/circuit_dag.py
+-rw-r--r--  2.0 unx      122 b- defN 24-May-27 13:50 quafu/exceptions/__init__.py
+-rw-r--r--  2.0 unx      233 b- defN 24-May-27 13:50 quafu/exceptions/user_error.py
+-rw-r--r--  2.0 unx      264 b- defN 24-May-27 13:50 quafu/exceptions/circuit_error.py
+-rw-r--r--  2.0 unx     1418 b- defN 24-May-27 13:50 quafu/exceptions/utils.py
+-rw-r--r--  2.0 unx      715 b- defN 24-May-27 13:50 quafu/exceptions/quafu_error.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-27 13:50 quafu/benchmark/__init__.py
+-rw-r--r--  2.0 unx     1413 b- defN 24-May-27 13:50 quafu/benchmark/variational_n4.py
+-rw-r--r--  2.0 unx     1758 b- defN 24-May-27 13:50 quafu/benchmark/deutsch_jozsa.py
+-rw-r--r--  2.0 unx      254 b- defN 24-May-27 13:50 quafu/benchmark/unitary_test.py
+-rw-r--r--  2.0 unx     2541 b- defN 24-May-27 13:50 quafu/benchmark/adder.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-27 13:50 quafu/utils/__init__.py
+-rw-r--r--  2.0 unx      445 b- defN 24-May-27 13:50 quafu/utils/platform.py
+-rw-r--r--  2.0 unx     1023 b- defN 24-May-27 13:50 quafu/utils/basis.py
+-rw-r--r--  2.0 unx     1126 b- defN 24-May-27 13:50 quafu/utils/client_wrapper.py
+-rw-r--r--  2.0 unx     1210 b- defN 24-May-27 13:50 quafu/utils/paulis.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-27 13:50 quafu/tasks/__init__.py
+-rw-r--r--  2.0 unx    12740 b- defN 24-May-27 13:50 quafu/tasks/tasks.py
+-rw-r--r--  2.0 unx     5892 b- defN 24-May-27 13:50 quafu/tasks/task_database.py
+-rw-r--r--  2.0 unx     1889 b- defN 24-May-27 13:50 quafu/simulators/__init__.py
+-rw-r--r--  2.0 unx     4236 b- defN 24-May-27 13:50 quafu/simulators/default_simulator.py
+-rw-r--r--  2.0 unx      678 b- defN 24-May-27 13:50 quafu/simulators/torch.py
+-rw-r--r--  2.0 unx     7676 b- defN 24-May-27 13:50 quafu/simulators/simulator.py
+-rwxr-xr-x  2.0 unx  7404825 b- defN 24-May-27 13:50 quafu/simulators/qfvm.cpython-38-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx        0 b- defN 24-May-27 13:50 quafu/results/__init__.py
+-rw-r--r--  2.0 unx     8880 b- defN 24-May-27 13:50 quafu/results/results.py
+-rw-r--r--  2.0 unx       32 b- defN 24-May-27 13:50 quafu/synthesis/__init__.py
+-rw-r--r--  2.0 unx     7191 b- defN 24-May-27 13:50 quafu/synthesis/evolution.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-27 13:50 quafu/users/__init__.py
+-rw-r--r--  2.0 unx     4645 b- defN 24-May-27 13:50 quafu/users/userapi.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-27 13:50 quafu/qfasm/__init__.py
+-rw-r--r--  2.0 unx     2133 b- defN 24-May-27 13:50 quafu/qfasm/qfasm_convertor.py
+-rw-r--r--  2.0 unx     5117 b- defN 24-May-27 13:50 quafu/qfasm/qelib1.inc
+-rw-r--r--  2.0 unx      932 b- defN 24-May-27 13:50 quafu/qfasm/exceptions.py
+-rw-r--r--  2.0 unx     3868 b- defN 24-May-27 13:50 quafu/qfasm/qfasm_utils.py
+-rw-r--r--  2.0 unx    46746 b- defN 24-May-27 13:50 quafu/qfasm/qfasm_parser.py
+-rw-r--r--  2.0 unx     6021 b- defN 24-May-27 13:50 quafu/qfasm/qfasm_lexer.py
+-rw-r--r--  2.0 unx      170 b- defN 24-May-27 13:50 quafu/circuits/__init__.py
+-rw-r--r--  2.0 unx    39798 b- defN 24-May-27 13:50 quafu/circuits/quantum_circuit.py
+-rw-r--r--  2.0 unx     1995 b- defN 24-May-27 13:50 quafu/circuits/classical_register.py
+-rw-r--r--  2.0 unx     2581 b- defN 24-May-27 13:50 quafu/circuits/quantum_register.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-27 13:50 quafu/visualisation/__init__.py
+-rw-r--r--  2.0 unx     3025 b- defN 24-May-27 13:50 quafu/visualisation/bloch_sphere.py
+-rw-r--r--  2.0 unx    20820 b- defN 24-May-27 13:50 quafu/visualisation/circuitPlot.py
+-rw-r--r--  2.0 unx     1592 b- defN 24-May-27 13:50 quafu/visualisation/draw_dag.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-27 13:50 quafu/algorithms/gradients/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-27 13:50 quafu/algorithms/interface/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-27 13:50 quafu/algorithms/templates/
+-rw-r--r--  2.0 unx      373 b- defN 24-May-27 13:50 quafu/algorithms/__init__.py
+-rw-r--r--  2.0 unx     5239 b- defN 24-May-27 13:50 quafu/algorithms/gradient.py
+-rw-r--r--  2.0 unx     5961 b- defN 24-May-27 13:50 quafu/algorithms/hamiltonian.py
+-rw-r--r--  2.0 unx     1044 b- defN 24-May-27 13:50 quafu/algorithms/interface_provider.py
+-rw-r--r--  2.0 unx      642 b- defN 24-May-27 13:50 quafu/algorithms/sampler.py
+-rw-r--r--  2.0 unx     3406 b- defN 24-May-27 13:50 quafu/algorithms/estimator.py
+-rw-r--r--  2.0 unx     5669 b- defN 24-May-27 13:50 quafu/algorithms/ansatz.py
+-rw-r--r--  2.0 unx     2463 b- defN 24-May-27 13:50 quafu/algorithms/optimizer.py
+-rw-r--r--  2.0 unx      700 b- defN 24-May-27 13:50 quafu/algorithms/gradients/__init__.py
+-rw-r--r--  2.0 unx     2176 b- defN 24-May-27 13:50 quafu/algorithms/gradients/param_shift.py
+-rw-r--r--  2.0 unx     4235 b- defN 24-May-27 13:50 quafu/algorithms/gradients/vjp.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-27 13:50 quafu/algorithms/interface/__init__.py
+-rw-r--r--  2.0 unx     2922 b- defN 24-May-27 13:50 quafu/algorithms/interface/torch.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-27 13:50 quafu/algorithms/templates/__init__.py
+-rw-r--r--  2.0 unx     2644 b- defN 24-May-27 13:50 quafu/algorithms/templates/angle.py
+-rw-r--r--  2.0 unx     4764 b- defN 24-May-27 13:50 quafu/algorithms/templates/basic_entangle.py
+-rw-r--r--  2.0 unx     9213 b- defN 24-May-27 13:50 quafu/algorithms/templates/amplitude.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-27 13:50 quafu/backends/__init__.py
+-rw-r--r--  2.0 unx     5053 b- defN 24-May-27 13:50 quafu/backends/backends.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-27 13:50 quafu/elements/matrices/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-27 13:50 quafu/elements/element_gates/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-27 13:50 quafu/elements/unitary/
+-rw-r--r--  2.0 unx      500 b- defN 24-May-27 13:50 quafu/elements/__init__.py
+-rw-r--r--  2.0 unx    17763 b- defN 24-May-27 13:50 quafu/elements/quantum_gate.py
+-rw-r--r--  2.0 unx     1366 b- defN 24-May-27 13:50 quafu/elements/classical_element.py
+-rw-r--r--  2.0 unx     4934 b- defN 24-May-27 13:50 quafu/elements/instruction.py
+-rw-r--r--  2.0 unx     8183 b- defN 24-May-27 13:50 quafu/elements/pulses.py
+-rw-r--r--  2.0 unx     7988 b- defN 24-May-27 13:50 quafu/elements/parameters.py
+-rw-r--r--  2.0 unx     3026 b- defN 24-May-27 13:50 quafu/elements/utils.py
+-rw-r--r--  2.0 unx     5637 b- defN 24-May-27 13:50 quafu/elements/oracle.py
+-rw-r--r--  2.0 unx     3633 b- defN 24-May-27 13:50 quafu/elements/noise.py
+-rw-r--r--  2.0 unx       84 b- defN 24-May-27 13:50 quafu/elements/matrices/__init__.py
+-rw-r--r--  2.0 unx     3754 b- defN 24-May-27 13:50 quafu/elements/matrices/mat_utils.py
+-rw-r--r--  2.0 unx     5421 b- defN 24-May-27 13:50 quafu/elements/matrices/mat_lib.py
+-rw-r--r--  2.0 unx     1017 b- defN 24-May-27 13:50 quafu/elements/element_gates/__init__.py
+-rw-r--r--  2.0 unx      156 b- defN 24-May-27 13:50 quafu/elements/element_gates/pauli.py
+-rw-r--r--  2.0 unx       90 b- defN 24-May-27 13:50 quafu/elements/element_gates/clifford.py
+-rw-r--r--  2.0 unx      116 b- defN 24-May-27 13:50 quafu/elements/element_gates/rotation.py
+-rw-r--r--  2.0 unx    12086 b- defN 24-May-27 13:50 quafu/elements/element_gates/element_gates.py
+-rw-r--r--  2.0 unx       61 b- defN 24-May-27 13:50 quafu/elements/unitary/__init__.py
+-rw-r--r--  2.0 unx    11461 b- defN 24-May-27 13:50 quafu/elements/unitary/decomposer.py
+-rwxr-xr-x  2.0 unx   168193 b- defN 24-May-27 13:50 pyquafu.libs/libgomp-a34b3233.so.1.0.0
+117 files, 7969528 bytes uncompressed, 1901440 bytes compressed:  76.1%
```

## zipnote {}

```diff
@@ -1,190 +1,352 @@
-Filename: quafu/__init__.py
+Filename: pyquafu-0.4.0.dist-info/
 Comment: 
 
-Filename: quafu/backends/__init__.py
+Filename: quafu/
 Comment: 
 
-Filename: quafu/backends/backends.py
+Filename: pyquafu.libs/
 Comment: 
 
-Filename: quafu/benchmark/__init__.py
+Filename: pyquafu-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: quafu/benchmark/adder.py
+Filename: pyquafu-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: quafu/benchmark/deutsch_jozsa.py
+Filename: pyquafu-0.4.0.dist-info/RECORD
 Comment: 
 
-Filename: quafu/benchmark/unitary_test.py
+Filename: pyquafu-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: quafu/benchmark/variational_n4.py
+Filename: pyquafu-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: quafu/circuits/__init__.py
+Filename: quafu/dagcircuits/
 Comment: 
 
-Filename: quafu/circuits/para_circuit.py
+Filename: quafu/exceptions/
 Comment: 
 
-Filename: quafu/circuits/quantum_circuit.py
+Filename: quafu/benchmark/
 Comment: 
 
-Filename: quafu/dagcircuits/__init__.py
+Filename: quafu/utils/
 Comment: 
 
-Filename: quafu/dagcircuits/circuit_dag.py
+Filename: quafu/tasks/
 Comment: 
 
-Filename: quafu/dagcircuits/dag_circuit.py
+Filename: quafu/simulators/
 Comment: 
 
-Filename: quafu/dagcircuits/instruction_node.py
+Filename: quafu/results/
 Comment: 
 
-Filename: quafu/elements/__init__.py
+Filename: quafu/synthesis/
 Comment: 
 
-Filename: quafu/elements/instruction.py
+Filename: quafu/users/
 Comment: 
 
-Filename: quafu/elements/pulses.py
+Filename: quafu/qfasm/
 Comment: 
 
-Filename: quafu/elements/quantum_gate.py
+Filename: quafu/circuits/
 Comment: 
 
-Filename: quafu/elements/element_gates/__init__.py
+Filename: quafu/visualisation/
 Comment: 
 
-Filename: quafu/elements/element_gates/c11.py
+Filename: quafu/algorithms/
 Comment: 
 
-Filename: quafu/elements/element_gates/c12.py
+Filename: quafu/backends/
 Comment: 
 
-Filename: quafu/elements/element_gates/clifford.py
+Filename: quafu/elements/
 Comment: 
 
-Filename: quafu/elements/element_gates/cm1.py
+Filename: quafu/__init__.py
 Comment: 
 
-Filename: quafu/elements/element_gates/pauli.py
+Filename: quafu/dagcircuits/__init__.py
 Comment: 
 
-Filename: quafu/elements/element_gates/phase.py
+Filename: quafu/dagcircuits/instruction_node.py
 Comment: 
 
-Filename: quafu/elements/element_gates/rotation.py
+Filename: quafu/dagcircuits/dag_circuit.py
 Comment: 
 
-Filename: quafu/elements/element_gates/swap.py
+Filename: quafu/dagcircuits/circuit_dag.py
 Comment: 
 
-Filename: quafu/elements/element_gates/unitary/__init__.py
+Filename: quafu/exceptions/__init__.py
 Comment: 
 
-Filename: quafu/elements/element_gates/unitary/decomposer.py
+Filename: quafu/exceptions/user_error.py
 Comment: 
 
-Filename: quafu/elements/matrices/__init__.py
+Filename: quafu/exceptions/circuit_error.py
 Comment: 
 
-Filename: quafu/elements/matrices/mat_lib.py
+Filename: quafu/exceptions/utils.py
 Comment: 
 
-Filename: quafu/elements/matrices/mat_utils.py
+Filename: quafu/exceptions/quafu_error.py
 Comment: 
 
-Filename: quafu/exceptions/__init__.py
+Filename: quafu/benchmark/__init__.py
 Comment: 
 
-Filename: quafu/exceptions/circuit_error.py
+Filename: quafu/benchmark/variational_n4.py
 Comment: 
 
-Filename: quafu/exceptions/quafu_error.py
+Filename: quafu/benchmark/deutsch_jozsa.py
 Comment: 
 
-Filename: quafu/qfasm/__init__.py
+Filename: quafu/benchmark/unitary_test.py
 Comment: 
 
-Filename: quafu/qfasm/qfasm_convertor.py
+Filename: quafu/benchmark/adder.py
 Comment: 
 
-Filename: quafu/qfasm/qfasm_parser.py
+Filename: quafu/utils/__init__.py
 Comment: 
 
-Filename: quafu/qfasm/qfasmlex.py
+Filename: quafu/utils/platform.py
 Comment: 
 
-Filename: quafu/results/__init__.py
+Filename: quafu/utils/basis.py
 Comment: 
 
-Filename: quafu/results/results.py
+Filename: quafu/utils/client_wrapper.py
+Comment: 
+
+Filename: quafu/utils/paulis.py
+Comment: 
+
+Filename: quafu/tasks/__init__.py
+Comment: 
+
+Filename: quafu/tasks/tasks.py
+Comment: 
+
+Filename: quafu/tasks/task_database.py
 Comment: 
 
 Filename: quafu/simulators/__init__.py
 Comment: 
 
 Filename: quafu/simulators/default_simulator.py
 Comment: 
 
-Filename: quafu/simulators/qfvm.cp39-win_amd64.pyd
+Filename: quafu/simulators/torch.py
 Comment: 
 
 Filename: quafu/simulators/simulator.py
 Comment: 
 
-Filename: quafu/tasks/__init__.py
+Filename: quafu/simulators/qfvm.cpython-38-x86_64-linux-gnu.so
 Comment: 
 
-Filename: quafu/tasks/task_database.py
+Filename: quafu/results/__init__.py
 Comment: 
 
-Filename: quafu/tasks/tasks.py
+Filename: quafu/results/results.py
 Comment: 
 
-Filename: quafu/users/__init__.py
+Filename: quafu/synthesis/__init__.py
+Comment: 
+
+Filename: quafu/synthesis/evolution.py
 Comment: 
 
-Filename: quafu/users/exceptions.py
+Filename: quafu/users/__init__.py
 Comment: 
 
 Filename: quafu/users/userapi.py
 Comment: 
 
-Filename: quafu/utils/__init__.py
+Filename: quafu/qfasm/__init__.py
 Comment: 
 
-Filename: quafu/utils/basis.py
+Filename: quafu/qfasm/qfasm_convertor.py
 Comment: 
 
-Filename: quafu/utils/paulis.py
+Filename: quafu/qfasm/qelib1.inc
 Comment: 
 
-Filename: quafu/utils/platform.py
+Filename: quafu/qfasm/exceptions.py
+Comment: 
+
+Filename: quafu/qfasm/qfasm_utils.py
+Comment: 
+
+Filename: quafu/qfasm/qfasm_parser.py
+Comment: 
+
+Filename: quafu/qfasm/qfasm_lexer.py
+Comment: 
+
+Filename: quafu/circuits/__init__.py
+Comment: 
+
+Filename: quafu/circuits/quantum_circuit.py
+Comment: 
+
+Filename: quafu/circuits/classical_register.py
+Comment: 
+
+Filename: quafu/circuits/quantum_register.py
 Comment: 
 
 Filename: quafu/visualisation/__init__.py
 Comment: 
 
+Filename: quafu/visualisation/bloch_sphere.py
+Comment: 
+
 Filename: quafu/visualisation/circuitPlot.py
 Comment: 
 
-Filename: pyquafu-0.3.6.dist-info/LICENSE
+Filename: quafu/visualisation/draw_dag.py
+Comment: 
+
+Filename: quafu/algorithms/gradients/
+Comment: 
+
+Filename: quafu/algorithms/interface/
+Comment: 
+
+Filename: quafu/algorithms/templates/
+Comment: 
+
+Filename: quafu/algorithms/__init__.py
+Comment: 
+
+Filename: quafu/algorithms/gradient.py
+Comment: 
+
+Filename: quafu/algorithms/hamiltonian.py
+Comment: 
+
+Filename: quafu/algorithms/interface_provider.py
+Comment: 
+
+Filename: quafu/algorithms/sampler.py
+Comment: 
+
+Filename: quafu/algorithms/estimator.py
+Comment: 
+
+Filename: quafu/algorithms/ansatz.py
+Comment: 
+
+Filename: quafu/algorithms/optimizer.py
+Comment: 
+
+Filename: quafu/algorithms/gradients/__init__.py
+Comment: 
+
+Filename: quafu/algorithms/gradients/param_shift.py
+Comment: 
+
+Filename: quafu/algorithms/gradients/vjp.py
+Comment: 
+
+Filename: quafu/algorithms/interface/__init__.py
+Comment: 
+
+Filename: quafu/algorithms/interface/torch.py
+Comment: 
+
+Filename: quafu/algorithms/templates/__init__.py
+Comment: 
+
+Filename: quafu/algorithms/templates/angle.py
+Comment: 
+
+Filename: quafu/algorithms/templates/basic_entangle.py
+Comment: 
+
+Filename: quafu/algorithms/templates/amplitude.py
+Comment: 
+
+Filename: quafu/backends/__init__.py
+Comment: 
+
+Filename: quafu/backends/backends.py
+Comment: 
+
+Filename: quafu/elements/matrices/
+Comment: 
+
+Filename: quafu/elements/element_gates/
+Comment: 
+
+Filename: quafu/elements/unitary/
+Comment: 
+
+Filename: quafu/elements/__init__.py
+Comment: 
+
+Filename: quafu/elements/quantum_gate.py
+Comment: 
+
+Filename: quafu/elements/classical_element.py
+Comment: 
+
+Filename: quafu/elements/instruction.py
+Comment: 
+
+Filename: quafu/elements/pulses.py
+Comment: 
+
+Filename: quafu/elements/parameters.py
+Comment: 
+
+Filename: quafu/elements/utils.py
+Comment: 
+
+Filename: quafu/elements/oracle.py
+Comment: 
+
+Filename: quafu/elements/noise.py
+Comment: 
+
+Filename: quafu/elements/matrices/__init__.py
+Comment: 
+
+Filename: quafu/elements/matrices/mat_utils.py
+Comment: 
+
+Filename: quafu/elements/matrices/mat_lib.py
+Comment: 
+
+Filename: quafu/elements/element_gates/__init__.py
+Comment: 
+
+Filename: quafu/elements/element_gates/pauli.py
+Comment: 
+
+Filename: quafu/elements/element_gates/clifford.py
+Comment: 
+
+Filename: quafu/elements/element_gates/rotation.py
 Comment: 
 
-Filename: pyquafu-0.3.6.dist-info/METADATA
+Filename: quafu/elements/element_gates/element_gates.py
 Comment: 
 
-Filename: pyquafu-0.3.6.dist-info/WHEEL
+Filename: quafu/elements/unitary/__init__.py
 Comment: 
 
-Filename: pyquafu-0.3.6.dist-info/top_level.txt
+Filename: quafu/elements/unitary/decomposer.py
 Comment: 
 
-Filename: pyquafu-0.3.6.dist-info/RECORD
+Filename: pyquafu.libs/libgomp-a34b3233.so.1.0.0
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## quafu/__init__.py

```diff
@@ -1,11 +1,24 @@
 from .circuits.quantum_circuit import QuantumCircuit
+from .algorithms.hamiltonian import Hamiltonian
+from .circuits.quantum_register import QuantumRegister, Qubit
 from .results.results import ExecResult, SimuResult
+from .simulators import simulate
 from .tasks.tasks import Task
 from .users.userapi import User
-from .simulators.simulator import simulate
 
-__all__ = ["QuantumCircuit", "ExecResult", "Task", "User", "SimuResult", "simulate", "get_version"]
+__all__ = [
+    "QuantumCircuit",
+    "QuantumRegister",
+    "Qubit",
+    "Hamiltonian",
+    "ExecResult",
+    "Task",
+    "User",
+    "SimuResult",
+    "simulate",
+    "get_version",
+]
 
 
 def get_version():
-    return "0.3.6"
+    return "0.4.0"
```

## quafu/backends/backends.py

```diff
@@ -8,103 +8,118 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import requests
-import json
 import re
+
+import matplotlib.pyplot as plt
 import networkx as nx
 import numpy as np
-import matplotlib.pyplot as plt
-
 from quafu.users.userapi import User
+from quafu.utils.client_wrapper import ClientWrapper
 
 
 class Backend(object):
     def __init__(self, backend_info: dict):
-        self.name = backend_info['system_name']
-        self._valid_gates = backend_info['valid_gates']
-        self.qubit_num = backend_info['qubits']
-        self.system_id = backend_info['system_id']
-        self.status = backend_info['status']
+        self.name = backend_info["system_name"]
+        self._valid_gates = backend_info["valid_gates"]
+        self.qubit_num = backend_info["qubits"]
+        self.system_id = backend_info["system_id"]
+        self.status = backend_info["status"]
         self.qv = backend_info["QV"]
         # self.task_in_queue = backend_info["task_in_queue"]
 
     def get_chip_info(self, user: User = None):
         user = User() if user is None else user
         api_token = user.api_token
         data = {"system_name": self.name.lower()}
         headers = {"api_token": api_token}
-        chip_info = requests.post(url=User.chip_api, data=data,
-                                  headers=headers)
-        chip_info = json.loads(chip_info.text)
+        url = User.url + User.chip_api
+        chip_info = ClientWrapper.post(url=url, data=data, headers=headers)
+        chip_info = chip_info.json()
         json_topo_struct = chip_info["topological_structure"]
         qubits_list = []
         for gate in json_topo_struct.keys():
-            qubit = gate.split('_')
+            qubit = gate.split("_")
             qubits_list.append(qubit[0])
             qubits_list.append(qubit[1])
         qubits_list = list(set(qubits_list))
         qubits_list = sorted(qubits_list, key=lambda x: int(re.findall(r"\d+", x)[0]))
         int_to_qubit = {k: v for k, v in enumerate(qubits_list)}
         qubit_to_int = {v: k for k, v in enumerate(qubits_list)}
 
         directed_weighted_edges = []
         weighted_edges = []
         edges_dict = {}
         clist = []
         for gate, name_fidelity in json_topo_struct.items():
-            gate_qubit = gate.split('_')
+            gate_qubit = gate.split("_")
             qubit1 = qubit_to_int[gate_qubit[0]]
             qubit2 = qubit_to_int[gate_qubit[1]]
             gate_name = list(name_fidelity.keys())[0]
-            fidelity = name_fidelity[gate_name]['fidelity']
+            fidelity = name_fidelity[gate_name]["fidelity"]
             directed_weighted_edges.append([qubit1, qubit2, fidelity])
             clist.append([qubit1, qubit2])
-            gate_reverse = gate.split('_')[1] + '_' + gate.split('_')[0]
+            gate_reverse = gate.split("_")[1] + "_" + gate.split("_")[0]
             if gate not in edges_dict and gate_reverse not in edges_dict:
                 edges_dict[gate] = fidelity
             else:
                 if fidelity < edges_dict[gate_reverse]:
                     edges_dict.pop(gate_reverse)
                     edges_dict[gate] = fidelity
 
         for gate, fidelity in edges_dict.items():
-            gate_qubit = gate.split('_')
+            gate_qubit = gate.split("_")
             qubit1, qubit2 = qubit_to_int[gate_qubit[0]], qubit_to_int[gate_qubit[1]]
             weighted_edges.append([qubit1, qubit2, np.round(fidelity, 3)])
 
         # draw topology
         G = nx.Graph()
         for key, value in int_to_qubit.items():
             G.add_node(key, name=value)
 
         G.add_weighted_edges_from(weighted_edges)
 
         elarge = [(u, v) for (u, v, d) in G.edges(data=True) if d["weight"] >= 0.9]
         esmall = [(u, v) for (u, v, d) in G.edges(data=True) if d["weight"] < 0.9]
-        elarge_labels = {(u, v): "%.3f" % d["weight"] for (u, v, d) in G.edges(data=True) if d["weight"] >= 0.9}
-        esmall_labels = {(u, v): "%.3f" % d["weight"] for (u, v, d) in G.edges(data=True) if d["weight"] < 0.9}
+        elarge_labels = {
+            (u, v): "%.3f" % d["weight"]
+            for (u, v, d) in G.edges(data=True)
+            if d["weight"] >= 0.9
+        }
+        esmall_labels = {
+            (u, v): "%.3f" % d["weight"]
+            for (u, v, d) in G.edges(data=True)
+            if d["weight"] < 0.9
+        }
 
         pos = nx.spring_layout(G, seed=1)
         fig, ax = plt.subplots()
         nx.draw_networkx_nodes(G, pos, node_size=400, ax=ax)
 
         nx.draw_networkx_edges(G, pos, edgelist=elarge, width=2, ax=ax)
         nx.draw_networkx_edges(
-            G, pos, edgelist=esmall, width=2, alpha=0.5, style="dashed"
-            , ax=ax)
+            G, pos, edgelist=esmall, width=2, alpha=0.5, style="dashed", ax=ax
+        )
 
         nx.draw_networkx_labels(G, pos, font_size=14, font_family="sans-serif", ax=ax)
         # edge_labels = nx.get_edge_attributes(G, "weight")
-        nx.draw_networkx_edge_labels(G, pos, elarge_labels, font_size=12, font_color="green", ax=ax)
-        nx.draw_networkx_edge_labels(G, pos, esmall_labels, font_size=12, font_color="red", ax=ax)
+        nx.draw_networkx_edge_labels(
+            G, pos, elarge_labels, font_size=12, font_color="green", ax=ax
+        )
+        nx.draw_networkx_edge_labels(
+            G, pos, esmall_labels, font_size=12, font_color="red", ax=ax
+        )
         fig.set_figwidth(14)
         fig.set_figheight(14)
         fig.tight_layout()
-        return {"mapping": int_to_qubit, "topology_diagram": fig, "full_info": chip_info}
+        return {
+            "mapping": int_to_qubit,
+            "topology_diagram": fig,
+            "full_info": chip_info,
+        }
 
     def get_valid_gates(self):
         return self._valid_gates
```

## quafu/benchmark/adder.py

```diff
@@ -1,126 +1,123 @@
-from quafu.circuits.quantum_circuit import QuantumCircuit
-import matplotlib.pyplot as plt
-
-"""
-// quantum ripple-carry adder from Cuccaro et al, quant-ph/0410184
-OPENQASM 2.0;
-include "qelib1.inc";
-"""
-
-n = 10
-qc = QuantumCircuit(n)
-
-
-def majority(a, b, c):
-    """
-    gate majority a,b,c
-    {
-      cx c,b;
-      cx c,a;
-      ccx a,b,c;
-    }
-    """
-    qc.cnot(c, b)
-    qc.cnot(a, b)
-    qc.mcx([a, b], c)
-
-
-def unmaj(a, b, c):
-    """
-    gate unmaj a,b,c
-    {
-      ccx a,b,c;
-      cx c,a;
-      cx a,b;
-    }
-    """
-    qc.mcx([a, b], c)
-    qc.cnot(c, a)
-    qc.cnot(a, b)
-
-
-def qreg(_i, name):
-    """
-    qreg cin[1];
-    qreg a[4];
-    qreg b[4];
-    qreg cout[1];
-    """
-    if name == 'cin':
-        return _i
-    elif name == 'a':
-        return _i + 1
-    elif name == 'b':
-        return _i + 5
-    elif name == 'cout':
-        return _i + 9
-    else:
-        raise ValueError('Unknown qreg name: {}'.format(name))
-
-
-def creg(_i, name):
-    """
-    creg ans[5];
-    """
-    if name == 'ans':
-        return _i
-    else:
-        raise ValueError('Unknown creg name: {}'.format(name))
-
-
-"""
-// set input states
-x a[0]; // a = 0001
-x b;    // b = 1111
-"""
-qc.x(qreg(0, 'a'))
-for i in range(4):
-    qc.x(qreg(i, 'b'))
-
-"""
-// add a to b, storing result in b
-majority cin[0],b[0],a[0];
-majority a[0],b[1],a[1];
-majority a[1],b[2],a[2];
-majority a[2],b[3],a[3];
-cx a[3],cout[0];
-unmaj a[2],b[3],a[3];
-unmaj a[1],b[2],a[2];
-unmaj a[0],b[1],a[1];
-unmaj cin[0],b[0],a[0];
-"""
-majority(qreg(0, 'cin'), qreg(0, 'b'), qreg(0, 'a'))
-majority(qreg(0, 'a'), qreg(1, 'b'), qreg(1, 'a'))
-for i in range(1, 4):
-    majority(qreg(i-1, 'a'), qreg(i, 'b'), qreg(i, 'a'))
-qc.cnot(qreg(3, 'a'), qreg(0, 'cout'))
-unmaj(qreg(2, 'a'), qreg(3, 'b'), qreg(3, 'a'))
-unmaj(qreg(1, 'a'), qreg(2, 'b'), qreg(2, 'a'))
-unmaj(qreg(0, 'a'), qreg(1, 'b'), qreg(1, 'a'))
-
-"""
-measure b[0] -> ans[0];
-measure b[1] -> ans[1];
-measure b[2] -> ans[2];
-measure b[3] -> ans[3];
-measure cout[0] -> ans[4];
-"""
-measure_pos = [qreg(i, 'b') for i in range(4)] + [qreg(0, 'cout')]
-measure_cbits = [creg(i, 'ans') for i in range(5)]
-qc.measure(measure_pos, cbits=measure_cbits)
-# qc.draw_circuit()
-# print(qc.to_openqasm())
-
-init_labels = dict.fromkeys(range(n))
-init_labels[0] = 'cin'
-for i in range(4):
-    init_labels[i+1] = f'a_{i}'
-for i in range(5):
-    init_labels[i+5] = f'b_{i}'
-
-end_labels = {i+5: f'ans_{i}' for i in range(5)}
-qc.plot_circuit(title='Quantum ripple-carry adder',
-                init_labels=init_labels,
-                end_labels=end_labels,
-                )
-plt.show()
+import matplotlib.pyplot as plt
+from quafu.circuits.quantum_circuit import QuantumCircuit
+
+# // quantum ripple-carry adder from Cuccaro et al, quant-ph/0410184
+# OPENQASM 2.0;
+# include "qelib1.inc";
+
+n = 10
+qc = QuantumCircuit(n)
+
+
+def majority(a, b, c):
+    """
+    gate majority a,b,c
+    {
+      cx c,b;
+      cx c,a;
+      ccx a,b,c;
+    }
+    """
+    qc.cnot(c, b)
+    qc.cnot(a, b)
+    qc.mcx([a, b], c)
+
+
+def unmaj(a, b, c):
+    """
+    gate unmaj a,b,c
+    {
+      ccx a,b,c;
+      cx c,a;
+      cx a,b;
+    }
+    """
+    qc.mcx([a, b], c)
+    qc.cnot(c, a)
+    qc.cnot(a, b)
+
+
+def qreg(_i, name):
+    """
+    qreg cin[1];
+    qreg a[4];
+    qreg b[4];
+    qreg cout[1];
+    """
+    if name == "cin":
+        return _i
+    elif name == "a":
+        return _i + 1
+    elif name == "b":
+        return _i + 5
+    elif name == "cout":
+        return _i + 9
+    else:
+        raise ValueError("Unknown qreg name: {}".format(name))
+
+
+def creg(_i, name):
+    """
+    creg ans[5];
+    """
+    if name == "ans":
+        return _i
+    else:
+        raise ValueError("Unknown creg name: {}".format(name))
+
+
+"""
+// set input states
+x a[0]; // a = 0001
+x b;    // b = 1111
+"""
+qc.x(qreg(0, "a"))
+for i in range(4):
+    qc.x(qreg(i, "b"))
+"""
+// add a to b, storing result in b
+majority cin[0],b[0],a[0];
+majority a[0],b[1],a[1];
+majority a[1],b[2],a[2];
+majority a[2],b[3],a[3];
+cx a[3],cout[0];
+unmaj a[2],b[3],a[3];
+unmaj a[1],b[2],a[2];
+unmaj a[0],b[1],a[1];
+unmaj cin[0],b[0],a[0];
+"""
+majority(qreg(0, "cin"), qreg(0, "b"), qreg(0, "a"))
+majority(qreg(0, "a"), qreg(1, "b"), qreg(1, "a"))
+for i in range(1, 4):
+    majority(qreg(i - 1, "a"), qreg(i, "b"), qreg(i, "a"))
+qc.cnot(qreg(3, "a"), qreg(0, "cout"))
+unmaj(qreg(2, "a"), qreg(3, "b"), qreg(3, "a"))
+unmaj(qreg(1, "a"), qreg(2, "b"), qreg(2, "a"))
+unmaj(qreg(0, "a"), qreg(1, "b"), qreg(1, "a"))
+"""
+measure b[0] -> ans[0];
+measure b[1] -> ans[1];
+measure b[2] -> ans[2];
+measure b[3] -> ans[3];
+measure cout[0] -> ans[4];
+"""
+measure_pos = [qreg(i, "b") for i in range(4)] + [qreg(0, "cout")]
+measure_cbits = [creg(i, "ans") for i in range(5)]
+qc.measure(measure_pos, cbits=measure_cbits)
+# qc.draw_circuit()
+# print(qc.to_openqasm())
+
+init_labels = dict.fromkeys(range(n))
+init_labels[0] = "cin"
+for i in range(4):
+    init_labels[i + 1] = f"a_{i}"
+for i in range(5):
+    init_labels[i + 5] = f"b_{i}"
+
+end_labels = {i + 5: f"ans_{i}" for i in range(5)}
+qc.plot_circuit(
+    title="Quantum ripple-carry adder",
+    init_labels=init_labels,
+    end_labels=end_labels,
+)
+plt.show()
```

## quafu/benchmark/deutsch_jozsa.py

```diff
@@ -1,71 +1,75 @@
-import random
-import matplotlib.pyplot as plt
-import numpy as np
-
-from quafu.circuits.quantum_circuit import QuantumCircuit
-from quafu.visualisation.circuitPlot import CircuitPlotManager
-
-
-def get_const_oracle(qc: QuantumCircuit):
-    n = qc.num - 1
-    output = np.random.randint(2)
-    if output == 1:
-        qc.x(n)
-    qc.name = 'Constant Oracle'
-    return qc
-
-
-def get_balanced_oracle(qc: QuantumCircuit):
-    n = qc.num - 1
-    b_str = ''.join([random.choice('01') for _ in range(n)])
-
-    # Place X-qu_gate
-    for qubit in range(len(b_str)):
-        if b_str[qubit] == '1':
-            qc.x(qubit)
-
-    # Use barrier as divider
-    qc.barrier()
-
-    # Controlled-NOT qu_gate
-    for qubit in range(n):
-        qc.cnot(qubit, n)
-
-    qc.barrier()
-
-    # Place X-qu_gate
-    for qubit in range(len(b_str)):
-        if b_str[qubit] == '1':
-            qc.x(qubit)
-
-    qc.name = 'Balanced Oracle'
-    return qc
-
-
-def deutsch_jozsa(n: int, case: str):
-    circuit = QuantumCircuit(n + 1)  # number of q-bit and c-bit
-    # Initialization
-    for qubit in range(n):
-        circuit.h(qubit)
-    circuit.x(n)
-    circuit.h(n)
-
-    # Add oracle
-    #################################################
-    if case == 'balanced':
-        get_balanced_oracle(circuit)
-    elif case == 'constant':
-        get_const_oracle(circuit)
-    else:
-        raise ValueError('undefined case: ' + case)
-    #################################################
-
-    # Repeat H-qu_gate
-    circuit.barrier()
-    for qubit in range(n):
-        circuit.h(qubit)
-    circuit.barrier()
-
-    # Measure
-    circuit.measure(list(range(n)), list(range(n)))
-    return circuit
+import random
+
+import matplotlib.pyplot as plt
+import numpy as np
+from quafu.circuits.quantum_circuit import QuantumCircuit
+from quafu.visualisation.circuitPlot import CircuitPlotManager
+
+
+def get_const_oracle(qc: QuantumCircuit):
+    n = qc.num - 1
+    output = np.random.randint(2)
+    if output == 1:
+        qc.x(n)
+    qc.name = "Constant Oracle"
+    return qc
+
+
+def get_balanced_oracle(qc: QuantumCircuit):
+    n = qc.num - 1
+    b_str = "".join([random.choice("01") for _ in range(n)])
+
+    # Place X-qu_gate
+    for qubit in range(len(b_str)):
+        if b_str[qubit] == "1":
+            qc.x(qubit)
+
+    # Use barrier as divider
+    qc.barrier()
+
+    # Controlled-NOT qu_gate
+    for qubit in range(n):
+        qc.cnot(qubit, n)
+
+    qc.barrier()
+
+    # Place X-qu_gate
+    for qubit in range(len(b_str)):
+        if b_str[qubit] == "1":
+            qc.x(qubit)
+
+    qc.name = "Balanced Oracle"
+    return qc
+
+
+def deutsch_jozsa(n: int, case: str):
+    circuit = QuantumCircuit(n + 1)  # number of q-bit and c-bit
+    # Initialization
+    for qubit in range(n):
+        circuit.h(qubit)
+    circuit.x(n)
+    circuit.h(n)
+
+    # Add oracle
+    #################################################
+    if case == "balanced":
+        get_balanced_oracle(circuit)
+    elif case == "constant":
+        get_const_oracle(circuit)
+    else:
+        raise ValueError("undefined case: " + case)
+    #################################################
+
+    # Repeat H-qu_gate
+    circuit.barrier()
+    for qubit in range(n):
+        circuit.h(qubit)
+    circuit.barrier()
+
+    # Measure
+    circuit.measure(list(range(n)), list(range(n)))
+    return circuit
+
+
+dj_qc = deutsch_jozsa(n=4, case="constant")
+dj_qc.plot_circuit(title="Deutsch-Josza Circuit", show=True)
```

## quafu/benchmark/unitary_test.py

```diff
@@ -1,11 +1,12 @@
-from scipy.stats import unitary_group
-from quafu import QuantumCircuit
-
-nqubit = 5
-qubits = list(range(nqubit))
-U0 = unitary_group.rvs(2 ** nqubit)
-
-# Using QSD to decompose the unitary
-qc = QuantumCircuit(nqubit)
-qc.unitary(U0, qubits)
-qc.draw_circuit()
+from scipy.stats import unitary_group
+
+from quafu import QuantumCircuit
+
+nqubit = 5
+qubits = list(range(nqubit))
+U0 = unitary_group.rvs(2**nqubit)
+
+# Using QSD to decompose the unitary
+qc = QuantumCircuit(nqubit)
+qc.unitary(U0, qubits)
+qc.draw_circuit()
```

## quafu/benchmark/variational_n4.py

```diff
@@ -1,91 +1,91 @@
-from quafu import QuantumCircuit
-
-n = 4
-qc = QuantumCircuit(n)
-
-qasm = """
-// Generated from Cirq v0.8.0
-
-OPENQASM 2.0;
-include "qelib1.inc";
-
-// Qubits: [0, 1, 2, 3]
-qreg q[4];
-creg c[4];
-
-x q[0];
-x q[1];
-
-// Gate: PhasedISWAP**0.9951774602384953
-rz(pi*0.25) q[1];
-rz(pi*-0.25) q[2];
-cx q[1],q[2];
-h q[1];
-cx q[2],q[1];
-rz(pi*0.4975887301) q[1];
-cx q[2],q[1];
-rz(pi*-0.4975887301) q[1];
-h q[1];
-cx q[1],q[2];
-rz(pi*-0.25) q[1];
-rz(pi*0.25) q[2];
-
-rz(0) q[2];
-
-// Gate: PhasedISWAP**-0.5024296754026449
-rz(pi*0.25) q[0];
-rz(pi*-0.25) q[1];
-cx q[0],q[1];
-h q[0];
-cx q[1],q[0];
-rz(pi*-0.2512148377) q[0];
-cx q[1],q[0];
-rz(pi*0.2512148377) q[0];
-h q[0];
-cx q[0],q[1];
-rz(pi*-0.25) q[0];
-rz(pi*0.25) q[1];
-
-rz(0) q[1];
-
-// Gate: PhasedISWAP**-0.49760685888033646
-rz(pi*0.25) q[2];
-rz(pi*-0.25) q[3];
-cx q[2],q[3];
-h q[2];
-cx q[3],q[2];
-rz(pi*-0.2488034294) q[2];
-cx q[3],q[2];
-rz(pi*0.2488034294) q[2];
-h q[2];
-cx q[2],q[3];
-rz(pi*-0.25) q[2];
-rz(pi*0.25) q[3];
-
-rz(0) q[3];
-
-// Gate: PhasedISWAP**0.004822678143889672
-rz(pi*0.25) q[1];
-rz(pi*-0.25) q[2];
-cx q[1],q[2];
-h q[1];
-cx q[2],q[1];
-rz(pi*0.0024113391) q[1];
-cx q[2],q[1];
-rz(pi*-0.0024113391) q[1];
-h q[1];
-cx q[1],q[2];
-rz(pi*-0.25) q[1];
-rz(pi*0.25) q[2];
-
-rz(0) q[2];
-
-measure q[0] -> c[0];
-measure q[1] -> c[1];
-measure q[2] -> c[2];
-measure q[3] -> c[3];
-"""
-
-qc.from_openqasm(qasm)
-qc.draw_circuit()
-qc.plot_circuit(show=True, title='Variational n4')
+from quafu import QuantumCircuit
+
+n = 4
+qc = QuantumCircuit(n)
+
+qasm = """
+// Generated from Cirq v0.8.0
+
+OPENQASM 2.0;
+include "qelib1.inc";
+
+// Qubits: [0, 1, 2, 3]
+qreg q[4];
+creg c[4];
+
+x q[0];
+x q[1];
+
+// Gate: PhasedISWAP**0.9951774602384953
+rz(pi*0.25) q[1];
+rz(pi*-0.25) q[2];
+cx q[1],q[2];
+h q[1];
+cx q[2],q[1];
+rz(pi*0.4975887301) q[1];
+cx q[2],q[1];
+rz(pi*-0.4975887301) q[1];
+h q[1];
+cx q[1],q[2];
+rz(pi*-0.25) q[1];
+rz(pi*0.25) q[2];
+
+rz(0) q[2];
+
+// Gate: PhasedISWAP**-0.5024296754026449
+rz(pi*0.25) q[0];
+rz(pi*-0.25) q[1];
+cx q[0],q[1];
+h q[0];
+cx q[1],q[0];
+rz(pi*-0.2512148377) q[0];
+cx q[1],q[0];
+rz(pi*0.2512148377) q[0];
+h q[0];
+cx q[0],q[1];
+rz(pi*-0.25) q[0];
+rz(pi*0.25) q[1];
+
+rz(0) q[1];
+
+// Gate: PhasedISWAP**-0.49760685888033646
+rz(pi*0.25) q[2];
+rz(pi*-0.25) q[3];
+cx q[2],q[3];
+h q[2];
+cx q[3],q[2];
+rz(pi*-0.2488034294) q[2];
+cx q[3],q[2];
+rz(pi*0.2488034294) q[2];
+h q[2];
+cx q[2],q[3];
+rz(pi*-0.25) q[2];
+rz(pi*0.25) q[3];
+
+rz(0) q[3];
+
+// Gate: PhasedISWAP**0.004822678143889672
+rz(pi*0.25) q[1];
+rz(pi*-0.25) q[2];
+cx q[1],q[2];
+h q[1];
+cx q[2],q[1];
+rz(pi*0.0024113391) q[1];
+cx q[2],q[1];
+rz(pi*-0.0024113391) q[1];
+h q[1];
+cx q[1],q[2];
+rz(pi*-0.25) q[1];
+rz(pi*0.25) q[2];
+
+rz(0) q[2];
+
+measure q[0] -> c[0];
+measure q[1] -> c[1];
+measure q[2] -> c[2];
+measure q[3] -> c[3];
+"""
+
+qc.from_openqasm(qasm)
+qc.draw_circuit()
+qc.plot_circuit(show=True, title="Variational n4")
```

## quafu/circuits/__init__.py

```diff
@@ -0,0 +1,11 @@
+00000000: 2222 2251 7561 6675 2071 7561 6e74 756d  """Quafu quantum
+00000010: 2063 6972 6375 6974 7322 2222 0a0a 6672   circuits"""..fr
+00000020: 6f6d 202e 636c 6173 7369 6361 6c5f 7265  om .classical_re
+00000030: 6769 7374 6572 2069 6d70 6f72 7420 436c  gister import Cl
+00000040: 6173 7369 6361 6c52 6567 6973 7465 720a  assicalRegister.
+00000050: 6672 6f6d 202e 7175 616e 7475 6d5f 6369  from .quantum_ci
+00000060: 7263 7569 7420 696d 706f 7274 2051 7561  rcuit import Qua
+00000070: 6e74 756d 4369 7263 7569 740a 6672 6f6d  ntumCircuit.from
+00000080: 202e 7175 616e 7475 6d5f 7265 6769 7374   .quantum_regist
+00000090: 6572 2069 6d70 6f72 7420 5175 616e 7475  er import Quantu
+000000a0: 6d52 6567 6973 7465 720a                 mRegister.
```

## quafu/circuits/quantum_circuit.py

```diff
@@ -1,879 +1,1238 @@
-# (C) Copyright 2023 Beijing Academy of Quantum Information Sciences
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#    http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from typing import List
-import warnings
-import numpy as np
-
-import quafu.elements.element_gates as qeg
-from quafu.elements import (
-    Instruction,
-    Measure,
-    Barrier,
-    Delay,
-    MultiQubitGate,
-    QuantumGate,
-    ControlledGate,
-    SingleQubitGate,
-    XYResonance,
-    QuantumPulse,
-)
-from ..exceptions import CircuitError
-
-
-class QuantumCircuit(object):
-    def __init__(self, num: int, *args, **kwargs):
-        """
-        Initialize a QuantumCircuit object.
-
-        Args:
-            num (int): Total qubit number used
-        """
-        self.num = num
-        self.instructions = []
-        self.openqasm = ""
-        self.circuit = []  # TODO: ?
-        self._measures = []  # type: list[Measure]
-        self._gates = []
-        self._used_qubits = []
-
-    @property
-    def used_qubits(self) -> List:
-        self.layered_circuit()
-        return self._used_qubits
-
-    @property
-    def measures(self):
-        measures = {}
-        for meas in self._measures:
-            if not set(measures.keys()).isdisjoint(set(meas.qbits)):
-                raise ValueError("Measured qubits overlap with existing measurements.")
-            measures = {**measures, **dict(zip(meas.qbits, meas.cbits))}
-        return measures
-
-    @measures.setter
-    def measures(self, measures):
-        self._measures = [Measure(measures)]
-
-    @property
-    def gates(self):
-        warnings.warn('Due to historical reason, ``gates`` contains not only instances of '
-                      'QuantumGate, meanwhile not contains measurements. This attributes might be deprecated in'
-                      ' the future. Better to use ``instructions`` which contains all the instructions.',
-                      category=DeprecationWarning)
-        return self._gates
-
-    @gates.setter
-    def gates(self, gates):
-        self._gates = gates
-
-    def add_ins(self, ins: Instruction):
-        """
-        Add instruction to circuit, with NO checking yet.
-        """
-        if isinstance(ins, (QuantumGate, Delay, Barrier, XYResonance)):
-            # TODO: Delay, Barrier added by add_gate for backward compatibility.
-            #       Figure out better handling in the future.
-            self.add_gate(ins)
-        self.instructions.append(ins)
-
-    def add_gate(self, gate: QuantumGate):
-        """
-        Add quantum gate to circuit, with some checking.
-        """
-        pos = np.array(gate.pos)
-        if np.any(pos >= self.num):
-            raise CircuitError(f"Gate position out of range: {gate.pos}")
-        self._gates.append(gate)
-
-    def layered_circuit(self) -> np.ndarray:
-        """
-        Make layered circuit from the gate sequence self.gates.
-
-        Returns:
-            A layered list with left justed circuit.
-        """
-        num = self.num
-        gatelist = self.gates
-        gateQlist = [[] for i in range(num)]
-        used_qubits = []
-        for gate in gatelist:
-            if isinstance(gate, (SingleQubitGate, Delay, QuantumPulse)):
-                gateQlist[gate.pos].append(gate)
-                if gate.pos not in used_qubits:
-                    used_qubits.append(gate.pos)
-
-            elif isinstance(gate, (Barrier, MultiQubitGate, XYResonance)):
-                pos1 = min(gate.pos)
-                pos2 = max(gate.pos)
-                gateQlist[pos1].append(gate)
-                for j in range(pos1 + 1, pos2 + 1):
-                    gateQlist[j].append(None)
-
-                if isinstance(gate, (MultiQubitGate, XYResonance)):
-                    for pos in gate.pos:
-                        if pos not in used_qubits:
-                            used_qubits.append(pos)
-
-                maxlayer = max([len(gateQlist[j]) for j in range(pos1, pos2 + 1)])
-                for j in range(pos1, pos2 + 1):
-                    layerj = len(gateQlist[j])
-                    pos = layerj - 1
-                    if not layerj == maxlayer:
-                        for i in range(abs(layerj - maxlayer)):
-                            gateQlist[j].insert(pos, None)
-
-        maxdepth = max([len(gateQlist[i]) for i in range(num)])
-
-        for gates in gateQlist:
-            gates.extend([None] * (maxdepth - len(gates)))
-
-        for m in self.measures.keys():
-            if m not in used_qubits:
-                used_qubits.append(m)
-        used_qubits = np.sort(used_qubits)
-
-        new_gateQlist = []
-        for old_qi in range(len(gateQlist)):
-            gates = gateQlist[old_qi]
-            if old_qi in used_qubits:
-                new_gateQlist.append(gates)
-
-        lc = np.array(new_gateQlist)
-        lc = np.vstack((used_qubits, lc.T)).T
-        self.circuit = lc
-        self._used_qubits = list(used_qubits)
-        return self.circuit
-
-    def draw_circuit(self, width: int = 4, return_str: bool = False):
-        """
-        Draw layered circuit using ASCII, print in terminal.
-
-        Args:
-            width (int): The width of each gate.
-            return_str: Whether return the circuit string.
-        """
-        self.layered_circuit()
-        gateQlist = self.circuit
-        num = gateQlist.shape[0]
-        depth = gateQlist.shape[1] - 1
-        printlist = np.array([[""] * depth for i in range(2 * num)], dtype="<U30")
-
-        reduce_map = dict(zip(gateQlist[:, 0], range(num)))
-        reduce_map_inv = dict(zip(range(num), gateQlist[:, 0]))
-        for l in range(depth):
-            layergates = gateQlist[:, l + 1]
-            maxlen = 1 + width
-            for i in range(num):
-                gate = layergates[i]
-                if isinstance(gate, SingleQubitGate) or isinstance(gate, Delay) or (isinstance(gate, QuantumPulse)):
-                    printlist[i * 2, l] = gate.symbol
-                    maxlen = max(maxlen, len(gate.symbol) + width)
-
-                elif isinstance(gate, MultiQubitGate) or isinstance(gate, XYResonance):
-                    q1 = reduce_map[min(gate.pos)]
-                    q2 = reduce_map[max(gate.pos)]
-                    printlist[2 * q1 + 1:2 * q2, l] = "|"
-                    printlist[q1 * 2, l] = "#"
-                    printlist[q2 * 2, l] = "#"
-                    if isinstance(gate, ControlledGate):  # Controlled-Multiqubit gate
-                        for ctrl in gate.ctrls:
-                            printlist[reduce_map[ctrl] * 2, l] = "*"
-
-                        if gate.targ_name == "SWAP":
-                            printlist[reduce_map[gate.targs[0]] * 2, l] = "x"
-                            printlist[reduce_map[gate.targs[1]] * 2, l] = "x"
-                        else:
-                            tq1 = reduce_map[min(gate.targs)]
-                            tq2 = reduce_map[max(gate.targs)]
-                            printlist[tq1 * 2, l] = "#"
-                            printlist[tq2 * 2, l] = "#"
-                            if tq1 + tq2 in [reduce_map[ctrl] * 2 for ctrl in gate.ctrls]:
-                                printlist[tq1 + tq2, l] = "*" + gate.symbol
-                            else:
-                                printlist[tq1 + tq2, l] = gate.symbol
-                            maxlen = max(maxlen, len(gate.symbol) + width)
-
-                    else:  # Multiqubit gate
-                        if gate.name == "SWAP":
-                            printlist[q1 * 2, l] = "x"
-                            printlist[q2 * 2, l] = "x"
-
-                        else:
-                            printlist[q1 + q2, l] = gate.symbol
-                            maxlen = max(maxlen, len(gate.symbol) + width)
-
-                elif isinstance(gate, Barrier):
-                    pos = [i for i in gate.pos if i in reduce_map.keys()]
-                    q1 = reduce_map[min(pos)]
-                    q2 = reduce_map[max(pos)]
-                    printlist[2 * q1:2 * q2 + 1, l] = "||"
-                    maxlen = max(maxlen, len("||"))
-
-            printlist[-1, l] = maxlen
-
-        circuitstr = []
-        for j in range(2 * num - 1):
-            if j % 2 == 0:
-                linestr = ("q[%d]" % (reduce_map_inv[j // 2])).ljust(6) + "".join(
-                    [printlist[j, l].center(int(printlist[-1, l]), "-") for l in range(depth)])
-                if reduce_map_inv[j // 2] in self.measures.keys():
-                    linestr += " M->c[%d]" % self.measures[reduce_map_inv[j // 2]]
-                circuitstr.append(linestr)
-            else:
-                circuitstr.append("".ljust(6) + "".join(
-                    [printlist[j, l].center(int(printlist[-1, l]), " ") for l in range(depth)]))
-        circuitstr = "\n".join(circuitstr)
-
-        if return_str:
-            return circuitstr
-        else:
-            print(circuitstr)
-
-    def plot_circuit(self, *args, **kwargs):
-        from quafu.visualisation.circuitPlot import CircuitPlotManager
-        cmp = CircuitPlotManager(self)
-        return cmp(*args, **kwargs)
-
-    def from_openqasm(self, openqasm: str):
-        """
-        Initialize the circuit from openqasm text.
-        Args:
-            openqasm: input openqasm str.
-        """
-        from numpy import pi
-        import re
-        self.openqasm = openqasm
-        # lines = self.openqasm.strip("\n").splitlines(";")
-        lines = self.openqasm.splitlines()
-        lines = [line for line in lines if line]
-        self.gates = []
-        self.measures = {}
-        measured_qubits = []
-        global_valid = True
-        for line in lines[2:]:
-            if line:
-                operations_qbs = line.split(" ", 1)
-                operations = operations_qbs[0]
-                if operations == "qreg":
-                    qbs = operations_qbs[1]
-                    self.num = int(re.findall(r"\d+", qbs)[0])
-                elif operations == "creg":
-                    pass
-                elif operations == "measure":
-                    qbs = operations_qbs[1]
-                    indstr = re.findall(r"\d+", qbs)
-                    inds = [int(indst) for indst in indstr]
-                    mb = inds[0]
-                    cb = inds[1]
-                    self.measure([mb], [cb])
-                    measured_qubits.append(mb)
-                else:
-                    qbs = operations_qbs[1]
-                    indstr = re.findall(r"\d+", qbs)
-                    inds = [int(indst) for indst in indstr]
-                    valid = True
-                    for pos in inds:
-                        if pos in measured_qubits:
-                            valid = False
-                            global_valid = False
-                            break
-
-                    if valid:
-                        if operations == "barrier":
-                            self.barrier(inds)
-
-                        else:
-                            sp_op = operations.split("(")
-                            gatename = sp_op[0]
-                            if gatename == "delay":
-                                paras = sp_op[1].strip("()")
-                                duration = int(re.findall(r"\d+", paras)[0])
-                                unit = re.findall("[a-z]+", paras)[0]
-                                self.delay(inds[0], duration, unit)
-                            elif gatename == "xy":
-                                paras = sp_op[1].strip("()")
-                                duration = int(re.findall(r"\d+", paras)[0])
-                                unit = re.findall("[a-z]+", paras)[0]
-                                self.xy(min(inds), max(inds), duration, unit)
-                            else:
-                                if len(sp_op) > 1:
-                                    paras = sp_op[1].strip("()")
-                                    parastr = paras.split(",")
-                                    paras = [eval(parai, {"pi": pi}) for parai in parastr]
-
-                                if gatename == "cx":
-                                    self.cnot(inds[0], inds[1])
-                                elif gatename == "cy":
-                                    self.cy(inds[0], inds[1])
-                                elif gatename == "cz":
-                                    self.cz(inds[0], inds[1])
-                                elif gatename == "cp":
-                                    self.cp(inds[0], inds[1], paras[0])
-                                elif gatename == "swap":
-                                    self.swap(inds[0], inds[1])
-                                elif gatename == "rx":
-                                    self.rx(inds[0], paras[0])
-                                elif gatename == "ry":
-                                    self.ry(inds[0], paras[0])
-                                elif gatename == "rz":
-                                    self.rz(inds[0], paras[0])
-                                elif gatename == "p":
-                                    self.p(inds[0], paras[0])
-                                elif gatename == "x":
-                                    self.x(inds[0])
-                                elif gatename == "y":
-                                    self.y(inds[0])
-                                elif gatename == "z":
-                                    self.z(inds[0])
-                                elif gatename == "h":
-                                    self.h(inds[0])
-                                elif gatename == "id":
-                                    self.id(inds[0])
-                                elif gatename == "s":
-                                    self.s(inds[0])
-                                elif gatename == "sdg":
-                                    self.sdg(inds[0])
-                                elif gatename == "t":
-                                    self.t(inds[0])
-                                elif gatename == "tdg":
-                                    self.tdg(inds[0])
-                                elif gatename == "sx":
-                                    self.sx(inds[0])
-                                elif gatename == "ccx":
-                                    self.toffoli(inds[0], inds[1], inds[2])
-                                elif gatename == "cswap":
-                                    self.fredkin(inds[0], inds[1], inds[2])
-                                elif gatename == "u1":
-                                    self.rz(inds[0], paras[0])
-                                elif gatename == "u2":
-                                    self.rz(inds[0], paras[1])
-                                    self.ry(inds[0], pi / 2)
-                                    self.rz(inds[0], paras[0])
-                                elif gatename == "u3":
-                                    self.rz(inds[0], paras[2])
-                                    self.ry(inds[0], paras[0])
-                                    self.rz(inds[0], paras[1])
-                                elif gatename == "rxx":
-                                    self.rxx(inds[0], inds[1], paras[0])
-                                elif gatename == "ryy":
-                                    self.ryy(inds[0], inds[1], paras[0])
-                                elif gatename == "rzz":
-                                    self.rzz(inds[0], inds[1], paras[0])
-                                else:
-                                    print(
-                                        "Warning: Operations %s may be not supported by QuantumCircuit class currently." % gatename)
-
-        if not self.measures:
-            self.measures = dict(zip(range(self.num), range(self.num)))
-        if not global_valid:
-            print("Warning: All operations after measurement will be removed for executing on experiment")
-
-    def to_openqasm(self) -> str:
-        """
-        Convert the circuit to openqasm text.
-
-        Returns:
-            openqasm text.
-        """
-        qasm = "OPENQASM 2.0;\ninclude \"qelib1.inc\";\n"
-        qasm += "qreg q[%d];\n" % self.num
-        qasm += "creg meas[%d];\n" % len(self.measures)
-        for gate in self.gates:
-            qasm += gate.to_qasm() + ";\n"
-
-        for key in self.measures:
-            qasm += "measure q[%d] -> meas[%d];\n" % (key, self.measures[key])
-
-        self.openqasm = qasm
-        return qasm
-
-    def id(self, pos: int) -> "QuantumCircuit":
-        """
-        Identity gate.
-
-        Args:
-            pos (int): qubit the gate act.
-        """
-        gate = qeg.IdGate(pos)
-        self.add_ins(gate)
-        return self
-
-    def h(self, pos: int) -> "QuantumCircuit":
-        """
-        Hadamard gate.
-
-        Args:
-            pos (int): qubit the gate act.
-        """
-        gate = qeg.HGate(pos)
-        self.add_ins(gate)
-        return self
-
-    def x(self, pos: int) -> "QuantumCircuit":
-        """
-        X gate.
-
-        Args:
-            pos (int): qubit the gate act.
-        """
-        gate = qeg.XGate(pos)
-        self.add_ins(gate)
-        return self
-
-    def y(self, pos: int) -> "QuantumCircuit":
-        """
-        Y gate.
-
-        Args:
-            pos (int): qubit the gate act.
-        """
-        gate = qeg.YGate(pos)
-        self.add_ins(gate)
-        return self
-
-    def z(self, pos: int) -> "QuantumCircuit":
-        """
-        Z gate.
-
-        Args:
-            pos (int): qubit the gate act.
-        """
-        self.add_ins(qeg.ZGate(pos))
-        return self
-
-    def t(self, pos: int) -> "QuantumCircuit":
-        """
-        T gate. (~Z^(1/4))
-
-        Args:
-            pos (int): qubit the gate act.
-        """
-        self.add_ins(qeg.TGate(pos))
-        return self
-
-    def tdg(self, pos: int) -> "QuantumCircuit":
-        """
-        Tdg gate. (Inverse of T gate)
-
-        Args:
-            pos (int): qubit the gate act.
-        """
-        self.add_ins(qeg.TdgGate(pos))
-        return self
-
-    def s(self, pos: int) -> "QuantumCircuit":
-        """
-        S gate. (~√Z)
-
-        Args:
-            pos (int): qubit the gate act.
-        """
-        self.add_ins(qeg.SGate(pos))
-        return self
-
-    def sdg(self, pos: int) -> "QuantumCircuit":
-        """
-        Sdg gate. (Inverse of S gate)
-
-        Args:
-            pos (int): qubit the gate act.
-        """
-        self.add_ins(qeg.SdgGate(pos))
-        return self
-
-    def sx(self, pos: int) -> "QuantumCircuit":
-        """
-        √X gate.
-
-        Args:
-            pos (int): qubit the gate act.
-        """
-        self.add_ins(qeg.SXGate(pos))
-        return self
-
-    def sxdg(self, pos: int) -> "QuantumCircuit":
-        """
-        Inverse of √X gate.
-
-        Args:
-            pos (int): qubit the gate act.
-        """
-        gate = qeg.SXdgGate(pos)
-        self.add_ins(gate)
-        return self
-
-    def sy(self, pos: int) -> "QuantumCircuit":
-        """
-        √Y gate.
-
-        Args:
-            pos (int): qubit the gate act.
-        """
-        self.add_ins(qeg.SYGate(pos))
-        return self
-
-    def sydg(self, pos: int) -> "QuantumCircuit":
-        """
-        Inverse of √Y gate.
-
-        Args:
-            pos (int): qubit the gate act.
-        """
-        gate = qeg.SYdgGate(pos)
-        self.add_ins(gate)
-        return self
-
-    def w(self, pos: int) -> "QuantumCircuit":
-        """
-        W gate. (~(X + Y)/√2)
-
-        Args:
-            pos (int): qubit the gate act.
-        """
-        self.add_ins(qeg.WGate(pos))
-        return self
-
-    def sw(self, pos: int) -> "QuantumCircuit":
-        """
-        √W gate.
-
-        Args:
-            pos (int): qubit the gate act.
-        """
-        self.add_ins(qeg.SWGate(pos))
-        return self
-
-    def rx(self, pos: int, para: float) -> "QuantumCircuit":
-        """
-        Single qubit rotation Rx gate.
-
-        Args:
-            pos (int): qubit the gate act.
-            para (float): rotation angle
-        """
-        self.add_ins(qeg.RXGate(pos, para))
-        return self
-
-    def ry(self, pos: int, para: float) -> "QuantumCircuit":
-        """
-        Single qubit rotation Ry gate.
-
-        Args:
-            pos (int): qubit the gate act.
-            para (float): rotation angle
-        """
-        self.add_ins(qeg.RYGate(pos, para))
-        return self
-
-    def rz(self, pos: int, para: float) -> "QuantumCircuit":
-        """
-        Single qubit rotation Rz gate.
-
-        Args:
-            pos (int): qubit the gate act.
-            para (float): rotation angle
-        """
-        self.add_ins(qeg.RZGate(pos, para))
-        return self
-
-    def p(self, pos: int, para: float) -> "QuantumCircuit":
-        """
-        Phase gate
-
-        Args:
-            pos (int): qubit the gate act.
-            para (float): rotation angle
-        """
-        self.add_ins(qeg.PhaseGate(pos, para))
-        return self
-
-    def cnot(self, ctrl: int, tar: int) -> "QuantumCircuit":
-        """
-        CNOT gate.
-
-        Args:
-            ctrl (int): control qubit.
-            tar (int): target qubit.
-        """
-        self.add_ins(qeg.CXGate(ctrl, tar))
-        return self
-
-    def cx(self, ctrl: int, tar: int) -> "QuantumCircuit":
-        """
-        Ally of cnot.
-        """
-        return self.cnot(ctrl=ctrl, tar=tar)
-
-    def cy(self, ctrl: int, tar: int) -> "QuantumCircuit":
-        """
-        Control-Y gate.
-
-        Args:
-            ctrl (int): control qubit.
-            tar (int): target qubit.
-        """
-        self.add_ins(qeg.CYGate(ctrl, tar))
-        return self
-
-    def cz(self, ctrl: int, tar: int) -> "QuantumCircuit":
-        """
-        Control-Z gate.
-
-        Args:
-            ctrl (int): control qubit.
-            tar (int): target qubit.
-        """
-        self.add_ins(qeg.CZGate(ctrl, tar))
-        return self
-
-    def cs(self, ctrl: int, tar: int) -> "QuantumCircuit":
-        """
-        Control-S gate.
-
-        Args:
-            ctrl (int): control qubit.
-            tar (int): target qubit.
-        """
-        self.add_ins(qeg.CSGate(ctrl, tar))
-        return self
-
-    def ct(self, ctrl: int, tar: int) -> "QuantumCircuit":
-        """
-        Control-T gate.
-
-        Args:
-            ctrl (int): control qubit.
-            tar (int): target qubit.
-        """
-
-        self.add_ins(qeg.CTGate(ctrl, tar))
-        return self
-
-    def cp(self, ctrl: int, tar: int, para: float) -> "QuantumCircuit":
-        """
-        Control-P gate.
-
-        Args:
-            ctrl (int): control qubit.
-            tar (int): target qubit.
-            para: theta
-        """
-        self.add_ins(qeg.CPGate(ctrl, tar, para))
-        return self
-
-    def swap(self, q1: int, q2: int) -> "QuantumCircuit":
-        """
-        SWAP gate
-
-        Args:
-            q1 (int): qubit the gate act.
-            q2 (int): qubit the gate act.
-        """
-        self.add_ins(qeg.SwapGate(q1, q2))
-        return self
-
-    def iswap(self, q1: int, q2: int) -> "QuantumCircuit":
-        """
-        iSWAP gate
-
-        Args:
-            q1 (int): qubit the gate act.
-            q2 (int): qubit the gate act.
-        """
-        self.add_ins(qeg.ISwapGate(q1, q2))
-        return self
-
-    def toffoli(self, ctrl1: int, ctrl2: int, targ: int) -> "QuantumCircuit":
-        """
-        Toffoli gate
-
-        Args:
-            ctrl1 (int): control qubit
-            ctrl2 (int): control qubit
-            targ (int): target qubit
-        """
-        self.add_ins(qeg.ToffoliGate(ctrl1, ctrl2, targ))
-        return self
-
-    def fredkin(self, ctrl: int, targ1: int, targ2: int) -> "QuantumCircuit":
-        """
-        Fredkin gate
-
-        Args:
-            ctrl (int):  control qubit
-            targ1 (int): target qubit
-            targ2 (int): target qubit
-        """
-        self.add_ins(qeg.FredkinGate(ctrl, targ1, targ2))
-        return self
-
-    def barrier(self, qlist: List[int] = None) -> "QuantumCircuit":
-        """
-        Add barrier for qubits in qlist.
-
-        Args:
-            qlist (list[int]): A list contain the qubit need add barrier. When qlist contain at least two qubit, the barrier will be added from minimum qubit to maximum qubit. For example: barrier([0, 2]) create barrier for qubits 0, 1, 2. To create discrete barrier, using barrier([0]), barrier([2]).
-        """
-        if qlist is None:
-            qlist = list(range(self.num))
-        self.add_ins(Barrier(qlist))
-        return self
-
-    def delay(self, pos, duration, unit="ns") -> "QuantumCircuit":
-        """
-        Let the qubit idle for a certain duration.
-
-        Args:
-            pos (int): qubit need delay.
-            duration (int): duration of qubit delay, which represents integer times of unit.
-            unit (str): time unit for the duration. Can be "ns" and "us".
-        """
-        self.add_ins(Delay(pos, duration, unit=unit))
-        return self
-
-    def xy(self, qs: int, qe: int, duration: int, unit: str = "ns") -> "QuantumCircuit":
-        """
-        XY resonance time evolution for quantum simulator
-
-        Args:
-            qs: start position of resonant qubits.
-            qe: end position of resonant qubits.
-            duration: duration must be integer, which represents integer times of unit.
-            unit: time unit of duration.
-
-        """
-        self.add_ins(XYResonance(qs, qe, duration, unit=unit))
-        return self
-
-    def rxx(self, q1: int, q2: int, theta):
-        """
-        Rotation about 2-qubit XX axis.
-
-        Args:
-            q1 (int): qubit the gate act.
-            q2 (int): qubit the gate act.
-            theta: rotation angle.
-
-        """
-        self.add_ins(qeg.RXXGate(q1, q2, theta))
-
-    def ryy(self, q1: int, q2: int, theta):
-        """
-        Rotation about 2-qubit YY axis.
-
-        Args:
-            q1 (int): qubit the gate act.
-            q2 (int): qubit the gate act.
-            theta: rotation angle.
-
-        """
-        self.add_ins(qeg.RYYGate(q1, q2, theta))
-
-    def rzz(self, q1: int, q2: int, theta):
-        """
-        Rotation about 2-qubit ZZ axis.
-
-        Args:
-            q1 (int): qubit the gate act.
-            q2 (int): qubit the gate act.
-            theta: rotation angle.
-
-        """
-        self.add_ins(qeg.RZZGate(q1, q2, theta))
-
-    def mcx(self, ctrls: List[int], targ: int):
-        """
-        Multi-controlled X gate.
-
-        Args:
-            ctrls: A list of control qubits.
-            targ: Target qubits.
-        """
-        self.add_ins(qeg.MCXGate(ctrls, targ))
-
-    def mcy(self, ctrls: List[int], targ: int):
-        """
-        Multi-controlled Y gate.
-
-        Args:
-            ctrls: A list of control qubits.
-            targ: Target qubits.
-        """
-        self.add_ins(qeg.MCYGate(ctrls, targ))
-
-    def mcz(self, ctrls: List[int], targ: int):
-        """
-        Multi-controlled Z gate.
-
-        Args:
-            ctrls: A list of control qubits.
-            targ: Target qubits.
-        """
-        self.add_ins(qeg.MCZGate(ctrls, targ))
-
-    def unitary(self, matrix: np.ndarray, pos: List[int]):
-        """
-        Apply unitary to circuit on specified qubits.
-
-        Args:
-            matrix (np.ndarray): unitary matrix.
-            pos (list[int]): qubits the gate act on.
-        """
-        compiler = qeg.UnitaryDecomposer(array=matrix, qubits=pos)
-        compiler.apply_to_qc(self)
-
-    def measure(self, pos: List[int] = None, cbits: List[int] = None) -> None:
-        """
-        Measurement setting for experiment device.
-
-        Args:
-            pos: Qubits need measure.
-            cbits: Classical bits keeping the measure results.
-        """
-        # checking
-        if pos is None:
-            pos = list(range(self.num))
-        if np.any(np.array(pos) >= self.num):
-            raise ValueError("Index out of range.")
-
-        e_num = len(self.measures)  # existing num of measures
-        n_num = len(pos)  # newly added num of measures
-        if n_num > len(set(pos)):
-            raise ValueError("Measured qubits not uniquely assigned.")
-
-        if cbits:
-            if not len(set(cbits)) == len(cbits):
-                raise ValueError("Classical bits not uniquely assigned.")
-            if not len(cbits) == n_num:
-                raise ValueError("Number of measured bits should equal to the number of classical bits")
-        else:
-            cbits = list(range(e_num, e_num + n_num))
-        # _sorted_indices = sorted(range(n_num), key=lambda k: cbits[k])
-        # cbits = [_sorted_indices.index(i) + e_num for i in range(n_num)]
-
-        measure = Measure(dict(zip(pos, cbits)))
-        self._measures.append(measure)
-        self.add_ins(measure)
-
-    def add_pulse(self,
-                  pulse: QuantumPulse,
-                  pos: int = None) -> "QuantumCircuit":
-        """
-        Add quantum gate from pulse.
-        """
-        if pos is not None:
-            pulse.pos = pos
-        self.add_ins(pulse)
-        return self
+# (C) Copyright 2023 Beijing Academy of Quantum Information Sciences
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#    http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import copy
+from contextlib import contextmanager
+from typing import Any, Iterable, List, Optional
+
+import numpy as np
+import quafu.elements.element_gates as qeg
+from quafu.elements import Measure, Reset, UnitaryDecomposer
+from quafu.elements.classical_element import Cif
+from quafu.elements.instruction import Instruction
+from quafu.elements.parameters import Parameter, ParameterExpression, ParameterType
+
+from ..elements import (
+    Barrier,
+    CircuitWrapper,
+    ControlledCircuitWrapper,
+    ControlledGate,
+    ControlledOracle,
+    Delay,
+    KrausChannel,
+    OracleGate,
+    QuantumGate,
+    QuantumPulse,
+    XYResonance,
+)
+from ..elements.quantum_gate import CircuitWrapper, ControlledCircuitWrapper
+from ..exceptions import CircuitError
+from .classical_register import ClassicalRegister
+from .quantum_register import QuantumRegister
+
+
+class QuantumCircuit:
+    """
+    Representation of quantum circuit.
+    """
+
+    def __init__(self, qnum: int, cnum: Optional[int] = None, name="", *args, **kwargs):
+        """
+        Initialize a QuantumCircuit object
+
+        Args:
+            qnum (int): Total qubit number used
+            cnum (int): Classical bit number, equals to qubit number in default
+        """
+        self.name = name
+        self.qregs = [QuantumRegister(qnum)] if qnum > 0 else []
+        cnum = self.num if cnum is None else cnum
+        self.cregs = [ClassicalRegister(cnum)] if cnum > 0 else []
+        self._gates = []
+        self.instructions = []
+        self.openqasm = ""
+        self.circuit = []
+        self._measures = []
+        self.executable_on_backend = True
+        self._used_qubits = []
+        self._parameterized_gates = []
+        self._parameter_grads = {}
+        self._variables = []
+        self._has_wrap = False
+
+    @property
+    def parameterized_gates(self):
+        """Return the list of gates which the parameters are tunable"""
+        if not self._parameterized_gates:
+            self._parameterized_gates = [g for g in self.gates if len(g.paras) != 0]
+        return self._parameterized_gates
+
+    @property
+    def num(self):
+        return sum([len(qreg) for qreg in self.qregs])
+
+    @num.setter
+    def num(self, num: int):
+        self.qregs = [QuantumRegister(num)] if num > 0 else []
+        self.cregs = [ClassicalRegister(num)] if num > 0 else []
+
+    @property
+    def cbits_num(self):
+        return sum([len(creg) for creg in self.cregs])
+
+    @property
+    def used_qubits(self) -> List:
+        self.layered_circuit()
+        return self._used_qubits
+
+    @property
+    def measures(self):
+        measures = {}
+        for meas in self._measures:
+            measures.update(dict(zip(meas.qbits, meas.cbits)))
+        return measures
+
+    @measures.setter
+    def measures(self, measures: dict):
+        self._measures = [Measure(measures)]
+
+    @property
+    def gates(self):
+        """Deprecated warning: due to historical reason, ``gates`` contains not only instances of
+        QuantumGate, meanwhile not contains measurements. This attributes might be deprecated in
+        the future. Better to use ``instructions`` which contains all the instructions.
+        """
+        return self._gates
+
+    @gates.setter
+    def gates(self, gates: list):
+        self._gates = gates
+
+    def __lshift__(self, operation: Instruction):
+        max_pos = (
+            max(operation.pos) if isinstance(operation.pos, Iterable) else operation.pos
+        )
+        if max_pos >= self.num:
+            raise CircuitError("Operation act on qubit that not allocated")
+        self.add_ins(operation)
+        if isinstance(operation, CircuitWrapper):
+            self._has_wrap = True
+        return self
+
+    # TODO(qtzhuang): add_gates is just a temporary call function to add gate from gate_list
+    def add_gates(self, gates: list):
+        for gate in gates:
+            self.add_ins(gate)
+
+    def add_gate(self, gate: QuantumGate):
+        """
+        Add quantum gate to circuit, with some checking.
+        """
+        pos = np.array(gate.pos)
+        if np.any(pos >= self.num):
+            raise CircuitError(f"Gate position out of range: {gate.pos}")
+        self.gates.append(gate)
+
+    def add_pulse(self, pulse: QuantumPulse, pos: int = None) -> "QuantumCircuit":
+        """
+        Add quantum gate from pulse.
+        """
+        if pos is not None:
+            pulse.set_pos(pos)
+        self.add_ins(pulse)
+        return self
+
+    def add_ins(self, ins: Instruction):
+        """
+        Add instruction to circuit, with NO checking yet.
+        """
+        if isinstance(ins, (QuantumGate, Delay, Barrier, XYResonance, KrausChannel)):
+            # TODO: Delay, Barrier added by add_gate for backward compatibility.
+            #       Figure out better handling in the future.
+            self.add_gate(ins)
+        self.instructions.append(ins)
+
+    def add_noise(self, channel: str, channel_args, qubits=[], gates=[]):
+        if channel not in ["bitflip", "dephasing", "depolarizing", "ampdamping"]:
+            raise ValueError("Invalid channel name")
+
+        for g in gates:
+            if g not in list(QuantumGate.gate_classes.keys()):
+                raise ValueError("Invalid gate name")
+
+        newinstructions = []
+        newgates = []
+        for op in self.instructions:
+            newinstructions.append(op)
+            if isinstance(op, (QuantumGate, Delay, Barrier, XYResonance)):
+                newgates.append(op)
+            if isinstance(op, QuantumGate):
+                add_q = False
+                add_g = False
+                if qubits:
+                    for q in op.pos:
+                        if q in qubits:
+                            add_q = True
+                else:
+                    add_q = True
+
+                if gates:
+                    if op.name.lower() in gates:
+                        add_g = True
+                else:
+                    add_g = True
+
+                if add_q and add_g:
+                    for q in op.pos:
+                        if q in qubits:
+                            newinstructions.append(
+                                Instruction.ins_classes[channel](q, *channel_args)
+                            )
+                            newgates.append(
+                                Instruction.ins_classes[channel](q, *channel_args)
+                            )
+        self.instructions = newinstructions
+        self._gates = newgates
+        return self
+
+    @property
+    def noised(self):
+        if self._has_wrap:
+            self.unwrap()
+
+        for op in self.instructions:
+            if isinstance(op, KrausChannel):
+                return True
+        return False
+
+    def get_parameter_grads(self):
+        if self._has_wrap:
+            print(
+                "warning: The circuit has wrapped gates, it will unwarp automaticllay"
+            )
+            self.unwrap()
+        self._parameter_grads = {}
+        for i, op in enumerate(self.gates):
+            for j, para in enumerate(op.paras):
+                if isinstance(para, Parameter):
+                    if para not in self._parameter_grads.keys():
+                        self._parameter_grads[para] = [[(i, j), 1.0]]
+                    else:
+                        self._parameter_grads[para].append([(i, j), 1.0])
+
+                elif isinstance(para, ParameterExpression):
+                    para_grads = para.grad()
+                    for var in para._variables:
+                        if var not in self._parameter_grads.keys():
+                            self._parameter_grads[var] = [
+                                [(i, j), para_grads[para._variables[var]]]
+                            ]
+                        else:
+                            self._parameter_grads[var].append(
+                                [(i, j), para_grads[para._variables[var]]]
+                            )
+        self._variables = list(self._parameter_grads.keys())
+        return self._parameter_grads
+
+    def _calc_parameter_grads(self):
+        """
+        Update parameter gradient value, not variables
+        """
+        for var, grads in self._parameter_grads.items():
+            for item in grads:
+                i, j = item[0]
+                para = self.gates[i].paras[j]
+                if isinstance(para, ParameterExpression):
+                    para_grads = para.grad()
+                    item[1] = para_grads[para._variables[var]]
+
+        return self._parameter_grads
+
+    @property
+    def variables(self):
+        self._variables = list(self.get_parameter_grads().keys())
+        return self._variables
+
+    def _update_params(self, values, order=[]):
+        """
+        Update variables' value, not variables
+        Args:
+            values: list of variables' value.
+            order: For transplied circuit that change the order of variables,
+            need pass the order to match untranspiled circuit's variable.
+        """
+
+        for i in range(len(values)):
+            val = values[order[i]] if order else values[i]
+            self._variables[i].value = val
+
+    def update_params(self, paras_list: List[Any]):
+        """Update parameters of parameterized gates
+        Args:
+            paras_list (List[Any]): list of params
+
+        Raise:
+            CircuitError
+        """
+        if len(paras_list) != len(self.parameterized_gates):
+            raise CircuitError(
+                "`params_list` must have the same size with parameterized gates"
+            )
+
+        # TODO(): Support updating part of params of a single gate
+        for gate, paras in zip(self.parameterized_gates, paras_list):
+            gate.update_params(paras)
+
+    def layered_circuit(self) -> np.ndarray:
+        """
+        Make layered circuit from the gate sequence self.gates.
+
+        Returns:
+            A layered list with left justed circuit.
+        """
+        num = self.num
+        gatelist = self.gates
+        gateQlist = [[] for i in range(num)]
+        used_qubits = []
+        for gate in gatelist:
+            if isinstance(gate, Delay) or isinstance(gate, QuantumPulse):
+                gateQlist[gate.pos].append(gate)
+                if gate.pos not in used_qubits:
+                    used_qubits.append(gate.pos)
+
+            else:
+                pos1 = min(gate.pos)
+                pos2 = max(gate.pos)
+                gateQlist[pos1].append(gate)
+                for j in range(pos1 + 1, pos2 + 1):
+                    gateQlist[j].append(None)
+
+                for pos in gate.pos:
+                    if pos not in used_qubits:
+                        used_qubits.append(pos)
+
+                maxlayer = max([len(gateQlist[j]) for j in range(pos1, pos2 + 1)])
+                for j in range(pos1, pos2 + 1):
+                    layerj = len(gateQlist[j])
+                    pos = layerj - 1
+                    if not layerj == maxlayer:
+                        for i in range(abs(layerj - maxlayer)):
+                            gateQlist[j].insert(pos, None)
+
+        # Add support of used_qubits for Reset and Cif
+        def get_used_qubits(instructions):
+            used_q = []
+            for ins in instructions:
+                if isinstance(ins, Cif):
+                    used_q_h = get_used_qubits(ins.instructions)
+                    for pos in used_q_h:
+                        if pos not in used_q:
+                            used_q.append(pos)
+                elif isinstance(ins, Barrier):
+                    continue
+                elif isinstance(ins.pos, int):
+                    if ins.pos not in used_q:
+                        used_q.append(ins.pos)
+                elif isinstance(ins.pos, list):
+                    for pos in ins.pos:
+                        if pos not in used_q:
+                            used_q.append(pos)
+            return used_q
+
+        # Only consider of reset and cif
+        for ins in self.instructions:
+            if isinstance(ins, (Reset, Cif)):
+                used_q = get_used_qubits([ins])
+                for pos in used_q:
+                    if pos not in used_qubits:
+                        used_qubits.append(pos)
+
+        maxdepth = max([len(gateQlist[i]) for i in range(num)])
+
+        for gates in gateQlist:
+            gates.extend([None] * (maxdepth - len(gates)))
+
+        for m in self.measures.keys():
+            if m not in used_qubits:
+                used_qubits.append(m)
+        used_qubits = np.sort(used_qubits)
+
+        new_gateQlist = []
+        for old_qi in range(len(gateQlist)):
+            gates = gateQlist[old_qi]
+            if old_qi in used_qubits:
+                new_gateQlist.append(gates)
+
+        lc = np.array(new_gateQlist)
+        lc = np.vstack((used_qubits, lc.T)).T
+        self.circuit = lc
+        self._used_qubits = list(used_qubits)
+        return self.circuit
+
+    def draw_circuit(self, width: int = 4, return_str: bool = False):
+        """
+        Draw layered circuit using ASCII, print in terminal.
+        Args:
+            width (int): The width of each gate.
+            return_str: Whether return the circuit string.
+        """
+        # TODO: support draw other instructions
+        self.layered_circuit()
+        gateQlist = self.circuit
+        num = gateQlist.shape[0]
+        depth = gateQlist.shape[1] - 1
+        printlist = np.array([[""] * depth for i in range(2 * num)], dtype="<U30")
+
+        reduce_map = dict(zip(gateQlist[:, 0], range(num)))
+        reduce_map_inv = dict(zip(range(num), gateQlist[:, 0]))
+        for l in range(depth):
+            layergates = gateQlist[:, l + 1]
+            maxlen = 1 + width
+            for i in range(num):
+                gate = layergates[i]
+                if isinstance(gate, Barrier):
+                    pos = [i for i in gate.pos if i in reduce_map.keys()]
+                    q1 = reduce_map[min(pos)]
+                    q2 = reduce_map[max(pos)]
+                    printlist[2 * q1 : 2 * q2 + 1, l] = "||"
+                    maxlen = max(maxlen, len("||"))
+                elif isinstance(gate, Instruction) and len(gate.pos) == 1:
+                    printlist[i * 2, l] = gate.symbol
+                    maxlen = max(maxlen, len(gate.symbol) + width)
+
+                elif isinstance(gate, Instruction) and len(gate.pos) > 1:
+                    q1 = reduce_map[min(gate.pos)]
+                    q2 = reduce_map[max(gate.pos)]
+                    printlist[2 * q1 + 1 : 2 * q2, l] = "|"
+                    printlist[q1 * 2, l] = "#"
+                    printlist[q2 * 2, l] = "#"
+                    if isinstance(gate, ControlledGate):  # Controlled-Multiqubit gate
+                        for ctrl in gate.ctrls:
+                            printlist[reduce_map[ctrl] * 2, l] = "*"
+
+                        if gate._targ_name == "SWAP":
+                            printlist[reduce_map[gate.targs[0]] * 2, l] = "x"
+                            printlist[reduce_map[gate.targs[1]] * 2, l] = "x"
+                        else:
+                            tq1 = reduce_map[min(gate.targs)]
+                            tq2 = reduce_map[max(gate.targs)]
+                            printlist[tq1 * 2, l] = "#"
+                            printlist[tq2 * 2, l] = "#"
+                            if tq1 + tq2 in [
+                                reduce_map[ctrl] * 2 for ctrl in gate.ctrls
+                            ]:
+                                printlist[tq1 + tq2, l] = "*" + gate.symbol
+                            else:
+                                printlist[tq1 + tq2, l] = gate.symbol
+                            maxlen = max(maxlen, len(gate.symbol) + width)
+
+                    else:  # Multiqubit gate
+                        if gate.name == "SWAP":
+                            printlist[q1 * 2, l] = "x"
+                            printlist[q2 * 2, l] = "x"
+
+                        else:
+                            printlist[q1 + q2, l] = gate.symbol
+                            maxlen = max(maxlen, len(gate.symbol) + width)
+
+            printlist[-1, l] = maxlen
+
+        circuitstr = []
+        for j in range(2 * num - 1):
+            if j % 2 == 0:
+                linestr = ("q[%d]" % (reduce_map_inv[j // 2])).ljust(6) + "".join(
+                    [
+                        printlist[j, l].center(int(printlist[-1, l]), "-")
+                        for l in range(depth)
+                    ]
+                )
+                if reduce_map_inv[j // 2] in self.measures.keys():
+                    linestr += " M->c[%d]" % self.measures[reduce_map_inv[j // 2]]
+                circuitstr.append(linestr)
+            else:
+                circuitstr.append(
+                    "".ljust(6)
+                    + "".join(
+                        [
+                            printlist[j, l].center(int(printlist[-1, l]), " ")
+                            for l in range(depth)
+                        ]
+                    )
+                )
+        circuitstr = "\n".join(circuitstr)
+
+        if return_str:
+            return circuitstr
+        else:
+            print(circuitstr)
+
+    def plot_circuit(self, *args, **kwargs):
+        from quafu.visualisation.circuitPlot import CircuitPlotManager
+
+        cmp = CircuitPlotManager(self)
+        return cmp(*args, **kwargs)
+
+    def from_openqasm(self, openqasm: str):
+        """
+        Initialize the circuit from openqasm text.
+        Args:
+            openqasm: input openqasm str.
+        """
+        from quafu.qfasm.qfasm_convertor import qasm2_to_quafu_qc
+
+        return qasm2_to_quafu_qc(self, openqasm)
+
+    def to_openqasm(self, with_para=False) -> str:
+        """
+        Convert the circuit to openqasm text.
+
+        Returns:
+            openqasm text.
+        """
+
+        valid_gates = list(
+            QuantumGate.gate_classes.keys()
+        )  # TODO:include instruction futher
+        valid_gates.extend(["barrier", "delay", "reset"])
+
+        qasm = 'OPENQASM 2.0;\ninclude "qelib1.inc";\n'
+        qasm += "qreg q[%d];\n" % self.num
+        qasm += "creg meas[%d];\n" % self.cbits_num
+        if with_para:
+            for variable in self.variables:
+                qasm += f"{variable.latex} = {variable.value};\n"
+        for gate in self.gates:
+            if gate.name.lower() in valid_gates:
+                qasm += gate.to_qasm(with_para) + ";\n"
+            else:
+                # TODO: add decompose subroutine
+                raise NotImplementedError(
+                    f"gate {gate.name} can not convert to qasm2 directly, you may decompose it manuallly"
+                )
+        for key in self.measures:
+            qasm += "measure q[%d] -> meas[%d];\n" % (key, self.measures[key])
+
+        self.openqasm = qasm
+        return qasm
+
+    def wrap_to_gate(self, name: str):
+        """
+        Wrap the circuit to a subclass of QuantumGate, create by metaclass.
+        """
+        from copy import deepcopy
+
+        from quafu.elements.oracle import customize_gate
+
+        # TODO: check validity of instructions
+        gate_structure = [deepcopy(ins) for ins in self.instructions]
+        customized = customize_gate(name, gate_structure, self.num)
+        return customized
+
+    def _reallocate(self, num, qbits: List[int]):
+        """Remap the qubits and gates to new positions."""
+        assert self.num == len(qbits)
+        if max(qbits) > num:
+            raise CircuitError("Bad allocation")
+
+        self.num = num
+        qbits_map = dict(zip(range(len(qbits)), qbits))
+        gates = self.instructions
+        for op in gates:
+            for i in range(len(op.pos)):
+                op.pos[i] = qbits_map[op.pos[i]]
+
+            if isinstance(op, ControlledGate):
+                for i in range(len(op.ctrls)):
+                    op.ctrls[i] = qbits_map[op.ctrls[i]]
+
+                for i in range(len(op.targs)):
+                    op.targs[i] = qbits_map[op.targs[i]]
+
+    def add_controls(
+        self, ctrlnum, ctrls: List[int] = [], targs: List[int] = [], inplace=False
+    ) -> "QuantumCircuit":
+        num = 0
+        instrs = []
+        if len(ctrls + targs) == 0:
+            ctrls = list(np.arange(ctrlnum) + self.num)
+            num = self.num + ctrlnum
+            instrs = self.instructions
+        else:
+            if len(ctrls) == 0 or len(targs) == 0:
+                raise ValueError("Must provide both ctrls and targs")
+            else:
+                assert len(targs) == self.num
+                assert len(ctrls) == ctrlnum
+                num = max(ctrls + targs) + 1
+                if inplace:
+                    self._reallocate(num, targs)
+                else:
+                    temp = copy.deepcopy(self)
+                    temp._reallocate(num, targs)
+                    instrs = temp.instructions
+
+        if inplace:
+            for op in self.instructions:
+                if isinstance(op, QuantumGate):
+                    op = op.ctrl_by(ctrls)
+            return self
+        else:
+            qc = QuantumCircuit(num)
+            for op in instrs:
+                if isinstance(op, QuantumGate):
+                    qc << op.ctrl_by(ctrls)
+        return qc
+
+    def join(
+        self,
+        qc: ["QuantumCircuit", CircuitWrapper, ControlledCircuitWrapper],
+        qbits: List[int] = [],
+        inplace=True,
+    ) -> "QuantumCircuit":
+        num = self.num
+        rnum = 0
+        if isinstance(qc, QuantumCircuit):
+            rnum = qc.num
+        else:
+            rnum = qc.circuit.num
+
+        if len(qbits) == 0:
+            num = max(self.num, rnum)
+        else:
+            num = max(self.num - 1, max(qbits)) + 1
+
+        nqc = QuantumCircuit(num)
+        if inplace:
+            self.num = num
+            nqc = self
+        else:
+            for op in self.instructions:
+                nqc << op
+
+        if isinstance(qc, QuantumCircuit):
+            if qbits:
+                newqc = copy.deepcopy(qc)
+                newqc._reallocate(num, qbits)
+                for op in newqc.instructions:
+                    nqc << op
+            else:
+                for op in qc.instructions:
+                    nqc << op
+        else:
+            if qbits:
+                qc._reallocate(qbits)
+            nqc << qc
+
+        return nqc
+
+    def power(self, n, inplace=False):
+        if inplace:
+            for _ in range(n - 1):
+                self.instructions += self.instructions
+            return self
+        else:
+            nq = QuantumCircuit(self.num)
+            for _ in range(n):
+                for op in self.instructions:
+                    nq << op
+            nq.measures = self.measures
+            return nq
+
+    def dagger(self, inplace=False):
+        if inplace:
+            self.instructions = self.instructions[::-1]
+            for op in self.instructions:
+                if isinstance(op, QuantumGate):
+                    op = op.dagger()
+            return self
+        else:
+            nq = QuantumCircuit(self.num)
+            for op in self.instructions[::-1]:
+                if isinstance(op, QuantumGate):
+                    nq << op.dagger()
+                else:
+                    nq << op
+            nq.measures = self.measures
+            return nq
+
+    def wrap(self, qbits=[]):
+        # TODO:use OracleGate
+        name = self.name if self.name else "Oracle"
+        return CircuitWrapper(name, self, qbits)
+
+    def unwrap(self):
+        instructions = []
+        gates = []
+        for op in self.instructions:
+            if isinstance(op, CircuitWrapper):
+                circ = op.circuit.unwrap()
+                for op_ in circ.instructions:
+                    instructions.append(op_)
+                    if isinstance(
+                        op_, (QuantumGate, Delay, Barrier, XYResonance, KrausChannel)
+                    ):
+                        gates.append(op_)
+            else:
+                instructions.append(op)
+                if isinstance(
+                    op, (QuantumGate, Delay, Barrier, XYResonance, KrausChannel)
+                ):
+                    gates.append(op)
+
+        self.instructions = instructions
+        self._gates = gates
+        self._has_wrap = False
+        return self
+
+    # # # # # # # # # # # # # # helper functions # # # # # # # # # # # # # #
+    def id(self, pos: int) -> "QuantumCircuit":
+        """
+        Identity gate.
+
+        Args:
+            pos (int): qubit the gate act.
+        """
+        gate = qeg.IdGate(pos)
+        self.add_ins(gate)
+        return self
+
+    def h(self, pos: int) -> "QuantumCircuit":
+        """
+        Hadamard gate.
+
+        Args:
+            pos (int): qubit the gate act.
+        """
+        gate = qeg.HGate(pos)
+        self.add_ins(gate)
+        return self
+
+    def x(self, pos: int) -> "QuantumCircuit":
+        """
+        X gate.
+
+        Args:
+            pos (int): qubit the gate act.
+        """
+        gate = qeg.XGate(pos)
+        self.add_ins(gate)
+        return self
+
+    def y(self, pos: int) -> "QuantumCircuit":
+        """
+        Y gate.
+
+        Args:
+            pos (int): qubit the gate act.
+        """
+        gate = qeg.YGate(pos)
+        self.add_ins(gate)
+        return self
+
+    def z(self, pos: int) -> "QuantumCircuit":
+        """
+        Z gate.
+
+        Args:
+            pos (int): qubit the gate act.
+        """
+        self.add_ins(qeg.ZGate(pos))
+        return self
+
+    def t(self, pos: int) -> "QuantumCircuit":
+        """
+        T gate. (~Z^(1/4))
+
+        Args:
+            pos (int): qubit the gate act.
+        """
+        self.add_ins(qeg.TGate(pos))
+        return self
+
+    def tdg(self, pos: int) -> "QuantumCircuit":
+        """
+        Tdg gate. (Inverse of T gate)
+
+        Args:
+            pos (int): qubit the gate act.
+        """
+        self.add_ins(qeg.TdgGate(pos))
+        return self
+
+    def s(self, pos: int) -> "QuantumCircuit":
+        """
+        S gate. (~√Z)
+
+        Args:
+            pos (int): qubit the gate act.
+        """
+        self.add_ins(qeg.SGate(pos))
+        return self
+
+    def sdg(self, pos: int) -> "QuantumCircuit":
+        """
+        Sdg gate. (Inverse of S gate)
+
+        Args:
+            pos (int): qubit the gate act.
+        """
+        self.add_ins(qeg.SdgGate(pos))
+        return self
+
+    def sx(self, pos: int) -> "QuantumCircuit":
+        """
+        √X gate.
+
+        Args:
+            pos (int): qubit the gate act.
+        """
+        self.add_ins(qeg.SXGate(pos))
+        return self
+
+    def sxdg(self, pos: int) -> "QuantumCircuit":
+        """
+        Inverse of √X gate.
+
+        Args:
+            pos (int): qubit the gate act.
+        """
+        gate = qeg.SXdgGate(pos)
+        self.add_ins(gate)
+        return self
+
+    def sy(self, pos: int) -> "QuantumCircuit":
+        """
+        √Y gate.
+
+        Args:
+            pos (int): qubit the gate act.
+        """
+        self.add_ins(qeg.SYGate(pos))
+        return self
+
+    def sydg(self, pos: int) -> "QuantumCircuit":
+        """
+        Inverse of √Y gate.
+
+        Args:
+            pos (int): qubit the gate act.
+        """
+        gate = qeg.SYdgGate(pos)
+        self.add_ins(gate)
+        return self
+
+    def w(self, pos: int) -> "QuantumCircuit":
+        """
+        W gate. (~(X + Y)/√2)
+
+        Args:
+            pos (int): qubit the gate act.
+        """
+        self.add_ins(qeg.WGate(pos))
+        return self
+
+    def sw(self, pos: int) -> "QuantumCircuit":
+        """
+        √W gate.
+
+        Args:
+            pos (int): qubit the gate act.
+        """
+        self.add_ins(qeg.SWGate(pos))
+        return self
+
+    def rx(self, pos: int, para: ParameterType) -> "QuantumCircuit":
+        """
+        Single qubit rotation Rx gate.
+
+        Args:
+            pos (int): qubit the gate act.
+            para (float): rotation angle
+        """
+        self.add_ins(qeg.RXGate(pos, para))
+        return self
+
+    def ry(self, pos: int, para: ParameterType) -> "QuantumCircuit":
+        """
+        Single qubit rotation Ry gate.
+
+        Args:
+            pos (int): qubit the gate act.
+            para (float): rotation angle
+        """
+        self.add_ins(qeg.RYGate(pos, para))
+        return self
+
+    def rz(self, pos: int, para: ParameterType) -> "QuantumCircuit":
+        """
+        Single qubit rotation Rz gate.
+
+        Args:
+            pos (int): qubit the gate act.
+            para (float): rotation angle
+        """
+        self.add_ins(qeg.RZGate(pos, para))
+        return self
+
+    def p(self, pos: int, para: ParameterType) -> "QuantumCircuit":
+        """
+        Phase gate
+
+        Args:
+            pos (int): qubit the gate act.
+            para (float): rotation angle
+        """
+        self.add_ins(qeg.PhaseGate(pos, para))
+        return self
+
+    def cnot(self, ctrl: int, tar: int) -> "QuantumCircuit":
+        """
+        CNOT gate.
+
+        Args:
+            ctrl (int): control qubit.
+            tar (int): target qubit.
+        """
+        self.add_ins(qeg.CXGate(ctrl, tar))
+        return self
+
+    def cx(self, ctrl: int, tar: int) -> "QuantumCircuit":
+        """
+        Ally of cnot.
+        """
+        return self.cnot(ctrl=ctrl, tar=tar)
+
+    def cy(self, ctrl: int, tar: int) -> "QuantumCircuit":
+        """
+        Control-Y gate.
+
+        Args:
+            ctrl (int): control qubit.
+            tar (int): target qubit.
+        """
+        self.add_ins(qeg.CYGate(ctrl, tar))
+        return self
+
+    def cz(self, ctrl: int, tar: int) -> "QuantumCircuit":
+        """
+        Control-Z gate.
+
+        Args:
+            ctrl (int): control qubit.
+            tar (int): target qubit.
+        """
+        self.add_ins(qeg.CZGate(ctrl, tar))
+        return self
+
+    def cs(self, ctrl: int, tar: int) -> "QuantumCircuit":
+        """
+        Control-S gate.
+
+        Args:
+            ctrl (int): control qubit.
+            tar (int): target qubit.
+        """
+        self.add_ins(qeg.CSGate(ctrl, tar))
+        return self
+
+    def ct(self, ctrl: int, tar: int) -> "QuantumCircuit":
+        """
+        Control-T gate.
+
+        Args:
+            ctrl (int): control qubit.
+            tar (int): target qubit.
+        """
+
+        self.add_ins(qeg.CTGate(ctrl, tar))
+        return self
+
+    def cp(self, ctrl: int, tar: int, para: ParameterType) -> "QuantumCircuit":
+        """
+        Control-P gate.
+
+        Args:
+            ctrl (int): control qubit.
+            tar (int): target qubit.
+            para: theta
+        """
+        self.add_ins(qeg.CPGate(ctrl, tar, para))
+        return self
+
+    def swap(self, q1: int, q2: int) -> "QuantumCircuit":
+        """
+        SWAP gate
+
+        Args:
+            q1 (int): qubit the gate act.
+            q2 (int): qubit the gate act.
+        """
+        self.add_ins(qeg.SwapGate(q1, q2))
+        return self
+
+    def iswap(self, q1: int, q2: int) -> "QuantumCircuit":
+        """
+        iSWAP gate
+
+        Args:
+            q1 (int): qubit the gate act.
+            q2 (int): qubit the gate act.
+        """
+        self.add_ins(qeg.ISwapGate(q1, q2))
+        return self
+
+    def toffoli(self, ctrl1: int, ctrl2: int, targ: int) -> "QuantumCircuit":
+        """
+        Toffoli gate
+
+        Args:
+            ctrl1 (int): control qubit
+            ctrl2 (int): control qubit
+            targ (int): target qubit
+        """
+        self.add_ins(qeg.ToffoliGate(ctrl1, ctrl2, targ))
+        return self
+
+    def fredkin(self, ctrl: int, targ1: int, targ2: int) -> "QuantumCircuit":
+        """
+        Fredkin gate
+
+        Args:
+            ctrl (int):  control qubit
+            targ1 (int): target qubit
+            targ2 (int): target qubit
+        """
+        self.add_ins(qeg.FredkinGate(ctrl, targ1, targ2))
+        return self
+
+    def barrier(self, qlist: List[int] = None) -> "QuantumCircuit":
+        """
+        Add barrier for qubits in qlist.
+
+        Args:
+            qlist (list[int]): A list contain the qubit need add barrier. When qlist contain at least two qubit, the barrier will be added from minimum qubit to maximum qubit. For example: barrier([0, 2]) create barrier for qubits 0, 1, 2. To create discrete barrier, using barrier([0]), barrier([2]).
+        """
+        if qlist is None:
+            qlist = list(range(self.num))
+        self.add_ins(Barrier(qlist))
+        return self
+
+    def xy(self, qs: int, qe: int, duration: int, unit: str = "ns") -> "QuantumCircuit":
+        """
+        XY resonance time evolution for quantum simulator
+
+        Args:
+            qs: start position of resonant qubits.
+            qe: end position of resonant qubits.
+            duration: duration must be integer, which represents integer times of unit.
+            unit: time unit of duration.
+
+        """
+        self.add_ins(XYResonance(qs, qe, duration, unit=unit))
+        return self
+
+    def rxx(self, q1: int, q2: int, theta):
+        """
+        Rotation about 2-qubit XX axis.
+
+        Args:
+            q1 (int): qubit the gate act.
+            q2 (int): qubit the gate act.
+            theta: rotation angle.
+
+        """
+        self.add_ins(qeg.RXXGate(q1, q2, theta))
+
+    def ryy(self, q1: int, q2: int, theta):
+        """
+        Rotation about 2-qubit YY axis.
+
+        Args:
+            q1 (int): qubit the gate act.
+            q2 (int): qubit the gate act.
+            theta: rotation angle.
+
+        """
+        self.add_ins(qeg.RYYGate(q1, q2, theta))
+
+    def rzz(self, q1: int, q2: int, theta):
+        """
+        Rotation about 2-qubit ZZ axis.
+
+        Args:
+            q1 (int): qubit the gate act.
+            q2 (int): qubit the gate act.
+            theta: rotation angle.
+
+        """
+        self.add_ins(qeg.RZZGate(q1, q2, theta))
+
+    def mcx(self, ctrls: List[int], targ: int):
+        """
+        Multi-controlled X gate.
+
+        Args:
+            ctrls: A list of control qubits.
+            targ: Target qubits.
+        """
+        self.add_ins(qeg.MCXGate(ctrls, targ))
+
+    def mcy(self, ctrls: List[int], targ: int):
+        """
+        Multi-controlled Y gate.
+
+        Args:
+            ctrls: A list of control qubits.
+            targ: Target qubits.
+        """
+        self.add_ins(qeg.MCYGate(ctrls, targ))
+
+    def mcz(self, ctrls: List[int], targ: int):
+        """
+        Multi-controlled Z gate.
+
+        Args:
+            ctrls: A list of control qubits.
+            targ: Target qubits.
+        """
+        self.add_ins(qeg.MCZGate(ctrls, targ))
+
+    def unitary(self, matrix: np.ndarray, pos: List[int]):
+        """
+        Apply unitary to circuit on specified qubits.
+
+        Args:
+            matrix (np.ndarray): unitary matrix.
+            pos (list[int]): qubits the gate act on.
+        """
+        compiler = UnitaryDecomposer(array=matrix, qubits=pos)
+        compiler.apply_to_qc(self)
+
+    def delay(self, pos, duration, unit="ns") -> "QuantumCircuit":
+        """
+        Let the qubit idle for a certain duration.
+
+        Args:
+            pos (int): qubit need delay.
+            duration (int): duration of qubit delay, which represents integer times of unit.
+            unit (str): time unit for the duration. Can be "ns" and "us".
+        """
+        self.add_ins(Delay(pos, duration, unit=unit))
+        return self
+
+    def reset(self, qlist: List[int] = None) -> "QuantumCircuit":
+        """
+        Add reset for qubits in qlist.
+
+        Args:
+            qlist (list[int]): A list contain the qubit need add reset. When qlist contain at least two qubit, the barrier will be added from minimum qubit to maximum qubit. For example: barrier([0, 2]) create barrier for qubits 0, 1, 2. To create discrete barrier, using barrier([0]), barrier([2]).
+
+        Note: reset only support for simulator `qfvm_circ`.
+        """
+        if qlist is None:
+            qlist = list(range(self.num))
+        self.add_ins(Reset(qlist))
+        self.executable_on_backend = False
+        return self
+
+    def measure(self, pos: List[int] = None, cbits: List[int] = None) -> None:
+        """
+        Measurement setting for experiment device.
+
+        Args:
+            pos: Qubits need measure.
+            cbits: Classical bits keeping the measure results.
+        """
+        # checking
+        if pos is None:
+            pos = list(range(self.num))
+        if np.any(np.array(pos) >= self.num):
+            raise ValueError("Index out of range.")
+
+        e_num = len(self.measures)  # existing num of measures
+        n_num = len(pos)  # newly added num of measures
+        if n_num > len(set(pos)):
+            raise ValueError("Measured qubits not uniquely assigned.")
+
+        if cbits:
+            if not len(set(cbits)) == len(cbits):
+                raise ValueError("Classical bits not uniquely assigned.")
+            if not len(cbits) == n_num:
+                raise ValueError(
+                    "Number of measured bits should equal to the number of classical bits"
+                )
+        else:
+            cbits = list(range(e_num, e_num + n_num))
+
+        for cbit in cbits:
+            if cbit < 0 or cbit > self.cbits_num:
+                raise ValueError("Cbits index out of range.")
+        # _sorted_indices = sorted(range(n_num), key=lambda k: cbits[k])
+        # cbits = [_sorted_indices.index(i) + e_num for i in range(n_num)]
+
+        measure = Measure(dict(zip(pos, cbits)))
+        self._measures.append(measure)
+        self.add_ins(measure)
+
+    @contextmanager
+    def cif(self, cbits: List[int], condition: int):
+        """
+        Create an `if` statement on this circuit.
+        If cbits equals to condition, the subsequent operaterations will be performed.
+        Use  the `measure` statement to explicitly assign value to the cbit before using it as `cbits` argument
+
+        Args:
+            cbits: List of cbit that are used for comparison.
+            condition(int): A condition to be evaluated with cbits that filled by `measure` operation.
+
+
+        For example::
+            from quafu import QuantumCircuit
+            qc = QuantumCircuit(2,2)
+
+            qc.h(0)
+            qc.cx(0,1)
+            qc.measure([0],[0])
+            with qc.cif(cbits=[0], condition=1):
+                qc.x(2)
+            qc.measure([2],[2])
+
+        Note: cif only support for simulator `qfvm_circ`.
+        """
+        # check cbits
+        if not len(set(cbits)) == len(cbits):
+            raise ValueError("Classical bits not uniquely assigned.")
+        if max(cbits) > self.cbits_num - 1 or min(cbits) < 0:
+            raise ValueError("Classical bits index out of range.")
+        # check condition
+        if condition < 0:
+            raise ValueError("Classical should be a positive integer.")
+        self.executable_on_backend = False
+        cif_ins = Cif(cbits=cbits, condition=condition)
+        self.add_ins(cif_ins)
+
+        yield
+
+        instructions = []
+        for i in range(len(self.instructions) - 1, -1, -1):
+            if (
+                isinstance(self.instructions[i], Cif)
+                and self.instructions[i].instructions is None
+            ):
+                instructions.reverse()
+                self.instructions[i].set_ins(instructions)
+                self.instructions = self.instructions[0 : i + 1]
+                return
+            else:
+                instructions.append(self.instructions[i])
```

## quafu/dagcircuits/__init__.py

```diff
@@ -1 +0,0 @@
-00000000: 0d0a                                     ..
```

## quafu/dagcircuits/circuit_dag.py

```diff
@@ -1,472 +1,449 @@
-from quafu import QuantumCircuit
-
-from quafu.elements.element_gates import * 
-from quafu.elements import Barrier, Delay, Measure, XYResonance
-from quafu.elements.pulses import GaussianPulse, RectPulse, FlattopPulse
-
-import networkx as nx
-from typing import Any, List
-import copy
-
-from quafu.dagcircuits.instruction_node import InstructionNode  # instruction_node.py in the same folder as circuit_dag.py now
-from quafu.dagcircuits.dag_circuit import DAGCircuit  #  dag_circuit.py in the same folder as circuit_dag.py now
-
-# import pygraphviz as pgv
-from networkx.drawing.nx_pydot import write_dot
-from IPython.display import Image, SVG
-
-
-
-# transform a gate in quantumcircuit of quafu(not include measure_gate),
-# into a node in the graph, with specific label.
-def gate_to_node(input_gate,specific_label: str):
-    ''' 
-    transform a gate in quantumcircuit of quafu(not include measure_gate),
-    into a node in the graph, with specific label.
-
-    Args:
-        inputgate: a gate in quantumcircuit of quafu(not include measure_gate)
-        label: the label of the node in the graph
-
-    Returns:
-        node: a node in the graph, with specific label. A GateWrapper object
-    
-    '''
-
-    import copy
-    gate = copy.deepcopy(input_gate) # avoid modifying the original gate
-    if not isinstance(gate.pos, list):  # if gate.pos is not a list, make it a list
-        gate.pos = [gate.pos]
-
-    # use getattr check 'paras' and other attributes if exist. if the attr doesn't exist,return None
-    gate.paras = getattr(gate, 'paras', None) or None
-    gate.duration = getattr(gate, 'duration', None) or None
-    gate.unit = getattr(gate, 'unit', None) or None 
-    gate.channel = getattr(gate, 'channel', None) or None
-    gate.time_func = getattr(gate, 'time_func', None) or None
-
-    if gate.paras and not isinstance(gate.paras, list):  # if paras is True and not a list, make it a list
-        gate.paras = [gate.paras]
-    
-    # hashable_gate = InstructionNode(gate.name, gate.pos, gate.paras,gate.matrix,gate.duration,gate.unit, label=i)
-    hashable_gate = InstructionNode(gate.name, gate.pos, gate.paras,gate.duration, gate.unit,gate.channel,gate.time_func, label=specific_label)
-    return hashable_gate
-
-# Building a DAG Graph using DAGCircuit from a QuantumCircuit
-def circuit_to_dag(circuit, measure_flag = True):
-    '''
-    Building a DAG Graph using DAGCircui from a QuantumCircuit
-    
-    Args:
-        circuit: a QuantumCircuit object
-        measure_flag: whether to add measure_gate node to the dag graph
-        
-    Returns:
-        g: a DAGCircuit object
-        
-    example:
-        .. jupyter-execute::
-        
-            from circuit_dag import circuit_to_dag, dag_to_circuit, draw_dag
-            from quafu import QuantumCircuit
-
-            # Create a quantum circuit as an example that you can modify as needed
-            circuit = QuantumCircuit(2)
-            circuit.h(0)
-            circuit.cnot(0, 1)
-
-            # Build the dag graph
-            dep_graph = circuit_to_dag(circuit)  #  dag graph     
-    '''
-    
-    # Starting Label Index
-    i = 0
-    
-    # A dictionary to store the last use of any qubit
-    qubit_last_use = {}
-    
-    # g = nx.MultiDiGraph()  # two nodes can have multiple edges
-    # g = nx.DiGraph()   # two nodes can only have one edge
-    g = DAGCircuit()   # two nodes can only have one edge
-    
-    # Add the start node 
-    # g.add_node(-1,{"color": "green"})
-    g.add_nodes_from([(-1, {"color": "green"})])
-    
-    # deepcopy the circuit to avoid modifying the original circuit
-    # gates = copy.deepcopy(circuit.gates) # need to import copy
-    # change to: gate = copy.deepcopy(input_gate) in gate_to_node()
-
-    for gate in circuit.gates:
-        # transform gate to node
-        hashable_gate = gate_to_node(gate,specific_label=i)
-        i += 1
-        
-        g.add_node(hashable_gate,color="blue")
-        
-        # Add edges based on qubit_last_use; update last use
-        for qubit in hashable_gate.pos:
-            if qubit in qubit_last_use:
-                g.add_edge(qubit_last_use[qubit], hashable_gate,label=f'q{qubit}')
-            else:
-                g.add_edge(-1, hashable_gate,label=f'q{qubit}',color="green")
-            
-            qubit_last_use[qubit] = hashable_gate
-
-    if measure_flag:  
-        # Add measure_gate node
-        qm = Any
-        qm.name = "measure"  
-        qm.paras, qm.duration, qm.unit = [None,None,None]
-        qm.channel, qm.time_func = [None,None]
-        qm.pos = copy.deepcopy(circuit.measures)  # circuit.measures is a dict
-        measure_gate = InstructionNode(qm.name, qm.pos, qm.paras, qm.duration, qm.unit, qm.channel, qm.time_func, label="m")
-        g.add_node(measure_gate,color="blue")
-        # Add edges from qubit_last_use[qubit] to measure_gate
-        for qubit in measure_gate.pos:
-            if qubit in qubit_last_use:
-                g.add_edge(qubit_last_use[qubit], measure_gate,label=f'q{qubit}')
-            else:
-                g.add_edge(-1, measure_gate,label=f'q{qubit}',color="green")
-
-            qubit_last_use[qubit] = measure_gate
-            
-    # Add the end node
-    # g.add_node(float('inf'),{"color": "red"})
-    g.add_nodes_from([(float('inf'), {"color": "red"})])
-    
-    for qubit in qubit_last_use:
-        g.add_edge(qubit_last_use[qubit], float('inf'),label=f'q{qubit}',color="red")
-    
-    # update  qubits_used, cbits_used, num_instruction_nodes
-    g.update_qubits_used()
-    g.update_cbits_used()
-    g.update_num_instruction_nodes()
-
-    return g
-
-
-# transform gate in dag nodes  to gate in circuit which can be added to circuit
-gate_classes = {
-    "x": XGate,
-    "y": YGate,
-    "z": ZGate,
-    "h": HGate,
-    "s": SGate,
-    "sdg": SdgGate,
-    "t": TGate,
-    "tdg": TdgGate,
-    "rx": RXGate,
-    "ry": RYGate,
-    "rz": RZGate,
-    "id": IdGate,
-    "sx": SXGate,
-    "sy": SYGate,
-    "w": WGate,
-    "sw": SWGate,
-    "p": PhaseGate,
-    "delay": Delay,
-    "barrier": Barrier,
-    "cx": CXGate,
-    "cnot": CXGate,
-    "cp": CPGate,
-    "swap": SwapGate,
-    "rxx": RXXGate,
-    "ryy": RYYGate,
-    "rzz": RZZGate,
-    "cy": CYGate,
-    "cz": CZGate,
-    "cs": CSGate,
-    "ct": CTGate,
-    "xy": XYResonance,
-    "ccx": ToffoliGate,
-    "toffoli": ToffoliGate,
-    "cswap": FredkinGate,
-    "fredkin": FredkinGate,
-    "mcx": MCXGate,
-    "mcy": MCYGate,
-    "mcz": MCZGate,
-    "gaussian": GaussianPulse,
-    "rect"    : RectPulse,
-    "flattop" : FlattopPulse,
-    "measure" : Measure
-}
-
-def node_to_gate(gate_in_dag):
-    """
-    transform gate in dag graph, to gate in circuit which can be added to circuit
-
-    Args:
-        gate_in_dag: a node in dag graph , gate_in_dag is a GateWrapper object. 
-            in instruction_node, gate_in_dag.name is uppercase, gate_in_dag.pos is a list or a dict
-            gate_transform support gate with one qubit or more qubits, not measures!
-            and you should exculde nodes [-1 ,float('inf') , measure_gate] in dag graph
-
-    Returns:
-        gate: gate  which can be added to circuit in quafu
-
-    example:
-            import networkx as nx
-            from quafu import QuantumCircuit
-            qcircuit = QuantumCircuit(n)
-
-            for gate in nx.topological_sort(dep_graph):
-            
-                if gate not in [-1, float('inf')]:
-                    # measure gate to do
-                    if gate.name == "measure":
-                        qcircuit.measures = gate.pos
-
-                    else:
-                        # use gate_transform to transform gate in dag graph to gate in circuit
-                        qcircuit.gates.append(node_to_gate(gate))
-            return qcircuit
-    
-    """
-
-    gate_name = gate_in_dag.name.lower()
-    gate_class = gate_classes.get(gate_name)
-
-    if not gate_class:
-        raise ValueError("gate is not supported")
-
-    if gate_name == "barrier":
-        return gate_class(gate_in_dag.pos)
-
-    # 从gate_in_dag获取参数列表
-    args = gate_in_dag.pos
-    if gate_in_dag.paras:
-        args += gate_in_dag.paras
-
-    # 处理 gate.duration 和 gate.unit
-    if gate_name in ["delay", "xy"]:
-        args.append(gate_in_dag.duration)
-        args.append(gate_in_dag.unit)
-
-    # 处理多量子比特门
-    if gate_name in ["mcx", "mcy", "mcz"]:
-        control_qubits = gate_in_dag.pos[:-1]
-        target_qubit = gate_in_dag.pos[-1]
-        return gate_class(control_qubits, target_qubit)
-
-    # pulse node
-    if gate_name in ["gaussian", "rect", "flattop"]:
-        duration = gate_in_dag.duration
-        unit = gate_in_dag.unit
-        paras = gate_in_dag.paras
-        pos = gate_in_dag.pos[0]
-        channel = gate_in_dag.channel
-        # time_func = gate_in_dag.time_func
-
-        return gate_class(pos, *paras, duration, unit, channel)
-    
-    # measure node
-    if gate_name == "measure":
-        return gate_class(gate_in_dag.pos)
-    
-    return gate_class(*args)
-
-
-
-# From DAG with Hashable Gates to quafu Gates added to circuit                  
-def dag_to_circuit(dep_graph, n: int):
-    '''
-    From DAG with Hashable Gates to quafu Gates added to circuit
-    
-    Args:
-        dep_graph (DAG): DAG with Hashable Gates
-        n (int): number of qubits
-    
-    Returns:
-        qcircuit (QuantumCircuit): quafu QuantumCircuit
-        
-    example:
-        .. jupyter-execute::
-
-            from circuit_dag import circuit_to_dag, dag_to_circuit, draw_dag
-            from quafu import QuantumCircuit
-
-            # Create a quantum circuit as an example that you can modify as needed
-            circuit = QuantumCircuit(2)
-            circuit.h(0)
-            circuit.cnot(0, 1)
-
-            # Build the dag graph
-            dep_graph = circuit_to_dag(circuit)  #  dag graph  
-            
-            # use dag_to_circuit to transform dag graph to a new circuit
-            reconstructed_circuit = dag_to_circuit(dep_graph, circuit.num)
-        
-     
-    '''
-    
-    qcircuit = QuantumCircuit(n)
-
-    for gate in nx.topological_sort(dep_graph):
-    
-        if gate not in [-1, float('inf')]:
-            # measure gate to do
-            if gate.name == "measure":
-                qcircuit.measures = gate.pos
-
-            else:
-                # use gate_transform to transform gate in dag graph to gate in circuit
-                qcircuit.gates.append(node_to_gate(gate))
-    return qcircuit
-
-# Helper function to visualize the DAG,check the example in the docstring
-def draw_dag(dep_g, output_format="png"):
-    '''
-    Helper function to visualize the DAG
-
-    Args:
-        dep_g (DAG): DAG with Hashable Gates
-        output_format (str): output format, "png" or "svg"
-
-    Returns:
-        img (Image or SVG): show the image of DAG, which is Image(filename="dag.png") or SVG(filename="dag.svg")
-
-    example:
-        .. jupyter-execute::
-        ex1:
-            # directly draw  PNG picture
-            draw_dag(dep_g, output_format="png")    # save a png picture "dag.png" and show it in jupyter notebook
-
-            # directly draw  SVG   picture
-            draw_dag(dep_g, output_format="svg")    # save a svg picture "dag.svg" and show it in jupyter notebook
-       
-        ex2:
-            # generate   PNG  picture
-            img_png = draw_dag(dep_g, output_format="png") 
-
-            # generate   SVG  picture
-            img_svg = draw_dag(dep_g, output_format="svg") 
-            
-            # show PNG picture
-            img_png
-            
-            # show SVG picture
-            img_svg        
-
-            
-    '''
-    import pygraphviz 
-    write_dot(dep_g, "dag.dot")
-    G = pygraphviz.AGraph("dag.dot")
-    G.layout(prog="dot")
-
-    if output_format == "png":
-        G.draw("dag.png")
-        return Image(filename="dag.png")
-    elif output_format == "svg":
-        G.draw("dag.svg")
-        return SVG(filename="dag.svg")
-    else:
-        raise ValueError("Unsupported output format: choose either 'png' or 'svg'")
-
-
-def nodelist_to_dag(op_nodes: List[Any]) -> DAGCircuit:
-    # Starting Label Index
-    i = 0
-    
-    # A dictionary to store the last use of any qubit
-    qubit_last_use = {}
-    
-    # g = nx.MultiDiGraph()  # two nodes can have multiple edges
-    # g = nx.DiGraph()   # two nodes can only have one edge
-    g = DAGCircuit() 
-    
-    # Add the start node 
-    # g.add_node(-1,{"color": "green"})
-    g.add_nodes_from([(-1, {"color": "green"})])
-    
-    # deepcopy the circuit to avoid modifying the original circuit
-    # gates = copy.deepcopy(circuit.gates) # need to import copy
-    # change to: gate = copy.deepcopy(input_gate) in gate_to_node()
-
-    for op_node in op_nodes:
-        # transform gate to node
-        hashable_gate = copy.deepcopy(op_node)
-        g.add_node(hashable_gate,color="blue")
-        
-        # Add edges based on qubit_last_use; update last use
-        for qubit in hashable_gate.pos:
-            if qubit in qubit_last_use:
-                g.add_edge(qubit_last_use[qubit], hashable_gate,label=f'q{qubit}')
-            else:
-                g.add_edge(-1, hashable_gate,label=f'q{qubit}',color="green")
-            
-            qubit_last_use[qubit] = hashable_gate
-
-            
-    # Add the end node
-    # g.add_node(float('inf'),{"color": "red"})
-    g.add_nodes_from([(float('inf'), {"color": "red"})])
-    
-    for qubit in qubit_last_use:
-        g.add_edge(qubit_last_use[qubit], float('inf'),label=f'q{qubit}',color="red")
-
-    # update the  qubits_used, cbits_used, num_instruction_nodes
-    g.qubits_used = g.update_qubits_used()
-    g.cbits_used = g.update_cbits_used()
-    g.num_instruction_nodes = g.update_num_instruction_nodes()
-    
-    return g
-
-# nodes_qubit_mapping_dict 
-def nodelist_qubit_mapping_dict(nodes_list):
-    '''
-    Args:
-        nodes_list: a list of nodes
-    Returns:
-        nodes_qubit_mapping_dict: a dict about keys are the qubits used by the nodes and values are the new qubits
-    '''
-    nodes_list_qubits_used = set()
-    for node in nodes_list:
-        if hasattr(node, 'pos') and node.pos is not None:
-            nodes_list_qubits_used = nodes_list_qubits_used | set(node.pos)
-    
-    mapping_pos = list(range(len(nodes_list_qubits_used)))  
-    # mapping, get a dict
-    nodes_qubit_mapping_dict = dict(zip(sorted(list(nodes_list_qubits_used)), mapping_pos))
-    nodes_qubit_mapping_dict
-
-    return nodes_qubit_mapping_dict
-
-def nodelist_qubit_mapping_dict_reverse(nodes_list):
-    '''
-    Args:
-        nodes_list: a list of nodes
-    Returns:
-        nodes_qubit_mapping_dict_reverse: a dict about keys are the new qubits and values are the qubits used by the nodes
-    ''' 
-    nodes_qubit_mapping_dict = nodelist_qubit_mapping_dict(nodes_list)
-    # reverse mapping, get a dict
-    nodes_qubit_mapping_dict_reverse = {value: key for key, value in nodes_qubit_mapping_dict.items()}
-     
-    return nodes_qubit_mapping_dict_reverse
-
-# a function to map nodes_list
-def nodes_list_mapping(nodes_list, nodes_qubit_mapping_dict):
-    '''
-    Args:
-        nodes_list: the nodes list of instruction nodes
-        nodes_qubit_mapping_dict: the dict of the mapping qubits
-
-    return: 
-        nodes_list_mapping: the nodes_list after mapping qubits
-    '''
-    nodes_qubit_mapping_dict 
-    nodes_list_mapping = []
-    for node in nodes_list:
-        node_new = copy.deepcopy(node)
-        if hasattr(node, 'pos') and node.pos is not None:
-            if isinstance(node.pos, list):
-                node_new.pos = [nodes_qubit_mapping_dict[qubit] for qubit in node.pos]
-            elif isinstance(node.pos, dict):
-                node_new.pos = {}
-                # the values of the dict are void, so we need to copy the values from the original dict
-                for qubit in node.pos:
-                    node_new.pos[nodes_qubit_mapping_dict[qubit]] = copy.deepcopy(node.pos[qubit])
-        nodes_list_mapping.append(node_new)
-    return nodes_list_mapping
+import copy
+from typing import Any, List
+
+import networkx as nx
+from quafu.dagcircuits.dag_circuit import (  # dag_circuit.py in the same folder as circuit_dag.py now
+    DAGCircuit,
+)
+from quafu.dagcircuits.instruction_node import (  # instruction_node.py in the same folder as circuit_dag.py now
+    InstructionNode,
+)
+from quafu.elements import Barrier, Delay, Measure, XYResonance
+from quafu.elements.element_gates import *
+from quafu.elements.pulses import FlattopPulse, GaussianPulse, RectPulse
+
+from quafu import QuantumCircuit
+
+
+# transform a gate in quantumcircuit of quafu(not include measure_gate),
+# into a node in the graph, with specific label.
+def gate_to_node(input_gate, specific_label: str):
+    """
+    transform a gate in quantumcircuit of quafu(not include measure_gate),
+    into a node in the graph, with specific label.
+
+    Args:
+        inputgate: a gate in quantumcircuit of quafu(not include measure_gate)
+        label: the label of the node in the graph
+
+    Returns:
+        node: a node in the graph, with specific label. A GateWrapper object
+
+    """
+
+    import copy
+
+    gate = copy.deepcopy(input_gate)  # avoid modifying the original gate
+    if not isinstance(gate.pos, list):  # if gate.pos is not a list, make it a list
+        gate.pos = [gate.pos]
+
+    # use getattr check 'paras' and other attributes if exist. if the attr doesn't exist,return None
+    gate.paras = getattr(gate, "paras", None) or None
+    gate.duration = getattr(gate, "duration", None) or None
+    gate.unit = getattr(gate, "unit", None) or None
+    gate.channel = getattr(gate, "channel", None) or None
+    gate.time_func = getattr(gate, "time_func", None) or None
+
+    if gate.paras and not isinstance(
+        gate.paras, list
+    ):  # if paras is True and not a list, make it a list
+        gate.paras = [gate.paras]
+
+    # hashable_gate = InstructionNode(gate.name, gate.pos, gate.paras,gate.matrix,gate.duration,gate.unit, label=i)
+    hashable_gate = InstructionNode(
+        gate.name,
+        gate.pos,
+        gate.paras,
+        gate.duration,
+        gate.unit,
+        gate.channel,
+        gate.time_func,
+        label=specific_label,
+    )
+    return hashable_gate
+
+
+# Building a DAG Graph using DAGCircuit from a QuantumCircuit
+def circuit_to_dag(circuit, measure_flag=True):
+    """
+    Building a DAG Graph using DAGCircui from a QuantumCircuit
+
+    Args:
+        circuit: a QuantumCircuit object
+        measure_flag: whether to add measure_gate node to the dag graph
+
+    Returns:
+        g: a DAGCircuit object
+
+    example:
+        .. jupyter-execute::
+
+            from circuit_dag import circuit_to_dag, dag_to_circuit, draw_dag
+            from quafu import QuantumCircuit
+
+            # Create a quantum circuit as an example that you can modify as needed
+            circuit = QuantumCircuit(2)
+            circuit.h(0)
+            circuit.cnot(0, 1)
+
+            # Build the dag graph
+            dep_graph = circuit_to_dag(circuit)  #  dag graph
+    """
+
+    # Starting Label Index
+    i = 0
+
+    # A dictionary to store the last use of any qubit
+    qubit_last_use = {}
+
+    # g = nx.MultiDiGraph()  # two nodes can have multiple edges
+    # g = nx.DiGraph()   # two nodes can only have one edge
+    g = DAGCircuit()  # two nodes can only have one edge
+
+    # Add the start node
+    # g.add_node(-1,{"color": "green"})
+    g.add_nodes_from([(-1, {"color": "green"})])
+
+    # deepcopy the circuit to avoid modifying the original circuit
+    # gates = copy.deepcopy(circuit.gates) # need to import copy
+    # change to: gate = copy.deepcopy(input_gate) in gate_to_node()
+
+    for gate in circuit.gates:
+        # transform gate to node
+        hashable_gate = gate_to_node(gate, specific_label=i)
+        i += 1
+
+        g.add_node(hashable_gate, color="blue")
+
+        # Add edges based on qubit_last_use; update last use
+        for qubit in hashable_gate.pos:
+            if qubit in qubit_last_use:
+                g.add_edge(qubit_last_use[qubit], hashable_gate, label=f"q{qubit}")
+            else:
+                g.add_edge(-1, hashable_gate, label=f"q{qubit}", color="green")
+
+            qubit_last_use[qubit] = hashable_gate
+
+    if measure_flag:
+        # Add measure_gate node
+        qm = Any
+        qm.name = "measure"
+        qm.paras, qm.duration, qm.unit = [None, None, None]
+        qm.channel, qm.time_func = [None, None]
+        qm.pos = copy.deepcopy(circuit.measures)  # circuit.measures is a dict
+        measure_gate = InstructionNode(
+            qm.name,
+            qm.pos,
+            qm.paras,
+            qm.duration,
+            qm.unit,
+            qm.channel,
+            qm.time_func,
+            label="m",
+        )
+        g.add_node(measure_gate, color="blue")
+        # Add edges from qubit_last_use[qubit] to measure_gate
+        for qubit in measure_gate.pos:
+            if qubit in qubit_last_use:
+                g.add_edge(qubit_last_use[qubit], measure_gate, label=f"q{qubit}")
+            else:
+                g.add_edge(-1, measure_gate, label=f"q{qubit}", color="green")
+
+            qubit_last_use[qubit] = measure_gate
+
+    # Add the end node
+    # g.add_node(float('inf'),{"color": "red"})
+    g.add_nodes_from([(float("inf"), {"color": "red"})])
+
+    for qubit in qubit_last_use:
+        g.add_edge(qubit_last_use[qubit], float("inf"), label=f"q{qubit}", color="red")
+
+    # update  qubits_used, cbits_used, num_instruction_nodes
+    g.update_qubits_used()
+    g.update_cbits_used()
+    g.update_num_instruction_nodes()
+
+    return g
+
+
+# transform gate in dag nodes  to gate in circuit which can be added to circuit
+gate_classes = {
+    "x": XGate,
+    "y": YGate,
+    "z": ZGate,
+    "h": HGate,
+    "s": SGate,
+    "sdg": SdgGate,
+    "t": TGate,
+    "tdg": TdgGate,
+    "rx": RXGate,
+    "ry": RYGate,
+    "rz": RZGate,
+    "id": IdGate,
+    "sx": SXGate,
+    "sy": SYGate,
+    "w": WGate,
+    "sw": SWGate,
+    "p": PhaseGate,
+    "delay": Delay,
+    "barrier": Barrier,
+    "cx": CXGate,
+    "cnot": CXGate,
+    "cp": CPGate,
+    "swap": SwapGate,
+    "rxx": RXXGate,
+    "ryy": RYYGate,
+    "rzz": RZZGate,
+    "cy": CYGate,
+    "cz": CZGate,
+    "cs": CSGate,
+    "ct": CTGate,
+    "xy": XYResonance,
+    "ccx": ToffoliGate,
+    "toffoli": ToffoliGate,
+    "cswap": FredkinGate,
+    "fredkin": FredkinGate,
+    "mcx": MCXGate,
+    "mcy": MCYGate,
+    "mcz": MCZGate,
+    "gaussian": GaussianPulse,
+    "rect": RectPulse,
+    "flattop": FlattopPulse,
+    "measure": Measure,
+}
+
+
+def node_to_gate(gate_in_dag):
+    """
+    transform gate in dag graph, to gate in circuit which can be added to circuit
+
+    Args:
+        gate_in_dag: a node in dag graph , gate_in_dag is a GateWrapper object.
+            in instruction_node, gate_in_dag.name is uppercase, gate_in_dag.pos is a list or a dict
+            gate_transform support gate with one qubit or more qubits, not measures!
+            and you should exculde nodes [-1 ,float('inf') , measure_gate] in dag graph
+
+    Returns:
+        gate: gate  which can be added to circuit in quafu
+
+    example:
+            import networkx as nx
+            from quafu import QuantumCircuit
+            qcircuit = QuantumCircuit(n)
+
+            for gate in nx.topological_sort(dep_graph):
+
+                if gate not in [-1, float('inf')]:
+                    # measure gate to do
+                    if gate.name == "measure":
+                        qcircuit.measures = gate.pos
+
+                    else:
+                        # use gate_transform to transform gate in dag graph to gate in circuit
+                        qcircuit.gates.append(node_to_gate(gate))
+            return qcircuit
+
+    """
+
+    gate_name = gate_in_dag.name.lower()
+    gate_class = gate_classes.get(gate_name)
+
+    if not gate_class:
+        raise ValueError("gate is not supported")
+
+    if gate_name == "barrier":
+        return gate_class(gate_in_dag.pos)
+
+    # 从gate_in_dag获取参数列表
+    args = gate_in_dag.pos
+    if gate_in_dag.paras:
+        args += gate_in_dag.paras
+
+    # 处理 gate.duration 和 gate.unit
+    if gate_name in ["delay", "xy"]:
+        args.append(gate_in_dag.duration)
+        args.append(gate_in_dag.unit)
+
+    # 处理多量子比特门
+    if gate_name in ["mcx", "mcy", "mcz"]:
+        control_qubits = gate_in_dag.pos[:-1]
+        target_qubit = gate_in_dag.pos[-1]
+        return gate_class(control_qubits, target_qubit)
+
+    # pulse node
+    if gate_name in ["gaussian", "rect", "flattop"]:
+        duration = gate_in_dag.duration
+        unit = gate_in_dag.unit
+        paras = gate_in_dag.paras
+        pos = gate_in_dag.pos[0]
+        channel = gate_in_dag.channel
+        # time_func = gate_in_dag.time_func
+
+        return gate_class(pos, *paras, duration, unit, channel)
+
+    # measure node
+    if gate_name == "measure":
+        return gate_class(gate_in_dag.pos)
+
+    return gate_class(*args)
+
+
+# From DAG with Hashable Gates to quafu Gates added to circuit
+def dag_to_circuit(dep_graph, n: int):
+    """
+    From DAG with Hashable Gates to quafu Gates added to circuit
+
+    Args:
+        dep_graph (DAG): DAG with Hashable Gates
+        n (int): number of qubits
+
+    Returns:
+        qcircuit (QuantumCircuit): quafu QuantumCircuit
+
+    example:
+        .. jupyter-execute::
+
+            from circuit_dag import circuit_to_dag, dag_to_circuit, draw_dag
+            from quafu import QuantumCircuit
+
+            # Create a quantum circuit as an example that you can modify as needed
+            circuit = QuantumCircuit(2)
+            circuit.h(0)
+            circuit.cnot(0, 1)
+
+            # Build the dag graph
+            dep_graph = circuit_to_dag(circuit)  #  dag graph
+
+            # use dag_to_circuit to transform dag graph to a new circuit
+            reconstructed_circuit = dag_to_circuit(dep_graph, circuit.num)
+
+
+    """
+
+    qcircuit = QuantumCircuit(n)
+
+    for gate in nx.topological_sort(dep_graph):
+        if gate not in [-1, float("inf")]:
+            # measure gate to do
+            if gate.name == "measure":
+                qcircuit.measures = gate.pos
+
+            else:
+                # use gate_transform to transform gate in dag graph to gate in circuit
+                qcircuit.gates.append(node_to_gate(gate))
+    return qcircuit
+
+
+def nodelist_to_dag(op_nodes: List[Any]) -> DAGCircuit:
+    # Starting Label Index
+    i = 0
+
+    # A dictionary to store the last use of any qubit
+    qubit_last_use = {}
+
+    # g = nx.MultiDiGraph()  # two nodes can have multiple edges
+    # g = nx.DiGraph()   # two nodes can only have one edge
+    g = DAGCircuit()
+
+    # Add the start node
+    # g.add_node(-1,{"color": "green"})
+    g.add_nodes_from([(-1, {"color": "green"})])
+
+    # deepcopy the circuit to avoid modifying the original circuit
+    # gates = copy.deepcopy(circuit.gates) # need to import copy
+    # change to: gate = copy.deepcopy(input_gate) in gate_to_node()
+
+    for op_node in op_nodes:
+        # transform gate to node
+        hashable_gate = copy.deepcopy(op_node)
+        g.add_node(hashable_gate, color="blue")
+
+        # Add edges based on qubit_last_use; update last use
+        for qubit in hashable_gate.pos:
+            if qubit in qubit_last_use:
+                g.add_edge(qubit_last_use[qubit], hashable_gate, label=f"q{qubit}")
+            else:
+                g.add_edge(-1, hashable_gate, label=f"q{qubit}", color="green")
+
+            qubit_last_use[qubit] = hashable_gate
+
+    # Add the end node
+    # g.add_node(float('inf'),{"color": "red"})
+    g.add_nodes_from([(float("inf"), {"color": "red"})])
+
+    for qubit in qubit_last_use:
+        g.add_edge(qubit_last_use[qubit], float("inf"), label=f"q{qubit}", color="red")
+
+    # update the  qubits_used, cbits_used, num_instruction_nodes
+    g.qubits_used = g.update_qubits_used()
+    g.cbits_used = g.update_cbits_used()
+    g.num_instruction_nodes = g.update_num_instruction_nodes()
+
+    return g
+
+
+# nodes_qubit_mapping_dict
+def nodelist_qubit_mapping_dict(nodes_list):
+    """
+    Args:
+        nodes_list: a list of nodes
+    Returns:
+        nodes_qubit_mapping_dict: a dict about keys are the qubits used by the nodes and values are the new qubits
+    """
+    nodes_list_qubits_used = set()
+    for node in nodes_list:
+        if hasattr(node, "pos") and node.pos is not None:
+            nodes_list_qubits_used = nodes_list_qubits_used | set(node.pos)
+
+    mapping_pos = list(range(len(nodes_list_qubits_used)))
+    # mapping, get a dict
+    nodes_qubit_mapping_dict = dict(
+        zip(sorted(list(nodes_list_qubits_used)), mapping_pos)
+    )
+    nodes_qubit_mapping_dict
+
+    return nodes_qubit_mapping_dict
+
+
+def nodelist_qubit_mapping_dict_reverse(nodes_list):
+    """
+    Args:
+        nodes_list: a list of nodes
+    Returns:
+        nodes_qubit_mapping_dict_reverse: a dict about keys are the new qubits and values are the qubits used by the nodes
+    """
+    nodes_qubit_mapping_dict = nodelist_qubit_mapping_dict(nodes_list)
+    # reverse mapping, get a dict
+    nodes_qubit_mapping_dict_reverse = {
+        value: key for key, value in nodes_qubit_mapping_dict.items()
+    }
+
+    return nodes_qubit_mapping_dict_reverse
+
+
+# a function to map nodes_list
+def nodes_list_mapping(nodes_list, nodes_qubit_mapping_dict):
+    """
+    Args:
+        nodes_list: the nodes list of instruction nodes
+        nodes_qubit_mapping_dict: the dict of the mapping qubits
+
+    return:
+        nodes_list_mapping: the nodes_list after mapping qubits
+    """
+    nodes_qubit_mapping_dict
+    nodes_list_mapping = []
+    for node in nodes_list:
+        node_new = copy.deepcopy(node)
+        if hasattr(node, "pos") and node.pos is not None:
+            if isinstance(node.pos, list):
+                node_new.pos = [nodes_qubit_mapping_dict[qubit] for qubit in node.pos]
+            elif isinstance(node.pos, dict):
+                node_new.pos = {}
+                # the values of the dict are void, so we need to copy the values from the original dict
+                for qubit in node.pos:
+                    node_new.pos[nodes_qubit_mapping_dict[qubit]] = copy.deepcopy(
+                        node.pos[qubit]
+                    )
+        nodes_list_mapping.append(node_new)
+    return nodes_list_mapping
```

## quafu/dagcircuits/dag_circuit.py

```diff
@@ -1,286 +1,331 @@
-import networkx as nx
-from typing import Dict, Any, List
-
-from quafu.dagcircuits.instruction_node import InstructionNode
-
-from networkx.classes.multidigraph import MultiDiGraph
-
-class DAGCircuit(MultiDiGraph):
-    def __init__(self,qubits_used=None, cbits_used=None, incoming_graph_data=None, **attr):
-        super().__init__(incoming_graph_data, **attr)
-              
-        if qubits_used is None:
-            self.qubits_used = set()
-        elif isinstance(qubits_used, set):
-            self.qubits_used = qubits_used
-        else:
-            raise ValueError('qubits_used should be a set or None')
-
-        if cbits_used is None:
-            self.cbits_used = set()
-        elif isinstance(cbits_used, set):
-            self.cbits_used = cbits_used
-        else:
-            raise ValueError('cbits_used should be a set or None')
-        
-        # num of instruction nodes
-        self.num_instruction_nodes = 0
-
-
-    # add new methods or override existing methods here.
-
-    def update_qubits_used(self):
-        '''
-        qubits_used is a set of qubits used in DAGCircuit
-        based on node -1's edges' labels, the qubits is the integer part of the label
-
-        return:
-            qubits_used: set of qubits used in DAGCircuit
-        '''
-        if -1 not in self.nodes:
-            raise ValueError('-1 should be in DAGCircuit, please add it first')
-        self.qubits_used = set([int(edge[2]['label'][1:]) for edge in self.out_edges(-1, data=True)])
-        return self.qubits_used
-    
-    def update_cbits_used(self):
-        '''
-        cbits_used is a set of cbits used in DAGCircuit
-        calculated by  measurenode's cbits        
-        return:
-            cbits_used: set of cbits used in DAGCircuit
-        '''
-        for node in self.nodes:
-        # if node.has a attribute 'name' and node.name == 'measure'
-            if hasattr(node, 'name') and node.name == 'measure':
-                self.cbits_used = set(node.pos.values())   
-        return self.cbits_used
-    
-    def update_num_instruction_nodes(self):
-        '''
-        num_instruction_nodes is the number of instruction nodes in DAGCircuit
-        '''
-        if -1 not in self.nodes:
-            raise ValueError('-1 should be in DAGCircuit, please add it first')
-        if float('inf') not in self.nodes:
-            raise ValueError('float("inf") should be in DAGCircuit, please add it first')
-        self.num_instruction_nodes = len(self.nodes) - 2
-
-        for node in self.nodes:
-            if hasattr(node, 'name') and node.name == 'measure':
-                self.num_instruction_nodes -= 1
-        return self.num_instruction_nodes
-
-    
-
-    def nodes_dict(self):
-        '''
-        nodes_dict is a dictionary of nodes with the node label as key and the node as value.
-        without  -1 and float('inf')
-        '''
-        nodes_dict = {}
-        for node in nx.topological_sort(self):
-            if node != -1 and node != float('inf'):
-                nodes_dict[node.label] = node
-        return nodes_dict
-     
-
-    def nodes_list(self):
-        ''' 
-        nodes_list is a list of nodes without  -1 and float('inf')
-        ''' 
-        nodes_list = []
-        for node in nx.topological_sort(self):
-            if node != -1 and node != float('inf'):
-                nodes_list.append(node)
-        return nodes_list
-    
-    def node_qubits_predecessors(self, node:InstructionNode):
-        '''
-        node_qubits_predecessors is a dict of {qubits -> predecessors }of node
-        Args:
-            node in DAGCircuit, node should not be -1
-        Returns:
-            node_qubits_predecessors: dict of {qubits -> predecessors }of node
-        '''
-        # for edge in self.in_edges(node, data=True):
-        #     print(edge[0], edge[1], edge[2])
-
-        if node not in self.nodes:
-            raise ValueError('node should be in DAGCircuit')
-        if node in [-1]:
-            raise ValueError('-1 has no predecessors')
-
-        predecessor_nodes = [edge[0] for edge in self.in_edges(node, data=True)]
-        qubits_labels = [int(edge[2]['label'][1:]) for edge in self.in_edges(node, data=True)]
-        node_qubits_predecessors = dict(zip(qubits_labels, predecessor_nodes))
-        return node_qubits_predecessors
-    
-    def node_qubits_successors(self, node:InstructionNode):
-        '''
-        node_qubits_successors is a dict of {qubits -> successors }of node
-        Args: 
-            node in DAGCircuit, node should not be  float('inf')
-        Returns:
-            node_qubits_successors: dict of {qubits -> successors }of node
-
-
-        '''
-        if node not in self.nodes:
-            raise ValueError('node should be in DAGCircuit')
-        if node in [float('inf')]:
-            raise ValueError('float("inf") has no successors')
-        successor_nodes = [edge[1] for edge in self.out_edges(node, data=True)]
-        qubits_labels = [int(edge[2]['label'][1:]) for edge in self.out_edges(node, data=True)]
-        node_qubits_successors = dict(zip(qubits_labels, successor_nodes))
-        return node_qubits_successors
-
-    def node_qubits_inedges(self, node:InstructionNode):
-        '''
-        node_qubits_inedges is a dict of {qubits -> inedges }of node
-        Args:
-            node in DAGCircuit, node should not be -1
-        Returns:
-            node_qubits_inedges: dict of {qubits -> inedges }of node
-        '''
-        if node not in self.nodes:
-            raise ValueError('node should be in DAGCircuit')
-        if node in [-1]:
-            raise ValueError('-1 has no predecessors')
-
-        inedges = [edge for edge in self.in_edges(node)]
-        qubits_labels = [int(edge[2]['label'][1:]) for edge in self.in_edges(node, data=True)]
-        node_qubits_inedges = dict(zip(qubits_labels, inedges))
-        return node_qubits_inedges
-    
-    def node_qubits_outedges(self, node:InstructionNode):
-        '''
-        node_qubits_outedges is a dict of {qubits -> outedges }of node
-        Args:
-            node in DAGCircuit, node should not be float('inf')
-        Returns:
-            node_qubits_outedges: dict of {qubits -> outedges }of node
-        '''
-        if node not in self.nodes:
-            raise ValueError('node should be in DAGCircuit')
-        if node in [float('inf')]:
-            raise ValueError('float("inf") has no successors')
-        outedges = [edge for edge in self.out_edges(node)]
-        qubits_labels = [int(edge[2]['label'][1:]) for edge in self.out_edges(node, data=True)]
-        node_qubits_outedges = dict(zip(qubits_labels, outedges))
-        return node_qubits_outedges
-    
-    def remove_instruction_node(self, gate:InstructionNode):
-        '''
-        remove a gate from DAGCircuit, and all edges connected to it.
-        add new edges about qubits of removed gate between all predecessors and successors of removed gate.
-        Args:
-            gate: InstructionNode, gate should be in DAGCircuit, gate should not be -1 or float('inf')
-        '''
-
-        if gate not in self.nodes:
-            raise ValueError('gate should be in DAGCircuit')
-        if gate in [-1, float('inf')]:
-            raise ValueError('gate should not be -1 or float("inf")')
-
-        qubits_predecessors = self.node_qubits_predecessors(gate)
-        qubits_successors = self.node_qubits_successors(gate)
-        for qubit in gate.pos:
-            if qubits_predecessors[qubit] != -1 and qubits_successors[qubit] != float('inf'):
-                self.add_edge(qubits_predecessors[qubit], qubits_successors[qubit], label=f'q{qubit}')
-            elif qubits_predecessors[qubit] == -1 and qubits_successors[qubit] != float('inf'):
-                self.add_edge(qubits_predecessors[qubit], qubits_successors[qubit], label=f'q{qubit}',color='green')
-            else:
-                self.add_edge(qubits_predecessors[qubit], qubits_successors[qubit], label=f'q{qubit}',color='red')
-
-        self.remove_node(gate)
-
-        # update qubits
-        self.qubits_used = self.update_qubits_used()
-
-
-    def merge_dag(self, other_dag):
-        '''
-        merge other_dag into self
-        Args:
-            other_dag: DAGCircuit
-        Returns:
-            self: DAGCircuit
-        '''
-        if not isinstance(other_dag, DAGCircuit):
-            raise ValueError('other_dag should be a DAGCircuit')
-        if other_dag == None:
-            return self
-        if self == None:
-            return other_dag
-        
-        # for the same qubits (intersection), 
-        # remove the outgoing edges from the final node of the original DAG and the incoming edges from the initial node of the other DAG,
-        # then connect the corresponding tail and head nodes by adding edges
-        other_dag_qubits_used = other_dag.update_qubits_used()
-        self_qubits_used = self.update_qubits_used()
-
-        insect_qubits = self_qubits_used & other_dag_qubits_used
-        end_edges_labels_1 = self.node_qubits_inedges(float('inf'))
-        start_edges_labels_2 = other_dag.node_qubits_outedges(-1)
-
-        if len(insect_qubits) != 0:
-            for insect_qubit in insect_qubits:
-                self.remove_edges_from([end_edges_labels_1[insect_qubit]])
-                other_dag.remove_edges_from([start_edges_labels_2[insect_qubit]])
-                self.add_edge(end_edges_labels_1[insect_qubit][0], start_edges_labels_2[insect_qubit][1], label=f'q{insect_qubit}')
-        
-        # add other_dag's nodes and edges into self
-        # ！if we add edges, we don't need to add nodes again
-        self.add_edges_from(other_dag.edges(data=True))
-
-        # remove the edges between -1 and float('inf')
-        self.remove_edges_from([edge for edge in self.edges(data=True) if edge[0] == -1 and edge[1] == float('inf')])
- 
-        # update qubits 
-        self.qubits_used = self.update_qubits_used()
-  
-    def add_instruction_node(self, gate:InstructionNode,predecessors_dict:Dict[int,InstructionNode],successors_dict:Dict[int,InstructionNode]):
-        '''
-        add a gate into DAGCircuit, and all edges connected to it.
-        add new edges about qubits of new gate between all predecessors and successors of new gate.
-        Args:
-            gate: InstructionNode, gate should not be -1 or float('inf')
-            predecessors_dict: dict of {qubits -> predecessors }of gate
-            successors_dict: dict of {qubits -> successors }of gate
-        '''
-        if gate in [-1, float('inf')]:
-            raise ValueError('gate should not be -1 or float("inf")')
-        
-        #remove the edges between the predessors,successors about the qubits used by the added node
-        qubits_pre_out_edges = []
-        qubits_suc_in_edges = []
-        for qubit in gate.pos:
-            pre_out_edges = self.node_qubits_outedges(predecessors_dict[qubit])
-            qubits_pre_out_edges.append(pre_out_edges[qubit])
-
-            suc_in_edges = self.node_qubits_inedges(successors_dict[qubit])
-            qubits_suc_in_edges.append(suc_in_edges[qubit])
-
-        self.remove_edges_from(qubits_pre_out_edges)
-        self.remove_edges_from(qubits_suc_in_edges)
-
-        # add the new node and edges
-        for qubit in gate.pos:
-            if predecessors_dict[qubit] == -1:
-                self.add_edge(predecessors_dict[qubit], gate, label=f'q{qubit}',color='green')
-            else:
-                self.add_edge(predecessors_dict[qubit], gate, label=f'q{qubit}')
-            if successors_dict[qubit] == float('inf'):
-                self.add_edge(gate, successors_dict[qubit], label=f'q{qubit}',color='red')
-            else:
-                self.add_edge(gate, successors_dict[qubit], label=f'q{qubit}')
-
-        # update qubits
-        self.qubits_used = self.update_qubits_used()
-
-
-    def is_dag(self):
-        '''
-        is_dag is a bool value to check if DAGCircuit is a DAG
-        '''
-        return nx.is_directed_acyclic_graph(self)
+from typing import Dict
+
+import networkx as nx
+from networkx.classes.multidigraph import MultiDiGraph
+from quafu.dagcircuits.instruction_node import InstructionNode
+
+
+class DAGCircuit(MultiDiGraph):
+    def __init__(
+        self, qubits_used=None, cbits_used=None, incoming_graph_data=None, **attr
+    ):
+        super().__init__(incoming_graph_data, **attr)
+
+        if qubits_used is None:
+            self.qubits_used = set()
+        elif isinstance(qubits_used, set):
+            self.qubits_used = qubits_used
+        else:
+            raise ValueError("qubits_used should be a set or None")
+
+        if cbits_used is None:
+            self.cbits_used = set()
+        elif isinstance(cbits_used, set):
+            self.cbits_used = cbits_used
+        else:
+            raise ValueError("cbits_used should be a set or None")
+
+        # num of instruction nodes
+        self.num_instruction_nodes = 0
+
+    # add new methods or override existing methods here.
+
+    def update_qubits_used(self):
+        """
+        qubits_used is a set of qubits used in DAGCircuit
+        based on node -1's edges' labels, the qubits is the integer part of the label
+
+        return:
+            qubits_used: set of qubits used in DAGCircuit
+        """
+        if -1 not in self.nodes:
+            raise ValueError("-1 should be in DAGCircuit, please add it first")
+        self.qubits_used = set(
+            [int(edge[2]["label"][1:]) for edge in self.out_edges(-1, data=True)]
+        )
+        return self.qubits_used
+
+    def update_cbits_used(self):
+        """
+        cbits_used is a set of cbits used in DAGCircuit
+        calculated by  measurenode's cbits
+        return:
+            cbits_used: set of cbits used in DAGCircuit
+        """
+        for node in self.nodes:
+            # if node.has a attribute 'name' and node.name == 'measure'
+            if hasattr(node, "name") and node.name == "measure":
+                self.cbits_used = set(node.pos.values())
+        return self.cbits_used
+
+    def update_num_instruction_nodes(self):
+        """
+        num_instruction_nodes is the number of instruction nodes in DAGCircuit
+        """
+        if -1 not in self.nodes:
+            raise ValueError("-1 should be in DAGCircuit, please add it first")
+        if float("inf") not in self.nodes:
+            raise ValueError(
+                'float("inf") should be in DAGCircuit, please add it first'
+            )
+        self.num_instruction_nodes = len(self.nodes) - 2
+
+        for node in self.nodes:
+            if hasattr(node, "name") and node.name == "measure":
+                self.num_instruction_nodes -= 1
+        return self.num_instruction_nodes
+
+    def nodes_dict(self):
+        """
+        nodes_dict is a dictionary of nodes with the node label as key and the node as value.
+        without  -1 and float('inf')
+        """
+        nodes_dict = {}
+        for node in nx.topological_sort(self):
+            if node != -1 and node != float("inf"):
+                nodes_dict[node.label] = node
+        return nodes_dict
+
+    def nodes_list(self):
+        """
+        nodes_list is a list of nodes without  -1 and float('inf')
+        """
+        nodes_list = []
+        for node in nx.topological_sort(self):
+            if node != -1 and node != float("inf"):
+                nodes_list.append(node)
+        return nodes_list
+
+    def node_qubits_predecessors(self, node: InstructionNode):
+        """
+        node_qubits_predecessors is a dict of {qubits -> predecessors }of node
+        Args:
+            node in DAGCircuit, node should not be -1
+        Returns:
+            node_qubits_predecessors: dict of {qubits -> predecessors }of node
+        """
+        # for edge in self.in_edges(node, data=True):
+        #     print(edge[0], edge[1], edge[2])
+
+        if node not in self.nodes:
+            raise ValueError("node should be in DAGCircuit")
+        if node in [-1]:
+            raise ValueError("-1 has no predecessors")
+
+        predecessor_nodes = [edge[0] for edge in self.in_edges(node, data=True)]
+        qubits_labels = [
+            int(edge[2]["label"][1:]) for edge in self.in_edges(node, data=True)
+        ]
+        node_qubits_predecessors = dict(zip(qubits_labels, predecessor_nodes))
+        return node_qubits_predecessors
+
+    def node_qubits_successors(self, node: InstructionNode):
+        """
+        node_qubits_successors is a dict of {qubits -> successors }of node
+        Args:
+            node in DAGCircuit, node should not be  float('inf')
+        Returns:
+            node_qubits_successors: dict of {qubits -> successors }of node
+
+
+        """
+        if node not in self.nodes:
+            raise ValueError("node should be in DAGCircuit")
+        if node in [float("inf")]:
+            raise ValueError('float("inf") has no successors')
+        successor_nodes = [edge[1] for edge in self.out_edges(node, data=True)]
+        qubits_labels = [
+            int(edge[2]["label"][1:]) for edge in self.out_edges(node, data=True)
+        ]
+        node_qubits_successors = dict(zip(qubits_labels, successor_nodes))
+        return node_qubits_successors
+
+    def node_qubits_inedges(self, node: InstructionNode):
+        """
+        node_qubits_inedges is a dict of {qubits -> inedges }of node
+        Args:
+            node in DAGCircuit, node should not be -1
+        Returns:
+            node_qubits_inedges: dict of {qubits -> inedges }of node
+        """
+        if node not in self.nodes:
+            raise ValueError("node should be in DAGCircuit")
+        if node in [-1]:
+            raise ValueError("-1 has no predecessors")
+
+        inedges = [edge for edge in self.in_edges(node)]
+        qubits_labels = [
+            int(edge[2]["label"][1:]) for edge in self.in_edges(node, data=True)
+        ]
+        node_qubits_inedges = dict(zip(qubits_labels, inedges))
+        return node_qubits_inedges
+
+    def node_qubits_outedges(self, node: InstructionNode):
+        """
+        node_qubits_outedges is a dict of {qubits -> outedges }of node
+        Args:
+            node in DAGCircuit, node should not be float('inf')
+        Returns:
+            node_qubits_outedges: dict of {qubits -> outedges }of node
+        """
+        if node not in self.nodes:
+            raise ValueError("node should be in DAGCircuit")
+        if node in [float("inf")]:
+            raise ValueError('float("inf") has no successors')
+        outedges = [edge for edge in self.out_edges(node)]
+        qubits_labels = [
+            int(edge[2]["label"][1:]) for edge in self.out_edges(node, data=True)
+        ]
+        node_qubits_outedges = dict(zip(qubits_labels, outedges))
+        return node_qubits_outedges
+
+    def remove_instruction_node(self, gate: InstructionNode):
+        """
+        remove a gate from DAGCircuit, and all edges connected to it.
+        add new edges about qubits of removed gate between all predecessors and successors of removed gate.
+        Args:
+            gate: InstructionNode, gate should be in DAGCircuit, gate should not be -1 or float('inf')
+        """
+
+        if gate not in self.nodes:
+            raise ValueError("gate should be in DAGCircuit")
+        if gate in [-1, float("inf")]:
+            raise ValueError('gate should not be -1 or float("inf")')
+
+        qubits_predecessors = self.node_qubits_predecessors(gate)
+        qubits_successors = self.node_qubits_successors(gate)
+        for qubit in gate.pos:
+            if qubits_predecessors[qubit] != -1 and qubits_successors[qubit] != float(
+                "inf"
+            ):
+                self.add_edge(
+                    qubits_predecessors[qubit],
+                    qubits_successors[qubit],
+                    label=f"q{qubit}",
+                )
+            elif qubits_predecessors[qubit] == -1 and qubits_successors[qubit] != float(
+                "inf"
+            ):
+                self.add_edge(
+                    qubits_predecessors[qubit],
+                    qubits_successors[qubit],
+                    label=f"q{qubit}",
+                    color="green",
+                )
+            else:
+                self.add_edge(
+                    qubits_predecessors[qubit],
+                    qubits_successors[qubit],
+                    label=f"q{qubit}",
+                    color="red",
+                )
+
+        self.remove_node(gate)
+
+        # update qubits
+        self.qubits_used = self.update_qubits_used()
+
+    def merge_dag(self, other_dag):
+        """
+        merge other_dag into self
+        Args:
+            other_dag: DAGCircuit
+        Returns:
+            self: DAGCircuit
+        """
+        if not isinstance(other_dag, DAGCircuit):
+            raise ValueError("other_dag should be a DAGCircuit")
+        if other_dag == None:
+            return self
+        if self == None:
+            return other_dag
+
+        # for the same qubits (intersection),
+        # remove the outgoing edges from the final node of the original DAG and the incoming edges from the initial node of the other DAG,
+        # then connect the corresponding tail and head nodes by adding edges
+        other_dag_qubits_used = other_dag.update_qubits_used()
+        self_qubits_used = self.update_qubits_used()
+
+        insect_qubits = self_qubits_used & other_dag_qubits_used
+        end_edges_labels_1 = self.node_qubits_inedges(float("inf"))
+        start_edges_labels_2 = other_dag.node_qubits_outedges(-1)
+
+        if len(insect_qubits) != 0:
+            for insect_qubit in insect_qubits:
+                self.remove_edges_from([end_edges_labels_1[insect_qubit]])
+                other_dag.remove_edges_from([start_edges_labels_2[insect_qubit]])
+                self.add_edge(
+                    end_edges_labels_1[insect_qubit][0],
+                    start_edges_labels_2[insect_qubit][1],
+                    label=f"q{insect_qubit}",
+                )
+
+        # add other_dag's nodes and edges into self
+        # ！if we add edges, we don't need to add nodes again
+        self.add_edges_from(other_dag.edges(data=True))
+
+        # remove the edges between -1 and float('inf')
+        self.remove_edges_from(
+            [
+                edge
+                for edge in self.edges(data=True)
+                if edge[0] == -1 and edge[1] == float("inf")
+            ]
+        )
+
+        # update qubits
+        self.qubits_used = self.update_qubits_used()
+
+    def add_instruction_node(
+        self,
+        gate: InstructionNode,
+        predecessors_dict: Dict[int, InstructionNode],
+        successors_dict: Dict[int, InstructionNode],
+    ):
+        """
+        add a gate into DAGCircuit, and all edges connected to it.
+        add new edges about qubits of new gate between all predecessors and successors of new gate.
+        Args:
+            gate: InstructionNode, gate should not be -1 or float('inf')
+            predecessors_dict: dict of {qubits -> predecessors }of gate
+            successors_dict: dict of {qubits -> successors }of gate
+        """
+        if gate in [-1, float("inf")]:
+            raise ValueError('gate should not be -1 or float("inf")')
+
+        # remove the edges between the predessors,successors about the qubits used by the added node
+        qubits_pre_out_edges = []
+        qubits_suc_in_edges = []
+        for qubit in gate.pos:
+            pre_out_edges = self.node_qubits_outedges(predecessors_dict[qubit])
+            qubits_pre_out_edges.append(pre_out_edges[qubit])
+
+            suc_in_edges = self.node_qubits_inedges(successors_dict[qubit])
+            qubits_suc_in_edges.append(suc_in_edges[qubit])
+
+        self.remove_edges_from(qubits_pre_out_edges)
+        self.remove_edges_from(qubits_suc_in_edges)
+
+        # add the new node and edges
+        for qubit in gate.pos:
+            if predecessors_dict[qubit] == -1:
+                self.add_edge(
+                    predecessors_dict[qubit], gate, label=f"q{qubit}", color="green"
+                )
+            else:
+                self.add_edge(predecessors_dict[qubit], gate, label=f"q{qubit}")
+            if successors_dict[qubit] == float("inf"):
+                self.add_edge(
+                    gate, successors_dict[qubit], label=f"q{qubit}", color="red"
+                )
+            else:
+                self.add_edge(gate, successors_dict[qubit], label=f"q{qubit}")
+
+        # update qubits
+        self.qubits_used = self.update_qubits_used()
+
+    def is_dag(self):
+        """
+        is_dag is a bool value to check if DAGCircuit is a DAG
+        """
+        return nx.is_directed_acyclic_graph(self)
```

## quafu/dagcircuits/instruction_node.py

```diff
@@ -1,40 +1,41 @@
-from typing import Dict, Any, List, Union
-import dataclasses 
-
-@dataclasses.dataclass
-class InstructionNode: 
-    name:Any            # gate.name
-    pos:Union[List[Any], Dict[Any,Any]]       # gate.pos |  Dict[Any,Any] for measure
-    paras:List[Any]        # gate.paras
-    # matrix:List[Any]   # for gate in [QuantumGate]
-    duration: Union[float,int]  # for gate in [Delay,XYResonance,QuantumPulse] in quafu
-    unit:str           # for gate in [Delay,XYResonance] in quafu
-    channel:str        # for gate in [QuantumPulse] in quafu
-    time_func: Any     # for gate in [QuantumPulse] in quafu
-    label:str          # used for specifying the instruction node
-        
-    def __hash__(self):
-        return hash((type(self.name), tuple(self.pos) ,self.label))
-    
-    def __str__(self):
-        if self.name == 'measure':
-            args = ','.join(str(q) for q in self.pos.keys())
-            args += f'=>{",".join(str(c) for c in self.pos.values())}'
-        else:    
-            args = ','.join(str(q) for q in self.pos)
-            
-        if self.paras == None:
-            return f'{self.label}{{{self.name}({args})}}' # no paras
-        else:
-            # if self.paras not a list, then make it a list  of str of .3f float
-            if not isinstance(self.paras, list):
-                formatted_paras = [f'{self.paras:.3f}']
-            else:
-                formatted_paras = [f'{p:.3f}' for p in self.paras]  
-                
-            formatted_paras_str = ','.join(formatted_paras)
-            
-            return f'{self.label}{{{self.name}({args})}}({formatted_paras_str})'
-    
-    def __repr__(self): 
-        return str(self)
+import dataclasses
+from typing import Any, Dict, List, Union
+
+
+@dataclasses.dataclass
+class InstructionNode:
+    name: Any  # gate.name
+    pos: Union[List[Any], Dict[Any, Any]]  # gate.pos |  Dict[Any,Any] for measure
+    paras: List[Any]  # gate.paras
+    # matrix:List[Any]   # for gate in [QuantumGate]
+    duration: Union[float, int]  # for gate in [Delay,XYResonance,QuantumPulse] in quafu
+    unit: str  # for gate in [Delay,XYResonance] in quafu
+    channel: str  # for gate in [QuantumPulse] in quafu
+    time_func: Any  # for gate in [QuantumPulse] in quafu
+    label: str  # used for specifying the instruction node
+
+    def __hash__(self):
+        return hash((type(self.name), tuple(self.pos), self.label))
+
+    def __str__(self):
+        if self.name == "measure":
+            args = ",".join(str(q) for q in self.pos.keys())
+            args += f'=>{",".join(str(c) for c in self.pos.values())}'
+        else:
+            args = ",".join(str(q) for q in self.pos)
+
+        if self.paras == None:
+            return f"{self.label}{{{self.name}({args})}}"  # no paras
+        else:
+            # if self.paras not a list, then make it a list  of str of .3f float
+            if not isinstance(self.paras, list):
+                formatted_paras = [f"{self.paras:.3f}"]
+            else:
+                formatted_paras = [f"{p:.3f}" for p in self.paras]
+
+            formatted_paras_str = ",".join(formatted_paras)
+
+            return f"{self.label}{{{self.name}({args})}}({formatted_paras_str})"
+
+    def __repr__(self):
+        return str(self)
```

## quafu/elements/__init__.py

```diff
@@ -1,3 +1,9 @@
-from .instruction import Instruction, Barrier, Measure
-from .pulses import Delay, XYResonance, QuantumPulse
-from .quantum_gate import QuantumGate, ControlledGate, MultiQubitGate, SingleQubitGate
+from .classical_element import Cif
+from .instruction import Barrier, Instruction, Measure, Reset
+from .pulses import Delay, QuantumPulse, XYResonance
+from .quantum_gate import ControlledGate, QuantumGate, CircuitWrapper, ControlledCircuitWrapper
+from .unitary import UnitaryDecomposer
+from .utils import extract_float, reorder_matrix
+from .oracle import OracleGate, ControlledOracle
+from .parameters import Parameter, ParameterExpression, ParameterType
+from .noise import KrausChannel, UnitaryChannel
```

## quafu/elements/instruction.py

```diff
@@ -1,129 +1,200 @@
-#  (C) Copyright 2023 Beijing Academy of Quantum Information Sciences
-#
-#  Licensed under the Apache License, Version 2.0 (the "License");
-#  you may not use this file except in compliance with the License.
-#  You may obtain a copy of the License at
-#
-#   http://www.apache.org/licenses/LICENSE-2.0
-#
-#  Unless required by applicable law or agreed to in writing, software
-#  distributed under the License is distributed on an "AS IS" BASIS,
-#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#  See the License for the specific language governing permissions and
-#  limitations under the License.
-
-from abc import ABC, abstractmethod
-from typing import Union, List, Dict
-
-
-__all__ = ['Instruction', 'Barrier', 'Measure', 'PosType', 'ParaType']
-
-PosType = Union[int, List[int]]
-ParaType = Union[float, int, List]
-
-
-class Instruction(ABC):
-    """Base class for ALL the possible instructions on Quafu superconducting quantum circuits.
-
-    Attributes:
-        pos: Qubit position(s) of the instruction on the circuit.
-        paras: Parameters of the instruction.
-
-    """
-    ins_classes = {}
-
-    def __init__(self, pos: PosType, paras: ParaType = None, *args, **kwargs):
-        self.pos = pos
-        self.paras = paras
-
-    @property
-    @abstractmethod
-    def name(self) -> str:
-        """Name of the instruction."""
-        raise NotImplementedError('name is not implemented for %s' % self.__class__.__name__
-                                  + ', this should never happen.')
-
-    @property
-    @abstractmethod
-    def named_paras(self) -> Dict:
-        """dict-mapping for parameters"""
-        return {}
-
-    @property
-    @abstractmethod
-    def named_pos(self) -> Dict:
-        """dict-mapping for positions"""
-        return {'pos': self.pos}
-
-    @name.setter
-    def name(self, _):
-        import warnings
-        warnings.warn("Invalid assignment, names of standard instructions are not alterable.")
-
-    @classmethod
-    def register_ins(cls, subclass, name: str = None):
-        assert issubclass(subclass, cls)
-
-        if name is None:
-            name = subclass.name
-        if name in cls.ins_classes:
-            raise ValueError(f"Name {name} already exists.")
-        cls.ins_classes[name] = subclass
-
-    @abstractmethod
-    def to_qasm(self):
-        pass
-
-
-class Barrier(Instruction):
-    """
-    Barrier instruction.
-    """
-    name = "barrier"
-
-    def __init__(self, pos):
-        super().__init__(pos)
-        self.symbol = "||"
-
-    @property
-    def named_pos(self):
-        return self.named_pos
-
-    @property
-    def named_paras(self):
-        return self.named_paras
-
-    def __repr__(self):
-        return f"{self.__class__.__name__}"
-
-    def to_qasm(self):
-        return "barrier " + ",".join(["q[%d]" % p for p in range(min(self.pos), max(self.pos) + 1)])
-
-
-class Measure(Instruction):
-    """
-    Measure instruction.
-    """
-    name = "measure"
-
-    def __init__(self, bitmap: dict):
-        super().__init__(list(bitmap.keys()))
-        self.qbits = self.pos
-        self.cbits = list(bitmap.values())
-
-    @property
-    def named_pos(self):
-        return {'pos': self.pos}  # TODO
-
-    @property
-    def named_paras(self):
-        return self.named_paras
-
-    def to_qasm(self):
-        lines = ["measure q[%d] -> meas[%d];\n" % (q, c) for q, c in zip(self.qbits, self.cbits)]
-        qasm = ''.join(lines)
-        return qasm
-
-
-Instruction.register_ins(Barrier)
-Instruction.register_ins(Measure)
+#  (C) Copyright 2023 Beijing Academy of Quantum Information Sciences
+#
+#  Licensed under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License.
+
+from abc import ABC, abstractmethod
+from typing import Dict, List, Optional, Union 
+
+from .parameters import ParameterType
+
+__all__ = ["Instruction", "Barrier", "Measure", "Reset"]
+
+
+
+class Instruction(ABC):
+    """Base class for ALL the possible instructions on Quafu superconducting quantum circuits.
+
+    Attributes:
+        pos: Qubit position(s) of the instruction on the circuit.
+        paras: Parameters of the instruction.
+
+    """
+
+    ins_classes = {}
+
+    def __init__(
+        self,
+        pos: List[int],
+        paras: List[ParameterType] = [],
+        *args,
+        **kwargs,
+    ):
+        self.pos = pos
+        self.paras = paras
+        self._symbol = None
+
+    @property
+    @abstractmethod
+    def name(self) -> str:
+        raise NotImplementedError(
+            "name is not implemented for %s" % self.__class__.__name__
+            + ", this should never happen."
+        )
+
+    @property
+    @abstractmethod
+    def named_paras(self) -> Dict:
+        """dict-mapping for parameters"""
+        return {}
+
+    @property
+    @abstractmethod
+    def named_pos(self) -> Dict:
+        """dict-mapping for positions"""
+        return {"pos": self.pos}
+
+    @name.setter
+    def name(self, _):
+        import warnings
+
+        warnings.warn(
+            "Invalid assignment, names of standard instructions are not alterable."
+        )
+
+    @classmethod
+    def register_ins(cls, subclass, name: str = None):
+        assert issubclass(subclass, cls)
+
+        if name is None:
+            name = str(subclass.__name__).lower()
+        if name in cls.ins_classes:
+            raise ValueError(f"Name {name} already exists.")
+        cls.ins_classes[name] = subclass
+        return subclass
+    
+    @classmethod
+    def register(cls, name: str = None):
+        def wrapper(subclass):
+            return cls.register_ins(subclass, name)
+        
+        return wrapper
+
+    @abstractmethod
+    def to_qasm(self, with_para):
+        pass
+
+
+class Barrier(Instruction):
+    """
+    Barrier instruction.
+    """
+
+    name = "barrier"
+
+    # def to_dag_node(self):
+    #     name = self.get_ins_id()
+    #     label = self.__repr__()
+    #
+    #     pos = self.pos
+    #     paras = self.paras
+    #     paras = {} if paras is None else paras
+    #     duration = paras.get('duration', None)
+    #     unit = paras.get('unit', None)
+    #     channel = paras.get('channel', None)
+    #     time_func = paras.get('time_func', None)
+    #
+    #     return InstructionNode(name, pos, paras, duration, unit, channel, time_func, label)
+
+    def __init__(self, pos):
+        super().__init__(pos)
+        self.symbol = "||"
+
+    @property
+    def named_pos(self):
+        return super().named_pos
+
+    @property
+    def named_paras(self):
+        return super().named_pos
+
+    def __repr__(self):
+        return f"{self.__class__.__name__}"
+
+    def to_qasm(self, with_para):
+        return "barrier " + ",".join(
+            ["q[%d]" % p for p in range(min(self.pos), max(self.pos) + 1)]
+        )
+
+
+class Reset(Instruction):
+    name = "reset"
+
+    def __init__(self, pos):
+        super().__init__(pos)
+
+    @property
+    def pos(self):
+        return self.__pos
+
+    @pos.setter
+    def pos(self, pos):
+        self.__pos = pos
+
+    @property
+    def named_pos(self):
+        return self.named_pos
+
+    @property
+    def named_paras(self):
+        return self.named_paras
+
+    def __repr__(self):
+        return f"{self.__class__.__name__}"
+
+    def to_qasm(self, with_para):
+        return "reset " + ",".join(
+            ["q[%d]" % p for p in range(min(self.pos), max(self.pos) + 1)]
+        )
+
+
+class Measure(Instruction):
+    """
+    Measure instruction.
+    """
+
+    name = "measure"
+
+    def __init__(self, bitmap: dict):
+        super().__init__(list(bitmap.keys()))
+        self.qbits = list(bitmap.keys())
+        self.cbits = list(bitmap.values())
+
+    @property
+    def named_pos(self):
+        return {"pos": self.pos}  # TODO
+
+    @property
+    def named_paras(self):
+        return self.named_paras
+
+    def to_qasm(self, with_para):
+        lines = [
+            "measure q[%d] -> meas[%d];\n" % (q, c)
+            for q, c in zip(self.qbits, self.cbits)
+        ]
+        qasm = "".join(lines)
+        return qasm
+
+
+Instruction.register_ins(Barrier)
+Instruction.register_ins(Measure)
```

## quafu/elements/pulses.py

```diff
@@ -1,270 +1,285 @@
-from abc import ABC, abstractmethod
-from copy import deepcopy
-from typing import Union, Optional, Dict
-
-import matplotlib.pyplot as plt
-import numpy as np
-
-from .instruction import Instruction, PosType
-
-TimeType = Union[np.ndarray, float, int]
-
-
-class QuantumPulse(Instruction, ABC):
-    pulse_classes = {}
-
-    def __init__(self,
-                 pos: PosType,
-                 duration: Union[float, int],
-                 unit: str = 'ns',
-                 channel: str = None,
-                 paras: list = None,
-                 ):
-        """
-        Quantum Pulse for generating a quantum gate.
-
-        Args:
-            pos (int): Qubit position.
-            paras (list): Parameters of the pulse.
-            duration (float, int): Pulse duration.
-            unit (str): Duration unit.
-        """
-        super().__init__(pos, paras)
-        self.duration = duration
-        self.unit = unit
-        if channel in ["XY", "Z"]:
-            self.channel = channel
-        else:
-            raise ValueError("channel must be 'XY' or 'Z'")
-
-    @property
-    def symbol(self):
-        return "%s(%d%s, %s)" % (self.name, self.duration, self.unit, self.channel)
-
-    @property
-    def named_pos(self) -> Dict:
-        return {'pos': self.pos}
-
-    @abstractmethod
-    def time_func(self, t: Union[np.ndarray, float, int]):
-        """
-        Return the pulse data.
-
-        Args:
-            t (np.ndarray, float, int): Time list.
-        """
-        pass
-
-    @classmethod
-    def register_pulse(cls, subclass, name: str = None):
-        assert issubclass(subclass, cls)
-
-        if name is None:
-            name = subclass.name
-        if name in cls.pulse_classes:
-            raise ValueError(f"Name {name} already exists.")
-        cls.pulse_classes[name] = subclass
-        Instruction.register_ins(subclass, name)
-
-    def __repr__(self):
-        return self.__str__()
-
-    def __str__(self):
-        symbol = "%s(%d%s" % (self.name, self.duration, self.unit)
-        for para in self.paras:
-            symbol += ", %s" % para
-        symbol += ", %s" % self.channel
-        symbol += ")"
-        return symbol
-
-    def __call__(self,
-                 t: TimeType,
-                 shift: Union[float, int] = 0.,
-                 offset: Union[float, int] = 0.
-                 ):
-        """
-        Return pulse data.
-
-        Args:
-            t (np.ndarray, float, int): Time list.
-            shift (float, int): Time shift.
-            offset (float, int): Pulse amplitude offset.
-        """
-        window = np.logical_and(0 <= t, t <= self.duration)
-        return window * self.time_func(t - shift)
-
-    def __copy__(self):
-        """ Return a deepcopy of the pulse """
-        return deepcopy(self)
-
-    def to_qasm(self):
-        return self.__str__() + " q[%d]" % self.pos
-
-    # TODO: deprecate this
-    def plot(self,
-             t: Optional[np.ndarray] = None,
-             shift: Union[float, int] = 0.,
-             offset: Union[float, int] = 0.,
-             plot_real: bool = True,
-             plot_imag: bool = True,
-             fig=None,
-             ax=None,
-             **plot_kws):
-        """
-        Plot the pulse waveform.
-
-        Args:
-            t (np.ndarray): Time list of the plot.
-            shift (float, int): Time shift of the pulse.
-            offset (float, int): Offset of the pulse.
-            plot_real (bool): Plot real of the pulse.
-            plot_imag (bool): Plot imag of the pulse.
-            fig (Figure): Figure of the plot.
-            ax (Axes): Axes of the plot.
-            plot_kws (dict, optional): Plot kwargs of `ax.plot`.
-        """
-        if t is None:
-            t = np.linspace(0, self.duration, 101)
-        if ax is None:
-            fig, ax = plt.subplots(1, 1, num=fig)
-        pulse_data = self(t, shift=shift, offset=offset)
-        if plot_real:
-            ax.plot(np.real(pulse_data), label='real', **plot_kws)
-        if plot_imag:
-            ax.plot(np.imag(pulse_data), label='imag', **plot_kws)
-        ax.set_xlabel("Time (%s)" % self.unit)
-        ax.set_ylabel("Pulse Amp (a.u.)")
-        ax.legend()
-        plt.show()
-
-    def set_unit(self, unit="ns"):
-        """ Set duration unit """
-        self.unit = unit
-        return self
-
-
-class RectPulse(QuantumPulse):
-    name = "rect"
-
-    def __init__(self, pos, amp, duration, unit, channel):
-        self.amp = amp
-
-        super().__init__(pos, duration, unit, channel, amp)
-
-    @property
-    def named_paras(self) -> Dict:
-        named_paras = {'amp': self.amp,
-                       'duration': self.duration}
-        return named_paras
-
-    def time_func(self, t: Union[np.ndarray, float, int]):
-        """ rect_time_func """
-        return self.amp * np.ones(np.array(t).shape)
-
-
-class FlattopPulse(QuantumPulse):
-    name = "flattop"
-
-    def __init__(self, pos, amp, fwhm, duration, unit, channel):
-        self.amp = amp
-        self.fwhm = fwhm
-
-        super().__init__(pos, duration, unit, channel, [amp, fwhm])
-
-    @property
-    def named_paras(self) -> Dict:
-        named_paras = {'amp': self.amp,
-                       'duration': self.duration,
-                       "fwhm": self.fwhm}
-        return named_paras
-    
-    def time_func(self, t):
-        """ flattop_time_func """
-        from scipy.special import erf
-        sigma_ = self.fwhm / (2 * np.sqrt(np.log(2)))
-        return self.amp * (erf((self.duration - t) / sigma_) + erf(t / sigma_) - 1.)
-
-
-class GaussianPulse(QuantumPulse):
-    name = "gaussian"
-
-    def __init__(self, pos, duration, unit, channel, amp, fwhm, phase):
-        self.amp = amp
-        self.fwhm = 0.5 * duration if fwhm is None else fwhm
-        self.phase = phase
-
-        super().__init__(pos, duration, unit, channel, [amp, fwhm, phase])
-
-    def time_func(self, t):
-        """ gaussian_time_func """
-        # start: t = 0, center: t = 0.5 * duration, end: t = duration
-        sigma_ = self.fwhm / np.sqrt(8 * np.log(2))  # fwhm to std. deviation
-        return self.amp * np.exp(
-            -(t - 0.5 * self.duration) ** 2 / (2 * sigma_ ** 2) + 1j * self.phase)
-
-    @property
-    def named_paras(self) -> Dict:
-        named_paras = {'amp': self.amp,
-                       'duration': self.duration,
-                       "fwhm": self.fwhm,
-                       "phase": self.phase}
-        return named_paras
-
-
-class Delay(Instruction):
-    name = "delay"
-
-    def __init__(self, pos: int, duration: int, unit="ns"):
-        if isinstance(duration, int):
-            self.duration = duration
-        else:
-            raise TypeError("duration must be int")
-        super().__init__(pos)
-        self.unit = unit
-        self.symbol = "Delay(%d%s)" % (duration, unit)
-
-    def __repr__(self):
-        return f"{self.__class__.__name__}"
-
-    def to_qasm(self):
-        return "delay(%d%s) q[%d]" % (self.duration, self.unit, self.pos)
-
-    @property
-    def named_paras(self) -> Dict:
-        return {}
-
-    @property
-    def named_pos(self) -> Dict:
-        return {'pos': self.pos}
-
-
-class XYResonance(Instruction):
-    name = "XY"
-
-    def __init__(self, qs: int, qe: int, duration: int, unit="ns"):
-        if isinstance(duration, int):
-            self.duration = duration
-        else:
-            raise TypeError("duration must be int")
-        super().__init__(list(range(qs, qe + 1)))
-        self.unit = unit
-        self.symbol = "XY(%d%s)" % (duration, unit)
-
-    def to_qasm(self):
-        return "xy(%d%s) " % (self.duration, self.unit) + ",".join(
-            ["q[%d]" % p for p in range(min(self.pos), max(self.pos) + 1)])
-
-    @property
-    def named_pos(self) -> Dict:
-        return {'pos': self.pos}
-
-    @property
-    def named_paras(self) -> Dict:
-        return {'duration': self.duration}
-
-
-QuantumPulse.register_pulse(RectPulse)
-QuantumPulse.register_pulse(FlattopPulse)
-QuantumPulse.register_pulse(GaussianPulse)
-Instruction.register_ins(Delay)
-Instruction.register_ins(XYResonance)
+from abc import ABC, abstractmethod
+from copy import deepcopy
+from typing import Optional, Union
+
+import matplotlib.pyplot as plt
+import numpy as np
+from quafu.elements.instruction import Instruction
+
+TimeType = Union[np.ndarray, float, int]
+
+
+class QuantumPulse(Instruction, ABC):
+    pulse_classes = {}
+
+    def __init__(
+        self,
+        pos: int,
+        paras: list,
+        duration: Union[float, int],
+        unit: str,
+        channel: str,
+    ):
+        """
+        Quantum Pulse for generating a quantum gate.
+
+        Args:
+            pos (int): Qubit position.
+            paras (list): Parameters of the pulse.
+            duration (float, int): Pulse duration.
+            unit (str): Duration unit.
+        """
+        super().__init__()
+        self.pos = pos
+        self.paras = paras
+        self.duration = duration
+        self.unit = unit
+        if channel in ["XY", "Z"]:
+            self.channel = channel
+        else:
+            raise ValueError("channel must be 'XY' or 'Z'")
+
+    @property
+    def symbol(self):
+        return "%s(%d%s, %s)" % (self.name, self.duration, self.unit, self.channel)
+
+    @abstractmethod
+    def time_func(self, t: Union[np.ndarray, float, int], **kwargs):
+        """
+        Return the pulse data.
+
+        Args:
+            t (np.ndarray, float, int): Time list.
+            kwargs (dict): Keyword arguments for the pulse.
+        """
+        pass
+
+    @classmethod
+    def register_pulse(cls, subclass, name: str = None):
+        assert issubclass(subclass, cls)
+
+        if name is None:
+            name = subclass.name
+        if name in cls.pulse_classes:
+            raise ValueError(f"Name {name} already exists.")
+        cls.pulse_classes[name] = subclass
+        Instruction.register_ins(subclass, name)
+
+    def __repr__(self):
+        return self.__str__()
+
+    def __str__(self):
+        symbol = "%s(%d%s" % (self.name, self.duration, self.unit)
+        for para in self.paras:
+            symbol += ", %s" % para
+        symbol += ", %s" % self.channel
+        symbol += ")"
+        return symbol
+
+    def __call__(
+        self,
+        t: TimeType,
+        shift: Union[float, int] = 0.0,
+        offset: Union[float, int] = 0.0,
+        args: dict = None,
+    ):
+        """
+        Return pulse data.
+
+        Args:
+            t (np.ndarray, float, int): Time list.
+            shift (float, int): Time shift.
+            offset (float, int): Pulse amplitude offset.
+        """
+        window = np.logical_and(0 <= t, t <= self.duration)
+        if args is None:
+            return window * self.time_func(t - shift)
+        else:
+            return window * self.time_func(t - shift, **args)
+
+    def __copy__(self):
+        """Return a deepcopy of the pulse"""
+        return deepcopy(self)
+
+    def to_qasm(self, with_para):
+        return self.__str__() + " q[%d]" % self.pos
+
+    def plot(
+        self,
+        t: Optional[np.ndarray] = None,
+        shift: Union[float, int] = 0.0,
+        offset: Union[float, int] = 0.0,
+        plot_real: bool = True,
+        plot_imag: bool = True,
+        fig=None,
+        ax=None,
+        **plot_kws,
+    ):
+        """
+        Plot the pulse waveform.
+
+        Args:
+            t (np.ndarray): Time list of the plot.
+            shift (float, int): Time shift of the pulse.
+            offset (float, int): Offset of the pulse.
+            plot_real (bool): Plot real of the pulse.
+            plot_imag (bool): Plot imag of the pulse.
+            fig (Figure): Figure of the plot.
+            ax (Axes): Axes of the plot.
+            plot_kws (dict, optional): Plot kwargs of `ax.plot`.
+        """
+        if t is None:
+            t = np.linspace(0, self.duration, 101)
+        if ax is None:
+            fig, ax = plt.subplots(1, 1, num=fig)
+        pulse_data = self(t, shift=shift, offset=offset)
+        if plot_real:
+            ax.plot(np.real(pulse_data), label="real", **plot_kws)
+        if plot_imag:
+            ax.plot(np.imag(pulse_data), label="imag", **plot_kws)
+        ax.set_xlabel("Time (%s)" % self.unit)
+        ax.set_ylabel("Pulse Amp (a.u.)")
+        ax.legend()
+        plt.show()
+
+    def set_pos(self, pos: int):
+        """Set qubit position"""
+        self.pos = pos
+        return self
+
+    def set_unit(self, unit="ns"):
+        """Set duration unit"""
+        self.unit = unit
+        return self
+
+
+class RectPulse(QuantumPulse):
+    name = "rect"
+
+    def __init__(self, pos, amp, duration, unit, channel):
+        self.amp = amp
+
+        super().__init__(pos, [amp], duration, unit, channel)
+
+    def time_func(self, t: Union[np.ndarray, float, int], **kwargs):
+        """rect_time_func"""
+        amp_ = kwargs["amp"]
+        return amp_ * np.ones(np.array(t).shape)
+
+    def __call__(
+        self,
+        t: TimeType,
+        shift: Union[float, int] = 0,
+        offset: Union[float, int] = 0,
+        *args,
+        **kwargs,
+    ):
+        args = {"amp": self.amp}
+        return super().__call__(t, shift, offset, args)
+
+
+class FlattopPulse(QuantumPulse):
+    name = "flattop"
+
+    def __init__(self, pos, amp, fwhm, duration, unit, channel):
+        self.amp = amp
+        self.fwhm = fwhm
+
+        super().__init__(pos, [amp, fwhm], duration, unit, channel)
+
+    def time_func(self, t, **kws):
+        """flattop_time_func"""
+        from scipy.special import erf
+
+        amp_, fwhm_ = kws["amp"], kws["fwhm"]
+        sigma_ = fwhm_ / (2 * np.sqrt(np.log(2)))
+        return amp_ * (erf((self.duration - t) / sigma_) + erf(t / sigma_) - 1.0)
+
+    def __call__(
+        self,
+        t: TimeType,
+        shift: Union[float, int] = 0,
+        offset: Union[float, int] = 0,
+        *args,
+        **kwargs,
+    ):
+        args = {"amp": self.amp, "fwhm": self.fwhm}
+        return super().__call__(t, shift, offset, args)
+
+
+class GaussianPulse(QuantumPulse):
+    name = "gaussian"
+
+    def __init__(self, pos, amp, fwhm, phase, duration, unit, channel):
+        self.amp = amp
+        if fwhm is None:
+            self.fwhm = 0.5 * duration
+        else:
+            self.fwhm = fwhm
+        self.phase = phase
+
+        super().__init__(pos, [amp, fwhm, phase], duration, unit, channel)
+
+    def time_func(self, t, **kws):
+        """gaussian_time_func"""
+        amp_, fwhm_, phase_ = kws["amp"], kws["fwhm"], kws["phase"]
+        # start: t = 0, center: t = 0.5 * duration, end: t = duration
+        sigma_ = fwhm_ / np.sqrt(8 * np.log(2))  # fwhm to std. deviation
+        return amp_ * np.exp(
+            -((t - 0.5 * self.duration) ** 2) / (2 * sigma_**2) + 1j * phase_
+        )
+
+    def __call__(
+        self,
+        t: TimeType,
+        shift: Union[float, int] = 0,
+        offset: Union[float, int] = 0,
+        *args,
+        **kwargs,
+    ):
+        args = {"amp": self.amp, "fwhm": self.fwhm, "phase": self.phase}
+        return super().__call__(t, shift, offset, args)
+
+
+class Delay(Instruction):
+    name = "delay"
+
+    def __init__(self, pos: int, duration: int, unit="ns"):
+        if isinstance(duration, int):
+            self.duration = duration
+        else:
+            raise TypeError("duration must be int")
+        super().__init__(pos)
+        self.unit = unit
+        self.symbol = "Delay(%d%s)" % (duration, unit)
+
+    def __repr__(self):
+        return f"{self.__class__.__name__}"
+
+    def to_qasm(self, with_para):
+        return "delay(%d%s) q[%d]" % (self.duration, self.unit, self.pos)
+
+
+class XYResonance(Instruction):
+    name = "XY"
+
+    def __init__(self, qs: int, qe: int, duration: int, unit="ns"):
+        if isinstance(duration, int):
+            self.duration = duration
+        else:
+            raise TypeError("duration must be int")
+        super().__init__(list(range(qs, qe + 1)))
+        self.unit = unit
+        self.symbol = "XY(%d%s)" % (duration, unit)
+
+    def to_qasm(self, with_para):
+        return "xy(%d%s) " % (self.duration, self.unit) + ",".join(
+            ["q[%d]" % p for p in range(min(self.pos), max(self.pos) + 1)]
+        )
+
+
+QuantumPulse.register_pulse(RectPulse)
+QuantumPulse.register_pulse(FlattopPulse)
+QuantumPulse.register_pulse(GaussianPulse)
+Instruction.register_ins(Delay)
+Instruction.register_ins(XYResonance)
```

## quafu/elements/quantum_gate.py

```diff
@@ -1,218 +1,523 @@
-from abc import ABC, abstractmethod
-from typing import List, Union, Iterable, Dict
-
-import numpy as np
-
-from quafu.elements.matrices.mat_utils import reorder_matrix
-from .instruction import Instruction, PosType
-
-
-class QuantumGate(Instruction, ABC):
-    """Base class for standard and combined quantum gates.
-
-    Attributes:
-
-    """
-    gate_classes = {}
-
-    def __init__(self,
-                 pos: PosType,
-                 paras: Union[float, List[float]] = None,
-                 ):
-        super().__init__(pos, paras)
-
-        if paras is not None:
-            if isinstance(paras, Iterable):
-                self.symbol = "%s(" % self.name + ",".join(["%.3f" % para for para in self.paras]) + ")"
-            else:
-                self.symbol = "%s(%.3f)" % (self.name, paras)
-        else:
-            self.symbol = "%s" % self.name
-
-    @property
-    @abstractmethod
-    def matrix(self):
-        raise NotImplementedError("Matrix is not implemented for %s" % self.__class__.__name__ +
-                                  ", this should never happen.")
-
-    @classmethod
-    def register_gate(cls, subclass):
-        assert issubclass(subclass, cls)
-
-        name = subclass.name
-        assert isinstance(name, str)
-
-        if name in cls.gate_classes:
-            raise ValueError(f"Name {name} already exists.")
-        cls.gate_classes[name] = subclass
-        Instruction.register_ins(subclass, name)
-
-    def __str__(self):
-        properties_names = ['pos', 'paras', 'matrix']
-        properties_values = [getattr(self, x) for x in properties_names]
-        return "%s:\n%s" % (self.__class__.__name__, '\n'.join(
-            [f"{x} = {repr(properties_values[i])}" for i, x in enumerate(properties_names)]))
-
-    def __repr__(self):
-        return f"{self.__class__.__name__}"
-
-    def to_qasm(self):
-        qstr = "%s" % self.name.lower()
-
-        if self.paras is not None:
-            if isinstance(self.paras, Iterable):
-                qstr += "(" + ",".join(["%s" % para for para in self.paras]) + ")"
-            else:
-                qstr += "(%s)" % self.paras
-        qstr += " "
-        if isinstance(self.pos, Iterable):
-            qstr += ",".join(["q[%d]" % p for p in self.pos])
-        else:
-            qstr += "q[%d]" % self.pos
-
-        return qstr
-
-
-# Gate types are statically implemented to support type identification
-# and provide shared attributes. However, single/multi qubit may be
-# inferred from ``pos``, while para/fixed type may be inferred by ``paras``.
-# Therefore, these types may be (partly) deprecated in the future.
-
-class SingleQubitGate(QuantumGate, ABC):
-    def __init__(self, pos: int, paras: float = None):
-        QuantumGate.__init__(self, pos=pos, paras=paras)
-
-    def get_targ_matrix(self):
-        return self.matrix
-
-    @property
-    def named_pos(self) -> Dict:
-        return {'pos': self.pos}
-
-
-class MultiQubitGate(QuantumGate, ABC):
-    def __init__(self, pos: List, paras: float = None):
-        QuantumGate.__init__(self, pos, paras)
-
-    def get_targ_matrix(self, reverse_order=False):
-        """
-
-        """
-        targ_matrix = self.matrix
-
-        if reverse_order and (len(self.pos) > 1):
-            qnum = len(self.pos)
-            dim = 2 ** qnum
-            order = np.array(range(len(self.pos))[::-1])
-            order = np.concatenate([order, order + qnum])
-            tensorm = targ_matrix.reshape([2] * 2 * qnum)
-            targ_matrix = np.transpose(tensorm, order).reshape([dim, dim])
-        return targ_matrix
-
-
-class ParametricGate(QuantumGate, ABC):
-    def __init__(self, pos: PosType, paras: Union[float, List[float]]):
-        if paras is None:
-            raise ValueError("`paras` can not be None for ParametricGate")
-        super().__init__(pos, paras)
-
-    @property
-    def named_paras(self) -> Dict:
-        return {'paras': self.paras}
-
-    @property
-    def named_pos(self) -> Dict:
-        return {'pos': self.pos}
-
-
-class FixedGate(QuantumGate, ABC):
-    def __init__(self, pos):
-        super().__init__(pos=pos, paras=None)
-
-    @property
-    def named_paras(self) -> Dict:
-        return {}
-
-
-# class ParaSingleQubitGate(SingleQubitGate, ABC):
-#     def __init__(self, pos, paras: float):
-#         if paras is None:
-#             raise ValueError("`paras` can not be None for ParaSingleQubitGate")
-#         elif isinstance(paras, int):
-#             paras = float(paras)
-#
-#         if not isinstance(paras, float):
-#             raise TypeError(f"`paras` must be float or int for ParaSingleQubitGate, "
-#                             f"instead of {type(paras)}")
-#         super().__init__(pos, paras=paras)
-#
-#     @property
-#     def named_paras(self) -> Dict:
-#         return {'paras': self.paras}
-
-# class FixedMultiQubitGate(MultiQubitGate, ABC):
-#     def __init__(self, pos: List[int]):
-#         super().__init__(pos=pos, paras=None)
-
-
-# class ParaMultiQubitGate(MultiQubitGate, ABC):
-#     def __init__(self, pos, paras):
-#         if paras is None:
-#             raise ValueError("`paras` can not be None for ParaMultiQubitGate")
-#         super().__init__(pos, paras)
-
-
-class ControlledGate(MultiQubitGate, ABC):
-    """ Controlled gate class, where the matrix act non-trivially on target qubits"""
-
-    def __init__(self, targe_name, ctrls: List[int], targs: List[int], paras, tar_matrix):
-        MultiQubitGate.__init__(self, ctrls + targs, paras)
-        self.ctrls = ctrls
-        self.targs = targs
-        self.targ_name = targe_name
-        self._targ_matrix = tar_matrix
-
-        # set matrix
-        # TODO: change matrix according to control-type 0/1
-        c_n, t_n, n = self.ct_nums
-        targ_dim = 2 ** t_n
-        dim = 2 ** n
-        ctrl_dim = dim - targ_dim
-        self._matrix = np.eye(dim, dtype=complex)
-        self._matrix[ctrl_dim:, ctrl_dim:] = tar_matrix
-        self._matrix = reorder_matrix(self._matrix, self.pos)
-
-        if paras is not None:
-            if isinstance(paras, Iterable):
-                self.symbol = "%s(" % self.targ_name + ",".join(["%.3f" % para for para in self.paras]) + ")"
-            else:
-                self.symbol = "%s(%.3f)" % (self.targ_name, paras)
-        else:
-            self.symbol = "%s" % self.targ_name
-
-    @property
-    def matrix(self):
-        # TODO: update matrix when paras of controlled-gate changed
-        return self._matrix
-
-    @property
-    def ct_nums(self):
-        targ_num = len(self.targs)
-        ctrl_num = len(self.ctrls)
-        num = targ_num + ctrl_num
-        return ctrl_num, targ_num, num
-
-    def get_targ_matrix(self, reverse_order=False):
-        targ_matrix = self._targ_matrix
-        if reverse_order and (len(self.targs) > 1):
-            qnum = len(self.targs)
-            order = np.array(range(len(self.targs))[::-1])
-            order = np.concatenate([order, order + qnum])
-            dim = 2 ** qnum
-            tensorm = targ_matrix.reshape([2] * 2 * qnum)
-            targ_matrix = np.transpose(tensorm, order).reshape([dim, dim])
-        return targ_matrix
-
-    @property
-    def named_pos(self) -> Dict:
-        return {'ctrls': self.ctrls, 'targs': self.targs}
+#  (C) Copyright 2023 Beijing Academy of Quantum Information Sciences
+#
+#  Licensed under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License.
+
+
+import copy
+from abc import ABC, abstractmethod
+from typing import Callable, Dict, Iterable, List, Optional, Union
+
+import numpy as np
+from numpy import ndarray
+from quafu.elements.matrices.mat_utils import reorder_matrix
+
+from .instruction import Instruction
+from .parameters import ParameterType
+from .utils import extract_float, handle_expression
+
+__all__ = [
+    "QuantumGate",
+    "ControlledGate",
+    "ControlledU"
+]
+
+HERMITIAN = [
+    "id",
+    "x",
+    "y",
+    "z",
+    "h",
+    "w",
+    "cx",
+    "cz",
+    "cy",
+    "cnot",
+    "swap",
+    "mcx",
+    "mxy",
+    "mcz",
+]
+ROTATION = ["rx", "ry", "rz", "p", "rxx", "ryy", "rzz", "cp"]
+paired = {k: k + "dg" for k in ["sx", "sy", "s", "t", "sw"]}
+PAIRED = {**paired, **{v: k for k, v in paired.items()}}
+
+MatrixType = Union[np.ndarray, Callable]
+
+
+class QuantumGate(Instruction):
+    """Base class for standard and combined quantum gates, namely unitary operation
+    upon quantum states.
+
+    Attributes:
+        pos: Position of this gate in the circuit.
+        paras: Parameters of this gate.
+
+    Properties:
+        symbol: Text symbolic representation of this gate.
+        matrix: Matrix representation of this gate.
+
+    Functions:
+        register_gate: Register a new gate class.
+        to_qasm: Convert this gate to QASM format.
+        update_paras: Update the parameters of this gate.
+
+    """
+
+    gate_classes = {}
+
+    def __init__(
+            self,
+            name: str,
+            pos: List[int],
+            paras: List[ParameterType] = [],
+            matrix: Optional[Union[ndarray, Callable]] = None,
+    ):
+        super().__init__(pos, paras)
+        self._name = name
+        self._symbol = None
+        self._raw_matrix = matrix
+
+    def __str__(self):
+        # only when the gate is a known(named) gate, the matrix is not shown
+        if self.name.lower() in self.gate_classes:
+            properties_names = ["pos", "paras"]
+        else:
+            properties_names = ["pos", "paras", "matrix"]
+        properties_values = [getattr(self, x) for x in properties_names]
+        return "%s:\n%s" % (
+            self.__class__.__name__,
+            "\n".join(
+                [
+                    f"{x} = {repr(properties_values[i])}"
+                    for i, x in enumerate(properties_names)
+                ]
+            ),
+        )
+
+    def __repr__(self):
+        return f"{self.__class__.__name__}"
+
+    @property
+    def name(self):
+        return self._name 
+    
+    @name.setter
+    def name(self, __name):
+        self._name = __name
+    
+    @property
+    def pos(self):
+        return  self._pos
+    
+    @pos.setter
+    def pos(self, __pos):
+        self._pos = copy.deepcopy(__pos)
+
+    @property
+    def named_pos(self) -> Dict:
+        return {"pos": self.pos}
+    
+    @property 
+    def named_paras(self) -> Dict:
+        return {"paras": self.paras}
+    
+    @classmethod
+    def register_gate(cls, subclass, name: str = None):
+        """Register a new gate class into gate_classes.
+
+        This method is used as a decorator.
+        """
+        assert issubclass(subclass, cls)
+
+        name = str(subclass.__name__).lower() if name is None else name
+        assert isinstance(name, str)
+        if name.endswith("gate"):
+            name = name[:-4]
+        if name in cls.gate_classes:
+            raise ValueError(f"Name {name} already exists.")
+        cls.gate_classes[name] = subclass
+        Instruction.register_ins(subclass, name)
+        return subclass
+
+    @classmethod
+    def register(cls, name: str = None):
+        """Decorator for register_gate."""
+
+        def wrapper(subclass):
+            return cls.register_gate(subclass, name)
+
+        return wrapper
+
+    @property
+    def _paras(self):
+        return extract_float(self.paras)
+
+    @property
+    def symbol(self) -> str:
+        """Symbol used in text-drawing."""
+        # TODO: Use latex repr for Parameter
+        if len(self.paras) > 0:
+            symbol = "%s(" %self.name + ",".join(["%.3f" %para for para in self._paras]) + ")"
+            return symbol
+        else:
+            return "%s" %self.name
+
+    @symbol.setter
+    def symbol(self, symbol: str):
+        self._symbol = symbol
+
+    @property
+    def matrix(self):
+        raw_mat = self._raw_matrix
+        if isinstance(self._raw_matrix, Callable):
+            raw_mat = self._raw_matrix(self._paras)
+
+        if len(self.pos) > 1:
+            return reorder_matrix(raw_mat, self.pos)
+        else:
+            return raw_mat
+    
+    def _get_raw_matrix(self, reverse_order=False):
+        raw_mat = self._raw_matrix
+        if isinstance(self._raw_matrix, Callable):
+            raw_mat = self._raw_matrix(self._paras)
+        if reverse_order and len(self.pos) > 1:
+            return reorder_matrix(raw_mat, np.arange(len(self.pos))[::-1])
+        else:
+           return raw_mat
+        
+  
+    def to_qasm(self, with_para=False) -> str:
+        """OPENQASM 2.0"""
+        # TODO: support register naming
+        qstr = "%s" %self.name.lower()
+        if self.paras:
+            if with_para:
+                qstr += "(" + ",".join(["%s" % handle_expression(para) for para in self.paras]) + ")"
+            else:
+                qstr += "(" + ",".join(["%s" % para for para in self._paras]) + ")"
+        qstr += " "
+        qstr += ",".join(["q[%d]" % p for p in self.pos])
+        return qstr
+
+    def update_params(self, paras: Union[ParameterType, List[ParameterType]]):
+        """Update parameters of this gate"""
+        if paras is None:
+            return
+        if isinstance(paras, list):
+            self.paras = paras
+        else:
+            self.paras = [paras] 
+
+    # # # # # # # # # # # # algebraic operations # # # # # # # # # # # #
+    def power(self, n) -> "QuantumGate":
+        """Return another gate equivalent to n-times operation of the present gate."""
+        name = self.name.lower()
+        name = 'sz' if name == 's' else name
+
+        order4 = ["sx", "sy", "s", 'sw']
+        order4 += [_+'dg' for _ in order4]
+        order8 = ["t", "tdg"]
+
+        if name in HERMITIAN:
+            if n % 2 == 0:
+                return self.gate_classes["id"](self.pos)
+            else:
+                return copy.deepcopy(self)
+        elif name in order4:  # ["sx", "sy", "s", "t", "sw"]
+            if n % 4 == 0:
+                return self.gate_classes["id"](self.pos)
+            elif n % 4 == 1:
+                return copy.deepcopy(self)
+            elif n % 4 == 2:
+                _square_name = 'z' if name == 's' else name[1:]
+                return self.gate_classes[_square_name](self.pos)
+            elif n % 4 == 3:
+                _conj_name = PAIRED[name]
+                return self.gate_classes[_conj_name](self.pos)
+        elif name in order8:  # ["t", "tdg"]
+            # note: here we transform a fixed gate into a parametric gate
+            #       which might cause error in future
+            theta = np.pi / 4
+            if name.endswith("dg"):
+                theta = -theta
+            return self.gate_classes["rz"](self.pos, theta * n)
+        elif name in ROTATION:
+            args = self.pos + [self.paras[0] * n]
+            return self.gate_classes[name](*args)
+        else:
+            name = self.name + "^%d" %n
+            raw_matrix = self._raw_matrix 
+            if isinstance(self._raw_matrix, Callable):
+                raw_matrix = lambda paras: np.linalg.matrix_power(self._raw_matrix(paras), n)
+            else:
+                raw_matrix = np.linalg.matrix_power(self._raw_matrix, n)
+            return QuantumGate(name, self.pos, self.paras, raw_matrix)
+
+    def dagger(self) -> "QuantumGate":
+        """Return the hermitian conjugate gate with same the position."""
+        name = self.name
+        if name in HERMITIAN:  # Hermitian gate
+            return copy.deepcopy(self)
+        if name in ROTATION:  # rotation gate
+            args = self.pos + [-self.paras[0]]
+            return self.gate_classes[name](*args)
+        elif name in PAIRED:  # pairwise-occurrence gate
+            _conj_name = PAIRED[name]
+            return self.gate_classes[_conj_name](self.pos)
+        else:
+            name = self.name + "^†"
+            raw_matrix = self._raw_matrix 
+            if isinstance(self._raw_matrix, Callable):
+                raw_matrix = lambda paras: self._raw_matrix(paras).conj().T
+            else:
+                raw_matrix = raw_matrix.conj().T
+            return QuantumGate(name, self.pos, self.paras, raw_matrix)
+
+    def ctrl_by(self, ctrls: Union[int, List[int]]) -> "ControlledGate":
+        """Return a controlled gate with present gate as the controlled target."""
+        ctrls = [ctrls] if not isinstance(ctrls, list) else ctrls
+        pos = [self.pos] if not isinstance(self.pos, list) else self.pos
+        name = self.name.lower()
+
+        if isinstance(self, ControlledGate):
+            """
+            [m1]control-([m2]control-U) = [m1+m2]control-U
+            """
+            if self.ctrls == ctrls:
+                raise ValueError("Can't not add the same control qubit.")
+            ctrls = list(set(self.ctrls) | set(ctrls))
+        elif set(ctrls) & set(pos):
+            raise ValueError("Control qubits should not be overlap with target qubits.")
+        
+        #named controlled gate
+        args = self.pos + self.paras
+        if self.name in ["X" ,"Y" ,"Z", "RX", "RY", "RZ"]: 
+            args = self.pos + self.paras
+            if len(ctrls) == 1:  # single-ctrl gate
+                cname = "c" + name
+                cop = QuantumGate.gate_classes[cname](ctrls[0], *args)
+                return cop
+            else:
+                cname = "mc" + name
+                cop = QuantumGate.gate_classes[cname](ctrls, *args)
+                return cop
+        elif self.name in ["CX" ,"CY" ,"CZ", "CRX", "CRY", "CRZ"]:
+            args=  self.targs + self.paras
+            cname = "m" + name
+            cop = QuantumGate.gate_classes[cname](ctrls, *args)
+            return cop
+        else: #unnamed controlled gate
+            if isinstance(self, ControlledGate):
+                cop = ControlledGate("MC"+self._targ_name, self._targ_name, ctrls+self.ctrls, self.targs, self.paras, self._targ_matrix)
+                return cop
+            else:
+                if len(ctrls) == 1:
+                    return ControlledU("MC"+name, ctrls, self)
+                else:
+                    return ControlledU("MC"+name, ctrls, self)
+
+
+class ControlledGate(QuantumGate):
+    """Controlled gate class, where the matrix act non-trivially on target qubits"""
+
+    def __init__(
+            self,
+            name: str,
+            targ_name: str,
+            ctrls: List[int],
+            targs: List[int],
+            paras: List[float] = [],
+            targ_matrix: MatrixType = None,
+    ):
+        self.ctrls = copy.deepcopy(ctrls)
+        self.targs = copy.deepcopy(targs)
+        self._targ_name = targ_name
+        super().__init__(name, ctrls+targs, paras, targ_matrix)
+        self._targ_matrix = targ_matrix
+        self._raw_matrix = self._rawmatfunc
+
+    @property
+    def symbol(self):
+        if len(self.paras) > 0:
+            symbol = "%s(" %self._targ_name + ",".join(["%.3f" %para for para in self._paras]) + ")"
+            return symbol
+        else:
+            return "%s" %self._targ_name
+        
+   
+    def _rawmatfunc(self, paras:List[float]):
+        targ_dim = 2**(len(self.targs))
+        qnum = len(self.pos)
+        dim = 2**(qnum)
+        raw_matrix =  np.zeros((dim , dim), dtype=complex)
+        targ_matrix = self._targ_matrix
+        if isinstance(self._targ_matrix, Callable):
+            targ_matrix = self._targ_matrix(paras)
+
+        if targ_matrix.shape[0] != targ_dim:
+            raise ValueError("Dimension dismatch")
+        else:
+            control_dim = 2**len(self.pos) - targ_dim
+            for i in range(control_dim):
+                raw_matrix[i, i] = 1.
+            
+            raw_matrix[control_dim:, control_dim:] = targ_matrix
+
+        return raw_matrix
+    
+    def power(self, n) -> "ControlledGate":
+        #TODO:Use implementation in QuantumGate via Controlled
+        name = self.name
+        if self._targ_name in ["RX", "RY", "RZ", "P", "RZZ", "RXX", "RYY"]:
+            return ControlledGate(name, self._targ_name, self.ctrls, self.targs, [self.paras[0] * n], self._targ_matrix)
+        else:
+            name = self.name + "^%d" %n
+            targ_matrix = self._targ_matrix 
+            if isinstance(self._targ_matrix, Callable):
+                targ_matrix = lambda paras: np.linalg.matrix_power(self._targ_matrix(paras), n)
+            else:
+                targ_matrix = np.linalg.matrix_power(self._targ_matrix, n)
+            return ControlledGate(name, self._targ_name+"^%d" %n, self.ctrls, self.targs, self.paras, targ_matrix)
+    
+        
+    def dagger(self) -> "ControlledGate":
+        #TODO:Use implementation in QuantumGate via ControlledU
+        name = self.name
+        if self._targ_name in ["RX", "RY", "RZ", "P", "RZZ", "RXX", "RYY"]:
+            return ControlledGate(name, self._targ_name, self.ctrls, self.targs, [-self.paras[0]], self._targ_matrix)
+        else:
+            name = self.name + "^†"
+            targ_matrix = self._targ_matrix 
+            if isinstance(self._targ_matrix, Callable):
+                targ_matrix = lambda paras: self._targ_matrix(paras).conj().T
+            else:
+                targ_matrix = targ_matrix.conj().T
+
+            return ControlledGate(name, self._targ_name+"^†", self.ctrls, self.targs, self.paras, targ_matrix)
+    
+
+    @property
+    def symbol(self):
+        if len(self.paras) > 0:
+            symbol = "%s(" %self._targ_name + ",".join(["%.3f" %para for para in self._paras]) + ")"
+            return symbol
+        else:
+            return "%s" %self._targ_name
+
+    @property
+    def ct_nums(self):
+        targ_num = len(self.targs)
+        ctrl_num = len(self.ctrls)
+        num = targ_num + ctrl_num
+        return ctrl_num, targ_num, num
+        
+    def _get_targ_matrix(self, reverse_order=False):
+        targ_mat = self._targ_matrix
+        if isinstance(self._targ_matrix, Callable):
+            targ_mat = self._targ_matrix(self._paras)
+        if reverse_order and (len(self.targs) > 1): 
+            return reorder_matrix(targ_mat, np.array(range(len(self.targs))[::-1]))
+        else:
+            return targ_mat
+    
+
+    @property
+    def named_pos(self) -> Dict:
+        return {"ctrls": self.ctrls, "targs": self.targs}
+
+    @property
+    def named_paras(self) -> Dict:
+        return {"paras": self.paras}
+
+    @classmethod
+    def from_target(cls, targ: QuantumGate, ctrls: List[int]):
+        """Shoud use controlledU"""
+        return cls(targ.name, ctrls, targ.pos, targ.paras, targ._raw_matrix)
+
+class ControlledU(ControlledGate):
+    def __init__(self, name, ctrls: List[int], U: QuantumGate):
+        self.targ_gate = U
+        targs = U.pos
+        super().__init__(name, U.name, ctrls, targs, U.paras, targ_matrix=self.targ_gate._raw_matrix)
+
+class CircuitWrapper(QuantumGate):
+    def __init__(self, name:str, circ, qbits=[]):
+        self.name  = name
+        self.pos = list(range(circ.num))
+        self.circuit = copy.deepcopy(circ)
+
+        
+        if qbits:
+            self._reallocate(qbits)
+    
+    def _reallocate(self, qbits):
+        num = max(self.circuit.num-1, max(qbits))+1
+        self.pos = qbits
+        self.circuit._reallocate(num, qbits)
+    
+    @property
+    def symbol(self):
+        return "%s" %self.name
+
+    def add_controls(self, ctrls:List[int]=[]) -> QuantumGate:
+        return ControlledCircuitWrapper("MC"+self.name, self, ctrls)
+
+    def power(self, n:int):
+        self.name +="^%d" %n
+        self.circuit = self.circuit.power(n)
+        return self
+
+    def dagger(self):
+        self.name += "^†"
+        self.circuit = self.circuit.dagger()
+        return self
+
+    def to_qasm(self, with_para=False):
+        qasm = ''
+        for operation in self.circuit.operations:
+            qasm += operation.to_qasm(with_para) + ";\n"
+        return qasm
+    
+class ControlledCircuitWrapper(CircuitWrapper):
+    def __init__(self, name:str, circwrp:CircuitWrapper, ctrls:List[int]):
+        self.name = name
+        self.ctrls = ctrls
+        self.targs = circwrp.pos
+        self.circuit = circwrp.circuit.add_controls(len(ctrls), ctrls, self.targs)
+        self.pos = list(range(self.circuit.num))
+        self._targ_name = circwrp.name
+
+    
+    @property
+    def symbol(self):
+        return "%s" %self._targ_name
+
+    def power(self, n: int):
+        self._targ_name += "^%d" %n
+        return super().power(n)
+
+    def dagger(self):
+        self.name += "^†"
+        return super().dagger()
+    
+    def _reallocate(self, qbits):
+        num = max(self.circuit.num-1, max(qbits))+1
+        self.pos = qbits
+        self.circuit._reallocate(num, qbits)
+        qbits_map = dict(zip(range(len(qbits)), qbits))
+        for i in range(len(self.ctrls)):
+            self.ctrls[i] = qbits_map[self.ctrls[i]]
+        
+        for i in range(len(self.targs)):
+            self.targs[i] = qbits_map[self.targs[i]]
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## quafu/elements/element_gates/__init__.py

```diff
@@ -1,18 +1,42 @@
-from .pauli import XGate, YGate, ZGate, IdGate, WGate, SWGate, SXGate, SXdgGate, SYGate, SYdgGate
-from .clifford import HGate, SGate, SdgGate, TGate, TdgGate
-from .phase import PhaseGate
-from .rotation import RXGate, RYGate, RZGate, RXXGate, RYYGate, RZZGate
-from .swap import SwapGate, ISwapGate
-from .c11 import CXGate, CYGate, CZGate, CSGate, CTGate, CPGate
-from .c12 import FredkinGate
-from .cm1 import MCXGate, MCYGate, MCZGate, ToffoliGate
-from .unitary import UnitaryDecomposer
-
-__all__ = ['XGate', 'YGate', 'ZGate', 'IdGate', 'WGate', 'SWGate', 'SXGate', 'SXdgGate', 'SYGate', 'SYdgGate',
-           'PhaseGate',
-           'HGate', 'SGate', 'SdgGate', 'TGate', 'TdgGate',
-           'RXGate', 'RYGate', 'RZGate', 'RXXGate', 'RYYGate', 'RZZGate',
-           'SwapGate', 'ISwapGate', 'FredkinGate',
-           'CXGate', 'CYGate', 'CZGate', 'CSGate', 'CTGate', 'CPGate',
-           'MCXGate', 'MCYGate', 'MCZGate', 'ToffoliGate',
-           'UnitaryDecomposer']
+# from .element_gates import XGate, YGate, ZGate, IdGate, WGate, HGate, SGate, SdgGate, TGate, TdgGate, SXGate, SXdgGate, SYGate, SYdgGate, SWGate, SWdgGate, RXGate, RYGate, RZGate, RXXGate, RYYGate, RZZGate, SwapGate, ISwapGate, CXGate, CYGate, CZGate, CSGate, CTGate, CPGate, ToffoliGate, FredkinGate, MCXGate, MCYGate, MCZGate
+# from .element_gates import PhaseGate
+from .element_gates import *
+
+# __all__ = [
+#     "XGate",
+#     "YGate",
+#     "ZGate",
+#     "IdGate",
+#     "WGate",
+#     "HGate",
+#     "SGate",
+#     "SdgGate",
+#     "TGate",
+#     "TdgGate",
+#     "SXGate",
+#     "SXdgGate",
+#     "SYGate",
+#     "SYdgGate",
+#     "SWGate",
+#     "SWdgGate",
+#     "RXGate",
+#     "RYGate",
+#     "RZGate",
+#     "PhaseGate"
+#     "RXXGate",
+#     "RYYGate",
+#     "RZZGate",
+#     "SwapGate",
+#     "ISwapGate",
+#     "CXGate",
+#     "CYGate",
+#     "CZGate",
+#     "CSGate",
+#     "CTGate",
+#     "CPGate",
+#     "ToffoliGate",
+#     "FredkinGate",
+#     "MCXGate",
+#     "MCYGate",
+#     "MCZGate",
+# ]
```

## quafu/elements/element_gates/clifford.py

```diff
@@ -1,54 +1,5 @@
-import numpy as np
-
-from quafu.elements.matrices import HMatrix, SMatrix
-from ..quantum_gate import SingleQubitGate, FixedGate
-
-__all__ = ['HGate', 'SGate', 'SdgGate', 'TGate', 'TdgGate']
-
-
-class HGate(SingleQubitGate, FixedGate):
-    name = "H"
-    matrix = HMatrix
-
-    def __init__(self, pos: int):
-        FixedGate.__init__(self, pos)
-
-
-class SGate(SingleQubitGate, FixedGate):
-    name = "S"
-    matrix = SMatrix
-
-    def __init__(self, pos: int):
-        FixedGate.__init__(self, pos)
-
-
-class SdgGate(SingleQubitGate, FixedGate):
-    name = "Sdg"
-    matrix = SMatrix.conj().T
-
-    def __init__(self, pos: int):
-        FixedGate.__init__(self, pos)
-
-
-class TGate(SingleQubitGate, FixedGate):
-    name = "T"
-    matrix = np.array([[1., 0.],
-                       [0., np.exp(1.j * np.pi / 4)]], dtype=complex)
-
-    def __init__(self, pos: int):
-        FixedGate.__init__(self, pos)
-
-
-class TdgGate(SingleQubitGate, FixedGate):
-    name = "Tdg"
-    matrix = TGate.matrix.conj().T
-
-    def __init__(self, pos: int):
-        FixedGate.__init__(self, pos)
-
-
-FixedGate.register_gate(HGate)
-FixedGate.register_gate(SGate)
-FixedGate.register_gate(SdgGate)
-FixedGate.register_gate(TGate)
-FixedGate.register_gate(TdgGate)
+from .element_gates import HGate, SGate, CXGate
+
+__all__ = ['HGate', 'SGate', 'CXGate']
+
+
```

## quafu/elements/element_gates/pauli.py

```diff
@@ -1,120 +1,3 @@
-import numpy as np
-
-from quafu.elements.matrices import XMatrix, YMatrix, ZMatrix, WMatrix, SWMatrix
-from quafu.elements.quantum_gate import FixedGate, SingleQubitGate
-
-__all__ = ['IdGate', 'XGate', 'YGate', 'ZGate',
-           'WGate', 'SWGate',
-           'SXGate', 'SYGate', 'SXdgGate', 'SYdgGate']
-
-
-class IdGate(FixedGate, SingleQubitGate):
-    name = "Id"
-    matrix = XMatrix
-
-    def __init__(self, pos: int):
-        FixedGate.__init__(self, pos)
-
-
-class XGate(FixedGate, SingleQubitGate):
-    name = "X"
-    matrix = XMatrix
-
-    def __init__(self, pos: int):
-        FixedGate.__init__(self, pos)
-
-
-class YGate(FixedGate, SingleQubitGate):
-    name = "Y"
-    matrix = YMatrix
-
-    def __init__(self, pos: int):
-        FixedGate.__init__(self, pos)
-
-
-class ZGate(FixedGate, SingleQubitGate):
-    name = "Z"
-    matrix = ZMatrix
-
-    def __init__(self, pos: int):
-        FixedGate.__init__(self, pos)
-
-
-class WGate(FixedGate, SingleQubitGate):
-    """ (X+Y)/sqrt(2) """
-    name = "W"
-    matrix = WMatrix
-
-    def __init__(self, pos: int):
-        FixedGate.__init__(self, pos)
-        self.symbol = "W"
-
-    def to_qasm(self):
-        return "rz(-pi/4) q[%d];\nrx(pi) q[%d];\nrz(pi/4) q[%d]" % (self.pos, self.pos, self.pos)
-
-
-class SWGate(FixedGate, SingleQubitGate):
-    name = "SW"
-    matrix = SWMatrix
-
-    def __init__(self, pos: int):
-        FixedGate.__init__(self, pos)
-        self.symbol = "√W"
-
-    def to_qasm(self):
-        return "rz(-pi/4) q[%d];\nrx(pi/2) q[%d];\nrz(pi/4) q[%d]" % (self.pos, self.pos, self.pos)
-
-
-class SXGate(FixedGate, SingleQubitGate):
-    name = "SX"
-    matrix = np.array([[0.5 + 0.5j, 0.5 - 0.5j],
-                       [0.5 - 0.5j, 0.5 + 0.5j]], dtype=complex)
-
-    def __init__(self, pos: int):
-        FixedGate.__init__(self, pos)
-
-
-class SXdgGate(FixedGate, SingleQubitGate):
-    name = "SXdg"
-    matrix = SXGate.matrix.conj().T
-
-    def __init__(self, pos: int):
-        FixedGate.__init__(self, pos)
-        self.symbol = "√X"
-
-
-class SYGate(FixedGate, SingleQubitGate):
-    name = "SY"
-    matrix = np.array([[0.5 + 0.5j, -0.5 - 0.5j],
-                       [0.5 + 0.5j, 0.5 + 0.5j]], dtype=complex)
-
-    def __init__(self, pos: int):
-        FixedGate.__init__(self, pos)
-        self.symbol = "√Y"
-
-    def to_qasm(self):
-        return "ry(pi/2) q[%d];" % self.pos
-
-
-class SYdgGate(FixedGate, SingleQubitGate):
-    name = "SYdg"
-    matrix = SYGate.matrix.conj().T
-
-    def __init__(self, pos: int):
-        FixedGate.__init__(self, pos)
-        self.symbol = "√Y†"
-
-    def to_qasm(self):
-        return "ry(-pi/2) q[%d]" % self.pos
-
-
-SingleQubitGate.register_gate(IdGate)
-SingleQubitGate.register_gate(XGate)
-SingleQubitGate.register_gate(YGate)
-SingleQubitGate.register_gate(ZGate)
-SingleQubitGate.register_gate(WGate)
-SingleQubitGate.register_gate(SWGate)
-SingleQubitGate.register_gate(SXGate)
-SingleQubitGate.register_gate(SXdgGate)
-SingleQubitGate.register_gate(SYGate)
-SingleQubitGate.register_gate(SYdgGate)
+from .element_gates import XGate, YGate, ZGate, IdGate
+
+__all__ = ['IdGate', 'XGate', 'YGate', 'ZGate']  # hint: "SZ" gate is S contained in Clifford gates
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## quafu/elements/element_gates/rotation.py

```diff
@@ -1,92 +1,3 @@
-from typing import Dict
-
-from quafu.elements.matrices import rx_mat, ry_mat, rz_mat, rxx_mat, ryy_mat, rzz_mat
-from ..quantum_gate import QuantumGate, SingleQubitGate, ParametricGate
-
-__all__ = ['RXGate', 'RYGate', 'RZGate', 'RXXGate', 'RYYGate', 'RZZGate']
-
-
-class RXGate(ParametricGate, SingleQubitGate):
-    name = "RX"
-    
-    def __init__(self, pos: int, theta: float = 0.):
-        ParametricGate.__init__(self, pos, paras=theta)
-
-    @property
-    def matrix(self):
-        return rx_mat(self.paras)
-
-
-class RYGate(ParametricGate, SingleQubitGate):
-    name = "RY"
-    
-    def __init__(self, pos: int, theta: float = 0.):
-        ParametricGate.__init__(self, pos, paras=theta)
-
-    @property
-    def matrix(self):
-        return ry_mat(self.paras)
-
-
-class RZGate(ParametricGate, SingleQubitGate):
-    name = "RZ"
-    
-    def __init__(self, pos: int, theta: float = 0.):
-        ParametricGate.__init__(self, pos, paras=theta)
-        
-    @property
-    def matrix(self):
-        return rz_mat(self.paras)
-
-
-class RXXGate(ParametricGate):
-    name = "RXX"
-
-    def __init__(self, q1: int, q2: int, theta: float = 0.):
-        ParametricGate.__init__(self, [q1, q2], paras=theta)
-
-    @property
-    def matrix(self):
-        return rxx_mat(self.paras)
-    
-    @property
-    def named_pos(self) -> Dict:
-        return {'pos': self.pos}
-
-
-class RYYGate(ParametricGate):
-    name = "RYY"
-
-    def __init__(self, q1: int, q2: int, theta: float = 0.):
-        ParametricGate.__init__(self, [q1, q2], paras=theta)
-
-    @property
-    def matrix(self):
-        return ryy_mat(self.paras)
-
-    @property
-    def named_pos(self) -> Dict:
-        return {'pos': self.pos}
-
-
-class RZZGate(ParametricGate):
-    name = "RZZ"
-
-    def __init__(self, q1: int, q2: int, theta: float = 0.):
-        ParametricGate.__init__(self, [q1, q2], paras=theta)
-
-    @property
-    def matrix(self):
-        return rzz_mat(self.paras)
-
-    @property
-    def named_pos(self) -> Dict:
-        return {'pos': self.pos}
-
-
-QuantumGate.register_gate(RXGate)
-QuantumGate.register_gate(RYGate)
-QuantumGate.register_gate(RZGate)
-QuantumGate.register_gate(RXXGate)
-QuantumGate.register_gate(RYYGate)
-QuantumGate.register_gate(RZZGate)
+from .element_gates import RXGate, RYGate, RZGate,RXXGate, RYYGate, RZZGate, PhaseGate, CRXGate, CRYGate, CRZGate
+
+
```

## quafu/elements/matrices/__init__.py

```diff
@@ -1,2 +1,2 @@
-from .mat_lib import *
-from .mat_utils import stack_matrices, is_zero, is_hermitian
+from .mat_lib import *
+from .mat_utils import is_hermitian, is_zero, stack_matrices
```

## quafu/elements/matrices/mat_lib.py

```diff
@@ -1,132 +1,207 @@
-import numpy as np
-
-"""
-Matrices library for quantum gates.
-"""
-
-IdMatrix = np.eye(2, dtype=complex)
-XMatrix = np.array([[0., 1.], [1., 0.]], dtype=complex)
-YMatrix = np.array([[0., -1.j], [1.j, 0.]], dtype=complex)
-ZMatrix = np.array([[1., 0.], [0., -1.]], dtype=complex)
-SMatrix = np.array([[1., 0.], [0., 1.j]], dtype=complex)
-SXMatrix = np.array([[1., 1.j], [1.j, 1.]], dtype=complex) / np.sqrt(2)
-SYMatrix = np.array([[1., -1.], [1., 1.]], dtype=complex) / np.sqrt(2)
-TMatrix = np.array([[1., 0.], [0., np.exp(1.j * np.pi / 4)]], dtype=complex)
-WMatrix = (XMatrix + YMatrix) / np.sqrt(2)
-SWMatrix = np.array([[0.5 + 0.5j, -np.sqrt(0.5) * 1j],
-                     [np.sqrt(0.5), 0.5 + 0.5j]], dtype=complex)
-HMatrix = (XMatrix + ZMatrix) / np.sqrt(2)
-SwapMatrix = np.array([[1., 0., 0., 0.],
-                       [0., 0., 1., 0.],
-                       [0., 1., 0., 0.],
-                       [0., 0., 0., 1.]], dtype=complex)
-ISwapMatrix = np.array([[1., 0., 0., 0.],
-                        [0., 0., 1.j, 0.],
-                        [0., 1.j, 0., 0.],
-                        [0., 0., 0., 1.]], dtype=complex)
-CXMatrix = np.array([[1., 0., 0., 0.],
-                     [0., 1., 0., 0.],
-                     [0., 0., 0., 1.],
-                     [0., 0., 1., 0.]], dtype=complex)
-CYMatrix = np.array([[1., 0., 0., 0.],
-                     [0., 1., 0., 0.],
-                     [0., 0., 0., -1.j],
-                     [0., 0., 1.j, 0.]], dtype=complex)
-CZMatrix = np.array([[1., 0., 0., 0.],
-                     [0., 1., 0., 0.],
-                     [0., 0., 1., 0.],
-                     [0., 0., 0., -1.]], dtype=complex)
-ToffoliMatrix = np.array([[1., 0., 0., 0., 0., 0., 0., 0.],
-                          [0., 1., 0., 0., 0., 0., 0., 0.],
-                          [0., 0., 1., 0., 0., 0., 0., 0.],
-                          [0., 0., 0., 1., 0., 0., 0., 0.],
-                          [0., 0., 0., 0., 1., 0., 0., 0.],
-                          [0., 0., 0., 0., 0., 1., 0., 0.],
-                          [0., 0., 0., 0., 0., 0., 0., 1.],
-                          [0., 0., 0., 0., 0., 0., 1., 0.]], dtype=complex)
-FredkinMatrix = np.array([[1., 0., 0., 0., 0., 0., 0., 0.],
-                          [0., 1., 0., 0., 0., 0., 0., 0.],
-                          [0., 0., 1., 0., 0., 0., 0., 0.],
-                          [0., 0., 0., 1., 0., 0., 0., 0.],
-                          [0., 0., 0., 0., 1., 0., 0., 0.],
-                          [0., 0., 0., 0., 0., 0., 1., 0.],
-                          [0., 0., 0., 0., 0., 1., 0., 0.],
-                          [0., 0., 0., 0., 0., 0., 0., 1.]], dtype=complex)
-
-
-def u2matrix(_phi=0., _lambda=0.):
-    """OpenQASM 3.0 specification"""
-    return np.array([[1., np.exp(-1.j * _lambda)],
-                     [np.exp(1.j * _phi), np.exp((_phi + _lambda) * 1.j)]], dtype=complex)
-
-
-def u3matrix(_theta=0., _phi=0., _lambda=0.):
-    """OpenQASM 3.0 specification"""
-    return np.array([[np.cos(0.5 * _theta), -np.exp(_lambda * 1.j) * np.sin(0.5 * _theta)],
-                     [np.exp(_phi * 1.j) * np.sin(0.5 * _theta),
-                      np.exp((_phi + _lambda) * 1.j) * np.cos(0.5 * _theta)]], dtype=complex)
-
-
-def rx_mat(theta):
-    return np.array([[np.cos(0.5 * theta), -1.j * np.sin(0.5 * theta)],
-                     [-1.j * np.sin(0.5 * theta), np.cos(0.5 * theta)]], dtype=complex)
-
-
-def ry_mat(theta):
-    return np.array([[np.cos(0.5 * theta), - np.sin(0.5 * theta)],
-                     [np.sin(0.5 * theta), np.cos(0.5 * theta)]], dtype=complex)
-
-
-def rz_mat(theta):
-    return np.array([[np.exp(-0.5j * theta), 0.],
-                     [0., np.exp(0.5j * theta)]], dtype=complex)
-
-
-def pmatrix(labda):
-    return np.array([[1, 0],
-                     [0, np.exp(1j * labda)]], dtype=complex)
-
-
-def rxx_mat(theta):
-    """Unitary evolution of XX interaction"""
-    return np.array([[np.cos(theta / 2), 0, 0, -1j * np.sin(theta / 2)],
-                     [0, np.cos(theta / 2), -1j * np.sin(theta / 2), 0],
-                     [0, -1j * np.sin(theta / 2), np.cos(theta / 2), 0],
-                     [-1j * np.sin(theta / 2), 0, 0, np.cos(theta / 2)]
-                     ])
-
-
-def ryy_mat(theta):
-    """ Unitary evolution of YY interaction"""
-    c = np.cos(theta / 2)
-    s = 1j * np.sin(theta / 2)
-    return np.array([[c, 0, 0, +s],
-                     [0, c, -s, 0],
-                     [0, -s, c, 0],
-                     [+s, 0, 0, c]
-                     ])
-
-
-def rzz_mat(theta):
-    return np.array([[np.exp(-1j * theta / 2), 0, 0, 0],
-                     [0, np.exp(1j * theta / 2), 0, 0],
-                     [0, 0, np.exp(1j * theta / 2), 0],
-                     [0, 0, 0, np.exp(-1j * theta / 2)]
-                     ])
-
-# def su2_matrix(gamma: float, beta: float, delta: float):
-#     """
-#     SU = Rz(beta)Ry(gamma)Rz(delta).
-#
-#     Symbol convention is the same as in the textbook
-#     of Chuang and Nielsen.
-#     """
-#     s, c = np.sin(gamma / 2), np.cos(gamma / 2)
-#     alpha1, alpha2 = (delta + beta) / 2, (delta - beta) / 2
-#     su2_mat = np.array([[np.exp(-1.j * alpha1) * c, -np.exp(-1.j * alpha2) * s],
-#                         [np.exp(1.j * alpha2) * s, np.exp(1.j * alpha1) * c]])
-#     return su2_mat
-#
-#
-# def u2_matrix(alpha: float, gamma: float, beta: float, delta: float):
-#     return np.exp(1.j * alpha) * su2_matrix(gamma, beta, delta)
+import numpy as np
+
+IdMatrix = np.eye(2, dtype=complex)
+XMatrix = np.array(
+    [[0.0, 1.0],
+     [1.0, 0.0]], dtype=complex)
+YMatrix = np.array(
+    [[0.0, -1.0j],
+     [1.0j, 0.0]], dtype=complex)
+ZMatrix = np.array(
+    [[1.0, 0.0],
+     [0.0, -1.0]], dtype=complex)
+SMatrix = np.array(
+    [[1.0, 0.0],
+     [0.0, 1.0j]], dtype=complex)
+SXMatrix = np.array(
+    [[1.0, 1.0j],
+     [1.0j, 1.0]], dtype=complex) / np.sqrt(2)
+SYMatrix = np.array(
+    [[1.0, -1.0],
+     [1.0, 1.0]], dtype=complex) / np.sqrt(2)
+TMatrix = np.array(
+    [[1.0, 0.0],
+     [0.0, np.exp(1.0j * np.pi / 4)]], dtype=complex)
+WMatrix = (XMatrix + YMatrix) / np.sqrt(2)
+SWMatrix = np.array(
+    [[0.5 + 0.5j, -np.sqrt(0.5) * 1j],
+     [np.sqrt(0.5), 0.5 + 0.5j]], dtype=complex)
+HMatrix = (XMatrix + ZMatrix) / np.sqrt(2)
+SwapMatrix = np.array(
+    [
+        [1.0, 0.0, 0.0, 0.0],
+        [0.0, 0.0, 1.0, 0.0],
+        [0.0, 1.0, 0.0, 0.0],
+        [0.0, 0.0, 0.0, 1.0],
+    ],
+    dtype=complex,
+)
+ISwapMatrix = np.array(
+    [
+        [1.0, 0.0, 0.0, 0.0],
+        [0.0, 0.0, 1.0j, 0.0],
+        [0.0, 1.0j, 0.0, 0.0],
+        [0.0, 0.0, 0.0, 1.0],
+    ],
+    dtype=complex,
+)
+CXMatrix = np.array(
+    [
+        [1.0, 0.0, 0.0, 0.0],
+        [0.0, 1.0, 0.0, 0.0],
+        [0.0, 0.0, 0.0, 1.0],
+        [0.0, 0.0, 1.0, 0.0],
+    ],
+    dtype=complex,
+)
+CYMatrix = np.array(
+    [
+        [1.0, 0.0, 0.0, 0.0],
+        [0.0, 1.0, 0.0, 0.0],
+        [0.0, 0.0, 0.0, -1.0j],
+        [0.0, 0.0, 1.0j, 0.0],
+    ],
+    dtype=complex,
+)
+CZMatrix = np.array(
+    [
+        [1.0, 0.0, 0.0, 0.0],
+        [0.0, 1.0, 0.0, 0.0],
+        [0.0, 0.0, 1.0, 0.0],
+        [0.0, 0.0, 0.0, -1.0],
+    ],
+    dtype=complex,
+)
+
+CTMatrix = np.asarray(
+    [
+        [1.0, 0.0, 0.0, 0.0],
+        [0.0, 1.0, 0.0, 0.0],
+        [0.0, 0.0, 1.0, 0.0],
+        [0.0, 0.0, 0.0, np.exp(1.0j * np.pi / 4)],
+    ],
+    dtype=complex,
+)
+
+ToffoliMatrix = np.array(
+    [
+        [1.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
+        [0.0, 1.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
+        [0.0, 0.0, 1.0, 0.0, 0.0, 0.0, 0.0, 0.0],
+        [0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0, 0.0],
+        [0.0, 0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0],
+        [0.0, 0.0, 0.0, 0.0, 0.0, 1.0, 0.0, 0.0],
+        [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 1.0],
+        [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 1.0, 0.0],
+    ],
+    dtype=complex,
+)
+FredkinMatrix = np.array(
+    [
+        [1.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
+        [0.0, 1.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
+        [0.0, 0.0, 1.0, 0.0, 0.0, 0.0, 0.0, 0.0],
+        [0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0, 0.0],
+        [0.0, 0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0],
+        [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 1.0, 0.0],
+        [0.0, 0.0, 0.0, 0.0, 0.0, 1.0, 0.0, 0.0],
+        [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 1.0],
+    ],
+    dtype=complex,
+)
+
+
+def rx_mat(theta):
+    return np.array(
+        [
+            [np.cos(0.5 * theta), -1.0j * np.sin(0.5 * theta)],
+            [-1.0j * np.sin(0.5 * theta), np.cos(0.5 * theta)],
+        ],
+        dtype=complex,
+    )
+
+
+def ry_mat(theta):
+    return np.array(
+        [
+            [np.cos(0.5 * theta), -np.sin(0.5 * theta)],
+            [np.sin(0.5 * theta), np.cos(0.5 * theta)],
+        ],
+        dtype=complex,
+    )
+
+
+def rz_mat(theta):
+    return np.array(
+        [[np.exp(-0.5j * theta), 0.0], [0.0, np.exp(0.5j * theta)]], dtype=complex
+    )
+
+
+def pmatrix(labda):
+    return np.array([[1, 0], [0, np.exp(1j * labda)]], dtype=complex)
+
+
+def rxx_mat(theta):
+    """Unitary evolution of XX interaction"""
+    return np.array(
+        [
+            [np.cos(theta / 2), 0, 0, -1j * np.sin(theta / 2)],
+            [0, np.cos(theta / 2), -1j * np.sin(theta / 2), 0],
+            [0, -1j * np.sin(theta / 2), np.cos(theta / 2), 0],
+            [-1j * np.sin(theta / 2), 0, 0, np.cos(theta / 2)],
+        ]
+    )
+
+
+def ryy_mat(theta):
+    """Unitary evolution of YY interaction"""
+    c = np.cos(theta / 2)
+    s = 1j * np.sin(theta / 2)
+    return np.array([[c, 0, 0, +s], [0, c, -s, 0], [0, -s, c, 0], [+s, 0, 0, c]])
+
+
+def rzz_mat(theta):
+    return np.array(
+        [
+            [np.exp(-1j * theta / 2), 0, 0, 0],
+            [0, np.exp(1j * theta / 2), 0, 0],
+            [0, 0, np.exp(1j * theta / 2), 0],
+            [0, 0, 0, np.exp(-1j * theta / 2)],
+        ]
+    )
+
+
+def u2matrix(_phi=0.0, _lambda=0.0):
+    """OpenQASM 3.0 specification"""
+    return np.array(
+        [
+            [1.0, np.exp(-1.0j * _lambda)],
+            [np.exp(1.0j * _phi), np.exp((_phi + _lambda) * 1.0j)],
+        ],
+        dtype=complex,
+    )
+
+
+def u3matrix(_theta=0.0, _phi=0.0, _lambda=0.0):
+    """OpenQASM 3.0 specification"""
+    return np.array(
+        [
+            [np.cos(0.5 * _theta), -np.exp(_lambda * 1.0j) * np.sin(0.5 * _theta)],
+            [
+                np.exp(_phi * 1.0j) * np.sin(0.5 * _theta),
+                np.exp((_phi + _lambda) * 1.0j) * np.cos(0.5 * _theta),
+            ],
+        ],
+        dtype=complex,
+    )
+
+
+mat_dict = {'id': IdMatrix, 'x': XMatrix, 'y': YMatrix, 'z': ZMatrix,
+            'h': HMatrix, 'w': WMatrix,
+            's': SMatrix, 't': TMatrix,
+            'cx': CXMatrix, 'cnot': CXMatrix, 'cy': CYMatrix, 'cz': CZMatrix,
+            'swap': SwapMatrix, 'iswap': ISwapMatrix,
+            'rx': rx_mat, 'ry': ry_mat, 'rz': rz_mat, 'p': pmatrix,
+            'rxx': rxx_mat, 'ryy': ryy_mat, 'rzz': rzz_mat,
+            'u2': u2matrix, 'u3': u3matrix
+            }
```

## quafu/elements/matrices/mat_utils.py

```diff
@@ -1,132 +1,134 @@
-import cmath
-
-import numpy as np
-from numpy import ndarray
-
-from .mat_lib import IdMatrix
-
-from typing import List
-
-
-def reorder_matrix(matrix: np.ndarray, pos: List):
-    """Reorder the input sorted matrix to the pos order """
-    qnum = len(pos)
-    dim = 2 ** qnum
-    inds = np.argsort(pos)
-    inds = np.concatenate([inds, inds + qnum])
-    tensorm = matrix.reshape([2] * 2 * qnum)
-    return np.transpose(tensorm, inds).reshape([dim, dim])
-
-def split_matrix(matrix: ndarray):
-    """
-    Evenly split a matrix into 4 sub-matrices.
-    """
-    top, bottom = np.vsplit(matrix, 2)
-    t_left, t_right = np.hsplit(top, 2)
-    b_left, b_right = np.hsplit(bottom, 2)
-    return t_left, t_right, b_left, b_right
-
-
-def stack_matrices(t_left, t_right, b_left, b_right):
-    """
-    Stack 4 sub-matrices into a matrix.
-    """
-    top = np.hstack((t_left, t_right))
-    bottom = np.hstack((b_left, b_right))
-    mat = np.vstack((top, bottom))
-    return mat
-
-
-def multi_kron(op1, op2, ind1, ind2, nspin):
-    tmp = 1
-    for i in range(nspin):
-        if i == ind1:
-            tmp = np.kron(tmp, op1)
-        elif i == ind2:
-            tmp = np.kron(tmp, op2)
-        else:
-            tmp = np.kron(tmp, IdMatrix)
-    return tmp
-
-
-def general_kron(op, ind, nqubit):
-    tmp = 1
-    for i in range(nqubit):
-        if i == ind:
-            tmp = np.kron(tmp, op)
-        else:
-            tmp = np.kron(tmp, IdMatrix)
-    return tmp
-
-
-#######################################################
-def is_zero(a):
-    return not np.any(np.absolute(a) > 1e-8)
-
-
-def is_approx(a, b, thres=1e-6):
-    # TODO: seems there are some very small elements that cannot be compared correctly
-    # if not np.allclose(a, b, rtol=thres, atol=thres):
-    #    print(np.sum(a-b))
-    return np.allclose(a, b, rtol=thres, atol=thres)
-
-
-def is_unitary(matrix):
-    mat_dg = np.conjugate(matrix).T
-    id_mat = np.eye(matrix.shape[0])
-    return is_approx(mat_dg @ matrix, id_mat) and is_approx(matrix @ mat_dg, id_mat)
-
-
-def is_hermitian(matrix):
-    tmp = np.conjuate(matrix).T
-    return is_approx(tmp, matrix)
-
-
-def is_diagonal(matrix: ndarray):
-    diag = np.diag(matrix)
-    diag_mat = np.diag(diag)
-    return is_approx(matrix, diag_mat)
-
-
-def is_kron_with_id2(matrix):
-    """
-    Check if the matrix is a Kronecker product of a matrix and identity matrix.
-    """
-    nsize = matrix.shape[0]
-
-    a_cond = is_zero(matrix[0:nsize:2, 1:nsize:2])
-    b_cond = is_zero(matrix[1:nsize:2, 0:nsize:2])
-    c_cond = is_approx(matrix[0, :-1], matrix[1, 1:])
-    d_cond = is_approx(matrix[-2, :-1], matrix[-1, 1:])
-
-    return a_cond and b_cond and c_cond and d_cond
-
-
-#######################################################
-def get_global_phase(unitary):
-    """ Get the global phase of arbitrary unitary, and get the special unitary.
-
-    Args:
-        unitary (np.array): arbitrary unitary
-    Returns:
-        global_phase: the global phase of arbitrary unitary
-        special_unitary (np.array)
-    """
-    coefficient = np.linalg.det(unitary) ** (-0.5)
-    global_phase = -cmath.phase(coefficient)
-    special_unitary = coefficient * unitary
-    return global_phase, special_unitary
-
-
-def matrix_distance_squared(unitary1, unitary2):
-    """ Used to compare the distance of two matrices. The global phase is ignored.
-
-    Args:
-        unitary1 (np.array): A unitary matrix in the form of a numpy ndarray.
-        unitary2 (np.array): Another unitary matrix.
-
-    Returns:
-        Float : A single value between 0 and 1 indicating how closely unitary1 and unitary2 match.
-        A value close to 0 indicates that unitary1 and unitary2 are the same unitary.
-    """
-    return np.abs(1 - np.abs(np.sum(np.multiply(unitary1, np.conj(unitary2)))) / unitary1.shape[0])
+import cmath
+from typing import List
+
+import numpy as np
+from numpy import ndarray
+
+from .mat_lib import IdMatrix
+
+
+def reorder_matrix(matrix: np.ndarray, pos: List):
+    """Reorder the input sorted matrix to the pos order"""
+    qnum = len(pos)
+    dim = 2**qnum
+    inds = np.argsort(pos)
+    inds = np.concatenate([inds, inds + qnum])
+    tensorm = matrix.reshape([2] * 2 * qnum)
+    return np.transpose(tensorm, inds).reshape([dim, dim])
+
+
+def split_matrix(matrix: ndarray):
+    """
+    Evenly split a matrix into 4 sub-matrices.
+    """
+    top, bottom = np.vsplit(matrix, 2)
+    t_left, t_right = np.hsplit(top, 2)
+    b_left, b_right = np.hsplit(bottom, 2)
+    return t_left, t_right, b_left, b_right
+
+
+def stack_matrices(t_left, t_right, b_left, b_right):
+    """
+    Stack 4 sub-matrices into a matrix.
+    """
+    top = np.hstack((t_left, t_right))
+    bottom = np.hstack((b_left, b_right))
+    mat = np.vstack((top, bottom))
+    return mat
+
+
+def multi_kron(op1, op2, ind1, ind2, nspin):
+    tmp = 1
+    for i in range(nspin):
+        if i == ind1:
+            tmp = np.kron(tmp, op1)
+        elif i == ind2:
+            tmp = np.kron(tmp, op2)
+        else:
+            tmp = np.kron(tmp, IdMatrix)
+    return tmp
+
+
+def general_kron(op, ind, nqubit):
+    tmp = 1
+    for i in range(nqubit):
+        if i == ind:
+            tmp = np.kron(tmp, op)
+        else:
+            tmp = np.kron(tmp, IdMatrix)
+    return tmp
+
+
+#######################################################
+def is_zero(a):
+    return not np.any(np.absolute(a) > 1e-8)
+
+
+def is_approx(a, b, thres=1e-6):
+    # TODO: seems there are some very small elements that cannot be compared correctly
+    # if not np.allclose(a, b, rtol=thres, atol=thres):
+    #    print(np.sum(a-b))
+    return np.allclose(a, b, rtol=thres, atol=thres)
+
+
+def is_unitary(matrix):
+    mat_dg = np.conjugate(matrix).T
+    id_mat = np.eye(matrix.shape[0])
+    return is_approx(mat_dg @ matrix, id_mat) and is_approx(matrix @ mat_dg, id_mat)
+
+
+def is_hermitian(matrix):
+    tmp = np.conjuate(matrix).T
+    return is_approx(tmp, matrix)
+
+
+def is_diagonal(matrix: ndarray):
+    diag = np.diag(matrix)
+    diag_mat = np.diag(diag)
+    return is_approx(matrix, diag_mat)
+
+
+def is_kron_with_id2(matrix):
+    """
+    Check if the matrix is a Kronecker product of a matrix and identity matrix.
+    """
+    nsize = matrix.shape[0]
+
+    a_cond = is_zero(matrix[0:nsize:2, 1:nsize:2])
+    b_cond = is_zero(matrix[1:nsize:2, 0:nsize:2])
+    c_cond = is_approx(matrix[0, :-1], matrix[1, 1:])
+    d_cond = is_approx(matrix[-2, :-1], matrix[-1, 1:])
+
+    return a_cond and b_cond and c_cond and d_cond
+
+
+#######################################################
+def get_global_phase(unitary):
+    """Get the global phase of arbitrary unitary, and get the special unitary.
+
+    Args:
+        unitary (np.array): arbitrary unitary
+    Returns:
+        global_phase: the global phase of arbitrary unitary
+        special_unitary (np.array)
+    """
+    coefficient = np.linalg.det(unitary) ** (-0.5)
+    global_phase = -cmath.phase(coefficient)
+    special_unitary = coefficient * unitary
+    return global_phase, special_unitary
+
+
+def matrix_distance_squared(unitary1, unitary2):
+    """Used to compare the distance of two matrices. The global phase is ignored.
+
+    Args:
+        unitary1 (np.array): A unitary matrix in the form of a numpy ndarray.
+        unitary2 (np.array): Another unitary matrix.
+
+    Returns:
+        Float : A single value between 0 and 1 indicating how closely unitary1 and unitary2 match.
+        A value close to 0 indicates that unitary1 and unitary2 are the same unitary.
+    """
+    return np.abs(
+        1 - np.abs(np.sum(np.multiply(unitary1, np.conj(unitary2)))) / unitary1.shape[0]
+    )
```

## quafu/exceptions/__init__.py

```diff
@@ -1,2 +1,4 @@
-from .quafu_error import *
-
+from .circuit_error import *
+from .quafu_error import *
+from .user_error import *
+from .utils import validate_server_resp
```

## quafu/exceptions/circuit_error.py

```diff
@@ -1,19 +1,20 @@
-from .quafu_error import CircuitError
-
-
-# TODO
-class IndexOutOfRangeError(CircuitError):
-    """  """
-    pass
-
-
-class InvalidParaError(CircuitError):
-    """  """
-    pass
-
-
-class UnsupportedYet(CircuitError):
-    """ Un-supported instructions occurs"""
-    pass
-
-
+from .quafu_error import CircuitError
+
+
+# TODO
+class IndexOutOfRangeError(CircuitError):
+    """ """
+
+    pass
+
+
+class InvalidParaError(CircuitError):
+    """ """
+
+    pass
+
+
+class UnsupportedYet(CircuitError):
+    """Un-supported instructions occurs"""
+
+    pass
```

## quafu/exceptions/quafu_error.py

```diff
@@ -1,31 +1,34 @@
-"""
-Exceptions for errors raised while building circuit.
-"""
-
-
-class QuafuError(Exception):
-    """Base class for errors raised by Quafu."""
-
-    def __init__(self, *message):
-        """Set the error message."""
-        super().__init__(" ".join(message))
-        self.message = " ".join(message)
-
-    def __str__(self):
-        """Return the message."""
-        return repr(self.message)
-
-
-class CircuitError(QuafuError):
-    """Exceptions for errors raised while building circuit."""
-    pass
-
-
-class ServerError(QuafuError):
-    """ Exceptions for errors raised while connecting to server."""
-    pass
-
-
-class CompileError(QuafuError):
-    """ Exceptions for errors raised while compiling circuit. """
-    pass
+"""
+Exceptions for errors raised while building circuit.
+"""
+
+
+class QuafuError(Exception):
+    """Base class for errors raised by Quafu."""
+
+    def __init__(self, *message):
+        """Set the error message."""
+        super().__init__(" ".join(message))
+        self.message = " ".join(message)
+
+    def __str__(self):
+        """Return the message."""
+        return repr(self.message)
+
+
+class CircuitError(QuafuError):
+    """Exceptions for errors raised while building circuit."""
+
+    pass
+
+
+class ServerError(QuafuError):
+    """Exceptions for errors raised while connecting to server."""
+
+    pass
+
+
+class CompileError(QuafuError):
+    """Exceptions for errors raised while compiling circuit."""
+
+    pass
```

## quafu/qfasm/qfasm_convertor.py

```diff
@@ -1,29 +1,58 @@
-from .qfasm_parser import QfasmParser, QregNode
-from quafu.dagcircuits.circuit_dag import node_to_gate
-from quafu.dagcircuits.instruction_node import InstructionNode
-from quafu.circuits.quantum_circuit import QuantumCircuit
-
-
-def qasm_to_circuit(qasm):
-    parser = QfasmParser()     
-    nodes = parser.parse(qasm)
-
-    n = 0
-    gates = []
-    measures = {}
-    for node in nodes:
-        if isinstance(node, QregNode):
-            n = node.n
-        if isinstance(node, InstructionNode):
-            if node.name == "measure":
-                for q, c in zip(node.pos.keys(), node.pos.values()):
-                    measures[q] = c
-            else:
-                gates.append(node_to_gate(node))
-
-    q = QuantumCircuit(n)
-    q.gates = gates
-    q.openqasm = qasm
-    q.measures = measures
-    return q
-
+# (C) Copyright 2023 Beijing Academy of Quantum Information Sciences
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#    http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from quafu.circuits.quantum_circuit import QuantumCircuit
+
+from .qfasm_parser import QfasmParser
+
+
+def qasm_to_quafu(openqasm: str):
+    """
+    Initialize pyquafu circuit from openqasm text, mainly by
+    utilizing regular expressions. This function is developed
+    not only to be backward compatible with pure quantum part of
+    OPENQASM2.0, but also to support provide foundation of more
+    powerful syntax parser.
+    """
+    qparser = QfasmParser()
+    qc = qparser.parse(openqasm)
+    qc.openqasm = openqasm
+    if not qc.executable_on_backend:
+        print(
+            "Warning: At present, quafu's back-end real machine does not support dynamic circuits."
+        )
+    return qc
+
+
+def qasm2_to_quafu_qc(qc: QuantumCircuit, openqasm: str):
+    """
+    Initialize pyquafu circuit from openqasm text, mainly by
+    utilizing regular expressions. This function is developed
+    not only to be backward compatible with pure quantum part of
+    OPENQASM2.0, but also to support provide foundation of more
+    powerful syntax parser.
+    """
+    qparser = QfasmParser()
+    newqc = qparser.parse(openqasm)
+    qc.openqasm = openqasm
+    qc.gates = newqc.gates
+    qc.instructions = newqc.instructions
+    qc._measures = newqc._measures
+    qc.qregs = newqc.qregs
+    qc.cregs = newqc.cregs
+    qc.executable_on_backend = newqc.executable_on_backend
+    if not qc.executable_on_backend:
+        print(
+            "Warning: At present, quafu's back-end real machine does not support dynamic circuits."
+        )
```

## quafu/qfasm/qfasm_parser.py

```diff
@@ -1,270 +1,1247 @@
-import ply.yacc as yacc
-
-from quafu.dagcircuits.instruction_node import InstructionNode
-from .qfasmlex import QfasmLexer
-
-
-import numpy as np
-
-
-class DeclarationNode(object):
-    pass
-
-
-class QregNode(DeclarationNode):
-    def __init__(self, n):
-        self.n = n
-
-    def __repr__(self):
-        return self.__str__()
-
-    def __str__(self):
-        return "qreg[%d]" % self.n
-
-
-class CregNode(DeclarationNode):
-    def __init__(self, n):
-        self.n = n
-
-    def __repr__(self):
-        return self.__str__()
-
-    def __str__(self):
-        return "creg[%d]" % self.n
-
-
-class IncludeNode(DeclarationNode):
-    def __init__(self, filename):
-        self.file = filename
-
-    def __repr__(self):
-        return self.__str__()
-
-    def __str__(self):
-        return "include %s" % self.file
-
-
-class OPENQASMNode(DeclarationNode):
-    def __init__(self, version):
-        self.version = version
-
-    def __repr__(self):
-        return self.__str__()
-
-    def __str__(self):
-        return "OPENQASM %.1f" % self.version
-
-
-class QfasmParser(object):
-    tokens = QfasmLexer.tokens
-
-    def __init__(self, debug=False):
-        self.parser = yacc.yacc(module=self, debug=debug)
-        self.parsed_nodes = []
-        self.lexer = QfasmLexer()
-
-    def parse(self, input: str):
-        self.parsed_nodes = self.parser.parse(input, lexer=QfasmLexer())
-        return self.parsed_nodes
-
-    def p_main_0(self, p):
-        """
-        main : program
-        """
-        p[0] = [p[1]]
-
-    def p_main_1(self, p):
-        """
-        main : main program
-        """
-        p[1].append(p[2])
-        p[0] = p[1]
-
-    def p_program(self, p):
-        """
-        program : instruction
-                | declaration
-        """
-        p[0] = p[1]
-
-    def p_declaration(self, p):
-        """
-        declaration : openqasm
-                    | include
-                    | qreg
-                    | creg
-        """
-        p[0] = p[1]
-
-    def p_openqasm(self, p):
-        """
-        openqasm : OPENQASM FLOAT ';'
-        """
-        p[0] = OPENQASMNode(p[2])
-
-    def p_include(self, p):
-        """
-        include : INCLUDE STRING ';'
-        """
-        p[0] = IncludeNode(p[2])
-
-    def p_qreg(self, p):  # TODO:verify register name
-        """
-        qreg : QREG bitreg ';'
-        """
-        p[0] = QregNode(p[2])
-
-    def p_creg(self, p):
-        """
-        creg : CREG bitreg ';'
-        """
-        p[0] = CregNode(p[2])
-
-    def p_instruction(self, p):
-        """
-        instruction : gate ';'
-                | pulse ';'
-                | measure ';'
-        """
-        p[0] = p[1]
-
-    def p_arg_list_0(self, p):
-        """
-        arg_list : expression
-        """
-        p[0] = [p[1]]
-
-    def p_arg_list_1(self, p):
-        """
-        arg_list : arg_list ',' expression
-        """
-        p[1].append(p[3])
-        p[0] = p[1]
-
-    def p_gate_like_0(self, p):
-        '''
-        gate : id qubit_list
-        '''
-        p[0] = InstructionNode(p[1], p[2], None, None, None, "", None, "")
-
-    def p_gate_like_1(self, p):
-        '''
-        gate : id '(' arg_list ')' qubit_list
-        '''
-        p[0] = InstructionNode(p[1], p[5], p[3], None, None, "", None, "")
-
-    def p_pulse_like_0(self, p):
-        '''
-        pulse : id '(' time ',' arg_list ')' qubit_list
-        '''
-        p[0] = InstructionNode(p[1], p[7], p[5], p[3][0], p[3][1], "", None, "")
-
-    def p_measure_0(self, p):
-        '''
-        measure : MEASURE bitreg ASSIGN bitreg
-        '''
-        p[0] = InstructionNode("measure", {p[2]: p[4]}, None, None, None, "", None, "")
-
-    def p_pulse_like_1(self, p):
-        '''
-        pulse : id '(' time ',' arg_list ',' channel ')' qubit_list
-        '''
-        p[0] = InstructionNode(p[1], p[9], p[5], p[3][0], p[3][1], p[7], None, "")
-
-    def p_bitreg(self, p):
-        """
-        bitreg : id '[' INT ']'
-        """
-        p[0] = p[3]
-
-    def p_qubit_list_0(self, p):
-        """
-        qubit_list : bitreg
-        """
-        p[0] = [p[1]]
-
-    def p_qubit_list_1(self, p):
-        """
-        qubit_list : qubit_list ',' bitreg
-        """
-        p[1].append(p[3])
-        p[0] = p[1]
-
-    def p_channel(self, p):
-        """
-        channel : CHANNEL
-        """
-        p[0] = p[1]
-
-    def p_time(self, p):
-        """
-        time : INT UNIT
-        """
-        p[0] = (p[1], p[2])
-
-    def p_expression_none(self, p):
-        """
-        expression : NONE
-        """
-        p[0] = p[1]
-
-    def p_expression_term(self, p):
-        'expression : term'
-        p[0] = p[1]
-
-    def p_expression_m(self, p):
-        """
-        expression : '-' expression
-        """
-        p[0] = -p[2]
-
-    def p_term_factor(self, p):
-        """
-        term : factor
-        """
-        p[0] = p[1]
-
-    def p_binary_operators(self, p):
-        '''expression : expression '+' term
-                    | expression '-' term
-        term       : term '*' factor
-                    | term '/' factor'''
-        if p[2] == '+':
-            p[0] = p[1] + p[3]
-        elif p[2] == '-':
-            p[0] = p[1] - p[3]
-        elif p[2] == '*':
-            p[0] = p[1] * p[3]
-        elif p[2] == '/':
-            p[0] = p[1] / p[3]
-
-    def p_factor_0(self, p):
-        '''
-        factor : FLOAT
-            | INT
-        '''
-        p[0] = p[1]
-
-    def p_factor_1(self, p):
-        '''
-        factor : '(' expression ')'
-        '''
-        p[0] = p[2]
-
-    def p_factor_pi(self, p):
-        '''
-        factor : PI
-        '''
-        p[0] = np.pi
-
-    def p_id(self, p):
-        ''' id : ID'''
-        p[0] = p[1]
-
-    def p_error(self, p):
-        if p:
-            print("Syntax error at token", p.type)
-            # Just discard the token and tell the parser it's okay.
-            self.parser.errok()
-        else:
-            print("Syntax error at EOF")
+# (C) Copyright 2023 Beijing Academy of Quantum Information Sciences
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#    http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import copy
+
+import numpy as np
+import ply.yacc as yacc
+from quafu.circuits.classical_register import ClassicalRegister
+from quafu.circuits.quantum_register import QuantumRegister
+from quafu.elements import *
+from quafu.elements.classical_element import Cif
+from quafu.qfasm.exceptions import ParserError
+
+from quafu import QuantumCircuit
+from quafu.elements import Parameter, ParameterExpression
+from .qfasm_lexer import QfasmLexer
+from .qfasm_utils import *
+
+unaryop = {"sin": "sin", "cos": "cos", "tan": "tan", "exp": "exp",
+           "ln": "log", "sqrt": "sqrt", "acos": "arccos", "atan": "arctan", "asin": "arcsin"}
+unarynp = {
+    "sin": np.sin,
+    "cos": np.cos,
+    "tan": np.tan,
+    "exp": np.exp,
+    "ln": np.log,
+    "sqrt": np.sqrt,
+    "acos": np.arccos,
+    "atan": np.arctan,
+    "asin": np.arcsin,
+}
+reserved = [
+    "creg",
+    "qreg",
+    "pi",
+    "measure",
+    "include",
+    "barrier",
+    "gate",
+    "opaque",
+    "reset",
+    "if",
+    "OPENQASM",
+]
+
+
+class QfasmParser(object):
+    """OPENQASM2.0 Parser"""
+
+    def __init__(self, filepath: str = None, debug=False):
+        self.lexer = QfasmLexer(filepath)
+        self.tokens = self.lexer.tokens
+        self.precedence = (
+            ("left", "+", "-"),
+            ("left", "*", "/"),
+            ("right", "^"),
+            ("right", "UMINUS"),
+        )
+        self.nuop = ["barrier", "reset", "measure"]
+        self.stdgate = list(gate_classes.keys())
+        # extent keyword(the )
+        self.stdgate.extend(["U", "CX"])
+        self.mulctrl = ["mcx", "mcz", "mcy"]
+        self.parser = yacc.yacc(module=self, debug=debug)
+        # when there is reset/op after measure/if, set to false
+        self.executable_on_backend = True
+        self.has_measured = False
+        self.circuit = QuantumCircuit(0)
+        self.global_symtab = {}
+        self.add_U_CX()
+        # function argument symtab
+        self.symtab = {}
+        # qubit num used
+        self.qnum = 0
+        # cbit num used
+        self.cnum = 0
+        # param
+        self.params = {}
+
+    def add_U_CX(self):
+        # Add U and CX in global_symtab
+        U_Id = Id("U", -1, None)
+        CX_Id = Id("CX", -1, None)
+        UNode = SymtabNode("GATE", U_Id)
+        UNode.fill_gate(qargs=[None], cargs=[None, None, None])
+        CXNode = SymtabNode("GATE", CX_Id)
+        CXNode.fill_gate(qargs=[None, None], cargs=[])
+        self.global_symtab["U"] = UNode
+        self.global_symtab["CX"] = CXNode
+
+    # parse data
+    def parse(self, data, debug=False):
+        self.parser.parse(data, lexer=self.lexer, debug=debug)
+        if self.circuit is None:
+            raise ParserError("Exception in parser;")
+        return self.circuit
+
+    def updateSymtab(self, symtabnode: SymtabNode):
+        # update Symtab
+        # reg
+        # print(symtabnode)
+        if symtabnode.name in reserved:
+            raise ParserError(f"Name cannot be reserved word:{reserved}")
+        if symtabnode.is_global:
+            if symtabnode.name in self.global_symtab:
+                hasnode = self.global_symtab[symtabnode.name]
+                raise ParserError(
+                    f"Duplicate declaration for {symtabnode.name} at line {symtabnode.lineno} file {symtabnode.filename}",
+                    f"First occureence at line {hasnode.lineno} file {hasnode.filename}",
+                )
+        else:
+            # just for arg and qarg in gate declaration, so it can duplicate
+            if symtabnode.name in self.symtab:
+                hasnode = self.symtab[symtabnode.name]
+                raise ParserError(
+                    f"Duplicate declaration for {symtabnode.name} at line {symtabnode.lineno} file {symtabnode.filename}"
+                )
+
+        if symtabnode.type == "QREG":
+            symtabnode.start = self.qnum
+            self.qnum += symtabnode.num
+            # add QuantumRegister
+            if len(self.circuit.qregs) == 0:
+                self.circuit.qregs.append(QuantumRegister(self.qnum, name="q"))
+            else:
+                self.circuit.qregs[0] = QuantumRegister(self.qnum, name="q")
+        if symtabnode.type == "CREG":
+            symtabnode.start = self.cnum
+            self.cnum += symtabnode.num
+            # add ClassicalRegister
+            if len(self.circuit.cregs) == 0:
+                self.circuit.cregs.append(ClassicalRegister(self.cnum, name="c"))
+            else:
+                self.circuit.cregs[0] = ClassicalRegister(self.cnum, name="c")
+
+        if symtabnode.is_global:
+            self.global_symtab[symtabnode.name] = symtabnode
+        else:
+            self.symtab[symtabnode.name] = symtabnode
+
+    def handle_gateins(self, gateins: GateInstruction):
+        gate_list = []
+        # end of recurse
+        if gateins.name in self.stdgate and gateins.name not in self.nuop:
+            args = []
+            # add qubits to args, it's might be a qubit or a qreg
+            for qarg in gateins.qargs:
+                if isinstance(qarg, IndexedId):
+                    # check qreg's num is the same
+                    if len(args) >= 1 and len(args[0]) != 1:
+                        raise ParserError(
+                            f"The num of qreg's qubit is inconsistent at line{gateins.lineno} file{gateins.filename}."
+                        )
+                    symnode = self.global_symtab[qarg.name]
+                    args.append([symnode.start + qarg.num])
+                elif isinstance(qarg, Id):
+                    # check qreg's num is the same
+                    symnode = self.global_symtab[qarg.name]
+                    if len(args) >= 1 and symnode.num != len(args[0]):
+                        raise ParserError(
+                            f"The num of qreg's qubit is inconsistent at line{gateins.lineno} file{gateins.filename}."
+                        )
+                    tempargs = []
+                    for i in range(symnode.num):
+                        tempargs.append(symnode.start + i)
+                    args.append(tempargs)
+            # change carg to parameter
+            for i in range(len(gateins.cargs)):
+                gateins.cargs[i] = self.compute_exp(gateins.cargs[i])
+            # call many times
+            for i in range(len(args[0])):
+                oneargs = []
+                for arg in args:
+                    oneargs.append(arg[i])
+                # if it's U or CX
+                if gateins.name == "CX":
+                    gateins.name = "cx"
+                    gate_list.append(gate_classes[gateins.name](*oneargs))
+                elif gateins.name == "U":
+                    gate_list.append(gate_classes["rz"](*[*oneargs, gateins.cargs[2]]))
+                    gate_list.append(gate_classes["ry"](*[*oneargs, gateins.cargs[0]]))
+                    gate_list.append(gate_classes["rz"](*[*oneargs, gateins.cargs[1]]))
+                elif gateins.name in self.mulctrl:
+                    gate_list.append(gate_classes[gateins.name](oneargs[:-1], oneargs[-1]))
+                else:
+                    # add carg to args if there is
+                    if gateins.cargs is not None and len(gateins.cargs) > 0:
+                        oneargs.extend(gateins.cargs)
+                    gate_list.append(gate_classes[gateins.name](*oneargs))
+
+        # if op is barrier or reset or measure
+        elif gateins.name == "reset":
+            for qarg in gateins.qargs:
+                symnode = self.global_symtab[qarg.name]
+                if isinstance(qarg, Id):
+                    qlist = []
+                    for i in range(symnode.num):
+                        qlist.append(symnode.start + i)
+                    gate_list.append(Reset(qlist))
+                elif isinstance(qarg, IndexedId):
+                    gate_list.append(Reset([symnode.start + qarg.num]))
+
+        elif gateins.name == "barrier":
+            qlist = []
+            for qarg in gateins.qargs:
+                symnode = self.global_symtab[qarg.name]
+                if isinstance(qarg, Id):
+                    for i in range(symnode.num):
+                        qlist.append(symnode.start + i)
+                elif isinstance(qarg, IndexedId):
+                    qlist.append(symnode.start + qarg.num)
+            gate_list.append(Barrier(qlist))
+
+        # we have check the num of cbit and qbit
+        elif gateins.name == "measure":
+            bitmap = {}
+            qarg = gateins.qargs[0]
+            cbit = gateins.cbits[0]
+            symnode = self.global_symtab[qarg.name]
+            symnodec = self.global_symtab[cbit.name]
+            if isinstance(qarg, Id):
+                for i in range(symnode.num):
+                    bitmap[symnode.start + i] = symnodec.start + i
+            elif isinstance(qarg, IndexedId):
+                bitmap[symnode.start + qarg.num] = symnodec.start + cbit.num
+            gate_list.append(Measure(bitmap=bitmap))
+            # self.circuit.measure(list(bitmap.keys()), list(bitmap.values()))
+        # if it's not a gate that can be trans to circuit gate, just recurse it
+        else:
+            gatenode: SymtabNode = self.global_symtab[gateins.name]
+            qargdict = {}
+            for i in range(len(gatenode.qargs)):
+                qargdict[gatenode.qargs[i].name] = gateins.qargs[i]
+            cargdict = {}
+            for i in range(len(gatenode.cargs)):
+                cargdict[gatenode.cargs[i].name] = gateins.cargs[i]
+            for ins in gatenode.instructions:
+                # cannot recurse itself!
+                if ins.name == gateins.name:
+                    raise ParserError(
+                        f"The gate {gateins.name} call itself, it's forbiddened at line {gateins.lineno} file {gateins.filename}"
+                    )
+                # change qarg/carg, no cbit in gate param
+                # deep copy
+                newins = copy.deepcopy(ins)
+                # change newins's qarg to real q
+                for i in range(len(newins.qargs)):
+                    newins.qargs[i] = qargdict[newins.qargs[i].name]
+                # change newins's carg to real carg (consider exp and parameter)
+                for i in range(len(newins.cargs)):
+                    # for expression and parameter, it will return parameter or int/float
+                    newins.cargs[i] = self.compute_exp(newins.cargs[i], cargdict)
+                # now, recurse
+                gate_list.extend(self.handle_gateins(newins))
+
+        return gate_list
+
+    def compute_exp(self, carg, cargdict: dict={}):
+        # recurse
+        if isinstance(carg, int) or isinstance(carg, float) or isinstance(carg, ParameterExpression):
+            return carg
+        # if it's id, should get real number from gateins
+        elif isinstance(carg, Id):
+            if carg.name in cargdict:
+                return cargdict[carg.name]
+            # if it's parameter, just return
+            else:
+                return self.params[carg.name]
+        elif isinstance(carg, UnaryExpr):
+            if carg.type == "-":
+                return -self.compute_exp(carg.children[0], cargdict)
+            elif carg.type in unaryop:
+                nowcarg = self.compute_exp(carg.children[0], cargdict)
+                if isinstance(nowcarg, ParameterExpression):
+                    func = getattr(nowcarg, unaryop[carg.type])
+                    return func()
+                else:
+                    return unarynp[carg.type](nowcarg)
+        elif isinstance(carg, BinaryExpr):
+            cargl = self.compute_exp(carg.children[0], cargdict)
+            cargr = self.compute_exp(carg.children[1], cargdict)
+            if carg.type == "+":
+                return cargl + cargr
+            elif carg.type == "-":
+                return cargl - cargr
+            elif carg.type == "*":
+                return cargl * cargr
+            elif carg.type == "/":
+                return cargl / cargr
+            elif carg.type == "^":
+                return cargl ** cargr
+
+    def addInstruction(self, qc: QuantumCircuit, ins):
+        if ins is None:
+            return
+        if isinstance(ins, GateInstruction):
+            gate_list = self.handle_gateins(ins)
+            for gate in gate_list:
+                # print(self.circuit.num)
+                qc.add_ins(gate)
+                if isinstance(gate, Measure):
+                    qc._measures.append(gate)
+        elif isinstance(ins, IfInstruction):
+            symtabnode = self.global_symtab[ins.cbits.name]
+            if isinstance(ins.cbits, Id):
+                cbits = []
+                for i in range(symtabnode.num):
+                    cbits.append(symtabnode.start + i)
+            else:
+                cbits = [symtabnode.start + ins.cbits.num]
+            # get quantum gate
+            gate_list = self.handle_gateins(ins.instruction)
+            qc.add_ins(Cif(cbits=cbits, condition=ins.value, instructions=gate_list))
+        else:
+            raise ParserError(f"Unexpected exception when parse.")
+
+    def check_measure_bit(self, gateins: GateInstruction):
+        cbit = gateins.cbits[0]
+        qarg = gateins.qargs[0]
+        cbit_num = 0
+        qbit_num = 0
+        # check qubit
+        if qarg.name not in self.global_symtab:
+            raise ParserError(
+                f"The qubit {qarg.name} is undefined in qubit register at line {qarg.lineno} file {qarg.filename}"
+            )
+        symnode = self.global_symtab[qarg.name]
+        if symnode.type != "QREG":
+            raise ParserError(
+                f"{qarg.name} is not declared as qubit register at line {qarg.lineno} file {qarg.filename}"
+            )
+        if isinstance(qarg, IndexedId):
+            qbit_num = 1
+            if qarg.num + 1 > symnode.num:
+                raise ParserError(
+                    f"Qubit arrays {qarg.name} are out of bounds at line {qarg.lineno} file {qarg.filename}"
+                )
+        else:
+            qbit_num = symnode.num
+        # check cbit
+        if cbit.name not in self.global_symtab:
+            raise ParserError(
+                f"The classical bit {cbit.name} is undefined in classical bit register at line {cbit.lineno} file {cbit.filename}"
+            )
+        symnode = self.global_symtab[cbit.name]
+        if symnode.type != "CREG":
+            raise ParserError(
+                f"{cbit.name} is not declared as classical bit register at line {cbit.lineno} file {cbit.filename}"
+            )
+        if isinstance(cbit, IndexedId):
+            cbit_num = 1
+            if cbit.num + 1 > symnode.num:
+                raise ParserError(
+                    f"Classical bit arrays {cbit.name} are out of bounds at line {cbit.lineno} file {cbit.filename}"
+                )
+        else:
+            cbit_num = symnode.num
+        # check qubits'num matches cbits's num
+        if cbit_num != qbit_num:
+            raise ParserError(
+                f"MEASURE: the num of qubit and clbit doesn't match at line {gateins.lineno} file {gateins.filename}"
+            )
+
+    def check_qargs(self, gateins: GateInstruction):
+        # check gatename declared
+        qargslist = []
+        if gateins.name not in self.nuop and gateins.name not in self.mulctrl:
+            if gateins.name not in self.global_symtab:
+                raise ParserError(
+                    f"The gate {gateins.name} is undefined at line {gateins.lineno} file {gateins.filename}"
+                )
+            # check if gateins.name is a gate
+            gatenote = self.global_symtab[gateins.name]
+            if gatenote.type != "GATE":
+                raise ParserError(
+                    f"The {gateins.name} is not declared as a gate at line {gateins.lineno} file {gateins.filename}"
+                )
+            # check args matches gate's declared args
+            if len(gateins.qargs) != len(gatenote.qargs):
+                raise ParserError(
+                    f"The numbe of qubit declared in gate {gateins.name} is inconsistent with instruction at line {gateins.lineno} file {gateins.filename}"
+                )
+        # check qubits must from global symtab
+        for qarg in gateins.qargs:
+            if qarg.name not in self.global_symtab:
+                raise ParserError(
+                    f"The qubit {qarg.name} is undefined in qubit register at line {qarg.lineno} file {qarg.filename}"
+                )
+            symnode = self.global_symtab[qarg.name]
+            if symnode.type != "QREG":
+                raise ParserError(
+                    f"{qarg.name} is not declared as qubit register at line {qarg.lineno} file {qarg.filename}"
+                )
+            # check if the qarg is out of bounds when qarg's type is indexed_id
+            if isinstance(qarg, IndexedId):
+                if qarg.num + 1 > symnode.num:
+                    raise ParserError(
+                        f"Qubit arrays {qarg.name} are out of bounds at line {qarg.lineno} file {qarg.filename}"
+                    )
+                qargslist.append((qarg.name, qarg.num))
+            else:
+                for num in range(symnode.num):
+                    qargslist.append((qarg.name, num))
+        # check  distinct qubits
+        if len(qargslist) != len(set(qargslist)):
+            raise ParserError(
+                f"Qubit used as different argument when call gate {gateins.name} at line {gateins.lineno} file {gateins.filename}"
+            )
+
+    def check_param(self, carg):
+        if isinstance(carg, int) or isinstance(carg, float):
+            return
+        elif isinstance(carg, Id) and carg.name not in self.params:
+            raise ParserError(f"The parameter {carg.name} is undefined at line {carg.lineno} file {carg.filename}")
+        elif isinstance(carg, UnaryExpr):
+            self.check_param(carg.children[0])
+        elif isinstance(carg, BinaryExpr):
+            self.check_param(carg.children[0])
+            self.check_param(carg.children[1])
+
+    def check_cargs(self, gateins: GateInstruction):
+        # check that cargs belongs to unary (they must be int or float or parameter)
+        # cargs is different from CREG
+        if gateins.name not in self.nuop and gateins.name not in self.mulctrl:
+            if gateins.name not in self.global_symtab:
+                raise ParserError(
+                    f"The gate {gateins.name} is undefined at line {gateins.lineno} file {gateins.filename}"
+                )
+            gatenote = self.global_symtab[gateins.name]
+            if gatenote.type != "GATE":
+                raise ParserError(
+                    f"The {gateins.name} is not declared as a gate at line {gateins.lineno} file {gateins.filename}"
+                )
+            # check every carg in [int, float, parameter]
+            for carg in gateins.cargs:
+                self.check_param(carg)
+            # check cargs's num matches gate's delcared cargs
+            if len(gateins.cargs) != len(gatenote.cargs):
+                raise ParserError(
+                    f"The number of classical argument declared in gate {gateins.name} is inconsistent with instruction at line {gateins.lineno} file {gateins.filename}"
+                )
+
+    def check_gate_qargs(self, gateins: GateInstruction):
+        # check type and number
+        qargs = gateins.qargs
+        gatename = gateins.name
+        qargsname = []
+        if gatename != "barrier":
+            # check gatename declared
+            if gatename not in self.global_symtab:
+                raise ParserError(
+                    f"The gate {gatename} is undefined at line {gateins.lineno} file {gateins.filename}"
+                )
+            gatenode = self.global_symtab[gatename]
+            if gatenode.type != "GATE":
+                raise ParserError(
+                    f"The {gatename} is not declared as a gate at line {gateins.lineno} file {gateins.filename}"
+                )
+            # check qarg's num matches gate's qargs, except barrier
+            if len(gatenode.qargs) != len(qargs):
+                raise ParserError(
+                    f"The numbe of qubit declared in gate {gatename} is inconsistent with instruction at line {gateins.lineno} file {gateins.filename}"
+                )
+        # check gate_op's qubit args, must from gate declared argument
+        for qarg in qargs:
+            qargsname.append(qarg.name)
+            # check qarg declaration
+            if qarg.name not in self.symtab:
+                raise ParserError(
+                    f"The qubit {qarg.name} is undefined in gate qubit parameters at line {qarg.lineno} file {qarg.filename}"
+                )
+            symnode = self.symtab[qarg.name]
+            if symnode.type != "QARG":
+                raise ParserError(
+                    f"{qarg.name} is not declared as a qubit at line {qarg.lineno} file {qarg.filename}"
+                )
+        if len(qargs) != len(set(qargsname)):
+            raise ParserError(
+                f"A qubit used as different argument when call gate {gateins.name} at line {gateins.lineno} file {gateins.filename}"
+            )
+
+    def check_gate_cargs(self, gateins: GateInstruction):
+        # check gate_op's classcal args, must matches num declared by gate
+        if gateins.name in ["barrier", "reset", "measure"] and len(gateins.cargs) > 0:
+            raise ParserError(
+                f"Barrier can not receive classical argument at line {gateins.lineno} file {gateins.filename}"
+            )
+        if gateins.name not in ["barrier", "reset", "measure"]:
+            if gateins.name not in self.global_symtab:
+                raise ParserError(
+                    f"The gate {gateins.name} is undefined at line {gateins.lineno} file {gateins.filename}"
+                )
+            gatenode = self.global_symtab[gateins.name]
+            if gatenode.type != "GATE":
+                raise ParserError(
+                    f"The {gateins.name} is not declared as a gate at line {gateins.lineno} file {gateins.filename}"
+                )
+            if len(gateins.cargs) != len(gatenode.cargs):
+                raise ParserError(
+                    f"The number of classical argument declared in gate {gateins.name} is inconsistent with instruction at line {gateins.lineno} file {gateins.filename}"
+                )
+            # check carg must from gate declared argument or int/float or parameter
+            for carg in gateins.cargs:
+                # recurse check expression
+                self.check_carg_declartion(carg)
+
+    def check_carg_declartion(self, node):
+        if isinstance(node, int) or isinstance(node, float):
+            return
+        if isinstance(node, Id):
+            # check declaration
+            if node.name in self.symtab:
+                symnode = self.symtab[node.name]
+                if symnode.type != "CARG":
+                    raise ParserError(
+                        f"The {node.name} is not declared as a classical bit at line {node.lineno} file {node.filename}"
+                    )
+                return
+            elif node.name not in self.params:
+                raise ParserError(
+                    f"The classical argument {node.name} is undefined at line {node.lineno} file {node.filename}"
+                )
+        if isinstance(node, UnaryExpr):
+            self.check_carg_declartion(node.children[0])
+        elif isinstance(node, BinaryExpr):
+            for i in range(2):
+                self.check_carg_declartion(node.children[i])
+
+    start = "main"
+
+    def p_main(self, p):
+        """
+        main : program
+        """
+        # now get the root node, return Citcuit
+        self.circuit.executable_on_backend = self.executable_on_backend
+
+    # when reduce statement into program, insert it to circuit and update symtab if it can.
+    def p_program(self, p):
+        """
+        program : statement
+        """
+        p[0] = self.circuit
+        self.addInstruction(p[0], p[1])
+
+    def p_program_list(self, p):
+        """
+        program : program statement
+        """
+        p[0] = p[1]
+        self.addInstruction(p[0], p[2])
+
+        # statement |= qdecl | gatedecl | qop | if | barrier
+
+    # statement
+    # error -> ply.lex.LexToken(value)
+    # others -> p -> ply.yacc.YaccProduction
+    #        -> p[1] -> t.value
+    def p_statement_openqasm(self, p):
+        """
+        statement : OPENQASM FLOAT ';'
+                    | OPENQASM FLOAT error
+                    | OPENQASM error
+        """
+        if len(p) == 3:
+            raise ParserError(f"Expecting FLOAT after OPENQASM, received {p[2].value}")
+        if p[3] != ";":
+            raise ParserError("Expecting ';' at end of OPENQASM statement")
+        if p[2] != 2.0:
+            raise ParserError("Only support OPENQASM 2.0 version")
+        p[0] = None
+
+    # qop
+    def p_statement_qop(self, p):
+        """
+        statement : qop ';'
+                | qop error
+                | qif ';'
+                | qif error
+        """
+        if p[2] != ";":
+            raise ParserError(f"Expecting ';' behind statement at line {p[1].lineno} file {p[1].filename}")
+        p[0] = p[1]
+
+    def p_statement_empty(self, p):
+        """
+        statement : ';'
+        """
+        p[0] = None
+
+    def p_statement_qif(self, p):
+        """
+        qif : IF '(' primary MATCHES INT ')' qop
+            | IF '(' primary MATCHES INT error
+            | IF '(' primary MATCHES error
+            | IF '(' primary error
+            | IF '(' error
+            | IF error
+        """
+        # check primary is a creg and check range
+        if len(p) == 7:
+            raise ParserError(
+                f"Illegal IF statement, Expecting ')' at line {p[1].lineno} file {p[1].filename}"
+            )
+        if len(p) == 6:
+            raise ParserError(
+                f"Illegal IF statement, Expecting INT: the Rvalue can only be INT at line {p[1].lineno} file {p[1].filename}"
+            )
+        if len(p) == 5:
+            raise ParserError(
+                f"Illegal IF statement, Expecting '==' at line {p[1].lineno} file {p[1].filename}"
+            )
+        if len(p) == 4:
+            raise ParserError(
+                f"Illegal IF statement, Expecting Cbit: the Lvalue can only be cbit at line {p[1].lineno} file {p[1].filename}"
+            )
+        if len(p) == 3:
+            raise ParserError(
+                f"Illegal IF statement, Expecting '(' at line {p[1].lineno} file {p[1].filename}"
+            )
+
+        cbit = p[3]
+        if cbit.name not in self.global_symtab:
+            raise ParserError(
+                f"The classical bit {cbit.name} is undefined in classical bit register at line {cbit.lineno} file {cbit.filename}"
+            )
+        symnode = self.global_symtab[cbit.name]
+        if symnode.type != "CREG":
+            raise ParserError(
+                f"{cbit.name} is not declared as classical bit register at line {cbit.lineno} file {cbit.filename}"
+            )
+        # check range if IndexedId
+        if isinstance(cbit, IndexedId):
+            if cbit.num >= symnode.num:
+                raise ParserError(
+                    f"{cbit.name} out of range at line {cbit.lineno} file {cbit.filename}"
+                )
+            # optimization: If the value that creg can represent is smaller than Rvalue, just throw it
+            if p[5] > 2:
+                p[0] = None
+            else:
+                p[0] = IfInstruction(
+                    node=p[1], cbits=p[3], value=p[5], instruction=p[7]
+                )
+        elif isinstance(cbit, Id):
+            # optimization: If the value that creg can represent is smaller than Rvalue, just throw it
+            num = symnode.num
+            if pow(2, num) - 1 < p[5]:
+                p[0] = None
+            else:
+                p[0] = IfInstruction(
+                    node=p[1], cbits=p[3], value=p[5], instruction=p[7]
+                )
+        self.executable_on_backend = False
+
+    def p_unitaryop(self, p):
+        """
+        qop : id primary_list
+            | id '(' ')' primary_list
+            | id '(' expression_list ')' primary_list
+        """
+        # return circuit gate instance
+        if len(p) == 5:
+            p[0] = GateInstruction(node=p[1], qargs=p[4], cargs=[])
+        if len(p) == 3:
+            p[0] = GateInstruction(node=p[1], qargs=p[2], cargs=[])
+        if len(p) == 6:
+            p[0] = GateInstruction(node=p[1], qargs=p[5], cargs=p[3])
+        # check args
+        self.check_qargs(p[0])
+        self.check_cargs(p[0])
+        if self.has_measured:
+            self.executable_on_backend = False
+
+    def p_unitaryop_error(self, p):
+        """
+        qop : id '(' ')' error
+            | id '(' error
+            | id '(' expression_list ')' error
+            | id '(' expression_list error
+        """
+        if len(p) == 4 or (len(p) == 5 and p[4] != ")"):
+            raise ParserError(
+                f"Expecting ')' after '(' at line {p[1].lineno} file {p[1].filename}"
+            )
+        raise ParserError(
+            f"Expecting qubit list, received {p[len(p)-1].value} at line {p[1].lineno} file {p[1].filename}"
+        )
+
+    # measure
+    def p_measure(self, p):
+        """
+        qop : MEASURE primary ASSIGN primary
+        """
+        # check and return gateInstruction
+        p[0] = GateInstruction(node=p[1], qargs=[p[2]], cargs=[], cbits=[p[4]])
+        self.check_measure_bit(p[0])
+        self.has_measured = True
+
+    def p_measure_error(self, p):
+        """
+        qop : MEASURE primary ASSIGN error
+            | MEASURE primary error
+            | MEASURE error
+        """
+        if len(p) == 5:
+            raise ParserError(
+                f"Expecting qubit or qubit register after '->' at line {p[1].lineno} file {p[1].filename}"
+            )
+        if len(p) == 4:
+            raise ParserError(
+                f"Expecting '->' for MEASURE at line {p[1].lineno} file {p[1].filename}"
+            )
+        if len(p) == 3:
+            raise ParserError(
+                f"Expecting qubit or qubit register after 'measure' at line {p[1].lineno} file {p[1].filename}"
+            )
+
+    # barrier
+    def p_barrier(self, p):
+        """
+        qop : BARRIER primary_list
+        """
+        # check and return gateInstruction
+        p[0] = GateInstruction(node=p[1], qargs=p[2], cargs=[])
+        self.check_qargs(p[0])
+
+    def p_barrier_error(self, p):
+        """
+        qop : BARRIER error
+        """
+        raise ParserError(
+            f"Expecting Qubit:BARRIER only opperate qubits at line {p[1].lineno} file {p[1].filename}"
+        )
+
+    # reset
+    def p_reset(self, p):
+        """
+        qop : RESET primary
+        """
+        p[0] = GateInstruction(node=p[1], qargs=[p[2]], cargs=[])
+        self.check_qargs(p[0])
+        self.executable_on_backend = False
+
+    def p_reset_error(self, p):
+        """
+        qop : RESET error
+        """
+        raise ParserError(
+            f"Expecting Qubit: RESET only opperate qubit at line {p[1].lineno} file {p[1].filename}"
+        )
+
+    # gate_qarg_list
+    def p_gate_qarg_list_begin(self, p):
+        """
+        qarg_list : id
+        """
+        p[0] = [p[1]]
+        newsymtabnode = SymtabNode("QARG", p[1], False, True)
+        self.updateSymtab(newsymtabnode)
+
+    def p_gate_qarg_list_next(self, p):
+        """
+        qarg_list : qarg_list ',' id
+        """
+        p[0] = p[1]
+        p[0].append(p[3])
+        newsymtabnode = SymtabNode("QARG", p[3], False, True)
+        self.updateSymtab(newsymtabnode)
+
+    # gate_carg_list
+    def p_gate_carg_list_begin(self, p):
+        """
+        carg_list : id
+        """
+        p[0] = [p[1]]
+        newsymtabnode = SymtabNode("CARG", p[1], False)
+        self.updateSymtab(newsymtabnode)
+
+    def p_gate_carg_list_next(self, p):
+        """
+        carg_list : carg_list ',' id
+        """
+        p[0] = p[1]
+        p[0].append(p[3])
+        newsymtabnode = SymtabNode("CARG", p[3], False)
+        self.updateSymtab(newsymtabnode)
+
+    # gatedecl
+    def p_statement_gatedecl_nolr(self, p):
+        """
+        statement : GATE id gate_scope qarg_list gate_body
+                | GATE error
+                | GATE id gate_scope error
+                | GATE id gate_scope qarg_list error
+        """
+        if len(p) == 3:
+            raise ParserError(
+                f"Expecting ID after 'gate', received {p[len(p)-1].value} at line {p[1].lineno} file {p[1].filename}"
+            )
+        if len(p) == 5:
+            raise ParserError(
+                f"Expecting '(' or qubit list after gate name, received {p[len(p)-1].value} at line {p[1].lineno} file {p[1].filename}"
+            )
+        if len(p) == 6 and not isinstance(p[5], list):
+            raise ParserError(
+                f"Expecting gate body qubit list, received {p[len(p)-1].value} at line {p[1].lineno} file {p[1].filename}"
+            )
+        newsymtabnode = SymtabNode("GATE", p[2])
+        newsymtabnode.fill_gate(p[4], p[5])
+        self.updateSymtab(newsymtabnode)
+
+    def p_statement_gatedecl_noargs(self, p):
+        """
+        statement : GATE id gate_scope '(' ')' qarg_list gate_body
+                | GATE id gate_scope '(' error
+                | GATE id gate_scope '(' ')' error
+                | GATE id gate_scope '(' ')' qarg_list error
+        """
+        if len(p) == 6:
+            raise ParserError(
+                f"Expecting ')' or argument list after '(', received {p[len(p)-1].value} at line {p[1].lineno} file {p[1].filename}"
+            )
+        if len(p) == 7:
+            raise ParserError(
+                f"Expecting qubit list after ')', received {p[len(p)-1].value} at line {p[1].lineno} file {p[1].filename}"
+            )
+        if len(p) == 8 and not isinstance(p[7], list):
+            raise ParserError(
+                f"Expecting gate body after qubit list, received {p[len(p)-1].value} at line {p[1].lineno} file {p[1].filename}"
+            )
+        newsymtabnode = SymtabNode("GATE", p[2])
+        newsymtabnode.fill_gate(p[6], p[7])
+        self.updateSymtab(newsymtabnode)
+
+    def p_statement_gatedecl_args(self, p):
+        """
+        statement : GATE id gate_scope '(' carg_list ')' qarg_list gate_body
+                | GATE id gate_scope '(' carg_list ')' qarg_list error
+                | GATE id gate_scope '(' carg_list ')' error
+                | GATE id gate_scope '(' carg_list error
+        """
+        if len(p) == 7:
+            raise ParserError(
+                f"Expecting ')' after argument list, received {p[len(p)-1].value} at line {p[1].lineno} file {p[1].filename}"
+            )
+        if len(p) == 8:
+            raise ParserError(
+                f"Expecting qubit list after ')', received {p[len(p)-1].value} at line {p[1].lineno} file {p[1].filename}"
+            )
+        if len(p) == 9 and not isinstance(p[8], list):
+            raise ParserError(
+                f"Expecting gate body after qubit list, received {p[len(p)-1].value} at line {p[1].lineno} file {p[1].filename}"
+            )
+        if len(p) != 9:
+            raise ParserError(f"Invaild GATE statement")
+        newsymtabnode = SymtabNode("GATE", p[2])
+        newsymtabnode.fill_gate(p[7], p[8], p[5])
+        self.updateSymtab(newsymtabnode)
+
+    def p_gate_scope(self, _):
+        """
+        gate_scope :
+        """
+        self.symtab = {}
+
+    # gatebody
+    def p_gate_body_emptybody(self, p):
+        """
+        gate_body : '{' gate_scope '}'
+                    | '{' gate_scope error
+        """
+        if p[3] != "}":
+            raise ParserError(
+                "Expecting '}' at the end of gate definition; received " + p[3].value
+            )
+        p[0] = []
+
+    def p_gate_body(self, p):
+        """
+        gate_body : '{' gop_list gate_scope '}'
+                    | '{' gop_list gate_scope error
+        """
+        if p[4] != "}":
+            raise ParserError(
+                "Expecting '}' at the end of gate definition; received " + p[4].value
+            )
+        p[0] = p[2]
+
+    def p_gop_list_begin(self, p):
+        """
+        gop_list : gop
+        """
+        p[0] = [p[1]]
+
+    def p_gop_list_next(self, p):
+        """
+        gop_list : gop_list gop
+        """
+        p[0] = p[1]
+        p[0].append(p[2])
+
+    # gop
+    # CX | U | ID(cargs)qargs | reset |
+    def p_gop_nocargs(self, p):
+        """
+        gop : id id_list ';'
+            | id id_list error
+            | id '(' ')' id_list ';'
+            | id '(' ')' id_list error
+            | id '(' ')' error
+            | id '(' error
+        """
+        if len(p) == 4 and p[2] == "(":
+            raise ParserError(
+                f"Expecting ')' for gate {p[1].name} at line {p[1].lineno} file {p[1].filename}"
+            )
+        if len(p) == 4 and p[3] != ";":
+            raise ParserError(
+                f"Expecting ';' after gate {p[1].name} at line {p[1].lineno} file {p[1].filename}"
+            )
+        if len(p) == 6 and p[5] != ";":
+            raise ParserError(
+                f"Expecting ';' after gate {p[1].name} at line {p[1].lineno} file {p[1].filename}"
+            )
+        if len(p) == 5:
+            raise ParserError(
+                f"Expecting ID: Invalid qubit list for gate {p[1].name} at line {p[1].lineno} file {p[1].filename}"
+            )
+        qargs = p[2] if len(p) == 4 else p[4]
+        p[0] = GateInstruction(node=p[1], qargs=qargs, cargs=[])
+        self.check_gate_qargs(p[0])
+        self.check_gate_cargs(p[0])
+
+    def p_gop_cargs(self, p):
+        """
+        gop : id '(' expression_list ')' id_list ';'
+            | id '(' expression_list ')' id_list error
+            | id '(' expression_list ')' error
+            | id '(' expression_list error
+        """
+        if len(p) == 7 and p[6] != ";":
+            raise ParserError(
+                f"Expecting ';' after gate {p[1].name} at line {p[1].lineno}"
+            )
+        if len(p) == 6:
+            raise ParserError(
+                f"Expecting qubit id after gate {p[1].name} at line {p[1].lineno}"
+            )
+        if len(p) == 5:
+            raise ParserError(
+                f"Expecting ')' after gate {p[1].name} at line {p[1].lineno}"
+            )
+        p[0] = GateInstruction(node=p[1], qargs=p[5], cargs=p[3])
+        # check qubit
+        self.check_gate_qargs(p[0])
+        # check expression_list
+        self.check_gate_cargs(p[0])
+
+    def p_gop_barrier(self, p):
+        """
+        gop : BARRIER id_list ';'
+            | BARRIER id_list error
+            | BARRIER error
+        """
+        if len(p) == 3:
+            raise ParserError(
+                f"Expecting ID: Invalid barrier qubit list inside gate definition, at line {p[1].lineno} file {p[1].filename}"
+            )
+        if len(p) == 4 and p[3] != ";":
+            raise ParserError(
+                f"Expecting ';' after barrier at line {p[1].lineno} file {p[1].filename}"
+            )
+        p[0] = GateInstruction(node=p[1], qargs=p[2], cargs=[])
+        self.check_gate_qargs(p[0])
+
+    # regdecl
+    def p_statement_bitdecl(self, p):
+        """
+        statement : qdecl ';'
+                    | cdecl ';'
+                    | defparam ';'
+                    | defparam error
+                    | qdecl error
+                    | cdecl error
+                    | error
+        """
+        if len(p) == 2:
+            raise ParserError(f"Expecting valid statement")
+        if p[2] != ";":
+            raise ParserError(
+                f"Expecting ';' in qreg or creg declaration at line {p.lineno(2)}"
+            )
+        p[0] = p[1]
+
+    def p_statement_defparam(self, p):
+        """
+        defparam : id EQUAL FLOAT
+                 | id EQUAL INT
+                 | id EQUAL error
+        """
+        if not isinstance(p[3], int) and not isinstance(p[3], float):
+            raise ParserError(f"Expecting 'INT' or 'FLOAT behind '=' at line {p[1].lineno} file {p[1].filename}")
+        param_name = p[1].name
+        if param_name in self.params:
+            raise ParserError(f"Duplicate declaration for parameter {p[1].name} at line {p[1].lineno} file {p[1].filename}")
+        self.params[param_name] = Parameter(param_name, p[3])
+        p[0] = None
+
+    def p_qdecl(self, p):
+        """
+        qdecl : QREG indexed_id
+                | QREG error
+        """
+        if not isinstance(p[2], IndexedId):
+            raise ParserError(
+                f"Expecting ID[int] after QREG at line {p[1].lineno} file {p[1].filename}, received {p[2].value}"
+            )
+        if p[2].num <= 0:
+            raise ParserError(
+                f"QREG size must be positive at line {p[2].lineno} file {p[2].filename}"
+            )
+        newsymtabnode = SymtabNode("QREG", p[2], True, True)
+        self.updateSymtab(newsymtabnode)
+        p[0] = None
+
+    def p_cdecl(self, p):
+        """
+        cdecl : CREG indexed_id
+                | CREG error
+        """
+        if not isinstance(p[2], IndexedId):
+            raise ParserError(
+                f"Expecting ID[int] after CREG at line {p[1].lineno} file {p[1].filename}, received {p[2].value}"
+            )
+        if p[2].num <= 0:
+            raise ParserError(
+                f"CREG size must be positive at line {p[2].lineno} file {p[2].filename}"
+            )
+        newsymtabnode = SymtabNode("CREG", p[2], True, False)
+        self.updateSymtab(newsymtabnode)
+        p[0] = None
+
+    # id
+    def p_id(self, p):
+        """
+        id : ID
+            | error
+        """
+        # It's instance of Id class, passed from t.value
+        if not isinstance(p[1], Id):
+            raise ParserError(f"Expecting an ID, received {str(p[1].value)}")
+        p[0] = p[1]
+
+    # indexed_id
+    def p_indexed_id(self, p):
+        """
+        indexed_id : id '[' INT ']'
+                    | id '[' INT error
+                    | id '[' error
+        """
+        if len(p) == 4 or (len(p) == 5 and p[4] != "]"):
+            raise ParserError(
+                f"Expecting INT after [, received{str(p[len(p)-1].value)}"
+            )
+        if len(p) == 5 and p[4] == "]":
+            p[0] = IndexedId(p[1], p[3])
+
+    # primary
+    # only q or q[], used for U CX measure reset
+    def p_primary(self, p):
+        """
+        primary : id
+                | indexed_id
+        """
+        p[0] = p[1]
+
+    # primary_list
+    # the anylist in bnf
+    def p_primary_list(self, p):
+        """
+        primary_list : primary
+                     | primary_list ',' primary
+        """
+        if len(p) == 2:
+            p[0] = [p[1]]
+        else:
+            p[0] = p[1]
+            p[0].append(p[3])
+
+    # id_list
+    # for decl gate
+    def p_id_list_begin(self, p):
+        """
+        id_list : id
+        """
+        p[0] = [p[1]]
+
+    def p_id_list_next(self, p):
+        """
+        id_list : id_list ',' id
+        """
+        p[0] = p[1]
+        p[0].append(p[3])
+
+    # unary
+    def p_unary_int(self, p):
+        """
+        unary : INT
+        """
+        p[0] = int(p[1])
+
+    def p_unary_float(self, p):
+        """
+        unary : FLOAT
+        """
+        p[0] = float(p[1])
+
+    def p_unary_pi(self, p):
+        """
+        unary : PI
+        """
+        p[0] = np.pi
+
+    # id from ID
+    def p_unary_id(self, p):
+        """
+        unary : id
+        """
+        p[0] = p[1]
+
+    # expr
+    def p_expr_binary(self, p):
+        """
+        expression : expression '*' expression
+                    | expression '/' expression
+                    | expression '+' expression
+                    | expression '-' expression
+                    | expression '^' expression
+        """
+        if p[2] == "/" and p[3] == 0:
+            raise ParserError(
+                f"Divided by 0 at line {self.lexer.lexer.lineno} file {self.lexer.lexer.filename}"
+            )
+        if isinstance(p[1], Node) or isinstance(p[3], Node):
+            p[0] = BinaryExpr(p[2], p[1], p[3])
+        else:
+            # int or float
+            if p[2] == "*":
+                p[0] = p[1] * p[3]
+            elif p[2] == "/":
+                p[0] = p[1] / p[3]
+            elif p[2] == "^":
+                p[0] = p[1] ** p[3]
+            elif p[2] == "+":
+                p[0] = p[1] + p[3]
+            elif p[2] == "-":
+                p[0] = p[1] - p[3]
+
+    def p_expr_uminus(self, p):
+        """
+        expression : - expression %prec UMINUS
+        """
+        if isinstance(p[2], Node):
+            p[0] = UnaryExpr("-", p[2])
+        else:
+            # int or float
+            p[0] = -p[2]
+
+    def p_expr_unary(self, p):
+        """
+        expression : unary
+        """
+        p[0] = p[1]
+
+    def p_expr_pare(self, p):
+        """
+        expression : '(' expression ')'
+        """
+        p[0] = p[2]
+
+    def p_expr_mathfunc(self, p):
+        """
+        expression : id '(' expression ')'
+        """
+        if p[1].name not in unaryop:
+            raise ParserError(
+                f"Math function {p[1].name} not supported, only support {unaryop.keys()} line {p[1].lineno} file {p[1].filename}"
+            )
+        if not isinstance(p[3], Node):
+            p[0] = unarynp[p[1].name](p[3])
+        else:
+            p[0] = UnaryExpr(p[1].name, p[3])
+
+    # Exprlist
+    def p_exprlist_begin(self, p):
+        """
+        expression_list : expression
+        """
+        p[0] = [p[1]]
+
+    def p_exprlist_next(self, p):
+        """
+        expression_list : expression_list ',' expression
+        """
+        p[0] = p[1]
+        p[0].append(p[3])
+
+    # Only filename provide string
+    # So, It will never get a string in parser
+    def p_ignore(self, _):
+        """
+        ignore : STRING
+        """
+        pass
+
+    def p_empty(self, p):
+        """
+        empty :
+        """
+        pass
+
+    def p_error(self, p):
+        # EOF case
+        if p is None or self.lexer.lexer.token() is None:
+            raise ParserError("Error at end of file")
+        print(
+            f"Error near line {self.lexer.lexer.lineno}, Column {self.cal_column(self.lexer.data, p)}"
+        )
+
+    def cal_column(self, data: str, p):
+        "Compute the column"
+        begin_of_line = data.rfind("\n", 0, p.lexpos)
+        begin_of_line = max(0, begin_of_line)
+        column = p.lexpos - begin_of_line + 1
+        return column
```

## quafu/results/results.py

```diff
@@ -1,196 +1,275 @@
-import copy
-from collections import OrderedDict
-
-import matplotlib.pyplot as plt
-from ..utils.basis import *
-
-
-class Result(object):
-    """Basis class for quantum results"""
-    pass
-
-
-class ExecResult(Result):
-    """ 
-    Class that save the execute results returned from backend.
-    
-    Attributes:
-        counts (dict): Samples counts on each bitstring.
-        probabilities (dict): Calculated probabilities on each bitstring.
-        taskid (int): Unique task id for the execute result.
-        transpiled_circuit (QuantumCircuit): Quantum circuit transpiled on backend.
-    """
-
-    def __init__(self, input_dict):
-        status_map = {0: "In Queue", 1: "Running", 2: "Completed", "Canceled": 3, 4: "Failed"}
-        self.taskid = input_dict['task_id']
-        self.taskname = input_dict['task_name']
-        self.transpiled_openqasm = input_dict["openqasm"]
-        from ..circuits.quantum_circuit import QuantumCircuit
-        self.transpiled_circuit = QuantumCircuit(0)
-        self.transpiled_circuit.from_openqasm(self.transpiled_openqasm)
-        self.measure_base = []
-
-        self.measures = self.transpiled_circuit.measures
-        self.task_status = status_map[input_dict["status"]]
-        self.res = eval(input_dict['res'])
-        self.counts = OrderedDict(sorted(self.res.items(), key=lambda s: s[0]))
-
-        self.logicalq_res = {}
-        cbits = list(self.measures.values())
-        indexed_cbits = {bit: i for i, bit in enumerate(sorted(cbits))}
-        squeezed_cbits = [indexed_cbits[bit] for bit in cbits]
-        for key, values in self.counts.items():
-            newkey = "".join([key[i] for i in squeezed_cbits])
-            self.logicalq_res[newkey] = values
-
-        total_counts = sum(self.counts.values())
-        self.probabilities = {}
-        for bit_str in self.counts:
-            self.probabilities[bit_str] = self.counts[bit_str] / total_counts
-
-    def calculate_obs(self, pos):
-        """
-        Calculate observables Z on input position using probabilities
-
-        Args: 
-            pos (list[int]): Positions of observalbes.
-        """
-        return measure_obs(pos, self.logicalq_res)
-
-    def plot_probabilities(self):
-        """
-        Plot the probabilities from execute results.
-        """
-        bitstrs = list(self.probabilities.keys())
-        probs = list(self.probabilities.values())
-        plt.figure()
-        plt.bar(range(len(probs)), probs, tick_label=bitstrs)
-        plt.xticks(rotation=70)
-        plt.ylabel("probabilities")
-
-
-class SimuResult(Result):
-    """
-    Class that save the execute simulation results returned from classical simulator.
-
-    Attributes:
-        num (int): Numbers of measured qubits
-        probabilities (ndarray): Calculated probabilities on each bitstring.
-        rho (ndarray): Simulated density matrix of measured qubits
-    """
-
-    def __init__(self, input, input_form):
-        self.num = int(np.log2(input.shape[0]))
-        if input_form == "density_matrix":
-            self.rho = np.array(input)
-            self.probabilities = np.diag(input)
-        elif input_form == "probabilities":
-            self.probabilities = input
-        elif input_form == "state_vector":
-            self.state_vector = input
-
-    def plot_probabilities(self, full: bool = False, reverse_basis: bool = False, sort: bool = None):
-        """
-        Plot the probabilities from simulated results, ordered in big endian convention.
-        
-        Args:
-            full: Whether plot on the full basis of measured qubits.
-            reverse_basis: Whether reverse the bitstring of basis. (Little endian convention).
-            sort:  Sort the results by probabilities values. Can be `"ascend"` order or `"descend"` order. 
-        """
-        plt.close()
-        probs = self.probabilities
-        inds = range(len(probs))
-        if not full:
-            inds = np.where(self.probabilities > 1e-14)[0]
-            probs = self.probabilities[inds]
-
-        basis = np.array([bin(i)[2:].zfill(self.num) for i in inds])
-        if reverse_basis:
-            basis = np.array([bin(i)[2:].zfill(self.num)[::-1] for i in inds])
-
-        if sort == "ascend":
-            orders = np.argsort(probs)
-            probs = probs[orders]
-            basis = basis[orders]
-        elif sort == "descend":
-            orders = np.argsort(probs)
-            probs = probs[orders][::-1]
-            basis = basis[orders][::-1]
-
-        plt.figure()
-        plt.bar(range(len(inds)), probs, tick_label=basis)
-        plt.xticks(rotation=70)
-        plt.ylabel("probabilities")
-
-    def get_statevector(self):
-        return self.state_vector
-
-    def calculate_obs(self, pos):
-        "Calculate observables Z on input position using probabilities"
-        inds = np.where(self.probabilities > 1e-14)[0]
-        probs = self.probabilities[inds]
-        basis = np.array([bin(i)[2:].zfill(self.num) for i in inds])
-        res_reduced = dict(zip(basis, probs))
-        return measure_obs(pos, res_reduced)
-
-
-def intersec(a, b):
-    inter = []
-    aind = []
-    bind = []
-    for i in range(len(a)):
-        for j in range(len(b)):
-            if a[i] == b[j]:
-                inter.append(a[i])
-                aind.append(i)
-                bind.append(j)
-
-    return inter, aind, bind
-
-
-def diff(a, b):
-    diff = []
-    aind = []
-    for i in range(len(a)):
-        if a[i] not in b:
-            diff.append(a[i])
-            aind.append(i)
-
-    return diff, aind
-
-
-def merge_measure(obslist):
-    obslist = copy.deepcopy(obslist)
-    measure_basis = []
-    targ_basis = []
-    for obs in obslist:
-        if len(measure_basis) == 0:
-            measure_basis.append(obs)
-            targ_basis.append(len(measure_basis) - 1)
-        else:
-            added = 0
-            for mi in range(len(measure_basis)):
-                measure_base = measure_basis[mi]
-                interset, intobsi, intbasei = intersec(obs[1], measure_base[1])
-                diffset, diffobsi = diff(obs[1], measure_base[1])
-                if not len(interset) == 0:
-                    if all(np.array(list(obs[0]))[intobsi] == np.array(list(measure_base[0]))[intbasei]):
-                        measure_base[0] += "".join(np.array(list(obs[0]))[diffobsi])
-                        measure_base[1].extend(diffset)
-                        targ_basis.append(mi)
-                        added = 1
-                        break
-                else:
-                    measure_base[0] += obs[0]
-                    measure_base[1].extend(obs[1])
-                    targ_basis.append(mi)
-                    added = 1
-                    break
-
-            if not added:
-                measure_basis.append(obs)
-                targ_basis.append(len(measure_basis) - 1)
-
-    return measure_basis, targ_basis
+import copy
+from collections import OrderedDict
+
+import matplotlib.pyplot as plt
+
+from ..algorithms.hamiltonian import Hamiltonian
+from ..utils.basis import *
+
+
+class Result(object):
+    """Basis class for quantum results"""
+
+    pass
+
+
+class ExecResult(Result):
+    """
+    Class that save the execute results returned from backend.
+
+    Attributes:
+        counts (dict): Samples counts on each bitstring.
+        probabilities (dict): Calculated probabilities on each bitstring.
+        taskid (int): Unique task id for the execute result.
+        transpiled_circuit (QuantumCircuit): Quantum circuit transpiled on backend.
+    """
+
+    def __init__(self, input_dict):
+        status_map = {
+            0: "In Queue",
+            1: "Running",
+            2: "Completed",
+            "Canceled": 3,
+            4: "Failed",
+        }
+        self.taskid = input_dict["task_id"]
+        self.taskname = input_dict["task_name"]
+        self.transpiled_openqasm = input_dict["openqasm"]
+        from ..circuits.quantum_circuit import QuantumCircuit
+
+        self.transpiled_circuit = QuantumCircuit(0)
+        self.transpiled_circuit.from_openqasm(self.transpiled_openqasm)
+        self.measure_base = []
+
+        self.measures = self.transpiled_circuit.measures
+        self.task_status = status_map[input_dict["status"]]
+        self.res = eval(input_dict["res"])
+        self.counts = OrderedDict(sorted(self.res.items(), key=lambda s: s[0]))
+
+        self.logicalq_res = {}
+        cbits = list(self.measures.values())
+        indexed_cbits = {bit: i for i, bit in enumerate(sorted(cbits))}
+        squeezed_cbits = [indexed_cbits[bit] for bit in cbits]
+        for key, values in self.counts.items():
+            newkey = "".join([key[i] for i in squeezed_cbits])
+            self.logicalq_res[newkey] = values
+
+        total_counts = sum(self.counts.values())
+        self.probabilities = {}
+        for bit_str in self.counts:
+            self.probabilities[bit_str] = self.counts[bit_str] / total_counts
+
+    def calculate_obs(self, pos):
+        """
+        Calculate observables Z on input position using probabilities
+
+        Args:
+            pos (list[int]): Positions of observalbes.
+        """
+        return measure_obs(pos, self.logicalq_res)
+
+    def plot_probabilities(self):
+        """
+        Plot the probabilities from execute results.
+        """
+        bitstrs = list(self.probabilities.keys())
+        probs = list(self.probabilities.values())
+        plt.figure()
+        plt.bar(range(len(probs)), probs, tick_label=bitstrs)
+        plt.xticks(rotation=70)
+        plt.ylabel("probabilities")
+
+
+class SimuResult(Result):
+    def __init__(self, res_info: dict):
+        """
+        Args:
+            res_info: data from simulator
+        """
+        self._meta_data = res_info
+        counts = res_info["counts"]
+        if counts:
+            if isinstance(list(counts.keys())[0], int):
+                cbits_num = len(res_info["measures"])
+                newcounts = {}
+                for key, value in counts.items():
+                    bitstr = bin(key)[2:].zfill(cbits_num)
+                    newcounts[bitstr] = value
+                self._meta_data["counts"] = newcounts
+
+        self._probabilities = []
+
+    def __getitem__(self, key: str):
+        """
+        Get meta_data of simulate results.
+        Args:
+            `"statevector"`: full state vector
+            `"counts"`: sampled  bitstring counts
+            `"pauli_expects"`: pauli expectations of input paulistrings
+        """
+        return self._meta_data[key]
+
+    def get_statevector(self):
+        try:
+            return self["statevector"]
+        except KeyError:
+            raise KeyError("no statevector saved from %s simulator" % self["simulator"])
+
+    @property
+    def probabilities(self):
+        if len(self._probabilities) == 0:
+            self.calc_probabilities()
+        return self._probabilities
+
+    @property
+    def counts(self):
+        return self["counts"]
+
+    def calc_probabilities(self):
+        psi = self.get_statevector()
+        num = self["qbitnum"]
+        measures = list(self["measures"].keys())
+        values_tmp = list(self["measures"].values())
+        values = np.argsort(values_tmp)
+
+        from ..simulators.default_simulator import permutebits, ptrace
+
+        psi = permutebits(psi, range(num)[::-1])
+        if measures:
+            self._probabilities = ptrace(psi, measures)
+            self._probabilities = permutebits(self._probabilities, values)
+        else:
+            self._probabilities = np.abs(psi) ** 2
+
+    def plot_probabilities(
+        self,
+        full: bool = False,
+        reverse_basis: bool = False,
+        sort: bool = None,
+        from_counts=False,
+    ):
+        """
+        Plot the probabilites of measured qubits
+        """
+        import matplotlib.pyplot as plt
+
+        if from_counts:
+            counts = self._meta_data["counts"]
+            total_counts = sum(counts.values())
+            probabilities = {}
+            for key in self._meta_data["counts"]:
+                probabilities[key] = counts[key] / total_counts
+
+            bitstrs = list(probabilities.keys())
+            probs = list(probabilities.values())
+            plt.figure()
+            plt.bar(range(len(probs)), probs, tick_label=bitstrs)
+            plt.xticks(rotation=70)
+            plt.ylabel("probabilities")
+
+        elif len(self.get_statevector()) > 0:
+            if not full:
+                inds = np.where(self.probabilities > 1e-14)[0]
+                probs = self.probabilities[inds]
+
+            measures = self._meta_data["measures"]
+            num = len(measures) if measures else self["qbitnum"]
+            basis = np.array([bin(i)[2:].zfill(num) for i in inds])
+            if reverse_basis:
+                basis = np.array([bin(i)[2:].zfill(num)[::-1] for i in inds])
+
+            if sort == "ascend":
+                orders = np.argsort(probs)
+                probs = probs[orders]
+                basis = basis[orders]
+            elif sort == "descend":
+                orders = np.argsort(probs)
+                probs = probs[orders][::-1]
+                basis = basis[orders][::-1]
+
+            plt.figure()
+            plt.bar(inds, probs, tick_label=basis)
+            plt.xticks(rotation=70)
+            plt.ylabel("probabilities")
+        else:
+            raise ValueError("No data for ploting")
+
+    def calc_density_matrix(self):
+        psi = self.get_statevector()
+        num = self["qbitnum"]
+        measures = list(self["measures"].keys())
+        values_tmp = list(self["measures"].values())
+        values = np.argsort(values_tmp)
+        if len(measures) == 0:
+            measures = list(range(num))
+            values = list(range(num))
+        from ..simulators.default_simulator import permutebits, ptrace
+
+        psi = permutebits(psi, range(num)[::-1])
+        rho = ptrace(psi, measures, diag=False)
+        rho = permutebits(rho, values)
+        return rho
+
+
+# TODO:These should merge to paulis
+def intersec(a, b):
+    inter = []
+    aind = []
+    bind = []
+    for i in range(len(a)):
+        for j in range(len(b)):
+            if a[i] == b[j]:
+                inter.append(a[i])
+                aind.append(i)
+                bind.append(j)
+
+    return inter, aind, bind
+
+
+def diff(a, b):
+    diff = []
+    aind = []
+    for i in range(len(a)):
+        if a[i] not in b:
+            diff.append(a[i])
+            aind.append(i)
+
+    return diff, aind
+
+
+def merge_measure(obslist):
+    obslist = copy.deepcopy(obslist)
+    measure_basis = []
+    targ_basis = []
+    for obs in obslist:
+        if len(measure_basis) == 0:
+            measure_basis.append(obs)
+            targ_basis.append(len(measure_basis) - 1)
+        else:
+            added = 0
+            for mi in range(len(measure_basis)):
+                measure_base = measure_basis[mi]
+                interset, intobsi, intbasei = intersec(obs[1], measure_base[1])
+                diffset, diffobsi = diff(obs[1], measure_base[1])
+                if not len(interset) == 0:
+                    if all(
+                        np.array(list(obs[0]))[intobsi]
+                        == np.array(list(measure_base[0]))[intbasei]
+                    ):
+                        measure_base[0] += "".join(np.array(list(obs[0]))[diffobsi])
+                        measure_base[1].extend(diffset)
+                        targ_basis.append(mi)
+                        added = 1
+                        break
+                else:
+                    measure_base[0] += obs[0]
+                    measure_base[1].extend(obs[1])
+                    targ_basis.append(mi)
+                    added = 1
+                    break
+
+            if not added:
+                measure_basis.append(obs)
+                targ_basis.append(len(measure_basis) - 1)
+
+    return measure_basis, targ_basis
```

## quafu/simulators/__init__.py

```diff
@@ -1 +1,119 @@
-00000000: 20                                        
+00000000: 6672 6f6d 202e 2e63 6972 6375 6974 732e  from ..circuits.
+00000010: 7175 616e 7475 6d5f 6369 7263 7569 7420  quantum_circuit 
+00000020: 696d 706f 7274 2051 7561 6e74 756d 4369  import QuantumCi
+00000030: 7263 7569 740a 6672 6f6d 2074 7970 696e  rcuit.from typin
+00000040: 6720 696d 706f 7274 2055 6e69 6f6e 0a0a  g import Union..
+00000050: 696d 706f 7274 206e 756d 7079 2061 7320  import numpy as 
+00000060: 6e70 0a66 726f 6d20 7175 6166 7520 696d  np.from quafu im
+00000070: 706f 7274 2051 7561 6e74 756d 4369 7263  port QuantumCirc
+00000080: 7569 740a 6672 6f6d 202e 2e72 6573 756c  uit.from ..resul
+00000090: 7473 2e72 6573 756c 7473 2069 6d70 6f72  ts.results impor
+000000a0: 7420 5369 6d75 5265 7375 6c74 0a0a 6465  t SimuResult..de
+000000b0: 6620 7369 6d75 6c61 7465 280a 2020 2020  f simulate(.    
+000000c0: 7163 3a20 556e 696f 6e5b 5175 616e 7475  qc: Union[Quantu
+000000d0: 6d43 6972 6375 6974 2c20 7374 725d 2c0a  mCircuit, str],.
+000000e0: 2020 2020 7073 693a 206e 702e 6e64 6172      psi: np.ndar
+000000f0: 7261 7920 3d20 6e70 2e61 7272 6179 285b  ray = np.array([
+00000100: 5d29 2c0a 2020 2020 7369 6d75 6c61 746f  ]),.    simulato
+00000110: 723a 2073 7472 203d 2022 7374 6174 6576  r: str = "statev
+00000120: 6563 746f 7222 2c0a 2020 2020 7368 6f74  ector",.    shot
+00000130: 733a 2069 6e74 203d 2031 3030 2c0a 2020  s: int = 100,.  
+00000140: 2020 6861 6d69 6c74 6f6e 6961 6e20 3d20    hamiltonian = 
+00000150: 4e6f 6e65 2c0a 2020 2020 7573 655f 6770  None,.    use_gp
+00000160: 753a 2062 6f6f 6c20 3d20 4661 6c73 652c  u: bool = False,
+00000170: 0a20 2020 2075 7365 5f63 7573 7461 7465  .    use_custate
+00000180: 7665 633a 2062 6f6f 6c20 3d20 4661 6c73  vec: bool = Fals
+00000190: 652c 0a29 202d 3e20 5369 6d75 5265 7375  e,.) -> SimuResu
+000001a0: 6c74 3a0a 2020 2020 2222 2253 696d 756c  lt:.    """Simul
+000001b0: 6174 6520 7175 616e 7475 6d20 6369 7263  ate quantum circ
+000001c0: 7569 740a 2020 2020 4172 6773 3a0a 2020  uit.    Args:.  
+000001d0: 2020 2020 2020 7163 3a20 7175 616e 7475        qc: quantu
+000001e0: 6d20 6369 7263 7569 7420 6f72 2071 6173  m circuit or qas
+000001f0: 6d20 7374 7269 6e67 2074 6861 7420 6e65  m string that ne
+00000200: 6564 2074 6f20 6265 2073 696d 756c 6174  ed to be simulat
+00000210: 6564 2e0a 2020 2020 2020 2020 7073 6920  ed..        psi 
+00000220: 3a20 496e 7075 7420 7374 6174 6520 7665  : Input state ve
+00000230: 6374 6f72 0a20 2020 2020 2020 2073 696d  ctor.        sim
+00000240: 756c 6174 6f72 3a0a 2020 2020 2020 2020  ulator:.        
+00000250: 2020 2020 6022 7374 6174 6576 6563 746f      `"statevecto
+00000260: 7222 603a 2054 6865 2068 6967 6820 7065  r"`: The high pe
+00000270: 7266 6f72 6d61 6e63 6520 432b 2b20 6369  rformance C++ ci
+00000280: 7263 7569 7420 7369 6d75 6c61 746f 7220  rcuit simulator 
+00000290: 7769 7468 206f 7074 696f 6e61 6c20 4750  with optional GP
+000002a0: 5520 7375 7070 6f72 742e 0a20 2020 2020  U support..     
+000002b0: 2020 2020 2020 2060 2263 6c69 6666 6f72         `"cliffor
+000002c0: 6422 603a 2054 6865 2068 6967 6820 7065  d"`: The high pe
+000002d0: 7266 6f72 6d61 6e63 6520 432b 2b20 6369  rformance C++ ci
+000002e0: 6666 6f72 6420 6369 7263 7569 7420 7369  fford circuit si
+000002f0: 6d75 6c61 746f 722e 0a20 2020 2020 2020  mulator..       
+00000300: 2020 2020 2060 226e 6f69 7379 2073 7461       `"noisy sta
+00000310: 7465 7665 746f 7222 603a 204e 6f73 6979  tevetor"`: Nosiy
+00000320: 2063 6972 6375 6974 2073 696d 756c 6174   circuit simulat
+00000330: 6f72 2069 6d70 6c65 6d65 6e74 6564 2077  or implemented w
+00000340: 6974 6820 7374 6174 6576 6563 746f 7220  ith statevector 
+00000350: 7369 6d75 6c61 746f 722e 0a0a 2020 2020  simulator...    
+00000360: 2020 2020 7368 6f74 733a 2054 6865 2073      shots: The s
+00000370: 686f 7473 206f 6620 7369 6d75 6c61 746f  hots of simulato
+00000380: 7220 6578 6563 7574 696f 6e73 2e0a 2020  r executions..  
+00000390: 2020 2020 2020 7573 655f 6770 753a 2055        use_gpu: U
+000003a0: 7365 2074 6865 2047 5055 2076 6572 7369  se the GPU versi
+000003b0: 6f6e 206f 6620 6073 7461 7465 7665 6374  on of `statevect
+000003c0: 6f72 6020 7369 6d75 6c61 746f 722e 0a20  or` simulator.. 
+000003d0: 2020 2020 2020 2075 7365 5f63 7573 7461         use_custa
+000003e0: 7465 7665 633a 2055 7365 2063 7553 7461  tevec: Use cuSta
+000003f0: 7465 5665 632d 6261 7365 6420 6073 7461  teVec-based `sta
+00000400: 7465 7665 6374 6f72 6020 7369 6d75 6c61  tevector` simula
+00000410: 746f 722e 2054 6865 2061 7267 756d 656e  tor. The argumen
+00000420: 7420 6075 7365 5f67 7075 6020 6d75 7374  t `use_gpu` must
+00000430: 2061 6c73 6f20 6265 2054 7275 652e 0a0a   also be True...
+00000440: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+00000450: 2020 2020 2053 696d 7552 6573 756c 7420       SimuResult 
+00000460: 6f62 6a65 6374 2074 6861 7420 636f 6e74  object that cont
+00000470: 6169 6e20 7468 6520 7265 7375 6c74 732e  ain the results.
+00000480: 2222 220a 2020 2020 0a20 2020 2071 6173  """.    .    qas
+00000490: 6d20 3d20 2222 0a20 2020 2069 6620 6973  m = "".    if is
+000004a0: 696e 7374 616e 6365 2871 632c 2073 7472  instance(qc, str
+000004b0: 293a 0a20 2020 2020 2020 2071 6173 6d20  ):.        qasm 
+000004c0: 3d20 7163 0a20 2020 2020 2020 2071 6320  = qc.        qc 
+000004d0: 3d20 5175 616e 7475 6d43 6972 6375 6974  = QuantumCircuit
+000004e0: 2830 290a 2020 2020 2020 2020 7163 2e66  (0).        qc.f
+000004f0: 726f 6d5f 6f70 656e 7161 736d 2871 6173  rom_openqasm(qas
+00000500: 6d29 0a0a 2020 2020 2320 7369 6d75 6c61  m)..    # simula
+00000510: 7465 0a20 2020 2069 6620 7369 6d75 6c61  te.    if simula
+00000520: 746f 7220 3d3d 2022 7374 6174 6576 6563  tor == "statevec
+00000530: 746f 7222 3a0a 2020 2020 2020 2020 6672  tor":.        fr
+00000540: 6f6d 202e 7369 6d75 6c61 746f 7220 696d  om .simulator im
+00000550: 706f 7274 2053 5653 696d 756c 6174 6f72  port SVSimulator
+00000560: 0a20 2020 2020 2020 2062 6163 6b65 6e64  .        backend
+00000570: 203d 2053 5653 696d 756c 6174 6f72 2875   = SVSimulator(u
+00000580: 7365 5f67 7075 2c20 7573 655f 6375 7374  se_gpu, use_cust
+00000590: 6174 6576 6563 290a 2020 2020 2020 2020  atevec).        
+000005a0: 7265 7475 726e 2062 6163 6b65 6e64 2e72  return backend.r
+000005b0: 756e 2871 632c 2070 7369 2c20 7368 6f74  un(qc, psi, shot
+000005c0: 732c 2068 616d 696c 746f 6e69 616e 290a  s, hamiltonian).
+000005d0: 2020 2020 656c 6966 2073 696d 756c 6174      elif simulat
+000005e0: 6f72 203d 3d20 226e 6f69 7379 2073 7461  or == "noisy sta
+000005f0: 7465 7665 746f 7222 3a0a 2020 2020 2020  tevetor":.      
+00000600: 2020 6672 6f6d 202e 7369 6d75 6c61 746f    from .simulato
+00000610: 7220 696d 706f 7274 204e 6f69 7365 5356  r import NoiseSV
+00000620: 5369 6d75 6c61 746f 720a 2020 2020 2020  Simulator.      
+00000630: 2020 6261 636b 656e 6420 3d20 4e6f 6973    backend = Nois
+00000640: 6553 5653 696d 756c 6174 6f72 2875 7365  eSVSimulator(use
+00000650: 5f67 7075 2c20 7573 655f 6375 7374 6174  _gpu, use_custat
+00000660: 6576 6563 290a 2020 2020 2020 2020 7265  evec).        re
+00000670: 7475 726e 2062 6163 6b65 6e64 2e72 756e  turn backend.run
+00000680: 2871 632c 2070 7369 2c20 7368 6f74 732c  (qc, psi, shots,
+00000690: 2068 616d 696c 746f 6e69 616e 290a 2020   hamiltonian).  
+000006a0: 2020 656c 6966 2073 696d 756c 6174 6f72    elif simulator
+000006b0: 203d 3d20 2263 6c69 6666 6f72 6422 3a0a   == "clifford":.
+000006c0: 2020 2020 2020 2020 6672 6f6d 202e 7369          from .si
+000006d0: 6d75 6c61 746f 7220 696d 706f 7274 2043  mulator import C
+000006e0: 6c69 6666 6f72 6453 696d 756c 6174 6f72  liffordSimulator
+000006f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00000700: 436c 6966 666f 7264 5369 6d75 6c61 746f  CliffordSimulato
+00000710: 7228 292e 7275 6e28 7163 2c20 7368 6f74  r().run(qc, shot
+00000720: 7329 0a0a 2020 2020 656c 7365 3a0a 2020  s)..    else:.  
+00000730: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00000740: 6545 7272 6f72 2822 696e 7661 6c69 6420  eError("invalid 
+00000750: 7369 6d75 6c61 746f 7220 6e61 6d65 2229  simulator name")
+00000760: 0a                                       .
```

## quafu/simulators/default_simulator.py

```diff
@@ -1,55 +1,75 @@
-# default circuit simulator for state vector
+# (C) Copyright 2023 Beijing Academy of Quantum Information Sciences
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#    http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+"""default circuit simulator for state vector"""
 
+import copy
 from typing import Iterable, List, Union
-from quafu.circuits.quantum_circuit import QuantumCircuit
-from ..results.results import SimuResult
-from quafu.elements import Barrier, Delay, QuantumGate, SingleQubitGate, MultiQubitGate, XYResonance
+
 import numpy as np
+from quafu.circuits.quantum_circuit import QuantumCircuit
+from scipy.sparse import coo_matrix, eye, kron
 from sparse import COO, SparseArray
-from scipy.sparse import kron, eye, coo_matrix
 
-import copy
+from ..elements import (
+    Barrier,
+    Delay,
+    QuantumGate,
+    XYResonance,
+)
+from ..results.results import SimuResult
 
 
 def global_op(gate: QuantumGate, global_qubits: List) -> coo_matrix:
     """Local operators to global operators"""
     num = len(global_qubits)
-    if isinstance(gate, SingleQubitGate):
+    if len(gate.pos) == 1:
         local_mat = coo_matrix(gate.matrix)
         pos = global_qubits.index(gate.pos)
-        local_mat = kron(kron(eye(2 ** pos), local_mat), eye(2 ** (num - pos - 1)))
+        local_mat = kron(kron(eye(2**pos), local_mat), eye(2 ** (num - pos - 1)))
         return local_mat
 
-    elif isinstance(gate, MultiQubitGate):
+    else:
         local_mat = coo_matrix(gate.matrix)
         pos = [global_qubits.index(p) for p in gate.pos]
         num_left = min(pos)
         num_right = num - max(pos) - 1
         num_center = max(pos) - min(pos) + 1
         center_mat = kron(local_mat, eye(2 ** (num_center - len(pos))))
         origin_order = sorted(pos)
         origin_order.extend([p for p in range(min(pos), max(pos) + 1) if p not in pos])
         new_order = np.argsort(origin_order)
         center_mat = COO.from_scipy_sparse(center_mat)
         center_mat = permutebits(center_mat, new_order).to_scipy_sparse()
-        center_mat = kron(kron(eye(2 ** num_left), center_mat), eye(2 ** num_right))
+        center_mat = kron(kron(eye(2**num_left), center_mat), eye(2**num_right))
         return center_mat
 
 
-def permutebits(mat: Union[SparseArray, np.ndarray], order: Iterable) \
-        -> Union[SparseArray, np.ndarray]:
+def permutebits(
+    mat: Union[SparseArray, np.ndarray], order: Iterable
+) -> Union[SparseArray, np.ndarray]:
     """permute qubits for operators or states"""
     num = len(order)
     order = np.array(order)
     r = len(mat.shape)
     mat = np.reshape(mat, [2] * r * num)
     order = np.concatenate([order + len(order) * i for i in range(r)])
     mat = np.transpose(mat, order)
-    mat = np.reshape(mat, [2 ** num] * r)
+    mat = np.reshape(mat, [2**num] * r)
     return mat
 
 
 def ptrace(psi, ind_A: List, diag: bool = True) -> np.ndarray:
     """partial trace on a state vector"""
     num = int(np.log2(psi.shape[0]))
     order = copy.deepcopy(ind_A)
@@ -63,36 +83,40 @@
         return psi
     else:
         psi = np.reshape(psi, [2 ** len(ind_A), 2 ** (num - len(ind_A))])
         rho = psi @ np.conj(np.transpose(psi))
         return rho
 
 
-def py_simulate(qc: QuantumCircuit,
-                state_ini: np.ndarray = np.array([]),
-                output: str = "amplitudes") -> SimuResult:
+def py_simulate(
+    qc: QuantumCircuit, state_ini: np.ndarray = np.array([]), output: str = "amplitudes"
+) -> SimuResult:
     """Simulate quantum circuit
-        Args:
-            qc: quantum circuit need to be simulated.
-            state_ini (numpy.ndarray): Input state vector
-            output (str): `"amplitudes"`: Return ampliteds on measured qubits.
-                          `"density_matrix"`: Return reduced density_amtrix on measured qubits.
-                          `"state_vector`: Return full statevector.
-        Returns:
-           SimuResult object that contain the results.
+    Args:
+        qc: quantum circuit need to be simulated.
+        state_ini (numpy.ndarray): Input state vector
+        output (str): `"amplitudes"`: Return ampliteds on measured qubits.
+                      `"density_matrix"`: Return reduced density_amtrix on measured qubits.
+                      `"state_vector`: Return full statevector.
+    Returns:
+       SimuResult object that contain the results.
     """
 
     used_qubits = qc.used_qubits
     num = len(used_qubits)
     if not state_ini:
-        psi = np.zeros(2 ** num)
+        psi = np.zeros(2**num)
         psi[0] = 1
 
     else:
         psi = state_ini
 
     for gate in qc.gates:
-        if not ((isinstance(gate, Delay)) or (isinstance(gate, Barrier)) or isinstance(gate, XYResonance)):
+        if not (
+            (isinstance(gate, Delay))
+            or (isinstance(gate, Barrier))
+            or isinstance(gate, XYResonance)
+        ):
             op = global_op(gate, used_qubits)
             psi = op @ psi
 
     return psi
```

## quafu/simulators/simulator.py

```diff
@@ -1,90 +1,204 @@
-from typing import Union
-from .default_simulator import py_simulate, ptrace, permutebits
-from .qfvm import simulate_circuit, execute
-from quafu import QuantumCircuit
-from ..results.results import SimuResult
-import numpy as np
-from ..exceptions import QuafuError
-
-
-def simulate(qc: Union[QuantumCircuit, str],
-             psi: np.ndarray = np.array([]),
-             simulator: str = "qfvm_circ",
-             output: str = "probabilities",
-             use_gpu: bool = False,
-             use_custatevec: bool = False) -> SimuResult:
-    """Simulate quantum circuit
-    Args:
-        qc: quantum circuit or qasm string that need to be simulated.
-        psi : Input state vector
-        simulator:`"qfvm_circ"`: The high performance C++ circuit simulator with optional GPU support. 
-                `"py_simu"`: Python implemented simulator by sparse matrix with low performance for large scale circuit.
-                `"qfvm_qasm"`: The high performance C++ qasm simulator with limited gate set.
-
-        output: `"probabilities"`: Return probabilities on measured qubits, ordered in big endian convention.
-                `"density_matrix"`: Return reduced density_amtrix on measured qubits, ordered in big endian convention.
-                `"state_vector`: Return original full statevector. The statevector returned by `qfvm` backend is ordered in little endian convention (same as qiskit), while `py_simu` backend is orderd in big endian convention.
-        use_gpu: Use the GPU version of `qfvm_circ` simulator.
-        use_custatevec: Use cuStateVec-based `qfvm_circ` simulator. The argument `use_gpu` must also be True.
-
-    Returns:
-        SimuResult object that contain the results.
-"""
-    qasm = ""
-    if simulator == "qfvm_qasm":
-        if not isinstance(qc, str):
-            raise ValueError("Must input valid qasm str for qfvm_qasm simulator")
-
-        qasm = qc
-        qc = QuantumCircuit(0)
-        qc.from_openqasm(qasm)
-
-    measures = [qc.used_qubits.index(i) for i in qc.measures.keys()]
-    num = 0
-    if simulator == "qfvm_circ":
-        num = max(qc.used_qubits) + 1
-        measures = list(qc.measures.keys())
-        if use_gpu:
-            if use_custatevec:
-                try:
-                    from .qfvm import simulate_circuit_custate
-                except ImportError:
-                    raise QuafuError(" pyquafu is installed with cuquantum support")
-                psi = simulate_circuit_custate(qc, psi)
-            else:
-                try:
-                    from .qfvm import simulate_circuit_gpu
-                except ImportError:
-                    raise QuafuError("you are not using the GPU version of pyquafu")
-                psi = simulate_circuit_gpu(qc, psi)
-        else:
-            psi = simulate_circuit(qc, psi)
-
-    elif simulator == "py_simu":
-        psi = py_simulate(qc, psi)
-    elif simulator == "qfvm_qasm":
-        num = qc.num
-        measures = list(qc.measures.keys())
-        psi = execute(qasm)
-    else:
-        raise ValueError("invalid circuit")
-
-    if output == "density_matrix":
-        if simulator in ["qfvm_circ", "qfvm_qasm"]:
-            psi = permutebits(psi, range(num)[::-1])
-        rho = ptrace(psi, measures, diag=False)
-        rho = permutebits(rho, list(qc.measures.values()))
-        return SimuResult(rho, output)
-
-    elif output == "probabilities":
-        if simulator in ["qfvm_circ", "qfvm_qasm"]:
-            psi = permutebits(psi, range(num)[::-1])
-        probabilities = ptrace(psi, measures)
-        probabilities = permutebits(probabilities, list(qc.measures.values()))
-        return SimuResult(probabilities, output)
-
-    elif output == "state_vector":
-        return SimuResult(psi, output)
-
-    else:
-        raise ValueError("output should in be 'density_matrix', 'probabilities', or 'state_vector'")
+# (C) Copyright 2023 Beijing Academy of Quantum Information Sciences
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#    http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+"""simulator for quantum circuit"""
+
+from ..elements import CircuitWrapper, QuantumGate, KrausChannel, UnitaryChannel
+from ..circuits import QuantumCircuit
+from abc  import ABC, abstractmethod
+from .qfvm import simulate_circuit, applyop_statevec, expect_statevec, sampling_statevec,simulate_circuit_clifford
+import numpy as np
+from ..exceptions import QuafuError
+from ..results.results import SimuResult
+from ..algorithms.hamiltonian import Hamiltonian
+
+class Simulator(ABC):
+    @abstractmethod
+    def run(self):
+        raise NotImplementedError
+    
+class SVSimulator(Simulator):
+    def __init__(self, use_gpu:bool=False, use_custatevec:bool=False):
+        self.use_gpu  = use_gpu
+        self.use_custatevec = use_custatevec
+
+    def config(self, **kwargs):
+        for attr, value in kwargs.items():
+            if hasattr(self, attr):
+                setattr(self, attr, value)
+            else:
+                raise ValueError("No such attribute")
+
+    def _apply_op(self, op, psi):
+        #TODO: support GPU
+        if isinstance(op,CircuitWrapper):
+            psi = self.run(op.circuit, psi)["statevector"]
+            return psi
+        elif isinstance(op, QuantumGate):
+            psi = applyop_statevec(op, psi)
+            return psi
+        elif isinstance(op, KrausChannel):
+            temppsi = np.copy(psi)
+            norm0 = np.linalg.norm(psi)
+            s = 0.
+            r = np.random.rand()
+            for kop in op.gatelist:
+                temppsi = applyop_statevec(kop, temppsi)
+                norm1 = np.linalg.norm(temppsi)
+                s += norm1 / norm0
+                if r < s:
+                    psi = temppsi
+                    psi = psi / norm1
+                    return psi
+                else:
+                    temppsi = np.copy(psi)
+            return psi
+        else:
+            raise NotImplementedError
+    
+    def _apply_hamil(self, hamil, psi):
+        psi_out = np.zeros(len(psi), dtype=complex) 
+        for pauli in hamil.paulis:
+            psi1 = np.copy(psi)
+            for name, pos in zip(pauli.paulistr, pauli.pos):
+                op = QuantumGate.gate_classes[name.lower()](pos)
+                psi1 = self._apply_op(op, psi1)
+            psi1 = psi1 * pauli.coeff
+            psi_out += psi1
+    
+        return psi_out
+
+    def run(self, qc : QuantumCircuit, psi : np.ndarray= np.array([]), shots:int=0, hamiltonian:Hamiltonian=None):
+        res_info = {}
+        if qc.noised:
+            raise QuafuError("Can not run noisy circuits with statevector simulator, please use the noisy version.")
+        
+        if self.use_gpu:
+            if qc.executable_on_backend == False:
+                raise QuafuError("classical operation do not support gpu currently")
+
+            if self.use_custatevec:
+                try:
+                    from .qfvm import simulate_circuit_custate
+                except ImportError:
+                    raise QuafuError("pyquafu isn't installed with cuquantum support")
+                psi = simulate_circuit_custate(qc, psi)
+                count_dict = sampling_statevec(qc.measures, psi, shots)
+                res_info["statevector"] = psi
+                res_info["counts"] = count_dict
+            else:
+                try:
+                    from .qfvm import simulate_circuit_gpu
+                except ImportError:
+                    raise QuafuError("you are not using the GPU version of pyquafu")
+                psi = simulate_circuit_gpu(qc, psi)
+                count_dict = sampling_statevec(qc.measures, psi, shots)
+        else:
+            count_dict, psi = simulate_circuit(qc, psi, shots)
+            res_info["statevector"] = psi
+            res_info["counts"] = count_dict
+
+        if hamiltonian:
+            paulis = hamiltonian.paulis
+            res = expect_statevec(res_info["statevector"], paulis)
+            for i in range(len(paulis)):
+                res[i] *= paulis[i].coeff
+            res_info["pauli_expects"] = res
+        else:
+            res_info["pauli_expects"] = []
+        res_info["qbitnum"] = qc.num
+        res_info["measures"] =  qc.measures
+        res_info["simulator"] = "statevector"
+        return SimuResult(res_info)
+
+class NoiseSVSimulator(Simulator):
+    def __init__(self, use_gpu:bool=False, use_custatevec:bool=False):
+        self.backend = SVSimulator(use_gpu=use_gpu, use_custatevec=use_custatevec)
+
+    def run_once(self, qc : QuantumCircuit, psi, hamiltonian=None):
+        newqc = self.gen_circuit(qc)
+        for op in newqc.instructions:
+            psi = self.backend._apply_op(op, psi)
+        sample = list(sampling_statevec(qc.measures, psi, 1).keys())[0]
+
+        if hamiltonian:
+            paulis = hamiltonian.paulis
+            res = expect_statevec(psi, paulis)
+            for i in range(len(paulis)):
+                res[i] *= paulis[i].coeff
+            return sample, res
+        return sample, None
+
+    def run(self, qc:QuantumCircuit,  psi : np.ndarray= np.array([]), shots:int=0, hamiltonian:Hamiltonian=None):
+        counts = {}
+        pauli_expects = 0.
+        
+        for _ in range(shots):
+            if not psi:
+                tpsi = np.zeros(2**qc.num, dtype=complex)
+                tpsi[0] = 1.0
+            else:
+                tpsi = np.copy(psi)
+            sample, pauli_res = self.run_once(qc, tpsi, hamiltonian)
+            if sample in counts.keys():
+                counts[sample] += 1
+            else:
+                counts[sample] = 1
+            if hamiltonian:
+                pauli_expects += np.array(pauli_res)
+        pauli_expects /= shots
+        if not hamiltonian:
+            pauli_expects = []
+        else:
+            pauli_expects = list(pauli_expects)
+        res_info = {"counts":counts, "pauli_expects": pauli_expects}
+        res_info["qbitnum"] = qc.num
+        res_info["measures"] =  qc.measures 
+        res_info["simulator"] = "noisy statevector"
+        return SimuResult(res_info)
+
+    @staticmethod
+    def gen_circuit(qc):
+        """
+        sample circuit from noise circuit
+        """ 
+        num = qc.num
+        new_qc = QuantumCircuit(num)
+        temp_qc = QuantumCircuit(num)
+        if qc._has_wrap:
+            qc.unwarp()
+
+        for op in qc.instructions:
+            if isinstance(op, QuantumGate):
+                temp_qc << op
+            elif isinstance(op, UnitaryChannel):
+                g = op.gen_gate()
+                if g.name != "ID":
+                    temp_qc << g
+            elif isinstance(op, KrausChannel):
+                new_qc << temp_qc.wrap()
+                new_qc << op
+                temp_qc =  QuantumCircuit(num)
+        new_qc << temp_qc.wrap()
+        return new_qc
+    
+class CliffordSimulator(Simulator):
+     def run(self, qc : QuantumCircuit, shots:int=0):
+        res_info = {}
+        count_dict = simulate_circuit_clifford(qc, shots)
+        res_info["qbitnum"] = qc.num
+        res_info["counts"] = count_dict
+        res_info["measures"] = qc.measures
+        res_info["simuator"] = "clifford"
+        return SimuResult(res_info)
+
```

## quafu/tasks/task_database.py

```diff
@@ -1,167 +1,176 @@
-# (C) Copyright 2023 Beijing Academy of Quantum Information Sciences
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#    http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import os
-import sqlite3
-from pathlib import Path
-
-
-def print_task_info(task):
-    """
-    Helper function to print task information.
-    """
-    task_id, group_name, task_name, status, priority, send_time, finish_time = task
-    print(f"Task ID: {task_id}")
-    print(f"Group Name: {group_name}")
-    print(f"Task Name: {task_name}")
-    print(f"Status: {status}")
-    print(f"Priority: {priority}")
-    print(f"Send Time: {send_time}")
-    print(f"Finish Time: {finish_time}")
-    print("------------------------")
-
-
-class QuafuTaskDatabase:
-    """
-    A helper class use sqlite3 database to handle information of quafu tasks at local equipment.
-    When initialized and called, it will connect a database file named 'tasks.db' (create new
-    one if not exist) at the specified directory. The database will contain a table named 'tasks'
-    in which every 'task' has a unique task_id. Other attributes include group name, task name,
-    status, priority and send time.
-
-    - Usage:
-    Use this class by 'with' statement. For example:
-    >>> with QuafuTaskDatabase(db_dir='./') as db:
-    ...     db.insert_task(1, "Done", group_name="Group 1", task_name="Task1", priority=2)
-    ...     print("Task list:")
-    ...     for task_info in db.find_all_tasks():
-    ...         print_task_info(task_info)
-    This way ensures the database connection is closed and submission committed automatically.
-    """
-
-    def __init__(self, db_dir='./'):
-        self.database_name = "tasks.db"
-        self.database_dir = Path(db_dir)
-        self.conn = None
-
-    def __enter__(self):
-        if not os.path.exists(self.database_dir):
-            os.makedirs(self.database_dir)
-        self.conn = sqlite3.connect(self.database_dir / self.database_name)
-        self._create_table()
-        return self
-
-    def __exit__(self, exc_type, exc_value, traceback):
-        if self.conn:
-            self.conn.commit()
-            self.conn.close()
-
-    def _create_table(self):
-        cursor = self.conn.cursor()
-        cursor.execute('''
-            CREATE TABLE IF NOT EXISTS tasks (
-                task_id TEXT PRIMARY KEY,
-                group_name TEXT DEFAULT NULL,
-                task_name TEXT DEFAULT NULL,
-                status TEXT,
-                priority INTEGER,
-                send_time TIMESTAMP,
-                finish_time TIMESTAMP DEFAULT NULL
-            )
-        ''')
-        cursor.close()
-
-    # region data manipulation
-    def insert_task(self,
-                    task_id,
-                    status,
-                    send_time: str = None,
-                    priority=2,
-                    group_name=None,
-                    task_name=None,
-                    finish_time: str = None
-                    ):
-        cursor = self.conn.cursor()
-        cursor.execute(
-            "INSERT INTO tasks "
-            "(task_id, group_name, task_name, status, priority, send_time, finish_time) "
-            "VALUES "
-            "(?, ?, ?, ?, ?, ?, ?)",
-            (task_id, group_name, task_name, status, priority, send_time, finish_time))
-        cursor.close()
-
-    def delete_task(self, task_id):
-        cursor = self.conn.cursor()
-        cursor.execute("DELETE FROM tasks WHERE task_id=?", (task_id,))
-        cursor.close()
-        print(f"Task {task_id} has been deleted from local database")
-
-    def update_task_status(self, task_id, status):
-        cursor = self.conn.cursor()
-        cursor.execute("UPDATE tasks SET status=? WHERE task_id=?", (status, task_id))
-        cursor.close()
-    # endregion
-
-    # region fetch tasks
-    def find_all_tasks(self):
-        cursor = self.conn.cursor()
-        cursor.execute("SELECT * FROM tasks")
-        tasks = cursor.fetchall()
-        cursor.close()
-        return tasks
-
-    def find_by_status(self, status):
-        cursor = self.conn.cursor()
-        cursor.execute("SELECT * FROM tasks WHERE status=?", (status,))
-        tasks = cursor.fetchall()
-        cursor.close()
-        return tasks
-
-    def find_by_priority(self, priority):
-        cursor = self.conn.cursor()
-        cursor.execute("SELECT * FROM tasks WHERE priority=?", (priority,))
-        tasks = cursor.fetchall()
-        cursor.close()
-        return tasks
-
-    def find_by_group(self, group_name):
-        cursor = self.conn.cursor()
-        if group_name is None:
-            cursor.execute("SELECT * FROM tasks WHERE group_name IS NULL")
-        else:
-            cursor.execute("SELECT * FROM tasks WHERE group_name=?", (group_name,))
-        tasks = cursor.fetchall()
-        cursor.close()
-        return tasks
-
-    def find_by_name(self, task_name):
-        cursor = self.conn.cursor()
-        if task_name is None:
-            cursor.execute("SELECT * FROM tasks WHERE task_name IS NULL")
-        else:
-            cursor.execute("SELECT * FROM tasks WHERE task_name=?", (task_name, ))
-        tasks = cursor.fetchall()
-        cursor.close()
-        return tasks
-
-    def find_by_time(self, start_time, end_time):
-        """
-        get tasks sent between start_time and end_time.
-        """
-        cursor = self.conn.cursor()
-        cursor.execute("SELECT * FROM tasks WHERE send_time BETWEEN ? AND ?", (start_time, end_time))
-        tasks = cursor.fetchall()
-        cursor.close()
-        return tasks
-    # endregion
+# (C) Copyright 2023 Beijing Academy of Quantum Information Sciences
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#    http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import os
+import sqlite3
+from pathlib import Path
+
+
+def print_task_info(task):
+    """
+    Helper function to print task information.
+    """
+    task_id, group_name, task_name, status, priority, send_time, finish_time = task
+    print(f"Task ID: {task_id}")
+    print(f"Group Name: {group_name}")
+    print(f"Task Name: {task_name}")
+    print(f"Status: {status}")
+    print(f"Priority: {priority}")
+    print(f"Send Time: {send_time}")
+    print(f"Finish Time: {finish_time}")
+    print("------------------------")
+
+
+class QuafuTaskDatabase:
+    """
+    A helper class use sqlite3 database to handle information of quafu tasks at local equipment.
+    When initialized and called, it will connect a database file named 'tasks.db' (create new
+    one if not exist) at the specified directory. The database will contain a table named 'tasks'
+    in which every 'task' has a unique task_id. Other attributes include group name, task name,
+    status, priority and send time.
+
+    - Usage:
+    Use this class by 'with' statement. For example:
+    >>> with QuafuTaskDatabase(db_dir='./') as db:
+    ...     db.insert_task(1, "Done", group_name="Group 1", task_name="Task1", priority=2)
+    ...     print("Task list:")
+    ...     for task_info in db.find_all_tasks():
+    ...         print_task_info(task_info)
+    This way ensures the database connection is closed and submission committed automatically.
+    """
+
+    def __init__(self, db_dir="./"):
+        self.database_name = "tasks.db"
+        self.database_dir = Path(db_dir)
+        self.conn = None
+
+    def __enter__(self):
+        if not os.path.exists(self.database_dir):
+            os.makedirs(self.database_dir)
+        self.conn = sqlite3.connect(self.database_dir / self.database_name)
+        self._create_table()
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        if self.conn:
+            self.conn.commit()
+            self.conn.close()
+
+    def _create_table(self):
+        cursor = self.conn.cursor()
+        cursor.execute(
+            """
+            CREATE TABLE IF NOT EXISTS tasks (
+                task_id TEXT PRIMARY KEY,
+                group_name TEXT DEFAULT NULL,
+                task_name TEXT DEFAULT NULL,
+                status TEXT,
+                priority INTEGER,
+                send_time TIMESTAMP,
+                finish_time TIMESTAMP DEFAULT NULL
+            )
+        """
+        )
+        cursor.close()
+
+    # region data manipulation
+    def insert_task(
+        self,
+        task_id,
+        status,
+        send_time: str = None,
+        priority=2,
+        group_name=None,
+        task_name=None,
+        finish_time: str = None,
+    ):
+        cursor = self.conn.cursor()
+        cursor.execute(
+            "INSERT INTO tasks "
+            "(task_id, group_name, task_name, status, priority, send_time, finish_time) "
+            "VALUES "
+            "(?, ?, ?, ?, ?, ?, ?)",
+            (task_id, group_name, task_name, status, priority, send_time, finish_time),
+        )
+        cursor.close()
+
+    def delete_task(self, task_id):
+        cursor = self.conn.cursor()
+        cursor.execute("DELETE FROM tasks WHERE task_id=?", (task_id,))
+        cursor.close()
+        print(f"Task {task_id} has been deleted from local database")
+
+    def update_task_status(self, task_id, status):
+        cursor = self.conn.cursor()
+        cursor.execute("UPDATE tasks SET status=? WHERE task_id=?", (status, task_id))
+        cursor.close()
+
+    # endregion
+
+    # region fetch tasks
+    def find_all_tasks(self):
+        cursor = self.conn.cursor()
+        cursor.execute("SELECT * FROM tasks")
+        tasks = cursor.fetchall()
+        cursor.close()
+        return tasks
+
+    def find_by_status(self, status):
+        cursor = self.conn.cursor()
+        cursor.execute("SELECT * FROM tasks WHERE status=?", (status,))
+        tasks = cursor.fetchall()
+        cursor.close()
+        return tasks
+
+    def find_by_priority(self, priority):
+        cursor = self.conn.cursor()
+        cursor.execute("SELECT * FROM tasks WHERE priority=?", (priority,))
+        tasks = cursor.fetchall()
+        cursor.close()
+        return tasks
+
+    def find_by_group(self, group_name):
+        cursor = self.conn.cursor()
+        if group_name is None:
+            cursor.execute("SELECT * FROM tasks WHERE group_name IS NULL")
+        else:
+            cursor.execute("SELECT * FROM tasks WHERE group_name=?", (group_name,))
+        tasks = cursor.fetchall()
+        cursor.close()
+        return tasks
+
+    def find_by_name(self, task_name):
+        cursor = self.conn.cursor()
+        if task_name is None:
+            cursor.execute("SELECT * FROM tasks WHERE task_name IS NULL")
+        else:
+            cursor.execute("SELECT * FROM tasks WHERE task_name=?", (task_name,))
+        tasks = cursor.fetchall()
+        cursor.close()
+        return tasks
+
+    def find_by_time(self, start_time, end_time):
+        """
+        get tasks sent between start_time and end_time.
+        """
+        cursor = self.conn.cursor()
+        cursor.execute(
+            "SELECT * FROM tasks WHERE send_time BETWEEN ? AND ?",
+            (start_time, end_time),
+        )
+        tasks = cursor.fetchall()
+        cursor.close()
+        return tasks
+
+    # endregion
```

## quafu/tasks/tasks.py

```diff
@@ -1,326 +1,351 @@
-# (C) Copyright 2023 Beijing Academy of Quantum Information Sciences
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#    http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import copy
-import logging
-from typing import Dict, List, Tuple
-from urllib import parse
-
-import numpy as np
-import requests
-
-from quafu.circuits.quantum_circuit import QuantumCircuit
-from quafu.users.userapi import User
-from ..exceptions import CircuitError, ServerError, CompileError
-from ..results.results import ExecResult, merge_measure
-from ..users.exceptions import UserError
-
-
-class Task(object):
-    """
-    Class for submitting quantum computation task to the backend.
-
-    Attributes:
-        shots (int): Numbers of single shot measurement.
-        compile (bool): Whether compile the circuit on the backend
-        tomo (bool): Whether do tomography (Not support yet)
-        user (User): User object corresponding to Quafu account
-        priority (int): priority level of the task
-        submit_history (dict): circuit submitted with this task
-        backend (dict): quantum backend that execute the task.
-
-    """
-
-    def __init__(self, user: User = None):
-        self.user = User() if user is None else user
-
-        self.shots = 1000
-        self.tomo = False
-        self.compile = True
-        self.priority = self.user.priority
-        self.runtime_job_id = ""
-        self.submit_history = {}
-        self._available_backends = self.user.get_available_backends(print_info=False)
-        self.backend = self._available_backends[list(self._available_backends.keys())[0]]
-
-    def config(self,
-               backend: str = "ScQ-P10",
-               shots: int = 1000,
-               compile: bool = True,
-               tomo: bool = False,
-               priority: int = 2) -> None:
-        """
-        Configure the task properties
-
-        Args:
-            backend: Select the experimental backend.
-            shots: Numbers of single shot measurement.
-            compile: Whether compile the circuit on the backend
-            tomo:  Whether to do tomography (Not support yet)
-            priority: Task priority.
-        """
-        if backend not in self._available_backends.keys():
-            raise UserError("backend %s is not valid, available backends are " % backend + ", ".join(
-                self._available_backends.keys()))
-
-        self.backend = self._available_backends[backend]
-        self.shots = shots
-        self.tomo = tomo
-        self.compile = compile
-        self.priority = priority
-
-    def get_history(self) -> Dict:
-        """
-        Get the history of submitted task.
-        Returns:
-            A dict of history. The key is the group name and the value is a list of task id in the group.
-        """
-        return self.submit_history
-
-    def get_backend_info(self) -> Dict:
-        """
-        Get the calibration information of the experimental backend.
-
-        Returns:
-            Backend information dictionary containing the mapping from the indices to the names of physical bits `'mapping'`, backend topology  `'topology_diagram'` and full calibration inforamtion `'full_info'`.
-        """
-        return self.backend.get_chip_info(self.user)
-
-    def submit(self,
-               qc: QuantumCircuit,
-               obslist: List = []) \
-            -> Tuple[List[ExecResult], List[int]]:
-        """
-        Execute the circuit with observable expectation measurement task.
-        Args:
-            qc (QuantumCircuit): Quantum circuit that need to be executed on backend.
-            obslist (list[str, list[int]]): List of pauli string and its position.
-
-        Returns:
-            List of executed results and list of measured observable
-
-        Examples:
-            1) input [["XYX", [0, 1, 2]], ["Z", [1]]] measure pauli operator XYX at 0, 1, 2 qubit, and Z at 1 qubit.\n
-            2) Measure 5-qubit Ising Hamiltonian we can use\n
-            obslist = [["X", [i]] for i in range(5)]]\n
-            obslist.extend([["ZZ", [i, i+1]] for i in range(4)])\n
-
-        For the energy expectation of Ising Hamiltonian \n
-        res, obsexp = q.submit_task(obslist)\n
-        E = sum(obsexp)
-        """
-        # save input circuit
-        inputs = copy.deepcopy(qc.gates)
-        measures = list(qc.measures.keys())
-        if len(obslist) == 0:
-            print("No observable measurement task.")
-            res = self.run(qc)
-            return res, []
-
-        else:
-            for obs in obslist:
-                for p in obs[1]:
-                    if p not in measures:
-                        raise CircuitError("Qubit %d in observer %s is not measured." % (p, obs[0]))
-
-            measure_basis, targlist = merge_measure(obslist)
-            print("Job start, need measured in ", measure_basis)
-
-            exec_res = []
-            for measure_base in measure_basis:
-                res = self.run(qc, measure_base=measure_base)
-                qc.gates = copy.deepcopy(inputs)
-                exec_res.append(res)
-
-            measure_results = []
-            for obi in range(len(obslist)):
-                obs = obslist[obi]
-                rpos = [measures.index(p) for p in obs[1]]
-                measure_results.append(exec_res[targlist[obi]].calculate_obs(rpos))
-
-        return exec_res, measure_results
-
-    def run(self,
-            qc: QuantumCircuit,
-            measure_base: List = None) -> ExecResult:
-        """Single run for measurement task.
-
-        Args:
-            qc (QuantumCircuit): Quantum circuit that need to be executed on backend.
-            measure_base (list[str, list[int]]): measure base and its positions.
-        """
-        if measure_base is None:
-            res = self.send(qc)
-            res.measure_base = ''
-
-        else:
-            for base, pos in zip(measure_base[0], measure_base[1]):
-                if base == "X":
-                    qc.ry(pos, -np.pi / 2)
-                elif base == "Y":
-                    qc.rx(pos, np.pi / 2)
-
-            res = self.send(qc)
-            res.measure_base = measure_base
-
-        return res
-
-    def send(self,
-             qc: QuantumCircuit,
-             name: str = "",
-             group: str = "",
-             wait: bool = True,
-             verbose: bool = False,
-             ) -> ExecResult:
-        """
-        Run the circuit on experimental device.
-
-        Args:
-            qc: Quantum circuit that need to be executed on backend.
-            name: Task name.
-            group: The task belong which group.
-            wait: Whether wait until the execution return.
-            verbose:
-        Returns:
-            ExecResult object that contain the dict return from quantum device.
-        """
-        from quafu import get_version
-        version = get_version()
-        if qc.num > self.backend.qubit_num:
-            raise CircuitError("The qubit number %d is too large for backend %s which has %d qubits" % (
-                qc.num, self.backend.name, self.backend.qubit_num))
-
-        self.check_valid_gates(qc)
-        qc.to_openqasm()
-        data = {"qtasm": qc.openqasm, "shots": self.shots, "qubits": qc.num, "scan": 0,
-                "tomo": int(self.tomo), "selected_server": self.backend.system_id,
-                "compile": int(self.compile), "priority": self.priority, "task_name": name,
-                "pyquafu_version": version, "runtime_job_id": self.runtime_job_id}
-
-        if wait:
-            url = User.exec_api
-        else:
-            url = User.exec_async_api
-
-        logging.debug('quantum circuit validated, sending task...')
-        headers = {'Content-Type': 'application/x-www-form-urlencoded;charset=UTF-8', 'api_token': self.user.api_token}
-        data = parse.urlencode(data)
-        data = data.replace("%27", "'")
-        response = requests.post(url, headers=headers, data=data)  # type: requests.models.Response
-
-        # TODO: completing status code checks
-        if not response.ok:
-            logging.warning("Received a non-200 response from the server.\n")
-        if response.status_code == 502:
-            logging.critical("Received a 502 Bad Gateway response. Please try again later.\n"
-                             "If there is persistent failure, please report it on our github page.")
-            raise UserError('502 Bad Gateway response')
-        else:
-            res_dict = response.json()  # type: dict
-            quafu_status = res_dict['status']
-            if verbose:
-                import pprint
-                pprint.pprint(res_dict)
-            if quafu_status in [201, 205]:
-                raise UserError(res_dict["message"])
-            elif quafu_status == 5001:
-                raise CircuitError(res_dict["message"])
-            elif quafu_status == 5003:
-                raise ServerError(res_dict["message"])
-            elif quafu_status == 5004:
-                raise CompileError(res_dict["message"])
-            else:
-                task_id = res_dict["task_id"]
-
-                if group not in self.submit_history:
-                    self.submit_history[group] = [task_id]
-                else:
-                    self.submit_history[group].append(task_id)
-
-                result = ExecResult(res_dict)
-                while wait and (self.shots > 0) and (not result.counts):
-                    if verbose:
-                        logging.warning('warning for quafu status: empty result.counts, retrieving task...')
-                    result = self.retrieve(result.taskid)
-                return result
-
-    def retrieve(self, taskid: str) -> ExecResult:
-        """
-        Retrieve the results of submited task by taskid.
-
-        Args:
-            taskid: The taskid of the task need to be retrieved.
-        """
-        data = {"task_id": taskid}
-        url = User.exec_recall_api
-
-        headers = {'Content-Type': 'application/x-www-form-urlencoded;charset=UTF-8', 'api_token': self.user.api_token}
-        response = requests.post(url, headers=headers, data=data)
-
-        res_dict = response.json()
-        return ExecResult(res_dict)
-
-    def retrieve_group(self,
-                       group: str,
-                       history: Dict = None,
-                       verbose: bool = True) -> List[ExecResult]:
-        """
-        Retrieve the results of submited task by group name.
-
-        Args:
-            group: The group name need to be retrieved.
-            history: History from which to retrieve the results. If not provided, the history will be the submit history of saved by current task.
-            verbose: Whether print the task status in the group.
-        Returns:
-            A list of execution results in the retrieved group. Only completed task will be added.
-        """
-        history = history if history else self.submit_history
-        taskids = history[group]
-
-        group_res = []
-        if verbose:
-            group = group if group else "Untitled group"
-            print("Group: ", group)
-            print((" " * 5).join(["task_id".ljust(16), "task_name".ljust(10), "status".ljust(10)]))
-        for taskid in taskids:
-            res = self.retrieve(taskid)
-            taskname = res.taskname
-            if verbose:
-                taskname = taskname if taskname else "Untitled"
-                print((" " * 5).join(
-                    [("%s" % res.taskid).ljust(16), ("%s" % taskname).ljust(10), ("%s" % res.task_status).ljust(10)]))
-            if res.task_status == "Completed":
-                group_res.append(res)
-
-        return group_res
-
-    def check_valid_gates(self, qc: QuantumCircuit) -> None:
-        """
-        Check the validity of the quantum circuit.
-        Args:
-            qc: QuantumCicuit object that need to be checked.
-        """
-        if not self.compile:
-            valid_gates = self.backend.get_valid_gates()
-            for gate in qc.gates:
-                if gate.name.lower() not in valid_gates:
-                    raise CircuitError("Invalid operations '%s' for backend '%s'" % (gate.name, self.backend.name))
-
-        else:
-            if self.backend.name == "ScQ-S41":
-                raise CircuitError("Backend ScQ-S41 must be used without compilation")
-            if self.backend.name == "ScQ-P136":
-                for gate in qc.gates:
-                    if gate.name.lower() in ["xy"]:
-                        raise CircuitError("Invalid operations '%s' for backend '%s'" % (gate.name, self.backend.name))
+# (C) Copyright 2023 Beijing Academy of Quantum Information Sciences
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#    http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import copy
+import logging
+from typing import Dict, List, Optional, Tuple
+from urllib import parse
+
+import numpy as np
+from quafu.circuits.quantum_circuit import QuantumCircuit
+from quafu.users.userapi import User
+
+from ..exceptions import CircuitError, UserError, validate_server_resp
+from ..results.results import ExecResult, merge_measure
+from ..utils.client_wrapper import ClientWrapper
+
+
+class Task:
+    """
+    Class for submitting quantum computation task to the backend.
+
+    Attributes:
+        shots (int): Numbers of single shot measurement.
+        compile (bool): Whether compile the circuit on the backend
+        tomo (bool): Whether do tomography (Not support yet)
+        user (User): User object corresponding to Quafu account
+        priority (int): priority level of the task
+        submit_history (dict): circuit submitted with this task
+        backend (dict): quantum backend that execute the task.
+
+    """
+
+    def __init__(self, user: Optional[User] = None):
+        self.user = User() if user is None else user
+
+        self.shots = 1000
+        self.tomo = False
+        self.compile = False
+        self.priority = self.user.priority
+        self.runtime_job_id = ""
+        self.submit_history = {}
+        self._available_backends = self.user.get_available_backends(print_info=False)
+        self.backend = self._available_backends[
+            list(self._available_backends.keys())[0]
+        ]
+
+    def config(
+        self,
+        backend: str = "ScQ-P10",
+        shots: int = 1000,
+        compile: bool = True,
+        tomo: bool = False,
+        priority: int = 2,
+    ) -> None:
+        """
+        Configure the task properties
+
+        Args:
+            backend: Select the experimental backend.
+            shots: Numbers of single shot measurement.
+            compile: Whether compile the circuit on the backend
+            tomo:  Whether to do tomography (Not support yet)
+            priority: Task priority.
+        """
+        if backend not in self._available_backends.keys():
+            raise UserError(
+                "backend %s is not valid, available backends are " % backend
+                + ", ".join(self._available_backends.keys())
+            )
+
+        self.backend = self._available_backends[backend]
+        self.shots = shots
+        self.tomo = tomo
+        self.compile = compile
+        self.priority = priority
+
+    def get_history(self) -> Dict:
+        """
+        Get the history of submitted task.
+        Returns:
+            A dict of history. The key is the group name and the value is a list of task id in the group.
+        """
+        return self.submit_history
+
+    def get_backend_info(self) -> Dict:
+        """
+        Get the calibration information of the experimental backend.
+
+        Returns:
+            Backend information dictionary containing the mapping from the indices to the names of physical bits `'mapping'`, backend topology  `'topology_diagram'` and full calibration inforamtion `'full_info'`.
+        """
+        return self.backend.get_chip_info(self.user)
+
+    def submit(
+        self, qc: QuantumCircuit, obslist: List = []
+    ) -> Tuple[List[ExecResult], List[int]]:
+        """
+        Execute the circuit with observable expectation measurement task.
+        Args:
+            qc (QuantumCircuit): Quantum circuit that need to be executed on backend.
+            obslist (list[str, list[int]]): List of pauli string and its position.
+
+        Returns:
+            List of executed results and list of measured observable
+
+        Examples:
+            1) input [["XYX", [0, 1, 2]], ["Z", [1]]] measure pauli operator XYX at 0, 1, 2 qubit, and Z at 1 qubit.\n
+            2) Measure 5-qubit Ising Hamiltonian we can use\n
+            obslist = [["X", [i]] for i in range(5)]]\n
+            obslist.extend([["ZZ", [i, i+1]] for i in range(4)])\n
+
+        For the energy expectation of Ising Hamiltonian \n
+        res, obsexp = q.submit_task(obslist)\n
+        E = sum(obsexp)
+        """
+        # save input circuit
+        inputs = copy.deepcopy(qc.gates)
+        measures = list(qc.measures.keys())
+        if len(obslist) == 0:
+            print("No observable measurement task.")
+            res = self.run(qc)
+            return res, []
+
+        else:
+            for obs in obslist:
+                for p in obs[1]:
+                    if p not in measures:
+                        raise CircuitError(
+                            "Qubit %d in observer %s is not measured." % (p, obs[0])
+                        )
+
+            measure_basis, targlist = merge_measure(obslist)
+            print("Job start, need measured in ", measure_basis)
+
+            exec_res = []
+            for measure_base in measure_basis:
+                res = self.run(qc, measure_base=measure_base)
+                qc.gates = copy.deepcopy(inputs)
+                exec_res.append(res)
+
+            measure_results = []
+            for obi in range(len(obslist)):
+                obs = obslist[obi]
+                rpos = [measures.index(p) for p in obs[1]]
+                measure_results.append(exec_res[targlist[obi]].calculate_obs(rpos))
+
+        return exec_res, measure_results
+
+    def run(self, qc: QuantumCircuit, measure_base: List = None) -> ExecResult:
+        """Single run for measurement task.
+
+        Args:
+            qc (QuantumCircuit): Quantum circuit that need to be executed on backend.
+            measure_base (list[str, list[int]]): measure base and its positions.
+        """
+        if measure_base is None:
+            res = self.send(qc)
+            res.measure_base = ""
+
+        else:
+            for base, pos in zip(measure_base[0], measure_base[1]):
+                if base == "X":
+                    qc.ry(pos, -np.pi / 2)
+                elif base == "Y":
+                    qc.rx(pos, np.pi / 2)
+
+            res = self.send(qc)
+            res.measure_base = measure_base
+
+        return res
+
+    def send(
+        self, qc: QuantumCircuit, name: str = "", group: str = "", wait: bool = False
+    ) -> ExecResult:
+        """
+        Run the circuit on experimental device.
+
+        Args:
+            qc: Quantum circuit that need to be executed on backend.
+            name: Task name.
+            group: The task belong which group.
+            wait: Whether wait until the execution return.
+        Returns:
+            ExecResult object that contain the dict return from quantum device.
+        """
+        from quafu import get_version
+
+        version = get_version()
+        if qc.num > self.backend.qubit_num:
+            raise CircuitError(
+                "The qubit number %d is too large for backend %s which has %d qubits"
+                % (qc.num, self.backend.name, self.backend.qubit_num)
+            )
+
+        if self.backend.name not in ["ScQ-P156", "ScQ-P106"]:
+            self.check_valid_gates(qc)
+        qc.to_openqasm()
+        data = {
+            "qtasm": qc.openqasm,
+            "shots": self.shots,
+            "qubits": qc.num,
+            "scan": 0,
+            "tomo": int(self.tomo),
+            "selected_server": self.backend.system_id,
+            "compile": int(self.compile),
+            "priority": self.priority,
+            "task_name": name,
+            "pyquafu_version": version,
+            "runtime_job_id": self.runtime_job_id,
+        }
+
+        if wait:
+            url = User.url + User.exec_api
+        else:
+            url = User.url + User.exec_async_api
+
+        logging.debug("quantum circuit validated, sending task...")
+        headers = {
+            "Content-Type": "application/x-www-form-urlencoded;charset=UTF-8",
+            "api_token": self.user.api_token,
+        }
+        data = parse.urlencode(data)
+        data = data.replace("%27", "'")
+        response = ClientWrapper.post(
+            url, headers=headers, data=data
+        )  # type: requests.models.Response
+
+        # TODO: completing status code checks
+        # FIXME: Maybe we need to delete below code
+        if not response.ok:
+            logging.warning("Received a non-200 response from the server.\n")
+        if response.status_code == 502:
+            logging.critical(
+                "Received a 502 Bad Gateway response. Please try again later.\n"
+                "If there is persistent failure, please report it on our github page."
+            )
+            raise UserError("502 Bad Gateway response")
+        # FIXME: Maybe we need to delete above code
+
+        res_dict = response.json()  # type: dict
+        validate_server_resp(res_dict)
+
+        task_id = res_dict["task_id"]
+
+        if group not in self.submit_history:
+            self.submit_history[group] = [task_id]
+        else:
+            self.submit_history[group].append(task_id)
+
+        return ExecResult(res_dict)
+
+    def retrieve(self, taskid: str) -> ExecResult:
+        """
+        Retrieve the results of submited task by taskid.
+
+        Args:
+            taskid: The taskid of the task need to be retrieved.
+        """
+        data = {"task_id": taskid}
+        url = User.url + User.exec_recall_api
+
+        headers = {
+            "Content-Type": "application/x-www-form-urlencoded;charset=UTF-8",
+            "api_token": self.user.api_token,
+        }
+        response = ClientWrapper.post(url, headers=headers, data=data)
+
+        res_dict = response.json()
+        return ExecResult(res_dict)
+
+    def retrieve_group(
+        self, group: str, history: Dict = None, verbose: bool = True
+    ) -> List[ExecResult]:
+        """
+        Retrieve the results of submited task by group name.
+
+        Args:
+            group: The group name need to be retrieved.
+            history: History from which to retrieve the results. If not provided, the history will be the submit history of saved by current task.
+            verbose: Whether print the task status in the group.
+        Returns:
+            A list of execution results in the retrieved group. Only completed task will be added.
+        """
+        history = history if history else self.submit_history
+        taskids = history[group]
+
+        group_res = []
+        if verbose:
+            group = group if group else "Untitled group"
+            print("Group: ", group)
+            print(
+                (" " * 5).join(
+                    ["task_id".ljust(16), "task_name".ljust(10), "status".ljust(10)]
+                )
+            )
+        for taskid in taskids:
+            res = self.retrieve(taskid)
+            taskname = res.taskname
+            if verbose:
+                taskname = taskname if taskname else "Untitled"
+                print(
+                    (" " * 5).join(
+                        [
+                            ("%s" % res.taskid).ljust(16),
+                            ("%s" % taskname).ljust(10),
+                            ("%s" % res.task_status).ljust(10),
+                        ]
+                    )
+                )
+            if res.task_status == "Completed":
+                group_res.append(res)
+
+        return group_res
+
+    def check_valid_gates(self, qc: QuantumCircuit) -> None:
+        """
+        Check the validity of the quantum circuit.
+        Args:
+            qc: QuantumCicuit object that need to be checked.
+        """
+        if not self.compile:
+            valid_gates = self.backend.get_valid_gates()
+            for gate in qc.gates:
+                if gate.name.lower() not in valid_gates:
+                    raise CircuitError(
+                        "Invalid operations '%s' for backend '%s'"
+                        % (gate.name, self.backend.name)
+                    )
+
+        else:
+            # TODO: use system_id for ScQ-S41
+            if self.backend.name == "ScQ-S41":
+                raise CircuitError("Backend ScQ-S41 must be used without compilation")
+            if self.backend.system_id == 2:  # ScQ-P136
+                for gate in qc.gates:
+                    if gate.name.lower() in ["xy"]:
+                        raise CircuitError(
+                            "Invalid operations '%s' for backend '%s'"
+                            % (gate.name, self.backend.name)
+                        )
```

## quafu/users/userapi.py

```diff
@@ -9,30 +9,32 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
+from typing import Optional
 
-import requests
-
-from .exceptions import UserError, APITokenNotFound
+from ..exceptions import APITokenNotFound, UserError, validate_server_resp
+from ..utils.client_wrapper import ClientWrapper
 from ..utils.platform import get_homedir
 
 
 class User(object):
     url = "https://quafu.baqis.ac.cn/"
-    backends_api = url + "qbackend/get_backends/"
-    chip_api = url + "qbackend/scq_get_chip_info/"
-    exec_api = url + "qbackend/scq_kit/"
-    exec_async_api = url + "qbackend/scq_kit_asyc/"
-    exec_recall_api = url + "qbackend/scq_task_recall/"
-
-    def __init__(self, api_token: str = None, token_dir: str = None):
+    backends_api = "qbackend/get_backends/"
+    chip_api = "qbackend/scq_get_chip_info/"
+    exec_api = "qbackend/scq_kit/"
+    exec_async_api = "qbackend/scq_kit_asyc/"
+    exec_recall_api = "qbackend/scq_task_recall/"
+
+    def __init__(
+        self, api_token: Optional[str] = None, token_dir: Optional[str] = None
+    ):
         """
         Initialize user account and load backend information.
 
         :param api_token: if provided
         :param token_dir: where api token is found or saved
         """
         self._available_backends = {}
@@ -48,28 +50,32 @@
             self._api_token = api_token
 
         self.priority = 2
 
     @property
     def api_token(self):
         if self._api_token is None:
-            raise APITokenNotFound(f"API token not set, neither found at dir: '{self.token_dir}'. "
-                                   "Please set up by providing api_token/token_dir when initializing User.")
+            raise APITokenNotFound(
+                f"API token not set, neither found at dir: '{self.token_dir}'. "
+                "Please set up by providing api_token/token_dir when initializing User."
+            )
         return self._api_token
 
     def save_apitoken(self, apitoken=None):
         """
         Save api-token associate your Quafu account.
         """
         if apitoken is not None:
             import warnings
-            warnings.warn("The argument 'apitoken' in this function will be deprecated "
-                          "in the future, please set api token by providing 'api_token' "
-                          "or 'token_dir' when initialize User()."
-                          )
+
+            warnings.warn(
+                "The argument 'apitoken' in this function will be deprecated "
+                "in the future, please set api token by providing 'api_token' "
+                "or 'token_dir' when initialize User()."
+            )
             self._api_token = apitoken
 
         file_dir = self.token_dir
         if not os.path.exists(file_dir):
             os.mkdir(file_dir)
         with open(file_dir + "api", "w") as f:
             f.write(self.api_token + "\n")
@@ -79,39 +85,49 @@
         """
         Load Quafu account, only api at present.
 
         TODO: expand to load more user information
         """
         file_dir = self.token_dir + "api"
         if not os.path.exists(file_dir):
-            return None
-        else:
-            f = open(file_dir, "r")
-            token = f.readline().strip()
+            raise UserError("Please first save api token using `User.save_apitoken()`")
+        with open(file_dir, "r") as f:
+            items = f.readlines()
+            token = items[0].strip()
+            self.__class__.url = items[1].strip()
         return token
 
     def _get_backends_info(self):
         """
         Get available backends information
         """
         headers = {"api_token": self.api_token}
-        response = requests.post(url=self.backends_api, headers=headers)
+        url = self.url + self.backends_api
+        response = ClientWrapper.post(url=url, headers=headers)
         backends_info = response.json()
-        if backends_info['status'] == 201:
-            raise UserError(backends_info["message"])
-        else:
-            return backends_info["data"]
+        validate_server_resp(backends_info)
+        return backends_info["data"]
 
     def get_available_backends(self, print_info=True):
         """
         Get available backends
         """
         from quafu.backends.backends import Backend
+
         backends_info = self._get_backends_info()
-        self._available_backends = {info["system_name"]: Backend(info) for info in backends_info}
+        self._available_backends = {
+            info["system_name"]: Backend(info) for info in backends_info
+        }
 
         if print_info:
             print("\t ".join(["system_name".ljust(10), "qubits".ljust(5), "status"]))
             for backend in self._available_backends.values():
-                print("\t ".join(
-                    [backend.name.ljust(10), str(backend.qubit_num).ljust(5), backend.status]))
+                print(
+                    "\t ".join(
+                        [
+                            backend.name.ljust(10),
+                            str(backend.qubit_num).ljust(5),
+                            backend.status,
+                        ]
+                    )
+                )
         return self._available_backends
```

## quafu/utils/basis.py

```diff
@@ -1,41 +1,46 @@
-import numpy as np
-
-def get_basis(ind, N):
-    basisstr = bin(int(ind))[2:]
-    basisstr = basisstr.zfill(N)
-    basis =  [int(i) for i in basisstr] 
-    return np.array(basis)
-
-def get_ind(basis):
-    biconv = 2**np.arange(len(basis))
-    ind = np.dot(basis, biconv[::-1].T)
-    return int(ind)
-    
-def reduce_probs(bitsA, res):
-    """The reduced probabilities from frequency """
-    dim = 2**(len(bitsA))
-    probs = np.zeros(dim)
-    for basestr in res:
-        basis = np.array([int(i) for i in basestr])
-        ind = get_ind(basis[bitsA])
-        probs[ind] += res[basestr]
-    
-    probs = probs/np.sum(probs)
-    return probs
-
-def measure_obs(bits, res):
-    n = len(bits)
-    baseobs = get_baselocal(n)
-    prob_r = reduce_probs(bits, res)
-    result = np.dot(prob_r, baseobs)
-    return result
-
-def get_baselocal(n):
-    NA = n
-    basisN = int(2**NA)
-    baseobs = np.zeros(basisN)
-    for i in range(basisN):
-        basisA = get_basis(i, NA)
-        baseobs[i] = (-1)**(np.sum(basisA))
-
-    return baseobs
+import numpy as np
+
+
+def get_basis(ind, N):
+    basisstr = bin(int(ind))[2:]
+    basisstr = basisstr.zfill(N)
+    basis = [int(i) for i in basisstr]
+    return np.array(basis)
+
+
+def get_ind(basis):
+    biconv = 2 ** np.arange(len(basis))
+    ind = np.dot(basis, biconv[::-1].T)
+    return int(ind)
+
+
+def reduce_probs(bitsA, res):
+    """The reduced probabilities from frequency"""
+    dim = 2 ** (len(bitsA))
+    probs = np.zeros(dim)
+    for basestr in res:
+        basis = np.array([int(i) for i in basestr])
+        ind = get_ind(basis[bitsA])
+        probs[ind] += res[basestr]
+
+    probs = probs / np.sum(probs)
+    return probs
+
+
+def measure_obs(bits, res):
+    n = len(bits)
+    baseobs = get_baselocal(n)
+    prob_r = reduce_probs(bits, res)
+    result = np.dot(prob_r, baseobs)
+    return result
+
+
+def get_baselocal(n):
+    NA = n
+    basisN = int(2**NA)
+    baseobs = np.zeros(basisN)
+    for i in range(basisN):
+        basisA = get_basis(i, NA)
+        baseobs[i] = (-1) ** (np.sum(basisA))
+
+    return baseobs
```

## quafu/utils/paulis.py

```diff
@@ -1,32 +1,37 @@
-import numpy as np
 from functools import reduce
+
+import numpy as np
 import sparse
 
-si = sparse.COO(np.array([[1., 0.],
-               [0., 1.]],dtype=complex))
+si = sparse.COO(np.array([[1.0, 0.0], [0.0, 1.0]], dtype=complex))
+
+sx = sparse.COO(np.array([[0.0, 1.0], [1.0, 0.0]], dtype=complex))
 
-sx = sparse.COO(np.array([[0., 1.],
-               [1., 0.]], dtype=complex))
+sy = sparse.COO(np.array([[0.0, -1.0j], [1.0j, 0.0]], dtype=complex))
 
-sy = sparse.COO(np.array([[0., -1.j],
-               [1.j, 0.]], dtype=complex)) 
+sz = sparse.COO(np.array([[1.0, 0.0], [0.0, -1.0]], dtype=complex))
 
-sz = sparse.COO(np.array([[1., 0.],    
-               [0., -1.]], dtype=complex))
+spin = [np.array([1.0, 0.0]), np.array([0.0, 1.0])]
 
-spin = [np.array([1., 0.]), np.array([0., 1.])]
 
 def rx(phi):
-    return np.array([[np.cos(phi / 2), -1j * np.sin(phi / 2)],
-                     [-1j * np.sin(phi / 2), np.cos(phi / 2)]])
-            
+    return np.array(
+        [
+            [np.cos(phi / 2), -1j * np.sin(phi / 2)],
+            [-1j * np.sin(phi / 2), np.cos(phi / 2)],
+        ]
+    )
+
+
 def ry(phi):
-    return np.array([[np.cos(phi / 2), -np.sin(phi / 2)],
-                     [np.sin(phi / 2), np.cos(phi / 2)]])
+    return np.array(
+        [[np.cos(phi / 2), -np.sin(phi / 2)], [np.sin(phi / 2), np.cos(phi / 2)]]
+    )
+
 
 def tensorl(ml):
     return reduce(sparse.kron, ml, 1)
 
 
 def Nbit_single(N):
     sx_list = []
@@ -43,8 +48,8 @@
 
         op_list[n] = sy
         sy_list.append(tensorl(op_list))
 
         op_list[n] = sz
         sz_list.append(tensorl(op_list))
 
-    return sx_list, sy_list, sz_list
+    return sx_list, sy_list, sz_list
```

## quafu/utils/platform.py

```diff
@@ -1,14 +1,17 @@
 import os
 import sys
+
 from ..exceptions import QuafuError
 
 
 def get_homedir():
-    if sys.platform == 'win32':
-        homedir = os.environ['USERPROFILE']
-    elif sys.platform == 'linux' or sys.platform == 'darwin':
-        homedir = os.environ['HOME']
+    if sys.platform == "win32":
+        homedir = os.environ["USERPROFILE"]
+    elif sys.platform == "linux" or sys.platform == "darwin":
+        homedir = os.environ["HOME"]
     else:
-        raise QuafuError(f'unsupported platform:{sys.platform}. '
-                         f'You may raise a request issue on github.')
+        raise QuafuError(
+            f"unsupported platform:{sys.platform}. "
+            f"You may raise a request issue on github."
+        )
     return homedir
```

## quafu/visualisation/circuitPlot.py

```diff
@@ -8,82 +8,104 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from typing import Dict
+
 import matplotlib.patheffects as pe
 import matplotlib.pyplot as plt
 import numpy as np
-from matplotlib.collections import PolyCollection, PatchCollection, LineCollection
-from matplotlib.patches import Circle, Arc
+from matplotlib.collections import (
+    LineCollection,
+    PatchCollection,
+    PathCollection,
+    PolyCollection,
+)
+from matplotlib.patches import Arc, Circle
+from matplotlib.path import Path
 from matplotlib.text import Text
-from quafu.elements import Instruction, ControlledGate
-from typing import Dict
+from quafu.elements import ControlledGate, Instruction
 
-from matplotlib.path import Path
-from matplotlib.collections import PathCollection
 # this line for developers only
 # from quafu.circuits.quantum_circuit import QuantumCircuit
 
 line_args = {}
 box_args = {}
 
-DEEPCOLOR = '#0C161F'
-BLUE = '#1f77b4'
-ORANGE = '#ff7f0e'
-GREEN = '#2ca02c'
-GOLDEN = '#FFB240'
-GARNET = '#C0392B'
-
+DEEPCOLOR = "#0C161F"
+BLUE = "#1f77b4"
+ORANGE = "#ff7f0e"
+GREEN = "#2ca02c"
+GOLDEN = "#FFB240"
+GARNET = "#C0392B"
 """
 layers(zorder):
 
 0: figure
 1: bkg box
 2: wires
 3: closed patches
 4: white bkg for label/text
 5: labels
 """
 
-su2_gate_names = ['x', 'y', 'z', 'id', 'w',
-                  'h', 't', 'tdg', 's', 'sdg', 'sx', 'sy', 'sw', 'sxdg', 'sydg', 'swdg',
-                  'p',
-                  'rx', 'ry', 'rz',
-                  ]
-
-swap_gate_names = ['swap', 'iswap']
-r2_gate_names = ['rxx', 'ryy', 'rzz']
-c2_gate_names = ['cp', 'cs', 'ct', 'cx', 'cy', 'cz']
-c3_gate_names = ['fredkin', 'toffoli']
-mc_gate_names = ['mcx', 'mcy', 'mcz']
-operation_names = ['barrier', 'delay']
+su2_gate_names = [
+    "x",
+    "y",
+    "z",
+    "id",
+    "w",
+    "h",
+    "t",
+    "tdg",
+    "s",
+    "sdg",
+    "sx",
+    "sy",
+    "sw",
+    "sxdg",
+    "sydg",
+    "swdg",
+    "p",
+    "rx",
+    "ry",
+    "rz",
+]
+
+swap_gate_names = ["swap", "iswap"]
+r2_gate_names = ["rxx", "ryy", "rzz"]
+c2_gate_names = ["cp", "cs", "ct", "cx", "cy", "cz"]
+c3_gate_names = ["fredkin", "toffoli"]
+mc_gate_names = ["mcx", "mcy", "mcz"]
+operation_names = ["barrier", "delay"]
 
 
 class CircuitPlotManager:
     """
     A class to manage the plotting of quantum circuits.
     Stores style parameters and provides functions to plot.
 
     To be initialized when circuit.plot() is called.
     """
+
     # colors
-    _wire_color = '#FF0000'
-    _light_blue = '#3B82F6'
+    _wire_color = "#FF0000"
+    _light_blue = "#3B82F6"
     _ec = DEEPCOLOR
 
     _wire_lw = 1.5
 
     _a_inch = 2 / 2.54  # physical lattice constant in inch
     _a = 0.5  # box width and height, unit: ax
     _barrier_width = _a / 3  # barrier width
 
-    _stroke = pe.withStroke(linewidth=2, foreground='white')
+    _stroke = pe.withStroke(linewidth=2, foreground="white")
 
     def __init__(self, qc):
         """
         Processing graphical info from a quantum circuit, decompose every
         gate/instruction into graphical elements and send the latter into
         corresponding containers.
 
@@ -123,29 +145,33 @@
 
         self.depth = np.max(self.dorders) + 1
 
         for q, c in qc.measures.items():
             self._proc_measure(self.depth - 1, q)
 
         # step2: initialize bit-label
-        self.q_label = {y: r'$|q_{%d}\rangle$' % i for i, y in self.used_qbit_y.items()}
-        self.c_label = {self.used_qbit_y[iq]: r'c_{%d}' % ic for iq, ic in qc.measures.items()}
+        self.q_label = {y: r"$|q_{%d}\rangle$" % i for i, y in self.used_qbit_y.items()}
+        self.c_label = {
+            self.used_qbit_y[iq]: r"c_{%d}" % ic for iq, ic in qc.measures.items()
+        }
 
         # step3: figure coordination
         self.xs = np.arange(-3 / 2, self.depth + 3 / 2)
         self.ys = np.arange(-2, self.used_qbit_num + 1 / 2)
 
-    def __call__(self,
-                 title=None,
-                 init_labels=None,
-                 end_labels=None,
-                 save_path: str = None,
-                 show: bool = False,
-                 *args,
-                 **kwargs):
+    def __call__(
+        self,
+        title=None,
+        init_labels=None,
+        end_labels=None,
+        save_path: str = None,
+        show: bool = False,
+        *args,
+        **kwargs,
+    ):
         """
         :param title
         :param init_labels: dict, {qbit: label}
         :param end_labels: dict, {qbit: label}
         :param save_path: str, path to save the figure
         :param show: bool, whether to show the figure
         :param args:
@@ -154,72 +180,80 @@
         More customization will be supported in the future.(TODO)
         """
         # Not supported by patch collections?
         # if 'xkcd' in kwargs:
         #     import random
         #     plt.gca().xkcd(randomness=random.randint(0, 1000))
         if title is not None:
-            title = Text((self.xs[0] + self.xs[-1]) / 2, -0.8,
-                         title,
-                         size=30,
-                         ha='center', va='baseline')
+            title = Text(
+                (self.xs[0] + self.xs[-1]) / 2,
+                -0.8,
+                title,
+                size=30,
+                ha="center",
+                va="baseline",
+            )
             self._text_list.append(title)
 
         # initialize a figure
         _size_x = self._a_inch * abs(self.xs[-1] - self.xs[0])
         _size_y = self._a_inch * abs(self.ys[-1] - self.ys[0])
         fig = plt.figure(figsize=(_size_x, _size_y))  # inch
-        ax = fig.add_axes([0, 0, 1, 1],
-                          aspect=1,
-                          xlim=[self.xs[0], self.xs[-1]],
-                          ylim=[self.ys[0], self.ys[-1]],
-                          )
-        ax.axis('off')
+        ax = fig.add_axes(
+            [0, 0, 1, 1],
+            aspect=1,
+            xlim=[self.xs[0], self.xs[-1]],
+            ylim=[self.ys[0], self.ys[-1]],
+        )
+        ax.axis("off")
         ax.invert_yaxis()
 
         self._circuit_wires()
         self._inits_label(labels=init_labels)
         self._measured_label(labels=end_labels)
         self._render_circuit()
 
         if save_path is not None:
-            plt.savefig(save_path, dpi=300, bbox_inches='tight')
+            plt.savefig(save_path, dpi=300, bbox_inches="tight")
         if show:
             plt.show()
 
     def _process_ins(self, ins: Instruction, append: bool = True):
-        name = ins.name
-        assert name in Instruction.ins_classes, 'If this should occur, please report a bug.'
+        name = ins.name.lower()
+        assert name in Instruction.ins_classes, (
+            "Name: %s not registered, if this should occur, please report a bug." % name
+        )
 
-        name = name.lower()
         _which = slice(np.min(ins.pos), np.max(ins.pos) + 1)
         depth = np.max(self.dorders[_which])
         paras = ins.paras
 
-        if name == 'barrier':
+        if name == "barrier":
             self._proc_barrier(depth, ins.pos)
-        elif name == 'measure':
+        elif name == "measure":
             self._proc_measure(depth, ins.pos)
         elif name in su2_gate_names:
-            self._proc_su2(name, depth, ins.pos, paras)
+            self._proc_su2(name, depth, ins.pos[0], paras)
         elif name in swap_gate_names:
-            self._proc_swap(depth, ins.pos, name == 'iswap')
+            self._proc_swap(depth, ins.pos, name == "iswap")
         elif name in r2_gate_names:
             # TODO: combine into one box
             self._ctrl_wire_points.append([[depth, ins.pos[0]], [depth, ins.pos[1]]])
 
             self._proc_su2(name[:-1], depth, min(ins.pos), None)
             self._proc_su2(name[:-1], depth, max(ins.pos), paras)
         elif isinstance(ins, ControlledGate):
             self._proc_ctrl(depth, ins)
-        elif name == 'delay':
+        elif name == "delay":
             self._delay(depth, ins.pos, ins.duration, ins.unit)
         else:
-            raise NotImplementedError(f'Gate {name} is not supported yet.\n'
-                                      f'If this should occur, please report a bug.')
+            raise NotImplementedError(
+                f"Gate {name} is not supported yet.\n"
+                f"If this should occur, please report a bug."
+            )
         if append:
             self.dorders[_which] = depth + 1
 
     #########################################################################
     # Helper functions for processing gates/instructions into graphical
     # elements. Add only points data of for the following collection-wise
     # plotting if possible, create a patch otherwise.
@@ -230,158 +264,176 @@
         """
         for pos, y in self.used_qbit_y.items():
             x0 = self.xs[0] + 1
             x1 = self.xs[-1] - 1
             self._h_wire_points.append([[x0, y], [x1, y]])
 
     def _inits_label(self, labels: Dict[int, str] = None):
-        """ qubit-labeling """
+        """qubit-labeling"""
         if labels is None:
             labels = self.q_label
 
         for i, label in labels.items():
-            txt = Text(-2 / 3, i,
-                       label,
-                       size=18,
-                       color=DEEPCOLOR,
-                       ha='right',
-                       va='center',
-                       )
+            txt = Text(
+                -2 / 3,
+                i,
+                label,
+                size=18,
+                color=DEEPCOLOR,
+                ha="right",
+                va="center",
+            )
             self._text_list.append(txt)
 
     def _measured_label(self, labels: Dict[int, str] = None):
-        """ measured qubit-labeling """
+        """measured qubit-labeling"""
         if labels is None:
             labels = self.c_label
 
         for i, label in labels.items():
-            label = r'$%s$' % label
-            txt = Text(self.xs[-1] - 3 / 4, i,
-                       label,
-                       size=18,
-                       color=DEEPCOLOR,
-                       ha='left',
-                       va='center',
-                       )
+            label = r"$%s$" % label
+            txt = Text(
+                self.xs[-1] - 3 / 4,
+                i,
+                label,
+                size=18,
+                color=DEEPCOLOR,
+                ha="left",
+                va="center",
+            )
             self._text_list.append(txt)
 
     def _gate_bbox(self, x, y, fc: str):
-        """ Single qubit gate box """
+        """Single qubit gate box"""
         a = self._a
         from matplotlib.patches import FancyBboxPatch
-        bbox = FancyBboxPatch((-a / 2 + x, -a / 2 + y), a, a,  # this warning belongs to matplotlib
-                              boxstyle=f'round, pad={0.2 * a}',
-                              edgecolor=DEEPCOLOR,
-                              facecolor=fc,
-                              )
+
+        bbox = FancyBboxPatch(
+            (-a / 2 + x, -a / 2 + y),
+            a,
+            a,  # this warning belongs to matplotlib
+            boxstyle=f"round, pad={0.2 * a}",
+            edgecolor=DEEPCOLOR,
+            facecolor=fc,
+        )
         self._closed_patches.append(bbox)
 
     def _gate_label(self, x, y, s):
         if not s:
             return None
         _dy = 0.05
-        text = Text(x, y + _dy,
-                    s,
-                    size=24,
-                    color=DEEPCOLOR,
-                    ha='center',
-                    va='center',
-                    )
+        text = Text(
+            x,
+            y + _dy,
+            s,
+            size=24,
+            color=DEEPCOLOR,
+            ha="center",
+            va="center",
+        )
         text.set_path_effects([self._stroke])
         self._text_list.append(text)
 
     def _para_label(self, x, y, para_txt):
-        """ label parameters """
+        """label parameters"""
         if not para_txt:
             return None
         _dx = 0
-        text = Text(x + _dx, y + 0.8 * self._a,
-                    para_txt,
-                    size=12,
-                    color=DEEPCOLOR,
-                    ha='center',
-                    va='top',
-                    )
+        text = Text(
+            x + _dx,
+            y + 0.8 * self._a,
+            para_txt,
+            size=12,
+            color=DEEPCOLOR,
+            ha="center",
+            va="top",
+        )
         self._text_list.append(text)
 
     def _measure_label(self, x, y):
         from matplotlib.patches import FancyArrow
+
         a = self._a
         r = 1.1 * a
         d = 1.2 * a / 3.5
 
-        arrow = FancyArrow(x=x,
-                           y=y + d,
-                           dx=0.15,
-                           dy=-0.35,
-                           width=0.04,
-                           facecolor=DEEPCOLOR,
-                           head_width=0.07,
-                           head_length=0.15,
-                           edgecolor='white')
-        arc = Arc((x, y + d),
-                  width=r,
-                  height=r,
-                  lw=1,
-                  theta1=180,
-                  theta2=0,
-                  fill=False,
-                  zorder=4,
-                  color=DEEPCOLOR,
-                  capstyle='round',
-                  )
-        center_bkg = Circle((x, y + d),
-                            radius=0.035,
-                            color='white',
-                            )
-        center = Circle((x, y + d),
-                        radius=0.025,
-                        facecolor=DEEPCOLOR,
-                        )
+        arrow = FancyArrow(
+            x=x,
+            y=y + d,
+            dx=0.15,
+            dy=-0.35,
+            width=0.04,
+            facecolor=DEEPCOLOR,
+            head_width=0.07,
+            head_length=0.15,
+            edgecolor="white",
+        )
+        arc = Arc(
+            (x, y + d),
+            width=r,
+            height=r,
+            lw=1,
+            theta1=180,
+            theta2=0,
+            fill=False,
+            zorder=4,
+            color=DEEPCOLOR,
+            capstyle="round",
+        )
+        center_bkg = Circle(
+            (x, y + d),
+            radius=0.035,
+            color="white",
+        )
+        center = Circle(
+            (x, y + d),
+            radius=0.025,
+            facecolor=DEEPCOLOR,
+        )
         self._mea_arc_patches.append(arc)
         self._mea_point_patches += [center_bkg, arrow, center]
 
     #########################################################################
     # region # # # # processing-functions: decompose ins into graphical elements # # #
     def _proc_su2(self, id_name, depth, pos, paras):
-        if id_name in ['x', 'y', 'z', 'h', 'id', 's', 't', 'p', 'w']:
-            fc = '#EE7057'
+        if id_name in ["x", "y", "z", "h", "id", "s", "t", "p", "w"]:
+            fc = "#EE7057"
             label = id_name.capitalize()[0]
-        elif id_name in ['sw', 'swdg', 'sx', 'sxdg', 'sy', 'sydg']:
-            fc = '#EE7057'
-            if id_name[-2:] == 'dg':
-                label = r'$\sqrt{%s}^\dagger$' % id_name[1]
+        elif id_name in ["sw", "swdg", "sx", "sxdg", "sy", "sydg"]:
+            fc = "#EE7057"
+            if id_name[-2:] == "dg":
+                label = r"$\sqrt{%s}^\dagger$" % id_name[1]
             else:
-                label = r'$\sqrt{%s}$' % id_name[1]
-        elif id_name in ['sdg', 'tdg']:
-            fc = '#EE7057'
-            label = id_name[0] + r'$^\dagger$'
-        elif id_name in ['rx', 'ry', 'rz']:
-            fc = '#6366F1'
+                label = r"$\sqrt{%s}$" % id_name[1]
+        elif id_name in ["sdg", "tdg"]:
+            fc = "#EE7057"
+            label = id_name[0] + r"$^\dagger$"
+        elif id_name in ["rx", "ry", "rz"]:
+            fc = "#6366F1"
             label = id_name.upper()
         else:
-            fc = '#8C9197'
-            label = '?'
+            fc = "#8C9197"
+            label = "?"
 
-        if id_name in ['rx', 'ry', 'rz', 'p']:
+        if id_name in ["rx", "ry", "rz", "p"]:
             # too long to display: r'$\theta=$' + f'{paras:.3f}' (TODO)
-            para_txt = f'({paras:.3f})' if paras else None
+            para_txt = f"({paras[0]:.3f})" if paras else None
         else:
             para_txt = None
 
         x = depth
         y = self.used_qbit_y[pos]
         self._gate_label(x=x, y=y, s=label)
         self._para_label(x=x, y=y, para_txt=para_txt)
         self._gate_bbox(x=x, y=y, fc=fc)
 
     def _delay(self, depth, pos, paras, unit):
         fc = BLUE
 
-        para_txt = '%d%s' % (paras, unit)
+        para_txt = "%d%s" % (paras, unit)
 
         x = depth
         y = self.used_qbit_y[pos]
         xs = self._a * np.array([-1, 0, 1, -1, 0, 1, -1, 0]) / 4 + x
         ys = self._a * np.array([1, 0, -1, -1, 0, 1, 1, 0]) / 3 + y
         self._white_path_points.append(np.column_stack((xs, ys)))
         self._para_label(x=x, y=y, para_txt=para_txt)
@@ -397,28 +449,31 @@
         for c in ctrl_pos:
             x = self.used_qbit_y[c]
             self._ctrl_points.append((depth, x, ctrl_type))
 
         # target part
         name = ins.name.lower()
         if ins.ct_nums == (1, 1, 2) or name in mc_gate_names:
-            tar_name = ins.targ_name.lower()[-1]
+            tar_name = ins._targ_name.lower()[-1]
             pos = ins.targs if isinstance(ins.targs, int) else ins.targs[0]
             x = self.used_qbit_y[pos]
-            if tar_name == 'x':
+            if tar_name == "x":
                 self._not_points.append((depth, x))
             else:
                 self._proc_su2(tar_name, depth, pos, ins.paras)
-        elif name == 'cswap':
+        elif name == "cswap":
             self._swap_points += [[depth, self.used_qbit_y[p]] for p in ins.targs]
-        elif name == 'ccx':
+        elif name == "ccx":
             self._not_points.append((depth, self.used_qbit_y[ins.targs[0]]))
         else:
             from quafu.elements.element_gates import ControlledU
-            assert isinstance(ins, ControlledU), f'unknown gate: {name}, {ins.__class__.__name__}'
+
+            assert isinstance(
+                ins, ControlledU
+            ), f"unknown gate: {name}, {ins.__class__.__name__}"
             self._process_ins(ins, append=False)
 
     def _proc_swap(self, depth, pos, iswap: bool = False):
         p1, p2 = pos
         x1, x2 = self.used_qbit_y[p1], self.used_qbit_y[p2]
         nodes = [[depth, x] for x in [x1, x2]]
         self._swap_points += nodes
@@ -428,16 +483,16 @@
 
     def _proc_barrier(self, depth, pos: list):
         x0 = depth - self._barrier_width
         x1 = depth + self._barrier_width
 
         for p in pos:
             y = self.used_qbit_y[p]
-            y0 = (y - 1 / 2)
-            y1 = (y + 1 / 2)
+            y0 = y - 1 / 2
+            y1 = y + 1 / 2
             nodes = [[x0, y0], [x0, y1], [x1, y1], [x1, y0], [x0, y0]]
             self._barrier_points.append(nodes)
 
     def _proc_measure(self, depth, pos: int):
         fc = GOLDEN
         y = self.used_qbit_y[pos]
         x = depth
@@ -445,151 +500,158 @@
         self._measure_label(x, y)
 
         # TODO: decide whether to draw double wire for measurement
         # y = pos + 0.02
         # x0 = depth
         # x1 = self.depth - 1 / 2
         # self._h_wire_points.append([[x0, y], [x1, y]])
+
     # endregion
     #########################################################################
 
     #########################################################################
     # # # # # # # # # # # # # # rendering functions # # # # # # # # # # # # #
     #########################################################################
     def _render_h_wires(self):
-        h_lines = LineCollection(self._h_wire_points,
-                                 zorder=0,
-                                 colors=self._wire_color,
-                                 alpha=0.8,
-                                 linewidths=2,
-                                 )
+        h_lines = LineCollection(
+            self._h_wire_points,
+            zorder=0,
+            colors=self._wire_color,
+            alpha=0.8,
+            linewidths=2,
+        )
         plt.gca().add_collection(h_lines)
 
     def _render_ctrl_wires(self):
-        v_lines = LineCollection(self._ctrl_wire_points,
-                                 zorder=0,
-                                 colors=self._light_blue,
-                                 alpha=0.8,
-                                 linewidths=4,
-                                 )
+        v_lines = LineCollection(
+            self._ctrl_wire_points,
+            zorder=0,
+            colors=self._light_blue,
+            alpha=0.8,
+            linewidths=4,
+        )
         plt.gca().add_collection(v_lines)
 
     def _render_closed_patch(self):
-        collection = PatchCollection(self._closed_patches,
-                                     match_original=True,
-                                     zorder=3,
-                                     ec=self._ec,
-                                     linewidths=0.5,
-                                     )
+        collection = PatchCollection(
+            self._closed_patches,
+            match_original=True,
+            zorder=3,
+            ec=self._ec,
+            linewidths=0.5,
+        )
         plt.gca().add_collection(collection)
 
     def _render_ctrl_nodes(self):
         circle_collection = []
         r = self._a / 4
         for x, y, ctrl in self._ctrl_points:
-            fc = '#3B82F6' if ctrl else 'white'
+            fc = "#3B82F6" if ctrl else "white"
             circle = Circle((x, y), radius=r, fc=fc)
             circle_collection.append(circle)
-        circles = PatchCollection(circle_collection,
-                                  match_original=True,
-                                  zorder=5,
-                                  ec=self._ec,
-                                  linewidths=2,
-                                  )
+        circles = PatchCollection(
+            circle_collection,
+            match_original=True,
+            zorder=5,
+            ec=self._ec,
+            linewidths=2,
+        )
         plt.gca().add_collection(circles)
 
     def _render_not_nodes(self):
         points = []
         rp = self._a * 0.3
         r = self._a * 0.5
 
         for x, y in self._not_points:
             points.append([[x, y - rp], [x, y + rp]])
             points.append([[x - rp, y], [x + rp, y]])
-            circle = Circle((x, y), radius=r, lw=1,
-                            fc='#3B82F6')
+            circle = Circle((x, y), radius=r, lw=1, fc="#3B82F6")
             self._closed_patches.append(circle)
 
-        collection = LineCollection(points,
-                                    zorder=5,
-                                    colors='white',
-                                    linewidths=2,
-                                    capstyle='round',
-                                    )
+        collection = LineCollection(
+            points,
+            zorder=5,
+            colors="white",
+            linewidths=2,
+            capstyle="round",
+        )
         plt.gca().add_collection(collection)
 
     def _render_swap_nodes(self):
         points = []
         r = self._a / (4 ** (1 / 2))
         for x, y in self._swap_points:
             points.append([[x - r, y - r], [x + r, y + r]])
             points.append([[x + r, y - r], [x - r, y + r]])
-        collection = LineCollection(points,
-                                    zorder=5,
-                                    colors='#3B82F6',
-                                    linewidths=4,
-                                    capstyle='round',
-                                    )
+        collection = LineCollection(
+            points,
+            zorder=5,
+            colors="#3B82F6",
+            linewidths=4,
+            capstyle="round",
+        )
         plt.gca().add_collection(collection)
 
         # iswap-cirlces
         i_circles = []
         for x, y in self._iswap_points:
-            circle = Circle((x, y), radius=2 ** (1 / 2) * r, lw=3,
-                            ec='#3B82F6', fill=False)
+            circle = Circle(
+                (x, y), radius=2 ** (1 / 2) * r, lw=3, ec="#3B82F6", fill=False
+            )
             i_circles.append(circle)
-        collection = PatchCollection(i_circles,
-                                     match_original=True,
-                                     zorder=5,
-                                     )
+        collection = PatchCollection(
+            i_circles,
+            match_original=True,
+            zorder=5,
+        )
         plt.gca().add_collection(collection)
 
     def _render_measure(self):
-        stroke = pe.withStroke(linewidth=4, foreground='white')
-        arcs = PatchCollection(self._mea_arc_patches,
-                               match_original=True,
-                               capstyle='round',
-                               zorder=4)
+        stroke = pe.withStroke(linewidth=4, foreground="white")
+        arcs = PatchCollection(
+            self._mea_arc_patches, match_original=True, capstyle="round", zorder=4
+        )
         arcs.set_path_effects([stroke])
 
         plt.gca().add_collection(arcs)
-        pointers = PatchCollection(self._mea_point_patches,  # note the order
-                                   match_original=True,
-                                   zorder=5,
-                                   facecolors=DEEPCOLOR,
-                                   linewidths=2,
-                                   )
+        pointers = PatchCollection(
+            self._mea_point_patches,  # note the order
+            match_original=True,
+            zorder=5,
+            facecolors=DEEPCOLOR,
+            linewidths=2,
+        )
         plt.gca().add_collection(pointers)
 
     def _render_barrier(self):
-        barrier = PolyCollection(self._barrier_points,
-                                 closed=True,
-                                 fc='lightgray',
-                                 hatch='///',
-                                 zorder=4)
+        barrier = PolyCollection(
+            self._barrier_points, closed=True, fc="lightgray", hatch="///", zorder=4
+        )
         plt.gca().add_collection(barrier)
 
     def _render_txt(self):
         for txt in self._text_list:
             plt.gca().add_artist(txt)
 
     def _render_white_path(self):
-        path_collection = PathCollection([Path(points) for points in self._white_path_points],
-                                         facecolor='none',
-                                         edgecolor='white',
-                                         zorder=4,
-                                         linewidth=2)
+        path_collection = PathCollection(
+            [Path(points) for points in self._white_path_points],
+            facecolor="none",
+            edgecolor="white",
+            zorder=4,
+            linewidth=2,
+        )
         plt.gca().add_collection(path_collection)
 
     def _render_circuit(self):
         self._render_h_wires()
         self._render_ctrl_wires()
         self._render_ctrl_nodes()
         self._render_not_nodes()
 
         self._render_swap_nodes()
         self._render_measure()
         self._render_barrier()
         self._render_closed_patch()
         self._render_white_path()
         self._render_txt()
-
```

## Comparing `pyquafu-0.3.6.dist-info/LICENSE` & `pyquafu-0.4.0.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -194,8 +194,8 @@
 
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
-   limitations under the License.
+   limitations under the License.
```

