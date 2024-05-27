# Comparing `tmp/swanlab-0.3.4.tar.gz` & `tmp/swanlab-0.3.5.tar.gz`

## Comparing `swanlab-0.3.4.tar` & `swanlab-0.3.5.tar`

### file list

```diff
@@ -1,854 +1,854 @@
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 swanlab-0.3.4/.eslintrc-auto-import.json
--rw-r--r--   0        0        0    28875 2020-02-02 00:00:00.000000 swanlab-0.3.4/README.md
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 swanlab-0.3.4/jsconfig.json
--rw-r--r--   0        0        0   236753 2020-02-02 00:00:00.000000 swanlab-0.3.4/package-lock.json
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 swanlab-0.3.4/package.json
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 swanlab-0.3.4/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swanlab-0.3.4/.config/copy_frontend.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 swanlab-0.3.4/.vscode/extensions.json
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 swanlab-0.3.4/.vscode/launch.json
--rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 swanlab-0.3.4/.vscode/settings.json
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 swanlab-0.3.4/.vscode/tailwind.json
--rw-r--r--   0        0        0   218889 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/.package-lock.json
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@alloc/quick-lru/package.json
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antfu/utils/package.json
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/adjust/package.json
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/adjust/node_modules/tslib/package.json
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/adjust/node_modules/tslib/modules/package.json
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/adjust/node_modules/tslib/test/validateModuleExportsMatchCommonJS/package.json
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/attr/package.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/color-util/package.json
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/component/package.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/component/node_modules/@antv/path-util/package.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/component/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/coord/package.json
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/dom-util/package.json
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/event-emitter/package.json
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/g-base/package.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/g-base/node_modules/@antv/path-util/package.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/g-base/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/g-canvas/package.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/g-canvas/node_modules/@antv/path-util/package.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/g-canvas/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/g-math/package.json
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/g-svg/package.json
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/g2/package.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/g2/node_modules/@antv/path-util/package.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/g2/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json
--rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/g2plot/package.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/matrix-util/package.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/path-util/package.json
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/scale/package.json
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/util/package.json
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@babel/parser/package.json
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@esbuild/linux-x64/package.json
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@eslint/eslintrc/package.json
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@eslint/js/package.json
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@eslint-community/eslint-utils/package.json
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@eslint-community/regexpp/package.json
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@headlessui/vue/package.json
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@humanwhocodes/config-array/package.json
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@humanwhocodes/module-importer/package.json
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@humanwhocodes/object-schema/package.json
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@intlify/core-base/package.json
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@intlify/message-compiler/package.json
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@intlify/shared/package.json
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@isaacs/cliui/package.json
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@isaacs/cliui/node_modules/ansi-regex/package.json
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@isaacs/cliui/node_modules/strip-ansi/package.json
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@jest/schemas/package.json
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@jridgewell/gen-mapping/package.json
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@jridgewell/resolve-uri/package.json
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@jridgewell/set-array/package.json
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@jridgewell/source-map/package.json
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@jridgewell/sourcemap-codec/package.json
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@jridgewell/trace-mapping/package.json
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@ljharb/resumer/package.json
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@ljharb/through/package.json
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@ljharb/through/tsconfig.json
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@nodelib/fs.scandir/package.json
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@nodelib/fs.stat/package.json
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@nodelib/fs.walk/package.json
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@pkgjs/parseargs/package.json
--rw-r--r--   0        0        0     4230 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@popperjs/core/package.json
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@rollup/pluginutils/package.json
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@rollup/pluginutils/dist/es/package.json
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@rollup/rollup-linux-x64-gnu/package.json
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@rollup/rollup-linux-x64-musl/package.json
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@sinclair/typebox/package.json
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@tanstack/virtual-core/package.json
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@tanstack/vue-virtual/package.json
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@types/d3-timer/package.json
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@types/estree/package.json
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@ungap/structured-clone/package.json
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@ungap/structured-clone/cjs/package.json
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vitejs/plugin-vue/package.json
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vitest/expect/package.json
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vitest/runner/package.json
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vitest/runner/node_modules/p-limit/package.json
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vitest/runner/node_modules/yocto-queue/package.json
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vitest/snapshot/package.json
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vitest/spy/package.json
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vitest/utils/package.json
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vitest/utils/node_modules/estree-walker/package.json
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vue/compiler-core/package.json
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vue/compiler-dom/package.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vue/compiler-sfc/package.json
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vue/compiler-ssr/package.json
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vue/devtools-api/package.json
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vue/reactivity/package.json
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vue/runtime-core/package.json
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vue/runtime-dom/package.json
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vue/server-renderer/package.json
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vue/shared/package.json
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/acorn/package.json
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/acorn-jsx/package.json
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/acorn-walk/package.json
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/ajv/package.json
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/ajv/lib/refs/data.json
--rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/ajv/lib/refs/json-schema-draft-04.json
--rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/ajv/lib/refs/json-schema-draft-06.json
--rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/ajv/lib/refs/json-schema-draft-07.json
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/ajv/lib/refs/json-schema-secure.json
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/align-text/package.json
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/amdefine/package.json
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/ansi-regex/package.json
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/ansi-styles/package.json
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/any-promise/package.json
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/anymatch/package.json
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/arg/package.json
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/argparse/package.json
--rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/array-buffer-byte-length/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/array-buffer-byte-length/tsconfig.json
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/arraybuffer.prototype.slice/package.json
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/assertion-error/package.json
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/asynckit/package.json
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/autoprefixer/package.json
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/available-typed-arrays/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/available-typed-arrays/tsconfig.json
--rw-r--r--   0        0        0     7671 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/axios/package.json
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/balanced-match/package.json
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/base64-arraybuffer/package.json
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/binary-extensions/binary-extensions.json
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/binary-extensions/package.json
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/boolbase/package.json
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/brace-expansion/package.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/braces/package.json
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/browserslist/package.json
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/buffer-from/package.json
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/cac/package.json
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/call-bind/package.json
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/callsites/package.json
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/camelcase/package.json
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/camelcase-css/package.json
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/caniuse-lite/package.json
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/center-align/package.json
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/chai/bower.json
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/chai/package.json
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/chalk/package.json
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/check-error/package.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/chokidar/package.json
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/chokidar/node_modules/glob-parent/package.json
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/cliui/package.json
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/color-convert/package.json
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/color-name/package.json
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/combined-stream/package.json
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/commander/package-support.json
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/commander/package.json
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/concat-map/package.json
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/confbox/package.json
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/contour_plot/package.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/cross-spawn/package.json
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/css-line-break/package.json
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/cssesc/package.json
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/csstype/package.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/d3-color/package.json
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/d3-ease/package.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/d3-hierarchy/package.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/d3-interpolate/package.json
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/d3-regression/package.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/d3-timer/package.json
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/data-view-buffer/package.json
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/data-view-buffer/tsconfig.json
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/data-view-byte-length/package.json
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/data-view-byte-length/tsconfig.json
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/data-view-byte-offset/package.json
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/data-view-byte-offset/tsconfig.json
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/debug/package.json
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/decamelize/package.json
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/deep-eql/package.json
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/deep-equal/package.json
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/deep-is/package.json
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/define-data-property/package.json
--rw-r--r--   0        0        0     4883 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/define-data-property/tsconfig.json
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/define-properties/package.json
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/defined/package.json
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/delayed-stream/package.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/detect-browser/package.json
--rwxr-xr-x   0        0        0      647 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/didyoumean/package.json
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/diff-sequences/package.json
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/dlv/package.json
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/doctrine/package.json
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/dotignore/package.json
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eastasianwidth/package.json
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/electron-to-chromium/chromium-versions.json
--rw-r--r--   0        0        0    50514 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/electron-to-chromium/full-chromium-versions.json
--rw-r--r--   0        0        0    78988 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/electron-to-chromium/full-versions.json
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/electron-to-chromium/package.json
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/electron-to-chromium/versions.json
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/emoji-regex/package.json
--rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/entities/package.json
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/entities/lib/esm/package.json
--rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/es-abstract/package.json
--rw-r--r--   0        0        0    22346 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/es-abstract/helpers/caseFolding.json
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/es-abstract/node_modules/object-inspect/package-support.json
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/es-abstract/node_modules/object-inspect/package.json
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/es-define-property/package.json
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/es-define-property/tsconfig.json
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/es-errors/package.json
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/es-errors/tsconfig.json
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/es-object-atoms/package.json
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/es-object-atoms/tsconfig.json
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/es-set-tostringtag/package.json
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/es-set-tostringtag/tsconfig.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/es-to-primitive/package.json
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/esbuild/package.json
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/escalade/package.json
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/escape-string-regexp/package.json
--rw-r--r--   0        0        0     5566 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint/package.json
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint/conf/replacements.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint/conf/rule-type-list.json
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint/lib/cli-engine/formatters/formatters-meta.json
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-config-prettier/package.json
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-plugin-prettier/package.json
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-plugin-vue/package.json
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/deprecated-html-elements.json
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/html-elements.json
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/inline-non-void-elements.json
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/js-reserved.json
--rw-r--r--   0        0        0     5270 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/key-aliases.json
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/math-elements.json
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/svg-attributes-weird-case.json
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/svg-elements.json
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/void-elements.json
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/vue-component-options.json
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/vue-reserved.json
--rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/vue3-export-names.json
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-scope/package.json
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-visitor-keys/package.json
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/espree/package.json
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/esquery/package.json
--rwxr-xr-x   0        0        0     1165 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/esrecurse/package.json
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/estraverse/package.json
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/estree-walker/package.json
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/estree-walker/dist/esm/package.json
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/estree-walker/src/package.json
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/esutils/package.json
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/execa/package.json
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/fast-deep-equal/package.json
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/fast-diff/package.json
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/fast-glob/package.json
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/fast-glob/node_modules/glob-parent/package.json
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/fast-json-stable-stringify/package.json
--rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/fast-json-stable-stringify/benchmark/test.json
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/fast-levenshtein/package.json
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/fastq/package.json
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/fastq/test/tsconfig.json
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/fecha/package.json
--rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/file-entry-cache/package.json
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/fill-range/package.json
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/find-up/package.json
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/flat-cache/package.json
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/flatted/package.json
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/flatted/cjs/package.json
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/fmin/.eslintrc.json
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/fmin/package.json
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/follow-redirects/package.json
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/for-each/package.json
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/foreground-child/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/foreground-child/dist/cjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/foreground-child/dist/mjs/package.json
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/form-data/package.json
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/fraction.js/package.json
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/fs.realpath/package.json
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/function-bind/package.json
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/function.prototype.name/package.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/functions-have-names/package.json
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/get-func-name/package.json
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/get-intrinsic/package.json
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/get-stream/package.json
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/get-symbol-description/package.json
--rwxr-xr-x   0        0        0      630 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/gl-matrix/package.json
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/gl-matrix/mat2/package.json
--rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/gl-matrix/mat2d/package.json
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/gl-matrix/mat3/package.json
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/gl-matrix/mat4/package.json
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/gl-matrix/quat/package.json
--rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/gl-matrix/quat2/package.json
--rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/gl-matrix/types.d.ts/package.json
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/gl-matrix/vec2/package.json
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/gl-matrix/vec3/package.json
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/gl-matrix/vec4/package.json
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/glob/package.json
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/glob-parent/package.json
--rw-r--r--   0        0        0    48140 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/globals/globals.json
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/globals/package.json
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/globalthis/package.json
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/gopd/package.json
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/graphemer/package.json
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/has/package.json
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/has-ansi/package.json
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/has-ansi/node_modules/ansi-regex/package.json
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/has-bigints/package.json
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/has-flag/package.json
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/has-property-descriptors/package.json
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/has-proto/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/has-proto/tsconfig.json
--rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/has-symbols/package.json
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/has-tostringtag/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/has-tostringtag/tsconfig.json
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/hasown/package.json
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/hasown/tsconfig.json
--rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/html2canvas/package.json
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/html2canvas/tsconfig.json
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/human-signals/package.json
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/husky/package.json
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/ignore/package.json
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/immutable/package.json
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/import-fresh/package.json
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/imurmurhash/package.json
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/inflight/package.json
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/inherits/package.json
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/internal-slot/package.json
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-arguments/package.json
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-array-buffer/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-array-buffer/tsconfig.json
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-bigint/package.json
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-binary-path/package.json
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-boolean-object/package.json
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-buffer/package.json
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-callable/package.json
--rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-core-module/core.json
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-core-module/package.json
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-data-view/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-data-view/tsconfig.json
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-date-object/package.json
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-extglob/package.json
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-fullwidth-code-point/package.json
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-glob/package.json
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-negative-zero/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-negative-zero/tsconfig.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-number/package.json
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-number-object/package.json
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-path-inside/package.json
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-regex/package.json
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-shared-array-buffer/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-shared-array-buffer/tsconfig.json
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-stream/package.json
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-string/package.json
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-symbol/package.json
--rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-typed-array/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-typed-array/tsconfig.json
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-weakref/package.json
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/isarray/package.json
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/isexe/package.json
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/jackspeak/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/jackspeak/dist/commonjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/jackspeak/dist/esm/package.json
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/jiti/package.json
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/js-tokens/package.json
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/js-yaml/package.json
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/json-buffer/package.json
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/json-schema-traverse/package.json
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/json-stable-stringify-without-jsonify/package.json
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/json2module/package.json
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/json5/package.json
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/keyv/package.json
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/kind-of/package.json
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/lazy-cache/package.json
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/levn/package.json
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/lilconfig/package.json
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/lines-and-columns/package.json
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/local-pkg/package.json
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/locate-path/package.json
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/lodash/package.json
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/lodash-es/package.json
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/lodash.merge/package.json
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/longest/package.json
--rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/loupe/package.json
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/lru-cache/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/lru-cache/dist/commonjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/lru-cache/dist/esm/package.json
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/magic-string/package.json
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/merge-stream/package.json
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/merge2/package.json
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/micromatch/package.json
--rw-r--r--   0        0        0   185882 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/mime-db/db.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/mime-db/package.json
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/mime-types/package.json
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/mimic-fn/package.json
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/minimatch/package.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/minimist/package.json
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/minipass/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/minipass/dist/commonjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/minipass/dist/esm/package.json
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/mlly/package.json
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/mock-property/package.json
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/mockjs/bower.json
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/mockjs/package.json
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/mockjs/test/bower.json
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/mockjs/test/package.json
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/moment/package.json
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/ms/package.json
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/mz/package.json
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/nanoid/package.json
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/nanoid/async/package.json
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/nanoid/non-secure/package.json
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/nanoid/url-alphabet/package.json
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/natural-compare/package.json
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/node-releases/package.json
--rw-r--r--   0        0        0    29857 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/node-releases/data/processed/envs.json
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/node-releases/data/release-schedule/release-schedule.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/normalize-path/package.json
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/normalize-range/package.json
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/npm-run-path/package.json
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/npm-run-path/node_modules/path-key/package.json
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/nth-check/package.json
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/nth-check/lib/esm/package.json
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/object-assign/package.json
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/object-hash/package.json
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/object-inspect/package-support.json
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/object-inspect/package.json
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/object-is/package.json
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/object-keys/package.json
--rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/object.assign/package.json
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/once/package.json
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/onetime/package.json
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/optionator/package.json
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/p-limit/package.json
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/p-locate/package.json
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/parent-module/package.json
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/path-exists/package.json
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/path-is-absolute/package.json
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/path-key/package.json
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/path-parse/package.json
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/path-scurry/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/path-scurry/dist/commonjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/path-scurry/dist/esm/package.json
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/pathe/package.json
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/pathval/package.json
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/pdfast/package.json
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/picocolors/package.json
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/picomatch/package.json
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/pify/package.json
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/pinia/package.json
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/pinia/node_modules/vue-demi/package.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/pirates/package.json
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/pkg-types/package.json
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/possible-typed-array-names/package.json
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/possible-typed-array-names/tsconfig.json
--rwxr-xr-x   0        0        0     2496 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/postcss/package.json
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/postcss-import/package.json
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/postcss-js/package.json
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/postcss-load-config/package.json
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/postcss-load-config/node_modules/lilconfig/package.json
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/postcss-nested/package.json
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/postcss-selector-parser/package.json
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/postcss-value-parser/package.json
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/prelude-ls/package.json
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/prettier/package.json
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/prettier-linter-helpers/package.json
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/prettier-linter-helpers/.vscode/settings.json
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/pretty-format/package.json
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/pretty-format/node_modules/ansi-styles/package.json
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/proxy-from-env/package.json
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/punycode/package.json
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/queue-microtask/package.json
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/react-is/package.json
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/read-cache/package.json
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/readdirp/package.json
--rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/regexp.prototype.flags/package.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/repeat-string/package.json
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve/package.json
--rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve/lib/core.json
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve/test/module_dir/zmodules/bbb/package.json
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve/test/resolver/baz/package.json
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve/test/resolver/browser_field/package.json
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve/test/resolver/dot_main/package.json
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve/test/resolver/dot_slash_main/package.json
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve/test/resolver/false_main/package.json
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve/test/resolver/incorrect_main/package.json
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve/test/resolver/invalid_main/package.json
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve/test/resolver/multirepo/lerna.json
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve/test/resolver/multirepo/package.json
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve/test/resolver/multirepo/packages/package-a/package.json
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve/test/resolver/multirepo/packages/package-b/package.json
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve/test/resolver/nested_symlinks/mylib/package.json
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve/test/resolver/symlinked/package/package.json
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve-from/package.json
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/reusify/package.json
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/right-align/package.json
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/rimraf/package.json
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/rollup/package.json
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/rollup/node_modules/ansi-regex/package.json
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/rollup/node_modules/ansi-styles/package.json
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/rollup/node_modules/chalk/package.json
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/rollup/node_modules/escape-string-regexp/package.json
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/rollup/node_modules/strip-ansi/package.json
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/rollup/node_modules/supports-color/package.json
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/run-parallel/package.json
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/rw/package.json
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/safe-array-concat/package.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/safe-array-concat/tsconfig.json
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/safe-regex-test/package.json
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/sass/package.json
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/scule/package.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/semver/package.json
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/set-function-length/package.json
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/set-function-length/tsconfig.json
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/set-function-name/package.json
--rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/set-function-name/tsconfig.json
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/shebang-command/package.json
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/shebang-regex/package.json
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/side-channel/package.json
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/side-channel/tsconfig.json
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/side-channel/node_modules/object-inspect/package-support.json
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/side-channel/node_modules/object-inspect/package.json
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/siginfo/package.json
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/signal-exit/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/signal-exit/dist/cjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/signal-exit/dist/mjs/package.json
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/size-sensor/package.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/source-map/package.json
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/source-map-js/package.json
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/source-map-support/package.json
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/stackback/package.json
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/std-env/package.json
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/string-width/package.json
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/string-width/node_modules/ansi-regex/package.json
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/string-width/node_modules/strip-ansi/package.json
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/string-width-cjs/package.json
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/string-width-cjs/node_modules/emoji-regex/package.json
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/string.prototype.trim/package.json
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/string.prototype.trimend/package.json
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/string.prototype.trimstart/package.json
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/strip-ansi/package.json
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/strip-ansi-cjs/package.json
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/strip-final-newline/package.json
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/strip-json-comments/package.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/strip-literal/package.json
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/sucrase/package.json
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/sucrase/node_modules/brace-expansion/package.json
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/sucrase/node_modules/commander/package.json
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/sucrase/node_modules/glob/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/sucrase/node_modules/glob/dist/commonjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/sucrase/node_modules/glob/dist/esm/package.json
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/sucrase/node_modules/minimatch/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/sucrase/node_modules/minimatch/dist/commonjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/sucrase/node_modules/minimatch/dist/esm/package.json
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/supports-color/package.json
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/supports-preserve-symlinks-flag/package.json
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/tailwindcss/package.json
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/tailwindcss/stubs/.prettierrc.json
--rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/tape/package.json
--rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/terser/package.json
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/terser/bin/package.json
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/terser/dist/package.json
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/terser/node_modules/commander/package.json
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/terser/node_modules/source-map/package.json
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/terser/node_modules/source-map-support/package.json
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/text-segmentation/package.json
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/text-table/package.json
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/thenify/package.json
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/thenify-all/package.json
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/tinybench/package.json
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/tinypool/package.json
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/tinyspy/package.json
--rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/tippy.js/package.json
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/tippy.js/headless/package.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/to-regex-range/package.json
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/ts-interface-checker/package.json
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/tslib/package.json
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/tslib/modules/package.json
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/type-check/package.json
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/type-detect/package.json
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/type-fest/package.json
--rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/typed-array-buffer/package.json
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/typed-array-buffer/tsconfig.json
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/typed-array-byte-length/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/typed-array-byte-length/tsconfig.json
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/typed-array-byte-offset/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/typed-array-byte-offset/tsconfig.json
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/typed-array-length/package.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/typed-array-length/tsconfig.json
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/ufo/package.json
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/uglify-js/package.json
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/uglify-js/node_modules/source-map/package.json
--rw-r--r--   0        0        0   142838 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/uglify-js/tools/domprops.json
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/uglify-to-browserify/package.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/unbox-primitive/package.json
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/unimport/package.json
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/unimport/node_modules/escape-string-regexp/package.json
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/unimport/node_modules/estree-walker/package.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/unimport/node_modules/local-pkg/package.json
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/unplugin/package.json
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/unplugin-auto-import/package.json
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/unplugin-auto-import/node_modules/brace-expansion/package.json
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/unplugin-auto-import/node_modules/minimatch/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/unplugin-auto-import/node_modules/minimatch/dist/commonjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/unplugin-auto-import/node_modules/minimatch/dist/esm/package.json
--rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/unplugin-vue-components/package.json
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/unplugin-vue-components/node_modules/brace-expansion/package.json
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/unplugin-vue-components/node_modules/minimatch/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/unplugin-vue-components/node_modules/minimatch/dist/cjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/unplugin-vue-components/node_modules/minimatch/dist/mjs/package.json
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/update-browserslist-db/.devcontainer.json
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/update-browserslist-db/package.json
--rwxr-xr-x   0        0        0     2172 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/uri-js/package.json
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/util-deprecate/package.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/utrie/package.json
--rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vite/package.json
--rw-r--r--   0        0        0    10895 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vite/node_modules/rollup/package.json
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vite/node_modules/rollup/dist/es/package.json
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vite/types/package.json
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vite-node/package.json
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vite-plugin-json5/package.json
--rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vitest/package.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vitest/node_modules/local-pkg/package.json
--rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vue/package.json
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vue/compiler-sfc/package.json
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vue/jsx-runtime/package.json
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vue/server-renderer/package.json
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vue-eslint-parser/package.json
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vue-i18n/package.json
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vue-i18n/vetur/attributes.json
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vue-i18n/vetur/tags.json
--rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vue-router/package.json
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vue-router/vetur/attributes.json
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vue-router/vetur/tags.json
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vue-tippy/package.json
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vue-tippy/tsconfig.json
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vue-tippy/vetur/attributes.json
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vue-tippy/vetur/tags.json
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/webpack-sources/package.json
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/webpack-virtual-modules/package.json
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/which/package.json
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/which-boxed-primitive/package.json
--rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/which-typed-array/package.json
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/which-typed-array/tsconfig.json
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/why-is-node-running/package.json
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/window-size/package.json
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/word-wrap/package.json
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/wordwrap/package.json
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/wrap-ansi/package.json
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/wrap-ansi/node_modules/ansi-regex/package.json
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/wrap-ansi/node_modules/ansi-styles/package.json
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/wrap-ansi/node_modules/strip-ansi/package.json
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/wrap-ansi-cjs/package.json
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/wrap-ansi-cjs/node_modules/emoji-regex/package.json
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/wrap-ansi-cjs/node_modules/string-width/package.json
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/wrappy/package.json
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/xml-name-validator/package.json
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/yaml/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/yaml/browser/package.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/yargs/package.json
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/yocto-queue/package.json
--rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/__init__.py
--rw-r--r--   0        0        0     9852 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/env.py
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/error.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/package.json
--rw-r--r--   0        0        0     5471 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/package.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/api/__init__.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/api/cos.py
--rw-r--r--   0        0        0     8817 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/api/http.py
--rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/api/info.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/api/auth/__init__.py
--rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/api/auth/login.py
--rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/api/upload/__init__.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/api/upload/model.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/cli/__init__.py
--rw-r--r--   0        0        0     7349 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/cli/main.py
--rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/cli/utils.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/cloud/__init__.py
--rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/cloud/_log_collector.py
--rw-r--r--   0        0        0     5508 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/cloud/start_thread.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/cloud/task_types.py
--rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/cloud/utils.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/cloud/dog/README.md
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/cloud/dog/__init__.py
--rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/cloud/dog/log_sniffer.py
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/cloud/dog/metadata_handle.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/cloud/dog/sniffer_queue.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/compat/README.md
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/compat/server/controller/experiment.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/converter/__init__.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/converter/tfb/__init__.py
--rw-r--r--   0        0        0     4493 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/converter/tfb/_utils.py
--rw-r--r--   0        0        0     4170 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/converter/tfb/tfb_converter.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/converter/wb/__init__.py
--rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/converter/wb/wb_converter.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/__init__.py
--rw-r--r--   0        0        0     7085 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/callback_cloud.py
--rw-r--r--   0        0        0     5983 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/callback_local.py
--rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/config.py
--rw-r--r--   0        0        0    13030 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/sdk.py
--rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/settings.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/modules/__init__.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/modules/_utils.py
--rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/modules/audio.py
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/modules/base.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/modules/chart.py
--rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/modules/image.py
--rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/modules/object_3d.py
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/modules/text.py
--rw-r--r--   0        0        0     7738 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/modules/video.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/modules/utils_modules/__init__.py
--rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/modules/utils_modules/bounding_boxes.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/modules/utils_modules/image_mask.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/run/__init__.py
--rw-r--r--   0        0        0     8506 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/run/callback.py
--rw-r--r--   0        0        0    16930 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/run/exp.py
--rw-r--r--   0        0        0    13553 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/run/main.py
--rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/run/operator.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/system/__init__.py
--rw-r--r--   0        0        0     8065 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/system/info.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/system/monitor.py
--rwxr-xr-x   0        0        0   337072 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/system/bin/apple_gpu_stats
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/__init__.py
--rw-r--r--   0        0        0     8012 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/callback.py
--rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/db_connect.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/error.py
--rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/model.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/table_config.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/docs/Errors.md
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/docs/README.md
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/migrate/__init__.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/migrate/chart.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/migrate/experiment.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/migrate/namespace.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/migrate/project.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/migrate/tag.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/models/__init__.py
--rw-r--r--   0        0        0     9068 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/models/charts.py
--rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/models/displays.py
--rw-r--r--   0        0        0     6632 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/models/experiments.py
--rw-r--r--   0        0        0     6326 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/models/namespaces.py
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/models/projects.py
--rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/models/sources.py
--rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/models/tags.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/utils/__init__.py
--rw-r--r--   0        0        0     9078 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/utils/chart.py
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/integration/fastai.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/integration/huggingface.py
--rw-r--r--   0        0        0     7392 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/integration/mmengine.py
--rw-r--r--   0        0        0     7301 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/integration/pytorch_lightning.py
--rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/integration/sb3.py
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/integration/ultralytics.py
--rw-r--r--   0        0        0     8539 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/integration/integration_utils/autologging.py
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/integration/integration_utils/get_modules.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/integration/integration_utils/timer.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/integration/openai/__init__.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/integration/openai/openai.py
--rw-r--r--   0        0        0    19701 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/integration/openai/resolver.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/integration/zhipuai/__init__.py
--rw-r--r--   0        0        0     7125 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/integration/zhipuai/resolver.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/integration/zhipuai/zhipuai.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/log/__init__.py
--rw-r--r--   0        0        0     5581 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/log/console.py
--rw-r--r--   0        0        0     9090 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/log/log.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/__init__.py
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/app.py
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/settings.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/controller/chart.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/controller/db.py
--rw-r--r--   0        0        0    16723 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/controller/experiment.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/controller/namespace.py
--rw-r--r--   0        0        0     8076 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/controller/project.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/controller/utils/__init__.py
--rw-r--r--   0        0        0     6976 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/controller/utils/charts.py
--rw-r--r--   0        0        0     5042 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/controller/utils/tag.py
--rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/middleware/common.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/module/__init__.py
--rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/module/resp.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/router/chart.py
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/router/experiment.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/router/media.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/router/namespace.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/router/project.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/index.html
--rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/ChartPage-C2Rj7xI3.js
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/ChartPage-DgOOkrVh.css
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/ChartsView-DpI6U3QH.js
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/EnvHardware-4H7mp2Bs.js
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/EnvIndex-B5_l1b65.js
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/EnvItems-B4PwmQT4.js
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/EnvItems-BfjcRO-X.css
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/EnvRequirements-BqyzUHLZ.css
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/EnvRequirements-Cpn2Fk1D.js
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/EnvironmentPage-Bb8ousXq.js
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/EnvironmentPage-C6uSuWBq.css
--rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/ExperimentView-BTbu21ka.js
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/ExperimentView-CCDMXo4h.css
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/FuncBar-Ct_nBdvU.js
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/FuncBar-DgVTuZfd.css
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/HelpView-C4wSXY1I.js
--rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/HomeView-BS7FyMAt.css
--rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/HomeView-BqTu9_fG.js
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/IndexPage-C5dvtib2.css
--rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/IndexPage-CrqN4Ekl.js
--rw-r--r--   0        0        0   273900 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/JetBrainsMono-Regular-Dh36KTnx.ttf
--rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/LogPage-B-fC6sB7.js
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/LogPage-DBzoauOW.css
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/NotFound-DijsQ96i.js
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/SLLoading-6DfF2aH0.js
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/SLStatusLabel-BRacn5XK.css
--rw-r--r--   0        0        0     5489 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/SLStatusLabel-DvEKZN8v.js
--rw-r--r--   0        0        0   119080 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/SourceSansPro-Regular-J3NOkSfZ.ttf
--rw-r--r--   0        0        0    12117 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/chart-DB312WPs.css
--rw-r--r--   0        0        0  1098521 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/chart-eW1meEc1.js
--rw-r--r--   0        0        0   393892 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/index-B5SDzoY4.js
--rw-r--r--   0        0        0    37013 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/index-B7Izi8NT.css
--rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/logo-ChHf2ozk.ico
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/utils/__init__.py
--rw-r--r--   0        0        0     7816 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/utils/file.py
--rw-r--r--   0        0        0     8727 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/utils/font.py
--rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/utils/judgment.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/utils/key.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/utils/time.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/create_error_chart.py
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/create_experiment.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/start_server.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/use_swanlog.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/config/config.json
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/config/load.yaml
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/integration/.gitignore
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/integration/README.md
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/integration/fastai/fastai_train.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/integration/fastai/requirements.txt
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/integration/huggingface/requirements.txt
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/integration/huggingface/transformers_bert_train.py
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/integration/lightning/lightning_base.py
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/integration/lightning/lightning_train.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/integration/lightning/requirements.txt
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/integration/sb3/requirements.txt
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/integration/sb3/sb3_PPO.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/integration/ultralytics/requirements.txt
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/integration/ultralytics/ultralytics_classifer.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/integration/ultralytics/ultralytics_detection.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/integration/ultralytics/ultralytics_pose.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/integration/ultralytics/ultralytics_segmentation.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/unit/conftest.py
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/unit/pytest_env.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/unit/pytest_example.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/unit/auth/pytest_login.py
--rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/unit/data/pytest_sdk.py
--rw-r--r--   0        0        0    20154 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/unit/data/run/pytest_main.py
--rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/unit/log/pytest_log.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/unit/server/controller/utils/utils.py
--rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/unit/utils/pytest_file.py
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/unit/utils/pytest_key.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/unit/utils/pytest_package.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 swanlab-0.3.4/.gitignore
--rw-r--r--   0        0        0    10779 2020-02-02 00:00:00.000000 swanlab-0.3.4/LICENSE
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 swanlab-0.3.4/pyproject.toml
--rw-r--r--   0        0        0    31012 2020-02-02 00:00:00.000000 swanlab-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 swanlab-0.3.5/.eslintrc-auto-import.json
+-rw-r--r--   0        0        0    28874 2020-02-02 00:00:00.000000 swanlab-0.3.5/README.md
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 swanlab-0.3.5/jsconfig.json
+-rw-r--r--   0        0        0   236753 2020-02-02 00:00:00.000000 swanlab-0.3.5/package-lock.json
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 swanlab-0.3.5/package.json
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 swanlab-0.3.5/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swanlab-0.3.5/.config/copy_frontend.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 swanlab-0.3.5/.vscode/extensions.json
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 swanlab-0.3.5/.vscode/launch.json
+-rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 swanlab-0.3.5/.vscode/settings.json
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 swanlab-0.3.5/.vscode/tailwind.json
+-rw-r--r--   0        0        0   218889 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/.package-lock.json
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@alloc/quick-lru/package.json
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@antfu/utils/package.json
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@antv/adjust/package.json
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@antv/adjust/node_modules/tslib/package.json
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@antv/adjust/node_modules/tslib/modules/package.json
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@antv/adjust/node_modules/tslib/test/validateModuleExportsMatchCommonJS/package.json
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@antv/attr/package.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@antv/color-util/package.json
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@antv/component/package.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@antv/component/node_modules/@antv/path-util/package.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@antv/component/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@antv/coord/package.json
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@antv/dom-util/package.json
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@antv/event-emitter/package.json
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@antv/g-base/package.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@antv/g-base/node_modules/@antv/path-util/package.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@antv/g-base/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@antv/g-canvas/package.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@antv/g-canvas/node_modules/@antv/path-util/package.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@antv/g-canvas/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@antv/g-math/package.json
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@antv/g-svg/package.json
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@antv/g2/package.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@antv/g2/node_modules/@antv/path-util/package.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@antv/g2/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json
+-rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@antv/g2plot/package.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@antv/matrix-util/package.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@antv/path-util/package.json
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@antv/scale/package.json
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@antv/util/package.json
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@babel/parser/package.json
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@esbuild/linux-x64/package.json
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@eslint/eslintrc/package.json
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@eslint/js/package.json
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@eslint-community/eslint-utils/package.json
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@eslint-community/regexpp/package.json
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@headlessui/vue/package.json
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@humanwhocodes/config-array/package.json
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@humanwhocodes/module-importer/package.json
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@humanwhocodes/object-schema/package.json
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@intlify/core-base/package.json
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@intlify/message-compiler/package.json
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@intlify/shared/package.json
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@isaacs/cliui/package.json
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@isaacs/cliui/node_modules/ansi-regex/package.json
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@isaacs/cliui/node_modules/strip-ansi/package.json
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@jest/schemas/package.json
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@jridgewell/gen-mapping/package.json
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@jridgewell/resolve-uri/package.json
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@jridgewell/set-array/package.json
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@jridgewell/source-map/package.json
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@jridgewell/sourcemap-codec/package.json
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@jridgewell/trace-mapping/package.json
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@ljharb/resumer/package.json
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@ljharb/through/package.json
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@ljharb/through/tsconfig.json
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@nodelib/fs.scandir/package.json
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@nodelib/fs.stat/package.json
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@nodelib/fs.walk/package.json
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@pkgjs/parseargs/package.json
+-rw-r--r--   0        0        0     4230 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@popperjs/core/package.json
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@rollup/pluginutils/package.json
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@rollup/pluginutils/dist/es/package.json
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@rollup/rollup-linux-x64-gnu/package.json
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@rollup/rollup-linux-x64-musl/package.json
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@sinclair/typebox/package.json
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@tanstack/virtual-core/package.json
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@tanstack/vue-virtual/package.json
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@types/d3-timer/package.json
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@types/estree/package.json
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@ungap/structured-clone/package.json
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@ungap/structured-clone/cjs/package.json
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@vitejs/plugin-vue/package.json
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@vitest/expect/package.json
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@vitest/runner/package.json
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@vitest/runner/node_modules/p-limit/package.json
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@vitest/runner/node_modules/yocto-queue/package.json
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@vitest/snapshot/package.json
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@vitest/spy/package.json
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@vitest/utils/package.json
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@vitest/utils/node_modules/estree-walker/package.json
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@vue/compiler-core/package.json
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@vue/compiler-dom/package.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@vue/compiler-sfc/package.json
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@vue/compiler-ssr/package.json
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@vue/devtools-api/package.json
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@vue/reactivity/package.json
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@vue/runtime-core/package.json
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@vue/runtime-dom/package.json
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@vue/server-renderer/package.json
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/@vue/shared/package.json
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/acorn/package.json
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/acorn-jsx/package.json
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/acorn-walk/package.json
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/ajv/package.json
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/ajv/lib/refs/data.json
+-rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/ajv/lib/refs/json-schema-draft-04.json
+-rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/ajv/lib/refs/json-schema-draft-06.json
+-rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/ajv/lib/refs/json-schema-draft-07.json
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/ajv/lib/refs/json-schema-secure.json
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/align-text/package.json
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/amdefine/package.json
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/ansi-regex/package.json
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/ansi-styles/package.json
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/any-promise/package.json
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/anymatch/package.json
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/arg/package.json
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/argparse/package.json
+-rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/array-buffer-byte-length/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/array-buffer-byte-length/tsconfig.json
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/arraybuffer.prototype.slice/package.json
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/assertion-error/package.json
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/asynckit/package.json
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/autoprefixer/package.json
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/available-typed-arrays/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/available-typed-arrays/tsconfig.json
+-rw-r--r--   0        0        0     7671 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/axios/package.json
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/balanced-match/package.json
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/base64-arraybuffer/package.json
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/binary-extensions/binary-extensions.json
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/binary-extensions/package.json
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/boolbase/package.json
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/brace-expansion/package.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/braces/package.json
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/browserslist/package.json
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/buffer-from/package.json
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/cac/package.json
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/call-bind/package.json
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/callsites/package.json
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/camelcase/package.json
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/camelcase-css/package.json
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/caniuse-lite/package.json
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/center-align/package.json
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/chai/bower.json
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/chai/package.json
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/chalk/package.json
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/check-error/package.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/chokidar/package.json
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/chokidar/node_modules/glob-parent/package.json
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/cliui/package.json
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/color-convert/package.json
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/color-name/package.json
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/combined-stream/package.json
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/commander/package-support.json
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/commander/package.json
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/concat-map/package.json
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/confbox/package.json
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/contour_plot/package.json
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/cross-spawn/package.json
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/css-line-break/package.json
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/cssesc/package.json
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/csstype/package.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/d3-color/package.json
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/d3-ease/package.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/d3-hierarchy/package.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/d3-interpolate/package.json
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/d3-regression/package.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/d3-timer/package.json
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/data-view-buffer/package.json
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/data-view-buffer/tsconfig.json
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/data-view-byte-length/package.json
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/data-view-byte-length/tsconfig.json
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/data-view-byte-offset/package.json
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/data-view-byte-offset/tsconfig.json
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/debug/package.json
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/decamelize/package.json
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/deep-eql/package.json
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/deep-equal/package.json
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/deep-is/package.json
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/define-data-property/package.json
+-rw-r--r--   0        0        0     4883 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/define-data-property/tsconfig.json
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/define-properties/package.json
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/defined/package.json
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/delayed-stream/package.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/detect-browser/package.json
+-rwxr-xr-x   0        0        0      647 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/didyoumean/package.json
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/diff-sequences/package.json
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/dlv/package.json
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/doctrine/package.json
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/dotignore/package.json
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/eastasianwidth/package.json
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/electron-to-chromium/chromium-versions.json
+-rw-r--r--   0        0        0    50514 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/electron-to-chromium/full-chromium-versions.json
+-rw-r--r--   0        0        0    78988 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/electron-to-chromium/full-versions.json
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/electron-to-chromium/package.json
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/electron-to-chromium/versions.json
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/emoji-regex/package.json
+-rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/entities/package.json
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/entities/lib/esm/package.json
+-rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/es-abstract/package.json
+-rw-r--r--   0        0        0    22346 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/es-abstract/helpers/caseFolding.json
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/es-abstract/node_modules/object-inspect/package-support.json
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/es-abstract/node_modules/object-inspect/package.json
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/es-define-property/package.json
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/es-define-property/tsconfig.json
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/es-errors/package.json
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/es-errors/tsconfig.json
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/es-object-atoms/package.json
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/es-object-atoms/tsconfig.json
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/es-set-tostringtag/package.json
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/es-set-tostringtag/tsconfig.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/es-to-primitive/package.json
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/esbuild/package.json
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/escalade/package.json
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/escape-string-regexp/package.json
+-rw-r--r--   0        0        0     5566 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/eslint/package.json
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/eslint/conf/replacements.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/eslint/conf/rule-type-list.json
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/eslint/lib/cli-engine/formatters/formatters-meta.json
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/eslint-config-prettier/package.json
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/eslint-plugin-prettier/package.json
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/eslint-plugin-vue/package.json
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/eslint-plugin-vue/lib/utils/deprecated-html-elements.json
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/eslint-plugin-vue/lib/utils/html-elements.json
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/eslint-plugin-vue/lib/utils/inline-non-void-elements.json
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/eslint-plugin-vue/lib/utils/js-reserved.json
+-rw-r--r--   0        0        0     5270 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/eslint-plugin-vue/lib/utils/key-aliases.json
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/eslint-plugin-vue/lib/utils/math-elements.json
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/eslint-plugin-vue/lib/utils/svg-attributes-weird-case.json
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/eslint-plugin-vue/lib/utils/svg-elements.json
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/eslint-plugin-vue/lib/utils/void-elements.json
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/eslint-plugin-vue/lib/utils/vue-component-options.json
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/eslint-plugin-vue/lib/utils/vue-reserved.json
+-rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/eslint-plugin-vue/lib/utils/vue3-export-names.json
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/eslint-scope/package.json
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/eslint-visitor-keys/package.json
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/espree/package.json
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/esquery/package.json
+-rwxr-xr-x   0        0        0     1165 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/esrecurse/package.json
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/estraverse/package.json
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/estree-walker/package.json
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/estree-walker/dist/esm/package.json
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/estree-walker/src/package.json
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/esutils/package.json
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/execa/package.json
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/fast-deep-equal/package.json
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/fast-diff/package.json
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/fast-glob/package.json
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/fast-glob/node_modules/glob-parent/package.json
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/fast-json-stable-stringify/package.json
+-rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/fast-json-stable-stringify/benchmark/test.json
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/fast-levenshtein/package.json
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/fastq/package.json
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/fastq/test/tsconfig.json
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/fecha/package.json
+-rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/file-entry-cache/package.json
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/fill-range/package.json
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/find-up/package.json
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/flat-cache/package.json
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/flatted/package.json
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/flatted/cjs/package.json
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/fmin/.eslintrc.json
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/fmin/package.json
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/follow-redirects/package.json
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/for-each/package.json
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/foreground-child/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/foreground-child/dist/cjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/foreground-child/dist/mjs/package.json
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/form-data/package.json
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/fraction.js/package.json
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/fs.realpath/package.json
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/function-bind/package.json
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/function.prototype.name/package.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/functions-have-names/package.json
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/get-func-name/package.json
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/get-intrinsic/package.json
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/get-stream/package.json
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/get-symbol-description/package.json
+-rwxr-xr-x   0        0        0      630 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/gl-matrix/package.json
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/gl-matrix/mat2/package.json
+-rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/gl-matrix/mat2d/package.json
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/gl-matrix/mat3/package.json
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/gl-matrix/mat4/package.json
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/gl-matrix/quat/package.json
+-rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/gl-matrix/quat2/package.json
+-rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/gl-matrix/types.d.ts/package.json
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/gl-matrix/vec2/package.json
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/gl-matrix/vec3/package.json
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/gl-matrix/vec4/package.json
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/glob/package.json
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/glob-parent/package.json
+-rw-r--r--   0        0        0    48140 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/globals/globals.json
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/globals/package.json
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/globalthis/package.json
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/gopd/package.json
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/graphemer/package.json
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/has/package.json
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/has-ansi/package.json
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/has-ansi/node_modules/ansi-regex/package.json
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/has-bigints/package.json
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/has-flag/package.json
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/has-property-descriptors/package.json
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/has-proto/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/has-proto/tsconfig.json
+-rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/has-symbols/package.json
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/has-tostringtag/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/has-tostringtag/tsconfig.json
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/hasown/package.json
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/hasown/tsconfig.json
+-rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/html2canvas/package.json
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/html2canvas/tsconfig.json
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/human-signals/package.json
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/husky/package.json
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/ignore/package.json
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/immutable/package.json
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/import-fresh/package.json
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/imurmurhash/package.json
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/inflight/package.json
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/inherits/package.json
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/internal-slot/package.json
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/is-arguments/package.json
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/is-array-buffer/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/is-array-buffer/tsconfig.json
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/is-bigint/package.json
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/is-binary-path/package.json
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/is-boolean-object/package.json
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/is-buffer/package.json
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/is-callable/package.json
+-rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/is-core-module/core.json
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/is-core-module/package.json
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/is-data-view/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/is-data-view/tsconfig.json
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/is-date-object/package.json
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/is-extglob/package.json
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/is-fullwidth-code-point/package.json
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/is-glob/package.json
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/is-negative-zero/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/is-negative-zero/tsconfig.json
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/is-number/package.json
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/is-number-object/package.json
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/is-path-inside/package.json
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/is-regex/package.json
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/is-shared-array-buffer/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/is-shared-array-buffer/tsconfig.json
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/is-stream/package.json
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/is-string/package.json
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/is-symbol/package.json
+-rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/is-typed-array/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/is-typed-array/tsconfig.json
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/is-weakref/package.json
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/isarray/package.json
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/isexe/package.json
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/jackspeak/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/jackspeak/dist/commonjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/jackspeak/dist/esm/package.json
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/jiti/package.json
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/js-tokens/package.json
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/js-yaml/package.json
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/json-buffer/package.json
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/json-schema-traverse/package.json
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/json-stable-stringify-without-jsonify/package.json
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/json2module/package.json
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/json5/package.json
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/keyv/package.json
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/kind-of/package.json
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/lazy-cache/package.json
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/levn/package.json
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/lilconfig/package.json
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/lines-and-columns/package.json
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/local-pkg/package.json
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/locate-path/package.json
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/lodash/package.json
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/lodash-es/package.json
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/lodash.merge/package.json
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/longest/package.json
+-rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/loupe/package.json
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/lru-cache/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/lru-cache/dist/commonjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/lru-cache/dist/esm/package.json
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/magic-string/package.json
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/merge-stream/package.json
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/merge2/package.json
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/micromatch/package.json
+-rw-r--r--   0        0        0   185882 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/mime-db/db.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/mime-db/package.json
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/mime-types/package.json
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/mimic-fn/package.json
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/minimatch/package.json
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/minimist/package.json
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/minipass/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/minipass/dist/commonjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/minipass/dist/esm/package.json
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/mlly/package.json
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/mock-property/package.json
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/mockjs/bower.json
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/mockjs/package.json
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/mockjs/test/bower.json
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/mockjs/test/package.json
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/moment/package.json
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/ms/package.json
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/mz/package.json
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/nanoid/package.json
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/nanoid/async/package.json
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/nanoid/non-secure/package.json
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/nanoid/url-alphabet/package.json
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/natural-compare/package.json
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/node-releases/package.json
+-rw-r--r--   0        0        0    29857 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/node-releases/data/processed/envs.json
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/node-releases/data/release-schedule/release-schedule.json
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/normalize-path/package.json
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/normalize-range/package.json
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/npm-run-path/package.json
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/npm-run-path/node_modules/path-key/package.json
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/nth-check/package.json
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/nth-check/lib/esm/package.json
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/object-assign/package.json
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/object-hash/package.json
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/object-inspect/package-support.json
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/object-inspect/package.json
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/object-is/package.json
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/object-keys/package.json
+-rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/object.assign/package.json
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/once/package.json
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/onetime/package.json
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/optionator/package.json
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/p-limit/package.json
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/p-locate/package.json
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/parent-module/package.json
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/path-exists/package.json
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/path-is-absolute/package.json
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/path-key/package.json
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/path-parse/package.json
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/path-scurry/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/path-scurry/dist/commonjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/path-scurry/dist/esm/package.json
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/pathe/package.json
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/pathval/package.json
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/pdfast/package.json
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/picocolors/package.json
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/picomatch/package.json
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/pify/package.json
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/pinia/package.json
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/pinia/node_modules/vue-demi/package.json
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/pirates/package.json
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/pkg-types/package.json
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/possible-typed-array-names/package.json
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/possible-typed-array-names/tsconfig.json
+-rwxr-xr-x   0        0        0     2496 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/postcss/package.json
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/postcss-import/package.json
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/postcss-js/package.json
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/postcss-load-config/package.json
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/postcss-load-config/node_modules/lilconfig/package.json
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/postcss-nested/package.json
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/postcss-selector-parser/package.json
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/postcss-value-parser/package.json
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/prelude-ls/package.json
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/prettier/package.json
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/prettier-linter-helpers/package.json
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/prettier-linter-helpers/.vscode/settings.json
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/pretty-format/package.json
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/pretty-format/node_modules/ansi-styles/package.json
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/proxy-from-env/package.json
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/punycode/package.json
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/queue-microtask/package.json
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/react-is/package.json
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/read-cache/package.json
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/readdirp/package.json
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/regexp.prototype.flags/package.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/repeat-string/package.json
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/resolve/package.json
+-rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/resolve/lib/core.json
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/resolve/test/module_dir/zmodules/bbb/package.json
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/resolve/test/resolver/baz/package.json
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/resolve/test/resolver/browser_field/package.json
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/resolve/test/resolver/dot_main/package.json
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/resolve/test/resolver/dot_slash_main/package.json
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/resolve/test/resolver/false_main/package.json
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/resolve/test/resolver/incorrect_main/package.json
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/resolve/test/resolver/invalid_main/package.json
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/resolve/test/resolver/multirepo/lerna.json
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/resolve/test/resolver/multirepo/package.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/resolve/test/resolver/multirepo/packages/package-a/package.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/resolve/test/resolver/multirepo/packages/package-b/package.json
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/resolve/test/resolver/nested_symlinks/mylib/package.json
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/resolve/test/resolver/symlinked/package/package.json
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/resolve-from/package.json
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/reusify/package.json
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/right-align/package.json
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/rimraf/package.json
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/rollup/package.json
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/rollup/node_modules/ansi-regex/package.json
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/rollup/node_modules/ansi-styles/package.json
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/rollup/node_modules/chalk/package.json
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/rollup/node_modules/escape-string-regexp/package.json
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/rollup/node_modules/strip-ansi/package.json
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/rollup/node_modules/supports-color/package.json
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/run-parallel/package.json
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/rw/package.json
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/safe-array-concat/package.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/safe-array-concat/tsconfig.json
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/safe-regex-test/package.json
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/sass/package.json
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/scule/package.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/semver/package.json
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/set-function-length/package.json
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/set-function-length/tsconfig.json
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/set-function-name/package.json
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/set-function-name/tsconfig.json
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/shebang-command/package.json
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/shebang-regex/package.json
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/side-channel/package.json
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/side-channel/tsconfig.json
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/side-channel/node_modules/object-inspect/package-support.json
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/side-channel/node_modules/object-inspect/package.json
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/siginfo/package.json
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/signal-exit/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/signal-exit/dist/cjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/signal-exit/dist/mjs/package.json
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/size-sensor/package.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/source-map/package.json
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/source-map-js/package.json
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/source-map-support/package.json
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/stackback/package.json
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/std-env/package.json
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/string-width/package.json
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/string-width/node_modules/ansi-regex/package.json
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/string-width/node_modules/strip-ansi/package.json
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/string-width-cjs/package.json
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/string-width-cjs/node_modules/emoji-regex/package.json
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/string.prototype.trim/package.json
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/string.prototype.trimend/package.json
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/string.prototype.trimstart/package.json
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/strip-ansi/package.json
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/strip-ansi-cjs/package.json
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/strip-final-newline/package.json
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/strip-json-comments/package.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/strip-literal/package.json
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/sucrase/package.json
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/sucrase/node_modules/brace-expansion/package.json
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/sucrase/node_modules/commander/package.json
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/sucrase/node_modules/glob/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/sucrase/node_modules/glob/dist/commonjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/sucrase/node_modules/glob/dist/esm/package.json
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/sucrase/node_modules/minimatch/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/sucrase/node_modules/minimatch/dist/commonjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/sucrase/node_modules/minimatch/dist/esm/package.json
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/supports-color/package.json
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/supports-preserve-symlinks-flag/package.json
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/tailwindcss/package.json
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/tailwindcss/stubs/.prettierrc.json
+-rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/tape/package.json
+-rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/terser/package.json
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/terser/bin/package.json
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/terser/dist/package.json
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/terser/node_modules/commander/package.json
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/terser/node_modules/source-map/package.json
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/terser/node_modules/source-map-support/package.json
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/text-segmentation/package.json
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/text-table/package.json
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/thenify/package.json
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/thenify-all/package.json
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/tinybench/package.json
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/tinypool/package.json
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/tinyspy/package.json
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/tippy.js/package.json
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/tippy.js/headless/package.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/to-regex-range/package.json
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/ts-interface-checker/package.json
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/tslib/package.json
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/tslib/modules/package.json
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/type-check/package.json
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/type-detect/package.json
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/type-fest/package.json
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/typed-array-buffer/package.json
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/typed-array-buffer/tsconfig.json
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/typed-array-byte-length/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/typed-array-byte-length/tsconfig.json
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/typed-array-byte-offset/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/typed-array-byte-offset/tsconfig.json
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/typed-array-length/package.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/typed-array-length/tsconfig.json
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/ufo/package.json
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/uglify-js/package.json
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/uglify-js/node_modules/source-map/package.json
+-rw-r--r--   0        0        0   142838 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/uglify-js/tools/domprops.json
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/uglify-to-browserify/package.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/unbox-primitive/package.json
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/unimport/package.json
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/unimport/node_modules/escape-string-regexp/package.json
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/unimport/node_modules/estree-walker/package.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/unimport/node_modules/local-pkg/package.json
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/unplugin/package.json
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/unplugin-auto-import/package.json
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/unplugin-auto-import/node_modules/brace-expansion/package.json
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/unplugin-auto-import/node_modules/minimatch/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/unplugin-auto-import/node_modules/minimatch/dist/commonjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/unplugin-auto-import/node_modules/minimatch/dist/esm/package.json
+-rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/unplugin-vue-components/package.json
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/unplugin-vue-components/node_modules/brace-expansion/package.json
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/unplugin-vue-components/node_modules/minimatch/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/unplugin-vue-components/node_modules/minimatch/dist/cjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/unplugin-vue-components/node_modules/minimatch/dist/mjs/package.json
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/update-browserslist-db/.devcontainer.json
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/update-browserslist-db/package.json
+-rwxr-xr-x   0        0        0     2172 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/uri-js/package.json
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/util-deprecate/package.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/utrie/package.json
+-rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/vite/package.json
+-rw-r--r--   0        0        0    10895 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/vite/node_modules/rollup/package.json
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/vite/node_modules/rollup/dist/es/package.json
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/vite/types/package.json
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/vite-node/package.json
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/vite-plugin-json5/package.json
+-rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/vitest/package.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/vitest/node_modules/local-pkg/package.json
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/vue/package.json
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/vue/compiler-sfc/package.json
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/vue/jsx-runtime/package.json
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/vue/server-renderer/package.json
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/vue-eslint-parser/package.json
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/vue-i18n/package.json
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/vue-i18n/vetur/attributes.json
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/vue-i18n/vetur/tags.json
+-rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/vue-router/package.json
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/vue-router/vetur/attributes.json
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/vue-router/vetur/tags.json
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/vue-tippy/package.json
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/vue-tippy/tsconfig.json
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/vue-tippy/vetur/attributes.json
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/vue-tippy/vetur/tags.json
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/webpack-sources/package.json
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/webpack-virtual-modules/package.json
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/which/package.json
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/which-boxed-primitive/package.json
+-rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/which-typed-array/package.json
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/which-typed-array/tsconfig.json
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/why-is-node-running/package.json
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/window-size/package.json
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/word-wrap/package.json
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/wordwrap/package.json
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/wrap-ansi/package.json
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/wrap-ansi/node_modules/ansi-regex/package.json
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/wrap-ansi/node_modules/ansi-styles/package.json
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/wrap-ansi/node_modules/strip-ansi/package.json
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/wrap-ansi-cjs/package.json
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/wrap-ansi-cjs/node_modules/emoji-regex/package.json
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/wrap-ansi-cjs/node_modules/string-width/package.json
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/wrappy/package.json
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/xml-name-validator/package.json
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/yaml/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/yaml/browser/package.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/yargs/package.json
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 swanlab-0.3.5/node_modules/yocto-queue/package.json
+-rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/__init__.py
+-rw-r--r--   0        0        0     9852 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/env.py
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/error.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/package.json
+-rw-r--r--   0        0        0     5471 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/package.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/api/__init__.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/api/cos.py
+-rw-r--r--   0        0        0     8817 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/api/http.py
+-rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/api/info.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/api/auth/__init__.py
+-rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/api/auth/login.py
+-rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/api/upload/__init__.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/api/upload/model.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/cli/__init__.py
+-rw-r--r--   0        0        0     7349 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/cli/main.py
+-rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/cli/utils.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/cloud/__init__.py
+-rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/cloud/_log_collector.py
+-rw-r--r--   0        0        0     5508 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/cloud/start_thread.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/cloud/task_types.py
+-rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/cloud/utils.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/cloud/dog/README.md
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/cloud/dog/__init__.py
+-rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/cloud/dog/log_sniffer.py
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/cloud/dog/metadata_handle.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/cloud/dog/sniffer_queue.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/compat/README.md
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/compat/server/controller/experiment.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/converter/__init__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/converter/tfb/__init__.py
+-rw-r--r--   0        0        0     4493 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/converter/tfb/_utils.py
+-rw-r--r--   0        0        0     4170 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/converter/tfb/tfb_converter.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/converter/wb/__init__.py
+-rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/converter/wb/wb_converter.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/data/__init__.py
+-rw-r--r--   0        0        0     7136 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/data/callback_cloud.py
+-rw-r--r--   0        0        0     5983 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/data/callback_local.py
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/data/config.py
+-rw-r--r--   0        0        0    13030 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/data/sdk.py
+-rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/data/settings.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/data/modules/__init__.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/data/modules/_utils.py
+-rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/data/modules/audio.py
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/data/modules/base.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/data/modules/chart.py
+-rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/data/modules/image.py
+-rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/data/modules/object_3d.py
+-rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/data/modules/text.py
+-rw-r--r--   0        0        0     7738 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/data/modules/video.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/data/modules/utils_modules/__init__.py
+-rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/data/modules/utils_modules/bounding_boxes.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/data/modules/utils_modules/image_mask.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/data/run/__init__.py
+-rw-r--r--   0        0        0     8506 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/data/run/callback.py
+-rw-r--r--   0        0        0    16930 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/data/run/exp.py
+-rw-r--r--   0        0        0    13553 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/data/run/main.py
+-rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/data/run/operator.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/data/system/__init__.py
+-rw-r--r--   0        0        0     8065 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/data/system/info.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/data/system/monitor.py
+-rwxr-xr-x   0        0        0   337072 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/data/system/bin/apple_gpu_stats
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/db/__init__.py
+-rw-r--r--   0        0        0     8012 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/db/callback.py
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/db/db_connect.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/db/error.py
+-rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/db/model.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/db/table_config.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/db/docs/Errors.md
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/db/docs/README.md
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/db/migrate/__init__.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/db/migrate/chart.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/db/migrate/experiment.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/db/migrate/namespace.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/db/migrate/project.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/db/migrate/tag.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/db/models/__init__.py
+-rw-r--r--   0        0        0     9068 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/db/models/charts.py
+-rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/db/models/displays.py
+-rw-r--r--   0        0        0     6632 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/db/models/experiments.py
+-rw-r--r--   0        0        0     6326 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/db/models/namespaces.py
+-rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/db/models/projects.py
+-rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/db/models/sources.py
+-rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/db/models/tags.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/db/utils/__init__.py
+-rw-r--r--   0        0        0     9078 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/db/utils/chart.py
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/integration/fastai.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/integration/huggingface.py
+-rw-r--r--   0        0        0     7392 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/integration/mmengine.py
+-rw-r--r--   0        0        0     7301 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/integration/pytorch_lightning.py
+-rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/integration/sb3.py
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/integration/ultralytics.py
+-rw-r--r--   0        0        0     8539 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/integration/integration_utils/autologging.py
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/integration/integration_utils/get_modules.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/integration/integration_utils/timer.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/integration/openai/__init__.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/integration/openai/openai.py
+-rw-r--r--   0        0        0    19701 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/integration/openai/resolver.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/integration/zhipuai/__init__.py
+-rw-r--r--   0        0        0     7125 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/integration/zhipuai/resolver.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/integration/zhipuai/zhipuai.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/log/__init__.py
+-rw-r--r--   0        0        0     5581 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/log/console.py
+-rw-r--r--   0        0        0     9090 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/log/log.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/server/__init__.py
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/server/app.py
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/server/settings.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/server/controller/chart.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/server/controller/db.py
+-rw-r--r--   0        0        0    16723 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/server/controller/experiment.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/server/controller/namespace.py
+-rw-r--r--   0        0        0     8076 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/server/controller/project.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/server/controller/utils/__init__.py
+-rw-r--r--   0        0        0     6976 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/server/controller/utils/charts.py
+-rw-r--r--   0        0        0     5042 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/server/controller/utils/tag.py
+-rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/server/middleware/common.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/server/module/__init__.py
+-rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/server/module/resp.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/server/router/chart.py
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/server/router/experiment.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/server/router/media.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/server/router/namespace.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/server/router/project.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/index.html
+-rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/assets/ChartPage-C2Rj7xI3.js
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/assets/ChartPage-DgOOkrVh.css
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/assets/ChartsView-DpI6U3QH.js
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/assets/EnvHardware-4H7mp2Bs.js
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/assets/EnvIndex-B5_l1b65.js
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/assets/EnvItems-B4PwmQT4.js
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/assets/EnvItems-BfjcRO-X.css
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/assets/EnvRequirements-BqyzUHLZ.css
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/assets/EnvRequirements-Cpn2Fk1D.js
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/assets/EnvironmentPage-Bb8ousXq.js
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/assets/EnvironmentPage-C6uSuWBq.css
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/assets/ExperimentView-BTbu21ka.js
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/assets/ExperimentView-CCDMXo4h.css
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/assets/FuncBar-Ct_nBdvU.js
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/assets/FuncBar-DgVTuZfd.css
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/assets/HelpView-C4wSXY1I.js
+-rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/assets/HomeView-BS7FyMAt.css
+-rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/assets/HomeView-BqTu9_fG.js
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/assets/IndexPage-C5dvtib2.css
+-rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/assets/IndexPage-CrqN4Ekl.js
+-rw-r--r--   0        0        0   273900 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/assets/JetBrainsMono-Regular-Dh36KTnx.ttf
+-rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/assets/LogPage-B-fC6sB7.js
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/assets/LogPage-DBzoauOW.css
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/assets/NotFound-DijsQ96i.js
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/assets/SLLoading-6DfF2aH0.js
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/assets/SLStatusLabel-BRacn5XK.css
+-rw-r--r--   0        0        0     5489 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/assets/SLStatusLabel-DvEKZN8v.js
+-rw-r--r--   0        0        0   119080 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/assets/SourceSansPro-Regular-J3NOkSfZ.ttf
+-rw-r--r--   0        0        0    12117 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/assets/chart-DB312WPs.css
+-rw-r--r--   0        0        0  1098521 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/assets/chart-eW1meEc1.js
+-rw-r--r--   0        0        0   393892 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/assets/index-B5SDzoY4.js
+-rw-r--r--   0        0        0    37013 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/assets/index-B7Izi8NT.css
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/template/assets/logo-ChHf2ozk.ico
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/utils/__init__.py
+-rw-r--r--   0        0        0     7816 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/utils/file.py
+-rw-r--r--   0        0        0     8727 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/utils/font.py
+-rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/utils/judgment.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/utils/key.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 swanlab-0.3.5/swanlab/utils/time.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 swanlab-0.3.5/test/create_error_chart.py
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 swanlab-0.3.5/test/create_experiment.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 swanlab-0.3.5/test/start_server.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 swanlab-0.3.5/test/use_swanlog.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 swanlab-0.3.5/test/config/config.json
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 swanlab-0.3.5/test/config/load.yaml
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 swanlab-0.3.5/test/integration/.gitignore
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 swanlab-0.3.5/test/integration/README.md
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 swanlab-0.3.5/test/integration/fastai/fastai_train.py
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 swanlab-0.3.5/test/integration/fastai/requirements.txt
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 swanlab-0.3.5/test/integration/huggingface/requirements.txt
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 swanlab-0.3.5/test/integration/huggingface/transformers_bert_train.py
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 swanlab-0.3.5/test/integration/lightning/lightning_base.py
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 swanlab-0.3.5/test/integration/lightning/lightning_train.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 swanlab-0.3.5/test/integration/lightning/requirements.txt
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 swanlab-0.3.5/test/integration/sb3/requirements.txt
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 swanlab-0.3.5/test/integration/sb3/sb3_PPO.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 swanlab-0.3.5/test/integration/ultralytics/requirements.txt
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 swanlab-0.3.5/test/integration/ultralytics/ultralytics_classifer.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 swanlab-0.3.5/test/integration/ultralytics/ultralytics_detection.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 swanlab-0.3.5/test/integration/ultralytics/ultralytics_pose.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 swanlab-0.3.5/test/integration/ultralytics/ultralytics_segmentation.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 swanlab-0.3.5/test/unit/conftest.py
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 swanlab-0.3.5/test/unit/pytest_env.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 swanlab-0.3.5/test/unit/pytest_example.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 swanlab-0.3.5/test/unit/auth/pytest_login.py
+-rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 swanlab-0.3.5/test/unit/data/pytest_sdk.py
+-rw-r--r--   0        0        0    20154 2020-02-02 00:00:00.000000 swanlab-0.3.5/test/unit/data/run/pytest_main.py
+-rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 swanlab-0.3.5/test/unit/log/pytest_log.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 swanlab-0.3.5/test/unit/server/controller/utils/utils.py
+-rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 swanlab-0.3.5/test/unit/utils/pytest_file.py
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 swanlab-0.3.5/test/unit/utils/pytest_key.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 swanlab-0.3.5/test/unit/utils/pytest_package.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 swanlab-0.3.5/.gitignore
+-rw-r--r--   0        0        0    10779 2020-02-02 00:00:00.000000 swanlab-0.3.5/LICENSE
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 swanlab-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0    31011 2020-02-02 00:00:00.000000 swanlab-0.3.5/PKG-INFO
```

### Comparing `swanlab-0.3.4/.eslintrc-auto-import.json` & `swanlab-0.3.5/.eslintrc-auto-import.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/README.md` & `swanlab-0.3.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -492,28 +492,28 @@
 
 ## 💻 Self-hosted
 
 The community edition supports offline viewing of SwanLab dashboards.
 
 ### Offline Experiment Tracking
 
-Set the parameters `logir` and `cloud` in swanlab.init to track experiments offline:
+Set the parameters `logir` and `mode` in swanlab.init to track experiments offline:
 
 ```python
 ...
 
 swanlab.init(
     logdir='./logs',
-    cloud=False,
+    mode='local',
 )
 
 ...
 ```
 
-- The parameter `cloud` is set to `False`, which disables synchronizing the experiment to the cloud.
+- The parameter `mode` is set to `local`, which disables synchronizing the experiment to the cloud.
 
 - The setting of the parameter `logdir` is optional, and it specifies the location for saving SwanLab log files (by
   default saved in the `swanlog` folder).
 
 - Log files will be created and updated during tracking of experiments, and launching offline dashboards will also be
   based on these log files.
```

### Comparing `swanlab-0.3.4/package-lock.json` & `swanlab-0.3.5/package-lock.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/package.json` & `swanlab-0.3.5/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/.vscode/extensions.json` & `swanlab-0.3.5/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/.vscode/launch.json` & `swanlab-0.3.5/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/.vscode/settings.json` & `swanlab-0.3.5/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/.vscode/tailwind.json` & `swanlab-0.3.5/.vscode/tailwind.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/.package-lock.json` & `swanlab-0.3.5/node_modules/.package-lock.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@alloc/quick-lru/package.json` & `swanlab-0.3.5/node_modules/@alloc/quick-lru/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@antfu/utils/package.json` & `swanlab-0.3.5/node_modules/@antfu/utils/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@antv/adjust/package.json` & `swanlab-0.3.5/node_modules/@antv/adjust/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@antv/adjust/node_modules/tslib/package.json` & `swanlab-0.3.5/node_modules/@antv/adjust/node_modules/tslib/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@antv/attr/package.json` & `swanlab-0.3.5/node_modules/@antv/attr/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@antv/color-util/package.json` & `swanlab-0.3.5/node_modules/@antv/color-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@antv/component/package.json` & `swanlab-0.3.5/node_modules/@antv/component/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@antv/component/node_modules/@antv/path-util/package.json` & `swanlab-0.3.5/node_modules/@antv/component/node_modules/@antv/path-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@antv/component/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json` & `swanlab-0.3.5/node_modules/@antv/component/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@antv/coord/package.json` & `swanlab-0.3.5/node_modules/@antv/coord/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@antv/dom-util/package.json` & `swanlab-0.3.5/node_modules/@antv/dom-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@antv/event-emitter/package.json` & `swanlab-0.3.5/node_modules/@antv/event-emitter/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@antv/g-base/package.json` & `swanlab-0.3.5/node_modules/@antv/g-base/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@antv/g-base/node_modules/@antv/path-util/package.json` & `swanlab-0.3.5/node_modules/@antv/g-base/node_modules/@antv/path-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@antv/g-base/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json` & `swanlab-0.3.5/node_modules/@antv/g-base/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@antv/g-canvas/package.json` & `swanlab-0.3.5/node_modules/@antv/g-canvas/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@antv/g-canvas/node_modules/@antv/path-util/package.json` & `swanlab-0.3.5/node_modules/@antv/g-canvas/node_modules/@antv/path-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@antv/g-canvas/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json` & `swanlab-0.3.5/node_modules/@antv/g-canvas/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@antv/g-math/package.json` & `swanlab-0.3.5/node_modules/@antv/g-math/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@antv/g-svg/package.json` & `swanlab-0.3.5/node_modules/@antv/g-svg/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@antv/g2/package.json` & `swanlab-0.3.5/node_modules/@antv/g2/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@antv/g2/node_modules/@antv/path-util/package.json` & `swanlab-0.3.5/node_modules/@antv/g2/node_modules/@antv/path-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@antv/g2/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json` & `swanlab-0.3.5/node_modules/@antv/g2/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@antv/g2plot/package.json` & `swanlab-0.3.5/node_modules/@antv/g2plot/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@antv/matrix-util/package.json` & `swanlab-0.3.5/node_modules/@antv/matrix-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@antv/path-util/package.json` & `swanlab-0.3.5/node_modules/@antv/path-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@antv/scale/package.json` & `swanlab-0.3.5/node_modules/@antv/scale/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@antv/util/package.json` & `swanlab-0.3.5/node_modules/@antv/util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@babel/parser/package.json` & `swanlab-0.3.5/node_modules/@babel/parser/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@eslint/eslintrc/package.json` & `swanlab-0.3.5/node_modules/@eslint/eslintrc/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@eslint/js/package.json` & `swanlab-0.3.5/node_modules/@eslint/js/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@eslint-community/eslint-utils/package.json` & `swanlab-0.3.5/node_modules/@eslint-community/eslint-utils/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@eslint-community/regexpp/package.json` & `swanlab-0.3.5/node_modules/@eslint-community/regexpp/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@headlessui/vue/package.json` & `swanlab-0.3.5/node_modules/@headlessui/vue/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@humanwhocodes/config-array/package.json` & `swanlab-0.3.5/node_modules/@humanwhocodes/config-array/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@humanwhocodes/module-importer/package.json` & `swanlab-0.3.5/node_modules/@humanwhocodes/module-importer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@humanwhocodes/object-schema/package.json` & `swanlab-0.3.5/node_modules/@humanwhocodes/object-schema/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@intlify/core-base/package.json` & `swanlab-0.3.5/node_modules/@intlify/core-base/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@intlify/message-compiler/package.json` & `swanlab-0.3.5/node_modules/@intlify/message-compiler/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@intlify/shared/package.json` & `swanlab-0.3.5/node_modules/@intlify/shared/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@isaacs/cliui/package.json` & `swanlab-0.3.5/node_modules/@isaacs/cliui/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@isaacs/cliui/node_modules/ansi-regex/package.json` & `swanlab-0.3.5/node_modules/@isaacs/cliui/node_modules/ansi-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@isaacs/cliui/node_modules/strip-ansi/package.json` & `swanlab-0.3.5/node_modules/@isaacs/cliui/node_modules/strip-ansi/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@jest/schemas/package.json` & `swanlab-0.3.5/node_modules/@jest/schemas/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@jridgewell/gen-mapping/package.json` & `swanlab-0.3.5/node_modules/@jridgewell/gen-mapping/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@jridgewell/resolve-uri/package.json` & `swanlab-0.3.5/node_modules/@jridgewell/resolve-uri/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@jridgewell/set-array/package.json` & `swanlab-0.3.5/node_modules/@jridgewell/set-array/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@jridgewell/source-map/package.json` & `swanlab-0.3.5/node_modules/@jridgewell/source-map/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@jridgewell/sourcemap-codec/package.json` & `swanlab-0.3.5/node_modules/@jridgewell/sourcemap-codec/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@jridgewell/trace-mapping/package.json` & `swanlab-0.3.5/node_modules/@jridgewell/trace-mapping/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@ljharb/resumer/package.json` & `swanlab-0.3.5/node_modules/@ljharb/resumer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@ljharb/through/package.json` & `swanlab-0.3.5/node_modules/@ljharb/through/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@nodelib/fs.scandir/package.json` & `swanlab-0.3.5/node_modules/@nodelib/fs.scandir/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@nodelib/fs.stat/package.json` & `swanlab-0.3.5/node_modules/@nodelib/fs.stat/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@nodelib/fs.walk/package.json` & `swanlab-0.3.5/node_modules/@nodelib/fs.walk/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@pkgjs/parseargs/package.json` & `swanlab-0.3.5/node_modules/@pkgjs/parseargs/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@popperjs/core/package.json` & `swanlab-0.3.5/node_modules/@popperjs/core/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@rollup/pluginutils/package.json` & `swanlab-0.3.5/node_modules/@rollup/pluginutils/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@sinclair/typebox/package.json` & `swanlab-0.3.5/node_modules/@sinclair/typebox/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@tanstack/virtual-core/package.json` & `swanlab-0.3.5/node_modules/@tanstack/virtual-core/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@tanstack/vue-virtual/package.json` & `swanlab-0.3.5/node_modules/@tanstack/vue-virtual/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@types/d3-timer/package.json` & `swanlab-0.3.5/node_modules/@types/d3-timer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@types/estree/package.json` & `swanlab-0.3.5/node_modules/@types/estree/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@ungap/structured-clone/package.json` & `swanlab-0.3.5/node_modules/@ungap/structured-clone/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@vitejs/plugin-vue/package.json` & `swanlab-0.3.5/node_modules/@vitejs/plugin-vue/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@vitest/expect/package.json` & `swanlab-0.3.5/node_modules/@vitest/expect/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@vitest/runner/package.json` & `swanlab-0.3.5/node_modules/@vitest/runner/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@vitest/runner/node_modules/p-limit/package.json` & `swanlab-0.3.5/node_modules/@vitest/runner/node_modules/p-limit/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@vitest/runner/node_modules/yocto-queue/package.json` & `swanlab-0.3.5/node_modules/@vitest/runner/node_modules/yocto-queue/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@vitest/snapshot/package.json` & `swanlab-0.3.5/node_modules/@vitest/snapshot/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@vitest/spy/package.json` & `swanlab-0.3.5/node_modules/@vitest/spy/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@vitest/utils/package.json` & `swanlab-0.3.5/node_modules/@vitest/utils/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@vitest/utils/node_modules/estree-walker/package.json` & `swanlab-0.3.5/node_modules/@vitest/utils/node_modules/estree-walker/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@vue/compiler-core/package.json` & `swanlab-0.3.5/node_modules/@vue/compiler-core/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@vue/compiler-dom/package.json` & `swanlab-0.3.5/node_modules/@vue/compiler-dom/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@vue/compiler-sfc/package.json` & `swanlab-0.3.5/node_modules/@vue/compiler-sfc/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@vue/compiler-ssr/package.json` & `swanlab-0.3.5/node_modules/@vue/compiler-ssr/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@vue/devtools-api/package.json` & `swanlab-0.3.5/node_modules/@vue/devtools-api/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@vue/reactivity/package.json` & `swanlab-0.3.5/node_modules/@vue/reactivity/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@vue/runtime-core/package.json` & `swanlab-0.3.5/node_modules/@vue/runtime-core/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@vue/runtime-dom/package.json` & `swanlab-0.3.5/node_modules/@vue/runtime-dom/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@vue/server-renderer/package.json` & `swanlab-0.3.5/node_modules/@vue/server-renderer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/@vue/shared/package.json` & `swanlab-0.3.5/node_modules/@vue/shared/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/acorn/package.json` & `swanlab-0.3.5/node_modules/acorn/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/acorn-jsx/package.json` & `swanlab-0.3.5/node_modules/acorn-jsx/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/acorn-walk/package.json` & `swanlab-0.3.5/node_modules/acorn-walk/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/ajv/package.json` & `swanlab-0.3.5/node_modules/ajv/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/ajv/lib/refs/data.json` & `swanlab-0.3.5/node_modules/ajv/lib/refs/data.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/ajv/lib/refs/json-schema-draft-04.json` & `swanlab-0.3.5/node_modules/ajv/lib/refs/json-schema-draft-04.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/ajv/lib/refs/json-schema-draft-06.json` & `swanlab-0.3.5/node_modules/ajv/lib/refs/json-schema-draft-06.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/ajv/lib/refs/json-schema-draft-07.json` & `swanlab-0.3.5/node_modules/ajv/lib/refs/json-schema-draft-07.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/ajv/lib/refs/json-schema-secure.json` & `swanlab-0.3.5/node_modules/ajv/lib/refs/json-schema-secure.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/align-text/package.json` & `swanlab-0.3.5/node_modules/align-text/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/ansi-regex/package.json` & `swanlab-0.3.5/node_modules/ansi-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/ansi-styles/package.json` & `swanlab-0.3.5/node_modules/ansi-styles/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/any-promise/package.json` & `swanlab-0.3.5/node_modules/any-promise/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/anymatch/package.json` & `swanlab-0.3.5/node_modules/anymatch/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/arg/package.json` & `swanlab-0.3.5/node_modules/arg/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/argparse/package.json` & `swanlab-0.3.5/node_modules/argparse/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/array-buffer-byte-length/package.json` & `swanlab-0.3.5/node_modules/array-buffer-byte-length/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/array-buffer-byte-length/tsconfig.json` & `swanlab-0.3.5/node_modules/array-buffer-byte-length/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/arraybuffer.prototype.slice/package.json` & `swanlab-0.3.5/node_modules/arraybuffer.prototype.slice/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/assertion-error/package.json` & `swanlab-0.3.5/node_modules/assertion-error/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/asynckit/package.json` & `swanlab-0.3.5/node_modules/asynckit/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/autoprefixer/package.json` & `swanlab-0.3.5/node_modules/autoprefixer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/available-typed-arrays/package.json` & `swanlab-0.3.5/node_modules/available-typed-arrays/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/available-typed-arrays/tsconfig.json` & `swanlab-0.3.5/node_modules/available-typed-arrays/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/axios/package.json` & `swanlab-0.3.5/node_modules/axios/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/balanced-match/package.json` & `swanlab-0.3.5/node_modules/balanced-match/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/base64-arraybuffer/package.json` & `swanlab-0.3.5/node_modules/base64-arraybuffer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/binary-extensions/binary-extensions.json` & `swanlab-0.3.5/node_modules/binary-extensions/binary-extensions.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/binary-extensions/package.json` & `swanlab-0.3.5/node_modules/binary-extensions/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/boolbase/package.json` & `swanlab-0.3.5/node_modules/boolbase/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/brace-expansion/package.json` & `swanlab-0.3.5/node_modules/brace-expansion/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/braces/package.json` & `swanlab-0.3.5/node_modules/braces/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/browserslist/package.json` & `swanlab-0.3.5/node_modules/browserslist/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/cac/package.json` & `swanlab-0.3.5/node_modules/cac/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/call-bind/package.json` & `swanlab-0.3.5/node_modules/call-bind/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/callsites/package.json` & `swanlab-0.3.5/node_modules/callsites/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/camelcase/package.json` & `swanlab-0.3.5/node_modules/camelcase/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/camelcase-css/package.json` & `swanlab-0.3.5/node_modules/camelcase-css/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/caniuse-lite/package.json` & `swanlab-0.3.5/node_modules/caniuse-lite/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/center-align/package.json` & `swanlab-0.3.5/node_modules/center-align/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/chai/package.json` & `swanlab-0.3.5/node_modules/chai/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/chalk/package.json` & `swanlab-0.3.5/node_modules/chalk/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/check-error/package.json` & `swanlab-0.3.5/node_modules/check-error/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/chokidar/package.json` & `swanlab-0.3.5/node_modules/chokidar/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/chokidar/node_modules/glob-parent/package.json` & `swanlab-0.3.5/node_modules/chokidar/node_modules/glob-parent/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/cliui/package.json` & `swanlab-0.3.5/node_modules/cliui/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/color-convert/package.json` & `swanlab-0.3.5/node_modules/color-convert/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/color-name/package.json` & `swanlab-0.3.5/node_modules/color-name/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/combined-stream/package.json` & `swanlab-0.3.5/node_modules/combined-stream/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/commander/package.json` & `swanlab-0.3.5/node_modules/commander/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/concat-map/package.json` & `swanlab-0.3.5/node_modules/concat-map/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/confbox/package.json` & `swanlab-0.3.5/node_modules/confbox/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/contour_plot/package.json` & `swanlab-0.3.5/node_modules/contour_plot/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/cross-spawn/package.json` & `swanlab-0.3.5/node_modules/cross-spawn/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/css-line-break/package.json` & `swanlab-0.3.5/node_modules/css-line-break/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/cssesc/package.json` & `swanlab-0.3.5/node_modules/cssesc/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/csstype/package.json` & `swanlab-0.3.5/node_modules/csstype/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/d3-color/package.json` & `swanlab-0.3.5/node_modules/d3-color/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/d3-ease/package.json` & `swanlab-0.3.5/node_modules/d3-ease/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/d3-hierarchy/package.json` & `swanlab-0.3.5/node_modules/d3-hierarchy/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/d3-interpolate/package.json` & `swanlab-0.3.5/node_modules/d3-interpolate/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/d3-regression/package.json` & `swanlab-0.3.5/node_modules/d3-regression/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/d3-timer/package.json` & `swanlab-0.3.5/node_modules/d3-timer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/data-view-buffer/package.json` & `swanlab-0.3.5/node_modules/data-view-buffer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/data-view-buffer/tsconfig.json` & `swanlab-0.3.5/node_modules/data-view-buffer/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/data-view-byte-length/package.json` & `swanlab-0.3.5/node_modules/data-view-byte-length/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/data-view-byte-offset/package.json` & `swanlab-0.3.5/node_modules/data-view-byte-offset/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/data-view-byte-offset/tsconfig.json` & `swanlab-0.3.5/node_modules/data-view-byte-offset/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/debug/package.json` & `swanlab-0.3.5/node_modules/debug/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/decamelize/package.json` & `swanlab-0.3.5/node_modules/decamelize/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/deep-eql/package.json` & `swanlab-0.3.5/node_modules/deep-eql/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/deep-equal/package.json` & `swanlab-0.3.5/node_modules/deep-equal/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/deep-is/package.json` & `swanlab-0.3.5/node_modules/deep-is/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/define-data-property/package.json` & `swanlab-0.3.5/node_modules/define-data-property/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/define-data-property/tsconfig.json` & `swanlab-0.3.5/node_modules/define-data-property/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/define-properties/package.json` & `swanlab-0.3.5/node_modules/define-properties/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/defined/package.json` & `swanlab-0.3.5/node_modules/defined/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/delayed-stream/package.json` & `swanlab-0.3.5/node_modules/delayed-stream/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/detect-browser/package.json` & `swanlab-0.3.5/node_modules/detect-browser/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/didyoumean/package.json` & `swanlab-0.3.5/node_modules/didyoumean/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/diff-sequences/package.json` & `swanlab-0.3.5/node_modules/diff-sequences/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/dlv/package.json` & `swanlab-0.3.5/node_modules/dlv/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/doctrine/package.json` & `swanlab-0.3.5/node_modules/doctrine/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/dotignore/package.json` & `swanlab-0.3.5/node_modules/dotignore/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/electron-to-chromium/chromium-versions.json` & `swanlab-0.3.5/node_modules/electron-to-chromium/chromium-versions.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/electron-to-chromium/full-chromium-versions.json` & `swanlab-0.3.5/node_modules/electron-to-chromium/full-chromium-versions.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/electron-to-chromium/full-versions.json` & `swanlab-0.3.5/node_modules/electron-to-chromium/full-versions.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/electron-to-chromium/package.json` & `swanlab-0.3.5/node_modules/electron-to-chromium/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/electron-to-chromium/versions.json` & `swanlab-0.3.5/node_modules/electron-to-chromium/versions.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/emoji-regex/package.json` & `swanlab-0.3.5/node_modules/emoji-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/entities/package.json` & `swanlab-0.3.5/node_modules/entities/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/es-abstract/package.json` & `swanlab-0.3.5/node_modules/es-abstract/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/es-abstract/helpers/caseFolding.json` & `swanlab-0.3.5/node_modules/es-abstract/helpers/caseFolding.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/es-abstract/node_modules/object-inspect/package.json` & `swanlab-0.3.5/node_modules/es-abstract/node_modules/object-inspect/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/es-define-property/package.json` & `swanlab-0.3.5/node_modules/es-define-property/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/es-define-property/tsconfig.json` & `swanlab-0.3.5/node_modules/es-define-property/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/es-errors/package.json` & `swanlab-0.3.5/node_modules/es-errors/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/es-errors/tsconfig.json` & `swanlab-0.3.5/node_modules/es-errors/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/es-object-atoms/package.json` & `swanlab-0.3.5/node_modules/es-object-atoms/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/es-set-tostringtag/package.json` & `swanlab-0.3.5/node_modules/es-set-tostringtag/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/es-set-tostringtag/tsconfig.json` & `swanlab-0.3.5/node_modules/es-set-tostringtag/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/es-to-primitive/package.json` & `swanlab-0.3.5/node_modules/es-to-primitive/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/esbuild/package.json` & `swanlab-0.3.5/node_modules/esbuild/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/escalade/package.json` & `swanlab-0.3.5/node_modules/escalade/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/escape-string-regexp/package.json` & `swanlab-0.3.5/node_modules/escape-string-regexp/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/eslint/package.json` & `swanlab-0.3.5/node_modules/eslint/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/eslint/conf/replacements.json` & `swanlab-0.3.5/node_modules/eslint/conf/replacements.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/eslint/conf/rule-type-list.json` & `swanlab-0.3.5/node_modules/eslint/conf/rule-type-list.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/eslint/lib/cli-engine/formatters/formatters-meta.json` & `swanlab-0.3.5/node_modules/eslint/lib/cli-engine/formatters/formatters-meta.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/eslint-plugin-prettier/package.json` & `swanlab-0.3.5/node_modules/eslint-plugin-prettier/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/eslint-plugin-vue/package.json` & `swanlab-0.3.5/node_modules/eslint-plugin-vue/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/html-elements.json` & `swanlab-0.3.5/node_modules/eslint-plugin-vue/lib/utils/html-elements.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/js-reserved.json` & `swanlab-0.3.5/node_modules/eslint-plugin-vue/lib/utils/js-reserved.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/key-aliases.json` & `swanlab-0.3.5/node_modules/eslint-plugin-vue/lib/utils/key-aliases.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/svg-attributes-weird-case.json` & `swanlab-0.3.5/node_modules/eslint-plugin-vue/lib/utils/svg-attributes-weird-case.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/svg-elements.json` & `swanlab-0.3.5/node_modules/eslint-plugin-vue/lib/utils/svg-elements.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/vue-component-options.json` & `swanlab-0.3.5/node_modules/eslint-plugin-vue/lib/utils/vue-component-options.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/vue3-export-names.json` & `swanlab-0.3.5/node_modules/eslint-plugin-vue/lib/utils/vue3-export-names.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/eslint-scope/package.json` & `swanlab-0.3.5/node_modules/eslint-scope/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/eslint-visitor-keys/package.json` & `swanlab-0.3.5/node_modules/eslint-visitor-keys/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/espree/package.json` & `swanlab-0.3.5/node_modules/espree/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/esquery/package.json` & `swanlab-0.3.5/node_modules/esquery/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/esrecurse/package.json` & `swanlab-0.3.5/node_modules/esrecurse/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/estraverse/package.json` & `swanlab-0.3.5/node_modules/estraverse/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/estree-walker/package.json` & `swanlab-0.3.5/node_modules/estree-walker/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/esutils/package.json` & `swanlab-0.3.5/node_modules/esutils/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/execa/package.json` & `swanlab-0.3.5/node_modules/execa/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/fast-deep-equal/package.json` & `swanlab-0.3.5/node_modules/fast-deep-equal/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/fast-diff/package.json` & `swanlab-0.3.5/node_modules/fast-diff/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/fast-glob/package.json` & `swanlab-0.3.5/node_modules/fast-glob/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/fast-glob/node_modules/glob-parent/package.json` & `swanlab-0.3.5/node_modules/fast-glob/node_modules/glob-parent/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/fast-json-stable-stringify/package.json` & `swanlab-0.3.5/node_modules/fast-json-stable-stringify/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/fast-json-stable-stringify/benchmark/test.json` & `swanlab-0.3.5/node_modules/fast-json-stable-stringify/benchmark/test.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/fast-levenshtein/package.json` & `swanlab-0.3.5/node_modules/fast-levenshtein/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/fastq/package.json` & `swanlab-0.3.5/node_modules/fastq/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/fecha/package.json` & `swanlab-0.3.5/node_modules/fecha/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/file-entry-cache/package.json` & `swanlab-0.3.5/node_modules/file-entry-cache/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/fill-range/package.json` & `swanlab-0.3.5/node_modules/fill-range/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/find-up/package.json` & `swanlab-0.3.5/node_modules/find-up/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/flat-cache/package.json` & `swanlab-0.3.5/node_modules/flat-cache/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/flatted/package.json` & `swanlab-0.3.5/node_modules/flatted/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/fmin/package.json` & `swanlab-0.3.5/node_modules/fmin/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/follow-redirects/package.json` & `swanlab-0.3.5/node_modules/follow-redirects/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/for-each/package.json` & `swanlab-0.3.5/node_modules/for-each/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/foreground-child/package.json` & `swanlab-0.3.5/node_modules/foreground-child/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/form-data/package.json` & `swanlab-0.3.5/node_modules/form-data/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/fraction.js/package.json` & `swanlab-0.3.5/node_modules/fraction.js/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/fs.realpath/package.json` & `swanlab-0.3.5/node_modules/fs.realpath/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/function-bind/package.json` & `swanlab-0.3.5/node_modules/function-bind/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/function.prototype.name/package.json` & `swanlab-0.3.5/node_modules/function.prototype.name/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/functions-have-names/package.json` & `swanlab-0.3.5/node_modules/functions-have-names/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/get-func-name/package.json` & `swanlab-0.3.5/node_modules/get-func-name/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/get-intrinsic/package.json` & `swanlab-0.3.5/node_modules/get-intrinsic/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/get-stream/package.json` & `swanlab-0.3.5/node_modules/get-stream/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/get-symbol-description/package.json` & `swanlab-0.3.5/node_modules/get-symbol-description/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/gl-matrix/package.json` & `swanlab-0.3.5/node_modules/gl-matrix/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/glob/package.json` & `swanlab-0.3.5/node_modules/glob/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/glob-parent/package.json` & `swanlab-0.3.5/node_modules/glob-parent/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/globals/globals.json` & `swanlab-0.3.5/node_modules/globals/globals.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/globals/package.json` & `swanlab-0.3.5/node_modules/globals/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/globalthis/package.json` & `swanlab-0.3.5/node_modules/globalthis/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/gopd/package.json` & `swanlab-0.3.5/node_modules/gopd/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/graphemer/package.json` & `swanlab-0.3.5/node_modules/graphemer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/has/package.json` & `swanlab-0.3.5/node_modules/has/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/has-ansi/package.json` & `swanlab-0.3.5/node_modules/has-ansi/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/has-ansi/node_modules/ansi-regex/package.json` & `swanlab-0.3.5/node_modules/has-ansi/node_modules/ansi-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/has-bigints/package.json` & `swanlab-0.3.5/node_modules/has-bigints/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/has-flag/package.json` & `swanlab-0.3.5/node_modules/has-flag/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/has-property-descriptors/package.json` & `swanlab-0.3.5/node_modules/has-property-descriptors/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/has-proto/package.json` & `swanlab-0.3.5/node_modules/has-proto/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/has-proto/tsconfig.json` & `swanlab-0.3.5/node_modules/has-proto/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/has-symbols/package.json` & `swanlab-0.3.5/node_modules/has-symbols/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/has-tostringtag/package.json` & `swanlab-0.3.5/node_modules/has-tostringtag/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/has-tostringtag/tsconfig.json` & `swanlab-0.3.5/node_modules/has-tostringtag/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/hasown/package.json` & `swanlab-0.3.5/node_modules/hasown/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/html2canvas/package.json` & `swanlab-0.3.5/node_modules/html2canvas/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/html2canvas/tsconfig.json` & `swanlab-0.3.5/node_modules/html2canvas/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/human-signals/package.json` & `swanlab-0.3.5/node_modules/human-signals/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/husky/package.json` & `swanlab-0.3.5/node_modules/husky/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/ignore/package.json` & `swanlab-0.3.5/node_modules/ignore/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/immutable/package.json` & `swanlab-0.3.5/node_modules/immutable/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/import-fresh/package.json` & `swanlab-0.3.5/node_modules/import-fresh/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/imurmurhash/package.json` & `swanlab-0.3.5/node_modules/imurmurhash/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/inflight/package.json` & `swanlab-0.3.5/node_modules/inflight/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/inherits/package.json` & `swanlab-0.3.5/node_modules/inherits/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/internal-slot/package.json` & `swanlab-0.3.5/node_modules/internal-slot/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/is-arguments/package.json` & `swanlab-0.3.5/node_modules/is-arguments/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/is-array-buffer/package.json` & `swanlab-0.3.5/node_modules/is-array-buffer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/is-array-buffer/tsconfig.json` & `swanlab-0.3.5/node_modules/is-array-buffer/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/is-bigint/package.json` & `swanlab-0.3.5/node_modules/is-bigint/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/is-binary-path/package.json` & `swanlab-0.3.5/node_modules/is-binary-path/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/is-boolean-object/package.json` & `swanlab-0.3.5/node_modules/is-boolean-object/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/is-buffer/package.json` & `swanlab-0.3.5/node_modules/is-buffer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/is-callable/package.json` & `swanlab-0.3.5/node_modules/is-callable/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/is-core-module/core.json` & `swanlab-0.3.5/node_modules/is-core-module/core.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/is-core-module/package.json` & `swanlab-0.3.5/node_modules/is-core-module/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/is-data-view/package.json` & `swanlab-0.3.5/node_modules/is-data-view/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/is-data-view/tsconfig.json` & `swanlab-0.3.5/node_modules/is-data-view/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/is-date-object/package.json` & `swanlab-0.3.5/node_modules/is-date-object/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/is-extglob/package.json` & `swanlab-0.3.5/node_modules/is-extglob/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/is-fullwidth-code-point/package.json` & `swanlab-0.3.5/node_modules/is-fullwidth-code-point/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/is-glob/package.json` & `swanlab-0.3.5/node_modules/is-glob/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/is-negative-zero/package.json` & `swanlab-0.3.5/node_modules/is-negative-zero/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/is-negative-zero/tsconfig.json` & `swanlab-0.3.5/node_modules/is-negative-zero/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/is-number/package.json` & `swanlab-0.3.5/node_modules/is-number/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/is-number-object/package.json` & `swanlab-0.3.5/node_modules/is-number-object/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/is-path-inside/package.json` & `swanlab-0.3.5/node_modules/is-path-inside/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/is-regex/package.json` & `swanlab-0.3.5/node_modules/is-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/is-shared-array-buffer/package.json` & `swanlab-0.3.5/node_modules/is-shared-array-buffer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/is-shared-array-buffer/tsconfig.json` & `swanlab-0.3.5/node_modules/is-shared-array-buffer/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/is-stream/package.json` & `swanlab-0.3.5/node_modules/is-stream/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/is-string/package.json` & `swanlab-0.3.5/node_modules/is-string/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/is-symbol/package.json` & `swanlab-0.3.5/node_modules/is-symbol/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/is-typed-array/package.json` & `swanlab-0.3.5/node_modules/is-typed-array/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/is-typed-array/tsconfig.json` & `swanlab-0.3.5/node_modules/is-typed-array/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/is-weakref/package.json` & `swanlab-0.3.5/node_modules/is-weakref/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/isarray/package.json` & `swanlab-0.3.5/node_modules/isarray/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/isexe/package.json` & `swanlab-0.3.5/node_modules/isexe/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/jackspeak/package.json` & `swanlab-0.3.5/node_modules/jackspeak/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/jiti/package.json` & `swanlab-0.3.5/node_modules/jiti/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/js-yaml/package.json` & `swanlab-0.3.5/node_modules/js-yaml/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/json-buffer/package.json` & `swanlab-0.3.5/node_modules/json-buffer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/json-schema-traverse/package.json` & `swanlab-0.3.5/node_modules/json-schema-traverse/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/json-stable-stringify-without-jsonify/package.json` & `swanlab-0.3.5/node_modules/json-stable-stringify-without-jsonify/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/json2module/package.json` & `swanlab-0.3.5/node_modules/json2module/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/json5/package.json` & `swanlab-0.3.5/node_modules/json5/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/keyv/package.json` & `swanlab-0.3.5/node_modules/keyv/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/kind-of/package.json` & `swanlab-0.3.5/node_modules/kind-of/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/lazy-cache/package.json` & `swanlab-0.3.5/node_modules/lazy-cache/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/levn/package.json` & `swanlab-0.3.5/node_modules/levn/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/lilconfig/package.json` & `swanlab-0.3.5/node_modules/lilconfig/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/lines-and-columns/package.json` & `swanlab-0.3.5/node_modules/lines-and-columns/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/local-pkg/package.json` & `swanlab-0.3.5/node_modules/local-pkg/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/locate-path/package.json` & `swanlab-0.3.5/node_modules/locate-path/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/lodash/package.json` & `swanlab-0.3.5/node_modules/lodash/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/lodash-es/package.json` & `swanlab-0.3.5/node_modules/lodash-es/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/lodash.merge/package.json` & `swanlab-0.3.5/node_modules/lodash.merge/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/longest/package.json` & `swanlab-0.3.5/node_modules/longest/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/loupe/package.json` & `swanlab-0.3.5/node_modules/loupe/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/lru-cache/package.json` & `swanlab-0.3.5/node_modules/lru-cache/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/magic-string/package.json` & `swanlab-0.3.5/node_modules/magic-string/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/merge2/package.json` & `swanlab-0.3.5/node_modules/merge2/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/micromatch/package.json` & `swanlab-0.3.5/node_modules/micromatch/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/mime-db/db.json` & `swanlab-0.3.5/node_modules/mime-db/db.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/mime-db/package.json` & `swanlab-0.3.5/node_modules/mime-db/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/mime-types/package.json` & `swanlab-0.3.5/node_modules/mime-types/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/mimic-fn/package.json` & `swanlab-0.3.5/node_modules/mimic-fn/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/minimatch/package.json` & `swanlab-0.3.5/node_modules/minimatch/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/minimist/package.json` & `swanlab-0.3.5/node_modules/minimist/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/minipass/package.json` & `swanlab-0.3.5/node_modules/minipass/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/mlly/package.json` & `swanlab-0.3.5/node_modules/mlly/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/mock-property/package.json` & `swanlab-0.3.5/node_modules/mock-property/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/mockjs/package.json` & `swanlab-0.3.5/node_modules/mockjs/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/moment/package.json` & `swanlab-0.3.5/node_modules/moment/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/ms/package.json` & `swanlab-0.3.5/node_modules/ms/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/mz/package.json` & `swanlab-0.3.5/node_modules/mz/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/nanoid/package.json` & `swanlab-0.3.5/node_modules/nanoid/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/natural-compare/package.json` & `swanlab-0.3.5/node_modules/natural-compare/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/node-releases/data/processed/envs.json` & `swanlab-0.3.5/node_modules/node-releases/data/processed/envs.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/node-releases/data/release-schedule/release-schedule.json` & `swanlab-0.3.5/node_modules/node-releases/data/release-schedule/release-schedule.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/normalize-path/package.json` & `swanlab-0.3.5/node_modules/normalize-path/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/normalize-range/package.json` & `swanlab-0.3.5/node_modules/normalize-range/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/npm-run-path/package.json` & `swanlab-0.3.5/node_modules/npm-run-path/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/npm-run-path/node_modules/path-key/package.json` & `swanlab-0.3.5/node_modules/npm-run-path/node_modules/path-key/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/nth-check/package.json` & `swanlab-0.3.5/node_modules/nth-check/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/object-assign/package.json` & `swanlab-0.3.5/node_modules/object-assign/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/object-hash/package.json` & `swanlab-0.3.5/node_modules/object-hash/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/object-inspect/package.json` & `swanlab-0.3.5/node_modules/object-inspect/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/object-is/package.json` & `swanlab-0.3.5/node_modules/object-is/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/object-keys/package.json` & `swanlab-0.3.5/node_modules/object-keys/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/object.assign/package.json` & `swanlab-0.3.5/node_modules/object.assign/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/once/package.json` & `swanlab-0.3.5/node_modules/once/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/onetime/package.json` & `swanlab-0.3.5/node_modules/onetime/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/optionator/package.json` & `swanlab-0.3.5/node_modules/optionator/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/p-limit/package.json` & `swanlab-0.3.5/node_modules/p-limit/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/p-locate/package.json` & `swanlab-0.3.5/node_modules/p-locate/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/parent-module/package.json` & `swanlab-0.3.5/node_modules/parent-module/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/path-exists/package.json` & `swanlab-0.3.5/node_modules/path-exists/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/path-is-absolute/package.json` & `swanlab-0.3.5/node_modules/path-is-absolute/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/path-key/package.json` & `swanlab-0.3.5/node_modules/path-key/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/path-parse/package.json` & `swanlab-0.3.5/node_modules/path-parse/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/path-scurry/package.json` & `swanlab-0.3.5/node_modules/path-scurry/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/pathe/package.json` & `swanlab-0.3.5/node_modules/pathe/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/pathval/package.json` & `swanlab-0.3.5/node_modules/pathval/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/pdfast/package.json` & `swanlab-0.3.5/node_modules/pdfast/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/picocolors/package.json` & `swanlab-0.3.5/node_modules/picocolors/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/picomatch/package.json` & `swanlab-0.3.5/node_modules/picomatch/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/pify/package.json` & `swanlab-0.3.5/node_modules/pify/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/pinia/package.json` & `swanlab-0.3.5/node_modules/pinia/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/pinia/node_modules/vue-demi/package.json` & `swanlab-0.3.5/node_modules/pinia/node_modules/vue-demi/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/pirates/package.json` & `swanlab-0.3.5/node_modules/pirates/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/pkg-types/package.json` & `swanlab-0.3.5/node_modules/pkg-types/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/possible-typed-array-names/package.json` & `swanlab-0.3.5/node_modules/possible-typed-array-names/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/possible-typed-array-names/tsconfig.json` & `swanlab-0.3.5/node_modules/possible-typed-array-names/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/postcss/package.json` & `swanlab-0.3.5/node_modules/postcss/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/postcss-import/package.json` & `swanlab-0.3.5/node_modules/postcss-import/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/postcss-js/package.json` & `swanlab-0.3.5/node_modules/postcss-js/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/postcss-load-config/package.json` & `swanlab-0.3.5/node_modules/postcss-load-config/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/postcss-load-config/node_modules/lilconfig/package.json` & `swanlab-0.3.5/node_modules/postcss-load-config/node_modules/lilconfig/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/postcss-nested/package.json` & `swanlab-0.3.5/node_modules/postcss-nested/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/postcss-selector-parser/package.json` & `swanlab-0.3.5/node_modules/postcss-selector-parser/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/postcss-value-parser/package.json` & `swanlab-0.3.5/node_modules/postcss-value-parser/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/prelude-ls/package.json` & `swanlab-0.3.5/node_modules/prelude-ls/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/prettier-linter-helpers/package.json` & `swanlab-0.3.5/node_modules/prettier-linter-helpers/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/pretty-format/package.json` & `swanlab-0.3.5/node_modules/pretty-format/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/pretty-format/node_modules/ansi-styles/package.json` & `swanlab-0.3.5/node_modules/pretty-format/node_modules/ansi-styles/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/proxy-from-env/package.json` & `swanlab-0.3.5/node_modules/proxy-from-env/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/punycode/package.json` & `swanlab-0.3.5/node_modules/punycode/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/queue-microtask/package.json` & `swanlab-0.3.5/node_modules/queue-microtask/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/read-cache/package.json` & `swanlab-0.3.5/node_modules/read-cache/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/readdirp/package.json` & `swanlab-0.3.5/node_modules/readdirp/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/regexp.prototype.flags/package.json` & `swanlab-0.3.5/node_modules/regexp.prototype.flags/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/repeat-string/package.json` & `swanlab-0.3.5/node_modules/repeat-string/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/resolve/package.json` & `swanlab-0.3.5/node_modules/resolve/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/resolve/lib/core.json` & `swanlab-0.3.5/node_modules/resolve/lib/core.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/resolve-from/package.json` & `swanlab-0.3.5/node_modules/resolve-from/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/reusify/package.json` & `swanlab-0.3.5/node_modules/reusify/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/right-align/package.json` & `swanlab-0.3.5/node_modules/right-align/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/rimraf/package.json` & `swanlab-0.3.5/node_modules/rimraf/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/rollup/package.json` & `swanlab-0.3.5/node_modules/rollup/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/rollup/node_modules/ansi-regex/package.json` & `swanlab-0.3.5/node_modules/rollup/node_modules/ansi-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/rollup/node_modules/ansi-styles/package.json` & `swanlab-0.3.5/node_modules/rollup/node_modules/ansi-styles/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/rollup/node_modules/chalk/package.json` & `swanlab-0.3.5/node_modules/rollup/node_modules/chalk/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/rollup/node_modules/escape-string-regexp/package.json` & `swanlab-0.3.5/node_modules/rollup/node_modules/escape-string-regexp/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/rollup/node_modules/strip-ansi/package.json` & `swanlab-0.3.5/node_modules/rollup/node_modules/strip-ansi/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/rollup/node_modules/supports-color/package.json` & `swanlab-0.3.5/node_modules/rollup/node_modules/supports-color/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/run-parallel/package.json` & `swanlab-0.3.5/node_modules/run-parallel/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/rw/package.json` & `swanlab-0.3.5/node_modules/rw/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/safe-array-concat/package.json` & `swanlab-0.3.5/node_modules/safe-array-concat/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/safe-regex-test/package.json` & `swanlab-0.3.5/node_modules/safe-regex-test/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/sass/package.json` & `swanlab-0.3.5/node_modules/sass/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/scule/package.json` & `swanlab-0.3.5/node_modules/scule/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/semver/package.json` & `swanlab-0.3.5/node_modules/semver/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/set-function-length/package.json` & `swanlab-0.3.5/node_modules/set-function-length/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/set-function-name/package.json` & `swanlab-0.3.5/node_modules/set-function-name/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/set-function-name/tsconfig.json` & `swanlab-0.3.5/node_modules/set-function-name/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/shebang-command/package.json` & `swanlab-0.3.5/node_modules/shebang-command/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/shebang-regex/package.json` & `swanlab-0.3.5/node_modules/shebang-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/side-channel/package.json` & `swanlab-0.3.5/node_modules/side-channel/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/side-channel/tsconfig.json` & `swanlab-0.3.5/node_modules/side-channel/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/side-channel/node_modules/object-inspect/package.json` & `swanlab-0.3.5/node_modules/side-channel/node_modules/object-inspect/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/siginfo/package.json` & `swanlab-0.3.5/node_modules/siginfo/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/signal-exit/package.json` & `swanlab-0.3.5/node_modules/signal-exit/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/size-sensor/package.json` & `swanlab-0.3.5/node_modules/size-sensor/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/source-map/package.json` & `swanlab-0.3.5/node_modules/source-map/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/source-map-js/package.json` & `swanlab-0.3.5/node_modules/source-map-js/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/source-map-support/package.json` & `swanlab-0.3.5/node_modules/source-map-support/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/std-env/package.json` & `swanlab-0.3.5/node_modules/std-env/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/string-width/package.json` & `swanlab-0.3.5/node_modules/string-width/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/string-width/node_modules/ansi-regex/package.json` & `swanlab-0.3.5/node_modules/string-width/node_modules/ansi-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/string-width/node_modules/strip-ansi/package.json` & `swanlab-0.3.5/node_modules/string-width/node_modules/strip-ansi/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/string-width-cjs/package.json` & `swanlab-0.3.5/node_modules/string-width-cjs/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/string-width-cjs/node_modules/emoji-regex/package.json` & `swanlab-0.3.5/node_modules/string-width-cjs/node_modules/emoji-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/string.prototype.trim/package.json` & `swanlab-0.3.5/node_modules/string.prototype.trim/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/string.prototype.trimend/package.json` & `swanlab-0.3.5/node_modules/string.prototype.trimend/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/string.prototype.trimstart/package.json` & `swanlab-0.3.5/node_modules/string.prototype.trimstart/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/strip-ansi/package.json` & `swanlab-0.3.5/node_modules/strip-ansi/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/strip-ansi-cjs/package.json` & `swanlab-0.3.5/node_modules/strip-ansi-cjs/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/strip-final-newline/package.json` & `swanlab-0.3.5/node_modules/strip-final-newline/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/strip-json-comments/package.json` & `swanlab-0.3.5/node_modules/strip-json-comments/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/strip-literal/package.json` & `swanlab-0.3.5/node_modules/strip-literal/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/sucrase/package.json` & `swanlab-0.3.5/node_modules/sucrase/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/sucrase/node_modules/brace-expansion/package.json` & `swanlab-0.3.5/node_modules/sucrase/node_modules/brace-expansion/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/sucrase/node_modules/commander/package.json` & `swanlab-0.3.5/node_modules/sucrase/node_modules/commander/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/sucrase/node_modules/glob/package.json` & `swanlab-0.3.5/node_modules/sucrase/node_modules/glob/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/sucrase/node_modules/minimatch/package.json` & `swanlab-0.3.5/node_modules/sucrase/node_modules/minimatch/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/supports-color/package.json` & `swanlab-0.3.5/node_modules/supports-color/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/supports-preserve-symlinks-flag/package.json` & `swanlab-0.3.5/node_modules/supports-preserve-symlinks-flag/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/tailwindcss/package.json` & `swanlab-0.3.5/node_modules/tailwindcss/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/tape/package.json` & `swanlab-0.3.5/node_modules/tape/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/terser/package.json` & `swanlab-0.3.5/node_modules/terser/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/terser/node_modules/commander/package.json` & `swanlab-0.3.5/node_modules/terser/node_modules/commander/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/terser/node_modules/source-map/package.json` & `swanlab-0.3.5/node_modules/terser/node_modules/source-map/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/terser/node_modules/source-map-support/package.json` & `swanlab-0.3.5/node_modules/terser/node_modules/source-map-support/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/text-segmentation/package.json` & `swanlab-0.3.5/node_modules/text-segmentation/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/text-table/package.json` & `swanlab-0.3.5/node_modules/text-table/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/thenify/package.json` & `swanlab-0.3.5/node_modules/thenify/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/thenify-all/package.json` & `swanlab-0.3.5/node_modules/thenify-all/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/tinybench/package.json` & `swanlab-0.3.5/node_modules/tinybench/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/tinypool/package.json` & `swanlab-0.3.5/node_modules/tinypool/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/tinyspy/package.json` & `swanlab-0.3.5/node_modules/tinyspy/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/tippy.js/package.json` & `swanlab-0.3.5/node_modules/tippy.js/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/to-regex-range/package.json` & `swanlab-0.3.5/node_modules/to-regex-range/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/ts-interface-checker/package.json` & `swanlab-0.3.5/node_modules/ts-interface-checker/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/tslib/package.json` & `swanlab-0.3.5/node_modules/tslib/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/type-check/package.json` & `swanlab-0.3.5/node_modules/type-check/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/type-detect/package.json` & `swanlab-0.3.5/node_modules/type-detect/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/type-fest/package.json` & `swanlab-0.3.5/node_modules/type-fest/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/typed-array-buffer/package.json` & `swanlab-0.3.5/node_modules/typed-array-buffer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/typed-array-buffer/tsconfig.json` & `swanlab-0.3.5/node_modules/typed-array-buffer/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/typed-array-byte-length/package.json` & `swanlab-0.3.5/node_modules/typed-array-byte-length/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/typed-array-byte-length/tsconfig.json` & `swanlab-0.3.5/node_modules/typed-array-byte-length/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/typed-array-byte-offset/package.json` & `swanlab-0.3.5/node_modules/typed-array-byte-offset/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/typed-array-byte-offset/tsconfig.json` & `swanlab-0.3.5/node_modules/typed-array-byte-offset/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/typed-array-length/package.json` & `swanlab-0.3.5/node_modules/typed-array-length/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/ufo/package.json` & `swanlab-0.3.5/node_modules/ufo/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/uglify-js/package.json` & `swanlab-0.3.5/node_modules/uglify-js/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/uglify-js/node_modules/source-map/package.json` & `swanlab-0.3.5/node_modules/uglify-js/node_modules/source-map/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/uglify-js/tools/domprops.json` & `swanlab-0.3.5/node_modules/uglify-js/tools/domprops.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/unbox-primitive/package.json` & `swanlab-0.3.5/node_modules/unbox-primitive/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/unimport/package.json` & `swanlab-0.3.5/node_modules/unimport/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/unimport/node_modules/escape-string-regexp/package.json` & `swanlab-0.3.5/node_modules/unimport/node_modules/escape-string-regexp/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/unimport/node_modules/estree-walker/package.json` & `swanlab-0.3.5/node_modules/unimport/node_modules/estree-walker/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/unimport/node_modules/local-pkg/package.json` & `swanlab-0.3.5/node_modules/unimport/node_modules/local-pkg/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/unplugin/package.json` & `swanlab-0.3.5/node_modules/unplugin/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/unplugin-auto-import/package.json` & `swanlab-0.3.5/node_modules/unplugin-auto-import/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/unplugin-auto-import/node_modules/brace-expansion/package.json` & `swanlab-0.3.5/node_modules/unplugin-auto-import/node_modules/brace-expansion/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/unplugin-auto-import/node_modules/minimatch/package.json` & `swanlab-0.3.5/node_modules/unplugin-auto-import/node_modules/minimatch/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/unplugin-vue-components/package.json` & `swanlab-0.3.5/node_modules/unplugin-vue-components/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/unplugin-vue-components/node_modules/brace-expansion/package.json` & `swanlab-0.3.5/node_modules/unplugin-vue-components/node_modules/brace-expansion/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/unplugin-vue-components/node_modules/minimatch/package.json` & `swanlab-0.3.5/node_modules/unplugin-vue-components/node_modules/minimatch/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/update-browserslist-db/.devcontainer.json` & `swanlab-0.3.5/node_modules/update-browserslist-db/.devcontainer.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/update-browserslist-db/package.json` & `swanlab-0.3.5/node_modules/update-browserslist-db/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/uri-js/package.json` & `swanlab-0.3.5/node_modules/uri-js/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/util-deprecate/package.json` & `swanlab-0.3.5/node_modules/util-deprecate/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/utrie/package.json` & `swanlab-0.3.5/node_modules/utrie/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/vite/package.json` & `swanlab-0.3.5/node_modules/vite/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/vite/node_modules/rollup/package.json` & `swanlab-0.3.5/node_modules/vite/node_modules/rollup/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/vite-node/package.json` & `swanlab-0.3.5/node_modules/vite-node/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/vite-plugin-json5/package.json` & `swanlab-0.3.5/node_modules/vite-plugin-json5/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/vitest/package.json` & `swanlab-0.3.5/node_modules/vitest/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/vitest/node_modules/local-pkg/package.json` & `swanlab-0.3.5/node_modules/vitest/node_modules/local-pkg/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/vue/package.json` & `swanlab-0.3.5/node_modules/vue/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/vue-eslint-parser/package.json` & `swanlab-0.3.5/node_modules/vue-eslint-parser/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/vue-i18n/package.json` & `swanlab-0.3.5/node_modules/vue-i18n/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/vue-i18n/vetur/attributes.json` & `swanlab-0.3.5/node_modules/vue-i18n/vetur/attributes.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/vue-i18n/vetur/tags.json` & `swanlab-0.3.5/node_modules/vue-i18n/vetur/tags.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/vue-router/package.json` & `swanlab-0.3.5/node_modules/vue-router/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/vue-router/vetur/attributes.json` & `swanlab-0.3.5/node_modules/vue-router/vetur/attributes.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/vue-router/vetur/tags.json` & `swanlab-0.3.5/node_modules/vue-router/vetur/tags.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/vue-tippy/package.json` & `swanlab-0.3.5/node_modules/vue-tippy/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/vue-tippy/tsconfig.json` & `swanlab-0.3.5/node_modules/vue-tippy/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/vue-tippy/vetur/attributes.json` & `swanlab-0.3.5/node_modules/vue-tippy/vetur/attributes.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/vue-tippy/vetur/tags.json` & `swanlab-0.3.5/node_modules/vue-tippy/vetur/tags.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/webpack-sources/package.json` & `swanlab-0.3.5/node_modules/webpack-sources/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/webpack-virtual-modules/package.json` & `swanlab-0.3.5/node_modules/webpack-virtual-modules/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/which/package.json` & `swanlab-0.3.5/node_modules/which/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/which-boxed-primitive/package.json` & `swanlab-0.3.5/node_modules/which-boxed-primitive/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/which-typed-array/package.json` & `swanlab-0.3.5/node_modules/which-typed-array/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/why-is-node-running/package.json` & `swanlab-0.3.5/node_modules/why-is-node-running/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/window-size/package.json` & `swanlab-0.3.5/node_modules/window-size/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/word-wrap/package.json` & `swanlab-0.3.5/node_modules/word-wrap/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/wordwrap/package.json` & `swanlab-0.3.5/node_modules/wordwrap/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/wrap-ansi/package.json` & `swanlab-0.3.5/node_modules/wrap-ansi/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/wrap-ansi/node_modules/ansi-regex/package.json` & `swanlab-0.3.5/node_modules/wrap-ansi/node_modules/ansi-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/wrap-ansi/node_modules/ansi-styles/package.json` & `swanlab-0.3.5/node_modules/wrap-ansi/node_modules/ansi-styles/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/wrap-ansi/node_modules/strip-ansi/package.json` & `swanlab-0.3.5/node_modules/wrap-ansi/node_modules/strip-ansi/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/wrap-ansi-cjs/package.json` & `swanlab-0.3.5/node_modules/wrap-ansi-cjs/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/wrap-ansi-cjs/node_modules/emoji-regex/package.json` & `swanlab-0.3.5/node_modules/wrap-ansi-cjs/node_modules/emoji-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/wrap-ansi-cjs/node_modules/string-width/package.json` & `swanlab-0.3.5/node_modules/wrap-ansi-cjs/node_modules/string-width/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/wrappy/package.json` & `swanlab-0.3.5/node_modules/wrappy/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/xml-name-validator/package.json` & `swanlab-0.3.5/node_modules/xml-name-validator/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/yaml/package.json` & `swanlab-0.3.5/node_modules/yaml/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/yargs/package.json` & `swanlab-0.3.5/node_modules/yargs/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/node_modules/yocto-queue/package.json` & `swanlab-0.3.5/node_modules/yocto-queue/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/env.py` & `swanlab-0.3.5/swanlab/env.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/error.py` & `swanlab-0.3.5/swanlab/error.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/package.py` & `swanlab-0.3.5/swanlab/package.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/api/cos.py` & `swanlab-0.3.5/swanlab/api/cos.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/api/http.py` & `swanlab-0.3.5/swanlab/api/http.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/api/info.py` & `swanlab-0.3.5/swanlab/api/info.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/api/auth/login.py` & `swanlab-0.3.5/swanlab/api/auth/login.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/api/upload/__init__.py` & `swanlab-0.3.5/swanlab/api/upload/__init__.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/api/upload/model.py` & `swanlab-0.3.5/swanlab/api/upload/model.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/cli/main.py` & `swanlab-0.3.5/swanlab/cli/main.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/cli/utils.py` & `swanlab-0.3.5/swanlab/cli/utils.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/cloud/_log_collector.py` & `swanlab-0.3.5/swanlab/cloud/_log_collector.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/cloud/start_thread.py` & `swanlab-0.3.5/swanlab/cloud/start_thread.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/cloud/task_types.py` & `swanlab-0.3.5/swanlab/cloud/task_types.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/cloud/utils.py` & `swanlab-0.3.5/swanlab/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/cloud/dog/log_sniffer.py` & `swanlab-0.3.5/swanlab/cloud/dog/log_sniffer.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/cloud/dog/metadata_handle.py` & `swanlab-0.3.5/swanlab/cloud/dog/metadata_handle.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/cloud/dog/sniffer_queue.py` & `swanlab-0.3.5/swanlab/cloud/dog/sniffer_queue.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/compat/server/controller/experiment.py` & `swanlab-0.3.5/swanlab/compat/server/controller/experiment.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/converter/tfb/_utils.py` & `swanlab-0.3.5/swanlab/converter/tfb/_utils.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/converter/tfb/tfb_converter.py` & `swanlab-0.3.5/swanlab/converter/tfb/tfb_converter.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/converter/wb/wb_converter.py` & `swanlab-0.3.5/swanlab/converter/wb/wb_converter.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/data/__init__.py` & `swanlab-0.3.5/swanlab/data/__init__.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/data/callback_cloud.py` & `swanlab-0.3.5/swanlab/data/callback_cloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,15 @@
         if self.login_info is None:
             swanlog.debug("Login info is None, get login info.")
             self.login_info = self.get_login_info()
         http = create_http(self.login_info)
         return http.mount_project(project, workspace).history_exp_count
 
     def on_run(self):
+        swanlog.install(self.settings.console_dir)
         # 注册实验信息
         try:
             get_http().mount_exp(
                 exp_name=self.settings.exp_name,
                 colors=self.settings.exp_colors,
                 description=self.settings.description,
             )
```

### Comparing `swanlab-0.3.4/swanlab/data/callback_local.py` & `swanlab-0.3.5/swanlab/data/callback_local.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/data/config.py` & `swanlab-0.3.5/swanlab/data/config.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/data/sdk.py` & `swanlab-0.3.5/swanlab/data/sdk.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/data/settings.py` & `swanlab-0.3.5/swanlab/data/settings.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/data/modules/_utils.py` & `swanlab-0.3.5/swanlab/data/modules/_utils.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/data/modules/audio.py` & `swanlab-0.3.5/swanlab/data/modules/audio.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/data/modules/base.py` & `swanlab-0.3.5/swanlab/data/modules/base.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/data/modules/chart.py` & `swanlab-0.3.5/swanlab/data/modules/chart.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/data/modules/image.py` & `swanlab-0.3.5/swanlab/data/modules/image.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/data/modules/object_3d.py` & `swanlab-0.3.5/swanlab/data/modules/object_3d.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/data/modules/text.py` & `swanlab-0.3.5/swanlab/data/modules/text.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/data/modules/video.py` & `swanlab-0.3.5/swanlab/data/modules/video.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/data/modules/utils_modules/bounding_boxes.py` & `swanlab-0.3.5/swanlab/data/modules/utils_modules/bounding_boxes.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/data/modules/utils_modules/image_mask.py` & `swanlab-0.3.5/swanlab/data/modules/utils_modules/image_mask.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/data/run/callback.py` & `swanlab-0.3.5/swanlab/data/run/callback.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/data/run/exp.py` & `swanlab-0.3.5/swanlab/data/run/exp.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/data/run/main.py` & `swanlab-0.3.5/swanlab/data/run/main.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/data/run/operator.py` & `swanlab-0.3.5/swanlab/data/run/operator.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/data/system/info.py` & `swanlab-0.3.5/swanlab/data/system/info.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/data/system/monitor.py` & `swanlab-0.3.5/swanlab/data/system/monitor.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/data/system/bin/apple_gpu_stats` & `swanlab-0.3.5/swanlab/data/system/bin/apple_gpu_stats`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/db/__init__.py` & `swanlab-0.3.5/swanlab/db/__init__.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/db/callback.py` & `swanlab-0.3.5/swanlab/db/callback.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/db/db_connect.py` & `swanlab-0.3.5/swanlab/db/db_connect.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/db/error.py` & `swanlab-0.3.5/swanlab/db/error.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/db/model.py` & `swanlab-0.3.5/swanlab/db/model.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/db/docs/Errors.md` & `swanlab-0.3.5/swanlab/db/docs/Errors.md`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/db/docs/README.md` & `swanlab-0.3.5/swanlab/db/docs/README.md`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/db/migrate/chart.py` & `swanlab-0.3.5/swanlab/db/migrate/chart.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/db/migrate/experiment.py` & `swanlab-0.3.5/swanlab/db/migrate/experiment.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/db/migrate/namespace.py` & `swanlab-0.3.5/swanlab/db/migrate/namespace.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/db/migrate/project.py` & `swanlab-0.3.5/swanlab/db/migrate/project.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/db/models/charts.py` & `swanlab-0.3.5/swanlab/db/models/charts.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/db/models/displays.py` & `swanlab-0.3.5/swanlab/db/models/displays.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/db/models/experiments.py` & `swanlab-0.3.5/swanlab/db/models/experiments.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/db/models/namespaces.py` & `swanlab-0.3.5/swanlab/db/models/namespaces.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/db/models/projects.py` & `swanlab-0.3.5/swanlab/db/models/projects.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/db/models/sources.py` & `swanlab-0.3.5/swanlab/db/models/sources.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/db/models/tags.py` & `swanlab-0.3.5/swanlab/db/models/tags.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/db/utils/chart.py` & `swanlab-0.3.5/swanlab/db/utils/chart.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/integration/fastai.py` & `swanlab-0.3.5/swanlab/integration/fastai.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/integration/huggingface.py` & `swanlab-0.3.5/swanlab/integration/huggingface.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/integration/mmengine.py` & `swanlab-0.3.5/swanlab/integration/mmengine.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/integration/pytorch_lightning.py` & `swanlab-0.3.5/swanlab/integration/pytorch_lightning.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/integration/sb3.py` & `swanlab-0.3.5/swanlab/integration/sb3.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/integration/ultralytics.py` & `swanlab-0.3.5/swanlab/integration/ultralytics.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/integration/integration_utils/autologging.py` & `swanlab-0.3.5/swanlab/integration/integration_utils/autologging.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/integration/integration_utils/get_modules.py` & `swanlab-0.3.5/swanlab/integration/integration_utils/get_modules.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/integration/integration_utils/timer.py` & `swanlab-0.3.5/swanlab/integration/integration_utils/timer.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/integration/openai/openai.py` & `swanlab-0.3.5/swanlab/integration/openai/openai.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/integration/openai/resolver.py` & `swanlab-0.3.5/swanlab/integration/openai/resolver.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/integration/zhipuai/resolver.py` & `swanlab-0.3.5/swanlab/integration/zhipuai/resolver.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/integration/zhipuai/zhipuai.py` & `swanlab-0.3.5/swanlab/integration/zhipuai/zhipuai.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/log/console.py` & `swanlab-0.3.5/swanlab/log/console.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/log/log.py` & `swanlab-0.3.5/swanlab/log/log.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/server/app.py` & `swanlab-0.3.5/swanlab/server/app.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/server/settings.py` & `swanlab-0.3.5/swanlab/server/settings.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/server/controller/chart.py` & `swanlab-0.3.5/swanlab/server/controller/chart.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/server/controller/experiment.py` & `swanlab-0.3.5/swanlab/server/controller/experiment.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/server/controller/namespace.py` & `swanlab-0.3.5/swanlab/server/controller/namespace.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/server/controller/project.py` & `swanlab-0.3.5/swanlab/server/controller/project.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/server/controller/utils/__init__.py` & `swanlab-0.3.5/swanlab/server/controller/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/server/controller/utils/charts.py` & `swanlab-0.3.5/swanlab/server/controller/utils/charts.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/server/controller/utils/tag.py` & `swanlab-0.3.5/swanlab/server/controller/utils/tag.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/server/middleware/common.py` & `swanlab-0.3.5/swanlab/server/middleware/common.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/server/module/resp.py` & `swanlab-0.3.5/swanlab/server/module/resp.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/server/router/chart.py` & `swanlab-0.3.5/swanlab/server/router/chart.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/server/router/experiment.py` & `swanlab-0.3.5/swanlab/server/router/experiment.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/server/router/media.py` & `swanlab-0.3.5/swanlab/server/router/media.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/server/router/namespace.py` & `swanlab-0.3.5/swanlab/server/router/namespace.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/server/router/project.py` & `swanlab-0.3.5/swanlab/server/router/project.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/template/assets/ChartPage-C2Rj7xI3.js` & `swanlab-0.3.5/swanlab/template/assets/ChartPage-C2Rj7xI3.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/template/assets/ChartsView-DpI6U3QH.js` & `swanlab-0.3.5/swanlab/template/assets/ChartsView-DpI6U3QH.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/template/assets/EnvHardware-4H7mp2Bs.js` & `swanlab-0.3.5/swanlab/template/assets/EnvHardware-4H7mp2Bs.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/template/assets/EnvIndex-B5_l1b65.js` & `swanlab-0.3.5/swanlab/template/assets/EnvIndex-B5_l1b65.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/template/assets/EnvItems-B4PwmQT4.js` & `swanlab-0.3.5/swanlab/template/assets/EnvItems-B4PwmQT4.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/template/assets/EnvItems-BfjcRO-X.css` & `swanlab-0.3.5/swanlab/template/assets/EnvItems-BfjcRO-X.css`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/template/assets/EnvRequirements-Cpn2Fk1D.js` & `swanlab-0.3.5/swanlab/template/assets/EnvRequirements-Cpn2Fk1D.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/template/assets/EnvironmentPage-Bb8ousXq.js` & `swanlab-0.3.5/swanlab/template/assets/EnvironmentPage-Bb8ousXq.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/template/assets/ExperimentView-BTbu21ka.js` & `swanlab-0.3.5/swanlab/template/assets/ExperimentView-BTbu21ka.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/template/assets/ExperimentView-CCDMXo4h.css` & `swanlab-0.3.5/swanlab/template/assets/ExperimentView-CCDMXo4h.css`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/template/assets/FuncBar-Ct_nBdvU.js` & `swanlab-0.3.5/swanlab/template/assets/FuncBar-Ct_nBdvU.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/template/assets/HomeView-BS7FyMAt.css` & `swanlab-0.3.5/swanlab/template/assets/HomeView-BS7FyMAt.css`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/template/assets/HomeView-BqTu9_fG.js` & `swanlab-0.3.5/swanlab/template/assets/HomeView-BqTu9_fG.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/template/assets/IndexPage-C5dvtib2.css` & `swanlab-0.3.5/swanlab/template/assets/IndexPage-C5dvtib2.css`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/template/assets/IndexPage-CrqN4Ekl.js` & `swanlab-0.3.5/swanlab/template/assets/IndexPage-CrqN4Ekl.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/template/assets/JetBrainsMono-Regular-Dh36KTnx.ttf` & `swanlab-0.3.5/swanlab/template/assets/JetBrainsMono-Regular-Dh36KTnx.ttf`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/template/assets/LogPage-B-fC6sB7.js` & `swanlab-0.3.5/swanlab/template/assets/LogPage-B-fC6sB7.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/template/assets/LogPage-DBzoauOW.css` & `swanlab-0.3.5/swanlab/template/assets/LogPage-DBzoauOW.css`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/template/assets/NotFound-DijsQ96i.js` & `swanlab-0.3.5/swanlab/template/assets/NotFound-DijsQ96i.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/template/assets/SLLoading-6DfF2aH0.js` & `swanlab-0.3.5/swanlab/template/assets/SLLoading-6DfF2aH0.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/template/assets/SLStatusLabel-BRacn5XK.css` & `swanlab-0.3.5/swanlab/template/assets/SLStatusLabel-BRacn5XK.css`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/template/assets/SLStatusLabel-DvEKZN8v.js` & `swanlab-0.3.5/swanlab/template/assets/SLStatusLabel-DvEKZN8v.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/template/assets/SourceSansPro-Regular-J3NOkSfZ.ttf` & `swanlab-0.3.5/swanlab/template/assets/SourceSansPro-Regular-J3NOkSfZ.ttf`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/template/assets/chart-DB312WPs.css` & `swanlab-0.3.5/swanlab/template/assets/chart-DB312WPs.css`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/template/assets/chart-eW1meEc1.js` & `swanlab-0.3.5/swanlab/template/assets/chart-eW1meEc1.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/template/assets/index-B5SDzoY4.js` & `swanlab-0.3.5/swanlab/template/assets/index-B5SDzoY4.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/template/assets/index-B7Izi8NT.css` & `swanlab-0.3.5/swanlab/template/assets/index-B7Izi8NT.css`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/template/assets/logo-ChHf2ozk.ico` & `swanlab-0.3.5/swanlab/template/assets/logo-ChHf2ozk.ico`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/utils/file.py` & `swanlab-0.3.5/swanlab/utils/file.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/utils/font.py` & `swanlab-0.3.5/swanlab/utils/font.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/utils/judgment.py` & `swanlab-0.3.5/swanlab/utils/judgment.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/swanlab/utils/key.py` & `swanlab-0.3.5/swanlab/utils/key.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/test/create_experiment.py` & `swanlab-0.3.5/test/create_experiment.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/test/start_server.py` & `swanlab-0.3.5/test/start_server.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/test/use_swanlog.py` & `swanlab-0.3.5/test/use_swanlog.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/test/integration/README.md` & `swanlab-0.3.5/test/integration/README.md`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/test/integration/fastai/fastai_train.py` & `swanlab-0.3.5/test/integration/fastai/fastai_train.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/test/integration/huggingface/transformers_bert_train.py` & `swanlab-0.3.5/test/integration/huggingface/transformers_bert_train.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/test/integration/lightning/lightning_base.py` & `swanlab-0.3.5/test/integration/lightning/lightning_base.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/test/integration/lightning/lightning_train.py` & `swanlab-0.3.5/test/integration/lightning/lightning_train.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/test/integration/sb3/sb3_PPO.py` & `swanlab-0.3.5/test/integration/sb3/sb3_PPO.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/test/unit/pytest_env.py` & `swanlab-0.3.5/test/unit/pytest_env.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/test/unit/pytest_example.py` & `swanlab-0.3.5/test/unit/pytest_example.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/test/unit/auth/pytest_login.py` & `swanlab-0.3.5/test/unit/auth/pytest_login.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/test/unit/data/pytest_sdk.py` & `swanlab-0.3.5/test/unit/data/pytest_sdk.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/test/unit/data/run/pytest_main.py` & `swanlab-0.3.5/test/unit/data/run/pytest_main.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/test/unit/log/pytest_log.py` & `swanlab-0.3.5/test/unit/log/pytest_log.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/test/unit/server/controller/utils/utils.py` & `swanlab-0.3.5/test/unit/server/controller/utils/utils.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/test/unit/utils/pytest_file.py` & `swanlab-0.3.5/test/unit/utils/pytest_file.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/test/unit/utils/pytest_key.py` & `swanlab-0.3.5/test/unit/utils/pytest_key.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/test/unit/utils/pytest_package.py` & `swanlab-0.3.5/test/unit/utils/pytest_package.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/LICENSE` & `swanlab-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/pyproject.toml` & `swanlab-0.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.4/PKG-INFO` & `swanlab-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: swanlab
-Version: 0.3.4
+Version: 0.3.5
 Summary: Python library for streamlined tracking and management of AI training processes.
 Project-URL: Homepage, https://swanhub.co
 Project-URL: Source, https://github.com/SwanHubX/SwanLab
 Project-URL: Bug Reports, https://github.com/SwanHubX/SwanLab/issues
 Project-URL: Documentation, https://geektechstudio.feishu.cn/wiki/space/7310593325374013444?ccm_open_type=lark_wiki_spaceLink&open_tab_from=wiki_home
 Author-email: Cunyue <team@swanhub.co>, Feudalman <team@swanhub.co>, ZeYi Lin <team@swanhub.co>, KashiwaByte <team@swanhub.co>
 License-Expression: Apache-2.0
@@ -535,28 +535,28 @@
 
 ## 💻 Self-hosted
 
 The community edition supports offline viewing of SwanLab dashboards.
 
 ### Offline Experiment Tracking
 
-Set the parameters `logir` and `cloud` in swanlab.init to track experiments offline:
+Set the parameters `logir` and `mode` in swanlab.init to track experiments offline:
 
 ```python
 ...
 
 swanlab.init(
     logdir='./logs',
-    cloud=False,
+    mode='local',
 )
 
 ...
 ```
 
-- The parameter `cloud` is set to `False`, which disables synchronizing the experiment to the cloud.
+- The parameter `mode` is set to `local`, which disables synchronizing the experiment to the cloud.
 
 - The setting of the parameter `logdir` is optional, and it specifies the location for saving SwanLab log files (by
   default saved in the `swanlog` folder).
 
 - Log files will be created and updated during tracking of experiments, and launching offline dashboards will also be
   based on these log files.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: swanlab Version: 0.3.4 Summary: Python library for
+Metadata-Version: 2.3 Name: swanlab Version: 0.3.5 Summary: Python library for
 streamlined tracking and management of AI training processes. Project-URL:
 Homepage, https://swanhub.co Project-URL: Source, https://github.com/SwanHubX/
 SwanLab Project-URL: Bug Reports, https://github.com/SwanHubX/SwanLab/issues
 Project-URL: Documentation, https://geektechstudio.feishu.cn/wiki/space/
 7310593325374013444?ccm_open_type=lark_wiki_spaceLink&open_tab_from=wiki_home
 Author-email: Cunyue
 swanhub.co>, Feudalman
@@ -206,27 +206,27 @@
 model.eval() correct = 0 total = 0 with torch.no_grad(): for batch in
 val_loader: x, y = batch x, y = x.to(device), y.to(device) output = model(x) _,
 predicted = torch.max(output, 1) total += y.size(0) correct += (predicted ==
 y).sum().item() accuracy = correct / total swanlab.log({"val/accuracy":
 accuracy}, step=epoch) ```
 ## ð» Self-hosted The community edition supports offline viewing of SwanLab
 dashboards. ### Offline Experiment Tracking Set the parameters `logir` and
-`cloud` in swanlab.init to track experiments offline: ```python ...
-swanlab.init( logdir='./logs', cloud=False, ) ... ``` - The parameter `cloud`
-is set to `False`, which disables synchronizing the experiment to the cloud. -
-The setting of the parameter `logdir` is optional, and it specifies the
-location for saving SwanLab log files (by default saved in the `swanlog`
-folder). - Log files will be created and updated during tracking of
-experiments, and launching offline dashboards will also be based on these log
-files. Other parts are completely consistent with cloud usage. ### Open Offline
-Board Open the terminal and use the following command to open a SwanLab
-dashboard: ```bash swanlab watch -l ./logs ``` After the operation is
-completed, SwanLab will provide you with a local URL link (default is [http://
-127.0.0.1:5092](http://127.0.0.1:5092)). Visit this link to view the experiment
-offline in the browser dashboard.
+`mode` in swanlab.init to track experiments offline: ```python ... swanlab.init
+( logdir='./logs', mode='local', ) ... ``` - The parameter `mode` is set to
+`local`, which disables synchronizing the experiment to the cloud. - The
+setting of the parameter `logdir` is optional, and it specifies the location
+for saving SwanLab log files (by default saved in the `swanlog` folder). - Log
+files will be created and updated during tracking of experiments, and launching
+offline dashboards will also be based on these log files. Other parts are
+completely consistent with cloud usage. ### Open Offline Board Open the
+terminal and use the following command to open a SwanLab dashboard: ```bash
+swanlab watch -l ./logs ``` After the operation is completed, SwanLab will
+provide you with a local URL link (default is [http://127.0.0.1:5092](http://
+127.0.0.1:5092)). Visit this link to view the experiment offline in the browser
+dashboard.
 ## ð Integration Combine your favorite framework with SwanLab, [More
 Integration](https://docs.swanlab.cn/zh/guide_cloud/integration/integration-
 pytorch-lightning.html). ?â??¡?ï?¸? PPyyTToorrcchh LLiigghhttnniinngg
 Create an instance using `SwanLabLogger` and pass it into the `logger`
 parameter of `Trainer` to enable SwanLab to record training metrics. ```python
 from swanlab.integration.pytorch_lightning import SwanLabLogger import
 importlib.util import os import pytorch_lightning as pl from torch import nn,
```

