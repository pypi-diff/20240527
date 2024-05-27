# Comparing `tmp/accesskit-0.3.3.tar.gz` & `tmp/accesskit-0.3.4.tar.gz`

## Comparing `accesskit-0.3.3.tar` & `accesskit-0.3.4.tar`

### file list

```diff
@@ -1,96 +1,96 @@
--rw-r--r--   0     1001      127      942 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/macos/Cargo.toml
--rw-r--r--   0     1001      127    16504 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/macos/CHANGELOG.md
--rw-r--r--   0     1001      127      183 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/macos/README.md
--rw-r--r--   0     1001      127     9554 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/macos/src/adapter.rs
--rw-r--r--   0     1001      127     2731 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/macos/src/context.rs
--rw-r--r--   0     1001      127     8399 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/macos/src/event.rs
--rw-r--r--   0     1001      127      282 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/macos/src/filters.rs
--rw-r--r--   0     1001      127      557 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/macos/src/lib.rs
--rw-r--r--   0     1001      127    33207 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/macos/src/node.rs
--rw-r--r--   0     1001      127     3146 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/macos/src/patch.rs
--rw-r--r--   0     1001      127     9523 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/macos/src/subclass.rs
--rw-r--r--   0     1001      127     2819 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/macos/src/util.rs
--rw-r--r--   0     1001      127      705 2024-05-26 10:52:10.000000 accesskit-0.3.3/common/Cargo.toml
--rw-r--r--   0     1001      127    15163 2024-05-26 10:52:10.000000 accesskit-0.3.3/common/CHANGELOG.md
--rw-r--r--   0     1001      127      740 2024-05-26 10:52:10.000000 accesskit-0.3.3/common/README.md
--rw-r--r--   0     1001      127    22792 2024-05-26 10:52:10.000000 accesskit-0.3.3/common/src/geometry.rs
--rw-r--r--   0     1001      127    78839 2024-05-26 10:52:10.000000 accesskit-0.3.3/common/src/lib.rs
--rw-r--r--   0     1001      127      435 2024-05-26 10:52:10.000000 accesskit-0.3.3/consumer/Cargo.toml
--rw-r--r--   0     1001      127    20361 2024-05-26 10:52:10.000000 accesskit-0.3.3/consumer/CHANGELOG.md
--rw-r--r--   0     1001      127      207 2024-05-26 10:52:10.000000 accesskit-0.3.3/consumer/README.md
--rw-r--r--   0     1001      127      958 2024-05-26 10:52:10.000000 accesskit-0.3.3/consumer/src/filters.rs
--rw-r--r--   0     1001      127    25548 2024-05-26 10:52:10.000000 accesskit-0.3.3/consumer/src/iterators.rs
--rw-r--r--   0     1001      127     7678 2024-05-26 10:52:10.000000 accesskit-0.3.3/consumer/src/lib.rs
--rw-r--r--   0     1001      127    31990 2024-05-26 10:52:10.000000 accesskit-0.3.3/consumer/src/node.rs
--rw-r--r--   0     1001      127    71808 2024-05-26 10:52:10.000000 accesskit-0.3.3/consumer/src/text.rs
--rw-r--r--   0     1001      127    27118 2024-05-26 10:52:10.000000 accesskit-0.3.3/consumer/src/tree.rs
--rw-r--r--   0     1001      127      956 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/windows/Cargo.toml
--rw-r--r--   0     1001      127    26831 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/windows/CHANGELOG.md
--rw-r--r--   0     1001      127      172 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/windows/README.md
--rw-r--r--   0     1001      127    11651 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/windows/examples/hello_world.rs
--rw-r--r--   0     1001      127    15277 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/windows/src/adapter.rs
--rw-r--r--   0     1001      127     1850 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/windows/src/context.rs
--rw-r--r--   0     1001      127      356 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/windows/src/filters.rs
--rw-r--r--   0     1001      127      482 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/windows/src/lib.rs
--rw-r--r--   0     1001      127    37084 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/windows/src/node.rs
--rw-r--r--   0     1001      127     6179 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/windows/src/subclass.rs
--rw-r--r--   0     1001      127    11438 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/windows/src/tests/mod.rs
--rw-r--r--   0     1001      127     6937 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/windows/src/tests/simple.rs
--rw-r--r--   0     1001      127     3536 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/windows/src/tests/subclassed.rs
--rw-r--r--   0     1001      127    19711 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/windows/src/text.rs
--rw-r--r--   0     1001      127     6500 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/windows/src/util.rs
--rw-r--r--   0     1001      127     1295 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/Cargo.toml
--rw-r--r--   0     1001      127    12315 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/CHANGELOG.md
--rw-r--r--   0     1001      127      487 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/README.md
--rw-r--r--   0     1001      127     6935 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/src/adapter.rs
--rw-r--r--   0     1001      127    16200 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/src/atspi/bus.rs
--rw-r--r--   0     1001      127     6218 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/src/atspi/interfaces/accessible.rs
--rw-r--r--   0     1001      127     1473 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/src/atspi/interfaces/action.rs
--rw-r--r--   0     1001      127     1096 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/src/atspi/interfaces/application.rs
--rw-r--r--   0     1001      127     2195 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/src/atspi/interfaces/component.rs
--rw-r--r--   0     1001      127      979 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/src/atspi/interfaces/mod.rs
--rw-r--r--   0     1001      127     4767 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/src/atspi/interfaces/text.rs
--rw-r--r--   0     1001      127     1459 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/src/atspi/interfaces/value.rs
--rw-r--r--   0     1001      127      404 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/src/atspi/mod.rs
--rw-r--r--   0     1001      127     1224 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/src/atspi/object_address.rs
--rw-r--r--   0     1001      127     2185 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/src/atspi/object_id.rs
--rw-r--r--   0     1001      127     8048 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/src/context.rs
--rw-r--r--   0     1001      127     4885 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/src/executor.rs
--rw-r--r--   0     1001      127     1005 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/src/lib.rs
--rw-r--r--   0     1001      127     1616 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/src/util.rs
--rw-r--r--   0     1001      127      670 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/atspi-common/Cargo.toml
--rw-r--r--   0     1001      127     5243 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/atspi-common/CHANGELOG.md
--rw-r--r--   0     1001      127      317 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/atspi-common/README.md
--rw-r--r--   0     1001      127      432 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/atspi-common/src/action.rs
--rw-r--r--   0     1001      127    18429 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/atspi-common/src/adapter.rs
--rw-r--r--   0     1001      127      583 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/atspi-common/src/callback.rs
--rw-r--r--   0     1001      127     3414 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/atspi-common/src/context.rs
--rw-r--r--   0     1001      127      677 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/atspi-common/src/error.rs
--rw-r--r--   0     1001      127     1278 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/atspi-common/src/events.rs
--rw-r--r--   0     1001      127      282 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/atspi-common/src/filters.rs
--rw-r--r--   0     1001      127      785 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/atspi-common/src/lib.rs
--rw-r--r--   0     1001      127    47783 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/atspi-common/src/node.rs
--rw-r--r--   0     1001      127      898 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/atspi-common/src/rect.rs
--rw-r--r--   0     1001      127    20319 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/atspi-common/src/simplified.rs
--rw-r--r--   0     1001      127     4041 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/atspi-common/src/util.rs
--rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 accesskit-0.3.3/bindings/python/Cargo.toml
--rw-r--r--   0     1001      127      224 2024-05-26 10:52:10.000000 accesskit-0.3.3/bindings/python/.cargo/config.toml
--rw-r--r--   0     1001      127     5791 2024-05-26 10:52:10.000000 accesskit-0.3.3/bindings/python/CHANGELOG.md
--rw-r--r--   0     1001      127      981 2024-05-26 10:52:10.000000 accesskit-0.3.3/bindings/python/README.md
--rw-r--r--   0     1001      127     3078 2024-05-26 10:52:10.000000 accesskit-0.3.3/bindings/python/examples/pygame/.gitignore
--rw-r--r--   0     1001      127      367 2024-05-26 10:52:10.000000 accesskit-0.3.3/bindings/python/examples/pygame/README.md
--rw-r--r--   0     1001      127     6979 2024-05-26 10:52:10.000000 accesskit-0.3.3/bindings/python/examples/pygame/hello_world.py
--rw-r--r--   0     1001      127       24 2024-05-26 10:52:10.000000 accesskit-0.3.3/bindings/python/examples/pygame/requirements.txt
--rw-r--r--   0     1001      127    24191 2024-05-26 10:52:10.000000 accesskit-0.3.3/bindings/python/src/common.rs
--rw-r--r--   0     1001      127     4784 2024-05-26 10:52:10.000000 accesskit-0.3.3/bindings/python/src/geometry.rs
--rw-r--r--   0     1001      127     2818 2024-05-26 10:52:10.000000 accesskit-0.3.3/bindings/python/src/lib.rs
--rw-r--r--   0     1001      127     7316 2024-05-26 10:52:10.000000 accesskit-0.3.3/bindings/python/src/macos.rs
--rw-r--r--   0     1001      127     1506 2024-05-26 10:52:10.000000 accesskit-0.3.3/bindings/python/src/unix.rs
--rw-r--r--   0     1001      127     4126 2024-05-26 10:52:10.000000 accesskit-0.3.3/bindings/python/src/windows.rs
--rw-r--r--   0     1001      127    73418 2024-05-26 10:52:10.000000 accesskit-0.3.3/Cargo.lock
--rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 accesskit-0.3.3/Cargo.toml
--rw-r--r--   0     1001      127     1043 2024-05-26 10:52:10.000000 accesskit-0.3.3/pyproject.toml
--rw-r--r--   0     1001      127     9723 2024-05-26 10:52:10.000000 accesskit-0.3.3/LICENSE-APACHE
--rw-r--r--   0     1001      127     1023 2024-05-26 10:52:10.000000 accesskit-0.3.3/LICENSE-MIT
--rw-r--r--   0     1001      127     1559 2024-05-26 10:52:10.000000 accesskit-0.3.3/LICENSE.chromium
--rw-r--r--   0        0        0     1958 1970-01-01 00:00:00.000000 accesskit-0.3.3/PKG-INFO
+-rw-r--r--   0     1001      127      435 2024-05-27 18:05:10.000000 accesskit-0.3.4/consumer/Cargo.toml
+-rw-r--r--   0     1001      127    20703 2024-05-27 18:05:10.000000 accesskit-0.3.4/consumer/CHANGELOG.md
+-rw-r--r--   0     1001      127      207 2024-05-27 18:05:10.000000 accesskit-0.3.4/consumer/README.md
+-rw-r--r--   0     1001      127      958 2024-05-27 18:05:10.000000 accesskit-0.3.4/consumer/src/filters.rs
+-rw-r--r--   0     1001      127    25548 2024-05-27 18:05:10.000000 accesskit-0.3.4/consumer/src/iterators.rs
+-rw-r--r--   0     1001      127     7678 2024-05-27 18:05:10.000000 accesskit-0.3.4/consumer/src/lib.rs
+-rw-r--r--   0     1001      127    32099 2024-05-27 18:05:10.000000 accesskit-0.3.4/consumer/src/node.rs
+-rw-r--r--   0     1001      127    71808 2024-05-27 18:05:10.000000 accesskit-0.3.4/consumer/src/text.rs
+-rw-r--r--   0     1001      127    27118 2024-05-27 18:05:10.000000 accesskit-0.3.4/consumer/src/tree.rs
+-rw-r--r--   0     1001      127      956 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/windows/Cargo.toml
+-rw-r--r--   0     1001      127    27314 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/windows/CHANGELOG.md
+-rw-r--r--   0     1001      127      172 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/windows/README.md
+-rw-r--r--   0     1001      127    11651 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/windows/examples/hello_world.rs
+-rw-r--r--   0     1001      127    15277 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/windows/src/adapter.rs
+-rw-r--r--   0     1001      127     1850 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/windows/src/context.rs
+-rw-r--r--   0     1001      127      356 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/windows/src/filters.rs
+-rw-r--r--   0     1001      127      482 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/windows/src/lib.rs
+-rw-r--r--   0     1001      127    37418 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/windows/src/node.rs
+-rw-r--r--   0     1001      127     6179 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/windows/src/subclass.rs
+-rw-r--r--   0     1001      127    11438 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/windows/src/tests/mod.rs
+-rw-r--r--   0     1001      127     6937 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/windows/src/tests/simple.rs
+-rw-r--r--   0     1001      127     3536 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/windows/src/tests/subclassed.rs
+-rw-r--r--   0     1001      127    19711 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/windows/src/text.rs
+-rw-r--r--   0     1001      127     6625 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/windows/src/util.rs
+-rw-r--r--   0     1001      127     1295 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/unix/Cargo.toml
+-rw-r--r--   0     1001      127    12441 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/unix/CHANGELOG.md
+-rw-r--r--   0     1001      127      487 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/unix/README.md
+-rw-r--r--   0     1001      127     6935 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/unix/src/adapter.rs
+-rw-r--r--   0     1001      127    16200 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/unix/src/atspi/bus.rs
+-rw-r--r--   0     1001      127     6218 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/unix/src/atspi/interfaces/accessible.rs
+-rw-r--r--   0     1001      127     1473 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/unix/src/atspi/interfaces/action.rs
+-rw-r--r--   0     1001      127     1096 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/unix/src/atspi/interfaces/application.rs
+-rw-r--r--   0     1001      127     2195 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/unix/src/atspi/interfaces/component.rs
+-rw-r--r--   0     1001      127      979 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/unix/src/atspi/interfaces/mod.rs
+-rw-r--r--   0     1001      127     4767 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/unix/src/atspi/interfaces/text.rs
+-rw-r--r--   0     1001      127     1459 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/unix/src/atspi/interfaces/value.rs
+-rw-r--r--   0     1001      127      404 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/unix/src/atspi/mod.rs
+-rw-r--r--   0     1001      127     1224 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/unix/src/atspi/object_address.rs
+-rw-r--r--   0     1001      127     2185 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/unix/src/atspi/object_id.rs
+-rw-r--r--   0     1001      127     8048 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/unix/src/context.rs
+-rw-r--r--   0     1001      127     4885 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/unix/src/executor.rs
+-rw-r--r--   0     1001      127     1005 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/unix/src/lib.rs
+-rw-r--r--   0     1001      127     1616 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/unix/src/util.rs
+-rw-r--r--   0     1001      127      670 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/atspi-common/Cargo.toml
+-rw-r--r--   0     1001      127     5969 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/atspi-common/CHANGELOG.md
+-rw-r--r--   0     1001      127      317 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/atspi-common/README.md
+-rw-r--r--   0     1001      127      432 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/atspi-common/src/action.rs
+-rw-r--r--   0     1001      127    18471 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/atspi-common/src/adapter.rs
+-rw-r--r--   0     1001      127      583 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/atspi-common/src/callback.rs
+-rw-r--r--   0     1001      127     3414 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/atspi-common/src/context.rs
+-rw-r--r--   0     1001      127      677 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/atspi-common/src/error.rs
+-rw-r--r--   0     1001      127     1278 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/atspi-common/src/events.rs
+-rw-r--r--   0     1001      127      282 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/atspi-common/src/filters.rs
+-rw-r--r--   0     1001      127      785 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/atspi-common/src/lib.rs
+-rw-r--r--   0     1001      127    48041 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/atspi-common/src/node.rs
+-rw-r--r--   0     1001      127      898 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/atspi-common/src/rect.rs
+-rw-r--r--   0     1001      127    20319 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/atspi-common/src/simplified.rs
+-rw-r--r--   0     1001      127     4041 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/atspi-common/src/util.rs
+-rw-r--r--   0     1001      127      705 2024-05-27 18:05:10.000000 accesskit-0.3.4/common/Cargo.toml
+-rw-r--r--   0     1001      127    15163 2024-05-27 18:05:10.000000 accesskit-0.3.4/common/CHANGELOG.md
+-rw-r--r--   0     1001      127      740 2024-05-27 18:05:10.000000 accesskit-0.3.4/common/README.md
+-rw-r--r--   0     1001      127    22792 2024-05-27 18:05:10.000000 accesskit-0.3.4/common/src/geometry.rs
+-rw-r--r--   0     1001      127    78839 2024-05-27 18:05:10.000000 accesskit-0.3.4/common/src/lib.rs
+-rw-r--r--   0     1001      127      942 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/macos/Cargo.toml
+-rw-r--r--   0     1001      127    16983 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/macos/CHANGELOG.md
+-rw-r--r--   0     1001      127      183 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/macos/README.md
+-rw-r--r--   0     1001      127     9554 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/macos/src/adapter.rs
+-rw-r--r--   0     1001      127     2731 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/macos/src/context.rs
+-rw-r--r--   0     1001      127     8399 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/macos/src/event.rs
+-rw-r--r--   0     1001      127      282 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/macos/src/filters.rs
+-rw-r--r--   0     1001      127      557 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/macos/src/lib.rs
+-rw-r--r--   0     1001      127    33827 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/macos/src/node.rs
+-rw-r--r--   0     1001      127     3146 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/macos/src/patch.rs
+-rw-r--r--   0     1001      127     9523 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/macos/src/subclass.rs
+-rw-r--r--   0     1001      127     2819 2024-05-27 18:05:10.000000 accesskit-0.3.4/platforms/macos/src/util.rs
+-rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 accesskit-0.3.4/bindings/python/Cargo.toml
+-rw-r--r--   0     1001      127      224 2024-05-27 18:05:10.000000 accesskit-0.3.4/bindings/python/.cargo/config.toml
+-rw-r--r--   0     1001      127     6015 2024-05-27 18:05:10.000000 accesskit-0.3.4/bindings/python/CHANGELOG.md
+-rw-r--r--   0     1001      127      981 2024-05-27 18:05:10.000000 accesskit-0.3.4/bindings/python/README.md
+-rw-r--r--   0     1001      127     3078 2024-05-27 18:05:10.000000 accesskit-0.3.4/bindings/python/examples/pygame/.gitignore
+-rw-r--r--   0     1001      127      367 2024-05-27 18:05:10.000000 accesskit-0.3.4/bindings/python/examples/pygame/README.md
+-rw-r--r--   0     1001      127     6979 2024-05-27 18:05:10.000000 accesskit-0.3.4/bindings/python/examples/pygame/hello_world.py
+-rw-r--r--   0     1001      127       24 2024-05-27 18:05:10.000000 accesskit-0.3.4/bindings/python/examples/pygame/requirements.txt
+-rw-r--r--   0     1001      127    24191 2024-05-27 18:05:10.000000 accesskit-0.3.4/bindings/python/src/common.rs
+-rw-r--r--   0     1001      127     4784 2024-05-27 18:05:10.000000 accesskit-0.3.4/bindings/python/src/geometry.rs
+-rw-r--r--   0     1001      127     2818 2024-05-27 18:05:10.000000 accesskit-0.3.4/bindings/python/src/lib.rs
+-rw-r--r--   0     1001      127     7316 2024-05-27 18:05:10.000000 accesskit-0.3.4/bindings/python/src/macos.rs
+-rw-r--r--   0     1001      127     1506 2024-05-27 18:05:10.000000 accesskit-0.3.4/bindings/python/src/unix.rs
+-rw-r--r--   0     1001      127     4126 2024-05-27 18:05:10.000000 accesskit-0.3.4/bindings/python/src/windows.rs
+-rw-r--r--   0     1001      127    73418 2024-05-27 18:05:10.000000 accesskit-0.3.4/Cargo.lock
+-rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 accesskit-0.3.4/Cargo.toml
+-rw-r--r--   0     1001      127     1043 2024-05-27 18:05:10.000000 accesskit-0.3.4/pyproject.toml
+-rw-r--r--   0     1001      127     9723 2024-05-27 18:05:10.000000 accesskit-0.3.4/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1023 2024-05-27 18:05:10.000000 accesskit-0.3.4/LICENSE-MIT
+-rw-r--r--   0     1001      127     1559 2024-05-27 18:05:10.000000 accesskit-0.3.4/LICENSE.chromium
+-rw-r--r--   0        0        0     1958 1970-01-01 00:00:00.000000 accesskit-0.3.4/PKG-INFO
```

### Comparing `accesskit-0.3.3/platforms/macos/Cargo.toml` & `accesskit-0.3.4/platforms/macos/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "accesskit_macos"
-version = "0.14.0"
+version = "0.15.0"
 authors.workspace = true
 license.workspace = true
 description = "AccessKit UI accessibility infrastructure: macOS adapter"
 categories.workspace = true
 keywords = ["gui", "ui", "accessibility"]
 repository.workspace = true
 readme = "README.md"
@@ -12,15 +12,15 @@
 rust-version.workspace = true
 
 [package.metadata.docs.rs]
 default-target = "x86_64-apple-darwin"
 
 [dependencies]
 accesskit = { version = "0.14.0", path = "../../common" }
-accesskit_consumer = { version = "0.21.0", path = "../../consumer" }
+accesskit_consumer = { version = "0.22.0", path = "../../consumer" }
 once_cell = "1.13.0"
 objc2 = "0.5.1"
 objc2-foundation = { version = "0.2.0", features = [
     "NSArray",
     "NSDictionary",
     "NSValue",
     "NSThread",
```

### Comparing `accesskit-0.3.3/platforms/macos/CHANGELOG.md` & `accesskit-0.3.4/platforms/macos/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,28 @@
     * accesskit bumped from 0.12.2 to 0.12.3
     * accesskit_consumer bumped from 0.17.0 to 0.17.1
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit_consumer bumped from 0.19.0 to 0.19.1
 
+## [0.15.0](https://github.com/AccessKit/accesskit/compare/accesskit_macos-v0.14.0...accesskit_macos-v0.15.0) (2024-05-27)
+
+
+### Features
+
+* Expose the `orientation` property ([#421](https://github.com/AccessKit/accesskit/issues/421)) ([590aada](https://github.com/AccessKit/accesskit/commit/590aada070dc812f9b8f171fb9e43ac984fad2a1))
+
+
+### Dependencies
+
+* The following workspace dependencies were updated
+  * dependencies
+    * accesskit_consumer bumped from 0.21.0 to 0.22.0
+
 ## [0.14.0](https://github.com/AccessKit/accesskit/compare/accesskit_macos-v0.13.2...accesskit_macos-v0.14.0) (2024-05-26)
 
 
 ### Features
 
 * Expose the `placeholder` property ([#417](https://github.com/AccessKit/accesskit/issues/417)) ([8f4a0a1](https://github.com/AccessKit/accesskit/commit/8f4a0a1c10f83fcc8580a37d8013fec2d110865b))
```

### Comparing `accesskit-0.3.3/platforms/macos/src/adapter.rs` & `accesskit-0.3.4/platforms/macos/src/adapter.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/macos/src/context.rs` & `accesskit-0.3.4/platforms/macos/src/context.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/macos/src/event.rs` & `accesskit-0.3.4/platforms/macos/src/event.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/macos/src/lib.rs` & `accesskit-0.3.4/platforms/macos/src/lib.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/macos/src/node.rs` & `accesskit-0.3.4/platforms/macos/src/node.rs`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 // Derived from Chromium's accessibility abstraction.
 // Copyright 2018 The Chromium Authors. All rights reserved.
 // Use of this source code is governed by a BSD-style license that can be
 // found in the LICENSE.chromium file.
 
 #![allow(non_upper_case_globals)]
 
-use accesskit::{Action, ActionData, ActionRequest, NodeId, Role, TextSelection, Toggled};
+use accesskit::{
+    Action, ActionData, ActionRequest, NodeId, Orientation, Role, TextSelection, Toggled,
+};
 use accesskit_consumer::{FilterResult, Node};
 use objc2::{
     declare_class, msg_send_id,
     mutability::InteriorMutable,
     rc::Id,
     runtime::{AnyObject, Sel},
     sel, ClassType, DeclaredClass,
@@ -463,14 +465,26 @@
         fn max_value(&self) -> Option<Id<NSNumber>> {
             self.resolve(|node| {
                 node.max_numeric_value().map(NSNumber::new_f64)
             })
             .flatten()
         }
 
+        #[method(accessibilityOrientation)]
+        fn orientation(&self) -> NSAccessibilityOrientation {
+            self.resolve(|node| {
+                match node.orientation() {
+                    Some(Orientation::Horizontal) => NSAccessibilityOrientation::Horizontal,
+                    Some(Orientation::Vertical) => NSAccessibilityOrientation::Vertical,
+                    None => NSAccessibilityOrientation::Unknown,
+                }
+            })
+            .unwrap_or(NSAccessibilityOrientation::Unknown)
+        }
+
         #[method(isAccessibilityElement)]
         fn is_accessibility_element(&self) -> bool {
             self.resolve(|node| filter(node) == FilterResult::Include)
                 .unwrap_or(false)
         }
 
         #[method(isAccessibilityFocused)]
@@ -765,14 +779,15 @@
                     || selector == sel!(accessibilityRoleDescription)
                     || selector == sel!(accessibilityTitle)
                     || selector == sel!(accessibilityHelp)
                     || selector == sel!(accessibilityPlaceholderValue)
                     || selector == sel!(accessibilityValue)
                     || selector == sel!(accessibilityMinValue)
                     || selector == sel!(accessibilityMaxValue)
+                    || selector == sel!(accessibilityOrientation)
                     || selector == sel!(isAccessibilityElement)
                     || selector == sel!(isAccessibilityFocused)
                     || selector == sel!(accessibilityNotifiesWhenDestroyed)
                     || selector == sel!(isAccessibilitySelectorAllowed:)
             })
             .unwrap_or(false)
         }
```

### Comparing `accesskit-0.3.3/platforms/macos/src/patch.rs` & `accesskit-0.3.4/platforms/macos/src/patch.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/macos/src/subclass.rs` & `accesskit-0.3.4/platforms/macos/src/subclass.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/macos/src/util.rs` & `accesskit-0.3.4/platforms/macos/src/util.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/common/Cargo.toml` & `accesskit-0.3.4/common/Cargo.toml`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/common/CHANGELOG.md` & `accesskit-0.3.4/common/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/common/README.md` & `accesskit-0.3.4/common/README.md`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/common/src/geometry.rs` & `accesskit-0.3.4/common/src/geometry.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/common/src/lib.rs` & `accesskit-0.3.4/common/src/lib.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/consumer/CHANGELOG.md` & `accesskit-0.3.4/consumer/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,21 @@
   * dependencies
     * accesskit bumped from 0.11.1 to 0.11.2
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit bumped from 0.12.2 to 0.12.3
 
+## [0.22.0](https://github.com/AccessKit/accesskit/compare/accesskit_consumer-v0.21.0...accesskit_consumer-v0.22.0) (2024-05-27)
+
+
+### Features
+
+* Expose the `orientation` property ([#421](https://github.com/AccessKit/accesskit/issues/421)) ([590aada](https://github.com/AccessKit/accesskit/commit/590aada070dc812f9b8f171fb9e43ac984fad2a1))
+
 ## [0.21.0](https://github.com/AccessKit/accesskit/compare/accesskit_consumer-v0.20.0...accesskit_consumer-v0.21.0) (2024-05-26)
 
 
 ### Features
 
 * Add basic text support on Unix ([#362](https://github.com/AccessKit/accesskit/issues/362)) ([52540f8](https://github.com/AccessKit/accesskit/commit/52540f82cf9fc148358351ed486bab3e7e91f1d6))
 * Expose the `placeholder` property ([#417](https://github.com/AccessKit/accesskit/issues/417)) ([8f4a0a1](https://github.com/AccessKit/accesskit/commit/8f4a0a1c10f83fcc8580a37d8013fec2d110865b))
```

### Comparing `accesskit-0.3.3/consumer/src/filters.rs` & `accesskit-0.3.4/consumer/src/filters.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/consumer/src/iterators.rs` & `accesskit-0.3.4/consumer/src/iterators.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/consumer/src/lib.rs` & `accesskit-0.3.4/consumer/src/lib.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/consumer/src/node.rs` & `accesskit-0.3.4/consumer/src/node.rs`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 // Copyright 2021 The Chromium Authors. All rights reserved.
 // Use of this source code is governed by a BSD-style license that can be
 // found in the LICENSE.chromium file.
 
 use std::{iter::FusedIterator, sync::Arc};
 
 use accesskit::{
-    Action, Affine, DefaultActionVerb, Live, Node as NodeData, NodeId, Point, Rect, Role,
-    TextSelection, Toggled,
+    Action, Affine, DefaultActionVerb, Live, Node as NodeData, NodeId, Orientation, Point, Rect,
+    Role, TextSelection, Toggled,
 };
 
 use crate::filters::FilterResult;
 use crate::iterators::{
     FilteredChildren, FollowingFilteredSiblings, FollowingSiblings, LabelledBy,
     PrecedingFilteredSiblings, PrecedingSiblings,
 };
@@ -392,14 +392,18 @@
         )
     }
 
     pub fn is_multiline(&self) -> bool {
         self.role() == Role::MultilineTextInput
     }
 
+    pub fn orientation(&self) -> Option<Orientation> {
+        self.data().orientation()
+    }
+
     pub fn default_action_verb(&self) -> Option<DefaultActionVerb> {
         self.data().default_action_verb()
     }
 
     // When probing for supported actions as the next several functions do,
     // it's tempting to check the role. But it's better to not assume anything
     // beyond what the provider has explicitly told us. Rationale:
```

### Comparing `accesskit-0.3.3/consumer/src/text.rs` & `accesskit-0.3.4/consumer/src/text.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/consumer/src/tree.rs` & `accesskit-0.3.4/consumer/src/tree.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/windows/Cargo.toml` & `accesskit-0.3.4/platforms/windows/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [package]
 name = "accesskit_windows"
-version = "0.19.0"
+version = "0.20.0"
 authors.workspace = true
 license.workspace = true
 description = "AccessKit UI accessibility infrastructure: Windows adapter"
 categories.workspace = true
 keywords = ["gui", "ui", "accessibility"]
 repository.workspace = true
 readme = "README.md"
 edition.workspace = true
 rust-version.workspace = true
 
 [dependencies]
 accesskit = { version = "0.14.0", path = "../../common" }
-accesskit_consumer = { version = "0.21.0", path = "../../consumer" }
+accesskit_consumer = { version = "0.22.0", path = "../../consumer" }
 paste = "1.0"
 static_assertions = "1.1.0"
 
 [dependencies.windows]
 version = "0.54"
 features = [
     "implement",
```

### Comparing `accesskit-0.3.3/platforms/windows/CHANGELOG.md` & `accesskit-0.3.4/platforms/windows/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,28 @@
     * accesskit_consumer bumped from 0.15.1 to 0.15.2
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit bumped from 0.12.2 to 0.12.3
     * accesskit_consumer bumped from 0.17.0 to 0.17.1
 
+## [0.20.0](https://github.com/AccessKit/accesskit/compare/accesskit_windows-v0.19.0...accesskit_windows-v0.20.0) (2024-05-27)
+
+
+### Features
+
+* Expose the `orientation` property ([#421](https://github.com/AccessKit/accesskit/issues/421)) ([590aada](https://github.com/AccessKit/accesskit/commit/590aada070dc812f9b8f171fb9e43ac984fad2a1))
+
+
+### Dependencies
+
+* The following workspace dependencies were updated
+  * dependencies
+    * accesskit_consumer bumped from 0.21.0 to 0.22.0
+
 ## [0.19.0](https://github.com/AccessKit/accesskit/compare/accesskit_windows-v0.18.2...accesskit_windows-v0.19.0) (2024-05-26)
 
 
 ### Features
 
 * Expose the `placeholder` property ([#417](https://github.com/AccessKit/accesskit/issues/417)) ([8f4a0a1](https://github.com/AccessKit/accesskit/commit/8f4a0a1c10f83fcc8580a37d8013fec2d110865b))
```

### Comparing `accesskit-0.3.3/platforms/windows/examples/hello_world.rs` & `accesskit-0.3.4/platforms/windows/examples/hello_world.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/windows/src/adapter.rs` & `accesskit-0.3.4/platforms/windows/src/adapter.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/windows/src/context.rs` & `accesskit-0.3.4/platforms/windows/src/context.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/windows/src/node.rs` & `accesskit-0.3.4/platforms/windows/src/node.rs`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 // Copyright 2021 The Chromium Authors. All rights reserved.
 // Use of this source code is governed by a BSD-style license that can be
 // found in the LICENSE.chromium file.
 
 #![allow(non_upper_case_globals)]
 
 use accesskit::{
-    Action, ActionData, ActionRequest, Live, NodeId, NodeIdContent, Point, Role, Toggled,
+    Action, ActionData, ActionRequest, Live, NodeId, NodeIdContent, Orientation, Point, Role,
+    Toggled,
 };
 use accesskit_consumer::{FilterResult, Node, TreeState};
 use paste::paste;
 use std::sync::{atomic::Ordering, Arc, Weak};
 use windows::{
     core::*,
     Win32::{Foundation::*, System::Com::*, UI::Accessibility::*},
@@ -294,14 +295,22 @@
         }
     }
 
     fn class_name(&self) -> Option<&str> {
         self.0.class_name()
     }
 
+    fn orientation(&self) -> OrientationType {
+        match self.0.orientation() {
+            Some(Orientation::Horizontal) => OrientationType_Horizontal,
+            Some(Orientation::Vertical) => OrientationType_Vertical,
+            None => OrientationType_None,
+        }
+    }
+
     fn is_toggle_pattern_supported(&self) -> bool {
         self.0.toggled().is_some() && !self.is_selection_item_pattern_supported()
     }
 
     fn toggle_state(&self) -> ToggleState {
         match self.0.toggled().unwrap() {
             Toggled::False => ToggleState_Off,
@@ -859,15 +868,16 @@
     (HelpText, placeholder),
     (IsContentElement, is_content_element),
     (IsControlElement, is_content_element),
     (IsEnabled, is_enabled),
     (IsKeyboardFocusable, is_focusable),
     (HasKeyboardFocus, is_focused),
     (LiveSetting, live_setting),
-    (ClassName, class_name)
+    (ClassName, class_name),
+    (Orientation, orientation)
 }
 
 patterns! {
     (Toggle, is_toggle_pattern_supported, (
         (ToggleState, toggle_state, ToggleState)
     ), (
         fn Toggle(&self) -> Result<()> {
```

### Comparing `accesskit-0.3.3/platforms/windows/src/subclass.rs` & `accesskit-0.3.4/platforms/windows/src/subclass.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/windows/src/tests/mod.rs` & `accesskit-0.3.4/platforms/windows/src/tests/mod.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/windows/src/tests/simple.rs` & `accesskit-0.3.4/platforms/windows/src/tests/simple.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/windows/src/tests/subclassed.rs` & `accesskit-0.3.4/platforms/windows/src/tests/subclassed.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/windows/src/text.rs` & `accesskit-0.3.4/platforms/windows/src/text.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/windows/src/util.rs` & `accesskit-0.3.4/platforms/windows/src/util.rs`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,20 @@
 
 impl From<UIA_CONTROLTYPE_ID> for Variant {
     fn from(value: UIA_CONTROLTYPE_ID) -> Self {
         Self(value.0.into())
     }
 }
 
+impl From<OrientationType> for Variant {
+    fn from(value: OrientationType) -> Self {
+        Self(value.0.into())
+    }
+}
+
 impl From<bool> for Variant {
     fn from(value: bool) -> Self {
         Self(value.into())
     }
 }
 
 impl<T: Into<Variant>> From<Option<T>> for Variant {
```

### Comparing `accesskit-0.3.3/platforms/unix/Cargo.toml` & `accesskit-0.3.4/platforms/unix/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "accesskit_unix"
-version = "0.10.0"
+version = "0.10.1"
 authors.workspace = true
 license.workspace = true
 description = "AccessKit UI accessibility infrastructure: Linux adapter"
 categories.workspace = true
 keywords = ["gui", "ui", "accessibility"]
 repository.workspace = true
 readme = "README.md"
@@ -14,15 +14,15 @@
 [features]
 default = ["async-io"]
 async-io = ["dep:async-channel", "dep:async-executor", "dep:async-task", "dep:futures-util", "atspi/async-std", "zbus/async-io"]
 tokio = ["dep:tokio", "dep:tokio-stream", "atspi/tokio", "zbus/tokio"]
 
 [dependencies]
 accesskit = { version = "0.14.0", path = "../../common" }
-accesskit_atspi_common = { version = "0.5.0", path = "../atspi-common" }
+accesskit_atspi_common = { version = "0.6.0", path = "../atspi-common" }
 atspi = { version = "0.19", default-features = false }
 futures-lite = "1.13"
 serde = "1.0"
 zbus = { version = "3.14", default-features = false }
 
 # async-io support
 async-channel = { version = "2.1.1", optional = true }
```

### Comparing `accesskit-0.3.3/platforms/unix/CHANGELOG.md` & `accesskit-0.3.4/platforms/unix/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,18 @@
   * dependencies
     * accesskit_atspi_common bumped from 0.4.0 to 0.4.1
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit_atspi_common bumped from 0.4.1 to 0.4.2
 
+* The following workspace dependencies were updated
+  * dependencies
+    * accesskit_atspi_common bumped from 0.5.0 to 0.6.0
+
 ## [0.10.0](https://github.com/AccessKit/accesskit/compare/accesskit_unix-v0.9.2...accesskit_unix-v0.10.0) (2024-05-26)
 
 
 ### Features
 
 * Add basic text support on Unix ([#362](https://github.com/AccessKit/accesskit/issues/362)) ([52540f8](https://github.com/AccessKit/accesskit/commit/52540f82cf9fc148358351ed486bab3e7e91f1d6))
 * Expose the `placeholder` property ([#417](https://github.com/AccessKit/accesskit/issues/417)) ([8f4a0a1](https://github.com/AccessKit/accesskit/commit/8f4a0a1c10f83fcc8580a37d8013fec2d110865b))
```

### Comparing `accesskit-0.3.3/platforms/unix/src/adapter.rs` & `accesskit-0.3.4/platforms/unix/src/adapter.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/unix/src/atspi/bus.rs` & `accesskit-0.3.4/platforms/unix/src/atspi/bus.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/unix/src/atspi/interfaces/accessible.rs` & `accesskit-0.3.4/platforms/unix/src/atspi/interfaces/accessible.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/unix/src/atspi/interfaces/action.rs` & `accesskit-0.3.4/platforms/unix/src/atspi/interfaces/action.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/unix/src/atspi/interfaces/application.rs` & `accesskit-0.3.4/platforms/unix/src/atspi/interfaces/application.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/unix/src/atspi/interfaces/component.rs` & `accesskit-0.3.4/platforms/unix/src/atspi/interfaces/component.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/unix/src/atspi/interfaces/mod.rs` & `accesskit-0.3.4/platforms/unix/src/atspi/interfaces/mod.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/unix/src/atspi/interfaces/text.rs` & `accesskit-0.3.4/platforms/unix/src/atspi/interfaces/text.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/unix/src/atspi/interfaces/value.rs` & `accesskit-0.3.4/platforms/unix/src/atspi/interfaces/value.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/unix/src/atspi/object_address.rs` & `accesskit-0.3.4/platforms/unix/src/atspi/object_address.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/unix/src/atspi/object_id.rs` & `accesskit-0.3.4/platforms/unix/src/atspi/object_id.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/unix/src/context.rs` & `accesskit-0.3.4/platforms/unix/src/context.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/unix/src/executor.rs` & `accesskit-0.3.4/platforms/unix/src/executor.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/unix/src/lib.rs` & `accesskit-0.3.4/platforms/unix/src/lib.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/unix/src/util.rs` & `accesskit-0.3.4/platforms/unix/src/util.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/atspi-common/Cargo.toml` & `accesskit-0.3.4/platforms/atspi-common/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [package]
 name = "accesskit_atspi_common"
-version = "0.5.0"
+version = "0.6.0"
 authors.workspace = true
 license.workspace = true
 description = "AccessKit UI accessibility infrastructure: core AT-SPI translation layer"
 categories.workspace = true
 keywords = ["gui", "ui", "accessibility"]
 repository.workspace = true
 readme = "README.md"
 edition.workspace = true
 rust-version.workspace = true
 
 [dependencies]
 accesskit = { version = "0.14.0", path = "../../common" }
-accesskit_consumer = { version = "0.21.0", path = "../../consumer" }
+accesskit_consumer = { version = "0.22.0", path = "../../consumer" }
 atspi-common = { version = "0.3.0", default-features = false }
 serde = "1.0"
 thiserror = "1.0.39"
 zvariant = { version = "3", default-features = false }
```

### Comparing `accesskit-0.3.3/platforms/atspi-common/CHANGELOG.md` & `accesskit-0.3.4/platforms/atspi-common/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,33 @@
     * accesskit bumped from 0.12.2 to 0.12.3
     * accesskit_consumer bumped from 0.17.0 to 0.17.1
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit_consumer bumped from 0.19.0 to 0.19.1
 
+## [0.6.0](https://github.com/AccessKit/accesskit/compare/accesskit_atspi_common-v0.5.0...accesskit_atspi_common-v0.6.0) (2024-05-27)
+
+
+### Features
+
+* Expose the `orientation` property ([#421](https://github.com/AccessKit/accesskit/issues/421)) ([590aada](https://github.com/AccessKit/accesskit/commit/590aada070dc812f9b8f171fb9e43ac984fad2a1))
+
+
+### Bug Fixes
+
+* Fix a logic error in suffix calculation for text changes ([#423](https://github.com/AccessKit/accesskit/issues/423)) ([1121723](https://github.com/AccessKit/accesskit/commit/1121723983cb2fa64b5053626ec64afb851ff6c4))
+
+
+### Dependencies
+
+* The following workspace dependencies were updated
+  * dependencies
+    * accesskit_consumer bumped from 0.21.0 to 0.22.0
+
 ## [0.5.0](https://github.com/AccessKit/accesskit/compare/accesskit_atspi_common-v0.4.2...accesskit_atspi_common-v0.5.0) (2024-05-26)
 
 
 ### Features
 
 * Add basic text support on Unix ([#362](https://github.com/AccessKit/accesskit/issues/362)) ([52540f8](https://github.com/AccessKit/accesskit/commit/52540f82cf9fc148358351ed486bab3e7e91f1d6))
 * Expose the `placeholder` property ([#417](https://github.com/AccessKit/accesskit/issues/417)) ([8f4a0a1](https://github.com/AccessKit/accesskit/commit/8f4a0a1c10f83fcc8580a37d8013fec2d110865b))
```

### Comparing `accesskit-0.3.3/platforms/atspi-common/src/adapter.rs` & `accesskit-0.3.4/platforms/atspi-common/src/adapter.rs`

 * *Files 0% similar despite different names*

```diff
@@ -100,18 +100,18 @@
                     prefix_byte_count += new_char.len_utf8();
                 }
                 (None, None) => return,
                 _ => break,
             }
         }
 
-        let suffix_byte_count = old_text
+        let suffix_byte_count = old_text[prefix_byte_count..]
             .chars()
             .rev()
-            .zip(new_text.chars().rev())
+            .zip(new_text[prefix_byte_count..].chars().rev())
             .take_while(|(old_char, new_char)| old_char == new_char)
             .fold(0, |count, (c, _)| count + c.len_utf8());
 
         let old_content = &old_text[prefix_byte_count..old_text.len() - suffix_byte_count];
         if let Ok(length) = old_content.chars().count().try_into() {
             if length > 0 {
                 self.adapter.emit_object_event(
```

### Comparing `accesskit-0.3.3/platforms/atspi-common/src/callback.rs` & `accesskit-0.3.4/platforms/atspi-common/src/callback.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/atspi-common/src/context.rs` & `accesskit-0.3.4/platforms/atspi-common/src/context.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/atspi-common/src/error.rs` & `accesskit-0.3.4/platforms/atspi-common/src/error.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/atspi-common/src/events.rs` & `accesskit-0.3.4/platforms/atspi-common/src/events.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/atspi-common/src/lib.rs` & `accesskit-0.3.4/platforms/atspi-common/src/lib.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/atspi-common/src/node.rs` & `accesskit-0.3.4/platforms/atspi-common/src/node.rs`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 // Derived from Chromium's accessibility abstraction.
 // Copyright 2017 The Chromium Authors. All rights reserved.
 // Use of this source code is governed by a BSD-style license that can be
 // found in the LICENSE.chromium file.
 
 use accesskit::{
-    Action, ActionData, ActionRequest, Affine, DefaultActionVerb, Live, NodeId, Point, Rect, Role,
-    Toggled,
+    Action, ActionData, ActionRequest, Affine, DefaultActionVerb, Live, NodeId, Orientation, Point,
+    Rect, Role, Toggled,
 };
 use accesskit_consumer::{FilterResult, Node, TreeState};
 use atspi_common::{
     CoordType, Granularity, Interface, InterfaceSet, Layer, Live as AtspiLive, Role as AtspiRole,
     ScrollType, State, StateSet,
 };
 use std::{
@@ -286,14 +286,21 @@
         if state.is_text_input() && !state.is_read_only() {
             atspi_state.insert(State::Editable);
         }
         // TODO: Focus and selection.
         if state.is_focusable() {
             atspi_state.insert(State::Focusable);
         }
+        if let Some(orientation) = state.orientation() {
+            atspi_state.insert(if orientation == Orientation::Horizontal {
+                State::Horizontal
+            } else {
+                State::Vertical
+            });
+        }
         let filter_result = filter(self.0);
         if filter_result == FilterResult::Include {
             atspi_state.insert(State::Visible | State::Showing);
         }
         if atspi_role != AtspiRole::ToggleButton && state.toggled().is_some() {
             atspi_state.insert(State::Checkable);
         }
```

### Comparing `accesskit-0.3.3/platforms/atspi-common/src/rect.rs` & `accesskit-0.3.4/platforms/atspi-common/src/rect.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/atspi-common/src/simplified.rs` & `accesskit-0.3.4/platforms/atspi-common/src/simplified.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/platforms/atspi-common/src/util.rs` & `accesskit-0.3.4/platforms/atspi-common/src/util.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/bindings/python/Cargo.toml` & `accesskit-0.3.4/bindings/python/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "accesskit_python"
-version = "0.3.3"
+version = "0.3.4"
 authors.workspace = true
 license.workspace = true
 description = "Python bindings to the AccessKit library"
 readme = "README.md"
 publish = false
 edition.workspace = true
 
@@ -17,14 +17,14 @@
 extension-module = ["pyo3/extension-module"]
 
 [dependencies]
 accesskit = { version = "0.14.0", path = "../../common", features = ["pyo3"] }
 pyo3 = { version = "0.20", features = ["abi3-py38", "multiple-pymethods"] }
 
 [target.'cfg(target_os = "windows")'.dependencies]
-accesskit_windows = { version = "0.19.0", path = "../../platforms/windows" }
+accesskit_windows = { version = "0.20.0", path = "../../platforms/windows" }
 
 [target.'cfg(target_os = "macos")'.dependencies]
-accesskit_macos = { version = "0.14.0", path = "../../platforms/macos" }
+accesskit_macos = { version = "0.15.0", path = "../../platforms/macos" }
 
 [target.'cfg(any(target_os = "linux", target_os = "dragonfly", target_os = "freebsd", target_os = "openbsd", target_os = "netbsd"))'.dependencies]
-accesskit_unix = { version = "0.10.0", path = "../../platforms/unix" }
+accesskit_unix = { version = "0.10.1", path = "../../platforms/unix" }
```

### Comparing `accesskit-0.3.3/bindings/python/CHANGELOG.md` & `accesskit-0.3.4/bindings/python/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,20 @@
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit_windows bumped from 0.18.2 to 0.19.0
     * accesskit_macos bumped from 0.13.2 to 0.14.0
     * accesskit_unix bumped from 0.9.2 to 0.10.0
 
+* The following workspace dependencies were updated
+  * dependencies
+    * accesskit_windows bumped from 0.19.0 to 0.20.0
+    * accesskit_macos bumped from 0.14.0 to 0.15.0
+    * accesskit_unix bumped from 0.10.0 to 0.10.1
+
 ## [0.3.1](https://github.com/AccessKit/accesskit/compare/accesskit_python-v0.3.0...accesskit_python-v0.3.1) (2024-05-11)
 
 
 ### Bug Fixes
 
 * Fix dead code warning on Unix platforms ([#403](https://github.com/AccessKit/accesskit/issues/403)) ([09d9157](https://github.com/AccessKit/accesskit/commit/09d91577dd88743e379a1fdea34b25a94726d0fb))
```

### Comparing `accesskit-0.3.3/bindings/python/README.md` & `accesskit-0.3.4/bindings/python/README.md`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/bindings/python/examples/pygame/.gitignore` & `accesskit-0.3.4/bindings/python/examples/pygame/.gitignore`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/bindings/python/examples/pygame/hello_world.py` & `accesskit-0.3.4/bindings/python/examples/pygame/hello_world.py`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/bindings/python/src/common.rs` & `accesskit-0.3.4/bindings/python/src/common.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/bindings/python/src/geometry.rs` & `accesskit-0.3.4/bindings/python/src/geometry.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/bindings/python/src/lib.rs` & `accesskit-0.3.4/bindings/python/src/lib.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/bindings/python/src/macos.rs` & `accesskit-0.3.4/bindings/python/src/macos.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/bindings/python/src/unix.rs` & `accesskit-0.3.4/bindings/python/src/unix.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/bindings/python/src/windows.rs` & `accesskit-0.3.4/bindings/python/src/windows.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/Cargo.lock` & `accesskit-0.3.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -26,69 +26,69 @@
  "pyo3",
  "schemars",
  "serde",
 ]
 
 [[package]]
 name = "accesskit_atspi_common"
-version = "0.5.0"
+version = "0.6.0"
 dependencies = [
  "accesskit",
  "accesskit_consumer",
  "atspi-common",
  "serde",
  "thiserror",
  "zvariant",
 ]
 
 [[package]]
 name = "accesskit_c"
-version = "0.10.2"
+version = "0.10.3"
 dependencies = [
  "accesskit",
  "accesskit_macos",
  "accesskit_unix",
  "accesskit_windows",
  "paste",
 ]
 
 [[package]]
 name = "accesskit_consumer"
-version = "0.21.0"
+version = "0.22.0"
 dependencies = [
  "accesskit",
  "immutable-chunkmap",
 ]
 
 [[package]]
 name = "accesskit_macos"
-version = "0.14.0"
+version = "0.15.0"
 dependencies = [
  "accesskit",
  "accesskit_consumer",
  "objc2",
  "objc2-app-kit",
  "objc2-foundation",
  "once_cell",
 ]
 
 [[package]]
 name = "accesskit_python"
-version = "0.3.3"
+version = "0.3.4"
 dependencies = [
  "accesskit",
  "accesskit_macos",
  "accesskit_unix",
  "accesskit_windows",
  "pyo3",
 ]
 
 [[package]]
 name = "accesskit_unix"
-version = "0.10.0"
+version = "0.10.1"
 dependencies = [
  "accesskit",
  "accesskit_atspi_common",
  "async-channel 2.1.1",
  "async-executor",
  "async-task",
  "atspi",
@@ -98,29 +98,29 @@
  "tokio",
  "tokio-stream",
  "zbus",
 ]
 
 [[package]]
 name = "accesskit_windows"
-version = "0.19.0"
+version = "0.20.0"
 dependencies = [
  "accesskit",
  "accesskit_consumer",
  "once_cell",
  "paste",
  "scopeguard",
  "static_assertions",
  "windows",
  "winit",
 ]
 
 [[package]]
 name = "accesskit_winit"
-version = "0.20.3"
+version = "0.20.4"
 dependencies = [
  "accesskit",
  "accesskit_macos",
  "accesskit_unix",
  "accesskit_windows",
  "raw-window-handle 0.5.2",
  "raw-window-handle 0.6.0",
```

### Comparing `accesskit-0.3.3/pyproject.toml` & `accesskit-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/LICENSE-APACHE` & `accesskit-0.3.4/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/LICENSE-MIT` & `accesskit-0.3.4/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/LICENSE.chromium` & `accesskit-0.3.4/LICENSE.chromium`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.3/PKG-INFO` & `accesskit-0.3.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: accesskit
-Version: 0.3.3
+Version: 0.3.4
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

