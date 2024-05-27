# Comparing `tmp/libdaw-0.6.0.tar.gz` & `tmp/libdaw-0.7.0.tar.gz`

## Comparing `libdaw-0.6.0.tar` & `libdaw-0.7.0.tar`

### file list

```diff
@@ -1,152 +1,157 @@
--rw-r--r--   0     1001      127      427 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/Cargo.toml
--rw-r--r--   0     1001      127     1879 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/lib.rs
--rw-r--r--   0     1001      127      281 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/metronome/parse.rs
--rw-r--r--   0     1001      127     9873 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/metronome.rs
--rw-r--r--   0     1001      127      531 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/nodes/add.rs
--rw-r--r--   0     1001      127      870 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/nodes/constant_value.rs
--rw-r--r--   0     1001      127     1987 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/nodes/delay.rs
--rw-r--r--   0     1001      127     2253 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/nodes/detune.rs
--rw-r--r--   0     1001      127     4867 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/nodes/envelope.rs
--rw-r--r--   0     1001      127      806 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/nodes/gain.rs
--rw-r--r--   0     1001      127     1045 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/nodes/graph/error.rs
--rw-r--r--   0     1001      127    17261 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/nodes/graph.rs
--rw-r--r--   0     1001      127     6778 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/nodes/instrument.rs
--rw-r--r--   0     1001      127     1195 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/nodes/multi_frequency.rs
--rw-r--r--   0     1001      127      564 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/nodes/multiply.rs
--rw-r--r--   0     1001      127      462 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/nodes/passthrough.rs
--rw-r--r--   0     1001      127     1783 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/nodes/sawtooth_oscillator.rs
--rw-r--r--   0     1001      127     1688 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/nodes/sine_oscillator.rs
--rw-r--r--   0     1001      127     2172 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/nodes/square_oscillator.rs
--rw-r--r--   0     1001      127     1806 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/nodes/triangle_oscillator.rs
--rw-r--r--   0     1001      127      802 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/nodes.rs
--rw-r--r--   0     1001      127     1097 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/notation/chord/parse.rs
--rw-r--r--   0     1001      127     3417 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/notation/chord.rs
--rw-r--r--   0     1001      127      429 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/notation/inversion/parse.rs
--rw-r--r--   0     1001      127      785 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/notation/inversion.rs
--rw-r--r--   0     1001      127     1320 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/notation/item/parse.rs
--rw-r--r--   0     1001      127     6282 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/notation/item.rs
--rw-r--r--   0     1001      127      897 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/notation/note/parse.rs
--rw-r--r--   0     1001      127     4193 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/notation/note.rs
--rw-r--r--   0     1001      127      885 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/notation/overlapped/parse.rs
--rw-r--r--   0     1001      127     2759 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/notation/overlapped.rs
--rw-r--r--   0     1001      127      798 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/notation/pitch/parse.rs
--rw-r--r--   0     1001      127     1894 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/notation/pitch.rs
--rw-r--r--   0     1001      127      329 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/notation/rest/parse.rs
--rw-r--r--   0     1001      127     1133 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/notation/rest.rs
--rw-r--r--   0     1001      127      679 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/notation/scale/parse.rs
--rw-r--r--   0     1001      127     1126 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/notation/scale.rs
--rw-r--r--   0     1001      127      867 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/notation/sequence/parse.rs
--rw-r--r--   0     1001      127     3209 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/notation/sequence.rs
--rw-r--r--   0     1001      127     1565 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/notation/set/parse.rs
--rw-r--r--   0     1001      127     1330 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/notation/set.rs
--rw-r--r--   0     1001      127      408 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/notation/state_member/parse.rs
--rw-r--r--   0     1001      127      677 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/notation/state_member.rs
--rw-r--r--   0     1001      127      553 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/notation/step/parse.rs
--rw-r--r--   0     1001      127     2194 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/notation/step.rs
--rw-r--r--   0     1001      127     1589 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/notation/tone_generation_state.rs
--rw-r--r--   0     1001      127      475 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/notation.rs
--rw-r--r--   0     1001      127     1576 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/parse.rs
--rw-r--r--   0     1001      127     2192 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/pitch/parse.rs
--rw-r--r--   0     1001      127     6415 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/pitch.rs
--rw-r--r--   0     1001      127     1726 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/stream/iter.rs
--rw-r--r--   0     1001      127     5784 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/stream.rs
--rw-r--r--   0     1001      127     1622 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/sync.rs
--rw-r--r--   0     1001      127     2361 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/time/duration.rs
--rw-r--r--   0     1001      127     2115 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/time/time.rs
--rw-r--r--   0     1001      127     3185 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/time/timestamp.rs
--rw-r--r--   0     1001      127      172 2024-05-26 22:05:12.000000 libdaw-0.6.0/libdaw/src/time.rs
--rw-r--r--   0     1001      127      101 2024-05-26 22:05:12.000000 libdaw-0.6.0/README.md
--rw-r--r--   0        0        0      390 1970-01-01 00:00:00.000000 libdaw-0.6.0/python-libdaw/Cargo.toml
--rw-r--r--   0     1001      127     3526 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      686 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/.gitignore
--rw-r--r--   0     1001      127      131 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/README.md
--rw-r--r--   0     1001      127        6 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/docs/.gitignore
--rw-r--r--   0     1001      127      638 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/docs/Makefile
--rw-r--r--   0     1001      127      804 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/docs/make.bat
--rw-r--r--   0     1001      127        5 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/docs/requirements.txt
--rw-r--r--   0     1001      127      962 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/docs/source/conf.py
--rw-r--r--   0     1001      127      445 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/docs/source/index.rst
--rw-r--r--   0     1001      127      147 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/docs/source/libdaw/metronome.rst
--rw-r--r--   0     1001      127      161 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/docs/source/libdaw/nodes/envelope.rst
--rw-r--r--   0     1001      127      154 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/docs/source/libdaw/nodes/graph.rst
--rw-r--r--   0     1001      127      168 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/docs/source/libdaw/nodes/instrument.rst
--rw-r--r--   0     1001      127      181 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/docs/source/libdaw/nodes.rst
--rw-r--r--   0     1001      127       93 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/docs/source/libdaw/notation.rst
--rw-r--r--   0     1001      127      134 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/docs/source/libdaw/pitch.rst
--rw-r--r--   0     1001      127      133 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/docs/source/libdaw/time.rst
--rw-r--r--   0     1001      127      192 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/docs/source/libdaw.rst
--rw-r--r--   0     1001      127     1780 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/examples/1564.py
--rw-r--r--   0     1001      127     1662 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/examples/blues.py
--rwxr-xr-x   0     1001      127     1689 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/examples/instrument-test.py
--rw-r--r--   0     1001      127     1425 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/examples/pachelbel-canon-progression.py
--rw-r--r--   0     1001      127     1576 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/examples/round.py
--rw-r--r--   0     1001      127     1526 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/examples/scale-inversion-notation.py
--rw-r--r--   0     1001      127     1482 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/examples/simple-notation.py
--rw-r--r--   0     1001      127     1389 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/examples/simple-scale-notation.py
--rw-r--r--   0     1001      127      169 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/python/libdaw/__init__.py
--rw-r--r--   0     1001      127      933 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/python/libdaw/__init__.pyi
--rw-r--r--   0     1001      127     1588 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/python/libdaw/metronome.pyi
--rw-r--r--   0     1001      127     2528 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/python/libdaw/nodes/__init__.pyi
--rw-r--r--   0     1001      127      173 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/python/libdaw/nodes/envelope.pyi
--rw-r--r--   0     1001      127       23 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/python/libdaw/nodes/graph.pyi
--rw-r--r--   0     1001      127      151 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/python/libdaw/nodes/instrument.pyi
--rw-r--r--   0     1001      127     7463 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/python/libdaw/notation.pyi
--rw-r--r--   0     1001      127     1061 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/python/libdaw/pitch.pyi
--rw-r--r--   0     1001      127        0 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/python/libdaw/py.typed
--rw-r--r--   0     1001      127     1497 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/python/libdaw/time.pyi
--rw-r--r--   0     1001      127      491 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/frequency_node.rs
--rw-r--r--   0     1001      127     3052 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/lib.rs
--rw-r--r--   0     1001      127     4697 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/metronome.rs
--rw-r--r--   0     1001      127      976 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/node.rs
--rw-r--r--   0     1001      127      514 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/nodes/add.rs
--rw-r--r--   0     1001      127      580 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/nodes/constant_value.rs
--rw-r--r--   0     1001      127      586 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/nodes/delay.rs
--rw-r--r--   0     1001      127      845 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/nodes/detune.rs
--rw-r--r--   0     1001      127     1868 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/nodes/envelope.rs
--rw-r--r--   0     1001      127      644 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/nodes/gain.rs
--rw-r--r--   0     1001      127     4581 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/nodes/graph.rs
--rw-r--r--   0     1001      127     2715 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/nodes/instrument.rs
--rw-r--r--   0     1001      127      672 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/nodes/multi_frequency.rs
--rw-r--r--   0     1001      127      534 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/nodes/multiply.rs
--rw-r--r--   0     1001      127      489 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/nodes/passthrough.rs
--rw-r--r--   0     1001      127      756 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/nodes/sawtooth_oscillator.rs
--rw-r--r--   0     1001      127      705 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/nodes/sine_oscillator.rs
--rw-r--r--   0     1001      127      748 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/nodes/square_oscillator.rs
--rw-r--r--   0     1001      127      756 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/nodes/triangle_oscillator.rs
--rw-r--r--   0     1001      127     1787 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/nodes.rs
--rw-r--r--   0     1001      127     6875 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/notation/chord.rs
--rw-r--r--   0     1001      127     1472 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/notation/inversion.rs
--rw-r--r--   0     1001      127     4835 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/notation/item.rs
--rw-r--r--   0     1001      127     1982 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/notation/note/note_pitch.rs
--rw-r--r--   0     1001      127     3871 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/notation/note.rs
--rw-r--r--   0     1001      127     6120 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/notation/overlapped.rs
--rw-r--r--   0     1001      127     2936 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/notation/pitch.rs
--rw-r--r--   0     1001      127     1561 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/notation/rest.rs
--rw-r--r--   0     1001      127     4458 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/notation/scale.rs
--rw-r--r--   0     1001      127     5955 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/notation/sequence.rs
--rw-r--r--   0     1001      127     2667 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/notation/set.rs
--rw-r--r--   0     1001      127     1218 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/notation/state_member.rs
--rw-r--r--   0     1001      127     1983 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/notation/step.rs
--rw-r--r--   0     1001      127     1078 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/notation.rs
--rw-r--r--   0     1001      127     5729 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/pitch/pitch.rs
--rw-r--r--   0     1001      127     2648 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/pitch.rs
--rw-r--r--   0     1001      127     2178 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/play.rs
--rw-r--r--   0     1001      127     2658 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/stream.rs
--rw-r--r--   0     1001      127     5721 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/src/time.rs
--rw-r--r--   0     1001      127        0 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/test/__init__.py
--rw-r--r--   0     1001      127      471 2024-05-26 22:05:12.000000 libdaw-0.6.0/python-libdaw/test/test_pitch.py
--rw-r--r--   0     1001      127    30727 2024-05-26 22:05:16.000000 libdaw-0.6.0/Cargo.lock
--rw-r--r--   0        0        0      237 1970-01-01 00:00:00.000000 libdaw-0.6.0/Cargo.toml
--rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 libdaw-0.6.0/pyproject.toml
--rw-r--r--   0     1001      127     7463 2024-05-26 22:05:12.000000 libdaw-0.6.0/python/libdaw/notation.pyi
--rw-r--r--   0     1001      127      169 2024-05-26 22:05:12.000000 libdaw-0.6.0/python/libdaw/__init__.py
--rw-r--r--   0     1001      127        0 2024-05-26 22:05:12.000000 libdaw-0.6.0/python/libdaw/py.typed
--rw-r--r--   0     1001      127     1061 2024-05-26 22:05:12.000000 libdaw-0.6.0/python/libdaw/pitch.pyi
--rw-r--r--   0     1001      127     1497 2024-05-26 22:05:12.000000 libdaw-0.6.0/python/libdaw/time.pyi
--rw-r--r--   0     1001      127      933 2024-05-26 22:05:12.000000 libdaw-0.6.0/python/libdaw/__init__.pyi
--rw-r--r--   0     1001      127     1588 2024-05-26 22:05:12.000000 libdaw-0.6.0/python/libdaw/metronome.pyi
--rw-r--r--   0     1001      127      151 2024-05-26 22:05:12.000000 libdaw-0.6.0/python/libdaw/nodes/instrument.pyi
--rw-r--r--   0     1001      127       23 2024-05-26 22:05:12.000000 libdaw-0.6.0/python/libdaw/nodes/graph.pyi
--rw-r--r--   0     1001      127      173 2024-05-26 22:05:12.000000 libdaw-0.6.0/python/libdaw/nodes/envelope.pyi
--rw-r--r--   0     1001      127     2528 2024-05-26 22:05:12.000000 libdaw-0.6.0/python/libdaw/nodes/__init__.pyi
--rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 libdaw-0.6.0/PKG-INFO
+-rw-r--r--   0     1001      127      427 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/Cargo.toml
+-rw-r--r--   0     1001      127     1879 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/lib.rs
+-rw-r--r--   0     1001      127      281 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/metronome/parse.rs
+-rw-r--r--   0     1001      127    10846 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/metronome.rs
+-rw-r--r--   0     1001      127      531 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/nodes/add.rs
+-rw-r--r--   0     1001      127      870 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/nodes/constant_value.rs
+-rw-r--r--   0     1001      127     1987 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/nodes/delay.rs
+-rw-r--r--   0     1001      127     2253 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/nodes/detune.rs
+-rw-r--r--   0     1001      127     5813 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/nodes/envelope.rs
+-rw-r--r--   0     1001      127      806 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/nodes/gain.rs
+-rw-r--r--   0     1001      127     1045 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/nodes/graph/error.rs
+-rw-r--r--   0     1001      127    17261 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/nodes/graph.rs
+-rw-r--r--   0     1001      127     6778 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/nodes/instrument.rs
+-rw-r--r--   0     1001      127     1195 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/nodes/multi_frequency.rs
+-rw-r--r--   0     1001      127      564 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/nodes/multiply.rs
+-rw-r--r--   0     1001      127      462 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/nodes/passthrough.rs
+-rw-r--r--   0     1001      127     1783 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/nodes/sawtooth_oscillator.rs
+-rw-r--r--   0     1001      127     1688 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/nodes/sine_oscillator.rs
+-rw-r--r--   0     1001      127     2172 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/nodes/square_oscillator.rs
+-rw-r--r--   0     1001      127     1806 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/nodes/triangle_oscillator.rs
+-rw-r--r--   0     1001      127      802 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/nodes.rs
+-rw-r--r--   0     1001      127     1111 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/notation/chord/parse.rs
+-rw-r--r--   0     1001      127     3649 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/notation/chord.rs
+-rw-r--r--   0     1001      127      950 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/notation/duration/parse.rs
+-rw-r--r--   0     1001      127     1160 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/notation/duration.rs
+-rw-r--r--   0     1001      127      429 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/notation/inversion/parse.rs
+-rw-r--r--   0     1001      127      780 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/notation/inversion.rs
+-rw-r--r--   0     1001      127     1320 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/notation/item/parse.rs
+-rw-r--r--   0     1001      127     6282 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/notation/item.rs
+-rw-r--r--   0     1001      127      538 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/notation/note/parse.rs
+-rw-r--r--   0     1001      127     2930 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/notation/note.rs
+-rw-r--r--   0     1001      127      432 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/notation/note_pitch/parse.rs
+-rw-r--r--   0     1001      127     1677 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/notation/note_pitch.rs
+-rw-r--r--   0     1001      127      885 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/notation/overlapped/parse.rs
+-rw-r--r--   0     1001      127     2753 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/notation/overlapped.rs
+-rw-r--r--   0     1001      127      798 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/notation/pitch/parse.rs
+-rw-r--r--   0     1001      127     1894 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/notation/pitch.rs
+-rw-r--r--   0     1001      127      329 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/notation/rest/parse.rs
+-rw-r--r--   0     1001      127     1133 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/notation/rest.rs
+-rw-r--r--   0     1001      127      679 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/notation/scale/parse.rs
+-rw-r--r--   0     1001      127     1125 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/notation/scale.rs
+-rw-r--r--   0     1001      127      867 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/notation/sequence/parse.rs
+-rw-r--r--   0     1001      127     3205 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/notation/sequence.rs
+-rw-r--r--   0     1001      127     2007 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/notation/set/parse.rs
+-rw-r--r--   0     1001      127     1530 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/notation/set.rs
+-rw-r--r--   0     1001      127      408 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/notation/state_member/parse.rs
+-rw-r--r--   0     1001      127      677 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/notation/state_member.rs
+-rw-r--r--   0     1001      127      553 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/notation/step/parse.rs
+-rw-r--r--   0     1001      127     2194 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/notation/step.rs
+-rw-r--r--   0     1001      127     1712 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/notation/tone_generation_state.rs
+-rw-r--r--   0     1001      127      551 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/notation.rs
+-rw-r--r--   0     1001      127     1576 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/parse.rs
+-rw-r--r--   0     1001      127     2192 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/pitch/parse.rs
+-rw-r--r--   0     1001      127     6401 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/pitch.rs
+-rw-r--r--   0     1001      127     1726 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/stream/iter.rs
+-rw-r--r--   0     1001      127     5784 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/stream.rs
+-rw-r--r--   0     1001      127     1622 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/sync.rs
+-rw-r--r--   0     1001      127     2361 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/time/duration.rs
+-rw-r--r--   0     1001      127     2115 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/time/time.rs
+-rw-r--r--   0     1001      127     3185 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/time/timestamp.rs
+-rw-r--r--   0     1001      127      172 2024-05-27 03:41:16.000000 libdaw-0.7.0/libdaw/src/time.rs
+-rw-r--r--   0     1001      127      101 2024-05-27 03:41:16.000000 libdaw-0.7.0/README.md
+-rw-r--r--   0        0        0      390 1970-01-01 00:00:00.000000 libdaw-0.7.0/python-libdaw/Cargo.toml
+-rw-r--r--   0     1001      127     3526 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/.gitignore
+-rw-r--r--   0     1001      127      131 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/README.md
+-rw-r--r--   0     1001      127        6 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/docs/.gitignore
+-rw-r--r--   0     1001      127      638 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/docs/Makefile
+-rw-r--r--   0     1001      127      804 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/docs/make.bat
+-rw-r--r--   0     1001      127        5 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/docs/requirements.txt
+-rw-r--r--   0     1001      127      962 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/docs/source/conf.py
+-rw-r--r--   0     1001      127      445 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/docs/source/index.rst
+-rw-r--r--   0     1001      127      147 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/docs/source/libdaw/metronome.rst
+-rw-r--r--   0     1001      127      161 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/docs/source/libdaw/nodes/envelope.rst
+-rw-r--r--   0     1001      127      154 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/docs/source/libdaw/nodes/graph.rst
+-rw-r--r--   0     1001      127      168 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/docs/source/libdaw/nodes/instrument.rst
+-rw-r--r--   0     1001      127      181 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/docs/source/libdaw/nodes.rst
+-rw-r--r--   0     1001      127       93 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/docs/source/libdaw/notation.rst
+-rw-r--r--   0     1001      127      134 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/docs/source/libdaw/pitch.rst
+-rw-r--r--   0     1001      127      133 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/docs/source/libdaw/time.rst
+-rw-r--r--   0     1001      127      192 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/docs/source/libdaw.rst
+-rw-r--r--   0     1001      127     1780 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/examples/1564.py
+-rw-r--r--   0     1001      127     1662 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/examples/blues.py
+-rwxr-xr-x   0     1001      127     1689 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/examples/instrument-test.py
+-rw-r--r--   0     1001      127     1425 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/examples/pachelbel-canon-progression.py
+-rw-r--r--   0     1001      127     1576 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/examples/round.py
+-rw-r--r--   0     1001      127     1526 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/examples/scale-inversion-notation.py
+-rw-r--r--   0     1001      127     1482 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/examples/simple-notation.py
+-rw-r--r--   0     1001      127     1389 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/examples/simple-scale-notation.py
+-rw-r--r--   0     1001      127      169 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/python/libdaw/__init__.py
+-rw-r--r--   0     1001      127      933 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/python/libdaw/__init__.pyi
+-rw-r--r--   0     1001      127     1588 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/python/libdaw/metronome.pyi
+-rw-r--r--   0     1001      127     2528 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/python/libdaw/nodes/__init__.pyi
+-rw-r--r--   0     1001      127      173 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/python/libdaw/nodes/envelope.pyi
+-rw-r--r--   0     1001      127       23 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/python/libdaw/nodes/graph.pyi
+-rw-r--r--   0     1001      127      151 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/python/libdaw/nodes/instrument.pyi
+-rw-r--r--   0     1001      127     7463 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/python/libdaw/notation.pyi
+-rw-r--r--   0     1001      127     1061 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/python/libdaw/pitch.pyi
+-rw-r--r--   0     1001      127        0 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/python/libdaw/py.typed
+-rw-r--r--   0     1001      127     1497 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/python/libdaw/time.pyi
+-rw-r--r--   0     1001      127      491 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/frequency_node.rs
+-rw-r--r--   0     1001      127     3052 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/lib.rs
+-rw-r--r--   0     1001      127     4697 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/metronome.rs
+-rw-r--r--   0     1001      127      976 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/node.rs
+-rw-r--r--   0     1001      127      514 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/nodes/add.rs
+-rw-r--r--   0     1001      127      580 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/nodes/constant_value.rs
+-rw-r--r--   0     1001      127      586 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/nodes/delay.rs
+-rw-r--r--   0     1001      127      845 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/nodes/detune.rs
+-rw-r--r--   0     1001      127     1868 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/nodes/envelope.rs
+-rw-r--r--   0     1001      127      644 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/nodes/gain.rs
+-rw-r--r--   0     1001      127     4581 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/nodes/graph.rs
+-rw-r--r--   0     1001      127     2715 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/nodes/instrument.rs
+-rw-r--r--   0     1001      127      672 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/nodes/multi_frequency.rs
+-rw-r--r--   0     1001      127      534 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/nodes/multiply.rs
+-rw-r--r--   0     1001      127      489 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/nodes/passthrough.rs
+-rw-r--r--   0     1001      127      756 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/nodes/sawtooth_oscillator.rs
+-rw-r--r--   0     1001      127      705 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/nodes/sine_oscillator.rs
+-rw-r--r--   0     1001      127      748 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/nodes/square_oscillator.rs
+-rw-r--r--   0     1001      127      756 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/nodes/triangle_oscillator.rs
+-rw-r--r--   0     1001      127     1787 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/nodes.rs
+-rw-r--r--   0     1001      127     7021 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/notation/chord.rs
+-rw-r--r--   0     1001      127     4134 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/notation/duration.rs
+-rw-r--r--   0     1001      127     1472 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/notation/inversion.rs
+-rw-r--r--   0     1001      127     4835 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/notation/item.rs
+-rw-r--r--   0     1001      127     1982 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/notation/note/note_pitch.rs
+-rw-r--r--   0     1001      127     4043 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/notation/note.rs
+-rw-r--r--   0     1001      127     6110 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/notation/overlapped.rs
+-rw-r--r--   0     1001      127     2936 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/notation/pitch.rs
+-rw-r--r--   0     1001      127     1561 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/notation/rest.rs
+-rw-r--r--   0     1001      127     4448 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/notation/scale.rs
+-rw-r--r--   0     1001      127     5945 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/notation/sequence.rs
+-rw-r--r--   0     1001      127     3323 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/notation/set.rs
+-rw-r--r--   0     1001      127     1218 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/notation/state_member.rs
+-rw-r--r--   0     1001      127     1983 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/notation/step.rs
+-rw-r--r--   0     1001      127     1195 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/notation.rs
+-rw-r--r--   0     1001      127     5729 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/pitch/pitch.rs
+-rw-r--r--   0     1001      127     2648 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/pitch.rs
+-rw-r--r--   0     1001      127     2178 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/play.rs
+-rw-r--r--   0     1001      127     2638 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/stream.rs
+-rw-r--r--   0     1001      127     5721 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/src/time.rs
+-rw-r--r--   0     1001      127        0 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/test/__init__.py
+-rw-r--r--   0     1001      127      471 2024-05-27 03:41:16.000000 libdaw-0.7.0/python-libdaw/test/test_pitch.py
+-rw-r--r--   0     1001      127    30727 2024-05-27 03:41:21.000000 libdaw-0.7.0/Cargo.lock
+-rw-r--r--   0        0        0      241 1970-01-01 00:00:00.000000 libdaw-0.7.0/Cargo.toml
+-rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 libdaw-0.7.0/pyproject.toml
+-rw-r--r--   0     1001      127     7463 2024-05-27 03:41:16.000000 libdaw-0.7.0/python/libdaw/notation.pyi
+-rw-r--r--   0     1001      127      169 2024-05-27 03:41:16.000000 libdaw-0.7.0/python/libdaw/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-27 03:41:16.000000 libdaw-0.7.0/python/libdaw/py.typed
+-rw-r--r--   0     1001      127     1061 2024-05-27 03:41:16.000000 libdaw-0.7.0/python/libdaw/pitch.pyi
+-rw-r--r--   0     1001      127     1497 2024-05-27 03:41:16.000000 libdaw-0.7.0/python/libdaw/time.pyi
+-rw-r--r--   0     1001      127      933 2024-05-27 03:41:16.000000 libdaw-0.7.0/python/libdaw/__init__.pyi
+-rw-r--r--   0     1001      127     1588 2024-05-27 03:41:16.000000 libdaw-0.7.0/python/libdaw/metronome.pyi
+-rw-r--r--   0     1001      127      151 2024-05-27 03:41:16.000000 libdaw-0.7.0/python/libdaw/nodes/instrument.pyi
+-rw-r--r--   0     1001      127       23 2024-05-27 03:41:16.000000 libdaw-0.7.0/python/libdaw/nodes/graph.pyi
+-rw-r--r--   0     1001      127      173 2024-05-27 03:41:16.000000 libdaw-0.7.0/python/libdaw/nodes/envelope.pyi
+-rw-r--r--   0     1001      127     2528 2024-05-27 03:41:16.000000 libdaw-0.7.0/python/libdaw/nodes/__init__.pyi
+-rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 libdaw-0.7.0/PKG-INFO
```

### Comparing `libdaw-0.6.0/libdaw/src/lib.rs` & `libdaw-0.7.0/libdaw/src/lib.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/libdaw/src/metronome.rs` & `libdaw-0.7.0/libdaw/src/metronome.rs`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 use crate::{parse::IResult, time::Timestamp};
 use ordered_float::OrderedFloat;
 use std::{
     fmt,
     hash::{Hash, Hasher},
     iter::Sum,
-    ops::{Add, AddAssign},
+    ops::{Add, AddAssign, Mul, MulAssign, Sub, SubAssign},
 };
 
 #[derive(Debug, Clone, Copy, PartialEq, Eq)]
 pub enum IllegalBeat {
     NaN,
     Negative,
 }
@@ -70,14 +70,22 @@
         Self(self.0.max(other.0))
     }
 
     pub fn checked_add(self, other: Self) -> Result<Self, IllegalBeat> {
         Self::new(self.0 + other.0)
     }
 
+    pub fn checked_sub(self, other: Self) -> Result<Self, IllegalBeat> {
+        Self::new(self.0 - other.0)
+    }
+
+    pub fn checked_mul(self, other: f64) -> Result<Self, IllegalBeat> {
+        Self::new(self.0 * other)
+    }
+
     pub fn parse(input: &str) -> IResult<&str, Self> {
         parse::beat(input)
     }
 }
 
 impl Add for Beat {
     type Output = Self;
@@ -89,20 +97,52 @@
 
 impl AddAssign for Beat {
     fn add_assign(&mut self, rhs: Self) {
         self.0 = self.checked_add(rhs).expect("added to illegal beat").0;
     }
 }
 
+impl Sub for Beat {
+    type Output = Self;
+
+    fn sub(self, rhs: Self) -> Self::Output {
+        self.checked_sub(rhs).expect("subtracted to illegal beat")
+    }
+}
+
+impl SubAssign for Beat {
+    fn sub_assign(&mut self, rhs: Self) {
+        self.0 = self.checked_sub(rhs).expect("subtracted to illegal beat").0;
+    }
+}
+
 impl Sum for Beat {
     fn sum<I: Iterator<Item = Self>>(iter: I) -> Self {
         Self::new(iter.map(|each| each.0).sum()).expect("summed to illegal beat")
     }
 }
 
+impl Mul<f64> for Beat {
+    type Output = Self;
+
+    fn mul(self, rhs: f64) -> Self::Output {
+        self.checked_mul(rhs)
+            .expect("multiplied with illegal value")
+    }
+}
+
+impl MulAssign<f64> for Beat {
+    fn mul_assign(&mut self, rhs: f64) {
+        self.0 = self
+            .checked_mul(rhs)
+            .expect("multiplied with illegal value")
+            .0;
+    }
+}
+
 #[derive(Debug, Clone, Copy, PartialEq, Eq)]
 pub enum IllegalBeatsPerMinute {
     NaN,
     NonPositive,
 }
 
 impl fmt::Display for IllegalBeatsPerMinute {
```

### Comparing `libdaw-0.6.0/libdaw/src/nodes/add.rs` & `libdaw-0.7.0/libdaw/src/nodes/add.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/libdaw/src/nodes/constant_value.rs` & `libdaw-0.7.0/libdaw/src/nodes/constant_value.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/libdaw/src/nodes/delay.rs` & `libdaw-0.7.0/libdaw/src/nodes/delay.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/libdaw/src/nodes/detune.rs` & `libdaw-0.7.0/libdaw/src/nodes/detune.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/libdaw/src/nodes/envelope.rs` & `libdaw-0.7.0/libdaw/src/nodes/envelope.rs`

 * *Files 15% similar despite different names*

```diff
@@ -71,36 +71,62 @@
     /// Construct the envelope.  If you give zero envelope points, this will
     /// effectively be a PassthroughNode.
     pub fn new(
         sample_rate: u32,
         length: Duration,
         envelope: impl IntoIterator<Item = Point>,
     ) -> Self {
+        let sample_time = 1.0 / sample_rate as f64;
+        let sample_length = (sample_rate as f64 * length.seconds()) as u64;
         let mut envelope: Vec<CalculatedPoint> = envelope
             .into_iter()
             .flat_map(move |point| {
                 let length = length.seconds();
-                let whence = length * point.whence;
+                // The end point for whence, so a whence of 1 ends up at the
+                // last sample, rather than one past the end.
+                let end = length - sample_time;
+                let whence = end * point.whence;
                 let time = match point.offset {
                     Offset::Time(offset) => whence + offset.seconds(),
                     Offset::Ratio(offset) => {
                         let offset = length * offset;
                         whence + offset
                     }
                 };
-                if time.is_nan() {
+                if !(0.0..=length).contains(&time) {
                     return None;
                 }
-                Some(CalculatedPoint {
-                    sample: (time * sample_rate as f64) as u64,
-                    volume: point.volume,
-                })
+                let sample = (time * (sample_rate) as f64) as u64;
+                if sample < sample_length {
+                    Some(CalculatedPoint {
+                        sample,
+                        volume: point.volume,
+                    })
+                } else {
+                    None
+                }
             })
             .collect();
-        envelope.sort();
+
+        // Filter points such that all points placed at the same time or later
+        // than a later-in-order point will be removed.
+        let mut min_sample = u64::MAX;
+        envelope.reverse();
+        envelope.retain(move |point| {
+            if point.sample < min_sample {
+                min_sample = point.sample;
+                true
+            } else {
+                false
+            }
+        });
+
+        envelope.reverse();
+        envelope.shrink_to_fit();
+
         Self {
             envelope: envelope.into(),
             sample: 0.into(),
         }
     }
 }
```

### Comparing `libdaw-0.6.0/libdaw/src/nodes/gain.rs` & `libdaw-0.7.0/libdaw/src/nodes/gain.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/libdaw/src/nodes/graph/error.rs` & `libdaw-0.7.0/libdaw/src/nodes/graph/error.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/libdaw/src/nodes/graph.rs` & `libdaw-0.7.0/libdaw/src/nodes/graph.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/libdaw/src/nodes/instrument.rs` & `libdaw-0.7.0/libdaw/src/nodes/instrument.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/libdaw/src/nodes/multi_frequency.rs` & `libdaw-0.7.0/libdaw/src/nodes/multi_frequency.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/libdaw/src/nodes/multiply.rs` & `libdaw-0.7.0/libdaw/src/nodes/multiply.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/libdaw/src/nodes/sawtooth_oscillator.rs` & `libdaw-0.7.0/libdaw/src/nodes/sawtooth_oscillator.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/libdaw/src/nodes/sine_oscillator.rs` & `libdaw-0.7.0/libdaw/src/nodes/sine_oscillator.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/libdaw/src/nodes/square_oscillator.rs` & `libdaw-0.7.0/libdaw/src/nodes/square_oscillator.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/libdaw/src/nodes/triangle_oscillator.rs` & `libdaw-0.7.0/libdaw/src/nodes/triangle_oscillator.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/libdaw/src/nodes.rs` & `libdaw-0.7.0/libdaw/src/nodes.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/libdaw/src/notation/chord/parse.rs` & `libdaw-0.7.0/libdaw/src/notation/chord/parse.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use super::{Chord, NotePitch, StateMember};
+use super::{Chord, Duration, NotePitch, StateMember};
 use crate::{metronome::Beat, parse::IResult};
 use nom::{
     branch::alt,
     bytes::complete::tag,
     character::complete::{multispace0, multispace1},
     combinator::{cut, opt},
     multi::separated_list1,
@@ -16,15 +16,15 @@
     let (input, _) = multispace0(input)?;
     let (input, _) = cut(tag("("))(input)?;
     let (input, _) = multispace0(input)?;
     let (input, pitches) = cut(separated_list1(multispace1, NotePitch::parse))(input)?;
     let (input, _) = multispace0(input)?;
     let (input, _) = cut(tag(")"))(input)?;
     let (input, length) = opt(preceded(tag(","), Beat::parse))(input)?;
-    let (input, duration) = opt(preceded(tag(","), Beat::parse))(input)?;
+    let (input, duration) = opt(preceded(tag(","), Duration::parse))(input)?;
     Ok((
         input,
         Chord {
             pitches,
             length,
             duration,
             state_member,
```

### Comparing `libdaw-0.6.0/libdaw/src/notation/chord.rs` & `libdaw-0.7.0/libdaw/src/notation/chord.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 mod parse;
 
-use super::{tone_generation_state::ToneGenerationState, NotePitch, StateMember};
+use super::{tone_generation_state::ToneGenerationState, Duration, NotePitch, StateMember};
 use crate::{
     metronome::{Beat, Metronome},
     nodes::instrument::Tone,
     parse::IResult,
     pitch::PitchStandard,
 };
 use nom::{combinator::all_consuming, error::convert_error, Finish as _};
@@ -16,15 +16,15 @@
     pub pitches: Vec<NotePitch>,
 
     // Conceptual length of the chord in beats
     pub length: Option<Beat>,
 
     // Actual playtime of the chord in beats, which will default to the length
     // usually.
-    pub duration: Option<Beat>,
+    pub duration: Option<Duration>,
 
     pub state_member: Option<StateMember>,
 }
 
 impl Chord {
     /// Resolve all the section's chords to playable instrument tones.
     /// The offset is the beat offset.
@@ -74,44 +74,51 @@
     }
 
     pub(super) fn inner_length(&self, state: &ToneGenerationState) -> Beat {
         self.length.unwrap_or(state.length)
     }
 
     pub(super) fn inner_duration(&self, state: &ToneGenerationState) -> Beat {
-        self.duration.or(self.length).unwrap_or(state.length)
+        let length = self.inner_length(state);
+        let duration = self.duration.unwrap_or(state.duration);
+        duration.resolve(length)
     }
     pub fn length(&self) -> Beat {
         self.inner_length(&Default::default())
     }
     pub fn duration(&self) -> Beat {
         self.inner_duration(&Default::default())
     }
 
     pub fn parse(input: &str) -> IResult<&str, Self> {
         parse::chord(input)
     }
     pub(super) fn update_state(&self, state: &mut ToneGenerationState) {
-        state.length = self.inner_length(state);
         match self.state_member {
             Some(StateMember::First) => self.pitches[0].update_state(state),
             Some(StateMember::Last) => {
                 for pitch in &self.pitches {
                     pitch.update_state(state);
                 }
             }
             None => (),
         }
+        if let Some(length) = self.length {
+            state.length = length;
+        }
+        if let Some(duration) = self.duration {
+            state.duration = duration;
+        }
     }
 }
 
 impl FromStr for Chord {
     type Err = String;
 
     fn from_str(s: &str) -> Result<Self, Self::Err> {
-        let chord = all_consuming(parse::chord)(s)
+        let chord = all_consuming(Self::parse)(s)
             .finish()
             .map_err(move |e| convert_error(s, e))?
             .1;
         Ok(chord)
     }
 }
```

### Comparing `libdaw-0.6.0/libdaw/src/notation/inversion.rs` & `libdaw-0.7.0/libdaw/src/notation/inversion.rs`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,14 @@
     }
 }
 
 impl FromStr for Inversion {
     type Err = String;
 
     fn from_str(s: &str) -> Result<Self, Self::Err> {
-        let inversion = all_consuming(parse::inversion)(s)
+        let inversion = all_consuming(Self::parse)(s)
             .finish()
             .map_err(move |e| convert_error(s, e))?
             .1;
         Ok(inversion)
     }
 }
```

### Comparing `libdaw-0.6.0/libdaw/src/notation/item/parse.rs` & `libdaw-0.7.0/libdaw/src/notation/item/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/libdaw/src/notation/item.rs` & `libdaw-0.7.0/libdaw/src/notation/item.rs`

 * *Files 4% similar despite different names*

```diff
@@ -160,14 +160,14 @@
     }
 }
 
 impl FromStr for Item {
     type Err = String;
 
     fn from_str(s: &str) -> Result<Self, Self::Err> {
-        let note = all_consuming(parse::item)(s)
+        let note = all_consuming(Self::parse)(s)
             .finish()
             .map_err(move |e| convert_error(s, e))?
             .1;
         Ok(note)
     }
 }
```

### Comparing `libdaw-0.6.0/libdaw/src/notation/note.rs` & `libdaw-0.7.0/libdaw/src/notation/note.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,81 +1,30 @@
 mod parse;
 
-use super::{tone_generation_state::ToneGenerationState, Pitch, Step};
+use super::{tone_generation_state::ToneGenerationState, Duration, NotePitch};
 use crate::{
     metronome::{Beat, Metronome},
     nodes::instrument::Tone,
     parse::IResult,
-    pitch::{Pitch as AbsolutePitch, PitchStandard},
+    pitch::PitchStandard,
 };
 use nom::{combinator::all_consuming, error::convert_error, Finish as _};
-use std::{
-    fmt,
-    str::FromStr,
-    sync::{Arc, Mutex},
-};
-
-#[derive(Clone)]
-pub enum NotePitch {
-    Pitch(Arc<Mutex<Pitch>>),
-    Step(Arc<Mutex<Step>>),
-}
-
-impl fmt::Debug for NotePitch {
-    fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
-        match self {
-            NotePitch::Pitch(pitch) => fmt::Debug::fmt(&pitch.lock().expect("poisoned"), f),
-            NotePitch::Step(step) => fmt::Debug::fmt(&step.lock().expect("poisoned"), f),
-        }
-    }
-}
-
-impl NotePitch {
-    pub fn parse(input: &str) -> IResult<&str, Self> {
-        parse::note_pitch(input)
-    }
-    /// Resolve to an absolute pitch
-    pub(super) fn absolute(&self, state: &ToneGenerationState) -> AbsolutePitch {
-        match self {
-            NotePitch::Pitch(pitch) => pitch.lock().expect("poisoned").absolute(state),
-            NotePitch::Step(step) => step.lock().expect("poisoned").absolute(state),
-        }
-    }
-    pub(super) fn update_state(&self, state: &mut ToneGenerationState) {
-        let pitch = self.absolute(state);
-        state.pitch = pitch;
-        if let Self::Step(step) = self {
-            step.lock().expect("poisoned").update_state(state);
-        }
-    }
-}
-
-impl FromStr for NotePitch {
-    type Err = String;
-
-    fn from_str(s: &str) -> Result<Self, Self::Err> {
-        let note = all_consuming(Self::parse)(s)
-            .finish()
-            .map_err(move |e| convert_error(s, e))?
-            .1;
-        Ok(note)
-    }
-}
+use std::str::FromStr;
 
 /// An absolute note, contextually relevant.
 #[derive(Debug, Clone)]
 pub struct Note {
     pub pitch: NotePitch,
 
     // Conceptual length of the note in beats
     pub length: Option<Beat>,
 
     // Actual playtime of the note in beats, which will default to the length
     // usually.
-    pub duration: Option<Beat>,
+    pub duration: Option<Duration>,
 }
 
 impl Note {
     /// Resolve all the section's notes to playable instrument tones.
     /// The offset is the beat offset.
     pub(super) fn inner_tone<S>(
         &self,
@@ -110,32 +59,38 @@
     }
 
     pub(super) fn inner_length(&self, state: &ToneGenerationState) -> Beat {
         self.length.unwrap_or(state.length)
     }
 
     pub(super) fn inner_duration(&self, state: &ToneGenerationState) -> Beat {
-        self.duration.or(self.length).unwrap_or(state.length)
+        let length = self.inner_length(state);
+        let duration = self.duration.unwrap_or(state.duration);
+        duration.resolve(length)
     }
 
     pub fn length(&self) -> Beat {
         self.inner_length(&Default::default())
     }
     pub fn duration(&self) -> Beat {
         self.inner_duration(&Default::default())
     }
 
     pub fn parse(input: &str) -> IResult<&str, Self> {
         parse::note(input)
     }
 
     pub(super) fn update_state(&self, state: &mut ToneGenerationState) {
-        let length = self.inner_length(state);
         self.pitch.update_state(state);
-        state.length = length;
+        if let Some(length) = self.length {
+            state.length = length;
+        }
+        if let Some(duration) = self.duration {
+            state.duration = duration;
+        }
     }
 }
 
 impl FromStr for Note {
     type Err = String;
 
     fn from_str(s: &str) -> Result<Self, Self::Err> {
```

### Comparing `libdaw-0.6.0/libdaw/src/notation/overlapped/parse.rs` & `libdaw-0.7.0/libdaw/src/notation/overlapped/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/libdaw/src/notation/overlapped.rs` & `libdaw-0.7.0/libdaw/src/notation/overlapped.rs`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,14 @@
     }
 }
 
 impl FromStr for Overlapped {
     type Err = String;
 
     fn from_str(s: &str) -> Result<Self, Self::Err> {
-        let note = all_consuming(parse::overlapped)(s)
+        let note = all_consuming(Self::parse)(s)
             .finish()
             .map_err(move |e| convert_error(s, e))?
             .1;
         Ok(note)
     }
 }
```

### Comparing `libdaw-0.6.0/libdaw/src/notation/pitch/parse.rs` & `libdaw-0.7.0/libdaw/src/notation/pitch/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/libdaw/src/notation/pitch.rs` & `libdaw-0.7.0/libdaw/src/notation/pitch.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/libdaw/src/notation/rest.rs` & `libdaw-0.7.0/libdaw/src/notation/rest.rs`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,14 @@
     }
 }
 
 impl FromStr for Rest {
     type Err = String;
 
     fn from_str(s: &str) -> Result<Self, Self::Err> {
-        let note = all_consuming(parse::rest)(s)
+        let note = all_consuming(Self::parse)(s)
             .finish()
             .map_err(move |e| convert_error(s, e))?
             .1;
         Ok(note)
     }
 }
```

### Comparing `libdaw-0.6.0/libdaw/src/notation/scale/parse.rs` & `libdaw-0.7.0/libdaw/src/notation/scale/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/libdaw/src/notation/scale.rs` & `libdaw-0.7.0/libdaw/src/notation/scale.rs`

 * *Files 12% similar despite different names*

```diff
@@ -29,14 +29,14 @@
     }
 }
 
 impl FromStr for Scale {
     type Err = String;
 
     fn from_str(s: &str) -> Result<Self, Self::Err> {
-        let scale = all_consuming(parse::scale)(s)
+        let scale = all_consuming(Self::parse)(s)
             .finish()
             .map_err(move |e| convert_error(s, e))?
             .1;
         Ok(scale)
     }
 }
```

### Comparing `libdaw-0.6.0/libdaw/src/notation/sequence/parse.rs` & `libdaw-0.7.0/libdaw/src/notation/sequence/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/libdaw/src/notation/sequence.rs` & `libdaw-0.7.0/libdaw/src/notation/sequence.rs`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     pub state_member: Option<StateMember>,
 }
 
 impl FromStr for Sequence {
     type Err = String;
 
     fn from_str(s: &str) -> Result<Self, Self::Err> {
-        let note = all_consuming(parse::sequence)(s)
+        let note = all_consuming(Self::parse)(s)
             .finish()
             .map_err(move |e| convert_error(s, e))?
             .1;
         Ok(note)
     }
 }
```

### Comparing `libdaw-0.6.0/libdaw/src/notation/set/parse.rs` & `libdaw-0.7.0/libdaw/src/notation/set/parse.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,67 @@
-use super::{NotePitch, Set};
+use super::{Duration, NotePitch, Set};
 use crate::{metronome::Beat, parse::IResult};
 use nom::{
     branch::alt,
     bytes::complete::tag,
-    character::complete::{multispace0, multispace1},
+    character::complete::{char, multispace0, multispace1},
     combinator::cut,
     multi::separated_list1,
 };
 
 fn pitch(input: &str) -> IResult<&str, Set> {
     let (input, _) = tag("pitch")(input)?;
     let (input, _) = multispace0(input)?;
-    let (input, _) = cut(tag(":"))(input)?;
+    let (input, _) = cut(char(':'))(input)?;
     let (input, _) = multispace0(input)?;
     let (input, pitch) = cut(NotePitch::parse)(input)?;
     Ok((
         input,
         Set {
             pitch: Some(pitch),
             ..Default::default()
         },
     ))
 }
 fn length(input: &str) -> IResult<&str, Set> {
     let (input, _) = tag("length")(input)?;
     let (input, _) = multispace0(input)?;
-    let (input, _) = cut(tag(":"))(input)?;
+    let (input, _) = cut(char(':'))(input)?;
     let (input, _) = multispace0(input)?;
     let (input, length) = cut(Beat::parse)(input)?;
     Ok((
         input,
         Set {
             length: Some(length),
             ..Default::default()
         },
     ))
 }
 
+fn duration(input: &str) -> IResult<&str, Set> {
+    let (input, _) = tag("duration")(input)?;
+    let (input, _) = multispace0(input)?;
+    let (input, _) = cut(char(':'))(input)?;
+    let (input, _) = multispace0(input)?;
+    let (input, duration) = cut(Duration::parse)(input)?;
+    Ok((
+        input,
+        Set {
+            duration: Some(duration),
+            ..Default::default()
+        },
+    ))
+}
+
 pub fn set(input: &str) -> IResult<&str, Set> {
     let (input, _) = alt((tag(":"), tag("set")))(input)?;
     let (input, _) = multispace0(input)?;
-    let (input, _) = cut(tag("("))(input)?;
+    let (input, _) = cut(char('('))(input)?;
     let (input, _) = multispace0(input)?;
-    let (input, sets) = cut(separated_list1(multispace1, alt((pitch, length))))(input)?;
+    let (input, sets) = cut(separated_list1(multispace1, alt((pitch, length, duration))))(input)?;
 
     // Prefer later settings to earlier
-    let set = sets.into_iter().reduce(|b, a| (b | a)).unwrap();
+    let set = sets.into_iter().reduce(|a, b| (b | a)).unwrap();
     let (input, _) = multispace0(input)?;
-    let (input, _) = cut(tag(")"))(input)?;
+    let (input, _) = cut(char(')'))(input)?;
     Ok((input, set))
 }
```

### Comparing `libdaw-0.6.0/libdaw/src/notation/set.rs` & `libdaw-0.7.0/libdaw/src/notation/set.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 mod parse;
 
-use super::{tone_generation_state::ToneGenerationState, NotePitch};
+use super::{tone_generation_state::ToneGenerationState, Duration, NotePitch};
 use crate::{metronome::Beat, parse::IResult};
 use nom::{combinator::all_consuming, error::convert_error, Finish as _};
 use std::{
     ops::{BitOr, BitOrAssign},
     str::FromStr,
 };
 
 #[derive(Debug, Clone, Default)]
 pub struct Set {
     pub pitch: Option<NotePitch>,
     pub length: Option<Beat>,
+    pub duration: Option<Duration>,
 }
 
 impl BitOrAssign for Set {
     fn bitor_assign(&mut self, rhs: Self) {
         self.pitch = self.pitch.take().or(rhs.pitch);
         self.length = self.length.or(rhs.length);
+        self.duration = self.duration.or(rhs.duration);
     }
 }
 impl BitOr for Set {
     type Output = Set;
 
     fn bitor(mut self, rhs: Self) -> Self::Output {
         self |= rhs;
@@ -36,21 +38,24 @@
     pub(super) fn update_state(&self, state: &mut ToneGenerationState) {
         if let Some(pitch) = &self.pitch {
             pitch.update_state(state);
         }
         if let Some(length) = self.length {
             state.length = length;
         }
+        if let Some(duration) = self.duration {
+            state.duration = duration;
+        }
     }
 }
 
 impl FromStr for Set {
     type Err = String;
 
     fn from_str(s: &str) -> Result<Self, Self::Err> {
-        let scale = all_consuming(parse::set)(s)
+        let scale = all_consuming(Self::parse)(s)
             .finish()
             .map_err(move |e| convert_error(s, e))?
             .1;
         Ok(scale)
     }
 }
```

### Comparing `libdaw-0.6.0/libdaw/src/notation/state_member.rs` & `libdaw-0.7.0/libdaw/src/notation/state_member.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/libdaw/src/notation/step/parse.rs` & `libdaw-0.7.0/libdaw/src/notation/step/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/libdaw/src/notation/step.rs` & `libdaw-0.7.0/libdaw/src/notation/step.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/libdaw/src/notation/tone_generation_state.rs` & `libdaw-0.7.0/libdaw/src/notation/tone_generation_state.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-use std::sync::{Arc, Mutex};
-
+use super::Duration;
 use crate::{
     metronome::Beat,
     pitch::{Pitch, PitchClass, PitchName},
 };
+use std::sync::{Arc, Mutex};
 
 /// A running state that is used to manage context-aware bits of tone
 /// generatian.
 #[derive(Debug, Clone)]
 pub struct ToneGenerationState {
     /// Previous resolved pitch.
     pub pitch: Pitch,
 
     /// Previous resolved length.
     pub length: Beat,
 
+    /// Previous set duration.
+    pub duration: Duration,
+
     /// The scale for scale-inversion notation.
     pub scale: Vec<Pitch>,
 
     /// The current scale inversion.
     pub inversion: i64,
 
     /// Previous used scale step, post-inversion.
@@ -35,14 +38,15 @@
                 pitch_class: Arc::new(Mutex::new(PitchClass {
                     name: PitchName::C,
                     adjustment: 0.0,
                 })),
                 octave: 4,
             },
             length: Beat::ONE,
+            duration: Duration::default(),
             scale: [
                 PitchName::C,
                 PitchName::D,
                 PitchName::E,
                 PitchName::F,
                 PitchName::G,
                 PitchName::A,
```

### Comparing `libdaw-0.6.0/libdaw/src/parse.rs` & `libdaw-0.7.0/libdaw/src/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/libdaw/src/pitch/parse.rs` & `libdaw-0.7.0/libdaw/src/pitch/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/libdaw/src/pitch.rs` & `libdaw-0.7.0/libdaw/src/pitch.rs`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     }
 }
 
 impl FromStr for PitchName {
     type Err = String;
 
     fn from_str(s: &str) -> Result<Self, Self::Err> {
-        let note = all_consuming(parse::pitch_name)(s)
+        let note = all_consuming(Self::parse)(s)
             .finish()
             .map_err(move |e| convert_error(s, e))?
             .1;
         Ok(note)
     }
 }
 
@@ -110,15 +110,15 @@
 /// Can also handle numeric adjustments, expressed in semitones, in square brackets,
 /// and ratios of these, along with symbolic ones.
 /// B𝄫𝄪###[14/12e8]-12 is a valid (but completely inaudible) absolute note.
 impl FromStr for PitchClass {
     type Err = String;
 
     fn from_str(s: &str) -> Result<Self, Self::Err> {
-        let note = all_consuming(parse::pitch_class)(s)
+        let note = all_consuming(Self::parse)(s)
             .finish()
             .map_err(move |e| convert_error(s, e))?
             .1;
         Ok(note)
     }
 }
 
@@ -152,15 +152,15 @@
 /// Can also handle numeric adjustments, expressed in semitones, in square brackets,
 /// and ratios of these, along with symbolic ones.
 /// B𝄫𝄪###[14/12e8]-12 is a valid (but completely inaudible) absolute note.
 impl FromStr for Pitch {
     type Err = String;
 
     fn from_str(s: &str) -> Result<Self, Self::Err> {
-        let note = all_consuming(parse::pitch)(s)
+        let note = all_consuming(Self::parse)(s)
             .finish()
             .map_err(move |e| convert_error(s, e))?
             .1;
         Ok(note)
     }
 }
```

### Comparing `libdaw-0.6.0/libdaw/src/stream/iter.rs` & `libdaw-0.7.0/libdaw/src/stream/iter.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/libdaw/src/stream.rs` & `libdaw-0.7.0/libdaw/src/stream.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/libdaw/src/sync.rs` & `libdaw-0.7.0/libdaw/src/sync.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/libdaw/src/time/duration.rs` & `libdaw-0.7.0/libdaw/src/time/duration.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/libdaw/src/time/time.rs` & `libdaw-0.7.0/libdaw/src/time/time.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/libdaw/src/time/timestamp.rs` & `libdaw-0.7.0/libdaw/src/time/timestamp.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/.github/workflows/CI.yml` & `libdaw-0.7.0/python-libdaw/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/.gitignore` & `libdaw-0.7.0/python-libdaw/.gitignore`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/docs/Makefile` & `libdaw-0.7.0/python-libdaw/docs/Makefile`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/docs/make.bat` & `libdaw-0.7.0/python-libdaw/docs/make.bat`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/docs/source/conf.py` & `libdaw-0.7.0/python-libdaw/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/examples/1564.py` & `libdaw-0.7.0/python-libdaw/examples/1564.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/examples/blues.py` & `libdaw-0.7.0/python-libdaw/examples/blues.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/examples/instrument-test.py` & `libdaw-0.7.0/python-libdaw/examples/instrument-test.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/examples/pachelbel-canon-progression.py` & `libdaw-0.7.0/python-libdaw/examples/pachelbel-canon-progression.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/examples/round.py` & `libdaw-0.7.0/python-libdaw/examples/round.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/examples/scale-inversion-notation.py` & `libdaw-0.7.0/python-libdaw/examples/scale-inversion-notation.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/examples/simple-notation.py` & `libdaw-0.7.0/python-libdaw/examples/simple-notation.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/examples/simple-scale-notation.py` & `libdaw-0.7.0/python-libdaw/examples/simple-scale-notation.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/python/libdaw/__init__.pyi` & `libdaw-0.7.0/python-libdaw/python/libdaw/__init__.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/python/libdaw/metronome.pyi` & `libdaw-0.7.0/python-libdaw/python/libdaw/metronome.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/python/libdaw/nodes/__init__.pyi` & `libdaw-0.7.0/python-libdaw/python/libdaw/nodes/__init__.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/python/libdaw/notation.pyi` & `libdaw-0.7.0/python-libdaw/python/libdaw/notation.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/python/libdaw/pitch.pyi` & `libdaw-0.7.0/python-libdaw/python/libdaw/pitch.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/python/libdaw/time.pyi` & `libdaw-0.7.0/python-libdaw/python/libdaw/time.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/src/lib.rs` & `libdaw-0.7.0/python-libdaw/src/lib.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/src/metronome.rs` & `libdaw-0.7.0/python-libdaw/src/metronome.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/src/node.rs` & `libdaw-0.7.0/python-libdaw/src/node.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/src/nodes/add.rs` & `libdaw-0.7.0/python-libdaw/src/nodes/add.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/src/nodes/constant_value.rs` & `libdaw-0.7.0/python-libdaw/src/nodes/constant_value.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/src/nodes/delay.rs` & `libdaw-0.7.0/python-libdaw/src/nodes/delay.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/src/nodes/detune.rs` & `libdaw-0.7.0/python-libdaw/src/nodes/detune.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/src/nodes/envelope.rs` & `libdaw-0.7.0/python-libdaw/src/nodes/envelope.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/src/nodes/gain.rs` & `libdaw-0.7.0/python-libdaw/src/nodes/gain.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/src/nodes/graph.rs` & `libdaw-0.7.0/python-libdaw/src/nodes/graph.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/src/nodes/instrument.rs` & `libdaw-0.7.0/python-libdaw/src/nodes/instrument.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/src/nodes/multi_frequency.rs` & `libdaw-0.7.0/python-libdaw/src/nodes/multi_frequency.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/src/nodes/multiply.rs` & `libdaw-0.7.0/python-libdaw/src/nodes/multiply.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/src/nodes/sawtooth_oscillator.rs` & `libdaw-0.7.0/python-libdaw/src/nodes/sawtooth_oscillator.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/src/nodes/sine_oscillator.rs` & `libdaw-0.7.0/python-libdaw/src/nodes/sine_oscillator.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/src/nodes/square_oscillator.rs` & `libdaw-0.7.0/python-libdaw/src/nodes/square_oscillator.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/src/nodes/triangle_oscillator.rs` & `libdaw-0.7.0/python-libdaw/src/nodes/triangle_oscillator.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/src/nodes.rs` & `libdaw-0.7.0/python-libdaw/src/nodes.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/src/notation/chord.rs` & `libdaw-0.7.0/python-libdaw/src/notation/chord.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use super::{NotePitch, StateMember};
+use super::{duration::Duration, NotePitch, StateMember};
 use crate::{
     metronome::{Beat, MaybeMetronome},
     nodes::instrument::Tone,
     pitch::MaybePitchStandard,
     resolve_index, resolve_index_for_insert,
 };
 use libdaw::{metronome::Beat as DawBeat, notation::Chord as DawChord};
@@ -44,26 +44,26 @@
 #[pymethods]
 impl Chord {
     #[new]
     pub fn new(
         py: Python<'_>,
         pitches: Option<Vec<NotePitch>>,
         length: Option<Beat>,
-        duration: Option<Beat>,
+        duration: Option<Duration>,
         state_member: Option<StateMember>,
     ) -> Self {
         let pitches = pitches.unwrap_or_default();
         Self {
             inner: Arc::new(Mutex::new(DawChord {
                 pitches: pitches
                     .iter()
                     .map(move |pitch| pitch.as_inner(py))
                     .collect(),
                 length: length.map(|beat| beat.0),
-                duration: duration.map(|beat| beat.0),
+                duration: duration.map(|duration| duration.inner),
                 state_member: state_member.map(Into::into),
             })),
             pitches,
         }
     }
     #[staticmethod]
     pub fn loads(py: Python<'_>, source: String) -> crate::Result<Py<Self>> {
@@ -99,20 +99,24 @@
         self.inner.lock().expect("poisoned").length.map(Beat)
     }
     #[setter]
     pub fn set_length(&mut self, value: Option<Beat>) {
         self.inner.lock().expect("poisoned").length = value.map(|beat| beat.0);
     }
     #[getter]
-    pub fn get_duration(&self) -> Option<Beat> {
-        self.inner.lock().expect("poisoned").duration.map(Beat)
+    pub fn get_duration(&self) -> Option<Duration> {
+        self.inner
+            .lock()
+            .expect("poisoned")
+            .duration
+            .map(|inner| Duration { inner })
     }
     #[setter]
-    pub fn set_duration(&mut self, value: Option<Beat>) {
-        self.inner.lock().expect("poisoned").duration = value.map(|beat| beat.0);
+    pub fn set_duration(&mut self, value: Option<Duration>) {
+        self.inner.lock().expect("poisoned").duration = value.map(|duration| duration.inner);
     }
     #[getter]
     pub fn get_state_member(&self) -> Option<StateMember> {
         self.inner
             .lock()
             .expect("poisoned")
             .state_member
@@ -185,22 +189,22 @@
         Ok(self.pitches.remove(index))
     }
     pub fn __getnewargs__(
         &self,
     ) -> (
         Vec<NotePitch>,
         Option<Beat>,
-        Option<Beat>,
+        Option<Duration>,
         Option<StateMember>,
     ) {
         let lock = self.inner.lock().expect("poisoned");
         (
             self.pitches.clone(),
             lock.length.map(Beat),
-            lock.duration.map(Beat),
+            lock.duration.map(|inner| Duration { inner }),
             lock.state_member.map(Into::into),
         )
     }
 
     fn __traverse__(&self, visit: PyVisit<'_>) -> Result<(), PyTraverseError> {
         for pitch in &self.pitches {
             visit.call(pitch)?
@@ -211,15 +215,15 @@
     pub fn __clear__(&mut self) {
         self.inner.lock().expect("poisoned").pitches.clear();
         self.pitches.clear();
     }
 }
 
 #[derive(Debug, Clone)]
-#[pyclass(sequence, module = "libdaw.notation")]
+#[pyclass(module = "libdaw.notation")]
 pub struct ChordIterator(pub std::vec::IntoIter<NotePitch>);
 
 #[pymethods]
 impl ChordIterator {
     pub fn __iter__(self_: Bound<'_, Self>) -> Bound<'_, Self> {
         self_
     }
```

### Comparing `libdaw-0.6.0/python-libdaw/src/notation/inversion.rs` & `libdaw-0.7.0/python-libdaw/src/notation/inversion.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/src/notation/item.rs` & `libdaw-0.7.0/python-libdaw/src/notation/item.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/src/notation/note/note_pitch.rs` & `libdaw-0.7.0/python-libdaw/src/notation/note/note_pitch.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/src/notation/note.rs` & `libdaw-0.7.0/python-libdaw/src/notation/note.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 mod note_pitch;
 
 pub use note_pitch::NotePitch;
 
+use super::duration::Duration;
 use crate::{
     metronome::{Beat, MaybeMetronome},
     nodes::instrument::Tone,
     pitch::MaybePitchStandard,
 };
 use libdaw::{metronome::Beat as DawBeat, notation::Note as DawNote};
 use pyo3::{pyclass, pymethods, IntoPy as _, Py, PyTraverseError, PyVisit, Python};
@@ -41,21 +42,21 @@
 #[pymethods]
 impl Note {
     #[new]
     pub fn new(
         py: Python<'_>,
         pitch: NotePitch,
         length: Option<Beat>,
-        duration: Option<Beat>,
+        duration: Option<Duration>,
     ) -> Self {
         Self {
             inner: Arc::new(Mutex::new(DawNote {
                 pitch: pitch.as_inner(py),
                 length: length.map(|beat| beat.0),
-                duration: duration.map(|beat| beat.0),
+                duration: duration.map(move |duration| duration.inner),
             })),
             pitch: Some(pitch),
         }
     }
 
     #[staticmethod]
     pub fn loads(py: Python<'_>, source: String) -> crate::Result<Py<Self>> {
@@ -95,40 +96,44 @@
         ))
     }
 
     #[getter]
     pub fn get_length(&self) -> Option<Beat> {
         self.inner.lock().expect("poisoned").length.map(Beat)
     }
-    #[getter]
-    pub fn get_duration(&self) -> Option<Beat> {
-        self.inner.lock().expect("poisoned").duration.map(Beat)
-    }
     #[setter]
     pub fn set_length(&mut self, value: Option<Beat>) {
         self.inner.lock().expect("poisoned").length = value.map(|beat| beat.0);
     }
+    #[getter]
+    pub fn get_duration(&self) -> Option<Duration> {
+        self.inner
+            .lock()
+            .expect("poisoned")
+            .duration
+            .map(|inner| Duration { inner })
+    }
     #[setter]
-    pub fn set_duration(&mut self, value: Option<Beat>) {
-        self.inner.lock().expect("poisoned").duration = value.map(|beat| beat.0);
+    pub fn set_duration(&mut self, value: Option<Duration>) {
+        self.inner.lock().expect("poisoned").duration = value.map(|duration| duration.inner);
     }
 
     pub fn __repr__(&self) -> String {
         format!("{:?}", self.inner.lock().expect("poisoned").deref())
     }
     pub fn __str__(&self) -> String {
         format!("{:#?}", self.inner.lock().expect("poisoned").deref())
     }
 
-    pub fn __getnewargs__(&self) -> (NotePitch, Option<Beat>, Option<Beat>) {
+    pub fn __getnewargs__(&self) -> (NotePitch, Option<Beat>, Option<Duration>) {
         let lock = self.inner.lock().expect("poisoned");
         (
             self.pitch.clone().expect("cleared"),
             lock.length.map(Beat),
-            lock.duration.map(Beat),
+            lock.duration.map(|inner| Duration { inner }),
         )
     }
 
     fn __traverse__(&self, visit: PyVisit<'_>) -> Result<(), PyTraverseError> {
         if let Some(pitch) = &self.pitch {
             visit.call(pitch)?
         }
```

### Comparing `libdaw-0.6.0/python-libdaw/src/notation/overlapped.rs` & `libdaw-0.7.0/python-libdaw/src/notation/overlapped.rs`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
     pub fn __clear__(&mut self) {
         self.inner.lock().expect("poisoned").items.clear();
         self.items.clear();
     }
 }
 
 #[derive(Debug, Clone)]
-#[pyclass(sequence, module = "libdaw.notation")]
+#[pyclass(module = "libdaw.notation")]
 pub struct OverlappedIterator(pub std::vec::IntoIter<Item>);
 
 #[pymethods]
 impl OverlappedIterator {
     pub fn __iter__(self_: Bound<'_, Self>) -> Bound<'_, Self> {
         self_
     }
```

### Comparing `libdaw-0.6.0/python-libdaw/src/notation/pitch.rs` & `libdaw-0.7.0/python-libdaw/src/notation/pitch.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/src/notation/rest.rs` & `libdaw-0.7.0/python-libdaw/src/notation/rest.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/src/notation/scale.rs` & `libdaw-0.7.0/python-libdaw/src/notation/scale.rs`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     pub fn __clear__(&mut self) {
         self.inner.lock().expect("poisoned").pitches.clear();
         self.pitches.clear();
     }
 }
 
 #[derive(Debug, Clone)]
-#[pyclass(sequence, module = "libdaw.notation")]
+#[pyclass(module = "libdaw.notation")]
 pub struct ScaleIterator(pub std::vec::IntoIter<NotePitch>);
 
 #[pymethods]
 impl ScaleIterator {
     pub fn __iter__(self_: Bound<'_, Self>) -> Bound<'_, Self> {
         self_
     }
```

### Comparing `libdaw-0.6.0/python-libdaw/src/notation/sequence.rs` & `libdaw-0.7.0/python-libdaw/src/notation/sequence.rs`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
     pub fn __clear__(&mut self) {
         self.inner.lock().expect("poisoned").items.clear();
         self.items.clear();
     }
 }
 
 #[derive(Debug, Clone)]
-#[pyclass(sequence, module = "libdaw.notation")]
+#[pyclass(module = "libdaw.notation")]
 pub struct SequenceIterator(pub std::vec::IntoIter<Item>);
 
 #[pymethods]
 impl SequenceIterator {
     pub fn __iter__(self_: Bound<'_, Self>) -> Bound<'_, Self> {
         self_
     }
```

### Comparing `libdaw-0.6.0/python-libdaw/src/notation/set.rs` & `libdaw-0.7.0/python-libdaw/src/notation/set.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use super::NotePitch;
+use super::{duration::Duration, NotePitch};
 use crate::metronome::Beat;
 use libdaw::notation::Set as DawSet;
 use pyo3::{pyclass, pymethods, IntoPy as _, Py, PyTraverseError, PyVisit, Python};
 use std::sync::{Arc, Mutex};
 
 #[pyclass(module = "libdaw.notation")]
 #[derive(Debug, Clone)]
@@ -27,19 +27,25 @@
             .unbind()
     }
 }
 
 #[pymethods]
 impl Set {
     #[new]
-    pub fn new(py: Python<'_>, pitch: Option<NotePitch>, length: Option<Beat>) -> Self {
+    pub fn new(
+        py: Python<'_>,
+        pitch: Option<NotePitch>,
+        length: Option<Beat>,
+        duration: Option<Duration>,
+    ) -> Self {
         Self {
             inner: Arc::new(Mutex::new(DawSet {
                 pitch: pitch.as_ref().map(move |pitch| pitch.as_inner(py)),
                 length: length.map(|beat| beat.0),
+                duration: duration.map(|duration| duration.inner),
             })),
             pitch,
         }
     }
     #[staticmethod]
     pub fn loads(py: Python<'_>, source: String) -> crate::Result<Py<Self>> {
         Ok(Self::from_inner(py, Arc::new(Mutex::new(source.parse()?))))
@@ -59,24 +65,41 @@
         self.inner.lock().expect("poisoned").length.map(Beat)
     }
     #[setter]
     pub fn set_length(&mut self, value: Option<Beat>) {
         self.inner.lock().expect("poisoned").length = value.map(|beat| beat.0);
     }
 
+    #[getter]
+    pub fn get_duration(&self) -> Option<Duration> {
+        self.inner
+            .lock()
+            .expect("poisoned")
+            .duration
+            .map(|inner| Duration { inner })
+    }
+    #[setter]
+    pub fn set_duration(&mut self, value: Option<Duration>) {
+        self.inner.lock().expect("poisoned").duration = value.map(|duration| duration.inner);
+    }
+
     pub fn __repr__(&self) -> String {
         format!("{:?}", self.inner.lock().expect("poisoned"))
     }
     pub fn __str__(&self) -> String {
         format!("{:#?}", self.inner.lock().expect("poisoned"))
     }
 
-    pub fn __getnewargs__(&self) -> (Option<NotePitch>, Option<Beat>) {
+    pub fn __getnewargs__(&self) -> (Option<NotePitch>, Option<Beat>, Option<Duration>) {
         let lock = self.inner.lock().expect("poisoned");
-        (self.pitch.clone(), lock.length.map(Beat))
+        (
+            self.pitch.clone(),
+            lock.length.map(Beat),
+            lock.duration.map(|inner| Duration { inner }),
+        )
     }
 
     fn __traverse__(&self, visit: PyVisit<'_>) -> Result<(), PyTraverseError> {
         for pitch in &self.pitch {
             visit.call(pitch)?
         }
         Ok(())
```

### Comparing `libdaw-0.6.0/python-libdaw/src/notation/state_member.rs` & `libdaw-0.7.0/python-libdaw/src/notation/state_member.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/src/notation/step.rs` & `libdaw-0.7.0/python-libdaw/src/notation/step.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/src/notation.rs` & `libdaw-0.7.0/python-libdaw/src/notation.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 mod chord;
+pub mod duration;
 mod inversion;
 mod item;
 mod note;
 mod overlapped;
 mod pitch;
 mod rest;
 mod scale;
@@ -20,14 +21,15 @@
 pub use rest::Rest;
 pub use scale::Scale;
 pub use sequence::Sequence;
 pub use set::Set;
 pub use state_member::StateMember;
 pub use step::Step;
 
+use crate::submodule;
 use pyo3::{
     types::{PyModule, PyModuleMethods as _},
     wrap_pyfunction, Bound, PyResult,
 };
 
 pub fn register(module: &Bound<'_, PyModule>) -> PyResult<()> {
     module.add_function(wrap_pyfunction!(item::loads, module)?)?;
@@ -38,9 +40,10 @@
     module.add_class::<Pitch>()?;
     module.add_class::<Rest>()?;
     module.add_class::<Scale>()?;
     module.add_class::<Sequence>()?;
     module.add_class::<Set>()?;
     module.add_class::<StateMember>()?;
     module.add_class::<Step>()?;
+    duration::register(&submodule!(module, "libdaw.notation", "duration"))?;
     Ok(())
 }
```

### Comparing `libdaw-0.6.0/python-libdaw/src/pitch/pitch.rs` & `libdaw-0.7.0/python-libdaw/src/pitch/pitch.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/src/pitch.rs` & `libdaw-0.7.0/python-libdaw/src/pitch.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/src/play.rs` & `libdaw-0.7.0/python-libdaw/src/play.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python-libdaw/src/stream.rs` & `libdaw-0.7.0/python-libdaw/src/stream.rs`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 use pyo3::{
     pyclass, pymethods,
     types::{PyAnyMethods as _, PyInt},
     Bound, PyAny, PyResult,
 };
 
 #[derive(Debug, Clone)]
-#[pyclass(sequence, module = "libdaw")]
+#[pyclass(module = "libdaw")]
 pub struct Stream(pub DawStream);
 
 #[pymethods]
 impl Stream {
     #[new]
     pub fn new(value: Bound<'_, PyAny>) -> PyResult<Self> {
         if let Ok(channels) = value.downcast::<PyInt>() {
@@ -74,15 +74,15 @@
 
     pub fn __iter__(&self) -> StreamIterator {
         StreamIterator(self.0.clone().into_iter())
     }
 }
 
 #[derive(Debug, Clone)]
-#[pyclass(sequence, module = "libdaw")]
+#[pyclass(module = "libdaw")]
 pub struct StreamIterator(pub <DawStream as IntoIterator>::IntoIter);
 
 #[pymethods]
 impl StreamIterator {
     pub fn __iter__(self_: Bound<'_, Self>) -> Bound<'_, Self> {
         self_
     }
```

### Comparing `libdaw-0.6.0/python-libdaw/src/time.rs` & `libdaw-0.7.0/python-libdaw/src/time.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/Cargo.lock` & `libdaw-0.7.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -351,15 +351,15 @@
 name = "libc"
 version = "0.2.155"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "97b3888a4aecf77e811145cadf6eef5901f4782c53886191b2f693f24761847c"
 
 [[package]]
 name = "libdaw"
-version = "0.6.0"
+version = "0.7.0"
 dependencies = [
  "nohash-hasher",
  "nom",
  "ordered-float",
 ]
 
 [[package]]
@@ -665,15 +665,15 @@
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "python-libdaw"
-version = "0.6.0"
+version = "0.7.0"
 dependencies = [
  "libdaw",
  "nohash-hasher",
  "pyo3",
  "rodio",
 ]
```

### Comparing `libdaw-0.6.0/pyproject.toml` & `libdaw-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python/libdaw/notation.pyi` & `libdaw-0.7.0/python/libdaw/notation.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python/libdaw/pitch.pyi` & `libdaw-0.7.0/python/libdaw/pitch.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python/libdaw/time.pyi` & `libdaw-0.7.0/python/libdaw/time.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python/libdaw/__init__.pyi` & `libdaw-0.7.0/python/libdaw/__init__.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python/libdaw/metronome.pyi` & `libdaw-0.7.0/python/libdaw/metronome.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/python/libdaw/nodes/__init__.pyi` & `libdaw-0.7.0/python/libdaw/nodes/__init__.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.6.0/PKG-INFO` & `libdaw-0.7.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: libdaw
-Version: 0.6.0
+Version: 0.7.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 License: MPL 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

