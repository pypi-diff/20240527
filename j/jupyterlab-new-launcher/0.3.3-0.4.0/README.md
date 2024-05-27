# Comparing `tmp/jupyterlab_new_launcher-0.3.3.tar.gz` & `tmp/jupyterlab_new_launcher-0.4.0.tar.gz`

## Comparing `jupyterlab_new_launcher-0.3.3.tar` & `jupyterlab_new_launcher-0.4.0.tar`

### file list

```diff
@@ -1,66 +1,70 @@
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/.copier-answers.yml
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/CHANGELOG.md
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/babel.config.js
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/jest.config.js
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/junit.xml
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/setup.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/tsconfig.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/tsconfig.test.json
--rw-r--r--   0        0        0   376569 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/yarn.lock
--rw-r--r--   0        0        0    54951 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/docs/images/dialog.png
--rw-r--r--   0        0        0    58321 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/docs/images/launcher.png
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/_version.py
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/labextension/package.json
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/package.json.orig
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/plugin.json
--rw-r--r--   0        0        0    11071 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/labextension/static/728.5be4ee0b94a07decd5f8.js
--rw-r--r--   0        0        0    30575 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/labextension/static/787.27ef72da905b049778be.js
--rw-r--r--   0        0        0     7174 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/labextension/static/remoteEntry.a10a814d39706cd65aea.js
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/labextension/static/style.js
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/schema/plugin.json
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/src/commands.ts
--rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/src/database.ts
--rw-r--r--   0        0        0    10672 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/src/dialogs.tsx
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/src/icons.ts
--rw-r--r--   0        0        0     7271 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/src/index.ts
--rw-r--r--   0        0        0     4627 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/src/item.ts
--rw-r--r--   0        0        0    10633 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/src/launcher.tsx
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/src/svg.d.ts
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/src/types.ts
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/src/typings.d.ts
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/src/__tests__/jupyterlab_new_launcher.spec.ts
--rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/src/components/base-table.tsx
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/src/components/card.tsx
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/src/components/section.tsx
--rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/src/components/table.tsx
--rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/style/index.js
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/style/webkit.raw.css
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/style/icons/code-server.svg
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/style/icons/md/LICENSE
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/style/icons/md/file.svg
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/style/icons/md/star.svg
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/ui-tests/playwright.config.js
--rw-r--r--   0        0        0   148126 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/ui-tests/yarn.lock
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/ui-tests/tests/jupyterlab_new_launcher.spec.ts
--rw-r--r--   0        0        0    27608 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-linux.png
--rw-r--r--   0        0        0    28063 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-search-in-individual-linux.png
--rw-r--r--   0        0        0    33928 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-with-starred-linux.png
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/table-context-menu-linux.png
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/table-context-menu-visible-columns-linux.png
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/.gitignore
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/LICENSE
--rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/README.md
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/.copier-answers.yml
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/babel.config.js
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/jest.config.js
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/junit.xml
+-rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/setup.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/tsconfig.test.json
+-rw-r--r--   0        0        0   376569 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/yarn.lock
+-rw-r--r--   0        0        0    54951 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/docs/images/dialog.png
+-rw-r--r--   0        0        0    58321 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/docs/images/launcher.png
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/jupyter-config/server-config/jupyterlab_new_launcher.json
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/jupyterlab_new_launcher/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/jupyterlab_new_launcher/_version.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/jupyterlab_new_launcher/handlers.py
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/jupyterlab_new_launcher/labextension/package.json
+-rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/package.json.orig
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/plugin.json
+-rw-r--r--   0        0        0    31806 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/jupyterlab_new_launcher/labextension/static/252.6edb090ef613ff9206b6.js
+-rw-r--r--   0        0        0    11071 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/jupyterlab_new_launcher/labextension/static/728.54b87b26a387a46f2b0d.js
+-rw-r--r--   0        0        0     7175 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/jupyterlab_new_launcher/labextension/static/remoteEntry.36348165586c2a5361a1.js
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/jupyterlab_new_launcher/labextension/static/style.js
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/jupyterlab_new_launcher/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/schema/plugin.json
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/src/commands.ts
+-rw-r--r--   0        0        0     4744 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/src/database.ts
+-rw-r--r--   0        0        0    10672 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/src/dialogs.tsx
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/src/handler.ts
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/src/icons.ts
+-rw-r--r--   0        0        0     7318 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/src/index.ts
+-rw-r--r--   0        0        0     4668 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/src/item.ts
+-rw-r--r--   0        0        0    11152 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/src/launcher.tsx
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/src/model.ts
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/src/svg.d.ts
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/src/types.ts
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/src/typings.d.ts
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/src/__tests__/jupyterlab_new_launcher.spec.ts
+-rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/src/components/base-table.tsx
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/src/components/card.tsx
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/src/components/section.tsx
+-rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/src/components/table.tsx
+-rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/style/index.js
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/style/webkit.raw.css
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/style/icons/code-server.svg
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/style/icons/md/LICENSE
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/style/icons/md/file.svg
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/style/icons/md/star.svg
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/ui-tests/package.json
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0   148126 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/ui-tests/yarn.lock
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts
+-rw-r--r--   0        0        0    27608 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-linux.png
+-rw-r--r--   0        0        0    28063 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-search-in-individual-linux.png
+-rw-r--r--   0        0        0    33928 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-with-starred-linux.png
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/table-context-menu-linux.png
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/table-context-menu-visible-columns-linux.png
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/README.md
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6432 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.0/PKG-INFO
```

### Comparing `jupyterlab_new_launcher-0.3.3/.copier-answers.yml` & `jupyterlab_new_launcher-0.4.0/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.3/RELEASE.md` & `jupyterlab_new_launcher-0.4.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.3/jest.config.js` & `jupyterlab_new_launcher-0.4.0/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.3/package.json` & `jupyterlab_new_launcher-0.4.0/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.4.0'"}*

```diff
@@ -195,9 +195,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.3.3"
+    "version": "0.4.0"
 }
```

### Comparing `jupyterlab_new_launcher-0.3.3/tsconfig.json` & `jupyterlab_new_launcher-0.4.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.3/yarn.lock` & `jupyterlab_new_launcher-0.4.0/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.3/docs/images/dialog.png` & `jupyterlab_new_launcher-0.4.0/docs/images/dialog.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.3/docs/images/launcher.png` & `jupyterlab_new_launcher-0.4.0/docs/images/launcher.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/labextension/package.json` & `jupyterlab_new_launcher-0.4.0/jupyterlab_new_launcher/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9788194444444445%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.36348165586c2a5361a1.js'}}",*

 * * "'version'": "'0.4.0'"}*

```diff
@@ -108,15 +108,15 @@
         "src/**/*.{ts,tsx}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/nebari-dev/jupyterlab-new-launcher",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.a10a814d39706cd65aea.js",
+            "load": "static/remoteEntry.36348165586c2a5361a1.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "@jupyterlab/launcher-extension",
             "@jupyterlab/apputils-extension:sessionDialogs"
         ],
         "extension": true,
@@ -200,9 +200,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.3.3"
+    "version": "0.4.0"
 }
```

### Comparing `jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/package.json.orig` & `jupyterlab_new_launcher-0.4.0/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.4.0'"}*

```diff
@@ -195,9 +195,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.3.3"
+    "version": "0.4.0"
 }
```

### Comparing `jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/plugin.json` & `jupyterlab_new_launcher-0.4.0/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/labextension/static/728.5be4ee0b94a07decd5f8.js` & `jupyterlab_new_launcher-0.4.0/jupyterlab_new_launcher/labextension/static/728.54b87b26a387a46f2b0d.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -136,15 +136,15 @@
         },
         56: (n, e, t) => {
             n.exports = function(n) {
                 var e = t.nc;
                 e && n.setAttribute("nonce", e)
             }
         },
-        206: n => {
+        825: n => {
             n.exports = function(n) {
                 if ("undefined" == typeof document) return {
                     update: function() {},
                     remove: function() {}
                 };
                 var e = n.insertStyleElement(n);
                 return {
@@ -176,15 +176,15 @@
                 }
             }
         },
         728: (n, e, t) => {
             t.r(e);
             var r = t(72),
                 a = t.n(r),
-                o = t(206),
+                o = t(825),
                 i = t.n(o),
                 p = t(659),
                 l = t.n(p),
                 s = t(56),
                 c = t.n(s),
                 d = t(540),
                 h = t.n(d),
```

### Comparing `jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/labextension/static/787.27ef72da905b049778be.js` & `jupyterlab_new_launcher-0.4.0/jupyterlab_new_launcher/labextension/static/252.6edb090ef613ff9206b6.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,66 +1,66 @@
 "use strict";
 (self.webpackChunkjupyterlab_new_launcher = self.webpackChunkjupyterlab_new_launcher || []).push([
-    [787], {
-        787: (e, t, n) => {
+    [252], {
+        252: (e, t, n) => {
             n.r(t), n.d(t, {
-                default: () => W
+                default: () => Z
             });
-            var a = n(626),
-                s = n(923),
-                o = n(670),
-                r = n(260),
-                l = n(825),
-                c = n(265),
-                i = n(527),
+            var s = n(201),
+                a = n(420),
+                o = n(989),
+                r = n(107),
+                l = n(218),
+                i = n(450),
+                c = n(760),
                 d = n(53),
                 m = n(345),
                 u = n.n(m);
-            const h = new i.LabIcon({
+            const h = new c.LabIcon({
                     name: "jupyterlab-new-launcher:star",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">\n  <path class="jp-icon3 jp-star-filled" fill="rgb(97,97,97)" d="M12 17.27L18.18 21l-1.64-7.03L22 9.24l-7.19-.61L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21z" />\n  <path class="jp-icon3 jp-star-border" fill="rgb(97,97,97)" d="M22 9.24l-7.19-.62L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21 12 17.27 18.18 21l-1.63-7.03L22 9.24zM12 15.4l-3.76 2.27 1-4.28-3.32-2.88 4.38-.38L12 6.1l1.71 4.04 4.38.38-3.32 2.88 1 4.28L12 15.4z" />\n</svg>\n'
                 }),
-                p = new i.LabIcon({
+                p = new c.LabIcon({
                     name: "jupyterlab-new-launcher:file",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">\n  <path class="jp-icon3" fill="rgb(97,97,97)" d="M13.81 22H6C4.89 22 4 21.11 4 20V4C4 2.9 4.89 2 6 2H14L20 8V13.09C19.67 13.04 19.34 13 19 13S18.33 13.04 18 13.09V9H13V4H6V20H13.09C13.21 20.72 13.46 21.39 13.81 22M23 18H20V15H18V18H15V20H18V23H20V20H23V18Z" />\n</svg>'
                 }),
-                g = new i.LabIcon({
+                g = new c.LabIcon({
                     name: "jupyterlab-new-launcher:code-server",
                     svgstr: '<svg width="64" viewBox="0 0 2250 2250" version="1.1" xmlns="http://www.w3.org/2000/svg" style="fill-rule:evenodd;clip-rule:evenodd;stroke-linejoin:round;stroke-miterlimit:2;">\n<g class="jp-icon0" fill="#000" style="fill-rule:nonzero;">\n  <path d="M1991.66,1034.72c-38.493,0 -64.144,-22.57 -64.144,-68.897l-0,-266.084c-0,-169.867 -69.982,-263.709 -250.762,-263.709l-83.976,0l-0,179.368l25.661,0c71.144,0 104.967,39.201 104.967,109.285l0,235.201c0,102.156 30.324,143.733 96.806,165.114c-66.482,20.196 -96.806,62.958 -96.806,165.114l0,174.621c0,48.7 0,96.216 -12.829,144.917c-12.829,45.141 -33.823,87.903 -62.98,124.726c-16.329,21.386 -34.991,39.202 -55.981,55.835l-0,23.755l83.971,-0c180.781,-0 250.763,-93.843 250.763,-263.709l-0,-266.084c-0,-47.516 24.485,-68.897 64.144,-68.897l47.822,-0l-0,-179.37l-46.656,-0l0,-1.186Z"/>\n  <path d="M1420.16,706.904l-258.923,0c-5.833,0 -10.495,-4.752 -10.495,-10.691l-0,-20.192c-0,-5.941 4.662,-10.692 10.495,-10.692l260.089,0c5.83,0 10.495,4.751 10.495,10.692l0,20.192c0,5.939 -5.833,10.691 -11.661,10.691Z" />\n  <path d="M1464.48,963.474l-188.942,0c-5.833,0 -10.501,-4.754 -10.501,-10.693l0,-20.192c0,-5.938 4.668,-10.691 10.501,-10.691l188.942,-0c5.833,-0 10.495,4.753 10.495,10.691l-0,20.192c-0,4.754 -4.662,10.693 -10.495,10.693Z"/>\n  <path d="M1539.12,835.188l-377.885,0c-5.833,0 -10.495,-4.75 -10.495,-10.689l-0,-20.196c-0,-5.939 4.662,-10.69 10.495,-10.69l376.719,0c5.833,0 10.499,4.751 10.499,10.69l-0,20.196c-0,4.75 -3.5,10.689 -9.333,10.689Z"/>\n  <path d="M861.493,765.074c25.658,0 51.319,2.376 75.811,8.316l0,-48.705c0,-68.897 34.989,-109.285 104.971,-109.285l25.658,0l-0,-179.368l-83.977,0c-180.781,0 -250.758,93.842 -250.758,263.709l0,87.901c40.819,-14.252 83.977,-22.568 128.295,-22.568Z"/>\n  <path d="M1618.44,1411.25c-18.662,-150.861 -132.962,-276.776 -279.919,-305.285c-40.818,-8.314 -81.642,-9.504 -121.295,-2.376c-1.166,-0 -1.166,-1.189 -2.332,-1.189c-64.148,-136.605 -201.772,-226.884 -351.063,-226.884c-149.289,-0 -285.747,87.905 -351.062,224.51c-1.166,-0 -1.166,1.188 -2.332,1.188c-41.987,-4.753 -83.975,-2.379 -125.963,8.314c-144.623,35.634 -254.257,159.175 -274.085,308.847c-2.332,15.441 -3.499,30.883 -3.499,45.141c0,45.136 30.325,86.713 74.645,92.652c54.817,8.317 102.636,-34.448 101.469,-89.089c0,-8.317 0,-17.821 1.167,-26.134c9.331,-76.025 66.48,-140.168 141.123,-157.99c23.328,-5.939 46.654,-7.124 68.814,-3.559c71.146,9.502 141.124,-27.324 171.449,-91.467c22.162,-47.516 57.151,-89.094 103.804,-111.664c51.314,-24.946 109.633,-28.506 163.286,-9.499c55.979,20.192 97.966,62.954 123.627,116.409c26.824,52.27 39.653,89.093 96.805,96.221c23.325,3.559 88.639,2.374 113.132,1.185c47.82,0 95.64,16.631 129.463,51.079c22.156,23.757 38.485,53.455 45.486,86.715c10.495,53.455 -2.334,106.908 -33.825,147.296c-22.162,28.509 -52.485,49.89 -86.308,59.394c-16.329,4.754 -32.657,5.939 -48.986,5.939l-257.757,0c-51.314,0 -92.138,-41.573 -92.138,-93.842l0,-348.049c0,-14.251 -11.661,-26.13 -25.658,-26.13l-36.156,0c-71.148,1.185 -128.295,81.964 -128.295,167.488l-0,312.415c-0,92.652 73.476,167.488 164.451,167.488c0,0 404.714,-1.19 410.544,-1.19c93.304,-9.503 179.614,-58.204 237.927,-133.04c58.319,-72.46 85.142,-167.492 73.481,-264.894Z"/>\n</g></svg>'
                 });
             var f = n(602);
             class v {
                 constructor(e) {
-                    var t, n, a, s;
+                    var t, n, s, a;
                     this._options = e, this._refreshLastUsed = new f.Signal(this), this._refreshClock = null;
                     const {
                         item: o,
                         commands: r,
                         cwd: l
-                    } = e, c = {
+                    } = e, i = {
                         ...o.args,
                         cwd: l
                     };
-                    this.command = o.command, this.args = c, this.category = o.category, this.rank = o.rank, this.kernelIconUrl = o.kernelIconUrl, this.metadata = null !== (t = o.metadata) && void 0 !== t ? t : {}, this.iconClass = r.iconClass(o.command, c), this.icon = r.icon(o.command, c), this.caption = r.caption(o.command, c), this.label = r.label(o.command, c);
-                    const i = this.metadata.kernel;
-                    if (i) {
-                        const e = (null !== (n = i.conda_env_name) && void 0 !== n ? n : "").match(/(?<namespace>.+)-(?<duplicate>\1)-(?<environment>.+)/);
+                    this.command = o.command, this.args = i, this.category = o.category, this.rank = o.rank, this.kernelIconUrl = o.kernelIconUrl, this.metadata = null !== (t = o.metadata) && void 0 !== t ? t : {}, this.iconClass = r.iconClass(o.command, i), this.icon = r.icon(o.command, i), this.caption = r.caption(o.command, i), this.label = r.label(o.command, i);
+                    const c = this.metadata.kernel;
+                    if (c) {
+                        const e = (null !== (n = c.conda_env_name) && void 0 !== n ? n : "").match(/(?<namespace>.+)-(?<duplicate>\1)-(?<environment>.+)/);
                         if (e && this.metadata) {
                             const t = e.groups;
-                            this.label = null !== (a = i.conda_language) && void 0 !== a ? a : t.environment, this.metadata = {
+                            this.label = null !== (s = c.conda_language) && void 0 !== s ? s : t.environment, delete c.conda_env_name, this.metadata = {
                                 ...this.metadata,
                                 kernel: {
                                     Namespace: t.namespace,
                                     conda_env_name: t.environment,
-                                    ...i
+                                    ...c
                                 }
                             }
                         }
                     }
-                    "server-proxy:open" === this.command && (null === (s = this.kernelIconUrl) || void 0 === s ? void 0 : s.endsWith("/vscode")) && (this.icon = g)
+                    "server-proxy:open" === this.command && (null === (a = this.kernelIconUrl) || void 0 === a ? void 0 : a.endsWith("/vscode")) && (this.icon = g)
                 }
                 get starred() {
                     var e;
                     const {
                         item: t,
                         favoritesDatabase: n
                     } = this._options;
@@ -107,57 +107,57 @@
                     const t = Date.now() - e.getTime(),
                         n = t < 6e4 ? 1e4 : t < 36e5 ? 6e4 : 36e5;
                     this._refreshClock = window.setTimeout((() => {
                         this._refreshLastUsed.emit(), this._setRefreshClock(this._lastUsed)
                     }), n)
                 }
             }
-            var b = n(702);
+            var b = n(445);
             const _ = "jp-sortable-table";
 
             function w(e) {
                 const [t, n] = (0, m.useState)({
                     sortKey: e.sortKey,
                     sortDirection: e.sortDirection || 1
                 });
-                let a = e.rows;
-                const s = e.columns.filter((e => e.id === t.sortKey))[0];
-                if (s) {
-                    const n = s.sort.bind(s);
-                    a = e.rows.sort(((e, a) => {
-                        var s;
-                        return (null !== (s = n(e.data, a.data)) && void 0 !== s ? s : 0) * t.sortDirection
+                let s = e.rows;
+                const a = e.columns.filter((e => e.id === t.sortKey))[0];
+                if (a) {
+                    const n = a.sort.bind(a);
+                    s = e.rows.sort(((e, s) => {
+                        var a;
+                        return (null !== (a = n(e.data, s.data)) && void 0 !== a ? a : 0) * t.sortDirection
                     }))
                 }
                 const o = e.columns.filter((e => (!e.isAvailable || e.isAvailable()) && !e.isHidden)),
                     [r, l] = u().useState({}),
-                    c = a.map((t => {
+                    i = s.map((t => {
                         const n = o.map((e => u().createElement("td", {
                             key: e.id + "-" + t.key,
                             className: r[e.id] ? "jp-mod-col-resized" : ""
                         }, e.renderCell(t.data))));
                         return u().createElement("tr", {
                             key: t.key,
                             "data-key": t.key,
                             onClick: e.onRowClick,
                             className: "jp-sortable-table-tr"
                         }, n)
                     })),
-                    i = o.map((e => u().createElement(y, {
+                    c = o.map((e => u().createElement(y, {
                         label: e.label,
                         id: e.id,
                         state: t,
                         key: e.id,
                         onSort: () => {
-                            var a;
-                            (a = e.id) === t.sortKey ? n({
-                                sortKey: a,
+                            var s;
+                            (s = e.id) === t.sortKey ? n({
+                                sortKey: s,
                                 sortDirection: -1 * t.sortDirection
                             }) : n({
-                                sortKey: a,
+                                sortKey: s,
                                 sortDirection: 1
                             })
                         },
                         onResize: () => {
                             l({
                                 ...r,
                                 [e.id]: !0
@@ -165,24 +165,24 @@
                         },
                         minWidth: e.minWidth
                     })));
                 return u().createElement("table", {
                     className: _
                 }, u().createElement("thead", null, u().createElement("tr", {
                     className: "jp-sortable-table-tr"
-                }, i)), u().createElement("tbody", null, c))
+                }, c)), u().createElement("tbody", null, i))
             }
 
             function y(e) {
                 var t;
                 const n = e.id === e.state.sortKey,
-                    a = n && 1 !== e.state.sortDirection ? i.caretDownIcon : i.caretUpIcon,
-                    [s, o] = u().useState(null),
+                    s = n && 1 !== e.state.sortDirection ? c.caretDownIcon : c.caretUpIcon,
+                    [a, o] = u().useState(null),
                     r = u().useRef(null),
-                    [l, c] = u().useState(!1),
+                    [l, i] = u().useState(!1),
                     [d, h] = (0, m.useState)(null);
                 requestAnimationFrame((() => {
                     if (r.current) {
                         const {
                             left: e
                         } = r.current.getBoundingClientRect();
                         h(e)
@@ -195,15 +195,15 @@
                                     if (!r.current) throw Error("Cannot resize: no reference to the current table");
                                     console.warn("Resize cache for column was not available"), n = r.current.getBoundingClientRect().left
                                 } else n = d;
                                 o(t.clientX - n), e.onResize()
                             }
                         },
                         n = e => {
-                            l && (document.body.classList.remove(f), c(!1), e.stopImmediatePropagation())
+                            l && (document.body.classList.remove(f), i(!1), e.stopImmediatePropagation())
                         };
                     return document.body.addEventListener("pointermove", t), document.body.addEventListener("pointerup", n), () => {
                         document.body.removeEventListener("pointermove", t), document.body.removeEventListener("pointerup", n)
                     }
                 }));
                 const p = [];
                 n && p.push("jp-sorted-header"), l && p.push("jp-header-resizing");
@@ -212,39 +212,39 @@
                 return u().createElement("th", {
                     key: e.id,
                     ref: r,
                     onClick: () => e.onSort(),
                     className: p.join(" "),
                     "data-id": e.id,
                     style: {
-                        width: null !== s ? `${Math.max(null!==(t=e.minWidth)&&void 0!==t?t:50,s)}px` : ""
+                        width: null !== a ? `${Math.max(null!==(t=e.minWidth)&&void 0!==t?t:50,a)}px` : ""
                     },
                     onPointerDown: e => {
-                        e.target instanceof HTMLElement && e.target.className === g && (document.body.classList.add(f), c(!0))
+                        e.target instanceof HTMLElement && e.target.className === g && (document.body.classList.add(f), i(!0))
                     }
                 }, u().createElement("div", {
                     className: "jp-sortable-table-th-wrapper"
-                }, u().createElement("label", null, e.label), u().createElement(a.react, {
+                }, u().createElement("label", null, e.label), u().createElement(s.react, {
                     tag: "span",
                     className: "jp-sort-icon"
                 })), u().createElement("div", {
                     className: g
                 }))
             }
             var C = n(262);
             const k = "jupyterlab-new-launcher:plugin";
             var E;
             ! function(e) {
                 e.create = "launcher:create", e.moveColumn = "new-launcher:table-move-column", e.toggleColumn = "new-launcher:table-toggle-column"
             }(E || (E = {}));
-            const D = new C.Token("jupyterlab-new-launcher:ILauncherDatabase", "Databases for new launcher."),
-                L = "jp-starIconButton",
+            const N = new C.Token("jupyterlab-new-launcher:ILauncherDatabase", "Databases for new launcher."),
+                S = "jp-starIconButton",
                 j = "jp-TableKernelItem";
 
-            function N(e) {
+            function L(e) {
                 if (0 === e.length) return "(empty)";
                 switch (e) {
                     case "conda_env_name":
                         return "Environment";
                     case "conda_env_path":
                         return "Environment path";
                     case "conda_language":
@@ -255,82 +255,82 @@
                         return "Base?";
                     case "conda_is_currently_running":
                         return "Running?"
                 }
                 return e[0].toUpperCase() + e.substring(1)
             }
 
-            function S(e) {
-                const [t, n] = m.useState(void 0), a = m.useRef(null);
+            function D(e) {
+                const [t, n] = m.useState(void 0), s = m.useRef(null);
                 return m.createElement("div", {
                     className: "jp-ellipsis-wrapper",
                     title: e.title
                 }, m.createElement("div", {
                     className: "jp-ellipsis",
                     title: t,
-                    ref: a,
+                    ref: s,
                     onMouseEnter: () => {
                         if (e.title) return;
-                        const t = a.current;
+                        const t = s.current;
                         t && t.scrollWidth > t.clientWidth ? n(t.innerText) : n(void 0)
                     }
                 }, e.children))
             }
 
             function U(e) {
-                var t, n, a, s;
+                var t, n, s, a;
                 const {
                     trans: o
                 } = e;
                 let r, l;
-                const [c, d] = m.useState("");
-                e.showSearchBox ? (r = c, l = d) : r = e.query;
+                const [i, d] = m.useState("");
+                e.showSearchBox ? (r = i, l = d) : r = e.query;
                 const [, u] = m.useReducer((e => e + 1), 0);
                 m.useEffect((() => (e.favouritesChanged.connect(u), () => {
                     e.favouritesChanged.disconnect(u)
                 }))), m.useEffect((() => (e.lastUsedChanged.connect(u), () => {
                     e.lastUsedChanged.disconnect(u)
                 })));
                 const p = new Set;
                 for (const n of e.items) {
                     const e = null === (t = n.metadata) || void 0 === t ? void 0 : t.kernel;
                     if (e)
                         for (const t of Object.keys(e)) p.add(t)
                 }
                 const g = [...p].map((e => ({
                     id: e,
-                    label: N(e),
+                    label: L(e),
                     renderCell: t => {
                         var n;
-                        const a = null === (n = t.metadata) || void 0 === n ? void 0 : n.kernel;
-                        return m.createElement(S, null, (() => {
-                            if (!a) return "-";
-                            const t = a[e];
+                        const s = null === (n = t.metadata) || void 0 === n ? void 0 : n.kernel;
+                        return m.createElement(D, null, (() => {
+                            if (!s) return "-";
+                            const t = s[e];
                             return "string" == typeof t ? t : JSON.stringify(t)
                         })())
                     },
                     sort: (t, n) => {
-                        var a, s;
-                        const o = null === (a = t.metadata) || void 0 === a ? void 0 : a.kernel,
-                            r = null === (s = n.metadata) || void 0 === s ? void 0 : s.kernel,
+                        var s, a;
+                        const o = null === (s = t.metadata) || void 0 === s ? void 0 : s.kernel,
+                            r = null === (a = n.metadata) || void 0 === a ? void 0 : a.kernel,
                             l = o ? o[e] : void 0,
-                            c = r ? r[e] : void 0;
-                        return l === c ? 0 : l ? c ? "string" == typeof l && "string" == typeof c ? l.localeCompare(c) : l > c ? 1 : -1 : -1 : 1
+                            i = r ? r[e] : void 0;
+                        return l === i ? 0 : l ? i ? "string" == typeof l && "string" == typeof i ? l.localeCompare(i) : l > i ? 1 : -1 : -1 : 1
                     }
                 })));
                 e.showWidgetType && g.push({
                     id: "widget-type",
                     label: o.__("Type"),
                     renderCell: e => e.command.split(":")[0],
                     sort: (e, t) => e.command.localeCompare(t.command)
                 });
                 const f = [{
                         id: "kernel",
                         label: o.__("Kernel"),
-                        renderCell: t => m.createElement(S, null, m.createElement("span", {
+                        renderCell: t => m.createElement(D, null, m.createElement("span", {
                             className: j,
                             onClick: n => {
                                 e.onClick(t), n.stopPropagation()
                             },
                             onKeyDown: e => {
                                 "Enter" === e.key && t.execute()
                             },
@@ -347,155 +347,155 @@
                         }, t.label[0].toUpperCase())), m.createElement("span", {
                             className: "jp-TableKernelItem-label"
                         }, t.label))),
                         sort: (e, t) => e.label.localeCompare(t.label)
                     }, ...g, {
                         id: "last-used",
                         label: o.__("Last Used"),
-                        renderCell: e => m.createElement(i.UseSignal, {
+                        renderCell: e => m.createElement(c.UseSignal, {
                             signal: e.refreshLastUsed
-                        }, (() => m.createElement(S, {
+                        }, (() => m.createElement(D, {
                             title: e.lastUsed ? b.Time.format(e.lastUsed) : o.__("No information about last use of this kernel is available in the layout database")
                         }, e.lastUsed ? b.Time.formatHuman(e.lastUsed) : o.__("Never")))),
                         sort: (e, t) => e.lastUsed === t.lastUsed ? 0 : e.lastUsed ? t.lastUsed && e.lastUsed > t.lastUsed ? 1 : -1 : 1
                     }, {
                         id: "star",
                         label: "",
                         renderCell: e => {
                             const t = e.starred,
                                 n = t ? o.__("Click to remove the kernel from favourites") : o.__("Click to add this kernel to favourites");
                             return m.createElement("button", {
-                                className: t ? `${L} jp-mod-starred` : L,
+                                className: t ? `${S} jp-mod-starred` : S,
                                 title: n,
                                 onClick: async t => {
                                     t.stopPropagation(), await e.toggleStar()
                                 }
                             }, m.createElement(h.react, {
                                 className: "jp-starIcon"
                             }))
                         },
                         sort: (e, t) => Number(e.starred) - Number(t.starred)
                     }],
                     v = null !== (n = e.hideColumns) && void 0 !== n ? n : [],
                     _ = f.filter((e => !v.includes(e.id))),
-                    [y, C] = m.useState(null !== (a = e.settings.composite.hiddenColumns) && void 0 !== a ? a : {}),
+                    [y, C] = m.useState(null !== (s = e.settings.composite.hiddenColumns) && void 0 !== s ? s : {}),
                     k = _.map((e => e.id)),
-                    [D, U] = m.useState(null !== (s = e.settings.composite.columnOrder) && void 0 !== s ? s : k),
+                    [N, U] = m.useState(null !== (a = e.settings.composite.columnOrder) && void 0 !== a ? a : k),
                     I = w,
                     x = () => {
                         var t, n;
-                        const a = null !== (t = e.settings.composite.hiddenColumns) && void 0 !== t ? t : {};
-                        y !== a && C(a);
-                        const s = null !== (n = e.settings.composite.columnOrder) && void 0 !== n ? n : k;
-                        D !== s && U(s)
+                        const s = null !== (t = e.settings.composite.hiddenColumns) && void 0 !== t ? t : {};
+                        y !== s && C(s);
+                        const a = null !== (n = e.settings.composite.columnOrder) && void 0 !== n ? n : k;
+                        N !== a && U(a)
                     };
                 return m.useEffect((() => (e.settings.changed.connect(x), () => {
                     e.settings.changed.disconnect(x)
                 }))), m.createElement("div", {
                     className: "jp-NewLauncher-table"
                 }, e.showSearchBox ? m.createElement("div", {
                     className: "jp-Launcher-searchBox"
-                }, m.createElement(i.FilterBox, {
+                }, m.createElement(c.FilterBox, {
                     placeholder: o.__("Filter kernels"),
                     updateFilter: (e, t) => {
                         l(null != t ? t : "")
                     },
                     initialQuery: "",
                     useFuzzyFilter: !1
                 })) : null, m.createElement("div", {
                     className: "jp-NewLauncher-table-scroller",
                     onContextMenu: t => {
                         var n;
                         t.preventDefault();
-                        const a = new i.MenuSvg({
+                        const s = new c.MenuSvg({
                             commands: e.commands
                         });
-                        a.addClass("jp-NewLauncher-contextMenu");
-                        const s = new i.MenuSvg({
+                        s.addClass("jp-NewLauncher-contextMenu");
+                        const a = new c.MenuSvg({
                             commands: e.commands
                         });
-                        s.addClass("jp-NewLauncher-contextMenu-visibleColumns");
-                        for (const e of _) s.addItem({
+                        a.addClass("jp-NewLauncher-contextMenu-visibleColumns");
+                        for (const e of _) a.addItem({
                             command: E.toggleColumn,
                             args: {
                                 id: e.id,
                                 label: e.label
                             }
                         });
-                        s.title.label = o.__("Visible Columns"), a.addItem({
+                        a.title.label = o.__("Visible Columns"), s.addItem({
                             type: "submenu",
-                            submenu: s
+                            submenu: a
                         });
                         const r = null === (n = t.target.closest("th[data-id]")) || void 0 === n ? void 0 : n.dataset.id;
-                        r && (a.addItem({
+                        r && (s.addItem({
                             command: E.moveColumn,
                             args: {
                                 direction: "left",
-                                order: D,
+                                order: N,
                                 id: r
                             }
-                        }), a.addItem({
+                        }), s.addItem({
                             command: E.moveColumn,
                             args: {
                                 direction: "right",
-                                order: D,
+                                order: N,
                                 id: r
                             }
-                        })), a.open(t.clientX, t.clientY)
+                        })), s.open(t.clientX, t.clientY)
                     }
                 }, m.createElement(I, {
                     rows: e.items.filter((e => {
                         var t;
                         const n = r.toLowerCase();
                         if (e.label.toLowerCase().includes(n)) return !0;
-                        const a = null === (t = e.metadata) || void 0 === t ? void 0 : t.kernel;
-                        if (a) {
+                        const s = null === (t = e.metadata) || void 0 === t ? void 0 : t.kernel;
+                        if (s) {
                             for (const e of p) {
-                                const t = a[e];
+                                const t = s[e];
                                 if ("string" == typeof t && t.toLowerCase().includes(n)) return !0
                             }
                             return !1
                         }
                     })).map((e => ({
                         data: e,
                         key: e.command + JSON.stringify(e.args)
                     }))),
                     blankIndicator: () => m.createElement("div", null, o.__("No entries")),
                     sortKey: "kernel",
                     onRowClick: e => {
                         const t = e.target,
                             n = t.closest("tr");
                         if (!n) return;
-                        const a = t.closest("td"),
-                            s = null == a ? void 0 : a.querySelector(`.${L}`);
-                        if (s) return s.click();
+                        const s = t.closest("td"),
+                            a = null == s ? void 0 : s.querySelector(`.${S}`);
+                        if (a) return a.click();
                         n.querySelector(`.${j}`).click()
                     },
                     columns: _.filter((e => "hidden" !== y[e.id])).map((e => {
                         var t;
                         return {
                             ...e,
-                            rank: null !== (t = D.indexOf(e.id)) && void 0 !== t ? t : 10
+                            rank: null !== (t = N.indexOf(e.id)) && void 0 !== t ? t : 10
                         }
                     })).sort(((e, t) => e.rank - t.rank))
                 })))
             }
 
             function I(e) {
                 const [t, n] = m.useState(e.open);
                 return m.createElement("details", {
                     onToggle: t => {
                         n(t.currentTarget.open), e.onToggled && e.onToggled(t.currentTarget.open)
                     },
-                    className: (0, i.classes)(e.className, "jp-CollapsibleSection"),
+                    className: (0, c.classes)(e.className, "jp-CollapsibleSection"),
                     open: t
                 }, m.createElement("summary", null, m.createElement("div", {
                     className: "jp-CollapsibleSection-CollapserIconWrapper",
                     "aria-hidden": "true"
-                }, m.createElement(i.caretRightIcon.react, {
+                }, m.createElement(c.caretRightIcon.react, {
                     className: "jp-CollapsibleSection-CollapserIcon"
                 })), m.createElement(e.icon.react, {
                     tag: "span",
                     className: "jp-CollapsibleSection-CategoryIcon"
                 }), m.createElement("h3", {
                     className: "jp-CollapsibleSection-Title"
                 }, e.title)), m.createElement("div", {
@@ -510,31 +510,31 @@
                 return m.createElement("div", {
                     onClick: () => t.execute(),
                     className: "jp-Launcher-TypeCard jp-LauncherCard",
                     title: t.caption || t.label,
                     tabIndex: 0
                 }, m.createElement("div", {
                     className: "jp-LauncherCard-icon"
-                }, m.createElement(i.LabIcon.resolveReact, {
+                }, m.createElement(c.LabIcon.resolveReact, {
                     icon: t.icon,
-                    iconClass: (0, i.classes)(t.iconClass, "jp-Icon-cover")
+                    iconClass: (0, c.classes)(t.iconClass, "jp-Icon-cover")
                 })), m.createElement("div", {
                     className: "jp-LauncherCard-label"
                 }, m.createElement("p", null, t.label)))
             }
 
             function B(e) {
                 var t;
                 const {
                     trans: n,
-                    cwd: a,
-                    typeItems: s,
+                    cwd: s,
+                    typeItems: a,
                     otherItems: o,
                     favouritesChanged: r
-                } = e, [l, c] = m.useState(""), [, d] = m.useReducer((e => e + 1), 0), [u, g] = m.useState(e.settings.composite.starredSection), [f, v] = m.useState(e.settings.composite.searchAllSections), b = () => {
+                } = e, [l, i] = m.useState(""), [, d] = m.useReducer((e => e + 1), 0), [u, g] = m.useState(e.settings.composite.starredSection), [f, v] = m.useState(e.settings.composite.searchAllSections), b = () => {
                     const t = e.settings.composite.starredSection;
                     u !== t && g(t);
                     const n = e.settings.composite.searchAllSections;
                     f !== n && v(n)
                 };
                 if (m.useEffect((() => (e.settings.changed.connect(b), () => {
                         e.settings.changed.disconnect(b)
@@ -549,219 +549,249 @@
                 const _ = new Set;
                 for (const n of e.notebookItems) {
                     const e = null === (t = n.metadata) || void 0 === t ? void 0 : t.kernel;
                     if (e)
                         for (const t of Object.keys(e)) _.add(t)
                 }
                 const w = [...e.notebookItems, ...e.consoleItems].filter((e => e.starred)),
-                    y = e.settings.composite.collapsedSections;
+                    y = e.settings.composite.collapsedSections,
+                    C = [{
+                        className: "jp-Launcher-openByType",
+                        title: n.__("Create Empty"),
+                        icon: p,
+                        id: "create-empty",
+                        rank: 1,
+                        render: () => a.filter((e => !l || -1 !== e.label.toLowerCase().indexOf(l.toLowerCase()))).map((e => m.createElement(x, {
+                            item: e,
+                            trans: n
+                        })))
+                    }, {
+                        className: "jp-Launcher-openByKernel jp-Launcher-launchNotebook",
+                        title: n.__("Launch New Notebook"),
+                        icon: c.notebookIcon,
+                        id: "launch-notebook",
+                        rank: 3,
+                        render: () => m.createElement(U, {
+                            items: e.notebookItems,
+                            commands: e.commands,
+                            showSearchBox: !f,
+                            query: l,
+                            settings: e.settings,
+                            trans: n,
+                            onClick: e => e.execute(),
+                            favouritesChanged: e.favouritesChanged,
+                            lastUsedChanged: e.lastUsedChanged
+                        })
+                    }, {
+                        className: "jp-Launcher-openByKernel jp-Launcher-launchConsole",
+                        title: n.__("Launch New Console"),
+                        icon: c.consoleIcon,
+                        id: "launch-console",
+                        rank: 5,
+                        render: () => m.createElement(U, {
+                            items: e.consoleItems,
+                            commands: e.commands,
+                            showSearchBox: !f,
+                            query: l,
+                            settings: e.settings,
+                            trans: n,
+                            onClick: e => e.execute(),
+                            favouritesChanged: e.favouritesChanged,
+                            lastUsedChanged: e.lastUsedChanged
+                        })
+                    }];
+                u && C.push({
+                    className: "jp-Launcher-openByKernel",
+                    title: n.__("Starred"),
+                    icon: h,
+                    id: "starred",
+                    rank: 2,
+                    render: () => w.length > 0 ? m.createElement(U, {
+                        items: w,
+                        commands: e.commands,
+                        showSearchBox: !f,
+                        showWidgetType: !0,
+                        query: l,
+                        settings: e.settings,
+                        trans: n,
+                        onClick: e => e.execute(),
+                        favouritesChanged: e.favouritesChanged,
+                        lastUsedChanged: e.lastUsedChanged
+                    }) : "No starred items"
+                });
+                const k = [...C, ...e.sections];
                 return m.createElement("div", {
                     className: "jp-LauncherBody"
                 }, m.createElement("div", {
                     className: "jp-NewLauncher-TopBar"
                 }, m.createElement("div", {
                     className: "jp-Launcher-cwd"
-                }, m.createElement("h3", null, n.__("Current folder:"), " ", m.createElement("code", null, a || "/"))), m.createElement("div", {
+                }, m.createElement("h3", null, n.__("Current folder:"), " ", m.createElement("code", null, s || "/"))), m.createElement("div", {
                     className: "jp-NewLauncher-OtherItems"
                 }, o.map((e => m.createElement(x, {
                     item: e,
                     trans: n
                 }))))), f ? m.createElement("div", {
                     className: "jp-Launcher-searchBox"
-                }, m.createElement(i.FilterBox, {
+                }, m.createElement(c.FilterBox, {
                     placeholder: n.__("Filter"),
                     updateFilter: (e, t) => {
-                        c(null != t ? t : "")
+                        i(null != t ? t : "")
                     },
                     initialQuery: "",
                     useFuzzyFilter: !1
-                })) : null, m.createElement(I, {
-                    className: "jp-Launcher-openByType",
-                    title: n.__("Create Empty"),
-                    icon: p,
-                    open: "collapsed" !== y["create-empty"]
-                }, s.filter((e => !l || -1 !== e.label.toLowerCase().indexOf(l.toLowerCase()))).map((e => m.createElement(x, {
-                    item: e,
-                    trans: n
-                })))), u ? m.createElement(I, {
-                    className: "jp-Launcher-openByKernel",
-                    title: n.__("Starred"),
-                    icon: h,
-                    open: "collapsed" !== y.starred
-                }, w.length > 0 ? m.createElement(U, {
-                    items: w,
-                    commands: e.commands,
-                    showSearchBox: !f,
-                    showWidgetType: !0,
-                    query: l,
-                    settings: e.settings,
-                    trans: n,
-                    onClick: e => e.execute(),
-                    favouritesChanged: e.favouritesChanged,
-                    lastUsedChanged: e.lastUsedChanged
-                }) : "No starred items") : null, m.createElement(I, {
-                    className: "jp-Launcher-openByKernel jp-Launcher-launchNotebook",
-                    title: n.__("Launch New Notebook"),
-                    icon: i.notebookIcon,
-                    open: "collapsed" !== y["launch-notebook"]
-                }, m.createElement(U, {
-                    items: e.notebookItems,
-                    commands: e.commands,
-                    showSearchBox: !f,
-                    query: l,
-                    settings: e.settings,
-                    trans: n,
-                    onClick: e => e.execute(),
-                    favouritesChanged: e.favouritesChanged,
-                    lastUsedChanged: e.lastUsedChanged
-                })), m.createElement(I, {
-                    className: "jp-Launcher-openByKernel jp-Launcher-launchConsole",
-                    title: n.__("Launch New Console"),
-                    icon: i.consoleIcon,
-                    open: "collapsed" !== y["launch-console"]
-                }, m.createElement(U, {
-                    items: e.consoleItems,
-                    commands: e.commands,
-                    showSearchBox: !f,
-                    query: l,
-                    settings: e.settings,
-                    trans: n,
-                    onClick: e => e.execute(),
-                    favouritesChanged: e.favouritesChanged,
-                    lastUsedChanged: e.lastUsedChanged
-                })))
+                })) : null, k.sort(((e, t) => e.rank - t.rank)).map((e => m.createElement(I, {
+                    className: e.className,
+                    title: e.title,
+                    icon: e.icon,
+                    open: "collapsed" !== y[e.id]
+                }, e.render()))))
             }
             const K = "server-proxy:open";
             class M extends r.Launcher {
                 constructor(e) {
                     super(e), this.renderCommand = e => new v({
                         item: e,
                         cwd: this.cwd,
                         commands: this.commands,
                         lastUsedDatabase: this._lastUsedDatabase,
                         favoritesDatabase: this._favoritesDatabase
-                    }), this.renderKernelCommand = e => this.renderCommand(e), this.commands = e.commands, this.trans = this.translator.load("jupyterlab-new-launcher"), this._lastUsedDatabase = e.lastUsedDatabase, this._favoritesDatabase = e.favoritesDatabase, this._settings = e.settings
+                    }), this.renderKernelCommand = e => this.renderCommand(e), this.commands = e.commands, this.trans = this.translator.load("jupyterlab-new-launcher"), this._lastUsedDatabase = e.lastUsedDatabase, this._favoritesDatabase = e.favoritesDatabase, this._settings = e.settings, this._newModel = e.model, this._newModel.sectionAdded.connect((() => {
+                        this.update()
+                    }))
                 }
                 render() {
                     if (!this.model) return null;
                     const e = this.trans,
                         t = [...this.model.items()],
                         n = e.__("Notebook"),
-                        a = e.__("Console"),
-                        s = [n, a],
+                        s = e.__("Console"),
+                        a = [n, s],
                         o = this._settings.composite.utilityCommands,
                         r = t.filter((e => o.includes(e.command))).map(this.renderCommand),
-                        l = t.filter((e => (!e.category || !s.includes(e.category)) && !o.includes(e.command) || e.command === K)),
-                        c = {
+                        l = t.filter((e => (!e.category || !a.includes(e.category)) && !o.includes(e.command) || e.command === K)),
+                        i = {
                             "terminal:create-new": 3,
                             "fileeditor:create-new": 6,
                             "fileeditor:create-new-markdown-file": 5
                         };
-                    for (const e of l) e.command in c && (e.rank = c[e.command]);
-                    const i = [{
+                    for (const e of l) e.command in i && (e.rank = i[e.command]);
+                    const c = [{
                             command: "notebook:create-new",
                             rank: 1
                         }, {
                             command: "console:create",
                             rank: 4
                         }, ...l].sort(((e, t) => {
-                            var n, a;
-                            return (null !== (n = null == e ? void 0 : e.rank) && void 0 !== n ? n : 0) - (null !== (a = null == t ? void 0 : t.rank) && void 0 !== a ? a : 0)
+                            var n, s;
+                            return (null !== (n = null == e ? void 0 : e.rank) && void 0 !== n ? n : 0) - (null !== (s = null == t ? void 0 : t.rank) && void 0 !== s ? s : 0)
                         })),
                         d = t.filter((e => e.category && e.category === n && e.command !== K)).map(this.renderKernelCommand),
-                        u = t.filter((e => e.category && e.category === a && e.command !== K)).map(this.renderKernelCommand),
-                        h = i.map(this.renderCommand);
+                        u = t.filter((e => e.category && e.category === s && e.command !== K)).map(this.renderKernelCommand),
+                        h = c.map(this.renderCommand);
                     return m.createElement(B, {
                         trans: this.trans,
                         cwd: this.cwd,
                         commands: this.commands,
                         typeItems: h,
                         notebookItems: d,
                         consoleItems: u,
                         otherItems: r,
                         settings: this._settings,
                         favouritesChanged: this._favoritesDatabase.changed,
-                        lastUsedChanged: this._lastUsedDatabase.changed
+                        lastUsedChanged: this._lastUsedDatabase.changed,
+                        sections: this._newModel.sections
                     })
                 }
             }
-            class T extends s.SessionContextDialogs {
+            class A extends r.LauncherModel {
+                constructor() {
+                    super(...arguments), this.sections = [], this._sectionAdded = new f.Signal(this)
+                }
+                addSection(e) {
+                    this.sections.push(e), this._sectionAdded.emit()
+                }
+                get sectionAdded() {
+                    return this._sectionAdded
+                }
+            }
+            class T extends a.SessionContextDialogs {
                 constructor(e) {
                     var t;
                     super(e), this.options = e;
-                    const n = null !== (t = e.translator) && void 0 !== t ? t : c.nullTranslator;
+                    const n = null !== (t = e.translator) && void 0 !== t ? t : i.nullTranslator;
                     this.trans = n.load("jupyterlab")
                 }
                 async selectKernel(e) {
                     const t = this.trans;
                     if (e.isDisposed) return Promise.resolve();
                     let n = t.__("Cancel");
                     e.hasNoKernel && (n = e.kernelDisplayName);
-                    const a = [s.Dialog.cancelButton({
+                    const s = [a.Dialog.cancelButton({
                             label: n
-                        }), s.Dialog.okButton({
+                        }), a.Dialog.okButton({
                             label: t.__("Select"),
                             ariaLabel: t.__("Select Kernel"),
                             className: "jp-KernelSelector-SelectButton"
                         })],
                         o = e.kernelPreference.autoStartDefault,
                         r = "boolean" == typeof o,
                         l = await this.options.settingRegistry.load(k),
-                        c = new s.Dialog({
+                        i = new a.Dialog({
                             title: t.__("Select Kernel"),
-                            body: new R({
+                            body: new O({
                                 data: {
                                     specs: e.specsManager.specs,
                                     sessions: e.sessionManager.running(),
                                     preference: e.kernelPreference
                                 },
                                 name: e.name,
                                 commands: this.options.commands,
                                 favoritesDatabase: this.options.database.favorites,
                                 lastUsedDatabase: this.options.database.lastUsed,
                                 settings: l,
                                 trans: t,
                                 acceptDialog: () => {
-                                    c.resolve(1)
+                                    i.resolve(1)
                                 },
                                 type: e.type
                             }),
-                            buttons: a,
+                            buttons: s,
                             checkbox: r ? {
                                 label: t.__("Always start the preferred kernel"),
                                 caption: t.__("Remember my choice and always start the preferred kernel"),
                                 checked: o
                             } : null
                         });
-                    c.node.classList.add("jp-KernelSelector-Dialog");
-                    const i = await c.launch();
-                    if (e.isDisposed || !i.button.accept) return;
-                    r && null !== i.isChecked && (e.kernelPreference = {
+                    i.node.classList.add("jp-KernelSelector-Dialog");
+                    const c = await i.launch();
+                    if (e.isDisposed || !c.button.accept) return;
+                    r && null !== c.isChecked && (e.kernelPreference = {
                         ...e.kernelPreference,
-                        autoStartDefault: i.isChecked
+                        autoStartDefault: c.isChecked
                     });
-                    const d = i.value;
+                    const d = c.value;
                     if (null === d && !e.hasNoKernel) return e.shutdown();
                     d && await e.changeKernel(d)
                 }
             }
-            const A = {
+            const R = {
                 id: "jupyterlab-new-launcher:dialogs",
                 description: "Session dialogs for redesigned JupyterLab launcher",
-                provides: s.ISessionContextDialogs,
+                provides: a.ISessionContextDialogs,
                 autoStart: !0,
-                requires: [c.ITranslator, D, l.ISettingRegistry],
-                activate: (e, t, n, a) => new T({
+                requires: [i.ITranslator, N, l.ISettingRegistry],
+                activate: (e, t, n, s) => new T({
                     translator: t,
                     database: n,
                     commands: e.commands,
-                    settingRegistry: a
+                    settingRegistry: s
                 })
             };
-            class R extends s.ReactWidget {
+            class O extends a.ReactWidget {
                 constructor(e) {
                     super(), this.options = e, this.renderKernelCommand = e => new v({
                         item: e,
                         cwd: "",
                         commands: this.commands,
                         lastUsedDatabase: this._lastUsedDatabase,
                         favoritesDatabase: this._favoritesDatabase
@@ -776,20 +806,20 @@
                         this.node.style.minWidth = e.width + "px", this.node.style.minHeight = e.height + "px"
                     }))
                 }
                 render() {
                     var e;
                     const t = [],
                         n = this.options.data.specs.kernelspecs,
-                        a = "console" === this.options.type ? "console:create" : "notebook:create-new";
+                        s = "console" === this.options.type ? "console:create" : "notebook:create-new";
                     for (const e of Object.values(n)) {
                         if (!e) continue;
                         const n = e.resources["logo-svg"] || e.resources["logo-64x64"];
                         t.push({
-                            command: a,
+                            command: s,
                             args: "console" === this.options.type ? {
                                 isLauncher: !0,
                                 kernelPreference: {
                                     name: e.name
                                 }
                             } : {
                                 isLauncher: !0,
@@ -797,22 +827,22 @@
                             },
                             kernelIconUrl: n,
                             metadata: {
                                 kernel: C.JSONExt.deepCopy(e.metadata || {})
                             }
                         })
                     }
-                    const s = [];
+                    const a = [];
                     for (const t of this.options.data.sessions) {
                         const o = t.kernel;
                         if (!o) continue;
                         const r = n[o.name],
                             l = r.resources["logo-svg"] || r.resources["logo-64x64"];
-                        s.push({
-                            command: a,
+                        a.push({
+                            command: s,
                             args: "console" === this.options.type ? {
                                 isLauncher: !0,
                                 kernelPreference: {
                                     name: r.name
                                 }
                             } : {
                                 isLauncher: !0,
@@ -826,15 +856,15 @@
                                     "used by": t.name
                                 },
                                 model: o
                             }
                         })
                     }
                     const o = t.map(this.renderKernelCommand),
-                        r = s.map(this.renderKernelCommand);
+                        r = a.map(this.renderKernelCommand);
                     return m.createElement(m.Fragment, null, m.createElement("h3", {
                         className: "jp-KernelSelector-Section"
                     }, this.trans.__('Start a new kernel for "%1"', this._name)), m.createElement(U, {
                         trans: this.trans,
                         commands: this.commands,
                         items: o,
                         settings: this._settings,
@@ -865,42 +895,61 @@
                 getValue() {
                     var e;
                     return this._selection ? (this._selection.markAsUsedNow().catch(console.warn), (null === (e = this._selection.metadata) || void 0 === e ? void 0 : e.model) ? this._selection.metadata.model : {
                         name: this._selection.args.kernelName
                     }) : null
                 }
             }
-            var z = n(101);
-            class O {
+            var z = n(590);
+            async function H(e = "", t = {}) {
+                const n = z.ServerConnection.makeSettings(),
+                    s = b.URLExt.join(n.baseUrl, "jupyterlab-new-launcher", e);
+                let a;
+                try {
+                    a = await z.ServerConnection.makeRequest(s, t, n)
+                } catch (e) {
+                    throw new z.ServerConnection.NetworkError(e)
+                }
+                let o = await a.text();
+                if (o.length > 0) try {
+                    o = JSON.parse(o)
+                } catch (e) {
+                    console.log("Not a JSON response body.", a)
+                }
+                if (!a.ok) throw new z.ServerConnection.ResponseError(a, o.message || o);
+                return o
+            }
+            class P {
                 constructor(e) {
-                    this._updateDB = async () => {
-                        const e = await this._fetch();
-                        this._db = e
-                    }, this._db = null, this._stateDB = e.stateDB;
+                    this._db = null, this._stateDB = e.stateDB;
                     const t = new C.PromiseDelegate;
-                    this.ready = t.promise, this._updateDB().then((() => t.resolve())), window.setInterval(this._updateDB, e.fetchInterval)
+                    this.ready = t.promise, window.setTimeout((() => this._updateDB().then((() => t.resolve()))), 0), window.setInterval(this._updateDB.bind(this), e.fetchInterval)
                 }
                 _get(e) {
                     return this._db ? this._db[this._itemKey(e)] : (console.error("Database is not ready!"), null)
                 }
                 async _set(e, t) {
                     const n = await this._fetch();
                     this._db = n, n[this._itemKey(e)] = t, await this._stateDB.save(this._stateDBKey, n)
                 }
+                async _updateDB() {
+                    const e = await this._fetch();
+                    this._db = e
+                }
                 async _fetch() {
                     let e = await this._stateDB.fetch(this._stateDBKey);
                     return void 0 === e && (e = await this._stateDB.fetch(this._stateDBKey)), void 0 === e ? {} : e
                 }
             }
-            class H extends O {
+            class F extends P {
                 _itemKey(e) {
                     return e.command + "_" + JSON.stringify(e.args)
                 }
             }
-            class F extends H {
+            class q extends F {
                 constructor() {
                     super(...arguments), this._stateDBKey = "new-launcher:last-used", this._changed = new f.Signal(this)
                 }
                 get(e) {
                     const t = super._get(e);
                     return t ? new Date(t) : null
                 }
@@ -910,58 +959,74 @@
                 async recordAsUsed(e, t) {
                     await this._set(e, t.toUTCString()), this._changed.emit()
                 }
                 get changed() {
                     return this._changed
                 }
             }
-            class P extends H {
+            class W extends F {
                 constructor() {
                     super(...arguments), this._stateDBKey = "new-launcher:favorites", this._changed = new f.Signal(this)
                 }
                 get(e) {
                     var t;
                     return null !== (t = super._get(e)) && void 0 !== t ? t : null
                 }
                 async set(e, t) {
                     await this._set(e, t), this._changed.emit()
                 }
                 get changed() {
                     return this._changed
                 }
             }
-            const q = {
+            class V {
+                constructor() {
+                    this._endpointsMap = {
+                        "new-launcher:favorites": "database/favorites",
+                        "new-launcher:last-used": "database/last-used"
+                    }
+                }
+                async fetch(e) {
+                    return console.log("endpoint", e, this._endpointsMap[e], this._endpointsMap), await H(this._endpointsMap[e])
+                }
+                async save(e, t) {
+                    await H(this._endpointsMap[e], {
+                        method: "POST",
+                        body: JSON.stringify(t)
+                    })
+                }
+            }
+            const J = {
                     id: "jupyterlab-new-launcher:database",
                     description: "A redesigned JupyterLab launcher databases",
-                    provides: D,
+                    provides: N,
                     autoStart: !0,
-                    requires: [z.IStateDB],
-                    activate: (e, t) => {
-                        const n = {
-                            stateDB: t,
+                    activate: e => {
+                        const t = {
+                            stateDB: new V,
                             fetchInterval: 1e4
                         };
                         return {
-                            lastUsed: new F(n),
-                            favorites: new P(n)
+                            lastUsed: new q(t),
+                            favorites: new W(t)
                         }
                     }
                 },
-                W = [{
+                Z = [{
                     id: k,
                     description: "A redesigned JupyterLab launcher",
                     provides: r.ILauncher,
                     autoStart: !0,
-                    requires: [c.ITranslator, l.ISettingRegistry, D],
-                    optional: [a.ILabShell, s.ICommandPalette, o.IDefaultFileBrowser],
-                    activate: function(e, t, n, a, o, l, c) {
+                    requires: [i.ITranslator, l.ISettingRegistry, N],
+                    optional: [s.ILabShell, a.ICommandPalette, o.IDefaultFileBrowser],
+                    activate: function(e, t, n, s, o, r, l) {
                         const {
-                            commands: m,
-                            shell: u
-                        } = e, h = t.load("jupyterlab-new-launcher"), p = new r.LauncherModel;
+                            commands: i,
+                            shell: m
+                        } = e, u = t.load("jupyterlab-new-launcher"), h = new A;
                         if (-1 !== navigator.userAgent.indexOf("AppleWebKit") && -1 === navigator.userAgent.indexOf("Chrome")) {
                             const e = function(e) {
                                 const t = document.createElement("style");
                                 return t.setAttribute("type", "text/css"), t.appendChild(document.createTextNode(".jp-starIconButton {\n  /* do not rotate on webkit as the result is off when zoomed in see https://bugs.webkit.org/show_bug.cgi?id=194903 */\n  --jp-transition-transform: rotate(0deg);\n}\n\n.jp-starIcon .jp-star-filled,\n.jp-starIcon .jp-star-border {\n  /* disable animation on webkit */\n  transition-property: none;\n}\n")), t
                             }();
                             document.body.appendChild(e)
                         }
@@ -974,119 +1039,119 @@
                                             const t = e.id;
                                             return t[0].toLocaleUpperCase() + t.substring(1)
                                         }
                                         return t.__("Toggle given column")
                                     },
                                     execute: async e => {
                                         var t;
-                                        const a = e.id;
-                                        if (!a) return console.error("Column ID missing");
-                                        const s = null !== (t = n.composite.hiddenColumns) && void 0 !== t ? t : {};
-                                        "visible" !== s[a] && s[a] ? s[a] = "visible" : s[a] = "hidden", await n.set("hiddenColumns", s)
+                                        const s = e.id;
+                                        if (!s) return console.error("Column ID missing");
+                                        const a = null !== (t = n.composite.hiddenColumns) && void 0 !== t ? t : {};
+                                        "visible" !== a[s] && a[s] ? a[s] = "visible" : a[s] = "hidden", await n.set("hiddenColumns", a)
                                     },
                                     isToggleable: !0,
                                     isToggled: e => {
                                         var t;
-                                        const a = e.id;
-                                        return a ? "hidden" !== (null !== (t = n.composite.hiddenColumns) && void 0 !== t ? t : {})[a] : (console.error("Column ID missing for checking if toggled"), !1)
+                                        const s = e.id;
+                                        return s ? "hidden" !== (null !== (t = n.composite.hiddenColumns) && void 0 !== t ? t : {})[s] : (console.error("Column ID missing for checking if toggled"), !1)
                                     }
                                 }), e.commands.addCommand(E.moveColumn, {
                                     label: e => "left" === e.direction ? t.__("Move Column Left") : "right" === e.direction ? t.__("Move Column Right") : t.__("Move column left or right"),
                                     execute: async e => {
                                         const t = e.order,
-                                            a = e.id,
-                                            s = t.indexOf(a),
-                                            o = s + ("left" === e.direction ? -1 : 1);
+                                            s = e.id,
+                                            a = t.indexOf(s),
+                                            o = a + ("left" === e.direction ? -1 : 1);
                                         if (o < 0 || o >= t.length) return void console.log("Cannot move the column any further");
                                         const r = t[o];
-                                        t[o] = a, t[s] = r, await n.set("columnOrder", t)
+                                        t[o] = s, t[a] = r, await n.set("columnOrder", t)
                                     }
                                 })
-                            }(e, h, t)
+                            }(e, u, t)
                         }));
-                        const g = {},
-                            f = async () => {
+                        const p = {},
+                            g = async () => {
                                 const t = [...e.serviceManager.sessions.running()];
                                 for (const e of t) {
                                     if (!e.kernel) continue;
                                     let t;
                                     t = "notebook" === e.type ? "notebook:create-new" : "console" === e.type ? "console:create" : "unknown";
                                     const n = t + "-" + e.kernel.name,
-                                        s = e.kernel.last_activity;
-                                    if (s && g[n] !== s) {
-                                        g[n] = s;
+                                        a = e.kernel.last_activity;
+                                    if (a && p[n] !== a) {
+                                        p[n] = a;
                                         const o = {
                                             command: t,
                                             args: {
                                                 isLauncher: !0,
                                                 kernelName: e.kernel.name
                                             }
                                         };
-                                        await a.lastUsed.recordAsUsed(o, new Date(s))
+                                        await s.lastUsed.recordAsUsed(o, new Date(a))
                                     }
                                 }
                             };
-                        return e.serviceManager.sessions.ready.then(f), e.serviceManager.sessions.runningChanged.connect(f), m.addCommand(E.create, {
-                            label: h.__("New Launcher"),
-                            icon: e => e.toolbar ? i.addIcon : void 0,
+                        return e.serviceManager.sessions.ready.then(g), e.serviceManager.sessions.runningChanged.connect(g), i.addCommand(E.create, {
+                            label: u.__("New Launcher"),
+                            icon: e => e.toolbar ? c.addIcon : void 0,
                             execute: async e => {
-                                var r, l;
-                                const g = null !== (l = null !== (r = e.cwd) && void 0 !== r ? r : null == c ? void 0 : c.model.path) && void 0 !== l ? l : "",
-                                    f = "launcher-" + V.id++,
+                                var r, p;
+                                const g = null !== (p = null !== (r = e.cwd) && void 0 !== r ? r : null == l ? void 0 : l.model.path) && void 0 !== p ? p : "",
+                                    f = "launcher-" + $.id++,
                                     v = await n.load(k);
-                                await Promise.all([a.lastUsed.ready, a.favorites.ready]);
+                                await Promise.all([s.lastUsed.ready, s.favorites.ready]);
                                 const b = new M({
-                                    model: p,
+                                    model: h,
                                     cwd: g,
                                     callback: e => {
-                                        (0, d.find)(u.widgets("main"), (t => t === e)) && (u.add(e, "main", {
+                                        (0, d.find)(m.widgets("main"), (t => t === e)) && (m.add(e, "main", {
                                             ref: f
                                         }), b.dispose())
                                     },
-                                    commands: m,
+                                    commands: i,
                                     translator: t,
-                                    lastUsedDatabase: a.lastUsed,
-                                    favoritesDatabase: a.favorites,
+                                    lastUsedDatabase: s.lastUsed,
+                                    favoritesDatabase: s.favorites,
                                     settings: v
                                 });
-                                b.model = p, b.title.icon = i.launcherIcon, b.title.label = h.__("Launcher");
-                                const _ = new s.MainAreaWidget({
+                                b.model = h, b.title.icon = c.launcherIcon, b.title.label = u.__("Launcher");
+                                const _ = new a.MainAreaWidget({
                                     content: b
                                 });
-                                if (_.title.closable = !!Array.from(u.widgets("main")).length, _.id = f, u.add(_, "main", {
+                                if (_.title.closable = !!Array.from(m.widgets("main")).length, _.id = f, m.add(_, "main", {
                                         activate: e.activate,
                                         ref: e.ref
                                     }), o && o.layoutModified.connect((() => {
                                         _.title.closable = Array.from(o.widgets("main")).length > 1
-                                    }), _), c) {
+                                    }), _), l) {
                                     const e = e => {
                                         b.cwd = e.path
                                     };
-                                    c.model.pathChanged.connect(e), b.disposed.connect((() => {
-                                        c.model.pathChanged.disconnect(e)
+                                    l.model.pathChanged.connect(e), b.disposed.connect((() => {
+                                        l.model.pathChanged.disconnect(e)
                                     }))
                                 }
                                 return _
                             }
-                        }), o && Promise.all([e.restored, null == c ? void 0 : c.model.restored]).then((() => {
+                        }), o && Promise.all([e.restored, null == l ? void 0 : l.model.restored]).then((() => {
                             o.layoutModified.connect((() => {
-                                o.isEmpty("main") && m.execute(E.create)
+                                o.isEmpty("main") && i.execute(E.create)
                             }))
-                        })), l && l.addItem({
+                        })), r && r.addItem({
                             command: E.create,
-                            category: h.__("Launcher")
+                            category: u.__("Launcher")
                         }), o && (o.addButtonEnabled = !0, o.addRequested.connect(((e, t) => {
                             var n;
-                            const a = (null === (n = t.currentTitle) || void 0 === n ? void 0 : n.owner.id) || t.titles[t.titles.length - 1].owner.id;
-                            return m.execute(E.create, {
-                                ref: a
+                            const s = (null === (n = t.currentTitle) || void 0 === n ? void 0 : n.owner.id) || t.titles[t.titles.length - 1].owner.id;
+                            return i.execute(E.create, {
+                                ref: s
                             })
-                        }))), p
+                        }))), h
                     }
-                }, A, q];
-            var V;
+                }, R, J];
+            var $;
             ! function(e) {
                 e.id = 0
-            }(V || (V = {}))
+            }($ || ($ = {}))
         }
     }
 ]);
```

### Comparing `jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/labextension/static/remoteEntry.a10a814d39706cd65aea.js` & `jupyterlab_new_launcher-0.4.0/jupyterlab_new_launcher/labextension/static/remoteEntry.36348165586c2a5361a1.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, n, a, o, i, u, l, f, s, d, p, c, h, v, b, g = {
             795: (e, r, t) => {
                 var n = {
-                        "./index": () => t.e(787).then((() => () => t(787))),
-                        "./extension": () => t.e(787).then((() => () => t(787))),
+                        "./index": () => t.e(252).then((() => () => t(252))),
+                        "./extension": () => t.e(252).then((() => () => t(252))),
                         "./style": () => t.e(728).then((() => () => t(728)))
                     },
                     a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
@@ -43,19 +43,19 @@
         }), r
     }, m.d = (e, r) => {
         for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
-        728: "5be4ee0b94a07decd5f8",
-        787: "27ef72da905b049778be"
+        252: "6edb090ef613ff9206b6",
+        728: "54b87b26a387a46f2b0d"
     } [e] + ".js?v=" + {
-        728: "5be4ee0b94a07decd5f8",
-        787: "27ef72da905b049778be"
+        252: "6edb090ef613ff9206b6",
+        728: "54b87b26a387a46f2b0d"
     } [e], m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -102,19 +102,19 @@
                 var o = m.S[t],
                     i = "jupyterlab-new-launcher",
                     u = [];
                 return "default" === t && ((e, r, t, n) => {
                     var a = o[e] = o[e] || {},
                         u = a[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (a[r] = {
-                        get: () => m.e(787).then((() => () => m(787))),
+                        get: () => m.e(252).then((() => () => m(252))),
                         from: i,
                         eager: !1
                     })
-                })("jupyterlab-new-launcher", "0.3.3"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("jupyterlab-new-launcher", "0.4.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         m.g.importScripts && (e = m.g.location + "");
         var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -209,28 +209,28 @@
     }, s = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, d = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, a) {
         var o = m.I(r);
         return o && o.then ? o.then(e.bind(e, r, m.S[r], t, n, a)) : e(r, m.S[r], t, n)
     })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), c = {}, h = {
         53: () => p("default", "@lumino/algorithm", [1, 2, 0, 0]),
-        101: () => p("default", "@jupyterlab/statedb", [1, 4, 2, 0]),
-        260: () => p("default", "@jupyterlab/launcher", [1, 4, 2, 0]),
+        107: () => p("default", "@jupyterlab/launcher", [1, 4, 2, 1]),
+        201: () => p("default", "@jupyterlab/application", [1, 4, 2, 1]),
+        218: () => p("default", "@jupyterlab/settingregistry", [1, 4, 2, 1]),
         262: () => p("default", "@lumino/coreutils", [1, 2, 0, 0]),
-        265: () => p("default", "@jupyterlab/translation", [1, 4, 2, 0]),
         345: () => p("default", "react", [1, 18, 2, 0]),
-        527: () => p("default", "@jupyterlab/ui-components", [1, 4, 2, 0]),
+        420: () => p("default", "@jupyterlab/apputils", [1, 4, 3, 1]),
+        445: () => p("default", "@jupyterlab/coreutils", [1, 6, 2, 1]),
+        450: () => p("default", "@jupyterlab/translation", [1, 4, 2, 1]),
+        590: () => p("default", "@jupyterlab/services", [1, 7, 2, 1]),
         602: () => p("default", "@lumino/signaling", [1, 2, 0, 0]),
-        626: () => p("default", "@jupyterlab/application", [1, 4, 2, 0]),
-        670: () => p("default", "@jupyterlab/filebrowser", [1, 4, 2, 0]),
-        702: () => p("default", "@jupyterlab/coreutils", [1, 6, 2, 0]),
-        825: () => p("default", "@jupyterlab/settingregistry", [1, 4, 2, 0]),
-        923: () => p("default", "@jupyterlab/apputils", [1, 4, 3, 0])
+        760: () => p("default", "@jupyterlab/ui-components", [1, 4, 2, 1]),
+        989: () => p("default", "@jupyterlab/filebrowser", [1, 4, 2, 1])
     }, v = {
-        787: [53, 101, 260, 262, 265, 345, 527, 602, 626, 670, 702, 825, 923]
+        252: [53, 107, 201, 218, 262, 345, 420, 445, 450, 590, 602, 760, 989]
     }, b = {}, m.f.consumes = (e, r) => {
         m.o(v, e) && v[e].forEach((e => {
             if (m.o(c, e)) return r.push(c[e]);
             if (!b[e]) {
                 var t = r => {
                     c[e] = 0, m.m[e] = t => {
                         delete m.c[e], t.exports = r()
```

### Comparing `jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/labextension/static/third-party-licenses.json` & `jupyterlab_new_launcher-0.4.0/jupyterlab_new_launcher/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.3/schema/plugin.json` & `jupyterlab_new_launcher-0.4.0/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.3/src/commands.ts` & `jupyterlab_new_launcher-0.4.0/src/commands.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.3/src/database.ts` & `jupyterlab_new_launcher-0.4.0/src/database.ts`

 * *Files 21% similar despite different names*

```diff
@@ -7,41 +7,45 @@
   IFavoritesDatabase,
   ILauncherDatabase
 } from './types';
 import {
   JupyterFrontEnd,
   JupyterFrontEndPlugin
 } from '@jupyterlab/application';
+import { requestAPI } from './handler';
+
+type SimpleDB = Omit<IStateDB, 'list' | 'toJSON' | 'remove'>;
 
 abstract class Database<V extends ReadonlyPartialJSONValue, K> {
   ready: Promise<void>;
-  constructor(options: { stateDB: IStateDB; fetchInterval: number }) {
+  constructor(options: { stateDB: SimpleDB; fetchInterval: number }) {
     this._stateDB = options.stateDB;
     const ready = new PromiseDelegate<void>();
     this.ready = ready.promise;
-    this._updateDB().then(() => ready.resolve());
-    window.setInterval(this._updateDB, options.fetchInterval);
+    // delay until the child class is ready (so that _stateDBKey is there)
+    window.setTimeout(() => this._updateDB().then(() => ready.resolve()), 0);
+    window.setInterval(this._updateDB.bind(this), options.fetchInterval);
   }
   protected _get(item: K) {
     if (!this._db) {
       console.error('Database is not ready!');
       return null;
     }
     return this._db[this._itemKey(item)];
   }
   protected async _set(item: K, value: V) {
     const db = await this._fetch();
     this._db = db;
     db[this._itemKey(item)] = value;
     await this._stateDB.save(this._stateDBKey, db);
   }
-  private _updateDB = async () => {
+  private async _updateDB() {
     const db = await this._fetch();
     this._db = db;
-  };
+  }
   private async _fetch(): Promise<Record<string, V>> {
     let db = (await this._stateDB.fetch(this._stateDBKey)) as
       | Record<string, V>
       | undefined;
     if (typeof db === 'undefined') {
       // retry once: sometimes state DB does not load up on first try
       db = (await this._stateDB.fetch(this._stateDBKey)) as
@@ -52,30 +56,30 @@
       return {};
     }
     return db;
   }
   protected abstract _itemKey(item: K): string;
   protected abstract _stateDBKey: string;
   private _db: Record<string, V> | null = null;
-  private _stateDB: IStateDB;
+  private _stateDB: SimpleDB;
 }
 
 export abstract class ItemDatabase<
   V extends ReadonlyPartialJSONValue
 > extends Database<V, ILauncher.IItemOptions> {
   protected _itemKey(item: ILauncher.IItemOptions): string {
     return item.command + '_' + JSON.stringify(item.args);
   }
 }
 
 export class LastUsedDatabase
   extends ItemDatabase<string>
   implements ILastUsedDatabase
 {
-  protected _stateDBKey = 'new-launcher:last-used';
+  protected readonly _stateDBKey = 'new-launcher:last-used';
 
   get(item: ILauncher.IItemOptions) {
     const date = super._get(item);
     return date ? new Date(date) : null;
   }
 
   async recordAsUsedNow(item: ILauncher.IItemOptions) {
@@ -94,15 +98,15 @@
   private _changed = new Signal<LastUsedDatabase, void>(this);
 }
 
 export class FavoritesDatabase
   extends ItemDatabase<boolean>
   implements IFavoritesDatabase
 {
-  protected _stateDBKey = 'new-launcher:favorites';
+  protected readonly _stateDBKey = 'new-launcher:favorites';
 
   get(item: ILauncher.IItemOptions) {
     return super._get(item) ?? null;
   }
 
   async set(item: ILauncher.IItemOptions, isFavourite: boolean) {
     await this._set(item, isFavourite);
@@ -112,26 +116,49 @@
   get changed() {
     return this._changed;
   }
 
   private _changed = new Signal<FavoritesDatabase, void>(this);
 }
 
+type DatabaseId = 'new-launcher:favorites' | 'new-launcher:last-used';
+
+class SingletonStateDB<
+  T extends ReadonlyPartialJSONValue = ReadonlyPartialJSONValue
+> implements SimpleDB
+{
+  async fetch(id: DatabaseId): Promise<T | undefined> {
+    console.log('endpoint', id, this._endpointsMap[id], this._endpointsMap);
+    return await requestAPI<T>(this._endpointsMap[id]);
+  }
+
+  async save(id: DatabaseId, value: T): Promise<any> {
+    await requestAPI<T>(this._endpointsMap[id], {
+      method: 'POST',
+      body: JSON.stringify(value)
+    });
+  }
+
+  private _endpointsMap = {
+    'new-launcher:favorites': 'database/favorites',
+    'new-launcher:last-used': 'database/last-used'
+  };
+}
+
 /**
  * Initialization data for the jupyterlab-new-launcher extension.
  */
 export const databasePlugin: JupyterFrontEndPlugin<ILauncherDatabase> = {
   id: 'jupyterlab-new-launcher:database',
   description: 'A redesigned JupyterLab launcher databases',
   provides: ILauncherDatabase,
   autoStart: true,
-  requires: [IStateDB],
-  activate: (app: JupyterFrontEnd, stateDB: IStateDB) => {
+  activate: (app: JupyterFrontEnd) => {
     const databaseOptions = {
-      stateDB,
+      stateDB: new SingletonStateDB(),
       fetchInterval: 10000
     };
     return {
       lastUsed: new LastUsedDatabase(databaseOptions),
       favorites: new FavoritesDatabase(databaseOptions)
     };
   }
```

### Comparing `jupyterlab_new_launcher-0.3.3/src/dialogs.tsx` & `jupyterlab_new_launcher-0.4.0/src/dialogs.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.3/src/icons.ts` & `jupyterlab_new_launcher-0.4.0/src/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.3/src/index.ts` & `jupyterlab_new_launcher-0.4.0/src/index.ts`

 * *Files 3% similar despite different names*

```diff
@@ -3,23 +3,29 @@
 import {
   ILabShell,
   JupyterFrontEnd,
   JupyterFrontEndPlugin
 } from '@jupyterlab/application';
 import { ICommandPalette, MainAreaWidget } from '@jupyterlab/apputils';
 import { FileBrowserModel, IDefaultFileBrowser } from '@jupyterlab/filebrowser';
-import { ILauncher, LauncherModel } from '@jupyterlab/launcher';
+import { ILauncher } from '@jupyterlab/launcher';
 import { ISettingRegistry } from '@jupyterlab/settingregistry';
 import { ITranslator } from '@jupyterlab/translation';
 import { addIcon, launcherIcon } from '@jupyterlab/ui-components';
 import { find } from '@lumino/algorithm';
 import { ReadonlyPartialJSONObject } from '@lumino/coreutils';
 import { DockPanel, TabBar, Widget } from '@lumino/widgets';
 import { NewLauncher as Launcher } from './launcher';
-import { CommandIDs, ILauncherDatabase, MAIN_PLUGIN_ID } from './types';
+import { NewModel as Model } from './model';
+import {
+  CommandIDs,
+  ILauncherDatabase,
+  INewLauncher,
+  MAIN_PLUGIN_ID
+} from './types';
 import { addCommands } from './commands';
 import { sessionDialogsPlugin } from './dialogs';
 import { databasePlugin } from './database';
 import webkitCSSPatch from '../style/webkit.raw.css';
 
 /**
  * Initialization data for the jupyterlab-new-launcher extension.
@@ -50,18 +56,18 @@
   app: JupyterFrontEnd,
   translator: ITranslator,
   settingRegistry: ISettingRegistry,
   database: ILauncherDatabase,
   labShell: ILabShell | null,
   palette: ICommandPalette | null,
   defaultBrowser: IDefaultFileBrowser | null
-): ILauncher {
+): INewLauncher {
   const { commands, shell } = app;
   const trans = translator.load('jupyterlab-new-launcher');
-  const model = new LauncherModel();
+  const model = new Model();
 
   if (
     navigator.userAgent.indexOf('AppleWebKit') !== -1 &&
     navigator.userAgent.indexOf('Chrome') === -1
   ) {
     const style = createStyleSheet(webkitCSSPatch);
     document.body.appendChild(style);
```

### Comparing `jupyterlab_new_launcher-0.3.3/src/item.ts` & `jupyterlab_new_launcher-0.4.0/src/item.ts`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
         (kernel['conda_env_name'] as string | undefined) ?? ''
       ).match(/(?<namespace>.+)-(?<duplicate>\1)-(?<environment>.+)/);
       if (condaStoreMatch && this.metadata) {
         const groups = condaStoreMatch.groups!;
         this.label =
           (kernel['conda_language'] as string | undefined) ??
           groups.environment;
+        delete kernel['conda_env_name'];
         this.metadata = {
           ...this.metadata,
           kernel: {
             Namespace: groups.namespace,
             conda_env_name: groups.environment,
             ...kernel
           }
```

### Comparing `jupyterlab_new_launcher-0.3.3/src/launcher.tsx` & `jupyterlab_new_launcher-0.4.0/src/launcher.tsx`

 * *Files 10% similar despite different names*

```diff
@@ -7,20 +7,22 @@
 import { TranslationBundle } from '@jupyterlab/translation';
 import {
   FilterBox,
   notebookIcon,
   consoleIcon
 } from '@jupyterlab/ui-components';
 import * as React from 'react';
+import { NewModel } from './model';
 import {
   IItem,
   IKernelItem,
   ILastUsedDatabase,
   IFavoritesDatabase,
-  ISettingsLayout
+  ISettingsLayout,
+  ISectionOptions
 } from './types';
 import { fileIcon, starIcon } from './icons';
 import { Item } from './item';
 import { KernelTable } from './components/table';
 import { CollapsibleSection } from './components/section';
 import { TypeCard } from './components/card';
 
@@ -31,14 +33,15 @@
   notebookItems: IKernelItem[];
   consoleItems: IKernelItem[];
   otherItems: IItem[];
   commands: CommandRegistry;
   settings: ISettingRegistry.ISettings;
   favouritesChanged: ISignal<IFavoritesDatabase, void>;
   lastUsedChanged: ISignal<ILastUsedDatabase, void>;
+  sections: ISectionOptions[];
 }): React.ReactElement {
   const { trans, cwd, typeItems, otherItems, favouritesChanged } = props;
   const [query, updateQuery] = React.useState<string>('');
   const [, forceUpdate] = React.useReducer(x => x + 1, 0);
   const [showStarred, updateShowStarred] = React.useState<
     ISettingsLayout['starredSection']
   >(
@@ -100,142 +103,169 @@
   const starred = [...props.notebookItems, ...props.consoleItems].filter(
     item => item.starred
   );
 
   const startCollapsed = props.settings.composite
     .collapsedSections as ISettingsLayout['collapsedSections'];
 
-  return (
-    <div className="jp-LauncherBody">
-      <div className="jp-NewLauncher-TopBar">
-        <div className="jp-Launcher-cwd">
-          <h3>
-            {trans.__('Current folder:')} <code>{cwd ? cwd : '/'}</code>
-          </h3>
-        </div>
-        <div className="jp-NewLauncher-OtherItems">
-          {otherItems.map(item => (
-            <TypeCard item={item} trans={trans} />
-          ))}
-        </div>
-      </div>
-      {searchAll ? (
-        <div className="jp-Launcher-searchBox">
-          <FilterBox
-            placeholder={trans.__('Filter')}
-            updateFilter={(_, query) => {
-              updateQuery(query ?? '');
-            }}
-            initialQuery={''}
-            useFuzzyFilter={false}
-          />
-        </div>
-      ) : null}
-      <CollapsibleSection
-        className="jp-Launcher-openByType"
-        title={trans.__('Create Empty')}
-        icon={fileIcon}
-        open={startCollapsed['create-empty'] !== 'collapsed'}
-      >
-        {typeItems
+  const builtinSections: ISectionOptions[] = [
+    {
+      className: 'jp-Launcher-openByType',
+      title: trans.__('Create Empty'),
+      icon: fileIcon,
+      id: 'create-empty',
+      rank: 1,
+      render: () =>
+        typeItems
           .filter(
             item =>
               !query ||
               item.label.toLowerCase().indexOf(query.toLowerCase()) !== -1
           )
-          .map(item => (
-            <TypeCard item={item} trans={trans} />
-          ))}
-      </CollapsibleSection>
-      {showStarred ? (
-        <CollapsibleSection
-          className="jp-Launcher-openByKernel"
-          title={trans.__('Starred')}
-          icon={starIcon}
-          open={startCollapsed['starred'] !== 'collapsed'}
-        >
-          {starred.length > 0 ? (
-            <KernelTable
-              items={starred}
-              commands={props.commands}
-              showSearchBox={!searchAll}
-              showWidgetType={true}
-              query={query}
-              settings={props.settings}
-              trans={trans}
-              onClick={item => item.execute()}
-              favouritesChanged={props.favouritesChanged}
-              lastUsedChanged={props.lastUsedChanged}
-            />
-          ) : (
-            'No starred items'
-          )}
-        </CollapsibleSection>
-      ) : null}
-      <CollapsibleSection
-        className="jp-Launcher-openByKernel jp-Launcher-launchNotebook"
-        title={trans.__('Launch New Notebook')}
-        icon={notebookIcon}
-        open={startCollapsed['launch-notebook'] !== 'collapsed'}
-      >
+          .map(item => <TypeCard item={item} trans={trans} />)
+    },
+    {
+      className: 'jp-Launcher-openByKernel jp-Launcher-launchNotebook',
+      title: trans.__('Launch New Notebook'),
+      icon: notebookIcon,
+      id: 'launch-notebook',
+      rank: 3,
+      render: () => (
         <KernelTable
           items={props.notebookItems}
           commands={props.commands}
           showSearchBox={!searchAll}
           query={query}
           settings={props.settings}
           trans={trans}
           onClick={item => item.execute()}
           favouritesChanged={props.favouritesChanged}
           lastUsedChanged={props.lastUsedChanged}
         />
-      </CollapsibleSection>
-      <CollapsibleSection
-        className="jp-Launcher-openByKernel jp-Launcher-launchConsole"
-        title={trans.__('Launch New Console')}
-        icon={consoleIcon}
-        open={startCollapsed['launch-console'] !== 'collapsed'}
-      >
+      )
+    },
+    {
+      className: 'jp-Launcher-openByKernel jp-Launcher-launchConsole',
+      title: trans.__('Launch New Console'),
+      icon: consoleIcon,
+      id: 'launch-console',
+      rank: 5,
+      render: () => (
         <KernelTable
           items={props.consoleItems}
           commands={props.commands}
           showSearchBox={!searchAll}
           query={query}
           settings={props.settings}
           trans={trans}
           onClick={item => item.execute()}
           favouritesChanged={props.favouritesChanged}
           lastUsedChanged={props.lastUsedChanged}
         />
-      </CollapsibleSection>
+      )
+    }
+  ];
+  if (showStarred) {
+    builtinSections.push({
+      className: 'jp-Launcher-openByKernel',
+      title: trans.__('Starred'),
+      icon: starIcon,
+      id: 'starred',
+      rank: 2,
+      render: () =>
+        starred.length > 0 ? (
+          <KernelTable
+            items={starred}
+            commands={props.commands}
+            showSearchBox={!searchAll}
+            showWidgetType={true}
+            query={query}
+            settings={props.settings}
+            trans={trans}
+            onClick={item => item.execute()}
+            favouritesChanged={props.favouritesChanged}
+            lastUsedChanged={props.lastUsedChanged}
+          />
+        ) : (
+          'No starred items'
+        )
+    });
+  }
+  const allSections = [...builtinSections, ...props.sections];
+
+  return (
+    <div className="jp-LauncherBody">
+      <div className="jp-NewLauncher-TopBar">
+        <div className="jp-Launcher-cwd">
+          <h3>
+            {trans.__('Current folder:')} <code>{cwd ? cwd : '/'}</code>
+          </h3>
+        </div>
+        <div className="jp-NewLauncher-OtherItems">
+          {otherItems.map(item => (
+            <TypeCard item={item} trans={trans} />
+          ))}
+        </div>
+      </div>
+      {searchAll ? (
+        <div className="jp-Launcher-searchBox">
+          <FilterBox
+            placeholder={trans.__('Filter')}
+            updateFilter={(_, query) => {
+              updateQuery(query ?? '');
+            }}
+            initialQuery={''}
+            useFuzzyFilter={false}
+          />
+        </div>
+      ) : null}
+      {allSections
+        .sort((a, b) => a.rank - b.rank)
+        .map(section => (
+          <CollapsibleSection
+            className={section.className}
+            title={section.title}
+            icon={section.icon}
+            open={startCollapsed[section.id] !== 'collapsed'}
+          >
+            {section.render()}
+          </CollapsibleSection>
+        ))}
     </div>
   );
 }
 
 export namespace NewLauncher {
   export interface IOptions extends ILauncher.IOptions {
     lastUsedDatabase: ILastUsedDatabase;
     favoritesDatabase: IFavoritesDatabase;
     settings: ISettingRegistry.ISettings;
+    model: NewModel;
   }
 }
 
 const SERVER_PROXY_COMMAND = 'server-proxy:open';
 
 export class NewLauncher extends Launcher {
   constructor(options: NewLauncher.IOptions) {
     super(options);
     this.commands = options.commands;
     this.trans = this.translator.load('jupyterlab-new-launcher');
     this._lastUsedDatabase = options.lastUsedDatabase;
     this._favoritesDatabase = options.favoritesDatabase;
     this._settings = options.settings;
+    this._newModel = options.model;
+    this._newModel.sectionAdded.connect(() => {
+      this.update();
+    });
   }
   private _lastUsedDatabase: ILastUsedDatabase;
   private _favoritesDatabase: IFavoritesDatabase;
+  private _newModel: NewModel;
+
   trans: TranslationBundle;
 
   renderCommand = (item: ILauncher.IItemOptions): IItem => {
     return new Item({
       item,
       cwd: this.cwd,
       commands: this.commands,
@@ -330,13 +360,14 @@
         typeItems={typeItems}
         notebookItems={notebookItems}
         consoleItems={consoleItems}
         otherItems={otherItems}
         settings={this._settings}
         favouritesChanged={this._favoritesDatabase.changed}
         lastUsedChanged={this._lastUsedDatabase.changed}
+        sections={this._newModel.sections}
       />
     );
   }
   protected commands: CommandRegistry;
   private _settings: ISettingRegistry.ISettings;
 }
```

### Comparing `jupyterlab_new_launcher-0.3.3/src/types.ts` & `jupyterlab_new_launcher-0.4.0/src/types.ts`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,30 @@
 // Copyright (c) Nebari Development Team.
 // Distributed under the terms of the Modified BSD License.
 import type { ILauncher } from '@jupyterlab/launcher';
 import type { VirtualElement } from '@lumino/virtualdom';
 import type { ISignal } from '@lumino/signaling';
 import { Token } from '@lumino/coreutils';
+import type { LabIcon } from '@jupyterlab/ui-components';
 
 export const MAIN_PLUGIN_ID = 'jupyterlab-new-launcher:plugin';
 
+export interface INewLauncher extends ILauncher {
+  addSection(options: ISectionOptions): void;
+}
+
+export interface ISectionOptions {
+  id: string;
+  title: string;
+  className: string;
+  icon: LabIcon;
+  render: () => React.ReactNode;
+  rank: number;
+}
+
 /**
  * The command IDs used by the launcher plugin.
  */
 export namespace CommandIDs {
   export const create = 'launcher:create';
   export const moveColumn = 'new-launcher:table-move-column';
   export const toggleColumn = 'new-launcher:table-toggle-column';
```

### Comparing `jupyterlab_new_launcher-0.3.3/src/components/base-table.tsx` & `jupyterlab_new_launcher-0.4.0/src/components/base-table.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.3/src/components/card.tsx` & `jupyterlab_new_launcher-0.4.0/src/components/card.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.3/src/components/section.tsx` & `jupyterlab_new_launcher-0.4.0/src/components/section.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.3/src/components/table.tsx` & `jupyterlab_new_launcher-0.4.0/src/components/table.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.3/style/base.css` & `jupyterlab_new_launcher-0.4.0/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.3/style/icons/code-server.svg` & `jupyterlab_new_launcher-0.4.0/style/icons/code-server.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.3/style/icons/md/LICENSE` & `jupyterlab_new_launcher-0.4.0/style/icons/md/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.3/ui-tests/README.md` & `jupyterlab_new_launcher-0.4.0/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.3/ui-tests/yarn.lock` & `jupyterlab_new_launcher-0.4.0/ui-tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.3/ui-tests/tests/jupyterlab_new_launcher.spec.ts` & `jupyterlab_new_launcher-0.4.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import { expect, test, galata } from '@jupyterlab/galata';
+import { Page } from '@playwright/test';
 
 const SETTINGS_ID = 'jupyterlab-new-launcher:plugin';
 
 test.describe('Default settings', () => {
   test('should render new launcher', async ({ page }) => {
     const launcher = page.locator('.jp-LauncherBody');
     expect(await launcher.screenshot()).toMatchSnapshot('launcher.png');
@@ -39,30 +40,36 @@
       [SETTINGS_ID]: {
         ...galata.DEFAULT_SETTINGS[SETTINGS_ID],
         starredSection: true
       }
     }
   });
 
+  const clickOnStars = async (page: Page) => {
+    await page
+      .locator('.jp-Launcher-launchNotebook .jp-starIconButton')
+      .click();
+    await page.locator('.jp-Launcher-launchConsole .jp-starIconButton').click();
+  };
+
   test('should render new launcher with starred section', async ({ page }) => {
     const launcher = page.locator('.jp-LauncherBody');
     // expand the console section
     await page.locator('.jp-Launcher-launchConsole summary').click();
     // star some items
-    await page
-      .locator('.jp-Launcher-launchNotebook .jp-starIconButton')
-      .click();
-    await page.locator('.jp-Launcher-launchConsole .jp-starIconButton').click();
+    await clickOnStars(page);
     // collapse the "create empty" section
     await page.locator('.jp-Launcher-openByType summary').click();
     // wait for animations to complete
     await page.waitForTimeout(400);
     expect(await launcher.screenshot()).toMatchSnapshot(
       'launcher-with-starred.png'
     );
+    // remove stars from the items
+    await clickOnStars(page);
   });
 });
 
 test.describe('Filter individual', () => {
   test.use({
     mockSettings: {
       ...galata.DEFAULT_SETTINGS,
```

### Comparing `jupyterlab_new_launcher-0.3.3/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-linux.png` & `jupyterlab_new_launcher-0.4.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.3/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-search-in-individual-linux.png` & `jupyterlab_new_launcher-0.4.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-search-in-individual-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.3/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-with-starred-linux.png` & `jupyterlab_new_launcher-0.4.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-with-starred-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.3/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/table-context-menu-linux.png` & `jupyterlab_new_launcher-0.4.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/table-context-menu-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.3/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/table-context-menu-visible-columns-linux.png` & `jupyterlab_new_launcher-0.4.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/table-context-menu-visible-columns-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.3/.gitignore` & `jupyterlab_new_launcher-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.3/LICENSE` & `jupyterlab_new_launcher-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.3/README.md` & `jupyterlab_new_launcher-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.3/pyproject.toml` & `jupyterlab_new_launcher-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
+    "jupyter_server>=2.0.1,<3",
 ]
 dynamic = ["version", "description", "authors", "urls", "keywords"]
 
 [tool.hatch.version]
 source = "nodejs"
 
 [tool.hatch.metadata.hooks.nodejs]
@@ -35,14 +36,15 @@
 [tool.hatch.build.targets.sdist]
 artifacts = ["jupyterlab_new_launcher/labextension"]
 exclude = [".github", "binder"]
 
 [tool.hatch.build.targets.wheel.shared-data]
 "jupyterlab_new_launcher/labextension" = "share/jupyter/labextensions/jupyterlab-new-launcher"
 "install.json" = "share/jupyter/labextensions/jupyterlab-new-launcher/install.json"
+"jupyter-config/server-config" = "etc/jupyter/jupyter_server_config.d"
 
 [tool.hatch.build.hooks.version]
 path = "jupyterlab_new_launcher/_version.py"
 
 [tool.hatch.build.hooks.jupyter-builder]
 dependencies = ["hatch-jupyter-builder>=0.5"]
 build-function = "hatch_jupyter_builder.npm_builder"
```

### Comparing `jupyterlab_new_launcher-0.3.3/PKG-INFO` & `jupyterlab_new_launcher-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlab-new-launcher
-Version: 0.3.3
+Version: 0.4.0
 Dynamic: Keywords
 Summary: A redesigned JupyterLab launcher
 Project-URL: Homepage, https://github.com/nebari-dev/jupyterlab-new-launcher
 Project-URL: Bug Tracker, https://github.com/nebari-dev/jupyterlab-new-launcher/issues
 Project-URL: Repository, https://github.com/nebari-dev/jupyterlab-new-launcher.git
 Author-email: Nebari development team <internal-it@quansight.com>
 License: BSD 3-Clause License
@@ -47,14 +47,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
+Requires-Dist: jupyter-server<3,>=2.0.1
 Description-Content-Type: text/markdown
 
 # jupyterlab-new-launcher
 
 [![Github Actions Status](https://github.com/nebari-dev/jupyterlab-new-launcher/workflows/Build/badge.svg)](https://github.com/nebari-dev/jupyterlab-new-launcher/actions/workflows/build.yml)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/nebari-dev/jupyterlab-new-launcher/main?urlpath=lab)
```

